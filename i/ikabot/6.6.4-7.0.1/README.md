# Comparing `tmp/ikabot-6.6.4.tar.gz` & `tmp/ikabot-7.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ikabot-6.6.4.tar", last modified: Wed Sep 20 19:51:26 2023, max compression
+gzip compressed data, was "ikabot-7.0.1.tar", last modified: Thu Apr 25 18:20:54 2024, max compression
```

## Comparing `ikabot-6.6.4.tar` & `ikabot-7.0.1.tar`

### file list

```diff
@@ -1,103 +1,108 @@
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-09-20 19:51:26.748486 ikabot-6.6.4/
--rw-r--r--   0 user      (1000) user      (1000)     1064 2023-09-20 19:50:59.000000 ikabot-6.6.4/LICENSE
--rw-r--r--   0 user      (1000) user      (1000)       56 2023-09-20 19:50:59.000000 ikabot-6.6.4/MANIFEST.in
--rw-r--r--   0 user      (1000) user      (1000)      318 2023-09-20 19:51:26.748486 ikabot-6.6.4/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)    11583 2023-09-20 19:50:59.000000 ikabot-6.6.4/README.md
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-09-20 19:51:26.738486 ikabot-6.6.4/ikabot/
--rw-r--r--   0 user      (1000) user      (1000)        0 2023-09-20 19:50:59.000000 ikabot-6.6.4/ikabot/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)       44 2023-09-20 19:50:59.000000 ikabot-6.6.4/ikabot/__main__.py
--rwxr-xr-x   0 user      (1000) user      (1000)     9540 2023-09-20 19:50:59.000000 ikabot-6.6.4/ikabot/command_line.py
--rw-r--r--   0 user      (1000) user      (1000)     2227 2023-09-20 19:50:59.000000 ikabot-6.6.4/ikabot/config.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-09-20 19:51:26.741820 ikabot-6.6.4/ikabot/function/
--rw-r--r--   0 user      (1000) user      (1000)        0 2023-09-20 19:50:59.000000 ikabot-6.6.4/ikabot/function/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)    11102 2023-09-20 19:50:59.000000 ikabot-6.6.4/ikabot/function/activateMiracle.py
--rw-r--r--   0 user      (1000) user      (1000)     5770 2023-09-20 19:50:59.000000 ikabot-6.6.4/ikabot/function/alertAttacks.py
--rw-r--r--   0 user      (1000) user      (1000)     3959 2023-09-20 19:50:59.000000 ikabot-6.6.4/ikabot/function/alertLowWine.py
--rw-r--r--   0 user      (1000) user      (1000)    20485 2023-09-20 19:50:59.000000 ikabot-6.6.4/ikabot/function/attackBarbarians.py
--rw-r--r--   0 user      (1000) user      (1000)    14270 2023-09-20 19:50:59.000000 ikabot-6.6.4/ikabot/function/autoPirate.py
--rw-r--r--   0 user      (1000) user      (1000)    11264 2023-09-20 19:50:59.000000 ikabot-6.6.4/ikabot/function/buyResources.py
--rw-r--r--   0 user      (1000) user      (1000)      674 2023-09-20 19:50:59.000000 ikabot-6.6.4/ikabot/function/checkForUpdate.py
--rw-r--r--   0 user      (1000) user      (1000)     4148 2023-09-20 19:50:59.000000 ikabot-6.6.4/ikabot/function/constructBuilding.py
--rw-r--r--   0 user      (1000) user      (1000)    20942 2023-09-20 19:50:59.000000 ikabot-6.6.4/ikabot/function/constructionList.py
--rw-r--r--   0 user      (1000) user      (1000)    51779 2023-09-20 19:50:59.000000 ikabot-6.6.4/ikabot/function/decaptchaConf.py
--rw-r--r--   0 user      (1000) user      (1000)    11987 2023-09-20 19:50:59.000000 ikabot-6.6.4/ikabot/function/distributeResources.py
--rw-r--r--   0 user      (1000) user      (1000)     5996 2023-09-20 19:50:59.000000 ikabot-6.6.4/ikabot/function/donate.py
--rw-r--r--   0 user      (1000) user      (1000)     8542 2023-09-20 19:50:59.000000 ikabot-6.6.4/ikabot/function/donationBot.py
--rw-r--r--   0 user      (1000) user      (1000)    19399 2023-09-20 19:50:59.000000 ikabot-6.6.4/ikabot/function/dumpWorld.py
--rw-r--r--   0 user      (1000) user      (1000)     6671 2023-09-20 19:50:59.000000 ikabot-6.6.4/ikabot/function/getStatus.py
--rw-r--r--   0 user      (1000) user      (1000)     3285 2023-09-20 19:50:59.000000 ikabot-6.6.4/ikabot/function/importExportCookie.py
--rw-r--r--   0 user      (1000) user      (1000)     6332 2023-09-20 19:50:59.000000 ikabot-6.6.4/ikabot/function/investigate.py
--rw-r--r--   0 user      (1000) user      (1000)     2004 2023-09-20 19:50:59.000000 ikabot-6.6.4/ikabot/function/killTasks.py
--rw-r--r--   0 user      (1000) user      (1000)     2342 2023-09-20 19:50:59.000000 ikabot-6.6.4/ikabot/function/loginDaily.py
--rw-r--r--   0 user      (1000) user      (1000)     6147 2023-09-20 19:50:59.000000 ikabot-6.6.4/ikabot/function/logs.py
--rw-r--r--   0 user      (1000) user      (1000)     3954 2023-09-20 19:50:59.000000 ikabot-6.6.4/ikabot/function/proxyConf.py
--rw-r--r--   0 user      (1000) user      (1000)     6887 2023-09-20 19:50:59.000000 ikabot-6.6.4/ikabot/function/searchForIslandSpaces.py
--rw-r--r--   0 user      (1000) user      (1000)    13788 2023-09-20 19:50:59.000000 ikabot-6.6.4/ikabot/function/sellResources.py
--rw-r--r--   0 user      (1000) user      (1000)     4717 2023-09-20 19:50:59.000000 ikabot-6.6.4/ikabot/function/sendResources.py
--rw-r--r--   0 user      (1000) user      (1000)     4325 2023-09-20 19:50:59.000000 ikabot-6.6.4/ikabot/function/shipMovements.py
--rw-r--r--   0 user      (1000) user      (1000)     7687 2023-09-20 19:50:59.000000 ikabot-6.6.4/ikabot/function/stationArmy.py
--rw-r--r--   0 user      (1000) user      (1000)    11734 2023-09-20 19:50:59.000000 ikabot-6.6.4/ikabot/function/trainArmy.py
--rw-r--r--   0 user      (1000) user      (1000)      886 2023-09-20 19:50:59.000000 ikabot-6.6.4/ikabot/function/update.py
--rw-r--r--   0 user      (1000) user      (1000)     1538 2023-09-20 19:50:59.000000 ikabot-6.6.4/ikabot/function/vacationMode.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-09-20 19:51:26.745153 ikabot-6.6.4/ikabot/helpers/
--rw-r--r--   0 user      (1000) user      (1000)        0 2023-09-20 19:50:59.000000 ikabot-6.6.4/ikabot/helpers/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)     5522 2023-09-20 19:50:59.000000 ikabot-6.6.4/ikabot/helpers/aesCipher.py
--rw-r--r--   0 user      (1000) user      (1000)    10349 2023-09-20 19:50:59.000000 ikabot-6.6.4/ikabot/helpers/botComm.py
--rw-r--r--   0 user      (1000) user      (1000)     5028 2023-09-20 19:50:59.000000 ikabot-6.6.4/ikabot/helpers/getJson.py
--rw-r--r--   0 user      (1000) user      (1000)     1972 2023-09-20 19:50:59.000000 ikabot-6.6.4/ikabot/helpers/gui.py
--rw-r--r--   0 user      (1000) user      (1000)     2493 2023-09-20 19:50:59.000000 ikabot-6.6.4/ikabot/helpers/market.py
--rw-r--r--   0 user      (1000) user      (1000)      868 2023-09-20 19:50:59.000000 ikabot-6.6.4/ikabot/helpers/naval.py
--rw-r--r--   0 user      (1000) user      (1000)     9333 2023-09-20 19:50:59.000000 ikabot-6.6.4/ikabot/helpers/pedirInfo.py
--rw-r--r--   0 user      (1000) user      (1000)     7483 2023-09-20 19:50:59.000000 ikabot-6.6.4/ikabot/helpers/planRoutes.py
--rw-r--r--   0 user      (1000) user      (1000)     2707 2023-09-20 19:50:59.000000 ikabot-6.6.4/ikabot/helpers/process.py
--rw-r--r--   0 user      (1000) user      (1000)     1940 2023-09-20 19:50:59.000000 ikabot-6.6.4/ikabot/helpers/resources.py
--rw-r--r--   0 user      (1000) user      (1000)     1150 2023-09-20 19:50:59.000000 ikabot-6.6.4/ikabot/helpers/signals.py
--rw-r--r--   0 user      (1000) user      (1000)     3417 2023-09-20 19:50:59.000000 ikabot-6.6.4/ikabot/helpers/varios.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-09-20 19:51:26.738486 ikabot-6.6.4/ikabot/locale/
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-09-20 19:51:26.738486 ikabot-6.6.4/ikabot/locale/es/
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-09-20 19:51:26.745153 ikabot-6.6.4/ikabot/locale/es/LC_MESSAGES/
--rw-r--r--   0 user      (1000) user      (1000)     2828 2023-09-20 19:50:59.000000 ikabot-6.6.4/ikabot/locale/es/LC_MESSAGES/activateMiracle.po
--rw-r--r--   0 user      (1000) user      (1000)      719 2023-09-20 19:50:59.000000 ikabot-6.6.4/ikabot/locale/es/LC_MESSAGES/aesCipher.po
--rw-r--r--   0 user      (1000) user      (1000)     1995 2023-09-20 19:50:59.000000 ikabot-6.6.4/ikabot/locale/es/LC_MESSAGES/alertAttacks.po
--rw-r--r--   0 user      (1000) user      (1000)     1481 2023-09-20 19:50:59.000000 ikabot-6.6.4/ikabot/locale/es/LC_MESSAGES/alertLowWine.po
--rw-r--r--   0 user      (1000) user      (1000)     2219 2023-09-20 19:50:59.000000 ikabot-6.6.4/ikabot/locale/es/LC_MESSAGES/botComm.po
--rw-r--r--   0 user      (1000) user      (1000)     2417 2023-09-20 19:50:59.000000 ikabot-6.6.4/ikabot/locale/es/LC_MESSAGES/buyResources.po
--rw-r--r--   0 user      (1000) user      (1000)      575 2023-09-20 19:50:59.000000 ikabot-6.6.4/ikabot/locale/es/LC_MESSAGES/checkForUpdate.po
--rw-r--r--   0 user      (1000) user      (1000)     2432 2023-09-20 19:50:59.000000 ikabot-6.6.4/ikabot/locale/es/LC_MESSAGES/command_line.po
--rw-r--r--   0 user      (1000) user      (1000)      755 2023-09-20 19:50:59.000000 ikabot-6.6.4/ikabot/locale/es/LC_MESSAGES/config.po
--rw-r--r--   0 user      (1000) user      (1000)     1001 2023-09-20 19:50:59.000000 ikabot-6.6.4/ikabot/locale/es/LC_MESSAGES/constructBuilding.po
--rw-r--r--   0 user      (1000) user      (1000)     4367 2023-09-20 19:50:59.000000 ikabot-6.6.4/ikabot/locale/es/LC_MESSAGES/constructionList.po
--rw-r--r--   0 user      (1000) user      (1000)     1547 2023-09-20 19:50:59.000000 ikabot-6.6.4/ikabot/locale/es/LC_MESSAGES/distributeResources.po
--rw-r--r--   0 user      (1000) user      (1000)     1416 2023-09-20 19:50:59.000000 ikabot-6.6.4/ikabot/locale/es/LC_MESSAGES/donate.po
--rw-r--r--   0 user      (1000) user      (1000)     1628 2023-09-20 19:50:59.000000 ikabot-6.6.4/ikabot/locale/es/LC_MESSAGES/donationBot.po
--rw-r--r--   0 user      (1000) user      (1000)     1673 2023-09-20 19:50:59.000000 ikabot-6.6.4/ikabot/locale/es/LC_MESSAGES/getStatus.po
--rw-r--r--   0 user      (1000) user      (1000)      376 2023-09-20 19:50:59.000000 ikabot-6.6.4/ikabot/locale/es/LC_MESSAGES/gui.mo
--rw-r--r--   0 user      (1000) user      (1000)      553 2023-09-20 19:50:59.000000 ikabot-6.6.4/ikabot/locale/es/LC_MESSAGES/gui.po
--rw-r--r--   0 user      (1000) user      (1000)      841 2023-09-20 19:50:59.000000 ikabot-6.6.4/ikabot/locale/es/LC_MESSAGES/loginDaily.po
--rw-r--r--   0 user      (1000) user      (1000)      837 2023-09-20 19:50:59.000000 ikabot-6.6.4/ikabot/locale/es/LC_MESSAGES/pedirInfo.mo
--rw-r--r--   0 user      (1000) user      (1000)     1255 2023-09-20 19:50:59.000000 ikabot-6.6.4/ikabot/locale/es/LC_MESSAGES/pedirInfo.po
--rw-r--r--   0 user      (1000) user      (1000)     1235 2023-09-20 19:50:59.000000 ikabot-6.6.4/ikabot/locale/es/LC_MESSAGES/searchForIslandSpaces.po
--rw-r--r--   0 user      (1000) user      (1000)     2792 2023-09-20 19:50:59.000000 ikabot-6.6.4/ikabot/locale/es/LC_MESSAGES/sellResources.po
--rw-r--r--   0 user      (1000) user      (1000)     3510 2023-09-20 19:50:59.000000 ikabot-6.6.4/ikabot/locale/es/LC_MESSAGES/sendResources.po
--rw-r--r--   0 user      (1000) user      (1000)     1253 2023-09-20 19:50:59.000000 ikabot-6.6.4/ikabot/locale/es/LC_MESSAGES/session.mo
--rw-r--r--   0 user      (1000) user      (1000)     1828 2023-09-20 19:50:59.000000 ikabot-6.6.4/ikabot/locale/es/LC_MESSAGES/session.po
--rw-r--r--   0 user      (1000) user      (1000)     1350 2023-09-20 19:50:59.000000 ikabot-6.6.4/ikabot/locale/es/LC_MESSAGES/shipMovements.po
--rw-r--r--   0 user      (1000) user      (1000)      497 2023-09-20 19:50:59.000000 ikabot-6.6.4/ikabot/locale/es/LC_MESSAGES/signals.mo
--rw-r--r--   0 user      (1000) user      (1000)      715 2023-09-20 19:50:59.000000 ikabot-6.6.4/ikabot/locale/es/LC_MESSAGES/signals.po
--rw-r--r--   0 user      (1000) user      (1000)     2464 2023-09-20 19:50:59.000000 ikabot-6.6.4/ikabot/locale/es/LC_MESSAGES/trainArmy.pot
--rw-r--r--   0 user      (1000) user      (1000)     3175 2023-09-20 19:50:59.000000 ikabot-6.6.4/ikabot/locale/es/LC_MESSAGES/trainFleets.po
--rw-r--r--   0 user      (1000) user      (1000)     3169 2023-09-20 19:50:59.000000 ikabot-6.6.4/ikabot/locale/es/LC_MESSAGES/trainTroops.po
--rw-r--r--   0 user      (1000) user      (1000)      579 2023-09-20 19:50:59.000000 ikabot-6.6.4/ikabot/locale/es/LC_MESSAGES/update.po
--rw-r--r--   0 user      (1000) user      (1000)      717 2023-09-20 19:50:59.000000 ikabot-6.6.4/ikabot/locale/es/LC_MESSAGES/vacationMode.po
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-09-20 19:51:26.748486 ikabot-6.6.4/ikabot/web/
--rw-r--r--   0 user      (1000) user      (1000)        0 2023-09-20 19:50:59.000000 ikabot-6.6.4/ikabot/web/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)    51809 2023-09-20 19:50:59.000000 ikabot-6.6.4/ikabot/web/session.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-09-20 19:51:26.741820 ikabot-6.6.4/ikabot.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)      318 2023-09-20 19:51:26.000000 ikabot-6.6.4/ikabot.egg-info/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)     3079 2023-09-20 19:51:26.000000 ikabot-6.6.4/ikabot.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1000) user      (1000)        1 2023-09-20 19:51:26.000000 ikabot-6.6.4/ikabot.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1000) user      (1000)       52 2023-09-20 19:51:26.000000 ikabot-6.6.4/ikabot.egg-info/entry_points.txt
--rw-r--r--   0 user      (1000) user      (1000)       45 2023-09-20 19:51:26.000000 ikabot-6.6.4/ikabot.egg-info/requires.txt
--rw-r--r--   0 user      (1000) user      (1000)        7 2023-09-20 19:51:26.000000 ikabot-6.6.4/ikabot.egg-info/top_level.txt
--rw-r--r--   0 user      (1000) user      (1000)       38 2023-09-20 19:51:26.748486 ikabot-6.6.4/setup.cfg
--rw-r--r--   0 user      (1000) user      (1000)      655 2023-09-20 19:50:59.000000 ikabot-6.6.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:20:54.899791 ikabot-7.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-25 18:20:51.000000 ikabot-7.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-25 18:20:51.000000 ikabot-7.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-04-25 18:20:54.899791 ikabot-7.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-04-25 18:20:51.000000 ikabot-7.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:20:54.883791 ikabot-7.0.1/ikabot/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/__main__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10483 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/command_line.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5123 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:20:54.891791 ikabot-7.0.1/ikabot/function/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/function/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12042 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/function/activateMiracle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5943 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/function/alertAttacks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4151 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/function/alertLowWine.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22648 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/function/attackBarbarians.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15191 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/function/autoPirate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11721 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/function/buyResources.py
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/function/checkForUpdate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4855 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/function/constructBuilding.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22475 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/function/constructionList.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52825 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/function/decaptchaConf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14348 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/function/distributeResources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6899 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/function/donate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10203 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/function/donationBot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24043 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/function/dumpWorld.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7969 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/function/getStatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3485 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/function/importExportCookie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6725 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/function/investigate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/function/killTasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/function/loadCustomModule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20484 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/function/loginDaily.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7345 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/function/logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4305 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/function/proxyConf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8748 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/function/searchForIslandSpaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15397 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/function/sellResources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5161 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/function/sendResources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4866 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/function/shipMovements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9303 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/function/stationArmy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/function/testTelegramBot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17449 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/function/trainArmy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/function/update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/function/vacationMode.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64399 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/function/webServer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:20:54.891791 ikabot-7.0.1/ikabot/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5777 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/helpers/aesCipher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3055 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/helpers/apiComm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10619 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/helpers/botComm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8908 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/helpers/dns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9125 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/helpers/getJson.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/helpers/gui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/helpers/market.py
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/helpers/naval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9342 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/helpers/pedirInfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7886 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/helpers/planRoutes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/helpers/process.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/helpers/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/helpers/signals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4568 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/helpers/varios.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:20:54.883791 ikabot-7.0.1/ikabot/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:20:54.883791 ikabot-7.0.1/ikabot/locale/es/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:20:54.899791 ikabot-7.0.1/ikabot/locale/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     2828 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/locale/es/LC_MESSAGES/activateMiracle.po
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/locale/es/LC_MESSAGES/aesCipher.po
+-rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/locale/es/LC_MESSAGES/alertAttacks.po
+-rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/locale/es/LC_MESSAGES/alertLowWine.po
+-rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/locale/es/LC_MESSAGES/botComm.po
+-rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/locale/es/LC_MESSAGES/buyResources.po
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/locale/es/LC_MESSAGES/checkForUpdate.po
+-rw-r--r--   0 runner    (1001) docker     (127)     2432 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/locale/es/LC_MESSAGES/command_line.po
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/locale/es/LC_MESSAGES/config.po
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/locale/es/LC_MESSAGES/constructBuilding.po
+-rw-r--r--   0 runner    (1001) docker     (127)     4367 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/locale/es/LC_MESSAGES/constructionList.po
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/locale/es/LC_MESSAGES/distributeResources.po
+-rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/locale/es/LC_MESSAGES/donate.po
+-rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/locale/es/LC_MESSAGES/donationBot.po
+-rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/locale/es/LC_MESSAGES/getStatus.po
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/locale/es/LC_MESSAGES/gui.mo
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/locale/es/LC_MESSAGES/gui.po
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/locale/es/LC_MESSAGES/loginDaily.po
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/locale/es/LC_MESSAGES/pedirInfo.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/locale/es/LC_MESSAGES/pedirInfo.po
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/locale/es/LC_MESSAGES/searchForIslandSpaces.po
+-rw-r--r--   0 runner    (1001) docker     (127)     2792 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/locale/es/LC_MESSAGES/sellResources.po
+-rw-r--r--   0 runner    (1001) docker     (127)     3510 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/locale/es/LC_MESSAGES/sendResources.po
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/locale/es/LC_MESSAGES/session.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/locale/es/LC_MESSAGES/session.po
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/locale/es/LC_MESSAGES/shipMovements.po
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/locale/es/LC_MESSAGES/signals.mo
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/locale/es/LC_MESSAGES/signals.po
+-rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/locale/es/LC_MESSAGES/trainArmy.pot
+-rw-r--r--   0 runner    (1001) docker     (127)     3175 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/locale/es/LC_MESSAGES/trainFleets.po
+-rw-r--r--   0 runner    (1001) docker     (127)     3169 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/locale/es/LC_MESSAGES/trainTroops.po
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/locale/es/LC_MESSAGES/update.po
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/locale/es/LC_MESSAGES/vacationMode.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:20:54.899791 ikabot-7.0.1/ikabot/web/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59884 2024-04-25 18:20:51.000000 ikabot-7.0.1/ikabot/web/session.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:20:54.899791 ikabot-7.0.1/ikabot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-04-25 18:20:54.000000 ikabot-7.0.1/ikabot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-04-25 18:20:54.000000 ikabot-7.0.1/ikabot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 18:20:54.000000 ikabot-7.0.1/ikabot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-25 18:20:54.000000 ikabot-7.0.1/ikabot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-25 18:20:54.000000 ikabot-7.0.1/ikabot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-25 18:20:54.000000 ikabot-7.0.1/ikabot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 18:20:54.899791 ikabot-7.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-25 18:20:51.000000 ikabot-7.0.1/setup.py
```

### Comparing `ikabot-6.6.4/LICENSE` & `ikabot-7.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ikabot-6.6.4/ikabot/command_line.py` & `ikabot-7.0.1/ikabot/command_line.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,54 +1,57 @@
 #! /usr/bin/env python3
 # -*- coding: utf-8 -*-
 
-import os
-import sys
+import datetime
 import gettext
 import multiprocessing
+import os
+import sys
 import time
-import datetime
+
 from ikabot.config import *
-from ikabot.web.session import *
-from ikabot.helpers.gui import *
-from ikabot.function.donate import donate
-from ikabot.function.update import update
-from ikabot.helpers.pedirInfo import read
-from ikabot.function.getStatus import getStatus
-from ikabot.function.donationBot import donationBot
-from ikabot.helpers.botComm import updateTelegramData, telegramDataIsValid
-from ikabot.helpers.process import updateProcessList
-from ikabot.function.constructionList import constructionList
-from ikabot.function.searchForIslandSpaces import searchForIslandSpaces
-from ikabot.function.alertAttacks import alertAttacks
-from ikabot.function.vacationMode import vacationMode
 from ikabot.function.activateMiracle import activateMiracle
-from ikabot.function.trainArmy import trainArmy
-from ikabot.function.sellResources import sellResources
-from ikabot.function.checkForUpdate import checkForUpdate
-from ikabot.function.distributeResources import distributeResources
+from ikabot.function.alertAttacks import alertAttacks
 from ikabot.function.alertLowWine import alertLowWine
+from ikabot.function.attackBarbarians import attackBarbarians
+from ikabot.function.autoPirate import autoPirate
 from ikabot.function.buyResources import buyResources
-from ikabot.function.loginDaily import loginDaily
-from ikabot.function.sendResources import sendResources
+from ikabot.function.checkForUpdate import checkForUpdate
 from ikabot.function.constructBuilding import constructBuilding
-from ikabot.function.shipMovements import shipMovements
+from ikabot.function.constructionList import constructionList
+from ikabot.function.decaptchaConf import decaptchaConf
+from ikabot.function.distributeResources import distributeResources
+from ikabot.function.donate import donate
+from ikabot.function.donationBot import donationBot
+from ikabot.function.dumpWorld import dumpWorld
+from ikabot.function.getStatus import getStatus
 from ikabot.function.importExportCookie import importExportCookie
-from ikabot.function.autoPirate import autoPirate
 from ikabot.function.investigate import investigate
-from ikabot.function.attackBarbarians import attackBarbarians
-from ikabot.function.proxyConf import proxyConf, show_proxy
 from ikabot.function.killTasks import killTasks
-from ikabot.function.decaptchaConf import decaptchaConf
-from ikabot.function.dumpWorld import dumpWorld
-from ikabot.function.stationArmy import stationArmy
+from ikabot.function.loginDaily import loginDaily
 from ikabot.function.logs import logs
+from ikabot.function.proxyConf import proxyConf, show_proxy
+from ikabot.function.searchForIslandSpaces import searchForIslandSpaces
+from ikabot.function.sellResources import sellResources
+from ikabot.function.sendResources import sendResources
+from ikabot.function.shipMovements import shipMovements
+from ikabot.function.stationArmy import stationArmy
+from ikabot.function.testTelegramBot import testTelegramBot
+from ikabot.function.trainArmy import trainArmy
+from ikabot.function.update import update
+from ikabot.function.vacationMode import vacationMode
+from ikabot.function.webServer import webServer
+from ikabot.function.loadCustomModule import loadCustomModule
+from ikabot.helpers.botComm import telegramDataIsValid, updateTelegramData
+from ikabot.helpers.gui import *
+from ikabot.helpers.pedirInfo import read
+from ikabot.helpers.process import updateProcessList
+from ikabot.web.session import *
 
-
-t = gettext.translation('command_line', localedir, languages=languages, fallback=True)
+t = gettext.translation("command_line", localedir, languages=languages, fallback=True)
 _ = t.gettext
 
 
 def menu(session, checkUpdate=True):
     """
     Parameters
     ----------
@@ -62,178 +65,234 @@
 
     banner()
 
     process_list = updateProcessList(session)
     if len(process_list) > 0:
         # Insert table header
         table = process_list.copy()
-        table.insert(0,{'pid':'pid', 'action':'task','date':'date','status':'status'})
+        table.insert(
+            0, {"pid": "pid", "action": "task", "date": "date", "status": "status"}
+        )
         # Get max length of strings in each category (date is always going to be 15)
-        maxPid, maxAction, maxStatus = [max(i) for i in [[len(str(r['pid'])) for r in table], [len(str(r['action'])) for r in table], [len(str(r['status'])) for r in table]]]
+        maxPid, maxAction, maxStatus = [
+            max(i)
+            for i in [
+                [len(str(r["pid"])) for r in table],
+                [len(str(r["action"])) for r in table],
+                [len(str(r["status"])) for r in table],
+            ]
+        ]
         # Print header
-        print('|{:^{maxPid}}|{:^{maxAction}}|{:^15}|{:^{maxStatus}}|'.format(table[0]['pid'], table[0]['action'], table[0]['date'], table[0]['status'], maxPid=maxPid, maxAction=maxAction, maxStatus=maxStatus))
+        print(
+            "|{:^{maxPid}}|{:^{maxAction}}|{:^15}|{:^{maxStatus}}|".format(
+                table[0]["pid"],
+                table[0]["action"],
+                table[0]["date"],
+                table[0]["status"],
+                maxPid=maxPid,
+                maxAction=maxAction,
+                maxStatus=maxStatus,
+            )
+        )
         # Print process list
-        [print('|{:^{maxPid}}|{:^{maxAction}}|{:^15}|{:^{maxStatus}}|'.format(r['pid'], r['action'], datetime.datetime.fromtimestamp(r['date']).strftime('%b %d %H:%M:%S'), r['status'], maxPid=maxPid, maxAction=maxAction, maxStatus=maxStatus)) for r in process_list]
-        print('')
+        [
+            print(
+                "|{:^{maxPid}}|{:^{maxAction}}|{:^15}|{:^{maxStatus}}|".format(
+                    r["pid"],
+                    r["action"],
+                    datetime.datetime.fromtimestamp(r["date"]).strftime(
+                        "%b %d %H:%M:%S"
+                    ),
+                    r["status"],
+                    maxPid=maxPid,
+                    maxAction=maxAction,
+                    maxStatus=maxStatus,
+                )
+            )
+            for r in process_list
+        ]
+        print("")
 
     menu_actions = {
-        1:            constructionList,
-        2:            sendResources,
-        3:            distributeResources,
-        4:            getStatus,
-        5:            searchForIslandSpaces,
-        6:            loginDaily,
-        101:            alertAttacks,
-        102:            alertLowWine,
-        111:            buyResources,
-        112:            sellResources,
-        121:            donate,
-        122:            donationBot,
-        10:            vacationMode,
-        11:            activateMiracle,
-        131:            trainArmy,
-        132:            stationArmy,
-        13:            shipMovements,
-        14:            constructBuilding,
-        15:            update,
-        16:            importExportCookie,
-        17:            autoPirate,
-        18:            investigate,
-        19:            attackBarbarians,
-        20:            dumpWorld,
-        141:            proxyConf,
-        142:            updateTelegramData,
-        143:            killTasks,
-        144:            decaptchaConf,
-        145:            logs,
-                    }
-
-    print(_('(0)  Exit'))
-    print(_('(1)  Construction list'))
-    print(_('(2)  Send resources'))
-    print(_('(3)  Distribute resources'))
-    print(_('(4)  Account status'))
-    print(_('(5)  Monitor islands'))
-    print(_('(6)  Login daily'))
-    print(_('(7)  Alerts / Notifications'))
-    print(_('(8)  Marketplace'))
-    print(_('(9)  Donate'))
-    print(_('(10) Activate vacation mode'))
-    print(_('(11) Activate miracle'))
-    print(_('(12) Military actions'))
-    print(_('(13) See movements'))
-    print(_('(14) Construct building'))
-    print(_('(15) Update Ikabot'))
-    print(_('(16) Import / Export cookie'))
-    print(_('(17) Auto-Pirate'))
-    print(_('(18) Investigate'))
-    print(_('(19) Attack barbarians'))
-    print(_('(20) Dump / View world'))
-    print(_('(21) Options / Settings'))
+        1: constructionList,
+        2: sendResources,
+        3: distributeResources,
+        4: getStatus,
+        5: searchForIslandSpaces,
+        6: loginDaily,
+        101: alertAttacks,
+        102: alertLowWine,
+        111: buyResources,
+        112: sellResources,
+        121: donate,
+        122: donationBot,
+        10: vacationMode,
+        11: activateMiracle,
+        131: trainArmy,
+        132: stationArmy,
+        13: shipMovements,
+        14: constructBuilding,
+        15: update,
+        16: webServer,
+        17: autoPirate,
+        18: investigate,
+        19: attackBarbarians,
+        20: dumpWorld,
+        141: proxyConf,
+        142: updateTelegramData,
+        143: killTasks,
+        144: decaptchaConf,
+        145: logs,
+        146: testTelegramBot,
+        147: importExportCookie,
+        148: loadCustomModule
+    }
+
+    print(_("(0)  Exit"))
+    print(_("(1)  Construction list"))
+    print(_("(2)  Send resources"))
+    print(_("(3)  Distribute resources"))
+    print(_("(4)  Account status"))
+    print(_("(5)  Monitor islands"))
+    print(_("(6)  Login daily"))
+    print(_("(7)  Alerts / Notifications"))
+    print(_("(8)  Marketplace"))
+    print(_("(9)  Donate"))
+    print(_("(10) Activate vacation mode"))
+    print(_("(11) Activate miracle"))
+    print(_("(12) Military actions"))
+    print(_("(13) See movements"))
+    print(_("(14) Construct building"))
+    print(_("(15) Update Ikabot"))
+    print(_("(16) Ikabot Web Server"))
+    print(_("(17) Auto-Pirate"))
+    print(_("(18) Investigate"))
+    print(_("(19) Attack barbarians"))
+    print(_("(20) Dump / View world"))
+    print(_("(21) Options / Settings"))
     total_options = len(menu_actions) + 1
-    selected = read(min=0, max=total_options, digit=True)
+    selected = read(min=0, max=total_options, digit=True, empty=True)
     
+    # refresh main menu on hitting enter
+    if selected == '':
+        return menu(session)
+
     if selected == 7:
         banner()
-        print(_('(0) Back'))
-        print(_('(1) Alert attacks'))
-        print(_('(2) Alert wine running out'))
+        print(_("(0) Back"))
+        print(_("(1) Alert attacks"))
+        print(_("(2) Alert wine running out"))
 
         selected = read(min=0, max=2, digit=True)
         if selected == 0:
             menu(session)
             return
         if selected > 0:
             selected += 100
-            
+
     if selected == 8:
         banner()
-        print(_('(0) Back'))
-        print(_('(1) Buy resources'))
-        print(_('(2) Sell resources'))
+        print(_("(0) Back"))
+        print(_("(1) Buy resources"))
+        print(_("(2) Sell resources"))
 
         selected = read(min=0, max=2, digit=True)
         if selected == 0:
             menu(session)
             return
         if selected > 0:
             selected += 110
-            
+
     if selected == 9:
         banner()
-        print(_('(0) Back'))
-        print(_('(1) Donate once'))
-        print(_('(2) Donate automatically'))
+        print(_("(0) Back"))
+        print(_("(1) Donate once"))
+        print(_("(2) Donate automatically"))
 
         selected = read(min=0, max=2, digit=True)
         if selected == 0:
             menu(session)
             return
         if selected > 0:
             selected += 120
-            
+
     if selected == 12:
         banner()
-        print(_('(0) Back'))
-        print(_('(1) Train Army'))
-        print(_('(2) Send Troops/Ships'))
+        print(_("(0) Back"))
+        print(_("(1) Train Army"))
+        print(_("(2) Send Troops/Ships"))
         selected = read(min=0, max=2, digit=True)
         if selected == 0:
             menu(session)
             return
         if selected > 0:
             selected += 130
 
     if selected == 21:
         banner()
-        print(_('(0) Back'))
-        print(_('(1) Configure Proxy'))
+        print(_("(0) Back"))
+        print(_("(1) Configure Proxy"))
         if telegramDataIsValid(session):
-            print(_('(2) Change the Telegram data'))
+            print(_("(2) Change the Telegram data"))
         else:
-            print(_('(2) Enter the Telegram data'))
-        print(_('(3) Kill tasks'))
-        print(_('(4) Configure captcha resolver'))
-        print(_('(5) Logs'))
+            print(_("(2) Enter the Telegram data"))
+        print(_("(3) Kill tasks"))
+        print(_("(4) Configure captcha resolver"))
+        print(_("(5) Logs"))
+        print(_("(6) Message Telegram Bot"))
+        print(_("(7) Import / Export cookie"))
+        print(_("(8) Load custom ikabot module"))
 
-        selected = read(min=0, max=5, digit=True)
+        selected = read(min=0, max=8, digit=True)
         if selected == 0:
             menu(session)
             return
         if selected > 0:
             selected += 140
-        
-
 
     if selected != 0:
         try:
             event = multiprocessing.Event()  # creates a new event
-            process = multiprocessing.Process(target=menu_actions[selected], args=(session, event, sys.stdin.fileno(), config.predetermined_input), name=menu_actions[selected].__name__)
+            config.has_params = len(config.predetermined_input) > 0
+            process = multiprocessing.Process(
+                target=menu_actions[selected],
+                args=(session, event, sys.stdin.fileno(), config.predetermined_input),
+                name=menu_actions[selected].__name__,
+            )
             process.start()
-            process_list.append({'pid': process.pid, 'action': menu_actions[selected].__name__, 'date': time.time(), 'status': 'started'})
+            process_list.append(
+                {
+                    "pid": process.pid,
+                    "action": menu_actions[selected].__name__,
+                    "date": time.time(),
+                    "status": "started",
+                }
+            )
             updateProcessList(session, programprocesslist=process_list)
             event.wait()  # waits for the process to fire the event that's been given to it. When it does  this process gets back control of the command line and asks user for more input
         except KeyboardInterrupt:
             pass
         menu(session, checkUpdate=False)
     else:
         if isWindows:
             # in unix, you can exit ikabot and close the terminal and the processes will continue to execute
             # in windows, you can exit ikabot but if you close the terminal, the processes will die
-            print(_('Closing this console will kill the processes.'))
+            print(_("Closing this console will kill the processes."))
             enter()
         clear()
-        os._exit(0)  # kills the process which executes this statement, but it does not kill it's child processes
+        os._exit(
+            0
+        )  # kills the process which executes this statement, but it does not kill it's child processes
 
 
 def init():
-    home = 'USERPROFILE' if isWindows else 'HOME'
+    home = "USERPROFILE" if isWindows else "HOME"
     os.chdir(os.getenv(home))
     if not os.path.isfile(ikaFile):
-        open(ikaFile, 'w')
+        open(ikaFile, "w")
         os.chmod(ikaFile, 0o600)
 
 
 def start():
     init()
     config.has_params = len(sys.argv) > 1
     for arg in sys.argv:
@@ -257,12 +316,12 @@
     config.predetermined_input = predetermined_input
     try:
         start()
     except KeyboardInterrupt:
         clear()
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     # On Windows calling this function is necessary.
-    if sys.platform.startswith('win'):
+    if sys.platform.startswith("win"):
         multiprocessing.freeze_support()
-    main()
+    main()
```

### Comparing `ikabot-6.6.4/ikabot/function/activateMiracle.py` & `ikabot-7.0.1/ikabot/function/activateMiracle.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 #! /usr/bin/env python3
 # -*- coding: utf-8 -*-
 
-import json
 import gettext
+import json
 import traceback
+
 from ikabot.config import *
-from ikabot.helpers.gui import *
-from ikabot.helpers.varios import *
 from ikabot.helpers.botComm import *
+from ikabot.helpers.getJson import getCity
+from ikabot.helpers.gui import *
 from ikabot.helpers.pedirInfo import *
 from ikabot.helpers.process import set_child_mode
-from ikabot.helpers.getJson import getCity
 from ikabot.helpers.signals import setInfoSignal
+from ikabot.helpers.varios import *
 
-t = gettext.translation('activateMiracle', localedir, languages=languages, fallback=True)
+t = gettext.translation(
+    "activateMiracle", localedir, languages=languages, fallback=True
+)
 _ = t.gettext
 
 
 def obtainMiraclesAvailable(session):
     """
     Parameters
     ----------
@@ -28,108 +31,135 @@
     islands: list[dict]
     """
     idsIslands = getIslandsIds(session)
     islands = []
     for idIsland in idsIslands:
         html = session.get(island_url + idIsland)
         island = getIsland(html)
-        island['activable'] = False
+        island["activable"] = False
         islands.append(island)
 
     ids, cities = getIdsOfCities(session)
     for city_id in cities:
         city = cities[city_id]
         # get the wonder for this city
-        wonder = [island['wonder'] for island in islands if city['coords'] == '[{}:{}] '.format(island['x'], island['y'])][0]
+        wonder = [
+            island["wonder"]
+            for island in islands
+            if city["coords"] == "[{}:{}] ".format(island["x"], island["y"])
+        ][0]
         # if the wonder is not new, continue
-        if wonder in [island['wonder'] for island in islands if island['activable']]:
+        if wonder in [island["wonder"] for island in islands if island["activable"]]:
             continue
 
-        html = session.get(city_url + str(city['id']))
+        html = session.get(city_url + str(city["id"]))
         city = getCity(html)
 
         # make sure that the city has a temple
-        for i in range(len(city['position'])):
-            if city['position'][i]['building'] == 'temple':
-                city['pos'] = str(i)
+        for i in range(len(city["position"])):
+            if city["position"][i]["building"] == "temple":
+                city["pos"] = str(i)
                 break
         else:
             continue
 
         # get wonder information
-        params = {"view": "temple", "cityId": city['id'], "position": city['pos'], "backgroundView": "city", "currentCityId": city['id'], "actionRequest": actionRequest, "ajax": "1"}
+        params = {
+            "view": "temple",
+            "cityId": city["id"],
+            "position": city["pos"],
+            "backgroundView": "city",
+            "currentCityId": city["id"],
+            "actionRequest": actionRequest,
+            "ajax": "1",
+        }
         data = session.post(params=params)
         data = json.loads(data, strict=False)
         data = data[2][1]
-        available = data['js_WonderViewButton']['buttonState'] == 'enabled'
+        available = data["js_WonderViewButton"]["buttonState"] == "enabled"
         if available is False:
             for elem in data:
-                if 'countdown' in data[elem]:
-                    enddate = data[elem]['countdown']['enddate']
-                    currentdate = data[elem]['countdown']['currentdate']
+                if "countdown" in data[elem]:
+                    enddate = data[elem]["countdown"]["enddate"]
+                    currentdate = data[elem]["countdown"]["currentdate"]
                     break
 
         # set the information on the island which wonder we can activate
         for island in islands:
-            if island['id'] == city['islandId']:
-                island['activable'] = True
-                island['ciudad'] = city
-                island['available'] = available
+            if island["id"] == city["islandId"]:
+                island["activable"] = True
+                island["ciudad"] = city
+                island["available"] = available
                 if available is False:
-                    island['available_in'] = enddate - currentdate
+                    island["available_in"] = enddate - currentdate
                 break
 
     # only return island which wonder we can activate
-    return [island for island in islands if island['activable']]
+    return [island for island in islands if island["activable"]]
 
 
 def activateMiracleHttpCall(session, island):
     """
     Parameters
     ----------
     session : ikabot.web.session.Session
     island : dict
 
     Returns
     -------
     json : dict
     """
-    params = {'action': 'CityScreen', 'cityId': island['ciudad']['id'], 'function': 'activateWonder', 'position': island['ciudad']['pos'], 'backgroundView': 'city', 'currentCityId': island['ciudad']['id'], 'templateView': 'temple', 'actionRequest': actionRequest, 'ajax': '1'}
+    params = {
+        "action": "CityScreen",
+        "cityId": island["ciudad"]["id"],
+        "function": "activateWonder",
+        "position": island["ciudad"]["pos"],
+        "backgroundView": "city",
+        "currentCityId": island["ciudad"]["id"],
+        "templateView": "temple",
+        "actionRequest": actionRequest,
+        "ajax": "1",
+    }
     response = session.post(params=params)
     return json.loads(response, strict=False)
 
 
 def chooseIsland(islands):
     """
     Parameters
     ----------
     islands : list[dict]
 
     Returns
     -------
     island : dict
     """
-    print(_('Which miracle do you want to activate?'))
+    print(_("Which miracle do you want to activate?"))
     # Sort islands by name
-    sorted_islands = sorted(islands, key=lambda x: x['wonderName'])
+    sorted_islands = sorted(islands, key=lambda x: x["wonderName"])
     i = 0
-    print(_('(0) Exit'))
+    print(_("(0) Exit"))
     for island in sorted_islands:
         i += 1
-        if island['available']:
-            print('({:d}) {}'.format(i, island['wonderName']))
+        if island["available"]:
+            print("({:d}) {}".format(i, island["wonderName"]))
         else:
-            print(_('({:d}) {} (available in: {})').format(i, island['wonderName'], daysHoursMinutes(island['available_in'])))
+            print(
+                _("({:d}) {} (available in: {})").format(
+                    i, island["wonderName"], daysHoursMinutes(island["available_in"])
+                )
+            )
 
     index = read(min=0, max=i)
     if index == 0:
         return None
     island = sorted_islands[index - 1]
     return island
 
+
 def activateMiracle(session, event, stdin_fd, predetermined_input):
     """
     Parameters
     ----------
     session : ikabot.web.session.Session
     event : multiprocessing.Event
     stdin_fd: int
@@ -138,185 +168,217 @@
     sys.stdin = os.fdopen(stdin_fd)
     config.predetermined_input = predetermined_input
     try:
         banner()
 
         islands = obtainMiraclesAvailable(session)
         if islands == []:
-            print(_('There are no miracles available.'))
+            print(_("There are no miracles available."))
             enter()
             event.set()
             return
 
         island = chooseIsland(islands)
         if island is None:
             event.set()
             return
 
-        if island['available']:
-            print(_('\nThe miracle {} will be activated').format(island['wonderName']))
-            print(_('Proceed? [Y/n]'))
-            activate_miracle_input = read(values=['y', 'Y', 'n', 'N', ''])
-            if activate_miracle_input.lower() == 'n':
+        if island["available"]:
+            print(_("\nThe miracle {} will be activated").format(island["wonderName"]))
+            print(_("Proceed? [Y/n]"))
+            activate_miracle_input = read(values=["y", "Y", "n", "N", ""])
+            if activate_miracle_input.lower() == "n":
                 event.set()
                 return
 
             miracle_activation_result = activateMiracleHttpCall(session, island)
 
-            if miracle_activation_result[1][1][0] == 'error':
-                print(_('The miracle {} could not be activated.').format(island['wonderName']))
+            if miracle_activation_result[1][1][0] == "error":
+                print(
+                    _("The miracle {} could not be activated.").format(
+                        island["wonderName"]
+                    )
+                )
                 enter()
                 event.set()
                 return
 
             data = miracle_activation_result[2][1]
             for elem in data:
-                if 'countdown' in data[elem]:
-                    enddate = data[elem]['countdown']['enddate']
-                    currentdate = data[elem]['countdown']['currentdate']
+                if "countdown" in data[elem]:
+                    enddate = data[elem]["countdown"]["enddate"]
+                    currentdate = data[elem]["countdown"]["currentdate"]
                     break
             wait_time = enddate - currentdate
 
-            print(_('The miracle {} was activated.').format(island['wonderName']))
+            print(_("The miracle {} was activated.").format(island["wonderName"]))
             enter()
             banner()
 
             while True:
-                print(_('Do you wish to activate it again when it is finished? [y/N]'))
+                print(_("Do you wish to activate it again when it is finished? [y/N]"))
 
-                reactivate_again_input = read(values=['y', 'Y', 'n', 'N', ''])
-                if reactivate_again_input.lower() != 'y':
+                reactivate_again_input = read(values=["y", "Y", "n", "N", ""])
+                if reactivate_again_input.lower() != "y":
                     event.set()
                     return
 
-                iterations = read(msg=_('How many times?: '), digit=True, min=0)
+                iterations = read(msg=_("How many times?: "), digit=True, min=0)
 
                 if iterations == 0:
                     event.set()
                     return
 
                 duration = wait_time * iterations
 
-                print(_('It will finish in:{}').format(daysHoursMinutes(duration)))
+                print(_("It will finish in:{}").format(daysHoursMinutes(duration)))
 
-                print(_('Proceed? [Y/n]'))
-                reactivate_again_input = read(values=['y', 'Y', 'n', 'N', ''])
-                if reactivate_again_input.lower() == 'n':
+                print(_("Proceed? [Y/n]"))
+                reactivate_again_input = read(values=["y", "Y", "n", "N", ""])
+                if reactivate_again_input.lower() == "n":
                     banner()
                     continue
                 break
         else:
-            print(_('\nThe miracle {} will be activated in {}').format(island['wonderName'], daysHoursMinutes(island['available_in'])))
-            print(_('Proceed? [Y/n]'))
-            user_confirm = read(values=['y', 'Y', 'n', 'N', ''])
-            if user_confirm.lower() == 'n':
+            print(
+                _("\nThe miracle {} will be activated in {}").format(
+                    island["wonderName"], daysHoursMinutes(island["available_in"])
+                )
+            )
+            print(_("Proceed? [Y/n]"))
+            user_confirm = read(values=["y", "Y", "n", "N", ""])
+            if user_confirm.lower() == "n":
                 event.set()
                 return
-            wait_time = island['available_in']
+            wait_time = island["available_in"]
             iterations = 1
 
-            print(_('\nThe mirable will be activated.'))
+            print(_("\nThe mirable will be activated."))
             enter()
             banner()
 
             while True:
-                print(_('Do you wish to activate it again when it is finished? [y/N]'))
+                print(_("Do you wish to activate it again when it is finished? [y/N]"))
 
-                reactivate_again_input = read(values=['y', 'Y', 'n', 'N', ''])
-                again = reactivate_again_input.lower() == 'y'
+                reactivate_again_input = read(values=["y", "Y", "n", "N", ""])
+                again = reactivate_again_input.lower() == "y"
                 if again is True:
                     try:
-                        iterations = read(msg=_('How many times?: '), digit=True, min=0)
+                        iterations = read(msg=_("How many times?: "), digit=True, min=0)
                     except KeyboardInterrupt:
                         iterations = 1
                         break
 
                     if iterations == 0:
                         iterations = 1
                         break
 
                     iterations += 1
                     duration = wait_time * iterations
-                    print(_('It is not possible to calculate the time of finalization. (at least: {})').format(daysHoursMinutes(duration)))
-                    print(_('Proceed? [Y/n]'))
+                    print(
+                        _(
+                            "It is not possible to calculate the time of finalization. (at least: {})"
+                        ).format(daysHoursMinutes(duration))
+                    )
+                    print(_("Proceed? [Y/n]"))
 
                     try:
-                        activate_input = read(values=['y', 'Y', 'n', 'N', ''])
+                        activate_input = read(values=["y", "Y", "n", "N", ""])
                     except KeyboardInterrupt:
                         iterations = 1
                         break
 
-                    if activate_input.lower() == 'n':
+                    if activate_input.lower() == "n":
                         iterations = 1
                         banner()
                         continue
                 break
     except KeyboardInterrupt:
         event.set()
         return
 
     set_child_mode(session)
     event.set()
 
-    info = _('\nI activate the miracle {} {:d} times\n').format(island['wonderName'], iterations)
+    info = _("\nI activate the miracle {} {:d} times\n").format(
+        island["wonderName"], iterations
+    )
     setInfoSignal(session, info)
     try:
         do_it(session, island, iterations)
     except Exception as e:
-        msg = _('Error in:\n{}\nCause:\n{}').format(info, traceback.format_exc())
+        msg = _("Error in:\n{}\nCause:\n{}").format(info, traceback.format_exc())
         sendToBot(session, msg)
     finally:
         session.logout()
 
 
 def wait_for_miracle(session, island):
     """
     Parameters
     ----------
     session : ikabot.web.session.Session
     island : dict
     """
     while True:
-        params = {"view": "temple", "cityId": island['ciudad']['id'], "position": island['ciudad']['pos'], "backgroundView": "city", "currentCityId": island['ciudad']['id'], "actionRequest": actionRequest, "ajax": "1"}
+        params = {
+            "view": "temple",
+            "cityId": island["ciudad"]["id"],
+            "position": island["ciudad"]["pos"],
+            "backgroundView": "city",
+            "currentCityId": island["ciudad"]["id"],
+            "actionRequest": actionRequest,
+            "ajax": "1",
+        }
         temple_response = session.post(params=params)
         temple_response = json.loads(temple_response, strict=False)
         temple_response = temple_response[2][1]
 
         for elem in temple_response:
-            if 'countdown' in temple_response[elem]:
-                enddate = temple_response[elem]['countdown']['enddate']
-                currentdate = temple_response[elem]['countdown']['currentdate']
+            if "countdown" in temple_response[elem]:
+                enddate = temple_response[elem]["countdown"]["enddate"]
+                currentdate = temple_response[elem]["countdown"]["currentdate"]
                 wait_time = enddate - currentdate
                 break
         else:
-            available = temple_response['js_WonderViewButton']['buttonState'] == 'enabled'
+            available = (
+                temple_response["js_WonderViewButton"]["buttonState"] == "enabled"
+            )
             if available:
                 return
             else:
                 wait_time = 60
 
-        msg = _('I wait {:d} seconds to activate the miracle {}').format(wait_time, island['wonderName'])
+        msg = _("I wait {:d} seconds to activate the miracle {}").format(
+            wait_time, island["wonderName"]
+        )
         sendToBotDebug(session, msg, debugON_activateMiracle)
         wait(wait_time + 5)
 
 
 def do_it(session, island, iterations):
     """
     Parameters
     ----------
     session : ikabot.web.session.Session
     island : dict
     iterations : int
     """
+    iterations_left = iterations
     for i in range(iterations):
 
         wait_for_miracle(session, island)
 
         response = activateMiracleHttpCall(session, island)
 
-        if response[1][1][0] == 'error':
-            msg = _('The miracle {} could not be activated.').format(island['wonderName'])
+        if response[1][1][0] == "error":
+            msg = _("The miracle {} could not be activated.").format(
+                island["wonderName"]
+            )
             sendToBot(session, msg)
             return
-
-        msg = _('Miracle {} successfully activated').format(island['wonderName'])
+        iterations_left -= 1
+        session.setStatus(
+            f"Activated {island['wonderName']} @{getDateTime()}, iterations left: {iterations_left}"
+        )
+        msg = _("Miracle {} successfully activated").format(island["wonderName"])
         sendToBotDebug(session, msg, debugON_activateMiracle)
```

### Comparing `ikabot-6.6.4/ikabot/function/alertAttacks.py` & `ikabot-7.0.1/ikabot/function/alertAttacks.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from ikabot.function.vacationMode import activateVacationMode
 from ikabot.helpers.botComm import *
 from ikabot.helpers.gui import enter
 from ikabot.helpers.process import set_child_mode
 from ikabot.helpers.signals import setInfoSignal
 from ikabot.helpers.varios import daysHoursMinutes
 
-t = gettext.translation('alertAttacks', localedir, languages=languages, fallback=True)
+t = gettext.translation("alertAttacks", localedir, languages=languages, fallback=True)
 _ = t.gettext
 
 
 def alertAttacks(session, event, stdin_fd, predetermined_input):
     """
     Parameters
     ----------
@@ -30,32 +30,37 @@
     try:
         if checkTelegramData(session) is False:
             event.set()
             return
 
         banner()
         default = 20
-        minutes = read(msg=_('How often should I search for attacks?(min:3, default: {:d}): ').format(default), min=3,
-                       default=default)
+        minutes = read(
+            msg=_(
+                "How often should I search for attacks?(min:3, default: {:d}): "
+            ).format(default),
+            min=3,
+            default=default,
+        )
         # min_units = read(msg=_('Attacks with less than how many units should be ignored? (default: 0): '), digit=True, default=0)
-        print(_('I will check for attacks every {:d} minutes').format(minutes))
+        print(_("I will check for attacks every {:d} minutes").format(minutes))
         enter()
     except KeyboardInterrupt:
         event.set()
         return
 
     set_child_mode(session)
     event.set()
 
-    info = _('\nI check for attacks every {:d} minutes\n').format(minutes)
+    info = _("\nI check for attacks every {:d} minutes\n").format(minutes)
     setInfoSignal(session, info)
     try:
         do_it(session, minutes)
     except Exception as e:
-        msg = _('Error in:\n{}\nCause:\n{}').format(info, traceback.format_exc())
+        msg = _("Error in:\n{}\nCause:\n{}").format(info, traceback.format_exc())
         sendToBot(session, msg)
     finally:
         session.logout()
 
 
 def respondToAttack(session):
     """
@@ -67,15 +72,15 @@
     # this allows the user to respond to an attack via telegram
     while True:
         time.sleep(60 * 3)
         responses = getUserResponse(session)
         for response in responses:
             # the response should be in the form of:
             # <pid>:<action number>
-            rta = re.search(r'(\d+):?\s*(\d+)', response)
+            rta = re.search(r"(\d+):?\s*(\d+)", response)
             if rta is None:
                 continue
 
             pid = int(rta.group(1))
             action = int(rta.group(2))
 
             # if the pid doesn't match, we ignore it
@@ -83,15 +88,15 @@
                 continue
 
             # currently just one action is supported
             if action == 1:
                 # mv
                 activateVacationMode(session)
             else:
-                sendToBot(session, _('Invalid command: {:d}').format(action))
+                sendToBot(session, _("Invalid command: {:d}").format(action))
 
 
 def do_it(session, minutes):
     """
     Parameters
     ----------
     session : ikabot.web.session.Session
@@ -105,52 +110,59 @@
     knownAttacks = []
     while True:
         ##Catch errors inside the function to not exit for any reason.
         currentAttacks = []
         try:
             # get the militaryMovements
             html = session.get()
-            city_id = re.search(r'currentCityId:\s(\d+),', html).group(1)
-            url = 'view=militaryAdvisor&oldView=city&oldBackgroundView=city&backgroundView=city&currentCityId={}&actionRequest={}&ajax=1'.format(
-                city_id, actionRequest)
+            city_id = re.search(r"currentCityId:\s(\d+),", html).group(1)
+            url = "view=militaryAdvisor&oldView=city&oldBackgroundView=city&backgroundView=city&currentCityId={}&actionRequest={}&ajax=1".format(
+                city_id, actionRequest
+            )
             movements_response = session.post(url)
             postdata = json.loads(movements_response, strict=False)
-            militaryMovements = postdata[1][1][2]['viewScriptParams']['militaryAndFleetMovements']
-            timeNow = int(postdata[0][1]['time'])
-
-            for militaryMovement in [mov for mov in militaryMovements if mov['isHostile']]:
-                event_id = militaryMovement['event']['id']
+            militaryMovements = postdata[1][1][2]["viewScriptParams"][
+                "militaryAndFleetMovements"
+            ]
+            timeNow = int(postdata[0][1]["time"])
+
+            for militaryMovement in [
+                mov for mov in militaryMovements if mov["isHostile"]
+            ]:
+                event_id = militaryMovement["event"]["id"]
                 currentAttacks.append(event_id)
                 # if we already alerted this, do nothing
                 if event_id not in knownAttacks:
                     knownAttacks.append(event_id)
 
                     # get information about the attack
-                    missionText = militaryMovement['event']['missionText']
-                    origin = militaryMovement['origin']
-                    target = militaryMovement['target']
-                    amountTroops = militaryMovement['army']['amount']
-                    amountFleets = militaryMovement['fleet']['amount']
-                    timeLeft = int(militaryMovement['eventTime']) - timeNow
+                    missionText = militaryMovement["event"]["missionText"]
+                    origin = militaryMovement["origin"]
+                    target = militaryMovement["target"]
+                    amountTroops = militaryMovement["army"]["amount"]
+                    amountFleets = militaryMovement["fleet"]["amount"]
+                    timeLeft = int(militaryMovement["eventTime"]) - timeNow
 
                     # send alert
-                    msg = _('-- ALERT --\n')
-                    msg += missionText + '\n'
-                    msg += _('from the city {} of {}\n').format(origin['name'], origin['avatarName'])
-                    msg += _('a {}\n').format(target['name'])
-                    msg += _('{} units\n').format(amountTroops)
-                    msg += _('{} fleet\n').format(amountFleets)
-                    msg += _('arrival in: {}\n').format(daysHoursMinutes(timeLeft))
-                    msg += _('If you want to put the account in vacation mode send:\n')
-                    msg += _('{:d}:1').format(os.getpid())
+                    msg = _("-- ALERT --\n")
+                    msg += missionText + "\n"
+                    msg += _("from the city {} of {}\n").format(
+                        origin["name"], origin["avatarName"]
+                    )
+                    msg += _("a {}\n").format(target["name"])
+                    msg += _("{} units\n").format(amountTroops)
+                    msg += _("{} fleet\n").format(amountFleets)
+                    msg += _("arrival in: {}\n").format(daysHoursMinutes(timeLeft))
+                    msg += _("If you want to put the account in vacation mode send:\n")
+                    msg += _("{:d}:1").format(os.getpid())
                     sendToBot(session, msg)
 
         except Exception as e:
-            info = _('\nI check for attacks every {:d} minutes\n').format(minutes)
-            msg = _('Error in:\n{}\nCause:\n{}').format(info, traceback.format_exc())
+            info = _("\nI check for attacks every {:d} minutes\n").format(minutes)
+            msg = _("Error in:\n{}\nCause:\n{}").format(info, traceback.format_exc())
             sendToBot(session, msg)
 
         # remove old attacks from knownAttacks
         for event_id in list(knownAttacks):
             if event_id not in currentAttacks:
                 knownAttacks.remove(event_id)
```

### Comparing `ikabot-6.6.4/ikabot/function/alertLowWine.py` & `ikabot-7.0.1/ikabot/function/alertLowWine.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 #! /usr/bin/env python3
 # -*- coding: utf-8 -*-
 
+import gettext
 import re
 import time
 import traceback
-import gettext
 from decimal import *
+
 from ikabot.config import *
-from ikabot.helpers.signals import setInfoSignal
-from ikabot.helpers.process import set_child_mode
+from ikabot.helpers.botComm import *
+from ikabot.helpers.getJson import getCity
 from ikabot.helpers.gui import *
 from ikabot.helpers.pedirInfo import getIdsOfCities
-from ikabot.helpers.varios import daysHoursMinutes
-from ikabot.helpers.getJson import getCity
+from ikabot.helpers.process import set_child_mode
 from ikabot.helpers.resources import *
-from ikabot.helpers.botComm import *
+from ikabot.helpers.signals import setInfoSignal
+from ikabot.helpers.varios import daysHoursMinutes
 
-t = gettext.translation('alertLowWine', localedir, languages=languages, fallback=True)
+t = gettext.translation("alertLowWine", localedir, languages=languages, fallback=True)
 _ = t.gettext
 
 getcontext().prec = 30
 
 
 def alertLowWine(session, event, stdin_fd, predetermined_input):
     """
@@ -34,30 +35,39 @@
     sys.stdin = os.fdopen(stdin_fd)
     config.predetermined_input = predetermined_input
     try:
         if checkTelegramData(session) is False:
             event.set()
             return
         banner()
-        hours = read(msg=_('How many hours should be left until the wine runs out in a city so that it\'s alerted?'), min=1)
-        print(_('It will be alerted when the wine runs out in less than {:d} hours in any city').format(hours))
+        hours = read(
+            msg=_(
+                "How many hours should be left until the wine runs out in a city so that it's alerted?"
+            ),
+            min=1,
+        )
+        print(
+            _(
+                "It will be alerted when the wine runs out in less than {:d} hours in any city"
+            ).format(hours)
+        )
         enter()
     except KeyboardInterrupt:
         event.set()
         return
 
     set_child_mode(session)
     event.set()
 
-    info = _('\nI alert if the wine runs out in less than {:d} hours\n').format(hours)
+    info = _("\nI alert if the wine runs out in less than {:d} hours\n").format(hours)
     setInfoSignal(session, info)
     try:
         do_it(session, hours)
     except Exception as e:
-        msg = _('Error in:\n{}\nCause:\n{}').format(info, traceback.format_exc())
+        msg = _("Error in:\n{}\nCause:\n{}").format(info, traceback.format_exc())
         sendToBot(session, msg)
     finally:
         session.logout()
 
 
 def do_it(session, hours):
     """
@@ -77,43 +87,46 @@
                 was_alerted[cityId] = False
 
         for cityId in cities:
             html = session.get(city_url + cityId)
             city = getCity(html)
 
             # if the city doesn't even have a tavern built, ignore it
-            if 'tavern' not in [building['building'] for building in city['position']]:
+            if "tavern" not in [building["building"] for building in city["position"]]:
                 continue
 
-            consumption_per_hour = city['consumo']
+            consumption_per_hour = city["wineConsumptionPerHour"]
 
             # is a wine city
-            if cities[cityId]['tradegood'] == '1':
-                wine_production = getProductionPerSecond(session, cityId)[1]
-                wine_production = wine_production * 60 * 60
+            if cities[cityId]["tradegood"] == "1":
+                wine_production = (
+                    getProductionPerSecond(session, cityId)[1] * SECONDS_IN_HOUR
+                )
                 if consumption_per_hour > wine_production:
                     consumption_per_hour -= wine_production
                 else:
                     was_alerted[cityId] = False
                     continue
 
             consumption_per_seg = Decimal(consumption_per_hour) / Decimal(3600)
-            wine_available = city['recursos'][1]
+            wine_available = city["availableResources"][1]
 
             if consumption_per_seg == 0:
                 if was_alerted[cityId] is False:
-                    msg = _('The city {} is not consuming wine!').format(city['name'])
+                    msg = _("The city {} is not consuming wine!").format(city["name"])
                     sendToBot(session, msg)
                     was_alerted[cityId] = True
                 continue
 
             seconds_left = Decimal(wine_available) / Decimal(consumption_per_seg)
-            if seconds_left < hours*60*60:
+            if seconds_left < hours * 60 * 60:
                 if was_alerted[cityId] is False:
                     time_left = daysHoursMinutes(seconds_left)
-                    msg = _('In {}, the wine will run out in {}').format(time_left, city['name'])
+                    msg = _("In {}, the wine will run out in {}").format(
+                        time_left, city["name"]
+                    )
                     sendToBot(session, msg)
                     was_alerted[cityId] = True
             else:
                 was_alerted[cityId] = False
 
-        time.sleep(20*60)
+        time.sleep(20 * 60)
```

### Comparing `ikabot-6.6.4/ikabot/function/autoPirate.py` & `ikabot-7.0.1/ikabot/function/autoPirate.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 #! /usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 import gettext
-import sys
-import requests
 import re
-import traceback
+import sys
 import time
-from ikabot.helpers.pedirInfo import *
-from ikabot.helpers.gui import *
+import traceback
+
+import requests
+
 from ikabot.config import *
-from ikabot.helpers.getJson import *
 from ikabot.helpers.botComm import *
-from ikabot.helpers.varios import wait
-from ikabot.helpers.process import run
-
+from ikabot.helpers.getJson import *
+from ikabot.helpers.gui import *
+from ikabot.helpers.pedirInfo import *
+from ikabot.helpers.process import run, set_child_mode
+from ikabot.helpers.varios import timeStringToSec, wait
+from ikabot.helpers.apiComm import getPiratesCaptchaSolution
 
-t = gettext.translation('buyResources', localedir, languages=languages, fallback=True)
+t = gettext.translation("buyResources", localedir, languages=languages, fallback=True)
 _ = t.gettext
 
 
 def autoPirate(session, event, stdin_fd, predetermined_input):
     """
     Parameters
     ----------
@@ -28,229 +30,297 @@
     event : multiprocessing.Event
     stdin_fd: int
     predetermined_input : multiprocessing.managers.SyncManager.list
     """
     sys.stdin = os.fdopen(stdin_fd)
     config.predetermined_input = predetermined_input
     banner()
-    try:
-        if not isWindows:
-            path = run('which nslookup')
-            is_installed = re.search(r'/.*?/nslookup', path) is not None
-            if is_installed is False:
-                print('you must first install nslookup')
-                enter()
-                event.set()
-                return
+    try:        
 
-        print('{}⚠️ USING THIS FEATURE WILL EXPOSE YOUR IP ADDRESS TO A THIRD PARTY FOR CAPTCHA SOLVING ⚠️{}\n\n'.format(bcolors.WARNING, bcolors.ENDC))
-        print('How many pirate missions should I do? (min = 1)')
+        print(
+            "{}⚠️ USING THIS FEATURE WILL EXPOSE YOUR IP ADDRESS TO A THIRD PARTY FOR CAPTCHA SOLVING ⚠️{}\n\n".format(
+                bcolors.WARNING, bcolors.ENDC
+            )
+        )
+        print("How many pirate missions should I do? (min = 1)")
         pirateCount = read(min=1, digit=True)
-        print('Should I schedule pirate missions by the time of day? (y/N)')
-        scheduleInput = read(values=['y', 'Y', 'n', 'N', ''])
-        if scheduleInput.lower() == 'y':
+        print("Should I schedule pirate missions by the time of day? (y/N)")
+        scheduleInput = read(values=["y", "Y", "n", "N", ""])
+        if scheduleInput.lower() == "y":
             pirateSchedule = True
-            print("""Which pirate mission should I do at daytime? (Default mission)
+            print(
+                """Which pirate mission should I do at daytime? (Default mission)
         (1) 2m 30s
         (2) 7m 30s
         (3) 15m
         (4) 30m
         (5) 1h
         (6) 2h
         (7) 4h
         (8) 8h
         (9) 16h
-        """)
+        """
+            )
             pirateMissionDayChoice = read(min=1, max=9, digit=True)
-            print("""At which hours should I operate at daytime? (Default: 9 hours from 10 till 18)
-            """)
+            print(
+                """At which hours should I operate at daytime? (Default: 9 hours from 10 till 18)
+            """
+            )
             print("From: ")
             dayStart = read()
-            if dayStart == '':
+            if dayStart == "":
                 dayStart = 10
             else:
                 dayStart = int(dayStart)
 
             print("Till: ")
             dayEnd = read()
-            if dayEnd == '':
+            if dayEnd == "":
                 dayEnd = 18
             else:
                 dayEnd = int(dayEnd)
 
-            print("""Which pirate mission should I do at night time?
+            print(
+                """Which pirate mission should I do at night time?
             (1) 2m 30s
             (2) 7m 30s
             (3) 15m
             (4) 30m
             (5) 1h
             (6) 2h
             (7) 4h
             (8) 8h
             (9) 16h
-            """)
+            """
+            )
             pirateMissionNightChoice = read(min=1, max=9, digit=True)
 
-            print("""At which hours should I operate at night time? (Default: 15 hours from 19 till 9): 
-            """)
+            print(
+                """At which hours should I operate at night time? (Default: 15 hours from 19 till 9): 
+            """
+            )
             print("From: ")
             nightStart = read()
-            if nightStart == '':
+            if nightStart == "":
                 nightStart = 19
             else:
                 nightStart = int(nightStart)
 
             print("Till: ")
             nightEnd = read()
-            if nightEnd == '':
+            if nightEnd == "":
                 nightEnd = 9
             else:
                 nightEnd = int(nightEnd)
         else:
             pirateSchedule = False
-            print("""Which pirate mission should I do?
+            print(
+                """Which pirate mission should I do?
         (1) 2m 30s
         (2) 7m 30s
         (3) 15m
         (4) 30m
         (5) 1h
         (6) 2h
         (7) 4h
         (8) 8h
         (9) 16h
-        """)
+        """
+            )
             pirateMissionChoice = read(min=1, max=9, digit=True)
         if pirateSchedule == True:
             current_hour = int(time.strftime("%H"))
             if current_hour >= dayStart and current_hour <= dayEnd:
                 pirateMissionChoice = pirateMissionDayChoice
             elif current_hour >= nightStart or current_hour <= nightEnd:
                 pirateMissionChoice = pirateMissionNightChoice
             else:
                 pirateMissionChoice = pirateMissionDayChoice
-        print('Do you want me to automatically convert capture points to crew strength? (Y|N)')
-        autoConvert = read(values=['y', 'Y', 'n', 'N'])
-        if autoConvert.lower() == 'y':
-            print('How many points should I convert every time I do a mission? (Type "all" to convert all points at once)')
-            convertPerMission = read(min=0, additionalValues=['all'], digit=True)
-        print('Enter a maximum additional random waiting time between missions in seconds. (min = 0)')
+        print(
+            "Do you want me to automatically convert capture points to crew strength? (Y|N)"
+        )
+        autoConvert = read(values=["y", "Y", "n", "N"])
+        if autoConvert.lower() == "y":
+            print(
+                'How many points should I convert every time I do a mission? (Type "all" to convert all points at once)'
+            )
+            convertPerMission = read(min=0, additionalValues=["all"], digit=True)
+        print(
+            "Enter a maximum additional random waiting time between missions in seconds. (min = 0)"
+        )
         maxRandomWaitingTime = read(min=0, digit=True)
         piracyCities = getPiracyCities(session, pirateMissionChoice)
         if piracyCities == []:
-            print('You do not have any city with a pirate fortress capable of executing this mission!')
+            print(
+                "You do not have any city with a pirate fortress capable of executing this mission!"
+            )
             enter()
             event.set()
             return
 
-        print('YAAAAAR!')  # get data for options such as auto-convert to crew strength, time intervals, number of piracy attempts... ^^
+        print(
+            "YAAAAAR!"
+        )  # get data for options such as auto-convert to crew strength, time intervals, number of piracy attempts... ^^
         enter()
     except KeyboardInterrupt:
         event.set()
         return
+
+    set_child_mode(session)
     event.set()
+
     try:
-        while (pirateCount > 0):
-            session.setStatus('Pirating for '+str(pirateCount)+' more runs')
+        while pirateCount > 0:
+            session.setStatus("Pirating for " + str(pirateCount) + " more runs")
             if pirateSchedule == True:
                 current_hour = int(time.strftime("%H"))
                 if current_hour >= dayStart and current_hour <= dayEnd:
                     pirateMissionChoice = pirateMissionDayChoice
                 elif current_hour >= nightStart or current_hour <= nightEnd:
                     pirateMissionChoice = pirateMissionNightChoice
                 else:
                     pirateMissionChoice = pirateMissionDayChoice
             pirateCount -= 1
-            piracyCities = getPiracyCities(session, pirateMissionChoice)  # this is done again inside the loop in case the user destroys / creates another pirate fortress while this module is running
+            piracyCities = getPiracyCities(
+                session, pirateMissionChoice
+            )  # this is done again inside the loop in case the user destroys / creates another pirate fortress while this module is running
             if piracyCities == []:
-                raise Exception('No city with pirate fortress capable of executing selected mission')
-            html = session.post(city_url + str(piracyCities[0]['id']))  # this is needed because for some reason you need to look at the town where you are sending a request from in the line below, before you send that request
-            if '"showPirateFortressShip":0' in html:  # this is in case the user has manually run a capture run, in that case, there is no need to wait 150secs instead we can check every 5
-                url = 'view=pirateFortress&cityId={}&position=17&backgroundView=city&currentCityId={}&actionRequest={}&ajax=1'.format(piracyCities[0]['id'], piracyCities[0]['id'], actionRequest)
+                raise Exception(
+                    "No city with pirate fortress capable of executing selected mission"
+                )
+            html = session.post(
+                city_url + str(piracyCities[0]["id"])
+            )  # this is needed because for some reason you need to look at the town where you are sending a request from in the line below, before you send that request
+            if (
+                '"showPirateFortressShip":0' in html
+            ):  # this is in case the user has manually run a capture run, in that case, there is no need to wait 150secs instead we can check every 5
+                url = "view=pirateFortress&cityId={}&position=17&backgroundView=city&currentCityId={}&actionRequest={}&ajax=1".format(
+                    piracyCities[0]["id"], piracyCities[0]["id"], actionRequest
+                )
                 html = session.post(url)
                 wait(getCurrentMissionWaitingTime(html), maxRandomWaitingTime)
                 pirateCount += 1  # don't count this as an iteration of the loop
                 continue
 
-            url = 'action=PiracyScreen&function=capture&buildingLevel={0}&view=pirateFortress&cityId={1}&position=17&activeTab=tabBootyQuest&backgroundView=city&currentCityId={1}&templateView=pirateFortress&actionRequest={2}&ajax=1'.format(piracyMissionToBuildingLevel[pirateMissionChoice], piracyCities[0]['id'], actionRequest)
+            url = "action=PiracyScreen&function=capture&buildingLevel={0}&view=pirateFortress&cityId={1}&position=17&activeTab=tabBootyQuest&backgroundView=city&currentCityId={1}&templateView=pirateFortress&actionRequest={2}&ajax=1".format(
+                piracyMissionToBuildingLevel[pirateMissionChoice],
+                piracyCities[0]["id"],
+                actionRequest,
+            )
             html = session.post(url)
 
-            if 'function=createCaptcha' in html:
+            if "function=createCaptcha" in html:
                 try:
                     for i in range(20):
-                        session.setStatus('Resolving captcha '+str(i)+'/20')
+                        session.setStatus("Resolving captcha " + str(i) + "/20")
                         if i == 19:
-                            msg = 'Failed to resolve captcha too many times, autoPirate has been terminated.'
+                            msg = "Failed to resolve captcha too many times, autoPirate has been terminated."
                             sendToBot(session, msg)
                             raise Exception("Failed to resolve captcha too many times")
-                        picture = session.get('action=Options&function=createCaptcha', fullResponse=True).content
+                        picture = session.get(
+                            "action=Options&function=createCaptcha", fullResponse=True
+                        ).content
                         captcha = resolveCaptcha(session, picture)
-                        session.setStatus('Got captcha: '+captcha)
-                        if captcha == 'Error':
+                        session.setStatus("Got captcha: " + captcha)
+                        if captcha == "Error":
+                            time.sleep(5)
                             continue
-                        session.post(city_url + str(piracyCities[0]['id']))
-                        params = {'action': 'PiracyScreen', 'function': 'capture', 'cityId': piracyCities[0]['id'], 'position': '17', 'captchaNeeded': '1', 'buildingLevel': str(piracyMissionToBuildingLevel[pirateMissionChoice]), 'captcha': captcha, 'activeTab': 'tabBootyQuest', 'backgroundView': 'city', 'currentCityId': piracyCities[0]['id'], 'templateView': 'pirateFortress', 'actionRequest': actionRequest, 'ajax': '1'}
+                        session.post(city_url + str(piracyCities[0]["id"]))
+                        params = {
+                            "action": "PiracyScreen",
+                            "function": "capture",
+                            "cityId": piracyCities[0]["id"],
+                            "position": "17",
+                            "captchaNeeded": "1",
+                            "buildingLevel": str(
+                                piracyMissionToBuildingLevel[pirateMissionChoice]
+                            ),
+                            "captcha": captcha,
+                            "activeTab": "tabBootyQuest",
+                            "backgroundView": "city",
+                            "currentCityId": piracyCities[0]["id"],
+                            "templateView": "pirateFortress",
+                            "actionRequest": actionRequest,
+                            "ajax": "1",
+                        }
                         html = session.post(params=params, noIndex=True)
-                        if '"showPirateFortressShip":1' in html:  # if this is true, then the crew is still in the town, that means that the request didn't succeed
+                        if (
+                            '"showPirateFortressShip":1' in html
+                        ):  # if this is true, then the crew is still in the town, that means that the request didn't succeed
+                            time.sleep(5)
                             continue
                         break
                 except Exception:
-                    info = ''
-                    msg = _('Error in:\n{}\nCause:\n{}').format(info, traceback.format_exc())
+                    info = ""
+                    msg = _("Error in:\n{}\nCause:\n{}").format(
+                        info, traceback.format_exc()
+                    )
                     sendToBot(session, msg)
                     break
-            if autoConvert.lower() == 'y':
+            if autoConvert.lower() == "y":
                 convertCapturePoints(session, piracyCities, convertPerMission)
             wait(piracyMissionWaitingTime[pirateMissionChoice], maxRandomWaitingTime)
 
     except Exception:
-        info = ''
-        msg = _('Error in:\n{}\nCause:\n{}').format(info, traceback.format_exc())
+        info = ""
+        msg = _("Error in:\n{}\nCause:\n{}").format(info, traceback.format_exc())
         sendToBot(session, msg)
         event.set()
         return
 
 
 def resolveCaptcha(session, picture):
     session_data = session.getSessionData()
-    if 'decaptcha' not in session_data or session_data['decaptcha']['name'] == 'default':
-        text = run('nslookup -q=txt ikagod.twilightparadox.com ns2.afraid.org')
-        parts = text.split('"')
-        if len(parts) < 2:
-            # the DNS output is not well formed
-            return 'Error'
-        address = parts[1]
-
-        files = {'upload_file': picture}
-        captcha = requests.post('http://{0}'.format(address), files=files).text
+    if (
+        "decaptcha" not in session_data
+        or session_data["decaptcha"]["name"] == "default"
+    ):
+        captcha = getPiratesCaptchaSolution(session, picture)
         return captcha
-    elif session_data['decaptcha']['name'] == 'custom':
-        files = {'upload_file': picture}
-        captcha = requests.post('{0}'.format(session_data['decaptcha']['endpoint']), files=files).text
+    elif session_data["decaptcha"]["name"] == "custom":
+        files = {"upload_file": picture}
+        captcha = requests.post(
+            "{0}".format(session_data["decaptcha"]["endpoint"]), files=files
+        ).text
         return captcha
-    elif session_data['decaptcha']['name'] == '9kw.eu':
-        credits = requests.get("https://www.9kw.eu/index.cgi?action=usercaptchaguthaben&apikey={}".format(session_data['decaptcha']['relevant_data']['apiKey'])).text
+    elif session_data["decaptcha"]["name"] == "9kw.eu":
+        credits = requests.get(
+            "https://www.9kw.eu/index.cgi?action=usercaptchaguthaben&apikey={}".format(
+                session_data["decaptcha"]["relevant_data"]["apiKey"]
+            )
+        ).text
         if int(credits) < 10:
-            raise Exception('You do not have enough 9kw.eu credits!')
-        captcha_id = requests.post("https://www.9kw.eu/index.cgi?action=usercaptchaupload&apikey={}".format(session_data['decaptcha']['relevant_data']['apiKey']), headers={'Content-Type': 'multipart/form-data'}, files={'file-upload-01': picture}).text
+            raise Exception("You do not have enough 9kw.eu credits!")
+        captcha_id = requests.post(
+            "https://www.9kw.eu/index.cgi?action=usercaptchaupload&apikey={}".format(
+                session_data["decaptcha"]["relevant_data"]["apiKey"]
+            ),
+            headers={"Content-Type": "multipart/form-data"},
+            files={"file-upload-01": picture},
+        ).text
         while True:
-            captcha_result = requests.get("https://www.9kw.eu/index.cgi?action=usercaptchacorrectdata&id={}&apikey={}".format(captcha_id, session_data['decaptcha']['relevant_data']['apiKey'])).text
-            if captcha_result != '':
+            captcha_result = requests.get(
+                "https://www.9kw.eu/index.cgi?action=usercaptchacorrectdata&id={}&apikey={}".format(
+                    captcha_id, session_data["decaptcha"]["relevant_data"]["apiKey"]
+                )
+            ).text
+            if captcha_result != "":
                 return captcha_result.upper()
             wait(5)
-    elif session_data['decaptcha']['name'] == 'telegram':
-        sendToBot(session, 'Please solve the captcha', Photo=picture)
+    elif session_data["decaptcha"]["name"] == "telegram":
+        sendToBot(session, "Please solve the captcha", Photo=picture)
         captcha_time = time.time()
-        while(True):
+        while True:
             response = getUserResponse(session, fullResponse=True)
             if len(response) == 0:
                 time.sleep(5)
                 continue
             response = response[-1]
-            if response['date'] > captcha_time:
-                return response['text']
+            if response["date"] > captcha_time:
+                return response["text"]
             time.sleep(5)
 
 
 def getPiracyCities(session, pirateMissionChoice):
     """Gets all user's cities which have a pirate fortress in them
     Parameters
     ----------
@@ -261,54 +331,67 @@
     piracyCities : list[dict]
     """
     cities_ids = getIdsOfCities(session)[0]
     piracyCities = []
     for city_id in cities_ids:
         html = session.get(city_url + city_id)
         city = getCity(html)
-        for pos, building in enumerate(city['position']):
-            if building['building'] == 'pirateFortress' and building['level'] >= piracyMissionToBuildingLevel[pirateMissionChoice]:
+        for pos, building in enumerate(city["position"]):
+            if (
+                building["building"] == "pirateFortress"
+                and building["level"]
+                >= piracyMissionToBuildingLevel[pirateMissionChoice]
+            ):
                 piracyCities.append(city)
                 break
     return piracyCities
 
 
 def convertCapturePoints(session, piracyCities, convertPerMission):
     """Converts all the users capture points into crew strength
     Parameters
     ----------
     session : ikabot.web.session.Session
     piracyCities: a list containing all cities which have a pirate fortress
     """
-    html = session.get('view=pirateFortress&activeTab=tabCrew&cityId={0}&position=17&backgroundView=city&currentCityId={0}&templateView=pirateFortress'.format(piracyCities[0]['id']))
+    params = {
+        "view": "pirateFortress",
+        "activeTab": "tabCrew",
+        "cityId": piracyCities[0]["id"],
+        "position": 17,
+        "backgroundView": "city",
+        "currentCityId": piracyCities[0]["id"],
+        "templateView": "pirateFortress",
+        "actionRequest": actionRequest,
+        "ajax": 1,
+    }
+    html = session.post(params=params)
     rta = re.search(r'\\"capturePoints\\":\\"(\d+)\\"', html)
     capturePoints = int(rta.group(1))
-    if convertPerMission == 'all':
+    if convertPerMission == "all":
         convertPerMission = capturePoints
-    if 'conversionProgressBar' in html:  # if a conversion is still in progress
+    if "conversionProgressBar" in html:  # if a conversion is still in progress
         return
-    data = {'action': 'PiracyScreen', 'function': 'convert', 'view': 'pirateFortress', 'cityId': piracyCities[0]['id'], 'islandId': piracyCities[0]['islandId'], 'activeTab': 'tabCrew', 'crewPoints': str(int(convertPerMission/10)), 'position': '17', 'backgroundView': 'city', 'currentCityId': piracyCities[0]['id'], 'templateView': 'pirateFortress', 'actionRequest': actionRequest, 'ajax': '1'}
+    data = {
+        "action": "PiracyScreen",
+        "function": "convert",
+        "view": "pirateFortress",
+        "cityId": piracyCities[0]["id"],
+        "islandId": piracyCities[0]["islandId"],
+        "activeTab": "tabCrew",
+        "crewPoints": str(int(convertPerMission / 10)),
+        "position": "17",
+        "backgroundView": "city",
+        "currentCityId": piracyCities[0]["id"],
+        "templateView": "pirateFortress",
+        "actionRequest": actionRequest,
+        "ajax": "1",
+    }
     html = session.post(params=data, noIndex=True)
 
 
 def getCurrentMissionWaitingTime(html):
-    match = re.search(r'missionProgressTime\\\\">(.*?)<\\\\\/div>', html)
-    if match is None:
-        return 0
-    else:
-        time_string = match.group(1)
-        hours = re.search(r'(\d+)h', time_string)
-        if hours is None:
-            hours = 0
-        else:
-            hours = int(hours.group(1)) * 3600
-        minutes = re.search(r'(\d+)m', time_string)
-        if minutes is None:
-            minutes = 0
-        else:
-            minutes = int(minutes.group(1)) * 60
-        seconds = re.search(r'(\d+)s', time_string)
-        if seconds is None:
-            seconds = 0
-        else:
-            seconds = int(seconds.group(1)) * 1
-        return hours + minutes + seconds
+    match = re.search(r'ongoingMissionTimeRemaining\\":(\d+),', html)
+    assert (
+        match
+    ), "Couldn't find remaining ongoing mission time, did you run a pirate mission manually?"
+    return int(match.group(1))
```

### Comparing `ikabot-6.6.4/ikabot/function/buyResources.py` & `ikabot-7.0.1/ikabot/function/buyResources.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,62 +1,62 @@
 #! /usr/bin/env python3
 # -*- coding: utf-8 -*-
 
-import re
-import math
-import json
 import gettext
+import json
+import math
+import re
 import traceback
 from decimal import *
-from ikabot.helpers.process import set_child_mode
-from ikabot.helpers.varios import addThousandSeparator
-from ikabot.helpers.gui import enter, banner
-from ikabot.helpers.getJson import getCity
-from ikabot.helpers.signals import setInfoSignal
-from ikabot.helpers.planRoutes import waitForArrival
-from ikabot.helpers.pedirInfo import getIdsOfCities, read
-from ikabot.helpers.naval import getTotalShips
+
 from ikabot.config import *
 from ikabot.helpers.botComm import *
-from ikabot.helpers.resources import *
+from ikabot.helpers.getJson import getCity
+from ikabot.helpers.gui import banner, enter
 from ikabot.helpers.market import *
+from ikabot.helpers.naval import getTotalShips
+from ikabot.helpers.pedirInfo import getIdsOfCities, read
+from ikabot.helpers.planRoutes import waitForArrival
+from ikabot.helpers.process import set_child_mode
+from ikabot.helpers.resources import *
+from ikabot.helpers.signals import setInfoSignal
+from ikabot.helpers.varios import addThousandSeparator
 
-
-t = gettext.translation('buyResources', localedir, languages=languages, fallback=True)
+t = gettext.translation("buyResources", localedir, languages=languages, fallback=True)
 _ = t.gettext
 
 
 def chooseResource(session, city):
     """
     Parameters
     ----------
     session : ikabot.web.session.Session
     city : dict
     """
-    print(_('Which resource do you want to buy?'))
+    print(_("Which resource do you want to buy?"))
     for index, material_name in enumerate(materials_names):
-        print('({:d}) {}'.format(index+1, material_name))
+        print("({:d}) {}".format(index + 1, material_name))
     choise = read(min=1, max=5)
     resource = choise - 1
     if resource == 0:
-        resource = 'resource'
+        resource = "resource"
     data = {
-        'cityId': city['id'],
-        'position': city['pos'],
-        'view': 'branchOffice',
-        'activeTab': 'bargain',
-        'type': 444,
-        'searchResource': resource,
-        'range': city['rango'],
-        'backgroundView': 'city',
-        'currentCityId': city['id'],
-        'templateView': 'branchOffice',
-        'currentTab': 'bargain',
-        'actionRequest': actionRequest,
-        'ajax': 1
+        "cityId": city["id"],
+        "position": city["pos"],
+        "view": "branchOffice",
+        "activeTab": "bargain",
+        "type": 444,
+        "searchResource": resource,
+        "range": city["rango"],
+        "backgroundView": "city",
+        "currentCityId": city["id"],
+        "templateView": "branchOffice",
+        "currentTab": "bargain",
+        "actionRequest": actionRequest,
+        "ajax": 1,
     }
     # this will set the chosen resource in the store
     session.post(params=data)
     resource = choise - 1
     # return the chosen resource
     return resource
 
@@ -68,45 +68,58 @@
     session : ikabot.web.session.Session
     city : dict
     Returns
     -------
     offers : list[dict]
     """
     html = getMarketHtml(session, city)
-    hits = re.findall(r'short_text80">(.*?) *<br/>\((.*?)\)\s *</td>\s *<td>(\d+)</td>\s *<td>(.*?)/td>\s *<td><img src="(.*?)\.png[\s\S]*?white-space:nowrap;">(\d+)\s[\s\S]*?href="\?view=takeOffer&destinationCityId=(\d+)&oldView=branchOffice&activeTab=bargain&cityId=(\d+)&position=(\d+)&type=(\d+)&resource=(\w+)"', html)
+    hits = re.findall(
+        r'short_text80">(.*?) *<br/>\((.*?)\)\s *</td>\s *<td>(\d+)</td>\s *<td>(.*?)/td>\s *<td><img src="(.*?)\.png[\s\S]*?white-space:nowrap;">(\d+)\s[\s\S]*?href="\?view=takeOffer&destinationCityId=(\d+)&oldView=branchOffice&activeTab=bargain&cityId=(\d+)&position=(\d+)&type=(\d+)&resource=(\w+)"',
+        html,
+    )
     offers = []
     for hit in hits:
         offer = {
-            'ciudadDestino': hit[0],
-            'jugadorAComprar': hit[1],
-            'bienesXminuto': int(hit[2]),
-            'amountAvailable': int(hit[3].replace(',', '').replace('.', '').replace('<', '')),
-            'tipo': hit[4],
-            'precio': int(hit[5]),
-            'destinationCityId': hit[6],
-            'cityId': hit[7],
-            'position': hit[8],
-            'type': hit[9],
-            'resource': hit[10]
+            "ciudadDestino": hit[0],
+            "jugadorAComprar": hit[1],
+            "bienesXminuto": int(hit[2]),
+            "amountAvailable": int(
+                hit[3].replace(",", "").replace(".", "").replace("<", "")
+            ),
+            "tipo": hit[4],
+            "precio": int(hit[5]),
+            "destinationCityId": hit[6],
+            "cityId": hit[7],
+            "position": hit[8],
+            "type": hit[9],
+            "resource": hit[10],
         }
-        
-        #Parse CDN Images to material type
-        if offer["tipo"] == '//gf2.geo.gfsrv.net/cdn19/c3527b2f694fb882563c04df6d8972':
-             offer["tipo"] = 'wood'
-        elif offer["tipo"] == '//gf1.geo.gfsrv.net/cdnc6/94ddfda045a8f5ced3397d791fd064':
-            offer["tipo"] = 'wine'     
-        elif  offer["tipo"] == '//gf3.geo.gfsrv.net/cdnbf/fc258b990c1a2a36c5aeb9872fc08a':
-             offer["tipo"] = 'marble'
-        elif  offer["tipo"] == '//gf2.geo.gfsrv.net/cdn1e/417b4059940b2ae2680c070a197d8c':
-             offer["tipo"] = 'glass'
-        elif  offer["tipo"] == '//gf1.geo.gfsrv.net/cdn9b/5578a7dfa3e98124439cca4a387a61':
-             offer["tipo"] = 'sulfur'
+
+        # Parse CDN Images to material type
+        if offer["tipo"] == "//gf2.geo.gfsrv.net/cdn19/c3527b2f694fb882563c04df6d8972":
+            offer["tipo"] = "wood"
+        elif (
+            offer["tipo"] == "//gf1.geo.gfsrv.net/cdnc6/94ddfda045a8f5ced3397d791fd064"
+        ):
+            offer["tipo"] = "wine"
+        elif (
+            offer["tipo"] == "//gf3.geo.gfsrv.net/cdnbf/fc258b990c1a2a36c5aeb9872fc08a"
+        ):
+            offer["tipo"] = "marble"
+        elif (
+            offer["tipo"] == "//gf2.geo.gfsrv.net/cdn1e/417b4059940b2ae2680c070a197d8c"
+        ):
+            offer["tipo"] = "glass"
+        elif (
+            offer["tipo"] == "//gf1.geo.gfsrv.net/cdn9b/5578a7dfa3e98124439cca4a387a61"
+        ):
+            offer["tipo"] = "sulfur"
         else:
             continue
-            
+
         offers.append(offer)
     return offers
 
 
 def calculateCost(offers, total_amount_to_buy):
     """
     Parameters
@@ -117,33 +130,33 @@
     -------
     total_cost : int
     """
     total_cost = 0
     for offer in offers:
         if total_amount_to_buy == 0:
             break
-        buy_amount = min(offer['amountAvailable'], total_amount_to_buy)
+        buy_amount = min(offer["amountAvailable"], total_amount_to_buy)
         total_amount_to_buy -= buy_amount
-        total_cost += buy_amount * offer['precio']
+        total_cost += buy_amount * offer["precio"]
     return total_cost
 
 
 def chooseCommertialCity(commercial_cities):
     """
     Parameters
     ----------
     commercial_cities : list[dict]
 
     Returns
     -------
     commercial_city : dict
     """
-    print(_('From which city do you want to buy resources?\n'))
+    print(_("From which city do you want to buy resources?\n"))
     for i, city in enumerate(commercial_cities):
-        print('({:d}) {}'.format(i + 1, city['name']))
+        print("({:d}) {}".format(i + 1, city["name"]))
     selected_city_index = read(min=1, max=len(commercial_cities))
     return commercial_cities[selected_city_index - 1]
 
 
 def buyResources(session, event, stdin_fd, predetermined_input):
     """
     Parameters
@@ -157,15 +170,15 @@
     config.predetermined_input = predetermined_input
     try:
         banner()
 
         # get all the cities with a store
         commercial_cities = getCommercialCities(session)
         if len(commercial_cities) == 0:
-            print(_('There is no store build'))
+            print(_("There is no store build"))
             enter()
             event.set()
             return
 
         # choose which city to buy from
         if len(commercial_cities) == 1:
             city = commercial_cities[0]
@@ -176,71 +189,89 @@
         # choose resource to buy
         resource = chooseResource(session, city)
         banner()
 
         # get all the offers of the chosen resource from the chosen city
         offers = getOffers(session, city)
         if len(offers) == 0:
-            print(_('There are no offers available.'))
+            print(_("There are no offers available."))
             enter()
             event.set()
             return
 
         # display offers to the user
         total_price = 0
         total_amount = 0
         for offer in offers:
-            amount = offer['amountAvailable']
-            price = offer['precio']
+            amount = offer["amountAvailable"]
+            price = offer["precio"]
             cost = amount * price
-            print(_('amount:{}').format(addThousandSeparator(amount)))
-            print(_('price :{:d}').format(price))
-            print(_('cost  :{}').format(addThousandSeparator(cost)))
-            print('')
+            print(_("amount:{}").format(addThousandSeparator(amount)))
+            print(_("price :{:d}").format(price))
+            print(_("cost  :{}").format(addThousandSeparator(cost)))
+            print("")
             total_price += cost
             total_amount += amount
 
         # ask how much to buy
-        print(_('Total amount available to purchase: {}, for {}').format(addThousandSeparator(total_amount), addThousandSeparator(total_price)))
-        available = city['freeSpaceForResources'][resource]
+        print(
+            _("Total amount available to purchase: {}, for {}").format(
+                addThousandSeparator(total_amount), addThousandSeparator(total_price)
+            )
+        )
+        available = city["freeSpaceForResources"][resource]
         if available < total_amount:
-            print(_('You just can buy {} due to storing capacity').format(addThousandSeparator(available)))
+            print(
+                _("You just can buy {} due to storing capacity").format(
+                    addThousandSeparator(available)
+                )
+            )
             total_amount = available
-        print('')
-        amount_to_buy = read(msg=_('How much do you want to buy?: '), min=0, max=total_amount)
+        print("")
+        amount_to_buy = read(
+            msg=_("How much do you want to buy?: "), min=0, max=total_amount
+        )
         if amount_to_buy == 0:
             event.set()
             return
 
         # calculate the total cost
         (gold, __) = getGold(session, city)
         total_cost = calculateCost(offers, amount_to_buy)
 
-        print(_('\nCurrent gold: {}.\nTotal cost  : {}.\nFinal gold  : {}.'). format(addThousandSeparator(gold), addThousandSeparator(total_cost), addThousandSeparator(gold - total_cost)))
-        print(_('Proceed? [Y/n]'))
-        rta = read(values=['y', 'Y', 'n', 'N', ''])
-        if rta.lower() == 'n':
+        print(
+            _("\nCurrent gold: {}.\nTotal cost  : {}.\nFinal gold  : {}.").format(
+                addThousandSeparator(gold),
+                addThousandSeparator(total_cost),
+                addThousandSeparator(gold - total_cost),
+            )
+        )
+        print(_("Proceed? [Y/n]"))
+        rta = read(values=["y", "Y", "n", "N", ""])
+        if rta.lower() == "n":
             event.set()
             return
 
-        print(_('It will be purchased {}').format(addThousandSeparator(amount_to_buy)))
+        print(_("It will be purchased {}").format(addThousandSeparator(amount_to_buy)))
         enter()
     except KeyboardInterrupt:
         event.set()
         return
 
     set_child_mode(session)
     event.set()
 
-    info = _('\nI will buy {} from {} to {}\n').format(addThousandSeparator(amount_to_buy), materials_names[resource], city['cityName'])
+    info = _("\nI will buy {} from {} to {}\n").format(
+        addThousandSeparator(amount_to_buy), materials_names[resource], city["cityName"]
+    )
     setInfoSignal(session, info)
     try:
         do_it(session, city, offers, amount_to_buy)
     except Exception as e:
-        msg = _('Error in:\n{}\nCause:\n{}').format(info, traceback.format_exc())
+        msg = _("Error in:\n{}\nCause:\n{}").format(info, traceback.format_exc())
         sendToBot(session, msg)
     finally:
         session.logout()
 
 
 def buy(session, city, offer, amount_to_buy, ships_available):
     """
@@ -249,56 +280,68 @@
     session : ikabot.web.session.Session
     city : dict
     offer : dict
     amount_to_buy : int
     """
     ships = int(math.ceil((Decimal(amount_to_buy) / Decimal(500))))
     data_dict = {
-        'action': 'transportOperations',
-        'function': 'buyGoodsAtAnotherBranchOffice',
-        'cityId': offer['cityId'],
-        'destinationCityId': offer['destinationCityId'],
-        'oldView': 'branchOffice',
-        'position': city['pos'],
-        'avatar2Name': offer['jugadorAComprar'],
-        'city2Name': offer['ciudadDestino'],
-        'type': int(offer['type']),
-        'activeTab': 'bargain',
-        'transportDisplayPrice': 0,
-        'premiumTransporter': 0,
-        'normalTransportersMax': ships_available,
-        'capacity': 5,
-        'max_capacity': 5,
-        'jetPropulsion': 0,
-        'transporters': ships,
-        'backgroundView': 'city',
-        'currentCityId': offer['cityId'],
-        'templateView': 'takeOffer',
-        'currentTab': 'bargain',
-        'actionRequest': actionRequest,
-        'ajax': 1
+        "action": "transportOperations",
+        "function": "buyGoodsAtAnotherBranchOffice",
+        "cityId": offer["cityId"],
+        "destinationCityId": offer["destinationCityId"],
+        "oldView": "branchOffice",
+        "position": city["pos"],
+        "avatar2Name": offer["jugadorAComprar"],
+        "city2Name": offer["ciudadDestino"],
+        "type": int(offer["type"]),
+        "activeTab": "bargain",
+        "transportDisplayPrice": 0,
+        "premiumTransporter": 0,
+        "normalTransportersMax": ships_available,
+        "capacity": 5,
+        "max_capacity": 5,
+        "jetPropulsion": 0,
+        "transporters": ships,
+        "backgroundView": "city",
+        "currentCityId": offer["cityId"],
+        "templateView": "takeOffer",
+        "currentTab": "bargain",
+        "actionRequest": actionRequest,
+        "ajax": 1,
     }
-    url = 'view=takeOffer&destinationCityId={}&oldView=branchOffice&activeTab=bargain&cityId={}&position={}&type={}&resource={}&backgroundView=city&currentCityId={}&templateView=branchOffice&actionRequest={}&ajax=1'.format(offer['destinationCityId'], offer['cityId'], offer['position'], offer['type'], offer['resource'], offer['cityId'], actionRequest)
+    url = "view=takeOffer&destinationCityId={}&oldView=branchOffice&activeTab=bargain&cityId={}&position={}&type={}&resource={}&backgroundView=city&currentCityId={}&templateView=branchOffice&actionRequest={}&ajax=1".format(
+        offer["destinationCityId"],
+        offer["cityId"],
+        offer["position"],
+        offer["type"],
+        offer["resource"],
+        offer["cityId"],
+        actionRequest,
+    )
     data = session.post(url)
     html = json.loads(data, strict=False)[1][1][1]
     hits = re.findall(r'"tradegood(\d)Price"\s*value="(\d+)', html)
     for hit in hits:
-        data_dict['tradegood{}Price'.format(hit[0])] = int(hit[1])
-        data_dict['cargo_tradegood{}'.format(hit[0])] = 0
+        data_dict["tradegood{}Price".format(hit[0])] = int(hit[1])
+        data_dict["cargo_tradegood{}".format(hit[0])] = 0
     hit = re.search(r'"resourcePrice"\s*value="(\d+)', html)
     if hit:
-        data_dict['resourcePrice'] = int(hit.group(1))
-        data_dict['cargo_resource'] = 0
-    resource = offer['resource']
-    if resource == 'resource':
-        data_dict['cargo_resource'] = amount_to_buy
+        data_dict["resourcePrice"] = int(hit.group(1))
+        data_dict["cargo_resource"] = 0
+    resource = offer["resource"]
+    if resource == "resource":
+        data_dict["cargo_resource"] = amount_to_buy
     else:
-        data_dict['cargo_tradegood{}'.format(resource)] = amount_to_buy
+        data_dict["cargo_tradegood{}".format(resource)] = amount_to_buy
     session.post(params=data_dict)
-    msg = _('I buy {} to {} from {}').format(addThousandSeparator(amount_to_buy), offer['ciudadDestino'], offer['jugadorAComprar'])
+    msg = _("I buy {} to {} from {}").format(
+        addThousandSeparator(amount_to_buy),
+        offer["ciudadDestino"],
+        offer["jugadorAComprar"],
+    )
     sendToBotDebug(session, msg, debugON_buyResources)
 
 
 def do_it(session, city, offers, amount_to_buy):
     """
     Parameters
     ----------
@@ -307,19 +350,19 @@
     offers : list[dict]
     amount_to_buy : int
     """
     while True:
         for offer in offers:
             if amount_to_buy == 0:
                 return
-            if offer['amountAvailable'] == 0:
+            if offer["amountAvailable"] == 0:
                 continue
 
             ships_available = waitForArrival(session)
             storageCapacity = ships_available * 500
-            buy_amount = min(amount_to_buy, storageCapacity, offer['amountAvailable'])
+            buy_amount = min(amount_to_buy, storageCapacity, offer["amountAvailable"])
 
             amount_to_buy -= buy_amount
-            offer['amountAvailable'] -= buy_amount
+            offer["amountAvailable"] -= buy_amount
             buy(session, city, offer, buy_amount, ships_available)
             # start from the beginning again, so that we always buy from the cheapest offers fisrt
             break
```

### Comparing `ikabot-6.6.4/ikabot/function/checkForUpdate.py` & `ikabot-7.0.1/ikabot/function/checkForUpdate.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 #! /usr/bin/env python3
 # -*- coding: utf-8 -*-
 
-import re
 import gettext
+import re
+
 import ikabot.config as config
 from ikabot.helpers.process import run
 
-t = gettext.translation('checkForUpdate', config.localedir, languages=config.languages, fallback=True)
+t = gettext.translation(
+    "checkForUpdate", config.localedir, languages=config.languages, fallback=True
+)
 _ = t.gettext
 
 
 def checkForUpdate():
-    upgrade = run('python3 -m pip search ikabot')
-    if 'ikabot' not in upgrade:
+    upgrade = run("python3 -m pip search ikabot")
+    if "ikabot" not in upgrade:
         return
 
-    upgrade = upgrade.split('\n')
+    upgrade = upgrade.split("\n")
     if len(upgrade) != 3:
         return
 
     upgrade = upgrade[2]
-    match = re.search(r' +.*?: +(.*)', upgrade)
+    match = re.search(r" +.*?: +(.*)", upgrade)
     if match is None:
         return
 
     new = match.group(1)
-    config.update_msg = _('[+] ikabot version {} is available\n').format(new)
+    config.update_msg = _("[+] ikabot version {} is available\n").format(new)
```

### Comparing `ikabot-6.6.4/ikabot/function/constructionList.py` & `ikabot-7.0.1/ikabot/function/constructionList.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,69 +1,85 @@
 #! /usr/bin/env python3
 # -*- coding: utf-8 -*-
 
-import re
-import time
+import gettext
+import hashlib
 import json
 import math
 import random
-import gettext
-import traceback
+import re
 import threading
-import hashlib
-import requests
+import time
+import traceback
 from decimal import *
+
+import requests
+
 from ikabot.config import *
-from ikabot.helpers.gui import *
-from ikabot.helpers.varios import *
 from ikabot.helpers.botComm import *
+from ikabot.helpers.getJson import getCity
+from ikabot.helpers.gui import *
 from ikabot.helpers.pedirInfo import *
-from ikabot.web.session import normal_get
 from ikabot.helpers.planRoutes import *
-from ikabot.helpers.getJson import getCity
-from ikabot.helpers.signals import setInfoSignal
 from ikabot.helpers.process import set_child_mode
 from ikabot.helpers.resources import getAvailableResources
-t = gettext.translation('constructionList', localedir, languages=languages, fallback=True)
+from ikabot.helpers.signals import setInfoSignal
+from ikabot.helpers.varios import *
+from ikabot.web.session import normal_get
+
+t = gettext.translation(
+    "constructionList", localedir, languages=languages, fallback=True
+)
 _ = t.gettext
 
 sendResources = True
 expand = True
 thread = None
 
-def waitForConstruction(session, city_id):
+
+def waitForConstruction(session, city_id, final_lvl):
     """
     Parameters
     ----------
     session : ikabot.web.session.Session
     city_id : int
+    final_lvl : int
 
     Returns
     -------
     city : dict
     """
     while True:
 
         html = session.get(city_url + city_id)
         city = getCity(html)
 
-        construction_buildings = [building for building in city['position'] if 'completed' in building]
+        construction_buildings = [
+            building for building in city["position"] if "completed" in building
+        ]
         if len(construction_buildings) == 0:
             break
 
         construction_building = construction_buildings[0]
-        construction_time = construction_building['completed']
+        construction_time = construction_building["completed"]
 
         current_time = int(time.time())
         final_time = int(construction_time)
         seconds_to_wait = final_time - current_time
 
-        msg = _('{}: I wait {:d} seconds so that {} gets to the level {:d}').format(city['cityName'], seconds_to_wait, construction_building['name'], construction_building['level'] + 1)
+        msg = _("{}: I wait {:d} seconds so that {} gets to the level {:d}").format(
+            city["cityName"],
+            seconds_to_wait,
+            construction_building["name"],
+            construction_building["level"] + 1,
+        )
         sendToBotDebug(session, msg, debugON_constructionList)
-
+        session.setStatus(
+            f"Waiting until {getDateTime(time.time()+seconds_to_wait+10)[8:]}, {construction_building['name']} {construction_building['level']} -> {construction_building['level']+1} in {city['name']}, final lvl: {final_lvl}"
+        )
         wait(seconds_to_wait + 10)
 
     html = session.get(city_url + city_id)
     city = getCity(html)
     return city
 
 
@@ -72,61 +88,76 @@
     Parameters
     ----------
     session : ikabot.web.session.Session
     cityId : int
     building : dict
     waitForResources : bool
     """
-    current_level = building['level']
-    if building['isBusy']:
+    current_level = building["level"]
+    if building["isBusy"]:
         current_level += 1
-    levels_to_upgrade = building['upgradeTo'] - current_level
-    position = building['position']
-
-    time.sleep(random.randint(5, 15))  # to avoid race conditions with sendResourcesNeeded
+    levels_to_upgrade = building["upgradeTo"] - current_level
+    position = building["position"]
+    upgradeTo = building["upgradeTo"]
+    time.sleep(
+        random.randint(5, 15)
+    )  # to avoid race conditions with sendResourcesNeeded
 
     for lv in range(levels_to_upgrade):
-        city = waitForConstruction(session, cityId)
-        building = city['position'][position]
+        city = waitForConstruction(session, cityId, upgradeTo)
+        building = city["position"][position]
 
-        if building['canUpgrade'] is False and waitForResources is True:
-            while building['canUpgrade'] is False:
+        if building["canUpgrade"] is False and waitForResources is True:
+            while building["canUpgrade"] is False:
                 time.sleep(60)
                 seconds = getMinimumWaitingTime(session)
                 html = session.get(city_url + cityId)
                 city = getCity(html)
-                building = city['position'][position]
+                building = city["position"][position]
                 # if no ships are comming, exit no matter if the building can or can't upgrade
                 if seconds == 0:
                     break
                 wait(seconds + 5)
 
-        if building['canUpgrade'] is False:
-            msg = _('City:{}\n').format(city['cityName'])
-            msg += _('Building:{}\n').format(building['name'])
-            msg += _('The building could not be completed due to lack of resources.\n')
-            msg += _('Missed {:d} levels').format(levels_to_upgrade - lv)
+        if building["canUpgrade"] is False:
+            msg = _("City:{}\n").format(city["cityName"])
+            msg += _("Building:{}\n").format(building["name"])
+            msg += _("The building could not be completed due to lack of resources.\n")
+            msg += _("Missed {:d} levels").format(levels_to_upgrade - lv)
             sendToBot(session, msg)
             return
 
-        url = 'action=CityScreen&function=upgradeBuilding&actionRequest={}&cityId={}&position={:d}&level={}&activeTab=tabSendTransporter&backgroundView=city&currentCityId={}&templateView={}&ajax=1'.format(actionRequest, cityId, position, building['level'], cityId, building['building'])
+        url = "action=CityScreen&function=upgradeBuilding&actionRequest={}&cityId={}&position={:d}&level={}&activeTab=tabSendTransporter&backgroundView=city&currentCityId={}&templateView={}&ajax=1".format(
+            actionRequest,
+            cityId,
+            position,
+            building["level"],
+            cityId,
+            building["building"],
+        )
         resp = session.post(url)
         html = session.get(city_url + cityId)
         city = getCity(html)
-        building = city['position'][position]
-        if building['isBusy'] is False:
-            msg = _('{}: The building {} was not extended').format(city['cityName'], building['name'])
+        building = city["position"][position]
+        if building["isBusy"] is False:
+            msg = _("{}: The building {} was not extended").format(
+                city["cityName"], building["name"]
+            )
             sendToBot(session, msg)
             sendToBot(session, resp)
             return
 
-        msg = _('{}: The building {} is being extended to level {:d}.').format(city['cityName'], building['name'], building['level']+1)
+        msg = _("{}: The building {} is being extended to level {:d}.").format(
+            city["cityName"], building["name"], building["level"] + 1
+        )
         sendToBotDebug(session, msg, debugON_constructionList)
 
-    msg = _('{}: The building {} finished extending to level: {:d}.').format(city['cityName'], building['name'], building['level']+1)
+    msg = _("{}: The building {} finished extending to level: {:d}.").format(
+        city["cityName"], building["name"], building["level"] + 1
+    )
     sendToBotDebug(session, msg, debugON_constructionList)
 
 
 def getCostsReducers(city):
     """
     Parameters
     ----------
@@ -135,27 +166,27 @@
     Returns
     -------
     reducers_per_material_level : dict[int, int]
     """
     reducers_per_material = [0] * len(materials_names)
     assert len(reducers_per_material) == 5
 
-    for building in city['position']:
-        if building['name'] == 'empty':
+    for building in city["position"]:
+        if building["name"] == "empty":
             continue
-        lv = building['level']
-        if building['building'] == 'carpentering':
+        lv = building["level"]
+        if building["building"] == "carpentering":
             reducers_per_material[0] = lv
-        elif building['building'] == 'vineyard':
+        elif building["building"] == "vineyard":
             reducers_per_material[1] = lv
-        elif building['building'] == 'architect':
+        elif building["building"] == "architect":
             reducers_per_material[2] = lv
-        elif building['building'] == 'optician':
+        elif building["building"] == "optician":
             reducers_per_material[3] = lv
-        elif building['building'] == 'fireworker':
+        elif building["building"] == "fireworker":
             reducers_per_material[4] = lv
     return reducers_per_material
 
 
 def getResourcesNeeded(session, city, building, current_level, final_level):
     """
     Parameters
@@ -167,71 +198,85 @@
     final_level : int
 
     Returns
     -------
     costs_per_material : dict[int, int]
     """
     # get html with information about buildings
-    building_detail_url = 'view=buildingDetail&buildingId=0&helpId=1&backgroundView=city&currentCityId={}&templateView=ikipedia&actionRequest={}&ajax=1'.format(city['id'], actionRequest)
+    building_detail_url = "view=buildingDetail&buildingId=0&helpId=1&backgroundView=city&currentCityId={}&templateView=ikipedia&actionRequest={}&ajax=1".format(
+        city["id"], actionRequest
+    )
     building_detail_response = session.post(building_detail_url)
     building_detail = json.loads(building_detail_response, strict=False)
     building_html = building_detail[1][1][1]
 
     # get html with information about buildings costs
-    regex_building_detail = r'<div class="(?:selected)? button_building ' + re.escape(building['building']) + r'"\s*onmouseover="\$\(this\)\.addClass\(\'hover\'\);" onmouseout="\$\(this\)\.removeClass\(\'hover\'\);"\s*onclick="ajaxHandlerCall\(\'\?(.*?)\'\);'
+    regex_building_detail = (
+        r'<div class="(?:selected)? button_building '
+        + re.escape(building["building"])
+        + r'"\s*onmouseover="\$\(this\)\.addClass\(\'hover\'\);" onmouseout="\$\(this\)\.removeClass\(\'hover\'\);"\s*onclick="ajaxHandlerCall\(\'\?(.*?)\'\);'
+    )
     match = re.search(regex_building_detail, building_html)
     building_costs_url = match.group(1)
-    building_costs_url += 'backgroundView=city&currentCityId={}&templateView=buildingDetail&actionRequest={}&ajax=1'.format(city['id'], actionRequest)
+    building_costs_url += "backgroundView=city&currentCityId={}&templateView=buildingDetail&actionRequest={}&ajax=1".format(
+        city["id"], actionRequest
+    )
     building_costs_response = session.post(building_costs_url)
     building_costs = json.loads(building_costs_response, strict=False)
     html_costs = building_costs[1][1][1]
 
     # if the user has all the resource saving studies, we save that in the session data (one less request)
     sessionData = session.getSessionData()
-    if 'reduccion_inv_max' in sessionData:
+    if "reduccion_inv_max" in sessionData:
         costs_reduction = 14
     else:
         # get the studies
-        url = 'view=noViewChange&researchType=economy&backgroundView=city&currentCityId={}&templateView=researchAdvisor&actionRequest={}&ajax=1'.format(city['id'], actionRequest)
+        url = "view=noViewChange&researchType=economy&backgroundView=city&currentCityId={}&templateView=researchAdvisor&actionRequest={}&ajax=1".format(
+            city["id"], actionRequest
+        )
         rta = session.post(url)
         rta = json.loads(rta, strict=False)
-        studies = rta[2][1]['new_js_params']
+        studies = rta[2][1]["new_js_params"]
         studies = json.loads(studies, strict=False)
-        studies = studies['currResearchType']
+        studies = studies["currResearchType"]
 
         # look for resource saving studies
         costs_reduction = 0
         for study in studies:
-            if studies[study]['liClass'] != 'explored':
+            if studies[study]["liClass"] != "explored":
                 continue
-            link = studies[study]['aHref']
-            if '2020' in link:
+            link = studies[study]["aHref"]
+            if "2020" in link:
                 costs_reduction += 2
-            elif '2060' in link:
+            elif "2060" in link:
                 costs_reduction += 4
-            elif '2100' in link:
+            elif "2100" in link:
                 costs_reduction += 8
 
         # if the user has all the resource saving studies, save that in the session data
         if costs_reduction == 14:
-            sessionData['reduccion_inv_max'] = True
+            sessionData["reduccion_inv_max"] = True
             session.setSessionData(sessionData)
 
     # calculate cost reductions
     costs_reduction /= 100
     costs_reduction = 1 - costs_reduction
 
     # get buildings that reduce the cost of upgrades
     costs_reductions = getCostsReducers(city)
 
     # get the type of resources that this upgrade will cost (wood, marble, etc)
-    resources_types = re.findall(r'<th class="costs"><img src="(.*?)\.png"/></th>', html_costs)[:-1]
+    resources_types = re.findall(
+        r'<th class="costs"><img src="(.*?)\.png"/></th>', html_costs
+    )[:-1]
 
     # get the actual cost of each upgrade
-    matches = re.findall(r'<td class="level">\d+</td>(?:\s+<td class="costs">.*?</td>)+', html_costs)
+    matches = re.findall(
+        r'<td class="level">\d+</td>(?:\s+<td class="costs">.*?</td>)+', html_costs
+    )
 
     # calculate the cost of the entire upgrade, taking into account all the possible reductions
     final_costs = [0] * len(materials_names)
     levels_to_upgrade = 0
     for match in matches:
         lv = re.search(r'"level">(\d+)</td>', match).group(1)
         lv = int(lv)
@@ -242,42 +287,48 @@
             break
 
         levels_to_upgrade += 1
         # get the costs for the current level
         costs = re.findall(r'<td class="costs">([\d,\.]*)</td>', match)
 
         for i in range(len(costs)):
-            #get hash from CDN images to identify the resource type
+            # get hash from CDN images to identify the resource type
             resource_type = checkhash("https:" + resources_types[i] + ".png")
 
             for j in range(len(materials_names_tec)):
                 name = materials_names_tec[j]
                 if resource_type == name:
                     resource_index = j
                     break
 
             # get the cost of the current resource type
             cost = costs[i]
-            cost = cost.replace(',', '').replace('.', '')
-            cost = 0 if cost == '' else int(cost)
+            cost = cost.replace(",", "").replace(".", "")
+            cost = 0 if cost == "" else int(cost)
 
             # calculate all the reductions
             real_cost = Decimal(cost)
             # investigation reduction
             original_cost = Decimal(real_cost) / Decimal(costs_reduction)
             # special building reduction
-            real_cost -= Decimal(original_cost) * (Decimal(costs_reductions[resource_index]) / Decimal(100))
+            real_cost -= Decimal(original_cost) * (
+                Decimal(costs_reductions[resource_index]) / Decimal(100)
+            )
 
             final_costs[resource_index] += math.ceil(real_cost)
 
     if levels_to_upgrade < final_level - current_level:
-        print(_('This building only allows you to expand {:d} more levels').format(levels_to_upgrade))
-        msg = _('Expand {:d} levels? [Y/n]:').format(levels_to_upgrade)
-        rta = read(msg=msg, values=['Y', 'y', 'N', 'n', ''])
-        if rta.lower() == 'n':
+        print(
+            _("This building only allows you to expand {:d} more levels").format(
+                levels_to_upgrade
+            )
+        )
+        msg = _("Expand {:d} levels? [Y/n]:").format(levels_to_upgrade)
+        rta = read(msg=msg, values=["Y", "y", "N", "n", ""])
+        if rta.lower() == "n":
             return [-1, -1, -1, -1, -1]
 
     return final_costs
 
 
 def sendResourcesNeeded(session, destination_city_id, city_origins, missing_resources):
     """
@@ -285,15 +336,15 @@
     ----------
     session : ikabot.web.session.Session
     destination_city_id : int
     city_origins : dict
     missing_resources : dict[int, int]
     """
 
-    info = _('\nTransport resources to upload building\n')
+    info = _("\nTransport resources to upload building\n")
 
     try:
         routes = []
         html = session.get(city_url + destination_city_id)
         cityD = getCity(html)
         for i in range(len(materials_names)):
             missing = missing_resources[i]
@@ -301,24 +352,24 @@
                 continue
 
             # send the resources from each origin city
             for cityOrigin in city_origins[i]:
                 if missing == 0:
                     break
 
-                available = cityOrigin['recursos'][i]
+                available = cityOrigin["availableResources"][i]
                 send = min(available, missing)
                 missing -= send
                 toSend = [0] * len(materials_names)
                 toSend[i] = send
-                route = (cityOrigin, cityD, cityD['islandId'], *toSend)
+                route = (cityOrigin, cityD, cityD["islandId"], *toSend)
                 routes.append(route)
         executeRoutes(session, routes)
     except Exception as e:
-        msg = _('Error in:\n{}\nCause:\n{}').format(info, traceback.format_exc())
+        msg = _("Error in:\n{}\nCause:\n{}").format(info, traceback.format_exc())
         sendToBot(session, msg)
         # no s.logout() because this is a thread, not a process
 
 
 def chooseResourceProviders(session, cities_ids, cities, city_id, resource, missing):
     """
     Parameters
@@ -332,59 +383,68 @@
     """
     global sendResources
     sendResources = True
     global expand
     expand = True
 
     banner()
-    print(_('From what cities obtain {}?').format(materials_names[resource].lower()))
+    print(_("From what cities obtain {}?").format(materials_names[resource].lower()))
 
     tradegood_initials = [material_name[0] for material_name in materials_names]
-    maxName = max([len(cities[city]['name']) for city in cities if cities[city]['id'] != city_id])
+    maxName = max(
+        [len(cities[city]["name"]) for city in cities if cities[city]["id"] != city_id]
+    )
 
     origin_cities = []
     total_available = 0
     for cityId in cities_ids:
         if cityId == city_id:
             continue
 
         html = session.get(city_url + cityId)
         city = getCity(html)
 
-        available = city['recursos'][resource]
+        available = city["availableResources"][resource]
         if available == 0:
             continue
 
         # ask the user it this city should provide resources
-        tradegood_initial = tradegood_initials[int(cities[cityId]['tradegood'])]
-        pad = ' ' * (maxName - len(cities[cityId]['name']))
-        msg = '{}{} ({}): {} [Y/n]:'.format(pad, cities[cityId]['name'], tradegood_initial, addThousandSeparator(available))
-        choice = read(msg=msg, values=['Y', 'y', 'N', 'n', ''])
-        if choice.lower() == 'n':
+        tradegood_initial = tradegood_initials[int(cities[cityId]["tradegood"])]
+        pad = " " * (maxName - len(cities[cityId]["name"]))
+        is_producer = (int(cities[cityId]["tradegood"]) == int(resource))
+        msg = "{}{} ({}): {} [{}]:".format(
+            pad,
+            cities[cityId]["name"],
+            tradegood_initial,
+            addThousandSeparator(available),
+            ("y/N", "Y/n")[is_producer == True]
+        )
+        choice = read(msg=msg, values=["Y", "y", "N", "n", ""], default=("N", "Y")[is_producer == True])
+        if choice.lower() == "n":
             continue
 
         # if so, save the city and calculate the total amount resources to send
         total_available += available
         origin_cities.append(city)
         # if we have enough resources, return
         if total_available >= missing:
             return origin_cities
 
     # if we reach this part, there are not enough resources to expand the building
-    print(_('\nThere are not enough resources.'))
+    print(_("\nThere are not enough resources."))
 
     if len(origin_cities) > 0:
-        print(_('\nSend the resources anyway? [Y/n]'))
-        choice = read(values=['y', 'Y', 'n', 'N', ''])
-        if choice.lower() == 'n':
+        print(_("\nSend the resources anyway? [Y/n]"))
+        choice = read(values=["y", "Y", "n", "N", ""])
+        if choice.lower() == "n":
             sendResources = False
 
-    print(_('\nTry to expand the building anyway? [y/N]'))
-    choice = read(values=['y', 'Y', 'n', 'N', ''])
-    if choice.lower() == 'n' or choice == '':
+    print(_("\nTry to expand the building anyway? [y/N]"))
+    choice = read(values=["y", "Y", "n", "N", ""])
+    if choice.lower() == "n" or choice == "":
         expand = False
 
     return origin_cities
 
 
 def sendResourcesMenu(session, city_id, missing):
     """
@@ -398,32 +458,46 @@
     cities_ids, cities = getIdsOfCities(session)
     origins = {}
     # for each missing resource, choose providers
     for resource in range(len(missing)):
         if missing[resource] <= 0:
             continue
 
-        origin_cities = chooseResourceProviders(session, cities_ids, cities, city_id, resource, missing[resource])
+        origin_cities = chooseResourceProviders(
+            session, cities_ids, cities, city_id, resource, missing[resource]
+        )
         if sendResources is False and expand:
-            print(_('\nThe building will be expanded if possible.'))
+            print(_("\nThe building will be expanded if possible."))
             enter()
             return
         elif sendResources is False:
             return
         origins[resource] = origin_cities
 
     if expand:
-        print(_('\nThe resources will be sent and the building will be expanded if possible.'))
+        print(
+            _(
+                "\nThe resources will be sent and the building will be expanded if possible."
+            )
+        )
     else:
-        print(_('\nThe resources will be sent.'))
+        print(_("\nThe resources will be sent."))
 
     enter()
 
     # create a new thread to send the resources
-    thread = threading.Thread(target=sendResourcesNeeded, args=(session, city_id, origins, missing,))
+    thread = threading.Thread(
+        target=sendResourcesNeeded,
+        args=(
+            session,
+            city_id,
+            origins,
+            missing,
+        ),
+    )
     thread.start()
 
 
 def getBuildingToExpand(session, cityId):
     """
     Parameters
     ----------
@@ -435,67 +509,79 @@
     building : dict
     """
     html = session.get(city_url + cityId)
     city = getCity(html)
 
     banner()
     # show the buildings available to expand (ignore empty spaces)
-    print(_('Which building do you want to expand?\n'))
-    print(_('(0)\t\texit'))
-    buildings = [building for building in city['position'] if building['name'] != 'empty']
+    print(_("Which building do you want to expand?\n"))
+    print(_("(0)\t\texit"))
+    buildings = [
+        building for building in city["position"] if building["name"] != "empty"
+    ]
     for i in range(len(buildings)):
         building = buildings[i]
 
-        level = building['level']
+        level = building["level"]
+        
+        if building["isMaxLevel"] is True:
+                color = bcolors.BLACK
+        elif building["canUpgrade"] is True:
+                color = bcolors.GREEN
+        else:
+                color = bcolors.RED
         if level < 10:
-            level = ' ' + str(level)
+            level = " " + str(level)
         else:
             level = str(level)
-        if building['isBusy']:
-            level = level + '+'
-        print(_('({:d})\tlv:{}\t{}').format(i+1, level, building['name']))
-
+        if building["isBusy"]:
+            level = level + "+"
+        print(_("({:d})\tlv:{}\t{}{}{}").format(i + 1, level, color, building["name"],bcolors.ENDC ))
+         
     selected_building_id = read(min=0, max=len(buildings))
     if selected_building_id == 0:
         return None
 
     building = buildings[selected_building_id - 1]
 
-    current_level = int(building['level'])
+    current_level = int(building["level"])
     # if the building is being expanded, add 1 level
-    if building['isBusy']:
+    if building["isBusy"]:
         current_level += 1
 
     banner()
-    print(_('building:{}').format(building['name']))
-    print(_('current level:{}').format(current_level))
+    print(_("building:{}").format(building["name"]))
+    print(_("current level:{}").format(current_level))
 
-    final_level = read(min=current_level, msg=_('increase to level:'))
-    building['upgradeTo'] = final_level
+    final_level = read(min=current_level, msg=_("increase to level:"))
+    building["upgradeTo"] = final_level
 
     return building
+
+
 def checkhash(url):
     m = hashlib.md5()
     r = requests.get(url)
     for data in r.iter_content(8192):
         m.update(data)
         if m.hexdigest() == config.material_img_hash[0]:
-            material = 'wood'
+            material = "wood"
         elif m.hexdigest() == config.material_img_hash[1]:
-            material = 'wine'
+            material = "wine"
         elif m.hexdigest() == config.material_img_hash[2]:
-            material = 'marble'
+            material = "marble"
         elif m.hexdigest() == config.material_img_hash[3]:
-            material = 'glass'
+            material = "glass"
         elif m.hexdigest() == config.material_img_hash[4]:
-            material = 'sulfur'
+            material = "sulfur"
         else:
             continue
     return material
 
+
 def constructionList(session, event, stdin_fd, predetermined_input):
     """
     Parameters
     ----------
     session : ikabot.web.session.Session
     event : multiprocessing.Event
     stdin_fd: int
@@ -507,90 +593,94 @@
         global expand
         global sendResources
         expand = True
         sendResources = True
 
         banner()
         wait_resources = False
-        print(_('In which city do you want to expand a building?'))
+        print(_("In which city do you want to expand a building?"))
         city = chooseCity(session)
-        cityId = city['id']
+        cityId = city["id"]
         building = getBuildingToExpand(session, cityId)
         if building is None:
             event.set()
             return
 
-        current_level = building['level']
-        if building['isBusy']:
+        current_level = building["level"]
+        if building["isBusy"]:
             current_level += 1
-        final_level = building['upgradeTo']
+        final_level = building["upgradeTo"]
 
         # calculate the resources that are needed
-        resourcesNeeded = getResourcesNeeded(session, city, building, current_level, final_level)
+        resourcesNeeded = getResourcesNeeded(
+            session, city, building, current_level, final_level
+        )
         if -1 in resourcesNeeded:
             event.set()
             return
 
-        print('\nMaterials needed:')
+        print("\nMaterials needed:")
         for i, name in enumerate(materials_names):
             amount = resourcesNeeded[i]
             if amount == 0:
                 continue
-            print('- {}: {}'.format(name, addThousandSeparator(amount)))
-        print('')
+            print("- {}: {}".format(name, addThousandSeparator(amount)))
+        print("")
 
         # calculate the resources that are missing
         missing = [0] * len(materials_names)
         for i in range(len(materials_names)):
-            if city['recursos'][i] < resourcesNeeded[i]:
-                missing[i] = resourcesNeeded[i] - city['recursos'][i]
+            if city["availableResources"][i] < resourcesNeeded[i]:
+                missing[i] = resourcesNeeded[i] - city["availableResources"][i]
 
         # show missing resources to the user
         if sum(missing) > 0:
-            print(_('\nMissing:'))
+            print(_("\nMissing:"))
             for i in range(len(materials_names)):
                 if missing[i] == 0:
                     continue
                 name = materials_names[i].lower()
-                print(_('{} of {}').format(addThousandSeparator(missing[i]), name))
-            print('')
+                print(_("{} of {}").format(addThousandSeparator(missing[i]), name))
+            print("")
 
             # if the user wants, send the resources from the selected cities
-            print(_('Automatically transport resources? [Y/n]'))
-            rta = read(values=['y', 'Y', 'n', 'N', ''])
-            if rta.lower() == 'n':
-                print(_('Proceed anyway? [Y/n]'))
-                rta = read(values=['y', 'Y', 'n', 'N', ''])
-                if rta.lower() == 'n':
+            print(_("Automatically transport resources? [Y/n]"))
+            rta = read(values=["y", "Y", "n", "N", ""])
+            if rta.lower() == "n":
+                print(_("Proceed anyway? [Y/n]"))
+                rta = read(values=["y", "Y", "n", "N", ""])
+                if rta.lower() == "n":
                     event.set()
                     return
             else:
                 wait_resources = True
                 sendResourcesMenu(session, cityId, missing)
         else:
-            print(_('\nYou have enough materials'))
-            print(_('Proceed? [Y/n]'))
-            rta = read(values=['y', 'Y', 'n', 'N', ''])
-            if rta.lower() == 'n':
+            print(_("\nYou have enough materials"))
+            print(_("Proceed? [Y/n]"))
+            rta = read(values=["y", "Y", "n", "N", ""])
+            if rta.lower() == "n":
                 event.set()
                 return
     except KeyboardInterrupt:
         event.set()
         return
 
     set_child_mode(session)
     event.set()
 
-    info = _('\nUpgrade building\n')
-    info = info + _('City: {}\nBuilding: {}. From {:d}, to {:d}').format(city['cityName'], building['name'], current_level, final_level)
+    info = _("\nUpgrade building\n")
+    info = info + _("City: {}\nBuilding: {}. From {:d}, to {:d}").format(
+        city["cityName"], building["name"], current_level, final_level
+    )
 
     setInfoSignal(session, info)
     try:
         if expand:
             expandBuilding(session, cityId, building, wait_resources)
         elif thread:
             thread.join()
     except Exception as e:
-        msg = _('Error in:\n{}\nCause:\n{}').format(info, traceback.format_exc())
+        msg = _("Error in:\n{}\nCause:\n{}").format(info, traceback.format_exc())
         sendToBot(session, msg)
     finally:
         session.logout()
```

### Comparing `ikabot-6.6.4/ikabot/function/decaptchaConf.py` & `ikabot-7.0.1/ikabot/function/decaptchaConf.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,42 @@
 #! /usr/bin/env python3
 # -*- coding: utf-8 -*-
+import base64
 import gettext
 import sys
-import requests
-import base64
 import time
-from ikabot.helpers.pedirInfo import read, enter
-from ikabot.helpers.gui import *
+
+import requests
+
 from ikabot.config import *
-from ikabot.helpers.process import updateProcessList, run
 from ikabot.helpers.botComm import *
+from ikabot.helpers.gui import *
+from ikabot.helpers.pedirInfo import enter, read
+from ikabot.helpers.process import run, updateProcessList
 
-t = gettext.translation('killTasks', localedir, languages=languages, fallback=True)
+t = gettext.translation("killTasks", localedir, languages=languages, fallback=True)
 _ = t.gettext
 
 decaptcha_test_pictures = [
-    {'ground_truth': 'WURY5G', 'picture': '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'},
-    {'ground_truth': 'XEPAMVW', 'picture': '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'},
-    {'ground_truth': 'T2YE3LV', 'picture': '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'},
-    {'ground_truth': 'GPJPYB', 'picture': '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'},
+    {
+        "ground_truth": "WURY5G",
+        "picture": "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",
+    },
+    {
+        "ground_truth": "XEPAMVW",
+        "picture": "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",
+    },
+    {
+        "ground_truth": "T2YE3LV",
+        "picture": "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",
+    },
+    {
+        "ground_truth": "GPJPYB",
+        "picture": "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",
+    },
 ]
 
 
 def decaptchaConf(session, event, stdin_fd, predetermined_input):
     """
     Parameters
     ----------
@@ -33,155 +47,204 @@
     """
     sys.stdin = os.fdopen(stdin_fd)
     config.predetermined_input = predetermined_input
     banner()
     try:
         session_data = session.getSessionData()
 
-        if 'decaptcha' not in session_data:
-            session_data['decaptcha'] = {'name': 'default', 'endpoint': 'default', 'relevant_data': {}}
+        if "decaptcha" not in session_data:
+            session_data["decaptcha"] = {
+                "name": "default",
+                "endpoint": "default",
+                "relevant_data": {},
+            }
             session.setSessionData(session_data)
 
-        if session_data['decaptcha']['name'] == 'default':
-            print('You are currently using the default decaptcha service')
-        elif session_data['decaptcha']['name'] == 'custom':
-            print('You are currently using your custom decaptcha service')
-            print('Endpoint : {}'.format(session_data['decaptcha']['endpoint']))
-        elif session_data['decaptcha']['name'] == '9kw.eu':
-            print('You are currently using 9kw.eu as your decaptcha service')
-            print("API key : {}".format(session_data['decaptcha']['relevant_data']['apiKey']))
-        elif session_data['decaptcha']['name'] == 'telegram':
-            print('You are currently using Telegram as your decaptcha service')
-            print("Telegram ID : {}".format(session_data['shared']['telegram']['chatId']))
+        if session_data["decaptcha"]["name"] == "default":
+            print("You are currently using the default decaptcha service")
+        elif session_data["decaptcha"]["name"] == "custom":
+            print("You are currently using your custom decaptcha service")
+            print("Endpoint : {}".format(session_data["decaptcha"]["endpoint"]))
+        elif session_data["decaptcha"]["name"] == "9kw.eu":
+            print("You are currently using 9kw.eu as your decaptcha service")
+            print(
+                "API key : {}".format(
+                    session_data["decaptcha"]["relevant_data"]["apiKey"]
+                )
+            )
+        elif session_data["decaptcha"]["name"] == "telegram":
+            print("You are currently using Telegram as your decaptcha service")
+            print(
+                "Telegram ID : {}".format(session_data["shared"]["telegram"]["chatId"])
+            )
         print()
-        print('(0) Exit')
-        print('(1) Default')
-        print('(2) Custom')
-        print('(3) 9kw.eu')
-        print('(4) Telegram')
+        print("(0) Exit")
+        print("(1) Default")
+        print("(2) Custom")
+        print("(3) 9kw.eu")
+        print("(4) Telegram")
 
         action = read(min=0, max=4, digit=True)
 
         if action == 0:
             event.set()
             return
 
         elif action == 1:
             banner()
-            session_data['decaptcha'] = {'name': 'default', 'endpoint': 'default', 'relevant_data': {}}
+            session_data["decaptcha"] = {
+                "name": "default",
+                "endpoint": "default",
+                "relevant_data": {},
+            }
             session.setSessionData(session_data)
-            print('Default decaptcha service set as decaptcha service!')
+            print("Default decaptcha service set as decaptcha service!")
             enter()
             event.set()
             return
 
         elif action == 2:
-            while(True):
+            while True:
                 banner()
-                endpoint = read(msg='Enter your custom endpoint : ')
-                if 'http' not in endpoint:
-                    print('Invalid endpoint!')
+                endpoint = read(msg="Enter your custom endpoint : ")
+                if "http" not in endpoint:
+                    print("Invalid endpoint!")
                     enter()
                     event.set()
                     return
-                session_data['decaptcha']['name'] = 'custom'
-                session_data['decaptcha']['endpoint'] = endpoint
-                print('Endpoint {} set! Remember, the picture will be sent via a POST request under the `upload_file` parameter'.format(endpoint))
-                print('Do you want to test this newly-set custom endpoint?(y|n)')
-                test_bool = read(values=['y', 'Y', 'n', 'N'])
-                if (test_bool.lower() == 'n'):
+                session_data["decaptcha"]["name"] = "custom"
+                session_data["decaptcha"]["endpoint"] = endpoint
+                print(
+                    "Endpoint {} set! Remember, the picture will be sent via a POST request under the `upload_file` parameter".format(
+                        endpoint
+                    )
+                )
+                print("Do you want to test this newly-set custom endpoint?(y|n)")
+                test_bool = read(values=["y", "Y", "n", "N"])
+                if test_bool.lower() == "n":
                     session.setSessionData(session_data)
                     event.set()
                     return
                 for test in decaptcha_test_pictures:
-                    if testCustomDecaptcha(test['ground_truth'], base64.b64decode(test['picture']), endpoint):
+                    if testCustomDecaptcha(
+                        test["ground_truth"],
+                        base64.b64decode(test["picture"]),
+                        endpoint,
+                    ):
                         session.setSessionData(session_data)
-                        print('Custom decaptcha passed at least one test, good enough!')
+                        print("Custom decaptcha passed at least one test, good enough!")
                         enter()
                         event.set()
                         return
-                print('All tests failed. Do you wish to set the endpoint again?')
-                input = read(values=['y', 'Y', 'n', 'N'])
-                if input.lower() == 'y':
+                print("All tests failed. Do you wish to set the endpoint again?")
+                input = read(values=["y", "Y", "n", "N"])
+                if input.lower() == "y":
                     continue
                 else:
                     event.set()
                     return
 
         elif action == 3:
             banner()
-            apiKey_9kw = read(msg='Enter your 9kw.eu API key : ')
-            response = requests.get("https://www.9kw.eu/index.cgi?action=usercaptchaguthaben&apikey={}".format(apiKey_9kw)).text
-            if 'API key not found' in response:
+            apiKey_9kw = read(msg="Enter your 9kw.eu API key : ")
+            response = requests.get(
+                "https://www.9kw.eu/index.cgi?action=usercaptchaguthaben&apikey={}".format(
+                    apiKey_9kw
+                )
+            ).text
+            if "API key not found" in response:
                 print("{}Failure!{} Wrong API key!".format(bcolors.RED, bcolors.ENDC))
                 enter()
                 event.set()
                 return
             else:
-                session_data['decaptcha']['name'] = '9kw.eu'
-                session_data['decaptcha']['endpoint'] = 'https://www.9kw.eu/index.cgi'
-                session_data['decaptcha']['relevant_data'] = {'apiKey': apiKey_9kw}
-                print("{}Success!{} You currently have {} credits".format(bcolors.GREEN, bcolors.ENDC, response))
+                session_data["decaptcha"]["name"] = "9kw.eu"
+                session_data["decaptcha"]["endpoint"] = "https://www.9kw.eu/index.cgi"
+                session_data["decaptcha"]["relevant_data"] = {"apiKey": apiKey_9kw}
+                print(
+                    "{}Success!{} You currently have {} credits".format(
+                        bcolors.GREEN, bcolors.ENDC, response
+                    )
+                )
                 enter()
                 session.setSessionData(session_data)
                 event.set()
                 return
 
         elif action == 4:
             banner()
             if checkTelegramData(session) is False:
-                print('Please first set the Telegram data')
+                print("Please first set the Telegram data")
                 enter()
                 event.set()
                 return
-            session_data['decaptcha']['name'] = 'telegram'
-            print('Do you wish to do a test?(y|n)')
-            test = read(values=['y', 'Y', 'n', 'N'])
-            if test.lower() == 'y':
-                print('A captcha has been sent to you over Telegram. Please open the picture fully and respond on Telegram')
-                sendToBot(session, 'Please resolve the captcha', Photo=base64.b64decode(decaptcha_test_pictures[0]['picture']))
+            session_data["decaptcha"]["name"] = "telegram"
+            print("Do you wish to do a test?(y|n)")
+            test = read(values=["y", "Y", "n", "N"])
+            if test.lower() == "y":
+                print(
+                    "A captcha has been sent to you over Telegram. Please open the picture fully and respond on Telegram"
+                )
+                sendToBot(
+                    session,
+                    "Please resolve the captcha",
+                    Photo=base64.b64decode(decaptcha_test_pictures[0]["picture"]),
+                )
                 captcha_time = time.time()
-                while(True):
+                while True:
                     response = getUserResponse(session, fullResponse=True)
                     if response == []:
                         time.sleep(5)
                         continue
                     response = response[-1]
-                    if response['date'] < captcha_time:
+                    if response["date"] < captcha_time:
                         time.sleep(5)
                         continue
                     else:
-                        captcha = response['text']
+                        captcha = response["text"]
                         break
                     time.sleep(5)
-                if captcha.lower() == decaptcha_test_pictures[0]['ground_truth'].lower():
-                    print('{}Success!{} Captcha is correct!'.format(bcolors.GREEN, bcolors.ENDC))
+                if (
+                    captcha.lower()
+                    == decaptcha_test_pictures[0]["ground_truth"].lower()
+                ):
+                    print(
+                        "{}Success!{} Captcha is correct!".format(
+                            bcolors.GREEN, bcolors.ENDC
+                        )
+                    )
                     enter()
                     session.setSessionData(session_data)
                     event.set()
                     return
                 else:
-                    print('{}Failure!{} Captcha is incorrect, try again!'.format(bcolors.GREEN, bcolors.ENDC))
+                    print(
+                        "{}Failure!{} Captcha is incorrect, try again!".format(
+                            bcolors.GREEN, bcolors.ENDC
+                        )
+                    )
                     enter()
                     event.set()
                     return
             else:
-                print('You will now recieve the piracy captcha over Telegram!')
+                print("You will now recieve the piracy captcha over Telegram!")
                 session.setSessionData(session_data)
                 enter()
                 event.set()
                 return
     except KeyboardInterrupt:
         event.set()
         return
 
 
 def testCustomDecaptcha(ground_truth, picture, address):
 
     try:
-        files = {'upload_file': picture}
-        captcha = requests.post('{0}'.format(address), files=files).text
-        if captcha.lower() != ground_truth.lower():  # Ikariam's captcha is not case-sensitive
+        files = {"upload_file": picture}
+        captcha = requests.post("{0}".format(address), files=files).text
+        if (
+            captcha.lower() != ground_truth.lower()
+        ):  # Ikariam's captcha is not case-sensitive
             return False
         return True
     except Exception:
         return False
```

### Comparing `ikabot-6.6.4/ikabot/function/distributeResources.py` & `ikabot-7.0.1/ikabot/function/distributeResources.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 #! /usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 import gettext
 import traceback
+
 from ikabot.config import *
 from ikabot.helpers.botComm import *
-from ikabot.helpers.pedirInfo import *
-from ikabot.helpers.signals import setInfoSignal
 from ikabot.helpers.getJson import getCity
+from ikabot.helpers.gui import banner
+from ikabot.helpers.pedirInfo import *
 from ikabot.helpers.planRoutes import executeRoutes
+from ikabot.helpers.process import set_child_mode
 from ikabot.helpers.resources import *
+from ikabot.helpers.signals import setInfoSignal
 from ikabot.helpers.varios import addThousandSeparator
-from ikabot.helpers.process import set_child_mode
-from ikabot.helpers.gui import banner
 
-t = gettext.translation('distributeResources', localedir, languages=languages, fallback=True)
+t = gettext.translation(
+    "distributeResources", localedir, languages=languages, fallback=True
+)
 _ = t.gettext
 
 
 def distributeResources(session, event, stdin_fd, predetermined_input):
     """
     Parameters
     ----------
@@ -28,242 +31,349 @@
     predetermined_input : multiprocessing.managers.SyncManager.list
     """
     sys.stdin = os.fdopen(stdin_fd)
     config.predetermined_input = predetermined_input
     try:
         banner()
 
-        print(_('What resource do you want to distribute?'))
-        print(_('(0) Exit'))
+        print(_("What resource do you want to distribute?"))
+        print(_("(0) Exit"))
         for i in range(len(materials_names)):
-            print('({:d}) {}'.format(i+1, materials_names[i]))
+            print("({:d}) {}".format(i + 1, materials_names[i]))
         resource = read(min=0, max=5)
         if resource == 0:
             event.set()  # give main process control before exiting
             return
         resource -= 1
 
         if resource == 0:
             evenly = True
         else:
-            print('\nHow do you want to distribute the resources?')
-            print('1) From cities that produce them to cities that do not')
-            print('2) Distribute them evenly among all cities')
+            print("\nHow do you want to distribute the resources?")
+            print("1) From cities that produce them to cities that do not")
+            print("2) Distribute them evenly among all cities")
             type_distribution = read(min=1, max=2)
             evenly = type_distribution == 2
 
+        (cities_ids, cities) = getIdsOfCities(session)
+        choice = None
+        ignored_cities = []
+        while True:
+            banner()
+            displayed_string = (
+                f'(currently ignoring: {", ".join(ignored_cities)})'
+                if ignored_cities
+                else ""
+            )
+            print(f"Select cities to ignore. {displayed_string}")
+            print("0) Continue")
+            choice_to_cityid_map = []
+            for i, city in enumerate(cities.values()):
+                choice_to_cityid_map.append(city["id"])
+                print(f'{i + 1}) {city["name"]} - {materials_names[city["tradegood"]]}')
+            choice = read(min=0, max=len(cities_ids))
+            if choice == 0:
+                break
+            city_id = choice_to_cityid_map[choice - 1]
+            cities_ids = list(filter(lambda x: x != str(city_id), cities_ids))
+            ignored_cities.append(cities[str(city_id)]["name"])
+            del cities[str(city_id)]
+
         if evenly:
-            routes = distribute_evenly(session, resource)
+            routes = distribute_evenly(session, resource, cities_ids, cities)
         else:
-            routes = distribute_unevenly(session, resource)
+            routes = distribute_unevenly(session, resource, cities_ids, cities)
 
         if routes is None:
             event.set()
             return
 
         banner()
-        print(_('\nThe following shipments will be made:\n'))
+        print(_("\nThe following shipments will be made:\n"))
         for route in routes:
-            print('{} -> {} : {} {}'.format(route[0]['name'], route[1]['name'], route[resource+3], materials_names[resource]))  # displays all routes to be executed in console
-
-        print(_('\nProceed? [Y/n]'))
-        rta = read(values=['y', 'Y', 'n', 'N', ''])
-        if rta.lower() == 'n':
+            print(
+                "{} -> {} : {} {}".format(
+                    route[0]["name"],
+                    route[1]["name"],
+                    route[resource + 3],
+                    materials_names[resource],
+                )
+            )  # displays all routes to be executed in console
+
+        print(_("\nProceed? [Y/n]"))
+        rta = read(values=["y", "Y", "n", "N", ""])
+        if rta.lower() == "n":
             event.set()
             return
 
     except KeyboardInterrupt:
         event.set()
         return
 
     set_child_mode(session)
     event.set()  # this is where we give back control to main process
 
-    info = _('\nDistribute {}\n').format(materials_names[resource])
+    info = _("\nDistribute {}\n").format(materials_names[resource])
     setInfoSignal(session, info)
 
     try:
         executeRoutes(session, routes)  # plan trips for all the routes
     except Exception as e:
-        msg = _('Error in:\n{}\nCause:\n{}').format(info, traceback.format_exc())
+        msg = _("Error in:\n{}\nCause:\n{}").format(info, traceback.format_exc())
         sendToBot(session, msg)  # sends message to telegram bot
     finally:
         session.logout()
 
 
-def distribute_evenly(session, resource_type):
+def distribute_evenly(session, resource_type, cities_ids, cities):
     """
     Parameters
     ----------
     session : ikabot.web.session.Session
     resource_type : int
     """
     resourceTotal = 0
-    (cityIDs, cities) = getIdsOfCities(session)
 
     originCities = {}
     destinationCities = {}
     allCities = {}
-    for cityID in cityIDs:
+    for cityID in cities_ids:
 
-        html = session.get(city_url + cityID)  # load html from the get request for that particular city
+        html = session.get(
+            city_url + cityID
+        )  # load html from the get request for that particular city
         city = getCity(html)  # convert the html to a city object
 
-        resourceTotal += city['recursos'][resource_type]  # the cities resources are added to the total
+        resourceTotal += city["availableResources"][
+            resource_type
+        ]  # the cities resources are added to the total
         allCities[cityID] = city  # adds the city to all cities
 
     # if a city doesn't have enough storage to fit resourceAverage
     # ikabot will send enough resources to fill the store to the max
     # then, resourceAverage will be recalculated
     resourceAverage = resourceTotal // len(allCities)
     while True:
 
         len_prev = len(destinationCities)
         for cityID in allCities:
             if cityID in destinationCities:
                 continue
-            freeStorage = allCities[cityID]['freeSpaceForResources'][resource_type]
-            storage = allCities[cityID]['storageCapacity']
+            freeStorage = allCities[cityID]["freeSpaceForResources"][resource_type]
+            storage = allCities[cityID]["storageCapacity"]
             if storage < resourceAverage:
                 destinationCities[cityID] = freeStorage
                 resourceTotal -= storage
 
         resourceAverage = resourceTotal // (len(allCities) - len(destinationCities))
 
         if len_prev == len(destinationCities):
             for cityID in allCities:
                 if cityID in destinationCities:
                     continue
-                if allCities[cityID]['recursos'][resource_type] > resourceAverage:
-                    originCities[cityID] = allCities[cityID]['recursos'][resource_type] - resourceAverage
+                if (
+                    allCities[cityID]["availableResources"][resource_type]
+                    > resourceAverage
+                ):
+                    originCities[cityID] = (
+                        allCities[cityID]["availableResources"][resource_type]
+                        - resourceAverage
+                    )
                 else:
-                    destinationCities[cityID] = resourceAverage - allCities[cityID]['recursos'][resource_type]
+                    destinationCities[cityID] = (
+                        resourceAverage
+                        - allCities[cityID]["availableResources"][resource_type]
+                    )
             break
 
-    originCities = {k: v for k, v in sorted(originCities.items(), key=lambda item: item[1], reverse=True)}  # sort origin cities in descending order
-    destinationCities = {k: v for k, v in sorted(destinationCities.items(), key=lambda item: item[1])}  # sort destination cities in ascending order
+    originCities = {
+        k: v
+        for k, v in sorted(originCities.items(), key=lambda item: item[1], reverse=True)
+    }  # sort origin cities in descending order
+    destinationCities = {
+        k: v for k, v in sorted(destinationCities.items(), key=lambda item: item[1])
+    }  # sort destination cities in ascending order
 
     routes = []
 
     for originCityID in originCities:  # iterate through all origin city ids
 
-        for destinationCityID in destinationCities:  # iterate through all destination city ids
-            if originCities[originCityID] == 0 or destinationCities[destinationCityID] == 0:
+        for (
+            destinationCityID
+        ) in destinationCities:  # iterate through all destination city ids
+            if (
+                originCities[originCityID] == 0
+                or destinationCities[destinationCityID] == 0
+            ):
                 continue
 
-            if originCities[originCityID] > destinationCities[destinationCityID]:  # if there's more resources above average in the origin city than resources below average in the destination city (origin city needs to have a surplus and destination city needs to have a deficit of resources for a route to be considered)
-                toSend = destinationCities[destinationCityID]  # number of resources to send is the number of resources below average in destination city
+            if (
+                originCities[originCityID] > destinationCities[destinationCityID]
+            ):  # if there's more resources above average in the origin city than resources below average in the destination city (origin city needs to have a surplus and destination city needs to have a deficit of resources for a route to be considered)
+                toSend = destinationCities[
+                    destinationCityID
+                ]  # number of resources to send is the number of resources below average in destination city
             else:
-                toSend = originCities[originCityID]  # send the amount of resources above average of the current origin city
+                toSend = originCities[
+                    originCityID
+                ]  # send the amount of resources above average of the current origin city
 
             if toSend == 0:
                 continue
 
             toSendArr = [0] * len(materials_names)
             toSendArr[resource_type] = toSend
-            route = (allCities[originCityID], allCities[destinationCityID], allCities[destinationCityID]['islandId'], *toSendArr)
+            route = (
+                allCities[originCityID],
+                allCities[destinationCityID],
+                allCities[destinationCityID]["islandId"],
+                *toSendArr,
+            )
             routes.append(route)
 
             # ROUTE BLOCK
             if originCities[originCityID] > destinationCities[destinationCityID]:
-                originCities[originCityID] -= destinationCities[destinationCityID]  # remove the sent amount from the origin city's surplus
-                destinationCities[destinationCityID] = 0  # set the amount of resources below average in destination city to 0
+                originCities[originCityID] -= destinationCities[
+                    destinationCityID
+                ]  # remove the sent amount from the origin city's surplus
+                destinationCities[destinationCityID] = (
+                    0  # set the amount of resources below average in destination city to 0
+                )
             else:
-                destinationCities[destinationCityID] -= originCities[originCityID]  # remove the sent amount from the amount of resources below average in current destination city
-                originCities[originCityID] = 0  # set the amount of resources above average in origin city to 0
+                destinationCities[destinationCityID] -= originCities[
+                    originCityID
+                ]  # remove the sent amount from the amount of resources below average in current destination city
+                originCities[originCityID] = (
+                    0  # set the amount of resources above average in origin city to 0
+                )
 
     return routes
 
 
-def distribute_unevenly(session, resource_type):
+def distribute_unevenly(session, resource_type, cities_ids, cities):
     """
     Parameters
     ----------
     session : ikabot.web.session.Session
     resource_type : int
     """
     total_available_resources_from_all_cities = 0
-    (cities_ids, cities) = getIdsOfCities(session)
     origin_cities = {}
     destination_cities = {}
     for destination_city_id in cities_ids:
-        is_city_mining_this_resource = cities[destination_city_id]['tradegood'] == str(resource_type)
+        is_city_mining_this_resource = (
+            cities[destination_city_id]["tradegood"] == resource_type
+        )
         if is_city_mining_this_resource:
             html = session.get(city_url + destination_city_id)
             city = getCity(html)
             if resource_type == 1:  # wine
-                city['available_amount_of_resource'] = city['recursos'][resource_type] - city['consumo'] - 1
+                city["available_amount_of_resource"] = (
+                    city["availableResources"][resource_type]
+                    - city["wineConsumptionPerHour"]
+                    - 1
+                )
             else:
-                city['available_amount_of_resource'] = city['recursos'][resource_type]
-            if city['available_amount_of_resource'] < 0:
-                city['available_amount_of_resource'] = 0
-            total_available_resources_from_all_cities += city['available_amount_of_resource']
+                city["available_amount_of_resource"] = city["availableResources"][
+                    resource_type
+                ]
+            if city["available_amount_of_resource"] < 0:
+                city["available_amount_of_resource"] = 0
+            total_available_resources_from_all_cities += city[
+                "available_amount_of_resource"
+            ]
             origin_cities[destination_city_id] = city
         else:
             html = session.get(city_url + destination_city_id)
             city = getCity(html)
-            city['free_storage_for_resource'] = city['freeSpaceForResources'][resource_type]
-            if city['free_storage_for_resource'] > 0:
+            city["free_storage_for_resource"] = city["freeSpaceForResources"][
+                resource_type
+            ]
+            if city["free_storage_for_resource"] > 0:
                 destination_cities[destination_city_id] = city
 
     if total_available_resources_from_all_cities <= 0:
-        print(_('\nThere are no resources to send.'))
+        print(_("\nThere are no resources to send."))
         enter()
         return None
     if len(destination_cities) == 0:
-        print(_('\nThere is no space available to send resources.'))
+        print(_("\nThere is no space available to send resources."))
         enter()
         return None
 
-    remaining_resources_to_be_sent_to_each_city = total_available_resources_from_all_cities // len(destination_cities)
-    free_storage_available_per_city = [destination_cities[city]['free_storage_for_resource'] for city in destination_cities]
+    remaining_resources_to_be_sent_to_each_city = (
+        total_available_resources_from_all_cities // len(destination_cities)
+    )
+    free_storage_available_per_city = [
+        destination_cities[city]["free_storage_for_resource"]
+        for city in destination_cities
+    ]
     total_free_storage_available_in_all_cities = sum(free_storage_available_per_city)
-    remaining_resources_to_send = min(total_available_resources_from_all_cities, total_free_storage_available_in_all_cities)
+    remaining_resources_to_send = min(
+        total_available_resources_from_all_cities,
+        total_free_storage_available_in_all_cities,
+    )
     toSend = {}
 
     while remaining_resources_to_send > 0:
         len_prev = len(toSend)
         for city_id in destination_cities:
             city = destination_cities[city_id]
-            if city_id not in toSend and city['free_storage_for_resource'] < remaining_resources_to_be_sent_to_each_city:
-                toSend[city_id] = city['free_storage_for_resource']
-                remaining_resources_to_send -= city['free_storage_for_resource']
+            if (
+                city_id not in toSend
+                and city["free_storage_for_resource"]
+                < remaining_resources_to_be_sent_to_each_city
+            ):
+                toSend[city_id] = city["free_storage_for_resource"]
+                remaining_resources_to_send -= city["free_storage_for_resource"]
 
         if len(toSend) == len_prev:
             for city_id in destination_cities:
                 if city_id not in toSend:
                     toSend[city_id] = remaining_resources_to_be_sent_to_each_city
             break
 
-        free_storage_available_per_city = [destination_cities[city]['free_storage_for_resource'] for city in destination_cities if city not in toSend]
+        free_storage_available_per_city = [
+            destination_cities[city]["free_storage_for_resource"]
+            for city in destination_cities
+            if city not in toSend
+        ]
         if len(free_storage_available_per_city) == 0:
             break
-        total_free_storage_available_in_all_cities = sum(free_storage_available_per_city)
-        remaining_resources_to_send = min(remaining_resources_to_send, total_free_storage_available_in_all_cities)
-        remaining_resources_to_be_sent_to_each_city = remaining_resources_to_send // len(free_storage_available_per_city)
+        total_free_storage_available_in_all_cities = sum(
+            free_storage_available_per_city
+        )
+        remaining_resources_to_send = min(
+            remaining_resources_to_send, total_free_storage_available_in_all_cities
+        )
+        remaining_resources_to_be_sent_to_each_city = (
+            remaining_resources_to_send // len(free_storage_available_per_city)
+        )
 
     routes = []
     for destination_city_id in destination_cities:
         destination_city = destination_cities[destination_city_id]
-        island_id = destination_city['islandId']
+        island_id = destination_city["islandId"]
         missing_resources = toSend[destination_city_id]
         for origin_city_id in origin_cities:
             if missing_resources == 0:
                 break
 
             origin_city = origin_cities[origin_city_id]
-            resources_available_in_this_city = origin_city['available_amount_of_resource']
+            resources_available_in_this_city = origin_city[
+                "available_amount_of_resource"
+            ]
             for route in routes:
                 origin = route[0]
                 resource = route[resource_type + 3]
-                if origin['id'] == origin_city_id:
+                if origin["id"] == origin_city_id:
                     resources_available_in_this_city -= resource
 
             send_this_round = min(missing_resources, resources_available_in_this_city)
-            available = destination_city['free_storage_for_resource']
+            available = destination_city["free_storage_for_resource"]
             if available == 0 or send_this_round == 0:
                 continue
 
             if available < send_this_round:
                 missing_resources = 0
                 send_this_round = available
             else:
```

### Comparing `ikabot-6.6.4/ikabot/function/dumpWorld.py` & `ikabot-7.0.1/ikabot/function/dumpWorld.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,41 +1,42 @@
 #! /usr/bin/env python3
 # -*- coding: utf-8 -*-
 
-import time
+import ast
 import gettext
-import traceback
-import sys
-import threading
-import json
 import gzip
-import re
+import json
 import os
-import ast
-import ikabot.config as config
+import re
+import sys
+import threading
+import time
+import traceback
 from pathlib import Path
+
+import ikabot.config as config
 from ikabot.config import *
-from ikabot.helpers.gui import enter, banner, bcolors
-from ikabot.helpers.varios import wait, getDateTime
 from ikabot.helpers.botComm import sendToBot
-from ikabot.helpers.signals import setInfoSignal
-from ikabot.helpers.pedirInfo import read
 from ikabot.helpers.getJson import getIsland
+from ikabot.helpers.gui import banner, bcolors, enter
+from ikabot.helpers.pedirInfo import read
 from ikabot.helpers.process import set_child_mode
+from ikabot.helpers.signals import setInfoSignal
+from ikabot.helpers.varios import getDateTime, wait
 
-t = gettext.translation('dumpWorld', localedir, languages=languages, fallback=True)
+t = gettext.translation("dumpWorld", localedir, languages=languages, fallback=True)
 _ = t.gettext
 
-LINE_UP = '\033[1A'
-LINE_CLEAR = '\x1b[2K'
+LINE_UP = "\033[1A"
+LINE_CLEAR = "\x1b[2K"
 #              status, history, start_time
 stop_updating = threading.Event()
 lock = threading.Lock()
-shared_data = ['','',0,stop_updating, lock]
-home = 'USERPROFILE' if isWindows else 'HOME'
+shared_data = ["", "", 0, stop_updating, lock]
+home = "USERPROFILE" if isWindows else "HOME"
 selected_islands = set()
 
 
 def dumpWorld(session, event, stdin_fd, predetermined_input):
     """
     Parameters
     ----------
@@ -45,343 +46,557 @@
     predetermined_input : multiprocessing.managers.SyncManager.list
     """
     sys.stdin = os.fdopen(stdin_fd)
     config.predetermined_input = predetermined_input
 
     try:
         banner()
-        if os.path.exists(os.getenv(home) + '/ikabot_world_dumps'):
-            print('1) Create new dump')
-            print('2) Load existing dump')
+        if os.path.exists(os.getenv(home) + "/ikabot_world_dumps"):
+            print("1) Create new dump")
+            print("2) Load existing dump")
             choice = read(min=1, max=2, digit=True)
             if choice == 2:
                 view_dump(session, event)
                 event.set()
                 return
         banner()
-        print('{}⚠️ BEWARE - THE RESULTING DUMP CONTAINS ACCOUNT IDENTIFYING INFORMATION ⚠️{}\n'.format(bcolors.WARNING, bcolors.ENDC))
-        print('This action will take a couple of hours to complete. Are you sure you want to initiate a data dump now? (Y|N)')
-        choice = read(values=['y', 'Y', 'n', 'N'])
-        if (choice in ['n','N']):
+        print(
+            "{}⚠️ BEWARE - THE RESULTING DUMP CONTAINS ACCOUNT IDENTIFYING INFORMATION ⚠️{}\n".format(
+                bcolors.WARNING, bcolors.ENDC
+            )
+        )
+        print(
+            "This action will take a couple of hours to complete. Are you sure you want to initiate a data dump now? (Y|N)"
+        )
+        choice = read(values=["y", "Y", "n", "N"])
+        if choice in ["n", "N"]:
             event.set()
             return
-        print('Type in the waiting time between each request in miliseconds (default = 1500): ')
+        print(
+            "Type in the waiting time between each request in miliseconds (default = 1500): "
+        )
         choice = read(min=0, max=10000, digit=True, default=1500)
-        waiting_time = int(choice)/1000
-        print('Start scan form island id (0 to start from beginning) (default = 0): ')
-        choice = read(min=0, digit=True, default=0)
-        start_id = int(choice)
-        print('Do you want only shallow data about the islands? If yes you will not be able to search the dump by player names but the dump will be quick. (Y|N): ')
-        choice = read(values=['y', 'Y', 'n', 'N'])
-        shallow = choice
-        
-        thread = threading.Thread(target=update_terminal, args=(shared_data,))
+        waiting_time = int(choice) / 1000
+        print(
+            "Do you want only shallow data about the islands? If yes you will not be able to search the dump by player names but the dump will be quick. (Y|N): "
+        )
+        choice = read(values=["y", "Y", "n", "N"])
+        shallow = choice in ["y", "Y"]
+        coords = None
+        radius = None
+        non_empty_islands = False
+        if not shallow:
+            print("Do you want to only dump a part of the map? (Y|N)")
+            choice = read(values=["y", "Y", "n", "N"])
+            if choice in ["y", "Y"]:
+                print('Type in a center point (x,y): (type "skip" to skip this step)')
+                input = read()
+                if input.strip().lower() != "skip":
+                    coords = input.replace("(", "").replace(")", "").split(",")
+                    coords = (int(coords[0]), int(coords[1]))
+                    print(
+                        "Type in a max distance from the center point: (default = 15)"
+                    )
+                    radius = read(min=0, max=200, digit=True, default=15)
+                print("Do you want to only dump islands with at least 1 town? (Y|N)")
+                choice = read(values=["y", "Y", "n", "N"])
+                non_empty_islands = choice in ["y", "Y"]
+
+        thread = threading.Thread(target=update_terminal, args=(shared_data,), daemon=True)
         thread.start()
         set_child_mode(session)
-        info = _('\nDumped world data\n')
+        info = _("\nDumped world data\n")
         setInfoSignal(session, info)
 
-        dump_path = do_it(session, waiting_time, start_id, shallow)
+        dump_path = do_it(
+            session, waiting_time, coords, radius, shallow, non_empty_islands
+        )
 
         shared_data[3].set()
         shared_data[4].acquire()
         time.sleep(5)
 
         banner()
-        print('\n{}SUCCESS!{} World data has been dumped to {} in {}s \n'.format(bcolors.GREEN, bcolors.ENDC,dump_path, str(round(time.time()-shared_data[2]))))
+        print(
+            "\n{}SUCCESS!{} World data has been dumped to {} in {}s \n".format(
+                bcolors.GREEN,
+                bcolors.ENDC,
+                dump_path,
+                str(round(time.time() - shared_data[2])),
+            )
+        )
         enter()
         event.set()
         return
     except Exception:
         shared_data[3].set()
         shared_data[4].acquire(timeout=10)
         event.set()
-        msg = _('Error in:\n{}\nCause:\n{}').format(info, traceback.format_exc())
+        msg = _("Error in:\n{}\nCause:\n{}").format(info, traceback.format_exc())
         sendToBot(session, msg)
         return
 
 
-def do_it(session, waiting_time, start_id, shallow):
+def do_it(session, waiting_time, coords, radius, shallow, non_empty_islands):
     """
     Parameters
     ----------
     session : ikabot.web.session.Session
         Session object
     waiting_time : int
         Time to wait between each network request (to prevent getting rate limited)
     start_id : int
         Id of the island to start the dump from (0 starts from beginning)
     shallow : str
         String that determines if the data should be shallow (only map accessible data)
-    
+
     Returns
     -------
     dump_path: str
     """
 
     shared_data[2] = time.time()
-    world = {'name': 's' + str(session.mundo) + '-' + str(session.servidor),
-             'self_name': session.username,
-             'dump_start_date': time.time(),
-             'dump_end_date': 0,
-             'islands': [],
-             'shallow': shallow in ['y', 'Y']
-            }
+    partial = (
+        True if (coords and radius and radius >= 0) or non_empty_islands else False
+    )
+    world = {
+        "name": "s" + str(session.mundo) + "-" + str(session.servidor),
+        "self_name": session.username,
+        "dump_start_date": time.time(),
+        "dump_end_date": 0,
+        "islands": [],
+        "shallow": shallow,
+        "partial": partial,
+    }
     shared_data.append(world)
-    #scan 0 to 50 x and y
+    # scan 0 to 50 x and y
     shallow_islands = []
-    update_status('Initiating first map sweep', 0, 0, True)
-    update_status('Getting (0-50,0-50) islands', 25, 1.25)
-    data = session.post('action=WorldMap&function=getJSONArea&x_min=0&x_max=50&y_min=0&y_max=50')
-    for x, val in json.loads(data)['data'].items():
+    update_status("Initiating first map sweep", 0, 0, True)
+    update_status("Getting (0-50,0-50) islands", 25, 1.25)
+    data = session.post(
+        "action=WorldMap&function=getJSONArea&x_min=0&x_max=50&y_min=0&y_max=50"
+    )
+    for x, val in json.loads(data)["data"].items():
         for y, val2 in val.items():
-            shallow_islands.append({'x': x, 'y': y, 'id': val2[0], 'name': val2[1], 'resource_type': val2[2], 'miracle_type': val2[3], 'wood_lvl': val2[6], 'players': val2[7] })
-    update_status('Getting (50-100,0-50) islands', 50, 2.5)
+            shallow_islands.append(
+                {
+                    "x": x,
+                    "y": y,
+                    "id": val2[0],
+                    "name": val2[1],
+                    "resource_type": val2[2],
+                    "miracle_type": val2[3],
+                    "wood_lvl": val2[6],
+                    "players": val2[7],
+                }
+            )
+    update_status("Getting (50-100,0-50) islands", 50, 2.5)
     time.sleep(0.5)
-    data = session.post('action=WorldMap&function=getJSONArea&x_min=50&x_max=100&y_min=0&y_max=50')
-    for x, val in json.loads(data)['data'].items():
+    data = session.post(
+        "action=WorldMap&function=getJSONArea&x_min=50&x_max=100&y_min=0&y_max=50"
+    )
+    for x, val in json.loads(data)["data"].items():
         for y, val2 in val.items():
-            shallow_islands.append({'x': x, 'y': y, 'id': val2[0], 'name': val2[1], 'resource_type': val2[2], 'miracle_type': val2[3], 'wood_lvl': val2[6], 'players': val2[7] })
-    update_status('Getting (0-50,50-100) islands', 75, 3.75)
+            shallow_islands.append(
+                {
+                    "x": x,
+                    "y": y,
+                    "id": val2[0],
+                    "name": val2[1],
+                    "resource_type": val2[2],
+                    "miracle_type": val2[3],
+                    "wood_lvl": val2[6],
+                    "players": val2[7],
+                }
+            )
+    update_status("Getting (0-50,50-100) islands", 75, 3.75)
     time.sleep(0.5)
-    data = session.post('action=WorldMap&function=getJSONArea&x_min=0&x_max=50&y_min=50&y_max=100')
-    for x, val in json.loads(data)['data'].items():
+    data = session.post(
+        "action=WorldMap&function=getJSONArea&x_min=0&x_max=50&y_min=50&y_max=100"
+    )
+    for x, val in json.loads(data)["data"].items():
         for y, val2 in val.items():
-            shallow_islands.append({'x': x, 'y': y, 'id': val2[0], 'name': val2[1], 'resource_type': val2[2], 'miracle_type': val2[3], 'wood_lvl': val2[6], 'players': val2[7] })
-    update_status('Getting (50-100,50-100) islands', 100, 5)
+            shallow_islands.append(
+                {
+                    "x": x,
+                    "y": y,
+                    "id": val2[0],
+                    "name": val2[1],
+                    "resource_type": val2[2],
+                    "miracle_type": val2[3],
+                    "wood_lvl": val2[6],
+                    "players": val2[7],
+                }
+            )
+    update_status("Getting (50-100,50-100) islands", 100, 5)
     time.sleep(0.5)
-    data = session.post('action=WorldMap&function=getJSONArea&x_min=50&x_max=100&y_min=50&y_max=100')
-    for x, val in json.loads(data)['data'].items():
+    data = session.post(
+        "action=WorldMap&function=getJSONArea&x_min=50&x_max=100&y_min=50&y_max=100"
+    )
+    for x, val in json.loads(data)["data"].items():
         for y, val2 in val.items():
-            shallow_islands.append({'x': x, 'y': y, 'id': val2[0], 'name': val2[1], 'resource_type': val2[2], 'miracle_type': val2[3], 'wood_lvl': val2[6], 'players': val2[7] })
-
-# [
-# "58",         //id 0
-# "Phytios",    //name 1
-# "1",          //resource type 2
-# "2",          //type of miracle 3
-# "5",          // ?? 4
-# "4",          // ?? 5
-# "9",          // lumber level  6
-# "12",         // number of people 7
-# 0,            // piracy in range 8
-# "0",          // helios tower 9
-# "0",          // red 10
-# "0"           // blue 11
-# ]
-    
-    dump_path = os.getenv(home) + '/ikabot_world_dumps/s' + str(session.mundo) + '-' + str(session.servidor) + '/'
-    dump_path = dump_path.replace('\\','/')
-    dump_name = getDateTime() + '.json.gz'
-
-    if shallow in ['y','Y']:
-        dump_name = dump_name.replace('.json.gz', '_shallow') + '.json.gz'
-        update_status('Shallow dump is on. Dumping data...', 100, 100, True)
-        world['islands'] = shallow_islands
+            shallow_islands.append(
+                {
+                    "x": x,
+                    "y": y,
+                    "id": val2[0],
+                    "name": val2[1],
+                    "resource_type": val2[2],
+                    "miracle_type": val2[3],
+                    "wood_lvl": val2[6],
+                    "players": val2[7],
+                }
+            )
+
+    # [
+    # "58",         //id 0
+    # "Phytios",    //name 1
+    # "1",          //resource type 2
+    # "2",          //type of miracle 3
+    # "5",          // ?? 4
+    # "4",          // ?? 5
+    # "9",          // lumber level  6
+    # "12",         // number of people 7
+    # 0,            // piracy in range 8
+    # "0",          // helios tower 9
+    # "0",          // red 10
+    # "0"           // blue 11
+    # ]
+
+    dump_path = (
+        os.getenv(home)
+        + "/ikabot_world_dumps/s"
+        + str(session.mundo)
+        + "-"
+        + str(session.servidor)
+        + "/"
+    )
+    dump_path = dump_path.replace("\\", "/")
+    dump_name = getDateTime() + ".json.gz"
+
+    if shallow:
+        dump_name = dump_name.replace(".json.gz", "_shallow") + ".json.gz"
+        update_status("Shallow dump is on. Dumping data...", 100, 100, True)
+        world["islands"] = shallow_islands
         dump(world, dump_path, dump_name)
         return dump_path + dump_name
 
-    all_island_ids = set()
+    all_island = set()
     total_settlements = 0
     for island in shallow_islands:
-        all_island_ids.add(island['id'])
-        total_settlements += int(island['players'])
-
-    update_status('Got {} islands with {} towns in total'.format(len(all_island_ids), str(total_settlements)), 100, 5, True)
-    update_status('Getting data for each island. This will take a while...', 0, 5, True)
-
-    #scan each island
-
-    world_islands_number = len(all_island_ids)
-    all_island_ids = list(split(sorted(map(int, all_island_ids)), 1))
-    
-    dump_islands(shared_data, all_island_ids[0], waiting_time, start_id, session, world_islands_number)
-
-    update_status('Got {} individual islands'.format(world_islands_number), 100, 100, True)
-
-    update_status('Dumping data to {}'.format(dump_path + dump_name), 100, 100, True)
+        island_id = int(island["id"])
+        x = int(island["x"])
+        y = int(island["y"])
+        if non_empty_islands and not int(island["players"]):
+            continue
+        if (
+            coords
+            and radius
+            and ((x - coords[0]) ** 2 + (y - coords[1]) ** 2) ** 0.5 > radius
+        ):
+            continue
+        all_island.add((island_id, x, y))
+        total_settlements += int(island["players"])
 
+    update_status(
+        "Got {} islands with {} towns in total".format(
+            len(all_island), str(total_settlements)
+        ),
+        100,
+        5,
+        True,
+    )
+    update_status("Getting data for each island. This will take a while...", 0, 5, True)
+
+    # scan each island
+
+    all_island = sorted(all_island)
+    dump_islands(shared_data, all_island, waiting_time, session)
+    update_status("Got {} individual islands".format(len(all_island)), 100, 100, True)
+
+    name_suffix = "_partial" if partial else ""
+    dump_name = dump_name.replace(".json.gz", name_suffix) + ".json.gz"
+    update_status("Dumping data to {}".format(dump_path + dump_name), 100, 100, True)
     dump(shared_data[5], dump_path, dump_name)
-    
-
     return dump_path + dump_name
 
-def split(a, n):
-    k, m = divmod(len(a), n)
-    return (a[i*k+min(i, m):(i+1)*k+min(i+1, m)] for i in range(n))
 
 def dump(world, dump_path, dump_name):
-    world['dump_end_date'] = time.time()
+    world["dump_end_date"] = time.time()
     p = Path(dump_path)
     p.mkdir(exist_ok=True, parents=True)
-    with gzip.open(dump_path+dump_name,'wb') as file:
-        json_string = json.dumps(world).encode('utf-8')
+    with gzip.open(dump_path + dump_name, "wb") as file:
+        json_string = json.dumps(world).encode("utf-8")
         file.write(json_string)
-       
-def dump_islands(shared_data, all_island_ids, waiting_time, start_id, session, world_islands_number):
-    for i, island_id in enumerate(sorted(map(int, all_island_ids))):
-        if(int(island_id) < start_id):
-            continue
-        update_status('Getting island id {}'.format(island_id), len(shared_data[5]['islands'])/world_islands_number*100, 5+(len(shared_data[5]['islands'])/world_islands_number * 95))
-        html = ''
+
+
+def dump_islands(shared_data, all_island, waiting_time, session):
+    world_islands_number = len(all_island)
+    for island in all_island:
+        island_id = island[0]
+        island_coords = (island[1], island[2])
+        update_status(
+            "Getting island id: {}, x: {}, y: {}".format(
+                island_id, island_coords[0], island_coords[1]
+            ),
+            len(shared_data[5]["islands"]) / world_islands_number * 100,
+            5 + (len(shared_data[5]["islands"]) / world_islands_number * 95),
+        )
+        html = ""
         try:
-            html = session.get('view=island&islandId=' + str(island_id))
+            html = session.get("view=island&islandId=" + str(island_id))
         except Exception:
             # try again
-            html = session.get('view=island&islandId=' + str(island_id))
+            html = session.get("view=island&islandId=" + str(island_id))
         island = getIsland(html)
         shared_data[4].acquire()
-        shared_data[5]['islands'].append(island)
+        shared_data[5]["islands"].append(island)
         shared_data[4].release()
         time.sleep(waiting_time)
 
+
 def update_terminal(shared_data):
-    while(True):
+    while True:
         banner()
-        print('\n')
+        print("\n")
         shared_data[4].acquire()
         print(shared_data[1])
         shared_data[4].release()
-        chars = ['\\','|','/','─']
+        chars = ["\\", "|", "/", "─"]
         for i in range(20):
             shared_data[4].acquire()
-            print(' '*120, end='\r')
-            print(shared_data[0] + ',\tdt: ' + str(round(time.time()-shared_data[2],2)) + 's\t' + chars[i%4] , end='\r')
+            print(" " * 120, end="\r")
+            print(
+                shared_data[0]
+                + ",\tdt: "
+                + str(round(time.time() - shared_data[2], 2))
+                + "s\t"
+                + chars[i % 4],
+                end="\r",
+            )
             shared_data[4].release()
             time.sleep(0.05)
         if stop_updating.is_set():
             return
-        
-def update_status(message, percent, percent_total, add_history = False):
+
+
+def update_status(message, percent, percent_total, add_history=False):
     shared_data[4].acquire()
-    shared_data[0] = message + '\t' + str(round(percent,1)) + '%,\ttotal: ' + str(round(percent_total,1)) + '%'
-    if(add_history):
-        shared_data[1] += shared_data[0] + '\n'
+    shared_data[0] = (
+        message
+        + "\t"
+        + str(round(percent, 1))
+        + "%,\ttotal: "
+        + str(round(percent_total, 1))
+        + "%"
+    )
+    if add_history:
+        shared_data[1] += shared_data[0] + "\n"
     shared_data[4].release()
-    
+
 
 def view_dump(session, event):
-    files = [file.replace('\\','/') for file in get_files(os.getenv(home) + '/ikabot_world_dumps') if '.json.gz' in file ]
+    files = [
+        file.replace("\\", "/")
+        for file in get_files(os.getenv(home) + "/ikabot_world_dumps")
+        if ".json.gz" in file
+    ]
 
-    print('All dumps are stored in ' + os.getenv(home) + '/ikabot_world_dumps\n')
-    print('Choose a dump to view:')
+    print("All dumps are stored in " + os.getenv(home) + "/ikabot_world_dumps\n")
+    print("Choose a dump to view:")
     for i, file in enumerate(files):
-        print(str(i) + ') ' + file.split('/')[-2] + ' ' + file.split('/')[-1].replace('.json.gz','').replace('_',' '))
-    choice = read(min = 0, max = len(files)-1, digit=True)
-    print('Loading dump...')
+        print(
+            str(i)
+            + ") "
+            + file.split("/")[-2]
+            + " "
+            + file.split("/")[-1].replace(".json.gz", "").replace("_", " ")
+        )
+    choice = read(min=0, max=len(files) - 1, digit=True)
+    print("Loading dump...")
     selected_dump = files[choice]
-    with gzip.open(selected_dump, 'rb') as file:
+    with gzip.open(selected_dump, "rb") as file:
         selected_dump = json.load(file)
-    
+
     while True:
         banner()
-        print_map(selected_dump['islands'])
-        print('0) Back')
-        print('1) Search islands by island criteria')
-        if not selected_dump['shallow']:
-            print('2) Search islands by player name')
-            print('3) Search for nearest inactive players')
+        print_map(selected_dump["islands"])
+        print("0) Back")
+        print("1) Search islands by island criteria")
+        if not selected_dump["shallow"]:
+            print("2) Search islands by player name")
+            print("3) Search for nearest inactive players")
 
         choice = read(min=0, max=3, digit=True)
         if choice == 0:
             event.set()
             return
         elif choice == 1:
-            print('Search island by a certain criteria. The available properties of an island are:')
-            print('resource_type : [1,2,3,4] // these are  Wine, Marble, Cristal, Sulfur')
-            print('miracle_type : [1,2,3,4,5,6,7,8] // hephaistos forge is number 5')
-            print('wood_lvl : [1..] // this is the forest level on the island')
-            print('players : [0..] // number of players on the island')
-            print('ex. If I wanted to find all islands with less than 10 players and forest level 30 with hephaistos I would type in:')
-            print('players < 10 and wood_lvl == 30 and miracle_type == 5\n')
+            print(
+                "Search island by a certain criteria. The available properties of an island are:"
+            )
+            print(
+                "resource_type : [1,2,3,4] // these are  Wine, Marble, Cristal, Sulfur"
+            )
+            print("miracle_type : [1,2,3,4,5,6,7,8] // hephaistos forge is number 5")
+            print("wood_lvl : [1..] // this is the forest level on the island")
+            print(
+                "luxury_lvl : [1..] // this is the level of the luxury resource on the island (Only available in full dumps)"
+            )
+            print("players : [0..] // number of players on the island")
+            print(
+                "ex. If I wanted to find all islands with less than 10 players and forest level 30 with hephaistos I would type in:"
+            )
+            print("players < 10 and wood_lvl == 30 and miracle_type == 5\n")
             condition = read(msg="Enter the condition: ")
 
             try:
-                filtered_islands = [island for island in filter(lambda x: filter_on_condition(x, condition), selected_dump['islands'] if selected_dump['shallow'] else convert_to_shallow(selected_dump['islands']))]
+                filtered_islands = [
+                    island
+                    for island in filter(
+                        lambda x: filter_on_condition(x, condition),
+                        (
+                            selected_dump["islands"]
+                            if selected_dump["shallow"]
+                            else convert_to_shallow(selected_dump["islands"])
+                        ),
+                    )
+                ]
             except (SyntaxError, KeyError):
-                print('Condition is bad, please use only the available island properties and use python standard conditional sytnax (and, or, <, >, ==, (, ), etc... )')
+                print(
+                    "Condition is bad, please use only the available island properties and use python standard conditional sytnax (and, or, <, >, ==, (, ), etc... )\nRemember luxury_lvl is only available in full dumps!"
+                )
                 enter()
                 continue
-            
-            print('The satisfying islands are:')
+
+            print("The satisfying islands are:")
             [print(island) for island in filtered_islands]
             enter()
         elif choice == 2:
-            if selected_dump['shallow']:
-                print('You can not search by player name because this dump is shallow and doesn\'t contain data about players!')
+            if selected_dump["shallow"]:
+                print(
+                    "You can not search by player name because this dump is shallow and doesn't contain data about players!"
+                )
                 enter()
                 continue
-            player_name = read(msg='Type in the player name: ')
+            player_name = read(msg="Type in the player name: ")
             # search for players by name
             players = []
-            for island in selected_dump['islands']:
-                for city in island['cities']:
-                    if city['type'] != 'empty' and player_name in city['Name']:
-                        players.append((player_name, island['id']))
+            for island in selected_dump["islands"]:
+                for city in island["cities"]:
+                    if city["type"] != "empty" and player_name in city["Name"]:
+                        players.append((player_name, island["id"]))
             # return if none are found
             if not len(players):
-                print('No players found!')
+                print("No players found!")
                 enter()
                 continue
-            # select one 
-            print('Chose a player to add to selection: ')
+            # select one
+            print("Chose a player to add to selection: ")
             for i, player in enumerate(unique_tuples(players)):
-                print(str(i) + ') ' + player[0])
-            choice = read(min=0, max=len(list(unique_tuples(players)))-1, digit=True)
+                print(str(i) + ") " + player[0])
+            choice = read(min=0, max=len(list(unique_tuples(players))) - 1, digit=True)
             # add his islands to selection
             for player in players:
                 if player[0] == list(unique_tuples(players))[choice][0]:
                     selected_islands.add(int(player[1]))
         elif choice == 3:
-            if selected_dump['shallow']:
-                print('You can not search by player name because this dump is shallow and doesn\'t contain data about players!')
+            if selected_dump["shallow"]:
+                print(
+                    "You can not search by player name because this dump is shallow and doesn't contain data about players!"
+                )
                 enter()
                 continue
-            coords = read(msg='Type in a center point (x,y): ').replace('(','').replace(')','').split(',')
+            coords = (
+                read(msg="Type in a center point (x,y): ")
+                .replace("(", "")
+                .replace(")", "")
+                .split(",")
+            )
             coords = (int(coords[0]), int(coords[1]))
-            number_of_inactives = read(msg='How many inactives should be displayed? (min=1, default=25): ', min = 1, digit=True, default=25)
-            #sort islands based on distance from center point
-            islands_sorted = sorted(selected_dump['islands'], key=lambda island: ((island['x'] - coords[0]) ** 2 + (island['y'] - coords[1]) ** 2) ** 0.5)
-            print('The nearest 25 inactive players are: ')
-            #below follows the unholiest way to get the first n cities which are contained in an island object which is contained in a list of islands without duplicates in one line of code using python list comprehension
+            number_of_inactives = read(
+                msg="How many inactives should be displayed? (min=1, default=25): ",
+                min=1,
+                digit=True,
+                default=25,
+            )
+            # sort islands based on distance from center point
+            islands_sorted = sorted(
+                selected_dump["islands"],
+                key=lambda island: (
+                    (island["x"] - coords[0]) ** 2 + (island["y"] - coords[1]) ** 2
+                )
+                ** 0.5,
+            )
+            print("The nearest 25 inactive players are: ")
+            # below follows the unholiest way to get the first n cities which are contained in an island object which is contained in a list of islands without duplicates in one line of code using python list comprehension
             seen = set()
-            inactives = [city for island in islands_sorted for city in island['cities'] if city['type'] != 'empty' and city['state'] == 'inactive' and isinstance([(seen.add(city['Name']),) if city['Name'] not in seen else None][0],tuple)][:number_of_inactives]
+            inactives = [
+                city
+                for island in islands_sorted
+                for city in island["cities"]
+                if city["type"] != "empty"
+                and city["state"] == "inactive"
+                and isinstance(
+                    [(seen.add(city["Name"]),) if city["Name"] not in seen else None][
+                        0
+                    ],
+                    tuple,
+                )
+            ][:number_of_inactives]
             for i, city in enumerate(inactives):
-                print(str(i+1) + ') ' + city['Name'])
+                print(str(i + 1) + ") " + city["Name"])
             enter()
 
 
 def print_map(islands):
     """Prints out a 100x100 matrix with all world islands on it. Selected islands are colored red.
     Parameters
     ----------
     islands : [object]
         List of island objects to be displayed
     """
 
-    map = [[bcolors.DARK_BLUE + '██' + bcolors.ENDC for j in range(100)] for i in range(100)] # 100x100 matrix of dark blue ██
+    map = [
+        [bcolors.DARK_BLUE + "██" + bcolors.ENDC for j in range(100)]
+        for i in range(100)
+    ]  # 100x100 matrix of dark blue ██
     selected_island_coords = []
 
     for island in islands:
-        if int(island['id']) in selected_islands:
-            map[int(island['x'])-1][int(island['y'])-1] = bcolors.DARK_RED + '◉ ' + bcolors.ENDC 
-            selected_island_coords.append((int(island['x']),int(island['y'])))
+        if int(island["id"]) in selected_islands:
+            map[int(island["x"]) - 1][int(island["y"]) - 1] = (
+                bcolors.DARK_RED + "◉ " + bcolors.ENDC
+            )
+            selected_island_coords.append((int(island["x"]), int(island["y"])))
         else:
-            map[int(island['x'])-1][int(island['y'])-1] = bcolors.DARK_GREEN + '◉ ' + bcolors.ENDC
+            map[int(island["x"]) - 1][int(island["y"]) - 1] = (
+                bcolors.DARK_GREEN + "◉ " + bcolors.ENDC
+            )
 
     for row in reversed(map):
-        print(''.join(row))
+        print("".join(row))
 
-    print(bcolors.DARK_BLUE + '██' + bcolors.ENDC + ' - Water, ' + \
-          bcolors.DARK_GREEN + '◉' + bcolors.ENDC + ' - Island, '+ \
-          bcolors.DARK_RED + '◉' + bcolors.ENDC + ' - Selected\n'
-        )
+    print(
+        bcolors.DARK_BLUE
+        + "██"
+        + bcolors.ENDC
+        + " - Water, "
+        + bcolors.DARK_GREEN
+        + "◉"
+        + bcolors.ENDC
+        + " - Island, "
+        + bcolors.DARK_RED
+        + "◉"
+        + bcolors.ENDC
+        + " - Selected\n"
+    )
+
+    print("Selected islands: " + str(selected_island_coords))
 
-    print('Selected islands: ' + str(selected_island_coords))
-    
 
 def filter_on_condition(island, condition):
     """Returns true if island satisfies condition
     Parameters
     ----------
     island : object
         Island to be tested on condition
@@ -394,52 +609,71 @@
         Bool indicating whether or not the island object satisfies the condition
     """
 
     condition = ast.parse(condition)
     for node in ast.walk(condition):
         if isinstance(node, ast.Compare):
             left = node.left.id
-            right = node.comparators[0].n if isinstance(node.comparators[0], ast.Num) else node.comparators[0].id
+            right = (
+                node.comparators[0].n
+                if isinstance(node.comparators[0], ast.Num)
+                else node.comparators[0].id
+            )
             op = node.ops[0]
             if op.__class__ == ast.Lt:
                 if not int(island[left]) < int(right):
                     return False
             elif op.__class__ == ast.Gt:
                 if not int(island[left]) > int(right):
                     return False
             elif op.__class__ == ast.Eq:
                 if not int(island[left]) == int(right):
                     return False
     return True
 
-    
 
 def convert_to_shallow(islands):
     """Converts a list of islands from a deep dump into a shallow dump version of that list
     Parameters
     ----------
     islands : [object]
         List of island objects to be converted
-    
+
     Returns
     -------
     islands : [object]
-        List of objects that represent the stripped-down version of an island 
+        List of objects that represent the stripped-down version of an island
     """
-    return [{'x': str(island['x']), 'y': str(island['y']), 'id': island['id'], 'name': island['name'], 'resource_type': island['tradegood'], 'miracle_type': island['wonder'], 'wood_lvl': island['resourceLevel'], 'players': len([city for city in island['cities'] if city['type'] != 'empty'])} for island in islands]
+    return [
+        {
+            "x": str(island["x"]),
+            "y": str(island["y"]),
+            "id": island["id"],
+            "name": island["name"],
+            "resource_type": island["tradegood"],
+            "miracle_type": island["wonder"],
+            "wood_lvl": island["resourceLevel"],
+            "luxury_lvl": island["tradegoodLevel"],
+            "players": len(
+                [city for city in island["cities"] if city["type"] != "empty"]
+            ),
+        }
+        for island in islands
+    ]
+
 
 def unique_tuples(tuples):
-    """Iterates over tuples with a unique first element
-    """
+    """Iterates over tuples with a unique first element"""
     seen = {}
     for t in tuples:
         if t[0] not in seen:
             seen[t[0]] = True
             yield t
 
+
 def get_files(path):
     """
     Returns all full paths to every file in a directory and all it's subdirectories
     Parameters
     ----------
     path : str
         Path to directory
```

### Comparing `ikabot-6.6.4/ikabot/function/importExportCookie.py` & `ikabot-7.0.1/ikabot/function/importExportCookie.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 #! /usr/bin/env python3
 # -*- coding: utf-8 -*-
 import gettext
 import json
 import sys
+
 import requests
-from ikabot.helpers.pedirInfo import read
-from ikabot.helpers.gui import *
+
 from ikabot.config import *
+from ikabot.helpers.gui import *
+from ikabot.helpers.pedirInfo import read
 
-t = gettext.translation('insertCookies', localedir, languages=languages, fallback=True)
+t = gettext.translation("insertCookies", localedir, languages=languages, fallback=True)
 _ = t.gettext
 
 
 def importExportCookie(session, event, stdin_fd, predetermined_input):
     """
     Parameters
     ----------
@@ -21,69 +23,89 @@
     stdin_fd: int
     predetermined_input : multiprocessing.managers.SyncManager.list
     """
     sys.stdin = os.fdopen(stdin_fd)
     config.predetermined_input = predetermined_input
     banner()
     try:
-        print('Do you want to import or export the cookie?')
-        print('(0) Exit')
-        print('(1) Import')
-        print('(2) Export')
+        print("Do you want to import or export the cookie?")
+        print("(0) Exit")
+        print("(1) Import")
+        print("(2) Export")
         action = read(min=0, max=2)
         if action == 1:
             importCookie(session)
         elif action == 2:
             exportCookie(session)
 
         event.set()
     except KeyboardInterrupt:
         event.set()
         return
 
 
 def importCookie(session):
     banner()
-    print('{}⚠️ INSERTING AN INVALID COOKIE WILL LOG YOU OUT OF YOUR OTHER SESSIONS ⚠️{}\n\n'.format(bcolors.WARNING, bcolors.ENDC))
-    print('Go ahead and export the cookie from another ikabot instance now and then')
+    print(
+        "{}⚠️ INSERTING AN INVALID COOKIE WILL LOG YOU OUT OF YOUR OTHER SESSIONS ⚠️{}\n\n".format(
+            bcolors.WARNING, bcolors.ENDC
+        )
+    )
+    print("Go ahead and export the cookie from another ikabot instance now and then")
     print('type your "ikariam" cookie below:')
     newcookie = read()
     newcookie = newcookie.strip()
-    newcookie = newcookie.replace('ikariam=', '')
-    cookies = session.getSessionData()['cookies']
-    cookies['ikariam'] = newcookie
+    newcookie = newcookie.replace("ikariam=", "")
+    cookies = session.getSessionData()["cookies"]
+    cookies["ikariam"] = newcookie
     if session.host in session.s.cookies._cookies:
-        session.s.cookies.set('ikariam', newcookie, domain=session.host, path='/')
+        session.s.cookies.set("ikariam", newcookie, domain=session.host, path="/")
     else:
-        session.s.cookies.set('ikariam', newcookie, domain='', path='/')
+        session.s.cookies.set("ikariam", newcookie, domain="", path="/")
 
     html = session.s.get(session.urlBase).text
 
     if session.isExpired(html):
-        print('{}Failure!{} All your other sessions have just been invalidated!'.format(bcolors.RED, bcolors.ENDC))
+        print(
+            "{}Failure!{} All your other sessions have just been invalidated!".format(
+                bcolors.RED, bcolors.ENDC
+            )
+        )
         enter()
     else:
-        print('{}Success!{} This ikabot session will now use the cookie you provided'.format(bcolors.GREEN, bcolors.ENDC))
+        print(
+            "{}Success!{} This ikabot session will now use the cookie you provided".format(
+                bcolors.GREEN, bcolors.ENDC
+            )
+        )
         sessionData = session.getSessionData()
-        sessionData['cookies']['ikariam'] = newcookie
+        sessionData["cookies"]["ikariam"] = newcookie
         session.setSessionData(sessionData)
         enter()
     session.get()
 
 
 def exportCookie(session):
     banner()
     session.get()  # get valid cookie in case user has logged the bot out before running this feature
-    ikariam = session.getSessionData()['cookies']['ikariam']
-    print('Use this cookie to synchronise two ikabot instances on 2 different machines\n\n')
-    print('ikariam='+ikariam+'\n\n')
-
-    cookie = json.dumps({"ikariam": ikariam})  # get ikariam cookie, only this cookie is invalidated when the bot logs the user out.
-    cookies_js = 'cookies={};i=0;for(let cookie in cookies){{document.cookie=Object.keys(cookies)[i]+\"=\"+cookies[cookie];i++}}'.format(cookie)
-    print("""To prevent ikabot from logging you out while playing Ikariam do the following:
+    ikariam = session.getSessionData()["cookies"]["ikariam"]
+    print(
+        "Use this cookie to synchronise two ikabot instances on 2 different machines\n\n"
+    )
+    print("ikariam=" + ikariam + "\n\n")
+
+    cookie = json.dumps(
+        {"ikariam": ikariam}
+    )  # get ikariam cookie, only this cookie is invalidated when the bot logs the user out.
+    cookies_js = 'cookies={};i=0;for(let cookie in cookies){{document.cookie=Object.keys(cookies)[i]+"="+cookies[cookie];i++}}'.format(
+        cookie
+    )
+    print(
+        """To prevent ikabot from logging you out while playing Ikariam do the following:
     1. Be on the "Your session has expired" screen
     2. Open Chrome javascript console by pressing CTRL + SHIFT + J
     3. Copy the text below, paste it into the console and press enter
     4. Press F5
-    """)
+    """
+    )
     print(cookies_js)
     enter()
```

### Comparing `ikabot-6.6.4/ikabot/function/investigate.py` & `ikabot-7.0.1/ikabot/function/investigate.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,63 +1,78 @@
 #! /usr/bin/env python3
 # -*- coding: utf-8 -*-
 
-import json
 import gettext
+import json
 import traceback
+
 from ikabot.config import *
-from ikabot.helpers.gui import *
-from ikabot.helpers.varios import *
 from ikabot.helpers.botComm import *
+from ikabot.helpers.getJson import getCity
+from ikabot.helpers.gui import *
 from ikabot.helpers.pedirInfo import *
 from ikabot.helpers.process import set_child_mode
-from ikabot.helpers.getJson import getCity
 from ikabot.helpers.signals import setInfoSignal
+from ikabot.helpers.varios import *
 
-t = gettext.translation('investigate', localedir, languages=languages, fallback=True)
+t = gettext.translation("investigate", localedir, languages=languages, fallback=True)
 _ = t.gettext
 
+
 def get_studies(session):
     html = session.get()
     city = getCity(html)
-    city_id = city['id']
-    url = 'view=researchAdvisor&oldView=updateGlobalData&cityId={0}&backgroundView=city&currentCityId={0}&templateView=researchAdvisor&actionRequest={1}&ajax=1'.format(city_id, actionRequest)
+    city_id = city["id"]
+    url = "view=researchAdvisor&oldView=updateGlobalData&cityId={0}&backgroundView=city&currentCityId={0}&templateView=researchAdvisor&actionRequest={1}&ajax=1".format(
+        city_id, actionRequest
+    )
     resp = session.post(url)
     resp = json.loads(resp, strict=False)
     return resp[2][1]
 
 
 def study(session, studies, num_study):
     html = session.get()
     city = getCity(html)
-    city_id = city['id']
-    research_type = studies['js_researchAdvisorChangeResearchType{}'.format(num_study)]['ajaxrequest'].split('=')[-1]
-    url = 'action=Advisor&function=doResearch&actionRequest={}&type={}&backgroundView=city&currentCityId={}&templateView=researchAdvisor&ajax=1'.format(actionRequest, research_type, city_id)
+    city_id = city["id"]
+    research_type = studies["js_researchAdvisorChangeResearchType{}".format(num_study)][
+        "ajaxrequest"
+    ].split("=")[-1]
+    url = "action=Advisor&function=doResearch&actionRequest={}&type={}&backgroundView=city&currentCityId={}&templateView=researchAdvisor&ajax=1".format(
+        actionRequest, research_type, city_id
+    )
     session.post(url)
 
+
 def experiment(session, experiments):
-     while experiments['qty'] > 0:
+    while experiments["qty"] > 0:
         # Validate if material is still there..oterwhise log it and send it via bot
-        session.get('view=city&cityId={}'.format(experiments["cityID"]), noIndex=True)
+        session.get("view=city&cityId={}".format(experiments["cityID"]), noIndex=True)
         data = session.get("view=updateGlobalData&ajax=1", noIndex=True)
         json_data = json.loads(data, strict=False)
-        json_data = json_data[0][1]['headerData']
-        current_glass = int(json_data['currentResources']['3'])
+        json_data = json_data[0][1]["headerData"]
+        current_glass = int(json_data["currentResources"]["3"])
 
-        if (current_glass < 300000):
-            sendToBot(session, f"Experiment process ended on {experiments['cityName']} due lack of glass ({addThousandSeparator(current_glass)})")
+        if current_glass < 300000:
+            sendToBot(
+                session,
+                f"Experiment process ended on {experiments['cityName']} due lack of glass ({addThousandSeparator(current_glass)})",
+            )
             break
 
         url = f'action=CityScreen&function=buyResearch&cityId={experiments["cityID"]}&position={experiments["pos"]}&backgroundView=city&currentCityId={experiments["cityID"]}&templateView=academy&actionRequest={actionRequest}&ajax=1'
         session.post(url)
-        experiments['qty'] = experiments['qty'] - 1
-        sendToBot(session, f"Experiment done on {experiments['cityName']}, left = {experiments['qty']} time (s)")
+        experiments["qty"] = experiments["qty"] - 1
+        sendToBot(
+            session,
+            f"Experiment done on {experiments['cityName']}, left = {experiments['qty']} time (s)",
+        )
 
         # Terminate it if no of experiments = 0
-        if (experiments['qty'] == 0):
+        if experiments["qty"] == 0:
             break
 
         # Every 4h, added 1m extra
         time.sleep(241 * 60)
 
 
 def investigate(session, event, stdin_fd, predetermined_input):
@@ -69,104 +84,119 @@
     stdin_fd: int
     predetermined_input : multiprocessing.managers.SyncManager.list
     """
     sys.stdin = os.fdopen(stdin_fd)
     config.predetermined_input = predetermined_input
     try:
         banner()
-        
-        print('\nSelect an option:')
-        print('1) Study')
-        print('2) Conduct experiment')
+
+        print("\nSelect an option:")
+        print("1) Study")
+        print("2) Conduct experiment")
         option = read(min=1, max=2)
 
         if option == 1:
             studies = get_studies(session)
             keys = list(studies.keys())
-            num_studies = len([key for key in keys if 'js_researchAdvisorChangeResearchTypeTxt' in key])
+            num_studies = len(
+                [
+                    key
+                    for key in keys
+                    if "js_researchAdvisorChangeResearchTypeTxt" in key
+                ]
+            )
 
             available = []
             for num_study in range(num_studies):
-                if 'js_researchAdvisorProgressTxt{}'.format(num_study) in studies:
+                if "js_researchAdvisorProgressTxt{}".format(num_study) in studies:
                     available.append(num_study)
 
             if len(available) == 0:
-                print(_('There are no available studies.'))
+                print(_("There are no available studies."))
                 enter()
                 event.set()
                 return
 
-            print(_('Which one do you wish to study?'))
-            print('0) None')
+            print(_("Which one do you wish to study?"))
+            print("0) None")
             for index, num_study in enumerate(available):
-                print('{:d}) {}'.format(index+1, studies['js_researchAdvisorNextResearchName{}'.format(num_study)]))
+                print(
+                    "{:d}) {}".format(
+                        index + 1,
+                        studies[
+                            "js_researchAdvisorNextResearchName{}".format(num_study)
+                        ],
+                    )
+                )
             choice = read(min=0, max=len(available))
 
             if choice == 0:
                 event.set()
                 return
 
-            study(session, studies, available[choice-1])
-            print(_('Done.'))
+            study(session, studies, available[choice - 1])
+            print(_("Done."))
             enter()
             event.set()
         else:
             # Experiment
             experiments = {}
             total_glass = 0
             found_academy = -1
 
-            #while (total_glass < 300000 or found_academy < 0):
+            # while (total_glass < 300000 or found_academy < 0):
             banner()
-            print('Pick city: ')
+            print("Pick city: ")
             city = chooseCity(session)
-            total_glass = int(city['recursos'][3])
-            
+            total_glass = int(city["availableResources"][3])
+
             # Check if enough glass
-            if (total_glass < 300000 ):
-                print(f'Not enough glass ({addThousandSeparator(total_glass)}), try another city. Min=300k')
+            if total_glass < 300000:
+                print(
+                    f"Not enough glass ({addThousandSeparator(total_glass)}), try another city. Min=300k"
+                )
                 time.sleep(2)
                 enter()
                 event.set()
                 return
-            
+
             # Search for Academy
-            for building in city['position']:
-                if building['building'] == 'academy':
-                    found_academy = building['position']
+            for building in city["position"]:
+                if building["building"] == "academy":
+                    found_academy = building["position"]
 
-            if (found_academy < 0):
-                print(f'No academy in this town, pick another one')
+            if found_academy < 0:
+                print(f"No academy in this town, pick another one")
                 time.sleep(2)
                 enter()
                 event.set()
                 return
-            
-            max_experiments = (total_glass // 300000)
+
+            max_experiments = total_glass // 300000
             banner()
-            print(f'How many experiments? Min=1, Max={max_experiments}')
+            print(f"How many experiments? Min=1, Max={max_experiments}")
             choice = read(min=1, max=max_experiments)
 
             # Build experiments dict
-            experiments['cityID'] = city['id']
-            experiments['cityName'] = city['name']
-            experiments['pos'] = found_academy
-            experiments['qty'] = choice
+            experiments["cityID"] = city["id"]
+            experiments["cityName"] = city["name"]
+            experiments["pos"] = found_academy
+            experiments["qty"] = choice
 
             # Process
             set_child_mode(session)
             event.set()
 
-            info = (f'Process: Experiments\n\nWill excecute {choice} times every 4h')
+            info = f"Process: Experiments\n\nWill excecute {choice} times every 4h"
 
             try:
                 sendToBot(session, info)
                 experiment(session, experiments)
             except Exception as e:
-                error_msg = f'Error in:\n{info}\nCause:\n{traceback.format_exc()}'
+                error_msg = f"Error in:\n{info}\nCause:\n{traceback.format_exc()}"
                 sendToBot(session, error_msg)
             finally:
                 session.logout()
 
     except KeyboardInterrupt:
         event.set()
         return
```

### Comparing `ikabot-6.6.4/ikabot/function/killTasks.py` & `ikabot-7.0.1/ikabot/function/killTasks.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 #! /usr/bin/env python3
 # -*- coding: utf-8 -*-
+import datetime
 import gettext
 import sys
-import datetime
-from ikabot.helpers.pedirInfo import read, enter
-from ikabot.helpers.gui import *
+
 from ikabot.config import *
-from ikabot.helpers.process import updateProcessList, run
+from ikabot.helpers.gui import *
+from ikabot.helpers.pedirInfo import enter, read
+from ikabot.helpers.process import run, updateProcessList
 
-t = gettext.translation('killTasks', localedir, languages=languages, fallback=True)
+t = gettext.translation("killTasks", localedir, languages=languages, fallback=True)
 _ = t.gettext
 
 
 def killTasks(session, event, stdin_fd, predetermined_input):
     """
     Parameters
     ----------
@@ -23,32 +24,47 @@
     """
     sys.stdin = os.fdopen(stdin_fd)
     config.predetermined_input = predetermined_input
     try:
         while True:
             banner()
             process_list = updateProcessList(session)
-            process_list = [process for process in process_list if process['action'] != 'killTasks']
+            process_list = [
+                process for process in process_list if process["action"] != "killTasks"
+            ]
             if len(process_list) == 0:
-                print(_('There are no tasks running'))
+                print(_("There are no tasks running"))
                 enter()
                 event.set()
                 return
-            print('Which task do you wish to kill?\n')
-            print('(0) Exit')
+            print("Which task do you wish to kill?\n")
+            print("(0) Exit")
             for process in process_list:
-                if 'date' in process:
-                    print("({}) {:<35}{:>20}".format(process_list.index(process) + 1, process['action'], datetime.datetime.fromtimestamp(process['date']).strftime('%b %d %H:%M:%S')))
+                if "date" in process:
+                    print(
+                        "({}) {:<35}{:>20}".format(
+                            process_list.index(process) + 1,
+                            process["action"],
+                            datetime.datetime.fromtimestamp(process["date"]).strftime(
+                                "%b %d %H:%M:%S"
+                            ),
+                        )
+                    )
                 else:
-                    print("({}) {:<35}".format(process_list.index(process) + 1, process['action'],))
+                    print(
+                        "({}) {:<35}".format(
+                            process_list.index(process) + 1,
+                            process["action"],
+                        )
+                    )
             choise = read(min=0, max=len(process_list), digit=True)
             if choise == 0:
                 event.set()
                 return
             else:
                 if isWindows:
-                    run("taskkill /F /PID {}".format(process_list[choise-1]['pid']))
+                    run("taskkill /F /PID {}".format(process_list[choise - 1]["pid"]))
                 else:
-                    run("kill -9 {}".format(process_list[choise-1]['pid']))
+                    run("kill -9 {}".format(process_list[choise - 1]["pid"]))
     except KeyboardInterrupt:
         event.set()
         return
```

### Comparing `ikabot-6.6.4/ikabot/function/loginDaily.py` & `ikabot-7.0.1/ikabot/helpers/market.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,71 +1,92 @@
 #! /usr/bin/env python3
 # -*- coding: utf-8 -*-
 
-import time
-import gettext
-import traceback
-import sys
+import json
+import re
+
 from ikabot.config import *
-from ikabot.helpers.botComm import *
-from ikabot.helpers.signals import setInfoSignal
-from ikabot.helpers.process import set_child_mode
-from ikabot.helpers.gui import enter
+from ikabot.helpers.getJson import getCity
 from ikabot.helpers.pedirInfo import getIdsOfCities
-from ikabot.helpers.varios import wait, getDateTime
 
-t = gettext.translation('loginDaily', localedir, languages=languages, fallback=True)
-_ = t.gettext
 
+def getCommercialCities(session):
+    """
+    Parameters
+    ----------
+    session : ikabot.web.session.Session
 
-def loginDaily(session, event, stdin_fd, predetermined_input):
+    Returns
+    -------
+    commercial_cities : list[dict]
+    """
+    cities_ids = getIdsOfCities(session)[0]
+    commercial_cities = []
+    for city_id in cities_ids:
+        html = session.get(city_url + city_id)
+        city = getCity(html)
+        for pos, building in enumerate(city["position"]):
+            if building["building"] == "branchOffice":
+                city["pos"] = pos
+                html = getMarketHtml(session, city)
+                positions = re.findall(r"<option.*?>(\d+)</option>", html)
+                city["rango"] = int(positions[-1])
+                commercial_cities.append(city)
+                break
+    return commercial_cities
+
+
+def getMarketHtml(session, city):
     """
     Parameters
     ----------
     session : ikabot.web.session.Session
-    event : multiprocessing.Event
-    stdin_fd: int
-    predetermined_input : multiprocessing.managers.SyncManager.list
-    """
-    sys.stdin = os.fdopen(stdin_fd)
-    config.predetermined_input = predetermined_input
-    try:
-        banner()
-        print(_('I will enter every day.'))
-        enter()
-    except KeyboardInterrupt:
-        event.set()
-        return
-
-    set_child_mode(session)
-    event.set()
-
-    info = _('\nI enter every day\n')
-    setInfoSignal(session, info)
-    try:
-        do_it(session)
-    except Exception as e:
-        msg = _('Error in:\n{}\nCause:\n{}').format(info, traceback.format_exc())
-        sendToBot(session, msg)
-    finally:
-        session.logout()
+    city : dict
+    """
+    url = "view=branchOffice&cityId={}&position={:d}&currentCityId={}&backgroundView=city&actionRequest={}&ajax=1".format(
+        city["id"], city["pos"], city["id"], actionRequest
+    )
+    data = session.post(url)
+    json_data = json.loads(data, strict=False)
+    return json_data[1][1][1]
+
+
+def storageCapacityOfMarket(html):
+    match = re.search(r"var\s*storageCapacity\s*=\s*(\d+);", html)
+    if match:
+        return int(match.group(1))
+    else:
+        return 0
+
+
+def onSellInMarket(html):
+    mad, vin, mar, cri, azu = re.findall(
+        r'<input type="text" class="textfield"\s*size="\d+"\s*name=".*?"\s*id=".*?"\s*value="(\d+)"',
+        html,
+    )
+    return [int(mad), int(vin), int(mar), int(cri), int(azu)]
 
 
-def do_it(session):
+def getGold(session, city):
     """
     Parameters
     ----------
     session : ikabot.web.session.Session
+    city : dict
+    Returns
+    -------
+    gold : int
     """
-    while True:
-        (ids, cities) = getIdsOfCities(session)
-        for id in ids:
-            html = session.post(city_url + str(id))
-            if 'class="fountain' in html:
-                url = 'action=AvatarAction&function=giveDailyActivityBonus&dailyActivityBonusCitySelect={0}&startPageShown=1&detectedDevice=1&autoLogin=on&cityId={0}&activeTab=multiTab2&backgroundView=city&currentCityId={0}&actionRequest={1}&ajax=1'.format(id, actionRequest)
-                session.post(url)
-                if 'class="fountain_active' in html:
-                    url = 'action=AmbrosiaFountainActions&function=collect&backgroundView=city&currentCityId={0}&templateView=ambrosiaFountain&actionRequest={1}&ajax=1'.format(id, actionRequest)
-                    session.post(url)
-                break
-        session.setStatus(f'Last login @{getDateTime()}')
-        wait(24*60*60, 60)
+    url = "view=finances&backgroundView=city&currentCityId={}&templateView=finances&actionRequest={}&ajax=1".format(
+        city["id"], actionRequest
+    )
+    data = session.post(url)
+    json_data = json.loads(data, strict=False)
+    gold = json_data[0][1]["headerData"]["gold"]
+    gold = gold.split(".")[0]
+    gold = int(gold)
+    gold_production = (
+        json_data[0][1]["headerData"]["scientistsUpkeep"]
+        + json_data[0][1]["headerData"]["income"]
+        + json_data[0][1]["headerData"]["upkeep"]
+    )
+    return gold, int(gold_production)
```

### Comparing `ikabot-6.6.4/ikabot/function/searchForIslandSpaces.py` & `ikabot-7.0.1/ikabot/function/searchForIslandSpaces.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 #! /usr/bin/env python3
 # -*- coding: utf-8 -*-
 
-import time
 import gettext
-import traceback
 import sys
+import time
+import traceback
+
 from ikabot.config import *
 from ikabot.helpers.botComm import *
-from ikabot.helpers.gui import enter, enter
-from ikabot.helpers.varios import wait, getDateTime
-from ikabot.helpers.signals import setInfoSignal
-from ikabot.helpers.pedirInfo import getIslandsIds
 from ikabot.helpers.getJson import getIsland
+from ikabot.helpers.gui import enter
+from ikabot.helpers.pedirInfo import getIslandsIds
 from ikabot.helpers.process import set_child_mode
+from ikabot.helpers.signals import setInfoSignal
+from ikabot.helpers.varios import getDateTime, wait
 
-t = gettext.translation('searchForIslandSpaces', localedir, languages=languages, fallback=True)
+t = gettext.translation(
+    "searchForIslandSpaces", localedir, languages=languages, fallback=True
+)
 _ = t.gettext
 
 
 def searchForIslandSpaces(session, event, stdin_fd, predetermined_input):
     """
     Parameters
     ----------
@@ -30,60 +33,68 @@
     sys.stdin = os.fdopen(stdin_fd)
     config.predetermined_input = predetermined_input
     try:
         if checkTelegramData(session) is False:
             event.set()
             return
         banner()
-        print('Do you want to search for spaces on your islands or a specific set of islands?')
-        print('(0) Exit')
-        print('(1) Search all islands I have colonised')
-        print('(2) Search a specific set of islands')
+        print(
+            "Do you want to search for spaces on your islands or a specific set of islands?"
+        )
+        print("(0) Exit")
+        print("(1) Search all islands I have colonised")
+        print("(2) Search a specific set of islands")
         choice = read(min=0, max=2)
         islandList = []
         if choice == 0:
             event.set()
             return
         elif choice == 2:
             banner()
-            print('Insert the coordinates of each island you want searched like so: X1:Y1, X2:Y2, X3:Y3...')
+            print(
+                "Insert the coordinates of each island you want searched like so: X1:Y1, X2:Y2, X3:Y3..."
+            )
             coords_string = read()
-            coords_string = coords_string.replace(' ', '')
-            coords = coords_string.split(',')
+            coords_string = coords_string.replace(" ", "")
+            coords = coords_string.split(",")
             for coord in coords:
-                coord = '&xcoord=' + coord
-                coord = coord.replace(':', '&ycoord=')
-                html = session.get('view=island' + coord)
+                coord = "&xcoord=" + coord
+                coord = coord.replace(":", "&ycoord=")
+                html = session.get("view=island" + coord)
                 island = getIsland(html)
-                islandList.append(island['id'])
+                islandList.append(island["id"])
         else:
             pass
 
         banner()
-        print('How frequently should the islands be searched in minutes (minimum is 3)?')
+        print(
+            "How frequently should the islands be searched in minutes (minimum is 3)?"
+        )
         time = read(min=3, digit=True)
         banner()
-        print('Do you wish to be notified when a fight breaks out and stops on a city on these islands? (Y|N)')
-        fights = read(values=['y', 'Y', 'n', 'N'])
+        print(
+            "Do you wish to be notified when a fight breaks out and stops on a city on these islands? (Y|N)"
+        )
+        fights = read(values=["y", "Y", "n", "N"])
         banner()
-        print(_('I will search for changes in the selected islands'))
+        print(_("I will search for changes in the selected islands"))
         enter()
     except KeyboardInterrupt:
         event.set()
         return
 
     set_child_mode(session)
     event.set()
 
-    info = _('\nI search for new spaces each hour\n')
+    info = _("\nI search for new spaces each hour\n")
     setInfoSignal(session, info)
     try:
         do_it(session, islandList, time, fights)
     except Exception as e:
-        msg = _('Error in:\n{}\nCause:\n{}').format(info, traceback.format_exc())
+        msg = _("Error in:\n{}\nCause:\n{}").format(info, traceback.format_exc())
         sendToBot(session, msg)
     finally:
         session.logout()
 
 
 def do_it(session, islandList, time, fights):
     """
@@ -109,43 +120,101 @@
             islandsIds = islandList
         else:
             islandsIds = getIslandsIds(session)
         for islandId in islandsIds:
             html = session.get(island_url + islandId)
             island = getIsland(html)
             # cities in the current island
-            cities_now = [city_space for city_space in island['cities'] if city_space['type'] != 'empty']  # loads the islands non empty cities into ciudades
+            cities_now = [
+                city_space
+                for city_space in island["cities"]
+                if city_space["type"] != "empty"
+            ]  # loads the islands non empty cities into ciudades
 
             # if we haven't scaned this island before,
             # save it and do nothing
             if islandId not in cities_before_per_island:
                 cities_before_per_island[islandId] = cities_now.copy()
             else:
                 cities_before = cities_before_per_island[islandId]
 
                 # someone disappeared
                 for city_before in cities_before:
-                    if city_before['id'] not in [city_now['id'] for city_now in cities_now]:
+                    if city_before["id"] not in [
+                        city_now["id"] for city_now in cities_now
+                    ]:
                         # we didn't find the city_before in the cities_now
-                        msg = _('The city {} of the player {} disappeared in {} {}:{} {}').format(city_before['name'], city_before['Name'], materials_names[int(island['tradegood'])], island['x'], island['y'], island['name'])
+                        msg = _(
+                            "The city {} of the player {} disappeared in {} {}:{} {}"
+                        ).format(
+                            city_before["name"],
+                            city_before["Name"],
+                            materials_names[int(island["tradegood"])],
+                            island["x"],
+                            island["y"],
+                            island["name"],
+                        )
                         sendToBot(session, msg)
 
-                    if fights.lower() == 'y':
+                    if fights.lower() == "y":
                         for city_now in cities_now:
-                            if city_now['id'] == city_before['id']:
-                                if 'infos' in city_now and 'infos' not in city_before and 'armyAction' in city_now['infos'] and city_now['infos']['armyAction'] == 'fight':
-                                    msg = _('A fight started in the city {} of the player {} on island {} {}:{} {}').format(city_before['name'], city_before['Name'], materials_names[int(island['tradegood'])], island['x'], island['y'], island['name'])
+                            if city_now["id"] == city_before["id"]:
+                                if (
+                                    "infos" in city_now
+                                    and "infos" not in city_before
+                                    and "armyAction" in city_now["infos"]
+                                    and city_now["infos"]["armyAction"] == "fight"
+                                ):
+                                    msg = _(
+                                        "A fight started in the city {} of the player {} on island {} {}:{} {}"
+                                    ).format(
+                                        city_before["name"],
+                                        city_before["Name"],
+                                        materials_names[int(island["tradegood"])],
+                                        island["x"],
+                                        island["y"],
+                                        island["name"],
+                                    )
                                     sendToBot(session, msg)
-                                if 'infos' not in city_now and 'infos' in city_before and 'armyAction' in city_before['infos'] and city_before['infos']['armyAction'] == 'fight':
-                                    msg = _('A fight stopped in the city {} of the player {} on island {} {}:{} {}').format(city_before['name'], city_before['Name'], materials_names[int(island['tradegood'])], island['x'], island['y'], island['name'])
+                                if (
+                                    "infos" not in city_now
+                                    and "infos" in city_before
+                                    and "armyAction" in city_before["infos"]
+                                    and city_before["infos"]["armyAction"] == "fight"
+                                ):
+                                    msg = _(
+                                        "A fight stopped in the city {} of the player {} on island {} {}:{} {}"
+                                    ).format(
+                                        city_before["name"],
+                                        city_before["Name"],
+                                        materials_names[int(island["tradegood"])],
+                                        island["x"],
+                                        island["y"],
+                                        island["name"],
+                                    )
                                     sendToBot(session, msg)
 
                 # someone colonised
                 for city_now in cities_now:
-                    if city_now['id'] not in [city_before['id'] for city_before in cities_before]:
+                    if city_now["id"] not in [
+                        city_before["id"] for city_before in cities_before
+                    ]:
                         # we didn't find the city_now in the cities_before
-                        msg = _('Player {} created a new city {} in {} {}:{} {}').format(city_now['Name'], city_now['name'], materials_names[int(island['tradegood'])], island['x'], island['y'], island['name'])
+                        msg = _(
+                            "Player {} created a new city {} in {} {}:{} {}"
+                        ).format(
+                            city_now["Name"],
+                            city_now["name"],
+                            materials_names[int(island["tradegood"])],
+                            island["x"],
+                            island["y"],
+                            island["name"],
+                        )
                         sendToBot(session, msg)
-                        
-                cities_before_per_island[islandId] = cities_now.copy() # update cities_before_per_island for the current island
-        session.setStatus(f'Checked islands {str([int(i) for i in islandsIds]).replace(" ","")} @ {getDateTime()[-8:]}')
+
+                cities_before_per_island[islandId] = (
+                    cities_now.copy()
+                )  # update cities_before_per_island for the current island
+        session.setStatus(
+            f'Checked islands {str([int(i) for i in islandsIds]).replace(" ","")} @ {getDateTime()[-8:]}'
+        )
         wait(time * 60)
```

### Comparing `ikabot-6.6.4/ikabot/function/sellResources.py` & `ikabot-7.0.1/ikabot/function/sellResources.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,44 +1,45 @@
 #! /usr/bin/env python3
 # -*- coding: utf-8 -*-
 
-import time
-import math
-import json
 import gettext
+import json
+import math
+import time
 import traceback
 from decimal import *
+
 from ikabot.config import *
+from ikabot.helpers.botComm import *
 from ikabot.helpers.gui import *
 from ikabot.helpers.market import *
-from ikabot.helpers.botComm import *
 from ikabot.helpers.naval import getTotalShips
-from ikabot.helpers.varios import addThousandSeparator, wait
 from ikabot.helpers.pedirInfo import read
-from ikabot.helpers.signals import setInfoSignal
-from ikabot.helpers.process import set_child_mode
 from ikabot.helpers.planRoutes import waitForArrival
+from ikabot.helpers.process import set_child_mode
+from ikabot.helpers.signals import setInfoSignal
+from ikabot.helpers.varios import addThousandSeparator, wait
 
-t = gettext.translation('sellResources', localedir, languages=languages, fallback=True)
+t = gettext.translation("sellResources", localedir, languages=languages, fallback=True)
 _ = t.gettext
 
 
 def chooseCommercialCity(commercial_cities):
     """
     Parameters
     ----------
     commercial_cities : list[dict]
 
     Returns
     -------
     commercial_city : dict
     """
-    print(_('In which city do you want to sell resources?\n'))
+    print(_("In which city do you want to sell resources?\n"))
     for i, city in enumerate(commercial_cities):
-        print('({:d}) {}'.format(i + 1, city['name']))
+        print("({:d}) {}".format(i + 1, city["name"]))
     ind = read(min=1, max=len(commercial_cities))
     return commercial_cities[ind - 1]
 
 
 def getMarketInfo(session, city):
     """
     Parameters
@@ -46,15 +47,26 @@
     session : ikabot.web.session.Session
     city : dict
 
     Returns
     -------
     response : dict
     """
-    params = {'view': 'branchOfficeOwnOffers', 'activeTab': 'tab_branchOfficeOwnOffers', 'cityId': city['id'], 'position': city['pos'], 'backgroundView': 'city', 'currentCityId': city['id'], 'templateView': 'branchOfficeOwnOffers', 'currentTab': 'tab_branchOfficeOwnOffers', 'actionRequest': actionRequest, 'ajax': '1'}
+    params = {
+        "view": "branchOfficeOwnOffers",
+        "activeTab": "tab_branchOfficeOwnOffers",
+        "cityId": city["id"],
+        "position": city["pos"],
+        "backgroundView": "city",
+        "currentCityId": city["id"],
+        "templateView": "branchOfficeOwnOffers",
+        "currentTab": "tab_branchOfficeOwnOffers",
+        "actionRequest": actionRequest,
+        "ajax": "1",
+    }
     resp = session.post(params=params, noIndex=True)
     return json.loads(resp, strict=False)[1][1][1]
 
 
 def getOffers(session, my_market_city, resource_type):
     """
     Parameters
@@ -64,21 +76,38 @@
     resource_type : int
 
     Returns
     -------
     offers : list
     """
     if resource_type == 0:
-        resource_type = 'resource'
+        resource_type = "resource"
     else:
         resource_type = str(resource_type)
-    data = {'cityId': my_market_city['id'], 'position': my_market_city['pos'], 'view': 'branchOffice', 'activeTab': 'bargain', 'type': '333', 'searchResource': resource_type, 'range': my_market_city['rango'], 'backgroundView': 'city', 'currentCityId': my_market_city['id'], 'templateView': 'branchOffice', 'currentTab': 'bargain', 'actionRequest': actionRequest, 'ajax': '1'}
+    data = {
+        "cityId": my_market_city["id"],
+        "position": my_market_city["pos"],
+        "view": "branchOffice",
+        "activeTab": "bargain",
+        "type": "333",
+        "searchResource": resource_type,
+        "range": my_market_city["rango"],
+        "backgroundView": "city",
+        "currentCityId": my_market_city["id"],
+        "templateView": "branchOffice",
+        "currentTab": "bargain",
+        "actionRequest": actionRequest,
+        "ajax": "1",
+    }
     resp = session.post(params=data)
     html = json.loads(resp, strict=False)[1][1][1]
-    return re.findall(r'<td class=".*?">(.*?)<br/>\((.*?)\)\s*</td>\s*<td>(.*?)</td>\s*<td><img src=".*?"\s*alt=".*?"\s*title=".*?"/></td>\s*<td style="white-space:nowrap;">(\d+)\s*<img src=".*?"\s*class=".*?"/>.*?</td>\s*<td>(\d+)</td>\s*<td><a onclick="ajaxHandlerCall\(this\.href\);return false;"\s*href="\?view=takeOffer&destinationCityId=(\d+)&', html)
+    return re.findall(
+        r'<td class=".*?">(.*?)<br/>\((.*?)\)\s*</td>\s*<td>(.*?)</td>\s*<td><img src=".*?"\s*alt=".*?"\s*title=".*?"/></td>\s*<td style="white-space:nowrap;">(\d+)\s*<img src=".*?"\s*class=".*?"/>.*?</td>\s*<td>(\d+)</td>\s*<td><a onclick="ajaxHandlerCall\(this\.href\);return false;"\s*href="\?view=takeOffer&destinationCityId=(\d+)&',
+        html,
+    )
 
 
 def sellToOffers(session, city_to_buy_from, resource_type, event):
     """
     Parameters
     ----------
     session : ikabot.web.session.Session
@@ -87,78 +116,98 @@
     event : multiprocessing.Event
     """
     banner()
 
     offers = getOffers(session, city_to_buy_from, resource_type)
 
     if len(offers) == 0:
-        print(_('No offers available.'))
+        print(_("No offers available."))
         enter()
         event.set()
         return
 
-    print(_('Which offers do you want to sell to?\n'))
+    print(_("Which offers do you want to sell to?\n"))
 
     chosen_offers = []
     total_amount = 0
     profit = 0
     for offer in offers:
         cityname, username, amount, price, dist, destination_city_id = offer
         cityname = cityname.strip()
-        amount = amount.replace(',', '').replace('.', '')
+        amount = amount.replace(",", "").replace(".", "")
         amount = int(amount)
         price = int(price)
-        msg = _('{} ({}): {} at {:d} each ({} in total) [Y/n]').format(cityname, username, addThousandSeparator(amount), price, addThousandSeparator(price*amount))
-        rta = read(msg=msg, values=['y', 'Y', 'n', 'N', ''])
-        if rta.lower() == 'n':
+        msg = _("{} ({}): {} at {:d} each ({} in total) [Y/n]").format(
+            cityname,
+            username,
+            addThousandSeparator(amount),
+            price,
+            addThousandSeparator(price * amount),
+        )
+        rta = read(msg=msg, values=["y", "Y", "n", "N", ""])
+        if rta.lower() == "n":
             continue
         chosen_offers.append(offer)
         total_amount += amount
         profit += amount * price
 
     if len(chosen_offers) == 0:
         event.set()
         return
 
-    available = city_to_buy_from['recursos'][resource_type]
+    available = city_to_buy_from["availableResources"][resource_type]
     amount_to_sell = min(available, total_amount)
 
     banner()
-    print(_('\nHow much do you want to sell? [max = {}]').format(addThousandSeparator(amount_to_sell)))
+    print(
+        _("\nHow much do you want to sell? [max = {}]").format(
+            addThousandSeparator(amount_to_sell)
+        )
+    )
     amount_to_sell = read(min=0, max=amount_to_sell)
     if amount_to_sell == 0:
         event.set()
         return
 
     left_to_sell = amount_to_sell
     profit = 0
     for offer in chosen_offers:
         cityname, username, amount, price, dist, destination_city_id = offer
         cityname = cityname.strip()
-        amount = amount.replace(',', '').replace('.', '')
+        amount = amount.replace(",", "").replace(".", "")
         amount = int(amount)
         price = int(price)
         sell = min(amount, left_to_sell)
         left_to_sell -= sell
         profit += sell * price
-    print(_('\nSell {} of {} for a total of {}? [Y/n]').format(addThousandSeparator(amount_to_sell), materials_names[resource_type], addThousandSeparator(profit)))
-    rta = read(values=['y', 'Y', 'n', 'N', ''])
-    if rta.lower() == 'n':
+    print(
+        _("\nSell {} of {} for a total of {}? [Y/n]").format(
+            addThousandSeparator(amount_to_sell),
+            materials_names[resource_type],
+            addThousandSeparator(profit),
+        )
+    )
+    rta = read(values=["y", "Y", "n", "N", ""])
+    if rta.lower() == "n":
         event.set()
         return
 
     set_child_mode(session)
     event.set()
 
-    info = _('\nI sell {} of {} in {}\n').format(addThousandSeparator(amount_to_sell), materials_names[resource_type], city_to_buy_from['name'])
+    info = _("\nI sell {} of {} in {}\n").format(
+        addThousandSeparator(amount_to_sell),
+        materials_names[resource_type],
+        city_to_buy_from["name"],
+    )
     setInfoSignal(session, info)
     try:
         do_it1(session, amount_to_sell, chosen_offers, resource_type, city_to_buy_from)
     except Exception as e:
-        msg = _('Error in:\n{}\nCause:\n{}').format(info, traceback.format_exc())
+        msg = _("Error in:\n{}\nCause:\n{}").format(info, traceback.format_exc())
         sendToBot(session, msg)
     finally:
         session.logout()
 
 
 def createOffer(session, my_offering_market_city, resource_type, event):
     """
@@ -169,44 +218,70 @@
     resource_type : int
     event : multiprocessing.Event
     """
     banner()
 
     html = getMarketInfo(session, my_offering_market_city)
     sell_market_capacity = storageCapacityOfMarket(html)
-    total_available_amount_of_resource = my_offering_market_city['recursos'][resource_type]
-
-    print(_('How much do you want to sell? [max = {}]').format(addThousandSeparator(total_available_amount_of_resource)))
+    total_available_amount_of_resource = my_offering_market_city["availableResources"][
+        resource_type
+    ]
+
+    print(
+        _("How much do you want to sell? [max = {}]").format(
+            addThousandSeparator(total_available_amount_of_resource)
+        )
+    )
     amount_to_sell = read(min=0, max=total_available_amount_of_resource)
     if amount_to_sell == 0:
         event.set()
         return
 
-    price_max, price_min = re.findall(r'\'upper\': (\d+),\s*\'lower\': (\d+)', html)[resource_type]
+    price_max, price_min = re.findall(r"\'upper\': (\d+),\s*\'lower\': (\d+)", html)[
+        resource_type
+    ]
     price_max = int(price_max)
     price_min = int(price_min)
-    print(_('\nAt what price? [min = {:d}, max = {:d}]').format(price_min, price_max))
+    print(_("\nAt what price? [min = {:d}, max = {:d}]").format(price_min, price_max))
     price = read(min=price_min, max=price_max)
 
-    print(_('\nI will sell {} of {} at {}: {}').format(addThousandSeparator(amount_to_sell), materials_names[resource_type], addThousandSeparator(price), addThousandSeparator(price * amount_to_sell)))
-    print(_('\nProceed? [Y/n]'))
-    rta = read(values=['y', 'Y', 'n', 'N', ''])
-    if rta.lower() == 'n':
+    print(
+        _("\nI will sell {} of {} at {}: {}").format(
+            addThousandSeparator(amount_to_sell),
+            materials_names[resource_type],
+            addThousandSeparator(price),
+            addThousandSeparator(price * amount_to_sell),
+        )
+    )
+    print(_("\nProceed? [Y/n]"))
+    rta = read(values=["y", "Y", "n", "N", ""])
+    if rta.lower() == "n":
         event.set()
         return
 
     set_child_mode(session)
     event.set()
 
-    info = _('\nI sell {} of {} in {}\n').format(addThousandSeparator(amount_to_sell), materials_names[resource_type], my_offering_market_city['name'])
+    info = _("\nI sell {} of {} in {}\n").format(
+        addThousandSeparator(amount_to_sell),
+        materials_names[resource_type],
+        my_offering_market_city["name"],
+    )
     setInfoSignal(session, info)
     try:
-        do_it2(session, amount_to_sell, price, resource_type, sell_market_capacity, my_offering_market_city)
+        do_it2(
+            session,
+            amount_to_sell,
+            price,
+            resource_type,
+            sell_market_capacity,
+            my_offering_market_city,
+        )
     except Exception as e:
-        msg = _('Error in:\n{}\nCause:\n{}').format(info, traceback.format_exc())
+        msg = _("Error in:\n{}\nCause:\n{}").format(info, traceback.format_exc())
         sendToBot(session, msg)
     finally:
         session.logout()
 
 
 def sellResources(session, event, stdin_fd, predetermined_input):
     """
@@ -220,33 +295,37 @@
     sys.stdin = os.fdopen(stdin_fd)
     config.predetermined_input = predetermined_input
     try:
         banner()
 
         commercial_cities = getCommercialCities(session)
         if len(commercial_cities) == 0:
-            print(_('There is no store built'))
+            print(_("There is no store built"))
             enter()
             event.set()
             return
 
         if len(commercial_cities) == 1:
             city = commercial_cities[0]
         else:
             city = chooseCommercialCity(commercial_cities)
             banner()
 
-        print(_('What resource do you want to sell?'))
+        print(_("What resource do you want to sell?"))
         for index, material_name in enumerate(materials_names):
-            print('({:d}) {}'.format(index+1, material_name))
+            print("({:d}) {}".format(index + 1, material_name))
         selected_material = read(min=1, max=len(materials_names))
         resource = selected_material - 1
         banner()
 
-        print(_('Do you want to sell to existing offers (1) or do you want to make your own offer (2)?'))
+        print(
+            _(
+                "Do you want to sell to existing offers (1) or do you want to make your own offer (2)?"
+            )
+        )
         selected = read(min=1, max=2)
         [sellToOffers, createOffer][selected - 1](session, city, resource, event)
     except KeyboardInterrupt:
         event.set()
         return
 
 
@@ -259,35 +338,59 @@
     offers : list[dict]
     resource_type : int
     city_to_buy_from : dict
     """
     for offer in offers:
         cityname, username, amount, precio, dist, destination_city_id = offer
         cityname = cityname.strip()
-        amount_to_buy = amount.replace(',', '').replace('.', '')
+        amount_to_buy = amount.replace(",", "").replace(".", "")
         amount_to_buy = int(amount_to_buy)
         while True:
             amount_to_sell = min(amount_to_buy, left_to_sell)
             ships_available = waitForArrival(session)
             ships_needed = math.ceil((Decimal(amount_to_sell) / Decimal(500)))
             ships_used = min(ships_available, ships_needed)
             if ships_needed > ships_used:
                 amount_to_sell = ships_used * 500
             left_to_sell -= amount_to_sell
             amount_to_buy -= amount_to_sell
 
-            data = {'action': 'transportOperations', 'function': 'sellGoodsAtAnotherBranchOffice', 'cityId': city_to_buy_from['id'], 'destinationCityId': destination_city_id, 'oldView': 'branchOffice', 'position': city_to_buy_from['pos'], 'avatar2Name': username, 'city2Name': cityname, 'type': '333', 'activeTab': 'bargain', 'transportDisplayPrice': '0', 'premiumTransporter': '0', 'normalTransportersMax': ships_available, 'capacity': '5', 'max_capacity': '5', 'jetPropulsion': '0', 'transporters': str(ships_used), 'backgroundView': 'city', 'currentCityId': city_to_buy_from['id'], 'templateView': 'takeOffer', 'currentTab': 'bargain', 'actionRequest': actionRequest, 'ajax': '1'}
+            data = {
+                "action": "transportOperations",
+                "function": "sellGoodsAtAnotherBranchOffice",
+                "cityId": city_to_buy_from["id"],
+                "destinationCityId": destination_city_id,
+                "oldView": "branchOffice",
+                "position": city_to_buy_from["pos"],
+                "avatar2Name": username,
+                "city2Name": cityname,
+                "type": "333",
+                "activeTab": "bargain",
+                "transportDisplayPrice": "0",
+                "premiumTransporter": "0",
+                "normalTransportersMax": ships_available,
+                "capacity": "5",
+                "max_capacity": "5",
+                "jetPropulsion": "0",
+                "transporters": str(ships_used),
+                "backgroundView": "city",
+                "currentCityId": city_to_buy_from["id"],
+                "templateView": "takeOffer",
+                "currentTab": "bargain",
+                "actionRequest": actionRequest,
+                "ajax": "1",
+            }
             if resource_type == 0:
-                data['cargo_resource'] = amount_to_sell
-                data['resourcePrice'] = precio
+                data["cargo_resource"] = amount_to_sell
+                data["resourcePrice"] = precio
             else:
-                data['tradegood{:d}Price'.format(resource_type)] = precio
-                data['cargo_tradegood{:d}'.format(resource_type)] = amount_to_sell
+                data["tradegood{:d}Price".format(resource_type)] = precio
+                data["cargo_tradegood{:d}".format(resource_type)] = amount_to_sell
 
-            session.get(city_url + city_to_buy_from['id'], noIndex=True)
+            session.get(city_url + city_to_buy_from["id"], noIndex=True)
             session.post(params=data)
 
             if left_to_sell == 0:
                 return
             if amount_to_buy == 0:
                 break
 
@@ -313,34 +416,64 @@
         if currently_on_sell < storageCapacityOfMarket(html):
             # add our new offer to the free space
             free_space = sell_market_capacity - currently_on_sell
             offer = min(amount_to_sell, free_space)
             amount_to_sell -= offer
             new_offer = currently_on_sell + offer
 
-            payloadPost = {'cityId': city['id'], 'position': city['pos'], 'action': 'CityScreen', 'function': 'updateOffers', 'resourceTradeType': '444', 'resource': '0', 'resourcePrice': '10', 'tradegood1TradeType': '444', 'tradegood1': '0', 'tradegood1Price': '11', 'tradegood2TradeType': '444', 'tradegood2': '0', 'tradegood2Price': '12', 'tradegood3TradeType': '444', 'tradegood3': '0', 'tradegood3Price': '17', 'tradegood4TradeType': '444', 'tradegood4': '0', 'tradegood4Price': '5', 'backgroundView': 'city', 'currentCityId': city['id'], 'templateView': 'branchOfficeOwnOffers', 'currentTab': 'tab_branchOfficeOwnOffers', 'actionRequest': actionRequest, 'ajax': '1'}
+            payloadPost = {
+                "cityId": city["id"],
+                "position": city["pos"],
+                "action": "CityScreen",
+                "function": "updateOffers",
+                "resourceTradeType": "444",
+                "resource": "0",
+                "resourcePrice": "10",
+                "tradegood1TradeType": "444",
+                "tradegood1": "0",
+                "tradegood1Price": "11",
+                "tradegood2TradeType": "444",
+                "tradegood2": "0",
+                "tradegood2Price": "12",
+                "tradegood3TradeType": "444",
+                "tradegood3": "0",
+                "tradegood3Price": "17",
+                "tradegood4TradeType": "444",
+                "tradegood4": "0",
+                "tradegood4Price": "5",
+                "backgroundView": "city",
+                "currentCityId": city["id"],
+                "templateView": "branchOfficeOwnOffers",
+                "currentTab": "tab_branchOfficeOwnOffers",
+                "actionRequest": actionRequest,
+                "ajax": "1",
+            }
             if resource_type == 0:
-                payloadPost['resource'] = new_offer
-                payloadPost['resourcePrice'] = price
+                payloadPost["resource"] = new_offer
+                payloadPost["resourcePrice"] = price
             else:
-                payloadPost['tradegood{:d}'.format(resource_type)] = new_offer
-                payloadPost['tradegood{:d}Price'.format(resource_type)] = price
+                payloadPost["tradegood{:d}".format(resource_type)] = new_offer
+                payloadPost["tradegood{:d}Price".format(resource_type)] = price
             session.post(params=payloadPost)
 
             # if we don't have any more to add to the offer, leave the loop
             if amount_to_sell == 0:
                 break
 
         # sleep for 2 hours
         wait(60 * 60 * 2)
 
     # wait until the last of our offer is actualy bought, and let the user know
     while True:
         html = getMarketInfo(session, city)
         currently_on_sell = onSellInMarket(html)[resource_type]
         if currently_on_sell <= previous_on_sell:
-            msg = _('{} of {} was sold at {:d}').format(addThousandSeparator(initial_amount_to_sell), materials_names[resource_type], price)
+            msg = _("{} of {} was sold at {:d}").format(
+                addThousandSeparator(initial_amount_to_sell),
+                materials_names[resource_type],
+                price,
+            )
             sendToBot(session, msg)
             return
 
         # sleep for 2 hours
         wait(60 * 60 * 2)
```

### Comparing `ikabot-6.6.4/ikabot/function/sendResources.py` & `ikabot-7.0.1/ikabot/function/sendResources.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 #! /usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 import gettext
 import traceback
+
 from ikabot.config import *
-from ikabot.helpers.gui import *
 from ikabot.helpers.botComm import *
+from ikabot.helpers.getJson import getCity
+from ikabot.helpers.gui import *
 from ikabot.helpers.pedirInfo import *
 from ikabot.helpers.planRoutes import executeRoutes
-from ikabot.helpers.signals import setInfoSignal
-from ikabot.helpers.getJson import getCity
 from ikabot.helpers.process import set_child_mode
-from ikabot.helpers.varios import addThousandSeparator
 from ikabot.helpers.resources import *
+from ikabot.helpers.signals import setInfoSignal
+from ikabot.helpers.varios import addThousandSeparator
 
-t = gettext.translation('sendResources', localedir, languages=languages, fallback=True)
+t = gettext.translation("sendResources", localedir, languages=languages, fallback=True)
 _ = t.gettext
 
 
 def sendResources(session, event, stdin_fd, predetermined_input):
     """
     Parameters
     ----------
@@ -30,102 +31,121 @@
     sys.stdin = os.fdopen(stdin_fd)
     config.predetermined_input = predetermined_input
     try:
         routes = []
         while True:
 
             banner()
-            print(_('Origin city:'))
+            print(_("Origin city:"))
             try:
                 cityO = chooseCity(session)
             except KeyboardInterrupt:
                 if routes:
-                    print(_('Send shipment? [Y/n]'))
-                    rta = read(values=['y', 'Y', 'n', 'N', ''])
-                    if rta.lower() != 'n':
+                    print(_("Send shipment? [Y/n]"))
+                    rta = read(values=["y", "Y", "n", "N", ""])
+                    if rta.lower() != "n":
                         break
                 event.set()
                 return
 
             banner()
-            print(_('Destination city'))
+            print(_("Destination city"))
             cityD = chooseCity(session, foreign=True)
-            idIsland = cityD['islandId']
+            idIsland = cityD["islandId"]
 
-            if cityO['id'] == cityD['id']:
+            if cityO["id"] == cityD["id"]:
                 continue
 
-            resources_left = cityO['recursos']
+            resources_left = cityO["availableResources"]
             for route in routes:
                 (origin_city, destination_city, __, *toSend) = route
-                if origin_city['id'] == cityO['id']:
+                if origin_city["id"] == cityO["id"]:
                     for i in range(len(materials_names)):
                         resources_left[i] -= toSend[i]
 
                 # the destination city might be from another player
-                if cityD['propia'] and destination_city['id'] == cityD['id']:
+                if cityD["isOwnCity"] and destination_city["id"] == cityD["id"]:
                     for i in range(len(materials_names)):
-                        cityD['freeSpaceForResources'][i] -= toSend[i]
+                        cityD["freeSpaceForResources"][i] -= toSend[i]
 
             banner()
             # the destination city might be from another player
-            if cityD['propia']:
-                msg = ''
+            if cityD["isOwnCity"]:
+                msg = ""
                 for i in range(len(materials_names)):
-                    if resources_left[i] > cityD['freeSpaceForResources'][i]:
-                        msg += '{} more {}\n'.format(addThousandSeparator(cityD['freeSpaceForResources'][i]), materials_names[i].lower())
+                    if resources_left[i] > cityD["freeSpaceForResources"][i]:
+                        msg += "{} more {}\n".format(
+                            addThousandSeparator(cityD["freeSpaceForResources"][i]),
+                            materials_names[i].lower(),
+                        )
 
                 if len(msg) > 0:
-                    print(_('You can store just:\n{}').format(msg))
+                    print(_("You can store just:\n{}").format(msg))
 
-            print(_('Available:'))
+            print(_("Available:"))
             for i in range(len(materials_names)):
-                print('{}:{} '.format(materials_names[i], addThousandSeparator(resources_left[i])), end='')
-            print('')
+                print(
+                    "{}:{} ".format(
+                        materials_names[i], addThousandSeparator(resources_left[i])
+                    ),
+                    end="",
+                )
+            print("")
 
-            print(_('Send:'))
+            print(_("Send:"))
             try:
                 max_name = max([len(material) for material in materials_names])
                 send = []
                 for i in range(len(materials_names)):
                     material_name = materials_names[i]
-                    pad = ' ' * (max_name - len(material_name))
-                    val = askForValue(_('{}{}:'.format(pad, material_name)), resources_left[i])
+                    pad = " " * (max_name - len(material_name))
+                    val = askForValue(
+                        _("{}{}:".format(pad, material_name)), resources_left[i]
+                    )
                     send.append(val)
             except KeyboardInterrupt:
                 continue
             if sum(send) == 0:
                 continue
 
             banner()
-            print(_('About to send from {} to {}').format(cityO['cityName'], cityD['cityName']))
+            print(
+                _("About to send from {} to {}").format(
+                    cityO["cityName"], cityD["cityName"]
+                )
+            )
             for i in range(len(materials_names)):
                 if send[i] > 0:
-                    print('{}:{} '.format(materials_names[i], addThousandSeparator(send[i])), end='')
-            print('')
-
-            print(_('Proceed? [Y/n]'))
-            rta = read(values=['y', 'Y', 'n', 'N', ''])
-            if rta.lower() != 'n':
+                    print(
+                        "{}:{} ".format(
+                            materials_names[i], addThousandSeparator(send[i])
+                        ),
+                        end="",
+                    )
+            print("")
+
+            print(_("Proceed? [Y/n]"))
+            rta = read(values=["y", "Y", "n", "N", ""])
+            if rta.lower() != "n":
                 route = (cityO, cityD, idIsland, *send)
                 routes.append(route)
-                print(_('Create another shipment? [y/N]'))
-                rta = read(values=['y', 'Y', 'n', 'N', ''])
-                if rta.lower() != 'y':
+                print(_("Create another shipment? [y/N]"))
+                rta = read(values=["y", "Y", "n", "N", ""])
+                if rta.lower() != "y":
                     break
     except KeyboardInterrupt:
         event.set()
         return
 
     set_child_mode(session)
     event.set()
 
-    info = _('\nSend resources\n')
+    info = _("\nSend resources\n")
 
     setInfoSignal(session, info)
     try:
         executeRoutes(session, routes)
     except Exception as e:
-        msg = _('Error in:\n{}\nCause:\n{}').format(info, traceback.format_exc())
+        msg = _("Error in:\n{}\nCause:\n{}").format(info, traceback.format_exc())
         sendToBot(session, msg)
     finally:
         session.logout()
```

### Comparing `ikabot-6.6.4/ikabot/function/shipMovements.py` & `ikabot-7.0.1/ikabot/function/shipMovements.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,41 +1,42 @@
 #! /usr/bin/env python3
 # -*- coding: utf-8 -*-
 
-import re
-import math
-import json
 import gettext
+import json
+import math
+import re
 import sys
-from ikabot.helpers.pedirInfo import read
-from ikabot import config
 from decimal import *
+
+from ikabot import config
 from ikabot.config import *
 from ikabot.helpers.gui import *
 from ikabot.helpers.naval import *
+from ikabot.helpers.pedirInfo import read
 from ikabot.helpers.varios import *
 
-t = gettext.translation('shipMovements', localedir, languages=languages, fallback=True)
+t = gettext.translation("shipMovements", localedir, languages=languages, fallback=True)
 _ = t.gettext
 
 
 def isHostile(movement):
     """
     Parameters
     ----------
     movement : dict
 
     Returns
     -------
     is hostile : bool
     """
-    if movement['army']['amount']:
+    if movement["army"]["amount"]:
         return True
-    for mov in movement['fleet']['ships']:
-        if mov['cssClass'] != 'ship_transport':
+    for mov in movement["fleet"]["ships"]:
+        if mov["cssClass"] != "ship_transport":
             return True
     return False
 
 
 def shipMovements(session, event, stdin_fd, predetermined_input):
     """
     Parameters
@@ -46,71 +47,101 @@
     predetermined_input : multiprocessing.managers.SyncManager.list
     """
     sys.stdin = os.fdopen(stdin_fd)
     config.predetermined_input = predetermined_input
     try:
         banner()
 
-        print(_('Ships {:d}/{:d}\n').format(getAvailableShips(session), getTotalShips(session)))
+        print(
+            _("Ships {:d}/{:d}\n").format(
+                getAvailableShips(session), getTotalShips(session)
+            )
+        )
 
         cityId = getCurrentCityId(session)
-        url = 'view=militaryAdvisor&oldView=city&oldBackgroundView=city&backgroundView=city&currentCityId={}&actionRequest={}&ajax=1'.format(cityId, actionRequest)
+        url = "view=militaryAdvisor&oldView=city&oldBackgroundView=city&backgroundView=city&currentCityId={}&actionRequest={}&ajax=1".format(
+            cityId, actionRequest
+        )
         resp = session.post(url)
         resp = json.loads(resp, strict=False)
-        movements = resp[1][1][2]['viewScriptParams']['militaryAndFleetMovements']
-        time_now = int(resp[0][1]['time'])
+        movements = resp[1][1][2]["viewScriptParams"]["militaryAndFleetMovements"]
+        time_now = int(resp[0][1]["time"])
 
         if len(movements) == 0:
-            print(_('There are no movements'))
+            print(_("There are no movements"))
             enter()
             event.set()
             return
 
         for movement in movements:
 
-            color = ''
-            if movement['isHostile']:
+            color = ""
+            if movement["isHostile"]:
                 color = bcolors.RED + bcolors.BOLD
-            elif movement['isOwnArmyOrFleet']:
+            elif movement["isOwnArmyOrFleet"]:
                 color = bcolors.BLUE + bcolors.BOLD
-            elif movement['isSameAlliance']:
+            elif movement["isSameAlliance"]:
                 color = bcolors.GREEN + bcolors.BOLD
 
-            origin = '{} ({})'.format(movement['origin']['name'], movement['origin']['avatarName'])
-            destination = '{} ({})'.format(movement['target']['name'], movement['target']['avatarName'])
-            arrow = '<-' if movement['event']['isFleetReturning'] else '->'
-            time_left = int(movement['eventTime']) - time_now
-            print('{}{} {} {}: {} ({}) {}'.format(color, origin, arrow, destination, movement['event']['missionText'], daysHoursMinutes(time_left), bcolors.ENDC))
-
-            if movement['isHostile']:
-                troops = movement['army']['amount']
-                fleets = movement['fleet']['amount']
-                print(_('Troops:{}\nFleets:{}').format(addThousandSeparator(troops), addThousandSeparator(fleets)))
+            origin = "{} ({})".format(
+                movement["origin"]["name"], movement["origin"]["avatarName"]
+            )
+            destination = "{} ({})".format(
+                movement["target"]["name"], movement["target"]["avatarName"]
+            )
+            arrow = "<-" if movement["event"]["isFleetReturning"] else "->"
+            time_left = int(movement["eventTime"]) - time_now
+            print(
+                "{}{} {} {}: {} ({}) {}".format(
+                    color,
+                    origin,
+                    arrow,
+                    destination,
+                    movement["event"]["missionText"],
+                    daysHoursMinutes(time_left),
+                    bcolors.ENDC,
+                )
+            )
+
+            if movement["isHostile"]:
+                troops = movement["army"]["amount"]
+                fleets = movement["fleet"]["amount"]
+                print(
+                    _("Troops:{}\nFleets:{}").format(
+                        addThousandSeparator(troops), addThousandSeparator(fleets)
+                    )
+                )
             elif isHostile(movement):
-                troops = movement['army']['amount']
+                troops = movement["army"]["amount"]
                 ships = 0
                 fleets = 0
-                for mov in movement['fleet']['ships']:
-                    if mov['cssClass'] == 'ship_transport':
-                        ships += int(mov['amount'])
+                for mov in movement["fleet"]["ships"]:
+                    if mov["cssClass"] == "ship_transport":
+                        ships += int(mov["amount"])
                     else:
-                        fleets += int(mov['amount'])
-                print(_('Troops:{}\nFleets:{}\n Ships:{}').format(addThousandSeparator(troops), addThousandSeparator(fleets), addThousandSeparator(ships)))
+                        fleets += int(mov["amount"])
+                print(
+                    _("Troops:{}\nFleets:{}\n Ships:{}").format(
+                        addThousandSeparator(troops),
+                        addThousandSeparator(fleets),
+                        addThousandSeparator(ships),
+                    )
+                )
             else:
                 assert len(materials_names) == 5
                 total_load = 0
-                for resource in movement['resources']:
-                    amount = resource['amount']
-                    tradegood = resource['cssClass'].split()[1]
+                for resource in movement["resources"]:
+                    amount = resource["amount"]
+                    tradegood = resource["cssClass"].split()[1]
                     # gold won't be translated
-                    if tradegood != 'gold':
+                    if tradegood != "gold":
                         index = materials_names_tec.index(tradegood)
                         tradegood = materials_names[index]
-                    total_load += int(amount.replace(',', '').replace('.', ''))
-                    print(_('{} of {}').format(amount, tradegood))
+                    total_load += int(amount.replace(",", "").replace(".", ""))
+                    print(_("{} of {}").format(amount, tradegood))
                 ships = int(math.ceil((Decimal(total_load) / Decimal(500))))
-                print(_('{:d} Ships').format(ships))
+                print(_("{:d} Ships").format(ships))
         enter()
         event.set()
     except KeyboardInterrupt:
         event.set()
         return
```

### Comparing `ikabot-6.6.4/ikabot/function/stationArmy.py` & `ikabot-7.0.1/ikabot/function/stationArmy.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,205 +1,273 @@
 import gettext
+import re
+
 from ikabot.config import *
-from ikabot.helpers.pedirInfo import *
 from ikabot.helpers.naval import getAvailableShips
+from ikabot.helpers.pedirInfo import *
+from ikabot.helpers.varios import addThousandSeparator
 
-t = gettext.translation('buyResources', localedir, languages=languages, fallback=True)
+t = gettext.translation("buyResources", localedir, languages=languages, fallback=True)
 _ = t.gettext
 
+
 def getCityMilitaryData(session, city_id):
     """
     Parameters
     ----------
     session : ikabot.web.session.Session
     city_id : int
-    
+
     returns
     -------
     data : dict
     """
     params = {
         "view": "cityMilitary",
         "activeTab": "tabUnits",
         "cityId": city_id,
         "currentTab": "tabUnits",
         "currentCityId": city_id,
         "templateView": "cityMilitary",
         "actionRequest": actionRequest,
-        "ajax": "1"
+        "ajax": "1",
     }
     data = session.post(params=params)
     data = json.loads(data, strict=False)
     return data[1][1][1]
 
+
 def extractTooltipsAndValues(data):
     tooltips = re.findall(r'<div class="tooltip">(.*?)</div>', data)
-    values = re.findall(r'<td>\s*([\d.-]+)\s*</td>', data)
+    values = re.findall(r"<td>\s*([\d.,-]+)\s*</td>", data)
     return tooltips, values
 
+
 def calculateTotals(tooltips, values):
     total_units = 0
     total_ships = 0
 
     desc_value_dict = {}
 
     for i, (tooltip, value) in enumerate(zip(tooltips, values)):
-        desc_value_dict.setdefault(tooltip, []).append(value)
+        value = value.replace(",", "")
+        is_digit = value.isdigit()
+        int_value = int(value) if is_digit else 0
 
-        if value.isdigit() and i <= 14:
-            total_units += int(value)
-        elif value.isdigit():
-            total_ships += int(value)
+        if value.isdigit() and int_value > 0:
+            desc_value_dict.setdefault(tooltip, []).append(int_value)
+
+            if i <= 14:
+                total_units += int_value
+            else:
+                total_ships += int_value
 
     return desc_value_dict, total_units, total_ships
 
+
 def getArmyAvailable(session, type_army, destination_city_id, origin_city_id, event):
     params = {
         "view": "deployment",
         "deploymentType": "army" if type_army else "fleet",
         "destinationCityId": destination_city_id,
         "backgroundView": "city",
         "currentCityId": origin_city_id,
         "actionRequest": actionRequest,
-        "ajax": 1
+        "ajax": 1,
     }
 
     data = session.post(params=params)
     amount_results = re.findall(r'<div class=\\"amount\\">(.*?)<\\/div>', data)
-    
+
     if type_army:
-        army_results = re.findall(r'name=\\"cargo_army_([^\\]+)_upkeep\\"\\n\s+value=\\"([^\\"]+)\\"', data)
+        army_results = re.findall(
+            r'name=\\"cargo_army_([^\\]+)_upkeep\\"\\n\s+value=\\"([^\\"]+)\\"', data
+        )
         weight_total_ships = int(getAvailableShips(session)) * 500 if type_army else 0
         weight_results = re.findall(r'<div class=\\"weight\\">(.*?)<\\/div>', data)
     else:
-        army_results = re.findall(r'name=\\"cargo_fleet_([^\\]+)_upkeep\\"\\n\s+value=\\"([^\\"]+)\\"', data)
-
+        army_results = re.findall(
+            r'name=\\"cargo_fleet_([^\\]+)_upkeep\\"\\n\s+value=\\"([^\\"]+)\\"', data
+        )
 
     army_available = {}
     weight_total_army = 0
 
     if army_results:
         for i, result in enumerate(army_results):
             army_code = result[0]
-            army = "cargo_{}_{}_upkeep".format("army" if type_army else "fleet", army_code)
-            army_only = "cargo_{}_{}".format("army" if type_army else "fleet", army_code)
+            army = "cargo_{}_{}_upkeep".format(
+                "army" if type_army else "fleet", army_code
+            )
+            army_only = "cargo_{}_{}".format(
+                "army" if type_army else "fleet", army_code
+            )
             upkeep = result[1]
             quantity = amount_results[i]
             army_available[army] = upkeep
             army_available[army_only] = quantity
             if type_army and weight_results and int(weight_results[i]) > 0:
                 weight_total_army += int(quantity) * int(weight_results[i])
-    
+
         if type_army and weight_total_army > weight_total_ships:
             banner()
-            print('Not enough ships to transport all the units!')
+            print("Not enough ships to transport all the units!")
             enter()
             return None
         return army_available
     return None
 
 
 def sendArmy(session, origin_city, destination_city, type_army, army_available):
     params = {
         "action": "transportOperations",
         "function": "deployArmy" if type_army else "deployFleet",
         "actionRequest": actionRequest,
-        "islandId": destination_city['islandId'],
-        "destinationCityId": destination_city['id'],
+        "islandId": destination_city["islandId"],
+        "destinationCityId": destination_city["id"],
         "deploymentType": "army" if type_army else "fleet",
         "backgroundView": "city",
-        "currentCityId": origin_city['id'],
+        "currentCityId": origin_city["id"],
         "templateView": "deployment",
-        "ajax": 1
+        "ajax": 1,
     }
 
     for army in army_available:
         params[army] = army_available[army]
 
     session.post(params=params)
 
-def stationArmy(session,event, stdin_fd, predetermined_input):
+
+def stationArmy(session, event, stdin_fd, predetermined_input):
     sys.stdin = os.fdopen(stdin_fd)
     config.predetermined_input = predetermined_input
     type_army = True
     try:
         banner()
 
         ids, cities = getIdsOfCities(session)
         army = {}
-        print('Total:')
-        print('{:>19}|{:>19}|{:>19}|'.format('', 'Units', 'Ships'))
+        print("Total:")
+        print("{:>19}|{:>19}|{:>19}|".format("", "Units", "Ships"))
 
         for city_id in cities:
             city = cities[city_id]
-            data = getCityMilitaryData(session, city['id'])
+            data = getCityMilitaryData(session, city["id"])
             desc, values = extractTooltipsAndValues(data)
             army, total_units, total_ships = calculateTotals(desc, values)
-            
-            print('{:>19}|{:>19}|{:>19}|'.format(city['name'], total_units, total_ships))
-        
+
+            print(
+                "{:>19}|{:>19}|{:>19}|".format(
+                    city["name"],
+                    addThousandSeparator(total_units),
+                    addThousandSeparator(total_ships),
+                )
+            )
+
         print()
-        print(_('(0) Back'))
-        print(_('(1) Move troops'))
-        print(_('(2) Move ships'))
-        print(_('(3) Move all ground units to a city.'))
-        print(_('(4) Move all maritime units to a city.'))
-        print(_('(5) Move all units to a city.'))
-        
+        print(_("(0) Back"))
+        print(_("(1) Move troops"))
+        print(_("(2) Move ships"))
+        print(_("(3) Move all ground units to a city."))
+        print(_("(4) Move all maritime units to a city."))
+        print(_("(5) Move all units to a city."))
+
         selected = read(min=0, max=5, digit=True)
         if selected == 0:
             event.set()
             return
         elif selected in (1, 2):
-            print('Origin city:')
+            print("Origin city:")
             origin_city = chooseCity(session)
             print()
-            print('Destination city:')
+            print("Destination city:")
             destination_city = chooseCity(session)
-            if origin_city['id'] == destination_city['id']:
+            if origin_city["id"] == destination_city["id"]:
                 banner()
-                print('The city of origin and the destination city cannot be the same!')
+                print("The city of origin and the destination city cannot be the same!")
                 enter()
                 event.set()
             else:
                 type_army = selected == 1
-                army_available = getArmyAvailable(session, type_army, destination_city['id'], origin_city['id'], event)
+                army_available = getArmyAvailable(
+                    session, type_army, destination_city["id"], origin_city["id"], event
+                )
                 if army_available != None:
-                    sendArmy(session, origin_city, destination_city, type_army, army_available)
-                    print('Army sent!')
+                    sendArmy(
+                        session,
+                        origin_city,
+                        destination_city,
+                        type_army,
+                        army_available,
+                    )
+                    print("Army sent!")
                     enter()
                     event.set()
                 else:
                     print()
-                    print('No {} units available in {}.'.format('ground' if type_army else 'maritime', origin_city['name']))
+                    print(
+                        "No {} units available in {}.".format(
+                            "ground" if type_army else "maritime", origin_city["name"]
+                        )
+                    )
                     enter()
                     event.set()
-        elif selected in (3,4,5):
-            print('Destination city:')
+        elif selected in (3, 4, 5):
+            print("Destination city:")
             destination_city = chooseCity(session)
             ids, cities = getIdsOfCities(session)
-            
-            if selected in (3,5):
+
+            if selected in (3, 5):
                 type_army = True
                 for city_id in cities:
-                    if city_id != destination_city['id']:
+                    if city_id != destination_city["id"]:
                         city = cities[city_id]
-                        army_available = getArmyAvailable(session, type_army, destination_city['id'], city['id'], event)
+                        army_available = getArmyAvailable(
+                            session,
+                            type_army,
+                            destination_city["id"],
+                            city["id"],
+                            event,
+                        )
                         if army_available != None:
-                            sendArmy(session, city, destination_city, type_army, army_available)
+                            sendArmy(
+                                session,
+                                city,
+                                destination_city,
+                                type_army,
+                                army_available,
+                            )
                         else:
-                            print('No ground units available in {}.'.format(city['name']))
-            if selected in (4,5):
+                            print(
+                                "No ground units available in {}.".format(city["name"])
+                            )
+            if selected in (4, 5):
                 type_army = False
                 for city_id in cities:
-                    if city_id != destination_city['id']:
+                    if city_id != destination_city["id"]:
                         city = cities[city_id]
-                        army_available = getArmyAvailable(session, type_army, destination_city['id'], city['id'], event)
+                        army_available = getArmyAvailable(
+                            session,
+                            type_army,
+                            destination_city["id"],
+                            city["id"],
+                            event,
+                        )
                         if army_available != None:
-                            sendArmy(session, city, destination_city, type_army, army_available)
+                            sendArmy(
+                                session,
+                                city,
+                                destination_city,
+                                type_army,
+                                army_available,
+                            )
                         else:
-                            print('No maritime units available in {}.'.format(city['name']))
+                            print(
+                                "No maritime units available in {}.".format(
+                                    city["name"]
+                                )
+                            )
             enter()
-            event.set()               
+            event.set()
     except KeyboardInterrupt:
         event.set()
-        return  
+        return
```

### Comparing `ikabot-6.6.4/ikabot/function/trainArmy.py` & `ikabot-7.0.1/ikabot/function/trainArmy.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 #! /usr/bin/env python3
 # -*- coding: utf-8 -*-
 
-import re
-import json
+import asyncio
+import copy
 import gettext
+import json
+import re
 import traceback
+
 from ikabot.config import *
-from ikabot.helpers.gui import *
 from ikabot.helpers.botComm import *
+from ikabot.helpers.getJson import getCity
+from ikabot.helpers.gui import *
 from ikabot.helpers.pedirInfo import *
-from ikabot.helpers.varios import *
 from ikabot.helpers.process import set_child_mode
-from ikabot.helpers.varios import addThousandSeparator
-from ikabot.helpers.getJson import getCity
-from ikabot.helpers.signals import setInfoSignal
 from ikabot.helpers.resources import getAvailableResources
+from ikabot.helpers.signals import setInfoSignal
+from ikabot.helpers.varios import *
+from ikabot.helpers.varios import addThousandSeparator
 
-t = gettext.translation('trainArmy',
-                        localedir,
-                        languages=languages,
-                        fallback=True)
+t = gettext.translation("trainArmy", localedir, languages=languages, fallback=True)
 _ = t.gettext
 
 
 def getBuildingInfo(session, city, trainTroops):
     """
     Parameters
     ----------
@@ -31,113 +31,140 @@
     city : dict
     trainTroops : bool
 
     Returns
     -------
     response : dict
     """
-    view = 'barracks' if trainTroops else 'shipyard'
-    params = {'view': view, 'cityId': city['id'], 'position': city['pos'], 'backgroundView': 'city', 'currentCityId': city['id'], 'actionRequest': actionRequest, 'ajax': '1'}
+    view = "barracks" if trainTroops else "shipyard"
+    params = {
+        "view": view,
+        "cityId": city["id"],
+        "position": city["pos"],
+        "backgroundView": "city",
+        "currentCityId": city["id"],
+        "actionRequest": actionRequest,
+        "ajax": "1",
+    }
     data = session.post(params=params)
     return json.loads(data, strict=False)
 
 
 def train(session, city, trainings, trainTroops):
     """
     Parameters
     ----------
     session : ikabot.web.session.Session
     city : dict
     trainings : list[dict]
     trainTroops : bool
     """
-    templateView = 'barracks' if trainTroops else 'shipyard'
-    function = 'buildUnits' if trainTroops else 'buildShips'
-    payload = {'action': 'CityScreen', 'function': function, 'actionRequest': 'REQUESTID', 'cityId': city['id'], 'position': city['pos'], 'backgroundView': 'city', 'currentCityId': city['id'], 'templateView': templateView, 'ajax': '1'}
+    templateView = "barracks" if trainTroops else "shipyard"
+    function = "buildUnits" if trainTroops else "buildShips"
+    payload = {
+        "action": "CityScreen",
+        "function": function,
+        "actionRequest": "REQUESTID",
+        "cityId": city["id"],
+        "position": city["pos"],
+        "backgroundView": "city",
+        "currentCityId": city["id"],
+        "templateView": templateView,
+        "ajax": "1",
+    }
     for training in trainings:
-        payload[training['unit_type_id']] = training['train']
+        payload[training["unit_type_id"]] = training["train"]
     session.post(params=payload)
 
 
 def waitForTraining(session, city, trainTroops):
     """
     Parameters
     ----------
     session : ikabot.web.session.Session
     city : dict
     trainTroops : bool
     """
     data = getBuildingInfo(session, city, trainTroops)
     html = data[1][1][1]
-    seconds = re.search(r'\'buildProgress\', (\d+),', html)
+    seconds = re.search(r"\'buildProgress\', (\d+),", html)
     if seconds:
         seconds = seconds.group(1)
-        seconds = int(seconds) - data[0][1]['time']
+        seconds = int(seconds) - data[0][1]["time"]
         wait(seconds + 5)
 
 
 def planTrainings(session, city, trainings, trainTroops):
     """
     Parameters
     ----------
     session : ikabot.web.session.Session
     city : dict
     trainings : list[list[dict]]
     trainTroops : bool
     """
-    buildingPos = city['pos']
+    buildingPos = city["pos"]
 
     # trainings might be divided in multriple rounds
     while True:
 
         # total number of units to create
-        total = sum([unit['cantidad'] for training in trainings for unit in training])
+        total = sum([unit["cantidad"] for training in trainings for unit in training])
         if total == 0:
             return
 
         for training in trainings:
             waitForTraining(session, city, trainTroops)
-            html = session.get(city_url + city['id'])
+            html = session.get(city_url + city["id"])
             city = getCity(html)
-            city['pos'] = buildingPos
+            city["pos"] = buildingPos
 
-            resourcesAvailable = city['recursos'].copy()
-            resourcesAvailable.append(city['ciudadanosDisp'])
+            resourcesAvailable = city["availableResources"].copy()
+            resourcesAvailable.append(city["freeCitizens"])
 
             # for each unit type in training
             for unit in training:
 
                 # calculate how many units can actually be trained based on the resources available
-                unit['train'] = unit['cantidad']
+                unit["train"] = unit["cantidad"]
 
                 for i in range(len(materials_names_english)):
                     material_name = materials_names_english[i].lower()
-                    if material_name in unit['costs']:
-                        limiting = resourcesAvailable[i] // unit['costs'][material_name]
-                        unit['train'] = min(unit['train'], limiting)
-
-                if 'citizens' in unit['costs']:
-                    limiting = resourcesAvailable[len(materials_names_english)] // unit['costs']['citizens']
-                    unit['train'] = min(unit['train'], limiting)
+                    if material_name in unit["costs"]:
+                        limiting = resourcesAvailable[i] // unit["costs"][material_name]
+                        unit["train"] = min(unit["train"], limiting)
+
+                if "citizens" in unit["costs"]:
+                    limiting = (
+                        resourcesAvailable[len(materials_names_english)]
+                        // unit["costs"]["citizens"]
+                    )
+                    unit["train"] = min(unit["train"], limiting)
 
                 # calculate the resources that will be left
                 for i in range(len(materials_names_english)):
                     material_name = materials_names_english[i].lower()
-                    if material_name in unit['costs']:
-                        resourcesAvailable[i] -= unit['costs'][material_name] * unit['train']
-
-                if 'citizens' in unit['costs']:
-                    resourcesAvailable[len(materials_names_english)] -= unit['costs']['citizens'] * unit['train']
+                    if material_name in unit["costs"]:
+                        resourcesAvailable[i] -= (
+                            unit["costs"][material_name] * unit["train"]
+                        )
+
+                if "citizens" in unit["costs"]:
+                    resourcesAvailable[len(materials_names_english)] -= (
+                        unit["costs"]["citizens"] * unit["train"]
+                    )
 
-                unit['cantidad'] -= unit['train']
+                unit["cantidad"] -= unit["train"]
 
             # amount of units that will be trained
-            total = sum([unit['train'] for unit in training])
+            total = sum([unit["train"] for unit in training])
             if total == 0:
-                msg = _('It was not possible to finish the training due to lack of resources.')
+                msg = _(
+                    "It was not possible to finish the training due to lack of resources."
+                )
                 sendToBot(session, msg)
                 return
 
             train(session, city, training, trainTroops)
 
 
 def generateArmyData(units_info):
@@ -148,17 +175,17 @@
 
     Returns
     -------
     units : list[dict]
     """
     i = 1
     units = []
-    while 'js_barracksSlider{:d}'.format(i) in units_info:
-        # {"identifier":"phalanx","unit_type_id":303,"costs":{"citizens":1,"wood":27,"sulfur":30,"upkeep":3,"completiontime":71.169695412658},"local_name":"Hoplita"}
-        info = units_info['js_barracksSlider{:d}'.format(i)]['slider']['control_data']
+    while "js_barracksSlider{:d}".format(i) in units_info:
+        # {'identifier':'phalanx','unit_type_id':303,'costs':{'citizens':1,'wood':27,'sulfur':30,'upkeep':3,'completiontime':71.169695412658},'local_name':'Hoplita'}
+        info = units_info["js_barracksSlider{:d}".format(i)]["slider"]["control_data"]
         info = json.loads(info, strict=False)
         units.append(info)
         i += 1
     return units
 
 
 def trainArmy(session, event, stdin_fd, predetermined_input):
@@ -171,152 +198,298 @@
     predetermined_input : multiprocessing.managers.SyncManager.list
     """
     sys.stdin = os.fdopen(stdin_fd)
     config.predetermined_input = predetermined_input
     try:
         banner()
 
-        print(_('Do you want to train troops (1) or ships (2)?'))
+        print(_("Do you want to train troops (1) or ships (2)?"))
         rta = read(min=1, max=2)
         trainTroops = rta == 1
         banner()
 
         if trainTroops:
-            print(_('In what city do you want to train the troops?'))
+            print(_("In what city do you want to train the troops?"))
         else:
-            print(_('In what city do you want to train the fleet?'))
+            print(_("In what city do you want to train the fleet?"))
         city = chooseCity(session)
         banner()
 
-        lookfor = 'barracks' if trainTroops else 'shipyard'
-        for i in range(len(city['position'])):
-            if city['position'][i]['building'] == lookfor:
-                city['pos'] = str(i)
+        lookfor = "barracks" if trainTroops else "shipyard"
+        for i in range(len(city["position"])):
+            if city["position"][i]["building"] == lookfor:
+                city["pos"] = str(i)
                 break
         else:
             if trainTroops:
-                print(_('Barracks not built.'))
+                print(_("Barracks not built."))
             else:
-                print(_('Shipyard not built.'))
+                print(_("Shipyard not built."))
             enter()
             event.set()
             return
 
         data = getBuildingInfo(session, city, trainTroops)
 
         units_info = data[2][1]
         units = generateArmyData(units_info)
 
-        maxSize = max([len(unit['local_name']) for unit in units])
+        maxSize = max([len(unit["local_name"]) for unit in units])
 
         tranings = []
         while True:
             units = generateArmyData(units_info)
-            print(_('Train:'))
+            print(_("Train:"))
             for unit in units:
-                pad = ' ' * (maxSize - len(unit['local_name']))
-                amount = read(msg='{}{}:'.format(pad, unit['local_name']), min=0, empty=True)
-                if amount == '':
+                pad = " " * (maxSize - len(unit["local_name"]))
+                amount = read(
+                    msg="{}{}:".format(pad, unit["local_name"]), min=0, empty=True
+                )
+                if amount == "":
                     amount = 0
-                unit['cantidad'] = amount
+                unit["cantidad"] = amount
 
             # calculate costs
             cost = [0] * (len(materials_names_english) + 3)
             for unit in units:
                 for i in range(len(materials_names_english)):
                     material_name = materials_names_english[i].lower()
-                    if material_name in unit['costs']:
-                        cost[i] += unit['costs'][material_name] * unit['cantidad']
+                    if material_name in unit["costs"]:
+                        cost[i] += unit["costs"][material_name] * unit["cantidad"]
 
-                if 'citizens' in unit['costs']:
-                    cost[len(materials_names_english)+0] += unit['costs']['citizens'] * unit['cantidad']
-                if 'upkeep' in unit['costs']:
-                    cost[len(materials_names_english)+1] += unit['costs']['upkeep'] * unit['cantidad']
-                if 'completiontime' in unit['costs']:
-                    cost[len(materials_names_english)+2] += unit['costs']['completiontime'] * unit['cantidad']
+                if "citizens" in unit["costs"]:
+                    cost[len(materials_names_english) + 0] += (
+                        unit["costs"]["citizens"] * unit["cantidad"]
+                    )
+                if "upkeep" in unit["costs"]:
+                    cost[len(materials_names_english) + 1] += (
+                        unit["costs"]["upkeep"] * unit["cantidad"]
+                    )
+                if "completiontime" in unit["costs"]:
+                    cost[len(materials_names_english) + 2] += (
+                        unit["costs"]["completiontime"] * unit["cantidad"]
+                    )
 
-            print(_('\nTotal cost:'))
+            print(_("\nTotal cost:"))
             for i in range(len(materials_names_english)):
                 if cost[i] > 0:
-                    print('{}: {}'.format(materials_names_english[i], addThousandSeparator(cost[i])))
-            if cost[len(materials_names_english)+0] > 0:
-                print(_('Citizens: {}').format(addThousandSeparator(cost[len(materials_names_english)+0])))
-            if cost[len(materials_names_english)+1] > 0:
-                print(_('Maintenance: {}').format(addThousandSeparator(cost[len(materials_names_english)+1])))
-            if cost[len(materials_names_english)+2] > 0:
-                print(_('Duration: {}').format(daysHoursMinutes(int(cost[len(materials_names_english)+2]))))
-
-            print(_('\nProceed? [Y/n]'))
-            rta = read(values=['y', 'Y', 'n', 'N', ''])
-            if rta.lower() == 'n':
+                    print(
+                        "{}: {}".format(
+                            materials_names_english[i], addThousandSeparator(cost[i])
+                        )
+                    )
+            if cost[len(materials_names_english) + 0] > 0:
+                print(
+                    _("Citizens: {}").format(
+                        addThousandSeparator(cost[len(materials_names_english) + 0])
+                    )
+                )
+            if cost[len(materials_names_english) + 1] > 0:
+                print(
+                    _("Maintenance: {}").format(
+                        addThousandSeparator(cost[len(materials_names_english) + 1])
+                    )
+                )
+            if cost[len(materials_names_english) + 2] > 0:
+                print(
+                    _("Duration: {}").format(
+                        daysHoursMinutes(int(cost[len(materials_names_english) + 2]))
+                    )
+                )
+
+            print(_("\nProceed? [Y/n]"))
+            rta = read(values=["y", "Y", "n", "N", ""])
+            if rta.lower() == "n":
                 event.set()
                 return
 
             tranings.append(units)
 
             if trainTroops:
-                print(_('\nDo you want to train more troops when you finish? [y/N]'))
+                print(_("\nDo you want to train more troops when you finish? [y/N]"))
             else:
-                print(_('\nDo you want to train more fleets when you finish? [y/N]'))
-            rta = read(values=['y', 'Y', 'n', 'N', ''])
-            if rta.lower() == 'y':
+                print(_("\nDo you want to train more fleets when you finish? [y/N]"))
+            rta = read(values=["y", "Y", "n", "N", ""])
+            if rta.lower() == "y":
                 banner()
-                continue
+                if trainTroops:
+                    print(_("Train new troops (1) or repeat (2)?"))
+                else:
+                    print(_("Train new fleets (1) or repeat (2)?"))
+                rta = read(min=1, max=2)
+                if rta == 1:
+                    continue
+                else:
+                    print(_("\nRepeat how many times?"))
+                    countRepeat = read(min=1, default=0)
+                    break
             else:
+                countRepeat = 0
                 break
 
+        print(_("Do you want to replicate the training to other cities? (y/N)"))
+        replicate = read(values=["y", "Y", "n", "N", ""])
+        if replicate.lower() == "y":
+            cityTrainings = []
+            ids, cities = getIdsOfCities(session)
+
+            print(_("(0) Back"))
+            print(_("(1) All the wine cities"))
+            print(_("(2) All the marble cities"))
+            print(_("(3) All the cristal cities"))
+            print(_("(4) All the sulfur cities"))
+            print(_("(5) Choose City"))
+            print(_("(6) All City"))
+
+            selected = read(min=0, max=6, digit=True)
+            if selected == 0:
+                event.set()
+                return
+            elif selected in [1, 2, 3, 4]:
+                cityTrainings = filterCitiesByResource(
+                    cities, resourceMapping[selected], cityTrainings
+                )
+            elif selected == 5:
+                city = []
+                while True:
+                    city = chooseCity(session)
+                    if city["id"] in cityTrainings:
+                        print(_("\nYou have already selected this city!"))
+                        continue
+                    cityTrainings.append(city["id"])
+                    print(_("\nDo you want to add another city? [y/N]"))
+                    rta = read(values=["y", "Y", "n", "N", ""])
+                    if rta.lower() == "y":
+                        continue
+                    else:
+                        break
+            elif selected == 6:
+                ids, cities = getIdsOfCities(session)
+                for cityId in ids:
+                    cityTrainings.append(cityId)
+
         # calculate if the city has enough resources
-        resourcesAvailable = city['recursos'].copy()
-        resourcesAvailable.append(city['ciudadanosDisp'])
+        resourcesAvailable = city["availableResources"].copy()
+        resourcesAvailable.append(city["freeCitizens"])
 
         for training in tranings:
             for unit in training:
-
-                for i in range(len(materials_names_english)):
-                    material_name = materials_names_english[i].lower()
-                    if material_name in unit['costs']:
-                        resourcesAvailable[i] -= unit['costs'][material_name] * unit['cantidad']
-
-                if 'citizens' in unit['costs']:
-                    resourcesAvailable[len(materials_names_english)] -= unit['costs']['citizens'] * unit['cantidad']
+                if unit["cantidad"] != 0:
+                    for i in range(len(materials_names_english)):
+                        material_name = materials_names_english[i].lower()
+                        if material_name in unit["costs"]:
+                            resourcesAvailable[i] -= (
+                                unit["costs"][material_name] * unit["cantidad"]
+                            )
+
+                    if "citizens" in unit["costs"]:
+                        resourcesAvailable[len(materials_names_english)] -= (
+                            unit["costs"]["citizens"] * unit["cantidad"]
+                        )
 
         not_enough = [elem for elem in resourcesAvailable if elem < 0] != []
 
         if not_enough:
-            print(_('\nThere are not enough resources:'))
+            print(_("\nThere are not enough resources:"))
             for i in range(len(materials_names_english)):
                 if resourcesAvailable[i] < 0:
-                    print('{}:{}'.format(materials_names[i], addThousandSeparator(resourcesAvailable[i]*-1)))
+                    print(
+                        "{}:{}".format(
+                            materials_names[i],
+                            addThousandSeparator(resourcesAvailable[i] * -1),
+                        )
+                    )
 
             if resourcesAvailable[len(materials_names_english)] < 0:
-                print(_('Citizens:{}').format(addThousandSeparator(resourcesAvailable[len(materials_names_english)]*-1)))
-
-            print(_('\nProceed anyway? [Y/n]'))
-            rta = read(values=['y', 'Y', 'n', 'N', ''])
-            if rta.lower() == 'n':
+                print(
+                    _("Citizens:{}").format(
+                        addThousandSeparator(
+                            resourcesAvailable[len(materials_names_english)] * -1
+                        )
+                    )
+                )
+
+            print(_("\nProceed anyway? [Y/n]"))
+            rta = read(values=["y", "Y", "n", "N", ""])
+            if rta.lower() == "n":
                 event.set()
                 return
 
         if trainTroops:
-            print(_('\nThe selected troops will be trained.'))
+            print(_("\nThe selected troops will be trained."))
         else:
-            print(_('\nThe selected fleet will be trained.'))
+            print(_("\nThe selected fleet will be trained."))
         enter()
+
+        if replicate == "y":
+            countRepeat = countRepeat + 1
+            while countRepeat > 0:
+                for cityId in cityTrainings:
+                    html = session.get(city_url + str(cityId))
+                    city = getCity(html)
+
+                    lookfor = "barracks" if trainTroops else "shipyard"
+                    try:
+                        for i in range(len(city["position"])):
+                            if city["position"][i]["building"] == lookfor:
+                                city["pos"] = str(i)
+                                tranings_copy = []
+                                units_copy = copy.deepcopy(units)
+                                tranings_copy.append(units_copy)
+                                loop = asyncio.get_event_loop()
+                                loop.run_until_complete(
+                                    planTrainings(
+                                        session, city, tranings_copy, trainTroops
+                                    )
+                                )
+                                break
+                    except Exception as e:
+                        if trainTroops:
+                            info = _("\nI train troops in {}\n").format(
+                                city["cityName"]
+                            )
+                        else:
+                            info = _("\nI train fleets in {}\n").format(
+                                city["cityName"]
+                            )
+                        msg = _("Error in:\n{}\nCause:\n{}").format(
+                            info, traceback.format_exc()
+                        )
+                        sendToBot(session, msg)
+                countRepeat = countRepeat - 1
+
+        else:
+            if trainTroops:
+                info = _("\nI train troops in {}\n").format(city["cityName"])
+            else:
+                info = _("\nI train fleets in {}\n").format(city["cityName"])
+            setInfoSignal(session, info)
+            try:
+                planTrainings(session, city, tranings, trainTroops)
+            except Exception as e:
+                msg = _("Error in:\n{}\nCause:\n{}").format(
+                    info, traceback.format_exc()
+                )
+                sendToBot(session, msg)
+            finally:
+                session.logout()
     except KeyboardInterrupt:
         event.set()
         return
 
     set_child_mode(session)
     event.set()
 
-    if trainTroops:
-        info = _('\nI train troops in {}\n').format(city['cityName'])
-    else:
-        info = _('\nI train fleets in {}\n').format(city['cityName'])
-    setInfoSignal(session, info)
-    try:
-        planTrainings(session, city, tranings, trainTroops)
-    except Exception as e:
-        msg = _('Error in:\n{}\nCause:\n{}').format(info, traceback.format_exc())
-        sendToBot(session, msg)
-    finally:
-        session.logout()
+
+def filterCitiesByResource(cities, resource_id, cityTrainings):
+    for cityId, cityData in cities.items():
+        if cityData["tradegood"] == resource_id:
+            cityTrainings.append(cityData["id"])
+    return cityTrainings
+
+
+resourceMapping = {
+    1: "1",  # Wine
+    2: "2",  # Marble
+    3: "3",  # Cristal
+    4: "4",  # Sulfur
+}
```

### Comparing `ikabot-6.6.4/ikabot/function/update.py` & `ikabot-7.0.1/ikabot/function/update.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 #! /usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 import gettext
 import sys
+
+from ikabot.config import *
+from ikabot.helpers.gui import *
 from ikabot.helpers.pedirInfo import read
 from ikabot.helpers.process import run
-from ikabot.helpers.gui import *
-from ikabot.config import *
 
-t = gettext.translation('update', localedir, languages=languages, fallback=True)
+t = gettext.translation("update", localedir, languages=languages, fallback=True)
 _ = t.gettext
 
 
 def update(session, event, stdin_fd, predetermined_input):
     """
     Parameters
     ----------
@@ -20,14 +21,14 @@
     event : multiprocessing.Event
     stdin_fd: int
     predetermined_input : multiprocessing.managers.SyncManager.list
     """
     sys.stdin = os.fdopen(stdin_fd)
     config.predetermined_input = predetermined_input
     try:
-        print(_('To update ikabot run:'))
-        print('python3 -m pip install --user --upgrade ikabot')
+        print(_("To update ikabot run:"))
+        print("python3 -m pip install --user --upgrade ikabot")
         enter()
         event.set()
     except KeyboardInterrupt:
         event.set()
         return
```

### Comparing `ikabot-6.6.4/ikabot/function/vacationMode.py` & `ikabot-7.0.1/ikabot/function/vacationMode.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,39 @@
 #! /usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 import gettext
 import sys
+
 from ikabot.config import *
+from ikabot.helpers.getJson import getCity
 from ikabot.helpers.gui import *
 from ikabot.helpers.pedirInfo import read
-from ikabot.helpers.getJson import getCity
 
-t = gettext.translation('vacationMode', localedir, languages=languages, fallback=True)
+t = gettext.translation("vacationMode", localedir, languages=languages, fallback=True)
 _ = t.gettext
 
 
 def activateVacationMode(session):
     """
     Parameters
     ----------
     session : ikabot.web.session.Session
     """
     html = session.get()
     city = getCity(html)
 
-    data = {'action': 'Options', 'function': 'activateVacationMode', 'actionRequest': actionRequest, 'backgroundView': 'city', 'currentCityId': city['id'], 'templateView': 'options_umod_confirm'}
+    data = {
+        "action": "Options",
+        "function": "activateVacationMode",
+        "actionRequest": actionRequest,
+        "backgroundView": "city",
+        "currentCityId": city["id"],
+        "templateView": "options_umod_confirm",
+    }
     session.post(params=data, ignoreExpire=True)
 
 
 def vacationMode(session, event, stdin_fd, predetermined_input):
     """
     Parameters
     ----------
@@ -34,23 +42,23 @@
     stdin_fd: int
     predetermined_input : multiprocessing.managers.SyncManager.list
     """
     sys.stdin = os.fdopen(stdin_fd)
     config.predetermined_input = predetermined_input
     try:
         banner()
-        print(_('Activate vacation mode? [Y/n]'))
-        rta = read(values=['y', 'Y', 'n', 'N', ''])
-        if rta.lower() == 'n':
+        print(_("Activate vacation mode? [Y/n]"))
+        rta = read(values=["y", "Y", "n", "N", ""])
+        if rta.lower() == "n":
             event.set()
             return
 
         activateVacationMode(session)
 
-        print(_('Vacation mode has been activated.'))
+        print(_("Vacation mode has been activated."))
         enter()
         event.set()
         clear()
         sys.exit()
     except KeyboardInterrupt:
         event.set()
         return
```

### Comparing `ikabot-6.6.4/ikabot/helpers/aesCipher.py` & `ikabot-7.0.1/ikabot/helpers/aesCipher.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,114 +1,128 @@
 #! /usr/bin/env python3
 # -*- coding: utf-8 -*-
 
-import os
-import json
 import base64
 import hashlib
+import json
+import os
+
+from cryptography.hazmat.primitives.ciphers.aead import AESGCM
+
 from ikabot.config import *
 from ikabot.helpers.botComm import *
-from cryptography.hazmat.primitives.ciphers.aead import AESGCM
 
-t = gettext.translation('aesCipher', localedir, languages=languages, fallback=True)
+t = gettext.translation("aesCipher", localedir, languages=languages, fallback=True)
 _ = t.gettext
 
 
 class AESCipher:
 
     def __init__(self, mail, password):
         if type(password) == int:
             password = str(password)
-        self.key = hashlib.sha256(mail.encode('utf-8') + b'\x00' + password.encode('utf-8')).digest()
-        for i in range(0xfff):
+        self.key = hashlib.sha256(
+            mail.encode("utf-8") + b"\x00" + password.encode("utf-8")
+        ).digest()
+        for i in range(0xFFF):
             self.key = hashlib.sha256(self.key).digest()
 
     def encrypt(self, plaintext):
         aesgcm = AESGCM(self.key)
         nonce = os.urandom(16)
-        ciphertext = aesgcm.encrypt(nonce, plaintext.encode('utf-8'), None)
-        return base64.b64encode(nonce + ciphertext).decode('utf-8')
+        ciphertext = aesgcm.encrypt(nonce, plaintext.encode("utf-8"), None)
+        return base64.b64encode(nonce + ciphertext).decode("utf-8")
 
     def decrypt(self, ciphertext):
         ciphertext = base64.b64decode(ciphertext)
         nonce = ciphertext[:16]
         ciphertext = ciphertext[16:]
         aesgcm = AESGCM(self.key)
         plaintext = aesgcm.decrypt(nonce, ciphertext, None)
-        return plaintext.decode('utf-8')
+        return plaintext.decode("utf-8")
 
     def getEntryKey(self, session):
         """
         Parameters
         ----------
         session : ikabot.web.session.Session
 
         Returns
         -------
         entry key : str
         """
-        return hashlib.sha256('ikabot'.encode('utf-8') + session.mail.encode('utf-8')).hexdigest()
+        return hashlib.sha256(
+            "ikabot".encode("utf-8") + session.mail.encode("utf-8")
+        ).hexdigest()
 
     def deleteSessionData(self, session):
         """
         Parameters
         ----------
         session : ikabot.web.session.Session
         """
         entry_key = self.getEntryKey(session)
-        with open(ikaFile, 'r') as filehandler:
+        with open(ikaFile, "r") as filehandler:
             data = filehandler.read()
 
-        newFile = ''
-        for line in data.split('\n'):
+        newFile = ""
+        for line in data.split("\n"):
             if entry_key != line[:64]:
-                newFile += line + '\n'
+                newFile += line + "\n"
 
-        with open(ikaFile, 'w') as filehandler:
+        with open(ikaFile, "w") as filehandler:
             filehandler.write(newFile.strip())
             filehandler.flush()
 
     def getSessionData(self, session, all=False):
         """
         Parameters
         ----------
         session : ikabot.web.session.Session
         all : bool
         """
         entry_key = self.getEntryKey(session)
-        with open(ikaFile, 'r') as filehandler:
+        with open(ikaFile, "r") as filehandler:
             ciphertexts = filehandler.read()
 
-        for ciphertext in ciphertexts.split('\n'):
+        for ciphertext in ciphertexts.split("\n"):
             if entry_key == ciphertext[:64]:
                 ciphertext = ciphertext[64:]
                 try:
                     plaintext = self.decrypt(ciphertext)
                 except Exception:
-                    msg = _('Error while decrypting session data.\nYou may have entered a wrong password.')
+                    msg = _(
+                        "Error while decrypting session data.\nYou may have entered a wrong password."
+                    )
                     if session.padre:
                         print(msg)
                     else:
                         sendToBot(session, msg)
-                    print(_('\nWould you like to delete the ikabot session data associated with this email address? [y/N]'))
-                    rta = read(values=['n', 'N', 'y', 'Y'])
-                    if rta.lower() == 'n':
+                    print(
+                        _(
+                            "\nWould you like to delete the ikabot session data associated with this email address? [y/N]"
+                        )
+                    )
+                    rta = read(values=["n", "N", "y", "Y"])
+                    if rta.lower() == "n":
                         os._exit(0)
                     self.deleteSessionData(session)
                     os._exit(0)
                 data_dict = json.loads(plaintext, strict=False)
                 if all:
                     return data_dict
                 else:
                     try:
                         try:
-                            session_data = data_dict[session.username][session.mundo][session.servidor]
+                            session_data = data_dict[session.username][session.mundo][
+                                session.servidor
+                            ]
                         except Exception:
                             session_data = {}
-                        session_data['shared'] = data_dict['shared']
+                        session_data["shared"] = data_dict["shared"]
                         return session_data
                     except KeyError:
                         return {}
         return {}
 
     def setSessionData(self, session, data, shared=False):
         """
@@ -116,40 +130,40 @@
         ----------
         session : ikabot.web.session.Session
         data : dict
         """
         session_data = self.getSessionData(session, True)
 
         if shared:
-            if 'shared' not in session_data:
-                session_data['shared'] = {}
-            if 'logLevel' not in session_data['shared']:
-                session_data['shared']['logLevel'] = 2 # Warn by default
-            session_data['shared'] = {**session_data['shared'], **data}
+            if "shared" not in session_data:
+                session_data["shared"] = {}
+            if "logLevel" not in session_data["shared"]:
+                session_data["shared"]["logLevel"] = 2  # Warn by default
+            session_data["shared"] = {**session_data["shared"], **data}
         else:
             if session.username not in session_data:
                 session_data[session.username] = {}
             if session.mundo not in session_data[session.username]:
                 session_data[session.username][session.mundo] = {}
             if session.servidor not in session_data[session.username][session.mundo]:
                 session_data[session.username][session.mundo][session.servidor] = {}
-            if 'shared' not in session_data:
-                session_data['shared'] = {}
+            if "shared" not in session_data:
+                session_data["shared"] = {}
             session_data[session.username][session.mundo][session.servidor] = data
 
         plaintext = json.dumps(session_data)
         ciphertext = self.encrypt(plaintext)
 
-        with open(ikaFile, 'r') as filehandler:
+        with open(ikaFile, "r") as filehandler:
             data = filehandler.read()
 
         entry_key = self.getEntryKey(session)
-        newFile = ''
-        newline = entry_key + ' ' + ciphertext
-        for line in data.split('\n'):
+        newFile = ""
+        newline = entry_key + " " + ciphertext
+        for line in data.split("\n"):
             if entry_key != line[:64]:
-                newFile += line + '\n'
-        newFile += newline + '\n'
+                newFile += line + "\n"
+        newFile += newline + "\n"
 
-        with open(ikaFile, 'w') as filehandler:
+        with open(ikaFile, "w") as filehandler:
             filehandler.write(newFile.strip())
             filehandler.flush()
```

### Comparing `ikabot-6.6.4/ikabot/helpers/botComm.py` & `ikabot-7.0.1/ikabot/helpers/botComm.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 #! /usr/bin/env python3
 # -*- coding: utf-8 -*-
 
-import re
-import os
+import gettext
 import json
+import os
 import random
-import gettext
+import re
 import sys
-import ikabot.web.session
-from ikabot.config import *
+import time
+from requests import get
 import ikabot.config as config
+from ikabot.config import *
 from ikabot.helpers.gui import *
 from ikabot.helpers.pedirInfo import read
 
-t = gettext.translation('botComm', localedir, languages=languages, fallback=True)
+t = gettext.translation("botComm", localedir, languages=languages, fallback=True)
 _ = t.gettext
 
 
 def sendToBotDebug(session, msg, debugON):
     """This function will send the ``msg`` argument passed to it as a message to the user on Telegram, only if ``debugOn`` is ``True``
     Parameters
     ----------
@@ -41,32 +42,54 @@
     msg : str
         a string representing the message to send to the user on Telegram
     Token : bool
         a boolean indicating whether or not to attach the process id, the users server, world and Ikariam username to the message
     Photo : bytes
         a bytes object representing a picture to be sent.
     """
-    
-    session.writeLog(msg = 'MESSAGE TO TG BOT: ' + msg, module = __name__, level = logLevels.WARN, logTraceback = True, logRequestHistory = True )
+
+    session.writeLog(
+        msg="MESSAGE TO TG BOT: " + msg,
+        module=__name__,
+        level=logLevels.WARN,
+        logTraceback=True,
+        logRequestHistory=True,
+    )
     if checkTelegramData(session) is False:
-        session.writeLog(msg = 'Tried to message TG bot without correct tg data!', module=__name__, level = logLevels.ERROR)
+        session.writeLog(
+            msg="Tried to message TG bot without correct tg data!",
+            module=__name__,
+            level=logLevels.ERROR,
+        )
         return
     if Token is False:
-        msg = 'pid:{}\n{}\n{}'.format(os.getpid(), config.infoUser, msg)
+        msg = "pid:{}\n{}\n{}".format(os.getpid(), config.infoUser, msg)
 
     sessionData = session.getSessionData()
-    telegram_data = sessionData['shared']['telegram']
+    telegram_data = sessionData["shared"]["telegram"]
     if Photo is None:
-        ikabot.web.session.normal_get('https://api.telegram.org/bot{}/sendMessage'.format(telegram_data['botToken']), params={'chat_id': telegram_data['chatId'], 'text': msg})
+        return get(
+            "https://api.telegram.org/bot{}/sendMessage".format(
+                telegram_data["botToken"]
+            ),
+            params={"chat_id": telegram_data["chatId"], "text": msg},
+        )
     else:
         # we need to clear the headers here because telegram doesn't like keep-alive, might as well get rid of all headers
         headers = session.s.headers.copy()
         session.s.headers.clear()
-        resp = session.s.post('https://api.telegram.org/bot{}/sendDocument'.format(telegram_data['botToken']), files={'document': ('captcha.png', Photo)}, data={'chat_id': telegram_data['chatId'],'caption': msg})
+        resp = session.s.post(
+            "https://api.telegram.org/bot{}/sendDocument".format(
+                telegram_data["botToken"]
+            ),
+            files={"document": ("captcha.png", Photo)},
+            data={"chat_id": telegram_data["chatId"], "caption": msg},
+        )
         session.s.headers = headers
+        return resp
 
 
 def telegramDataIsValid(session):
     """This function checks whether or not there is any Telegram data stored in the .ikabot file
     Parameters
     ----------
     session : ikabot.web.session.Session
@@ -76,15 +99,18 @@
     -------
     valid : bool
         a boolean indicating whether or not there is any Telegram data stored in the .ikabot file
 
     """
     sessionData = session.getSessionData()
     try:
-        return len(sessionData['shared']['telegram']['botToken']) > 0 and len(sessionData['shared']['telegram']['chatId']) > 0
+        return (
+            len(sessionData["shared"]["telegram"]["botToken"]) > 0
+            and len(sessionData["shared"]["telegram"]["chatId"]) > 0
+        )
     except KeyError:
         return False
 
 
 def getUserResponse(session, fullResponse=False):
     """This function will retrieve a list of messages the user sent to the bot on Telegram.
     Parameters
@@ -99,27 +125,41 @@
     """
     # returns messages that the user sends to the telegram bot
 
     if checkTelegramData(session) is False:
         return []
 
     sessionData = session.getSessionData()
-    telegram_data = sessionData['shared']['telegram']
+    telegram_data = sessionData["shared"]["telegram"]
 
     try:
-        updates = ikabot.web.session.normal_get('https://api.telegram.org/bot{}/getUpdates'.format(telegram_data['botToken'])).text
+        updates = get(
+            "https://api.telegram.org/bot{}/getUpdates".format(
+                telegram_data["botToken"]
+            )
+        ).text
         updates = json.loads(updates, strict=False)
-        if updates['ok'] is False:
+        if updates["ok"] is False:
             return []
-        updates = updates['result']
+        updates = updates["result"]
         # only return messages from the chatId of our user
         if fullResponse:
-            return [update['message'] for update in updates if 'message' in update and update['message']['chat']['id'] == int(telegram_data['chatId'])]
+            return [
+                update["message"]
+                for update in updates
+                if "message" in update
+                and update["message"]["chat"]["id"] == int(telegram_data["chatId"])
+            ]
         else:
-            return [update['message']['text'] for update in updates if 'message' in update and update['message']['chat']['id'] == int(telegram_data['chatId'])]
+            return [
+                update["message"]["text"]
+                for update in updates
+                if "message" in update
+                and update["message"]["chat"]["id"] == int(telegram_data["chatId"])
+            ]
     except KeyError:
         return []
 
 
 def checkTelegramData(session):
     """This function doesn't actually check any data itself, that is done by the ``telegramDataIsValid`` function. This function returns ``True`` if there is any Telegram data in the .ikabot file, and if there is none, it will ask the user to input it.
     Parameters
@@ -131,27 +171,36 @@
     -------
     valid : bool
         a boolean indicating whether or not there is valid Telegram data in the .ikabot file.
     """
     if telegramDataIsValid(session):
         return True
     else:
+        if not session.padre:  # stop asking people if process is detached
+            return False
         banner()
-        print(_('You must provide valid credentials to communicate by telegram.'))
-        print(_('You require the token of the bot you are going to use and your chat_id'))
-        print(_('For more information about how to obtain them read the readme at https://github.com/physics-sp/ikabot'))
-        rta = read(msg=_('Will you provide the credentials now? [y/N]'), values=['y', 'Y', 'n', 'N', ''])
-        if rta.lower() != 'y':
+        print(_("You must provide valid credentials to communicate by telegram."))
+        print(_("You require the token of the bot you are going to use."))
+        print(
+            _(
+                "For more information about how to obtain them read the readme at https://github.com/physics-sp/ikabot"
+            )
+        )
+        rta = read(
+            msg=_("Will you provide the credentials now? [y/N]"),
+            values=["y", "Y", "n", "N", ""],
+        )
+        if rta.lower() != "y":
             return False
         else:
             return updateTelegramData(session)
 
 
 def updateTelegramData(session, event=None, stdin_fd=None, predetermined_input=[]):
-    """This function asks the user to input the Telegram bot's token and the user's own Telegram chat id. After the user has inputted the neccessary data, this function will generate a random 4 digit number, send it to the user as a Telegram message using the token the user provided. It will then ask the user to input that number as validation.
+    """This function asks the user to input the Telegram bot's token. After the user has input the token, this function will generate a random 4 digit number, and request of the user to send it as a command to their bot. Once the command has been sent to the bot, ikabot will save the incoming message's sender's chatid and save it into the session data.
     Parameters
     ----------
     session : ikabot.web.session.Session
         Session object
     event : multiprocessing.Event
         an event which, when fired, gives back control of the terminal to the main process
     stdin_fd : int
@@ -164,94 +213,90 @@
     valid : bool
         a boolean indicating whether or not the Telegram data has been successfully updated
     """
     if event is not None and stdin_fd is not None:
         sys.stdin = os.fdopen(stdin_fd)  # give process access to terminal
     config.predetermined_input = predetermined_input
     banner()
-    print(_('To create your own Telegram Bot, read this: https://core.telegram.org/bots#3-how-do-i-create-a-bot'))
-    print(_('Just talk to @botfather in Telegram, send /newbot and then choose the bot\'s name.'))
-    print(_('Talk to your new bot and send /start'))
-    print(_('Remember to keep the token secret!\n'))
-    botToken = read(msg=_('Bot\'s token:'))
-
-    updates = ikabot.web.session.normal_get('https://api.telegram.org/bot{}/getUpdates'.format(botToken)).json()
-    if 'ok' not in updates or updates['ok'] is False:
-        print(_('invalid telegram bot, try again.'))
+    print(
+        _(
+            "To create your own Telegram bot, read this: https://core.telegram.org/bots#3-how-do-i-create-a-bot"
+        )
+    )
+    print(
+        _(
+            "1. Just talk to @botfather in Telegram, send /newbot and then choose the bot's name."
+        )
+    )
+    print(_("2. Obtain your new bot's token"))
+    print(_("3. Remember to keep the token secret!\n"))
+    botToken = read(msg=_("Bot's token: "))
+
+    updates = get(
+        "https://api.telegram.org/bot{}/getUpdates".format(botToken)
+    ).json()
+    me = get(
+        "https://api.telegram.org/bot{}/getMe".format(botToken)
+    ).json()
+    if "ok" not in updates or updates["ok"] is False:
+        print(_("Invalid Telegram bot, try again."))
         enter()
         if event is not None and stdin_fd is not None:
             event.set()
         return False
 
-    user_ids = []
-    users = []
-    for update in updates['result']:
-        if 'message' in update:
-            user = update['message']['from']
-            if user['id'] not in user_ids and 'username' in user:
-                users.append(user)
-                user_ids.append(user['id'])
+    rand = str(random.randint(0, 9999)).zfill(4)
+    print(f"\n{bcolors.GREEN}SUCCESS!{bcolors.ENDC} Telegram token is good!")
+    print(
+        f"\n4. Now send your bot the command {bcolors.BLUE}/ikabot {rand}{bcolors.ENDC} on Telegram.\nYour bot's username is @{me['result']['username']}"
+    )
 
-    if len(users) == 0:
-        print(_('make sure your personal Telegram account has a username configured and then send a random message to your bot'))
+    start = time.time()
+    user_id = None
+    try:
+        while True:
+            print(
+                f"Waiting to receive the command on Telegram... Press CTRL + C to abort.\tdt:{round(time.time()-start)}s",
+                end="\r",
+            )
+            updates = get(
+                "https://api.telegram.org/bot{}/getUpdates".format(botToken)
+            ).json()
+
+            for update in updates["result"]:
+                if "message" in update:
+                    if "text" in update["message"]:
+                        if update["message"]["text"].strip() == f"/ikabot {rand}":
+                            user_id = update["message"]["from"]["id"]
+                            break
+            time.sleep(2)
+            print(" " * 100, end="\r")
+            if user_id:
+                break
+    except KeyboardInterrupt:
+        print(
+            f"{bcolors.RED}FAILURE!{bcolors.ENDC} Did not find command {bcolors.BLUE}/ikabot {rand}{bcolors.ENDC} among received messages!\n\n{str(updates)}"
+        )
         enter()
         if event is not None and stdin_fd is not None:
             event.set()
         return False
-    elif len(users) == 1:
-        resp = read(msg=_('is your username {}? [Y/n]').format(users[0]['username']), default='y', values=['y', 'Y', 'N', 'n'])
-        if resp.lower() == 'n':
-            print(_('talk to your bot and try again'))
-            if event is not None and stdin_fd is not None:
-                event.set()
-            return False
-        else:
-            chat_id = users[0]['id']
-    else:
-        print(_('select your username:'))
-        print(_('0) My username is not listed'))
-        for i, user in enumerate(users):
-            print(_('{:d}) {}').format(i+1, user['username']))
-        resp = read(min=0, max=len(users))
-        if resp == 0:
-            print(_('talk to your bot and try again'))
-            if event is not None and stdin_fd is not None:
-                event.set()
-            return False
-        else:
-            chat_id = users[resp - 1]['id']
 
     telegram_data = {}
-    telegram_data['telegram'] = {}
-    telegram_data['telegram']['botToken'] = botToken.replace(' ', '')
-    telegram_data['telegram']['chatId'] = str(chat_id)
+    telegram_data["telegram"] = {}
+    telegram_data["telegram"]["botToken"] = botToken.replace(" ", "")
+    telegram_data["telegram"]["chatId"] = str(user_id)
     session.setSessionData(telegram_data, shared=True)
 
-    rand = str(random.randint(0, 9999)).zfill(4)
-    msg = _('The token is:{}').format(rand)
-    sendToBot(session, msg, Token=True)
+    sendToBot(session, "You have successfully set up Telegram with ikabot.", Token=True)
 
-    rta = read(msg=_('A message was sent by telegram, did you receive it? [Y/n]'), values=['y', 'Y', 'n', 'N', ''])
-    if rta.lower() == 'n':
-        valid = False
-    else:
-        recibido = read(msg=_('Enter the received token in telegram:'))
-        if rand != recibido:
-            print(_('The token is incorrect'))
-            valid = False
-        else:
-            print(_('The token is correct'))
-            valid = True
-
-    if valid is False:
-        telegram_data['telegram']['botToken'] = ''
-        telegram_data['telegram']['chatId'] = ''
-        session.setSessionData(telegram_data, shared=True)
-        print(_('Check the credentials and re-supply them.'))
-    else:
-        print(_('The data was saved.'))
+    print(
+        "\nA message was sent to you on Telegram informing you about the successful setup of the Telegram bot."
+    )
+    print(
+        "If you did not receive any message on Telegram then something has gone wrong and you will need to set up the Telegram data again!"
+    )
     enter()
 
     if event is not None and stdin_fd is not None:
         event.set()  # give main process control before exiting
-    return valid
-
+    return True
```

### Comparing `ikabot-6.6.4/ikabot/helpers/gui.py` & `ikabot-7.0.1/ikabot/helpers/gui.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,74 +1,77 @@
 #! /usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 import getpass
-import os
 import gettext
+import os
+
 from ikabot import config
 from ikabot.config import *
 
-t = gettext.translation('gui', localedir, languages=languages, fallback=True)
+t = gettext.translation("gui", localedir, languages=languages, fallback=True)
 _ = t.gettext
 
 
 def enter():
-    """Wait for the user to press Enter
-    """
+    """Wait for the user to press Enter"""
     try:
         if config.has_params:
             return
     except Exception:
         pass
     if isWindows:
-        input(_('\n[Enter]'))  # TODO improve this
+        input(_("\n[Enter]"))  # TODO improve this
     else:
-        getpass.getpass(_('\n[Enter]'))
+        getpass.getpass(_("\n[Enter]"))
 
 
 def clear():
-    """Clears all text on the console
-    """
+    """Clears all text on the console"""
     if isWindows:
-        os.system('cls')
+        os.system("cls")
     else:
-        os.system('clear')
+        os.system("clear")
 
 
 def banner():
-    """Clears all text on the console and displays the Ikabot ASCII art banner
-    """
+    """Clears all text on the console and displays the Ikabot ASCII art banner"""
     clear()
-    bner = """
+    bner = f"""
     `7MMF'  `7MM                       `7MM\"""Yp,                 mm
       MM      MM                         MM    Yb                 MM
       MM      MM  ,MP'   ,6"Yb.          MM    dP    ,pW"Wq.    mmMMmm
       MM      MM ;Y     8)   MM          MM\"""bg.   6W'   `Wb     MM
       MM      MM;Mm      ,pm9MM          MM    `Y   8M     M8     MM
       MM      MM `Mb.   8M   MM          MM    ,9   YA.   ,A9     MM
     .JMML.  .JMML. YA.  `Moo9^Yo.      .JMMmmmd9     `Ybmd9'      `Mbmo
-    """
-    print('\n{}\n\n{}\n{}'.format(bner, config.infoUser, config.update_msg))
+                                                            {IKABOT_VERSION_TAG}"""
+    print("\n{}\n\n{}\n{}".format(bner, config.infoUser, config.update_msg))
+
 
 def printChoiceList(list):
     """Prints the list with padded numbers next to each list entry.
     Parameters
     ----------
     list : list
         list to be printed
     """
-    [print('{:>{pad}}) '.format(str(i+1), pad=len(str(len(list)))) + str(item)) for i, item in enumerate(list)]
+    [
+        print("{:>{pad}}) ".format(str(i + 1), pad=len(str(len(list)))) + str(item))
+        for i, item in enumerate(list)
+    ]
+
 
 class bcolors:
-    HEADER = '\033[95m'
-    STONE = '\033[37m'
-    BLUE = '\033[94m'
-    GREEN = '\033[92m'
-    WARNING = '\033[93m'
-    RED = '\033[91m'
-    BLACK = '\033[90m'
-    ENDC = '\033[0m'
-    BOLD = '\033[1m'
-    UNDERLINE = '\033[4m'
-    DARK_RED = '\033[31m'
-    DARK_BLUE = '\033[34m'
-    DARK_GREEN = '\033[32m'
+    HEADER = "\033[95m"
+    STONE = "\033[37m"
+    BLUE = "\033[94m"
+    GREEN = "\033[92m"
+    WARNING = "\033[93m"
+    RED = "\033[91m"
+    BLACK = "\033[90m"
+    ENDC = "\033[0m"
+    BOLD = "\033[1m"
+    UNDERLINE = "\033[4m"
+    DARK_RED = "\033[31m"
+    DARK_BLUE = "\033[34m"
+    DARK_GREEN = "\033[32m"
```

### Comparing `ikabot-6.6.4/ikabot/helpers/naval.py` & `ikabot-7.0.1/ikabot/helpers/naval.py`

 * *Files identical despite different names*

### Comparing `ikabot-6.6.4/ikabot/helpers/pedirInfo.py` & `ikabot-7.0.1/ikabot/helpers/pedirInfo.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,39 @@
 #! /usr/bin/env python3
 # -*- coding: utf-8 -*-
 
-import re
-import sys
-import json
 import gettext
+import json
 import os
-from ikabot import config
+import re
+import sys
 from decimal import *
+
+from ikabot import config
 from ikabot.config import *
 from ikabot.helpers.getJson import *
 from ikabot.helpers.gui import *
+from ikabot.helpers.varios import decodeUnicodeEscape
 
-t = gettext.translation('pedirInfo', localedir, languages=languages, fallback=True)
+t = gettext.translation("pedirInfo", localedir, languages=languages, fallback=True)
 _ = t.gettext
 
 getcontext().prec = 30
 
 
-def read(min=None, max=None, digit=False, msg=prompt, values=None, empty=False, additionalValues=None, default=None):  # user input
+def read(
+    min=None,
+    max=None,
+    digit=False,
+    msg=prompt,
+    values=None,
+    empty=False,
+    additionalValues=None,
+    default=None,
+):  # user input
     """Reads input from user
     Parameters
     ----------
     min : int
         smallest number acceptable as input
     max : int
         greatest number acceptable as input
@@ -45,29 +56,29 @@
     try:
         if len(config.predetermined_input) != 0:
             return config.predetermined_input.pop(0)
     except Exception:
         pass
 
     def _invalid():
-        print('\033[1A\033[K', end="")  # remove line
+        print("\033[1A\033[K", end="")  # remove line
         return read(min, max, digit, msg, values, additionalValues=additionalValues)
 
     try:
         read_input = input(msg)
     except EOFError:
         return _invalid()
 
     if additionalValues is not None and read_input in additionalValues:
         return read_input
 
-    if read_input == '' and default is not None:
+    if read_input == "" and default is not None:
         return default
 
-    if read_input == '' and empty is True:
+    if read_input == "" and empty is True:
         return read_input
 
     if digit is True or min is not None or max is not None:
         if read_input.isdigit() is False:
             return _invalid()
         else:
             try:
@@ -95,46 +106,47 @@
     Returns
     -------
     city : City
         a city object representing the chosen city
     """
     global menu_cities
     (ids, cities) = getIdsOfCities(session)
-    if menu_cities == '':
+    if menu_cities == "":
         longest_city_name_length = 0
         for city_id in ids:
-            length = len(cities[city_id]['name'])
+            length = len(cities[city_id]["name"])
             if length > longest_city_name_length:
                 longest_city_name_length = length
 
         def pad(city_name):
-            return ' ' * (longest_city_name_length - len(city_name) + 2)
+            return " " * (longest_city_name_length - len(city_name) + 2)
 
-        resources_abbreviations = {'1': _('(W)'), '2': _('(M)'), '3': _('(C)'), '4': _('(S)')}
+        resources_abbreviations = {
+            "1": _("(W)"),
+            "2": _("(M)"),
+            "3": _("(C)"),
+            "4": _("(S)"),
+        }
 
         i = 0
         if foreign:
-            print(_(' 0: foreign city'))
+            print(_(" 0: foreign city"))
         else:
-            print('')
+            print("")
         for city_id in ids:
             i += 1
-            resource_index = cities[city_id]['tradegood']
+            resource_index = str(cities[city_id]["tradegood"])
             resource_abb = resources_abbreviations[resource_index]
-            city_name = cities[city_id]['name']
-            matches = re.findall(r'u[0-9a-f]{4}', city_name)
-            for match in matches:
-                to_unicode = '\\' + match
-                to_unicode = to_unicode.encode().decode('unicode-escape')
-                city_name = city_name.replace(match, to_unicode)
-            num = ' ' + str(i) if i < 10 else str(i)
-            menu_cities += '{}: {}{}{}\n'.format(num, city_name, pad(city_name), resource_abb)
+            city_name = decodeUnicodeEscape(cities[city_id]["name"])
+            menu_cities += "{: >2}: {}{}{}\n".format(
+                i, city_name, pad(city_name), resource_abb
+            )
         menu_cities = menu_cities[:-1]
     if foreign:
-        print(_(' 0: foreign city'))
+        print(_(" 0: foreign city"))
     print(menu_cities)
 
     if foreign:
         selected_city_index = read(min=0, max=len(ids))
     else:
         selected_city_index = read(min=1, max=len(ids))
     if selected_city_index == 0:
@@ -153,56 +165,61 @@
 
     Returns
     -------
     city : City
         a city object representing the city the user chose
     """
     banner()
-    x = read(msg='coordinate x:', digit=True)
-    y = read(msg='coordinate y:', digit=True)
-    print('')
-    url = 'view=worldmap_iso&islandX={}&islandY={}&oldBackgroundView=island&islandWorldviewScale=1'.format(x, y)
+    x = read(msg="coordinate x:", digit=True)
+    y = read(msg="coordinate y:", digit=True)
+    print("")
+    url = "view=worldmap_iso&islandX={}&islandY={}&oldBackgroundView=island&islandWorldviewScale=1".format(
+        x, y
+    )
     html = session.get(url)
     try:
-        islands_json = re.search(r'jsonData = \'(.*?)\';', html).group(1)
+        islands_json = re.search(r"jsonData = \'(.*?)\';", html).group(1)
         islands_json = json.loads(islands_json, strict=False)
-        island_id = islands_json['data'][str(x)][str(y)][0]
+        island_id = islands_json["data"][str(x)][str(y)][0]
     except Exception:
-        print(_('Incorrect coordinates'))
+        print(_("Incorrect coordinates"))
         enter()
         banner()
         return chooseCity(session, foreign=True)
     html = session.get(island_url + island_id)
     island = getIsland(html)
-    longest_city_name_length = 0
-    for city in island['cities']:
-        if city['type'] == 'city':
-            city_name_length = len(city['name'])
-            if city_name_length > longest_city_name_length:
-                longest_city_name_length = city_name_length
 
-    def pad(name):
-        return ' ' * (longest_city_name_length - len(name) + 2)
     i = 0
     city_options = []
-    for city in island['cities']:
-        if city['type'] == 'city' and city['state'] == '' and city['Name'] != session.username:
+    for city in island["cities"]:
+        if (
+            city["type"] == "city"
+            and city["state"] == ""
+            and city["Name"] != session.username
+        ):
             i += 1
-            num = ' ' + str(i) if i < 10 else str(i)
-            print('{}: {}{}({})'.format(num, city['name'], pad(city['name']), city['Name']))
+            num = " " + str(i) if i < 10 else str(i)
+            print(
+                "{: >2}: {: >{max_city_name_length}} ({})".format(
+                    num,
+                    decodeUnicodeEscape(city["name"]),
+                    decodeUnicodeEscape(city["Name"]),
+                    max_city_name_length=MAXIMUM_CITY_NAME_LENGTH,
+                )
+            )
             city_options.append(city)
     if i == 0:
-        print(_('There are no cities where to send resources on this island'))
+        print(_("There are no cities where to send resources on this island"))
         enter()
         return chooseCity(session, foreign=True)
     selected_city_index = read(min=1, max=i)
     city = city_options[selected_city_index - 1]
-    city['islandId'] = island['id']
-    city['cityName'] = city['name']
-    city['propia'] = False
+    city["islandId"] = island["id"]
+    city["cityName"] = decodeUnicodeEscape(city["name"])
+    city["isOwnCity"] = False
     return city
 
 
 def askForValue(text, max_val):
     """Displays text and asks the user to enter a value between 0 and max
 
     Parameters
@@ -214,18 +231,20 @@
 
     Returns
     -------
     var : int
         integer representing the user's input
         if the user has inputed nothing, 0 will be returned instead
     """
-    var = read(msg=text, min=0, max=max_val, default=0, additionalValues=['all', 'half'])
-    if var == 'all':
+    var = read(
+        msg=text, min=0, max=max_val, default=0, additionalValues=["all", "half"]
+    )
+    if var == "all":
         var = max_val
-    elif var == 'half':
+    elif var == "half":
         var = max_val // 2
     return var
 
 
 def getIdsOfCities(session, all=False):
     """Gets the user's cities
     Parameters
@@ -240,26 +259,39 @@
     (ids, cities) : tuple
         a tuple containing the a list of city IDs and a list of city objects
     """
     global cities_cache
     global ids_cache
     if ids_cache is None or cities_cache is None or session.padre is False:
         html = session.get()
-        cities_cache = re.search(r'relatedCityData:\sJSON\.parse\(\'(.+?),\\"additionalInfo', html).group(1) + '}'
-        cities_cache = cities_cache.replace('\\', '')
-        cities_cache = cities_cache.replace('city_', '')
+        cities_cache = (
+            re.search(
+                r'relatedCityData:\sJSON\.parse\(\'(.+?),\\"additionalInfo', html
+            ).group(1)
+            + "}"
+        )
+        cities_cache = cities_cache.replace("\\", "")
+        cities_cache = cities_cache.replace("city_", "")
         cities_cache = json.loads(cities_cache, strict=False)
 
         ids_cache = [city_id for city_id in cities_cache]
         ids_cache = sorted(ids_cache)
 
     # {'coords': '[x:y] ', 'id': idCiudad, 'tradegood': '..', 'name': 'nomberCiudad', 'relationship': 'ownCity'|'occupiedCities'|..}
     if all is False:
-        ids_own = [city_id for city_id in cities_cache if cities_cache[city_id]['relationship'] == 'ownCity']
-        ids_other = [city_id for city_id in cities_cache if cities_cache[city_id]['relationship'] != 'ownCity']
+        ids_own = [
+            city_id
+            for city_id in cities_cache
+            if cities_cache[city_id]["relationship"] == "ownCity"
+        ]
+        ids_other = [
+            city_id
+            for city_id in cities_cache
+            if cities_cache[city_id]["relationship"] != "ownCity"
+        ]
         own_cities = cities_cache.copy()
         for id in ids_other:
             del own_cities[id]
         return ids_own, own_cities
     else:
         return ids_cache, cities_cache
 
@@ -277,10 +309,10 @@
         a list containing the IDs of the users islands
     """
     (cities_ids, cities) = getIdsOfCities(session)
     islands_ids = set()
     for city_id in cities_ids:
         html = session.get(city_url + city_id)
         city = getCity(html)
-        island_id = city['islandId']
+        island_id = city["islandId"]
         islands_ids.add(island_id)
     return list(islands_ids)
```

### Comparing `ikabot-6.6.4/ikabot/helpers/planRoutes.py` & `ikabot-7.0.1/ikabot/helpers/planRoutes.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 #! /usr/bin/env python3
 # -*- coding: utf-8 -*-
 
-import re
-import time
-import math
 import json
+import math
 import random
+import re
+import time
 from decimal import *
+
 from ikabot.config import *
-from ikabot.helpers.varios import wait
 from ikabot.helpers.getJson import getCity
 from ikabot.helpers.naval import *
+from ikabot.helpers.varios import wait
 
 
 def sendGoods(session, originCityId, destinationCityId, islandId, ships, send):
     """This function will execute one route
     Parameters
     ----------
     session : ikabot.web.session.Session
@@ -32,67 +33,67 @@
     """
 
     # this can fail if a random request is made in between this two posts
     while True:
         html = session.get()
         current_city = getCity(html)  # the city the bot is right now
         city = getCity(session.get(city_url + originCityId))  # the origin city
-        currId = current_city['id']
+        currId = current_city["id"]
 
         # Change from the city the bot is sitting right now to the city we want to load resources from
         data = {
-            'action': 'header',
-            'function': 'changeCurrentCity',
-            'actionRequest': actionRequest,
-            'oldView': 'city',
-            'cityId': originCityId,
-            'backgroundView': 'city',
-            'currentCityId': currId,
-            'ajax': '1'
+            "action": "header",
+            "function": "changeCurrentCity",
+            "actionRequest": actionRequest,
+            "oldView": "city",
+            "cityId": originCityId,
+            "backgroundView": "city",
+            "currentCityId": currId,
+            "ajax": "1",
         }
 
         session.post(params=data)
 
         # Request to send the resources from the origin to the target
         data = {
-            'action': 'transportOperations',
-            'function': 'loadTransportersWithFreight',
-            'destinationCityId': destinationCityId,
-            'islandId': islandId,
-            'oldView': '',
-            'position': '',
-            'avatar2Name': '',
-            'city2Name': '',
-            'type': '',
-            'activeTab': '',
-            'transportDisplayPrice': '0',
-            'premiumTransporter': '0',
-            'transporters': ships,
-            'capacity': '5',
-            'max_capacity': '5',
-            'jetPropulsion': '0',
-            'backgroundView': 'city',
-            'currentCityId': originCityId,
-            'templateView': 'transport',
-            'currentTab': 'tabSendTransporter',
-            'actionRequest': actionRequest,
-            'ajax': '1'
+            "action": "transportOperations",
+            "function": "loadTransportersWithFreight",
+            "destinationCityId": destinationCityId,
+            "islandId": islandId,
+            "oldView": "",
+            "position": "",
+            "avatar2Name": "",
+            "city2Name": "",
+            "type": "",
+            "activeTab": "",
+            "transportDisplayPrice": "0",
+            "premiumTransporter": "0",
+            "transporters": ships,
+            "capacity": "5",
+            "max_capacity": "5",
+            "jetPropulsion": "0",
+            "backgroundView": "city",
+            "currentCityId": originCityId,
+            "templateView": "transport",
+            "currentTab": "tabSendTransporter",
+            "actionRequest": actionRequest,
+            "ajax": "1",
         }
 
         # add amounts of resources to send
         for i in range(len(send)):
-            if city['recursos'][i] > 0:
-                key = 'cargo_resource' if i == 0 else 'cargo_tradegood{:d}'.format(i)
+            if city["availableResources"][i] > 0:
+                key = "cargo_resource" if i == 0 else "cargo_tradegood{:d}".format(i)
                 data[key] = send[i]
 
         resp = session.post(params=data)
         resp = json.loads(resp, strict=False)
-        if resp[3][1][0]['type'] == 10:
+        if resp[3][1][0]["type"] == 10:
             break
-        elif resp[3][1][0]['type'] == 11:
+        elif resp[3][1][0]["type"] == 11:
             wait(getMinimumWaitingTime(session))
         time.sleep(5)
 
 
 def executeRoutes(session, routes):
     """This function will execute all the routes passed to it, regardless if there are enough ships available to do so
     Parameters
@@ -100,49 +101,68 @@
     session : ikabot.web.session.Session
         Session object
     routes : list
         a list of tuples, each of which represent a route. A route is defined like so : (originCity,destinationCity,islandId,wood,wine,marble,crystal,sulfur). originCity and destintionCity should be passed as City objects
     """
     for route in routes:
         (origin_city, destination_city, island_id, *toSend) = route
-        destination_city_id = destination_city['id']
+        destination_city_id = destination_city["id"]
 
         while sum(toSend) > 0:
-            session.setStatus(f'Sending {toSend[0]}W, {toSend[1]}V, {toSend[2]}M, {toSend[3]}C, {toSend[4]}S ---> {destination_city["name"]}')
+            session.setStatus(
+                f'Sending {toSend[0]}W, {toSend[1]}V, {toSend[2]}M, {toSend[3]}C, {toSend[4]}S ---> {destination_city["name"]}'
+            )
             ships_available = waitForArrival(session)
             storageCapacityInShips = ships_available * 500
 
-            html = session.get(city_url + str(origin_city['id']))
+            html = session.get(city_url + str(origin_city["id"]))
             origin_city = getCity(html)
             html = session.get(city_url + str(destination_city_id))
             destination_city = getCity(html)
-            foreign = str(destination_city['id']) != str(destination_city_id)
+            foreign = str(destination_city["id"]) != str(destination_city_id)
             if foreign is False:
-                storageCapacityInCity = destination_city['freeSpaceForResources']
+                storageCapacityInCity = destination_city["freeSpaceForResources"]
 
             send = []
             for i in range(len(toSend)):
                 if foreign is False:
-                    min_val = min(origin_city['recursos'][i], toSend[i], storageCapacityInShips,
-                                  storageCapacityInCity[i])
+                    min_val = min(
+                        origin_city["availableResources"][i],
+                        toSend[i],
+                        storageCapacityInShips,
+                        storageCapacityInCity[i],
+                    )
                 else:
-                    min_val = min(origin_city['recursos'][i], toSend[i], storageCapacityInShips)
+                    min_val = min(
+                        origin_city["availableResources"][i],
+                        toSend[i],
+                        storageCapacityInShips,
+                    )
                 send.append(min_val)
                 storageCapacityInShips -= send[i]
                 toSend[i] -= send[i]
 
             resources_to_send = sum(send)
             if resources_to_send == 0:
                 # no space available
                 # wait an hour and try again
                 wait(60 * 60)
                 continue
 
-            available_ships = int(math.ceil((Decimal(resources_to_send) / Decimal(500))))
-            sendGoods(session, origin_city['id'], destination_city_id, island_id, available_ships, send)
+            available_ships = int(
+                math.ceil((Decimal(resources_to_send) / Decimal(500)))
+            )
+            sendGoods(
+                session,
+                origin_city["id"],
+                destination_city_id,
+                island_id,
+                available_ships,
+                send,
+            )
 
 
 def get_random_wait_time():
     return random.randint(0, 20) * 3
 
 
 def getMinimumWaitingTime(session):
@@ -154,24 +174,27 @@
 
     Returns
     -------
     timeToWait : int
         the minimum waiting time for the closest fleet to arrive
     """
     html = session.get()
-    idCiudad = re.search(r'currentCityId:\s(\d+),', html).group(1)
-    url = 'view=militaryAdvisor&oldView=city&oldBackgroundView=city&backgroundView=city&currentCityId={}&actionRequest={}&ajax=1'.format(
-        idCiudad, actionRequest)
+    idCiudad = re.search(r"currentCityId:\s(\d+),", html).group(1)
+    url = "view=militaryAdvisor&oldView=city&oldBackgroundView=city&backgroundView=city&currentCityId={}&actionRequest={}&ajax=1".format(
+        idCiudad, actionRequest
+    )
     posted = session.post(url)
     postdata = json.loads(posted, strict=False)
-    militaryMovements = postdata[1][1][2]['viewScriptParams']['militaryAndFleetMovements']
-    current_time = int(postdata[0][1]['time'])
+    militaryMovements = postdata[1][1][2]["viewScriptParams"][
+        "militaryAndFleetMovements"
+    ]
+    current_time = int(postdata[0][1]["time"])
     delivered_times = []
-    for militaryMovement in [mv for mv in militaryMovements if mv['isOwnArmyOrFleet']]:
-        remaining_time = int(militaryMovement['eventTime']) - current_time
+    for militaryMovement in [mv for mv in militaryMovements if mv["isOwnArmyOrFleet"]]:
+        remaining_time = int(militaryMovement["eventTime"]) - current_time
         delivered_times.append(remaining_time)
     if delivered_times:
         return min(delivered_times) + get_random_wait_time()
     else:
         return 0
```

### Comparing `ikabot-6.6.4/ikabot/helpers/process.py` & `ikabot-7.0.1/ikabot/helpers/process.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 #! /usr/bin/env python3
 # -*- coding: utf-8 -*-
 
-import os
 import json
-import psutil
+import os
 import subprocess
+
+import psutil
+
 from ikabot.config import *
 from ikabot.helpers.signals import deactivate_sigint
 from ikabot.helpers.varios import normalizeDicts
 
 
 def set_child_mode(session):
     """
@@ -17,17 +19,19 @@
     session : ikabot.web.session.Session
     """
     session.padre = False
     deactivate_sigint()
 
 
 def run(command):
-    ret = subprocess.Popen(command, shell=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE).stdout.read()
+    ret = subprocess.Popen(
+        command, shell=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE
+    ).stdout.read()
     try:
-        return ret.decode('utf-8').strip()
+        return ret.decode("utf-8").strip()
     except Exception:
         return ret
 
 
 def updateProcessList(session, programprocesslist=[]):
     """This function will return data about all the active ikabot processes. If it is passed the ``programprocesslist`` argument, it will write new processes from that list to the .ikabot file
     Parameters
@@ -41,41 +45,45 @@
     -------
     runningIkabotProcessList : list[dict]
         a list of dictionaries containing relevant data about a running ikabot process ('pid', 'proxies' and 'action')
     """
     # read from file
     sessionData = session.getSessionData()
     try:
-        fileList = sessionData['processList']
+        fileList = sessionData["processList"]
     except KeyError:
         fileList = []
 
     # check it's still running
     runningIkabotProcessList = []
     ika_process = psutil.Process(pid=os.getpid()).name()
     for process in fileList:
         try:
-            proc = psutil.Process(pid=process['pid'])
+            proc = psutil.Process(pid=process["pid"])
         except psutil.NoSuchProcess:
             continue
 
         # windows doesn't support the status method
-        isAlive = True if isWindows else proc.status() != 'zombie'
+        isAlive = True if isWindows else proc.status() != "zombie"
 
         if proc.name() == ika_process and isAlive:
             runningIkabotProcessList.append(process)
 
     # add new to the list and write to file only if it's given
     for process in programprocesslist:
         if process not in runningIkabotProcessList:
             runningIkabotProcessList.append(process)
 
     # check if all proceses have new status field
-    if len([p for p in runningIkabotProcessList if 'status' not in p]) == len(runningIkabotProcessList) and len(runningIkabotProcessList):
-        runningIkabotProcessList[0]['status'] = 'running'
+    if len([p for p in runningIkabotProcessList if "status" not in p]) == len(
+        runningIkabotProcessList
+    ) and len(runningIkabotProcessList):
+        runningIkabotProcessList[0]["status"] = "running"
 
     # write to file
-    sessionData['processList'] = runningIkabotProcessList
+    sessionData["processList"] = runningIkabotProcessList
     session.setSessionData(sessionData)
 
-    #normalize process list (all processes must have properties pid, action, date and status)
-    return normalizeDicts(runningIkabotProcessList)    
+    # normalize process list (all processes must have properties pid, action, date and status)
+    normalized_processes = normalizeDicts(runningIkabotProcessList)
+    # remove dupes by pid
+    return list({d["pid"]: d for d in normalized_processes}.values())
```

### Comparing `ikabot-6.6.4/ikabot/helpers/resources.py` & `ikabot-7.0.1/ikabot/helpers/resources.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #! /usr/bin/env python3
 # -*- coding: utf-8 -*-
 
-import re
 import json
+import re
 from decimal import *
+
 from ikabot.config import *
 
 getcontext().prec = 30
 
 
 def getAvailableResources(html, num=False):
     """
@@ -15,44 +16,61 @@
     ----------
     html : string
 
     Returns
     -------
     resources_available : list[int] | list[str]
     """
-    resources = re.search(r'\\"resource\\":(\d+),\\"2\\":(\d+),\\"1\\":(\d+),\\"4\\":(\d+),\\"3\\":(\d+)}', html)
+    resources = re.search(
+        r'\\"resource\\":(\d+),\\"2\\":(\d+),\\"1\\":(\d+),\\"4\\":(\d+),\\"3\\":(\d+)}',
+        html,
+    )
     if num:
-        return [int(resources.group(1)), int(resources.group(3)), int(resources.group(2)), int(resources.group(5)), int(resources.group(4))]
+        return [
+            int(resources.group(1)),
+            int(resources.group(3)),
+            int(resources.group(2)),
+            int(resources.group(5)),
+            int(resources.group(4)),
+        ]
     else:
-        return [resources.group(1), resources.group(3), resources.group(2), resources.group(5), resources.group(4)]
+        return [
+            resources.group(1),
+            resources.group(3),
+            resources.group(2),
+            resources.group(5),
+            resources.group(4),
+        ]
 
 
 def getWarehouseCapacity(html):
     """
     Parameters
     ----------
     html : string
     Returns
     -------
     capacity : int
     """
-    capacity = re.search(r'maxResources:\s*JSON\.parse\(\'{\\"resource\\":(\d+),', html).group(1)
+    capacity = re.search(
+        r'maxResources:\s*JSON\.parse\(\'{\\"resource\\":(\d+),', html
+    ).group(1)
     return int(capacity)
 
 
-def getWineConsumption(html):
+def getWineConsumptionPerHour(html):
     """
     Parameters
     ----------
     html : string
     Returns
     -------
     capacity : int
     """
-    result = re.search(r'wineSpendings:\s(\d+)', html)
+    result = re.search(r"wineSpendings:\s(\d+)", html)
     if result:
         return int(result.group(1))
     return 0
 
 
 def getProductionPerSecond(session, city_id):
     """
@@ -61,15 +79,23 @@
     session : ikabot.web.session.Session
     city_id : int
 
     Returns
     -------
     production: tuple[Decimal, Decimal, int]
     """
-    prod = session.post(params={'action': 'header', 'function': 'changeCurrentCity', 'actionRequest': actionRequest, 'cityId': city_id, 'ajax': '1'})
+    prod = session.post(
+        params={
+            "action": "header",
+            "function": "changeCurrentCity",
+            "actionRequest": actionRequest,
+            "cityId": city_id,
+            "ajax": "1",
+        }
+    )
     prod = json.loads(prod, strict=False)
-    prod = prod[0][1]['headerData']
-    wood_production = Decimal(prod['resourceProduction'])
-    luxury_production = Decimal(prod['tradegoodProduction'])
-    luxury_resource_type = int(prod['producedTradegood'])
+    prod = prod[0][1]["headerData"]
+    wood_production = Decimal(prod["resourceProduction"])
+    luxury_production = Decimal(prod["tradegoodProduction"])
+    luxury_resource_type = int(prod["producedTradegood"])
 
     return wood_production, luxury_production, luxury_resource_type
```

### Comparing `ikabot-6.6.4/ikabot/helpers/signals.py` & `ikabot-7.0.1/ikabot/helpers/signals.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,45 +1,53 @@
 #! /usr/bin/env python3
 # -*- coding: utf-8 -*-
 
+import gettext
 import os
 import signal
-import gettext
+
 from ikabot.config import *
 from ikabot.helpers.botComm import *
 
-t = gettext.translation('signals', localedir, languages=languages, fallback=True)
+t = gettext.translation("signals", localedir, languages=languages, fallback=True)
 _ = t.gettext
 
 
 def do_nothing(signal, frame):
     pass
 
 
 def deactivate_sigint():
     signal.signal(signal.SIGINT, do_nothing)
 
 
 def create_handler(s):
     def _handler(signum, frame):
-        raise Exception(_('Signal number {:d} received').format(signum))
+        raise Exception(_("Signal number {:d} received").format(signum))
+
     return _handler
 
 
 def setSignalsHandlers(s):
-    signals = [signal.SIGINT, signal.SIGTERM]  # signal.SIGQUIT replaced with signal.SIGINT for compatibility
+    signals = [
+        signal.SIGINT,
+        signal.SIGTERM,
+    ]  # signal.SIGQUIT replaced with signal.SIGINT for compatibility
     for sgn in signals:
         signal.signal(sgn, create_handler(s))
 
 
 def setInfoSignal(session, info):  # send process info to bot
     """
     Parameters
     ----------
     session : ikabot.web.session.Session
     info : str
     """
-    info = _('information of the process {}:\n{}').format(os.getpid(), info)
+    info = _("information of the process {}:\n{}").format(os.getpid(), info)
 
     def _sendInfo(signum, frame):
         sendToBot(session, info)
-    signal.signal(signal.SIGABRT, _sendInfo)  # kill -SIGUSR1 pid, SIGUSR1 replaced with SIGABRT for compatibility
+
+    signal.signal(
+        signal.SIGABRT, _sendInfo
+    )  # kill -SIGUSR1 pid, SIGUSR1 replaced with SIGABRT for compatibility
```

### Comparing `ikabot-6.6.4/ikabot/helpers/varios.py` & `ikabot-7.0.1/ikabot/helpers/varios.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 #! /usr/bin/env python3
 # -*- coding: utf-8 -*-
 
+import random
 import re
 import time
-import random
-from decimal import *
 from datetime import datetime
+from decimal import *
 
 getcontext().prec = 30
 
 
-def addThousandSeparator(num, character='.'):
+def addThousandSeparator(num, character="."):
     """Formats the number into a string and adds a `character` for every thousand (eg. 3000 -> 3.000)
     Parameters
     ----------
     num : int
         integer number to format
     character : str
         character to act as the thousand separator
 
     Returns
     -------
     number : str
         a string representing that number with added `character` for every thousand
     """
-    return '{0:,}'.format(int(num)).replace(',', character)
+    return "{0:,}".format(int(num)).replace(",", character)
 
 
 def daysHoursMinutes(totalSeconds):
     """Formats the total number of seconds into days hours minutes (eg. 321454 -> 3D 17H)
     Parameters
     ----------
     totalSeconds : int
@@ -36,27 +36,27 @@
 
     Returns
     -------
     text : str
         formatted string (D H M)
     """
     if totalSeconds == 0:
-        return '0 s'
+        return "0 s"
     dias = int(totalSeconds / Decimal(86400))
     totalSeconds -= dias * Decimal(86400)
     horas = int(totalSeconds / Decimal(3600))
     totalSeconds -= horas * Decimal(3600)
     minutos = int(totalSeconds / Decimal(60))
-    texto = ''
+    texto = ""
     if dias > 0:
-        texto = str(dias) + 'D '
+        texto = str(dias) + "D "
     if horas > 0:
-        texto = texto + str(horas) + 'H '
+        texto = texto + str(horas) + "H "
     if minutos > 0 and dias == 0:
-        texto = texto + str(minutos) + 'M '
+        texto = texto + str(minutos) + "M "
     return texto[:-1]
 
 
 def wait(seconds, maxrandom=0):
     """This function will wait the provided number of seconds plus a random number of seconds between 0 and maxrandom
     Parameters
     -----------
@@ -64,15 +64,15 @@
         the number of seconds to wait for
     maxrandom : int
         the maximum number of additional seconds to wait for
     """
     if seconds <= 0:
         return
     randomTime = random.randint(0, maxrandom)
-    ratio = (1 + 5 ** 0.5) / 2 - 1  # 0.6180339887498949
+    ratio = (1 + 5**0.5) / 2 - 1  # 0.6180339887498949
     comienzo = time.time()
     fin = comienzo + seconds
     restantes = seconds
     while restantes > 0:
         time.sleep(restantes * ratio)
         restantes = fin - time.time()
     time.sleep(randomTime)
@@ -81,38 +81,85 @@
 def getCurrentCityId(session):
     """
     Parameters
     ----------
     session : ikabot.web.session.Session
     """
     html = session.get()
-    return re.search(r'currentCityId:\s(\d+),', html).group(1)
+    return re.search(r"currentCityId:\s(\d+),", html).group(1)
+
 
-def getDateTime(timestamp = None):
+def getDateTime(timestamp=None):
     """Returns a string of the current date and time in the YYYY-mm-dd_HH-MM-SS, if `timestamp` is provided then it converts it into the given format.
     Parameters
     ----------
     timestamp : int
         Unix timestamp to be converted
-    
+
     Returns
     -------
     text : str
         Formatted string YYYY-mm-dd_HH-MM-SS
     """
     timestamp = timestamp if timestamp else time.time()
-    return datetime.fromtimestamp(timestamp).strftime('%Y-%m-%d_%H-%M-%S')
+    return datetime.fromtimestamp(timestamp).strftime("%Y-%m-%d_%H-%M-%S")
+
 
 def normalizeDicts(list_of_dicts):
     """Returns a list of dicts that all have the same keys. Keys will be initialized to None
     Parameters
     ----------
     list_of_dicts : [dict]
         List of dicts that may have different keys (one dict has some keys that another doesn't)
-    
+
     Returns
     -------
     normalized_dicts : [dict]
         List of dicts that all have the same keys, with new ones initialized to None.
     """
     all_keys = set().union(*[d.keys() for d in list_of_dicts])
-    return [ {k: (d[k] if k in d else None) for k in all_keys} for d in list_of_dicts]
+    return [{k: (d[k] if k in d else None) for k in all_keys} for d in list_of_dicts]
+
+
+def decodeUnicodeEscape(input_string):
+    """
+    Replace Unicode escape sequences (e.g., u043c) with corresponding UTF-8 characters.
+
+    Parameters:
+    - input_string (str): The original string.
+
+    Returns:
+    - str: The string with replaced Unicode escape sequences.
+    """
+    return re.sub(
+        r"u([0-9a-fA-F]{4})", lambda x: chr(int(x.group(1), 16)), input_string
+    )
+
+
+def timeStringToSec(time_string):
+    """Returns number of seconds from a time string (eg. 5h 35m -> 20100s)
+    Parameters
+    ----------
+    time_string : str
+        String that needs to be converted to number of seconds
+
+    Returns
+    -------
+    seconds : int
+        Number of seconds
+    """
+    hours = re.search(r"(\d+)h", time_string)
+    if hours is None:
+        hours = 0
+    else:
+        hours = int(hours.group(1)) * 3600
+    minutes = re.search(r"(\d+)m", time_string)
+    if minutes is None:
+        minutes = 0
+    else:
+        minutes = int(minutes.group(1)) * 60
+    seconds = re.search(r"(\d+)s", time_string)
+    if seconds is None:
+        seconds = 0
+    else:
+        seconds = int(seconds.group(1)) * 1
+    return hours + minutes + seconds
```

### Comparing `ikabot-6.6.4/ikabot/locale/es/LC_MESSAGES/activateMiracle.po` & `ikabot-7.0.1/ikabot/locale/es/LC_MESSAGES/activateMiracle.po`

 * *Files identical despite different names*

### Comparing `ikabot-6.6.4/ikabot/locale/es/LC_MESSAGES/aesCipher.po` & `ikabot-7.0.1/ikabot/locale/es/LC_MESSAGES/aesCipher.po`

 * *Files identical despite different names*

### Comparing `ikabot-6.6.4/ikabot/locale/es/LC_MESSAGES/alertAttacks.po` & `ikabot-7.0.1/ikabot/locale/es/LC_MESSAGES/alertAttacks.po`

 * *Files identical despite different names*

### Comparing `ikabot-6.6.4/ikabot/locale/es/LC_MESSAGES/alertLowWine.po` & `ikabot-7.0.1/ikabot/locale/es/LC_MESSAGES/alertLowWine.po`

 * *Files identical despite different names*

### Comparing `ikabot-6.6.4/ikabot/locale/es/LC_MESSAGES/botComm.po` & `ikabot-7.0.1/ikabot/locale/es/LC_MESSAGES/botComm.po`

 * *Files identical despite different names*

### Comparing `ikabot-6.6.4/ikabot/locale/es/LC_MESSAGES/buyResources.po` & `ikabot-7.0.1/ikabot/locale/es/LC_MESSAGES/buyResources.po`

 * *Files identical despite different names*

### Comparing `ikabot-6.6.4/ikabot/locale/es/LC_MESSAGES/checkForUpdate.po` & `ikabot-7.0.1/ikabot/locale/es/LC_MESSAGES/checkForUpdate.po`

 * *Files identical despite different names*

### Comparing `ikabot-6.6.4/ikabot/locale/es/LC_MESSAGES/command_line.po` & `ikabot-7.0.1/ikabot/locale/es/LC_MESSAGES/command_line.po`

 * *Files identical despite different names*

### Comparing `ikabot-6.6.4/ikabot/locale/es/LC_MESSAGES/config.po` & `ikabot-7.0.1/ikabot/locale/es/LC_MESSAGES/config.po`

 * *Files identical despite different names*

### Comparing `ikabot-6.6.4/ikabot/locale/es/LC_MESSAGES/constructBuilding.po` & `ikabot-7.0.1/ikabot/locale/es/LC_MESSAGES/constructBuilding.po`

 * *Files identical despite different names*

### Comparing `ikabot-6.6.4/ikabot/locale/es/LC_MESSAGES/constructionList.po` & `ikabot-7.0.1/ikabot/locale/es/LC_MESSAGES/constructionList.po`

 * *Files identical despite different names*

### Comparing `ikabot-6.6.4/ikabot/locale/es/LC_MESSAGES/distributeResources.po` & `ikabot-7.0.1/ikabot/locale/es/LC_MESSAGES/distributeResources.po`

 * *Files identical despite different names*

### Comparing `ikabot-6.6.4/ikabot/locale/es/LC_MESSAGES/donate.po` & `ikabot-7.0.1/ikabot/locale/es/LC_MESSAGES/donate.po`

 * *Files identical despite different names*

### Comparing `ikabot-6.6.4/ikabot/locale/es/LC_MESSAGES/donationBot.po` & `ikabot-7.0.1/ikabot/locale/es/LC_MESSAGES/donationBot.po`

 * *Files identical despite different names*

### Comparing `ikabot-6.6.4/ikabot/locale/es/LC_MESSAGES/getStatus.po` & `ikabot-7.0.1/ikabot/locale/es/LC_MESSAGES/getStatus.po`

 * *Files identical despite different names*

### Comparing `ikabot-6.6.4/ikabot/locale/es/LC_MESSAGES/gui.po` & `ikabot-7.0.1/ikabot/locale/es/LC_MESSAGES/gui.po`

 * *Files identical despite different names*

### Comparing `ikabot-6.6.4/ikabot/locale/es/LC_MESSAGES/loginDaily.po` & `ikabot-7.0.1/ikabot/locale/es/LC_MESSAGES/loginDaily.po`

 * *Files identical despite different names*

### Comparing `ikabot-6.6.4/ikabot/locale/es/LC_MESSAGES/pedirInfo.mo` & `ikabot-7.0.1/ikabot/locale/es/LC_MESSAGES/pedirInfo.mo`

 * *Files identical despite different names*

### Comparing `ikabot-6.6.4/ikabot/locale/es/LC_MESSAGES/pedirInfo.po` & `ikabot-7.0.1/ikabot/locale/es/LC_MESSAGES/pedirInfo.po`

 * *Files identical despite different names*

### Comparing `ikabot-6.6.4/ikabot/locale/es/LC_MESSAGES/searchForIslandSpaces.po` & `ikabot-7.0.1/ikabot/locale/es/LC_MESSAGES/searchForIslandSpaces.po`

 * *Files identical despite different names*

### Comparing `ikabot-6.6.4/ikabot/locale/es/LC_MESSAGES/sellResources.po` & `ikabot-7.0.1/ikabot/locale/es/LC_MESSAGES/sellResources.po`

 * *Files identical despite different names*

### Comparing `ikabot-6.6.4/ikabot/locale/es/LC_MESSAGES/sendResources.po` & `ikabot-7.0.1/ikabot/locale/es/LC_MESSAGES/sendResources.po`

 * *Files identical despite different names*

### Comparing `ikabot-6.6.4/ikabot/locale/es/LC_MESSAGES/session.mo` & `ikabot-7.0.1/ikabot/locale/es/LC_MESSAGES/session.mo`

 * *Files identical despite different names*

### Comparing `ikabot-6.6.4/ikabot/locale/es/LC_MESSAGES/session.po` & `ikabot-7.0.1/ikabot/locale/es/LC_MESSAGES/session.po`

 * *Files identical despite different names*

### Comparing `ikabot-6.6.4/ikabot/locale/es/LC_MESSAGES/shipMovements.po` & `ikabot-7.0.1/ikabot/locale/es/LC_MESSAGES/shipMovements.po`

 * *Files identical despite different names*

### Comparing `ikabot-6.6.4/ikabot/locale/es/LC_MESSAGES/signals.po` & `ikabot-7.0.1/ikabot/locale/es/LC_MESSAGES/signals.po`

 * *Files identical despite different names*

### Comparing `ikabot-6.6.4/ikabot/locale/es/LC_MESSAGES/trainArmy.pot` & `ikabot-7.0.1/ikabot/locale/es/LC_MESSAGES/trainArmy.pot`

 * *Files identical despite different names*

### Comparing `ikabot-6.6.4/ikabot/locale/es/LC_MESSAGES/trainFleets.po` & `ikabot-7.0.1/ikabot/locale/es/LC_MESSAGES/trainFleets.po`

 * *Files identical despite different names*

### Comparing `ikabot-6.6.4/ikabot/locale/es/LC_MESSAGES/trainTroops.po` & `ikabot-7.0.1/ikabot/locale/es/LC_MESSAGES/trainTroops.po`

 * *Files identical despite different names*

### Comparing `ikabot-6.6.4/ikabot/locale/es/LC_MESSAGES/update.po` & `ikabot-7.0.1/ikabot/locale/es/LC_MESSAGES/update.po`

 * *Files identical despite different names*

### Comparing `ikabot-6.6.4/ikabot/locale/es/LC_MESSAGES/vacationMode.po` & `ikabot-7.0.1/ikabot/locale/es/LC_MESSAGES/vacationMode.po`

 * *Files identical despite different names*

### Comparing `ikabot-6.6.4/ikabot.egg-info/SOURCES.txt` & `ikabot-7.0.1/ikabot.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -27,28 +27,33 @@
 ikabot/function/donate.py
 ikabot/function/donationBot.py
 ikabot/function/dumpWorld.py
 ikabot/function/getStatus.py
 ikabot/function/importExportCookie.py
 ikabot/function/investigate.py
 ikabot/function/killTasks.py
+ikabot/function/loadCustomModule.py
 ikabot/function/loginDaily.py
 ikabot/function/logs.py
 ikabot/function/proxyConf.py
 ikabot/function/searchForIslandSpaces.py
 ikabot/function/sellResources.py
 ikabot/function/sendResources.py
 ikabot/function/shipMovements.py
 ikabot/function/stationArmy.py
+ikabot/function/testTelegramBot.py
 ikabot/function/trainArmy.py
 ikabot/function/update.py
 ikabot/function/vacationMode.py
+ikabot/function/webServer.py
 ikabot/helpers/__init__.py
 ikabot/helpers/aesCipher.py
+ikabot/helpers/apiComm.py
 ikabot/helpers/botComm.py
+ikabot/helpers/dns.py
 ikabot/helpers/getJson.py
 ikabot/helpers/gui.py
 ikabot/helpers/market.py
 ikabot/helpers/naval.py
 ikabot/helpers/pedirInfo.py
 ikabot/helpers/planRoutes.py
 ikabot/helpers/process.py
```

### Comparing `ikabot-6.6.4/setup.py` & `ikabot-7.0.1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 import setuptools
 
+from ikabot.config import IKABOT_VERSION
+
 setuptools.setup(
     name="ikabot",
-    version="6.6.4",
+    version=IKABOT_VERSION,
     author="physics-sp",
     author_email="physics-sp@protonmail.com",
-    license='MIT',
-    description="A bot for ikariam",
-    url="https://github.com/physics-sp/ikabot",
+    license="MIT",
+    long_description=open("README.md", "r").read(),
+    long_description_content_type="text/markdown",
+    url="https://github.com/Ikabot-Collective/ikabot",
     include_package_data=True,
     packages=setuptools.find_packages(),
-    install_requires=[
-        'requests',
-        'requests[socks]',
-        'cryptography',
-        'psutil'
-    ],
+    install_requires=["requests", "requests[socks]", "cryptography", "psutil"],
     entry_points={
-        'console_scripts': ['ikabot=ikabot.command_line:main'],
+        "console_scripts": ["ikabot=ikabot.command_line:main"],
     },
     classifiers=[
         "Programming Language :: Python :: 3",
-        "License :: OSI Approved :: MIT License"
+        "License :: OSI Approved :: MIT License",
     ],
 )
```


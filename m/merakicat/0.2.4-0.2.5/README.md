# Comparing `tmp/merakicat-0.2.4.tar.gz` & `tmp/merakicat-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "merakicat-0.2.4.tar", last modified: Fri Apr 12 16:51:37 2024, max compression
+gzip compressed data, was "merakicat-0.2.5.tar", last modified: Thu Apr 25 13:24:34 2024, max compression
```

## Comparing `merakicat-0.2.4.tar` & `merakicat-0.2.5.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:51:37.393708 merakicat-0.2.4/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:51:37.381708 merakicat-0.2.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:51:37.381708 merakicat-0.2.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-12 16:51:28.000000 merakicat-0.2.4/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2154 2024-04-12 16:51:28.000000 merakicat-0.2.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-12 16:51:28.000000 merakicat-0.2.4/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-04-12 16:51:28.000000 merakicat-0.2.4/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3180 2024-04-12 16:51:28.000000 merakicat-0.2.4/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-12 16:51:28.000000 merakicat-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-12 16:51:28.000000 merakicat-0.2.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-04-12 16:51:28.000000 merakicat-0.2.4/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)    11871 2024-04-12 16:51:37.389708 merakicat-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7622 2024-04-12 16:51:28.000000 merakicat-0.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:51:37.381708 merakicat-0.2.4/files/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-12 16:51:28.000000 merakicat-0.2.4/files/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:51:37.385708 merakicat-0.2.4/images/
--rw-r--r--   0 runner    (1001) docker     (127)    55062 2024-04-12 16:51:28.000000 merakicat-0.2.4/images/botcongrats.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    78377 2024-04-12 16:51:28.000000 merakicat-0.2.4/images/cisco_meraki.png
--rw-r--r--   0 runner    (1001) docker     (127)    54965 2024-04-12 16:51:28.000000 merakicat-0.2.4/images/createbot.jpg
--rw-r--r--   0 runner    (1001) docker     (127)  1774034 2024-04-12 16:51:28.000000 merakicat-0.2.4/images/mc_quick.gif
--rw-r--r--   0 runner    (1001) docker     (127)    12826 2024-04-12 16:51:28.000000 merakicat-0.2.4/images/merakicat.png
--rw-r--r--   0 runner    (1001) docker     (127)    22117 2024-04-12 16:51:28.000000 merakicat-0.2.4/images/newapp.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    87754 2024-04-12 16:51:28.000000 merakicat-0.2.4/images/newbot.jpg
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-12 16:51:28.000000 merakicat-0.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-12 16:51:28.000000 merakicat-0.2.4/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 16:51:37.393708 merakicat-0.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-04-12 16:51:28.000000 merakicat-0.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:51:37.381708 merakicat-0.2.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:51:37.389708 merakicat-0.2.4/src/merakicat/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:51:28.000000 merakicat-0.2.4/src/merakicat/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:51:37.389708 merakicat-0.2.4/src/merakicat/batch_helper/
--rw-r--r--   0 runner    (1001) docker     (127)    14141 2024-04-12 16:51:28.000000 merakicat-0.2.4/src/merakicat/batch_helper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-04-12 16:51:28.000000 merakicat-0.2.4/src/merakicat/batch_helper/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6935 2024-04-12 16:51:28.000000 merakicat-0.2.4/src/merakicat/batch_helper/exceptions.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      338 2024-04-12 16:51:28.000000 merakicat-0.2.4/src/merakicat/bulk_check.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      397 2024-04-12 16:51:28.000000 merakicat-0.2.4/src/merakicat/bulk_migrate.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)     6424 2024-04-12 16:51:28.000000 merakicat-0.2.4/src/merakicat/mc_cfg_check.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4629 2024-04-12 16:51:28.000000 merakicat-0.2.4/src/merakicat/mc_claim.py
--rw-r--r--   0 runner    (1001) docker     (127)     5901 2024-04-12 16:51:28.000000 merakicat-0.2.4/src/merakicat/mc_cloud_mon.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1215 2024-04-12 16:51:28.000000 merakicat-0.2.4/src/merakicat/mc_file_exists.py
--rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-04-12 16:51:28.000000 merakicat-0.2.4/src/merakicat/mc_get_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-04-12 16:51:28.000000 merakicat-0.2.4/src/merakicat/mc_get_nms.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    54918 2024-04-12 16:51:28.000000 merakicat-0.2.4/src/merakicat/mc_pedia.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      631 2024-04-12 16:51:28.000000 merakicat-0.2.4/src/merakicat/mc_ping.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8817 2024-04-12 16:51:28.000000 merakicat-0.2.4/src/merakicat/mc_register.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2215 2024-04-12 16:51:28.000000 merakicat-0.2.4/src/merakicat/mc_splitcheck_serials.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    35749 2024-04-12 16:51:28.000000 merakicat-0.2.4/src/merakicat/mc_translate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-04-12 16:51:28.000000 merakicat-0.2.4/src/merakicat/mc_user_info.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    90886 2024-04-12 16:51:28.000000 merakicat-0.2.4/src/merakicat/merakicat.py
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-12 16:51:28.000000 merakicat-0.2.4/src/merakicat/test.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:51:37.389708 merakicat-0.2.4/src/merakicat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11871 2024-04-12 16:51:37.000000 merakicat-0.2.4/src/merakicat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-04-12 16:51:37.000000 merakicat-0.2.4/src/merakicat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 16:51:37.000000 merakicat-0.2.4/src/merakicat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 16:51:37.000000 merakicat-0.2.4/src/merakicat.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-12 16:51:37.000000 merakicat-0.2.4/src/merakicat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-12 16:51:37.000000 merakicat-0.2.4/src/merakicat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-12 16:51:28.000000 merakicat-0.2.4/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:24:34.895661 merakicat-0.2.5/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:24:34.883662 merakicat-0.2.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:24:34.887662 merakicat-0.2.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-25 13:24:28.000000 merakicat-0.2.5/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2154 2024-04-25 13:24:28.000000 merakicat-0.2.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-25 13:24:28.000000 merakicat-0.2.5/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-04-25 13:24:28.000000 merakicat-0.2.5/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3271 2024-04-25 13:24:28.000000 merakicat-0.2.5/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-25 13:24:28.000000 merakicat-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-25 13:24:28.000000 merakicat-0.2.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-04-25 13:24:28.000000 merakicat-0.2.5/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)    12147 2024-04-25 13:24:34.895661 merakicat-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7815 2024-04-25 13:24:28.000000 merakicat-0.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:24:34.887662 merakicat-0.2.5/files/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-25 13:24:28.000000 merakicat-0.2.5/files/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:24:34.891662 merakicat-0.2.5/images/
+-rw-r--r--   0 runner    (1001) docker     (127)    55062 2024-04-25 13:24:28.000000 merakicat-0.2.5/images/botcongrats.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    78377 2024-04-25 13:24:28.000000 merakicat-0.2.5/images/cisco_meraki.png
+-rw-r--r--   0 runner    (1001) docker     (127)    54965 2024-04-25 13:24:28.000000 merakicat-0.2.5/images/createbot.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)  1774034 2024-04-25 13:24:28.000000 merakicat-0.2.5/images/mc_quick.gif
+-rw-r--r--   0 runner    (1001) docker     (127)    12826 2024-04-25 13:24:28.000000 merakicat-0.2.5/images/merakicat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    22117 2024-04-25 13:24:28.000000 merakicat-0.2.5/images/newapp.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    87754 2024-04-25 13:24:28.000000 merakicat-0.2.5/images/newbot.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-25 13:24:28.000000 merakicat-0.2.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-25 13:24:28.000000 merakicat-0.2.5/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 13:24:34.895661 merakicat-0.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-04-25 13:24:28.000000 merakicat-0.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:24:34.883662 merakicat-0.2.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:24:34.895661 merakicat-0.2.5/src/merakicat/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:24:28.000000 merakicat-0.2.5/src/merakicat/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:24:34.895661 merakicat-0.2.5/src/merakicat/batch_helper/
+-rw-r--r--   0 runner    (1001) docker     (127)    14141 2024-04-25 13:24:28.000000 merakicat-0.2.5/src/merakicat/batch_helper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-04-25 13:24:28.000000 merakicat-0.2.5/src/merakicat/batch_helper/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6935 2024-04-25 13:24:28.000000 merakicat-0.2.5/src/merakicat/batch_helper/exceptions.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      338 2024-04-25 13:24:28.000000 merakicat-0.2.5/src/merakicat/bulk_check.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      397 2024-04-25 13:24:28.000000 merakicat-0.2.5/src/merakicat/bulk_migrate.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6487 2024-04-25 13:24:28.000000 merakicat-0.2.5/src/merakicat/mc_cfg_check.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4690 2024-04-25 13:24:28.000000 merakicat-0.2.5/src/merakicat/mc_claim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5779 2024-04-25 13:24:28.000000 merakicat-0.2.5/src/merakicat/mc_cloud_mon.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1275 2024-04-25 13:24:28.000000 merakicat-0.2.5/src/merakicat/mc_file_exists.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-04-25 13:24:28.000000 merakicat-0.2.5/src/merakicat/mc_get_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-04-25 13:24:28.000000 merakicat-0.2.5/src/merakicat/mc_get_nms.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    54918 2024-04-25 13:24:28.000000 merakicat-0.2.5/src/merakicat/mc_pedia.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      631 2024-04-25 13:24:28.000000 merakicat-0.2.5/src/merakicat/mc_ping.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8881 2024-04-25 13:24:28.000000 merakicat-0.2.5/src/merakicat/mc_register.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2215 2024-04-25 13:24:28.000000 merakicat-0.2.5/src/merakicat/mc_splitcheck_serials.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    35813 2024-04-25 13:24:28.000000 merakicat-0.2.5/src/merakicat/mc_translate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-04-25 13:24:28.000000 merakicat-0.2.5/src/merakicat/mc_user_info.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    91540 2024-04-25 13:24:28.000000 merakicat-0.2.5/src/merakicat/merakicat.py
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-25 13:24:28.000000 merakicat-0.2.5/src/merakicat/test.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:24:34.895661 merakicat-0.2.5/src/merakicat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12147 2024-04-25 13:24:34.000000 merakicat-0.2.5/src/merakicat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-04-25 13:24:34.000000 merakicat-0.2.5/src/merakicat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 13:24:34.000000 merakicat-0.2.5/src/merakicat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 13:24:34.000000 merakicat-0.2.5/src/merakicat.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-25 13:24:34.000000 merakicat-0.2.5/src/merakicat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-25 13:24:34.000000 merakicat-0.2.5/src/merakicat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-25 13:24:28.000000 merakicat-0.2.5/tox.ini
```

### Comparing `merakicat-0.2.4/.gitignore` & `merakicat-0.2.5/.gitignore`

 * *Files identical despite different names*

### Comparing `merakicat-0.2.4/CONTRIBUTING.rst` & `merakicat-0.2.5/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `merakicat-0.2.4/HISTORY.md` & `merakicat-0.2.5/HISTORY.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # History
 
+## 0.2.5 (04-25-2024)
+
+  - Reverted back to Finbarr Brady's webex-bot after a pull merge.
+
 ## 0.2.4 (04-12-2024)
 
   - Added Private VLAN -> Port Isolation to encyclopedia.
   - Removed older bot code.
   - Updated AUTHORS.rst.
   - Updated .gitignore
```

### Comparing `merakicat-0.2.4/LICENSE` & `merakicat-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `merakicat-0.2.4/Makefile` & `merakicat-0.2.5/Makefile`

 * *Files identical despite different names*

### Comparing `merakicat-0.2.4/PKG-INFO` & `merakicat-0.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: merakicat
-Version: 0.2.4
+Version: 0.2.5
 Summary: An app to check and translate Catalyst switch configs to Meraki.
 Home-page: https://github.com/ecoen66/merakicat
 Author: Ed Coen
 Author-email: ecoen@cisco.com
 License: MIT license
 Keywords: merakicat,catalyst,meraki,cisco,migration,webexteamsbot
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -13,15 +13,15 @@
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.rst
-Requires-Dist: webex-bot-ecoen66==0.4.3
+Requires-Dist: webex-bot==0.4.7
 Requires-Dist: webexteamssdk==1.6.1
 Requires-Dist: Flask>=0.12.1
 Requires-Dist: netmiko==4.3.0
 Requires-Dist: tabulate==0.9.0
 Requires-Dist: ciscoconfparse2==0.5
 Requires-Dist: meraki==1.42.0
 Requires-Dist: python-docx==1.1.0
@@ -230,26 +230,35 @@
 Migrate a list of Catalyst switches to a Meraki network, 20 switches at a time, until the entire list is exhausted. The list is provided in an input file, one hostname/fqdn/IP address per line:
 ```
 cd src/merakicat
 bulk_migrate.sh <input file> <Meraki network name>
 ```
 
 
+# Donations
+
+If you found this repo to be useful, please consider donating to Life Decisions, Rockford, IL through a purchase from the [Merakicat store](https://bonfire.com/store/merakicat).
+
+
 # Credits
 **This project is _heavily_ based on the work of others:**
 
 `Catalyst_to_Meraki_Migration_Tool` by [Fady Sharobeem](https://github.com/fadysharobeem).
 
 `Catalyst_2_Meraki_Config_Checker` by [Fady Sharobeem](https://github.com/fadysharobeem).
 
 The bot functionality is based on the `webex_bot` project by [Finbarr Brady](https://github.com/fbradyirl).
 
 
 # History
 
+## 0.2.5 (04-25-2024)
+
+  - Reverted back to Finbarr Brady's webex-bot after a pull merge.
+
 ## 0.2.4 (04-12-2024)
 
   - Added Private VLAN -> Port Isolation to encyclopedia.
   - Removed older bot code.
   - Updated AUTHORS.rst.
   - Updated .gitignore
```

### Comparing `merakicat-0.2.4/README.md` & `merakicat-0.2.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -200,14 +200,19 @@
 Migrate a list of Catalyst switches to a Meraki network, 20 switches at a time, until the entire list is exhausted. The list is provided in an input file, one hostname/fqdn/IP address per line:
 ```
 cd src/merakicat
 bulk_migrate.sh <input file> <Meraki network name>
 ```
 
 
+# Donations
+
+If you found this repo to be useful, please consider donating to Life Decisions, Rockford, IL through a purchase from the [Merakicat store](https://bonfire.com/store/merakicat).
+
+
 # Credits
 **This project is _heavily_ based on the work of others:**
 
 `Catalyst_to_Meraki_Migration_Tool` by [Fady Sharobeem](https://github.com/fadysharobeem).
 
 `Catalyst_2_Meraki_Config_Checker` by [Fady Sharobeem](https://github.com/fadysharobeem).
```

### Comparing `merakicat-0.2.4/images/botcongrats.jpg` & `merakicat-0.2.5/images/botcongrats.jpg`

 * *Files identical despite different names*

### Comparing `merakicat-0.2.4/images/cisco_meraki.png` & `merakicat-0.2.5/images/cisco_meraki.png`

 * *Files identical despite different names*

### Comparing `merakicat-0.2.4/images/createbot.jpg` & `merakicat-0.2.5/images/createbot.jpg`

 * *Files identical despite different names*

### Comparing `merakicat-0.2.4/images/mc_quick.gif` & `merakicat-0.2.5/images/mc_quick.gif`

 * *Files identical despite different names*

### Comparing `merakicat-0.2.4/images/merakicat.png` & `merakicat-0.2.5/images/merakicat.png`

 * *Files identical despite different names*

### Comparing `merakicat-0.2.4/images/newapp.jpg` & `merakicat-0.2.5/images/newapp.jpg`

 * *Files identical despite different names*

### Comparing `merakicat-0.2.4/images/newbot.jpg` & `merakicat-0.2.5/images/newbot.jpg`

 * *Files identical despite different names*

### Comparing `merakicat-0.2.4/setup.py` & `merakicat-0.2.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 with open('README.md') as readme_file:
     readme = readme_file.read()
 
 with open('HISTORY.md') as history_file:
     history = history_file.read()
 
 requirements = [
-    "webex-bot-ecoen66==0.4.3",
+    "webex-bot==0.4.7",
     "webexteamssdk==1.6.1",
     "Flask>=0.12.1",
     "netmiko==4.3.0",
     "tabulate==0.9.0",
     "ciscoconfparse2==0.5",
     "meraki==1.42.0",
     "python-docx==1.1.0",
```

### Comparing `merakicat-0.2.4/src/merakicat/batch_helper/__init__.py` & `merakicat-0.2.5/src/merakicat/batch_helper/__init__.py`

 * *Files identical despite different names*

### Comparing `merakicat-0.2.4/src/merakicat/batch_helper/config.py` & `merakicat-0.2.5/src/merakicat/batch_helper/config.py`

 * *Files identical despite different names*

### Comparing `merakicat-0.2.4/src/merakicat/batch_helper/exceptions.py` & `merakicat-0.2.5/src/merakicat/batch_helper/exceptions.py`

 * *Files identical despite different names*

### Comparing `merakicat-0.2.4/src/merakicat/mc_cfg_check.py` & `merakicat-0.2.5/src/merakicat/mc_cfg_check.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 from ciscoconfparse2 import CiscoConfParse
-from mc_user_info import DEBUG, DEBUG_CHECKER
 from mc_pedia import mc_pedia
+try:
+    from mc_user_info import DEBUG, DEBUG_CHECKER
+except ImportError:
+    DEBUG = DEBUG_CHECKER = False
 
 
 def CheckFeatures(sw_file):
     """
     This function will check a Catalyst switch config file for feature
     mapping to Meraki.
     :param sw_file: The incoming config filespec
```

### Comparing `merakicat-0.2.4/src/merakicat/mc_claim.py` & `merakicat-0.2.5/src/merakicat/mc_claim.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 import meraki
 import re
-from mc_user_info import DEBUG, DEBUG_CLAIM
+try:
+    from mc_user_info import DEBUG, DEBUG_CLAIM
+except ImportError:
+    DEBUG = DEBUG_CLAIM = False
 
 
 def Claim(dashboard, dest_net, serials):
     """
     This function will claim a set of Meraki network device serial numbers
     to a Meraki network.
     :param dashboard: The active Meraki dashboard API session to use
```

### Comparing `merakicat-0.2.4/src/merakicat/mc_cloud_mon.py` & `merakicat-0.2.5/src/merakicat/mc_cloud_mon.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 from netmiko import ConnectHandler
 import meraki
-from mc_user_info import DEBUG
 import re
 import os
+try:
+    from mc_user_info import DEBUG
+except ImportError:
+    DEBUG = False
 
 
-def CloudSwitch(dashboard, meraki_org, host_id, ios_username, ios_password, ios_port, ios_secret):
+def CloudSwitch(dashboard, meraki_org, host_id, ios_username, ios_password,
+                ios_port, ios_secret):
     """
-    This function will write a Catalyst switch config to a file, check the
-    switch for compatibility with Cloud Monitoring, create a backup config
-    on the switch, enroll the switch and modify the config for Cloud
-    Monitoring.
+    This function is under construction....
+    It will enroll a Catalyst switch into Dashboard for Cloud Monitoring.
     :param dashboard: Dashboard API session instance
     :param meraki_org: Meraki Organization ID
     :param host_id: The switch or stack to SSH into
     :param ios_username: Username for SSH
     :param ios_password: Password for SSH
     :param ios_port: Port number for SSH
     :param ios_secret: IOSXE secret password for CLI escalation
-    :return: The hostname & the filespec for the saved config file.
+    :return: (I'm not sure yet what I will return other than success/failure')
     """
 
     debug = DEBUG
 
     devices = list()
     host_name = ""
 
@@ -40,15 +42,16 @@
     net_connect = ConnectHandler(**session_info)
     switch_name = net_connect.find_prompt()
     net_connect.enable()
     switch_name = net_connect.find_prompt()
     switch_name = switch_name[:len(switch_name) - 1]
     net_connect.send_command('term len 0')
     config = net_connect.send_command('show running-config')
-    sudi_chain = net_connect.send_command('show cry pki certificates pem CISCO_IDEVID_SUDI')
+    sudi_chain = net_connect.send_command(
+      'show cry pki certificates pem CISCO_IDEVID_SUDI')
     regex = re.compile(r"%\sGeneral Purpose Certificate:\s *", flags=re.I)
     if len(regex.split(sudi_chain)) > 1:
         if not regex.split(sudi_chain)[1] == "":
             maybe_sudi = regex.split(sudi_chain)[1]
             print(f"maybe_sudi = \n{maybe_sudi}")
             sudi = maybe_sudi.replace('\n','\n        ')
             print(f"sudi = \n{sudi}")
@@ -102,14 +105,12 @@
 
     devices.append(dev_info2)
     # devices = []
     # devices = [{'sudi': '-----BEGIN CERTIFICATE-----\n        MIIDyTCCArGgAwIBAgIKBBNXOVCGU1YztjANBgkqhkiG9w0BAQsFADAnMQ4wDAYD\n        VQQKEwVDaXNjbzEVMBMGA1UEAxMMQUNUMiBTVURJIENBMB4XDTIxMDUzMTEzNTUx\n        NVoXDTI5MDUxNDIwMjU0MVowbTEpMCcGA1UEBRMgUElEOkM5MjAwTC0yNFAtNEcg\n        U046SkFFMjUyMjBSMksxDjAMBgNVBAoTBUNpc2NvMRgwFgYDVQQLEw9BQ1QtMiBM\n        aXRlIFNVREkxFjAUBgNVBAMTDUM5MjAwTC0yNFAtNEcwggEiMA0GCSqGSIb3DQEB\n        AQUAA4IBDwAwggEKAoIBAQDaUPxW76gT5MdoEAt+UrDFiYA9RYh2iHicDViBEyow\n        TR1TuP36bHh13X3vtGiDsCD88Ci2TZIqd/EDkkc7v9ipUUYVVH+YDrPt2Aukb1PH\n        D6K0R+KhgEzRo5x54TlU6oWvjUpwNZUwwdhMWIQaUVkMyZBYNy0jGPLO8jwZhyBg\n        1Fneybr9pwedGbLrAaz+gdEikB8B4a/fvPjVfL5Ngb4QRjFqWuE+X3nLc0kHedep\n        6nfgpUNXMlStVm5nIXKP6OjmzfCHPYh9L2Ehs1TrSk1ser9Ofx0ZMVL/jBZR2EIj\n        OZ8tH6KlX2/B2pbSPIO6kD5c4UA8Cf1SbDJCwJ/kI9ihAgMBAAGjgbAwga0wDgYD\n        VR0PAQH/BAQDAgXgMAwGA1UdEwEB/wQCMAAwHwYDVR0jBBgwFoAUSNjx8cJw1Vu7\n        fHMJk6+4uDAD+H8wTQYDVR0RBEYwRKBCBgkrBgEEAQkVAgOgNRMzQ2hpcElEPVVV\n        VUNNaElGcUVFMklFUUVBQWNBQUFBQUFBQUFBQUFBQUFBQUFBQUFBQUE9MB0GA1Ud\n        DgQWBBRdhMkFD/z5hokaQeLbaRsp4hkvbzANBgkqhkiG9w0BAQsFAAOCAQEAMtuh\n        YpBz4xEZ7YdJsLpw67Q0TTJGnTBRpzAeY1urYDoDz8TSx556XG7z3IRzuED5KVSp\n        OwmH/iZ+tDfYQ3W3ElWTW93871DkuW4WQIfbnoHg/F7bF0DKYVkD3rpZjyz3NhzH\n        d7cjTdJXQ85bTAOXDuxKH3qewrXxxOGXgh3I6NUq0UwMTWh84lND7Jl+ZAQkYNS2\n        iHanTZFQBk3ML0NUb7fKDYGRTZRqwQ/upIO4S6LV1cxH/6V0qbMy3sCSHZoMLrW3\n        0m3M6yKpe5+VZzHZwmWdUf3Ot+zKjhveK5/YNsMIASdvtvymxUizq2Hr1hvR/kPc\n        p1vuyWxipU8JfzOh/A==\n        -----END CERTIFICATE-----\n        ', 'tunnel': {'certificateName': 'DeviceSUDI', 'name': 'MERAKI', 'loopbackNumber': 1000, 'localInterface': 1}, 'user': {'username': 'Meraki'}, 'vty': {'startLineNumber': 16, 'endLineNumber': 17, 'authentication': {'group': {'name': ''}}, 'authorization': {'group': {'name': 'MERAKI'}}, 'accessList': {'vtyIn': {'name': 'MERAKI_IN'}, 'vtyOut': {'name': 'MERAKI_OUT'}}, 'rotaryNumber': 50}}]
 
     print(f"devices = {devices}")
     print(f"meraki_org = {meraki_org}")
-    # try:
-    # db = meraki.DashboardAPI('9939da9713a2ca5f4ef503900c264fb911c1d890')
     response = dashboard.organizations.getOrganizationInventoryOnboardingCloudMonitoringNetworks(meraki_org, 'switch', total_pages='all')
     print(f"Response = {response}")
     response = dashboard.organizations.createOrganizationInventoryOnboardingCloudMonitoringPrepare(meraki_org, devices)
     print(f"Response = {response}")
     return(switch_name, config_file)
```

### Comparing `merakicat-0.2.4/src/merakicat/mc_file_exists.py` & `merakicat-0.2.5/src/merakicat/mc_file_exists.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 import os
-from mc_user_info import DEBUG, DEBUG_FILE
+try:
+    from mc_user_info import DEBUG, DEBUG_FILE
+except ImportError:
+    DEBUG = DEBUG_FILE = False
 
 
 def FileExists(filespec):
     """
     Checks to see if a filespec can be found, and is a file.
     :param filespec: The incoming user text from Teams or the command line
     :return :The filespec (possibly modified) and True or False
```

### Comparing `merakicat-0.2.4/src/merakicat/mc_get_config.py` & `merakicat-0.2.5/src/merakicat/mc_get_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 from netmiko import ConnectHandler
-from mc_user_info import DEBUG
 import os
+try:
+    from mc_user_info import DEBUG
+except ImportError:
+    DEBUG = False
 
 
 def GetConfig(host_id, ios_username, ios_password, ios_port, ios_secret):
     """
     This function will write a Catalyst switch config to a file.
     :param host: The hostname, fqdn or IP address of a switch/stack.
     :return: The hostname, the filespec for the saved config file.
```

### Comparing `merakicat-0.2.4/src/merakicat/mc_get_nms.py` & `merakicat-0.2.5/src/merakicat/mc_get_nms.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 from netmiko import ConnectHandler
-from mc_user_info import DEBUG
 import re
+try:
+    from mc_user_info import DEBUG
+except ImportError:
+    DEBUG = False
 
 
 def GetNmList(host_id, ios_username, ios_password, ios_port, ios_secret):
     """
     This function will check a Catalyst IOSXE switch for compatibility with
     Meraki management prior to registering the switch (or stack) to Dashboard.
     Items checked include:
@@ -60,8 +63,8 @@
         else:
             nm_list.append("")
         x += 1
     if debug:
         print(f"For the {qty_switches} switches in the stack, " +
               f"the NM modules are {nm_list}")
     net_connect.disconnect()
-    return(nm_list)
+    return(nm_list)
```

### Comparing `merakicat-0.2.4/src/merakicat/mc_pedia.py` & `merakicat-0.2.5/src/merakicat/mc_pedia.py`

 * *Files identical despite different names*

### Comparing `merakicat-0.2.4/src/merakicat/mc_ping.py` & `merakicat-0.2.5/src/merakicat/mc_ping.py`

 * *Files identical despite different names*

### Comparing `merakicat-0.2.4/src/merakicat/mc_register.py` & `merakicat-0.2.5/src/merakicat/mc_register.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 from netmiko import ConnectHandler
-from mc_user_info import DEBUG, DEBUG_REGISTER
 from mc_get_nms import GetNmList
 import re
+try:
+    from mc_user_info import DEBUG, DEBUG_REGISTER
+except ImportError:
+    DEBUG = DEBUG_REGISTER = False
 
 
 def Register(host_id, ios_username, ios_password, ios_port, ios_secret):
     """
     This function will check a Catalyst IOSXE switch for compatibility with
     Meraki management prior to registering the switch (or stack) to Dashboard.
     Items checked include:
```

### Comparing `merakicat-0.2.4/src/merakicat/mc_splitcheck_serials.py` & `merakicat-0.2.5/src/merakicat/mc_splitcheck_serials.py`

 * *Files identical despite different names*

### Comparing `merakicat-0.2.4/src/merakicat/mc_translate.py` & `merakicat-0.2.5/src/merakicat/mc_translate.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 import batch_helper
 import json
 import pprint
 import re
 import sys
 from ciscoconfparse2 import CiscoConfParse
 from collections import defaultdict
-from mc_user_info import DEBUG, DEBUG_TRANSLATOR
 from mc_pedia import mc_pedia, nm_dict
+try:
+    from mc_user_info import DEBUG, DEBUG_TRANSLATOR
+except ImportError:
+    DEBUG = DEBUG_TRANSLATOR = False
 
 
 def Evaluate(config_file, nm_list):
     """
     This parent function will evaluate a Catalyst switch config file and
     reports on which features that are being used can and cannot be mapped to
     Meraki features.
@@ -351,15 +354,15 @@
             print(f"Switch with serial number {sw['serial']} has "+
                   f"{port_max} ports.")
         if not port_max == sw['ports']:
             print(f"Switch with serial number {sw['serial']} has {port_max} "+
                   f"ports, not {sw['ports']}!")
             sys.exit()
 
-    # Create a batch action lists
+    # Create batch action lists
     action_list = list()
     all_actions = list()
     returns_dict = {}
     post_ports_list = list()
     # Create good and bad port lists
     conf_ports = defaultdict(list)
     unconf_ports = defaultdict(list)
```

### Comparing `merakicat-0.2.4/src/merakicat/mc_user_info.py` & `merakicat-0.2.5/src/merakicat/mc_user_info.py`

 * *Files identical despite different names*

### Comparing `merakicat-0.2.4/src/merakicat/merakicat.py` & `merakicat-0.2.5/src/merakicat/merakicat.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,39 @@
 # -*- coding: utf-8 -*-
 """
 Meraki Cat webexteamsbot is a chat bot with a swiss army knife
 of functions for checking & translating Catalyst IOSXE to Meraki
 switch configs, registering Catalyst switches to Dashboard and
 claiming them.  It can also be run from the command line or in
 batch from a shell script.
+
+
+Please excuse the code, I need to refactor it -- badly.
 """
 import meraki
 import urllib.request
 import requests
 import shutil
 import docx
 import os
 import json
 import re
 import sys
 import time
-from webex_bot_ecoen66.webex_bot import WebexBot
-from webex_bot_ecoen66.models.response import Response
-from webex_bot_ecoen66.models.command import Command
+from webex_bot.webex_bot import WebexBot
+from webex_bot.models.response import Response
+from webex_bot.models.command import Command
 from netmiko import ConnectHandler
 from docx2pdf import convert
 from docx.enum.text import WD_ALIGN_PARAGRAPH
 from docx.shared import Inches
 from docx.oxml import OxmlElement
 from docx.oxml.ns import qn
 from mc_cfg_check import CheckFeatures
-from mc_translate import Evaluate, MerakiConfig  # ,MerakiConfig_up
+from mc_translate import Evaluate, MerakiConfig
 from mc_claim import Claim
 from mc_register import Register
 from mc_cloud_mon import CloudSwitch
 from mc_get_nms import GetNmList
 from mc_splitcheck_serials import SplitCheckSerials
 from mc_ping import Ping
 from mc_file_exists import FileExists
@@ -102,97 +105,115 @@
 from mc_pedia import mc_pedia
 
 # If we were run without arguments, run as a BOT
 # Otherwise, we will attempt to use the args in batch mode
 BOT = False
 if len(sys.argv) == 1:
     BOT = True
+
+
 class RunCheck(Command):
 
     def __init__(self):
         super().__init__(
             command_keyword="check",
             help_message="Check a Catalyst switch config for both translatable and possible \
 Meraki features",
             delete_previous_message=True)
 
     def execute(self, message, attachment_actions, activity):
-        print(f"attachment_actions={attachment_actions}")
         return greeting(attachment_actions)
 
+
 class RunRegister(Command):
 
     def __init__(self):
         super().__init__(
             command_keyword="register",
             help_message="Register a Catalyst switch to the Meraki Dashboard",
             delete_previous_message=True)
 
     def execute(self, message, attachment_actions, activity):
         return greeting(attachment_actions)
 
+
 class RunClaim(Command):
 
     def __init__(self):
         super().__init__(
             command_keyword="claim",
             help_message="Claim Catalyst switches to a Meraki Network",
             delete_previous_message=True)
 
     def execute(self, message, attachment_actions, activity):
         return greeting(attachment_actions)
 
+
 class RunTranslate(Command):
 
     def __init__(self):
         super().__init__(
             command_keyword="translate",
             help_message="Translate a Catalyst switch config from a file or \
 host to claimed Meraki serial numbers",
             delete_previous_message=True)
 
     def execute(self, message, attachment_actions, activity):
         return greeting(attachment_actions)
 
+
 class RunMigrate(Command):
 
     def __init__(self):
         super().__init__(
             command_keyword="migrate",
             help_message="Migrate a Catalyst switch to a Meraki switch - \
 register, claim & translate",
             delete_previous_message=True)
 
     def execute(self, message, attachment_actions, activity):
         return greeting(attachment_actions)
 
+
 class RunDemo(Command):
 
     def __init__(self):
         super().__init__(
             command_keyword="demo",
             help_message="Create a demo report for all features currently in \
 the feature encyclopedia",
             delete_previous_message=True)
 
     def execute(self, message, attachment_actions, activity):
         return greeting(attachment_actions)
 
+
 class RunHelp(Command):
 
     def __init__(self):
         super().__init__(
-            command_keyword="help",
+            command_keyword="help|?",
             help_message="Get help",
             delete_previous_message=True)
 
     def execute(self, message, attachment_actions, activity):
         return greeting(attachment_actions)
 
 
+class RunHello(Command):
+
+    def __init__(self):
+        super().__init__(
+            command_keyword="hello|hi",
+            help_message="Say hello",
+            delete_previous_message=True)
+
+    def execute(self, message, attachment_actions, activity):
+        return greeting(attachment_actions)
+
 teams_emails = list()
 if BOT:
     # Retrieve required details from environment variables
     bot_email = os.getenv("TEAMS_BOT_EMAIL")
     bot_app_name = os.getenv("TEAMS_BOT_APP_NAME")
     teams_token = os.getenv("TEAMS_BOT_TOKEN")
     if not os.getenv("TEAMS_EMAILS") is None:
@@ -253,16 +274,14 @@
 ios_password = os.getenv("IOS_PASSWORD")
 ios_secret = os.getenv("IOS_SECRET")
 ios_port = os.getenv("IOS_PORT")
 # If the required details were not in the environment variables
 # grab them from the mc_user_info.py file
 if ios_username is None:
     ios_username = IOS_USERNAME
-if ios_username is None:
-    ios_username = IOS_USERNAME
 if ios_password is None:
     ios_password = IOS_PASSWORD
 if ios_secret is None:
     ios_secret = IOS_SECRET
 if ios_port is None:
     ios_port = IOS_PORT
     if ios_port is None:
@@ -289,15 +308,14 @@
         print(f"meraki_orgs = {meraki_orgs}")
     x = 0
     while x <= len(meraki_orgs) - 1:
         if meraki_orgs[x]['name'] == meraki_org_name:
             try:
                 raw_nets = dashboard.organizations.getOrganizationNetworks(
                     organizationId=meraki_orgs[x]['id'])
-
             except meraki.exceptions.APIError:
                 print("We were unable to get the list of networks" +
                       f" for {meraki_orgs[x]['name']}.")
                 sys.exit()
             if debug:
                 print(raw_nets)
             y = 0
@@ -358,16 +376,16 @@
         # approved_domains=[],
         # approved_rooms=[],
         threads=False,
         help_command=RunHelp(),
         log_level="ERROR"
     )
 
-# Create a custom bot greeting function, returned when no /command is given.
-# The default behavior of the bot is to return the '/help' command response
+# The greeting processes user input before calling the correct command.
+# The default behavior of the bot is to return the 'help' command response
 # If there is an English language command line, try to work with that.
 
 
 def greeting(incoming_msg):
 
     global config_file, host_id, meraki_net, meraki_net_name
     global meraki_serials, times, report, detailed
@@ -435,15 +453,16 @@
                 user_text = regex.split(user_text)[0].strip()
                 if not re.search(',', maybe_targets, re.IGNORECASE) == None:
                     maybe_targets = maybe_targets.replace(" ", "")
                 if debug:
                     print(f"maybe_targets = {maybe_targets}")
                 if not len(maybe_targets)==0:
                     targets = re.split(';|,|\s',maybe_targets)
-                    print(f"regex.split(user_text)[0] = {regex.split(user_text)[0]}")
+                    if debug:
+                        print(f"regex.split(user_text)[0] = {regex.split(user_text)[0]}")
         if debug:
             print(f"targets = {targets}")
         # Did they enter a network name after "network"?
         dest_net = meraki_net
         regex = re.compile(r"\s*network\s *", flags=re.I)
         if not regex.split(user_text)[1] == "":
             # They did, so register it!
@@ -902,15 +921,15 @@
                     else:
                         # All good, let's go claim the serial numbers to
                         # the network
                         response.markdown = claim_switch(incoming_msg,
                                                          dest_net=dest_net,
                                                          serials=serials)
 
-        case "help":
+        case "help" | "?":
             if BOT:
                 # Lookup details about sender for our default response
                 sender = bot.teams.people.get(incoming_msg.personId)
                 r = "Well {}, here's a list of ".format(sender.firstName)
                 r += "commands that I understand. "
                 response.markdown = r
                 for line in bot_commands:
@@ -987,15 +1006,15 @@
     # Grab the list of devices for that Network
     try:
         devices = dashboard.networks.getNetworkDevices(dest_net)
     except meraki.exceptions.APIError:
         r = "We were unable to get the list of devices for that network."
         return (r)
     if debug:
-        print(f"devices = {switches}")
+        print(f"devices = {devices}")
 
     # Loop through the devices searching for cloud monitored C9300s
     success_list = list()
     if targets == []:
         targets = ['C9300']
     if debug:
         print(f"targets = {targets}")
@@ -1009,50 +1028,59 @@
                 print(f"short_mod = {short_mod}")
             if short_mod in targets:
                 # Found one...
                 sw_name = devices[x]['name']
 
                 # Grab the list of config files archived for the switch
                 try:
-                    url = f"https://api.meraki.com/api/v1/devices/{devices[x]['serial']}/switch/configs"
+                    url = "https://api.meraki.com/api/v1/devices/"
+                    url += f"{devices[x]['serial']}/switch/configs"
                     payload = {}
                     headers = {
                       'X-Cisco-Meraki-API-Key': meraki_api_key
                     }
-                    response = requests.request("GET", url, headers=headers, data=payload)
+                    response = requests.request("GET",
+                                                url,
+                                                headers=headers,
+                                                data=payload)
                 except:
                     print(f"ERROR getting the config list for {sw_name}")
                     x += 1
                 conf_list = response.json()
                 # If the Python meraki SDK ever supports this it should look
                 # like this:
                 #
-                # conf_list = dashboard.devices.getSwitchConfigs(devices[x]['serial'])
+                # conf_list = dashboard.devices.getSwitchConfigs(
+                #   devices[x]['serial'])
 
                 if debug:
                     print(f"conf_list = {conf_list}")
                     print(f"len(conf_list) = {len(conf_list)}")
                     print(f"conf_list[0] = {conf_list[0]}")
 
-                # Assuming there are and configs in the list, we will grab a copy
-                # of the first (latest) one.
+                # Assuming there are and configs in the list, we will grab a
+                # copy of the first (latest) one.
                 if len(conf_list) > 0:
                     url += "/" + conf_list[0]['id']
                     if debug:
                         print(f"url = {url}")
                     try:
-                        response = requests.request("GET", url, headers=headers, data=payload)
+                        response = requests.request("GET",
+                                                    url,
+                                                    headers=headers,
+                                                    data=payload)
                     except:
                         print(f"ERROR getting config for {sw_name}")
                         x += 1
                     c = response.json()
-                    # If the Python meraki SDK ever supports this it should look
-                    # like this:
+                    # If the Python meraki SDK ever supports this it should
+                    # look like this:
                     #
-                    # c = dashboard.devices.getSwitchConfigs(devices[x]['serial'],conf_list[0]['id'])
+                    # c = dashboard.devices.getSwitchConfigs(
+                    #   devices[x]['serial'],conf_list[0]['id'])
 
                     # Now that we have the config, let's save a copy
                     dir = os.path.join(os.getcwd(), "../../files")
                     config_file = os.path.join(dir, sw_name + ".cfg")
                     file = open(config_file, "w")
                     file.writelines(c['config'])
                     file.close()
@@ -1610,15 +1638,15 @@
                 payload = "```\n%s" % thing + "\n```" + timing
                 r = f"We **{status}** registered **{vals.count('Registered')}"
                 r += "** switch"
                 r += f"{'es' if (vals.count('Registered') > 1) else ''}"
                 return (r + f":\n{payload}")
             else:
                 payload = "\n%s" % thing + timing
-                r = f"\n\nWe {status} registered {vals.count('Registered')}"
+                r = f"\n\nWe {status} registered {vals.count('Registered')} "
                 r += f"switch{'es' if (vals.count('Registered') > 1) else ''}"
                 return (r + f":\n{payload}")
         else:
             payload = ""
             for issue in issues:
                 payload += issue + "\n"
             r = f"We were unsuccessful registering {host}:\n\n{payload}"
@@ -2150,14 +2178,15 @@
          "Migrate a Catalyst switch to a Meraki switch - register, claim & \
 translate"],
 
         ["* **demo report**",
          "Create a demo report for all features currently in the feature \
 encyclopedia"]])
 
+    bot.add_command(RunHello())
     bot.add_command(RunHelp())
     bot.add_command(RunCheck())
     bot.add_command(RunRegister())
     bot.add_command(RunClaim())
     bot.add_command(RunTranslate())
     bot.add_command(RunMigrate())
     bot.add_command(RunDemo())
```

### Comparing `merakicat-0.2.4/src/merakicat.egg-info/PKG-INFO` & `merakicat-0.2.5/src/merakicat.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: merakicat
-Version: 0.2.4
+Version: 0.2.5
 Summary: An app to check and translate Catalyst switch configs to Meraki.
 Home-page: https://github.com/ecoen66/merakicat
 Author: Ed Coen
 Author-email: ecoen@cisco.com
 License: MIT license
 Keywords: merakicat,catalyst,meraki,cisco,migration,webexteamsbot
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -13,15 +13,15 @@
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.rst
-Requires-Dist: webex-bot-ecoen66==0.4.3
+Requires-Dist: webex-bot==0.4.7
 Requires-Dist: webexteamssdk==1.6.1
 Requires-Dist: Flask>=0.12.1
 Requires-Dist: netmiko==4.3.0
 Requires-Dist: tabulate==0.9.0
 Requires-Dist: ciscoconfparse2==0.5
 Requires-Dist: meraki==1.42.0
 Requires-Dist: python-docx==1.1.0
@@ -230,26 +230,35 @@
 Migrate a list of Catalyst switches to a Meraki network, 20 switches at a time, until the entire list is exhausted. The list is provided in an input file, one hostname/fqdn/IP address per line:
 ```
 cd src/merakicat
 bulk_migrate.sh <input file> <Meraki network name>
 ```
 
 
+# Donations
+
+If you found this repo to be useful, please consider donating to Life Decisions, Rockford, IL through a purchase from the [Merakicat store](https://bonfire.com/store/merakicat).
+
+
 # Credits
 **This project is _heavily_ based on the work of others:**
 
 `Catalyst_to_Meraki_Migration_Tool` by [Fady Sharobeem](https://github.com/fadysharobeem).
 
 `Catalyst_2_Meraki_Config_Checker` by [Fady Sharobeem](https://github.com/fadysharobeem).
 
 The bot functionality is based on the `webex_bot` project by [Finbarr Brady](https://github.com/fbradyirl).
 
 
 # History
 
+## 0.2.5 (04-25-2024)
+
+  - Reverted back to Finbarr Brady's webex-bot after a pull merge.
+
 ## 0.2.4 (04-12-2024)
 
   - Added Private VLAN -> Port Isolation to encyclopedia.
   - Removed older bot code.
   - Updated AUTHORS.rst.
   - Updated .gitignore
```

### Comparing `merakicat-0.2.4/src/merakicat.egg-info/SOURCES.txt` & `merakicat-0.2.5/src/merakicat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `merakicat-0.2.4/tox.ini` & `merakicat-0.2.5/tox.ini`

 * *Files identical despite different names*


# Comparing `tmp/nonebot_plugin_simulator_xiuxian-0.5.27.tar.gz` & `tmp/nonebot_plugin_simulator_xiuxian-0.5.30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_simulator_xiuxian-0.5.27.tar", last modified: Tue Apr 23 18:55:28 2024, max compression
+gzip compressed data, was "nonebot_plugin_simulator_xiuxian-0.5.30.tar", last modified: Thu Apr 25 01:36:11 2024, max compression
```

## Comparing `nonebot_plugin_simulator_xiuxian-0.5.27.tar` & `nonebot_plugin_simulator_xiuxian-0.5.30.tar`

### file list

```diff
@@ -1,26 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-23 18:55:28.752312 nonebot_plugin_simulator_xiuxian-0.5.27/
--rw-rw-rw-   0        0        0     1089 2024-04-22 01:25:08.000000 nonebot_plugin_simulator_xiuxian-0.5.27/LICENSE
--rw-rw-rw-   0        0        0     5638 2024-04-23 18:55:28.752312 nonebot_plugin_simulator_xiuxian-0.5.27/PKG-INFO
--rw-rw-rw-   0        0        0     4958 2024-04-22 01:25:08.000000 nonebot_plugin_simulator_xiuxian-0.5.27/README.md
-drwxrwxrwx   0        0        0        0 2024-04-23 18:55:28.740392 nonebot_plugin_simulator_xiuxian-0.5.27/nonebot_plugin_simulator_xiuxian/
--rw-rw-rw-   0        0        0     1790 2024-04-22 23:37:32.000000 nonebot_plugin_simulator_xiuxian-0.5.27/nonebot_plugin_simulator_xiuxian/__init__.py
--rw-rw-rw-   0        0        0     1960 2024-04-22 01:25:08.000000 nonebot_plugin_simulator_xiuxian-0.5.27/nonebot_plugin_simulator_xiuxian/cd_manager.py
--rw-rw-rw-   0        0        0      360 2024-04-22 22:16:40.000000 nonebot_plugin_simulator_xiuxian-0.5.27/nonebot_plugin_simulator_xiuxian/config.py
--rw-rw-rw-   0        0        0     2849 2024-04-22 01:25:08.000000 nonebot_plugin_simulator_xiuxian-0.5.27/nonebot_plugin_simulator_xiuxian/data_source.py
--rw-rw-rw-   0        0        0     1787 2024-04-22 01:25:08.000000 nonebot_plugin_simulator_xiuxian-0.5.27/nonebot_plugin_simulator_xiuxian/exp_util.py
--rw-rw-rw-   0        0        0     4430 2024-04-22 01:25:08.000000 nonebot_plugin_simulator_xiuxian-0.5.27/nonebot_plugin_simulator_xiuxian/item_json.py
--rw-rw-rw-   0        0        0    50728 2024-04-22 01:25:08.000000 nonebot_plugin_simulator_xiuxian-0.5.27/nonebot_plugin_simulator_xiuxian/player_fight.py
--rw-rw-rw-   0        0        0     8141 2024-04-22 01:25:08.000000 nonebot_plugin_simulator_xiuxian-0.5.27/nonebot_plugin_simulator_xiuxian/read_buff.py
--rw-rw-rw-   0        0        0     8555 2024-04-22 01:25:08.000000 nonebot_plugin_simulator_xiuxian-0.5.27/nonebot_plugin_simulator_xiuxian/utils.py
--rw-rw-rw-   0        0        0    54293 2024-04-22 01:25:08.000000 nonebot_plugin_simulator_xiuxian-0.5.27/nonebot_plugin_simulator_xiuxian/xiuxian2_handle.py
--rw-rw-rw-   0        0        0     5780 2024-04-22 01:25:08.000000 nonebot_plugin_simulator_xiuxian-0.5.27/nonebot_plugin_simulator_xiuxian/xiuxian_config.py
--rw-rw-rw-   0        0        0      787 2024-04-22 01:25:08.000000 nonebot_plugin_simulator_xiuxian-0.5.27/nonebot_plugin_simulator_xiuxian/xiuxian_opertion.py
--rw-rw-rw-   0        0        0     2477 2024-04-23 18:31:40.000000 nonebot_plugin_simulator_xiuxian-0.5.27/nonebot_plugin_simulator_xiuxian/xiuxian_xiazaishuju.py
-drwxrwxrwx   0        0        0        0 2024-04-23 18:55:28.751320 nonebot_plugin_simulator_xiuxian-0.5.27/nonebot_plugin_simulator_xiuxian.egg-info/
--rw-rw-rw-   0        0        0     5638 2024-04-23 18:55:28.000000 nonebot_plugin_simulator_xiuxian-0.5.27/nonebot_plugin_simulator_xiuxian.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      938 2024-04-23 18:55:28.000000 nonebot_plugin_simulator_xiuxian-0.5.27/nonebot_plugin_simulator_xiuxian.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 18:55:28.000000 nonebot_plugin_simulator_xiuxian-0.5.27/nonebot_plugin_simulator_xiuxian.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      101 2024-04-23 18:55:28.000000 nonebot_plugin_simulator_xiuxian-0.5.27/nonebot_plugin_simulator_xiuxian.egg-info/requires.txt
--rw-rw-rw-   0        0        0       33 2024-04-23 18:55:28.000000 nonebot_plugin_simulator_xiuxian-0.5.27/nonebot_plugin_simulator_xiuxian.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       85 2024-04-23 18:55:28.756255 nonebot_plugin_simulator_xiuxian-0.5.27/setup.cfg
--rw-rw-rw-   0        0        0      980 2024-04-23 18:38:28.000000 nonebot_plugin_simulator_xiuxian-0.5.27/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-25 01:36:11.679252 nonebot_plugin_simulator_xiuxian-0.5.30/
+-rw-rw-rw-   0        0        0     1089 2024-04-22 01:25:08.000000 nonebot_plugin_simulator_xiuxian-0.5.30/LICENSE
+-rw-rw-rw-   0        0        0     5940 2024-04-25 01:36:11.679252 nonebot_plugin_simulator_xiuxian-0.5.30/PKG-INFO
+-rw-rw-rw-   0        0        0     4958 2024-04-22 01:25:08.000000 nonebot_plugin_simulator_xiuxian-0.5.30/README.md
+drwxrwxrwx   0        0        0        0 2024-04-25 01:36:11.672243 nonebot_plugin_simulator_xiuxian-0.5.30/nonebot_plugin_simulator_xiuxian/
+-rw-rw-rw-   0        0        0      381 2024-04-25 01:04:12.000000 nonebot_plugin_simulator_xiuxian-0.5.30/nonebot_plugin_simulator_xiuxian/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-25 01:36:11.678243 nonebot_plugin_simulator_xiuxian-0.5.30/nonebot_plugin_simulator_xiuxian.egg-info/
+-rw-rw-rw-   0        0        0     5940 2024-04-25 01:36:11.000000 nonebot_plugin_simulator_xiuxian-0.5.30/nonebot_plugin_simulator_xiuxian.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      360 2024-04-25 01:36:11.000000 nonebot_plugin_simulator_xiuxian-0.5.30/nonebot_plugin_simulator_xiuxian.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 01:36:11.000000 nonebot_plugin_simulator_xiuxian-0.5.30/nonebot_plugin_simulator_xiuxian.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      243 2024-04-25 01:36:11.000000 nonebot_plugin_simulator_xiuxian-0.5.30/nonebot_plugin_simulator_xiuxian.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       33 2024-04-25 01:36:11.000000 nonebot_plugin_simulator_xiuxian-0.5.30/nonebot_plugin_simulator_xiuxian.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       85 2024-04-25 01:36:11.680243 nonebot_plugin_simulator_xiuxian-0.5.30/setup.cfg
+-rw-rw-rw-   0        0        0     1407 2024-04-25 01:36:05.000000 nonebot_plugin_simulator_xiuxian-0.5.30/setup.py
```

### Comparing `nonebot_plugin_simulator_xiuxian-0.5.27/LICENSE` & `nonebot_plugin_simulator_xiuxian-0.5.30/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_simulator_xiuxian-0.5.27/PKG-INFO` & `nonebot_plugin_simulator_xiuxian-0.5.30/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot_plugin_simulator_xiuxian
-Version: 0.5.27
+Version: 0.5.30
 Summary: 修仙
 Home-page: https://github.com/luoyefufeng/nonebot_plugin_simulator_xiuxian
 Author: 甘城菜月
 Author-email: 2859385794@qq.com
 License: MIT license
 Platform: all
 Description-Content-Type: text/markdown
@@ -13,14 +13,24 @@
 Requires-Dist: nonebot-adapter-onebot
 Requires-Dist: wget
 Requires-Dist: nonebot_plugin_apscheduler
 Requires-Dist: Pillow==9.5.0
 Requires-Dist: pydantic
 Requires-Dist: wcwidth
 Requires-Dist: ujson
+Requires-Dist: xiuxianxiuxian_base
+Requires-Dist: xiuxian_bank
+Requires-Dist: xiuxian_base
+Requires-Dist: xiuxian_boss
+Requires-Dist: xiuxian_buff
+Requires-Dist: xiuxian_info
+Requires-Dist: xiuxian_mixelixir
+Requires-Dist: xiuxian_rift
+Requires-Dist: xiuxian_sect
+Requires-Dist: xiuxian_work
 
 # nonebot_plugin_simulator_xiuxian
 
 _:tada::tada::tada:修仙模拟器！:tada::tada::tada:_
 
 ## 简介
```

### Comparing `nonebot_plugin_simulator_xiuxian-0.5.27/README.md` & `nonebot_plugin_simulator_xiuxian-0.5.30/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_simulator_xiuxian-0.5.27/nonebot_plugin_simulator_xiuxian.egg-info/PKG-INFO` & `nonebot_plugin_simulator_xiuxian-0.5.30/nonebot_plugin_simulator_xiuxian.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot_plugin_simulator_xiuxian
-Version: 0.5.27
+Version: 0.5.30
 Summary: 修仙
 Home-page: https://github.com/luoyefufeng/nonebot_plugin_simulator_xiuxian
 Author: 甘城菜月
 Author-email: 2859385794@qq.com
 License: MIT license
 Platform: all
 Description-Content-Type: text/markdown
@@ -13,14 +13,24 @@
 Requires-Dist: nonebot-adapter-onebot
 Requires-Dist: wget
 Requires-Dist: nonebot_plugin_apscheduler
 Requires-Dist: Pillow==9.5.0
 Requires-Dist: pydantic
 Requires-Dist: wcwidth
 Requires-Dist: ujson
+Requires-Dist: xiuxianxiuxian_base
+Requires-Dist: xiuxian_bank
+Requires-Dist: xiuxian_base
+Requires-Dist: xiuxian_boss
+Requires-Dist: xiuxian_buff
+Requires-Dist: xiuxian_info
+Requires-Dist: xiuxian_mixelixir
+Requires-Dist: xiuxian_rift
+Requires-Dist: xiuxian_sect
+Requires-Dist: xiuxian_work
 
 # nonebot_plugin_simulator_xiuxian
 
 _:tada::tada::tada:修仙模拟器！:tada::tada::tada:_
 
 ## 简介
```


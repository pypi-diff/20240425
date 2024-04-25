# Comparing `tmp/nonebot_plugin_game_collection-3.0.3.post1.tar.gz` & `tmp/nonebot_plugin_game_collection-3.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_game_collection-3.0.3.post1.tar", max compression
+gzip compressed data, was "nonebot_plugin_game_collection-3.0.4.tar", max compression
```

## Comparing `nonebot_plugin_game_collection-3.0.3.post1.tar` & `nonebot_plugin_game_collection-3.0.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1086 2023-10-28 21:32:04.942263 nonebot_plugin_game_collection-3.0.3.post1/LICENSE
--rw-r--r--   0        0        0      931 2024-04-16 11:46:27.481877 nonebot_plugin_game_collection-3.0.3.post1/nonebot_plugin_game_collection/__init__.py
--rw-r--r--   0        0        0      402 2024-04-23 17:24:05.134340 nonebot_plugin_game_collection-3.0.3.post1/pyproject.toml
--rw-r--r--   0        0        0     2984 2024-04-15 12:09:00.697493 nonebot_plugin_game_collection-3.0.3.post1/README.md
--rw-r--r--   0        0        0     3360 1970-01-01 00:00:00.000000 nonebot_plugin_game_collection-3.0.3.post1/PKG-INFO
+-rw-r--r--   0        0        0     1086 2023-10-28 21:32:04.942263 nonebot_plugin_game_collection-3.0.4/LICENSE
+-rw-r--r--   0        0        0      854 2024-04-25 17:17:19.355663 nonebot_plugin_game_collection-3.0.4/nonebot_plugin_game_collection/__init__.py
+-rw-r--r--   0        0        0      394 2024-04-25 17:18:24.127869 nonebot_plugin_game_collection-3.0.4/pyproject.toml
+-rw-r--r--   0        0        0     2984 2024-04-15 12:09:00.697493 nonebot_plugin_game_collection-3.0.4/README.md
+-rw-r--r--   0        0        0     3348 1970-01-01 00:00:00.000000 nonebot_plugin_game_collection-3.0.4/PKG-INFO
```

### Comparing `nonebot_plugin_game_collection-3.0.3.post1/LICENSE` & `nonebot_plugin_game_collection-3.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-3.0.3.post1/nonebot_plugin_game_collection/__init__.py` & `nonebot_plugin_game_collection-3.0.4/nonebot_plugin_game_collection/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-from clovers.core.plugin import PluginLoader
-from nonebot_plugin_clovers import adapter, __plugin_meta__ as nonebot_plugin_clovers_plugin_meta
 from nonebot.log import logger
 from nonebot.plugin import PluginMetadata
+from clovers.core.plugin import PluginLoader
+from nonebot_plugin_clovers import clovers
 
 __plugin_meta__ = PluginMetadata(
     name="小游戏合集",
     description="各种群内小游戏",
     usage="金币签到",
     type="application",
     homepage="https://github.com/KarisAya/nonebot_plugin_game_collection",
-    supported_adapters=nonebot_plugin_clovers_plugin_meta.supported_adapters,
+    supported_adapters={"nonebot.adapters.onebot.v11"},
 )
 
 
 def load_plugin(name: str):
     plugin = PluginLoader.load(name)
     if plugin is None:
         logger.error(f"未找到{name}")
-    elif plugin not in adapter.plugins:
-        adapter.plugins.append(plugin)
+    elif plugin not in clovers.plugins:
+        clovers.plugins.append(plugin)
         logger.success(f"{name}加载成功")
     else:
         logger.success(f"{name}已存在")
 
 
 load_plugin("clovers_apscheduler")
 load_plugin("clovers_leafgame")
```

### Comparing `nonebot_plugin_game_collection-3.0.3.post1/README.md` & `nonebot_plugin_game_collection-3.0.4/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-3.0.3.post1/PKG-INFO` & `nonebot_plugin_game_collection-3.0.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-game-collection
-Version: 3.0.3.post1
+Version: 3.0.4
 Summary: 
 Author: KarisAya
 Author-email: 1048827424@qq.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: clovers-leafgame (>=0.1.4,<0.2.0)
-Requires-Dist: nonebot-plugin-clovers[nonebot] (>=0.1.2.post3,<0.2.0)
+Requires-Dist: nonebot-plugin-clovers[nonebot] (>=0.1.4,<0.2.0)
 Description-Content-Type: text/markdown
 
 <!-- markdownlint-disable MD031 MD033 MD036 MD041 -->
 
 <div align="center">
 
 <a href="https://v2.nonebot.dev/store">
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-game-collection Version: 3.0.3.post1
+Metadata-Version: 2.1 Name: nonebot-plugin-game-collection Version: 3.0.4
 Summary: Author: KarisAya Author-email: 1048827424@qq.com Requires-Python:
 >=3.10,<4.0 Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Requires-Dist: clovers-leafgame (>=0.1.4,<0.2.0) Requires-Dist:
-nonebot-plugin-clovers[nonebot] (>=0.1.2.post3,<0.2.0) Description-Content-
-Type: text/markdown
+nonebot-plugin-clovers[nonebot] (>=0.1.4,<0.2.0) Description-Content-Type:
+text/markdown
                               _[_N_o_n_e_B_o_t_P_l_u_g_i_n_L_o_g_o_]
                               [NoneBotPluginText]
 # nonebot-plugin-game-collection _â¨ æ¹èª [nonebot_plugin_russian](https://
   github.com/HibiKier/nonebot_plugin_russian) å [nonebot_plugin_horserace]
 (https://github.com/shinianj/nonebot_plugin_horserace) çå°æ¸¸æåé â¨_
                     [python]_[_l_i_c_e_n_s_e_]_[_p_y_p_i_]_[_p_y_p_i_ _d_o_w_n_l_o_a_d_]
 ## ð¿ å®è£ ä»¥ä¸æå°çæ¹æ³ ä»»é**å¶ä¸** å³å¯ [æ¨è] ä½¿ç¨
```


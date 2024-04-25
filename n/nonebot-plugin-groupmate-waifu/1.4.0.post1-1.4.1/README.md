# Comparing `tmp/nonebot_plugin_groupmate_waifu-1.4.0.post1.tar.gz` & `tmp/nonebot_plugin_groupmate_waifu-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_groupmate_waifu-1.4.0.post1.tar", max compression
+gzip compressed data, was "nonebot_plugin_groupmate_waifu-1.4.1.tar", max compression
```

## Comparing `nonebot_plugin_groupmate_waifu-1.4.0.post1.tar` & `nonebot_plugin_groupmate_waifu-1.4.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1086 2023-11-06 04:36:06.280670 nonebot_plugin_groupmate_waifu-1.4.0.post1/LICENSE
--rw-r--r--   0        0        0      944 2024-04-23 16:45:25.163822 nonebot_plugin_groupmate_waifu-1.4.0.post1/nonebot_plugin_groupmate_waifu/__init__.py
--rw-r--r--   0        0        0      437 2024-04-23 17:19:03.163918 nonebot_plugin_groupmate_waifu-1.4.0.post1/pyproject.toml
--rw-r--r--   0        0        0     2520 2024-04-23 16:36:28.534422 nonebot_plugin_groupmate_waifu-1.4.0.post1/README.md
--rw-r--r--   0        0        0     2949 1970-01-01 00:00:00.000000 nonebot_plugin_groupmate_waifu-1.4.0.post1/PKG-INFO
+-rw-r--r--   0        0        0     1086 2023-11-06 04:36:06.280670 nonebot_plugin_groupmate_waifu-1.4.1/LICENSE
+-rw-r--r--   0        0        0      867 2024-04-25 17:20:52.736619 nonebot_plugin_groupmate_waifu-1.4.1/nonebot_plugin_groupmate_waifu/__init__.py
+-rw-r--r--   0        0        0      409 2024-04-25 17:22:13.753605 nonebot_plugin_groupmate_waifu-1.4.1/pyproject.toml
+-rw-r--r--   0        0        0     2520 2024-04-23 16:36:28.534422 nonebot_plugin_groupmate_waifu-1.4.1/README.md
+-rw-r--r--   0        0        0     2897 1970-01-01 00:00:00.000000 nonebot_plugin_groupmate_waifu-1.4.1/PKG-INFO
```

### Comparing `nonebot_plugin_groupmate_waifu-1.4.0.post1/LICENSE` & `nonebot_plugin_groupmate_waifu-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_groupmate_waifu-1.4.0.post1/nonebot_plugin_groupmate_waifu/__init__.py` & `nonebot_plugin_groupmate_waifu-1.4.1/nonebot_plugin_groupmate_waifu/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from clovers.core.plugin import PluginLoader
-from nonebot_plugin_clovers import adapter, __plugin_meta__ as nonebot_plugin_clovers_plugin_meta
+from nonebot_plugin_clovers import clovers
 from nonebot.log import logger
 from nonebot.plugin import PluginMetadata
 
 __plugin_meta__ = PluginMetadata(
     name="娶群友",
     description="娶一个群友做老婆",
     usage="娶群友，透群友",
     type="application",
     homepage="https://github.com/KarisAya/nonebot_plugin_groupmate_waifu",
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
 load_plugin("clovers_groupmate_waifu")
```

### Comparing `nonebot_plugin_groupmate_waifu-1.4.0.post1/README.md` & `nonebot_plugin_groupmate_waifu-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_groupmate_waifu-1.4.0.post1/PKG-INFO` & `nonebot_plugin_groupmate_waifu-1.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-groupmate-waifu
-Version: 1.4.0.post1
+Version: 1.4.1
 Summary: 
 Author: KarisAya
 Author-email: 1048827424@qq.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: clovers (>=0.1.4,<0.2.0)
 Requires-Dist: clovers-groupmate-waifu (>=0.1.0.post3,<0.2.0)
-Requires-Dist: nonebot-plugin-clovers[nonebot] (>=0.1.2.post3,<0.2.0)
+Requires-Dist: nonebot-plugin-clovers[nonebot] (>=0.1.4,<0.2.0)
 Description-Content-Type: text/markdown
 
 <div align="center">
 
 <a href="https://v2.nonebot.dev/store">
   <img src="https://raw.githubusercontent.com/A-kirami/nonebot-plugin-template/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo">
 </a>
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-groupmate-waifu Version: 1.4.0.post1
+Metadata-Version: 2.1 Name: nonebot-plugin-groupmate-waifu Version: 1.4.1
 Summary: Author: KarisAya Author-email: 1048827424@qq.com Requires-Python:
 >=3.10,<4.0 Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
-Python :: 3.11 Requires-Dist: clovers (>=0.1.4,<0.2.0) Requires-Dist: clovers-
-groupmate-waifu (>=0.1.0.post3,<0.2.0) Requires-Dist: nonebot-plugin-clovers
-[nonebot] (>=0.1.2.post3,<0.2.0) Description-Content-Type: text/markdown
+Python :: 3.11 Requires-Dist: clovers-groupmate-waifu (>=0.1.0.post3,<0.2.0)
+Requires-Dist: nonebot-plugin-clovers[nonebot] (>=0.1.4,<0.2.0) Description-
+Content-Type: text/markdown
                               _[_N_o_n_e_B_o_t_P_l_u_g_i_n_L_o_g_o_]
                               [NoneBotPluginText]
     # nonebot-plugin-groupmate-waifu å¨¶ç¾¤å[python]_[_l_i_c_e_n_s_e_]_[_p_y_p_i_]_[_p_y_p_i
                                    _d_o_w_n_l_o_a_d_]
 ## ð¿ å®è£ ä»¥ä¸æå°çæ¹æ³ ä»»é**å¶ä¸** å³å¯ [æ¨è] ä½¿ç¨
 nb-cli å®è£ å¨ nonebot2 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡,
 è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ ```bash nb plugin install
```


# Comparing `tmp/nonebot-plugin-hx-yinying-1.0.5.tar.gz` & `tmp/nonebot-plugin-hx-yinying-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-hx-yinying-1.0.5.tar", last modified: Wed Apr 24 16:29:01 2024, max compression
+gzip compressed data, was "nonebot-plugin-hx-yinying-1.0.6.tar", last modified: Thu Apr 25 16:12:09 2024, max compression
```

## Comparing `nonebot-plugin-hx-yinying-1.0.5.tar` & `nonebot-plugin-hx-yinying-1.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-24 16:29:01.298565 nonebot-plugin-hx-yinying-1.0.5/
--rw-rw-rw-   0        0        0     1098 2024-04-16 15:27:11.000000 nonebot-plugin-hx-yinying-1.0.5/LICENSE
--rw-rw-rw-   0        0        0     3487 2024-04-24 16:29:01.298565 nonebot-plugin-hx-yinying-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     3047 2024-04-24 16:28:33.000000 nonebot-plugin-hx-yinying-1.0.5/README.md
-drwxrwxrwx   0        0        0        0 2024-04-24 16:29:01.165185 nonebot-plugin-hx-yinying-1.0.5/nonebot_plugin_hx_yinying/
--rw-rw-rw-   0        0        0    43992 2024-04-24 16:03:12.000000 nonebot-plugin-hx-yinying-1.0.5/nonebot_plugin_hx_yinying/__init__.py
--rw-rw-rw-   0        0        0    55886 2024-04-24 16:27:18.000000 nonebot-plugin-hx-yinying-1.0.5/nonebot_plugin_hx_yinying/chat.py
--rw-rw-rw-   0        0        0      396 2024-04-24 16:19:18.000000 nonebot-plugin-hx-yinying-1.0.5/nonebot_plugin_hx_yinying/config.py
-drwxrwxrwx   0        0        0        0 2024-04-24 16:29:01.293431 nonebot-plugin-hx-yinying-1.0.5/nonebot_plugin_hx_yinying.egg-info/
--rw-rw-rw-   0        0        0     3487 2024-04-24 16:29:00.000000 nonebot-plugin-hx-yinying-1.0.5/nonebot_plugin_hx_yinying.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      388 2024-04-24 16:29:00.000000 nonebot-plugin-hx-yinying-1.0.5/nonebot_plugin_hx_yinying.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-24 16:29:00.000000 nonebot-plugin-hx-yinying-1.0.5/nonebot_plugin_hx_yinying.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      141 2024-04-24 16:29:00.000000 nonebot-plugin-hx-yinying-1.0.5/nonebot_plugin_hx_yinying.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2024-04-24 16:29:00.000000 nonebot-plugin-hx-yinying-1.0.5/nonebot_plugin_hx_yinying.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       85 2024-04-24 16:29:01.312319 nonebot-plugin-hx-yinying-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0      859 2024-04-24 16:28:55.000000 nonebot-plugin-hx-yinying-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-25 16:12:09.526256 nonebot-plugin-hx-yinying-1.0.6/
+-rw-rw-rw-   0        0        0     1098 2024-04-16 15:27:11.000000 nonebot-plugin-hx-yinying-1.0.6/LICENSE
+-rw-rw-rw-   0        0        0     5087 2024-04-25 16:12:09.526256 nonebot-plugin-hx-yinying-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     4647 2024-04-25 16:11:37.000000 nonebot-plugin-hx-yinying-1.0.6/README.md
+drwxrwxrwx   0        0        0        0 2024-04-25 16:12:09.262818 nonebot-plugin-hx-yinying-1.0.6/nonebot_plugin_hx_yinying/
+-rw-rw-rw-   0        0        0    61842 2024-04-25 15:58:39.000000 nonebot-plugin-hx-yinying-1.0.6/nonebot_plugin_hx_yinying/__init__.py
+-rw-rw-rw-   0        0        0    84465 2024-04-25 16:10:17.000000 nonebot-plugin-hx-yinying-1.0.6/nonebot_plugin_hx_yinying/chat.py
+-rw-rw-rw-   0        0        0      396 2024-04-25 14:22:54.000000 nonebot-plugin-hx-yinying-1.0.6/nonebot_plugin_hx_yinying/config.py
+drwxrwxrwx   0        0        0        0 2024-04-25 16:12:09.526256 nonebot-plugin-hx-yinying-1.0.6/nonebot_plugin_hx_yinying.egg-info/
+-rw-rw-rw-   0        0        0     5087 2024-04-25 16:12:08.000000 nonebot-plugin-hx-yinying-1.0.6/nonebot_plugin_hx_yinying.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      388 2024-04-25 16:12:08.000000 nonebot-plugin-hx-yinying-1.0.6/nonebot_plugin_hx_yinying.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 16:12:08.000000 nonebot-plugin-hx-yinying-1.0.6/nonebot_plugin_hx_yinying.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      141 2024-04-25 16:12:08.000000 nonebot-plugin-hx-yinying-1.0.6/nonebot_plugin_hx_yinying.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2024-04-25 16:12:08.000000 nonebot-plugin-hx-yinying-1.0.6/nonebot_plugin_hx_yinying.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       85 2024-04-25 16:12:09.553215 nonebot-plugin-hx-yinying-1.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      859 2024-04-25 16:11:47.000000 nonebot-plugin-hx-yinying-1.0.6/setup.py
```

### Comparing `nonebot-plugin-hx-yinying-1.0.5/LICENSE` & `nonebot-plugin-hx-yinying-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-hx-yinying-1.0.5/PKG-INFO` & `nonebot-plugin-hx-yinying-1.0.6/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-hx-yinying
-Version: 1.0.5
+Version: 1.0.6
 Summary: chat with yinying
 Home-page: https://github.com/huanxin996/nonebot_plugin_hx-yinying
 Author: Huan Xin
 Author-email: mc.xiaolang@foxmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -15,15 +15,15 @@
 <!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
 [![All Contributors](https://img.shields.io/badge/all_contributors-2-orange.svg?style=flat-square)](#contributors-)
 <!-- ALL-CONTRIBUTORS-BADGE:END -->
 
  * @Author         : huanxin996
  * @Date           : 2024-4-17
  * @LastEditors    : huanxin996
- * @LastEditTime   : 2024-4-22
+ * @LastEditTime   : 2024-4-26
  * @Description    : None
  * @GitHub         : https://github.com/huanxin996
 -->
 
 <!-- markdownlint-disable MD033 MD036 MD041 -->
 
 <p align="center">
@@ -66,26 +66,96 @@
 - @Bot 或者回复即可
 
 OneBot:
 
 - @Bot
 - 回复Bot
 
+
+<details>
+  <summary><b style="font-size: 1.5rem">指令集</b></summary>
+
+/hx
+- 别名：chat
+- 主要对话命令
+
+/刷新对话
+- 别名：clear
+- 主动刷新对话
+
+/导出对话
+- 别名：getchat
+- 导出对话记录，没有对话记录会出错。
+
+/设置全局配置
+- 别名：设置配置全局，globalset
+- 设置bot的全局配置
+
+/导出全局配置
+- 别名：getset_global
+- 导出bot的全局配置
+- 该命令包含在"设置全局配置"里
+
+/模型列表
+- 别名：modellist，chat模型列表
+- 发送bot可用模型
+
+/切换模型 [模型id]
+- 别名：qhmodel，切换chat模型，模型切换
+- 切换bot当前使用的模型
+- 私聊群聊动态响应，如果在群内输入则切换群内加载的模型，私聊输入则切换私聊的。
+
+/easycyber
+- 别名：easycyber设置，hxworld
+- 模型easycyberfurry主要配置
+- 内有多个指令
+
+/控制台操作
+- 别名：管理控制台，setstart
+- 模型easycyberfurry的角色投稿管理，即将更新cyber的角色投稿管理
+- 内有多个指令
+
+/确认版本
+- 别名：旅行伙伴确认，版本确认
+- 确认bot当前使用的版本和当前加载的模型。区分群聊和私聊动态响应
+
+/sd [名称] [设定]
+- 别名：旅行伙伴加入，设定加入
+- [名称]可为空，即发送 旅行伙伴加入 [设定]
+- [设定]不可为空，必填
+- 载入用户的设定信息和自定义昵称
+
+
+
+
+
+
+
+
+
+
+
+
+</details>
+<br>
+
 ## 配置项
 
 > [!WARNING]
 > GitHub 仓库中的文档为最新 DEV 版本，配置方式请参考 [PyPI](https://pypi.python.org/pypi/nonebot-plugin-hx-yinying) 上的文档。
 
 > [!WARNING]
 > 秩乱(乱乱)的联系方式如下，QQ:1660466270，官方qq群聊:175334224 [官网链接](https://chat.wingmark.cn/) .
 
 > [!WARNING]
 > 请注意，该项目是接入了乱乱的项目，你需要遵守api使用的 [规范](https://wingmark.feishu.cn/docx/NFgJddgQAotygKxXiu6cpyg5nqr)。
 
 配置方式：直接在 NoneBot 全局配置文件中添加以下配置项即可。
+<details>
+  <summary><b style="font-size: 1.5rem">配置项列表</b></summary>
 
 ### yinying_appid
 
 - 类型：`str`
 - 默认值：`None`
 - 说明：你的appid
 - 重要：必填
@@ -105,14 +175,17 @@
 
 ### SUPERUSERS
 - 类型：`list`
 - 默认值：`None`
 - 说明：这里是超级管理员（插件）
 - 重要：必填（你需要这个来管理该插件）
 
+</details>
+<br>
+
 配置文件示例（默认模板）
 
 ```dotenv
 yinying_appid=你的appid
 yinying_token=你的token(不带bearer)
 hx_path=C:\Users\user\Desktop
 ```
```

#### html2text {}

```diff
@@ -1,35 +1,55 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-hx-yinying Version: 1.0.5 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-hx-yinying Version: 1.0.6 Summary:
 chat with yinying Home-page: https://github.com/huanxin996/nonebot_plugin_hx-
 yinying Author: Huan Xin Author-email: mc.xiaolang@foxmail.com Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Description-Content-
 Type: text/markdown License-File: LICENSE [![All Contributors](https://
 img.shields.io/badge/all_contributors-2-orange.svg?style=flat-square)]
 (#contributors-) * @Author : huanxin996 * @Date : 2024-4-17 * @LastEditors :
-huanxin996 * @LastEditTime : 2024-4-22 * @Description : None * @GitHub : https:
+huanxin996 * @LastEditTime : 2024-4-26 * @Description : None * @GitHub : https:
 //github.com/huanxin996 -->
                                    _[_n_o_n_e_b_o_t_]
                 # nonebot_plugin_hx-yinying _â¨ Hx vs YinYing
                   (å¨çº¿ä¸é¶å½±è¿è¡å¯¹è¯çæä»¶) â¨_
                             _[_l_i_c_e_n_s_e_]_[_p_y_p_i_][python]
 ## å®è£ pipå®è£ ```dotenv pip install nonebot-plugin-hx-yinying ``` nb
 pluginå®è£ ```dotenv nb plugin install nonebot-plugin-hx-yinying ``` ##
-ä½¿ç¨æ¹å¼ éç¨: - @Bot æèåå¤å³å¯ OneBot: - @Bot - åå¤Bot ##
-éç½®é¡¹ > [!WARNING] > GitHub ä»åºä¸­çææ¡£ä¸ºææ° DEV
+ä½¿ç¨æ¹å¼ éç¨: - @Bot æèåå¤å³å¯ OneBot: - @Bot - åå¤Bot
+?æ???ä?»?¤?é?? /hx - å«åï¼chat - ä¸»è¦å¯¹è¯å½ä»¤ /å·æ°å¯¹è¯ -
+å«åï¼clear - ä¸»å¨å·æ°å¯¹è¯ /å¯¼åºå¯¹è¯ - å«åï¼getchat -
+å¯¼åºå¯¹è¯è®°å½ï¼æ²¡æå¯¹è¯è®°å½ä¼åºéã /è®¾ç½®å¨å±éç½® -
+å«åï¼è®¾ç½®éç½®å¨å±ï¼globalset - è®¾ç½®botçå¨å±éç½® /
+å¯¼åºå¨å±éç½® - å«åï¼getset_global - å¯¼åºbotçå¨å±éç½® -
+è¯¥å½ä»¤åå«å¨"è®¾ç½®å¨å±éç½®"é /æ¨¡ååè¡¨ -
+å«åï¼modellistï¼chatæ¨¡ååè¡¨ - åébotå¯ç¨æ¨¡å /åæ¢æ¨¡å
+[æ¨¡åid] - å«åï¼qhmodelï¼åæ¢chatæ¨¡åï¼æ¨¡ååæ¢ -
+åæ¢botå½åä½¿ç¨çæ¨¡å -
+ç§èç¾¤èå¨æååºï¼å¦æå¨ç¾¤åè¾å¥ååæ¢ç¾¤åå è½½çæ¨¡åï¼ç§èè¾å¥ååæ¢ç§èçã
+/easycyber - å«åï¼easycyberè®¾ç½®ï¼hxworld -
+æ¨¡åeasycyberfurryä¸»è¦éç½® - åæå¤ä¸ªæä»¤ /æ§å¶å°æä½ -
+å«åï¼ç®¡çæ§å¶å°ï¼setstart -
+æ¨¡åeasycyberfurryçè§è²æç¨¿ç®¡çï¼å³å°æ´æ°cyberçè§è²æç¨¿ç®¡ç
+- åæå¤ä¸ªæä»¤ /ç¡®è®¤çæ¬ - å«åï¼æè¡ä¼ä¼´ç¡®è®¤ï¼çæ¬ç¡®è®¤
+-
+ç¡®è®¤botå½åä½¿ç¨ççæ¬åå½åå è½½çæ¨¡åãåºåç¾¤èåç§èå¨æååº
+/sd [åç§°] [è®¾å®] - å«åï¼æè¡ä¼ä¼´å å¥ï¼è®¾å®å å¥ -
+[åç§°]å¯ä¸ºç©ºï¼å³åé æè¡ä¼ä¼´å å¥ [è®¾å®] -
+[è®¾å®]ä¸å¯ä¸ºç©ºï¼å¿å¡« - è½½å¥ç¨æ·çè®¾å®ä¿¡æ¯åèªå®ä¹æµç§°
+## éç½®é¡¹ > [!WARNING] > GitHub ä»åºä¸­çææ¡£ä¸ºææ° DEV
 çæ¬ï¼éç½®æ¹å¼è¯·åè [PyPI](https://pypi.python.org/pypi/nonebot-
 plugin-hx-yinying) ä¸çææ¡£ã > [!WARNING] > ç§©ä¹±
 (ä¹±ä¹±)çèç³»æ¹å¼å¦ä¸ï¼QQ:1660466270ï¼å®æ¹qqç¾¤è:175334224
 [å®ç½é¾æ¥](https://chat.wingmark.cn/) . > [!WARNING] >
 è¯·æ³¨æï¼è¯¥é¡¹ç®æ¯æ¥å¥äºä¹±ä¹±çé¡¹ç®ï¼ä½ éè¦éµå®apiä½¿ç¨ç
 [è§è](https://wingmark.feishu.cn/docx/NFgJddgQAotygKxXiu6cpyg5nqr)ã
 éç½®æ¹å¼ï¼ç´æ¥å¨ NoneBot
-å¨å±éç½®æä»¶ä¸­æ·»å ä»¥ä¸éç½®é¡¹å³å¯ã ### yinying_appid -
-ç±»åï¼`str` - é»è®¤å¼ï¼`None` - è¯´æï¼ä½ çappid - éè¦ï¼å¿å¡«
-### yinying_token - ç±»åï¼`str` - é»è®¤å¼ï¼`None` -
+å¨å±éç½®æä»¶ä¸­æ·»å ä»¥ä¸éç½®é¡¹å³å¯ã ?é???ç?½?®?é?¡?¹?å???è?¡?¨ ###
+yinying_appid - ç±»åï¼`str` - é»è®¤å¼ï¼`None` - è¯´æï¼ä½ çappid -
+éè¦ï¼å¿å¡« ### yinying_token - ç±»åï¼`str` - é»è®¤å¼ï¼`None` -
 è¯´æï¼è¿éåä½ æ¾ç§©ä¹±è·åå°çapi_key - éè¦ï¼å¿å¡« ### hx_path
 - ç±»åï¼`str` - é»è®¤å¼ï¼`None` -
 è¯´æï¼è¿éæ¯æä»¶æ¬å°éç½®çå­å¨ç®å½ - éè¦ï¼éå¿å¡« ###
 SUPERUSERS - ç±»åï¼`list` - é»è®¤å¼ï¼`None` -
 è¯´æï¼è¿éæ¯è¶çº§ç®¡çåï¼æä»¶ï¼ -
 éè¦ï¼å¿å¡«ï¼ä½ éè¦è¿ä¸ªæ¥ç®¡çè¯¥æä»¶ï¼
 éç½®æä»¶ç¤ºä¾ï¼é»è®¤æ¨¡æ¿ï¼ ```dotenv yinying_appid=ä½ çappid
```

### Comparing `nonebot-plugin-hx-yinying-1.0.5/nonebot_plugin_hx_yinying/__init__.py` & `nonebot-plugin-hx-yinying-1.0.6/nonebot_plugin_hx_yinying/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,49 +1,27 @@
 from nonebot.plugin import PluginMetadata
 from .config import Config
-from nonebot import on_command, on_message ,get_plugin_config
+from nonebot import on_command, on_message ,get_plugin_config,require
+require("nonebot_plugin_apscheduler")
+from nonebot_plugin_apscheduler import scheduler
 from nonebot.params import CommandArg
 from nonebot.adapters.onebot.v11 import (
     Bot,
     GroupMessageEvent,
     MessageEvent,
     Message,
     Event,
 )
 from html import unescape
 from nonebot.typing import T_State
 from nonebot.log import logger
 from nonebot.matcher import Matcher
 from nonebot.rule import to_me
-import json,os
-from .chat import (
-    get_id,
-    get_answer_at,
-    get_answer_ml,
-    get_nick,
-    send_msg,
-    clear_id,
-    get_history,
-    config_in_group,
-    config_in_user,
-    config_in_global,
-    model_got,
-    get_groupid,
-    json_get,
-    path_in,
-    update_hx,
-    get_config_global,
-    send_msg_reject,
-    easycyber_in,
-    json_replace,
-    json_get_text,
-    easycyber_in_tg,
-    place,
-    config_list,
-)
+import json,os,random
+from .chat import *
 
 __plugin_meta__ = PluginMetadata(
     name="Hx_YinYing",
     description="快来和可爱的赛博狼狼聊天！",
     usage=(
         "通过QQ艾特机器人来进行对话"
     ),
@@ -51,54 +29,79 @@
     homepage="https://github.com/huanxin996/nonebot_plugin_hx-yinying",
     config=Config,
     supported_adapters={
         "~onebot.v11"
     },
 )
 
-
 hx_config = get_plugin_config(Config)
+global_config = config_in_global()
+dy_list = json_get(config_in_global(),"dy_list")
 log_dir = path_in()
    
+#检查更新
 new_verision, time = update_hx()
-if new_verision <= hx_config.hx_version:
-    logger.success(f"[Hx_YinYing]:你的Hx_YinYing已经是最新版本了！当前版本为{hx_config.hx_version}")
+
+if not new_verision and not time:
+    logger.error(f"[Hx_YinYing]:无法获取最新的版本，当前版本为{hx_config.hx_version}，可能已经过时！")
 else:
-    logger.success("[Hx_YinYing]:检查到Hx_YinYing有新版本！")
-    logger.warning("【Hx】正在自动更新中")
-    os.system(f'pip install nonebot-plugin-hx-yinying=={new_verision} -i https://pypi.Python.org/simple/')
-    logger.success(f"[Hx_YinYing]:更新完成！最新版本为{new_verision}|当前使用版本为{hx_config.hx_version}")
-    logger.warning(f"[Hx_YinYing]:你可能需要重新启动nonebot来完成插件的重载")
+    if new_verision <= hx_config.hx_version:
+        logger.success(f"[Hx_YinYing]:你的Hx_YinYing已经是最新版本了！当前版本为{hx_config.hx_version}")
+    else:
+        if os.path.exists(f"{log_dir}\config\config_glob21.json"):
+            logger.success("121")
+        else:
+            logger.success("[Hx_YinYing]:检查到Hx_YinYing有新版本！")
+            logger.warning("【Hx】正在自动更新中--未找到虚拟环境【安装在本地环境！】")
+            os.system(f'pip install nonebot-plugin-hx-yinying=={new_verision} -i https://pypi.Python.org/simple/')
+            logger.success(f"[Hx_YinYing]:更新完成！最新版本为{new_verision}|当前使用版本为{hx_config.hx_version}")
+            logger.warning(f"[Hx_YinYing]:你可能需要重新启动nonebot来完成插件的重载")
 
+#检查关键配置
 if hx_config.yinying_appid == None or hx_config.yinying_token == None:
     logger.opt(colors=True).error("未设置核心配置？！,请检查你配置里的yinying_appid和yinying_token")
 else:
     logger.opt(colors=True).success("【Hx】加载核心配置成功")
 
-
+#根据订阅信息注册定身任务
+try:
+    extent = int(len(dy_list))
+    for key in dy_list:
+        config_1 = config_in_user(key,False)
+        user_config = json_get(config_1,key)
+        config_time = json_get_time(user_config,"dy_time")
+        config_minute = json_get_time(user_config,"dy_minute")
+        scheduler.add_job(func=get_chat,trigger='interval',args=[key] ,hours=config_time, minutes=config_minute, id=key)
+    logger.opt(colors=True).success(f"【Hx】定时任务加载成功,当前共加载{extent}个订阅用户")
+except Exception as e:
+    logger.opt(colors=True).error(f"【Hx】:错误捕获{e}，联系开发者！")
+    logger.opt(colors=True).error("【Hx】定时任务加载失败！！，联系开发者！")
 
 msg_at = on_message(rule=to_me(), priority=10, block=True)
 msg_ml = on_command("hx", aliases={"chat"}, priority=10, block=True)
 clear =  on_command("刷新对话", aliases={"clear"}, priority=0, block=True)
 history_get = on_command("导出对话", aliases={"getchat"}, priority=0, block=True)
 set_global_config = on_command("设置全局配置", aliases={"设置配置全局","globalset"}, priority=0, block=True)
 set_get_global = on_command("导出全局设置", aliases={"getset_global"}, priority=0, block=True)
 model_list = on_command("模型列表", aliases={"modellist","chat模型列表"}, priority=0, block=True)
-model_handoff = on_command("切换模型", aliases={"qhmodel","切换chat模型"}, priority=0, block=True)
+model_handoff = on_command("切换模型", aliases={"qhmodel","切换chat模型","模型切换"}, priority=0, block=True)
 rule_reply = on_command("对话回复", aliases={"chat回复"}, priority=0, block=True)
 rule_reply_at = on_command("回复艾特", aliases={"chat回复艾特"}, priority=0, block=True)
 private = on_command("私聊回复", aliases={"私聊chat"}, priority=0, block=True)
 at_reply = on_command("艾特回复", aliases={"bot艾特回复"}, priority=0, block=True)
 easycyber_set = on_command("easycyber", aliases={"easycyber设置","hxworld"}, priority=0, block=True)
+cyber_set = on_command("cyber", aliases={"cyber设置","Hxworld"}, priority=0, block=True)
 admin_set = on_command("控制台操作", aliases={"管理控制台","setstart"}, priority=0, block=True)
 verision = on_command("确认版本", aliases={"旅行伙伴确认","版本确认"}, priority=0, block=True)
 character = on_command("sd", aliases={"旅行伙伴加入","设定加入"}, priority=0, block=True)
+chat_ne = on_command("加入订阅", aliases={"旅行伙伴觉醒","订阅加入"}, priority=0, block=True)
+ces = on_command("ces", aliases={"测试"}, priority=0, block=True)
 
 @character.handle()
-async def verision_get(matcher: Matcher,bot:Bot, event: MessageEvent, events:Event, msg: Message = CommandArg()):
+async def character(matcher: Matcher,bot:Bot, event: MessageEvent, events:Event, msg: Message = CommandArg()):
     user = get_id(event)
     nick = await get_nick(bot,event)
     config = config_in_user(user,nick)
     config_get = json_get(config,user)
     text = msg.extract_plain_text()
     if text == "" or text == None:
         msg = "没有获取到要加入伙伴的设定哦"
@@ -106,69 +109,93 @@
     else:
         try:
             msg = text.split(" ")
             if int(len(msg)) == 1:
                 config_get["nick"] = nick
                 config_get["character"] = text
                 config[f"{user}"] = config_get
-                with open(f'{log_dir}/config/config_user.json','w',encoding='utf-8') as file:
+                with open(f'{log_dir}\config\config_user.json','w',encoding='utf-8') as file:
                     json.dump(config,file)
                     msg = f"{nick}加入成功"
             elif int(len(msg)) == 2:
                 config_get["nick"] = msg[1]
                 config_get["character"] = msg[0]
                 config[f"{user}"] = config_get
-                with open(f'{log_dir}/config/config_user.json','w',encoding='utf-8') as file:
+                with open(f'{log_dir}\config\config_user.json','w',encoding='utf-8') as file:
                     json.dump(config,file)
                     msg = f"{msg[0]}加入成功！"
             else:
                 msg = "没有获取到要加入伙伴的设定哦"
             await send_msg(matcher, event, msg)
         except Exception as e:
             msg = False
             logger.opt(colors=True).error(f"{e}")
         
 @verision.handle()
 async def verision_get(matcher: Matcher, event: MessageEvent, events:Event):
     new_verision, time = update_hx()
     if isinstance(events, GroupMessageEvent):
-        config = json_get(config_in_group(get_groupid(event)),get_groupid(event))
+        id = get_groupid(event)
+        e_config = config_in_group(id)
+        config = json_get(e_config,id)
         model = json_get(config,"use_model")
-        if new_verision > hx_config.hx_version:
+        if not new_verision and not hx_config.hx_version:
             if model == "easycyberfurry-001":
                 model_in = json_get(config,"easycharacter_in")
-                if model_in or not model_in:
+                if model_in:
+                    msg =f"(歪头)\n======================\n当前版本号:v{hx_config.hx_version}[？？？]\n你的插件版本可能已过时，当前无法获取最新版本\n当前群聊使用模型:{model}\n当前模型载入角色:Hx\n最后更新时间:====>\n{time}\n======================"
+                msg = f"(歪头)\n======================\n当前版本号:v{hx_config.hx_version}[？？？]\n你的插件版本可能已过时，当前无法获取最新版本\n当前群聊使用模型:{model}\n当前模型载入角色:{model_in}\n最后更新时间:====>\n{time}\n======================"
+            else:
+                msg = f"(歪头)\n======================\n当前版本号:v{hx_config.hx_version}[？？？]\n你的插件版本可能已过时，当前无法获取最新版本\n当前群聊使用模型:{model}\n最后更新时间:====>\n{time}\n======================"
+        elif new_verision > hx_config.hx_version:
+            if model == "easycyberfurry-001":
+                model_in = json_get(config,"easycharacter_in")
+                if not model_in or model_in == None:
                     msg =f"(歪头)\n======================\n当前版本号:v{hx_config.hx_version}[已过时(]\n你的插件版本已过时，当前最新版本为v{new_verision}\n当前群聊使用模型:{model}\n当前模型载入角色:Hx\n最后更新时间:====>\n{time}\n======================"
-                msg = f"(歪头)\n======================\n当前版本号:v{hx_config.hx_version}[已过时(]\n你的插件版本已过时，当前最新版本为v{new_verision}\n当前群聊使用模型:{model}\n当前模型载入角色:{model_in}\n最后更新时间:====>\n{time}\n======================"
-            msg = f"(歪头)\n======================\n当前版本号:v{hx_config.hx_version}[已过时(]\n你的插件版本已过时，当前最新版本为v{new_verision}\n当前群聊使用模型:{model}\n最后更新时间:====>\n{time}\n======================"
+                else:
+                    msg = f"(歪头)\n======================\n当前版本号:v{hx_config.hx_version}[已过时(]\n你的插件版本已过时，当前最新版本为v{new_verision}\n当前群聊使用模型:{model}\n当前模型载入角色:{model_in}\n最后更新时间:====>\n{time}\n======================"
+            else:
+                msg = f"(歪头)\n======================\n当前版本号:v{hx_config.hx_version}[已过时(]\n你的插件版本已过时，当前最新版本为v{new_verision}\n当前群聊使用模型:{model}\n最后更新时间:====>\n{time}\n======================"
         else:
             if model == "easycyberfurry-001":
                 model_in = json_get(config,"easycharacter_in")
-                if model_in or not model_in:
-                    msg =f"(歪头)\n======================\n当前版本号:v{hx_config.hx_version}[最新！]\n当前群聊使用模型:{model}\n当前模型载入角色:Hx\n最后更新时间:====>\n{time}\n======================"
-                msg = f"(歪头)\n======================\n当前版本号:v{hx_config.hx_version}[最新！]\n当前群聊使用模型:{model}\n当前模型载入角色:{model_in}\n最后更新时间:====>\n{time}\n======================"
-            msg = f"(点头)\n======================\n当前版本号:v{hx_config.hx_version}[最新！]\n当前群聊使用模型:\n最后更新时间:====>\n{time}\n======================"
+                if  not model_in or model_in == None:
+                    msg =f"(点头)\n======================\n当前版本号:v{hx_config.hx_version}[最新！]\n当前群聊使用模型:{model}\n当前模型载入角色:Hx\n最后更新时间:====>\n{time}\n======================"
+                else:
+                    msg = f"(点头)\n======================\n当前版本号:v{hx_config.hx_version}[最新！]\n当前群聊使用模型:{model}\n当前模型载入角色:{model_in}\n最后更新时间:====>\n{time}\n======================"
+            else:
+                msg = f"(点头)\n======================\n当前版本号:v{hx_config.hx_version}[最新！]\n当前群聊使用模型:{model}\n最后更新时间:====>\n{time}\n======================"
         await send_msg(matcher, event, msg)
     else:
         config = json_get(config_in_user(get_id(event),False),get_id(event))
         model = json_get(config,"private_model")
-        if new_verision > hx_config.hx_version:
+        if not new_verision and not hx_config.hx_version:
+            if model == "easycyberfurry-001":
+                model_in = json_get(config,"easycharacter_in")
+                if model_in:
+                    msg =f"(歪头)\n======================\n当前版本号:v{hx_config.hx_version}[？？？]\n你的插件版本可能已过时，当前无法获取最新版本\n当前私聊使用模型:{model}\n当前模型载入角色:Hx\n最后更新时间:====>\n{time}\n======================"
+                msg = f"(歪头)\n======================\n当前版本号:v{hx_config.hx_version}[？？？]\n你的插件版本可能已过时，当前无法获取最新版本\n当前私聊使用模型:{model}\n当前模型载入角色:{model_in}\n最后更新时间:====>\n{time}\n======================"
+            else:
+                msg = f"(歪头)\n======================\n当前版本号:v{hx_config.hx_version}[？？？]\n你的插件版本可能已过时，当前无法获取最新版本\n当前私聊使用模型:{model}\n最后更新时间:====>\n{time}\n======================"
+        elif new_verision > hx_config.hx_version:
             if model == "easycyberfurry-001":
                 model_in = json_get(config,"easycharacter_in")
-                if model_in or not model_in:
+                if model_in:
                     msg =f"(歪头)\n======================\n当前版本号:v{hx_config.hx_version}[已过时(]\n你的插件版本已过时，当前最新版本为v{new_verision}\n当前私聊使用模型:{model}\n当前模型载入角色:Hx\n最后更新时间:====>\n{time}\n======================"
                 msg = f"(歪头)\n======================\n当前版本号:v{hx_config.hx_version}[已过时(]\n你的插件版本已过时，当前最新版本为v{new_verision}\n当前私聊使用模型:{model}\n当前模型载入角色:{model_in}\n最后更新时间:====>\n{time}\n======================"
-            msg = f"(歪头)\n======================\n当前版本号:v{hx_config.hx_version}[已过时(]\n你的插件版本已过时，当前最新版本为v{new_verision}\n当前私聊使用模型:{model}\n最后更新时间:====>\n{time}\n======================"
+            else:
+                msg = f"(歪头)\n======================\n当前版本号:v{hx_config.hx_version}[已过时(]\n你的插件版本已过时，当前最新版本为v{new_verision}\n当前私聊使用模型:{model}\n最后更新时间:====>\n{time}\n======================"
         else:
             if model == "easycyberfurry-001":
                 model_in = json_get(config,"easycharacter_in")
-                if model_in or not model_in:
-                    msg =f"(歪头)\n======================\n当前版本号:v{hx_config.hx_version}[最新！]\n当前私聊使用模型:{model}\n当前模型载入角色:Hx\n最后更新时间:====>\n{time}\n======================"
-                msg = f"(歪头)\n======================\n当前版本号:v{hx_config.hx_version}[最新！]\n当前私聊使用模型:{model}\n当前模型载入角色:{model_in}\n最后更新时间:====>\n{time}\n======================"
-            msg = f"(点头)\n======================\n当前版本号:v{hx_config.hx_version}[最新！]\n当前私聊使用模型:\n最后更新时间:====>\n{time}\n======================"
+                if model_in:
+                    msg =f"(点头)\n======================\n当前版本号:v{hx_config.hx_version}[最新！]\n当前私聊使用模型:{model}\n当前模型载入角色:Hx\n最后更新时间:====>\n{time}\n======================"
+                msg = f"(点头)\n======================\n当前版本号:v{hx_config.hx_version}[最新！]\n当前私聊使用模型:{model}\n当前模型载入角色:{model_in}\n最后更新时间:====>\n{time}\n======================"
+            else:
+                msg = f"(点头)\n======================\n当前版本号:v{hx_config.hx_version}[最新！]\n当前私聊使用模型:{model}\n最后更新时间:====>\n{time}\n======================"
         await send_msg(matcher, event, msg)
 
 @msg_at.handle()
 async def at(matcher: Matcher, event: MessageEvent, bot: Bot, events:Event):
     config_global = config_in_global()
     at_reply = json_get(config_global,"at_reply")
     if not at_reply:
@@ -222,15 +249,15 @@
             config = config_in_global()
             get_config = json_get_text(config,text)
             if get_config == 0:
                 s["last"] = True
                 msg = "无法查找到该配置项！，请检查其是否为正确的配置名"
                 await send_msg(matcher,event,msg)
             else:
-                TFkey, Wkey, Listkey, app_key = config_list(config)
+                TFkey, Wkey, Listkey = config_list(config)
                 if text in TFkey:
                     s["last"] = "修改TF"
                     s["set"] = text
                     msg = "请发送开启或关闭【也可以是on或者off或者开和关】"
                     await send_msg_reject(matcher,event,msg)
                 elif text in Wkey:
                     s["last"] = "修改w"
@@ -255,33 +282,33 @@
                 text = False
                 if get_config and text:
                     msg = f"该配置项[{config_name}]已经开启了，不需要重复开启噢"
                 elif not get_config and not text:
                     msg = f"该配置项[{config_name}]已经关闭了，不需要重复关闭噢"
                 elif text:
                     config[f"{config_name}"] = True
-                    with open(f'{log_dir}/config/config_global.json','w',encoding='utf-8') as file:
+                    with open(f'{log_dir}\config\config_global.json','w',encoding='utf-8') as file:
                         json.dump(config,file)
                     msg = f"{config_name}的状态已更改为{text}"
                 elif not text:
                     config[f"{config_name}"] = False
-                    with open(f'{log_dir}/config/config_global.json','w',encoding='utf-8') as file:
+                    with open(f'{log_dir}\config\config_global.json','w',encoding='utf-8') as file:
                         json.dump(config,file)
                     msg = f"{config_name}的状态已更改为{text}"
             s["last"] = True
             if text == "退出":
                 msg = "已退出"
             await send_msg(matcher,event,msg)        
         
         if s["last"] == "修改w":
             config = config_in_global()
             config_name = s["set"]
             get_config = json_get_text(config,config_name)
             config[f"{config_name}"] = text
-            with open(f'{log_dir}/config/config_global.json','w',encoding='utf-8') as file:
+            with open(f'{log_dir}\config\config_global.json','w',encoding='utf-8') as file:
                 json.dump(config,file)
             msg = f"{config_name}的id已更改为{text}"
             s["last"] = True
             await send_msg(matcher,event,msg)
 
         if s["last"] == "updata_LK":
             s["type"] = text
@@ -304,24 +331,24 @@
             config_get = json_get(config,config_name)
             if config_set_type == "增加" or config_set_type == "添加":
                 if text in config_get:
                     msg = "该id已经在这个配置项里了，不可以重复添加哦"
                 else:
                     config_get.append(text)
                     config["config_name"] = config_get
-                    with open(f'{log_dir}/config/config_global.json','w',encoding='utf-8') as file:
+                    with open(f'{log_dir}\config\config_global.json','w',encoding='utf-8') as file:
                         json.dump(config,file)
                         msg = "该id已添加在这个配置项里"
             elif config_set_type == "移除" or config_set_type == "删除":
                 if text not in config_get:
                     msg = "该id不在这个配置项里，无法重复删除"
                 else:
                     config_get.remove(text)
                     config["config_name"] = config_get
-                    with open(f'{log_dir}/config/config_global.json','w',encoding='utf-8') as file:
+                    with open(f'{log_dir}\config\config_global.json','w',encoding='utf-8') as file:
                         json.dump(config,file)
                         msg = "该id已在这个配置项里被移除"
             await send_msg(matcher,event,msg) 
         
         
     #查看
     if text == "查看" or text == "查看配置":
@@ -361,80 +388,84 @@
     if isinstance(events, GroupMessageEvent):
         await bot.send_group_forward_msg(group_id=event.group_id, messages=msg_list)  # type: ignore
     elif json_get(config_in_global(),"private"):
         await bot.send_private_forward_msg(user_id=id, messages=msg_list)  # type: ignore
 
 @model_list.handle()
 async def list(matcher: Matcher, event: MessageEvent):
-        msg = "1.yinyingllm-v1\n2.yinyingllm-v2\n3.yinyingllm-v3\n4.cyberfurry-001\n5.easycyberfurry-001\n切换模型请发送:模型切换(序号)"
+        msg = "1.yinyingllm-v1\n2.yinyingllm-v2\n3.yinyingllm-v3\n4.cyberfurry-001\n5.easycyberfurry-001\n切换模型请发送:切换模型(序号)"
         await send_msg(matcher, event, msg)
 
 @model_handoff.handle()
 async def handoff(matcher: Matcher, bot: Bot, event: MessageEvent,events: Event, msg: Message = CommandArg()):
     text = msg.extract_plain_text()
+    nick = await get_nick(bot,event)
+    id = get_id(event)
     model = model_got(text)
     if not text == "" or text == None:
         if isinstance(events, GroupMessageEvent):
             groupid = get_groupid(event)
             config_group = config_in_group(groupid)
             group_config = json_get(config_group,groupid)
             if group_config["use_model"] == model:
                 msg =f"(当前模型已经是{model}了)不需要重复切换哦"
                 await send_msg(matcher,event,msg)
             else:
                 group_config["use_model"] = model
                 config_group[f"{groupid}"] = group_config
-                with open(f'{log_dir}/config/config_group.json','w',encoding='utf-8') as file:
+                with open(f'{log_dir}\config\config_group.json','w',encoding='utf-8') as file:
                     json.dump(config_group,file)
+                    clear_id(id,nick)
                     msg =f"切换成功（当前模型已切换为{model})"
                     await send_msg(matcher,event,msg)
         else:
             id = get_id(event)
             nick = get_nick(bot,event)
             config_user = config_in_user(id,nick)
             user_config = json_get(config_user,id)
             if user_config["private_model"] == model:
                 msg =f"(当前模型已经是{model}了)不需要重复切换哦"
                 await send_msg(matcher,event,msg)
             else:
                 user_config['private_model'] = f"{model}"
                 config_user[f"{id}"] = user_config
-                with open(f'{log_dir}/config/config_user.json','w',encoding='utf-8') as file:
+                with open(f'{log_dir}\config\config_user.json','w',encoding='utf-8') as file:
                     json.dump(config_user,file)
+                    clear_id(id,nick)
                     msg =f"切换成功（当前模型已切换为{model})"
                     await send_msg(matcher,event,msg)
     else:
         msg = "请注意，切换模型后不能为空哦"
         await send_msg(matcher,event,msg)
 
 @rule_reply.handle()
-async def reply(matcher: Matcher, bot: Bot, event: MessageEvent, msg: Message = CommandArg()):
+async def reply(matcher: Matcher, event: MessageEvent, msg: Message = CommandArg()):
     text = msg.extract_plain_text()
     if not text == "" or text == None:
         if text == "开启" or text == "on" or text == "开":
             config_global = config_in_global()
             zt_reply = json_get(config_global,"reply")
             if zt_reply == True:
                 msg = "请勿重复开启对话回复哦"
                 await send_msg(matcher,event,msg)
             else:
                 config_global["reply"] = True
-                with open(f'{log_dir}/config/config_global.json','w',encoding='utf-8') as file:
+                with open(f'{log_dir}\config\config_global.json','w',encoding='utf-8') as file:
                     json.dump(config_global,file) 
                 msg = "对话回复已开启"
                 await send_msg(matcher,event,msg)
         elif text == "关闭" or text == "off" or text == "关":
             config_global = config_in_global()
             zt_reply = json_get(config_global,"reply")
             if zt_reply == False:
                 msg = "请勿重复关闭对话回复哦"
                 await send_msg(matcher,event,msg)
             else:
                 config_global["reply"] = False
-                with open(f'{log_dir}/config/config_global.json','w',encoding='utf-8') as file:
+                with open(f'{log_dir}\config\config_global.json','w',encoding='utf-8') as file:
                     json.dump(config_global,file)
                 msg = "对话回复已关闭"
                 await send_msg(matcher,event,msg)
     else:
         msg = f"请注意，正确的格式应该是\n对话回复{text}"
         await send_msg(matcher,event,msg)
 
@@ -447,27 +478,27 @@
                 config_global = config_in_global()
                 zt_reply = json_get(config_global,"reply_at")
                 if zt_reply == True:
                     msg = "请勿重复开启回复艾特哦"
                     await send_msg(matcher,event,msg)
                 else:
                     config_global["reply_at"] = True
-                    with open(f'{log_dir}/config/config_global.json','w',encoding='utf-8') as file:
+                    with open(f'{log_dir}\config\config_global.json','w',encoding='utf-8') as file:
                         json.dump(config_global,file) 
                     msg = "回复艾特已开启"
                     await send_msg(matcher,event,msg)
             elif text == "关闭" or text == "off" or text == "关":
                 config_global = config_in_global()
                 zt_reply = json_get(config_global,"reply_at")
                 if zt_reply == False:
                     msg = "请勿重复关闭对话回复哦"
                     await send_msg(matcher,event,msg)
                 else:
                     config_global["reply_at"] = False
-                    with open(f'{log_dir}/config/config_global.json','w',encoding='utf-8') as file:
+                    with open(f'{log_dir}\config\config_global.json','w',encoding='utf-8') as file:
                         json.dump(config_global,file)
                     msg = "回复艾特已关闭"
                     await send_msg(matcher,event,msg)
         else:
             msg = "在对话回复开启的状况下（,回复艾特无效"
             await send_msg(matcher,event,msg)
     else:
@@ -491,27 +522,27 @@
             config_global = config_in_global()
             zt_reply = json_get(config_global,"private")
             if zt_reply == True:
                 msg = "请勿重复开启私聊回复哦"
                 await send_msg(matcher,event,msg)
             else:
                 config_global["private"] = True
-                with open(f'{log_dir}/config/config_global.json','w',encoding='utf-8') as file:
+                with open(f'{log_dir}\config\config_global.json','w',encoding='utf-8') as file:
                     json.dump(config_global,file) 
                 msg = "私聊回复已启用"
                 await send_msg(matcher,event,msg)
         elif text == "关闭" or text == "off" or text == "关":
             config_global = config_in_global()
             zt_reply = json_get(config_global,"private")
             if zt_reply == False:
                 msg = "请勿重复关闭私聊回复哦"
                 await send_msg(matcher,event,msg)
             else:
                 config_global["private"] = False
-                with open(f'{log_dir}/config/config_global.json','w',encoding='utf-8') as file:
+                with open(f'{log_dir}\config\config_global.json','w',encoding='utf-8') as file:
                     json.dump(config_global,file)
                 msg = "私聊回复已停用"
                 await send_msg(matcher,event,msg)
     else:
         msg = f"请注意，正确的格式应该是\n私聊回复{text}"
         await send_msg(matcher,event,msg)
 
@@ -520,42 +551,42 @@
     text = msg.extract_plain_text()
     if not text == "" or text == None:
         if text == "开启" or text == "on" or text == "开":
             config_global = config_in_global()
             at_reply = json_get(config_global,"at_reply")
             if not at_reply:
                 config_global["at_reply"] = True
-                with open(f'{log_dir}/config/config_global.json','w',encoding='utf-8') as file:
+                with open(f'{log_dir}\config\config_global.json','w',encoding='utf-8') as file:
                     json.dump(config_global,file) 
                 msg = "艾特回复已启用【bot被@将会回复】"
                 await send_msg(matcher,event,msg)
             elif at_reply == True:
                 msg = "请勿重复开启艾特回复哦【bot被@已经会回复了】"
                 await send_msg(matcher,event,msg)
             else:
                 config_global["at_reply"] = True
-                with open(f'{log_dir}/config/config_global.json','w',encoding='utf-8') as file:
+                with open(f'{log_dir}\config\config_global.json','w',encoding='utf-8') as file:
                     json.dump(config_global,file) 
                 msg = "艾特回复已启用【bot被@将会回复】"
                 await send_msg(matcher,event,msg)
         elif text == "关闭" or text == "off" or text == "关":
             config_global = config_in_global()
             at_reply = json_get(config_global,"at_reply")
             if not at_reply:
                 config_global["at_reply"] = False
-                with open(f'{log_dir}/config/config_global.json','w',encoding='utf-8') as file:
+                with open(f'{log_dir}\config\config_global.json','w',encoding='utf-8') as file:
                     json.dump(config_global,file)
                 msg = "艾特回复已停用【bot被@回复已停用】"
                 await send_msg(matcher,event,msg)
             elif at_reply == False:
                 msg = "请勿重复关闭艾特回复哦【bot被@已经不会回复了】"
                 await send_msg(matcher,event,msg)
             else:
                 config_global["at_reply"] = False
-                with open(f'{log_dir}/config/config_global.json','w',encoding='utf-8') as file:
+                with open(f'{log_dir}\config\config_global.json','w',encoding='utf-8') as file:
                     json.dump(config_global,file) 
                 msg = "艾特回复已停用【bot被@回复已停用】"
                 await send_msg(matcher,event,msg)
     else:
         msg = f"请注意，正确的格式应该是\n私聊回复{text}"
         await send_msg(matcher,event,msg)
 
@@ -592,114 +623,122 @@
                 await send_msg_reject(matcher,event,msg)
 
         if s["last"] == "cfconage":
             if text == "退出":
                 s["last"] = True
                 msg = "已退出"
                 await send_msg(matcher,event,msg)
-            key = ['child','young','adult']
-            if not text in key:
-                s["last"] = True
-                msg = "未找到该类型的角色表现！已自动退出"
-                await send_msg(matcher,event,msg)
             else:
-                s["cfconage"] = text
-                s["last"] = "cfconstyle"
-                msg = "请输入角色聊天风格:(比如\n vivid--[活泼]\n sentiment--[富有情感(共情大师？)]\n assistant--[助理]\n chilly--[冷酷无情]\n social_anxiety--[社恐]\nps:只输入--前面的英文即可"
-                await send_msg_reject(matcher,event,msg)
+                key = ['child','young','adult']
+                if not text in key:
+                    s["last"] = "cfconage"
+                    msg = "未找到该类型的角色聊天年龄!请重新输入，如需退出请发送：退出"
+                    await send_msg_reject(matcher,event,msg)
+                else:
+                    s["cfconage"] = text
+                    s["last"] = "cfconstyle"
+                    msg = "请输入角色聊天风格:(比如\n vivid--[活泼]\n sentiment--[富有情感(共情大师？)]\n assistant--[助理]\n chilly--[冷酷无情]\n social_anxiety--[社恐]\nps:只输入--前面的英文即可"
+                    await send_msg_reject(matcher,event,msg)
 
         if s["last"] == "cfconstyle":
             if text == "退出":
                 s["last"] = True
                 msg = "已退出"
                 await send_msg(matcher,event,msg)
-            key = ['vivid','sentiment','assistant','chilly','social_anxiety']
-            if not text in key:
-                s["last"] = True
-                msg = "未找到该类型的角色聊天风格！已自动退出"
-                await send_msg(matcher,event,msg)
             else:
-                s["cfconstyle"] = json_replace(text)
-                s["last"] = "cfstory"
-                msg = "请输入角色的背景故事（这对他真的很重要\n[胡言乱语：我要给他完整的一生！！！]"
-                await send_msg_reject(matcher,event,msg)
+                key = ['vivid','sentiment','assistant','chilly','social_anxiety']
+                if not text in key:
+                    s["last"] = "cfconstyle"
+                    msg = "未找到该类型的角色聊天风格！请重新输入，如需退出请发送：退出"
+                    await send_msg_reject(matcher,event,msg)
+                else:
+                    s["cfconstyle"] = json_replace(text)
+                    s["last"] = "cfstory"
+                    msg = "请输入角色的背景故事（这对他真的很重要\n[胡言乱语：我要给他完整的一生！！！]"
+                    await send_msg_reject(matcher,event,msg)
 
         if s["last"] == "cfstory":
             if text == "退出":
                 s["last"] = True
                 msg = "已退出"
                 await send_msg(matcher,event,msg)
             else:
                 s["cfstory"] = text
                 s["last"] = "public"
-                msg = "该角色是否公开？(最后一步)完成将发送到bot管理站进行审核，审核通过后即可使用"
+                msg = "该角色是否公开？(最后一步)完成将发送到bot管理站进行审核，审核通过后即可使用,请发送是或否或者公开或不公开"
                 await send_msg_reject(matcher,event,msg)
 
         if s["last"] == "public":
             if text == "退出":
                 s["last"] = True
                 msg = "已退出"
                 await send_msg(matcher,event,msg)
             else:
-                name = s["cfnickname"]
-                species = s["cfSpecies"]
-                age = s["cfconage"]
-                stytle = s["cfconstyle"]
-                story = s["cfstory"]
-                easycyber_package["cfNickname"] = s["cfnickname"]
-                easycyber_package["cfSpecies"] = s["cfSpecies"]
-                easycyber_package["cfConAge"] = s["cfconage"]
-                easycyber_package["cfConStyle"] = s["cfconstyle"]
-                easycyber_package["cfStory"] = s["cfstory"]
-                easycyber_package["public"] = text
-                easycyber_package["creator"] = id
-                s["last"] = True
-                cybernick = s["cfnickname"]
-                g = json_get(config_in_global(),"admin_group")
-                u = json_get(config_in_global(),"admin_pro")
-                g_k = json_get(config_in_global(),"admin_group_switch")
-                u_k = json_get(config_in_global(),"admin_user_switch")
-                if not g and u:
-                    logger.opt(colors=True).success(f"{g},{u}")
-                    msg ="bot管理者未配置，超级管理员和bot控制台,审核失败！"
-                elif u == None and g == None:
-                    logger.opt(colors=True).success("false")
-                    msg ="bot管理者未配置，超级管理员和bot控制台,审核失败！"
-                elif u == None and g_k:
-                    easycyber_in_tg(cybernick,easycyber_package)
-                    groupid = json_get(config_in_global(),"admin_group")
-                    msg_tg = f"新投稿！\n来源于QQ[{id}]\n以下为设定内容\n===========\n昵称:{name}\n物种:{species}\n年龄:{age}\n回复风格:{stytle}\n角色故事:{story}\n==========="
-                    await bot.call_api("send_group_msg",group_id=groupid, message=msg_tg)
-                    msg = "投稿成功！，等待审核(问就是权限还没写好)]"
-                elif g == None and u_k:
-                    easycyber_in_tg(cybernick,easycyber_package)
-                    adminid = json_get(config_in_global(),"admin_pro")
-                    msg_tg = f"新投稿！\n来源于QQ[{id}]\n以下为设定内容\n===========\n昵称:{name}\物种:{species}\n年龄:{age}\n回复风格:{stytle}\n角色故事:{story}\n==========="
-                    await bot.call_api("send_private_msg",user_id=adminid, messages=msg_tg)
-                    msg = "投稿成功！，等待审核(问就是权限还没写好)]"
-                elif u_k and g_k:
-                    easycyber_in_tg(cybernick,easycyber_package)
-                    groupid = json_get(config_in_global(),"admin_group")
-                    adminid = json_get(config_in_global(),"admin_pro")
-                    msg_tg = f"新投稿！\n来源于QQ[{id}]\n以下为设定内容\n===========\n昵称:{name}\物种:{species}\n年龄:{age}\n回复风格:{stytle}\n角色故事:{story}\n==========="
-                    await bot.call_api("send_group_msg",group_id=groupid, message=msg_tg)
-                    await bot.call_api("send_private_msg",user_id=adminid, messages=msg_tg)
-                    msg = "投稿成功！，等待审核(问就是权限还没写好)]"
-                elif g_k:
-                    easycyber_in_tg(cybernick,easycyber_package)
-                    adminid = json_get(config_in_global(),"admin_pro")
-                    msg_tg = f"新投稿！\n来源于QQ[{id}]\n以下为设定内容\n===========\n昵称:{name}\物种:{species}\n年龄:{age}\n回复风格:{stytle}\n角色故事:{story}\n==========="
-                    await bot.call_api("send_private_msg",user_id=adminid, messages=msg_tg)
-                else:
-                    easycyber_in_tg(cybernick,easycyber_package)
-                    groupid = json_get(config_in_global(),"admin_group")
-                    msg_tg = f"新投稿！\n来源于QQ[{id}]\n以下为设定内容\n===========\n昵称:{name}\n物种:{species}\n年龄:{age}\n回复风格:{stytle}\n角色故事:{story}\n==========="
-                    await bot.call_api("send_group_msg",group_id=groupid, message=msg_tg)
-                    msg = "投稿成功！，等待审核(问就是权限还没写好)]"
-                await send_msg(matcher,event,msg)
+                key = {"是":True,"否":False,"公开":True,"不公开":False}
+                if not text in key:
+                    s["last"] = "public"
+                    msg = "非正确格式！请重新输入，如需退出请发送：退出"
+                    await send_msg_reject(matcher,event,msg)
+                else:
+                    name = s["cfnickname"]
+                    species = s["cfSpecies"]
+                    age = s["cfconage"]
+                    stytle = s["cfconstyle"]
+                    story = s["cfstory"]
+                    easycyber_package["cfNickname"] = s["cfnickname"]
+                    easycyber_package["cfSpecies"] = s["cfSpecies"]
+                    easycyber_package["cfConAge"] = s["cfconage"]
+                    easycyber_package["cfConStyle"] = s["cfconstyle"]
+                    easycyber_package["cfStory"] = s["cfstory"]
+                    easycyber_package["public"] = key[f"{text}"]
+                    easycyber_package["creator"] = id
+                    s["last"] = True
+                    cybernick = s["cfnickname"]
+                    g = json_get(config_in_global(),"admin_group")
+                    u = json_get(config_in_global(),"admin_pro")
+                    g_k = json_get(config_in_global(),"admin_group_switch")
+                    u_k = json_get(config_in_global(),"admin_user_switch")
+                    if not g and u:
+                        logger.opt(colors=True).success(f"{g},{u}")
+                        msg ="bot管理者未配置，超级管理员和bot控制台,审核失败！"
+                    elif u == None and g == None:
+                        logger.opt(colors=True).success("false")
+                        msg ="bot管理者未配置，超级管理员和bot控制台,审核失败！"
+                    elif u == None and g_k:
+                        easycyber_in_tg(cybernick,easycyber_package)
+                        groupid = json_get(config_in_global(),"admin_group")
+                        msg_tg = f"新投稿！\n来源于QQ[{id}]\n以下为设定内容\n===========\n昵称:{name}\n物种:{species}\n年龄:{age}\n回复风格:{stytle}\n角色故事:{story}\n==========="
+                        await bot.call_api("send_group_msg",group_id=groupid, message=msg_tg)
+                        msg = "投稿成功！，等待审核(问就是权限还没写好)]"
+                    elif g == None and u_k:
+                        easycyber_in_tg(cybernick,easycyber_package)
+                        adminid = json_get(config_in_global(),"admin_pro")
+                        msg_tg = f"新投稿！\n来源于QQ[{id}]\n以下为设定内容\n===========\n昵称:{name}\物种:{species}\n年龄:{age}\n回复风格:{stytle}\n角色故事:{story}\n==========="
+                        await bot.call_api("send_private_msg",user_id=adminid, messages=msg_tg)
+                        msg = "投稿成功！，等待审核(问就是权限还没写好)]"
+                    elif u_k and g_k:
+                        easycyber_in_tg(cybernick,easycyber_package)
+                        groupid = json_get(config_in_global(),"admin_group")
+                        adminid = json_get(config_in_global(),"admin_pro")
+                        msg_tg = f"新投稿！\n来源于QQ[{id}]\n以下为设定内容\n===========\n昵称:{name}\物种:{species}\n年龄:{age}\n回复风格:{stytle}\n角色故事:{story}\n==========="
+                        await bot.call_api("send_group_msg",group_id=groupid, message=msg_tg)
+                        await bot.call_api("send_private_msg",user_id=adminid, messages=msg_tg)
+                        msg = "投稿成功！，等待审核(问就是权限还没写好)]"
+                    elif g_k:
+                        easycyber_in_tg(cybernick,easycyber_package)
+                        adminid = json_get(config_in_global(),"admin_pro")
+                        msg_tg = f"新投稿！\n来源于QQ[{id}]\n以下为设定内容\n===========\n昵称:{name}\物种:{species}\n年龄:{age}\n回复风格:{stytle}\n角色故事:{story}\n==========="
+                        await bot.call_api("send_private_msg",user_id=adminid, messages=msg_tg)
+                    else:
+                        easycyber_in_tg(cybernick,easycyber_package)
+                        groupid = json_get(config_in_global(),"admin_group")
+                        msg_tg = f"新投稿！\n来源于QQ[{id}]\n以下为设定内容\n===========\n昵称:{name}\n物种:{species}\n年龄:{age}\n回复风格:{stytle}\n角色故事:{story}\n==========="
+                        await bot.call_api("send_group_msg",group_id=groupid, message=msg_tg)
+                        msg = "投稿成功！，等待审核(问就是权限还没写好)]"
+                    await send_msg(matcher,event,msg)
 
 
         if s["last"] == "载入":
             if text == "退出":
                 s["last"] = True
                 msg = "已退出"
                 await send_msg(matcher,event,msg)
@@ -710,69 +749,246 @@
                     config = config_in_group(groupid)
                     config_group = json_get(config,groupid)
                     promte = json_get(easycyber_in(False,False),f"{text}")
                     public = json_get(promte,"public")
                     if not public:
                         msg = f"{text}模型拒绝被加载(可能是模型不存在或者模型非公开！)"      
                     else:
+                        if config_group["easycharacter_in"] == text:
+                            msg = f"{text}模型已加载，请勿重新加载"  
+                        else:
+                            config_group["easycharacter_in"] = f"{text}"
+                            config[f"{groupid}"] = config_group
+                            with open(f'{log_dir}\config\config_group.json','w',encoding='utf-8') as file:
+                                json.dump(config,file)
+                                msg = f"{text}加载成功！" 
+                else:
+                    config_user = config_in_user(id,False)
+                    user = json_get(config_user,f"{id}")
+                    promte = json_get(easycyber_in(False,False),f"{text}")
+                    public = json_get(promte,"public")
+                    creator = json_get(promte,"creator")
+                    if creator == id:
+                        if user["easycharacter_in"]== text:
+                            msg = f"{text}模型已加载，请勿重新加载"  
+                        else:
+                            user["easycharacter_in"] = f"{text}"
+                            config_user[f"{id}"] = user
+                            with open(f'{log_dir}\config\config_user.json','w',encoding='utf-8') as file:
+                                json.dump(config_user,file)
+                                msg = f"{text}加载成功！"
+                    elif not public:
+                        msg = f"{text}模型拒绝被加载(可能是模型不存在或者模型非公开！)"      
+                    else:
+                        if user["easycharacter_in"] == text:
+                            msg = f"{text}模型已加载，请勿重新加载"  
+                        else:
+                            user["easycharacter_in"] = f"{text}"
+                            config_user[f"{id}"] = user
+                            with open(f'{log_dir}\config\config_user.json','w',encoding='utf-8') as file:
+                                json.dump(config_user,file)
+                                msg = f"{text}加载成功！" 
+                await send_msg(matcher,event,msg)
+    # 增加预设
+    if text == "投稿":
+        s["last"] = "增加"
+        msg = "请输入角色昵称"
+        await send_msg_reject(matcher,event,msg)
+    if text == "载入":
+        s["last"] = "载入"
+        msg = "请输入公开的角色昵称【非公开会载入失败！】"
+        await send_msg_reject(matcher,event,msg)
+    if text == "查看列表":
+        s["last"] = True
+        list_in = easycyber_in(False,False)
+        try:
+            list_got = []
+            for key in list_in:
+                if list_in[f"{key}"]["public"]:
+                    list_got.append(format(key))
+                else:
+                    return
+            msg = f"[easycyber]可用角色(公开)\n"
+            msg += "\n".join(list_got)
+        except Exception as e:
+            logger.opt(colors=True).error(f"【Hx】:错误捕获:{e}")
+            msg = "当前没有公开的角色哦"
+        await send_msg(matcher,event,msg)
+    # 退出
+    if s["last"]:
+        return
+    else:
+        msg = f"未知命令“{text}”，已退出"
+        await send_msg(matcher,event,msg)
+
+@cyber_set.got(
+    "msg",
+    prompt=f"发送以下选项执行相应功能\n投稿 #投稿自定义预设(不允许同名)\n载入 #载入自定义预设(不允许不存在)\n查看列表 #列出所有公开的自定义预设\n退出 #退出设置\n发送非预期命令则退出",
+)
+async def _(matcher: Matcher, bot:Bot, event: MessageEvent, s: T_State,events: Event):
+    id = get_id(event)
+    text = unescape(event.get_plaintext().strip())
+    easycyber_package = {}
+    if "last" not in s:
+        s["last"] = ""
+    if s["last"]:
+        if s["last"] == "增加":
+            if text == "Hx" or text == "HX" or text == "幻歆":
+                s["last"] = True
+                msg = "cyber预设“Hx”不能删除或修改，如要改动请改源码"
+                await send_msg(matcher,event,msg)
+            else:
+                s["cynickname"] = text
+                s["last"] = "system"
+                msg = "该角色的systempromote是？"
+                await send_msg_reject(matcher,event,msg)
+
+        if s["last"] == "system":
+            if text == "退出":
+                s["last"] = True
+                msg = "已退出"
+                await send_msg(matcher,event,msg)
+            else:
+                s["systempromote"] = text
+                s["last"] = "public"
+                msg = "该角色是否公开u\n请发送公开或不公开（也可以是是或否或者True或False）"
+                await send_msg_reject(matcher,event,msg)
+
+        if s["last"] == "public":
+            if text == "退出":
+                s["last"] = True
+                msg = "已退出"
+                await send_msg(matcher,event,msg)
+            else:
+                key = {"是":True,"否":False,"公开":True,"不公开":False}
+                if not text in key:
+                    s["last"] = "public"
+                    msg = "非正确格式！请重新输入，如需退出请发送：退出"
+                    await send_msg_reject(matcher,event,msg)
+                else:
+                    name = s["cfnickname"]
+                    systempromote = s["systempromote"]
+                    easycyber_package["system"] = s["systempromote"]
+                    easycyber_package["public"] = key[f"{text}"]
+                    easycyber_package["creator"] = id
+                    s["last"] = True
+                    g = json_get(config_in_global(),"admin_group")
+                    u = json_get(config_in_global(),"admin_pro")
+                    g_k = json_get(config_in_global(),"admin_group_switch")
+                    u_k = json_get(config_in_global(),"admin_user_switch")
+                    if not g and u:
+                        logger.opt(colors=True).success(f"{g},{u}")
+                        msg ="bot管理者未配置，超级管理员和bot控制台,审核失败！"
+                    elif u == None and g == None:
+                        logger.opt(colors=True).success("false")
+                        msg ="bot管理者未配置，超级管理员和bot控制台,审核失败！"
+                    elif u == None and g_k:
+                        cyber_in_tg(name,easycyber_package)
+                        groupid = json_get(config_in_global(),"admin_group")
+                        msg_tg = f"新投稿！\n来源于QQ[{id}]\n以下为设定内容\n===========\n昵称:{name}\nsystem:{systempromote}==========="
+                        await bot.call_api("send_group_msg",group_id=groupid, message=msg_tg)
+                        msg = "投稿成功！，等待审核(问就是权限还没写好)]"
+                    elif g == None and u_k:
+                        cyber_in_tg(name,easycyber_package)
+                        adminid = json_get(config_in_global(),"admin_pro")
+                        msg_tg = f"新投稿！\n来源于QQ[{id}]\n以下为设定内容\n===========\n昵称:{name}\nsystem:{systempromote}==========="
+                        await bot.call_api("send_private_msg",user_id=adminid, messages=msg_tg)
+                        msg = "投稿成功！，等待审核(问就是权限还没写好)]"
+                    elif u_k and g_k:
+                        cyber_in_tg(name,easycyber_package)
+                        groupid = json_get(config_in_global(),"admin_group")
+                        adminid = json_get(config_in_global(),"admin_pro")
+                        msg_tg = f"新投稿！\n来源于QQ[{id}]\n以下为设定内容\n===========\n昵称:{name}\nsystem:{systempromote}==========="
+                        await bot.call_api("send_group_msg",group_id=groupid, message=msg_tg)
+                        await bot.call_api("send_private_msg",user_id=adminid, messages=msg_tg)
+                        msg = "投稿成功！，等待审核(问就是权限还没写好)]"
+                    elif g_k:
+                        cyber_in_tg(name,easycyber_package)
+                        adminid = json_get(config_in_global(),"admin_pro")
+                        msg_tg = f"新投稿！\n来源于QQ[{id}]\n以下为设定内容\n===========\n昵称:{name}\nsystem:{systempromote}==========="
+                        await bot.call_api("send_private_msg",user_id=adminid, messages=msg_tg)
+                    else:
+                        cyber_in_tg(name,easycyber_package)
+                        groupid = json_get(config_in_global(),"admin_group")
+                        msg_tg = f"新投稿！\n来源于QQ[{id}]\n以下为设定内容\n===========\n昵称:{name}\nsystem:{systempromote}==========="
+                        await bot.call_api("send_group_msg",group_id=groupid, message=msg_tg)
+                        msg = "投稿成功！，等待审核(问就是权限还没写好)]"
+                    await send_msg(matcher,event,msg)
+        if s["last"] == "载入":
+            if text == "退出":
+                s["last"] = True
+                msg = "已退出"
+                await send_msg(matcher,event,msg)
+            else:
+                s["last"] = True
+                if isinstance(events, GroupMessageEvent):
+                    groupid = get_groupid(event)
+                    config = config_in_group(groupid)
+                    config_group = json_get(config,groupid)
+                    promte = json_get(cyber_in(False,False),f"{text}")
+                    public = json_get(promte,"public")
+                    if not public:
+                        msg = f"{text}模型拒绝被加载(可能是模型不存在或者模型非公开！)"      
+                    else:
                         if config_group["character_in"] == text:
                             msg = f"{text}模型已加载，请勿重新加载"  
                         else:
                             config_group["character_in"] = f"{text}"
                             config[f"{groupid}"] = config_group
-                            with open(f'{log_dir}/config/config_group.json','w',encoding='utf-8') as file:
+                            with open(f'{log_dir}\config\config_group.json','w',encoding='utf-8') as file:
                                 json.dump(config,file)
                                 msg = f"{text}加载成功！" 
                 else:
                     config_user = config_in_user(id,False)
                     user = json_get(config_user,f"{id}")
-                    promte = json_get(easycyber_in(False,False),f"{text}")
+                    promte = json_get(cyber_in(False,False),f"{text}")
                     public = json_get(promte,"public")
                     creator = json_get(promte,"creator")
                     if creator == id:
                         if user["character_in"]== text:
                             msg = f"{text}模型已加载，请勿重新加载"  
                         else:
                             user["character_in"] = f"{text}"
                             config_user[f"{id}"] = user
-                            with open(f'{log_dir}/config/config_user.json','w',encoding='utf-8') as file:
+                            with open(f'{log_dir}\config\config_user.json','w',encoding='utf-8') as file:
                                 json.dump(config_user,file)
                                 msg = f"{text}加载成功！"
                     elif not public:
                         msg = f"{text}模型拒绝被加载(可能是模型不存在或者模型非公开！)"      
                     else:
                         if user["character_in"] == text:
                             msg = f"{text}模型已加载，请勿重新加载"  
                         else:
                             user["character_in"] = f"{text}"
                             config_user[f"{id}"] = user
-                            with open(f'{log_dir}/config/config_user.json','w',encoding='utf-8') as file:
+                            with open(f'{log_dir}\config\config_user.json','w',encoding='utf-8') as file:
                                 json.dump(config_user,file)
                                 msg = f"{text}加载成功！" 
                 await send_msg(matcher,event,msg)
     # 增加预设
     if text == "投稿":
         s["last"] = "增加"
         msg = "请输入角色昵称"
         await send_msg_reject(matcher,event,msg)
     if text == "载入":
         s["last"] = "载入"
         msg = "请输入公开的角色昵称【非公开会载入失败！】"
         await send_msg_reject(matcher,event,msg)
     if text == "查看列表":
         s["last"] = True
-        list_in = easycyber_in(False,False)
+        list_in = cyber_in(False,False)
         try:
             list_got = []
             for key in list_in:
                 if list_in[f"{key}"]["public"]:
                     list_got.append(format(key))
                 else:
                     return
-            msg = f"{list_got}"
+            msg = f"[cyber]可用角色(公开)\n"
+            msg += "\n".join(list_got)
         except Exception as e:
             msg = "当前没有公开的角色哦"
         await send_msg(matcher,event,msg)
     # 退出
     if s["last"]:
         return
     else:
@@ -794,27 +1010,27 @@
             if s["last"] == "通过1":
                 json_1 = easycyber_in_tg(False,False)
                 json_data = json_get(json_1,text)
                 json_data["tg_admin"] = id
                 user = json_data["creator"]
                 in_ok = easycyber_in(text,json_data)
                 end_json = json_1.pop(f"{text}")
-                with open(f'{log_dir}/file/easycyber_tg.json','w',encoding='utf-8') as file:
+                with open(f'{log_dir}\file\easycyber_tg.json','w',encoding='utf-8') as file:
                     json.dump(json_1,file)
                     s["last"] = True
                     msg = f"已通过投稿用户为{user}关于角色{text}的投稿"
                 await send_msg(matcher,event,msg)
 
             if s["last"] == "拒绝":
                 s["last"] = True
                 json_1 = easycyber_in_tg(False,False)
                 json_data = json_get(json_1,text)
                 user = json_data["creator"]
                 end_json = json_1.pop(f"{text}")
-                with open(f'{log_dir}/file/easycyber_tg.json','w',encoding='utf-8') as file:
+                with open(f'{log_dir}\file\easycyber_tg.json','w',encoding='utf-8') as file:
                     json.dump(json_1,file)
                     msg = f"已拒绝投稿用户为{user}关于角色{text}的投稿"
                 await send_msg(matcher,event,msg)
 
         if text == "通过":
             s["last"] = "通过1"
             msg = "请输入要加入角色昵称"
@@ -837,8 +1053,87 @@
             return
         else:
             msg = f"未知命令“{text}”，已退出"
             await send_msg(matcher,event,msg)
 
     else:
         msg = f"你的权限为{place_user},权限不足，无法操作"
-        await send_msg(matcher, event, msg)
+        await send_msg(matcher, event, msg)
+
+@chat_ne.got(
+    "msg",
+    prompt=f"发送以下选项执行相应功能\n加入 #银影将会主动来找你聊天》？\n退出 #呜呜呜，真的要赶银影走吗\n查看加入列表 #字如其意(仅限管理员使用)\n发送非预期命令则退出",
+)
+async def _(matcher: Matcher,event: MessageEvent, s: T_State):
+    id = get_id(event)
+    text = unescape(event.get_plaintext().strip())
+    config_1 = config_in_user(id,False)
+    user_config = json_get(config_1,id)
+    global_config = config_in_global()
+    dy_list = json_get(global_config,"dy_list")
+    if "last" not in s:
+        s["last"] = ""
+    if s["last"]:
+        if s["last"] == "加入":
+            if text == "惊喜":
+                s["last"] = True
+                hour = random.randint(1,2)
+                minute = random.randint(1,59)
+                user_config["dy_time"] = hour
+                user_config["dy_minute"] = minute
+                dy_list.append(id)
+                config_1[f"{id}"] = user_config
+                global_config["dy_list"] = dy_list
+                msg = "好哦，银影会不定时来找你聊天的！"
+                scheduler.add_job(func=get_chat,trigger='interval',args=[id] ,hours=hour, minutes=minute, id=id)
+                with open(f'{log_dir}\config\config_global.json','w',encoding='utf-8') as file:
+                    json.dump(global_config,file)
+                with open(f'{log_dir}\config\config_user.json','w',encoding='utf-8') as file:
+                    json.dump(config_1,file)
+                await send_msg(matcher,event,msg)
+            elif text == "意外":
+                s["last"] = True
+                msg = "在写了在写了"
+                await send_msg_reject(matcher,event,msg)
+
+
+    if text == "加入":
+        s["last"] = "加入"
+        global_config = config_in_global()
+        dy_list = json_get(global_config,"dy_list")
+        if id in dy_list:
+            msg = "你已经在银影的特关列表了），请不要重复添加"
+        else:
+            msg = "请选择惊喜or稳定\n发送：惊喜或者稳定即可"
+        await send_msg_reject(matcher,event,msg)
+
+    if text == "退出":
+        s["last"] = True
+        global_config = config_in_global()
+        dy_list = json_get(global_config,"dy_list")
+        if not id in dy_list:
+            msg = "你不在银影的特关列表哦（"
+        else:
+            msg = "那再见咯，银影会想你的"
+            end_json = dy_list.remove(id)
+            global_config["dy_list"] = f"{dy_list}"
+            scheduler.remove_job(id)
+            with open(f'{log_dir}\config\config_global.json','w',encoding='utf-8') as file:
+                json.dump(global_config,file)
+        await send_msg_reject(matcher,event,msg)
+
+    if text == "查看加入列表":
+        s["last"] = True
+        msg = "在写了在写了，呜呜呜呜呜呜呜"
+        await send_msg(matcher,event,msg)
+
+    # 退出
+    if s["last"]:
+        return
+    else:
+        msg = f"未知命令“{text}”，已退出"
+        await send_msg(matcher,event,msg)
+
+@ces.handle()
+async def _(event: MessageEvent):
+    id = get_id(event)
+    await get_chat(id)
```

### Comparing `nonebot-plugin-hx-yinying-1.0.5/nonebot_plugin_hx_yinying.egg-info/PKG-INFO` & `nonebot-plugin-hx-yinying-1.0.6/nonebot_plugin_hx_yinying.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-hx-yinying
-Version: 1.0.5
+Version: 1.0.6
 Summary: chat with yinying
 Home-page: https://github.com/huanxin996/nonebot_plugin_hx-yinying
 Author: Huan Xin
 Author-email: mc.xiaolang@foxmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -15,15 +15,15 @@
 <!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
 [![All Contributors](https://img.shields.io/badge/all_contributors-2-orange.svg?style=flat-square)](#contributors-)
 <!-- ALL-CONTRIBUTORS-BADGE:END -->
 
  * @Author         : huanxin996
  * @Date           : 2024-4-17
  * @LastEditors    : huanxin996
- * @LastEditTime   : 2024-4-22
+ * @LastEditTime   : 2024-4-26
  * @Description    : None
  * @GitHub         : https://github.com/huanxin996
 -->
 
 <!-- markdownlint-disable MD033 MD036 MD041 -->
 
 <p align="center">
@@ -66,26 +66,96 @@
 - @Bot 或者回复即可
 
 OneBot:
 
 - @Bot
 - 回复Bot
 
+
+<details>
+  <summary><b style="font-size: 1.5rem">指令集</b></summary>
+
+/hx
+- 别名：chat
+- 主要对话命令
+
+/刷新对话
+- 别名：clear
+- 主动刷新对话
+
+/导出对话
+- 别名：getchat
+- 导出对话记录，没有对话记录会出错。
+
+/设置全局配置
+- 别名：设置配置全局，globalset
+- 设置bot的全局配置
+
+/导出全局配置
+- 别名：getset_global
+- 导出bot的全局配置
+- 该命令包含在"设置全局配置"里
+
+/模型列表
+- 别名：modellist，chat模型列表
+- 发送bot可用模型
+
+/切换模型 [模型id]
+- 别名：qhmodel，切换chat模型，模型切换
+- 切换bot当前使用的模型
+- 私聊群聊动态响应，如果在群内输入则切换群内加载的模型，私聊输入则切换私聊的。
+
+/easycyber
+- 别名：easycyber设置，hxworld
+- 模型easycyberfurry主要配置
+- 内有多个指令
+
+/控制台操作
+- 别名：管理控制台，setstart
+- 模型easycyberfurry的角色投稿管理，即将更新cyber的角色投稿管理
+- 内有多个指令
+
+/确认版本
+- 别名：旅行伙伴确认，版本确认
+- 确认bot当前使用的版本和当前加载的模型。区分群聊和私聊动态响应
+
+/sd [名称] [设定]
+- 别名：旅行伙伴加入，设定加入
+- [名称]可为空，即发送 旅行伙伴加入 [设定]
+- [设定]不可为空，必填
+- 载入用户的设定信息和自定义昵称
+
+
+
+
+
+
+
+
+
+
+
+
+</details>
+<br>
+
 ## 配置项
 
 > [!WARNING]
 > GitHub 仓库中的文档为最新 DEV 版本，配置方式请参考 [PyPI](https://pypi.python.org/pypi/nonebot-plugin-hx-yinying) 上的文档。
 
 > [!WARNING]
 > 秩乱(乱乱)的联系方式如下，QQ:1660466270，官方qq群聊:175334224 [官网链接](https://chat.wingmark.cn/) .
 
 > [!WARNING]
 > 请注意，该项目是接入了乱乱的项目，你需要遵守api使用的 [规范](https://wingmark.feishu.cn/docx/NFgJddgQAotygKxXiu6cpyg5nqr)。
 
 配置方式：直接在 NoneBot 全局配置文件中添加以下配置项即可。
+<details>
+  <summary><b style="font-size: 1.5rem">配置项列表</b></summary>
 
 ### yinying_appid
 
 - 类型：`str`
 - 默认值：`None`
 - 说明：你的appid
 - 重要：必填
@@ -105,14 +175,17 @@
 
 ### SUPERUSERS
 - 类型：`list`
 - 默认值：`None`
 - 说明：这里是超级管理员（插件）
 - 重要：必填（你需要这个来管理该插件）
 
+</details>
+<br>
+
 配置文件示例（默认模板）
 
 ```dotenv
 yinying_appid=你的appid
 yinying_token=你的token(不带bearer)
 hx_path=C:\Users\user\Desktop
 ```
```

#### html2text {}

```diff
@@ -1,35 +1,55 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-hx-yinying Version: 1.0.5 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-hx-yinying Version: 1.0.6 Summary:
 chat with yinying Home-page: https://github.com/huanxin996/nonebot_plugin_hx-
 yinying Author: Huan Xin Author-email: mc.xiaolang@foxmail.com Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Description-Content-
 Type: text/markdown License-File: LICENSE [![All Contributors](https://
 img.shields.io/badge/all_contributors-2-orange.svg?style=flat-square)]
 (#contributors-) * @Author : huanxin996 * @Date : 2024-4-17 * @LastEditors :
-huanxin996 * @LastEditTime : 2024-4-22 * @Description : None * @GitHub : https:
+huanxin996 * @LastEditTime : 2024-4-26 * @Description : None * @GitHub : https:
 //github.com/huanxin996 -->
                                    _[_n_o_n_e_b_o_t_]
                 # nonebot_plugin_hx-yinying _â¨ Hx vs YinYing
                   (å¨çº¿ä¸é¶å½±è¿è¡å¯¹è¯çæä»¶) â¨_
                             _[_l_i_c_e_n_s_e_]_[_p_y_p_i_][python]
 ## å®è£ pipå®è£ ```dotenv pip install nonebot-plugin-hx-yinying ``` nb
 pluginå®è£ ```dotenv nb plugin install nonebot-plugin-hx-yinying ``` ##
-ä½¿ç¨æ¹å¼ éç¨: - @Bot æèåå¤å³å¯ OneBot: - @Bot - åå¤Bot ##
-éç½®é¡¹ > [!WARNING] > GitHub ä»åºä¸­çææ¡£ä¸ºææ° DEV
+ä½¿ç¨æ¹å¼ éç¨: - @Bot æèåå¤å³å¯ OneBot: - @Bot - åå¤Bot
+?æ???ä?»?¤?é?? /hx - å«åï¼chat - ä¸»è¦å¯¹è¯å½ä»¤ /å·æ°å¯¹è¯ -
+å«åï¼clear - ä¸»å¨å·æ°å¯¹è¯ /å¯¼åºå¯¹è¯ - å«åï¼getchat -
+å¯¼åºå¯¹è¯è®°å½ï¼æ²¡æå¯¹è¯è®°å½ä¼åºéã /è®¾ç½®å¨å±éç½® -
+å«åï¼è®¾ç½®éç½®å¨å±ï¼globalset - è®¾ç½®botçå¨å±éç½® /
+å¯¼åºå¨å±éç½® - å«åï¼getset_global - å¯¼åºbotçå¨å±éç½® -
+è¯¥å½ä»¤åå«å¨"è®¾ç½®å¨å±éç½®"é /æ¨¡ååè¡¨ -
+å«åï¼modellistï¼chatæ¨¡ååè¡¨ - åébotå¯ç¨æ¨¡å /åæ¢æ¨¡å
+[æ¨¡åid] - å«åï¼qhmodelï¼åæ¢chatæ¨¡åï¼æ¨¡ååæ¢ -
+åæ¢botå½åä½¿ç¨çæ¨¡å -
+ç§èç¾¤èå¨æååºï¼å¦æå¨ç¾¤åè¾å¥ååæ¢ç¾¤åå è½½çæ¨¡åï¼ç§èè¾å¥ååæ¢ç§èçã
+/easycyber - å«åï¼easycyberè®¾ç½®ï¼hxworld -
+æ¨¡åeasycyberfurryä¸»è¦éç½® - åæå¤ä¸ªæä»¤ /æ§å¶å°æä½ -
+å«åï¼ç®¡çæ§å¶å°ï¼setstart -
+æ¨¡åeasycyberfurryçè§è²æç¨¿ç®¡çï¼å³å°æ´æ°cyberçè§è²æç¨¿ç®¡ç
+- åæå¤ä¸ªæä»¤ /ç¡®è®¤çæ¬ - å«åï¼æè¡ä¼ä¼´ç¡®è®¤ï¼çæ¬ç¡®è®¤
+-
+ç¡®è®¤botå½åä½¿ç¨ççæ¬åå½åå è½½çæ¨¡åãåºåç¾¤èåç§èå¨æååº
+/sd [åç§°] [è®¾å®] - å«åï¼æè¡ä¼ä¼´å å¥ï¼è®¾å®å å¥ -
+[åç§°]å¯ä¸ºç©ºï¼å³åé æè¡ä¼ä¼´å å¥ [è®¾å®] -
+[è®¾å®]ä¸å¯ä¸ºç©ºï¼å¿å¡« - è½½å¥ç¨æ·çè®¾å®ä¿¡æ¯åèªå®ä¹æµç§°
+## éç½®é¡¹ > [!WARNING] > GitHub ä»åºä¸­çææ¡£ä¸ºææ° DEV
 çæ¬ï¼éç½®æ¹å¼è¯·åè [PyPI](https://pypi.python.org/pypi/nonebot-
 plugin-hx-yinying) ä¸çææ¡£ã > [!WARNING] > ç§©ä¹±
 (ä¹±ä¹±)çèç³»æ¹å¼å¦ä¸ï¼QQ:1660466270ï¼å®æ¹qqç¾¤è:175334224
 [å®ç½é¾æ¥](https://chat.wingmark.cn/) . > [!WARNING] >
 è¯·æ³¨æï¼è¯¥é¡¹ç®æ¯æ¥å¥äºä¹±ä¹±çé¡¹ç®ï¼ä½ éè¦éµå®apiä½¿ç¨ç
 [è§è](https://wingmark.feishu.cn/docx/NFgJddgQAotygKxXiu6cpyg5nqr)ã
 éç½®æ¹å¼ï¼ç´æ¥å¨ NoneBot
-å¨å±éç½®æä»¶ä¸­æ·»å ä»¥ä¸éç½®é¡¹å³å¯ã ### yinying_appid -
-ç±»åï¼`str` - é»è®¤å¼ï¼`None` - è¯´æï¼ä½ çappid - éè¦ï¼å¿å¡«
-### yinying_token - ç±»åï¼`str` - é»è®¤å¼ï¼`None` -
+å¨å±éç½®æä»¶ä¸­æ·»å ä»¥ä¸éç½®é¡¹å³å¯ã ?é???ç?½?®?é?¡?¹?å???è?¡?¨ ###
+yinying_appid - ç±»åï¼`str` - é»è®¤å¼ï¼`None` - è¯´æï¼ä½ çappid -
+éè¦ï¼å¿å¡« ### yinying_token - ç±»åï¼`str` - é»è®¤å¼ï¼`None` -
 è¯´æï¼è¿éåä½ æ¾ç§©ä¹±è·åå°çapi_key - éè¦ï¼å¿å¡« ### hx_path
 - ç±»åï¼`str` - é»è®¤å¼ï¼`None` -
 è¯´æï¼è¿éæ¯æä»¶æ¬å°éç½®çå­å¨ç®å½ - éè¦ï¼éå¿å¡« ###
 SUPERUSERS - ç±»åï¼`list` - é»è®¤å¼ï¼`None` -
 è¯´æï¼è¿éæ¯è¶çº§ç®¡çåï¼æä»¶ï¼ -
 éè¦ï¼å¿å¡«ï¼ä½ éè¦è¿ä¸ªæ¥ç®¡çè¯¥æä»¶ï¼
 éç½®æä»¶ç¤ºä¾ï¼é»è®¤æ¨¡æ¿ï¼ ```dotenv yinying_appid=ä½ çappid
```

### Comparing `nonebot-plugin-hx-yinying-1.0.5/setup.py` & `nonebot-plugin-hx-yinying-1.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="nonebot-plugin-hx-yinying",
-    version="1.0.5",
+    version="1.0.6",
     author="Huan Xin",
     author_email="mc.xiaolang@foxmail.com",
     description="chat with yinying",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/huanxin996/nonebot_plugin_hx-yinying",
     packages=setuptools.find_packages(),
```


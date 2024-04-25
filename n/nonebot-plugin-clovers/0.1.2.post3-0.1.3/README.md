# Comparing `tmp/nonebot_plugin_clovers-0.1.2.post3.tar.gz` & `tmp/nonebot_plugin_clovers-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_clovers-0.1.2.post3.tar", max compression
+gzip compressed data, was "nonebot_plugin_clovers-0.1.3.tar", max compression
```

## Comparing `nonebot_plugin_clovers-0.1.2.post3.tar` & `nonebot_plugin_clovers-0.1.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1086 2024-04-15 11:49:16.312798 nonebot_plugin_clovers-0.1.2.post3/LICENSE
--rw-r--r--   0        0        0     2522 2024-04-20 03:42:50.974654 nonebot_plugin_clovers-0.1.2.post3/nonebot_plugin_clovers/__init__.py
--rw-r--r--   0        0        0      842 2024-04-15 02:23:00.900179 nonebot_plugin_clovers-0.1.2.post3/nonebot_plugin_clovers/adapters/main.py
--rw-r--r--   0        0        0     4240 2024-04-23 10:10:22.146061 nonebot_plugin_clovers-0.1.2.post3/nonebot_plugin_clovers/adapters/onebot/v11.py
--rw-r--r--   0        0        0     1732 2024-04-20 03:58:16.439239 nonebot_plugin_clovers-0.1.2.post3/nonebot_plugin_clovers/adapters/qq.py
--rw-r--r--   0        0        0      365 2024-04-20 03:23:59.271766 nonebot_plugin_clovers-0.1.2.post3/nonebot_plugin_clovers/config.py
--rw-r--r--   0        0        0      557 2024-04-23 17:15:09.977152 nonebot_plugin_clovers-0.1.2.post3/pyproject.toml
--rw-r--r--   0        0        0     2514 2024-04-15 11:57:25.353441 nonebot_plugin_clovers-0.1.2.post3/README.md
--rw-r--r--   0        0        0     3036 1970-01-01 00:00:00.000000 nonebot_plugin_clovers-0.1.2.post3/PKG-INFO
+-rw-r--r--   0        0        0     1086 2024-04-15 11:49:16.312798 nonebot_plugin_clovers-0.1.3/LICENSE
+-rw-r--r--   0        0        0     2778 2024-04-25 16:26:30.767928 nonebot_plugin_clovers-0.1.3/nonebot_plugin_clovers/__init__.py
+-rw-r--r--   0        0        0      843 2024-04-25 15:59:33.461893 nonebot_plugin_clovers-0.1.3/nonebot_plugin_clovers/adapters/main.py
+-rw-r--r--   0        0        0     4241 2024-04-25 16:04:21.704665 nonebot_plugin_clovers-0.1.3/nonebot_plugin_clovers/adapters/onebot/v11.py
+-rw-r--r--   0        0        0     1724 2024-04-25 16:00:47.948721 nonebot_plugin_clovers-0.1.3/nonebot_plugin_clovers/adapters/qq.py
+-rw-r--r--   0        0        0      365 2024-04-20 03:23:59.271766 nonebot_plugin_clovers-0.1.3/nonebot_plugin_clovers/config.py
+-rw-r--r--   0        0        0      570 2024-04-25 16:26:29.280518 nonebot_plugin_clovers-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2514 2024-04-15 11:57:25.353441 nonebot_plugin_clovers-0.1.3/README.md
+-rw-r--r--   0        0        0     3065 1970-01-01 00:00:00.000000 nonebot_plugin_clovers-0.1.3/PKG-INFO
```

### Comparing `nonebot_plugin_clovers-0.1.2.post3/LICENSE` & `nonebot_plugin_clovers-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_clovers-0.1.2.post3/nonebot_plugin_clovers/__init__.py` & `nonebot_plugin_clovers-0.1.3/nonebot_plugin_clovers/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,33 +1,38 @@
 import os
 from pathlib import Path
 from nonebot import get_driver, get_plugin_config, on_message
 from nonebot.matcher import Matcher
 from nonebot.plugin import PluginMetadata
-from clovers.core.adapter import AdapterMethod
+from nonebot.log import LoguruHandler, logger
+from clovers.core.logger import logger as clovers_logger
+from clovers.core.adapter import Adapter
 from clovers.core.plugin import PluginLoader
-from .adapters.main import extract_command, new_adapter
+from .adapters.main import extract_command, new_clovers
 from .config import Config, ConfigClovers
 
 __plugin_meta__ = PluginMetadata(
     name="clovers插件框架",
     description="NoneBot clovers框架",
     usage="加载即用",
     type="application",
     homepage="https://github.com/KarisAya/nonebot_plugin_clovers",
     config=Config,
     supported_adapters={
         "nonebot.adapters.qq",
         "nonebot.adapters.onebot.v11",
     },
 )
-
+driver = get_driver()
+# 配置日志记录器
+log_level = driver.config.log_level
+clovers_logger.setLevel(log_level)
+clovers_logger.addHandler(LoguruHandler(log_level))
 # 加载配置
 config_data = get_plugin_config(Config)
-
 clovers_config_file = config_data.clovers_config_file
 clovers_priority = config_data.clovers_priority
 
 os.environ["clovers_config_file"] = clovers_config_file
 
 # 添加环境变量之后加载config
 
@@ -39,29 +44,30 @@
 clovers_config.save()
 
 
 plugins_path = Path(clovers_config_data.plugins_path)
 plugins_path.mkdir(exist_ok=True, parents=True)
 
 loader = PluginLoader(plugins_path, clovers_config_data.plugins_list)
-adapter = new_adapter(loader.plugins)
 
-get_driver().on_startup(adapter.startup)
+clovers = new_clovers(loader.plugins)
+
+driver.on_startup(clovers.startup)
 
 main = on_message(priority=clovers_priority, block=False)
 
 
-def add_response(Bot, Event, adapter_method: AdapterMethod, adapter_key: str):
-    print(f"加载适配器：{adapter_key}")
-    adapter.methods[adapter_key] = adapter_method
+def add_response(Bot, Event, adapter: Adapter, adapter_key: str):
+    logger.info(f"加载适配器：{adapter_key}")
+    clovers.adapter_dict[adapter_key] = adapter
 
     @main.handle()
     async def _(matcher: Matcher, bot: Bot, event: Event):
         command = extract_command(event.get_plaintext())
-        if await adapter.response(adapter_key, command, bot=bot, event=event):
+        if await clovers.response(adapter_key, command, bot=bot, event=event):
             matcher.stop_propagation()
 
 
 using_adapters = config_data.using_adapters
 
 
 if "nonebot.adapters.qq" in using_adapters:
```

### Comparing `nonebot_plugin_clovers-0.1.2.post3/nonebot_plugin_clovers/adapters/main.py` & `nonebot_plugin_clovers-0.1.3/nonebot_plugin_clovers/adapters/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from nonebot import get_driver
 from clovers.core.plugin import Plugin
-from clovers.core.adapter import Adapter
+from clovers import Clovers
 
 # 加载配置
 driver = get_driver()
 global_config = driver.config
 
 command_start = {x for x in global_config.command_start if x}
 
@@ -16,18 +16,18 @@
     return msg
 
 
 Bot_NICKNAME = list(global_config.nickname)
 Bot_NICKNAME = Bot_NICKNAME[0] if Bot_NICKNAME else "bot"
 
 
-def new_adapter(plugins: list[Plugin] | None = None):
-    """创建新的adapter，包括注入插件和全局方法"""
-    adapter = Adapter()
+def new_clovers(plugins: list[Plugin] | None = None):
+    """创建新的Clovers实例，包括注入插件和全局方法"""
+    clovers = Clovers()
     if plugins:
-        adapter.plugins = plugins
+        clovers.plugins = plugins
 
-    @adapter.method.kwarg("Bot_Nickname")
+    @clovers.global_adapter.kwarg("Bot_Nickname")
     async def _():
         return Bot_NICKNAME
 
-    return adapter
+    return clovers
```

### Comparing `nonebot_plugin_clovers-0.1.2.post3/nonebot_plugin_clovers/adapters/onebot/v11.py` & `nonebot_plugin_clovers-0.1.3/nonebot_plugin_clovers/adapters/onebot/v11.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,118 +1,118 @@
 from io import BytesIO
 from collections.abc import Callable, Coroutine, AsyncGenerator
-from clovers.core.adapter import AdapterMethod
+from clovers.core.adapter import Adapter
 from clovers.core.plugin import Result
 from nonebot.matcher import Matcher
 from nonebot.permission import SUPERUSER
 from nonebot.adapters.onebot.v11 import (
     Bot,
     MessageEvent,
     GroupMessageEvent,
     Message,
     MessageSegment,
     GROUP_ADMIN,
     GROUP_OWNER,
 )
 
 
-def initializer(main: type[Matcher]) -> AdapterMethod:
-    method = AdapterMethod()
+def initializer(main: type[Matcher]) -> Adapter:
+    adapter = Adapter()
 
-    @method.send("text")
+    @adapter.send("text")
     async def _(message: str, send: Callable[..., Coroutine] = main.send):
         """发送纯文本"""
         await send(message)
 
-    @method.send("image")
+    @adapter.send("image")
     async def _(message: BytesIO, send: Callable[..., Coroutine] = main.send):
         """发送图片"""
         await send(MessageSegment.image(message))
 
-    @method.send("list")
+    @adapter.send("list")
     async def _(message: list[Result], send: Callable[..., Coroutine] = main.send):
         """发送图片文本混合信息，@信息在此发送"""
         msg = Message()
         for seg in message:
             match seg.send_method:
                 case "text":
                     msg += seg.data
                 case "image":
                     msg += MessageSegment.image(seg.data)
                 case "at":
                     msg += MessageSegment.at(seg.data)
         await send(msg)
 
-    @method.send("segmented")
+    @adapter.send("segmented")
     async def _(message: AsyncGenerator[Result, None], send: Callable[..., Coroutine] = main.send):
         """发送分段信息"""
         async for seg in message:
-            await method.send_dict[seg.send_method](seg.data, send)
+            await adapter.send_dict[seg.send_method](seg.data, send)
 
-    @method.kwarg("user_id")
+    @adapter.kwarg("user_id")
     async def _(event: MessageEvent):
         return event.get_user_id()
 
-    @method.kwarg("group_id")
+    @adapter.kwarg("group_id")
     async def _(event: MessageEvent):
         group_id = getattr(event, "group_id", None)
         return str(group_id) if group_id else None
 
-    @method.kwarg("to_me")
+    @adapter.kwarg("to_me")
     async def _(event: MessageEvent):
         return event.to_me
 
-    @method.kwarg("nickname")
+    @adapter.kwarg("nickname")
     async def _(event: MessageEvent):
         return event.sender.card or event.sender.nickname
 
-    @method.kwarg("avatar")
+    @adapter.kwarg("avatar")
     async def _(event: MessageEvent) -> str:
         return f"https://q1.qlogo.cn/g?b=qq&nk={event.user_id}&s=640"
 
-    @method.kwarg("group_avatar")
+    @adapter.kwarg("group_avatar")
     async def _(event: MessageEvent) -> str:
         if isinstance(event, GroupMessageEvent):
             return f"https://p.qlogo.cn/gh/{event.group_id}/{event.group_id}/640"
         return ""
 
-    @method.kwarg("image_list")
+    @adapter.kwarg("image_list")
     async def _(event: MessageEvent):
         url = [msg.data["url"] for msg in event.message if msg.type == "image"]
         if event.reply:
             url += [msg.data["url"] for msg in event.reply.message if msg.type == "image"]
         return url
 
-    @method.kwarg("permission")
+    @adapter.kwarg("permission")
     async def _(bot: Bot, event: MessageEvent) -> int:
         if await SUPERUSER(bot, event):
             return 3
         if await GROUP_OWNER(bot, event):
             return 2
         if await GROUP_ADMIN(bot, event):
             return 1
         return 0
 
-    @method.kwarg("at")
+    @adapter.kwarg("at")
     async def _(event: MessageEvent) -> list[str]:
         return [str(msg.data["qq"]) for msg in event.message if msg.type == "at"]
 
-    @method.kwarg("send_group_message")
+    @adapter.kwarg("send_group_message")
     async def _(bot: Bot) -> Callable[[int, Result], Coroutine]:
         async def send_group_message(group_id: int, result: Result):
             send = lambda message: bot.send_group_msg(group_id=group_id, message=message)
-            await method.send_dict[result.send_method](result.data, send)
+            await adapter.send_dict[result.send_method](result.data, send)
 
         return send_group_message
 
-    @method.kwarg("group_member_list")
+    @adapter.kwarg("group_member_list")
     async def _(bot: Bot, event: MessageEvent) -> None | list[dict]:
         if not isinstance(event, GroupMessageEvent):
             return None
         info_list = await bot.get_group_member_list(group_id=event.group_id)
         for user_info in info_list:
             user_id = str(user_info["user_id"])
             user_info["user_id"] = user_id
             user_info["avatar"] = f"https://q1.qlogo.cn/g?b=qq&nk={user_id}&s=640"
         return info_list
 
-    return method
+    return adapter
```

### Comparing `nonebot_plugin_clovers-0.1.2.post3/nonebot_plugin_clovers/adapters/qq.py` & `nonebot_plugin_clovers-0.1.3/nonebot_plugin_clovers/adapters/qq.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,53 +1,53 @@
 from io import BytesIO
 from collections.abc import Callable, AsyncGenerator
-from clovers.core.adapter import AdapterMethod
+from clovers.core.adapter import Adapter
 from clovers.core.plugin import Result
 from nonebot.matcher import Matcher
 from nonebot.adapters.qq import MessageEvent, Message, MessageSegment
 
 
-def initializer(main: type[Matcher]) -> AdapterMethod:
+def initializer(main: type[Matcher]) -> Adapter:
 
-    method = AdapterMethod()
+    adapter = Adapter()
 
-    @method.send("text")
+    @adapter.send("text")
     async def _(message: str):
         """发送纯文本"""
         await main.send(message)
 
-    @method.send("image_url")
+    @adapter.send("image_url")
     async def _(message: str, main: type[Matcher]):
         """发送图片"""
         await main.send(MessageSegment.image(message))
 
-    @method.send("image")
+    @adapter.send("image")
     async def _(message: BytesIO, main: type[Matcher]):
         """发送图片"""
         await main.send(MessageSegment.file_image(message))
 
-    @method.send("list")
+    @adapter.send("list")
     async def _(message: list[Result], main: type[Matcher]):
         """发送图片文本混合信息"""
         msg = Message()
         for seg in message:
             if seg.send_method == "text":
                 msg += seg.data
             elif seg.send_method == "image":
                 msg += MessageSegment.image(seg.data)
         await main.send(msg)
 
-    @method.send("segmented")
+    @adapter.send("segmented")
     async def _(message: AsyncGenerator[Result, None]):
         """发送分段信息"""
         async for seg in message:
-            await method.send_dict[seg.send_method](seg.data)
+            await adapter.send_dict[seg.send_method](seg.data)
 
-    @method.kwarg("user_id")
+    @adapter.kwarg("user_id")
     async def _(event: MessageEvent):
         return event.get_user_id()
 
-    @method.kwarg("group_id")
+    @adapter.kwarg("group_id")
     async def _(event: MessageEvent):
         return getattr(event, "group_id", getattr(event, "guild_id", None))
 
-    return method
+    return adapter
```

### Comparing `nonebot_plugin_clovers-0.1.2.post3/pyproject.toml` & `nonebot_plugin_clovers-0.1.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 [tool.poetry]
 name = "nonebot-plugin-clovers"
-version = "0.1.2r3"
+version = "0.1.3"
 description = ""
 authors = ["KarisAya <1048827424@qq.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 nonebot2 = "^2.2.1"
-clovers = "^0.1.4.post1"
+pydantic = "^2.7.1"
+clovers = "^0.1.5"
 nonebot-adapter-onebot = {version = "^2.4.3", optional = true}
 nonebot-adapter-qq = {version = "^1.4.3", optional = true}
 
 
 [tool.poetry.extras]
 onebot = ["nonebot-adapter-onebot",]
 qq = ["nonebot-adapter-qq",]
```

### Comparing `nonebot_plugin_clovers-0.1.2.post3/README.md` & `nonebot_plugin_clovers-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_clovers-0.1.2.post3/PKG-INFO` & `nonebot_plugin_clovers-0.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-clovers
-Version: 0.1.2.post3
+Version: 0.1.3
 Summary: 
 Author: KarisAya
 Author-email: 1048827424@qq.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: onebot
 Provides-Extra: qq
-Requires-Dist: clovers (>=0.1.4.post1,<0.2.0)
+Requires-Dist: clovers (>=0.1.5,<0.2.0)
 Requires-Dist: nonebot-adapter-onebot (>=2.4.3,<3.0.0) ; extra == "onebot"
 Requires-Dist: nonebot-adapter-qq (>=1.4.3,<2.0.0) ; extra == "qq"
 Requires-Dist: nonebot2 (>=2.2.1,<3.0.0)
+Requires-Dist: pydantic (>=2.7.1,<3.0.0)
 Description-Content-Type: text/markdown
 
 <p align="center">
   <a href="https://v2.nonebot.dev/"><img src="https://v2.nonebot.dev/logo.png" width="200" height="200" alt="nonebot"></a>
 </p>
 <div align="center">
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-clovers Version: 0.1.2.post3
-Summary: Author: KarisAya Author-email: 1048827424@qq.com Requires-Python:
->=3.10,<4.0 Classifier: Programming Language :: Python :: 3 Classifier:
-Programming Language :: Python :: 3.10 Classifier: Programming Language ::
-Python :: 3.11 Provides-Extra: onebot Provides-Extra: qq Requires-Dist: clovers
-(>=0.1.4.post1,<0.2.0) Requires-Dist: nonebot-adapter-onebot (>=2.4.3,<3.0.0) ;
-extra == "onebot" Requires-Dist: nonebot-adapter-qq (>=1.4.3,<2.0.0) ; extra ==
-"qq" Requires-Dist: nonebot2 (>=2.2.1,<3.0.0) Description-Content-Type: text/
-markdown
+Metadata-Version: 2.1 Name: nonebot-plugin-clovers Version: 0.1.3 Summary:
+Author: KarisAya Author-email: 1048827424@qq.com Requires-Python: >=3.10,<4.0
+Classifier: Programming Language :: Python :: 3 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: onebot Provides-Extra: qq Requires-Dist: clovers
+(>=0.1.5,<0.2.0) Requires-Dist: nonebot-adapter-onebot (>=2.4.3,<3.0.0) ; extra
+== "onebot" Requires-Dist: nonebot-adapter-qq (>=1.4.3,<2.0.0) ; extra == "qq"
+Requires-Dist: nonebot2 (>=2.2.1,<3.0.0) Requires-Dist: pydantic
+(>=2.7.1,<3.0.0) Description-Content-Type: text/markdown
                                    _[_n_o_n_e_b_o_t_]
         # nonebot_plugin_clovers[python]_[_l_i_c_e_n_s_e_]_[_p_y_p_i_]_[_p_y_p_i_ _d_o_w_n_l_o_a_d_]
 ## ð¿ å®è£ æ¨èä½¿ç¨ nb-cli å®è£ å¨ nonebot2
 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡, è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ ```bash nb
 plugin install nonebot_plugin_clovers ``` ä½¿ç¨åç®¡çå¨å®è£ pip ```bash
 pip install nonebot_plugin_clovers ``` poetry ```bash poetry add
 nonebot_plugin_clovers ``` æå¼ nonebot2 é¡¹ç®æ ¹ç®å½ä¸ç
```


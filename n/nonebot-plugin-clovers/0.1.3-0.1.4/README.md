# Comparing `tmp/nonebot_plugin_clovers-0.1.3.tar.gz` & `tmp/nonebot_plugin_clovers-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_clovers-0.1.3.tar", max compression
+gzip compressed data, was "nonebot_plugin_clovers-0.1.4.tar", max compression
```

## Comparing `nonebot_plugin_clovers-0.1.3.tar` & `nonebot_plugin_clovers-0.1.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1086 2024-04-15 11:49:16.312798 nonebot_plugin_clovers-0.1.3/LICENSE
--rw-r--r--   0        0        0     2778 2024-04-25 16:26:30.767928 nonebot_plugin_clovers-0.1.3/nonebot_plugin_clovers/__init__.py
--rw-r--r--   0        0        0      843 2024-04-25 15:59:33.461893 nonebot_plugin_clovers-0.1.3/nonebot_plugin_clovers/adapters/main.py
--rw-r--r--   0        0        0     4241 2024-04-25 16:04:21.704665 nonebot_plugin_clovers-0.1.3/nonebot_plugin_clovers/adapters/onebot/v11.py
--rw-r--r--   0        0        0     1724 2024-04-25 16:00:47.948721 nonebot_plugin_clovers-0.1.3/nonebot_plugin_clovers/adapters/qq.py
--rw-r--r--   0        0        0      365 2024-04-20 03:23:59.271766 nonebot_plugin_clovers-0.1.3/nonebot_plugin_clovers/config.py
--rw-r--r--   0        0        0      570 2024-04-25 16:26:29.280518 nonebot_plugin_clovers-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     2514 2024-04-15 11:57:25.353441 nonebot_plugin_clovers-0.1.3/README.md
--rw-r--r--   0        0        0     3065 1970-01-01 00:00:00.000000 nonebot_plugin_clovers-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1086 2024-04-15 11:49:16.312798 nonebot_plugin_clovers-0.1.4/LICENSE
+-rw-r--r--   0        0        0     3317 2024-04-25 17:12:21.573796 nonebot_plugin_clovers-0.1.4/nonebot_plugin_clovers/__init__.py
+-rw-r--r--   0        0        0      843 2024-04-25 15:59:33.461893 nonebot_plugin_clovers-0.1.4/nonebot_plugin_clovers/adapters/main.py
+-rw-r--r--   0        0        0     4241 2024-04-25 16:04:21.704665 nonebot_plugin_clovers-0.1.4/nonebot_plugin_clovers/adapters/onebot/v11.py
+-rw-r--r--   0        0        0     1724 2024-04-25 16:00:47.948721 nonebot_plugin_clovers-0.1.4/nonebot_plugin_clovers/adapters/qq.py
+-rw-r--r--   0        0        0      365 2024-04-25 17:15:05.004223 nonebot_plugin_clovers-0.1.4/nonebot_plugin_clovers/config.py
+-rw-r--r--   0        0        0      570 2024-04-25 16:56:39.551479 nonebot_plugin_clovers-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     2514 2024-04-15 11:57:25.353441 nonebot_plugin_clovers-0.1.4/README.md
+-rw-r--r--   0        0        0     3065 1970-01-01 00:00:00.000000 nonebot_plugin_clovers-0.1.4/PKG-INFO
```

### Comparing `nonebot_plugin_clovers-0.1.3/LICENSE` & `nonebot_plugin_clovers-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_clovers-0.1.3/nonebot_plugin_clovers/__init__.py` & `nonebot_plugin_clovers-0.1.4/nonebot_plugin_clovers/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -66,19 +66,32 @@
         if await clovers.response(adapter_key, command, bot=bot, event=event):
             matcher.stop_propagation()
 
 
 using_adapters = config_data.using_adapters
 
 
-if "nonebot.adapters.qq" in using_adapters:
-    from .adapters import qq
-    from nonebot.adapters.qq import Bot, MessageEvent
+flag_name = lambda flag: "成功！" if flag else "失败..."
 
-    add_response(Bot, MessageEvent, qq.initializer(main), "QQ")
+if "nonebot.adapters.qq" in using_adapters:
+    flag = True
+    try:
+        from .adapters import qq
+        from nonebot.adapters.qq import Bot, MessageEvent
+    except ModuleNotFoundError:
+        logger.error("nonebot.adapters.qq 加载失败...")
+        flag = False
+    if flag:
+        add_response(Bot, MessageEvent, qq.initializer(main), "QQ")
+        logger.success("nonebot.adapters.qq 加载成功！")
 
 if "nonebot.adapters.onebot.v11" in using_adapters:
-
-    from .adapters.onebot import v11
-    from nonebot.adapters.onebot.v11 import Bot, MessageEvent
-
-    add_response(Bot, MessageEvent, v11.initializer(main), "onebot.v11".upper())
+    flag = True
+    try:
+        from .adapters.onebot import v11
+        from nonebot.adapters.onebot.v11 import Bot, MessageEvent
+    except ModuleNotFoundError:
+        flag = False
+        logger.error("nonebot.adapters.onebot.v11 加载失败...")
+    if flag:
+        add_response(Bot, MessageEvent, v11.initializer(main), "onebot.v11".upper())
+        logger.success("nonebot.adapters.onebot.v11 加载成功！")
```

### Comparing `nonebot_plugin_clovers-0.1.3/nonebot_plugin_clovers/adapters/main.py` & `nonebot_plugin_clovers-0.1.4/nonebot_plugin_clovers/adapters/main.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_clovers-0.1.3/nonebot_plugin_clovers/adapters/onebot/v11.py` & `nonebot_plugin_clovers-0.1.4/nonebot_plugin_clovers/adapters/onebot/v11.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_clovers-0.1.3/nonebot_plugin_clovers/adapters/qq.py` & `nonebot_plugin_clovers-0.1.4/nonebot_plugin_clovers/adapters/qq.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_clovers-0.1.3/pyproject.toml` & `nonebot_plugin_clovers-0.1.4/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-clovers"
-version = "0.1.3"
+version = "0.1.4"
 description = ""
 authors = ["KarisAya <1048827424@qq.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 nonebot2 = "^2.2.1"
```

### Comparing `nonebot_plugin_clovers-0.1.3/README.md` & `nonebot_plugin_clovers-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_clovers-0.1.3/PKG-INFO` & `nonebot_plugin_clovers-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-clovers
-Version: 0.1.3
+Version: 0.1.4
 Summary: 
 Author: KarisAya
 Author-email: 1048827424@qq.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-clovers Version: 0.1.3 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-clovers Version: 0.1.4 Summary:
 Author: KarisAya Author-email: 1048827424@qq.com Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: onebot Provides-Extra: qq Requires-Dist: clovers
 (>=0.1.5,<0.2.0) Requires-Dist: nonebot-adapter-onebot (>=2.4.3,<3.0.0) ; extra
 == "onebot" Requires-Dist: nonebot-adapter-qq (>=1.4.3,<2.0.0) ; extra == "qq"
 Requires-Dist: nonebot2 (>=2.2.1,<3.0.0) Requires-Dist: pydantic
```


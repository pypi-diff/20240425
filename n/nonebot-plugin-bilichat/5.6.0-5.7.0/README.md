# Comparing `tmp/nonebot_plugin_bilichat-5.6.0.tar.gz` & `tmp/nonebot_plugin_bilichat-5.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_bilichat-5.6.0.tar", last modified: Thu Apr 18 05:50:07 2024, max compression
+gzip compressed data, was "nonebot_plugin_bilichat-5.7.0.tar", last modified: Thu Apr 25 13:14:17 2024, max compression
```

## Comparing `nonebot_plugin_bilichat-5.6.0.tar` & `nonebot_plugin_bilichat-5.7.0.tar`

### file list

```diff
@@ -1,80 +1,81 @@
--rw-r--r--   0        0        0    34523 2024-04-18 05:50:04.069064 nonebot_plugin_bilichat-5.6.0/LICENSE
--rw-r--r--   0        0        0    17907 2024-04-18 05:50:04.069064 nonebot_plugin_bilichat-5.6.0/README.md
--rw-r--r--   0        0        0     2674 2024-04-18 05:50:04.089064 nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/__init__.py
--rw-r--r--   0        0        0     1120 2024-04-18 05:50:04.089064 nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/api/__init__.py
--rw-r--r--   0        0        0      740 2024-04-18 05:50:04.089064 nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/api/base.py
--rw-r--r--   0        0        0     2232 2024-04-18 05:50:04.089064 nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/api/bilibili_auth.py
--rw-r--r--   0        0        0     1656 2024-04-18 05:50:04.089064 nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/api/subs_config.py
--rw-r--r--   0        0        0     2686 2024-04-18 05:50:04.089064 nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/api/webui.py
--rw-r--r--   0        0        0     8214 2024-04-18 05:50:04.089064 nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/base_content_parsing.py
--rw-r--r--   0        0        0       60 2024-04-18 05:50:04.089064 nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/commands/__init__.py
--rw-r--r--   0        0        0     1311 2024-04-18 05:50:04.089064 nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/commands/auto_delete_subs.py
--rw-r--r--   0        0        0     1063 2024-04-18 05:50:04.089064 nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/commands/base.py
--rw-r--r--   0        0        0      942 2024-04-18 05:50:04.089064 nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/commands/functions.py
--rw-r--r--   0        0        0     3848 2024-04-18 05:50:04.089064 nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/commands/login.py
--rw-r--r--   0        0        0     5230 2024-04-18 05:50:04.089064 nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/commands/subs.py
--rw-r--r--   0        0        0     4996 2024-04-18 05:50:04.089064 nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/commands/subs_cfg.py
--rw-r--r--   0        0        0     9273 2024-04-18 05:50:04.089064 nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/config.py
--rw-r--r--   0        0        0       81 2024-04-18 05:50:04.089064 nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/content/__init__.py
--rw-r--r--   0        0        0     3166 2024-04-18 05:50:04.089064 nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/content/column.py
--rw-r--r--   0        0        0     4233 2024-04-18 05:50:04.089064 nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/content/dynamic.py
--rw-r--r--   0        0        0     3942 2024-04-18 05:50:04.089064 nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/content/video.py
--rw-r--r--   0        0        0      518 2024-04-18 05:50:04.089064 nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/lib/b23_extract.py
--rw-r--r--   0        0        0     6192 2024-04-18 05:50:04.089064 nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/lib/bcut_asr.py
--rw-r--r--   0        0        0      506 2024-04-18 05:50:04.089064 nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/lib/bilibili_request/__init__.py
--rw-r--r--   0        0        0     2406 2024-04-18 05:50:04.089064 nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/lib/bilibili_request/auth.py
--rw-r--r--   0        0        0      966 2024-04-18 05:50:04.089064 nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/lib/bilibili_request/gRPC.py
--rw-r--r--   0        0        0     2653 2024-04-18 05:50:04.089064 nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/lib/bilibili_request/restAPI.py
--rw-r--r--   0        0        0     2657 2024-04-18 05:50:04.089064 nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/lib/browser.py
--rw-r--r--   0        0        0      456 2024-04-18 05:50:04.089064 nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/lib/cache/__init__.py
--rw-r--r--   0        0        0      437 2024-04-18 05:50:04.089064 nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/lib/cache/cache.py
--rw-r--r--   0        0        0      871 2024-04-18 05:50:04.089064 nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/lib/cache/json_cache.py
--rw-r--r--   0        0        0      531 2024-04-18 05:50:04.089064 nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/lib/cache/mongo_cache.py
--rw-r--r--   0        0        0      521 2024-04-18 05:50:04.089064 nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/lib/draw/__init__.py
--rw-r--r--   0        0        0      217 2024-04-18 05:50:04.089064 nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/lib/draw/column/__init__.py
--rw-r--r--   0        0        0     3262 2024-04-18 05:50:04.089064 nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/lib/draw/column/browser_shot.py
--rw-r--r--   0        0        0      220 2024-04-18 05:50:04.089064 nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/lib/draw/dynamic/__init__.py
--rw-r--r--   0        0        0     5145 2024-04-18 05:50:04.089064 nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/lib/draw/dynamic/browser_shot.py
--rw-r--r--   0        0        0     1160 2024-04-18 05:50:04.089064 nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/lib/draw/dynamic/dynamicrender.py
--rw-r--r--   0        0        0     7333 2024-04-18 05:50:04.089064 nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/lib/draw/video/__init__.py
--rw-r--r--   0        0        0     6326 2024-04-18 05:50:04.089064 nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/lib/draw/video/bbot_default.py
--rw-r--r--   0        0        0     3040 2024-04-18 05:50:04.093064 nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/lib/draw/video/style_blue.py
--rw-r--r--   0        0        0     3796 2024-04-18 05:50:04.093064 nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/lib/fetch_dynamic.py
--rw-r--r--   0        0        0     3376 2024-04-18 05:50:04.093064 nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/lib/fonts_provider.py
--rw-r--r--   0        0        0      525 2024-04-18 05:50:04.093064 nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/lib/store.py
--rw-r--r--   0        0        0     3115 2024-04-18 05:50:04.093064 nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/lib/strings.py
--rw-r--r--   0        0        0     3329 2024-04-18 05:50:04.093064 nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/lib/text_to_image.py
--rw-r--r--   0        0        0     1732 2024-04-18 05:50:04.093064 nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/lib/tools.py
--rw-r--r--   0        0        0     1788 2024-04-18 05:50:04.093064 nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/lib/uid_extract.py
--rw-r--r--   0        0        0     4033 2024-04-18 05:50:04.093064 nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/lib/video_subtitle.py
--rw-r--r--   0        0        0      568 2024-04-18 05:50:04.093064 nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/model/api/__init__.py
--rw-r--r--   0        0        0      184 2024-04-18 05:50:04.093064 nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/model/api/bilibili_auth.py
--rw-r--r--   0        0        0      833 2024-04-18 05:50:04.093064 nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/model/api/subs_config.py
--rw-r--r--   0        0        0      532 2024-04-18 05:50:04.093064 nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/model/arguments.py
--rw-r--r--   0        0        0     3019 2024-04-18 05:50:04.093064 nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/model/bcut_asr.py
--rw-r--r--   0        0        0     1326 2024-04-18 05:50:04.093064 nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/model/bilibili/live.py
--rw-r--r--   0        0        0     1040 2024-04-18 05:50:04.093064 nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/model/bilibili/summary.py
--rw-r--r--   0        0        0     1163 2024-04-18 05:50:04.093064 nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/model/exception.py
--rw-r--r--   0        0        0      323 2024-04-18 05:50:04.093064 nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/model/openai.py
--rw-r--r--   0        0        0      270 2024-04-18 05:50:04.093064 nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/optional.py
--rw-r--r--   0        0        0     9390 2024-04-18 05:50:04.093064 nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/static/browser/mobile_style.js
--rw-r--r--   0        0        0     1187 2024-04-18 05:50:04.093064 nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/static/style_blue/assets/business.png
--rw-r--r--   0        0        0     1200 2024-04-18 05:50:04.093064 nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/static/style_blue/assets/personal.png
--rw-r--r--   0        0        0    93905 2024-04-18 05:50:04.093064 nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/static/style_blue/assets/video_bottom.png
--rw-r--r--   0        0        0     7545 2024-04-18 05:50:04.093064 nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/static/style_blue/video-details.html
--rw-r--r--   0        0        0     5777 2024-04-18 05:50:04.093064 nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/static/summary/bilibili.png
--rw-r--r--   0        0        0     2098 2024-04-18 05:50:04.093064 nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/static/summary/index.html
--rw-r--r--   0        0        0    47433 2024-04-18 05:50:04.093064 nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/static/summary/marked.min.js
--rw-r--r--   0        0        0    59199 2024-04-18 05:50:04.093064 nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/static/summary/openai.png
--rw-r--r--   0        0        0     9556 2024-04-18 05:50:04.093064 nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/static/upload-webui.html
--rw-r--r--   0        0        0   300664 2024-04-18 05:50:04.093064 nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/static/webui.tar.gz
--rw-r--r--   0        0        0     3111 2024-04-18 05:50:04.093064 nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/subscribe/__init__.py
--rw-r--r--   0        0        0     7217 2024-04-18 05:50:04.093064 nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/subscribe/dynamic.py
--rw-r--r--   0        0        0     4023 2024-04-18 05:50:04.093064 nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/subscribe/live.py
--rw-r--r--   0        0        0    15841 2024-04-18 05:50:04.093064 nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/subscribe/manager.py
--rw-r--r--   0        0        0      478 2024-04-18 05:50:04.093064 nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/summary/__init__.py
--rw-r--r--   0        0        0     4931 2024-04-18 05:50:04.093064 nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/summary/openai.py
--rw-r--r--   0        0        0     2268 2024-04-18 05:50:04.093064 nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/summary/openai_summarise.py
--rw-r--r--   0        0        0     1615 2024-04-18 05:50:04.093064 nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/wordcloud.py
--rw-r--r--   0        0        0     1754 2024-04-18 05:50:07.745081 nonebot_plugin_bilichat-5.6.0/pyproject.toml
--rw-r--r--   0        0        0    19602 1970-01-01 00:00:00.000000 nonebot_plugin_bilichat-5.6.0/PKG-INFO
+-rw-r--r--   0        0        0    34523 2024-04-25 13:14:11.917305 nonebot_plugin_bilichat-5.7.0/LICENSE
+-rw-r--r--   0        0        0    17907 2024-04-25 13:14:11.917305 nonebot_plugin_bilichat-5.7.0/README.md
+-rw-r--r--   0        0        0     2718 2024-04-25 13:14:11.937305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/__init__.py
+-rw-r--r--   0        0        0     1120 2024-04-25 13:14:11.937305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/api/__init__.py
+-rw-r--r--   0        0        0      740 2024-04-25 13:14:11.937305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/api/base.py
+-rw-r--r--   0        0        0     2176 2024-04-25 13:14:11.937305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/api/bilibili_auth.py
+-rw-r--r--   0        0        0     1622 2024-04-25 13:14:11.937305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/api/subs_config.py
+-rw-r--r--   0        0        0     2655 2024-04-25 13:14:11.937305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/api/webui.py
+-rw-r--r--   0        0        0     7996 2024-04-25 13:14:11.937305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/base_content_parsing.py
+-rw-r--r--   0        0        0       60 2024-04-25 13:14:11.937305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/commands/__init__.py
+-rw-r--r--   0        0        0     1280 2024-04-25 13:14:11.937305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/commands/auto_delete_subs.py
+-rw-r--r--   0        0        0     1063 2024-04-25 13:14:11.937305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/commands/base.py
+-rw-r--r--   0        0        0      942 2024-04-25 13:14:11.937305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/commands/functions.py
+-rw-r--r--   0        0        0     3848 2024-04-25 13:14:11.937305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/commands/login.py
+-rw-r--r--   0        0        0     5196 2024-04-25 13:14:11.937305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/commands/subs.py
+-rw-r--r--   0        0        0     4996 2024-04-25 13:14:11.941305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/commands/subs_cfg.py
+-rw-r--r--   0        0        0     9227 2024-04-25 13:14:11.941305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/config.py
+-rw-r--r--   0        0        0       81 2024-04-25 13:14:11.941305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/content/__init__.py
+-rw-r--r--   0        0        0     3130 2024-04-25 13:14:11.941305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/content/column.py
+-rw-r--r--   0        0        0     4227 2024-04-25 13:14:11.941305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/content/dynamic.py
+-rw-r--r--   0        0        0     3958 2024-04-25 13:14:11.941305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/content/video.py
+-rw-r--r--   0        0        0      494 2024-04-25 13:14:11.941305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/lib/b23_extract.py
+-rw-r--r--   0        0        0     6142 2024-04-25 13:14:11.941305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/lib/bcut_asr.py
+-rw-r--r--   0        0        0      506 2024-04-25 13:14:11.941305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/lib/bilibili_request/__init__.py
+-rw-r--r--   0        0        0     2346 2024-04-25 13:14:11.941305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/lib/bilibili_request/auth.py
+-rw-r--r--   0        0        0      966 2024-04-25 13:14:11.941305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/lib/bilibili_request/gRPC.py
+-rw-r--r--   0        0        0     2653 2024-04-25 13:14:11.941305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/lib/bilibili_request/restAPI.py
+-rw-r--r--   0        0        0     2657 2024-04-25 13:14:11.941305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/lib/browser.py
+-rw-r--r--   0        0        0      456 2024-04-25 13:14:11.941305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/lib/cache/__init__.py
+-rw-r--r--   0        0        0      366 2024-04-25 13:14:11.941305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/lib/cache/cache.py
+-rw-r--r--   0        0        0      871 2024-04-25 13:14:11.941305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/lib/cache/json_cache.py
+-rw-r--r--   0        0        0      531 2024-04-25 13:14:11.941305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/lib/cache/mongo_cache.py
+-rw-r--r--   0        0        0      521 2024-04-25 13:14:11.941305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/lib/draw/__init__.py
+-rw-r--r--   0        0        0      217 2024-04-25 13:14:11.941305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/lib/draw/column/__init__.py
+-rw-r--r--   0        0        0     3262 2024-04-25 13:14:11.941305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/lib/draw/column/browser_shot.py
+-rw-r--r--   0        0        0      220 2024-04-25 13:14:11.941305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/lib/draw/dynamic/__init__.py
+-rw-r--r--   0        0        0     5145 2024-04-25 13:14:11.941305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/lib/draw/dynamic/browser_shot.py
+-rw-r--r--   0        0        0     1136 2024-04-25 13:14:11.941305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/lib/draw/dynamic/dynamicrender.py
+-rw-r--r--   0        0        0     7275 2024-04-25 13:14:11.941305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/lib/draw/video/__init__.py
+-rw-r--r--   0        0        0     6326 2024-04-25 13:14:11.941305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/lib/draw/video/bbot_default.py
+-rw-r--r--   0        0        0     3040 2024-04-25 13:14:11.941305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/lib/draw/video/style_blue.py
+-rw-r--r--   0        0        0     3187 2024-04-25 13:14:11.941305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/lib/fetch_dynamic.py
+-rw-r--r--   0        0        0     3376 2024-04-25 13:14:11.941305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/lib/fonts_provider.py
+-rw-r--r--   0        0        0      525 2024-04-25 13:14:11.941305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/lib/store.py
+-rw-r--r--   0        0        0     3091 2024-04-25 13:14:11.941305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/lib/strings.py
+-rw-r--r--   0        0        0     3329 2024-04-25 13:14:11.941305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/lib/text_to_image.py
+-rw-r--r--   0        0        0     1701 2024-04-25 13:14:11.941305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/lib/tools.py
+-rw-r--r--   0        0        0     1739 2024-04-25 13:14:11.941305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/lib/uid_extract.py
+-rw-r--r--   0        0        0     3988 2024-04-25 13:14:11.941305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/lib/video_subtitle.py
+-rw-r--r--   0        0        0      552 2024-04-25 13:14:11.941305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/model/api/__init__.py
+-rw-r--r--   0        0        0      184 2024-04-25 13:14:11.941305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/model/api/bilibili_auth.py
+-rw-r--r--   0        0        0      809 2024-04-25 13:14:11.941305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/model/api/subs_config.py
+-rw-r--r--   0        0        0      532 2024-04-25 13:14:11.941305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/model/arguments.py
+-rw-r--r--   0        0        0     2988 2024-04-25 13:14:11.941305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/model/bcut_asr.py
+-rw-r--r--   0        0        0     1326 2024-04-25 13:14:11.941305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/model/bilibili/live.py
+-rw-r--r--   0        0        0     1016 2024-04-25 13:14:11.941305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/model/bilibili/summary.py
+-rw-r--r--   0        0        0      596 2024-04-25 13:14:11.941305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/model/const.py
+-rw-r--r--   0        0        0     1163 2024-04-25 13:14:11.941305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/model/exception.py
+-rw-r--r--   0        0        0      291 2024-04-25 13:14:11.941305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/model/openai.py
+-rw-r--r--   0        0        0      270 2024-04-25 13:14:11.941305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/optional.py
+-rw-r--r--   0        0        0     9390 2024-04-25 13:14:11.941305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/static/browser/mobile_style.js
+-rw-r--r--   0        0        0     1187 2024-04-25 13:14:11.941305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/static/style_blue/assets/business.png
+-rw-r--r--   0        0        0     1200 2024-04-25 13:14:11.941305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/static/style_blue/assets/personal.png
+-rw-r--r--   0        0        0    93905 2024-04-25 13:14:11.941305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/static/style_blue/assets/video_bottom.png
+-rw-r--r--   0        0        0     7545 2024-04-25 13:14:11.941305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/static/style_blue/video-details.html
+-rw-r--r--   0        0        0     5777 2024-04-25 13:14:11.941305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/static/summary/bilibili.png
+-rw-r--r--   0        0        0     2098 2024-04-25 13:14:11.941305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/static/summary/index.html
+-rw-r--r--   0        0        0    47433 2024-04-25 13:14:11.941305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/static/summary/marked.min.js
+-rw-r--r--   0        0        0    59199 2024-04-25 13:14:11.941305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/static/summary/openai.png
+-rw-r--r--   0        0        0     9556 2024-04-25 13:14:11.941305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/static/upload-webui.html
+-rw-r--r--   0        0        0   300664 2024-04-25 13:14:11.941305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/static/webui.tar.gz
+-rw-r--r--   0        0        0     3111 2024-04-25 13:14:11.945305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/subscribe/__init__.py
+-rw-r--r--   0        0        0     7187 2024-04-25 13:14:11.945305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/subscribe/dynamic.py
+-rw-r--r--   0        0        0     4023 2024-04-25 13:14:11.945305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/subscribe/live.py
+-rw-r--r--   0        0        0    15592 2024-04-25 13:14:11.945305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/subscribe/manager.py
+-rw-r--r--   0        0        0      478 2024-04-25 13:14:11.945305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/summary/__init__.py
+-rw-r--r--   0        0        0     4894 2024-04-25 13:14:11.945305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/summary/openai.py
+-rw-r--r--   0        0        0     2243 2024-04-25 13:14:11.945305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/summary/openai_summarise.py
+-rw-r--r--   0        0        0     1578 2024-04-25 13:14:11.945305 nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/wordcloud.py
+-rw-r--r--   0        0        0     1755 2024-04-25 13:14:17.689287 nonebot_plugin_bilichat-5.7.0/pyproject.toml
+-rw-r--r--   0        0        0    19603 1970-01-01 00:00:00.000000 nonebot_plugin_bilichat-5.7.0/PKG-INFO
```

### Comparing `nonebot_plugin_bilichat-5.6.0/LICENSE` & `nonebot_plugin_bilichat-5.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.6.0/README.md` & `nonebot_plugin_bilichat-5.7.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -186,25 +186,25 @@
 
 ### 指令配置项
 
 |          配置项           |   类型    |          默认值          |           说明            |
 | :-----------------------: | :-------: | :----------------------: | :-----------------------: |
 |  bilichat_command_to_me   |   bool    |           True           |    命令是否需要@机器人    |
 |    bilichat_cmd_start     |    str    |        "bilichat"        | 命令的起始词，可设置为空  |
-|   bilichat_cmd_add_sub    | List[str] |     ["订阅", "关注"]     |      "sub"命令的别名      |
-|  bilichat_cmd_remove_sub  | List[str] |     ["退订", "取关"]     |     "unsub"命令的别名     |
-|  bilichat_cmd_check_sub   | List[str] |   ["查看", "查看订阅"]   |     "check"命令的别名     |
-|  bilichat_cmd_reset_sub   | List[str] |   ["重置", "重置配置"]   |     "reset"命令的别名     |
-|    bilichat_cmd_at_all    | List[str] | ["全体成员", "at 全体"]  |     "atall"命令的别名     |
-|   bilichat_cmd_dynamic    | List[str] | ["动态通知", "动态订阅"] |    "dynamic"命令的别名    |
-|     bilichat_cmd_live     | List[str] | ["直播通知", "直播订阅"] |     "live"命令的别名      |
-| bilichat_cmd_checkdynamic | List[str] |       ["查看动态"]       | "checkdynamic" 命令的别名 |
-| bilichat_cmd_check_login  | List[str] |     ["查看登录账号"]     |  "checklogin" 命令的别名  |
-| bilichat_cmd_login_qrcode | List[str] |       ["扫码登录"]       |   "qrlogin" 命令的别名    |
-|    bilichat_cmd_logout    | List[str] |       ["登出账号"]       |    "logout" 命令的别名    |
+|   bilichat_cmd_add_sub    | list[str] |     ["订阅", "关注"]     |      "sub"命令的别名      |
+|  bilichat_cmd_remove_sub  | list[str] |     ["退订", "取关"]     |     "unsub"命令的别名     |
+|  bilichat_cmd_check_sub   | list[str] |   ["查看", "查看订阅"]   |     "check"命令的别名     |
+|  bilichat_cmd_reset_sub   | list[str] |   ["重置", "重置配置"]   |     "reset"命令的别名     |
+|    bilichat_cmd_at_all    | list[str] | ["全体成员", "at 全体"]  |     "atall"命令的别名     |
+|   bilichat_cmd_dynamic    | list[str] | ["动态通知", "动态订阅"] |    "dynamic"命令的别名    |
+|     bilichat_cmd_live     | list[str] | ["直播通知", "直播订阅"] |     "live"命令的别名      |
+| bilichat_cmd_checkdynamic | list[str] |       ["查看动态"]       | "checkdynamic" 命令的别名 |
+| bilichat_cmd_check_login  | list[str] |     ["查看登录账号"]     |  "checklogin" 命令的别名  |
+| bilichat_cmd_login_qrcode | list[str] |       ["扫码登录"]       |   "qrlogin" 命令的别名    |
+|    bilichat_cmd_logout    | list[str] |       ["登出账号"]       |    "logout" 命令的别名    |
 
 ### 基础信息配置项
 
 |            配置项            | 类型 | 默认值 |                        说明                        |
 | :--------------------------: | :--: | :----: | :------------------------------------------------: |
 |     bilichat_basic_info      | bool |  True  |                是否开启视频基本信息                |
 |  bilichat_basic_info_style   | str  |  Auto  |       视频详情的图片样式，可用样式见下方备注       |
@@ -256,15 +256,15 @@
 ### 词云配置项
 
 开启此功能需要安装对应的依赖 `nonebot-plugin-bilichat[wordcloud]`
 
 |          配置项          |   类型    |   默认值    |       说明       |
 | :----------------------: | :-------: | :---------: | :--------------: |
 |   bilichat_word_cloud    |   bool    |    False    | 是否开启词云功能 |
-| bilichat_word_cloud_size | List[int] | [1000, 800] |   词云图片尺寸   |
+| bilichat_word_cloud_size | list[int] | [1000, 800] |   词云图片尺寸   |
 
 ### AI 视频总结配置项
 
 开启此功能需要安装对应的依赖 `nonebot-plugin-bilichat[summary]`
 
 |            配置项            | 类型 |       默认值       |                                      说明                                      |
 | :--------------------------: | :--: | :----------------: | :----------------------------------------------------------------------------: |
```

#### html2text {}

```diff
@@ -72,28 +72,28 @@
 æ¬¡æ°æå åéåéè¯æ¥å°è¯éæ°çæå­å¹ 5. å½
 `bilichat_cache_serive` ä¸º `mongodb` æ¶ï¼éè¦å®è£å¹¶éç½® [nonebot-
 plugin-mongodb](https://github.com/Well2333/nonebot-plugin-mongodb)
 æå¯æ­£å¸¸ä½¿ç¨ ### æä»¤éç½®é¡¹ | éç½®é¡¹ | ç±»å | é»è®¤å¼ |
 è¯´æ | | :-----------------------: | :-------: | :----------------------: | :
 -----------------------: | | bilichat_command_to_me | bool | True |
 å½ä»¤æ¯å¦éè¦@æºå¨äºº | | bilichat_cmd_start | str | "bilichat" |
-å½ä»¤çèµ·å§è¯ï¼å¯è®¾ç½®ä¸ºç©º | | bilichat_cmd_add_sub | List[str] |
-["è®¢é", "å³æ³¨"] | "sub"å½ä»¤çå«å | | bilichat_cmd_remove_sub | List
+å½ä»¤çèµ·å§è¯ï¼å¯è®¾ç½®ä¸ºç©º | | bilichat_cmd_add_sub | list[str] |
+["è®¢é", "å³æ³¨"] | "sub"å½ä»¤çå«å | | bilichat_cmd_remove_sub | list
 [str] | ["éè®¢", "åå³"] | "unsub"å½ä»¤çå«å | |
-bilichat_cmd_check_sub | List[str] | ["æ¥ç", "æ¥çè®¢é"] |
-"check"å½ä»¤çå«å | | bilichat_cmd_reset_sub | List[str] | ["éç½®",
-"éç½®éç½®"] | "reset"å½ä»¤çå«å | | bilichat_cmd_at_all | List[str] |
+bilichat_cmd_check_sub | list[str] | ["æ¥ç", "æ¥çè®¢é"] |
+"check"å½ä»¤çå«å | | bilichat_cmd_reset_sub | list[str] | ["éç½®",
+"éç½®éç½®"] | "reset"å½ä»¤çå«å | | bilichat_cmd_at_all | list[str] |
 ["å¨ä½æå", "at å¨ä½"] | "atall"å½ä»¤çå«å | | bilichat_cmd_dynamic
-| List[str] | ["å¨æéç¥", "å¨æè®¢é"] | "dynamic"å½ä»¤çå«å | |
-bilichat_cmd_live | List[str] | ["ç´æ­éç¥", "ç´æ­è®¢é"] |
-"live"å½ä»¤çå«å | | bilichat_cmd_checkdynamic | List[str] |
+| list[str] | ["å¨æéç¥", "å¨æè®¢é"] | "dynamic"å½ä»¤çå«å | |
+bilichat_cmd_live | list[str] | ["ç´æ­éç¥", "ç´æ­è®¢é"] |
+"live"å½ä»¤çå«å | | bilichat_cmd_checkdynamic | list[str] |
 ["æ¥çå¨æ"] | "checkdynamic" å½ä»¤çå«å | | bilichat_cmd_check_login
-| List[str] | ["æ¥çç»å½è´¦å·"] | "checklogin" å½ä»¤çå«å | |
-bilichat_cmd_login_qrcode | List[str] | ["æ«ç ç»å½"] | "qrlogin"
-å½ä»¤çå«å | | bilichat_cmd_logout | List[str] | ["ç»åºè´¦å·"] |
+| list[str] | ["æ¥çç»å½è´¦å·"] | "checklogin" å½ä»¤çå«å | |
+bilichat_cmd_login_qrcode | list[str] | ["æ«ç ç»å½"] | "qrlogin"
+å½ä»¤çå«å | | bilichat_cmd_logout | list[str] | ["ç»åºè´¦å·"] |
 "logout" å½ä»¤çå«å | ### åºç¡ä¿¡æ¯éç½®é¡¹ | éç½®é¡¹ | ç±»å |
 é»è®¤å¼ | è¯´æ | | :--------------------------: | :--: | :----: | :--------
 ----------------------------------------: | | bilichat_basic_info | bool | True
 | æ¯å¦å¼å¯è§é¢åºæ¬ä¿¡æ¯ | | bilichat_basic_info_style | str | Auto |
 è§é¢è¯¦æçå¾çæ ·å¼ï¼å¯ç¨æ ·å¼è§ä¸æ¹å¤æ³¨ | |
 bilichat_basic_info_url | bool | True |
 å¼å¯è§é¢è¿æ¬ä¿¡æ¯çæåµä¸ï¼æ¯å¦ä¸ååå¤ä¸ä¸ªé¾æ¥ | |
@@ -114,15 +114,15 @@
 bilichat_use_browser ä¸º True æ Autoï¼ï¼å¶å¯ç¨çæ ·å¼å¦ä¸æç¤º
 dynamicrender ï¼æ æµè§å¨æ¶é»è®¤ï¼ ![](docs/dynamicrender.jpg)
 browser_mobile ï¼ææµè§å¨æ¶é»è®¤ï¼ ![](docs/dynamic_mobile.jpg)
 browser_pc ![](docs/dynamic_pc.jpg) ### è¯äºéç½®é¡¹
 å¼å¯æ­¤åè½éè¦å®è£å¯¹åºçä¾èµ `nonebot-plugin-bilichat[wordcloud]`
 | éç½®é¡¹ | ç±»å | é»è®¤å¼ | è¯´æ | | :----------------------: | :-----
 --: | :---------: | :--------------: | | bilichat_word_cloud | bool | False |
-æ¯å¦å¼å¯è¯äºåè½ | | bilichat_word_cloud_size | List[int] | [1000, 800]
+æ¯å¦å¼å¯è¯äºåè½ | | bilichat_word_cloud_size | list[int] | [1000, 800]
 | è¯äºå¾çå°ºå¯¸ | ### AI è§é¢æ»ç»éç½®é¡¹
 å¼å¯æ­¤åè½éè¦å®è£å¯¹åºçä¾èµ `nonebot-plugin-bilichat[summary]` |
 éç½®é¡¹ | ç±»å | é»è®¤å¼ | è¯´æ | | :--------------------------: | :--:
 | :----------------: | :-------------------------------------------------------
 ---------------------: | | bilichat_summary_ignore_null | bool | True |
 æ¯å¦å¿½ç¥æ æä¹çæ»ç»åå®¹ | | bilichat_official_summary | bool |
 False | æ¯å¦å¼å¯å®æ¹æ»ç»ï¼æ­¤æ»ç»ç¬ç«äºä¸æ¹ AI
```

### Comparing `nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/__init__.py` & `nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from nonebot import require
 from nonebot.plugin import PluginMetadata
 
 from .config import __version__, plugin_config, raw_config
 
 require("nonebot_plugin_apscheduler")
 require("nonebot_plugin_alconna")
+require("nonebot_plugin_auto_bot_selector")
 
 cmd_perfix = f"{raw_config.command_start}{plugin_config.bilichat_cmd_start}{raw_config.command_sep}"
 
 __plugin_meta__ = PluginMetadata(
     name="nonebot-plugin-bilichat",
     description="多种B站链接解析，视频词云，AI总结，你想要的都在 bilichat",
     usage="视频、专栏、动态解析直接发送链接、小程序、xml卡片即可，指令请参考 https://github.com/Well2333/nonebot-plugin-bilichat",
```

### Comparing `nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/api/__init__.py` & `nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/api/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/api/base.py` & `nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/api/base.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/api/bilibili_auth.py` & `nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/api/bilibili_auth.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,57 +1,55 @@
-from typing import Dict, List, Union
-
 from bilireq.auth import Auth
 from bilireq.login import ResponseCodeError
 from bilireq.login.qrcode_login import get_qrcode_login_info, get_qrcode_login_result
 
 from ..lib.bilibili_request.auth import AuthManager
 from ..model.api import FaildResponse, Response
 from ..model.api.bilibili_auth import AuthInfo, Qrcode
 from .base import app
 
 
 @app.get("/api/bili_grpc_auth")
-async def list_auth() -> Response[List[AuthInfo]]:
-    return Response[List[AuthInfo]](
+async def list_auth() -> Response[list[AuthInfo]]:
+    return Response[list[AuthInfo]](
         data=[
             AuthInfo(id=auth.uid, token_expired=auth.tokens_expired, cookie_expired=auth.cookies_expired)
             for auth in AuthManager.grpc_auths
         ]
     )
 
 
 @app.post("/api/bili_grpc_auth")
-async def add_auth(raw_auth: Dict) -> Union[Response, FaildResponse]:
+async def add_auth(raw_auth: dict) -> Response | FaildResponse:
     try:
         auth = Auth(raw_auth)
         auth = await auth.refresh()
     except Exception as e:
         return FaildResponse(code=400, message=str(e))
     AuthManager.add_auth(auth)
     return Response[AuthInfo](
         data=AuthInfo(id=auth.uid, token_expired=auth.tokens_expired, cookie_expired=auth.cookies_expired),
     )
 
 
 @app.delete("/api/bili_grpc_auth")
-async def remove_auth(uid: int) -> Union[Response, FaildResponse]:
+async def remove_auth(uid: int) -> Response | FaildResponse:
     if msg := AuthManager.remove_auth(uid):
         return FaildResponse(code=404, message=msg)
     return Response(data={})
 
 
 @app.get("/api/bili_grpc_login/qrcode")
 async def generate_qrcode() -> Response[Qrcode]:
     r = await get_qrcode_login_info()
     return Response[Qrcode](data=Qrcode(qrcode_url=r["url"], auth_code=r["auth_code"]))
 
 
 @app.post("/api/bili_grpc_login/qrcode")
-async def login_by_qrcode(auth_code: str) -> Union[Response[AuthInfo], FaildResponse]:
+async def login_by_qrcode(auth_code: str) -> Response[AuthInfo] | FaildResponse:
     try:
         resp = await get_qrcode_login_result(auth_code)
         auth = Auth()
         auth.data = auth.refresh_handler(resp)
         auth = await auth.refresh()
         AuthManager.add_auth(auth)
         return Response[AuthInfo](
```

### Comparing `nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/api/subs_config.py` & `nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/api/subs_config.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from typing import Dict, List, Union
-
 import nonebot
 from nonebot.compat import model_dump
 from nonebot.log import logger
 from nonebot_plugin_auto_bot_selector.target import SupportedPlatform
 from pydantic import ValidationError
 
 from ..model.api import FaildResponse, Response
@@ -12,40 +10,40 @@
 from .base import app
 
 config = nonebot.get_driver().config
 
 
 @app.get("/api/subs_config")
 async def get_subs() -> Response[Subs]:
-    return Response[Subs](data=Subs(**SubscriptionSystem.dict()))
+    return Response[Subs](data=Subs(**SubscriptionSystem.dump_dict()))
 
 
 @app.put("/api/subs_config")
-async def update_subs(data: Subs) -> Union[Response[Subs], FaildResponse]:
+async def update_subs(data: Subs) -> Response[Subs] | FaildResponse:
     try:
         # 不接收来自前端的 uploaders，由后端自行推导并校验
         await SubscriptionSystem.load(
             model_dump(
                 data,
                 exclude={
                     "uploaders",
                 },
             )
         )
-        return Response[Subs](data=Subs(**SubscriptionSystem.dict()))
+        return Response[Subs](data=Subs(**SubscriptionSystem.dump_dict()))
     except (ValueError, ValidationError) as e:
         return FaildResponse(code=422, message=str(e))
     except Exception as e:
         logger.exception(e)
         return FaildResponse(code=400, message=str(e))
 
 
 @app.get("/api/subs_config/platform")
-async def get_supported_platform() -> Response[List[Dict[str, str]]]:
-    return Response[List[Dict[str, str]]](
+async def get_supported_platform() -> Response[list[dict[str, str]]]:
+    return Response[list[dict[str, str]]](
         data=[
             {
                 "value": SupportedPlatform.qq_group,
                 "label": "QQ群",
             },
             {
                 "value": SupportedPlatform.qq_guild_channel,
```

### Comparing `nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/api/webui.py` & `nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/api/webui.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import shutil
 import tarfile
 import tempfile
 import zipfile
 from io import BytesIO
 from pathlib import Path
-from typing import Union
 
 from fastapi import File, UploadFile
 from fastapi.responses import HTMLResponse
 from fastapi.staticfiles import StaticFiles
 from nonebot.log import logger
 from starlette.routing import Mount
 
@@ -22,15 +21,15 @@
 
 @app.get("/webui")
 async def read_html():
     return HTMLResponse(static_dir.joinpath("upload-webui.html").read_text(encoding="utf-8"))
 
 
 @app.post("/webui/update")
-async def upload_file(file: UploadFile = File(...)) -> Union[Response[None], FaildResponse]:
+async def upload_file(file: UploadFile = File(...)) -> Response[None] | FaildResponse:
     file_data = await file.read()
     filename = file.filename or ""
 
     with tempfile.TemporaryDirectory() as temp_dir:
         if filename.endswith(".zip"):
             zip_file = zipfile.ZipFile(BytesIO(file_data))
             zip_file.extractall(temp_dir)
```

### Comparing `nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/base_content_parsing.py` & `nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/base_content_parsing.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import asyncio
 import re
 import shlex
 import time
-from typing import Dict, Union
 
 from nonebot.adapters import Bot, Event
 from nonebot.exception import FinishedException
 from nonebot.log import logger
 from nonebot.plugin import on_message
 from nonebot.rule import Rule
 from nonebot.typing import T_State
@@ -22,27 +21,20 @@
 
 if plugin_config.bilichat_openai_token:
     from .summary import summarization
 
 if plugin_config.bilichat_word_cloud:
     from .wordcloud import wordcloud
 
-cd: Dict[str, int] = {}
+cd: dict[str, int] = {}
 cd_size_limit = plugin_config.bilichat_cd_time // 2
+lock = asyncio.Lock()
 
-# 临时解决方案
-try:
-    lock = asyncio.Lock()
-except RuntimeError:
-    loop = asyncio.new_event_loop()
-    asyncio.set_event_loop(loop)
-    lock = asyncio.Lock(loop=loop)  # type: ignore
 
-
-def check_cd(uid: Union[int, str], check: bool = True):
+def check_cd(uid: int | str, check: bool = True):
     global cd
     now = int(time.time())
     uid = str(uid)
     # gc
     if len(cd) > cd_size_limit:
         cd = {k: cd[k] for k in cd if cd[k] < now}
     # not check cd
@@ -103,15 +95,15 @@
             if seg in _msg_str.lower():
                 bililink = _msg_str
                 break
 
     if not bililink:
         return False
 
-    content: Union[Column, Video, Dynamic, None] = None
+    content: Column | Video | Dynamic | None = None
     options: Options = state["_options_"]
 
     try:
         ## video handle
         if matched := re.search(r"av(\d{1,15})|BV(1[A-Za-z0-9]{2}4.1.7[A-Za-z0-9]{2})", bililink):
             _id = matched.group()
             logger.info(f"video id: {_id}")
@@ -162,15 +154,15 @@
     priority=1,
     rule=Rule(_pre_check),
 )
 
 
 @bilichat.handle()
 async def content_info(event: Event, origin_msg: UniMsg, state: T_State):
-    content: Union[Column, Video, Dynamic] = state["_content_"]
+    content: Column | Video | Dynamic = state["_content_"]
     reply = Reply(id=origin_msg.get_message_id())
     if plugin_config.bilichat_basic_info:
         content_image = await content.get_image(plugin_config.bilichat_basic_info_style)
 
         msgs = UniMessage()
         msgs.append(reply)
         if content_image:
```

### Comparing `nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/commands/auto_delete_subs.py` & `nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/commands/auto_delete_subs.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from typing import Union
-
 from nonebot.log import logger
 from nonebot.plugin import on_notice
 from nonebot_plugin_alconna.uniseg import MsgTarget
 
 from ..subscribe.manager import CONFIG_LOCK, SubscriptionSystem, User
 
 auto_delete_subs = on_notice(block=False)
@@ -20,15 +18,15 @@
 
 
 try:
     from nonebot.adapters.mirai2.event import BotLeaveEventActive, BotLeaveEventDisband, BotLeaveEventKick
 
     @auto_delete_subs.handle()
     async def remove_sub_mirai2(
-        event: Union[BotLeaveEventKick, BotLeaveEventDisband, BotLeaveEventActive], target: MsgTarget
+        event: BotLeaveEventKick | BotLeaveEventDisband | BotLeaveEventActive, target: MsgTarget
     ):
         await remove_sub(target)
 
 except ImportError:
     pass
 
 try:
```

### Comparing `nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/commands/base.py` & `nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/commands/base.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/commands/functions.py` & `nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/commands/functions.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/commands/login.py` & `nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/commands/login.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/commands/subs.py` & `nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/commands/subs.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from asyncio import Lock
-from typing import Optional
 
 from nonebot.adapters import Message
 from nonebot.params import CommandArg, Depends
 from nonebot.permission import SUPERUSER
 
 from ..config import plugin_config
 from ..lib.uid_extract import uid_extract
@@ -47,15 +46,15 @@
                 re_msg = await user.remove_subscription(up) or f"已经成功取关 {up} 啦\n(*^▽^*)"
                 await bili_add_sub.finish(re_msg)
         await bili_add_sub.finish("未找到该 UP 主呢\n`(*>﹏<*)′")
 
 
 @bili_check_sub.handle()
 async def check_sub(
-    user: User = Depends(get_user), msg: Optional[Message] = CommandArg(), lock: Lock = Depends(check_lock)
+    user: User = Depends(get_user), msg: Message | None = CommandArg(), lock: Lock = Depends(check_lock)
 ):
     async with lock:
         if not user.subscriptions:
             await bili_check_sub.finish("本群并未订阅任何UP主呢...\n`(*>﹏<*)′")
         # 查看本群的订阅
         if not msg:
             ups = user.subscribe_ups
@@ -83,15 +82,15 @@
                     re_msg = "\n".join(prompt)
                     break
         await bili_check_sub.finish(re_msg)
 
 
 @bili_reset_sub.handle()
 async def reset_sub(
-    user: User = Depends(get_user), msg: Optional[Message] = CommandArg(), lock: Lock = Depends(check_lock)
+    user: User = Depends(get_user), msg: Message | None = CommandArg(), lock: Lock = Depends(check_lock)
 ):
     async with lock:
         if not msg:
             await bili_reset_sub.finish("请输入UP主的昵称或 UID 呢\n`(*>﹏<*)′")
         keyword = msg.extract_plain_text().lower()
         if keyword in ["all", "全部"]:
             for sub in user.subscriptions:
```

### Comparing `nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/commands/subs_cfg.py` & `nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/commands/subs_cfg.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/config.py` & `nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,87 +1,81 @@
 import importlib.util
 import json
-import sys
+from importlib.metadata import version
 from pathlib import Path
-from typing import List, Literal, Optional, Union
+from typing import Literal
 
 from nonebot import get_driver, get_plugin_config, require
 from nonebot.log import logger
 from pydantic import BaseModel, Field, validator
 
 from .lib.store import cache_dir
 
-# get package version
-if sys.version_info < (3, 10):
-    from importlib_metadata import version
-else:
-    from importlib.metadata import version
-
 try:
     __version__ = version("nonebot_plugin_bilichat")
 except Exception:
     __version__ = None
 
 
 class Config(BaseModel):
     # general
     bilichat_block: bool = False
     bilichat_enable_self: bool = False
     bilichat_only_self: bool = False
     bilichat_only_to_me: bool = False
-    bilichat_whitelist: List[str] = []
-    bilichat_blacklist: List[str] = []
+    bilichat_whitelist: list[str] = []
+    bilichat_blacklist: list[str] = []
     bilichat_cd_time: int = 120
     bilichat_neterror_retry: int = 3
     bilichat_show_error_msg: bool = True
     bilichat_use_browser: bool = Field(default="Auto")
     bilichat_browser_shot_quality: int = Field(default=75, ge=10, le=100)
     bilichat_cache_serive: Literal["json", "mongodb"] = Field(default="Auto")
     bilichat_text_fonts: str = "default"
     bilichat_emoji_fonts: str = "default"
-    bilichat_webui_path: Optional[str] = "bilichat"
+    bilichat_webui_path: str | None = "bilichat"
 
     # command and subscribe
     bilichat_command_to_me: bool = True
     bilichat_cmd_start: str = "bilichat"
-    bilichat_cmd_add_sub: List[str] = ["订阅", "关注"]
-    bilichat_cmd_remove_sub: List[str] = ["退订", "取关"]
-    bilichat_cmd_check_sub: List[str] = ["查看", "查看订阅"]
-    bilichat_cmd_reset_sub: List[str] = ["重置", "重置配置"]
-    bilichat_cmd_at_all: List[str] = ["全体成员", "at全体"]
-    bilichat_cmd_dynamic: List[str] = ["动态通知", "动态订阅"]
-    bilichat_cmd_live: List[str] = ["直播通知", "直播订阅"]
-    bilichat_cmd_checkdynamic: List[str] = ["查看动态"]
-    bilichat_cmd_check_login: List[str] = ["查看登录账号"]
-    bilichat_cmd_login_qrcode: List[str] = ["扫码登录"]
-    bilichat_cmd_logout: List[str] = ["登出账号"]
+    bilichat_cmd_add_sub: list[str] = ["订阅", "关注"]
+    bilichat_cmd_remove_sub: list[str] = ["退订", "取关"]
+    bilichat_cmd_check_sub: list[str] = ["查看", "查看订阅"]
+    bilichat_cmd_reset_sub: list[str] = ["重置", "重置配置"]
+    bilichat_cmd_at_all: list[str] = ["全体成员", "at全体"]
+    bilichat_cmd_dynamic: list[str] = ["动态通知", "动态订阅"]
+    bilichat_cmd_live: list[str] = ["直播通知", "直播订阅"]
+    bilichat_cmd_checkdynamic: list[str] = ["查看动态"]
+    bilichat_cmd_check_login: list[str] = ["查看登录账号"]
+    bilichat_cmd_login_qrcode: list[str] = ["扫码登录"]
+    bilichat_cmd_logout: list[str] = ["登出账号"]
 
     # basic info
     bilichat_basic_info: bool = True
     bilichat_basic_info_style: Literal["bbot_default", "style_blue"] = Field(default="Auto")
     bilichat_basic_info_url: bool = True
     bilichat_reply_to_basic_info: bool = True
 
     # dynamic
     bilichat_dynamic: bool = True
     bilichat_dynamic_style: Literal["dynamicrender", "browser_mobile", "browser_pc"] = Field(default="Auto")
-    bilichat_bilibili_cookie: Optional[str] = None
+    bilichat_bilibili_cookie: str | None = None
 
     # both WC and AI
     bilichat_use_bcut_asr: bool = True
 
     # Word Cloud
     bilichat_word_cloud: bool = False
-    bilichat_word_cloud_size: List[int] = [1000, 800]
+    bilichat_word_cloud_size: list[int] = [1000, 800]
 
     # AI Summary
     bilichat_summary_ignore_null: bool = True
     bilichat_official_summary: bool = False
-    bilichat_openai_token: Optional[str] = None
-    bilichat_openai_proxy: Optional[str] = None
+    bilichat_openai_token: str | None = None
+    bilichat_openai_proxy: str | None = None
     bilichat_openai_model: Literal[
         "gpt-3.5-turbo",
         "gpt-3.5-turbo-0301",
         "gpt-3.5-turbo-0613",
         "gpt-3.5-turbo-16k",
         "gpt-3.5-turbo-16k-0613",
         "gpt-4",
@@ -93,14 +87,16 @@
     bilichat_openai_api_base: str = "https://api.openai.com"
 
     @validator("bilichat_cache_serive", always=True, pre=True)
     def check_cache_serive(cls, v):
         if v == "json":
             return v
         try:
+            if not importlib.util.find_spec("nonebot_plugin_mongodb"):
+                raise ImportError
             require("nonebot_plugin_mongodb")
             if v == "Auto":
                 logger.info("bilichat_cache_serive 可以使用 MongoDB 作为缓存服务")
             return "mongodb"
         except Exception as e:
             if v == "Auto":
                 logger.info("bilichat_cache_serive 无法使用 MongoDB 作为缓存服务, 使用 JSON 文件作为缓存服务")
@@ -228,15 +224,15 @@
         if not v:
             return v
         v = v.strip("/")
         if "/" in v:
             raise ValueError("bilichat_webui_path 不应包含 '/'")
         return v
 
-    def verify_permission(self, uid: Union[str, int]):
+    def verify_permission(self, uid: str | int) -> bool:
         if self.bilichat_whitelist:
             return str(uid) in self.bilichat_whitelist
         elif self.bilichat_blacklist:
             return str(uid) not in self.bilichat_blacklist
         else:
             return True
```

### Comparing `nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/content/column.py` & `nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/content/column.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from typing import Optional
-
 from httpx._exceptions import TimeoutException
 from lxml import etree
 from lxml.etree import _Element, _ElementUnicodeResult
 from nonebot.log import logger
 from pydantic import BaseModel
 
 from ..lib.bilibili_request import get_b23_url, hc
@@ -20,21 +18,21 @@
     id: int
     """专栏cv号"""
     title: str
     """专栏标题"""
     url: str
     """b23 链接"""
     cache: BaseCache
-    
+
     @property
     def bili_id(self) -> str:
         return f"cv{self.id}"
 
     @classmethod
-    async def from_id(cls, bili_number: str, options: Optional[Options] = None):
+    async def from_id(cls, bili_number: str, options: Options | None = None):
         try:
             cvid = bili_number[2:]
             cv = await hc.get(f"https://www.bilibili.com/read/cv{cvid}", cookies=AuthManager.get_cookies())
             if cv.status_code != 200:
                 logger.debug(f"cv{cvid} status code: {cv.status_code} content: \n{cv.content}")
                 raise AbortError("未找到此专栏，可能已被 UP 主删除。")
             cv.encoding = "utf-8"
```

### Comparing `nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/content/dynamic.py` & `nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/content/dynamic.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Dict, Literal
+from typing import Literal
 
 from bilireq.exceptions import GrpcError, ResponseCodeError
 from bilireq.grpc.dynamic import grpc_get_dynamic_detail
 from bilireq.grpc.protos.bilibili.app.dynamic.v2.dynamic_pb2 import DynamicType, DynModuleType
 from google.protobuf.json_format import MessageToDict
 from nonebot.log import logger
 from pydantic import BaseModel
@@ -17,15 +17,15 @@
 class Dynamic(BaseModel):
     id: str
     """动态编号"""
     url: str
     """b23 链接"""
     dynamic_type: DynamicType.ValueType = DynamicType.dyn_none
     "动态类型"
-    raw: Dict = {}
+    raw: dict = {}
     """动态的原始信息"""
     raw_type: Literal["web", "grpc", None] = None
     
     @property
     def bili_id(self) -> str:
         return f"动态id: {self.id}"
```

### Comparing `nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/content/video.py` & `nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/content/video.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from typing import Optional
-
 from bilireq.grpc.protos.bilibili.app.view.v1.view_pb2 import ViewReply
 from bilireq.utils import get
 from nonebot.log import logger
 from pydantic import BaseModel, ValidationError
 
 from ..lib.bilibili_request import get_b23_url, grpc_get_view_info
 from ..lib.cache import BaseCache, Cache
@@ -30,15 +28,15 @@
         arbitrary_types_allowed = True
 
     @property
     def bili_id(self) -> str:
         return f"av{self.id}"
 
     @classmethod
-    async def from_id(cls, bili_number: str, options: Optional[Options] = None):
+    async def from_id(cls, bili_number: str, options: Options | None = None):
         logger.info(f"Parsing video {bili_number}")
         video_info = None
         if bili_number[:2].lower() == "av":
             if aid := int(bili_number[2:]):
                 video_info = await grpc_get_view_info(aid=aid)
         else:
             video_info = await grpc_get_view_info(bvid=bili_number)
@@ -85,17 +83,19 @@
         return await (await VideoImage.from_view_rely(self.raw, self.url)).render(style)
 
     async def get_offical_summary(self):
         resp = await get(
             "https://api.bilibili.com/x/web-interface/view/conclusion/get",
             params={
                 "bvid": self.raw.bvid,
-                "cid": self.raw.activity_season.pages[0].page.cid
-                if self.raw.activity_season.pages
-                else self.raw.pages[0].page.cid,
+                "cid": (
+                    self.raw.activity_season.pages[0].page.cid
+                    if self.raw.activity_season.pages
+                    else self.raw.pages[0].page.cid
+                ),
                 "up_mid": self.raw.arc.author.mid,
                 "web_location": "0.0",
             },
             is_wbi=True,
         )
         logger.debug(resp)
         try:
```

### Comparing `nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/lib/bcut_asr.py` & `nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/lib/bcut_asr.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import time
 from os import PathLike
 from pathlib import Path
-from typing import List, Literal, Optional, Union
+from typing import Literal
 
 import httpx
 from nonebot.log import logger
 
 from ..model.bcut_asr import (
     ResourceCompleteRspSchema,
     ResourceCreateRspSchema,
@@ -40,33 +40,33 @@
     session: httpx.AsyncClient
     sound_name: str
     sound_bin: bytes
     sound_fmt: SUPPORT_SOUND_FORMAT
     __in_boss_key: str
     __resource_id: str
     __upload_id: str
-    __upload_urls: List[str]
+    __upload_urls: list[str]
     __per_size: int
     __clips: int
-    __etags: List[str]
+    __etags: list[str]
     __download_url: str
     task_id: str
 
-    def __init__(self, file: Optional[Union[str, PathLike]] = None) -> None:
+    def __init__(self, file: str | PathLike | None = None) -> None:
         self.session = httpx.AsyncClient()
         self.task_id = ""
         self.__etags = []
         if file:
             self.set_data(file)
 
     def set_data(
         self,
-        _file: Optional[Union[str, PathLike]] = None,
-        raw_data: Optional[bytes] = None,
-        data_fmt: Optional[SUPPORT_SOUND_FORMAT] = None,
+        _file: str | PathLike | None = None,
+        raw_data: bytes | None = None,
+        data_fmt: SUPPORT_SOUND_FORMAT | None = None,
     ) -> None:
         "设置欲识别的数据"
         if _file:
             if not isinstance(_file, (str, PathLike)):
                 raise TypeError("unknow file ptr")
             # 文件类
             _file = Path(_file)
@@ -160,15 +160,15 @@
         if code := resp["code"]:
             raise APIError(code, resp["message"])
         resp_data = TaskCreateRspSchema(**resp["data"])
         self.task_id = resp_data.task_id
         logger.info(f"Conversion task created: {self.task_id}")
         return self.task_id
 
-    async def result(self, task_id: Optional[str] = None) -> ResultRspSchema:
+    async def result(self, task_id: str | None = None) -> ResultRspSchema:
         "查询转换结果"
         resp = await self.session.get(API_QUERY_RESULT, params={"model_id": 7, "task_id": task_id or self.task_id})
         resp.raise_for_status()
         resp = resp.json()
         if code := resp["code"]:
             raise APIError(code, resp["message"])
         return ResultRspSchema(**resp["data"])
```

### Comparing `nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/lib/bilibili_request/auth.py` & `nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/lib/bilibili_request/auth.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 import json
 import random
-from typing import Any, Dict, List, Union
 
 from bilireq.auth import Auth
 from nonebot import get_driver
 from nonebot.log import logger
 
 from ..store import cache_dir
 
 bili_grpc_auth_file = cache_dir.joinpath("bili_grpc_auth.json")
 bili_grpc_auth_file.touch(0o700, exist_ok=True)
 
 
 class AuthManager:
-    grpc_auths: List[Auth] = []
+    grpc_auths: list[Auth] = []
 
     @classmethod
     async def load_grpc_auths(cls) -> None:
-        data: Union[List[Dict], Dict] = json.loads(bili_grpc_auth_file.read_bytes() or "[]")
+        data: list[dict] | dict = json.loads(bili_grpc_auth_file.read_bytes() or "[]")
         data = data if isinstance(data, list) else [data]
         cls.grpc_auths.clear()
         for raw_auth in data:
             auth = Auth(raw_auth)
             try:
                 auth = await auth.refresh()
                 cls.grpc_auths.append(auth)
@@ -33,38 +32,38 @@
     @classmethod
     def dump_grpc_auths(cls):
         bili_grpc_auth_file.write_text(
             json.dumps([auth.data for auth in cls.grpc_auths], indent=2, ensure_ascii=False), encoding="utf-8"
         )
 
     @classmethod
-    def get_cookies(cls) -> Dict[str, str]:
+    def get_cookies(cls) -> dict[str, str]:
         if auths := cls.grpc_auths.copy():
             random.shuffle(auths)
             for auth in auths:
                 if auth.cookies:
                     return auth.cookies.copy()
         logger.warning("没有可用的 bilibili cookies，请求可能风控")
         return {}
 
     @classmethod
-    def get_auth(cls) -> Union[Auth, None]:
+    def get_auth(cls) -> Auth | None:
         return random.choice(cls.grpc_auths).copy() if cls.grpc_auths else None
 
     @classmethod
     def add_auth(cls, auth: Auth) -> None:
         for old_auth in cls.grpc_auths:
             if old_auth.uid == auth.uid:
                 cls.grpc_auths.remove(old_auth)
                 break
         cls.grpc_auths.append(auth)
         cls.dump_grpc_auths()
 
     @classmethod
-    def remove_auth(cls, uid: int) -> Union[str, None]:
+    def remove_auth(cls, uid: int) -> str | None:
         for old_auth in cls.grpc_auths:
             if old_auth.uid == uid:
                 cls.grpc_auths.remove(old_auth)
                 cls.dump_grpc_auths()
                 return
         logger.warning(f"没有找到 uid 为 {uid} 的账号")
         return f"没有找到 uid 为 {uid} 的账号"
```

### Comparing `nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/lib/bilibili_request/gRPC.py` & `nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/lib/bilibili_request/gRPC.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/lib/bilibili_request/restAPI.py` & `nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/lib/bilibili_request/restAPI.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/lib/browser.py` & `nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/lib/browser.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/lib/cache/json_cache.py` & `nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/lib/cache/json_cache.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/lib/cache/mongo_cache.py` & `nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/lib/cache/mongo_cache.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/lib/draw/__init__.py` & `nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/lib/draw/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/lib/draw/column/browser_shot.py` & `nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/lib/draw/column/browser_shot.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/lib/draw/dynamic/browser_shot.py` & `nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/lib/draw/dynamic/browser_shot.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/lib/draw/dynamic/dynamicrender.py` & `nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/lib/draw/dynamic/dynamicrender.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from io import BytesIO
-from typing import Dict
 
 import skia
 from dynamicadaptor.DynamicConversion import formate_message
 from dynrender_skia.Core import DynRender
 
 from ....config import plugin_config
 from ...fonts_provider import get_font_sync
@@ -24,14 +23,14 @@
         get_font_sync("nte.ttf")
         if plugin_config.bilichat_emoji_fonts == "default"
         else plugin_config.bilichat_emoji_fonts
     ),
 )
 
 
-async def skia_dynamic(raw: Dict, raw_type: str, **kwargs):
+async def skia_dynamic(raw: dict, raw_type: str, **kwargs):
     if dynamic_formate := await formate_message(raw_type, raw):
         img_bio = BytesIO()
         image_array = await render.run(dynamic_formate) # type: ignore
         img = skia.Image.fromarray(image_array, colorType=skia.ColorType.kRGBA_8888_ColorType)
         img.save(img_bio)
         return img_bio.getvalue()
```

### Comparing `nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/lib/draw/video/__init__.py` & `nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/lib/draw/video/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 from datetime import datetime
 from io import BytesIO
-from typing import List, Optional, Union
 
 from bilireq.exceptions import ResponseCodeError
 from bilireq.grpc.protos.bilibili.app.view.v1.view_pb2 import ViewReply
 from httpx import AsyncClient
 
 from ...bilibili_request import get_user_space_info, hc
 from ...strings import num_fmt
 
 
 class UP:
     def __init__(
         self,
         name: str,
-        face: Union[bytes, BytesIO],
+        face: bytes | BytesIO,
         level: int,
         fans: str,
         video_counts: int,
         title: str = "UP主",
         name_color: str = "black",
         official_verify: int = -1,
     ) -> None:
@@ -70,30 +69,30 @@
 
 
 class VideoImage:
     _render_methods = {}
 
     def __init__(
         self,
-        cover: Union[bytes, BytesIO],
+        cover: bytes | BytesIO,
         duration: int,
         type_name: str,
         title: str,
         view: str,
         danmaku: str,
         favorite: str,
         coin: str,
         like: str,
         reply: str,
         share: str,
         pubdate: datetime,
-        uploaders: List[UP],
+        uploaders: list[UP],
         b23_url: str,
         aid: str,
-        desc: Optional[str] = None,
+        desc: str|None = None,
     ):
         self.cover: BytesIO = cover if isinstance(cover, BytesIO) else BytesIO(cover)
         """视频封面"""
         minutes, self.seconds = divmod(duration, 60)
         self.hours, self.minutes = divmod(minutes, 60)
         self.type_name: str = type_name
         """视频分区"""
@@ -113,15 +112,15 @@
         """点赞"""
         self.reply: str = reply
         """评论"""
         self.share: str = share
         """分享"""
         self.pubdate: datetime = pubdate
         """发布时间"""
-        self.uploaders: List[UP] = uploaders
+        self.uploaders: list[UP] = uploaders
         """up主列表"""
         self.b23_url: str = b23_url
         """b23短链"""
         self.aid: str = aid
         """av号"""
 
     @classmethod
```

### Comparing `nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/lib/draw/video/bbot_default.py` & `nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/lib/draw/video/bbot_default.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/lib/draw/video/style_blue.py` & `nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/lib/draw/video/style_blue.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/lib/fetch_dynamic.py` & `nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/lib/fetch_dynamic.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,63 +1,40 @@
 import asyncio
-from typing import List, Union
 
 from bilireq.exceptions import GrpcError, ResponseCodeError
 from bilireq.grpc.dynamic import grpc_get_user_dynamics
-from bilireq.grpc.protos.bilibili.app.dynamic.v2.dynamic_pb2 import (
-    DynamicType,
-)
 from google.protobuf.json_format import MessageToDict
 from grpc.aio import AioRpcError
 from httpx import TimeoutException
 from nonebot.log import logger
 
 from ..base_content_parsing import check_cd
 from ..content.dynamic import Dynamic
 from ..lib.bilibili_request import get_b23_url, get_user_dynamics
 from ..lib.bilibili_request.auth import AuthManager
 from ..lib.uid_extract import SearchUp
+from ..model.const import DYNAMIC_TYPE_IGNORE
 from ..model.exception import AbortError
 from ..optional import capture_exception
 from ..subscribe.manager import SubscriptionSystem
 
-DYNAMIC_TYPE_MAP = {
-    "DYNAMIC_TYPE_FORWARD": DynamicType.forward,
-    "DYNAMIC_TYPE_WORD": DynamicType.word,
-    "DYNAMIC_TYPE_DRAW": DynamicType.draw,
-    "DYNAMIC_TYPE_AV": DynamicType.av,
-    "DYNAMIC_TYPE_ARTICLE": DynamicType.article,
-    "DYNAMIC_TYPE_MUSIC": DynamicType.music,
-}
-
-DYNAMIC_TYPE_IGNORE = {
-    "DYNAMIC_TYPE_AD",
-    "DYNAMIC_TYPE_LIVE",
-    "DYNAMIC_TYPE_LIVE_RCMD",
-    "DYNAMIC_TYPE_BANNER",
-    DynamicType.ad,
-    DynamicType.live,
-    DynamicType.live_rcmd,
-    DynamicType.banner,
-}
 
-
-async def fetch_last_dynamic(up: SearchUp) -> Union[Dynamic, None]:
+async def fetch_last_dynamic(up: SearchUp) -> Dynamic | None:
     if SubscriptionSystem.config.dynamic_grpc:
         try:
             return await _fetch_grpc(up.mid, up.nickname)
         except AbortError:
             return await _fetch_rest(up.mid, up.nickname)
     else:
         return await _fetch_rest(up.mid, up.nickname)
 
 
-async def _fetch_rest(up_mid: int, up_name: str) -> Union[Dynamic, None]:
+async def _fetch_rest(up_mid: int, up_name: str) -> Dynamic | None:
     try:
-        resp: List = (await get_user_dynamics(up_mid))["items"]
+        resp: list = (await get_user_dynamics(up_mid))["items"]
     except TimeoutException:
         logger.error(f"[Dynamic] 获取 {up_name}({up_mid}) 超时")
         raise AbortError("Dynamic Abort")
     except ResponseCodeError as e:
         logger.error(
             f"[Dynamic] 获取 {up_name}({up_mid}) 失败: "
             f"[{e.code}] {e.details() if isinstance(e, AioRpcError) else e.msg}"
@@ -74,15 +51,15 @@
     check_cd(dyn["id_str"], check=False)
 
     url = await get_b23_url(f"https://t.bilibili.com/{dyn['id_str']}")
     dynamic = Dynamic(id=dyn["id_str"], url=url, raw=dyn, raw_type="web")
     return dynamic
 
 
-async def _fetch_grpc(up_mid: int, up_name: str) -> Union[Dynamic, None]:
+async def _fetch_grpc(up_mid: int, up_name: str) -> Dynamic | None:
     try:
         resp = await asyncio.wait_for(grpc_get_user_dynamics(up_mid, auth=AuthManager.get_auth()), timeout=10)
     except asyncio.TimeoutError:
         logger.error(f"[Dynamic] 获取 {up_name}({up_mid}) 超时")
         raise AbortError("Dynamic Abort")
     except (GrpcError, AioRpcError) as e:
         logger.error(
```

### Comparing `nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/lib/fonts_provider.py` & `nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/lib/fonts_provider.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/lib/store.py` & `nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/lib/store.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/lib/strings.py` & `nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/lib/strings.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import re
 import string
-from typing import List
 
 
 def num_fmt(num: int):
     if num < 10000:
         return str(num)
     elif num < 100000000:
         return ("%.2f" % (num / 10000)) + "万"
@@ -57,15 +56,15 @@
         elif p[-1] == "\n":
             p = p[:-1]
         non_wrap_str.append(p)
         i += 1
     return non_wrap_str
 
 
-def generate_framed_text(content: List[str], width=88, padding=4):
+def generate_framed_text(content: list[str], width=88, padding=4):
     """
     Generates a framed text block with specified width and padding.
 
     Parameters:
     content (list of str): The content to be framed.
     width (int): The total width of the framed block including the border.
     padding (int): The padding between the text and the border.
```

### Comparing `nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/lib/text_to_image.py` & `nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/lib/text_to_image.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/lib/tools.py` & `nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/lib/tools.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import datetime
 import re
-from typing import Union
 
 
-def calc_time_total(t: Union[float, int]):
+def calc_time_total(t: float | int):
     """
     Calculate the total time in a human-readable format.
 
     Args:
         t (float | int): The time in seconds.
 
     Returns:
```

### Comparing `nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/lib/uid_extract.py` & `nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/lib/uid_extract.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import asyncio
 from concurrent.futures import ThreadPoolExecutor
-from typing import List, Union
 
 from nonebot.log import logger
 from pydantic import BaseModel, Field
 
 from .bilibili_request import search_user
 
 
@@ -13,30 +12,30 @@
     mid: int
 
     def __str__(self) -> str:
         return f"{self.nickname}({self.mid})"
 
 
 class SearchResult(BaseModel):
-    items: List[SearchUp] = []
+    items: list[SearchUp] = []
 
 
-async def search(text_u: str) -> Union[str, SearchUp]:
+async def search(text_u: str) -> str | SearchUp:
     resp = await search_user(text_u)
     result = SearchResult(**resp)
     if result.items:
         for up in result.items:
             if up.nickname == text_u or str(up.mid) in text_u:
                 logger.debug(up)
                 return up
         return "未找到该 UP，你可能在找：\n" + "\n".join([str(up) for up in result.items])
     return "未找到该 UP 主呢\n`(*>﹏<*)′"
 
 
-async def uid_extract(text: str) -> Union[str, SearchUp]:
+async def uid_extract(text: str) -> str | SearchUp:
     text_u = text.strip(""""'“”‘’""").strip().replace("：", ":")
     up = await search(text_u)
     if isinstance(up, str) and text_u.isdigit():
         up = await search("UID: " + text_u)
     return up
 
 
@@ -51,10 +50,10 @@
             loop.close()  # 关闭事件循环
 
     with ThreadPoolExecutor(max_workers=1) as executor:
         future = executor.submit(asyncio.run, thread_func())
         return future.result()
 
 
-def uid_extract_sync(text: str) -> Union[str, SearchUp]:
+def uid_extract_sync(text: str) -> str | SearchUp:
     # 调用 run_async_in_thread 来运行异步函数并获取结果
     return run_async_in_thread(uid_extract, text)
```

### Comparing `nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/lib/video_subtitle.py` & `nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/lib/video_subtitle.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 import asyncio
-from typing import Dict, List, Optional
 
 import httpx
 from nonebot.log import logger
 
 from ..config import plugin_config
 from ..model.bcut_asr import ResultStateEnum
 from ..model.exception import AbortError
 from .bcut_asr import BcutASR
 from .bilibili_request import get_player, grpc_get_playview, hc
 
 
-async def get_subtitle_url(aid: int, cid: int) -> Optional[str]:
+async def get_subtitle_url(aid: int, cid: int) -> str|None:
     video_player = await get_player(aid, cid)
-    subtitles_raw: List[Dict] = video_player["subtitle"]["subtitles"]
+    subtitles_raw: list[dict] = video_player["subtitle"]["subtitles"]
     logger.debug(subtitles_raw)
 
     if not subtitles_raw:
         return
 
     logger.debug(subtitles_raw)
     ai_subtitles = {}
@@ -36,15 +35,15 @@
     for sub in preferred_subs:
         if sub in manual_subtitles:
             return manual_subtitles[sub]
 
     return next(iter(manual_subtitles.values()))
 
 
-async def get_subtitle(aid: int, cid: int) -> List[str]:
+async def get_subtitle(aid: int, cid: int) -> list[str]:
     subtitle_url = await get_subtitle_url(aid, cid)
     if subtitle_url:
         logger.debug(subtitle_url)
         subtitle = await hc.get(f"https:{subtitle_url}")
         if subtitle.status_code != 200:
             logger.warning(
                 f"Subtitle fetch failed: {aid} {cid}, status code: {subtitle.status_code}, content: {subtitle.text}"
```

### Comparing `nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/model/api/__init__.py` & `nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/model/api/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-from typing import Generic, Optional, TypeVar
+from typing import Generic, TypeVar
 
 from nonebot.compat import PYDANTIC_V2
 from pydantic import BaseModel
 
 DataType = TypeVar("DataType")
 
 if PYDANTIC_V2:
 
     class Response(BaseModel, Generic[DataType]):  # type: ignore
         code: int = 0
         message: str = ""
-        data: Optional[DataType]
+        data: DataType | None
 
 else:
     from pydantic.generics import GenericModel
 
     class Response(GenericModel, Generic[DataType]):
         code: int = 0
         message: str = ""
-        data: Optional[DataType]
+        data: DataType | None
 
 
 class FaildResponse(BaseModel):
     code: int
     message: str
```

### Comparing `nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/model/api/subs_config.py` & `nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/model/api/subs_config.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from typing import List
 
 from nonebot_plugin_auto_bot_selector.target import SupportedPlatform
 from pydantic import BaseModel, Field
 
 
 class SubsConfig(BaseModel):
     subs_limit: int = Field(5, ge=0, le=50)
@@ -20,19 +19,19 @@
     live_at_all: bool = False
 
 
 class User(BaseModel):
     user_id: str
     platform: SupportedPlatform
     at_all: bool = False
-    subscriptions: List[UserSubConfig]
+    subscriptions: list[UserSubConfig]
 
 
 class Uploader(BaseModel):
     uid: int
     nickname: str = ""
 
 
 class Subs(BaseModel):
     config: SubsConfig
-    uploaders: List[Uploader] = []
-    users: List[User] = []
+    uploaders: list[Uploader] = []
+    users: list[User] = []
```

### Comparing `nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/model/arguments.py` & `nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/model/arguments.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/model/bcut_asr.py` & `nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/model/bcut_asr.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from enum import Enum
-from typing import List, Tuple
 
 from nonebot.compat import PYDANTIC_V2
 from pydantic import BaseModel
 
 
 class ASRDataSeg(BaseModel):
     "文字识别-断句"
@@ -14,40 +13,40 @@
         start_time: int
         end_time: int
         confidence: int
 
     start_time: int
     end_time: int
     transcript: str
-    words: List[ASRDataWords]
+    words: list[ASRDataWords]
     confidence: int
 
     def to_srt_ts(self) -> str:
         "转换为srt时间戳"
 
-        def _conv(ms: int) -> Tuple[int, int, int, int]:
+        def _conv(ms: int) -> tuple[int, int, int, int]:
             return ms // 3600000, ms // 60000 % 60, ms // 1000 % 60, ms % 1000
 
         s_h, s_m, s_s, s_ms = _conv(self.start_time)
         e_h, e_m, e_s, e_ms = _conv(self.end_time)
         return f"{s_h:02d}:{s_m:02d}:{s_s:02d},{s_ms:03d} --> {e_h:02d}:{e_m:02d}:{e_s:02d},{e_ms:03d}"
 
     def to_lrc_ts(self) -> str:
         "转换为lrc时间戳"
 
-        def _conv(ms: int) -> Tuple[int, int, int]:
+        def _conv(ms: int) -> tuple[int, int, int]:
             return ms // 60000, ms // 1000 % 60, ms % 1000 // 10
 
         s_m, s_s, s_ms = _conv(self.start_time)
         return f"[{s_m:02d}:{s_s:02d}.{s_ms:02d}]"
 
 
 class ASRData(BaseModel):
     "语音识别结果"
-    utterances: List[ASRDataSeg]
+    utterances: list[ASRDataSeg]
     version: str
 
     def __iter__(self):
         "iter穿透"
         return iter(self.utterances)
 
     def has_data(self) -> bool:
@@ -72,15 +71,15 @@
 class ResourceCreateRspSchema(BaseModel):
     "上传申请响应"
     resource_id: str
     title: str
     type: int
     in_boss_key: str
     size: int
-    upload_urls: List[str]
+    upload_urls: list[str]
     upload_id: str
     per_size: int
 
 
 class ResourceCompleteRspSchema(BaseModel):
     "上传提交响应"
     resource_id: str
```

### Comparing `nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/model/bilibili/live.py` & `nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/model/bilibili/live.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/model/bilibili/summary.py` & `nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/model/bilibili/summary.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 import time
-from typing import List
 
 from pydantic import BaseModel, Field
 
 
 class PartOutline(BaseModel):
     timestamp: int
     content: str
 
 
 class Outline(BaseModel):
     title: str
     """分段标题"""
-    part_outline: List[PartOutline]
+    part_outline: list[PartOutline]
     """分段中的细分内容"""
     timestamp: int
 
 
 class ModelResult(BaseModel):
     result_type: int
     summary: str
     """视频总结"""
-    outline: List[Outline]
+    outline: list[Outline]
     """分段总结"""
 
     @staticmethod
     def _format_ts(ts: int):
         return time.strftime("%M:%S", time.gmtime(ts))
 
     def markdown(self) -> str:
```

### Comparing `nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/model/exception.py` & `nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/model/exception.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/static/browser/mobile_style.js` & `nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/static/browser/mobile_style.js`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/static/style_blue/assets/business.png` & `nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/static/style_blue/assets/business.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/static/style_blue/assets/personal.png` & `nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/static/style_blue/assets/personal.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/static/style_blue/assets/video_bottom.png` & `nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/static/style_blue/assets/video_bottom.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/static/style_blue/video-details.html` & `nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/static/style_blue/video-details.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/static/summary/bilibili.png` & `nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/static/summary/bilibili.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/static/summary/index.html` & `nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/static/summary/index.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/static/summary/marked.min.js` & `nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/static/summary/marked.min.js`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/static/summary/openai.png` & `nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/static/summary/openai.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/static/upload-webui.html` & `nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/static/upload-webui.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/static/webui.tar.gz` & `nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/static/webui.tar.gz`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/subscribe/__init__.py` & `nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/subscribe/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/subscribe/dynamic.py` & `nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/subscribe/dynamic.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import asyncio
-from typing import List
 
 from bilireq.exceptions import GrpcError, ResponseCodeError
 from bilireq.grpc.dynamic import grpc_get_user_dynamics
 from bilireq.grpc.protos.bilibili.app.dynamic.v2.dynamic_pb2 import (
     DynamicType,
     DynModuleType,
 )
@@ -13,23 +12,23 @@
 from nonebot.log import logger
 
 from ..base_content_parsing import check_cd
 from ..config import plugin_config
 from ..content.dynamic import Dynamic
 from ..lib.bilibili_request import get_b23_url, get_user_dynamics
 from ..lib.bilibili_request.auth import AuthManager
-from ..lib.fetch_dynamic import DYNAMIC_TYPE_IGNORE, DYNAMIC_TYPE_MAP
+from ..model.const import DYNAMIC_TYPE_MAP, DYNAMIC_TYPE_IGNORE
 from ..model.exception import AbortError
 from ..optional import capture_exception
 from .manager import Uploader
 
 
 async def fetch_dynamics_rest(up: Uploader):
     try:
-        resp: List = (await get_user_dynamics(up.uid))["items"]
+        resp: list = (await get_user_dynamics(up.uid))["items"]
     except TimeoutException:
         logger.error(f"[Dynamic] 获取 {up.nickname}({up.uid}) 超时")
         raise AbortError("Dynamic Abort")
     except ResponseCodeError as e:
         logger.error(
             f"[Dynamic] 获取 {up.nickname}({up.uid}) 失败: "
             f"[{e.code}] {e.details() if isinstance(e, AioRpcError) else e.msg}"
```

### Comparing `nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/subscribe/live.py` & `nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/subscribe/live.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/subscribe/manager.py` & `nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/subscribe/manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import asyncio
 import json
 import random
 import time
-from typing import Any, Dict, List, Optional, Tuple, Union
+from typing import Any
 
 from apscheduler.job import Job
 from nonebot import get_driver
 from nonebot.adapters import Bot
 from nonebot.compat import PYDANTIC_V2
 from nonebot.log import logger
 from nonebot_plugin_alconna.uniseg import AtAll, Image, Target, UniMessage
@@ -26,21 +26,15 @@
 from pydantic import BaseModel, Field, validator
 
 from ..lib.store import data_dir
 from ..lib.tools import calc_time_total
 from ..lib.uid_extract import uid_extract_sync
 from ..optional import capture_exception
 
-# 临时解决方案
-try:
-    CONFIG_LOCK = asyncio.Lock()
-except RuntimeError:
-    loop = asyncio.new_event_loop()
-    asyncio.set_event_loop(loop)
-    CONFIG_LOCK = asyncio.Lock(loop=loop)  # type: ignore
+CONFIG_LOCK = asyncio.Lock()
 
 subscribe_file = data_dir.joinpath("subscribe.json")
 subscribe_file.touch(0o755, True)
 
 driver = get_driver()
 
 
@@ -58,19 +52,19 @@
         if not self.nickname:
             up = uid_extract_sync(f"UID: {self.uid}")
             if isinstance(up, str):
                 raise ValueError(f"未找到 uid 为 {self.uid} 的 UP")
             self.nickname = up.nickname
 
     @property
-    def subscribed_users(self) -> List["User"]:
+    def subscribed_users(self) -> list["User"]:
         """Get a list of user IDs subscribed to this uploader."""
         return [user for user in SubscriptionSystem.users.values() if self.uid in user.subscriptions]
 
-    def dict(self, **kwargs) -> Dict[str, Any]:
+    def dict(self, **kwargs) -> dict[str, Any]:
         exclude_properties = {name for name, value in type(self).__dict__.items() if isinstance(value, property)}
         exclude_properties.add("living")
         exclude_properties.add("dyn_offset")
         if PYDANTIC_V2:
             dict_ = super().model_dump(**{**kwargs, "exclude": exclude_properties})  # type: ignore
         else:
             dict_ = super().dict(**{**kwargs, "exclude": exclude_properties})  # type: ignore
@@ -122,18 +116,18 @@
 
 class User(BaseModel):
     """Represents a user in the system."""
 
     user_id: str
     platform: str
     at_all: bool = False
-    subscriptions: Dict[int, UserSubConfig] = {}
+    subscriptions: dict[int, UserSubConfig] = {}
 
     @validator("subscriptions", pre=True, always=True)
-    def validate_subscriptions(cls, v: Union[Dict[str, Dict[str, Any]], List[Dict[str, Any]]]):
+    def validate_subscriptions(cls, v: dict[str, dict[str, Any]] | list[dict[str, Any]]):
         if not v:
             return {}
 
         if isinstance(v, list):
             # 列表形式的输入：直接解包每个字典创建 UserSubConfig 实例
             return {sub.get("uid"): UserSubConfig(**sub) for sub in v if sub.get("uid") is not None}
 
@@ -150,15 +144,15 @@
             except (ValueError, TypeError):
                 # 处理 uid 转换为 int 时可能发生的错误
                 continue
 
         return validated_subs
 
     @classmethod
-    def extract_alc_target(cls, target: Target) -> Tuple[str, str]:
+    def extract_alc_target(cls, target: Target) -> tuple[str, str]:
         t = extract_target(target)
         return t.platform_type, target.id
 
     def create_saa_target(self) -> PlatformTarget:
         if self.platform == SupportedPlatform.qq_group:
             return TargetQQGroup(group_id=int(self.user_id))
         elif self.platform == SupportedPlatform.qq_private:
@@ -170,39 +164,39 @@
         # Other
         else:
             raise NotImplementedError("Unsupported platform type")
 
     def create_alc_target(self) -> Target:
         return create_target(self.create_saa_target())
 
-    def dict(self, **kwargs) -> Dict[str, Any]:
+    def dict(self, **kwargs) -> dict[str, Any]:
         exclude_properties = {name for name, value in type(self).__dict__.items() if isinstance(value, property)}
         exclude_properties.add("subscriptions")
         if PYDANTIC_V2:
             dict_ = super().model_dump(**{**kwargs, "exclude": exclude_properties})  # type: ignore
         else:
             dict_ = super().dict(**{**kwargs, "exclude": exclude_properties})  # type: ignore
         dict_["subscriptions"] = [sub.dict() for sub in self.subscriptions.values()]
         return dict_
 
     @property
-    def subscribe_ups(self) -> List[Uploader]:
+    def subscribe_ups(self) -> list[Uploader]:
         uplist = []
         for uid in self.subscriptions.keys():
             if up := SubscriptionSystem.uploaders.get(int(uid)):
                 uplist.append(up)
             else:
                 del self.subscriptions[uid]
         return uplist
 
     @property
     def _id(self) -> str:
         return f"{self.platform}-_-{self.user_id}"
 
-    async def push_to_user(self, content: List[Union[str, bytes]], at_all: Optional[bool] = None):
+    async def push_to_user(self, content: list[str | bytes], at_all: bool | None = None):
         if not at_all:
             at = ""
         elif self.platform == SupportedPlatform.qq_group:
             at = AtAll()
         elif self.platform == SupportedPlatform.qq_guild_channel:
             at = "@everyone"
         else:
@@ -226,15 +220,15 @@
             except Exception as e:
                 capture_exception(e)
                 logger.exception(f"推送失败 -> {bot}")
         logger.error(f"无法为用户 {self.user_id} 推送消息")
 
         await asyncio.sleep(SubscriptionSystem.config.push_delay)
 
-    def add_subscription(self, uploader: Uploader) -> Union[None, str]:
+    def add_subscription(self, uploader: Uploader) -> str | None:
         """Add a subscription for a user to an uploader."""
 
         if len(self.subscriptions) > SubscriptionSystem.config.subs_limit:
             return "本群的订阅已经满啦\n删除无用的订阅再试吧\n`(*>﹏<*)′"
 
         if uploader.uid in self.subscriptions:
             return "本群已经订阅了此UP主呢...\n`(*>﹏<*)′"
@@ -244,15 +238,15 @@
         SubscriptionSystem.uploaders[uploader.uid] = uploader
         SubscriptionSystem.activate_uploaders[uploader.uid] = uploader
         SubscriptionSystem.users[self._id] = self
 
         SubscriptionSystem.get_activate_uploaders()
         SubscriptionSystem.save_to_file()
 
-    async def remove_subscription(self, uploader: Uploader) -> Union[None, str]:
+    async def remove_subscription(self, uploader: Uploader) -> str | None:
         """Remove a subscription for a user from an uploader."""
         if uploader.uid not in self.subscriptions:
             return "本群并未订阅此UP主呢...\n`(*>﹏<*)′"
 
         del self.subscriptions[uploader.uid]
         SubscriptionSystem.users[self._id] = self
         if not self.subscriptions:
@@ -271,26 +265,26 @@
     live_interval: int = Field(30, ge=10)
     push_delay: int = Field(3, ge=0)
     dynamic_grpc: bool = False
 
 
 class SubscriptionCfgFile(BaseModel):
     config: SubscriptionConfig = SubscriptionConfig(**{})
-    uploaders: List[Uploader] = []
-    users: List[User] = []
+    uploaders: list[Uploader] = []
+    users: list[User] = []
 
     @validator("uploaders", always=True, pre=True)
-    def validate_uploaders(cls, v: Union[Dict[str, Dict[str, Any]], List[Dict[str, Any]]]):
+    def validate_uploaders(cls, v: dict[str, dict[str, Any]] | list[dict[str, Any]]):
         if not v:
             return []
         ups = v.values() if isinstance(v, dict) else v
         return [Uploader(**up) for up in ups]
 
     @validator("users", always=True, pre=True)
-    def validate_users(cls, v: Union[Dict[str, Dict[str, Any]], List[Dict[str, Any]]]):
+    def validate_users(cls, v: dict[str, dict[str, Any]] | list[dict[str, Any]]):
         if not v:
             return []
         users = v.values() if isinstance(v, dict) else v
         users_obj = []
         for user in users:
             # 兼容旧版本配置文件
             if "platfrom" in user:
@@ -303,29 +297,29 @@
             users_obj.append(User(**user))
         return users_obj
 
 
 class SubscriptionSystem:
     """Manages the subscription system."""
 
-    uploaders: Dict[int, Uploader] = {}
-    activate_uploaders: Dict[int, Uploader] = {}
-    users: Dict[str, User] = {}
+    uploaders: dict[int, Uploader] = {}
+    activate_uploaders: dict[int, Uploader] = {}
+    users: dict[str, User] = {}
     config: SubscriptionConfig = SubscriptionConfig(**{})
 
     @classmethod
-    def dict(cls):
+    def dump_dict(cls):
         return {
             "config": cls.config.dict(),
             "uploaders": [up.dict() for up in cls.uploaders.values()],
             "users": [user.dict() for user in cls.users.values()],
         }
 
     @classmethod
-    async def load(cls, data: Dict[str, Union[Dict[str, Any], List[Dict[str, Any]]]]):
+    async def load(cls, data: dict[str, dict[str, Any] | list[dict[str, Any]]]):
         raw_cfg = SubscriptionCfgFile.parse_obj(data)
         while CONFIG_LOCK.locked():
             await asyncio.sleep(0)
         async with CONFIG_LOCK:
             cls.config = raw_cfg.config
             cls.uploaders.update({up.uid: up for up in raw_cfg.uploaders})
             cls.users = {f"{u.platform}-_-{u.user_id}": u for u in raw_cfg.users}
@@ -369,15 +363,15 @@
         await cls.load(json.loads(text or "{}"))
 
     @classmethod
     def save_to_file(cls):
         """Save data to the JSON file."""
         subscribe_file.write_text(
             json.dumps(
-                cls.dict(),
+                cls.dump_dict(),
                 ensure_ascii=False,
                 indent=2,
                 sort_keys=True,
             ),
             encoding="utf-8",
         )
```

### Comparing `nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/summary/openai.py` & `nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/summary/openai.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import random
 from collections import OrderedDict
-from typing import Dict, List, Literal, Optional
+from typing import Literal
 
 import httpx
 import tiktoken
 from nonebot.log import logger
 
 from ..config import plugin_config
 from ..model.openai import OpenAI, TokenUsage
@@ -27,15 +27,15 @@
             "\n不要随意翻译任何内容。仅使用中文总结。"
             "\n不说与总结无关的其他内容，你的回复仅限固定格式提供的“概述”和“要点”两项。"
             f"{type_[:2]}标题为“{title}”，{type_}数据如下，立刻开始总结：“{transcript}”"
         )
     )
 
 
-def count_tokens(prompts: List[Dict[str, str]]):
+def count_tokens(prompts: list[dict[str, str]]):
     """根据内容计算 token 数"""
 
     if plugin_config.bilichat_openai_model.startswith("gpt-3.5"):
         tokens_per_message = 4
         tokens_per_name = -1
     elif plugin_config.bilichat_openai_model.startswith("gpt-4"):
         tokens_per_message = 3
@@ -51,24 +51,24 @@
             if key == "name":
                 num_tokens += tokens_per_name
     num_tokens += 3
     return num_tokens
 
 
 def get_small_size_transcripts(
-    title: str, text_data: List[str], token_limit: int = plugin_config.bilichat_openai_token_limit
+    title: str, text_data: list[str], token_limit: int = plugin_config.bilichat_openai_token_limit
 ):
     unique_texts = list(OrderedDict.fromkeys(text_data))
     while count_tokens(get_summarise_prompt(title, " ".join(unique_texts))) > token_limit:
         unique_texts.pop(random.randint(0, len(unique_texts) - 1))
     return " ".join(unique_texts)
 
 
-def get_full_prompt(prompt: Optional[str] = None, system: Optional[str] = None, language: Optional[str] = None):
-    plist: List[Dict[str, str]] = []
+def get_full_prompt(prompt: str | None = None, system: str | None = None, language: str | None = None):
+    plist: list[dict[str, str]] = []
     if system:
         plist.append({"role": "system", "content": system})
     if prompt:
         plist.append({"role": "user", "content": prompt})
     if language:
         plist.extend(
             (
@@ -81,18 +81,18 @@
         )
     if not plist:
         raise ValueError("No prompt provided")
     return plist
 
 
 async def openai_req(
-    prompt_message: List[Dict[str, str]],
-    token: Optional[str] = plugin_config.bilichat_openai_token,
+    prompt_message: list[dict[str, str]],
+    token: str | None = plugin_config.bilichat_openai_token,
     model: str = plugin_config.bilichat_openai_model,
-    temperature: Optional[float] = None,
+    temperature: float | None = None,
     api_base: str = plugin_config.bilichat_openai_api_base,
 ):
     if not token:
         return OpenAI(error=True, message="未配置 OpenAI API Token")
     async with httpx.AsyncClient(
         proxies=plugin_config.bilichat_openai_proxy,
         headers={
```

### Comparing `nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/summary/openai_summarise.py` & `nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/summary/openai_summarise.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,25 @@
-from typing import List
-
 from nonebot.log import logger
 
 from ..config import plugin_config
 from ..lib.cache import BaseCache
 from ..lib.text_to_image import t2i
 from ..model.exception import ProssesError
 from ..optional import capture_exception  # type: ignore
 from .openai import get_small_size_transcripts, get_summarise_prompt, openai_req
 
 
-async def subtitle_summarise(title: str, sub: List[str]):
+async def subtitle_summarise(title: str, sub: list[str]):
     small_size_transcripts = get_small_size_transcripts(title, sub)
     prompt = get_summarise_prompt(title, small_size_transcripts)
     logger.debug(prompt)
     return await openai_req(prompt)
 
 
-async def column_summarise(cv_title: str, cv_text: List[str]):
+async def column_summarise(cv_title: str, cv_text: list[str]):
     small_size_transcripts = get_small_size_transcripts(cv_title, cv_text)
     prompt = get_summarise_prompt(cv_title, small_size_transcripts, type_="专栏文章")
     logger.debug(prompt)
     return await openai_req(prompt)
 
 
 async def openai_summarization(cache: BaseCache):
```

### Comparing `nonebot_plugin_bilichat-5.6.0/nonebot_plugin_bilichat/wordcloud.py` & `nonebot_plugin_bilichat-5.7.0/nonebot_plugin_bilichat/wordcloud.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 import asyncio
 from io import BytesIO
-from typing import Dict, Optional
 
 from jieba.analyse.tfidf import TFIDF
 from nonebot.log import logger
 from wordcloud import WordCloud
 
 from .config import plugin_config
 from .lib.cache import BaseCache
 from .lib.fonts_provider import get_font_async
 from .optional import capture_exception  # type: ignore
 
 tfidf = TFIDF()
 
 
-async def wordcloud(cache: BaseCache) -> Optional[bytes]:
+async def wordcloud(cache: BaseCache) -> bytes | None:
     try:
         logger.info(f"生成 {cache.id} 的词云")
         if not cache.content:
             return None
         elif not cache.jieba:
             loop = asyncio.get_running_loop()
             cache.jieba = await loop.run_in_executor(None, get_frequencies, cache.content)
@@ -26,15 +25,15 @@
         return await get_worldcloud_image(cache.jieba)
     except Exception as e:
         capture_exception()
         logger.exception(f"内容 {cache.id} 的词云生成失败: {e}")
         return None
 
 
-def get_frequencies(msg_list) -> Dict[str, float]:
+def get_frequencies(msg_list) -> dict[str, float]:
     text = "\n".join(msg_list)
     return dict(tfidf.extract_tags(text, topK=200, withWeight=True))
 
 
 async def get_worldcloud_image(frequencies):
     wc = WordCloud(
         font_path=str(await get_font_async()),
```

### Comparing `nonebot_plugin_bilichat-5.6.0/pyproject.toml` & `nonebot_plugin_bilichat-5.7.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-bilichat"
-version = "5.6.0"
+version = "5.7.0"
 description = "多种B站链接解析，视频词云，AI总结，你想要的都在 bilichat"
 authors = [
     { name = "djkcyl", email = "cyl@cyllive.cn" },
     { name = "Well404", email = "well_404@outlook.com" },
 ]
 dependencies = [
     "bilireq>=0.2.8",
@@ -17,15 +17,15 @@
     "dynrender-skia-opt>=0.3.8",
     "nonebot-plugin-apscheduler>=0.3.0",
     "packaging>=23.2",
     "python-multipart>=0.0.6",
     "nonebot-plugin-alconna>=0.42.3",
     "nonebot-plugin-auto-bot-selector>=0.2.0",
 ]
-requires-python = ">=3.8,<4.0"
+requires-python = ">=3.10,<4.0"
 readme = "README.md"
 
 [project.license]
 text = "AGPL3.0"
 
 [project.optional-dependencies]
 extra = [
```

### Comparing `nonebot_plugin_bilichat-5.6.0/PKG-INFO` & `nonebot_plugin_bilichat-5.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-bilichat
-Version: 5.6.0
+Version: 5.7.0
 Summary: 多种B站链接解析，视频词云，AI总结，你想要的都在 bilichat
 Author-Email: djkcyl <cyl@cyllive.cn>, Well404 <well_404@outlook.com>
 License: AGPL3.0
-Requires-Python: <4.0,>=3.8
+Requires-Python: <4.0,>=3.10
 Requires-Dist: bilireq>=0.2.8
 Requires-Dist: qrcode>=7.4.2
 Requires-Dist: pillow>=9.5.0
 Requires-Dist: lxml>=4.9.2
 Requires-Dist: nonebot-plugin-localstore>=0.4.1
 Requires-Dist: nonebot2[fastapi,websockets]>=2.0.0
 Requires-Dist: httpx>=0.24.1
@@ -226,25 +226,25 @@
 
 ### 指令配置项
 
 |          配置项           |   类型    |          默认值          |           说明            |
 | :-----------------------: | :-------: | :----------------------: | :-----------------------: |
 |  bilichat_command_to_me   |   bool    |           True           |    命令是否需要@机器人    |
 |    bilichat_cmd_start     |    str    |        "bilichat"        | 命令的起始词，可设置为空  |
-|   bilichat_cmd_add_sub    | List[str] |     ["订阅", "关注"]     |      "sub"命令的别名      |
-|  bilichat_cmd_remove_sub  | List[str] |     ["退订", "取关"]     |     "unsub"命令的别名     |
-|  bilichat_cmd_check_sub   | List[str] |   ["查看", "查看订阅"]   |     "check"命令的别名     |
-|  bilichat_cmd_reset_sub   | List[str] |   ["重置", "重置配置"]   |     "reset"命令的别名     |
-|    bilichat_cmd_at_all    | List[str] | ["全体成员", "at 全体"]  |     "atall"命令的别名     |
-|   bilichat_cmd_dynamic    | List[str] | ["动态通知", "动态订阅"] |    "dynamic"命令的别名    |
-|     bilichat_cmd_live     | List[str] | ["直播通知", "直播订阅"] |     "live"命令的别名      |
-| bilichat_cmd_checkdynamic | List[str] |       ["查看动态"]       | "checkdynamic" 命令的别名 |
-| bilichat_cmd_check_login  | List[str] |     ["查看登录账号"]     |  "checklogin" 命令的别名  |
-| bilichat_cmd_login_qrcode | List[str] |       ["扫码登录"]       |   "qrlogin" 命令的别名    |
-|    bilichat_cmd_logout    | List[str] |       ["登出账号"]       |    "logout" 命令的别名    |
+|   bilichat_cmd_add_sub    | list[str] |     ["订阅", "关注"]     |      "sub"命令的别名      |
+|  bilichat_cmd_remove_sub  | list[str] |     ["退订", "取关"]     |     "unsub"命令的别名     |
+|  bilichat_cmd_check_sub   | list[str] |   ["查看", "查看订阅"]   |     "check"命令的别名     |
+|  bilichat_cmd_reset_sub   | list[str] |   ["重置", "重置配置"]   |     "reset"命令的别名     |
+|    bilichat_cmd_at_all    | list[str] | ["全体成员", "at 全体"]  |     "atall"命令的别名     |
+|   bilichat_cmd_dynamic    | list[str] | ["动态通知", "动态订阅"] |    "dynamic"命令的别名    |
+|     bilichat_cmd_live     | list[str] | ["直播通知", "直播订阅"] |     "live"命令的别名      |
+| bilichat_cmd_checkdynamic | list[str] |       ["查看动态"]       | "checkdynamic" 命令的别名 |
+| bilichat_cmd_check_login  | list[str] |     ["查看登录账号"]     |  "checklogin" 命令的别名  |
+| bilichat_cmd_login_qrcode | list[str] |       ["扫码登录"]       |   "qrlogin" 命令的别名    |
+|    bilichat_cmd_logout    | list[str] |       ["登出账号"]       |    "logout" 命令的别名    |
 
 ### 基础信息配置项
 
 |            配置项            | 类型 | 默认值 |                        说明                        |
 | :--------------------------: | :--: | :----: | :------------------------------------------------: |
 |     bilichat_basic_info      | bool |  True  |                是否开启视频基本信息                |
 |  bilichat_basic_info_style   | str  |  Auto  |       视频详情的图片样式，可用样式见下方备注       |
@@ -296,15 +296,15 @@
 ### 词云配置项
 
 开启此功能需要安装对应的依赖 `nonebot-plugin-bilichat[wordcloud]`
 
 |          配置项          |   类型    |   默认值    |       说明       |
 | :----------------------: | :-------: | :---------: | :--------------: |
 |   bilichat_word_cloud    |   bool    |    False    | 是否开启词云功能 |
-| bilichat_word_cloud_size | List[int] | [1000, 800] |   词云图片尺寸   |
+| bilichat_word_cloud_size | list[int] | [1000, 800] |   词云图片尺寸   |
 
 ### AI 视频总结配置项
 
 开启此功能需要安装对应的依赖 `nonebot-plugin-bilichat[summary]`
 
 |            配置项            | 类型 |       默认值       |                                      说明                                      |
 | :--------------------------: | :--: | :----------------: | :----------------------------------------------------------------------------: |
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-bilichat Version: 5.6.0 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-bilichat Version: 5.7.0 Summary:
 å¤ç§Bç«é¾æ¥è§£æï¼è§é¢è¯äºï¼AIæ»ç»ï¼ä½ æ³è¦çé½å¨ bilichat
 Author-Email: djkcyl
 cyllive.cn>, Well404
-outlook.com> License: AGPL3.0 Requires-Python: <4.0,>=3.8 Requires-Dist:
+outlook.com> License: AGPL3.0 Requires-Python: <4.0,>=3.10 Requires-Dist:
 bilireq>=0.2.8 Requires-Dist: qrcode>=7.4.2 Requires-Dist: pillow>=9.5.0
 Requires-Dist: lxml>=4.9.2 Requires-Dist: nonebot-plugin-localstore>=0.4.1
 Requires-Dist: nonebot2[fastapi,websockets]>=2.0.0 Requires-Dist: httpx>=0.24.1
 Requires-Dist: dynrender-skia-opt>=0.3.8 Requires-Dist: nonebot-plugin-
 apscheduler>=0.3.0 Requires-Dist: packaging>=23.2 Requires-Dist: python-
 multipart>=0.0.6 Requires-Dist: nonebot-plugin-alconna>=0.42.3 Requires-Dist:
 nonebot-plugin-auto-bot-selector>=0.2.0 Requires-Dist: numpy<1.25.0,>=1.20.1;
@@ -96,28 +96,28 @@
 æ¬¡æ°æå åéåéè¯æ¥å°è¯éæ°çæå­å¹ 5. å½
 `bilichat_cache_serive` ä¸º `mongodb` æ¶ï¼éè¦å®è£å¹¶éç½® [nonebot-
 plugin-mongodb](https://github.com/Well2333/nonebot-plugin-mongodb)
 æå¯æ­£å¸¸ä½¿ç¨ ### æä»¤éç½®é¡¹ | éç½®é¡¹ | ç±»å | é»è®¤å¼ |
 è¯´æ | | :-----------------------: | :-------: | :----------------------: | :
 -----------------------: | | bilichat_command_to_me | bool | True |
 å½ä»¤æ¯å¦éè¦@æºå¨äºº | | bilichat_cmd_start | str | "bilichat" |
-å½ä»¤çèµ·å§è¯ï¼å¯è®¾ç½®ä¸ºç©º | | bilichat_cmd_add_sub | List[str] |
-["è®¢é", "å³æ³¨"] | "sub"å½ä»¤çå«å | | bilichat_cmd_remove_sub | List
+å½ä»¤çèµ·å§è¯ï¼å¯è®¾ç½®ä¸ºç©º | | bilichat_cmd_add_sub | list[str] |
+["è®¢é", "å³æ³¨"] | "sub"å½ä»¤çå«å | | bilichat_cmd_remove_sub | list
 [str] | ["éè®¢", "åå³"] | "unsub"å½ä»¤çå«å | |
-bilichat_cmd_check_sub | List[str] | ["æ¥ç", "æ¥çè®¢é"] |
-"check"å½ä»¤çå«å | | bilichat_cmd_reset_sub | List[str] | ["éç½®",
-"éç½®éç½®"] | "reset"å½ä»¤çå«å | | bilichat_cmd_at_all | List[str] |
+bilichat_cmd_check_sub | list[str] | ["æ¥ç", "æ¥çè®¢é"] |
+"check"å½ä»¤çå«å | | bilichat_cmd_reset_sub | list[str] | ["éç½®",
+"éç½®éç½®"] | "reset"å½ä»¤çå«å | | bilichat_cmd_at_all | list[str] |
 ["å¨ä½æå", "at å¨ä½"] | "atall"å½ä»¤çå«å | | bilichat_cmd_dynamic
-| List[str] | ["å¨æéç¥", "å¨æè®¢é"] | "dynamic"å½ä»¤çå«å | |
-bilichat_cmd_live | List[str] | ["ç´æ­éç¥", "ç´æ­è®¢é"] |
-"live"å½ä»¤çå«å | | bilichat_cmd_checkdynamic | List[str] |
+| list[str] | ["å¨æéç¥", "å¨æè®¢é"] | "dynamic"å½ä»¤çå«å | |
+bilichat_cmd_live | list[str] | ["ç´æ­éç¥", "ç´æ­è®¢é"] |
+"live"å½ä»¤çå«å | | bilichat_cmd_checkdynamic | list[str] |
 ["æ¥çå¨æ"] | "checkdynamic" å½ä»¤çå«å | | bilichat_cmd_check_login
-| List[str] | ["æ¥çç»å½è´¦å·"] | "checklogin" å½ä»¤çå«å | |
-bilichat_cmd_login_qrcode | List[str] | ["æ«ç ç»å½"] | "qrlogin"
-å½ä»¤çå«å | | bilichat_cmd_logout | List[str] | ["ç»åºè´¦å·"] |
+| list[str] | ["æ¥çç»å½è´¦å·"] | "checklogin" å½ä»¤çå«å | |
+bilichat_cmd_login_qrcode | list[str] | ["æ«ç ç»å½"] | "qrlogin"
+å½ä»¤çå«å | | bilichat_cmd_logout | list[str] | ["ç»åºè´¦å·"] |
 "logout" å½ä»¤çå«å | ### åºç¡ä¿¡æ¯éç½®é¡¹ | éç½®é¡¹ | ç±»å |
 é»è®¤å¼ | è¯´æ | | :--------------------------: | :--: | :----: | :--------
 ----------------------------------------: | | bilichat_basic_info | bool | True
 | æ¯å¦å¼å¯è§é¢åºæ¬ä¿¡æ¯ | | bilichat_basic_info_style | str | Auto |
 è§é¢è¯¦æçå¾çæ ·å¼ï¼å¯ç¨æ ·å¼è§ä¸æ¹å¤æ³¨ | |
 bilichat_basic_info_url | bool | True |
 å¼å¯è§é¢è¿æ¬ä¿¡æ¯çæåµä¸ï¼æ¯å¦ä¸ååå¤ä¸ä¸ªé¾æ¥ | |
@@ -138,15 +138,15 @@
 bilichat_use_browser ä¸º True æ Autoï¼ï¼å¶å¯ç¨çæ ·å¼å¦ä¸æç¤º
 dynamicrender ï¼æ æµè§å¨æ¶é»è®¤ï¼ ![](docs/dynamicrender.jpg)
 browser_mobile ï¼ææµè§å¨æ¶é»è®¤ï¼ ![](docs/dynamic_mobile.jpg)
 browser_pc ![](docs/dynamic_pc.jpg) ### è¯äºéç½®é¡¹
 å¼å¯æ­¤åè½éè¦å®è£å¯¹åºçä¾èµ `nonebot-plugin-bilichat[wordcloud]`
 | éç½®é¡¹ | ç±»å | é»è®¤å¼ | è¯´æ | | :----------------------: | :-----
 --: | :---------: | :--------------: | | bilichat_word_cloud | bool | False |
-æ¯å¦å¼å¯è¯äºåè½ | | bilichat_word_cloud_size | List[int] | [1000, 800]
+æ¯å¦å¼å¯è¯äºåè½ | | bilichat_word_cloud_size | list[int] | [1000, 800]
 | è¯äºå¾çå°ºå¯¸ | ### AI è§é¢æ»ç»éç½®é¡¹
 å¼å¯æ­¤åè½éè¦å®è£å¯¹åºçä¾èµ `nonebot-plugin-bilichat[summary]` |
 éç½®é¡¹ | ç±»å | é»è®¤å¼ | è¯´æ | | :--------------------------: | :--:
 | :----------------: | :-------------------------------------------------------
 ---------------------: | | bilichat_summary_ignore_null | bool | True |
 æ¯å¦å¿½ç¥æ æä¹çæ»ç»åå®¹ | | bilichat_official_summary | bool |
 False | æ¯å¦å¼å¯å®æ¹æ»ç»ï¼æ­¤æ»ç»ç¬ç«äºä¸æ¹ AI
```


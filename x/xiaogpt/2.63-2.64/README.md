# Comparing `tmp/xiaogpt-2.63.tar.gz` & `tmp/xiaogpt-2.64.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xiaogpt-2.63.tar", last modified: Sat Apr 20 13:44:29 2024, max compression
+gzip compressed data, was "xiaogpt-2.64.tar", last modified: Thu Apr 25 02:23:43 2024, max compression
```

## Comparing `xiaogpt-2.63.tar` & `xiaogpt-2.64.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1063 2024-04-20 13:44:25.301787 xiaogpt-2.63/LICENSE
--rw-r--r--   0        0        0    22390 2024-04-20 13:44:25.301787 xiaogpt-2.63/README.md
--rw-r--r--   0        0        0     3938 2024-04-20 13:44:29.009775 xiaogpt-2.63/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-20 13:44:25.305787 xiaogpt-2.63/xiaogpt/__init__.py
--rw-r--r--   0        0        0       61 2024-04-20 13:44:25.305787 xiaogpt-2.63/xiaogpt/__main__.py
--rw-r--r--   0        0        0     1006 2024-04-20 13:44:25.305787 xiaogpt-2.63/xiaogpt/bot/__init__.py
--rw-r--r--   0        0        0     1467 2024-04-20 13:44:25.305787 xiaogpt-2.63/xiaogpt/bot/base_bot.py
--rw-r--r--   0        0        0     3656 2024-04-20 13:44:25.305787 xiaogpt-2.63/xiaogpt/bot/chatgptapi_bot.py
--rw-r--r--   0        0        0     2773 2024-04-20 13:44:25.305787 xiaogpt-2.63/xiaogpt/bot/doubao_bot.py
--rw-r--r--   0        0        0     2516 2024-04-20 13:44:25.305787 xiaogpt-2.63/xiaogpt/bot/gemini_bot.py
--rw-r--r--   0        0        0     1825 2024-04-20 13:44:25.305787 xiaogpt-2.63/xiaogpt/bot/glm_bot.py
--rw-r--r--   0        0        0     1944 2024-04-20 13:44:25.305787 xiaogpt-2.63/xiaogpt/bot/langchain_bot.py
--rw-r--r--   0        0        0     2289 2024-04-20 13:44:25.305787 xiaogpt-2.63/xiaogpt/bot/newbing_bot.py
--rw-r--r--   0        0        0     3657 2024-04-20 13:44:25.305787 xiaogpt-2.63/xiaogpt/bot/qwen_bot.py
--rw-r--r--   0        0        0     4956 2024-04-20 13:44:25.305787 xiaogpt-2.63/xiaogpt/cli.py
--rw-r--r--   0        0        0     6535 2024-04-20 13:44:25.305787 xiaogpt-2.63/xiaogpt/config.py
--rw-r--r--   0        0        0     2616 2024-04-20 13:44:25.305787 xiaogpt-2.63/xiaogpt/langchain/callbacks.py
--rw-r--r--   0        0        0     1495 2024-04-20 13:44:25.305787 xiaogpt-2.63/xiaogpt/langchain/chain.py
--rw-r--r--   0        0        0     6372 2024-04-20 13:44:25.305787 xiaogpt-2.63/xiaogpt/langchain/examples/email/mail_box.py
--rw-r--r--   0        0        0     1561 2024-04-20 13:44:25.305787 xiaogpt-2.63/xiaogpt/langchain/examples/email/mail_summary_tools.py
--rw-r--r--   0        0        0      145 2024-04-20 13:44:25.305787 xiaogpt-2.63/xiaogpt/tts/__init__.py
--rw-r--r--   0        0        0     4656 2024-04-20 13:44:25.305787 xiaogpt-2.63/xiaogpt/tts/base.py
--rw-r--r--   0        0        0     1095 2024-04-20 13:44:25.305787 xiaogpt-2.63/xiaogpt/tts/mi.py
--rw-r--r--   0        0        0     1903 2024-04-20 13:44:25.305787 xiaogpt-2.63/xiaogpt/tts/tetos.py
--rw-r--r--   0        0        0     2072 2024-04-20 13:44:25.305787 xiaogpt-2.63/xiaogpt/utils.py
--rw-r--r--   0        0        0    15826 2024-04-20 13:44:25.305787 xiaogpt-2.63/xiaogpt/xiaogpt.py
--rw-r--r--   0        0        0    28355 1970-01-01 00:00:00.000000 xiaogpt-2.63/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-04-25 02:23:36.228737 xiaogpt-2.64/LICENSE
+-rw-r--r--   0        0        0    22689 2024-04-25 02:23:36.228737 xiaogpt-2.64/README.md
+-rw-r--r--   0        0        0     3938 2024-04-25 02:23:43.912794 xiaogpt-2.64/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-25 02:23:36.228737 xiaogpt-2.64/xiaogpt/__init__.py
+-rw-r--r--   0        0        0       61 2024-04-25 02:23:36.228737 xiaogpt-2.64/xiaogpt/__main__.py
+-rw-r--r--   0        0        0     1006 2024-04-25 02:23:36.228737 xiaogpt-2.64/xiaogpt/bot/__init__.py
+-rw-r--r--   0        0        0     1467 2024-04-25 02:23:36.228737 xiaogpt-2.64/xiaogpt/bot/base_bot.py
+-rw-r--r--   0        0        0     3656 2024-04-25 02:23:36.228737 xiaogpt-2.64/xiaogpt/bot/chatgptapi_bot.py
+-rw-r--r--   0        0        0     2773 2024-04-25 02:23:36.228737 xiaogpt-2.64/xiaogpt/bot/doubao_bot.py
+-rw-r--r--   0        0        0     2516 2024-04-25 02:23:36.228737 xiaogpt-2.64/xiaogpt/bot/gemini_bot.py
+-rw-r--r--   0        0        0     1825 2024-04-25 02:23:36.228737 xiaogpt-2.64/xiaogpt/bot/glm_bot.py
+-rw-r--r--   0        0        0     1944 2024-04-25 02:23:36.228737 xiaogpt-2.64/xiaogpt/bot/langchain_bot.py
+-rw-r--r--   0        0        0     2289 2024-04-25 02:23:36.228737 xiaogpt-2.64/xiaogpt/bot/newbing_bot.py
+-rw-r--r--   0        0        0     3657 2024-04-25 02:23:36.228737 xiaogpt-2.64/xiaogpt/bot/qwen_bot.py
+-rw-r--r--   0        0        0     4956 2024-04-25 02:23:36.228737 xiaogpt-2.64/xiaogpt/cli.py
+-rw-r--r--   0        0        0     6560 2024-04-25 02:23:36.228737 xiaogpt-2.64/xiaogpt/config.py
+-rw-r--r--   0        0        0     2616 2024-04-25 02:23:36.228737 xiaogpt-2.64/xiaogpt/langchain/callbacks.py
+-rw-r--r--   0        0        0     1495 2024-04-25 02:23:36.228737 xiaogpt-2.64/xiaogpt/langchain/chain.py
+-rw-r--r--   0        0        0     6372 2024-04-25 02:23:36.228737 xiaogpt-2.64/xiaogpt/langchain/examples/email/mail_box.py
+-rw-r--r--   0        0        0     1561 2024-04-25 02:23:36.228737 xiaogpt-2.64/xiaogpt/langchain/examples/email/mail_summary_tools.py
+-rw-r--r--   0        0        0      145 2024-04-25 02:23:36.228737 xiaogpt-2.64/xiaogpt/tts/__init__.py
+-rw-r--r--   0        0        0     4656 2024-04-25 02:23:36.228737 xiaogpt-2.64/xiaogpt/tts/base.py
+-rw-r--r--   0        0        0     1095 2024-04-25 02:23:36.228737 xiaogpt-2.64/xiaogpt/tts/mi.py
+-rw-r--r--   0        0        0     1058 2024-04-25 02:23:36.228737 xiaogpt-2.64/xiaogpt/tts/tetos.py
+-rw-r--r--   0        0        0     2072 2024-04-25 02:23:36.232737 xiaogpt-2.64/xiaogpt/utils.py
+-rw-r--r--   0        0        0    15960 2024-04-25 02:23:36.232737 xiaogpt-2.64/xiaogpt/xiaogpt.py
+-rw-r--r--   0        0        0    28654 1970-01-01 00:00:00.000000 xiaogpt-2.64/PKG-INFO
```

### Comparing `xiaogpt-2.63/LICENSE` & `xiaogpt-2.64/LICENSE`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.63/README.md` & `xiaogpt-2.64/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -74,15 +74,15 @@
 # 使用流式响应，获得更快的响应
 xiaogpt --hardware LX06  --mute_xiaoai --stream
 # 如果你想使用 google 的 gemini
 xiaogpt --hardware LX06  --mute_xiaoai --use_gemini --gemini_key ${gemini_key}
 # 如果你想使用自己的 google gemini 服务
 python3 xiaogpt.py --hardware LX06  --mute_xiaoai --use_gemini --gemini_key ${gemini_key} --gemini_api_domain ${gemini_api_domain}
 # 如果你想使用阿里的通义千问
-xiaogpt --hardware LX06  --mute_xiaoai --use_qwen --qen_key ${qwen_key}
+xiaogpt --hardware LX06  --mute_xiaoai --use_qwen --qwen_key ${qwen_key}
 # 如果你想使用豆包
 xiaogpt --hardware LX06  --mute_xiaoai --use_doubao --stream --volc_access_key xxxx --volc_secret_key xxx
 # 如果你想用 edge-tts
 xiaogpt --hardware LX06 --cookie ${cookie} --use_chatgpt_api --tts edge
 # 如果你想使用 LangChain + SerpApi 实现上网检索或其他本地服务（目前仅支持 stream 模式）
 export OPENAI_API_KEY=${your_api_key}
 export SERPAPI_API_KEY=${your_serpapi_key}
@@ -105,15 +105,15 @@
 # 如果你想使用 ChatGLM api
 python3 xiaogpt.py --hardware LX06  --mute_xiaoai --use_glm --glm_key ${glm_key}
 # 如果你想使用 google 的 gemini
 python3 xiaogpt.py --hardware LX06  --mute_xiaoai --use_gemini --gemini_key ${gemini_key}
 # 如果你想使用自己的 google gemini 服务
 python3 xiaogpt.py --hardware LX06  --mute_xiaoai --use_gemini --gemini_key ${gemini_key} --gemini_api_domain ${gemini_api_domain}
 # 如果你想使用阿里的通义千问
-python3 xiaogpt.py --hardware LX06  --mute_xiaoai --use_qwen --qen_key ${qwen_key}
+python3 xiaogpt.py --hardware LX06  --mute_xiaoai --use_qwen --qwen_key ${qwen_key}
 # 如果你想使用豆包
 python3 xiaogpt.py --hardware LX06  --mute_xiaoai --use_doubao --stream --volc_access_key xxxx --volc_secret_key xxx
 # 如果你想使用 LangChain+SerpApi 实现上网检索或其他本地服务（目前仅支持 stream 模式）
 export OPENAI_API_KEY=${your_api_key}
 export SERPAPI_API_KEY=${your_serpapi_key}
 python3 xiaogpt.py --hardware Lx06 --use_langchain --mute_xiaoai --stream --openai_key ${your_api_key} --serpapi_api_key ${your_serpapi_key}
 ```
@@ -151,47 +151,47 @@
 ```
 
 具体参数作用请参考 [Open AI API 文档](https://platform.openai.com/docs/api-reference/chat/create)。
 ChatGLM [文档](http://open.bigmodel.cn/doc/api#chatglm_130b)
 
 ## 配置项说明
 
-| 参数                  | 说明                                                                                        | 默认值                                                                                                    | 可选值                                                |
-| --------------------- | ------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------- | ----------------------------------------------------- |
-| hardware              | 设备型号                                                                                    |                                                                                                           |                                                       |
-| account               | 小爱账户                                                                                    |                                                                                                           |                                                       |
-| password              | 小爱账户密码                                                                                |                                                                                                           |                                                       |
-| openai_key            | openai的apikey                                                                              |                                                                                                           |                                                       |
-| serpapi_api_key       | serpapi的key 参考 [SerpAPI](https://serpapi.com/)                                           |                                                                                                           |                                                       |
-| glm_key               | chatglm 的 apikey                                                                           |                                                                                                           |                                                       |
-| gemini_key            | gemini 的 apikey [参考](https://makersuite.google.com/app/apikey)                           |                                                                                                           |                                                       |
-| gemini_api_domain            | gemini 的自定义域名 [参考](https://github.com/antergone/palm-netlify-proxy)                                                      |                                                                                                           |
-| qwen_key              | qwen 的 apikey [参考](https://help.aliyun.com/zh/dashscope/developer-reference/api-details) |                                                                                                           |                                                       |
-| cookie                | 小爱账户cookie （如果用上面密码登录可以不填）                                               |                                                                                                           |                                                       |
-| mi_did                | 设备did                                                                                     |                                                                                                           |                                                       |
-| use_command           | 使用 MI command 与小爱交互                                                                  | `false`                                                                                                   |                                                       |
-| mute_xiaoai           | 快速停掉小爱自己的回答                                                                      | `true`                                                                                                    |                                                       |
-| verbose               | 是否打印详细日志                                                                            | `false`                                                                                                   |                                                       |
-| bot                   | 使用的 bot 类型，目前支持 chatgptapi,newbing, qwen, gemini                                  | `chatgptapi`                                                                                              |                                                       |
-| tts                   | 使用的 TTS 类型                                                                             | `mi`                                                                                                      | `edge`、 `openai`、`azure`、`volc`、`baidu`、`google` |
-| tts_options           | TTS 参数字典，参考 [tetos](https://github.com/frostming/tetos) 获取可用参数                 |                                                                                                           |                                                       |
-| prompt                | 自定义prompt                                                                                | `请用100字以内回答`                                                                                       |                                                       |
-| keyword               | 自定义请求词列表                                                                            | `["请"]`                                                                                                  |                                                       |
-| change_prompt_keyword | 更改提示词触发列表                                                                          | `["更改提示词"]`                                                                                          |                                                       |
-| start_conversation    | 开始持续对话关键词                                                                          | `开始持续对话`                                                                                            |                                                       |
-| end_conversation      | 结束持续对话关键词                                                                          | `结束持续对话`                                                                                            |                                                       |
-| stream                | 使用流式响应，获得更快的响应                                                                | `false`                                                                                                   |                                                       |
-| proxy                 | 支持 HTTP 代理，传入 http proxy URL                                                         | ""                                                                                                        |                                                       |
-| gpt_options           | OpenAI API 的参数字典                                                                       | `{}`                                                                                                      |                                                       |
-| bing_cookie_path      | NewBing使用的cookie路径，参考[这里]获取                                                     | 也可通过环境变量 `COOKIE_FILE` 设置                                                                       |                                                       |
-| bing_cookies          | NewBing使用的cookie字典，参考[这里]获取                                                     |                                                                                                           |                                                       |
-| deployment_id         | Azure OpenAI 服务的 deployment ID                                                           | 参考这个[如何找到deployment_id](https://github.com/yihong0618/xiaogpt/issues/347#issuecomment-1784410784) |                                                       |
-| api_base              | 如果需要替换默认的api,或者使用Azure OpenAI 服务                                             | 例如：`https://abc-def.openai.azure.com/`                                                                 | 
-| volc_access_key       | 火山引擎的 access key 请在[这里](https://console.volcengine.com/iam/keymanage/)获取         |                                                                                                           |                                                       |
-| volc_secret_key       | 火山引擎的 secret key 请在[这里](https://console.volcengine.com/iam/keymanage/)获取         |                                                                                                           |                                                       |
+| 参数                  | 说明                                                                                        | 默认值                                                                                                    | 可选值                                                           |
+| --------------------- | ------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------- |
+| hardware              | 设备型号                                                                                    |                                                                                                           |                                                                  |
+| account               | 小爱账户                                                                                    |                                                                                                           |                                                                  |
+| password              | 小爱账户密码                                                                                |                                                                                                           |                                                                  |
+| openai_key            | openai的apikey                                                                              |                                                                                                           |                                                                  |
+| serpapi_api_key       | serpapi的key 参考 [SerpAPI](https://serpapi.com/)                                           |                                                                                                           |                                                                  |
+| glm_key               | chatglm 的 apikey                                                                           |                                                                                                           |                                                                  |
+| gemini_key            | gemini 的 apikey [参考](https://makersuite.google.com/app/apikey)                           |                                                                                                           |                                                                  |
+| gemini_api_domain     | gemini 的自定义域名 [参考](https://github.com/antergone/palm-netlify-proxy)                 |                                                                                                           |
+| qwen_key              | qwen 的 apikey [参考](https://help.aliyun.com/zh/dashscope/developer-reference/api-details) |                                                                                                           |                                                                  |
+| cookie                | 小爱账户cookie （如果用上面密码登录可以不填）                                               |                                                                                                           |                                                                  |
+| mi_did                | 设备did                                                                                     |                                                                                                           |                                                                  |
+| use_command           | 使用 MI command 与小爱交互                                                                  | `false`                                                                                                   |                                                                  |
+| mute_xiaoai           | 快速停掉小爱自己的回答                                                                      | `true`                                                                                                    |                                                                  |
+| verbose               | 是否打印详细日志                                                                            | `false`                                                                                                   |                                                                  |
+| bot                   | 使用的 bot 类型，目前支持 chatgptapi,newbing, qwen, gemini                                  | `chatgptapi`                                                                                              |                                                                  |
+| tts                   | 使用的 TTS 类型                                                                             | `mi`                                                                                                      | `edge`、 `openai`、`azure`、`volc`、`baidu`、`google`、`minimax` |
+| tts_options           | TTS 参数字典，参考 [tetos](https://github.com/frostming/tetos) 获取可用参数                 |                                                                                                           |                                                                  |
+| prompt                | 自定义prompt                                                                                | `请用100字以内回答`                                                                                       |                                                                  |
+| keyword               | 自定义请求词列表                                                                            | `["请"]`                                                                                                  |                                                                  |
+| change_prompt_keyword | 更改提示词触发列表                                                                          | `["更改提示词"]`                                                                                          |                                                                  |
+| start_conversation    | 开始持续对话关键词                                                                          | `开始持续对话`                                                                                            |                                                                  |
+| end_conversation      | 结束持续对话关键词                                                                          | `结束持续对话`                                                                                            |                                                                  |
+| stream                | 使用流式响应，获得更快的响应                                                                | `false`                                                                                                   |                                                                  |
+| proxy                 | 支持 HTTP 代理，传入 http proxy URL                                                         | ""                                                                                                        |                                                                  |
+| gpt_options           | OpenAI API 的参数字典                                                                       | `{}`                                                                                                      |                                                                  |
+| bing_cookie_path      | NewBing使用的cookie路径，参考[这里]获取                                                     | 也可通过环境变量 `COOKIE_FILE` 设置                                                                       |                                                                  |
+| bing_cookies          | NewBing使用的cookie字典，参考[这里]获取                                                     |                                                                                                           |                                                                  |
+| deployment_id         | Azure OpenAI 服务的 deployment ID                                                           | 参考这个[如何找到deployment_id](https://github.com/yihong0618/xiaogpt/issues/347#issuecomment-1784410784) |                                                                  |
+| api_base              | 如果需要替换默认的api,或者使用Azure OpenAI 服务                                             | 例如：`https://abc-def.openai.azure.com/`                                                                 |
+| volc_access_key       | 火山引擎的 access key 请在[这里](https://console.volcengine.com/iam/keymanage/)获取         |                                                                                                           |                                                                  |
+| volc_secret_key       | 火山引擎的 secret key 请在[这里](https://console.volcengine.com/iam/keymanage/)获取         |                                                                                                           |                                                                  |
 [这里]: https://github.com/acheong08/EdgeGPT#getting-authentication-required
 
 ## 注意
 
 1. 请开启小爱同学的蓝牙
 2. 如果要更改提示词和 PROMPT 在代码最上面自行更改
 3. 目前已知 LX04、X10A 和 L05B L05C 可能需要使用 `--use_command`，否则可能会出现终端能输出GPT的回复但小爱同学不回答GPT的情况。这几个型号也只支持小爱原本的 tts.
```

### Comparing `xiaogpt-2.63/pyproject.toml` & `xiaogpt-2.64/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -21,18 +21,18 @@
     "EdgeGPT==0.1.26",
     "langchain>=0.0.343",
     "beautifulsoup4>=4.12.0",
     "google-search-results>=2.4.2",
     "google-generativeai",
     "numexpr>=2.8.6",
     "dashscope>=1.10.0",
-    "tetos>=0.1.1",
+    "tetos>=0.2.1",
 ]
 dynamic = []
-version = "2.63"
+version = "2.64"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 Homepage = "https://github.com/yihong0618/xiaogpt"
 
@@ -116,15 +116,15 @@
     "rich==13.7.1",
     "rsa==4.9",
     "sniffio==1.3.0",
     "socksio==1.0.0",
     "soupsieve==2.5",
     "sqlalchemy==2.0.25",
     "tenacity==8.2.3",
-    "tetos==0.1.1",
+    "tetos==0.2.1",
     "tqdm==4.66.1",
     "typing-extensions==4.9.0",
     "typing-inspect==0.9.0",
     "uritemplate==4.1.1",
     "urllib3==2.1.0",
     "wcwidth==0.2.13",
     "websockets==12.0",
```

### Comparing `xiaogpt-2.63/xiaogpt/bot/__init__.py` & `xiaogpt-2.64/xiaogpt/bot/__init__.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.63/xiaogpt/bot/base_bot.py` & `xiaogpt-2.64/xiaogpt/bot/base_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.63/xiaogpt/bot/chatgptapi_bot.py` & `xiaogpt-2.64/xiaogpt/bot/chatgptapi_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.63/xiaogpt/bot/doubao_bot.py` & `xiaogpt-2.64/xiaogpt/bot/doubao_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.63/xiaogpt/bot/gemini_bot.py` & `xiaogpt-2.64/xiaogpt/bot/gemini_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.63/xiaogpt/bot/glm_bot.py` & `xiaogpt-2.64/xiaogpt/bot/glm_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.63/xiaogpt/bot/langchain_bot.py` & `xiaogpt-2.64/xiaogpt/bot/langchain_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.63/xiaogpt/bot/newbing_bot.py` & `xiaogpt-2.64/xiaogpt/bot/newbing_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.63/xiaogpt/bot/qwen_bot.py` & `xiaogpt-2.64/xiaogpt/bot/qwen_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.63/xiaogpt/cli.py` & `xiaogpt-2.64/xiaogpt/cli.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.63/xiaogpt/config.py` & `xiaogpt-2.64/xiaogpt/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,15 +72,17 @@
     api_base: str | None = None
     deployment_id: str | None = None
     use_command: bool = False
     verbose: bool = False
     start_conversation: str = "开始持续对话"
     end_conversation: str = "结束持续对话"
     stream: bool = False
-    tts: Literal["mi", "edge", "azure", "openai", "baidu", "google", "volc"] = "mi"
+    tts: Literal[
+        "mi", "edge", "azure", "openai", "baidu", "google", "volc", "minimax"
+    ] = "mi"
     tts_options: dict[str, Any] = field(default_factory=dict)
     gpt_options: dict[str, Any] = field(default_factory=dict)
     bing_cookie_path: str = ""
     bing_cookies: dict | None = None
 
     def __post_init__(self) -> None:
         if self.proxy:
```

### Comparing `xiaogpt-2.63/xiaogpt/langchain/callbacks.py` & `xiaogpt-2.64/xiaogpt/langchain/callbacks.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.63/xiaogpt/langchain/chain.py` & `xiaogpt-2.64/xiaogpt/langchain/chain.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.63/xiaogpt/langchain/examples/email/mail_box.py` & `xiaogpt-2.64/xiaogpt/langchain/examples/email/mail_box.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.63/xiaogpt/langchain/examples/email/mail_summary_tools.py` & `xiaogpt-2.64/xiaogpt/langchain/examples/email/mail_summary_tools.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.63/xiaogpt/tts/base.py` & `xiaogpt-2.64/xiaogpt/tts/base.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.63/xiaogpt/tts/mi.py` & `xiaogpt-2.64/xiaogpt/tts/mi.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.63/xiaogpt/utils.py` & `xiaogpt-2.64/xiaogpt/utils.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.63/xiaogpt/xiaogpt.py` & `xiaogpt-2.64/xiaogpt/xiaogpt.py`

 * *Files 1% similar despite different names*

```diff
@@ -414,13 +414,19 @@
         text = await text_stream.__anext__()
         # See if the first part contains language code(e.g. en-US|Hello world)
         lang, _, first_chunk = text.rpartition("|")
         if len(lang) > 7:
             # It is not a legal language code, discard it
             lang, first_chunk = "", text
 
+        lang = (
+            matches[0]
+            if (matches := re.findall(r"([a-z]{2}-[A-Z]{2})", lang))
+            else "zh-CN"
+        )
+
         async def gen():  # reconstruct the generator
             yield first_chunk
             async for text in text_stream:
                 yield text
 
-        await self.tts.synthesize(lang or "zh-CN", gen())
+        await self.tts.synthesize(lang, gen())
```

### Comparing `xiaogpt-2.63/PKG-INFO` & `xiaogpt-2.64/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xiaogpt
-Version: 2.63
+Version: 2.64
 Summary: Play ChatGPT or other LLM with xiaomi AI speaker
 Author-Email: yihong0618 <zouzou0208@gmail.com>
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Project-URL: Homepage, https://github.com/yihong0618/xiaogpt
@@ -18,15 +18,15 @@
 Requires-Dist: EdgeGPT==0.1.26
 Requires-Dist: langchain>=0.0.343
 Requires-Dist: beautifulsoup4>=4.12.0
 Requires-Dist: google-search-results>=2.4.2
 Requires-Dist: google-generativeai
 Requires-Dist: numexpr>=2.8.6
 Requires-Dist: dashscope>=1.10.0
-Requires-Dist: tetos>=0.1.1
+Requires-Dist: tetos>=0.2.1
 Requires-Dist: aiohttp==3.9.5; extra == "locked"
 Requires-Dist: aiosignal==1.3.1; extra == "locked"
 Requires-Dist: annotated-types==0.6.0; extra == "locked"
 Requires-Dist: anyio==4.3.0; extra == "locked"
 Requires-Dist: async-timeout==4.0.3; python_version < "3.11" and extra == "locked"
 Requires-Dist: attrs==23.2.0; extra == "locked"
 Requires-Dist: azure-cognitiveservices-speech==1.37.0; extra == "locked"
@@ -98,15 +98,15 @@
 Requires-Dist: rich==13.7.1; extra == "locked"
 Requires-Dist: rsa==4.9; extra == "locked"
 Requires-Dist: sniffio==1.3.0; extra == "locked"
 Requires-Dist: socksio==1.0.0; extra == "locked"
 Requires-Dist: soupsieve==2.5; extra == "locked"
 Requires-Dist: sqlalchemy==2.0.25; extra == "locked"
 Requires-Dist: tenacity==8.2.3; extra == "locked"
-Requires-Dist: tetos==0.1.1; extra == "locked"
+Requires-Dist: tetos==0.2.1; extra == "locked"
 Requires-Dist: tqdm==4.66.1; extra == "locked"
 Requires-Dist: typing-extensions==4.9.0; extra == "locked"
 Requires-Dist: typing-inspect==0.9.0; extra == "locked"
 Requires-Dist: uritemplate==4.1.1; extra == "locked"
 Requires-Dist: urllib3==2.1.0; extra == "locked"
 Requires-Dist: wcwidth==0.2.13; extra == "locked"
 Requires-Dist: websockets==12.0; extra == "locked"
@@ -191,15 +191,15 @@
 # 使用流式响应，获得更快的响应
 xiaogpt --hardware LX06  --mute_xiaoai --stream
 # 如果你想使用 google 的 gemini
 xiaogpt --hardware LX06  --mute_xiaoai --use_gemini --gemini_key ${gemini_key}
 # 如果你想使用自己的 google gemini 服务
 python3 xiaogpt.py --hardware LX06  --mute_xiaoai --use_gemini --gemini_key ${gemini_key} --gemini_api_domain ${gemini_api_domain}
 # 如果你想使用阿里的通义千问
-xiaogpt --hardware LX06  --mute_xiaoai --use_qwen --qen_key ${qwen_key}
+xiaogpt --hardware LX06  --mute_xiaoai --use_qwen --qwen_key ${qwen_key}
 # 如果你想使用豆包
 xiaogpt --hardware LX06  --mute_xiaoai --use_doubao --stream --volc_access_key xxxx --volc_secret_key xxx
 # 如果你想用 edge-tts
 xiaogpt --hardware LX06 --cookie ${cookie} --use_chatgpt_api --tts edge
 # 如果你想使用 LangChain + SerpApi 实现上网检索或其他本地服务（目前仅支持 stream 模式）
 export OPENAI_API_KEY=${your_api_key}
 export SERPAPI_API_KEY=${your_serpapi_key}
@@ -222,15 +222,15 @@
 # 如果你想使用 ChatGLM api
 python3 xiaogpt.py --hardware LX06  --mute_xiaoai --use_glm --glm_key ${glm_key}
 # 如果你想使用 google 的 gemini
 python3 xiaogpt.py --hardware LX06  --mute_xiaoai --use_gemini --gemini_key ${gemini_key}
 # 如果你想使用自己的 google gemini 服务
 python3 xiaogpt.py --hardware LX06  --mute_xiaoai --use_gemini --gemini_key ${gemini_key} --gemini_api_domain ${gemini_api_domain}
 # 如果你想使用阿里的通义千问
-python3 xiaogpt.py --hardware LX06  --mute_xiaoai --use_qwen --qen_key ${qwen_key}
+python3 xiaogpt.py --hardware LX06  --mute_xiaoai --use_qwen --qwen_key ${qwen_key}
 # 如果你想使用豆包
 python3 xiaogpt.py --hardware LX06  --mute_xiaoai --use_doubao --stream --volc_access_key xxxx --volc_secret_key xxx
 # 如果你想使用 LangChain+SerpApi 实现上网检索或其他本地服务（目前仅支持 stream 模式）
 export OPENAI_API_KEY=${your_api_key}
 export SERPAPI_API_KEY=${your_serpapi_key}
 python3 xiaogpt.py --hardware Lx06 --use_langchain --mute_xiaoai --stream --openai_key ${your_api_key} --serpapi_api_key ${your_serpapi_key}
 ```
@@ -268,47 +268,47 @@
 ```
 
 具体参数作用请参考 [Open AI API 文档](https://platform.openai.com/docs/api-reference/chat/create)。
 ChatGLM [文档](http://open.bigmodel.cn/doc/api#chatglm_130b)
 
 ## 配置项说明
 
-| 参数                  | 说明                                                                                        | 默认值                                                                                                    | 可选值                                                |
-| --------------------- | ------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------- | ----------------------------------------------------- |
-| hardware              | 设备型号                                                                                    |                                                                                                           |                                                       |
-| account               | 小爱账户                                                                                    |                                                                                                           |                                                       |
-| password              | 小爱账户密码                                                                                |                                                                                                           |                                                       |
-| openai_key            | openai的apikey                                                                              |                                                                                                           |                                                       |
-| serpapi_api_key       | serpapi的key 参考 [SerpAPI](https://serpapi.com/)                                           |                                                                                                           |                                                       |
-| glm_key               | chatglm 的 apikey                                                                           |                                                                                                           |                                                       |
-| gemini_key            | gemini 的 apikey [参考](https://makersuite.google.com/app/apikey)                           |                                                                                                           |                                                       |
-| gemini_api_domain            | gemini 的自定义域名 [参考](https://github.com/antergone/palm-netlify-proxy)                                                      |                                                                                                           |
-| qwen_key              | qwen 的 apikey [参考](https://help.aliyun.com/zh/dashscope/developer-reference/api-details) |                                                                                                           |                                                       |
-| cookie                | 小爱账户cookie （如果用上面密码登录可以不填）                                               |                                                                                                           |                                                       |
-| mi_did                | 设备did                                                                                     |                                                                                                           |                                                       |
-| use_command           | 使用 MI command 与小爱交互                                                                  | `false`                                                                                                   |                                                       |
-| mute_xiaoai           | 快速停掉小爱自己的回答                                                                      | `true`                                                                                                    |                                                       |
-| verbose               | 是否打印详细日志                                                                            | `false`                                                                                                   |                                                       |
-| bot                   | 使用的 bot 类型，目前支持 chatgptapi,newbing, qwen, gemini                                  | `chatgptapi`                                                                                              |                                                       |
-| tts                   | 使用的 TTS 类型                                                                             | `mi`                                                                                                      | `edge`、 `openai`、`azure`、`volc`、`baidu`、`google` |
-| tts_options           | TTS 参数字典，参考 [tetos](https://github.com/frostming/tetos) 获取可用参数                 |                                                                                                           |                                                       |
-| prompt                | 自定义prompt                                                                                | `请用100字以内回答`                                                                                       |                                                       |
-| keyword               | 自定义请求词列表                                                                            | `["请"]`                                                                                                  |                                                       |
-| change_prompt_keyword | 更改提示词触发列表                                                                          | `["更改提示词"]`                                                                                          |                                                       |
-| start_conversation    | 开始持续对话关键词                                                                          | `开始持续对话`                                                                                            |                                                       |
-| end_conversation      | 结束持续对话关键词                                                                          | `结束持续对话`                                                                                            |                                                       |
-| stream                | 使用流式响应，获得更快的响应                                                                | `false`                                                                                                   |                                                       |
-| proxy                 | 支持 HTTP 代理，传入 http proxy URL                                                         | ""                                                                                                        |                                                       |
-| gpt_options           | OpenAI API 的参数字典                                                                       | `{}`                                                                                                      |                                                       |
-| bing_cookie_path      | NewBing使用的cookie路径，参考[这里]获取                                                     | 也可通过环境变量 `COOKIE_FILE` 设置                                                                       |                                                       |
-| bing_cookies          | NewBing使用的cookie字典，参考[这里]获取                                                     |                                                                                                           |                                                       |
-| deployment_id         | Azure OpenAI 服务的 deployment ID                                                           | 参考这个[如何找到deployment_id](https://github.com/yihong0618/xiaogpt/issues/347#issuecomment-1784410784) |                                                       |
-| api_base              | 如果需要替换默认的api,或者使用Azure OpenAI 服务                                             | 例如：`https://abc-def.openai.azure.com/`                                                                 | 
-| volc_access_key       | 火山引擎的 access key 请在[这里](https://console.volcengine.com/iam/keymanage/)获取         |                                                                                                           |                                                       |
-| volc_secret_key       | 火山引擎的 secret key 请在[这里](https://console.volcengine.com/iam/keymanage/)获取         |                                                                                                           |                                                       |
+| 参数                  | 说明                                                                                        | 默认值                                                                                                    | 可选值                                                           |
+| --------------------- | ------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------- |
+| hardware              | 设备型号                                                                                    |                                                                                                           |                                                                  |
+| account               | 小爱账户                                                                                    |                                                                                                           |                                                                  |
+| password              | 小爱账户密码                                                                                |                                                                                                           |                                                                  |
+| openai_key            | openai的apikey                                                                              |                                                                                                           |                                                                  |
+| serpapi_api_key       | serpapi的key 参考 [SerpAPI](https://serpapi.com/)                                           |                                                                                                           |                                                                  |
+| glm_key               | chatglm 的 apikey                                                                           |                                                                                                           |                                                                  |
+| gemini_key            | gemini 的 apikey [参考](https://makersuite.google.com/app/apikey)                           |                                                                                                           |                                                                  |
+| gemini_api_domain     | gemini 的自定义域名 [参考](https://github.com/antergone/palm-netlify-proxy)                 |                                                                                                           |
+| qwen_key              | qwen 的 apikey [参考](https://help.aliyun.com/zh/dashscope/developer-reference/api-details) |                                                                                                           |                                                                  |
+| cookie                | 小爱账户cookie （如果用上面密码登录可以不填）                                               |                                                                                                           |                                                                  |
+| mi_did                | 设备did                                                                                     |                                                                                                           |                                                                  |
+| use_command           | 使用 MI command 与小爱交互                                                                  | `false`                                                                                                   |                                                                  |
+| mute_xiaoai           | 快速停掉小爱自己的回答                                                                      | `true`                                                                                                    |                                                                  |
+| verbose               | 是否打印详细日志                                                                            | `false`                                                                                                   |                                                                  |
+| bot                   | 使用的 bot 类型，目前支持 chatgptapi,newbing, qwen, gemini                                  | `chatgptapi`                                                                                              |                                                                  |
+| tts                   | 使用的 TTS 类型                                                                             | `mi`                                                                                                      | `edge`、 `openai`、`azure`、`volc`、`baidu`、`google`、`minimax` |
+| tts_options           | TTS 参数字典，参考 [tetos](https://github.com/frostming/tetos) 获取可用参数                 |                                                                                                           |                                                                  |
+| prompt                | 自定义prompt                                                                                | `请用100字以内回答`                                                                                       |                                                                  |
+| keyword               | 自定义请求词列表                                                                            | `["请"]`                                                                                                  |                                                                  |
+| change_prompt_keyword | 更改提示词触发列表                                                                          | `["更改提示词"]`                                                                                          |                                                                  |
+| start_conversation    | 开始持续对话关键词                                                                          | `开始持续对话`                                                                                            |                                                                  |
+| end_conversation      | 结束持续对话关键词                                                                          | `结束持续对话`                                                                                            |                                                                  |
+| stream                | 使用流式响应，获得更快的响应                                                                | `false`                                                                                                   |                                                                  |
+| proxy                 | 支持 HTTP 代理，传入 http proxy URL                                                         | ""                                                                                                        |                                                                  |
+| gpt_options           | OpenAI API 的参数字典                                                                       | `{}`                                                                                                      |                                                                  |
+| bing_cookie_path      | NewBing使用的cookie路径，参考[这里]获取                                                     | 也可通过环境变量 `COOKIE_FILE` 设置                                                                       |                                                                  |
+| bing_cookies          | NewBing使用的cookie字典，参考[这里]获取                                                     |                                                                                                           |                                                                  |
+| deployment_id         | Azure OpenAI 服务的 deployment ID                                                           | 参考这个[如何找到deployment_id](https://github.com/yihong0618/xiaogpt/issues/347#issuecomment-1784410784) |                                                                  |
+| api_base              | 如果需要替换默认的api,或者使用Azure OpenAI 服务                                             | 例如：`https://abc-def.openai.azure.com/`                                                                 |
+| volc_access_key       | 火山引擎的 access key 请在[这里](https://console.volcengine.com/iam/keymanage/)获取         |                                                                                                           |                                                                  |
+| volc_secret_key       | 火山引擎的 secret key 请在[这里](https://console.volcengine.com/iam/keymanage/)获取         |                                                                                                           |                                                                  |
 [这里]: https://github.com/acheong08/EdgeGPT#getting-authentication-required
 
 ## 注意
 
 1. 请开启小爱同学的蓝牙
 2. 如果要更改提示词和 PROMPT 在代码最上面自行更改
 3. 目前已知 LX04、X10A 和 L05B L05C 可能需要使用 `--use_command`，否则可能会出现终端能输出GPT的回复但小爱同学不回答GPT的情况。这几个型号也只支持小爱原本的 tts.
```


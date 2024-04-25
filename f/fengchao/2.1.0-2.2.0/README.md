# Comparing `tmp/fengchao-2.1.0.tar.gz` & `tmp/fengchao-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fengchao-2.1.0.tar", last modified: Wed Mar 13 07:37:45 2024, max compression
+gzip compressed data, was "fengchao-2.2.0.tar", last modified: Thu Apr 25 01:35:18 2024, max compression
```

## Comparing `fengchao-2.1.0.tar` & `fengchao-2.2.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 07:37:45.170378 fengchao-2.1.0/
--rw-r--r--   0 root         (0) root         (0)     1044 2024-02-26 05:39:20.000000 fengchao-2.1.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1232 2024-03-13 07:37:45.170378 fengchao-2.1.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    28342 2024-03-13 06:20:07.000000 fengchao-2.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 07:37:45.169378 fengchao-2.1.0/fengchao/
--rw-r--r--   0 root         (0) root         (0)      296 2024-03-06 03:21:37.000000 fengchao-2.1.0/fengchao/__init__.py
--rw-r--r--   0 root         (0) root         (0)      210 2024-03-13 06:55:39.000000 fengchao-2.1.0/fengchao/__version__.py
--rw-r--r--   0 root         (0) root         (0)      488 2024-03-13 06:12:25.000000 fengchao-2.1.0/fengchao/comments.py
--rw-r--r--   0 root         (0) root         (0)    19349 2024-03-13 05:57:25.000000 fengchao-2.1.0/fengchao/core.py
--rw-r--r--   0 root         (0) root         (0)     1007 2024-03-06 03:39:51.000000 fengchao-2.1.0/fengchao/examples.py
--rw-r--r--   0 root         (0) root         (0)     4188 2024-03-07 06:12:35.000000 fengchao-2.1.0/fengchao/protocol.py
--rw-r--r--   0 root         (0) root         (0)     1227 2024-03-06 07:29:31.000000 fengchao-2.1.0/fengchao/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 07:37:45.170378 fengchao-2.1.0/fengchao.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1232 2024-03-13 07:37:45.000000 fengchao-2.1.0/fengchao.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      349 2024-03-13 07:37:45.000000 fengchao-2.1.0/fengchao.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-13 07:37:45.000000 fengchao-2.1.0/fengchao.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       69 2024-03-13 07:37:45.000000 fengchao-2.1.0/fengchao.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-03-13 07:37:45.000000 fengchao-2.1.0/fengchao.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-13 07:37:45.170378 fengchao-2.1.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     4405 2024-03-06 06:36:37.000000 fengchao-2.1.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 07:37:45.170378 fengchao-2.1.0/test/
--rw-r--r--   0 root         (0) root         (0)     5765 2024-02-28 09:08:44.000000 fengchao-2.1.0/test/test_example.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 01:35:18.018903 fengchao-2.2.0/
+-rw-r--r--   0 root         (0) root         (0)     1050 2024-03-04 06:08:30.000000 fengchao-2.2.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1271 2024-04-25 01:35:18.018903 fengchao-2.2.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    30196 2024-04-24 01:54:29.000000 fengchao-2.2.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 01:35:18.017903 fengchao-2.2.0/fengchao/
+-rw-r--r--   0 root         (0) root         (0)      296 2024-03-06 06:59:50.000000 fengchao-2.2.0/fengchao/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      210 2024-04-24 01:54:29.000000 fengchao-2.2.0/fengchao/__version__.py
+-rw-r--r--   0 root         (0) root         (0)     1046 2024-04-24 01:54:29.000000 fengchao-2.2.0/fengchao/comments.py
+-rw-r--r--   0 root         (0) root         (0)    20260 2024-04-24 01:54:29.000000 fengchao-2.2.0/fengchao/core.py
+-rw-r--r--   0 root         (0) root         (0)     1043 2024-03-06 06:59:50.000000 fengchao-2.2.0/fengchao/examples.py
+-rw-r--r--   0 root         (0) root         (0)     4188 2024-03-07 06:13:49.000000 fengchao-2.2.0/fengchao/protocol.py
+-rw-r--r--   0 root         (0) root         (0)     1227 2024-03-06 07:33:13.000000 fengchao-2.2.0/fengchao/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 01:35:18.017903 fengchao-2.2.0/fengchao.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1271 2024-04-25 01:35:17.000000 fengchao-2.2.0/fengchao.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      349 2024-04-25 01:35:17.000000 fengchao-2.2.0/fengchao.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-25 01:35:17.000000 fengchao-2.2.0/fengchao.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       69 2024-04-25 01:35:17.000000 fengchao-2.2.0/fengchao.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-04-25 01:35:17.000000 fengchao-2.2.0/fengchao.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-25 01:35:18.018903 fengchao-2.2.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     4405 2024-03-06 06:59:50.000000 fengchao-2.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 01:35:18.017903 fengchao-2.2.0/test/
+-rw-r--r--   0 root         (0) root         (0)     5810 2024-03-18 08:04:59.000000 fengchao-2.2.0/test/test_example.py
```

### Comparing `fengchao-2.1.0/LICENSE` & `fengchao-2.2.0/LICENSE`

 * *Ordering differences only*

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-Copyright 2024 zhang
-
-Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
-
+Copyright 2024 zhang
+
+Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `fengchao-2.1.0/PKG-INFO` & `fengchao-2.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fengchao
-Version: 2.1.0
+Version: 2.2.0
 Summary: 大模型框架服务调用SDK.
 Home-page: 
 Author: ijiwei
 Author-email: 
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -47,7 +47,10 @@
 * 支持外网
 
 ### v2.0.4
 * 增加花费数据
 
 ### v2.1.0
 * 增加敏感词替换功能
+
+### v2.2.0
+* 增加文件上传功能
```

### Comparing `fengchao-2.1.0/README.md` & `fengchao-2.2.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -15,36 +15,48 @@
 | 查看知识库列表    |  否   |   否    |
 | 对话服务：同步对话  |  是   |   是    |
 | 对话服务：异步对话  |  是   |   是    |
 | 对话服务：异步结果  |  是   |   是    |
 | 对话服务：流式对话  |  是   |   是    |
 
 ### 支持的模型
-| 模型                          | 是否第三方 |
-|-----------------------------|:-----:|
-| glm-4                       |   是   |
-| gpt-3.5-turbo               |   是   |
-| gpt-3.5-turbo-1106          |   是   |
-| gpt-3.5-turbo-16k           |   是   |
-| gpt-3.5-turbo-16k-0613      |   是   |
-| Qwen1.5-0.5B-Chat           |   否   |
-| Qwen1.5-1.8B-Chat           |   否   |
-| ERNIE-Bot-4                 |   是   |
-| ERNIE-Bot-8k                |   是   |
-| ERNIE-Bot                   |   是   |
-| ERNIE-Bot-turbo             |   是   |
-| BLOOMZ-7B                   |   是   |
-| Llama-2-7b-chat             |   是   |
-| Llama-2-13b-chat            |   是   |
-| Llama-2-70b-chat            |   是   |
-| Mixtral-8x7B-Instruct       |   是   |
-| Qianfan-Chinese-Llama-2-7B  |   是   |
-| Qianfan-Chinese-Llama-2-13B |   是   |
-| claude-3-opus-20240229      |   是   |
-| claude-3-sonnet-20240229    |   是   |
+| 模型                          | 是否第三方 | 支持文件上传 |
+|-----------------------------|:-----:|:------:|
+| glm-4                       |   是   |   否    |
+| gpt-3.5-turbo               |   是   |   否    |
+| gpt-3.5-turbo-1106          |   是   |   否    |
+| gpt-3.5-turbo-16k           |   是   |   否    |
+| gpt-3.5-turbo-16k-0613      |   是   |   否    |
+| Qwen1.5-0.5B-Chat           |   否   |   否    |
+| Qwen1.5-1.8B-Chat           |   否   |   否    |
+| ERNIE-Bot-4                 |   是   |   否    |
+| ERNIE-Bot-8k                |   是   |   否    |
+| ERNIE-Bot                   |   是   |   否    |
+| ERNIE-Bot-turbo             |   是   |   否    |
+| BLOOMZ-7B                   |   是   |   否    |
+| Llama-2-7b-chat             |   是   |   否    |
+| Llama-2-13b-chat            |   是   |   否    |
+| Llama-2-70b-chat            |   是   |   否    |
+| Mixtral-8x7B-Instruct       |   是   |   否    |
+| Qianfan-Chinese-Llama-2-7B  |   是   |   否    |
+| Qianfan-Chinese-Llama-2-13B |   是   |   否    |
+| claude-3-opus-20240229      |   是   |   否    |
+| claude-3-sonnet-20240229    |   是   |   否    |
+| skylark-lite-public         |   是   |   否    |
+| skylark-plus-public         |   是   |   否    |
+| skylark-pro-public          |   是   |   否    |
+| skylark-chat                |   是   |   否    |
+| Skylark2-lite-8k            |   是   |   否    |
+| Skylark2-pro-4k             |   是   |   否    |
+| Skylark2-pro-character-4k   |   是   |   否    |
+| Skylark2-pro-32k            |   是   |   否    |
+| Skylark2-pro-turbo-8k       |   是   |   否    |
+| moonshot-v1-8k              |   是   |   是    |
+| moonshot-v1-32k             |   是   |   是    |
+| moonshot-v1-128k            |   是   |   是    |
 
 
 ### 支持的指令
 
 #### 默认的system描述：
 你是一个乐于助人、尊重他人、诚实的INTP-T人工智能助理，名叫jiweiGPT。你在和一个人类用户说话。在安全的情况下，总是尽可能地给出有帮助的、合乎逻辑的回答。
 你的回答不应包括任何有害、政治、宗教、不道德、种族主义、性别歧视、有毒、危险或非法的内容。请确保你的回答是社会公正和积极的。如果一个问题没有任何意义，
@@ -532,14 +544,42 @@
 ##### 响应参数说明：
 | 字段       | 描述     |
 |----------|--------|
 | id       | 知识库名称  |
 | desc     | 知识库描述  |
 | created  | 创建时间   |
 
+### 上传文件
+
+##### 请求方式：POST
+##### 请求地址：/aigc/uploadfiles/
+##### 请求参数：
+```python
+import requests
+from pathlib import Path
+files = ["file_path1", "file_path2"]
+files = [('files', (Path(file).name, open(file, 'rb'), "application/json")) for file in files]
+response = requests.post("http://127.0.0.1:5000/aigc/uploadfiles/", files=files)
+```
+
+##### 响应参数示例：
+```json
+{
+    "files": [],
+    "msg": "执行成功",
+    "status": 200
+}
+```
+##### 响应参数说明：
+| 字段     | 描述       |
+|--------|----------|
+| status | 状态码      |
+| msg    | 描述信息     |
+| files  | 上传后的文件名  |
+
 ### 对话服务
 
 ##### 请求方式：POST
 ##### 在线模型请求地址：/aigc/chat/
 ##### 本地模型请求地址：/aigc/local_chat/
 ##### 请求参数：参考【请求参数说明】
 ##### 响应示例
@@ -570,34 +610,35 @@
 ```
 ##### 响应参数说明：参考【响应参数说明】
 
 </details>
 <br/>
 <details><summary style="font-size: large">请求参数说明</summary>
 
-| 字段                | 必填 | 描述                                                                                                                                                                   | 默认     |
-|-------------------|----|----------------------------------------------------------------------------------------------------------------------------------------------------------------------|--------|
-| model             | 是  | 模型名称，支持的模型通过查看模型列表服务查询，id即为模型的名称                                                                                                                                     |        |
-| query             | 否  | 问题,非异步结果调用时不能为空                                                                                                                                                      | None   |
-| request_id        | 否  | 请求ID，如果未设置则会随机生成，同一上下文对话request_id应保持一致，建议自行设置，也可以将第一次对话返回的request_id作为后续请求的参数。                                                                                      | 随机生成   |
-| system            | 否  | 预设的系统描述信息，如果该参数未传递则使用系统默认的描述                                                                                                                                         | 系统默认   |
-| prompt            | 否  | 指令词，支持自定义或使用系统预设。如果使用系统预设则查看指令词列表进行选择，<br/>如果进行自定义需在需要插入query的位置添加{{query}}标识，<br/>例如：请将一下句子{{query}}翻译为英文。                                                          | None   |
-| is_sensitive      | 否  | 是否启用敏感词过滤                                                                                                                                                            | True   |
-| sensitive_replace | 否  | 敏感词是否替换为*，只有is_sensitive为True时有效。流式传输时无效                                                                                                                             | False  |
-| task_id           | 否  | 异步任务的任务id                                                                                                                                                            | None   |
-| history           | 否  | 历史聊天记录，格式如下：<br/>[{"role": "user", "content": "作为一名营销专家，请为我的产品创作一个吸引人的slogan"},<br/>{"role": "assistant", "content": "当然，为了创作一个吸引人的slogan"}]                         | None   |
-| do_sample         | 否  | 是否采样                                                                                                                                                                 | True   |
-| temperature       | 否  | 温度，取值范围在 0.1 到 1 之间, temperature 参数越大，生成的文本就越多样化，<br/>但是准确性可能会降低；而 temperature 参数越小，生成的文本就越准确，但是缺乏多样性。                                                               | 0.8    |
-| top_p             | 否  | top_p参数，也被称为nucleus sampling，是文本生成策略中的一种方法。在这种方法中，<br/>模型会生成一组候选token，然后从累计概率达到或超过p的token中随机选择一个作为输出。<br/>例如，如果top_p设为0.9，那么模型会选择一组最可能的token，这些token的累计概率达到或超过0.9。   | 0.75   |
-| max_tokens        | 否  | 生成文本最大长度                                                                                                                                                             | 256    |
-| mode              | 否  | 选择模式，同步：invoke，异步：async，异步结果：async_result，流式：stream                                                                                                                  | invoke |
-| knowledge         | 否  | 选择知识库，通过知识库接口查看支持的知识库,默认不使用知识库                                                                                                                                       | None   |
-| top_k             | 否  | 知识库参数，命中知识数量                                                                                                                                                         | 5      |
-| threshold         | 否  | 知识库参数，阈值，数值范围约为0-1100，如果为0，则不生效，经测试设置为小于500时，匹配结果更精准                                                                                                                 | 500    |
-| retry_action      | 否  | 自定义重试操作行为，需继承Retry类，重写其中的方法                                                                                                                                          | None   |
+| 字段                | 必填 | 描述                                                                                                                                                                 | 默认     |
+|-------------------|----|--------------------------------------------------------------------------------------------------------------------------------------------------------------------|--------|
+| model             | 是  | 模型名称，支持的模型通过查看模型列表服务查询，id即为模型的名称                                                                                                                                   |        |
+| query             | 否  | 问题,非异步结果调用时不能为空                                                                                                                                                    | None   |
+| request_id        | 否  | 请求ID，如果未设置则会随机生成，同一上下文对话request_id应保持一致，建议自行设置，也可以将第一次对话返回的request_id作为后续请求的参数。                                                                                    | 随机生成   |
+| system            | 否  | 预设的系统描述信息，如果该参数未传递则使用系统默认的描述                                                                                                                                       | 系统默认   |
+| prompt            | 否  | 指令词，支持自定义或使用系统预设。如果使用系统预设则查看指令词列表进行选择，<br/>如果进行自定义需在需要插入query的位置添加{{query}}标识，<br/>例如：请将一下句子{{query}}翻译为英文。                                                        | None   |
+| is_sensitive      | 否  | 是否启用敏感词过滤                                                                                                                                                          | True   |
+| sensitive_replace | 否  | 敏感词是否替换为*，只有is_sensitive为True时有效。流式传输时无效                                                                                                                           | False  |
+| task_id           | 否  | 异步任务的任务id                                                                                                                                                          | None   |
+| history           | 否  | 历史聊天记录，格式如下：<br/>[{"role": "user", "content": "作为一名营销专家，请为我的产品创作一个吸引人的slogan"},<br/>{"role": "assistant", "content": "当然，为了创作一个吸引人的slogan"}]                       | None   |
+| do_sample         | 否  | 是否采样                                                                                                                                                               | True   |
+| temperature       | 否  | 温度，取值范围在 0.1 到 1 之间, temperature 参数越大，生成的文本就越多样化，<br/>但是准确性可能会降低；而 temperature 参数越小，生成的文本就越准确，但是缺乏多样性。                                                             | 0.8    |
+| top_p             | 否  | top_p参数，也被称为nucleus sampling，是文本生成策略中的一种方法。在这种方法中，<br/>模型会生成一组候选token，然后从累计概率达到或超过p的token中随机选择一个作为输出。<br/>例如，如果top_p设为0.9，那么模型会选择一组最可能的token，这些token的累计概率达到或超过0.9。 | 0.75   |
+| max_tokens        | 否  | 生成文本最大长度                                                                                                                                                           | 256    |
+| mode              | 否  | 选择模式，同步：invoke，异步：async，异步结果：async_result，流式：stream                                                                                                                | invoke |
+| knowledge         | 否  | 选择知识库，通过知识库接口查看支持的知识库,默认不使用知识库                                                                                                                                     | None   |
+| top_k             | 否  | 知识库参数，命中知识数量                                                                                                                                                       | 5      |
+| threshold         | 否  | 知识库参数，阈值，数值范围约为0-1100，如果为0，则不生效，经测试设置为小于500时，匹配结果更精准                                                                                                               | 500    |
+| retry_action      | 否  | 自定义重试操作行为，需继承Retry类，重写其中的方法                                                                                                                                        | None   |
+| files             | 否  | 需要上传的文件，如果是API方式调用，需要先调用/aigc/uploadfiles/接口，返回结果中的files字段为该字段的值。如果为SDK调用该值为本地文件路径。                                                                                | None   |
 
 </details>
 <br/>
 <details><summary style="font-size: large">响应参数说明</summary>
 
 | 字段                | 描述                  |
 |-------------------|---------------------|
```

### Comparing `fengchao-2.1.0/fengchao/core.py` & `fengchao-2.2.0/fengchao/core.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,21 +5,22 @@
 # Author     ：andy
 # version    ：python 3.9
 """
 import json
 import sys
 import uuid
 from typing import Union, Generator, Optional
+from pathlib import Path
 from urllib.parse import urljoin
 
 import requests
 from loguru import logger
 from tenacity import retry, stop_after_attempt
 
-from .comments import Comments
+from .comments import Comments, file_type
 from .protocol import ModelCard, ModelList, FinalResponse, PromptCard, PromptList, KGList, KGCard, \
     ChatCompletionResponseChoice, ChatMessage, ChatCompletionResponseUsage, ChatCompletionResponse
 from .utils import create_token, Retry
 
 
 class Base:
     def __init__(self, api_key: str, secret_key: str, base_url: str, logger_level: str):
@@ -52,14 +53,23 @@
         @_retry
         def _do():
             path_url = urljoin(self.base_url, url)
             response = requests.request(method, path_url, json=payload, headers=headers, stream=stream, timeout=Comments.TIMEOUT)
             return response
         return _do()
 
+    @retry(stop=stop_after_attempt(Comments.RETRY.retry_num))
+    def upload_file(self, files):
+        if isinstance(files, str):
+            files = [files]
+        files = [('files', (Path(file).name, open(file, 'rb'), file_type.get(Path(file).suffix, file_type.get('*')))) for file in files]
+        response = requests.post(urljoin(self.base_url, Comments.UPLOAD_URL), files=files)
+        return json.loads(response.text)
+
+
     def models(self) -> FinalResponse:
         """
         查看支持的模型列表
         :return:
         """
         headers = {
             "content-type": "application/json"
@@ -227,26 +237,30 @@
                         else: # 响应异常
                             yield FinalResponse(status=result.status, msg=result.msg, data=result)
             else: # 请求异常
                 yield FinalResponse(status=response.status_code, msg=response.text)
 
     def prepare_args(self, model, query ,request_id ,system, prompt ,is_sensitive, sensitive_replace, task_id,
                            history, do_sample ,temperature, top_p, max_tokens, mode, knowledge,
-                           top_k, threshold, try_num, timeout, retry_action):
+                           top_k, threshold, try_num, timeout, retry_action, files):
         token = create_token(self.api_key, self.secret_key)
         if timeout is not None:
             Comments.TIMEOUT = timeout
         if try_num is not None:
             Comments.RETRY.retry_num = try_num
         if history is None:
             history = []
         if request_id is None:
             request_id = uuid.uuid1().__str__()
         if retry_action is not None:
             Comments.RETRY = retry_action
+        if files:
+            response = self.upload_file(files)
+            if response['status'] == 200:
+                files = response['files']
         if mode == 'async_result' and task_id is None: raise ValueError("task_id不能为空")
         headers = {
             "content-type": "application/json",
             "Authorization": token
         }
         payload = {
             'model': model,
@@ -261,15 +275,16 @@
             'do_sample': do_sample,
             'temperature': temperature,
             'top_p': top_p,
             'max_tokens': max_tokens,
             'knowledge': knowledge,
             'top_k': top_k,
             'threshold': threshold,
-            'mode': mode
+            'mode': mode,
+            'files': files
         }
         url = Comments.LOCAL_URL if self.check_model_channel(model) == "本地模型" else Comments.ONLINE_URL
         return headers, payload, url
 
 
 class FengChao(Base):
     def __init__(self, api_key: str, secret_key: str, base_url: str = Comments.BASE_URL, logger_level: str = 'INFO'):
@@ -299,15 +314,16 @@
              max_tokens: int =256,
              mode: str ='invoke',
              knowledge: Optional[str]=None,
              top_k: int =5,
              threshold: int=500,
              try_num: Optional[int] = None,
              timeout: Optional[int] = None,
-             retry_action: Optional[Retry] = None) -> Union[FinalResponse, Generator]:
+             retry_action: Optional[Retry] = None,
+             files: Optional[Union[list, str]] = None) -> Union[FinalResponse, Generator]:
         """
         创建对话服务
         :param model: 选择模型，具体查看models()函数
         :param query: 请求问题
         :param request_id: 请求ID
         :param system: 系统描述信息
         :param prompt: 指令描述信息
@@ -322,19 +338,20 @@
         :param mode: 选择对话模式，同步：invoke，异步：async，异步结果：async_result，流式：stream。默认：invoke
         :param knowledge: 选择要使用的知识库，默认：None
         :param top_k: 知识库参数，命中知识数量
         :param threshold: 知识库参数，阈值，数值范围约为0-1100，如果为0，则不生效，经测试设置为小于500时，匹配结果更精准
         :param try_num: 请求失败重试次数，默认：3
         :param timeout: 请求超时时间，单位秒，默认：600
         :param retry_action: 自定义重试操作行为，需继承Retry类，重写其中的方法
+        :param files: 需要上传的文件，文件地址
         :return:
         """
         headers, payload, url = self.prepare_args(model, query ,request_id ,system, prompt ,is_sensitive, sensitive_replace,
                                                   task_id, history, do_sample ,temperature, top_p, max_tokens, mode, knowledge,
-                                                top_k, threshold, try_num, timeout, retry_action)
+                                                top_k, threshold, try_num, timeout, retry_action, files)
         if mode == 'invoke':
             return self.invoke_chat(url, headers, payload)
         elif mode == 'async':
             return self.async_invoke_chat(url, headers, payload)
         elif mode == 'async_result':
             return self.invoke_chat(url, headers, payload)
         elif mode == 'stream':
@@ -379,15 +396,16 @@
              max_tokens: int =256,
              mode: str ='invoke',
              knowledge: Optional[str]=None,
              top_k: int =5,
              threshold: int=500,
              try_num: Optional[int] = None,
              timeout: Optional[int] = None,
-             retry_action: Optional[Retry] = None) -> Union[FinalResponse, Generator]:
+             retry_action: Optional[Retry] = None,
+             files: Optional[Union[list, str]] = None) -> Union[FinalResponse, Generator]:
         """
         创建对话服务
         :param model: 选择模型，具体查看models()函数
         :param query: 请求问题
         :param request_id: 请求ID
         :param system: 系统描述信息
         :param prompt: 指令描述信息
@@ -402,19 +420,20 @@
         :param mode: 选择对话模式，同步：invoke，异步：async，异步结果：async_result，流式：stream。默认：invoke
         :param knowledge: 选择要使用的知识库，默认：None
         :param top_k: 知识库参数，命中知识数量
         :param threshold: 知识库参数，阈值，数值范围约为0-1100，如果为0，则不生效，经测试设置为小于500时，匹配结果更精准
         :param try_num: 请求失败重试次数，默认：3
         :param timeout: 请求超时时间，单位秒，默认：600
         :param retry_action: 自定义重试操作行为，需继承Retry类，重写其中的方法
+        :param files: 需要上传的文件，文件地址
         :return:
         """
         headers, payload, url = self.prepare_args(model, query, request_id, system, prompt, is_sensitive, sensitive_replace,
                                                   task_id, history, do_sample, temperature, top_p, max_tokens, mode, knowledge,
-                                                  top_k, threshold, try_num, timeout, retry_action)
+                                                  top_k, threshold, try_num, timeout, retry_action, files)
         if mode == 'invoke':
             result = await self.invoke_chat(url, headers, payload)
             return result
         elif mode == 'async':
             result = await self.async_invoke_chat(url, headers, payload)
             return result
         elif mode == 'async_result':
```

### Comparing `fengchao-2.1.0/fengchao/protocol.py` & `fengchao-2.2.0/fengchao/protocol.py`

 * *Files identical despite different names*

### Comparing `fengchao-2.1.0/fengchao/utils.py` & `fengchao-2.2.0/fengchao/utils.py`

 * *Files identical despite different names*

### Comparing `fengchao-2.1.0/fengchao.egg-info/PKG-INFO` & `fengchao-2.2.0/fengchao.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fengchao
-Version: 2.1.0
+Version: 2.2.0
 Summary: 大模型框架服务调用SDK.
 Home-page: 
 Author: ijiwei
 Author-email: 
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -47,7 +47,10 @@
 * 支持外网
 
 ### v2.0.4
 * 增加花费数据
 
 ### v2.1.0
 * 增加敏感词替换功能
+
+### v2.2.0
+* 增加文件上传功能
```

### Comparing `fengchao-2.1.0/setup.py` & `fengchao-2.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `fengchao-2.1.0/test/test_example.py` & `fengchao-2.2.0/test/test_example.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 models_url = "http://192.168.1.233:5014/models/"
 prompts_url = "http://192.168.1.233:5014/prompts/"
 kgs_url = "http://192.168.1.233:5014/kgs/"
 token=None
 effective_time=-1
 test_case = [("Qwen1.5-0.5B-Chat", local_url),
              ("Qwen1.5-1.8B-Chat", local_url),
+             ("gpt-3.5-turbo", online_url),
              ("ERNIE-Bot-4", online_url),
              ("ERNIE-Bot-8k", online_url),
              ("ERNIE-Bot", online_url),
              ("ERNIE-Bot-turbo", online_url),
              ("BLOOMZ-7B", online_url),
              ("Llama-2-7b-chat", online_url),
              ("Llama-2-13b-chat", online_url),
```


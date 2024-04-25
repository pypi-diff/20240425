# Comparing `tmp/tencentcloud-sdk-python-hunyuan-3.0.1136.tar.gz` & `tmp/tencentcloud-sdk-python-hunyuan-3.0.1137.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-hunyuan-3.0.1136.tar", last modified: Wed Apr 24 20:41:21 2024, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-hunyuan-3.0.1137.tar", last modified: Thu Apr 25 20:52:12 2024, max compression
```

## Comparing `tencentcloud-sdk-python-hunyuan-3.0.1136.tar` & `tencentcloud-sdk-python-hunyuan-3.0.1137.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 20:41:21.000000 tencentcloud-sdk-python-hunyuan-3.0.1136/
--rw-r--r--   0 root         (0) root         (0)     1680 2024-04-24 20:41:21.000000 tencentcloud-sdk-python-hunyuan-3.0.1136/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 20:41:21.000000 tencentcloud-sdk-python-hunyuan-3.0.1136/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      631 2024-04-24 20:41:21.000000 tencentcloud-sdk-python-hunyuan-3.0.1136/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 20:41:21.000000 tencentcloud-sdk-python-hunyuan-3.0.1136/tencentcloud/hunyuan/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-24 20:41:21.000000 tencentcloud-sdk-python-hunyuan-3.0.1136/tencentcloud/hunyuan/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 20:41:21.000000 tencentcloud-sdk-python-hunyuan-3.0.1136/tencentcloud/hunyuan/v20230901/
--rw-r--r--   0 root         (0) root         (0)     2094 2024-04-24 20:41:21.000000 tencentcloud-sdk-python-hunyuan-3.0.1136/tencentcloud/hunyuan/v20230901/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    30312 2024-04-24 20:41:21.000000 tencentcloud-sdk-python-hunyuan-3.0.1136/tencentcloud/hunyuan/v20230901/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-24 20:41:21.000000 tencentcloud-sdk-python-hunyuan-3.0.1136/tencentcloud/hunyuan/v20230901/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5369 2024-04-24 20:41:21.000000 tencentcloud-sdk-python-hunyuan-3.0.1136/tencentcloud/hunyuan/v20230901/hunyuan_client.py
--rw-r--r--   0 root         (0) root         (0)       88 2024-04-24 20:41:21.000000 tencentcloud-sdk-python-hunyuan-3.0.1136/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1081 2024-04-24 20:41:21.000000 tencentcloud-sdk-python-hunyuan-3.0.1136/setup.py
--rw-r--r--   0 root         (0) root         (0)      749 2024-04-24 20:41:21.000000 tencentcloud-sdk-python-hunyuan-3.0.1136/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 20:41:21.000000 tencentcloud-sdk-python-hunyuan-3.0.1136/tencentcloud_sdk_python_hunyuan.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1680 2024-04-24 20:41:21.000000 tencentcloud-sdk-python-hunyuan-3.0.1136/tencentcloud_sdk_python_hunyuan.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2024-04-24 20:41:21.000000 tencentcloud-sdk-python-hunyuan-3.0.1136/tencentcloud_sdk_python_hunyuan.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-24 20:41:21.000000 tencentcloud-sdk-python-hunyuan-3.0.1136/tencentcloud_sdk_python_hunyuan.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      539 2024-04-24 20:41:21.000000 tencentcloud-sdk-python-hunyuan-3.0.1136/tencentcloud_sdk_python_hunyuan.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       40 2024-04-24 20:41:21.000000 tencentcloud-sdk-python-hunyuan-3.0.1136/tencentcloud_sdk_python_hunyuan.egg-info/requires.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:52:12.000000 tencentcloud-sdk-python-hunyuan-3.0.1137/
+-rw-r--r--   0 root         (0) root         (0)     1680 2024-04-25 20:52:12.000000 tencentcloud-sdk-python-hunyuan-3.0.1137/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:52:12.000000 tencentcloud-sdk-python-hunyuan-3.0.1137/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      631 2024-04-25 20:52:12.000000 tencentcloud-sdk-python-hunyuan-3.0.1137/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:52:12.000000 tencentcloud-sdk-python-hunyuan-3.0.1137/tencentcloud/hunyuan/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-25 20:52:12.000000 tencentcloud-sdk-python-hunyuan-3.0.1137/tencentcloud/hunyuan/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:52:12.000000 tencentcloud-sdk-python-hunyuan-3.0.1137/tencentcloud/hunyuan/v20230901/
+-rw-r--r--   0 root         (0) root         (0)     2032 2024-04-25 20:52:12.000000 tencentcloud-sdk-python-hunyuan-3.0.1137/tencentcloud/hunyuan/v20230901/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    39586 2024-04-25 20:52:12.000000 tencentcloud-sdk-python-hunyuan-3.0.1137/tencentcloud/hunyuan/v20230901/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-25 20:52:12.000000 tencentcloud-sdk-python-hunyuan-3.0.1137/tencentcloud/hunyuan/v20230901/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6925 2024-04-25 20:52:12.000000 tencentcloud-sdk-python-hunyuan-3.0.1137/tencentcloud/hunyuan/v20230901/hunyuan_client.py
+-rw-r--r--   0 root         (0) root         (0)       88 2024-04-25 20:52:12.000000 tencentcloud-sdk-python-hunyuan-3.0.1137/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1081 2024-04-25 20:52:12.000000 tencentcloud-sdk-python-hunyuan-3.0.1137/setup.py
+-rw-r--r--   0 root         (0) root         (0)      749 2024-04-25 20:52:12.000000 tencentcloud-sdk-python-hunyuan-3.0.1137/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:52:12.000000 tencentcloud-sdk-python-hunyuan-3.0.1137/tencentcloud_sdk_python_hunyuan.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1680 2024-04-25 20:52:12.000000 tencentcloud-sdk-python-hunyuan-3.0.1137/tencentcloud_sdk_python_hunyuan.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2024-04-25 20:52:12.000000 tencentcloud-sdk-python-hunyuan-3.0.1137/tencentcloud_sdk_python_hunyuan.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-25 20:52:12.000000 tencentcloud-sdk-python-hunyuan-3.0.1137/tencentcloud_sdk_python_hunyuan.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      539 2024-04-25 20:52:12.000000 tencentcloud-sdk-python-hunyuan-3.0.1137/tencentcloud_sdk_python_hunyuan.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       40 2024-04-25 20:52:12.000000 tencentcloud-sdk-python-hunyuan-3.0.1137/tencentcloud_sdk_python_hunyuan.egg-info/requires.txt
```

### Comparing `tencentcloud-sdk-python-hunyuan-3.0.1136/PKG-INFO` & `tencentcloud-sdk-python-hunyuan-3.0.1137/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-hunyuan
-Version: 3.0.1136
+Version: 3.0.1137
 Summary: Tencent Cloud Hunyuan SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-hunyuan-3.0.1136/tencentcloud/__init__.py` & `tencentcloud-sdk-python-hunyuan-3.0.1137/tencentcloud/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.1136'
+__version__ = '3.0.1137'
```

### Comparing `tencentcloud-sdk-python-hunyuan-3.0.1136/tencentcloud/hunyuan/v20230901/errorcodes.py` & `tencentcloud-sdk-python-hunyuan-3.0.1137/tencentcloud/hunyuan/v20230901/errorcodes.py`

 * *Files 5% similar despite different names*

```diff
@@ -46,12 +46,12 @@
 
 # 参数错误。
 INVALIDPARAMETER = 'InvalidParameter'
 
 # 参数取值错误。
 INVALIDPARAMETERVALUE = 'InvalidParameterValue'
 
+# 模型不存在。
+INVALIDPARAMETERVALUE_MODEL = 'InvalidParameterValue.Model'
+
 # 超过配额限制。
 LIMITEXCEEDED = 'LimitExceeded'
-
-# 非白名单帐号，请前往控制台申请试用。
-UNSUPPORTEDOPERATION_NONWHITELISTACCOUNT = 'UnsupportedOperation.NonWhitelistAccount'
```

### Comparing `tencentcloud-sdk-python-hunyuan-3.0.1136/tencentcloud/hunyuan/v20230901/models.py` & `tencentcloud-sdk-python-hunyuan-3.0.1137/tencentcloud/hunyuan/v20230901/models.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,14 +14,254 @@
 # limitations under the License.
 
 import warnings
 
 from tencentcloud.common.abstract_model import AbstractModel
 
 
+class ChatCompletionsRequest(AbstractModel):
+    """ChatCompletions请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Model: 模型名称，可选值包括 hunyuan-lite、hunyuan-standard、hunyuan-pro。
+各模型介绍请阅读 [产品概述](https://cloud.tencent.com/document/product/1729/104753) 中的说明。
+
+注意：
+不同的模型计费不同，请根据 [购买指南](https://cloud.tencent.com/document/product/1729/97731) 按需调用。
+        :type Model: str
+        :param _Messages: 聊天上下文信息。
+说明：
+1. 长度最多为 40，按对话时间从旧到新在数组中排列。
+2. Message.Role 可选值：system、user、assistant。
+其中，system 角色可选，如存在则必须位于列表的最开始。user 和 assistant 需交替出现（一问一答），以 user 提问开始和结束，且 Content 不能为空。Role 的顺序示例：[system（可选） user assistant user assistant user ...]。
+3. Messages 中 Content 总长度不超过 16000 Token，超过则会截断最前面的内容，只保留尾部内容。建议不超过 4000 Token。
+        :type Messages: list of Message
+        :param _Stream: 流式调用开关。
+说明：
+1. 未传值时默认为非流式调用（false）。
+2. 流式调用时以 SSE 协议增量返回结果（返回值取 Choices[n].Delta 中的值，需要拼接增量数据才能获得完整结果）。
+3. 非流式调用时：
+调用方式与普通 HTTP 请求无异。
+接口响应耗时较长，**如需更低时延建议设置为 true**。
+只返回一次最终结果（返回值取 Choices[n].Message 中的值）。
+
+注意：
+通过 SDK 调用时，流式和非流式调用需用**不同的方式**获取返回值，具体参考 SDK 中的注释或示例（在各语言 SDK 代码仓库的 examples/hunyuan/v20230901/ 目录中）。
+        :type Stream: bool
+        :param _StreamModeration: 流式输出审核开关。
+说明：
+1. 输出审核有流式和同步两种模式，**流式模式首包响应更快**。
+2. 当使用流式输出（Stream 字段值为 true）时，该字段生效。
+3. 如果值为 true，将对输出内容进行分段审核，审核通过的内容流式输出返回。如果出现审核不过，响应中的 FinishReason 值为 sensitive。
+4. 如果未传值或值为 false，则不使用流式输出审核，需要审核完所有输出内容后再返回结果。
+
+注意：
+当选择流式输出审核时，可能会出现部分内容已输出，但中间某一段响应中的 FinishReason 值为 sensitive，此时说明安全审核未通过。如果业务场景有实时文字上屏的需求，需要自行撤回已上屏的内容，并建议自定义替换为一条提示语，如 “这个问题我不方便回答，不如我们换个话题试试”，以保障终端体验。
+        :type StreamModeration: bool
+        :param _TopP: 说明：
+1. 影响输出文本的多样性，取值越大，生成文本的多样性越强。
+2. 默认 1.0，取值区间为 [0.0, 1.0]。
+3. 非必要不建议使用，不合理的取值会影响效果。
+        :type TopP: float
+        :param _Temperature: 说明：
+1. 较高的数值会使输出更加随机，而较低的数值会使其更加集中和确定。
+2. 默认 1.0，取值区间为 [0.0, 2.0]。
+3. 非必要不建议使用，不合理的取值会影响效果。
+        :type Temperature: float
+        """
+        self._Model = None
+        self._Messages = None
+        self._Stream = None
+        self._StreamModeration = None
+        self._TopP = None
+        self._Temperature = None
+
+    @property
+    def Model(self):
+        return self._Model
+
+    @Model.setter
+    def Model(self, Model):
+        self._Model = Model
+
+    @property
+    def Messages(self):
+        return self._Messages
+
+    @Messages.setter
+    def Messages(self, Messages):
+        self._Messages = Messages
+
+    @property
+    def Stream(self):
+        return self._Stream
+
+    @Stream.setter
+    def Stream(self, Stream):
+        self._Stream = Stream
+
+    @property
+    def StreamModeration(self):
+        return self._StreamModeration
+
+    @StreamModeration.setter
+    def StreamModeration(self, StreamModeration):
+        self._StreamModeration = StreamModeration
+
+    @property
+    def TopP(self):
+        return self._TopP
+
+    @TopP.setter
+    def TopP(self, TopP):
+        self._TopP = TopP
+
+    @property
+    def Temperature(self):
+        return self._Temperature
+
+    @Temperature.setter
+    def Temperature(self, Temperature):
+        self._Temperature = Temperature
+
+
+    def _deserialize(self, params):
+        self._Model = params.get("Model")
+        if params.get("Messages") is not None:
+            self._Messages = []
+            for item in params.get("Messages"):
+                obj = Message()
+                obj._deserialize(item)
+                self._Messages.append(obj)
+        self._Stream = params.get("Stream")
+        self._StreamModeration = params.get("StreamModeration")
+        self._TopP = params.get("TopP")
+        self._Temperature = params.get("Temperature")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class ChatCompletionsResponse(AbstractModel):
+    """ChatCompletions返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Created: Unix 时间戳，单位为秒。
+        :type Created: int
+        :param _Usage: Token 统计信息。
+按照总 Token 数量计费。
+        :type Usage: :class:`tencentcloud.hunyuan.v20230901.models.Usage`
+        :param _Note: 免责声明。
+        :type Note: str
+        :param _Id: 本轮对话的 ID。
+        :type Id: str
+        :param _Choices: 回复内容。
+        :type Choices: list of Choice
+        :param _ErrorMsg: 错误信息。
+如果流式返回中服务处理异常，返回该错误信息。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ErrorMsg: :class:`tencentcloud.hunyuan.v20230901.models.ErrorMsg`
+        :param _RequestId: 唯一请求 ID，由服务端生成，每次请求都会返回（若请求因其他原因未能抵达服务端，则该次请求不会获得 RequestId）。定位问题时需要提供该次请求的 RequestId。本接口为流式响应接口，当请求成功时，RequestId 会被放在 HTTP 响应的 Header "X-TC-RequestId" 中。
+        :type RequestId: str
+        """
+        self._Created = None
+        self._Usage = None
+        self._Note = None
+        self._Id = None
+        self._Choices = None
+        self._ErrorMsg = None
+        self._RequestId = None
+
+    @property
+    def Created(self):
+        return self._Created
+
+    @Created.setter
+    def Created(self, Created):
+        self._Created = Created
+
+    @property
+    def Usage(self):
+        return self._Usage
+
+    @Usage.setter
+    def Usage(self, Usage):
+        self._Usage = Usage
+
+    @property
+    def Note(self):
+        return self._Note
+
+    @Note.setter
+    def Note(self, Note):
+        self._Note = Note
+
+    @property
+    def Id(self):
+        return self._Id
+
+    @Id.setter
+    def Id(self, Id):
+        self._Id = Id
+
+    @property
+    def Choices(self):
+        return self._Choices
+
+    @Choices.setter
+    def Choices(self, Choices):
+        self._Choices = Choices
+
+    @property
+    def ErrorMsg(self):
+        return self._ErrorMsg
+
+    @ErrorMsg.setter
+    def ErrorMsg(self, ErrorMsg):
+        self._ErrorMsg = ErrorMsg
+
+    @property
+    def RequestId(self):
+        return self._RequestId
+
+    @RequestId.setter
+    def RequestId(self, RequestId):
+        self._RequestId = RequestId
+
+
+    def _deserialize(self, params):
+        self._Created = params.get("Created")
+        if params.get("Usage") is not None:
+            self._Usage = Usage()
+            self._Usage._deserialize(params.get("Usage"))
+        self._Note = params.get("Note")
+        self._Id = params.get("Id")
+        if params.get("Choices") is not None:
+            self._Choices = []
+            for item in params.get("Choices"):
+                obj = Choice()
+                obj._deserialize(item)
+                self._Choices.append(obj)
+        if params.get("ErrorMsg") is not None:
+            self._ErrorMsg = ErrorMsg()
+            self._ErrorMsg._deserialize(params.get("ErrorMsg"))
+        self._RequestId = params.get("RequestId")
+
+
 class ChatProRequest(AbstractModel):
     """ChatPro请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -34,33 +274,36 @@
         :param _TopP: 说明：
 1. 影响输出文本的多样性，取值越大，生成文本的多样性越强。
 2. 默认 1.0，取值区间为 [0.0, 1.0]。
 3. 非必要不建议使用，不合理的取值会影响效果。
         :type TopP: float
         :param _Temperature: 说明：
 1. 较高的数值会使输出更加随机，而较低的数值会使其更加集中和确定。
-2. 默认 1.0，取值区间为 [0.0，2.0]。
+2. 默认 1.0，取值区间为 [0.0, 2.0]。
 3. 非必要不建议使用，不合理的取值会影响效果。
         :type Temperature: float
         :param _Stream: 流式调用开关。
 说明：
 1. 未传值时默认为流式调用。
 2. 流式调用时以 SSE 协议增量返回结果。
 3. 非流式调用时接口响应耗时较长，非必要不建议使用。
 4. 非流式调用时只返回一次最终结果，调用方式与普通 HTTP 请求无异。
+
+注意：
+通过 SDK 调用时，流式和非流式调用需要用**不同的方式**获取返回值，具体参考 SDK 中的注释或示例（在各语言 SDK 代码仓库的 examples/hunyuan/v20230901/ 目录中）。
         :type Stream: bool
         :param _StreamModeration: 流式输出审核开关。
 说明：
-1. 当 Stream 字段值为 true 时，该字段有效。
-2. 未传值时默认不使用流式输出审核。
-3. 如果值为 true，将对输出内容进行分段审核，审核通过的内容流式输出返回。如果出现审核不过，响应中的 finish_reason 值为 sensitive。
-4. 如果值为 false，则需要审核完所有输出内容后再返回结果。
+1. 输出审核有流式和同步两种模式，**流式模式首包响应更快**。
+2. 当使用流式输出（Stream 字段值为 true）时，该字段生效。
+3. 如果值为 true，将对输出内容进行分段审核，审核通过的内容流式输出返回。如果出现审核不过，响应中的 FinishReason 值为 sensitive。
+4. 如果未传值或值为 false，则不使用流式输出审核，需要审核完所有输出内容后再返回结果。
 
 注意：
-当选择流式输出审核时，可能会出现部分内容已输出，但中间某一段响应中的 finish_reason 值为 sensitive，此时说明安全审核未通过。如果业务场景有实时文字上屏的需求，需要自行撤回已上屏的内容，并建议自定义替换为一条提示语，如 “这个问题我不方便回答，不如我们换个话题试试”，以保障终端体验。
+当选择流式输出审核时，可能会出现部分内容已输出，但中间某一段响应中的 FinishReason 值为 sensitive，此时说明安全审核未通过。如果业务场景有实时文字上屏的需求，需要自行撤回已上屏的内容，并建议自定义替换为一条提示语，如 “这个问题我不方便回答，不如我们换个话题试试”，以保障终端体验。
         :type StreamModeration: bool
         """
         self._Messages = None
         self._TopP = None
         self._Temperature = None
         self._Stream = None
         self._StreamModeration = None
@@ -253,33 +496,36 @@
         :param _TopP: 说明：
 1. 影响输出文本的多样性，取值越大，生成文本的多样性越强。
 2. 默认 1.0，取值区间为 [0.0, 1.0]。
 3. 非必要不建议使用，不合理的取值会影响效果。
         :type TopP: float
         :param _Temperature: 说明：
 1. 较高的数值会使输出更加随机，而较低的数值会使其更加集中和确定。
-2. 默认 1.0，取值区间为 [0.0，2.0]。
+2. 默认 1.0，取值区间为 [0.0, 2.0]。
 3. 非必要不建议使用，不合理的取值会影响效果。
         :type Temperature: float
         :param _Stream: 流式调用开关。
 说明：
 1. 未传值时默认为流式调用。
 2. 流式调用时以 SSE 协议增量返回结果。
 3. 非流式调用时接口响应耗时较长，非必要不建议使用。
 4. 非流式调用时只返回一次最终结果，调用方式与普通 HTTP 请求无异。
+
+注意：
+通过 SDK 调用时，流式和非流式调用需要用**不同的方式**获取返回值，具体参考 SDK 中的注释或示例（在各语言 SDK 代码仓库的 examples/hunyuan/v20230901/ 目录中）。
         :type Stream: bool
         :param _StreamModeration: 流式输出审核开关。
 说明：
-1. 当 Stream 字段值为 true 时，该字段有效。
-2. 未传值时默认不使用流式输出审核。
-3. 如果值为 true，将对输出内容进行分段审核，审核通过的内容流式输出返回。如果出现审核不过，响应中的 finish_reason 值为 sensitive。
-4. 如果值为 false，则需要审核完所有输出内容后再返回结果。
+1. 输出审核有流式和同步两种模式，**流式模式首包响应更快**。
+2. 当使用流式输出（Stream 字段值为 true）时，该字段生效。
+3. 如果值为 true，将对输出内容进行分段审核，审核通过的内容流式输出返回。如果出现审核不过，响应中的 FinishReason 值为 sensitive。
+4. 如果未传值或值为 false，则不使用流式输出审核，需要审核完所有输出内容后再返回结果。
 
 注意：
-当选择流式输出审核时，可能会出现部分内容已输出，但中间某一段响应中的 finish_reason 值为 sensitive，此时说明安全审核未通过。如果业务场景有实时文字上屏的需求，需要自行撤回已上屏的内容，并建议自定义替换为一条提示语，如 “这个问题我不方便回答，不如我们换个话题试试”，以保障终端体验。
+当选择流式输出审核时，可能会出现部分内容已输出，但中间某一段响应中的 FinishReason 值为 sensitive，此时说明安全审核未通过。如果业务场景有实时文字上屏的需求，需要自行撤回已上屏的内容，并建议自定义替换为一条提示语，如 “这个问题我不方便回答，不如我们换个话题试试”，以保障终端体验。
         :type StreamModeration: bool
         """
         self._Messages = None
         self._TopP = None
         self._Temperature = None
         self._Stream = None
         self._StreamModeration = None
@@ -560,15 +806,15 @@
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
 class EmbeddingData(AbstractModel):
-    """embedding 信息，当前不支持批量，所以数组元素数目为1。
+    """Embedding 信息。
 
     """
 
     def __init__(self):
         r"""
         :param _Embedding: embedding 信息。
 注意：此字段可能返回 null，表示取不到有效值。
@@ -719,15 +965,15 @@
 class GetEmbeddingRequest(AbstractModel):
     """GetEmbedding请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _Input: 输入文本。总长度不超过1024 个token, 超过则会截断最后面的内容。
+        :param _Input: 输入文本。总长度不超过 1024 个 Token，超过则会截断最后面的内容。
         :type Input: str
         """
         self._Input = None
 
     @property
     def Input(self):
         return self._Input
@@ -752,17 +998,17 @@
 class GetEmbeddingResponse(AbstractModel):
     """GetEmbedding返回参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _Data: 返回的 embedding 信息。
+        :param _Data: 返回的 Embedding 信息。当前不支持批量，所以数组元素数目为 1。
         :type Data: list of EmbeddingData
-        :param _Usage: token 使用计数，按照总token数量收费。
+        :param _Usage: Token 使用计数，按照总 Token 数量收费。
         :type Usage: :class:`tencentcloud.hunyuan.v20230901.models.EmbeddingUsage`
         :param _RequestId: 唯一请求 ID，由服务端生成，每次请求都会返回（若请求因其他原因未能抵达服务端，则该次请求不会获得 RequestId）。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self._Data = None
         self._Usage = None
         self._RequestId = None
@@ -904,15 +1150,15 @@
 
     """
 
     def __init__(self):
         r"""
         :param _Role: 角色
         :type Role: str
-        :param _Content: 消息内容
+        :param _Content: 文本内容
         :type Content: str
         """
         self._Role = None
         self._Content = None
 
     @property
     def Role(self):
```

### Comparing `tencentcloud-sdk-python-hunyuan-3.0.1136/tencentcloud/hunyuan/v20230901/hunyuan_client.py` & `tencentcloud-sdk-python-hunyuan-3.0.1137/tencentcloud/hunyuan/v20230901/hunyuan_client.py`

 * *Files 14% similar despite different names*

```diff
@@ -22,20 +22,42 @@
 
 class HunyuanClient(AbstractClient):
     _apiVersion = '2023-09-01'
     _endpoint = 'hunyuan.tencentcloudapi.com'
     _service = 'hunyuan'
 
 
+    def ChatCompletions(self, request):
+        """腾讯混元大模型是由腾讯研发的大语言模型，具备强大的中文创作能力，复杂语境下的逻辑推理能力，以及可靠的任务执行能力。本接口支持流式或非流式调用，当使用流式调用时为 SSE 协议。
+
+         1. 本接口暂不支持返回图片内容。
+         2. 默认每种模型单账号限制并发数为 5 路，如您有提高并发限制的需求请 [联系我们](https://cloud.tencent.com/act/event/Online_service) 。
+         3. 请使用 SDK 调用本接口，每种开发语言的 SDK Git 仓库 examples/hunyuan/v20230901/ 目录下有提供示例供参考。SDK 链接在文档下方 “**开发者资源 - SDK**” 部分提供。
+
+        :param request: Request instance for ChatCompletions.
+        :type request: :class:`tencentcloud.hunyuan.v20230901.models.ChatCompletionsRequest`
+        :rtype: :class:`tencentcloud.hunyuan.v20230901.models.ChatCompletionsResponse`
+
+        """
+        try:
+            params = request._serialize()
+            return self._call_and_deserialize("ChatCompletions", params, models.ChatCompletionsResponse, headers=request.headers)
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(type(e).__name__, str(e))
+
+
     def ChatPro(self, request):
-        """腾讯混元大模型高级版是由腾讯研发的大语言模型，具备强大的中文创作能力，复杂语境下的逻辑推理能力，以及可靠的任务执行能力。本接口支持流式或非流式调用，当使用流式调用时为 SSE 协议。
+        """腾讯混元大模型（hunyuan-pro）是由腾讯研发的大语言模型，具备强大的中文创作能力，复杂语境下的逻辑推理能力，以及可靠的任务执行能力。本接口支持流式或非流式调用，当使用流式调用时为 SSE 协议。
 
          1. 本接口暂不支持返回图片内容。
          2. 默认单账号限制并发数为 5 路，如您有提高并发限制的需求请 [联系我们](https://cloud.tencent.com/act/event/Online_service) 。
-         3. 请使用 SDK 调用本接口，每种开发语言的 SDK Git 仓库 examples/hunyuan/v20230901/ 目录下有提供示例供参考。
+         3. 请使用 SDK 调用本接口，每种开发语言的 SDK Git 仓库 examples/hunyuan/v20230901/ 目录下有提供示例供参考。SDK 链接在文档下方 “**开发者资源 - SDK**” 部分提供。
 
         :param request: Request instance for ChatPro.
         :type request: :class:`tencentcloud.hunyuan.v20230901.models.ChatProRequest`
         :rtype: :class:`tencentcloud.hunyuan.v20230901.models.ChatProResponse`
 
         """
         try:
@@ -49,15 +71,15 @@
 
 
     def ChatStd(self, request):
         """腾讯混元大模型标准版是由腾讯研发的大语言模型，具备强大的中文创作能力，复杂语境下的逻辑推理能力，以及可靠的任务执行能力。本接口支持流式或非流式调用，当使用流式调用时为 SSE 协议。
 
          1. 本接口暂不支持返回图片内容。
          2. 默认单账号限制并发数为 5 路，如您有提高并发限制的需求请 [联系我们](https://cloud.tencent.com/act/event/Online_service) 。
-         3. 请使用 SDK 调用本接口，每种开发语言的 SDK Git 仓库 examples/hunyuan/v20230901/ 目录下有提供示例供参考。
+         3. 请使用 SDK 调用本接口，每种开发语言的 SDK Git 仓库 examples/hunyuan/v20230901/ 目录下有提供示例供参考。SDK 链接在文档下方 “**开发者资源 - SDK**” 部分提供。
 
         :param request: Request instance for ChatStd.
         :type request: :class:`tencentcloud.hunyuan.v20230901.models.ChatStdRequest`
         :rtype: :class:`tencentcloud.hunyuan.v20230901.models.ChatStdResponse`
 
         """
         try:
@@ -67,15 +89,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetEmbedding(self, request):
-        """腾讯混元-Embedding接口，可以将文本转化为高质量的向量数据。
+        """腾讯混元 Embedding 接口，可以将文本转化为高质量的向量数据。
 
         :param request: Request instance for GetEmbedding.
         :type request: :class:`tencentcloud.hunyuan.v20230901.models.GetEmbeddingRequest`
         :rtype: :class:`tencentcloud.hunyuan.v20230901.models.GetEmbeddingResponse`
 
         """
         try:
```

### Comparing `tencentcloud-sdk-python-hunyuan-3.0.1136/setup.py` & `tencentcloud-sdk-python-hunyuan-3.0.1137/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import tencentcloud
 
 ROOT = os.path.dirname(__file__)
 
 setup(
     name='tencentcloud-sdk-python-hunyuan',
-    install_requires=["tencentcloud-sdk-python-common==3.0.1136"],
+    install_requires=["tencentcloud-sdk-python-common==3.0.1137"],
     version=tencentcloud.__version__,
     description='Tencent Cloud Hunyuan SDK for Python',
     long_description=open('README.rst').read(),
     author='Tencent Cloud',
     url='https://github.com/TencentCloud/tencentcloud-sdk-python',
     maintainer_email="tencentcloudapi@tencent.com",
     scripts=[],
```

### Comparing `tencentcloud-sdk-python-hunyuan-3.0.1136/README.rst` & `tencentcloud-sdk-python-hunyuan-3.0.1137/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-hunyuan-3.0.1136/tencentcloud_sdk_python_hunyuan.egg-info/PKG-INFO` & `tencentcloud-sdk-python-hunyuan-3.0.1137/tencentcloud_sdk_python_hunyuan.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-hunyuan
-Version: 3.0.1136
+Version: 3.0.1137
 Summary: Tencent Cloud Hunyuan SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-hunyuan-3.0.1136/tencentcloud_sdk_python_hunyuan.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-hunyuan-3.0.1137/tencentcloud_sdk_python_hunyuan.egg-info/SOURCES.txt`

 * *Files identical despite different names*


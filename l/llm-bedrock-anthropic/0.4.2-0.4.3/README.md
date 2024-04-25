# Comparing `tmp/llm-bedrock-anthropic-0.4.2.tar.gz` & `tmp/llm_bedrock_anthropic-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm-bedrock-anthropic-0.4.2.tar", last modified: Mon Mar 18 14:03:54 2024, max compression
+gzip compressed data, was "llm_bedrock_anthropic-0.4.3.tar", last modified: Thu Apr 25 01:09:43 2024, max compression
```

## Comparing `llm-bedrock-anthropic-0.4.2.tar` & `llm_bedrock_anthropic-0.4.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 sean       (501) staff       (20)        0 2024-03-18 14:03:54.938255 llm-bedrock-anthropic-0.4.2/
--rw-r--r--   0 sean       (501) staff       (20)    11357 2023-10-10 13:24:27.000000 llm-bedrock-anthropic-0.4.2/LICENSE
--rw-r--r--   0 sean       (501) staff       (20)     1864 2024-03-18 14:03:54.937206 llm-bedrock-anthropic-0.4.2/PKG-INFO
--rw-r--r--   0 sean       (501) staff       (20)     1410 2024-03-10 15:10:37.000000 llm-bedrock-anthropic-0.4.2/README.md
-drwxr-xr-x   0 sean       (501) staff       (20)        0 2024-03-18 14:03:54.936099 llm-bedrock-anthropic-0.4.2/llm_bedrock_anthropic.egg-info/
--rw-r--r--   0 sean       (501) staff       (20)     1864 2024-03-18 14:03:54.000000 llm-bedrock-anthropic-0.4.2/llm_bedrock_anthropic.egg-info/PKG-INFO
--rw-r--r--   0 sean       (501) staff       (20)      329 2024-03-18 14:03:54.000000 llm-bedrock-anthropic-0.4.2/llm_bedrock_anthropic.egg-info/SOURCES.txt
--rw-r--r--   0 sean       (501) staff       (20)        1 2024-03-18 14:03:54.000000 llm-bedrock-anthropic-0.4.2/llm_bedrock_anthropic.egg-info/dependency_links.txt
--rw-r--r--   0 sean       (501) staff       (20)       45 2024-03-18 14:03:54.000000 llm-bedrock-anthropic-0.4.2/llm_bedrock_anthropic.egg-info/entry_points.txt
--rw-r--r--   0 sean       (501) staff       (20)       33 2024-03-18 14:03:54.000000 llm-bedrock-anthropic-0.4.2/llm_bedrock_anthropic.egg-info/requires.txt
--rw-r--r--   0 sean       (501) staff       (20)       22 2024-03-18 14:03:54.000000 llm-bedrock-anthropic-0.4.2/llm_bedrock_anthropic.egg-info/top_level.txt
--rw-r--r--   0 sean       (501) staff       (20)     6727 2024-03-18 13:57:27.000000 llm-bedrock-anthropic-0.4.2/llm_bedrock_anthropic.py
--rw-r--r--   0 sean       (501) staff       (20)      537 2024-03-18 13:49:35.000000 llm-bedrock-anthropic-0.4.2/pyproject.toml
--rw-r--r--   0 sean       (501) staff       (20)       38 2024-03-18 14:03:54.938513 llm-bedrock-anthropic-0.4.2/setup.cfg
+drwxr-xr-x   0 sean       (501) staff       (20)        0 2024-04-25 01:09:43.536137 llm_bedrock_anthropic-0.4.3/
+-rw-r--r--   0 sean       (501) staff       (20)    11357 2023-10-10 13:24:27.000000 llm_bedrock_anthropic-0.4.3/LICENSE
+-rw-r--r--   0 sean       (501) staff       (20)     2371 2024-04-25 01:09:43.535878 llm_bedrock_anthropic-0.4.3/PKG-INFO
+-rw-r--r--   0 sean       (501) staff       (20)     1916 2024-04-25 01:08:09.000000 llm_bedrock_anthropic-0.4.3/README.md
+drwxr-xr-x   0 sean       (501) staff       (20)        0 2024-04-25 01:09:43.535614 llm_bedrock_anthropic-0.4.3/llm_bedrock_anthropic.egg-info/
+-rw-r--r--   0 sean       (501) staff       (20)     2371 2024-04-25 01:09:43.000000 llm_bedrock_anthropic-0.4.3/llm_bedrock_anthropic.egg-info/PKG-INFO
+-rw-r--r--   0 sean       (501) staff       (20)      329 2024-04-25 01:09:43.000000 llm_bedrock_anthropic-0.4.3/llm_bedrock_anthropic.egg-info/SOURCES.txt
+-rw-r--r--   0 sean       (501) staff       (20)        1 2024-04-25 01:09:43.000000 llm_bedrock_anthropic-0.4.3/llm_bedrock_anthropic.egg-info/dependency_links.txt
+-rw-r--r--   0 sean       (501) staff       (20)       45 2024-04-25 01:09:43.000000 llm_bedrock_anthropic-0.4.3/llm_bedrock_anthropic.egg-info/entry_points.txt
+-rw-r--r--   0 sean       (501) staff       (20)       33 2024-04-25 01:09:43.000000 llm_bedrock_anthropic-0.4.3/llm_bedrock_anthropic.egg-info/requires.txt
+-rw-r--r--   0 sean       (501) staff       (20)       22 2024-04-25 01:09:43.000000 llm_bedrock_anthropic-0.4.3/llm_bedrock_anthropic.egg-info/top_level.txt
+-rw-r--r--   0 sean       (501) staff       (20)     7335 2024-04-25 00:16:16.000000 llm_bedrock_anthropic-0.4.3/llm_bedrock_anthropic.py
+-rw-r--r--   0 sean       (501) staff       (20)      537 2024-04-25 01:08:58.000000 llm_bedrock_anthropic-0.4.3/pyproject.toml
+-rw-r--r--   0 sean       (501) staff       (20)       38 2024-04-25 01:09:43.536182 llm_bedrock_anthropic-0.4.3/setup.cfg
```

### Comparing `llm-bedrock-anthropic-0.4.2/LICENSE` & `llm_bedrock_anthropic-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `llm-bedrock-anthropic-0.4.2/PKG-INFO` & `llm_bedrock_anthropic-0.4.3/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,17 @@
-Metadata-Version: 2.1
-Name: llm-bedrock-anthropic
-Version: 0.4.2
-Summary: LLM plugin for Anthropic's Claude on AWS Bedrock
-Author: Sean Blakey, Will Sorenson
-License: Apache-2.0
-Project-URL: Homepage, https://github.com/sblakey/llm-bedrock-anthropic
-Classifier: License :: OSI Approved :: Apache Software License
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: llm
-Requires-Dist: boto3>=1.34.55
-Requires-Dist: pydantic>=2.0
-
 # llm-bedrock-anthropic
 
 [![PyPI](https://img.shields.io/pypi/v/llm-bedrock-anthropic.svg)](https://pypi.org/project/llm-bedrock-anthropic/)
 [![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://github.com/sblakey/llm-bedrock-anthropic/blob/main/LICENSE)
 
 Plugin for [LLM](https://llm.datasette.io/) adding support for Anthropic's Claude models.
 
+## New: claude opus model 
+### claude-3-opus available on us-west-2
+
 ## Installation
 
 Install this plugin in the same environment as LLM. From the current directory
 ```bash
 llm install llm-bedrock-anthropic
 ```
 ## Configuration
@@ -58,7 +47,18 @@
 ```bash
 llm -m bedrock-claude -o max_tokens_to_sample 20 "Sing me the alphabet"
  Here is the alphabet song:
 
 A B C D E F G
 H I J
 ```
+
+- `bedrock_model_id`: allows you to override the `model_id` passed to Bedrock.
+
+Can be a base model ID or ARN from https://docs.aws.amazon.com/bedrock/latest/userguide/model-ids.html#model-ids-arns
+
+Can also be an ARN of provisioned throughput for a base or custom model.
+
+Use it like this:
+```bash
+llm -m bedrock-claude-haiku -o bedrock_model_id anthropic.claude-3-sonnet-20240229-v1:0 "Remind me how to post a new version to PyPI"
+```
```

### Comparing `llm-bedrock-anthropic-0.4.2/llm_bedrock_anthropic.egg-info/PKG-INFO` & `llm_bedrock_anthropic-0.4.3/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm-bedrock-anthropic
-Version: 0.4.2
+Version: 0.4.3
 Summary: LLM plugin for Anthropic's Claude on AWS Bedrock
 Author: Sean Blakey, Will Sorenson
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/sblakey/llm-bedrock-anthropic
 Classifier: License :: OSI Approved :: Apache Software License
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -15,14 +15,17 @@
 # llm-bedrock-anthropic
 
 [![PyPI](https://img.shields.io/pypi/v/llm-bedrock-anthropic.svg)](https://pypi.org/project/llm-bedrock-anthropic/)
 [![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://github.com/sblakey/llm-bedrock-anthropic/blob/main/LICENSE)
 
 Plugin for [LLM](https://llm.datasette.io/) adding support for Anthropic's Claude models.
 
+## New: claude opus model 
+### claude-3-opus available on us-west-2
+
 ## Installation
 
 Install this plugin in the same environment as LLM. From the current directory
 ```bash
 llm install llm-bedrock-anthropic
 ```
 ## Configuration
@@ -58,7 +61,18 @@
 ```bash
 llm -m bedrock-claude -o max_tokens_to_sample 20 "Sing me the alphabet"
  Here is the alphabet song:
 
 A B C D E F G
 H I J
 ```
+
+- `bedrock_model_id`: allows you to override the `model_id` passed to Bedrock.
+
+Can be a base model ID or ARN from https://docs.aws.amazon.com/bedrock/latest/userguide/model-ids.html#model-ids-arns
+
+Can also be an ARN of provisioned throughput for a base or custom model.
+
+Use it like this:
+```bash
+llm -m bedrock-claude-haiku -o bedrock_model_id anthropic.claude-3-sonnet-20240229-v1:0 "Remind me how to post a new version to PyPI"
+```
```

### Comparing `llm-bedrock-anthropic-0.4.2/llm_bedrock_anthropic.py` & `llm_bedrock_anthropic-0.4.3/llm_bedrock_anthropic.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,14 +32,24 @@
             "bedrock-claude-sonnet",
             "bedrock-sonnet",
             "bedrock-claude"
             "bc",
         ),
     )
     register(
+        BedrockClaude("anthropic.claude-3-opus-20240229-v1:0"),
+        aliases=(
+            "bedrock-claude-v3-opus",
+            "bedrock-claude-v3-opus",
+            "bedrock-claude-opus",
+            "bedrock-opus",
+            "bo",
+        ),
+    )
+    register(
         BedrockClaude("anthropic.claude-3-haiku-20240307-v1:0"),
         aliases=(
             "bedrock-claude-v3-haiku",
             "bedrock-claude-haiku",
             "bedrock-haiku",
             "bh",
         ),
@@ -50,14 +60,18 @@
 
     # TODO: expose other Options
     class Options(llm.Options):
         max_tokens_to_sample: Optional[int] = Field(
             description="The maximum number of tokens to generate before stopping",
             default=8191,  # Bedrock complained when I passed a higher number into claude-instant
         )
+        bedrock_model_id: Optional[str] = Field(
+            description="Bedrock modelId or ARN of base, custom, or provisioned model",
+            default=None,
+        )
 
         @field_validator("max_tokens_to_sample")
         def validate_length(cls, max_tokens_to_sample):
             if not (0 < max_tokens_to_sample <= 1_000_000):
                 raise ValueError("max_tokens_to_sample must be in range 1-1,000,000")
             return max_tokens_to_sample
 
@@ -118,30 +132,31 @@
             "system": prompt.system or "",
             "messages": prompt.messages,
         }
         encoded_data = json.dumps(body)
         prompt.prompt_json = encoded_data
 
         client = boto3.client('bedrock-runtime')
+        bedrock_model_id = prompt.options.bedrock_model_id or self.model_id
         if stream:
             bedrock_response = client.invoke_model_with_response_stream(
-                modelId=self.model_id, body=prompt.prompt_json
+                modelId=bedrock_model_id, body=prompt.prompt_json
             )
             chunks = bedrock_response.get("body")
 
             for event in chunks:
                 chunk = event.get("chunk")
                 response = json.loads(chunk.get("bytes").decode())
                 if response["type"] == "content_block_delta":
                     completion = response["delta"]["text"]
                     yield completion
 
         else:
             bedrock_response = client.invoke_model(
-                modelId=self.model_id, body=prompt.prompt_json
+                modelId=bedrock_model_id, body=prompt.prompt_json
             )
             body = bedrock_response["body"].read()
             response.response_json = json.loads(body)
             completion = response.response_json["content"][-1]["text"]
             yield completion
 
     def execute_v3(self, prompt, stream, response, conversation):
@@ -152,29 +167,30 @@
             "anthropic_version": "bedrock-2023-05-31",
             "max_tokens": prompt.options.max_tokens_to_sample,
             "messages": messages
         }
         if prompt.system:
             prompt_json.update({"system": prompt.system})
         prompt.prompt_json = prompt_json
+        bedrock_model_id = prompt.options.bedrock_model_id or self.model_id
         if stream:
             bedrock_response = client.invoke_model_with_response_stream(
-                modelId=self.model_id, body=json.dumps(prompt_json)
+                modelId=bedrock_model_id, body=json.dumps(prompt_json)
             )
             chunks = bedrock_response.get("body")
 
             for event in chunks:
                 chunk = event.get("chunk")
                 if chunk:
                     response = json.loads(chunk.get("bytes").decode())
                     if response['type'] == 'content_block_delta':
                         if response["delta"]['type'] == 'text_delta':
                             yield response["delta"]["text"]
         else:
             bedrock_response = client.invoke_model(
-                modelId=self.model_id,
+                modelId=bedrock_model_id,
                 body=json.dumps(prompt_json),
             )
             body = bedrock_response["body"].read()
             response.response_json = json.loads(body)
             completion = response.response_json["content"][0]["text"]
-            yield completion
+            yield completion
```

### Comparing `llm-bedrock-anthropic-0.4.2/pyproject.toml` & `llm_bedrock_anthropic-0.4.3/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "llm-bedrock-anthropic"
-version = "0.4.2"
+version = "0.4.3"
 
 description = "LLM plugin for Anthropic's Claude on AWS Bedrock"
 readme = "README.md"
 authors = [{name = "Sean Blakey"}, {name = "Will Sorenson"}]
 license = {text = "Apache-2.0"}
 classifiers = [
     "License :: OSI Approved :: Apache Software License"
```


# Comparing `tmp/continuous_eval-0.3.6.tar.gz` & `tmp/continuous_eval-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "continuous_eval-0.3.6.tar", max compression
+gzip compressed data, was "continuous_eval-0.3.7.tar", max compression
```

## Comparing `continuous_eval-0.3.6.tar` & `continuous_eval-0.3.7.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0    11357 2024-01-17 21:26:45.588731 continuous_eval-0.3.6/LICENSE
--rw-r--r--   0        0        0     9137 2024-04-02 16:24:12.028523 continuous_eval-0.3.6/README.md
--rw-r--r--   0        0        0        0 2024-02-25 04:22:14.516782 continuous_eval-0.3.6/continuous_eval/__init__.py
--rw-r--r--   0        0        0       64 2024-02-17 05:39:52.426571 continuous_eval-0.3.6/continuous_eval/classifiers/__init__.py
--rw-r--r--   0        0        0     3058 2024-03-22 00:37:22.186238 continuous_eval-0.3.6/continuous_eval/classifiers/ensemble.py
--rw-r--r--   0        0        0      652 2024-03-22 00:45:46.211844 continuous_eval-0.3.6/continuous_eval/classifiers/utils.py
--rw-r--r--   0        0        0     3031 2024-02-25 04:22:14.517248 continuous_eval-0.3.6/continuous_eval/data_downloader.py
--rw-r--r--   0        0        0     3609 2024-03-22 00:37:22.186380 continuous_eval-0.3.6/continuous_eval/datatypes.py
--rw-r--r--   0        0        0      251 2024-02-25 04:22:14.517467 continuous_eval-0.3.6/continuous_eval/eval/__init__.py
--rw-r--r--   0        0        0     6234 2024-04-08 17:58:05.099379 continuous_eval-0.3.6/continuous_eval/eval/dataset.py
--rw-r--r--   0        0        0     9394 2024-03-08 08:55:45.667192 continuous_eval-0.3.6/continuous_eval/eval/manager.py
--rw-r--r--   0        0        0     1627 2024-02-28 21:52:45.358114 continuous_eval-0.3.6/continuous_eval/eval/modules.py
--rw-r--r--   0        0        0     4539 2024-02-29 19:22:06.462595 continuous_eval-0.3.6/continuous_eval/eval/pipeline.py
--rw-r--r--   0        0        0     4420 2024-03-22 00:45:46.482746 continuous_eval-0.3.6/continuous_eval/eval/result_types.py
--rw-r--r--   0        0        0     1380 2024-02-25 04:22:14.518180 continuous_eval-0.3.6/continuous_eval/eval/tests.py
--rw-r--r--   0        0        0      122 2024-02-25 04:22:14.518248 continuous_eval-0.3.6/continuous_eval/eval/types.py
--rw-r--r--   0        0        0     1107 2024-02-29 19:29:39.554407 continuous_eval-0.3.6/continuous_eval/eval/utils.py
--rw-r--r--   0        0        0       69 2024-02-17 05:39:52.427862 continuous_eval-0.3.6/continuous_eval/generators/__init__.py
--rw-r--r--   0        0        0    12800 2024-03-16 15:09:59.783830 continuous_eval-0.3.6/continuous_eval/generators/simple.py
--rw-r--r--   0        0        0    10006 2024-03-27 05:39:44.586759 continuous_eval-0.3.6/continuous_eval/llm_factory.py
--rw-r--r--   0        0        0        0 2024-03-27 04:22:00.195998 continuous_eval-0.3.6/continuous_eval/llms/__init__.py
--rw-r--r--   0        0        0      780 2024-03-27 05:39:44.227478 continuous_eval-0.3.6/continuous_eval/llms/bedrock.py
--rw-r--r--   0        0        0       48 2024-02-25 04:22:14.519065 continuous_eval-0.3.6/continuous_eval/metrics/__init__.py
--rw-r--r--   0        0        0     1732 2024-03-27 04:07:30.402986 continuous_eval-0.3.6/continuous_eval/metrics/_utils/simple_tokenizer.py
--rw-r--r--   0        0        0     2471 2024-03-08 08:55:45.593923 continuous_eval-0.3.6/continuous_eval/metrics/base.py
--rw-r--r--   0        0        0       91 2024-02-27 06:09:06.065186 continuous_eval-0.3.6/continuous_eval/metrics/classification/__init__.py
--rw-r--r--   0        0        0     2233 2024-02-27 06:09:06.065562 continuous_eval-0.3.6/continuous_eval/metrics/classification/classification.py
--rw-r--r--   0        0        0      111 2024-03-08 07:02:54.302236 continuous_eval-0.3.6/continuous_eval/metrics/code/python/__init__.py
--rw-r--r--   0        0        0    11635 2024-03-08 08:55:45.681607 continuous_eval-0.3.6/continuous_eval/metrics/code/python/code_deterministic_metrics.py
--rw-r--r--   0        0        0      678 2024-03-17 22:25:39.167477 continuous_eval-0.3.6/continuous_eval/metrics/generation/text/__init__.py
--rw-r--r--   0        0        0     3109 2024-03-16 15:32:17.406679 continuous_eval-0.3.6/continuous_eval/metrics/generation/text/bert.py
--rw-r--r--   0        0        0     2879 2024-03-27 04:56:36.204502 continuous_eval-0.3.6/continuous_eval/metrics/generation/text/custom.py
--rw-r--r--   0        0        0     4814 2024-03-08 08:55:45.614834 continuous_eval-0.3.6/continuous_eval/metrics/generation/text/deterministic.py
--rw-r--r--   0        0        0    11472 2024-03-27 05:39:44.567238 continuous_eval-0.3.6/continuous_eval/metrics/generation/text/llm_based.py
--rw-r--r--   0        0        0     5741 2024-03-17 22:25:39.168561 continuous_eval-0.3.6/continuous_eval/metrics/generation/text/semantic.py
--rw-r--r--   0        0        0     2865 2024-03-27 05:39:44.530970 continuous_eval-0.3.6/continuous_eval/metrics/generation/text/utils.py
--rw-r--r--   0        0        0      437 2024-02-25 04:22:14.520214 continuous_eval-0.3.6/continuous_eval/metrics/retrieval/__init__.py
--rw-r--r--   0        0        0     6541 2024-04-05 23:59:38.533703 continuous_eval-0.3.6/continuous_eval/metrics/retrieval/llm_based.py
--rw-r--r--   0        0        0     1918 2024-02-25 04:22:14.520478 continuous_eval-0.3.6/continuous_eval/metrics/retrieval/matching_strategy.py
--rw-r--r--   0        0        0     2470 2024-04-02 16:24:12.028818 continuous_eval-0.3.6/continuous_eval/metrics/retrieval/precision_recall_f1.py
--rw-r--r--   0        0        0     3394 2024-04-02 16:24:12.029049 continuous_eval-0.3.6/continuous_eval/metrics/retrieval/ranked.py
--rw-r--r--   0        0        0     1500 2024-02-25 04:22:14.520753 continuous_eval-0.3.6/continuous_eval/metrics/tools/match.py
--rw-r--r--   0        0        0     4013 2024-02-26 23:53:19.235416 continuous_eval-0.3.6/continuous_eval/utils/telemetry.py
--rw-r--r--   0        0        0     1850 2024-04-08 17:57:33.865982 continuous_eval-0.3.6/pyproject.toml
--rw-r--r--   0        0        0    11375 1970-01-01 00:00:00.000000 continuous_eval-0.3.6/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-12-10 20:19:38.190467 continuous_eval-0.3.7/LICENSE
+-rw-r--r--   0        0        0     9137 2024-04-25 01:13:40.195509 continuous_eval-0.3.7/README.md
+-rw-r--r--   0        0        0        0 2024-02-25 01:21:36.780803 continuous_eval-0.3.7/continuous_eval/__init__.py
+-rw-r--r--   0        0        0       64 2024-01-12 14:57:28.874524 continuous_eval-0.3.7/continuous_eval/classifiers/__init__.py
+-rw-r--r--   0        0        0     3058 2024-04-01 22:15:42.805184 continuous_eval-0.3.7/continuous_eval/classifiers/ensemble.py
+-rw-r--r--   0        0        0      652 2024-04-01 22:15:42.806178 continuous_eval-0.3.7/continuous_eval/classifiers/utils.py
+-rw-r--r--   0        0        0     3031 2024-02-25 01:21:36.781330 continuous_eval-0.3.7/continuous_eval/data_downloader.py
+-rw-r--r--   0        0        0     3609 2024-04-01 22:15:42.806551 continuous_eval-0.3.7/continuous_eval/datatypes.py
+-rw-r--r--   0        0        0      251 2024-02-25 01:21:36.781535 continuous_eval-0.3.7/continuous_eval/eval/__init__.py
+-rw-r--r--   0        0        0     6234 2024-04-25 01:13:40.196141 continuous_eval-0.3.7/continuous_eval/eval/dataset.py
+-rw-r--r--   0        0        0     9394 2024-03-08 16:03:17.678226 continuous_eval-0.3.7/continuous_eval/eval/manager.py
+-rw-r--r--   0        0        0     1627 2024-02-25 01:21:36.781780 continuous_eval-0.3.7/continuous_eval/eval/modules.py
+-rw-r--r--   0        0        0     4539 2024-02-25 01:21:36.781864 continuous_eval-0.3.7/continuous_eval/eval/pipeline.py
+-rw-r--r--   0        0        0     4420 2024-04-01 22:15:42.808392 continuous_eval-0.3.7/continuous_eval/eval/result_types.py
+-rw-r--r--   0        0        0     1380 2024-02-25 01:21:36.782015 continuous_eval-0.3.7/continuous_eval/eval/tests.py
+-rw-r--r--   0        0        0      122 2024-02-25 01:21:36.782079 continuous_eval-0.3.7/continuous_eval/eval/types.py
+-rw-r--r--   0        0        0     1107 2024-03-04 17:53:52.558401 continuous_eval-0.3.7/continuous_eval/eval/utils.py
+-rw-r--r--   0        0        0       69 2024-01-12 14:57:28.877604 continuous_eval-0.3.7/continuous_eval/generators/__init__.py
+-rw-r--r--   0        0        0    12800 2024-03-26 21:20:35.487618 continuous_eval-0.3.7/continuous_eval/generators/simple.py
+-rw-r--r--   0        0        0    10016 2024-04-25 01:36:49.832110 continuous_eval-0.3.7/continuous_eval/llm_factory.py
+-rw-r--r--   0        0        0        0 2024-04-01 22:15:42.809284 continuous_eval-0.3.7/continuous_eval/llms/__init__.py
+-rw-r--r--   0        0        0      780 2024-04-01 22:15:42.809509 continuous_eval-0.3.7/continuous_eval/llms/bedrock.py
+-rw-r--r--   0        0        0       48 2024-02-25 01:21:36.782270 continuous_eval-0.3.7/continuous_eval/metrics/__init__.py
+-rw-r--r--   0        0        0     1732 2024-04-01 22:15:42.809855 continuous_eval-0.3.7/continuous_eval/metrics/_utils/simple_tokenizer.py
+-rw-r--r--   0        0        0     2471 2024-03-08 16:03:17.679836 continuous_eval-0.3.7/continuous_eval/metrics/base.py
+-rw-r--r--   0        0        0       91 2024-02-27 06:34:50.556016 continuous_eval-0.3.7/continuous_eval/metrics/classification/__init__.py
+-rw-r--r--   0        0        0     2233 2024-02-27 06:34:50.556112 continuous_eval-0.3.7/continuous_eval/metrics/classification/classification.py
+-rw-r--r--   0        0        0      111 2024-03-08 16:03:17.679999 continuous_eval-0.3.7/continuous_eval/metrics/code/python/__init__.py
+-rw-r--r--   0        0        0    11635 2024-03-08 16:03:17.680796 continuous_eval-0.3.7/continuous_eval/metrics/code/python/code_deterministic_metrics.py
+-rw-r--r--   0        0        0      678 2024-03-26 21:20:35.488791 continuous_eval-0.3.7/continuous_eval/metrics/generation/text/__init__.py
+-rw-r--r--   0        0        0     3109 2024-03-26 21:20:35.489197 continuous_eval-0.3.7/continuous_eval/metrics/generation/text/bert.py
+-rw-r--r--   0        0        0     2879 2024-04-01 22:15:42.810274 continuous_eval-0.3.7/continuous_eval/metrics/generation/text/custom.py
+-rw-r--r--   0        0        0     4814 2024-03-08 16:03:17.681650 continuous_eval-0.3.7/continuous_eval/metrics/generation/text/deterministic.py
+-rw-r--r--   0        0        0    11472 2024-04-01 22:15:42.811029 continuous_eval-0.3.7/continuous_eval/metrics/generation/text/llm_based.py
+-rw-r--r--   0        0        0     5741 2024-03-26 21:20:35.489763 continuous_eval-0.3.7/continuous_eval/metrics/generation/text/semantic.py
+-rw-r--r--   0        0        0     2865 2024-04-01 22:15:42.811345 continuous_eval-0.3.7/continuous_eval/metrics/generation/text/utils.py
+-rw-r--r--   0        0        0      437 2024-04-25 01:13:57.116186 continuous_eval-0.3.7/continuous_eval/metrics/retrieval/__init__.py
+-rw-r--r--   0        0        0     6541 2024-03-26 21:20:35.490910 continuous_eval-0.3.7/continuous_eval/metrics/retrieval/llm_based.py
+-rw-r--r--   0        0        0     1918 2024-04-25 01:13:52.350927 continuous_eval-0.3.7/continuous_eval/metrics/retrieval/matching_strategy.py
+-rw-r--r--   0        0        0     2470 2024-04-25 01:13:40.196878 continuous_eval-0.3.7/continuous_eval/metrics/retrieval/precision_recall_f1.py
+-rw-r--r--   0        0        0     3394 2024-04-25 01:13:40.198789 continuous_eval-0.3.7/continuous_eval/metrics/retrieval/ranked.py
+-rw-r--r--   0        0        0     1500 2024-02-25 01:21:36.783877 continuous_eval-0.3.7/continuous_eval/metrics/tools/match.py
+-rw-r--r--   0        0        0     4013 2024-02-27 06:34:50.556585 continuous_eval-0.3.7/continuous_eval/utils/telemetry.py
+-rw-r--r--   0        0        0     1850 2024-04-25 01:38:41.759442 continuous_eval-0.3.7/pyproject.toml
+-rw-r--r--   0        0        0    11375 1970-01-01 00:00:00.000000 continuous_eval-0.3.7/PKG-INFO
```

### Comparing `continuous_eval-0.3.6/LICENSE` & `continuous_eval-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `continuous_eval-0.3.6/README.md` & `continuous_eval-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `continuous_eval-0.3.6/continuous_eval/classifiers/ensemble.py` & `continuous_eval-0.3.7/continuous_eval/classifiers/ensemble.py`

 * *Files identical despite different names*

### Comparing `continuous_eval-0.3.6/continuous_eval/classifiers/utils.py` & `continuous_eval-0.3.7/continuous_eval/classifiers/utils.py`

 * *Files identical despite different names*

### Comparing `continuous_eval-0.3.6/continuous_eval/data_downloader.py` & `continuous_eval-0.3.7/continuous_eval/data_downloader.py`

 * *Files identical despite different names*

### Comparing `continuous_eval-0.3.6/continuous_eval/datatypes.py` & `continuous_eval-0.3.7/continuous_eval/datatypes.py`

 * *Files identical despite different names*

### Comparing `continuous_eval-0.3.6/continuous_eval/eval/dataset.py` & `continuous_eval-0.3.7/continuous_eval/eval/dataset.py`

 * *Files identical despite different names*

### Comparing `continuous_eval-0.3.6/continuous_eval/eval/manager.py` & `continuous_eval-0.3.7/continuous_eval/eval/manager.py`

 * *Files identical despite different names*

### Comparing `continuous_eval-0.3.6/continuous_eval/eval/modules.py` & `continuous_eval-0.3.7/continuous_eval/eval/modules.py`

 * *Files identical despite different names*

### Comparing `continuous_eval-0.3.6/continuous_eval/eval/pipeline.py` & `continuous_eval-0.3.7/continuous_eval/eval/pipeline.py`

 * *Files identical despite different names*

### Comparing `continuous_eval-0.3.6/continuous_eval/eval/result_types.py` & `continuous_eval-0.3.7/continuous_eval/eval/result_types.py`

 * *Files identical despite different names*

### Comparing `continuous_eval-0.3.6/continuous_eval/eval/tests.py` & `continuous_eval-0.3.7/continuous_eval/eval/tests.py`

 * *Files identical despite different names*

### Comparing `continuous_eval-0.3.6/continuous_eval/eval/utils.py` & `continuous_eval-0.3.7/continuous_eval/eval/utils.py`

 * *Files identical despite different names*

### Comparing `continuous_eval-0.3.6/continuous_eval/generators/simple.py` & `continuous_eval-0.3.7/continuous_eval/generators/simple.py`

 * *Files identical despite different names*

### Comparing `continuous_eval-0.3.6/continuous_eval/llm_factory.py` & `continuous_eval-0.3.7/continuous_eval/llm_factory.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,16 +19,16 @@
 try:
     from anthropic import AI_PROMPT, HUMAN_PROMPT, Anthropic
 
     ANTHROPIC_AVAILABLE = True
 except ImportError:
     ANTHROPIC_AVAILABLE = False
 try:
-    from langchain.chat_models import AzureChatOpenAI
     from langchain.schema import HumanMessage, SystemMessage
+    from langchain_community.chat_models import AzureChatOpenAI
 
     AZURE_OPENAI_AVAILABLE = True
 except ImportError:
     AZURE_OPENAI_AVAILABLE = False
 try:
     from cohere import Client as CohereClient
```

### Comparing `continuous_eval-0.3.6/continuous_eval/llms/bedrock.py` & `continuous_eval-0.3.7/continuous_eval/llms/bedrock.py`

 * *Files identical despite different names*

### Comparing `continuous_eval-0.3.6/continuous_eval/metrics/_utils/simple_tokenizer.py` & `continuous_eval-0.3.7/continuous_eval/metrics/_utils/simple_tokenizer.py`

 * *Files identical despite different names*

### Comparing `continuous_eval-0.3.6/continuous_eval/metrics/base.py` & `continuous_eval-0.3.7/continuous_eval/metrics/base.py`

 * *Files identical despite different names*

### Comparing `continuous_eval-0.3.6/continuous_eval/metrics/classification/classification.py` & `continuous_eval-0.3.7/continuous_eval/metrics/classification/classification.py`

 * *Files identical despite different names*

### Comparing `continuous_eval-0.3.6/continuous_eval/metrics/code/python/code_deterministic_metrics.py` & `continuous_eval-0.3.7/continuous_eval/metrics/code/python/code_deterministic_metrics.py`

 * *Files identical despite different names*

### Comparing `continuous_eval-0.3.6/continuous_eval/metrics/generation/text/__init__.py` & `continuous_eval-0.3.7/continuous_eval/metrics/generation/text/__init__.py`

 * *Files identical despite different names*

### Comparing `continuous_eval-0.3.6/continuous_eval/metrics/generation/text/bert.py` & `continuous_eval-0.3.7/continuous_eval/metrics/generation/text/bert.py`

 * *Files identical despite different names*

### Comparing `continuous_eval-0.3.6/continuous_eval/metrics/generation/text/custom.py` & `continuous_eval-0.3.7/continuous_eval/metrics/generation/text/custom.py`

 * *Files identical despite different names*

### Comparing `continuous_eval-0.3.6/continuous_eval/metrics/generation/text/deterministic.py` & `continuous_eval-0.3.7/continuous_eval/metrics/generation/text/deterministic.py`

 * *Files identical despite different names*

### Comparing `continuous_eval-0.3.6/continuous_eval/metrics/generation/text/llm_based.py` & `continuous_eval-0.3.7/continuous_eval/metrics/generation/text/llm_based.py`

 * *Files identical despite different names*

### Comparing `continuous_eval-0.3.6/continuous_eval/metrics/generation/text/semantic.py` & `continuous_eval-0.3.7/continuous_eval/metrics/generation/text/semantic.py`

 * *Files identical despite different names*

### Comparing `continuous_eval-0.3.6/continuous_eval/metrics/generation/text/utils.py` & `continuous_eval-0.3.7/continuous_eval/metrics/generation/text/utils.py`

 * *Files identical despite different names*

### Comparing `continuous_eval-0.3.6/continuous_eval/metrics/retrieval/llm_based.py` & `continuous_eval-0.3.7/continuous_eval/metrics/retrieval/llm_based.py`

 * *Files identical despite different names*

### Comparing `continuous_eval-0.3.6/continuous_eval/metrics/retrieval/matching_strategy.py` & `continuous_eval-0.3.7/continuous_eval/metrics/retrieval/matching_strategy.py`

 * *Files identical despite different names*

### Comparing `continuous_eval-0.3.6/continuous_eval/metrics/retrieval/precision_recall_f1.py` & `continuous_eval-0.3.7/continuous_eval/metrics/retrieval/precision_recall_f1.py`

 * *Files identical despite different names*

### Comparing `continuous_eval-0.3.6/continuous_eval/metrics/retrieval/ranked.py` & `continuous_eval-0.3.7/continuous_eval/metrics/retrieval/ranked.py`

 * *Files identical despite different names*

### Comparing `continuous_eval-0.3.6/continuous_eval/metrics/tools/match.py` & `continuous_eval-0.3.7/continuous_eval/metrics/tools/match.py`

 * *Files identical despite different names*

### Comparing `continuous_eval-0.3.6/continuous_eval/utils/telemetry.py` & `continuous_eval-0.3.7/continuous_eval/utils/telemetry.py`

 * *Files identical despite different names*

### Comparing `continuous_eval-0.3.6/pyproject.toml` & `continuous_eval-0.3.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "continuous-eval"
-version = "0.3.6"
+version = "0.3.7"
 description = "Open-Source Evaluation for GenAI Application Pipelines."
 authors = ["Yi Zhang <yi@relari.ai>", "Pasquale Antonante <pasquale@relari.ai>"]
 readme = "README.md"
 license = "Apache-2.0"
 packages = [{include = "continuous_eval"}]
 
 [tool.poetry.dependencies]
```

### Comparing `continuous_eval-0.3.6/PKG-INFO` & `continuous_eval-0.3.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: continuous-eval
-Version: 0.3.6
+Version: 0.3.7
 Summary: Open-Source Evaluation for GenAI Application Pipelines.
 License: Apache-2.0
 Author: Yi Zhang
 Author-email: yi@relari.ai
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: continuous-eval Version: 0.3.6 Summary: Open-Source
+Metadata-Version: 2.1 Name: continuous-eval Version: 0.3.7 Summary: Open-Source
 Evaluation for GenAI Application Pipelines. License: Apache-2.0 Author: Yi
 Zhang Author-email: yi@relari.ai Requires-Python: >=3.9,<4.0 Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: anthropic Provides-Extra: bedrock Provides-Extra: cohere
```


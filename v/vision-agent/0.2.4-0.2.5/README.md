# Comparing `tmp/vision_agent-0.2.4.tar.gz` & `tmp/vision_agent-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vision_agent-0.2.4.tar", max compression
+gzip compressed data, was "vision_agent-0.2.5.tar", max compression
```

## Comparing `vision_agent-0.2.4.tar` & `vision_agent-0.2.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0    11357 2024-04-24 18:03:21.372106 vision_agent-0.2.4/LICENSE
--rw-r--r--   0        0        0     6639 2024-04-24 18:03:21.372106 vision_agent-0.2.4/README.md
--rw-r--r--   0        0        0     2099 2024-04-24 18:03:21.936108 vision_agent-0.2.4/pyproject.toml
--rw-r--r--   0        0        0      108 2024-04-24 18:03:21.384106 vision_agent-0.2.4/vision_agent/__init__.py
--rw-r--r--   0        0        0      127 2024-04-24 18:03:21.384106 vision_agent-0.2.4/vision_agent/agent/__init__.py
--rw-r--r--   0        0        0      529 2024-04-24 18:03:21.384106 vision_agent-0.2.4/vision_agent/agent/agent.py
--rw-r--r--   0        0        0    11511 2024-04-24 18:03:21.384106 vision_agent-0.2.4/vision_agent/agent/easytool.py
--rw-r--r--   0        0        0     4526 2024-04-24 18:03:21.384106 vision_agent-0.2.4/vision_agent/agent/easytool_prompts.py
--rw-r--r--   0        0        0    10506 2024-04-24 18:03:21.384106 vision_agent-0.2.4/vision_agent/agent/reflexion.py
--rw-r--r--   0        0        0     9342 2024-04-24 18:03:21.384106 vision_agent-0.2.4/vision_agent/agent/reflexion_prompts.py
--rw-r--r--   0        0        0    24849 2024-04-24 18:03:21.384106 vision_agent-0.2.4/vision_agent/agent/vision_agent.py
--rw-r--r--   0        0        0     7342 2024-04-24 18:03:21.384106 vision_agent-0.2.4/vision_agent/agent/vision_agent_prompts.py
--rw-r--r--   0        0        0        0 2024-04-24 18:03:21.384106 vision_agent-0.2.4/vision_agent/fonts/__init__.py
--rw-r--r--   0        0        0  1594400 2024-04-24 18:03:21.396106 vision_agent-0.2.4/vision_agent/fonts/default_font_ch_en.ttf
--rw-r--r--   0        0        0     7554 2024-04-24 18:03:21.396106 vision_agent-0.2.4/vision_agent/image_utils.py
--rw-r--r--   0        0        0       48 2024-04-24 18:03:21.396106 vision_agent-0.2.4/vision_agent/llm/__init__.py
--rw-r--r--   0        0        0     5383 2024-04-24 18:03:21.396106 vision_agent-0.2.4/vision_agent/llm/llm.py
--rw-r--r--   0        0        0       67 2024-04-24 18:03:21.396106 vision_agent-0.2.4/vision_agent/lmm/__init__.py
--rw-r--r--   0        0        0    10552 2024-04-24 18:03:21.396106 vision_agent-0.2.4/vision_agent/lmm/lmm.py
--rw-r--r--   0        0        0      413 2024-04-24 18:03:21.396106 vision_agent-0.2.4/vision_agent/tools/__init__.py
--rw-r--r--   0        0        0     1430 2024-04-24 18:03:21.396106 vision_agent-0.2.4/vision_agent/tools/prompts.py
--rw-r--r--   0        0        0    42779 2024-04-24 18:03:21.396106 vision_agent-0.2.4/vision_agent/tools/tools.py
--rw-r--r--   0        0        0     7653 2024-04-24 18:03:21.396106 vision_agent-0.2.4/vision_agent/tools/video.py
--rw-r--r--   0        0        0     1792 2024-04-24 18:03:21.396106 vision_agent-0.2.4/vision_agent/type_defs.py
--rw-r--r--   0        0        0     7697 1970-01-01 00:00:00.000000 vision_agent-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-25 04:26:04.208605 vision_agent-0.2.5/LICENSE
+-rw-r--r--   0        0        0     6639 2024-04-25 04:26:04.208605 vision_agent-0.2.5/README.md
+-rw-r--r--   0        0        0     2099 2024-04-25 04:26:04.800603 vision_agent-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0      108 2024-04-25 04:26:04.220605 vision_agent-0.2.5/vision_agent/__init__.py
+-rw-r--r--   0        0        0      127 2024-04-25 04:26:04.220605 vision_agent-0.2.5/vision_agent/agent/__init__.py
+-rw-r--r--   0        0        0      529 2024-04-25 04:26:04.220605 vision_agent-0.2.5/vision_agent/agent/agent.py
+-rw-r--r--   0        0        0    11511 2024-04-25 04:26:04.220605 vision_agent-0.2.5/vision_agent/agent/easytool.py
+-rw-r--r--   0        0        0     4526 2024-04-25 04:26:04.220605 vision_agent-0.2.5/vision_agent/agent/easytool_prompts.py
+-rw-r--r--   0        0        0    10506 2024-04-25 04:26:04.220605 vision_agent-0.2.5/vision_agent/agent/reflexion.py
+-rw-r--r--   0        0        0     9342 2024-04-25 04:26:04.220605 vision_agent-0.2.5/vision_agent/agent/reflexion_prompts.py
+-rw-r--r--   0        0        0    25195 2024-04-25 04:26:04.220605 vision_agent-0.2.5/vision_agent/agent/vision_agent.py
+-rw-r--r--   0        0        0     7342 2024-04-25 04:26:04.220605 vision_agent-0.2.5/vision_agent/agent/vision_agent_prompts.py
+-rw-r--r--   0        0        0        0 2024-04-25 04:26:04.220605 vision_agent-0.2.5/vision_agent/fonts/__init__.py
+-rw-r--r--   0        0        0  1594400 2024-04-25 04:26:04.232605 vision_agent-0.2.5/vision_agent/fonts/default_font_ch_en.ttf
+-rw-r--r--   0        0        0     7554 2024-04-25 04:26:04.232605 vision_agent-0.2.5/vision_agent/image_utils.py
+-rw-r--r--   0        0        0       48 2024-04-25 04:26:04.232605 vision_agent-0.2.5/vision_agent/llm/__init__.py
+-rw-r--r--   0        0        0     5383 2024-04-25 04:26:04.232605 vision_agent-0.2.5/vision_agent/llm/llm.py
+-rw-r--r--   0        0        0       67 2024-04-25 04:26:04.232605 vision_agent-0.2.5/vision_agent/lmm/__init__.py
+-rw-r--r--   0        0        0    10539 2024-04-25 04:26:04.232605 vision_agent-0.2.5/vision_agent/lmm/lmm.py
+-rw-r--r--   0        0        0      413 2024-04-25 04:26:04.232605 vision_agent-0.2.5/vision_agent/tools/__init__.py
+-rw-r--r--   0        0        0     1430 2024-04-25 04:26:04.232605 vision_agent-0.2.5/vision_agent/tools/prompts.py
+-rw-r--r--   0        0        0    42779 2024-04-25 04:26:04.232605 vision_agent-0.2.5/vision_agent/tools/tools.py
+-rw-r--r--   0        0        0     7653 2024-04-25 04:26:04.232605 vision_agent-0.2.5/vision_agent/tools/video.py
+-rw-r--r--   0        0        0     1792 2024-04-25 04:26:04.232605 vision_agent-0.2.5/vision_agent/type_defs.py
+-rw-r--r--   0        0        0     7697 1970-01-01 00:00:00.000000 vision_agent-0.2.5/PKG-INFO
```

### Comparing `vision_agent-0.2.4/LICENSE` & `vision_agent-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `vision_agent-0.2.4/README.md` & `vision_agent-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `vision_agent-0.2.4/pyproject.toml` & `vision_agent-0.2.5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "vision-agent"
-version = "0.2.4"
+version = "0.2.5"
 description = "Toolset for Vision Agent"
 authors = ["Landing AI <dev@landing.ai>"]
 readme = "README.md"
 packages = [{include = "vision_agent"}]
 
 [tool.poetry.urls]
 "Homepage" = "https://landing.ai"
```

### Comparing `vision_agent-0.2.4/vision_agent/agent/agent.py` & `vision_agent-0.2.5/vision_agent/agent/agent.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.2.4/vision_agent/agent/easytool.py` & `vision_agent-0.2.5/vision_agent/agent/easytool.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.2.4/vision_agent/agent/easytool_prompts.py` & `vision_agent-0.2.5/vision_agent/agent/easytool_prompts.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.2.4/vision_agent/agent/reflexion.py` & `vision_agent-0.2.5/vision_agent/agent/reflexion.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.2.4/vision_agent/agent/reflexion_prompts.py` & `vision_agent-0.2.5/vision_agent/agent/reflexion_prompts.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.2.4/vision_agent/agent/vision_agent.py` & `vision_agent-0.2.5/vision_agent/agent/vision_agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -362,14 +362,28 @@
         image_to_data[image]["masks"].extend(call_result.get("masks", []))
         if "mask_shape" in call_result:
             image_to_data[image]["mask_shape"] = call_result["mask_shape"]
 
     return image_to_data
 
 
+def sample_n_evenly_spaced(lst: Sequence, n: int) -> Sequence:
+    if n <= 0:
+        return []
+    elif len(lst) == 0:
+        return []
+    elif n == 1:
+        return [lst[0]]
+    elif n >= len(lst):
+        return lst
+
+    spacing = (len(lst) - 1) / (n - 1)
+    return [lst[round(spacing * i)] for i in range(n)]
+
+
 def visualize_result(all_tool_results: List[Dict]) -> Sequence[Union[str, Path]]:
     image_to_data: Dict[str, Dict] = {}
     for tool_result in all_tool_results:
         # only handle bbox/mask tools or frame extraction
         if tool_result["tool_name"] not in [
             "grounding_sam_",
             "grounding_dino_",
@@ -580,15 +594,15 @@
                 task_depend[task["id"]]["call_result"] = call_results  # type: ignore
             final_answer = answer_summarize(
                 self.answer_model, question, answers, reflections
             )
             visualized_output = visualize_result(all_tool_results)
             all_tool_results.append({"visualized_output": visualized_output})
             if len(visualized_output) > 0:
-                reflection_images = visualized_output
+                reflection_images = sample_n_evenly_spaced(visualized_output, 3)
             elif image is not None:
                 reflection_images = [image]
             else:
                 reflection_images = None
             reflection = self_reflect(
                 self.reflect_model,
                 question,
```

### Comparing `vision_agent-0.2.4/vision_agent/agent/vision_agent_prompts.py` & `vision_agent-0.2.5/vision_agent/agent/vision_agent_prompts.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.2.4/vision_agent/fonts/default_font_ch_en.ttf` & `vision_agent-0.2.5/vision_agent/fonts/default_font_ch_en.ttf`

 * *Files identical despite different names*

### Comparing `vision_agent-0.2.4/vision_agent/image_utils.py` & `vision_agent-0.2.5/vision_agent/image_utils.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.2.4/vision_agent/llm/llm.py` & `vision_agent-0.2.5/vision_agent/llm/llm.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.2.4/vision_agent/lmm/lmm.py` & `vision_agent-0.2.5/vision_agent/lmm/lmm.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,18 +5,15 @@
 from abc import ABC, abstractmethod
 from pathlib import Path
 from typing import Any, Callable, Dict, List, Optional, Union, cast
 
 import requests
 from openai import AzureOpenAI, OpenAI
 
-from vision_agent.tools import (
-    CHOOSE_PARAMS,
-    SYSTEM_PROMPT,
-)
+from vision_agent.tools import CHOOSE_PARAMS, SYSTEM_PROMPT
 
 _LOGGER = logging.getLogger(__name__)
 
 _LLAVA_ENDPOINT = "https://svtswgdnleslqcsjvilau4p6u40jwrkn.lambda-url.us-east-2.on.aws"
 
 
 def encode_image(image: Union[str, Path]) -> str:
```

### Comparing `vision_agent-0.2.4/vision_agent/tools/prompts.py` & `vision_agent-0.2.5/vision_agent/tools/prompts.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.2.4/vision_agent/tools/tools.py` & `vision_agent-0.2.5/vision_agent/tools/tools.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 from vision_agent.image_utils import (
     convert_to_b64,
     denormalize_bbox,
     get_image_size,
     normalize_bbox,
     rle_decode,
 )
+from vision_agent.lmm import OpenAILMM
 from vision_agent.tools.video import extract_frames_from_video
 from vision_agent.type_defs import LandingaiAPIKey
-from vision_agent.lmm import OpenAILMM
 
 _LOGGER = logging.getLogger(__name__)
 _LND_API_KEY = LandingaiAPIKey().api_key
 _LND_API_URL = "https://api.dev.landing.ai/v1/agent"
 
 
 class Tool(ABC):
```

### Comparing `vision_agent-0.2.4/vision_agent/tools/video.py` & `vision_agent-0.2.5/vision_agent/tools/video.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.2.4/vision_agent/type_defs.py` & `vision_agent-0.2.5/vision_agent/type_defs.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.2.4/PKG-INFO` & `vision_agent-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vision-agent
-Version: 0.2.4
+Version: 0.2.5
 Summary: Toolset for Vision Agent
 Author: Landing AI
 Author-email: dev@landing.ai
 Requires-Python: >=3.9
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```


# Comparing `tmp/vision_agent-0.2.5.tar.gz` & `tmp/vision_agent-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vision_agent-0.2.5.tar", max compression
+gzip compressed data, was "vision_agent-0.2.6.tar", max compression
```

## Comparing `vision_agent-0.2.5.tar` & `vision_agent-0.2.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0    11357 2024-04-25 04:26:04.208605 vision_agent-0.2.5/LICENSE
--rw-r--r--   0        0        0     6639 2024-04-25 04:26:04.208605 vision_agent-0.2.5/README.md
--rw-r--r--   0        0        0     2099 2024-04-25 04:26:04.800603 vision_agent-0.2.5/pyproject.toml
--rw-r--r--   0        0        0      108 2024-04-25 04:26:04.220605 vision_agent-0.2.5/vision_agent/__init__.py
--rw-r--r--   0        0        0      127 2024-04-25 04:26:04.220605 vision_agent-0.2.5/vision_agent/agent/__init__.py
--rw-r--r--   0        0        0      529 2024-04-25 04:26:04.220605 vision_agent-0.2.5/vision_agent/agent/agent.py
--rw-r--r--   0        0        0    11511 2024-04-25 04:26:04.220605 vision_agent-0.2.5/vision_agent/agent/easytool.py
--rw-r--r--   0        0        0     4526 2024-04-25 04:26:04.220605 vision_agent-0.2.5/vision_agent/agent/easytool_prompts.py
--rw-r--r--   0        0        0    10506 2024-04-25 04:26:04.220605 vision_agent-0.2.5/vision_agent/agent/reflexion.py
--rw-r--r--   0        0        0     9342 2024-04-25 04:26:04.220605 vision_agent-0.2.5/vision_agent/agent/reflexion_prompts.py
--rw-r--r--   0        0        0    25195 2024-04-25 04:26:04.220605 vision_agent-0.2.5/vision_agent/agent/vision_agent.py
--rw-r--r--   0        0        0     7342 2024-04-25 04:26:04.220605 vision_agent-0.2.5/vision_agent/agent/vision_agent_prompts.py
--rw-r--r--   0        0        0        0 2024-04-25 04:26:04.220605 vision_agent-0.2.5/vision_agent/fonts/__init__.py
--rw-r--r--   0        0        0  1594400 2024-04-25 04:26:04.232605 vision_agent-0.2.5/vision_agent/fonts/default_font_ch_en.ttf
--rw-r--r--   0        0        0     7554 2024-04-25 04:26:04.232605 vision_agent-0.2.5/vision_agent/image_utils.py
--rw-r--r--   0        0        0       48 2024-04-25 04:26:04.232605 vision_agent-0.2.5/vision_agent/llm/__init__.py
--rw-r--r--   0        0        0     5383 2024-04-25 04:26:04.232605 vision_agent-0.2.5/vision_agent/llm/llm.py
--rw-r--r--   0        0        0       67 2024-04-25 04:26:04.232605 vision_agent-0.2.5/vision_agent/lmm/__init__.py
--rw-r--r--   0        0        0    10539 2024-04-25 04:26:04.232605 vision_agent-0.2.5/vision_agent/lmm/lmm.py
--rw-r--r--   0        0        0      413 2024-04-25 04:26:04.232605 vision_agent-0.2.5/vision_agent/tools/__init__.py
--rw-r--r--   0        0        0     1430 2024-04-25 04:26:04.232605 vision_agent-0.2.5/vision_agent/tools/prompts.py
--rw-r--r--   0        0        0    42779 2024-04-25 04:26:04.232605 vision_agent-0.2.5/vision_agent/tools/tools.py
--rw-r--r--   0        0        0     7653 2024-04-25 04:26:04.232605 vision_agent-0.2.5/vision_agent/tools/video.py
--rw-r--r--   0        0        0     1792 2024-04-25 04:26:04.232605 vision_agent-0.2.5/vision_agent/type_defs.py
--rw-r--r--   0        0        0     7697 1970-01-01 00:00:00.000000 vision_agent-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-25 06:01:28.383648 vision_agent-0.2.6/LICENSE
+-rw-r--r--   0        0        0     6639 2024-04-25 06:01:28.383648 vision_agent-0.2.6/README.md
+-rw-r--r--   0        0        0     2099 2024-04-25 06:01:28.939650 vision_agent-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0      108 2024-04-25 06:01:28.395648 vision_agent-0.2.6/vision_agent/__init__.py
+-rw-r--r--   0        0        0      127 2024-04-25 06:01:28.395648 vision_agent-0.2.6/vision_agent/agent/__init__.py
+-rw-r--r--   0        0        0      529 2024-04-25 06:01:28.395648 vision_agent-0.2.6/vision_agent/agent/agent.py
+-rw-r--r--   0        0        0    11511 2024-04-25 06:01:28.395648 vision_agent-0.2.6/vision_agent/agent/easytool.py
+-rw-r--r--   0        0        0     4526 2024-04-25 06:01:28.395648 vision_agent-0.2.6/vision_agent/agent/easytool_prompts.py
+-rw-r--r--   0        0        0    10506 2024-04-25 06:01:28.395648 vision_agent-0.2.6/vision_agent/agent/reflexion.py
+-rw-r--r--   0        0        0     9342 2024-04-25 06:01:28.395648 vision_agent-0.2.6/vision_agent/agent/reflexion_prompts.py
+-rw-r--r--   0        0        0    25971 2024-04-25 06:01:28.395648 vision_agent-0.2.6/vision_agent/agent/vision_agent.py
+-rw-r--r--   0        0        0     7342 2024-04-25 06:01:28.395648 vision_agent-0.2.6/vision_agent/agent/vision_agent_prompts.py
+-rw-r--r--   0        0        0        0 2024-04-25 06:01:28.395648 vision_agent-0.2.6/vision_agent/fonts/__init__.py
+-rw-r--r--   0        0        0  1594400 2024-04-25 06:01:28.407648 vision_agent-0.2.6/vision_agent/fonts/default_font_ch_en.ttf
+-rw-r--r--   0        0        0     7552 2024-04-25 06:01:28.407648 vision_agent-0.2.6/vision_agent/image_utils.py
+-rw-r--r--   0        0        0       48 2024-04-25 06:01:28.407648 vision_agent-0.2.6/vision_agent/llm/__init__.py
+-rw-r--r--   0        0        0     5383 2024-04-25 06:01:28.407648 vision_agent-0.2.6/vision_agent/llm/llm.py
+-rw-r--r--   0        0        0       67 2024-04-25 06:01:28.407648 vision_agent-0.2.6/vision_agent/lmm/__init__.py
+-rw-r--r--   0        0        0    10539 2024-04-25 06:01:28.407648 vision_agent-0.2.6/vision_agent/lmm/lmm.py
+-rw-r--r--   0        0        0      413 2024-04-25 06:01:28.407648 vision_agent-0.2.6/vision_agent/tools/__init__.py
+-rw-r--r--   0        0        0     1430 2024-04-25 06:01:28.407648 vision_agent-0.2.6/vision_agent/tools/prompts.py
+-rw-r--r--   0        0        0    43013 2024-04-25 06:01:28.407648 vision_agent-0.2.6/vision_agent/tools/tools.py
+-rw-r--r--   0        0        0     7653 2024-04-25 06:01:28.407648 vision_agent-0.2.6/vision_agent/tools/video.py
+-rw-r--r--   0        0        0     1792 2024-04-25 06:01:28.407648 vision_agent-0.2.6/vision_agent/type_defs.py
+-rw-r--r--   0        0        0     7697 1970-01-01 00:00:00.000000 vision_agent-0.2.6/PKG-INFO
```

### Comparing `vision_agent-0.2.5/LICENSE` & `vision_agent-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `vision_agent-0.2.5/README.md` & `vision_agent-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `vision_agent-0.2.5/pyproject.toml` & `vision_agent-0.2.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "vision-agent"
-version = "0.2.5"
+version = "0.2.6"
 description = "Toolset for Vision Agent"
 authors = ["Landing AI <dev@landing.ai>"]
 readme = "README.md"
 packages = [{include = "vision_agent"}]
 
 [tool.poetry.urls]
 "Homepage" = "https://landing.ai"
```

### Comparing `vision_agent-0.2.5/vision_agent/agent/agent.py` & `vision_agent-0.2.6/vision_agent/agent/agent.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.2.5/vision_agent/agent/easytool.py` & `vision_agent-0.2.6/vision_agent/agent/easytool.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.2.5/vision_agent/agent/easytool_prompts.py` & `vision_agent-0.2.6/vision_agent/agent/easytool_prompts.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.2.5/vision_agent/agent/reflexion.py` & `vision_agent-0.2.6/vision_agent/agent/reflexion.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.2.5/vision_agent/agent/reflexion_prompts.py` & `vision_agent-0.2.6/vision_agent/agent/reflexion_prompts.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.2.5/vision_agent/agent/vision_agent.py` & `vision_agent-0.2.6/vision_agent/agent/vision_agent.py`

 * *Files 3% similar despite different names*

```diff
@@ -310,14 +310,15 @@
     for video_file_output in tool_result["call_results"]:
         for frame, _ in video_file_output:
             image = frame
             if image not in image_to_data:
                 image_to_data[image] = {
                     "bboxes": [],
                     "masks": [],
+                    "heat_map": [],
                     "labels": [],
                     "scores": [],
                 }
     return image_to_data
 
 
 def _handle_viz_tools(
@@ -336,34 +337,40 @@
     elif isinstance(tool_result["parameters"], list):
         if len(tool_result["parameters"]) < 1 or (
             "image" not in tool_result["parameters"][0]
         ):
             return image_to_data
 
     for param, call_result in zip(parameters, tool_result["call_results"]):
-        # calls can fail, so we need to check if the call was successful
+        # Calls can fail, so we need to check if the call was successful. It can either:
+        # 1. return a str or some error that's not a dictionary
+        # 2. return a dictionary but not have the necessary keys
+
         if not isinstance(call_result, dict) or (
-            "bboxes" not in call_result and "masks" not in call_result
+            "bboxes" not in call_result and "heat_map" not in call_result
         ):
             return image_to_data
 
         # if the call was successful, then we can add the image data
         image = param["image"]
         if image not in image_to_data:
             image_to_data[image] = {
                 "bboxes": [],
                 "masks": [],
+                "heat_map": [],
                 "labels": [],
                 "scores": [],
             }
 
         image_to_data[image]["bboxes"].extend(call_result.get("bboxes", []))
         image_to_data[image]["labels"].extend(call_result.get("labels", []))
         image_to_data[image]["scores"].extend(call_result.get("scores", []))
         image_to_data[image]["masks"].extend(call_result.get("masks", []))
+        # only single heatmap is returned
+        image_to_data[image]["heat_map"].append(call_result.get("heat_map", []))
         if "mask_shape" in call_result:
             image_to_data[image]["mask_shape"] = call_result["mask_shape"]
 
     return image_to_data
 
 
 def sample_n_evenly_spaced(lst: Sequence, n: int) -> Sequence:
@@ -476,17 +483,22 @@
         image: Optional[Union[str, Path]] = None,
         reference_data: Optional[Dict[str, str]] = None,
         visualize_output: Optional[bool] = False,
     ) -> str:
         """Invoke the vision agent.
 
         Parameters:
-            input: a prompt that describe the task or a conversation in the format of
+            chat: A conversation in the format of
                 [{"role": "user", "content": "describe your task here..."}].
-            image: the input image referenced in the prompt parameter.
+            image: The input image referenced in the chat parameter.
+            reference_data: A dictionary containing the reference image, mask or bounding
+                box in the format of:
+                {"image": "image.jpg", "mask": "mask.jpg", "bbox": [0.1, 0.2, 0.1, 0.2]}
+                where the bounding box coordinates are normalized.
+            visualize_output: Whether to visualize the output.
 
         Returns:
             The result of the vision agent in text.
         """
         if isinstance(input, str):
             input = [{"role": "user", "content": input}]
         return self.chat(
@@ -518,20 +530,22 @@
         image: Optional[Union[str, Path]] = None,
         reference_data: Optional[Dict[str, str]] = None,
         visualize_output: Optional[bool] = False,
     ) -> Tuple[str, List[Dict]]:
         """Chat with the vision agent and return the final answer and all tool results.
 
         Parameters:
-            chat: a conversation in the format of
+            chat: A conversation in the format of
                 [{"role": "user", "content": "describe your task here..."}].
-            image: the input image referenced in the chat parameter.
-            reference_data: a dictionary containing the reference image and mask. in the
-                format of {"image": "image.jpg", "mask": "mask.jpg}
-            visualize_output: whether to visualize the output.
+            image: The input image referenced in the chat parameter.
+            reference_data: A dictionary containing the reference image, mask or bounding
+                box in the format of:
+                {"image": "image.jpg", "mask": "mask.jpg", "bbox": [0.1, 0.2, 0.1, 0.2]}
+                where the bounding box coordinates are normalized.
+            visualize_output: Whether to visualize the output.
 
         Returns:
             A tuple where the first item is the final answer and the second item is a
             list of all the tool results. The last item in the tool results also
             contains the visualized output.
         """
         question = chat[0]["content"]
```

### Comparing `vision_agent-0.2.5/vision_agent/agent/vision_agent_prompts.py` & `vision_agent-0.2.6/vision_agent/agent/vision_agent_prompts.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.2.5/vision_agent/fonts/default_font_ch_en.ttf` & `vision_agent-0.2.6/vision_agent/fonts/default_font_ch_en.ttf`

 * *Files identical despite different names*

### Comparing `vision_agent-0.2.5/vision_agent/image_utils.py` & `vision_agent-0.2.6/vision_agent/image_utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -207,25 +207,25 @@
         masks["labels"] = [""] * len(masks["masks"])
 
     color = {
         label: COLORS[i % len(COLORS)] for i, label in enumerate(set(masks["labels"]))
     }
 
     for label, mask in zip(masks["labels"], masks["masks"]):
-        if isinstance(mask, str):
+        if isinstance(mask, str) or isinstance(mask, Path):
             mask = np.array(Image.open(mask))
         np_mask = np.zeros((image.size[1], image.size[0], 4))
         np_mask[mask > 0, :] = color[label] + (255 * alpha,)
         mask_img = Image.fromarray(np_mask.astype(np.uint8))
         image = Image.alpha_composite(image.convert("RGBA"), mask_img)
     return image.convert("RGB")
 
 
 def overlay_heat_map(
-    image: Union[str, Path, np.ndarray, ImageType], masks: Dict, alpha: float = 0.8
+    image: Union[str, Path, np.ndarray, ImageType], heat_map: Dict, alpha: float = 0.8
 ) -> ImageType:
     r"""Plots heat map on to an image.
 
     Parameters:
         image: the input image
         masks: the heatmap to overlay
         alpha: the transparency of the overlay
@@ -234,22 +234,20 @@
         The image with the heatmap overlayed
     """
     if isinstance(image, (str, Path)):
         image = Image.open(image)
     elif isinstance(image, np.ndarray):
         image = Image.fromarray(image)
 
-    if "masks" not in masks:
+    if "heat_map" not in heat_map:
         return image.convert("RGB")
 
-    # Only one heat map per image, so no need to loop through masks
     image = image.convert("L")
-
-    if isinstance(masks["masks"][0], str):
-        mask = b64_to_pil(masks["masks"][0])
+    # Only one heat map per image, so no need to loop through masks
+    mask = Image.fromarray(heat_map["heat_map"][0])
 
     overlay = Image.new("RGBA", mask.size)
     odraw = ImageDraw.Draw(overlay)
     odraw.bitmap(
         (0, 0), mask, fill=(255, 0, 0, round(alpha * 255))
     )  # fill=(R, G, B, Alpha)
     combined = Image.alpha_composite(image.convert("RGBA"), overlay.resize(image.size))
```

### Comparing `vision_agent-0.2.5/vision_agent/llm/llm.py` & `vision_agent-0.2.6/vision_agent/llm/llm.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.2.5/vision_agent/lmm/lmm.py` & `vision_agent-0.2.6/vision_agent/lmm/lmm.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.2.5/vision_agent/tools/prompts.py` & `vision_agent-0.2.6/vision_agent/tools/prompts.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.2.5/vision_agent/tools/tools.py` & `vision_agent-0.2.6/vision_agent/tools/tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 import numpy as np
 import requests
 from PIL import Image
 from PIL.Image import Image as ImageType
 
 from vision_agent.image_utils import (
+    b64_to_pil,
     convert_to_b64,
     denormalize_bbox,
     get_image_size,
     normalize_bbox,
     rle_decode,
 )
 from vision_agent.lmm import OpenAILMM
@@ -512,15 +513,17 @@
             A dictionary containing the key 'count' and the count as value. E.g. {count: 12}
         """
         image_b64 = convert_to_b64(image)
         data = {
             "image": image_b64,
             "tool": "zero_shot_counting",
         }
-        return _send_inference_request(data, "tools")
+        resp_data = _send_inference_request(data, "tools")
+        resp_data["heat_map"] = np.array(b64_to_pil(resp_data["heat_map"][0]))
+        return resp_data
 
 
 class VisualPromptCounting(Tool):
     r"""VisualPromptCounting is a tool that can count total number of instances of an object
     present in an image belonging to same class with help of an visual prompt which is a bounding box.
 
     Example
@@ -581,15 +584,17 @@
         image_b64 = convert_to_b64(image)
 
         data = {
             "image": image_b64,
             "prompt": prompt,
             "tool": "few_shot_counting",
         }
-        return _send_inference_request(data, "tools")
+        resp_data = _send_inference_request(data, "tools")
+        resp_data["heat_map"] = np.array(b64_to_pil(resp_data["heat_map"][0]))
+        return resp_data
 
 
 class VisualQuestionAnswering(Tool):
     r"""VisualQuestionAnswering is a tool that can explain contents of an image and answer questions about the same
 
     Example
     -------
```

### Comparing `vision_agent-0.2.5/vision_agent/tools/video.py` & `vision_agent-0.2.6/vision_agent/tools/video.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.2.5/vision_agent/type_defs.py` & `vision_agent-0.2.6/vision_agent/type_defs.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.2.5/PKG-INFO` & `vision_agent-0.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vision-agent
-Version: 0.2.5
+Version: 0.2.6
 Summary: Toolset for Vision Agent
 Author: Landing AI
 Author-email: dev@landing.ai
 Requires-Python: >=3.9
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```


# Comparing `tmp/uform-2.1.1.tar.gz` & `tmp/uform-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uform-2.1.1.tar", last modified: Tue Apr 16 03:56:09 2024, max compression
+gzip compressed data, was "uform-3.0.1.tar", last modified: Thu Apr 25 03:22:00 2024, max compression
```

## Comparing `uform-2.1.1.tar` & `uform-3.0.1.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:56:09.698954 uform-2.1.1/
--rwxr-xr-x   0 runner    (1001) docker     (127)    11357 2024-04-16 03:56:05.000000 uform-2.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    27269 2024-04-16 03:56:09.698954 uform-2.1.1/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)    25346 2024-04-16 03:56:05.000000 uform-2.1.1/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)     2656 2024-04-16 03:56:05.000000 uform-2.1.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:56:09.694954 uform-2.1.1/python/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:56:09.698954 uform-2.1.1/python/uform/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1963 2024-04-16 03:56:05.000000 uform-2.1.1/python/uform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3359 2024-04-16 03:56:05.000000 uform-2.1.1/python/uform/chat.py
--rw-r--r--   0 runner    (1001) docker     (127)    16130 2024-04-16 03:56:05.000000 uform-2.1.1/python/uform/gen_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3585 2024-04-16 03:56:05.000000 uform-2.1.1/python/uform/numpy_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (127)     8242 2024-04-16 03:56:05.000000 uform-2.1.1/python/uform/onnx_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     3474 2024-04-16 03:56:05.000000 uform-2.1.1/python/uform/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)    16376 2024-04-16 03:56:05.000000 uform-2.1.1/python/uform/torch_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     3054 2024-04-16 03:56:05.000000 uform-2.1.1/python/uform/torch_preprocessor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:56:09.698954 uform-2.1.1/python/uform.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    27269 2024-04-16 03:56:09.000000 uform-2.1.1/python/uform.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-16 03:56:09.000000 uform-2.1.1/python/uform.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 03:56:09.000000 uform-2.1.1/python/uform.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-16 03:56:09.000000 uform-2.1.1/python/uform.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-16 03:56:09.000000 uform-2.1.1/python/uform.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-16 03:56:09.000000 uform-2.1.1/python/uform.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 03:56:09.698954 uform-2.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:22:00.183577 uform-3.0.1/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11357 2024-04-25 03:21:55.000000 uform-3.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    15291 2024-04-25 03:22:00.183577 uform-3.0.1/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)    13249 2024-04-25 03:21:55.000000 uform-3.0.1/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2699 2024-04-25 03:21:55.000000 uform-3.0.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:22:00.179577 uform-3.0.1/python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:22:00.179577 uform-3.0.1/python/uform/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8414 2024-04-25 03:21:55.000000 uform-3.0.1/python/uform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3422 2024-04-25 03:21:55.000000 uform-3.0.1/python/uform/chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-25 03:21:55.000000 uform-3.0.1/python/uform/gen_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4473 2024-04-25 03:21:55.000000 uform-3.0.1/python/uform/numpy_processors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5232 2024-04-25 03:21:55.000000 uform-3.0.1/python/uform/onnx_encoders.py
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-25 03:21:55.000000 uform-3.0.1/python/uform/shared.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16161 2024-04-25 03:21:55.000000 uform-3.0.1/python/uform/torch_decoders.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14158 2024-04-25 03:21:55.000000 uform-3.0.1/python/uform/torch_encoders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3964 2024-04-25 03:21:55.000000 uform-3.0.1/python/uform/torch_processors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 03:22:00.183577 uform-3.0.1/python/uform.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15291 2024-04-25 03:22:00.000000 uform-3.0.1/python/uform.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-25 03:22:00.000000 uform-3.0.1/python/uform.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 03:22:00.000000 uform-3.0.1/python/uform.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-25 03:22:00.000000 uform-3.0.1/python/uform.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-25 03:22:00.000000 uform-3.0.1/python/uform.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-25 03:22:00.000000 uform-3.0.1/python/uform.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 03:22:00.183577 uform-3.0.1/setup.cfg
```

### Comparing `uform-2.1.1/LICENSE` & `uform-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `uform-2.1.1/pyproject.toml` & `uform-3.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -27,32 +27,34 @@
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
     "Topic :: Scientific/Engineering :: Image Processing",
     "Topic :: Scientific/Engineering :: Image Recognition",
 ]
 dependencies = [
     "huggingface_hub>=0.16.4",
     "tokenizers>=0.13.3",
-    "pillow"
+    "pillow",
+    "simsimd",
 ]
 description = "Pocket-Sized Multimodal AI for Content Understanding and Generation"
 maintainers = [
     {email = "info@unum.cloud", name = "Unum Cloud"},
 ]
 name = "uform"
 readme = "README.md"
 requires-python = ">=3.7"
-version = "2.1.1"
+version = "3.0.1"
 
 [project.scripts]
 uform-chat = "uform.chat:main"
 
 [project.optional-dependencies]
 torch = ["torch>=1.13.1", "torchvision", "transformers>=4.36.2"]
 onnx = ["onnx>=1.15.0", "onnxruntime>=1.17.1", "numpy"]
 onnx-gpu = ["onnx>=1.15.0", "onnxruntime-gpu>=1.17.1", "numpy"]
+dev = ["pytest", "pandas"]
 
 [project.urls]
 "Homepage" = "https://github.com/unum-cloud/uform"
 
 [tool.setuptools.packages.find]
 where = ["python"]
 include = ["uform"]
```

### Comparing `uform-2.1.1/python/uform/chat.py` & `uform-3.0.1/python/uform/chat.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,55 +1,47 @@
 from argparse import ArgumentParser
 
 import requests
 import torch
 from PIL import Image
-from transformers import TextStreamer
-
-from uform.gen_model import VLMForCausalLM, VLMProcessor
-
-EOS_TOKEN = 32001
+from transformers import TextStreamer, AutoModel, AutoProcessor
 
 
 def parse_args():
     parser = ArgumentParser(description="Chat with UForm generative model")
 
-    parser.add_argument("--model", type=str, default="unum-cloud/uform-gen-chat")
-    parser.add_argument("--image", type=str, help="", required=True)
-    parser.add_argument("--device", type=str, required=True)
-    parser.add_argument("--fp16", action="store_true")
+    parser.add_argument("--model", type=str, default="unum-cloud/uform-gen-chat", help="Model name or path")
+    parser.add_argument("--image", type=str, required=True, help="Path to image or URL")
+    parser.add_argument("--device", type=str, required=True, help="Device to run on, like `cpu` or `cuda:0`")
+    parser.add_argument("--fp16", action="store_true", help="Use half-precision math for faster inference")
 
     return parser.parse_args()
 
 
 def run_chat(opts, model, processor):
     streamer = TextStreamer(
         processor.tokenizer,
         skip_prompt=True,
         skip_special_tokens=True,
     )
 
     messages = [{"role": "system", "content": "You are a helpful assistant."}]
     is_first_message = True
+
     if opts.image.startswith("http"):
-        image = (
-            processor.image_processor(
-                Image.open(requests.get(opts.image, stream=True).raw),
-            )
-            .unsqueeze(0)
-            .to(torch.bfloat16 if opts.fp16 else torch.float32)
-            .to(opts.device)
-        )
+        image = Image.open(requests.get(opts.image, stream=True).raw)
     else:
-        image = (
-            processor.image_processor(Image.open(opts.image))
-            .unsqueeze(0)
-            .to(torch.bfloat16 if opts.fp16 else torch.float32)
-            .to(opts.device)
-        )
+        image = Image.open(opts.image)
+
+    image = (
+        processor.feature_extractor(image)  #
+        .unsqueeze(0)
+        .to(torch.bfloat16 if opts.fp16 else torch.float32)
+        .to(opts.device)
+    )
 
     while True:
         if messages[-1]["role"] in ("system", "assistant"):
             message = input("User: ")
             if is_first_message:
                 message = f" <image> {message}"
                 is_first_message = False
@@ -64,51 +56,53 @@
                 add_generation_prompt=True,
             ).to(opts.device)
 
             attention_mask = torch.ones(
                 1,
                 input_ids.shape[1] + processor.num_image_latents - 1,
             ).to(opts.device)
-            x = {
+            inputs = {
                 "input_ids": input_ids,
                 "attention_mask": attention_mask,
                 "images": image,
             }
 
             print("Assistant: ", end="")
             with torch.inference_mode():
-                y = model.generate(
-                    **x,
+                output = model.generate(
+                    **inputs,
                     do_sample=False,
                     use_cache=True,
                     max_new_tokens=1024,
-                    eos_token_id=EOS_TOKEN,
+                    eos_token_id=151645,
                     pad_token_id=processor.tokenizer.pad_token_id,
                     streamer=streamer,
                 )
             print()
 
-            message = processor.batch_decode(y[:, x["input_ids"].shape[1] : -1])[0]
+            prompt_len = inputs["input_ids"].shape[1]
+            message = processor.batch_decode(output[:, prompt_len:-1])[0]
 
             messages.append({"role": "assistant", "content": message})
 
 
 def main():
     try:
         opts = parse_args()
-
+        processor = AutoProcessor.from_pretrained(opts.model, trust_remote_code=True)
         model = (
-            VLMForCausalLM.from_pretrained(
+            AutoModel.from_pretrained(
                 opts.model,
                 torch_dtype=torch.bfloat16 if opts.fp16 else torch.float32,
+                ignore_mismatched_sizes=True,
+                trust_remote_code=True,
             )
             .eval()
             .to(opts.device)
         )
-        processor = VLMProcessor.from_pretrained(opts.model)
 
         run_chat(opts, model, processor)
 
     except KeyboardInterrupt:
         print("Bye!")
         pass
```

### Comparing `uform-2.1.1/python/uform/gen_model.py` & `uform-3.0.1/python/uform/torch_decoders.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 from typing import List, Optional, Tuple, Union
 
 import torch
 import torch.nn.functional as F
 from torch import nn
-from torchvision.transforms import (CenterCrop, Compose, InterpolationMode,
-                                    Normalize, RandomResizedCrop, Resize,
-                                    ToTensor)
+from torchvision.transforms import (
+    CenterCrop,
+    Compose,
+    InterpolationMode,
+    Normalize,
+    RandomResizedCrop,
+    Resize,
+    ToTensor,
+)
 from transformers import AutoConfig, AutoTokenizer
 from transformers.configuration_utils import PretrainedConfig
 from transformers.modeling_outputs import CausalLMOutputWithPast
 from transformers.modeling_utils import PreTrainedModel
-from transformers.models.auto.modeling_auto import (AutoModel,
-                                                    AutoModelForCausalLM)
+from transformers.models.auto.modeling_auto import AutoModel, AutoModelForCausalLM
 from transformers.processing_utils import ProcessorMixin
 from transformers.tokenization_utils_base import BatchEncoding
 
-from uform.torch_models import VisualEncoder
+from uform.torch_encoders import ImageEncoder
 
 IMAGENET_MEAN = (0.48145466, 0.4578275, 0.40821073)
 IMAGENET_STD = (0.26862954, 0.26130258, 0.27577711)
 
 
 def convert_to_rgb(image):
     return image.convert("RGB")
@@ -134,25 +139,25 @@
         super().__init__(config)
 
         self.config = config
         self.text_config = AutoConfig.from_pretrained(config.text_decoder_name_or_path)
         self.text_config.vocab_size += 3
         self.text_decoder = AutoModelForCausalLM.from_config(self.text_config)
 
-        self.image_encoder = VisualEncoder(
+        self.image_encoder = ImageEncoder(
             self.config.image_encoder_hidden_size,
             self.config.image_encoder_patch_size,
             self.config.image_size,
             self.config.image_encoder_num_layers,
             self.config.image_encoder_num_heads,
             self.config.image_encoder_embedding_dim,
             self.config.image_encoder_pooling,
         )
 
-        # replace models' layerscales because `transformers` automatically renames keys in state_dict
+        # replace models' layerscales because `transformers` automatically renames keys in `state_dict`
         for i in range(len(self.image_encoder.blocks)):
             self.image_encoder.blocks[i].ls1 = LayerScale(
                 self.image_encoder.blocks[i].ls1.dim,
             )
             self.image_encoder.blocks[i].ls2 = LayerScale(
                 self.image_encoder.blocks[i].ls2.dim,
             )
@@ -209,29 +214,22 @@
         inputs_embeds: Optional[torch.FloatTensor] = None,
         use_cache: Optional[bool] = None,
         labels: Optional[torch.Tensor] = None,
         output_attentions: Optional[bool] = None,
         output_hidden_states: Optional[bool] = None,
         return_dict: Optional[bool] = None,
     ) -> Union[dict, Tuple, CausalLMOutputWithPast]:
-        output_attentions = (
-            output_attentions
-            if output_attentions is not None
-            else self.config.output_attentions
-        )
+
+        output_attentions = output_attentions if output_attentions is not None else self.config.output_attentions
         output_hidden_states = (
-            output_hidden_states
-            if output_hidden_states is not None
-            else self.config.output_hidden_states
+            output_hidden_states if output_hidden_states is not None else self.config.output_hidden_states
         )
         use_cache = use_cache if use_cache is not None else self.config.use_cache
 
-        return_dict = (
-            return_dict if return_dict is not None else self.config.use_return_dict
-        )
+        return_dict = return_dict if return_dict is not None else self.config.use_return_dict
 
         if input_ids is not None and inputs_embeds is not None:
             raise ValueError(
                 "You cannot specify both input_ids and inputs_embeds at the same time",
             )
         elif input_ids is None and inputs_embeds is None:
             raise ValueError("You have to specify either input_is or inputs_embeds")
@@ -244,19 +242,15 @@
                 inputs_embeds = self.gather_continuous_embeddings(
                     input_ids,
                     inputs_embeds,
                     image_embeds,
                 )
 
         if position_ids is None:
-            seq_length = (
-                inputs_embeds.shape[1]
-                if inputs_embeds is not None
-                else input_ids.shape[1]
-            )
+            seq_length = inputs_embeds.shape[1] if inputs_embeds is not None else input_ids.shape[1]
             past_key_values_length = 0
 
             if past_key_values is not None:
                 past_key_values_length = past_key_values[0][0].shape[2]
 
             device = input_ids.device if input_ids is not None else inputs_embeds.device
             position_ids = torch.arange(
@@ -406,15 +400,18 @@
             attention_mask = F.pad(
                 attention_mask,
                 pad=(0, self.num_image_latents - 1),
                 value=1,
             )
 
             encoding = BatchEncoding(
-                data={"input_ids": input_ids, "attention_mask": attention_mask},
+                data={
+                    "input_ids": input_ids,
+                    "attention_mask": attention_mask,
+                },
             )
 
         if images is not None:
             if isinstance(images, (list, tuple)):
                 image_features = torch.empty(
                     (len(images), 3, self.config.image_size, self.config.image_size),
                     dtype=torch.float32,
@@ -452,13 +449,21 @@
         cache_dir=None,
         force_download: bool = False,
         local_files_only: bool = False,
         token=None,
         revision: str = "main",
         **kwargs,
     ):
-        config = AutoConfig.from_pretrained(pretrained_model_name_or_path)
+        config = AutoConfig.from_pretrained(
+            pretrained_model_name_or_path,
+            cache_dir=cache_dir,
+            force_download=force_download,
+            local_files_only=local_files_only,
+            revision=revision,
+            token=token,
+            **kwargs,
+        )
         return cls(config)
 
 
 AutoConfig.register("vlm", VLMConfig)
 AutoModel.register(VLMConfig, VLMForCausalLM)
```

### Comparing `uform-2.1.1/python/uform/numpy_preprocessor.py` & `uform-3.0.1/python/uform/torch_processors.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,97 +1,124 @@
 from os import PathLike
-from typing import Dict, List, Union
+from typing import Dict, List, Union, Sequence
+import json
 
-from PIL.Image import Image, BICUBIC
+import torch
+from PIL.Image import Image
 from tokenizers import Tokenizer
-import numpy as np
+from torch import Tensor
+from torchvision.transforms import (
+    CenterCrop,
+    Compose,
+    InterpolationMode,
+    Normalize,
+    Resize,
+    ToTensor,
+)
+
+from uform.shared import read_config
+
+
+# lambda is not pickle-able
+def convert_to_rgb(image):
+    return image.convert("RGB")
 
 
-class NumPyProcessor:
-    def __init__(self, config: Dict, tokenizer_path: PathLike):
+class TextProcessor:
+    def __init__(self, config_path: PathLike, tokenizer_path: PathLike):
         """
         :param config: model config
         :param tokenizer_path: path to tokenizer file
-        :param tensor_type: which tensors to return, either pt (PyTorch) or np (NumPy)
         """
 
-        self._image_size = config["image_encoder"]["image_size"]
-        self._max_seq_len = config["text_encoder"]["max_position_embeddings"]
+        config = read_config(config_path)
+        if "text_encoder" in config:
+            config = config["text_encoder"]
+
+        self._max_seq_len = config["max_position_embeddings"]
         self._tokenizer = Tokenizer.from_file(tokenizer_path)
         self._tokenizer.no_padding()
-        self._pad_token_idx = config["text_encoder"]["padding_idx"]
-
-        self.image_mean = np.array([0.48145466, 0.4578275, 0.40821073], dtype=np.float32)[None, None]
-        self.image_std = np.array([0.26862954, 0.26130258, 0.27577711], dtype=np.float32)[None, None]
+        self._pad_token_idx = config["padding_idx"]
 
-    def preprocess_text(self, texts: Union[str, List[str]]) -> Dict[str, np.ndarray]:
+    def __call__(self, texts: Union[str, List[str]]) -> Dict[str, Tensor]:
         """Transforms one or more strings into dictionary with tokenized strings and attention masks.
 
         :param texts: text of list of texts to tokenizer
+        :return: dictionary with tokenized strings and attention masks as values
         """
         if isinstance(texts, str):
             texts = [texts]
 
-        input_ids = np.full(
+        input_ids = torch.full(
             (len(texts), self._max_seq_len),
             fill_value=self._pad_token_idx,
-            dtype=np.int64,
+            dtype=torch.int64,
         )
 
-        attention_mask = np.zeros(
-            (len(texts), self._max_seq_len),
-            dtype=np.int32,
+        attention_mask = torch.zeros(
+            len(texts),
+            self._max_seq_len,
+            dtype=torch.int32,
         )
         encoded = self._tokenizer.encode_batch(texts)
 
         for i, seq in enumerate(encoded):
             seq_len = min(len(seq), self._max_seq_len)
-            input_ids[i, :seq_len] = seq.ids[:seq_len]
-
+            input_ids[i, :seq_len] = torch.LongTensor(
+                seq.ids[:seq_len],
+            )
             attention_mask[i, :seq_len] = 1
 
         return {"input_ids": input_ids, "attention_mask": attention_mask}
 
-    def preprocess_image(self, images: Union[Image, List[Image]]) -> np.ndarray:
+
+class ImageProcessor:
+    def __init__(self, config_path: PathLike):
+        """
+        :param config: model config
+        """
+
+        config = read_config(config_path)
+        if "image_encoder" in config:
+            config = config["image_encoder"]
+
+        self._image_size = config["image_size"]
+        self._normalization_means = config["normalization_means"]
+        self._normalization_deviations = config["normalization_deviations"]
+
+        assert isinstance(self._image_size, int) and self._image_size > 0
+        assert isinstance(self._normalization_means, list) and isinstance(self._normalization_deviations, list)
+        assert len(self._normalization_means) == len(self._normalization_deviations) == 3
+
+        self._image_transform = Compose(
+            [
+                Resize(self._image_size, interpolation=InterpolationMode.BICUBIC),
+                convert_to_rgb,
+                CenterCrop(self._image_size),
+                ToTensor(),
+                Normalize(
+                    mean=tuple(self._normalization_means),
+                    std=tuple(self._normalization_deviations),
+                ),
+            ],
+        )
+
+    def __call__(self, images: Union[Image, Sequence[Image]]) -> Dict[str, Tensor]:
         """Transforms one or more Pillow images into Torch Tensors.
 
         :param images: image or list of images to preprocess
+        :return: dictionary with float-represented images in tensors as values
         """
 
-        if isinstance(images, list):
-            batch_images = np.empty(
+        if isinstance(images, Sequence):
+            batch_images = torch.empty(
                 (len(images), 3, self._image_size, self._image_size),
-                dtype=np.float32,
+                dtype=torch.float32,
             )
 
             for i, image in enumerate(images):
-                batch_images[i] = self._resize_crop_normalize(image)
+                batch_images[i] = self._image_transform(image)
 
         else:
-            batch_images = self._resize_crop_normalize(images)[None]
-
-        return batch_images
-
-    def _resize_crop_normalize(self, image: Image):
-        width, height = image.size
-
-        if width < height:
-            width = self._image_size
-            height = int(height / width * self._image_size)
-        else:
-            width = int(width / height * self._image_size)
-            height = self._image_size
-
-        image = image.resize((width, height), resample=BICUBIC)
-
-        left = (width - self._image_size) / 2
-        top = (height - self._image_size) / 2
-        right = (width + self._image_size) / 2
-        bottom = (height + self._image_size) / 2
-
-        image = image.convert("RGB").crop((left, top, right, bottom))
-        # At this point `image` is a PIL Image with RGB channels.
-        # If you convert it to `np.ndarray` it will have shape (H, W, C) where C is the number of channels.
-        image = (np.array(image).astype(np.float32) / 255.0 - self.image_mean) / self.image_std
+            batch_images = self._image_transform(images).unsqueeze(0)
 
-        # To make it compatible with PyTorch, we need to transpose the image to (C, H, W).
-        return np.transpose(image, (2, 0, 1))
+        return {"images": batch_images}
```

### Comparing `uform-2.1.1/python/uform/torch_models.py` & `uform-3.0.1/python/uform/torch_encoders.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,27 @@
+from __future__ import annotations
+
 from dataclasses import dataclass
 from os import PathLike
-from typing import Dict, Optional, Tuple, Union
+from typing import Dict, Optional, Union, Mapping, Any, Tuple
 
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 from torch import Tensor
+from PIL.Image import Image
+
+from uform.shared import read_config
+
+
+def _is_on_gpu(model: nn.Module) -> bool:
+    try:
+        return next(model.parameters()).device.type == "cuda"
+    except StopIteration:
+        return False
 
 
 @dataclass(eq=False)
 class Attention(nn.Module):
     dim: int
     num_heads: int
     dropout_prob: float = 0
@@ -128,15 +140,15 @@
                 x + self.dropout(self.crossattn(x, context=context)),
             )
 
         return self.norm_mlp(x + self.dropout(self.mlp(x)))
 
 
 @dataclass(eq=False)
-class VisualEncoderBlock(nn.Module):
+class ImageEncoderBlock(nn.Module):
     dim: int
     num_heads: int
 
     def __post_init__(self):
         super().__init__()
         self.norm1 = nn.LayerNorm(self.dim, eps=1e-6)
         self.attn = Attention(self.dim, self.num_heads)
@@ -215,44 +227,22 @@
 
         for block in self.blocks:
             if not block.cross_attention:
                 x = block(x, attn_mask)
 
         return x
 
-    def forward_multimodal(
-        self,
-        x: Tensor,
-        attn_mask: Tensor,
-        context: Tensor,
-    ) -> Tensor:
-        context = self.context_projection(context)
-        expanded_attn_mask = self.get_attention_mask(attn_mask, x.dtype)
-        for block in self.blocks:
-            if block.cross_attention:
-                x = block(x, expanded_attn_mask, context)
-
-        return self.pool_features(x, attn_mask)
-
     def forward_embedding(self, x: Tensor, attn_mask: Tensor) -> Tensor:
         return self.embedding_projection(self.pool_features(x, attn_mask))
 
-    def forward_matching(self, x: Tensor) -> Tensor:
-        logits = self.matching_head(x)
-        if self.head_one_neuron:
-            return torch.sigmoid(logits)[:, 0]
-
-        return F.softmax(logits, dim=1)[:, 1]
-
     def pool_features(self, x: Tensor, attn_mask: Tensor) -> Tensor:
         if self.pooling == "cls":
             return x[:, 0]
 
         attn_mask = attn_mask.unsqueeze(2).type_as(x)
-
         return (x * attn_mask).sum(dim=1) / attn_mask.sum(dim=1)
 
     def get_attention_mask(self, attn_mask: Tensor, dtype: torch.dtype) -> Tensor:
         attn_mask = attn_mask.to(dtype)
         attn_mask = (1.0 - attn_mask) * torch.finfo(dtype).min
         return attn_mask.unsqueeze(1).expand(-1, attn_mask.shape[1], -1).unsqueeze(1)
 
@@ -269,34 +259,79 @@
         return self.dropout(self.layer_norm(x))
 
     def forward(
         self,
         x: Union[Tensor, dict],
         attention_mask: Optional[Tensor] = None,
         return_features: Optional[bool] = None,
-    ) -> Tensor:
+    ) -> Union[Tensor, Tuple[Tensor, Tensor]]:
+
         if isinstance(x, dict):
             assert attention_mask is None, "If `x` is a dictionary, then `attention_mask` should be None"
             attention_mask = x["attention_mask"]
             x = x["input_ids"]
         elif attention_mask is None:
             # If no attention mask is provided - create one with all ones
             attention_mask = torch.ones_like(x)
 
+        # If the model is on the GPU and the input matrices are not, shift them there
+        if _is_on_gpu(self) and not x.is_cuda:
+            x = x.cuda()
+            attention_mask = attention_mask.cuda()
+
         features = self.forward_features(x, attention_mask)
         embeddings = self.forward_embedding(features, attention_mask)
 
         return_features = return_features if return_features is not None else self.return_features
         if return_features:
             return features, embeddings
         return embeddings
 
+    def encode(
+        self,
+        x: Union[Tensor, dict],
+        attention_mask: Optional[Tensor] = None,
+        return_features: Optional[bool] = None,
+    ) -> Union[Tensor, Tuple[Tensor, Tensor]]:
+
+        result = self.forward(x, attention_mask, return_features)
+        if isinstance(result, tuple):
+            return result[0].detach(), result[1].detach()
+        else:
+            return result.detach()
+
+    @staticmethod
+    def from_pretrained(config: Union[PathLike, str, object], model: Union[PathLike, str]) -> TextEncoder:
+        """Load the image encoder from the given configuration and model path.
+
+        :param config: the configuration dictionary or path to the JSON configuration file
+        :param model: the model state dictionary or path to the `.pt` model file
+        """
+        config = read_config(config)
+        if "text_encoder" in config:
+            config = config["text_encoder"]
+
+        # We must strip all the non-member attributes before initializing the classes.
+        text_fields = TextEncoder.__dataclass_fields__
+        config = {k: v for k, v in config.items() if k in text_fields}
+        encoder = TextEncoder(**config)
+
+        # Load from disk
+        if isinstance(model, (PathLike, str)):
+            state = torch.load(model)
+        else:
+            state = model
+        if "text_encoder" in state:
+            state = state["text_encoder"]
+        encoder.load_state_dict(state)
+        return encoder
+
 
 @dataclass(eq=False)
-class VisualEncoder(nn.Module):
+class ImageEncoder(nn.Module):
     dim: int
     patch_size: int
     image_size: int
     num_layers: int
     num_heads: int
     embedding_dim: int
     pooling: str
@@ -310,196 +345,84 @@
         self.pos_embed = nn.Parameter(torch.randn(1, seq_len, self.dim) * 0.02)
         self.cls_token = nn.Parameter(torch.zeros(1, 1, self.dim))
 
         if self.num_reg_tokens > 0:
             self.reg_token = nn.Parameter(torch.zeros(1, self.num_reg_tokens, self.dim))
 
         self.blocks = nn.Sequential(
-            *[VisualEncoderBlock(self.dim, self.num_heads) for _ in range(self.num_layers)],
+            *[ImageEncoderBlock(self.dim, self.num_heads) for _ in range(self.num_layers)],
         )
 
         self.norm = nn.LayerNorm(self.dim, eps=1e-6)
         self.embedding_projection = nn.Linear(self.dim, self.embedding_dim, bias=False)
         self.return_features = False
 
-    def forward_features(self, x: Tensor) -> Tensor:
+    def forward_features(self, x: Union[Tensor, dict]) -> Tensor:
         x = self.patch_embed(x).flatten(start_dim=2).transpose(2, 1)
         x = x + self.pos_embed
-
         special_tokens = [self.cls_token.expand(x.shape[0], -1, -1)]
 
         if self.num_reg_tokens > 0:
             special_tokens.append(self.reg_token.expand(x.shape[0], -1, -1))
 
         x = torch.cat(special_tokens + [x], dim=1)
-
         x = self.blocks(x)
-
         return self.norm(x)
 
     def forward_embedding(self, x: Tensor) -> Tensor:
         if self.pooling == "cls":
             x = x[:, 0]
         else:
             x = x.mean(dim=1)
 
         return self.embedding_projection(x)
 
-    def forward(self, x: Tensor, return_features: Optional[bool] = None) -> Tensor:
+    def forward(self, x: Union[Tensor, dict], return_features: Optional[bool] = None) -> Tensor:
+        if isinstance(x, dict):
+            x = x["images"]
+
+        # If the model is on the GPU and the input matrices are not, shift them there
+        if _is_on_gpu(self) and not x.is_cuda:
+            x = x.cuda()
+
         features = self.forward_features(x)
         embeddings = self.forward_embedding(features)
         return_features = return_features if return_features is not None else self.return_features
         if return_features:
             return features, embeddings
         return embeddings
 
+    def encode(self, x: Union[Tensor, dict], return_features: Optional[bool] = None) -> Tensor:
+        result = self.forward(x, return_features)
+        if isinstance(result, tuple):
+            return result[0].detach(), result[1].detach()
+        else:
+            return result.detach()
 
-class VLM(nn.Module):
-    """
-    Vision-Language Model for Multimodal embeddings.
-    """
-
-    def __init__(self, config: Dict, tokenizer_path: PathLike):
-        """
-        :param config: Model config
-        """
-
-        super().__init__()
-        self._embedding_dim = config["text_encoder"]["embedding_dim"]
-
-        self.text_encoder = TextEncoder(**config["text_encoder"])
-        self.image_encoder = VisualEncoder(**config["image_encoder"])
-
-    def encode_image(
-        self,
-        images: Tensor,
-        return_features: bool = False,
-    ) -> Union[Tensor, Tuple[Tensor, Tensor]]:
-        """Passes the pre-processed images through `image_encoder` to produce images features (optional) and embeddings.
-
-        :param images: Preprocessed image
-        :param return_features: Whether to return images features or return only embeddings
-        """
-
-        features = self.image_encoder.forward_features(images)
-        embeddings = self.image_encoder.forward_embedding(features)
-
-        if return_features:
-            return features, embeddings
-
-        return embeddings
-
-    def encode_text(
-        self,
-        texts: Dict[str, Tensor],
-        return_features: bool = False,
-    ) -> Union[Tensor, Tuple[Tensor, Tensor]]:
-        """Passes the pre-processed texts through `text_encoder` to produce texts features (optional) and embeddings.
-
-        :param texts: Dictionary with tokenized texts and attention masks
-        :param return_features: Whether to return texts features or return only embeddings
-        """
-
-        features = self.text_encoder.forward_features(
-            texts["input_ids"],
-            texts["attention_mask"],
-        )
-        embeddings = self.text_encoder.forward_embedding(
-            features,
-            texts["attention_mask"],
-        )
-
-        if return_features:
-            return features, embeddings
-
-        return embeddings
-
-    def encode_multimodal(
-        self,
-        image: Optional[Tensor] = None,
-        text: Optional[Dict] = None,
-        image_features: Optional[Tensor] = None,
-        text_features: Optional[Tensor] = None,
-        attention_mask: Optional[Tensor] = None,
-        return_scores: bool = False,
-    ) -> Union[Tensor, Tuple[Tensor, Tensor]]:
-        """Passes preprocessed texts (or precomputed texts features) and
-            preprocessed images (or precomputed images features) through multimodal encoded to produce multimodal joint embeddings.
-
-        :param image: Preprocessed images
-        :param text: Preprocessed texts
-        :param image_features: Precomputed images features
-        :param text_features: Precomputed text features
-        :param attention_mask: Attention masks, not required if pass `text` instead of text_features
-        """
-
-        assert image is not None or image_features is not None, "Either `image` or `image_features` should be non None"
-        assert text is not None or text_features is not None, "Either `text_data` or `text_features` should be non None"
-
-        if text_features is not None:
-            assert attention_mask is not None, "if `text_features` is not None, then you should pass `attention_mask`"
-
-        if image_features is None:
-            image_features = self.image_encoder.forward_features(image)
-
-        if text_features is None:
-            text_features = self.text_encoder.forward_features(
-                text["input_ids"],
-                text["attention_mask"],
-            )
-
-        embeddings = self.text_encoder.forward_multimodal(
-            text_features,
-            attention_mask if attention_mask is not None else text["attention_mask"],
-            image_features,
-        )
-
-        if return_scores:
-            return self.get_matching_scores(embeddings), embeddings
-
-        return embeddings
-
-    def get_matching_scores(self, embeddings: Tensor) -> Tensor:
-        """Computes the probability that there is a match between images and texts based on their multimodal embeddings
-
-        :param embeddings: multimodal joint embeddings
-        """
-
-        return self.text_encoder.forward_matching(embeddings)
+    @staticmethod
+    def from_pretrained(
+        config: Union[PathLike, str, object],
+        model: Union[PathLike, str, Mapping[str, Any]],
+    ) -> ImageEncoder:
+        """Load the image encoder from the given configuration and model path.
 
-    def forward(
-        self,
-        images: Tensor,
-        texts: Dict[str, Tensor],
-    ) -> Union[Tensor, Tensor]:
-        """Inference forward method
-
-        :param images: Preprocessed images
-        :param texts: Preprocessed texts
-        :return: embeddings for images and texts
+        :param config: the configuration dictionary or path to the JSON configuration file
+        :param model: the model state dictionary or path to the `.pt` model file
         """
-        _, image_embeddings = self.image_encoder(images)
-        _, text_embeddings = self.text_encoder(texts)
-        return image_embeddings, text_embeddings
-
-    @property
-    def text_features_dim(self) -> int:
-        """Dimensionality of the text encoder features."""
-
-        return self.text_encoder.dim
-
-    @property
-    def image_features_dim(self) -> int:
-        """Dimensionality of the image encoder features."""
-
-        return self.image_encoder.dim
-
-    @property
-    def embedding_dim(self) -> int:
-        """Dimensionality of shared space embedding."""
-
-        return self._embedding_dim
-
-    @property
-    def multimodal_embedding_dim(self) -> int:
-        """Dimensionality of multimodal joint embedding."""
-        return self.text_encoder.dim
+        config = read_config(config)
+        if "image_encoder" in config:
+            config = config["image_encoder"]
+
+        # We must strip all the non-member attributes before initializing the classes.
+        image_fields = ImageEncoder.__dataclass_fields__
+        config = {k: v for k, v in config.items() if k in image_fields}
+        encoder = ImageEncoder(**config)
+
+        # Load from disk
+        if isinstance(model, (PathLike, str)):
+            state = torch.load(model)
+        else:
+            state = model
+        if "image_encoder" in state:
+            state = state["image_encoder"]
+        encoder.load_state_dict(state)
+        return encoder
```


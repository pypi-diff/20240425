# Comparing `tmp/ai2-olmo-0.2.5.tar.gz` & `tmp/ai2_olmo-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai2-olmo-0.2.5.tar", last modified: Thu Mar  7 00:27:29 2024, max compression
+gzip compressed data, was "ai2_olmo-0.3.0.tar", last modified: Thu Apr 25 19:22:32 2024, max compression
```

## Comparing `ai2-olmo-0.2.5.tar` & `ai2_olmo-0.3.0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 00:27:29.537897 ai2-olmo-0.2.5/
--rw-r--r--   0 runner    (1001) docker     (127)    11359 2024-03-07 00:26:55.000000 ai2-olmo-0.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    25352 2024-03-07 00:27:29.537897 ai2-olmo-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10798 2024-03-07 00:26:55.000000 ai2-olmo-0.2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 00:27:29.533897 ai2-olmo-0.2.5/ai2_olmo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    25352 2024-03-07 00:27:29.000000 ai2-olmo-0.2.5/ai2_olmo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-03-07 00:27:29.000000 ai2-olmo-0.2.5/ai2_olmo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-07 00:27:29.000000 ai2-olmo-0.2.5/ai2_olmo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-03-07 00:27:29.000000 ai2-olmo-0.2.5/ai2_olmo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-07 00:27:29.000000 ai2-olmo-0.2.5/ai2_olmo.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 00:27:29.529897 ai2-olmo-0.2.5/hf_olmo/
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-03-07 00:26:55.000000 ai2-olmo-0.2.5/hf_olmo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-03-07 00:26:55.000000 ai2-olmo-0.2.5/hf_olmo/configuration_olmo.py
--rw-r--r--   0 runner    (1001) docker     (127)     4184 2024-03-07 00:26:55.000000 ai2-olmo-0.2.5/hf_olmo/convert_olmo_to_hf.py
--rw-r--r--   0 runner    (1001) docker     (127)     5484 2024-03-07 00:26:55.000000 ai2-olmo-0.2.5/hf_olmo/modeling_olmo.py
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-03-07 00:26:55.000000 ai2-olmo-0.2.5/hf_olmo/tokenization_olmo_fast.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 00:27:29.533897 ai2-olmo-0.2.5/olmo/
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-03-07 00:26:55.000000 ai2-olmo-0.2.5/olmo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-03-07 00:26:55.000000 ai2-olmo-0.2.5/olmo/aliases.py
--rw-r--r--   0 runner    (1001) docker     (127)    46609 2024-03-07 00:26:55.000000 ai2-olmo-0.2.5/olmo/beam_search.py
--rw-r--r--   0 runner    (1001) docker     (127)    66628 2024-03-07 00:26:55.000000 ai2-olmo-0.2.5/olmo/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)    30112 2024-03-07 00:26:55.000000 ai2-olmo-0.2.5/olmo/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 00:27:29.533897 ai2-olmo-0.2.5/olmo/data/
--rw-r--r--   0 runner    (1001) docker     (127)     4730 2024-03-07 00:26:55.000000 ai2-olmo-0.2.5/olmo/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4265 2024-03-07 00:26:55.000000 ai2-olmo-0.2.5/olmo/data/collator.py
--rw-r--r--   0 runner    (1001) docker     (127)     8356 2024-03-07 00:26:55.000000 ai2-olmo-0.2.5/olmo/data/iterable_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     9049 2024-03-07 00:26:55.000000 ai2-olmo-0.2.5/olmo/data/memmap_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 00:27:29.533897 ai2-olmo-0.2.5/olmo/eval/
--rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-03-07 00:26:55.000000 ai2-olmo-0.2.5/olmo/eval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    42878 2024-03-07 00:26:55.000000 ai2-olmo-0.2.5/olmo/eval/downstream.py
--rw-r--r--   0 runner    (1001) docker     (127)     3363 2024-03-07 00:26:55.000000 ai2-olmo-0.2.5/olmo/eval/evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-03-07 00:26:55.000000 ai2-olmo-0.2.5/olmo/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3501 2024-03-07 00:26:55.000000 ai2-olmo-0.2.5/olmo/initialization.py
--rw-r--r--   0 runner    (1001) docker     (127)    73338 2024-03-07 00:26:55.000000 ai2-olmo-0.2.5/olmo/model.py
--rw-r--r--   0 runner    (1001) docker     (127)    34137 2024-03-07 00:26:55.000000 ai2-olmo-0.2.5/olmo/optim.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 00:26:55.000000 ai2-olmo-0.2.5/olmo/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     2448 2024-03-07 00:26:55.000000 ai2-olmo-0.2.5/olmo/safetensors_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     6828 2024-03-07 00:26:55.000000 ai2-olmo-0.2.5/olmo/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4027 2024-03-07 00:26:55.000000 ai2-olmo-0.2.5/olmo/torch_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    47596 2024-03-07 00:26:55.000000 ai2-olmo-0.2.5/olmo/train.py
--rw-r--r--   0 runner    (1001) docker     (127)    22994 2024-03-07 00:26:55.000000 ai2-olmo-0.2.5/olmo/util.py
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-03-07 00:26:55.000000 ai2-olmo-0.2.5/olmo/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-03-07 00:26:55.000000 ai2-olmo-0.2.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-07 00:27:29.537897 ai2-olmo-0.2.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:22:32.609150 ai2_olmo-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11359 2024-04-25 19:22:02.000000 ai2_olmo-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    26373 2024-04-25 19:22:32.609150 ai2_olmo-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11819 2024-04-25 19:22:02.000000 ai2_olmo-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:22:32.605150 ai2_olmo-0.3.0/ai2_olmo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    26373 2024-04-25 19:22:32.000000 ai2_olmo-0.3.0/ai2_olmo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-25 19:22:32.000000 ai2_olmo-0.3.0/ai2_olmo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 19:22:32.000000 ai2_olmo-0.3.0/ai2_olmo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-25 19:22:32.000000 ai2_olmo-0.3.0/ai2_olmo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-25 19:22:32.000000 ai2_olmo-0.3.0/ai2_olmo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:22:32.601150 ai2_olmo-0.3.0/hf_olmo/
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-25 19:22:02.000000 ai2_olmo-0.3.0/hf_olmo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-04-25 19:22:02.000000 ai2_olmo-0.3.0/hf_olmo/configuration_olmo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4530 2024-04-25 19:22:02.000000 ai2_olmo-0.3.0/hf_olmo/convert_olmo_to_hf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9669 2024-04-25 19:22:02.000000 ai2_olmo-0.3.0/hf_olmo/modeling_olmo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-25 19:22:02.000000 ai2_olmo-0.3.0/hf_olmo/tokenization_olmo_fast.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:22:32.605150 ai2_olmo-0.3.0/olmo/
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-25 19:22:02.000000 ai2_olmo-0.3.0/olmo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-25 19:22:02.000000 ai2_olmo-0.3.0/olmo/aliases.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46609 2024-04-25 19:22:02.000000 ai2_olmo-0.3.0/olmo/beam_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)    75141 2024-04-25 19:22:02.000000 ai2_olmo-0.3.0/olmo/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32209 2024-04-25 19:22:02.000000 ai2_olmo-0.3.0/olmo/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:22:32.605150 ai2_olmo-0.3.0/olmo/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     4882 2024-04-25 19:22:02.000000 ai2_olmo-0.3.0/olmo/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4265 2024-04-25 19:22:02.000000 ai2_olmo-0.3.0/olmo/data/collator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8356 2024-04-25 19:22:02.000000 ai2_olmo-0.3.0/olmo/data/iterable_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9049 2024-04-25 19:22:02.000000 ai2_olmo-0.3.0/olmo/data/memmap_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:22:32.605150 ai2_olmo-0.3.0/olmo/eval/
+-rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-04-25 19:22:02.000000 ai2_olmo-0.3.0/olmo/eval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47606 2024-04-25 19:22:02.000000 ai2_olmo-0.3.0/olmo/eval/downstream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3363 2024-04-25 19:22:02.000000 ai2_olmo-0.3.0/olmo/eval/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-25 19:22:02.000000 ai2_olmo-0.3.0/olmo/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3501 2024-04-25 19:22:02.000000 ai2_olmo-0.3.0/olmo/initialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    67982 2024-04-25 19:22:02.000000 ai2_olmo-0.3.0/olmo/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35220 2024-04-25 19:22:02.000000 ai2_olmo-0.3.0/olmo/optim.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 19:22:02.000000 ai2_olmo-0.3.0/olmo/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     2448 2024-04-25 19:22:02.000000 ai2_olmo-0.3.0/olmo/safetensors_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7128 2024-04-25 19:22:02.000000 ai2_olmo-0.3.0/olmo/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4138 2024-04-25 19:22:02.000000 ai2_olmo-0.3.0/olmo/torch_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52446 2024-04-25 19:22:02.000000 ai2_olmo-0.3.0/olmo/train.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24451 2024-04-25 19:22:02.000000 ai2_olmo-0.3.0/olmo/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-25 19:22:02.000000 ai2_olmo-0.3.0/olmo/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-04-25 19:22:02.000000 ai2_olmo-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 19:22:32.609150 ai2_olmo-0.3.0/setup.cfg
```

### Comparing `ai2-olmo-0.2.5/LICENSE` & `ai2_olmo-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ai2-olmo-0.2.5/PKG-INFO` & `ai2_olmo-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ai2-olmo
-Version: 0.2.5
+Version: 0.3.0
 Summary: Open Language Model (OLMo)
 Author-email: Allen Institute for Artificial Intelligence <olmo@allenai.org>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 https://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -280,25 +280,34 @@
 
 Otherwise you can install the model code by itself directly from PyPI with:
 
 ```bash
 pip install ai2-olmo
 ```
 
-## Models overview
+## Models
+
+### Overview
 
 The core models in the OLMo family released so far are (all trained on the [Dolma dataset](https://huggingface.co/datasets/allenai/dolma)): 
 | Model | Training Tokens | Context Length | Training Config | W&B Logs | Data Order File(s) ☨ |
 |-------|-----------------|:--------------:|-----------------|----------|--------------------|
 | [OLMo 1B](https://huggingface.co/allenai/OLMo-1B) | 3 Trillion | 2048 | [configs/official/OLMo-1B.yaml](https://github.com/allenai/OLMo/blob/main/configs/official/OLMo-1B.yaml) | [wandb.ai/…/OLMo-1B](https://wandb.ai/ai2-llm/OLMo-1B/reports/OLMo-1B--Vmlldzo2NzY1Njk1) | [epoch 1](https://olmo-checkpoints.org/ai2-llm/olmo-small/46zc5fly/train_data/global_indices.npy) |
 | [OLMo 7B](https://huggingface.co/allenai/OLMo-7B) | 2.5 Trillion | 2048 | [configs/official/OLMo-7B.yaml](https://github.com/allenai/OLMo/blob/main/configs/official/OLMo-7B.yaml) | [wandb.ai/…/OLMo-7B](https://wandb.ai/ai2-llm/OLMo-7B/reports/OLMo-7B--Vmlldzo2NzQyMzk5) | [epoch 1](https://olmo-checkpoints.org/ai2-llm/olmo-medium/wvc30anm/train_data/global_indices.npy), [epoch 2](https://olmo-checkpoints.org/ai2-llm/olmo-medium/wd2gxrza/train_data/global_indices.npy) |
 | [OLMo 7B Twin 2T](https://huggingface.co/allenai/OLMo-7B-Twin-2T) | 2 Trillion  | 2048 | [configs/official/OLMo-7B.yaml](https://github.com/allenai/OLMo/blob/main/configs/official/OLMo-7B.yaml) | [wandb.ai/…/OLMo-7B-Twin-2T](https://wandb.ai/ai2-llm/OLMo-7B/reports/OLMo-7B-Twin-2T--Vmlldzo2NzU0NTIz) | [epoch 1](https://olmo-checkpoints.org/ai2-llm/olmo-medium/wvc30anm/train_data/global_indices.npy) |
 
 > ☨ *See [Inspecting training data](#inspecting-training-data) below for usage.*
 
+### Checkpoints
+
+URLs to checkpoints at intermediate steps of the models' trainings can be found in the csv files under [`checkpoints/official/`](https://github.com/allenai/OLMo/blob/main/checkpoints/official). These 'directory' URLs cannot currently be directly accessed, but files within the directory are publicly accessible. These URLs can also be provided to the training script to resume training from the checkpoint (see [Training](#training)). Each checkpoint directory consists of:
+
+- `config.yaml`: the config at that training step.
+- `model.pt`, `optim.pt`, `train.pt`: model, optimizer and training state at that training step.
+
 ## Inference
 
 You can utilize our Hugging Face integration to run inference on the olmo checkpoints:
 
 ```python
 from hf_olmo import * # registers the Auto* classes
 
@@ -359,14 +368,21 @@
 
 ```bash
 torchrun --nproc_per_node=8 scripts/train.py configs/official/OLMo-1B.yaml
 ```
 
 You can use the same method to launch multi-node jobs as well. See [the documentation](https://pytorch.org/docs/stable/elastic/run.html) for `torchrun` to understand the additional arguments you'll need to configure the rendezvous backend / endpoint.
 
+To resume training from a checkpoint, you can pass its path (local or URL)
+to `scripts/train.py` with the `--load_path` arguments. For example, to resume training from step 1000 of the OLMo 1B run:
+
+```bash
+torchrun --nproc_per_node=8 scripts/train.py configs/official/OLMo-1B.yaml --load_path https://olmo-checkpoints.org/ai2-llm/olmo-small/w1r5xfzt/step1000-unsharded
+```
+
 ### Inspecting training data
 
 You may be interesting in inspecting the exact tokens that composed a particular batch during the training of one of the OLMo models.
 We provide tools to do this, but first you'll need to download the data as above (unless you have an R2 API key) and update the corresponding config accordingly.
 
 Then take note of the URL of the data order file you want, which can be found in the [Models Overview](#models-overview) table. For example, the data order file for the first epoch of the OLMo-7B model is [https://olmo-checkpoints.org/ai2-llm/olmo-medium/wvc30anm/train_data/global_indices.npy](https://olmo-checkpoints.org/ai2-llm/olmo-small/46zc5fly/train_data/global_indices.npy).
```

### Comparing `ai2-olmo-0.2.5/README.md` & `ai2_olmo-0.3.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -34,25 +34,34 @@
 
 Otherwise you can install the model code by itself directly from PyPI with:
 
 ```bash
 pip install ai2-olmo
 ```
 
-## Models overview
+## Models
+
+### Overview
 
 The core models in the OLMo family released so far are (all trained on the [Dolma dataset](https://huggingface.co/datasets/allenai/dolma)): 
 | Model | Training Tokens | Context Length | Training Config | W&B Logs | Data Order File(s) ☨ |
 |-------|-----------------|:--------------:|-----------------|----------|--------------------|
 | [OLMo 1B](https://huggingface.co/allenai/OLMo-1B) | 3 Trillion | 2048 | [configs/official/OLMo-1B.yaml](https://github.com/allenai/OLMo/blob/main/configs/official/OLMo-1B.yaml) | [wandb.ai/…/OLMo-1B](https://wandb.ai/ai2-llm/OLMo-1B/reports/OLMo-1B--Vmlldzo2NzY1Njk1) | [epoch 1](https://olmo-checkpoints.org/ai2-llm/olmo-small/46zc5fly/train_data/global_indices.npy) |
 | [OLMo 7B](https://huggingface.co/allenai/OLMo-7B) | 2.5 Trillion | 2048 | [configs/official/OLMo-7B.yaml](https://github.com/allenai/OLMo/blob/main/configs/official/OLMo-7B.yaml) | [wandb.ai/…/OLMo-7B](https://wandb.ai/ai2-llm/OLMo-7B/reports/OLMo-7B--Vmlldzo2NzQyMzk5) | [epoch 1](https://olmo-checkpoints.org/ai2-llm/olmo-medium/wvc30anm/train_data/global_indices.npy), [epoch 2](https://olmo-checkpoints.org/ai2-llm/olmo-medium/wd2gxrza/train_data/global_indices.npy) |
 | [OLMo 7B Twin 2T](https://huggingface.co/allenai/OLMo-7B-Twin-2T) | 2 Trillion  | 2048 | [configs/official/OLMo-7B.yaml](https://github.com/allenai/OLMo/blob/main/configs/official/OLMo-7B.yaml) | [wandb.ai/…/OLMo-7B-Twin-2T](https://wandb.ai/ai2-llm/OLMo-7B/reports/OLMo-7B-Twin-2T--Vmlldzo2NzU0NTIz) | [epoch 1](https://olmo-checkpoints.org/ai2-llm/olmo-medium/wvc30anm/train_data/global_indices.npy) |
 
 > ☨ *See [Inspecting training data](#inspecting-training-data) below for usage.*
 
+### Checkpoints
+
+URLs to checkpoints at intermediate steps of the models' trainings can be found in the csv files under [`checkpoints/official/`](https://github.com/allenai/OLMo/blob/main/checkpoints/official). These 'directory' URLs cannot currently be directly accessed, but files within the directory are publicly accessible. These URLs can also be provided to the training script to resume training from the checkpoint (see [Training](#training)). Each checkpoint directory consists of:
+
+- `config.yaml`: the config at that training step.
+- `model.pt`, `optim.pt`, `train.pt`: model, optimizer and training state at that training step.
+
 ## Inference
 
 You can utilize our Hugging Face integration to run inference on the olmo checkpoints:
 
 ```python
 from hf_olmo import * # registers the Auto* classes
 
@@ -113,14 +122,21 @@
 
 ```bash
 torchrun --nproc_per_node=8 scripts/train.py configs/official/OLMo-1B.yaml
 ```
 
 You can use the same method to launch multi-node jobs as well. See [the documentation](https://pytorch.org/docs/stable/elastic/run.html) for `torchrun` to understand the additional arguments you'll need to configure the rendezvous backend / endpoint.
 
+To resume training from a checkpoint, you can pass its path (local or URL)
+to `scripts/train.py` with the `--load_path` arguments. For example, to resume training from step 1000 of the OLMo 1B run:
+
+```bash
+torchrun --nproc_per_node=8 scripts/train.py configs/official/OLMo-1B.yaml --load_path https://olmo-checkpoints.org/ai2-llm/olmo-small/w1r5xfzt/step1000-unsharded
+```
+
 ### Inspecting training data
 
 You may be interesting in inspecting the exact tokens that composed a particular batch during the training of one of the OLMo models.
 We provide tools to do this, but first you'll need to download the data as above (unless you have an R2 API key) and update the corresponding config accordingly.
 
 Then take note of the URL of the data order file you want, which can be found in the [Models Overview](#models-overview) table. For example, the data order file for the first epoch of the OLMo-7B model is [https://olmo-checkpoints.org/ai2-llm/olmo-medium/wvc30anm/train_data/global_indices.npy](https://olmo-checkpoints.org/ai2-llm/olmo-small/46zc5fly/train_data/global_indices.npy).
```

#### html2text {}

```diff
@@ -5,15 +5,15 @@
 OLMo is a repository for training and using AI2's state-of-the-art open
 language models. It is built by scientists, for scientists. ## Installation
 First install [PyTorch](https://pytorch.org) according to the instructions
 specific to your operating system. To install from source (recommended for
 training/fine-tuning) run: ```bash git clone https://github.com/allenai/
 OLMo.git cd OLMo pip install -e .[all] ``` Otherwise you can install the model
 code by itself directly from PyPI with: ```bash pip install ai2-olmo ``` ##
-Models overview The core models in the OLMo family released so far are (all
+Models ### Overview The core models in the OLMo family released so far are (all
 trained on the [Dolma dataset](https://huggingface.co/datasets/allenai/dolma)):
 | Model | Training Tokens | Context Length | Training Config | W&B Logs | Data
 Order File(s) â¨ | |-------|-----------------|:--------------:|---------------
 --|----------|--------------------| | [OLMo 1B](https://huggingface.co/allenai/
 OLMo-1B) | 3 Trillion | 2048 | [configs/official/OLMo-1B.yaml](https://
 github.com/allenai/OLMo/blob/main/configs/official/OLMo-1B.yaml) | [wandb.ai/
 â¦/OLMo-1B](https://wandb.ai/ai2-llm/OLMo-1B/reports/OLMo-1B--
@@ -27,22 +27,31 @@
 checkpoints.org/ai2-llm/olmo-medium/wd2gxrza/train_data/global_indices.npy) | |
 [OLMo 7B Twin 2T](https://huggingface.co/allenai/OLMo-7B-Twin-2T) | 2 Trillion
 | 2048 | [configs/official/OLMo-7B.yaml](https://github.com/allenai/OLMo/blob/
 main/configs/official/OLMo-7B.yaml) | [wandb.ai/â¦/OLMo-7B-Twin-2T](https://
 wandb.ai/ai2-llm/OLMo-7B/reports/OLMo-7B-Twin-2T--Vmlldzo2NzU0NTIz) | [epoch 1]
 (https://olmo-checkpoints.org/ai2-llm/olmo-medium/wvc30anm/train_data/
 global_indices.npy) | > â¨ *See [Inspecting training data](#inspecting-
-training-data) below for usage.* ## Inference You can utilize our Hugging Face
-integration to run inference on the olmo checkpoints: ```python from hf_olmo
-import * # registers the Auto* classes from transformers import
-AutoModelForCausalLM, AutoTokenizer olmo = AutoModelForCausalLM.from_pretrained
-("allenai/OLMo-7B") tokenizer = AutoTokenizer.from_pretrained("allenai/OLMo-
-7B") message = ["Language modeling is "] inputs = tokenizer(message,
-return_tensors='pt', return_token_type_ids=False) response = olmo.generate
-(**inputs, max_new_tokens=100, do_sample=True, top_k=50, top_p=0.95) print
+training-data) below for usage.* ### Checkpoints URLs to checkpoints at
+intermediate steps of the models' trainings can be found in the csv files under
+[`checkpoints/official/`](https://github.com/allenai/OLMo/blob/main/
+checkpoints/official). These 'directory' URLs cannot currently be directly
+accessed, but files within the directory are publicly accessible. These URLs
+can also be provided to the training script to resume training from the
+checkpoint (see [Training](#training)). Each checkpoint directory consists of:
+- `config.yaml`: the config at that training step. - `model.pt`, `optim.pt`,
+`train.pt`: model, optimizer and training state at that training step. ##
+Inference You can utilize our Hugging Face integration to run inference on the
+olmo checkpoints: ```python from hf_olmo import * # registers the Auto* classes
+from transformers import AutoModelForCausalLM, AutoTokenizer olmo =
+AutoModelForCausalLM.from_pretrained("allenai/OLMo-7B") tokenizer =
+AutoTokenizer.from_pretrained("allenai/OLMo-7B") message = ["Language modeling
+is "] inputs = tokenizer(message, return_tensors='pt',
+return_token_type_ids=False) response = olmo.generate(**inputs,
+max_new_tokens=100, do_sample=True, top_k=50, top_p=0.95) print
 (tokenizer.batch_decode(response, skip_special_tokens=True)[0]) ```
 Alternatively, with the Hugging Face pipeline abstraction: ```python from
 transformers import pipeline olmo_pipe = pipeline("text-generation",
 model="allenai/OLMo-7B") print(olmo_pipe("Language modeling is")) ``` ###
 Inference on finetuned checkpoints If you finetune the model using the code
 above, you can use the conversion script to convert a native OLMo checkpoint to
 a Hugging Face-compatible checkpoint ```bash python hf_olmo/
@@ -66,41 +75,46 @@
 v1_5/gpt-neox-20b-pii-special/part-000-00000.npy` Once you've updated the data
 paths in the config you can launch a training run via `torchrun`. For example,
 to launch the 1B model training on a single 8x GPU node, you would run: ```bash
 torchrun --nproc_per_node=8 scripts/train.py configs/official/OLMo-1B.yaml ```
 You can use the same method to launch multi-node jobs as well. See [the
 documentation](https://pytorch.org/docs/stable/elastic/run.html) for `torchrun`
 to understand the additional arguments you'll need to configure the rendezvous
-backend / endpoint. ### Inspecting training data You may be interesting in
-inspecting the exact tokens that composed a particular batch during the
-training of one of the OLMo models. We provide tools to do this, but first
-you'll need to download the data as above (unless you have an R2 API key) and
-update the corresponding config accordingly. Then take note of the URL of the
-data order file you want, which can be found in the [Models Overview](#models-
-overview) table. For example, the data order file for the first epoch of the
-OLMo-7B model is [https://olmo-checkpoints.org/ai2-llm/olmo-medium/wvc30anm/
-train_data/global_indices.npy](https://olmo-checkpoints.org/ai2-llm/olmo-small/
-46zc5fly/train_data/global_indices.npy). Once you have that you can use this
-snippet to inspect the data within a particular batch: ```python import numpy
-as np from cached_path import cached_path from olmo.config import TrainConfig
-from olmo.data import build_memmap_dataset # Update these paths to what you
-want: data_order_file_path = cached_path("https://olmo-checkpoints.org/ai2-llm/
-olmo-medium/wvc30anm/train_data/global_indices.npy") train_config_path =
-"configs/official/OLMo-7B.yaml" cfg = TrainConfig.load(train_config_path)
-dataset = build_memmap_dataset(cfg, cfg.data) batch_size =
-cfg.global_train_batch_size global_indices = np.memmap(data_order_file_path,
-mode="r+", dtype=np.uint32) def get_batch_instances(batch_idx: int) -> list
-[list[int]]: batch_start = batch_idx * batch_size batch_end = (batch_idx + 1) *
-batch_size batch_indices = global_indices[batch_start:batch_end]
-batch_instances = [] for index in batch_indices: token_ids = dataset[index]
-["input_ids"].tolist() batch_instances.append(token_ids) return batch_instances
-# Get all 2048 x 2048 token IDs in the first batch. get_batch_instances(0) ```
-## Fine-tuning To fine-tune an OLMo model using our trainer you'll first need
-to prepare your dataset by tokenizing it and saving the tokens IDs to a flat
-numpy memory-mapped array. See [`scripts/prepare_tulu_data.py`](./scripts/
+backend / endpoint. To resume training from a checkpoint, you can pass its path
+(local or URL) to `scripts/train.py` with the `--load_path` arguments. For
+example, to resume training from step 1000 of the OLMo 1B run: ```bash torchrun
+--nproc_per_node=8 scripts/train.py configs/official/OLMo-1B.yaml --load_path
+https://olmo-checkpoints.org/ai2-llm/olmo-small/w1r5xfzt/step1000-unsharded ```
+### Inspecting training data You may be interesting in inspecting the exact
+tokens that composed a particular batch during the training of one of the OLMo
+models. We provide tools to do this, but first you'll need to download the data
+as above (unless you have an R2 API key) and update the corresponding config
+accordingly. Then take note of the URL of the data order file you want, which
+can be found in the [Models Overview](#models-overview) table. For example, the
+data order file for the first epoch of the OLMo-7B model is [https://olmo-
+checkpoints.org/ai2-llm/olmo-medium/wvc30anm/train_data/global_indices.npy]
+(https://olmo-checkpoints.org/ai2-llm/olmo-small/46zc5fly/train_data/
+global_indices.npy). Once you have that you can use this snippet to inspect the
+data within a particular batch: ```python import numpy as np from cached_path
+import cached_path from olmo.config import TrainConfig from olmo.data import
+build_memmap_dataset # Update these paths to what you want:
+data_order_file_path = cached_path("https://olmo-checkpoints.org/ai2-llm/olmo-
+medium/wvc30anm/train_data/global_indices.npy") train_config_path = "configs/
+official/OLMo-7B.yaml" cfg = TrainConfig.load(train_config_path) dataset =
+build_memmap_dataset(cfg, cfg.data) batch_size = cfg.global_train_batch_size
+global_indices = np.memmap(data_order_file_path, mode="r+", dtype=np.uint32)
+def get_batch_instances(batch_idx: int) -> list[list[int]]: batch_start =
+batch_idx * batch_size batch_end = (batch_idx + 1) * batch_size batch_indices =
+global_indices[batch_start:batch_end] batch_instances = [] for index in
+batch_indices: token_ids = dataset[index]["input_ids"].tolist()
+batch_instances.append(token_ids) return batch_instances # Get all 2048 x 2048
+token IDs in the first batch. get_batch_instances(0) ``` ## Fine-tuning To
+fine-tune an OLMo model using our trainer you'll first need to prepare your
+dataset by tokenizing it and saving the tokens IDs to a flat numpy memory-
+mapped array. See [`scripts/prepare_tulu_data.py`](./scripts/
 prepare_tulu_data.py) for an example with the Tulu V2 dataset, which can be
 easily modified for other datasets. Next, prepare your training config. There
 are many examples in the [`configs/`](https://github.com/allenai/OLMo/blob/
 main/configs) directory that you can use as a starting point. The most
 important thing is to make sure the model parameters (the `model` field in the
 config) match up with the checkpoint you're starting from. To be safe you can
 always start from the config that comes with the model checkpoint. At a minimum
```

### Comparing `ai2-olmo-0.2.5/ai2_olmo.egg-info/PKG-INFO` & `ai2_olmo-0.3.0/ai2_olmo.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ai2-olmo
-Version: 0.2.5
+Version: 0.3.0
 Summary: Open Language Model (OLMo)
 Author-email: Allen Institute for Artificial Intelligence <olmo@allenai.org>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 https://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -280,25 +280,34 @@
 
 Otherwise you can install the model code by itself directly from PyPI with:
 
 ```bash
 pip install ai2-olmo
 ```
 
-## Models overview
+## Models
+
+### Overview
 
 The core models in the OLMo family released so far are (all trained on the [Dolma dataset](https://huggingface.co/datasets/allenai/dolma)): 
 | Model | Training Tokens | Context Length | Training Config | W&B Logs | Data Order File(s) ☨ |
 |-------|-----------------|:--------------:|-----------------|----------|--------------------|
 | [OLMo 1B](https://huggingface.co/allenai/OLMo-1B) | 3 Trillion | 2048 | [configs/official/OLMo-1B.yaml](https://github.com/allenai/OLMo/blob/main/configs/official/OLMo-1B.yaml) | [wandb.ai/…/OLMo-1B](https://wandb.ai/ai2-llm/OLMo-1B/reports/OLMo-1B--Vmlldzo2NzY1Njk1) | [epoch 1](https://olmo-checkpoints.org/ai2-llm/olmo-small/46zc5fly/train_data/global_indices.npy) |
 | [OLMo 7B](https://huggingface.co/allenai/OLMo-7B) | 2.5 Trillion | 2048 | [configs/official/OLMo-7B.yaml](https://github.com/allenai/OLMo/blob/main/configs/official/OLMo-7B.yaml) | [wandb.ai/…/OLMo-7B](https://wandb.ai/ai2-llm/OLMo-7B/reports/OLMo-7B--Vmlldzo2NzQyMzk5) | [epoch 1](https://olmo-checkpoints.org/ai2-llm/olmo-medium/wvc30anm/train_data/global_indices.npy), [epoch 2](https://olmo-checkpoints.org/ai2-llm/olmo-medium/wd2gxrza/train_data/global_indices.npy) |
 | [OLMo 7B Twin 2T](https://huggingface.co/allenai/OLMo-7B-Twin-2T) | 2 Trillion  | 2048 | [configs/official/OLMo-7B.yaml](https://github.com/allenai/OLMo/blob/main/configs/official/OLMo-7B.yaml) | [wandb.ai/…/OLMo-7B-Twin-2T](https://wandb.ai/ai2-llm/OLMo-7B/reports/OLMo-7B-Twin-2T--Vmlldzo2NzU0NTIz) | [epoch 1](https://olmo-checkpoints.org/ai2-llm/olmo-medium/wvc30anm/train_data/global_indices.npy) |
 
 > ☨ *See [Inspecting training data](#inspecting-training-data) below for usage.*
 
+### Checkpoints
+
+URLs to checkpoints at intermediate steps of the models' trainings can be found in the csv files under [`checkpoints/official/`](https://github.com/allenai/OLMo/blob/main/checkpoints/official). These 'directory' URLs cannot currently be directly accessed, but files within the directory are publicly accessible. These URLs can also be provided to the training script to resume training from the checkpoint (see [Training](#training)). Each checkpoint directory consists of:
+
+- `config.yaml`: the config at that training step.
+- `model.pt`, `optim.pt`, `train.pt`: model, optimizer and training state at that training step.
+
 ## Inference
 
 You can utilize our Hugging Face integration to run inference on the olmo checkpoints:
 
 ```python
 from hf_olmo import * # registers the Auto* classes
 
@@ -359,14 +368,21 @@
 
 ```bash
 torchrun --nproc_per_node=8 scripts/train.py configs/official/OLMo-1B.yaml
 ```
 
 You can use the same method to launch multi-node jobs as well. See [the documentation](https://pytorch.org/docs/stable/elastic/run.html) for `torchrun` to understand the additional arguments you'll need to configure the rendezvous backend / endpoint.
 
+To resume training from a checkpoint, you can pass its path (local or URL)
+to `scripts/train.py` with the `--load_path` arguments. For example, to resume training from step 1000 of the OLMo 1B run:
+
+```bash
+torchrun --nproc_per_node=8 scripts/train.py configs/official/OLMo-1B.yaml --load_path https://olmo-checkpoints.org/ai2-llm/olmo-small/w1r5xfzt/step1000-unsharded
+```
+
 ### Inspecting training data
 
 You may be interesting in inspecting the exact tokens that composed a particular batch during the training of one of the OLMo models.
 We provide tools to do this, but first you'll need to download the data as above (unless you have an R2 API key) and update the corresponding config accordingly.
 
 Then take note of the URL of the data order file you want, which can be found in the [Models Overview](#models-overview) table. For example, the data order file for the first epoch of the OLMo-7B model is [https://olmo-checkpoints.org/ai2-llm/olmo-medium/wvc30anm/train_data/global_indices.npy](https://olmo-checkpoints.org/ai2-llm/olmo-small/46zc5fly/train_data/global_indices.npy).
```

### Comparing `ai2-olmo-0.2.5/ai2_olmo.egg-info/SOURCES.txt` & `ai2_olmo-0.3.0/ai2_olmo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ai2-olmo-0.2.5/hf_olmo/configuration_olmo.py` & `ai2_olmo-0.3.0/hf_olmo/configuration_olmo.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 """
 OLMo configuration
 """
 
+import transformers
+from packaging import version
 from transformers import AutoConfig, PretrainedConfig
 from transformers.utils import logging
 
 from olmo.config import ModelConfig
 
 logger = logging.get_logger(__name__)
 
@@ -16,18 +18,15 @@
 
     def __init__(self, use_cache: bool = False, **kwargs):
         model_config = ModelConfig()
         all_kwargs = model_config.asdict()
         all_kwargs.update(kwargs)
         all_kwargs.update({"use_cache": use_cache})
         all_kwargs.update(
-            {
-                "architectures": all_kwargs.get("architectures", ["OlmoModelForCausalLM"])
-                or ["OlmoModelForCausalLM"]
-            }
+            {"architectures": all_kwargs.get("architectures", ["OLMoForCausalLM"]) or ["OLMoForCausalLM"]}
         )
         super().__init__(**all_kwargs)
 
     @property
     def num_attention_heads(self):
         return self.n_heads
 
@@ -36,9 +35,11 @@
         return self.n_layers
 
     @property
     def hidden_size(self):
         return self.d_model
 
 
-# Register the config class so that it is available for transformer pipelines, auto-loading etc.
-AutoConfig.register("olmo", OLMoConfig)
+if version.parse(transformers.__version__) < version.parse("4.40.0"):
+    # Register the config class so that it is available for transformer pipelines, auto-loading etc.
+    # OLMo is integrated directly in transformers from v4.40.0 onwards
+    AutoConfig.register("olmo", OLMoConfig)
```

### Comparing `ai2-olmo-0.2.5/hf_olmo/convert_olmo_to_hf.py` & `ai2_olmo-0.3.0/hf_olmo/convert_olmo_to_hf.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import argparse
 import logging
 import os
 import shutil
 
 import torch
+from omegaconf import OmegaConf as om
 
 from hf_olmo.configuration_olmo import OLMoConfig
 from hf_olmo.modeling_olmo import OLMoForCausalLM
 from hf_olmo.tokenization_olmo_fast import OLMoTokenizerFast
 from olmo import ModelConfig, Tokenizer
 
 logger = logging.getLogger(__name__)
@@ -87,14 +88,22 @@
         else:
             logger.info(f"File already present at {final_location}")
 
     convert_checkpoint(local_model_path)
     return local_model_path
 
 
+def fix_bad_tokenizer(checkpoint_dir: str):
+    path = os.path.join(checkpoint_dir, "config.yaml")
+    conf = om.load(path)
+    conf["tokenizer"]["identifier"] = "allenai/gpt-neox-olmo-dolma-v1_5"
+    conf["model"]["eos_token_id"] = 50279
+    om.save(conf, path)
+
+
 def main():
     parser = argparse.ArgumentParser(
         description="Adds a config.json to the checkpoint directory, and creates pytorch_model.bin, "
         "making it easier to load weights as HF models."
     )
     parser.add_argument(
         "--checkpoint-dir",
@@ -105,12 +114,13 @@
         "--ignore-olmo-compatibility",
         action="store_true",
         help="Ignore compatibility with the olmo codebase. "
         "This will remove files that are needed specifically for olmo codebase, eg. config.yaml, etc.",
     )
 
     args = parser.parse_args()
+    fix_bad_tokenizer(args.checkpoint_dir)
     convert_checkpoint(args.checkpoint_dir, args.ignore_olmo_compatibility)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `ai2-olmo-0.2.5/hf_olmo/tokenization_olmo_fast.py` & `ai2_olmo-0.3.0/hf_olmo/tokenization_olmo_fast.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from transformers import AutoTokenizer, PreTrainedTokenizerFast
 
 from hf_olmo.configuration_olmo import OLMoConfig
 
 
 class OLMoTokenizerFast(PreTrainedTokenizerFast):
-    # Note: Olmo's tokenizer is already a wrapper around huggingface. This is potentially unnecessary.
+    # Note: OLMo's tokenizer is already a wrapper around huggingface. This is potentially unnecessary.
     pass
 
     # def save_vocabulary(self, save_directory: str, filename_prefix: Optional[str] = None) -> Tuple[str]:
     #     # This is required to make the implementation complete.
     #     pass
```

### Comparing `ai2-olmo-0.2.5/olmo/beam_search.py` & `ai2_olmo-0.3.0/olmo/beam_search.py`

 * *Files identical despite different names*

### Comparing `ai2-olmo-0.2.5/olmo/checkpoint.py` & `ai2_olmo-0.3.0/olmo/checkpoint.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 import gc
 import io
 import logging
 import pickle
 import shutil
+import traceback
 from abc import ABCMeta, abstractmethod
 from collections import defaultdict
-from concurrent.futures import ThreadPoolExecutor, as_completed
+from concurrent.futures import ProcessPoolExecutor, ThreadPoolExecutor, as_completed
 from contextlib import contextmanager
 from copy import deepcopy
 from dataclasses import dataclass, field, replace
 from functools import reduce
+from multiprocessing import shared_memory
 from pathlib import Path
 from typing import Any, Dict, Generator, List, Optional, Set, Tuple, cast
 
 import numpy as np
 import torch
 import torch.distributed.checkpoint as dist_cp
-from numpy import ndarray
+import torch.multiprocessing as mp
 from packaging import version
 from torch.distributed import _remote_device
 from torch.distributed._shard._utils import narrow_tensor_by_index
 from torch.distributed._shard.metadata import ShardMetadata
 from torch.distributed._shard.sharded_tensor import ShardedTensor
 from torch.distributed.checkpoint.filesystem import WriteResult, _StorageInfo
 from torch.distributed.checkpoint.metadata import Metadata, MetadataIndex
@@ -37,20 +39,30 @@
 from torch.futures import Future
 
 try:
     from torch.distributed.fsdp.flat_param import FlatParamHandle  # type: ignore
 except ModuleNotFoundError:
     from torch.distributed.fsdp._flat_param import FlatParamHandle  # type: ignore
 
+from olmo import util
+
 from .aliases import PathOrStr
 from .config import BaseConfig, ShardedCheckpointerType, TrainConfig
+from .exceptions import OLMoCheckpointError
 from .optim import Optimizer, fix_optim_state_dict
 from .safetensors_util import safetensors_file_to_state_dict
-from .torch_util import barrier, get_fs_local_rank, get_global_rank, get_world_size
+from .torch_util import (
+    barrier,
+    gc_cuda,
+    get_fs_local_rank,
+    get_global_rank,
+    get_world_size,
+)
 from .util import (
+    _get_s3_client,
     default_thread_count,
     dir_is_empty,
     get_bytes_range,
     get_progress_bar,
     resource_path,
     upload,
     wait_for,
@@ -181,15 +193,15 @@
             optimizer_key="optim",
             storage_reader=RemoteFileSystemReader(
                 f"{load_path}/{MODEL_AND_OPTIM_FOLDER}",
                 local_cache=None if local_cache is None else local_cache / MODEL_AND_OPTIM_FOLDER,
             ),
         )
         del model_state
-        torch.cuda.empty_cache()
+        gc_cuda()
         load_fsdp_optim_state(fsdp_model, optim, optim_state["optim"])
 
 
 def load_fsdp_optim_state(fsdp_model: FSDP, optim: Optimizer, optim_state: Dict[str, Any]):
     log.info("Flattening sharded optimizer state...")
     # NOTE: Careful! The order of the these arguments has changed from 2.0 to 2.1... ¯\_(ツ)_/¯
     if version.parse(torch.__version__) < version.parse("2.1.0"):
@@ -202,15 +214,15 @@
     # Put optim state on CPU since `Optimizer.load_state_dict()` will create a deepcopy of the whole state dict,
     # which takes up unnecessary GPU memory.
     for state in flattened_osd["state"].values():
         for k in state.keys():
             v = state[k]
             if isinstance(v, torch.Tensor):
                 state[k] = v.to(device="cpu")
-    torch.cuda.empty_cache()
+    gc_cuda()
     optim.load_state_dict(fix_optim_state_dict(optim, flattened_osd))
 
 
 def save_state_dict(
     checkpoint_dir: PathOrStr,
     fname: str,
     state_dict: Dict[str, Any],
@@ -266,21 +278,25 @@
     :param checkpoint_dir: A local or remote checkpoint directory.
     :param fname: The target file within the ``checkpoint_dir``. This should be a path relative to the ``checkpoint_dir``.
     :param local_cache: A local cache of the checkpoint directory. Use this when the ``checkpoint_dir`` is a
         remote "directory" but there might be a cached version of the same artifacts.
 
     :raises FileNotFoundError: If ``fname`` doesn't exist in the ``checkpoint_dir`` or the local cache.
     """
-    path = resource_path(str(checkpoint_dir).rstrip("/"), fname, local_cache=local_cache)
-
-    if path.suffix == ".pt":
-        safetensors_path = path.with_suffix(".safetensors")
-        if safetensors_path.is_file():
-            return safetensors_file_to_state_dict(safetensors_path, map_location=map_location)
+    if fname.endswith(".pt"):
+        # Try safetensors version first.
+        try:
+            path = resource_path(
+                str(checkpoint_dir).rstrip("/"), fname[:-2] + "safetensors", local_cache=local_cache
+            )
+            return safetensors_file_to_state_dict(path, map_location=map_location)
+        except FileNotFoundError:
+            pass
 
+    path = resource_path(str(checkpoint_dir).rstrip("/"), fname, local_cache=local_cache)
     return torch.load(path, map_location=map_location)
 
 
 def load_model_state(checkpoint_dir: PathOrStr, model: torch.nn.Module):
     """
     Load model state from a distributed FSDP model checkpoint created from :func:`save_fsdp_model_and_optim_state()`.
     Note that ``model`` should not be wrapped with FSDP.
@@ -312,15 +328,18 @@
     ) -> None:
         if thread_count is not None and thread_count <= 0:
             raise ValueError("thread count must be at least 1")
         super().__init__(
             path,
             single_file_per_rank=single_file_per_rank,
             sync_files=sync_files,
-            thread_count=thread_count or default_thread_count(),
+            # NOTE: we default to 1 thread here instead of whatever `default_thread_count()`
+            # returns because uploading big checkpoint files with multiple threads causes
+            # boto3 to fail in weird ways.
+            thread_count=thread_count or 1,
             per_thread_copy_ahead=per_thread_copy_ahead,
         )
         self.upload_to = None if upload_to is None else upload_to.rstrip("/")
         self.save_overwrite = save_overwrite
 
     def write_data(
         self,
@@ -329,23 +348,35 @@
     ) -> Future[List[WriteResult]]:
         fut = super().write_data(plan, planner)
         if self.upload_to is not None:
             files_to_upload = set()
             for write_result in fut.wait():
                 files_to_upload.add(write_result.storage_data.relative_path)
 
+            # Create the global S3 client up front to work around a threading issue in boto.
+            if self.upload_to.startswith("s3://"):
+                _get_s3_client("s3")
+            elif self.upload_to.startswith("r2://"):
+                _get_s3_client("r2")
+
             with ThreadPoolExecutor(max_workers=self.thread_count) as executor:
                 futures = []
                 for fname in files_to_upload:
                     source = self.path / fname
                     target = f"{self.upload_to}/{fname}"
                     log.info(f"Uploading {source} to {target}...")
                     futures.append(executor.submit(upload, source, target, save_overwrite=self.save_overwrite))
                 for f in as_completed(futures):
-                    f.result()
+                    try:
+                        f.result()
+                    except BaseException:
+                        # NOTE: we might get an error here that can't be pickled, which causes a different failure
+                        # later when PyTorch tries to reduce that error across ranks. So here we just make
+                        # sure we're raising a simple error type that can be pickled.
+                        raise OLMoCheckpointError(f"Original error:\n{traceback.format_exc()}")
         return fut
 
     def finish(self, metadata: Metadata, results: List[List[WriteResult]]) -> None:
         super().finish(metadata, results)
         if self.upload_to is not None:
             source = self.path / ".metadata"
             target = f"{self.upload_to}/.metadata"
@@ -379,21 +410,34 @@
 
     def _get_content_for_read(self, read_item: ReadItem) -> Tuple[ReadItem, bytes]:
         sinfo = self.storage_data[read_item.storage_index]
         content = self._get_bytes(sinfo.relative_path, sinfo.offset, sinfo.length)
         return (read_item, content)
 
     def read_data(self, plan: dist_cp.LoadPlan, planner: dist_cp.LoadPlanner) -> Future[None]:
+        # Create the global S3 client up front to work around a threading issue in boto.
+        if isinstance(self.path, str):
+            if self.path.startswith("s3://"):
+                _get_s3_client("s3")
+            elif self.path.startswith("r2://"):
+                _get_s3_client("r2")
+
         with ThreadPoolExecutor(max_workers=self.thread_count) as executor:
             read_item_content_futures = []
             for read_item in plan.items:
                 read_item_content_futures.append(executor.submit(self._get_content_for_read, read_item))
             read_item_content_results = []
             for f in as_completed(read_item_content_futures):
-                read_item_content_results.append(f.result())
+                try:
+                    read_item_content_results.append(f.result())
+                except BaseException:
+                    # NOTE: we might get an error here that can't be pickled, which causes a different failure
+                    # later when PyTorch tries to reduce that error across ranks. So here we just make
+                    # sure we're raising a simple error type that can be pickled.
+                    raise OLMoCheckpointError(f"Original error:\n{traceback.format_exc()}")
 
         # Modified from `FileSystemReader.read_data()`
         for read_item, content in read_item_content_results:
             bytes = io.BytesIO(content)
             bytes.seek(0)
             if read_item.type == LoadItemType.BYTE_IO:
                 planner.load_bytes(read_item, bytes)
@@ -909,14 +953,170 @@
         optim_state = full_state_dict.pop("optim")
         return (
             model_state,
             optim_state if load_optimizer_state else None,
             full_state_dict if load_trainer_state else None,
         )
 
+    def _copy_sharded_tensors_to_shared_mem(self, state: Dict, world_size: int, rank: int, key: Tuple):
+        key = tuple() if key is None else key
+        if isinstance(state, (list, tuple, set)):
+            for i, sub_state in enumerate(state):
+                self._copy_sharded_tensors_to_shared_mem(sub_state, world_size, rank, key + (i,))
+        elif isinstance(state, dict):
+            for name in state.keys():
+                self._copy_sharded_tensors_to_shared_mem(state[name], world_size, rank, key + (name,))
+        elif isinstance(state, ShardedTensor):
+            self._copy_sharded_tensor_to_shared_mem(state, world_size, rank, key)
+            return
+        else:
+            return
+
+    def _get_shard_placement_and_rank_sizes(
+        self, shards_metadata: List[ShardMetadata], world_size: int
+    ) -> Tuple[Dict[ShardMetadata, Tuple[int, int]], List[int]]:
+        def shard_size(shard_md):
+            return reduce((lambda x, y: x * y), shard_md.shard_sizes)  # type: ignore[attr-defined]
+
+        rank_sizes = [0 for _ in range(world_size)]
+        shard_placement: Dict[ShardMetadata, Tuple[int, int]] = {}
+        for shard_md in shards_metadata:
+            shard_rank = cast(_remote_device, shard_md.placement).rank()
+            assert shard_rank is not None
+            if shard_rank >= world_size:
+                raise RuntimeError(f"Shard rank {shard_rank} exceeds world size {world_size}")
+
+            shard_placement[shard_md] = (shard_rank, rank_sizes[shard_rank])
+            rank_sizes[shard_rank] += shard_size(shard_md)
+
+        return shard_placement, rank_sizes
+
+    def _copy_sharded_tensor_to_shared_mem(
+        self, sharded_tensor: ShardedTensor, world_size: int, rank: int, key: Tuple
+    ) -> Any:
+        shard0_md = sharded_tensor.metadata()
+        shard_placement, rank_sizes = self._get_shard_placement_and_rank_sizes(
+            shard0_md.shards_metadata, world_size
+        )
+
+        rank_size = rank_sizes[rank]
+        assert rank_size >= 0
+        if rank_size == 0:
+            return
+
+        assert shard0_md.tensor_properties.dtype == torch.float32, "Expected sharded tensor to be fp32"
+        numpy_type = np.float32
+
+        sharded_memory_name = "-".join(key + (str(rank),))
+
+        shm = shared_memory.SharedMemory(
+            create=True, size=rank_size * np.dtype(numpy_type).itemsize, name=sharded_memory_name
+        )
+        np_arr = np.ndarray((rank_size,), dtype=numpy_type, buffer=shm.buf)
+
+        for local_shard in sharded_tensor.local_shards():
+            shard_rank = cast(_remote_device, local_shard.metadata.placement).rank()
+            assert shard_rank == rank
+
+            src = local_shard.tensor.flatten()
+            shard_offset = shard_placement[local_shard.metadata][1]
+
+            np_arr[shard_offset : shard_offset + src.numel()] = src.numpy()
+
+        shm.close()
+
+    def _copy_sharded_data_to_shared_mem(self, world_size: int, shard_filepath: Path):
+        shard_number = int(shard_filepath.name[4:-3])
+        log.info("Starting unsharding shard number %d to shared memory", shard_number)
+
+        with self._patch_sharded_tensor_load():
+            shard = torch.load(shard_filepath, map_location="cpu")
+            log.debug("Done loading shard number %d", shard_number)
+
+        self._copy_sharded_tensors_to_shared_mem(
+            shard, world_size, shard_number, (str(shard_filepath.parent).replace("/", "_"),)
+        )
+        log.info("Done unsharding shard number %d to shared memory", shard_number)
+
+    def _unshard_using_sharded_mem(
+        self, state: Any, world_size: int, device: torch.device, shard_dir: PathOrStr
+    ) -> Any:
+        return self._unshard_state_using_shared_mem(state, world_size, device, (str(shard_dir).replace("/", "_"),))
+
+    def _unshard_state_using_shared_mem(
+        self, state: Any, world_size: int, device: torch.device, key: Tuple
+    ) -> Any:
+        if isinstance(state, (list, tuple, set)):
+            return state.__class__(
+                self._unshard_state_using_shared_mem(sub_state, world_size, device, key + (i,))
+                for i, sub_state in enumerate(state)
+            )
+        elif isinstance(state, dict):
+            return {
+                name: self._unshard_state_using_shared_mem(state[name], world_size, device, key + (name,))
+                for name in state.keys()
+            }
+        elif isinstance(state, ShardedTensor):
+            return self._unshard_tensor_using_shared_mem(state, world_size, device, key)
+        elif isinstance(state, torch.Tensor):
+            return state.to(device=device)
+        else:
+            return state
+
+    def _unshard_tensor_using_shared_mem(
+        self, sharded_tensor: ShardedTensor, world_size: int, device: torch.device, key: Tuple
+    ) -> torch.Tensor:
+        shard0_md = sharded_tensor.metadata()
+
+        def shard_size(shard_md):
+            return reduce((lambda x, y: x * y), shard_md.shard_sizes)  # type: ignore[attr-defined]
+
+        shard_placement, rank_sizes = self._get_shard_placement_and_rank_sizes(
+            shard0_md.shards_metadata, world_size
+        )
+
+        assert shard0_md.tensor_properties.dtype == torch.float32, "Expected sharded tensor to be fp32"
+        numpy_type = np.float32
+
+        out = torch.empty(
+            *sharded_tensor.metadata().size, dtype=sharded_tensor.metadata().tensor_properties.dtype, device=device
+        )
+        dims = len(sharded_tensor.metadata().size)
+        for shard_md, (rank, rank_offset) in shard_placement.items():
+            if rank >= world_size:
+                raise RuntimeError(f"Shard rank {rank} exceeds world size {world_size}")
+
+            sharded_memory_name = "-".join(key + (str(rank),))
+            shm = shared_memory.SharedMemory(name=sharded_memory_name)
+
+            rank_size = rank_sizes[rank]
+            assert rank_size >= 0
+            if rank_size == 0:
+                continue
+
+            np_arr = np.ndarray((rank_size,), dtype=numpy_type, buffer=shm.buf)
+
+            tensor = torch.from_numpy(np_arr)[rank_offset : rank_offset + shard_size(shard_md)]
+            tensor = tensor.view(shard_md.shard_sizes)
+
+            out_narrow_view = out
+            for dim in range(dims):
+                out_narrow_view = out_narrow_view.narrow(
+                    dim,
+                    shard_md.shard_offsets[dim],
+                    shard_md.shard_sizes[dim],
+                )
+
+            out_narrow_view.copy_(tensor)
+
+            shm.close()
+            shm.unlink()
+
+        return out
+
     @contextmanager
     def _patch_sharded_tensor_load(self):
         """
         Monkeypatch for torch's ShardedTensor, so we can unpickle without having torch.distributed set up.
         """
 
         def _rebuild_from_type_v2_monkey(func, new_type, args, state):
@@ -944,135 +1144,76 @@
         try:
             torch._tensor._rebuild_from_type_v2 = _rebuild_from_type_v2_monkey
             yield
         finally:
             torch._tensor._rebuild_from_type_v2 = original_rebuild_from_type_v2
 
     def _unshard(self, input_dir: PathOrStr, device: torch.device, skip_keys: Optional[Set[str]] = None):
+        """
+        The current unsharding implementation consists of:
+
+        1. Loading each shard on a separate process and copying their sharded tensors to shared memory.
+        2. Loading 1 shard on the main process as a base unsharded object.
+        3. Using the sharded tensors in shared memory to populate the base unsharded object.
+
+        This implementation replaced a prior implementation that instead loaded
+        all shards using threads, because that implementation turned out to
+        be extremely slow (e.g. 6+ hours) sometimes when the world size was 1024.
+        The current implementation is slower than the old one in many scenarios,
+        but is significantly faster in the above mentioned case (e.g. 30 minutes)
+        if there are enough CPUs.
+        """
+
         input_dir = Path(input_dir)
         skip_keys = skip_keys or set()
 
-        with self._patch_sharded_tensor_load():
-            # We load in threads because it's faster.
-            executor = ThreadPoolExecutor()
-            shards_dict = {}
-            for shard_name in input_dir.glob("rank*.pt"):
-                log.info("Loading %s ...", shard_name)
-                shard_number = int(shard_name.name[4:-3])  # shard names look like "rankXX.pt"
-                shards_dict[shard_number] = executor.submit(torch.load, shard_name, map_location="cpu")
-            shards = [None] * len(shards_dict)
-            for rank, shard_future in shards_dict.items():
-                shard = shard_future.result()
-                for key in skip_keys:
-                    if key in shard:
-                        del shard[key]
-                shards[rank] = shard
-            assert all(shard is not None for shard in shards)
-            executor.shutdown()
-            del shards_dict
-
-        log.info("Unsharding from %d shards ...", len(shards))
-
-        unsharded_state_dict = self._unshard_object(shards, device=device)
-        # At this point in time we need 2x memory :-(
-        del shards
-
-        return unsharded_state_dict
-
-    def _unshard_object(self, os: List[Any], device: torch.device) -> Any:
-        rank0_item = os[0]
-        assert all(type(o) is type(rank0_item) for o in os)
-        if isinstance(rank0_item, str):
-            assert all(o == rank0_item for o in os)
-            return rank0_item
-        elif isinstance(rank0_item, (list, tuple, set)):
-            assert all(len(o) == len(rank0_item) for o in os)
-            return rank0_item.__class__(self._unshard_object(o, device=device) for o in zip(*os))
-        elif isinstance(rank0_item, dict):
-            assert all(o.keys() == rank0_item.keys() for o in os)
-            return {key: self._unshard_object([o[key] for o in os], device=device) for key in rank0_item.keys()}
-        elif isinstance(rank0_item, ShardedTensor):
-            return self._gather(os, device=device)
-        else:
-            assert all(self._objects_are_equal(o, rank0_item) for o in os)
-            return rank0_item
-
-    def _gather(self, shards: List[ShardedTensor], device: torch.device) -> torch.Tensor:
-        world_size = len(shards)
-        shard0_md = shards[0].metadata()
-        # Make sure all shards agree on the metadata
-        assert all(shard.metadata() == shard0_md for shard in shards)
-        # Make sure the nth shard expects to be the nth shard.
-        assert all(
-            shard_md.placement.rank() == rank  # type: ignore
-            for rank, shard_md in enumerate(shard0_md.shards_metadata)
+        shard_filepaths = list(input_dir.glob("rank*.pt"))
+        world_size = len(shard_filepaths)
+        if world_size == 0:
+            raise RuntimeError("No shards found for unsharding")
+
+        log.info("Number of shards: %d", world_size)
+        shard_size_gb = shard_filepaths[0].stat().st_size / (1024 * 1024 * 1024)
+        min_ram_required_estimate_gb = shard_size_gb * world_size
+        log.info(
+            "Shards are %.2fGB each, at least %.2fGB RAM is required", shard_size_gb, min_ram_required_estimate_gb
         )
 
-        def shard_size(shard_md):
-            return reduce((lambda x, y: x * y), shard_md.shard_sizes)  # type: ignore[attr-defined]
-
-        rank_sizes = [0 for _ in range(world_size)]
-        max_rank_size = 0
-        shard_placement: Dict[ShardMetadata, Tuple[int, int]] = {}
-        for shard_md in shard0_md.shards_metadata:
-            shard_rank = cast(_remote_device, shard_md.placement).rank()
-            assert shard_rank is not None
-
-            shard_placement[shard_md] = (shard_rank, rank_sizes[shard_rank])
-            rank_sizes[shard_rank] += shard_size(shard_md)
-            max_rank_size = max(max_rank_size, rank_sizes[shard_rank])
+        log.info("Copying sharded tensors to shared memory using multiple processes")
+        # Copy sharded data to shared memory using multiple processes, so this process can load
+        # from memory rather than disk. We spawn a new process instead of forking since shared memory
+        # appears to get deleted when forked processes end for some reason.
+        executor = ProcessPoolExecutor(
+            mp_context=mp.get_context("spawn"), initializer=util.prepare_cli_environment
+        )
+        futures = []
+        for shard_filepath in shard_filepaths:
+            shard_rank = int(shard_filepath.name[4:-3])
+
+            if shard_rank >= world_size:
+                raise RuntimeError(
+                    f"Shard rank {shard_rank} of file {shard_filepath} exceeds world size {world_size}"
+                )
 
-        gather_list: List[torch.Tensor] = [torch.empty((max_rank_size,)) for _ in range(world_size)]
+            futures.append(executor.submit(self._copy_sharded_data_to_shared_mem, world_size, shard_filepath))
 
-        datas = []
-        with torch.no_grad():
-            for shard in shards:
-                data = torch.empty(max_rank_size)
-
-                for local_shard in shard.local_shards():
-                    src = local_shard.tensor.flatten()
-                    shard_offset = shard_placement[local_shard.metadata][1]
-                    data[shard_offset : shard_offset + src.numel()].copy_(src)
-
-                datas.append(data)
-
-        # torch.gather in a nutshell
-        for rank, data in enumerate(datas):
-            gather_list[rank].copy_(data)
-
-        full_size = shard0_md.size
-        out = torch.empty(*full_size, dtype=shard0_md.tensor_properties.dtype, device=device)
-        dims = len(full_size)
-        for shard_md in shard0_md.shards_metadata:
-            rank, rank_offset = shard_placement[shard_md]
-            tensor = gather_list[rank]
-            tensor = tensor[rank_offset : rank_offset + shard_size(shard_md)]
-            tensor = tensor.view(shard_md.shard_sizes)
+        for f in as_completed(futures):
+            f.result()
+        executor.shutdown()
 
-            out_narrow_view = out
-            for dim in range(dims):
-                out_narrow_view = out_narrow_view.narrow(
-                    dim,
-                    shard_md.shard_offsets[dim],
-                    shard_md.shard_sizes[dim],
-                )
+        log.info("Loading a shard on the main process to be unsharded state")
+        with self._patch_sharded_tensor_load():
+            state = torch.load(shard_filepaths[0], map_location="cpu")
 
-            out_narrow_view.copy_(tensor)
+        for key in skip_keys:
+            if key in state:
+                del state[key]
 
-        return out
-
-    def _objects_are_equal(self, a: Any, b: Any) -> bool:
-        if type(a) is not type(b):
-            return False
-        if isinstance(a, ndarray):
-            return np.array_equal(a, b)
-        elif isinstance(a, torch.Tensor):
-            return torch.equal(a, b)
-        else:
-            return a == b
+        log.info("Unsharding from %d shards ...", world_size)
+        return self._unshard_using_sharded_mem(state, world_size, device, input_dir)
 
 
 @dataclass
 class _LocalShardedCheckpointerMetadata(BaseConfig):
     world_size: int = field(default_factory=get_world_size)
 
 
@@ -1129,26 +1270,20 @@
         if torch.cuda.is_available():
             torch.cuda.synchronize()
         _lazy_init(fsdp_model, fsdp_model)
 
     def _fsdp_handles(self, fsdp_model: FSDP) -> List[FlatParamHandle]:
         if version.parse(torch.__version__) < version.parse("2.1.0"):
             return fsdp_model._handles  # type: ignore
-        elif version.parse(torch.__version__) < version.parse("2.2.0"):
+        elif version.parse(torch.__version__) < version.parse("2.3.0"):
             # Handle could be None if the FSDP wrapper doesn't manage any parameters.
             if hasattr(fsdp_model, "_handle") and fsdp_model._handle is not None:
                 return [fsdp_model._handle]  # type: ignore
             else:
                 return []
-        elif version.parse(torch.__version__) < version.parse("2.3.0"):
-            # Could be None if the FSDP wrapper doesn't manage any parameters.
-            if hasattr(fsdp_model, "_all_handles") and fsdp_model._all_handles is not None:
-                return fsdp_model._all_handles
-            else:
-                return []
         else:
             # Need to verify FSDP internals with newer versions.
             raise NotImplementedError
 
     @torch.no_grad()
     def _get_flat_param_state_to_save(self, fsdp_model: FSDP) -> Dict[str, Any]:
         self._prepare_fsdp_model(fsdp_model)
@@ -1241,20 +1376,22 @@
                 checkpoint_dir,
                 f"train/rank{get_global_rank()}.pt",
                 trainer_state,
                 upload_to=upload_to,
                 save_overwrite=self.cfg.save_overwrite,
             )
 
-            # Save config.
-            self._save_config(checkpoint_dir, upload_to=upload_to)
-
             # Save metadata.
             self._save_metadata(checkpoint_dir, upload_to=upload_to)
 
+            # Save config. We do this last b/c the presence of a config in a remote checkpoint
+            # "directory" indicates that the folder is valid, as a opposed to a partially
+            # uploaded checkpoint directory that failed before completing.
+            self._save_config(checkpoint_dir, upload_to=upload_to)
+
     def restore_checkpoint(
         self,
         load_path: PathOrStr,
         fsdp_model: FSDP,
         optim: Optimizer,
         *,
         local_cache: Optional[PathOrStr] = None,
@@ -1516,19 +1653,80 @@
             for future in as_completed(futures):
                 rank, path = future.result()
                 results[rank] = path
 
         return [results[rank] for rank in range(world_size)]
 
 
+class OlmoCoreCheckpointer(Checkpointer):
+    def save_checkpoint(
+        self,
+        dir: PathOrStr,
+        fsdp_model: FSDP,
+        optim: Optimizer,
+        trainer_state: Dict[str, Any],
+        *,
+        upload_to: Optional[str] = None,
+    ) -> None:
+        from olmo_core.distributed.checkpoint import (  # type: ignore
+            save_model_and_optim_state,
+        )
+
+        with self._temporary_wd(dir) as checkpoint_dir:
+            log.info("Saving model and optim state...")
+            save_model_and_optim_state(checkpoint_dir, fsdp_model, optim, save_overwrite=self.cfg.save_overwrite)
+            if upload_to is not None and get_fs_local_rank() == 0:
+                for path in Path(checkpoint_dir).glob("**/*"):
+                    if not path.is_file():
+                        continue
+                    upload_target = f"{upload_to.rstrip('/')}/{path.relative_to(checkpoint_dir)}"
+                    log.info(f"Uploading {path} to {upload_target}...")
+                    upload(path, upload_target, save_overwrite=self.cfg.save_overwrite)
+
+            log.info("Saving trainer state...")
+            save_state_dict(
+                checkpoint_dir,
+                f"train/rank{get_global_rank()}.pt",
+                trainer_state,
+                save_overwrite=self.cfg.save_overwrite,
+                upload_to=upload_to,
+            )
+
+            self._save_config(checkpoint_dir, upload_to=upload_to)
+
+    def restore_checkpoint(
+        self,
+        load_path: PathOrStr,
+        fsdp_model: FSDP,
+        optim: Optimizer,
+        *,
+        local_cache: Optional[PathOrStr] = None,
+        load_optimizer_state: bool = True,
+    ) -> Dict[str, Any]:
+        from olmo_core.distributed.checkpoint import (  # type: ignore
+            load_model_and_optim_state,
+        )
+
+        log.info("Loading model and optim state...")
+        load_model_and_optim_state(load_path, fsdp_model, optim if load_optimizer_state else None)
+
+        log.info("Loading trainer state...")
+        trainer_state = load_state_dict(load_path, f"train/rank{get_global_rank()}.pt", local_cache=local_cache)
+
+        barrier()
+        return trainer_state
+
+
 def build_sharded_checkpointer(
     cfg: TrainConfig, *, name: Optional[ShardedCheckpointerType] = None
 ) -> Checkpointer:
     name = name or cfg.sharded_checkpointer
     if name == ShardedCheckpointerType.torch_new:
         return TorchNewStyleShardedCheckpointer(cfg)
     elif name == ShardedCheckpointerType.torch_legacy:
         return TorchLegacyShardedCheckpointer(cfg)
     elif name == ShardedCheckpointerType.local:
         return LocalShardedCheckpointer(cfg)
+    elif name == ShardedCheckpointerType.olmo_core:
+        return OlmoCoreCheckpointer(cfg)
     else:
         raise NotImplementedError(name)
```

### Comparing `ai2-olmo-0.2.5/olmo/config.py` & `ai2_olmo-0.3.0/olmo/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,22 +19,21 @@
 import torch
 from omegaconf import DictConfig, ListConfig
 from omegaconf import OmegaConf as om
 from omegaconf.errors import OmegaConfBaseException
 from torch.distributed.fsdp import MixedPrecision, ShardingStrategy
 
 from .aliases import PathOrStr
-from .exceptions import OlmoConfigurationError
+from .exceptions import OLMoConfigurationError
 from .util import StrEnum
 
 __all__ = [
     "ActivationType",
     "ActivationCheckpointingStrategy",
     "BlockType",
-    "CompilerConfig",
     "LayerNormType",
     "InitFnType",
     "ModelConfig",
     "OptimizerType",
     "OptimizerConfig",
     "SchedulerType",
     "SchedulerConfig",
@@ -112,15 +111,15 @@
         cls._register_resolvers()
         conf = om.structured(cls)
         try:
             if kwargs:
                 conf = om.merge(conf, kwargs)
             return cast(C, om.to_object(conf))
         except OmegaConfBaseException as e:
-            raise OlmoConfigurationError(str(e))
+            raise OLMoConfigurationError(str(e))
 
     @classmethod
     def load(
         cls: Type[C],
         path: PathOrStr,
         overrides: Optional[List[str]] = None,
         key: Optional[str] = None,
@@ -135,15 +134,15 @@
                 raw = raw[key]  # type: ignore
             raw = cls.update_legacy_settings(raw)
             conf = om.merge(schema, raw)
             if overrides:
                 conf = om.merge(conf, om.from_dotlist(overrides))
             return cast(C, om.to_object(conf))
         except OmegaConfBaseException as e:
-            raise OlmoConfigurationError(str(e))
+            raise OLMoConfigurationError(str(e))
 
     def save(self, path: PathOrStr) -> None:
         """Save to a YAML file."""
         om.save(config=self, f=str(path))
 
     def asdict(self, exclude: Optional[Iterable[str]] = None) -> Dict[str, Any]:
         out = asdict(self)  # type: ignore
@@ -167,29 +166,23 @@
 
     rms = "rms"
     """
     An RMSNorm implementation. When using ``torch.compile`` this is
     probably the fastest implementation.
     """
 
-    amd_compatible = "amd_compatible"
-    """
-    LayerNorm implemented manually to work around an issue with ROCm.
-    """
-
 
 class ActivationType(StrEnum):
     gelu = "gelu"
     relu = "relu"
     swiglu = "swiglu"
 
 
 class BlockType(StrEnum):
     sequential = "sequential"
-    parallel = "parallel"
 
     llama = "llama"
     """
     A block similar to the sequential block with slightly different
     implementations of operations like attention to imitate the behavior of Llama.
     """
 
@@ -239,14 +232,22 @@
     """
 
     n_heads: int = 12
     """
     The number of self-attention heads.
     """
 
+    n_kv_heads: Optional[int] = None
+    """
+    The number of heads to use for keys and values. Defaults to `n_heads`.
+    Set this to ``None`` or ``n_heads`` for normal multi-head attention.
+    Set this to 1 for multi-query attention.
+    Set it to some in-between value for Llama2-style grouped query attention.
+    """
+
     clip_qkv: Optional[float] = None
     """
     Clip QKV to this value when set.
     """
 
     n_layers: int = 12
     """
@@ -308,18 +309,17 @@
     """
 
     attention_dropout: float = 0.1
     """
     The dropout probability within the attention modules.
     """
 
-    multi_query_attention: bool = False
+    multi_query_attention: Optional[bool] = None
     """
-    Use the Multi-Query formulation of attention used in PaLM. This reduces the number of parameters
-    and is more efficient during inference.
+    Deprecated. Use n_kv_heads instead.
     """
 
     attention_layer_norm: bool = False
     """
     Apply layer norm to the keys and queries within the attention mechanism.
     This can help stabilize training.
     """
@@ -429,14 +429,35 @@
 
     precision: Optional[str] = None
     """
     Precision used to train/evaluate with. You shouldn't set this directly.
     See :data:`TrainConfig.precision` instead.
     """
 
+    @property
+    def effective_n_kv_heads(self) -> int:
+        if self.n_kv_heads is None:
+            if self.multi_query_attention is True:
+                return 1
+            else:
+                return self.n_heads
+        else:
+            if self.multi_query_attention is None:
+                return self.n_kv_heads
+            if self.multi_query_attention:
+                n_kv_heads_should_be = 1
+            else:
+                n_kv_heads_should_be = self.n_heads
+            if self.n_kv_heads == n_kv_heads_should_be:
+                return n_kv_heads_should_be
+            else:
+                raise OLMoConfigurationError(
+                    "You can't set `multi_query_attention` and `n_kv_heads` at the same time."
+                )
+
 
 class OptimizerType(StrEnum):
     lionw = "lionw"
     adamw = "adamw"
 
 
 @dataclass
@@ -506,14 +527,20 @@
 
     grad_clip_warmup_factor: Optional[float] = None
     """
     The ratio of the max allowed gradient norm (or norm ratio) for clipping during the warmup period
     vs after the warmup period.
     """
 
+    warmup_min_lr: Optional[float] = None
+    """
+    The starting LR during the warmup period. If not set this defaults to 10% of
+    the target LR.
+    """
+
 
 class PaddingDirection(StrEnum):
     right = "right"
     left = "left"
 
 
 @dataclass
@@ -525,14 +552,15 @@
     generate_attention_mask: bool = False
     num_workers: int = 0
     drop_last: bool = False
     pin_memory: bool = False
     prefetch_factor: Optional[int] = None
     persistent_workers: bool = False
     timeout: int = 0
+    seed: Optional[int] = None
 
 
 class EvaluatorType(StrEnum):
     downstream = "downstream"
     lm = "lm"
 
 
@@ -655,25 +683,34 @@
     """
     The wrapping strategy to use. If ``None``, the default, the model is wrapped with a single top-level
     FSDP instance.
     """
 
     precision: FSDPPrecision = FSDPPrecision.pure
 
+    hybrid_sharding_num_model_replicas: Optional[int] = None
+    """
+    The number of model instances, when using a hybrid sharding strategy.
+    If not ``None``, this must divide the total number of nodes. If ``None``, the default,
+    a model instance is used per node (as determined by ``get_world_size() // get_local_world_size()``).
+    PyTorch's default HSDP behavior matches this default behavior.
+    """
+
 
 class CheckpointType(StrEnum):
     sharded = "sharded"
     unsharded = "unsharded"
     sharded_ephemeral = "sharded_ephemeral"
 
 
 class ShardedCheckpointerType(StrEnum):
     torch_new = "torch_new"
     torch_legacy = "torch_legacy"
     local = "local"
+    olmo_core = "olmo_core"
 
 
 class ActivationCheckpointingStrategy(StrEnum):
     whole_layer = "whole_layer"
     """
     Checkpoint every transformer layer.
     """
@@ -689,14 +726,24 @@
     """
 
     one_in_four = "one_in_four"
     """
     Checkpoint one in four transformer layers.
     """
 
+    two_in_three = "two_in_three"
+    """
+    Checkpoint two out of every three transformer layers.
+    """
+
+    three_in_four = "three_in_four"
+    """
+    Checkpoint three out of four of every transformer layers.
+    """
+
     fine_grained = "fine_grained"
     """
     Focus checkpointing on where it is cheap to recompute and saves most memory.
     """
 
 
 @dataclass
@@ -951,14 +998,20 @@
     """
 
     console_log_interval: int = 1
     """
     How often to log to the console.
     """
 
+    gen1_gc_interval: Optional[int] = 1
+    """
+    How often (in steps) to run generation 1 garbage collection.
+    Set to ``None`` to use automatic garbage collection (i.e. we don't mess with it).
+    """
+
     compile: Optional[CompilerConfig] = None
     """
     Settings for compiling the model with ``torch.compile()``.
     """
 
     fsdp: FSDPConfig = field(default_factory=FSDPConfig)
     """
@@ -1003,19 +1056,29 @@
     """
 
     stop_at: Optional[int] = None
     """
     Stop at a specific step.
     """
 
+    stop_after: Optional[int] = None
+    """
+    Stop after a specific number of steps.
+    """
+
     activation_checkpointing: Optional[ActivationCheckpointingStrategy] = None
     """
     The activation checkpointing strategy to use.
     """
 
+    fused_loss: Optional[bool] = None
+    """
+    Whether to use the fused CE loss function from `flash-attn`.
+    """
+
     @property
     def autocast_precision(self) -> torch.dtype:
         if self.precision == "amp_bf16":
             return torch.bfloat16
         elif self.precision == "amp_fp16":
             return torch.float16
         elif self.precision == "fp32":
```

### Comparing `ai2-olmo-0.2.5/olmo/data/__init__.py` & `ai2_olmo-0.3.0/olmo/data/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from pathlib import Path
 from typing import Any, Dict, List, Optional, cast
 
 from torch.utils.data import DataLoader, DistributedSampler
 
 from ..aliases import PathOrStr
 from ..config import DataConfig, TrainConfig
-from ..exceptions import OlmoConfigurationError
+from ..exceptions import OLMoConfigurationError
 from ..torch_util import barrier, get_global_rank, get_world_size
 from .collator import DataCollator
 from .iterable_dataset import IterableDataset
 from .memmap_dataset import MemMapDataset
 
 __all__ = ["MemMapDataset", "DataCollator", "IterableDataset", "build_eval_dataloader", "build_train_dataloader"]
 
@@ -17,26 +17,26 @@
 def build_memmap_dataset(
     train_config: TrainConfig, data_config: DataConfig, include_instance_metadata: bool = True
 ) -> MemMapDataset:
     paths: List[str]
     metadata: List[Dict[str, Any]] = []
     if data_config.paths:
         if data_config.datasets:
-            raise OlmoConfigurationError("DataConfig.paths is mutually exclusive with DataConfig.datasets")
+            raise OLMoConfigurationError("DataConfig.paths is mutually exclusive with DataConfig.datasets")
         paths = data_config.paths
         for path in paths:
             metadata.append({"path": str(path)})
     elif data_config.datasets:
         paths = []
         for label in sorted(data_config.datasets.keys()):
             label_paths = data_config.datasets[label]
             paths.extend(label_paths)
             metadata.extend([{"label": label}] * len(label_paths))
     else:
-        raise OlmoConfigurationError("One of DataConfig.paths or DataConfig.datasets is required")
+        raise OLMoConfigurationError("One of DataConfig.paths or DataConfig.datasets is required")
     return MemMapDataset(
         *paths,
         chunk_size=train_config.model.max_sequence_length,
         metadata=metadata,
         include_instance_metadata=include_instance_metadata,
         pad_token_id=train_config.model.pad_token_id,
         generate_attention_mask=data_config.generate_attention_mask,
@@ -53,21 +53,22 @@
     dataset = build_memmap_dataset(train_config, data_config, include_instance_metadata=True)
     collator = DataCollator(pad_direction=data_config.pad_direction, pad_token_id=train_config.model.pad_token_id)
     if data_config.drop_last:
         # Make sure batch size is small enough.
         samples_per_device = len(dataset) // get_world_size()
         batch_size = min(batch_size, samples_per_device)
         assert batch_size > 0, f"dataset for {data_config.paths} is too small"
+    seed = data_config.seed if data_config.seed is not None else train_config.seed
     sampler = DistributedSampler(
         dataset,
         drop_last=data_config.drop_last,
         shuffle=shuffle,
         num_replicas=get_world_size(),
         rank=get_global_rank(),
-        seed=train_config.seed,
+        seed=seed,
     )
     return DataLoader(
         dataset,
         batch_size=batch_size,
         collate_fn=collator,
         num_workers=data_config.num_workers,
         sampler=sampler,
@@ -83,25 +84,26 @@
     collator = DataCollator(
         pad_direction=train_config.data.pad_direction, pad_token_id=train_config.model.pad_token_id
     )
     dataset = build_memmap_dataset(train_config, train_config.data, include_instance_metadata=False)
     work_dir = Path(train_config.save_folder) / "train_data"
     if get_global_rank() == 0:
         if work_dir.is_dir() and not train_config.save_overwrite:
-            raise OlmoConfigurationError(
+            raise OLMoConfigurationError(
                 "train data working directory already exists, use --save_overwrite to overwrite"
             )
         else:
             work_dir.mkdir(exist_ok=True, parents=True)
     barrier()
+    seed = train_config.data.seed if train_config.data.seed is not None else train_config.seed
     return DataLoader(
         IterableDataset(
             dataset,  # type: ignore
             train_config.global_train_batch_size,
-            seed=train_config.seed + (train_config.epoch or 0),
+            seed=seed + (train_config.epoch or 0),
             shuffle=True,
             drop_last=train_config.data.drop_last,
             work_dir=work_dir,
         ),
         batch_size=train_config.device_train_batch_size,
         drop_last=train_config.data.drop_last,
         collate_fn=collator,
```

### Comparing `ai2-olmo-0.2.5/olmo/data/collator.py` & `ai2_olmo-0.3.0/olmo/data/collator.py`

 * *Files identical despite different names*

### Comparing `ai2-olmo-0.2.5/olmo/data/iterable_dataset.py` & `ai2_olmo-0.3.0/olmo/data/iterable_dataset.py`

 * *Files identical despite different names*

### Comparing `ai2-olmo-0.2.5/olmo/data/memmap_dataset.py` & `ai2_olmo-0.3.0/olmo/data/memmap_dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from copy import deepcopy
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 import numpy as np
 import torch
 from torch.utils.data import Dataset
 
-from olmo.exceptions import OlmoEnvironmentError
+from olmo.exceptions import OLMoEnvironmentError
 
 from ..aliases import PathOrStr
 from ..util import _get_s3_client, file_size, get_bytes_range
 
 __all__ = ["MemMapDataset"]
 
 
@@ -89,15 +89,15 @@
 
     @property
     def offsets(self) -> List[Tuple[int, int]]:
         # Create the global S3 client up front to work around a threading issue in boto.
         _get_s3_client("s3")
         try:
             _get_s3_client("r2")
-        except OlmoEnvironmentError:
+        except OLMoEnvironmentError:
             # R2 might not be needed, so ignore this error. We will get an error
             # later if R2 is needed.
             pass
 
         if self._mmap_offsets is None:
             import concurrent.futures
```

### Comparing `ai2-olmo-0.2.5/olmo/eval/__init__.py` & `ai2_olmo-0.3.0/olmo/eval/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Dict, List, Union
 
 import torch
 from torch.utils.data import DataLoader, DistributedSampler
 from torchmetrics import MeanMetric, Metric
 
 from ..config import EvaluatorConfig, EvaluatorType, TrainConfig
-from ..exceptions import OlmoConfigurationError
+from ..exceptions import OLMoConfigurationError
 from ..tokenizer import Tokenizer
 from ..torch_util import get_global_rank, get_world_size
 from .downstream import ICLMetric, label_to_task_map
 from .evaluator import Evaluator
 
 __all__ = [
     "Evaluator",
@@ -89,15 +89,15 @@
 
         eval_metric: Union[Metric, Dict[str, Metric]]
         if eval_config.data.paths:
             eval_metric = make_metric()
         elif eval_config.data.datasets:
             eval_metric = {label: make_metric() for label in eval_config.data.datasets.keys()}
         else:
-            raise OlmoConfigurationError("One of DataConfig.paths or DataConfig.datasets is required")
+            raise OLMoConfigurationError("One of DataConfig.paths or DataConfig.datasets is required")
 
         return Evaluator(
             label=eval_config.label,
             type=eval_config.type,
             eval_loader=eval_loader,
             eval_metric=eval_metric,
             subset_num_batches=eval_config.subset_num_batches,
```

### Comparing `ai2-olmo-0.2.5/olmo/eval/downstream.py` & `ai2_olmo-0.3.0/olmo/eval/downstream.py`

 * *Files 4% similar despite different names*

```diff
@@ -161,15 +161,15 @@
 
         self.tokenizer = tokenizer
         self.dataset_path = dataset_path
         self.dataset_name = dataset_name
         self.model_ctx_len = model_ctx_len
         self.prompts = prompts
         self.current_prompt = None
-        self.log_instances = 5  # Log the first few instances as a sanity check
+        self.log_instances = 0  # Set to > 0 to log the first few instances as a sanity check
 
         self.samples: List[Dict[str, Any]] = []
         dataset_names: Sequence[Optional[str]]
         if isinstance(dataset_name, str) or dataset_name is None:
             dataset_names = [dataset_name]
         else:
             dataset_names = dataset_name
@@ -585,15 +585,15 @@
         'label': ['A', 'B', 'C', 'D']},
         'answerKey': 'A'
     }
     """
 
     metric_type = "len_norm"
 
-    def __init__(self, tokenizer, dataset_path="openbookqa", dataset_name=None):
+    def __init__(self, tokenizer, dataset_path="openbookqa", dataset_name="main"):
         super().__init__(
             tokenizer=tokenizer,
             dataset_path=dataset_path,
             dataset_name=dataset_name,
         )
 
     def doc_to_text(self, doc):
@@ -750,14 +750,93 @@
         super().__init__(
             tokenizer=tokenizer,
             dataset_path=dataset_path,
             dataset_name=dataset_name,
         )
 
 
+class BasicArithmetic(ArcEasy):
+    """This is a basic arithmetic task follows the same prompt format as ArcEasy.
+    Example:
+    {"id": "q85_1d1d_max1d_plus",
+    "question": "Calculate 2 + 5 =",
+    "choices": {"text": ["8", "7", "6", "17"],
+    "label": ["A", "B", "C", "D"]},
+    "answerKey": "B", "type_tag": "easy"}
+
+    """
+
+    metric_type = "acc"
+
+    def __init__(self, tokenizer, dataset_path="allenai/basic_arithmetic", dataset_name=None):
+        super().__init__(
+            tokenizer=tokenizer,
+            dataset_path=dataset_path,
+            dataset_name=dataset_name,
+        )
+
+
+class CommonsenseQA(ArcEasy):
+    """CommonsenseQA
+    Example:
+    {'id': 'e68fb2448fd74e402aae9982aa76e527',
+    'question': 'Where are  you likely to find a hamburger?',
+    'question_concept': 'hamburger',
+    'choices': {'label': ['A', 'B', 'C', 'D', 'E'],
+    'text': ['fast food restaurant', 'pizza', 'ground up dead cows', 'mouth', 'cow carcus']},
+    'answerKey': 'A'}
+    """
+
+    metric_type = "len_norm"
+
+    def __init__(self, tokenizer, dataset_path="tau/commonsense_qa", dataset_name=None):
+        super().__init__(
+            tokenizer=tokenizer,
+            dataset_path=dataset_path,
+            dataset_name=dataset_name,
+        )
+
+
+class SocialIQa(ICLMultiChoiceTaskDataset):
+    """SocialIQa
+    Example:
+    {'context': 'Jordan was in charge of taking the food on the camping trip and left all the food at home.',
+     'question': 'How would Jordan feel afterwards?',
+     'answerA': 'horrible that he let his friends down on the camping trip',
+     'answerB': "happy that he doesn't need to do the cooking on the trip",
+     'answerC': 'very proud and accomplished about the camping trip', 'label': '1'}
+    """
+
+    metric_type = "len_norm"
+
+    def __init__(self, tokenizer, dataset_path="social_i_qa", dataset_name=None):
+        super().__init__(
+            tokenizer=tokenizer,
+            dataset_path=dataset_path,
+            dataset_name=dataset_name,
+        )
+
+    def doc_to_text(self, doc):
+        return "Question: " + doc["context"] + " " + doc["question"] + "\nAnswer:"
+
+    def doc_to_continuations(self, doc):
+        # add spaces in front of continuation
+        return [
+            " " + doc["answerA"],
+            " " + doc["answerB"],
+            " " + doc["answerC"],
+        ]
+
+    def doc_to_label(self, doc):
+        return int(doc["label"]) - 1
+
+    def doc_to_domain_conditional(self, doc):
+        return "Answer:"
+
+
 class COPA(ICLMultiChoiceTaskDataset):
     """Prompt: "PREMISE.strip()[:-1] because/therefore"
     Req_loglikelihood('The pair of students came under scrutiny by the teacher because', ' the students both received excellent grades.'
     continuations: CHOICE1/CHOICE2
 
     "cause": "because",
     "effect": "therefore",
@@ -1080,14 +1159,15 @@
     def __init__(
         self,
         tokenizer,
         dataset_path="hails/mmlu_no_train",
         dataset_name=None,
         split="validation",
         prompt_variations=None,
+        mc_labels=False,
     ):
         dataset_names = []
         # Collect the relevant categories
         if dataset_name in MMLU._categories:
             for sub_cat in MMLU._categories[dataset_name]:
                 for name, cats in MMLU._subcategories.items():
                     if sub_cat in cats:
@@ -1095,50 +1175,75 @@
         elif dataset_name in MMLU._subcategories:
             dataset_names.append(dataset_name)
         else:  # E.g., "math"
             for name, cats in MMLU._subcategories.items():
                 if dataset_name in cats:
                     dataset_names.append(name)
         self.dev_set = {}
-        if prompt_variations == 1:
-            prompts = [None, "inst", "inst+1", "inst+2", "inst+3", "inst+4", "inst+5"]
+        self.mc_labels = mc_labels
+        prompts: List[Union[None, str]] = [None]
+        if prompt_variations is not None:
+            if prompt_variations == 1:
+                prompts = [None, "inst", "inst+1", "inst+2", "inst+3", "inst+4", "inst+5"]
+            elif prompt_variations == 2:
+                prompts = ["inst+5"]
+            else:
+                raise ValueError(f"Unknown prompt variations: {prompt_variations}")
             # Need to grab the dev set for the few-shot prompts
             for name in dataset_names:
                 self.dev_set[name] = datasets.load_dataset(
                     path=dataset_path, name=name, split="dev", trust_remote_code=True
                 )
         super().__init__(
             tokenizer=tokenizer,
             dataset_path=dataset_path,
             dataset_name=dataset_names,
             split=split,
             prompts=prompts,
         )
 
     def doc_to_text(self, doc):
-        output_text = "Question: " + doc["question"] + "\nAnswer:"
+        def format_example(doc, keys):
+            question_prefix = ""
+            if not self.mc_labels:
+                question_prefix = "Question: "  # To make context more clear
+            question = question_prefix + doc["question"].strip()
+            choices = ""
+            if self.mc_labels:
+                choices = "".join([f"{key}. {choice}\n" for key, choice in zip(keys, doc["choices"])])
+            prompt = f"{question}\n{choices}Answer:"
+            return prompt
+
+        keys = ["A", "B", "C", "D"]
+        output_text = format_example(doc, keys)
+
         if self.current_prompt is not None:
             prefix = ""
             if "inst" in self.current_prompt:
                 subject = doc.get("subject").replace("_", " ")
                 prefix = f"The following are multiple choice questions (with answers) about {subject}:\n\n"
             num_shots = re.findall("\\+(\\d+)", self.current_prompt)
             if num_shots:
                 dev_set = self.dev_set.get(doc.get("subject"), [])
                 num_shots_int = int(num_shots[0])
                 for idx, dev_doc in enumerate(dev_set):
                     if idx >= num_shots_int:
                         break
-                    answer = dev_doc["choices"][dev_doc["answer"]]
-                    prefix += "Question: " + dev_doc["question"] + "\nAnswer: " + answer + "\n\n"
+                    if self.mc_labels:
+                        answer = keys[dev_doc["answer"]]
+                    else:
+                        answer = dev_doc["choices"][dev_doc["answer"]]
+                    prefix += format_example(dev_doc, keys) + " " + answer + "\n\n"
             output_text = prefix + output_text
         return output_text
 
     def doc_to_continuations(self, doc):
         # add spaces in front of continuation
+        if self.mc_labels:
+            return [" A", " B", " C", " D"]
         return [" " + choice for choice in doc["choices"]]
 
     def doc_to_label(self, doc):
         return doc["answer"]
 
     def doc_to_domain_conditional(self, doc):
         del doc
@@ -1150,25 +1255,51 @@
     "hellaswag": HellaSwag,
     "winogrande": WinoGrande,
     "openbook_qa": OpenBookQA,
     "boolq": BoolQ,
     "sciq": SciQ,
     "arc_easy": ArcEasy,
     "arc_challenge": ArcChallenge,
+    "basic_arithmetic": BasicArithmetic,
     "copa": COPA,
     "rte": RTE,
     "commitment_bank": CommitmentBank,
     "mrpc": MRPC,
     "sst2": SST2,
+    "commonsense_qa": CommonsenseQA,
+    "social_iqa": SocialIQa,
     "mmlu_stem_test": (MMLU, {"dataset_name": "stem", "split": "test"}),
     "mmlu_humanities_test": (MMLU, {"dataset_name": "humanities", "split": "test"}),
     "mmlu_social_sciences_test": (MMLU, {"dataset_name": "social_sciences", "split": "test"}),
     "mmlu_other_test": (MMLU, {"dataset_name": "other", "split": "test"}),
     "mmlu_stem": (MMLU, {"dataset_name": "stem"}),
     "mmlu_humanities": (MMLU, {"dataset_name": "humanities"}),
     "mmlu_social_sciences": (MMLU, {"dataset_name": "social_sciences"}),
     "mmlu_other": (MMLU, {"dataset_name": "other"}),
     "mmlu_stem_var": (MMLU, {"dataset_name": "stem", "prompt_variations": 1}),
     "mmlu_humanities_var": (MMLU, {"dataset_name": "humanities", "prompt_variations": 1}),
     "mmlu_social_sciences_var": (MMLU, {"dataset_name": "social_sciences", "prompt_variations": 1}),
     "mmlu_other_var": (MMLU, {"dataset_name": "other", "prompt_variations": 1}),
+    "mmlu_stem_mc_5shot": (MMLU, {"dataset_name": "stem", "prompt_variations": 2, "mc_labels": True}),
+    "mmlu_humanities_mc_5shot": (MMLU, {"dataset_name": "humanities", "prompt_variations": 2, "mc_labels": True}),
+    "mmlu_social_sciences_mc_5shot": (
+        MMLU,
+        {"dataset_name": "social_sciences", "prompt_variations": 2, "mc_labels": True},
+    ),
+    "mmlu_other_mc_5shot": (MMLU, {"dataset_name": "other", "prompt_variations": 2, "mc_labels": True}),
+    "mmlu_stem_mc_5shot_test": (
+        MMLU,
+        {"dataset_name": "stem", "split": "test", "prompt_variations": 2, "mc_labels": True},
+    ),
+    "mmlu_humanities_mc_5shot_test": (
+        MMLU,
+        {"dataset_name": "humanities", "split": "test", "prompt_variations": 2, "mc_labels": True},
+    ),
+    "mmlu_social_sciences_mc_5shot_test": (
+        MMLU,
+        {"dataset_name": "social_sciences", "split": "test", "prompt_variations": 2, "mc_labels": True},
+    ),
+    "mmlu_other_mc_5shot_test": (
+        MMLU,
+        {"dataset_name": "other", "split": "test", "prompt_variations": 2, "mc_labels": True},
+    ),
 }
```

### Comparing `ai2-olmo-0.2.5/olmo/eval/evaluator.py` & `ai2_olmo-0.3.0/olmo/eval/evaluator.py`

 * *Files identical despite different names*

### Comparing `ai2-olmo-0.2.5/olmo/exceptions.py` & `ai2_olmo-0.3.0/olmo/exceptions.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,37 +1,50 @@
-__all__ = ["OlmoError", "OlmoConfigurationError", "OlmoCliError", "OlmoEnvironmentError", "OlmoNetworkError"]
+__all__ = [
+    "OLMoError",
+    "OLMoConfigurationError",
+    "OLMoCliError",
+    "OLMoEnvironmentError",
+    "OLMoNetworkError",
+    "OLMoCheckpointError",
+]
 
 
-class OlmoError(Exception):
+class OLMoError(Exception):
     """
     Base class for all custom OLMo exceptions.
     """
 
 
-class OlmoConfigurationError(OlmoError):
+class OLMoConfigurationError(OLMoError):
     """
     An error with a configuration file.
     """
 
 
-class OlmoCliError(OlmoError):
+class OLMoCliError(OLMoError):
     """
     An error from incorrect CLI usage.
     """
 
 
-class OlmoEnvironmentError(OlmoError):
+class OLMoEnvironmentError(OLMoError):
     """
     An error from incorrect environment variables.
     """
 
 
-class OlmoNetworkError(OlmoError):
+class OLMoNetworkError(OLMoError):
     """
     An error with a network request.
     """
 
 
-class OlmoThreadError(Exception):
+class OLMoCheckpointError(OLMoError):
+    """
+    An error occurred reading or writing from a checkpoint.
+    """
+
+
+class OLMoThreadError(Exception):
     """
     Raised when a thread fails.
     """
```

### Comparing `ai2-olmo-0.2.5/olmo/initialization.py` & `ai2_olmo-0.3.0/olmo/initialization.py`

 * *Files identical despite different names*

### Comparing `ai2-olmo-0.2.5/olmo/model.py` & `ai2_olmo-0.3.0/olmo/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,41 +38,39 @@
     ActivationType,
     BlockType,
     CheckpointType,
     FSDPWrapStrategy,
     LayerNormType,
     ModelConfig,
 )
-from .exceptions import OlmoConfigurationError
+from .exceptions import OLMoConfigurationError
 from .initialization import ModuleType, init_weights
 from .torch_util import ensure_finite_
 
 if sys.version_info.minor > 8:
     from collections.abc import MutableMapping
 elif sys.version_info.minor == 8:
     from typing import MutableMapping
 else:
     raise SystemExit("This script supports Python 3.8 or higher")
 
 __all__ = [
     "LayerNormBase",
     "LayerNorm",
     "RMSLayerNorm",
-    "AMDLayerNorm",
     "RotaryEmbedding",
     "Activation",
     "GELU",
     "ReLU",
     "SwiGLU",
-    "OlmoBlock",
-    "OlmoSequentialBlock",
-    "OlmoParallelBlock",
-    "Olmo",
-    "OlmoOutput",
-    "OlmoGenerateOutput",
+    "OLMoBlock",
+    "OLMoSequentialBlock",
+    "OLMo",
+    "OLMoOutput",
+    "OLMoGenerateOutput",
 ]
 
 
 log = logging.getLogger(__name__)
 
 
 def activation_checkpoint_function(cfg: ModelConfig):
@@ -84,14 +82,30 @@
     return partial(
         checkpoint,
         preserve_rng_state=preserve_rng_state,
         use_reentrant=False,
     )
 
 
+def should_checkpoint_block(strategy: Optional[ActivationCheckpointingStrategy], block_idx: int) -> bool:
+    if strategy is None:
+        return False
+    elif (
+        (strategy == ActivationCheckpointingStrategy.whole_layer)
+        or (strategy == ActivationCheckpointingStrategy.one_in_two and block_idx % 2 == 0)
+        or (strategy == ActivationCheckpointingStrategy.one_in_three and block_idx % 3 == 0)
+        or (strategy == ActivationCheckpointingStrategy.one_in_four and block_idx % 4 == 0)
+        or (strategy == ActivationCheckpointingStrategy.two_in_three and block_idx % 3 != 0)
+        or (strategy == ActivationCheckpointingStrategy.three_in_four and block_idx % 4 != 0)
+    ):
+        return True
+    else:
+        return False
+
+
 class BufferCache(dict, MutableMapping[str, torch.Tensor]):
     """
     Cache for attention biases and other things that would normally be stored as buffers.
     We avoid using buffers because we've run into various issues doing so with FSDP.
     In general it appears the way FSDP handles buffers is not well-defined.
     It doesn't shard them but apparently it does synchronize them across processes, which we want to avoid
     since (A) it isn't necessary, and (B) we sometimes have `-inf` in these biases which might get turned into
@@ -148,16 +162,14 @@
     def build(cls, config: ModelConfig, size: Optional[int] = None, **kwargs) -> LayerNormBase:
         if config.layer_norm_type == LayerNormType.default:
             return LayerNorm(config, size=size, low_precision=False, **kwargs)
         elif config.layer_norm_type == LayerNormType.low_precision:
             return LayerNorm(config, size=size, low_precision=True, **kwargs)
         elif config.layer_norm_type == LayerNormType.rms:
             return RMSLayerNorm(config, size=size, **kwargs)
-        elif config.layer_norm_type == LayerNormType.amd_compatible:
-            return AMDLayerNorm(config, size=size, **kwargs)
         else:
             raise NotImplementedError(f"Unknown LayerNorm type: '{config.layer_norm_type}'")
 
     def _cast_if_autocast_enabled(self, tensor: torch.Tensor, dtype: Optional[torch.dtype] = None) -> torch.Tensor:
         # NOTE: `is_autocast_enabled()` only checks for CUDA autocast, so we use the separate function
         # `is_autocast_cpu_enabled()` for CPU autocast.
         # See https://github.com/pytorch/pytorch/issues/110966.
@@ -203,46 +215,14 @@
                 return F.layer_norm(
                     downcast_x, self.normalized_shape, weight=downcast_weight, bias=downcast_bias, eps=self.eps
                 )
         else:
             return F.layer_norm(x, self.normalized_shape, weight=self.weight, bias=self.bias, eps=self.eps)
 
 
-class AMDLayerNorm(LayerNormBase):
-    """
-    LayerNorm implemented using PyTorch primitives.
-
-    We do this to work around a bug in the PyTorch/ROCm implementation of layer norm that fails with a
-    segfault when the bias is not present.
-    """
-
-    def __init__(
-        self,
-        config: ModelConfig,
-        size: Optional[int] = None,
-        elementwise_affine: Optional[bool] = None,
-        eps: float = 1e-05,
-    ):
-        super().__init__(config, size=size, elementwise_affine=elementwise_affine, eps=eps)
-
-    def forward(self, x: torch.Tensor) -> torch.Tensor:
-        og_dtype = x.dtype
-        x = self._cast_if_autocast_enabled(x, dtype=torch.float32)
-        with torch.autocast(enabled=False, device_type=x.device.type):
-            var, mean = torch.var_mean(x, dim=-1, correction=0, keepdim=True)
-            var.add_(self.eps)
-            var.rsqrt_()  # rsqrt should be more stable than 1/sqrt
-            x = var * (x - mean)
-            if self.weight is not None:
-                x.mul_(self.weight)
-            if self.bias is not None:
-                x.add_(self.bias)
-            return x.to(og_dtype)
-
-
 class RMSLayerNorm(LayerNormBase):
     """
     RMS layer norm, a simplified :class:`LayerNorm` implementation
     """
 
     def __init__(
         self,
@@ -417,15 +397,15 @@
     m = torch.arange(1, config.n_heads + 1, dtype=torch.float, device=device)
     m.mul_(config.alibi_bias_max / config.n_heads)
 
     # shape: (1, n_heads, seq_len, seq_len)
     return alibi_bias * (1.0 / (2 ** m.view(1, config.n_heads, 1, 1)))  # type: ignore
 
 
-class OlmoBlock(nn.Module):
+class OLMoBlock(nn.Module):
     """
     A base class for transformer block implementations.
     """
 
     def __init__(self, layer_id: int, config: ModelConfig, cache: BufferCache):
         super().__init__()
         self.layer_id = layer_id
@@ -441,17 +421,18 @@
         # Dropout.
         self.dropout = Dropout(config.residual_dropout)
 
         # Layer norms.
         self.k_norm: Optional[LayerNormBase] = None
         self.q_norm: Optional[LayerNormBase] = None
         if config.attention_layer_norm:
+            assert config.effective_n_kv_heads is not None
             self.k_norm = LayerNormBase.build(
                 config,
-                size=config.d_model // config.n_heads if config.multi_query_attention else None,
+                size=(config.d_model // config.n_heads) * config.effective_n_kv_heads,
                 elementwise_affine=config.attention_layer_norm_with_affine,
             )
             self.q_norm = LayerNormBase.build(config, elementwise_affine=config.attention_layer_norm_with_affine)
 
         # Make sure QKV clip coefficient is positive, otherwise it's not well-defined.
         if config.clip_qkv is not None:
             assert config.clip_qkv > 0
@@ -474,14 +455,23 @@
         )
         self.ff_out._is_residual = True  # type: ignore
 
         # Rotary embeddings.
         if self.config.rope:
             self.rotary_emb = RotaryEmbedding(config, self.__cache)
 
+        self.flash_attn_func = None
+        if config.flash_attention:
+            try:
+                from flash_attn import flash_attn_func  # type: ignore
+
+                self.flash_attn_func = flash_attn_func
+            except ModuleNotFoundError:
+                pass
+
     def reset_parameters(self):
         if self.k_norm is not None:
             self.k_norm.reset_parameters()
         if self.q_norm is not None:
             self.q_norm.reset_parameters()
         init_weights(
             self.config,
@@ -527,25 +517,38 @@
         attn_mask: Optional[torch.Tensor] = None,
         dropout_p: float = 0.0,
         is_causal: bool = False,
     ) -> torch.Tensor:
         """
         Computes scaled dot product attention on query, key and value tensors, using an optional
         attention mask if passed, and applying dropout if a probability greater than 0.0 is specified.
-
-        This method is based on PyTorch's `scaled_dot_product_attention`.
         """
-        return F.scaled_dot_product_attention(
-            q,
-            k,
-            v,
-            attn_mask=attn_mask,
-            dropout_p=dropout_p,
-            is_causal=is_causal,
-        )
+        if self.flash_attn_func is not None and attn_mask is None:
+            r = self.flash_attn_func(
+                q.transpose(1, 2), k.transpose(1, 2), v.transpose(1, 2), dropout_p=dropout_p, causal=is_causal
+            )
+            return r.transpose(1, 2)
+        else:
+            # torch's sdpa doesn't support GQA, so we're doing this
+            assert k.size(1) == v.size(1)
+            num_kv_heads = k.size(1)
+            num_q_heads = q.size(1)
+            if num_q_heads != num_kv_heads:
+                assert num_q_heads % num_kv_heads == 0
+                k = k.repeat_interleave(num_q_heads // num_kv_heads, dim=1, output_size=num_q_heads)
+                v = v.repeat_interleave(num_q_heads // num_kv_heads, dim=1, output_size=num_q_heads)
+
+            return F.scaled_dot_product_attention(
+                q,
+                k,
+                v,
+                attn_mask=attn_mask,
+                dropout_p=dropout_p,
+                is_causal=is_causal,
+            )
 
     def attention(
         self,
         q: torch.Tensor,
         k: torch.Tensor,
         v: torch.Tensor,
         attention_bias: Optional[torch.Tensor] = None,
@@ -559,24 +562,18 @@
         if self.q_norm is not None and self.k_norm is not None:
             q = self.q_norm(q).to(dtype=dtype)
             k = self.k_norm(k).to(dtype=dtype)
 
         # Move head forward to be next to the batch dim.
         # shape: (B, nh, T, hs)
         q = q.view(B, T, self.config.n_heads, C // self.config.n_heads).transpose(1, 2)
-        if self.config.multi_query_attention:
-            # shape: (B, 1, T, hs)
-            k = k.view(B, T, 1, C // self.config.n_heads).transpose(1, 2)
-            # shape: (B, 1, T, hs)
-            v = v.view(B, T, 1, C // self.config.n_heads).transpose(1, 2)
-        else:
-            # shape: (B, nh, T, hs)
-            k = k.view(B, T, self.config.n_heads, C // self.config.n_heads).transpose(1, 2)
-            # shape: (B, nh, T, hs)
-            v = v.view(B, T, self.config.n_heads, C // self.config.n_heads).transpose(1, 2)
+        # shape: (B, n_kv_h, T, hs)
+        k = k.view(B, T, self.config.effective_n_kv_heads, C // self.config.n_heads).transpose(1, 2)
+        # shape: (B, n_kv_h, T, hs)
+        v = v.view(B, T, self.config.effective_n_kv_heads, C // self.config.n_heads).transpose(1, 2)
 
         if layer_past is not None:
             past_key, past_value = layer_past
             k = torch.cat((past_key, k), dim=-2)
             v = torch.cat((past_value, v), dim=-2)
 
         present = (k, v) if use_cache else None
@@ -620,41 +617,42 @@
         attention_bias: Optional[torch.FloatTensor] = None,
         layer_past: Optional[Tuple[torch.Tensor, torch.Tensor]] = None,
         use_cache: bool = False,
     ) -> Tuple[torch.Tensor, Optional[Tuple[torch.Tensor, torch.Tensor]]]:
         raise NotImplementedError
 
     @classmethod
-    def build(cls, layer_id: int, config: ModelConfig, cache: BufferCache) -> OlmoBlock:
+    def build(cls, layer_id: int, config: ModelConfig, cache: BufferCache) -> OLMoBlock:
         if config.block_type == BlockType.sequential:
-            return OlmoSequentialBlock(layer_id, config, cache)
-        elif config.block_type == BlockType.parallel:
-            return OlmoParallelBlock(layer_id, config, cache)
+            return OLMoSequentialBlock(layer_id, config, cache)
         elif config.block_type == BlockType.llama:
-            return OlmoLlamaBlock(layer_id, config, cache)
+            return OLMoLlamaBlock(layer_id, config, cache)
         else:
             raise NotImplementedError(f"Unknown block type: '{config.block_type}'")
 
 
-class OlmoSequentialBlock(OlmoBlock):
+class OLMoSequentialBlock(OLMoBlock):
     """
     This is a typical transformer block where the output is computed as ``MLP(LN(x + Attention(LN(x))))``
     (plus another skip connection).
     """
 
     def __init__(self, layer_id: int, config: ModelConfig, cache: BufferCache):
         super().__init__(layer_id, config, cache)
         # Layer norms.
         self.attn_norm = LayerNorm.build(config)
         self.ff_norm = LayerNorm.build(config)
         # Attention input projection. Projects x -> (q, k, v)
-        if config.multi_query_attention:
-            self.fused_dims = (config.d_model, config.d_model // config.n_heads, config.d_model // config.n_heads)
-        else:
-            self.fused_dims = (config.d_model, config.d_model, config.d_model)
+
+        head_dim = config.d_model // config.n_heads
+        self.fused_dims = (
+            config.d_model,
+            config.effective_n_kv_heads * head_dim,
+            config.effective_n_kv_heads * head_dim,
+        )
         self.att_proj = nn.Linear(
             config.d_model, sum(self.fused_dims), bias=config.include_bias, device=config.init_device
         )
         # Feed-forward input projection.
         self.ff_proj = nn.Linear(
             config.d_model, self.hidden_size, bias=config.include_bias, device=config.init_device
         )
@@ -679,14 +677,16 @@
         use_cache: bool = False,
     ) -> Tuple[torch.Tensor, Optional[Tuple[torch.Tensor, torch.Tensor]]]:
         # Get query, key, value projections.
         # shape:
         #  - for regular attn q, k, v: (batch_size, seq_len, d_model)
         #  - for multi-query attn q: (batch_size, seq_len, d_model)
         #                      k, v: (batch_size, seq_len, d_model // n_heads)
+        #  - for group query attn q: (batch_size, seq_len, d_model)
+        #                      k, v: (batch_size, seq_len, d_model // n_kv_heads)
         if self._activation_checkpoint_fn is not None:
             qkv = self.att_proj(self._activation_checkpoint_fn(self.attn_norm, x))
         else:
             qkv = self.att_proj(self.attn_norm(x))
 
         if self.config.clip_qkv is not None:
             qkv.clamp_(min=-self.config.clip_qkv, max=self.config.clip_qkv)
@@ -720,110 +720,18 @@
         x = self.ff_out(x)
         x = self.dropout(x)
         x = og_x + x
 
         return x, cache
 
 
-class OlmoParallelBlock(OlmoBlock):
-    """
-    This is a transformer block where the output is computed as ``MLP(LN(x)) + Attention(LN(x))``
-    as in the PaLM architecture, as opposed to the typical ``MLP(LN(x + Attention(LN(x))))``
-    as in :class:`OlmoSequentialBlock` (ignoring some skip connections).
-
-    The decoupling of the MLP and Attention functions allow us to fuse the separate input projections
-    into a single linear layer to increase throughput. In this configuration it's also straight-forward
-    to fuse the output projections, but we found that didn't help.
-    """
-
-    def __init__(self, layer_id: int, config: ModelConfig, cache: BufferCache):
-        super().__init__(layer_id, config, cache)
-        self.norm = LayerNorm.build(config)
-        # Fused attention and feed-forward projection.
-        # NOTE: we could also fuse the attention and feed-forward output projections but we
-        # found that didn't help, possibly because of the overhead of joining the `att` and
-        # `ff` activations together. See https://github.com/allenai/LLM/pull/79 for details.
-        if config.multi_query_attention:
-            self.fused_dims = (
-                config.d_model,
-                config.d_model // config.n_heads,
-                config.d_model // config.n_heads,
-                self.hidden_size,
-            )
-        else:
-            self.fused_dims = (config.d_model, config.d_model, config.d_model, self.hidden_size)
-        self.fused_attn_ff_proj = nn.Linear(
-            config.d_model, sum(self.fused_dims), bias=config.include_bias, device=config.init_device
-        )
-
-    def reset_parameters(self):
-        super().reset_parameters()
-        self.norm.reset_parameters()
-        # NOTE: the standard deviation for these weights does not depend on the layer.
-        init_weights(
-            self.config,
-            self.fused_attn_ff_proj,
-            d=self.config.d_model,
-            layer_id=None,
-            type_of_module=ModuleType.in_module,
-        )
-
-    def forward(
-        self,
-        x: torch.Tensor,
-        attention_bias: Optional[torch.Tensor] = None,
-        layer_past: Optional[Tuple[torch.Tensor, torch.Tensor]] = None,
-        use_cache: bool = False,
-    ) -> Tuple[torch.Tensor, Optional[Tuple[torch.Tensor, torch.Tensor]]]:
-        # Get query, key, value, and feed-forward projections.
-        # shape of q, k, v:
-        #  - for regular attn q, k, v: (batch_size, seq_len, d_model)
-        #  - for multi-query attn q: (batch_size, seq_len, d_model)
-        #                      k, v: (batch_size, seq_len, d_model // n_heads)
-        # shape of ff:      (batch_size, seq_len, hidden_size)
-        if self._activation_checkpoint_fn is not None:
-            q, k, v, ff = self.fused_attn_ff_proj(self._activation_checkpoint_fn(self.norm, x)).split(
-                self.fused_dims, dim=-1
-            )
-        else:
-            q, k, v, ff = self.fused_attn_ff_proj(self.norm(x)).split(self.fused_dims, dim=-1)
-
-        if self.config.clip_qkv is not None:
-            q.clamp_(min=-self.config.clip_qkv, max=self.config.clip_qkv)
-            k.clamp_(min=-self.config.clip_qkv, max=self.config.clip_qkv)
-            v.clamp_(min=-self.config.clip_qkv, max=self.config.clip_qkv)
-
-        # Get attention scores.
-        # shape: (B, T, C)
-        if self._activation_checkpoint_fn is not None:
-            att, cache = self._activation_checkpoint_fn(  # type: ignore
-                self.attention, q, k, v, attention_bias, layer_past=layer_past, use_cache=use_cache
-            )
-        else:
-            att, cache = self.attention(q, k, v, attention_bias, layer_past=layer_past, use_cache=use_cache)
-
-        # Apply output projections (and activation function) and sum the results.
-        # We keep these projections separate because we found that we got better throughput this
-        # way compared to fusing them.
-        if self._activation_checkpoint_fn is not None:
-            return (
-                x + self.dropout(self.ff_out(self._activation_checkpoint_fn(self.act, ff))) + self.dropout(att),
-                cache,
-            )
-        else:
-            return (
-                x + self.dropout(self.ff_out(self.act(ff))) + self.dropout(att),
-                cache,
-            )
-
-
-class OlmoLlamaBlock(OlmoBlock):
+class OLMoLlamaBlock(OLMoBlock):
     """
     This is a transformer block where the output is computed as ``MLP(LN(x + Attention(LN(x))))``
-    (plus another skip connection). This block is similar to `OlmoSequentialBlock`
+    (plus another skip connection). This block is similar to `OLMoSequentialBlock`
     but some operations have slightly different implementations to imitate the
     behavior of Llama.
     """
 
     def __init__(self, layer_id: int, config: ModelConfig, cache: BufferCache):
         super().__init__(layer_id, config, cache)
         # Layer norms.
@@ -935,15 +843,15 @@
         x = self.ff_out(x)
         x = self.dropout(x)
         x = og_x + x
 
         return x, cache
 
 
-class OlmoOutput(NamedTuple):
+class OLMoOutput(NamedTuple):
     logits: torch.FloatTensor
     """
     A tensor of shape `(batch_size, seq_len, vocab_size)` representing the log probabilities
     for the next token *before* normalization via (log) softmax.
     """
 
     attn_key_values: Optional[List[Tuple[torch.Tensor, torch.Tensor]]]
@@ -953,28 +861,28 @@
 
     hidden_states: Optional[Tuple[torch.Tensor]]
     """
     Hidden states from each block.
     """
 
 
-class OlmoGenerateOutput(NamedTuple):
+class OLMoGenerateOutput(NamedTuple):
     token_ids: torch.LongTensor
     """
     The generated token IDs, a tensor of shape `(batch_size, beam_size, max_steps)`.
     These do *not* include the original input IDs.
     """
 
     scores: torch.FloatTensor
     """
     The scores of the generated sequences, a tensor of shape `(batch_size, beam_size)`.
     """
 
 
-class OlmoBlockGroup(nn.ModuleList):
+class OLMoBlockGroup(nn.ModuleList):
     def __init__(self, config: ModelConfig, layer_offset: int, modules: Optional[Iterable[nn.Module]] = None):
         super().__init__(modules)
         self.config = config
         self.layer_offset = layer_offset
         self.activation_checkpointing_strategy: Optional[ActivationCheckpointingStrategy] = None
         self._activation_checkpoint_fn = activation_checkpoint_function(self.config)
 
@@ -985,29 +893,15 @@
         layers_past: Optional[List[Tuple[torch.Tensor, torch.Tensor]]] = None,
         use_cache: bool = False,
     ) -> Tuple[torch.Tensor, Optional[List[Tuple[torch.Tensor, torch.Tensor]]]]:
         attn_key_values: Optional[List[Tuple[torch.Tensor, torch.Tensor]]] = [] if use_cache else None
         for block_idx, block in enumerate(self):
             layer_past = None if layers_past is None else layers_past[block_idx]
             block_idx += self.layer_offset
-            if (
-                (self.activation_checkpointing_strategy == ActivationCheckpointingStrategy.whole_layer)
-                or (
-                    self.activation_checkpointing_strategy == ActivationCheckpointingStrategy.one_in_two
-                    and block_idx % 2 == 0
-                )
-                or (
-                    self.activation_checkpointing_strategy == ActivationCheckpointingStrategy.one_in_three
-                    and block_idx % 3 == 0
-                )
-                or (
-                    self.activation_checkpointing_strategy == ActivationCheckpointingStrategy.one_in_four
-                    and block_idx % 4 == 0
-                )
-            ):
+            if should_checkpoint_block(self.activation_checkpointing_strategy, block_idx):
                 # shape: (batch_size, seq_len, d_model)
                 x, cache = self._activation_checkpoint_fn(  # type: ignore
                     block, x, attention_bias=attention_bias, layer_past=layer_past, use_cache=use_cache
                 )
             else:
                 # shape: (batch_size, seq_len, d_model)
                 x, cache = block(x, attention_bias=attention_bias, layer_past=layer_past, use_cache=use_cache)
@@ -1022,63 +916,63 @@
 
     def set_activation_checkpointing(self, strategy: Optional[ActivationCheckpointingStrategy]):
         self.activation_checkpointing_strategy = strategy
         for block in self:
             block.set_activation_checkpointing(strategy)
 
 
-class Olmo(nn.Module):
+class OLMo(nn.Module):
     def __init__(self, config: ModelConfig, init_params: bool = True):
         super().__init__()
         self.config = config
         self.__cache = BufferCache()
 
         # Validate config.
         if self.config.alibi and self.config.flash_attention:
-            raise OlmoConfigurationError("ALiBi is currently not supported with FlashAttention")
+            raise OLMoConfigurationError("ALiBi is currently not supported with FlashAttention")
 
         if self.config.alibi and self.config.rope:
-            raise OlmoConfigurationError("ALiBi and RoPE are mutually exclusive")
+            raise OLMoConfigurationError("ALiBi and RoPE are mutually exclusive")
 
         if self.config.embedding_size is not None and self.config.embedding_size != self.config.vocab_size:
             if self.config.embedding_size < self.config.vocab_size:
-                raise OlmoConfigurationError("embedding size should be at least as big as vocab size")
+                raise OLMoConfigurationError("embedding size should be at least as big as vocab size")
             elif self.config.embedding_size % 128 != 0:
                 import warnings
 
                 warnings.warn(
                     "Embedding size is not a multiple of 128! This could hurt throughput performance.", UserWarning
                 )
 
         self.activation_checkpointing_strategy: Optional[ActivationCheckpointingStrategy] = None
         self._activation_checkpoint_fn: Callable = activation_checkpoint_function(self.config)
 
         if not (
             0 < self.config.block_group_size <= self.config.n_layers
             and self.config.n_layers % self.config.block_group_size == 0
         ):
-            raise OlmoConfigurationError("n layers must be divisible by block group size")
+            raise OLMoConfigurationError("n layers must be divisible by block group size")
 
-        torch.backends.cuda.enable_flash_sdp(self.config.flash_attention)
+        torch.backends.cuda.enable_flash_sdp(True)
         torch.backends.cuda.enable_mem_efficient_sdp(False)  # this is super slow so make sure torch won't use it
 
         self.transformer = nn.ModuleDict(
             dict(
                 wte=nn.Embedding(
                     config.embedding_size or config.vocab_size, config.d_model, device=config.init_device
                 ),
                 emb_drop=Dropout(config.embedding_dropout),
                 ln_f=LayerNorm.build(config),
             )
         )
 
-        blocks = [OlmoBlock.build(i, config, self.__cache) for i in range(config.n_layers)]
+        blocks = [OLMoBlock.build(i, config, self.__cache) for i in range(config.n_layers)]
         if self.config.block_group_size > 1:
             block_groups = [
-                OlmoBlockGroup(config, i, blocks[i : i + config.block_group_size])
+                OLMoBlockGroup(config, i, blocks[i : i + config.block_group_size])
                 for i in range(0, config.n_layers, config.block_group_size)
             ]
             self.transformer.update({"block_groups": nn.ModuleList(block_groups)})
         else:
             self.transformer.update({"blocks": nn.ModuleList(blocks)})
 
         if not (self.config.alibi or self.config.rope):
@@ -1169,15 +1063,15 @@
         input_embeddings: Optional[torch.FloatTensor] = None,
         attention_mask: Optional[torch.Tensor] = None,
         attention_bias: Optional[torch.Tensor] = None,
         past_key_values: Optional[Sequence[Tuple[torch.Tensor, torch.Tensor]]] = None,
         use_cache: bool = False,
         last_logits_only: bool = False,
         output_hidden_states: Optional[bool] = None,
-    ) -> OlmoOutput:
+    ) -> OLMoOutput:
         """
         :param input_ids: A tensor of shape `(batch_size, seq_len)`.
         :param input_embeddings: A tensor of shape `(batch_size, seq_len, d_model)` with input
             embeddings. When provided, it is treated as the output of the input embedding layer.
         :param attention_mask: A tensor of shape `(batch_size, seq_len)` that indicates
             which input IDs are masked. A `1` value in the mask means that
             the corresponding input ID should *not* be ignored. A `0` means
@@ -1282,36 +1176,23 @@
         if self.config.block_group_size == 1:
             for block_idx, block in enumerate(self.transformer.blocks):
                 if output_hidden_states:
                     # add hidden states
                     all_hidden_states.append(x)
 
                 layer_past = None if past_key_values is None else past_key_values[block_idx]
-                if (
-                    (self.activation_checkpointing_strategy == ActivationCheckpointingStrategy.whole_layer)
-                    or (
-                        self.activation_checkpointing_strategy == ActivationCheckpointingStrategy.one_in_two
-                        and block_idx % 2 == 0
-                    )
-                    or (
-                        self.activation_checkpointing_strategy == ActivationCheckpointingStrategy.one_in_three
-                        and block_idx % 3 == 0
-                    )
-                    or (
-                        self.activation_checkpointing_strategy == ActivationCheckpointingStrategy.one_in_four
-                        and block_idx % 4 == 0
-                    )
-                ):
+                if should_checkpoint_block(self.activation_checkpointing_strategy, block_idx):
                     # shape: (batch_size, seq_len, d_model)
                     x, cache = self._activation_checkpoint_fn(
                         block, x, attention_bias=attention_bias, layer_past=layer_past, use_cache=use_cache
                     )
                 else:
                     # shape: (batch_size, seq_len, d_model)
                     x, cache = block(x, attention_bias=attention_bias, layer_past=layer_past, use_cache=use_cache)
+
                 if attn_key_values is not None:
                     assert cache is not None
                     attn_key_values.append(cache)
         else:
             for group_idx, block_group in enumerate(self.transformer.block_groups):
                 if output_hidden_states:
                     # add hidden states
@@ -1347,15 +1228,15 @@
         if self.config.weight_tying:
             logits = F.linear(x, self.transformer.wte.weight, None)  # type: ignore
         else:
             logits = self.transformer.ff_out(x)  # type: ignore
         if self.config.scale_logits:
             logits.mul_(1 / math.sqrt(self.config.d_model))
 
-        return OlmoOutput(logits=logits, attn_key_values=attn_key_values, hidden_states=tuple(all_hidden_states) if output_hidden_states else None)  # type: ignore[arg-type]
+        return OLMoOutput(logits=logits, attn_key_values=attn_key_values, hidden_states=tuple(all_hidden_states) if output_hidden_states else None)  # type: ignore[arg-type]
 
     def get_fsdp_wrap_policy(self, wrap_strategy: Optional[FSDPWrapStrategy] = None):
         if wrap_strategy is None:
             return None
 
         # The 'recurse' mode for the wrap function does not behave like you'd expect.
         # Even if we return False, it may still recurse because PyTorch does what it wants,
@@ -1367,56 +1248,56 @@
         if hasattr(self.transformer, "ff_out"):
             size_based_module_to_wrap.add(self.transformer.ff_out)
 
         if wrap_strategy == FSDPWrapStrategy.by_block:
 
             def fsdp_wrap_fn(module, recurse: bool = True, nonwrapped_numel: int = 0):
                 del nonwrapped_numel
-                wrap = isinstance(module, OlmoBlock)
+                wrap = isinstance(module, OLMoBlock)
                 if recurse:
                     return True
                 else:
                     return wrap
 
             return fsdp_wrap_fn
         elif wrap_strategy == FSDPWrapStrategy.by_block_and_size:
 
             def fsdp_wrap_fn(module, recurse: bool = True, nonwrapped_numel: int = 0):
                 del nonwrapped_numel
-                wrap = isinstance(module, (OlmoBlock,)) or module in size_based_module_to_wrap
+                wrap = isinstance(module, (OLMoBlock,)) or module in size_based_module_to_wrap
                 if recurse:
                     return True
                 else:
                     return wrap
 
             return fsdp_wrap_fn
         elif wrap_strategy == FSDPWrapStrategy.by_block_group:
             if self.config.block_group_size <= 1:
-                raise OlmoConfigurationError(
+                raise OLMoConfigurationError(
                     "'by_block_group' FSDP wrapping strategy requires block group size greater than 1"
                 )
 
             def fsdp_wrap_fn(module, recurse: bool = True, nonwrapped_numel: int = 0):
                 del nonwrapped_numel
-                wrap = isinstance(module, OlmoBlockGroup)
+                wrap = isinstance(module, OLMoBlockGroup)
                 if recurse:
                     return True
                 else:
                     return wrap
 
             return fsdp_wrap_fn
         elif wrap_strategy == FSDPWrapStrategy.by_block_group_and_size:
             if self.config.block_group_size <= 1:
-                raise OlmoConfigurationError(
+                raise OLMoConfigurationError(
                     "'by_block_group_and_size' FSDP wrapping strategy requires block group size greater than 1"
                 )
 
             def fsdp_wrap_fn(module, recurse: bool = True, nonwrapped_numel: int = 0):
                 del nonwrapped_numel
-                wrap = isinstance(module, (OlmoBlockGroup,)) or module in size_based_module_to_wrap
+                wrap = isinstance(module, (OLMoBlockGroup,)) or module in size_based_module_to_wrap
                 if recurse:
                     return True
                 else:
                     return wrap
 
             return fsdp_wrap_fn
         elif wrap_strategy == FSDPWrapStrategy.size_based:
@@ -1434,15 +1315,15 @@
                 FSDPWrapStrategy.one_in_three: 3,
                 FSDPWrapStrategy.one_in_four: 4,
                 FSDPWrapStrategy.one_in_five: 5,
             }[wrap_strategy]
 
             def fsdp_wrap_fn(module, recurse: bool = True, nonwrapped_numel: int = 0):
                 del nonwrapped_numel
-                wrap = isinstance(module, OlmoBlock) and module.layer_id % c == 0
+                wrap = isinstance(module, OLMoBlock) and module.layer_id % c == 0
                 if recurse:
                     return True
                 else:
                     return wrap
 
             return fsdp_wrap_fn
         else:
@@ -1485,15 +1366,15 @@
         max_steps: int = 10,
         beam_size: int = 1,
         per_node_beam_size: Optional[int] = None,
         sampler: Optional[Sampler] = None,
         min_steps: Optional[int] = None,
         final_sequence_scorer: Optional[FinalSequenceScorer] = None,
         constraints: Optional[List[Constraint]] = None,
-    ) -> OlmoGenerateOutput:
+    ) -> OLMoGenerateOutput:
         """
         Generate token IDs using beam search.
 
         Note that by default ``beam_size`` is set to 1, which is greedy decoding.
 
         :param input_ids: A tensor of shape `(batch_size, seq_len)`.
         :param attention_mask: A optional tensor of shape `(batch_size, seq_len)`, the same
@@ -1595,23 +1476,23 @@
         if attention_mask is not None:
             state["attention_mask"] = attention_mask
         if attention_bias is not None:
             state["attention_bias"] = attention_bias
         with torch.no_grad():
             token_ids, scores = beam_search.search(initial_preds, state, step)
 
-        return OlmoGenerateOutput(
+        return OLMoGenerateOutput(
             token_ids=token_ids,  # type: ignore[arg-type]
             scores=scores,  # type: ignore[arg-type]
         )
 
     @classmethod
     def from_checkpoint(
         cls, checkpoint_dir: PathOrStr, device: str = "cpu", checkpoint_type: Optional[CheckpointType] = None
-    ) -> Olmo:
+    ) -> OLMo:
         """
         Load an OLMo model from a checkpoint.
         """
         from .util import resource_path
 
         # Guess checkpoint type.
         if checkpoint_type is None:
@@ -1626,28 +1507,28 @@
         # Load config.
         config_path = resource_path(checkpoint_dir, "config.yaml")
         model_config = ModelConfig.load(config_path, key="model", validate_paths=False)
 
         if checkpoint_type == CheckpointType.unsharded:
             # Initialize model (always on CPU to start with so we don't run out of GPU memory).
             model_config.init_device = "cpu"
-            model = Olmo(model_config)
+            model = OLMo(model_config)
 
             # Load state dict directly to target device.
             state_dict_path = resource_path(checkpoint_dir, "model.pt")
             state_dict = torch.load(state_dict_path, map_location="cpu")
             model.load_state_dict(model._make_state_dict_compatible(state_dict)[0])
             model = model.to(torch.device(device))
         else:
             from .checkpoint import load_model_state
 
             # Initialize model on target device. In this case the state dict is loaded in-place
             # so it's not necessary to start on CPU if the target device is a GPU.
             model_config.init_device = device
-            model = Olmo(model_config)
+            model = OLMo(model_config)
 
             # Load state dict in place.
             load_model_state(checkpoint_dir, model)
 
         return model.eval()
 
     def _make_state_dict_compatible(
```

### Comparing `ai2-olmo-0.2.5/olmo/optim.py` & `ai2_olmo-0.3.0/olmo/optim.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,18 @@
 
 class Optimizer(OptimizerBase):
     def _clean_param_name(self, name: str) -> str:
         return name.replace("_fsdp_wrapped_module.", "")
 
     @torch.no_grad()
     def clip_grads_and_collect_metrics(
-        self, global_step: int, collect_param_metrics: bool = True
+        self,
+        global_step: int,
+        collect_param_metrics: bool = True,
+        process_group: Optional[dist.ProcessGroup] = None,
     ) -> Dict[str, torch.Tensor]:
         """
         Clips gradients for every group that has the field `max_grad_norm`.
         At the same time collect metrics for each parameter and its gradient.
         """
         device = get_default_device()
 
@@ -65,14 +68,18 @@
         per_param_numel_metrics: List[torch.Tensor] = []
 
         per_param_min_metric_names: List[str] = []
         per_param_max_metric_names: List[str] = []
         per_param_avg_metric_names: List[str] = []
         per_param_norm_metric_names: List[str] = []
 
+        dst_rank = 0
+        if process_group is not None:
+            dst_rank = dist.get_global_rank(process_group, 0)
+
         # Collect metrics locally.
         for group in self.param_groups:
             if is_distributed():
                 # TODO (epwalsh): handle non-sharded params. We don't have any right now but we would
                 # with ReLoRa, for example.
                 assert group.get("sharded", True) is True
 
@@ -140,36 +147,36 @@
         if is_distributed():  # TODO (epwalsh): skip for non-sharded params
             # Reduce metrics across all ranks. Note that we can use a `reduce` for most cases
             # instead of an `all_reduce`, but we need `all_reduce` for norms so that all ranks
             # get the right value for gradient norms so they can clip correctly.
             # Reduce mins.
             if per_param_min_metrics:
                 all_mins = torch.cat(per_param_min_metrics).to(device)
-                dist.reduce(all_mins, 0, op=dist.ReduceOp.MIN)
+                dist.reduce(all_mins, dst_rank, op=dist.ReduceOp.MIN, group=process_group)
                 per_param_min_metrics = all_mins.split(1)
             # Reduce maxs.
             if per_param_max_metrics:
                 all_maxs = torch.cat(per_param_max_metrics).to(device)
-                dist.reduce(all_maxs, 0, op=dist.ReduceOp.MAX)
+                dist.reduce(all_maxs, dst_rank, op=dist.ReduceOp.MAX, group=process_group)
                 per_param_max_metrics = all_maxs.split(1)
             # Reduce sums or just norms.
             all_norms = torch.cat(per_param_norm_metrics).to(device) ** 2.0
             if per_param_sum_metrics and per_param_numel_metrics:
                 all_sums = torch.cat(per_param_sum_metrics).to(device)
                 all_numels = torch.cat(per_param_numel_metrics).to(device)
                 all_sums_norms_numels = torch.cat(
                     [all_sums.unsqueeze(0), all_norms.unsqueeze(0), all_numels.unsqueeze(0)], dim=0
                 )
-                dist.all_reduce(all_sums_norms_numels, op=dist.ReduceOp.SUM)
+                dist.all_reduce(all_sums_norms_numels, op=dist.ReduceOp.SUM, group=process_group)
                 all_sums, all_norms, all_numels = all_sums_norms_numels.split(1)
                 # Get averages.
                 # NOTE: could get infs for non-rank0 processes but that's okay.
                 per_param_avg_metrics = (all_sums / all_numels).squeeze(0).split(1)
             else:
-                dist.all_reduce(all_norms, op=dist.ReduceOp.SUM)
+                dist.all_reduce(all_norms, op=dist.ReduceOp.SUM, group=process_group)
             grad_norm_metric_mask = torch.tensor(
                 [float(is_grad_norm_metric(n)) for n in per_param_norm_metric_names], device=all_norms.device
             )
             total_grad_norm = (all_norms * grad_norm_metric_mask).sum() ** 0.5
             per_param_norm_metrics = (all_norms ** (0.5)).squeeze(0).split(1)
         else:
             total_grad_norm = (
@@ -321,16 +328,18 @@
             # Note that multiplying by the clamped coefficient is meaningless when it is
             # equal to 1, but it avoids the host-device sync that would result from `if clip_coef_clamped < 1`.
             if p.grad is not None:
                 # p.grad could be none for some ranks when using FSDP.
                 p.grad.detach().mul_(clip_coef_clamped.to(p.grad.device, p.grad.dtype))
         return num_grads_clipped
 
-    def get_post_step_metrics(self, module: nn.Module) -> Dict[str, torch.Tensor]:
-        del module
+    def get_post_step_metrics(
+        self, module: nn.Module, process_group: Optional[dist.ProcessGroup] = None
+    ) -> Dict[str, torch.Tensor]:
+        del module, process_group
         return {}
 
     def get_state_for_param(self, param: nn.Parameter) -> Dict[str, Optional[torch.Tensor]]:
         del param
         return {}
 
 
@@ -352,29 +361,35 @@
         super().__init__(params, defaults)
         for group in self.param_groups:
             group["initial_lr"] = group["lr"]
         self._update_total_dot_prod: Optional[torch.Tensor] = None
         self._update_total_norm: Optional[torch.Tensor] = None
         self._signed_update_total_norm: Optional[torch.Tensor] = None
 
-    def get_post_step_metrics(self, module: nn.Module) -> Dict[str, torch.Tensor]:
+    def get_post_step_metrics(
+        self, module: nn.Module, process_group: Optional[dist.ProcessGroup] = None
+    ) -> Dict[str, torch.Tensor]:
         update_total_dot_prod = self._update_total_dot_prod
         update_total_norm = self._update_total_norm
         signed_update_total_norm = self._signed_update_total_norm
         if update_total_dot_prod is None or update_total_norm is None or signed_update_total_norm is None:
             return {}
 
         if is_distributed() and isinstance(module, FullyShardedDataParallel):
             # Reduce total dot prod and norms across all ranks.
             update_total_norm = update_total_norm**2.0
             signed_update_total_norm = signed_update_total_norm**2.0
             # Reduce all together to avoid multiple communication calls.
             all_together = torch.stack([update_total_dot_prod, update_total_norm, signed_update_total_norm])
             # Only need the final result on rank0, since that's where we log from.
-            dist.reduce(all_together, 0)
+            dist.reduce(
+                all_together,
+                0 if process_group is None else dist.get_global_rank(process_group, 0),
+                group=process_group,
+            )
             update_total_dot_prod, update_total_norm, signed_update_total_norm = all_together
             update_total_norm = update_total_norm**0.5
             signed_update_total_norm = signed_update_total_norm**0.5
 
         update_cos_sim = update_total_dot_prod / torch.max(
             update_total_norm * signed_update_total_norm, torch.tensor(1e-8, device=get_default_device())
         )
@@ -445,14 +460,15 @@
 
 @dataclass
 class Scheduler(metaclass=ABCMeta):
     # NOTE: these fields are not given default values because otherwise dataclasses complains
     # about how the scheduler subclasses are defined.
     grad_clip_warmup_steps: Optional[int]
     grad_clip_warmup_factor: Optional[float]
+    warmup_min_lr: Optional[float]
 
     @abstractmethod
     def get_lr(self, initial_lr: float, step: int, max_steps: int) -> float:
         raise NotImplementedError
 
     def _get_max_grad_norm_coeff(
         self, initial_value: Optional[float], step: int, max_steps: int
@@ -476,15 +492,17 @@
 
     def get_max_grad_norm_ratio(
         self, initial_max_grad_norm_ratio: Optional[float], step: int, max_steps: int
     ) -> Optional[float]:
         return self._get_max_grad_norm_coeff(initial_max_grad_norm_ratio, step, max_steps)
 
     def _linear_warmup(self, initial_lr: float, step: int, warmup_steps: int = 2000) -> float:
-        return initial_lr * (0.1 + 0.9 * min(step, warmup_steps) / warmup_steps)
+        warmup_min_lr = self.warmup_min_lr if self.warmup_min_lr is not None else initial_lr * 0.10
+        assert 0 <= warmup_min_lr < initial_lr
+        return warmup_min_lr + (initial_lr - warmup_min_lr) * min(step, warmup_steps) / warmup_steps
 
 
 @dataclass
 class CosWithWarmup(Scheduler):
     warmup_steps: int
     alpha_f: float = 0.1
     t_max: Optional[int] = None
@@ -553,14 +571,15 @@
     def wrap(cls, scheduler: Scheduler, warmup_start: int, warmup_end: int) -> "BoltOnWarmupScheduler":
         return cls(
             grad_clip_warmup_steps=None,
             grad_clip_warmup_factor=None,
             inner=scheduler,
             warmup_start=warmup_start,
             warmup_end=warmup_end,
+            warmup_min_lr=None,
         )
 
     def get_lr(self, initial_lr: float, step: int, max_steps: int) -> float:
         if step < self.warmup_start:
             return 0.0
         if step < self.warmup_end:
             lr_at_intercept = self.inner.get_lr(initial_lr, self.warmup_end, max_steps)
@@ -726,44 +745,49 @@
             grad_clip_warmup_steps=None
             if sched_cfg.grad_clip_warmup_steps is None
             else int(sched_cfg.grad_clip_warmup_steps),
             grad_clip_warmup_factor=sched_cfg.grad_clip_warmup_factor,
             warmup_steps=int(sched_cfg.t_warmup),
             alpha_f=sched_cfg.alpha_f,
             t_max=None if sched_cfg.t_max is None else int(sched_cfg.t_max),
+            warmup_min_lr=sched_cfg.warmup_min_lr,
         )
     elif sched_cfg.name == SchedulerType.linear_with_warmup:
         return LinearWithWarmup(
             grad_clip_warmup_steps=None
             if sched_cfg.grad_clip_warmup_steps is None
             else int(sched_cfg.grad_clip_warmup_steps),
             grad_clip_warmup_factor=sched_cfg.grad_clip_warmup_factor,
             warmup_steps=int(sched_cfg.t_warmup),
             alpha_f=sched_cfg.alpha_f,
             t_max=None if sched_cfg.t_max is None else int(sched_cfg.t_max),
+            warmup_min_lr=sched_cfg.warmup_min_lr,
         )
     elif sched_cfg.name == SchedulerType.inverse_sqrt_with_warmup:
         return InvSqrtWithWarmup(
             grad_clip_warmup_steps=None
             if sched_cfg.grad_clip_warmup_steps is None
             else int(sched_cfg.grad_clip_warmup_steps),
             grad_clip_warmup_factor=sched_cfg.grad_clip_warmup_factor,
             warmup_steps=int(sched_cfg.t_warmup),
+            warmup_min_lr=sched_cfg.warmup_min_lr,
         )
     elif sched_cfg.name == SchedulerType.max_scheduler:
         return MaxScheduler(
             grad_clip_warmup_steps=None
             if sched_cfg.grad_clip_warmup_steps is None
             else int(sched_cfg.grad_clip_warmup_steps),
             grad_clip_warmup_factor=sched_cfg.grad_clip_warmup_factor,
             sched1=build_scheduler(cfg, replace(sched_cfg, name=SchedulerType.cosine_with_warmup)),
             sched2=build_scheduler(cfg, replace(sched_cfg, name=SchedulerType.inverse_sqrt_with_warmup)),
+            warmup_min_lr=sched_cfg.warmup_min_lr,
         )
     elif sched_cfg.name == SchedulerType.constant:
         return ConstantScheduler(
             grad_clip_warmup_steps=None
             if sched_cfg.grad_clip_warmup_steps is None
             else int(sched_cfg.grad_clip_warmup_steps),
             grad_clip_warmup_factor=sched_cfg.grad_clip_warmup_factor,
+            warmup_min_lr=sched_cfg.warmup_min_lr,
         )
     else:
         raise NotImplementedError
```

### Comparing `ai2-olmo-0.2.5/olmo/safetensors_util.py` & `ai2_olmo-0.3.0/olmo/safetensors_util.py`

 * *Files identical despite different names*

### Comparing `ai2-olmo-0.2.5/olmo/tokenizer.py` & `ai2_olmo-0.3.0/olmo/tokenizer.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pathlib import Path
 from typing import List, Optional, Union
 
 from tokenizers import Tokenizer as BaseTokenizer
 
 from .aliases import PathOrStr
 from .config import ModelConfig, TokenizerConfig, TrainConfig, TruncationDirection
-from .exceptions import OlmoConfigurationError
+from .exceptions import OLMoConfigurationError
 
 __all__ = ["Tokenizer"]
 
 
 class Tokenizer:
     """
     A :class:`Tokenizer` is a light-weight wrapper around a HuggingFace :class:`tokenizers.Tokenizer`.
@@ -64,15 +64,15 @@
         else:
             tokenizer = cls.from_pretrained(
                 tokenizer_identifier,
                 eos_token_id=config.model.eos_token_id,
                 pad_token_id=config.model.pad_token_id,
             )
         if config.model.vocab_size != tokenizer.vocab_size:
-            raise OlmoConfigurationError("vocab size mismatch between config and tokenizer")
+            raise OLMoConfigurationError("vocab size mismatch between config and tokenizer")
         return tokenizer
 
     @classmethod
     def from_pretrained(cls, identifier: str, **kwargs) -> Tokenizer:
         """
         Initialize a tokenizer from a pretrained tokenizer on the HuggingFace Hub.
 
@@ -107,21 +107,28 @@
 
         # Load configs.
         config_path = cached_path(os.path.join(checkpoint_dir, "config.yaml"))
         tokenizer_config = TokenizerConfig.load(config_path, key="tokenizer")
         model_config = ModelConfig.load(config_path, key="model")
 
         # Initialize tokenizer and validate vocab size.
-        tokenizer = cls.from_pretrained(
-            tokenizer_config.identifier,
-            eos_token_id=model_config.eos_token_id,
-            pad_token_id=model_config.pad_token_id,
-        )
+        if Path(tokenizer_config.identifier).is_file():
+            tokenizer = cls.from_file(
+                tokenizer_config.identifier,
+                eos_token_id=model_config.eos_token_id,
+                pad_token_id=model_config.pad_token_id,
+            )
+        else:
+            tokenizer = cls.from_pretrained(
+                tokenizer_config.identifier,
+                eos_token_id=model_config.eos_token_id,
+                pad_token_id=model_config.pad_token_id,
+            )
         if model_config.vocab_size != tokenizer.vocab_size:
-            raise OlmoConfigurationError("vocab size mismatch between config and tokenizer")
+            raise OLMoConfigurationError("vocab size mismatch between config and tokenizer")
         return tokenizer
 
     def add_special_tokens(self, input_ids: List[int]) -> List[int]:
         """
         Add special tokens in-place (if not already present) to the given token IDs.
         """
         if not input_ids or input_ids[-1] != self.eos_token_id:
```

### Comparing `ai2-olmo-0.2.5/olmo/torch_util.py` & `ai2_olmo-0.3.0/olmo/torch_util.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import gc
 import os
 from typing import Optional, TypeVar
 
 import torch
 import torch.distributed as dist
 
 T = TypeVar("T")
@@ -126,7 +127,13 @@
         return value_tensor.item()  # type: ignore
     else:
         return value
 
 
 def synchronize_flag(flag: bool, device: torch.device) -> bool:
     return synchronize_value(flag, device)
+
+
+def gc_cuda():
+    gc.collect()
+    if torch.cuda.is_available():
+        torch.cuda.empty_cache()
```

### Comparing `ai2-olmo-0.2.5/olmo/train.py` & `ai2_olmo-0.3.0/olmo/train.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from __future__ import annotations
 
 import cProfile
+import gc
 import logging
 import math
 import os
 import random
 import shutil
 import time
 from collections import deque
 from dataclasses import dataclass, field
 from itertools import islice
 from pathlib import Path
 from pstats import SortKey
-from typing import Any, Deque, Dict, List, Optional, TextIO, Tuple
+from typing import Any, Callable, Deque, Dict, List, Optional, TextIO, Tuple
 
 import numpy as np
 import torch
 import torch.distributed as dist
 import torch.nn.functional as F
 import wandb
 from torch.distributed.fsdp import FullyShardedDataParallel as FSDP
@@ -29,19 +30,20 @@
     SchedulerUnits,
     ShardedCheckpointerType,
     SpeedMonitorConfig,
     TrainConfig,
 )
 from .data import IterableDataset
 from .eval import Evaluator
-from .exceptions import OlmoConfigurationError
-from .model import Olmo
+from .exceptions import OLMoConfigurationError
+from .model import OLMo
 from .optim import Optimizer, Scheduler
 from .torch_util import (
     barrier,
+    gc_cuda,
     get_fs_local_rank,
     get_global_rank,
     get_world_size,
     move_to_device,
     peak_gpu_memory,
     synchronize_flag,
     synchronize_value,
@@ -89,18 +91,37 @@
     optim: torch.optim.Optimizer
 
     def check(self) -> Dict[str, float]:
         lrs = [group["lr"] for group in self.optim.param_groups]
         return {f"optim/learning_rate_group{idx}": lr for idx, lr in enumerate(lrs)}
 
 
+def cross_entropy_loss(
+    logits, labels, ignore_index: int = -100, reduction: str = "mean", compute_z_loss: bool = False
+):
+    loss = F.cross_entropy(logits, labels, ignore_index=ignore_index, reduction=reduction)
+
+    if not compute_z_loss:
+        return loss, None
+
+    z_squared = logits.logsumexp(-1).pow(2)
+    if reduction == "mean":
+        z_squared = (z_squared * (labels != ignore_index)).mean()
+    elif reduction == "sum":
+        z_squared = (z_squared * (labels != ignore_index)).sum()
+
+    z_loss = 1e-4 * z_squared
+
+    return loss, z_loss
+
+
 @dataclass
 class Trainer:
     cfg: TrainConfig
-    model: Olmo
+    model: OLMo
     fsdp_model: FSDP
     optim: Optimizer
     scheduler: Scheduler
     train_loader: DataLoader
     device: torch.device
     evaluators: List[Evaluator]
     epoch: Optional[int] = None
@@ -113,14 +134,61 @@
     checkpoints: List[Path] = field(default_factory=list)
     unsharded_checkpoints: List[Path] = field(default_factory=list)
     ephemeral_checkpoints: List[Path] = field(default_factory=list)
     min_train_loss: float = float("inf")
     cur_train_loss: float = float("inf")
     indices_file: Optional[TextIO] = None
     _start_time: float = 0.0
+    _gc_init_state: bool = True
+    loss_fn: Callable[..., torch.Tensor] = field(default_factory=lambda: cross_entropy_loss)  # type: ignore
+    last_sharded_checkpoint_step: Optional[int] = None
+    last_unsharded_checkpoint_step: Optional[int] = None
+
+    def __post_init__(self):
+        if self.cfg.fused_loss:
+            from flash_attn.ops.triton.cross_entropy import (  # type: ignore
+                cross_entropy_loss,
+            )
+
+            def fused_loss_fn(
+                logits, labels, ignore_index: int = -100, reduction: str = "mean", compute_z_loss: bool = False
+            ):
+                loss, z_loss = cross_entropy_loss(
+                    logits,
+                    labels,
+                    label_smoothing=0.0,
+                    logit_scale=1.0,
+                    lse_square_scale=0.0,
+                    ignored_index=ignore_index,
+                    inplace_backward=False,
+                    process_group=None,
+                )
+
+                mask = labels != ignore_index
+
+                if reduction == "mean":
+                    loss = loss.sum() / mask.sum()
+                elif reduction == "sum":
+                    loss = loss.sum()
+                else:
+                    loss = loss
+
+                if not compute_z_loss:
+                    return loss, None
+
+                if reduction == "mean":
+                    z_loss = z_loss.sum() / mask.sum()
+                elif reduction == "sum":
+                    z_loss = z_loss.sum()
+                else:
+                    z_loss = z_loss
+
+                return loss, z_loss
+
+            self.loss_fn = fused_loss_fn
 
     @property
     def dataset(self) -> IterableDataset:
         assert isinstance(self.train_loader.dataset, IterableDataset)
         return self.train_loader.dataset
 
     @property
@@ -347,15 +415,15 @@
                 checkpoint_dir,
                 self.fsdp_model,
                 self.optim,
                 self.trainer_state_dict(),
                 upload_to=remote_checkpoint_dir,
             )
         except FileExistsError:
-            raise OlmoConfigurationError(
+            raise OLMoConfigurationError(
                 f"Checkpoint for step {self.global_step} already exists, use --save-overwrite to overwrite it"
             )
 
         if link_latest:
             # Link to 'latest'.
             latest_path = Path(self.cfg.save_folder) / f"latest{suffix}"
             latest_path.unlink(missing_ok=True)
@@ -378,19 +446,23 @@
         if remote_checkpoint_dir is not None:
             return remote_checkpoint_dir, checkpoint_dir
         else:
             return checkpoint_dir, None
 
     def save_sharded_checkpoint(self) -> Tuple[PathOrStr, Optional[PathOrStr]]:
         checkpointer = build_sharded_checkpointer(self.cfg)
-        return self._save_checkpoint(checkpointer, CheckpointType.sharded)
+        result = self._save_checkpoint(checkpointer, CheckpointType.sharded)
+        self.last_sharded_checkpoint_step = self.global_step
+        return result
 
     def save_ephemeral_checkpoint(self) -> Tuple[PathOrStr, Optional[PathOrStr]]:
         checkpointer = build_sharded_checkpointer(self.cfg)
-        return self._save_checkpoint(checkpointer, CheckpointType.sharded_ephemeral)
+        result = self._save_checkpoint(checkpointer, CheckpointType.sharded_ephemeral)
+        self.last_sharded_checkpoint_step = self.global_step
+        return result
 
     def _remove_sharded_checkpoint(self, idx: int, checkpoints: List[Path]):
         oldest_checkpoint = checkpoints.pop(idx)
         barrier()
         if get_fs_local_rank() == 0 and oldest_checkpoint.is_dir():
             shutil.rmtree(oldest_checkpoint, ignore_errors=True)
             latest_path = Path(self.cfg.save_folder) / "latest"
@@ -425,15 +497,17 @@
         )
         if load_trainer_state:
             self.load_trainer_state_dict(trainer_state)
         barrier()
 
     def save_unsharded_checkpoint(self) -> Tuple[PathOrStr, Optional[PathOrStr]]:
         checkpointer = FullCheckpointer(self.cfg)
-        return self._save_checkpoint(checkpointer, CheckpointType.unsharded)
+        result = self._save_checkpoint(checkpointer, CheckpointType.unsharded)
+        self.last_unsharded_checkpoint_step = self.global_step
+        return result
 
     def remove_unsharded_checkpoint(self, idx: int = 0):
         barrier()
         oldest_checkpoint = self.unsharded_checkpoints.pop(idx)
         if get_global_rank() == 0 and oldest_checkpoint.is_dir():
             shutil.rmtree(oldest_checkpoint, ignore_errors=True)
             latest_path = Path(self.cfg.save_folder) / "latest-unsharded"
@@ -462,23 +536,27 @@
         if load_trainer_state:
             self.load_trainer_state_dict(trainer_state)
         barrier()
 
     def save_checkpoint(
         self, checkpoint_type: CheckpointType = CheckpointType.sharded
     ) -> Tuple[PathOrStr, Optional[PathOrStr]]:
+        result: Tuple[PathOrStr, Optional[PathOrStr]]
         if checkpoint_type == CheckpointType.sharded:
-            return self.save_sharded_checkpoint()
+            result = self.save_sharded_checkpoint()
         elif checkpoint_type == CheckpointType.unsharded:
-            return self.save_unsharded_checkpoint()
+            result = self.save_unsharded_checkpoint()
         elif checkpoint_type == CheckpointType.sharded_ephemeral:
-            return self.save_ephemeral_checkpoint()
+            result = self.save_ephemeral_checkpoint()
         else:
             raise NotImplementedError(checkpoint_type)
 
+        gc_cuda()
+        return result
+
     def restore_checkpoint(
         self,
         load_path: PathOrStr,
         *,
         checkpoint_type: Optional[CheckpointType] = None,
         local_cache: Optional[PathOrStr] = None,
         load_optimizer_state: bool = True,
@@ -501,14 +579,16 @@
                 load_optimizer_state=load_optimizer_state,
                 load_trainer_state=load_trainer_state,
                 sharded_checkpointer=sharded_checkpointer,
             )
         elif checkpoint_type is not None:
             raise NotImplementedError(checkpoint_type)
 
+        gc_cuda()
+
     def remove_checkpoint(self, idx: int = 0, checkpoint_type: CheckpointType = CheckpointType.sharded):
         if checkpoint_type == CheckpointType.sharded:
             self.remove_sharded_checkpoint(idx=idx)
         elif checkpoint_type == CheckpointType.unsharded:
             self.remove_unsharded_checkpoint(idx=idx)
         elif checkpoint_type == CheckpointType.sharded_ephemeral:
             self.remove_ephemeral_checkpoint(idx=idx)
@@ -525,60 +605,67 @@
         if label_mask is not None:
             labels.masked_fill_(~label_mask, -100)
         if attention_mask is not None:
             labels.masked_fill_(attention_mask == 0.0, -100)
         return labels[..., 1:].contiguous()
 
     def model_forward(
-        self, batch: Dict[str, Any], loss_reduction: str = "mean"
-    ) -> Tuple[torch.Tensor, torch.Tensor]:
+        self, batch: Dict[str, Any], loss_reduction: str = "mean", compute_z_loss: bool = False
+    ) -> Tuple[torch.Tensor, Optional[torch.Tensor], torch.Tensor]:
         # shape: (batch_size, seq_len, vocab_size)
         logits = self.fsdp_model(
             input_ids=batch["input_ids"],
             attention_mask=batch.get("attention_mask"),
             attention_bias=batch.get("attention_bias"),
         ).logits
         logits_for_loss = logits[..., :-1, :].contiguous()
         # shape: (batch_size * seq_len, vocab_size)
         logits_for_loss = logits_for_loss.view(-1, logits_for_loss.size(-1))
         # shape: (batch_size, seq_len)
         labels = self.get_labels(batch)
         # shape: (batch_size * seq_len,)
         labels = labels.view(-1)
-        ce_loss = F.cross_entropy(logits_for_loss, labels, ignore_index=-100, reduction=loss_reduction)
+        ce_loss, z_loss = self.loss_fn(
+            logits_for_loss, labels, ignore_index=-100, reduction=loss_reduction, compute_z_loss=compute_z_loss
+        )
         if loss_reduction == "none":
             # Reshape (batch_size * seq_len,) -> (batch_size, seq_len)
             ce_loss = ce_loss.view(batch["input_ids"].shape[0], -1)
-        return ce_loss, logits
+            if z_loss is not None:
+                z_loss = z_loss.view(batch["input_ids"].shape[0], -1)
+        return ce_loss, z_loss, logits
 
     def train_batch(self, batch: Dict[str, Any]) -> Tuple[torch.Tensor, Optional[torch.Tensor]]:
         # Split into micro-batches.
         micro_batches = self.split_batch(batch)
 
         # In case this helps with memory utilization.
         del batch
 
         ce_batch_loss = torch.tensor(0.0, device=self.device)
         z_batch_loss = None if not self.cfg.softmax_auxiliary_loss else torch.tensor(0.0, device=self.device)
         for micro_batch in micro_batches:
             with torch.autocast("cuda", enabled=True, dtype=self.cfg.autocast_precision):
                 # Run forward pass.
-                ce_loss, logits = self.model_forward(micro_batch)
+                ce_loss, z_loss, logits = self.model_forward(
+                    micro_batch, compute_z_loss=self.cfg.softmax_auxiliary_loss
+                )
                 ce_loss = ce_loss / len(micro_batches)
 
                 # In case this helps with memory utilization.
                 del micro_batch
 
                 # Update overall CE batch loss.
                 ce_batch_loss += ce_loss.detach()
 
                 # Get loss to optimize for.
                 if self.cfg.softmax_auxiliary_loss:
-                    z_squared = logits.logsumexp(-1).pow(2).mean()
-                    z_loss = 1e-4 * z_squared / len(micro_batches)
+                    assert z_loss is not None
+                    assert z_batch_loss is not None
+                    z_loss = z_loss / len(micro_batches)
                     loss = ce_loss + z_loss
 
                     # Update overall Z batch loss.
                     z_batch_loss += z_loss.detach()
                 else:
                     loss = ce_loss
 
@@ -613,15 +700,19 @@
             if z_batch_loss is not None:
                 dist.reduce(z_batch_loss, 0)
                 z_batch_loss.div_(get_world_size())
 
         # Clip gradient norms and collect param/gradient/optim metrics.
         should_log_optim_metrics_this_step = self.should_log_optim_metrics_this_step()
         optim_metrics = self.optim.clip_grads_and_collect_metrics(
-            self.global_step, collect_param_metrics=should_log_optim_metrics_this_step
+            self.global_step,
+            collect_param_metrics=should_log_optim_metrics_this_step,
+            # passing this process group here ensures metrics are reduced correctly when we're using
+            # HYBRID sharding.
+            process_group=self.fsdp_model.process_group,
         )
 
         # Adjust the learning rate.
         for group in self.optim.param_groups:
             # TODO (epwalsh): if we want to enable different LRs or gradient clipping settings per group
             # we should pass `group["initial_lr"]` or `group["initial_max_grad_norm"]` here instead of
             # the corresponding values from `self.cfg`.
@@ -651,23 +742,25 @@
         metrics["train/CrossEntropyLoss"] = self.cur_train_loss
         metrics["train/Perplexity"] = math.exp(self.cur_train_loss)
         if z_batch_loss is not None:
             metrics["train/ZLoss"] = z_batch_loss.item()
 
         # Maybe collect post-step optimizer-specific metrics.
         if should_log_optim_metrics_this_step:
-            optim_metrics = self.optim.get_post_step_metrics(self.fsdp_model)
+            optim_metrics = self.optim.get_post_step_metrics(
+                self.fsdp_model, process_group=self.fsdp_model.process_group
+            )
             for key, value in optim_metrics.items():
                 metrics[f"optim/{key}"] = value.item()
 
         return metrics
 
     def eval_batch(self, batch: Dict[str, Any]) -> Tuple[torch.Tensor, torch.Tensor]:
         with torch.autocast("cuda", enabled=True, dtype=self.cfg.autocast_precision):
-            ce_loss, logits = self.model_forward(batch, loss_reduction="none")
+            ce_loss, _, logits = self.model_forward(batch, loss_reduction="none")
         return ce_loss.mean(dim=-1), logits
 
     def eval_step(self, batch: Dict[str, Any], evaluator: Evaluator) -> None:
         # Move tensors to the right device.
         batch = move_to_device(batch, self.device)
 
         # Run forward pass.
@@ -817,39 +910,57 @@
                 # Next check if early stopping loss criteria is met.
                 should_cancel = True
                 cancel_reason = "early stopping from loss increase"
             elif wandb.run is not None and (api_key := os.environ.get("WANDB_API_KEY")) is not None:
                 # Finally, check if someone canceled the run from W&B by adding the 'cancel' / 'canceled' tag..
                 # We won't see it in the run object. So we have to use the import/export API to check.
                 from requests.exceptions import RequestException
+                from wandb.errors import CommError
 
                 try:
                     api = wandb.Api(api_key=api_key)
                     run = api.run(wandb.run.path)
                     for tag in run.tags or []:
                         if tag.lower() in {"cancel", "canceled", "cancelled"}:
                             should_cancel = True
                             cancel_reason = "Weights & Biases tag"
                             extra_steps = self.cfg.extra_steps_after_cancel
                             break
-                except RequestException:
-                    pass
+                except (RequestException, CommError):
+                    log.info("Failed to check if W&B run is cancelled, continuing run.")
 
         run_canceled = synchronize_flag(should_cancel, self.device)
-        if run_canceled and cancel_reason is not None:
+        if run_canceled:
             extra_steps = synchronize_value(extra_steps, self.device)
-            if extra_steps > 0:
-                log.warning(f"Run canceled due to {cancel_reason}, stopping in {extra_steps} more steps...")
+            if cancel_reason is None:
+                if extra_steps > 0:
+                    log.warning(f"Run canceled, stopping in {extra_steps} more steps...")
+                else:
+                    log.warning("Run canceled")
             else:
-                log.warning(f"Run canceled due to {cancel_reason}")
+                if extra_steps > 0:
+                    log.warning(f"Run canceled due to {cancel_reason}, stopping in {extra_steps} more steps...")
+                else:
+                    log.warning(f"Run canceled due to {cancel_reason}")
 
         return run_canceled, extra_steps
 
     def fit(self):
+        if self.cfg.stop_after is not None:
+            if self.cfg.stop_at is None:
+                self.cfg.stop_at = self.global_step + self.cfg.stop_after
+            else:
+                self.cfg.stop_at = min(self.cfg.stop_at, self.global_step + self.cfg.stop_after)
+
         self._start_time = time.time()
+        self._gc_init_state = gc.isenabled()  # cache if garbage collection is enabled, reset on close.
+
+        # Disable automatic garbage collection, FSDP doesn't work well with it.
+        if self.cfg.gen1_gc_interval is not None:
+            gc.disable()
 
         if self.cfg.load_path is not None and self.global_step > 0 and self.cfg.eval_on_load:
             eval_metrics = self.eval()
             if wandb.run is not None:
                 wandb.log(eval_metrics, step=self.global_step)
 
         # Set model to 'train' mode.
@@ -955,15 +1066,18 @@
                         # System metrics.
                         metrics.update(self.system_metrics())
                         # Learning rate metrics.
                         metrics.update(lr_monitor.check())
 
                     # Log metrics to console.
                     if self.global_step % self.cfg.console_log_interval == 0:
-                        self.log_metrics_to_console(f"[step={self.global_step}/{self.max_steps}]", metrics)
+                        if get_global_rank() == 0:
+                            self.log_metrics_to_console(f"[step={self.global_step}/{self.max_steps}]", metrics)
+                        else:
+                            log.info(f"[step={self.global_step}/{self.max_steps}]")
 
                     # Log metrics to W&B.
                     if (
                         wandb.run is not None
                         and self.cfg.wandb is not None
                         and self.global_step % self.cfg.wandb.log_interval == 0
                     ):
@@ -1044,14 +1158,18 @@
                     first_batch = False
                     if p is not None:
                         p.step()
 
                     if stop_at is not None and self.global_step >= stop_at:
                         break
 
+                    # Run generation 1 garbage collection.
+                    if self.cfg.gen1_gc_interval is not None and self.global_step % self.cfg.gen1_gc_interval == 0:
+                        gc.collect(1)
+
                     # Python Profiler stuff
                     # We do this now, at the bottom of this loop, so we capture the work of getting the next batch.
                     if python_profiler is not None:
                         if self.global_step == 5:
                             python_profiler.enable()
                         elif self.global_step == 8:
                             python_profiler.disable()
@@ -1065,27 +1183,39 @@
                         self.dataset.reshuffle()
                     continue
 
                 break
 
         # Save final checkpoint.
         if save_checkpoints:
-            if self.cfg.save_interval_unsharded is not None:
+            if (
+                self.cfg.save_interval_unsharded is not None
+                and self.last_unsharded_checkpoint_step != self.global_step
+            ):
                 log.info("Saving final unsharded model checkpoint...")
                 checkpoint_path, _ = self.save_checkpoint(CheckpointType.unsharded)
                 log.info(f"Unsharded checkpoint saved to {checkpoint_path}")
-            elif self.cfg.save_num_checkpoints_to_keep != 0:
+            elif (
+                self.cfg.save_num_checkpoints_to_keep != 0
+                and self.last_sharded_checkpoint_step != self.global_step
+            ):
                 log.info("Saving final checkpoint...")
                 checkpoint_path, _ = self.save_checkpoint(CheckpointType.sharded)
                 log.info(f"Checkpoint saved to {checkpoint_path}")
 
     def close(self, exit_code: int = 0) -> None:
+        gc_cuda()
+
         if self.indices_file is not None:
             self.indices_file.flush()
             self.indices_file.close()
+        if self._gc_init_state:
+            gc.enable()
+        else:
+            gc.disable()
         if wandb.run is not None:
             wandb.finish(exit_code=exit_code, quiet=True)
 
     def __enter__(self) -> Trainer:
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb) -> None:
```

### Comparing `ai2-olmo-0.2.5/olmo/util.py` & `ai2_olmo-0.3.0/olmo/util.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,19 +21,19 @@
 from rich.highlighter import NullHighlighter
 from rich.progress import Progress
 from rich.text import Text
 from rich.traceback import Traceback
 
 from .aliases import PathOrStr
 from .exceptions import (
-    OlmoCliError,
-    OlmoEnvironmentError,
-    OlmoError,
-    OlmoNetworkError,
-    OlmoThreadError,
+    OLMoCliError,
+    OLMoEnvironmentError,
+    OLMoError,
+    OLMoNetworkError,
+    OLMoThreadError,
 )
 from .torch_util import get_global_rank, get_local_rank, get_node_rank, is_distributed
 
 try:
     from functools import cache
 except ImportError:
     from functools import lru_cache as cache
@@ -146,17 +146,17 @@
 
 def excepthook(exctype, value, traceback):
     """
     Used to patch `sys.excepthook` in order to log exceptions.
     """
     if issubclass(exctype, KeyboardInterrupt):
         sys.__excepthook__(exctype, value, traceback)
-    elif issubclass(exctype, OlmoCliError):
+    elif issubclass(exctype, OLMoCliError):
         rich.get_console().print(f"[yellow]{value}[/]", highlight=False)
-    elif issubclass(exctype, OlmoError):
+    elif issubclass(exctype, OLMoError):
         rich.get_console().print(Text(f"{exctype.__name__}:", style="red"), value, highlight=False)
     else:
         log.critical("Uncaught %s: %s", exctype.__name__, value, exc_info=(exctype, value, traceback))
 
 
 def install_excepthook():
     sys.excepthook = excepthook
@@ -326,14 +326,16 @@
         from urllib.parse import urlparse
 
         parsed = urlparse(str(path))
         if parsed.scheme == "gs":
             return _gcs_file_size(parsed.netloc, parsed.path.strip("/"))
         elif parsed.scheme in ("s3", "r2"):
             return _s3_file_size(parsed.scheme, parsed.netloc, parsed.path.strip("/"))
+        elif parsed.scheme in ("http", "https"):
+            return _http_file_size(parsed.scheme, parsed.netloc, parsed.path.strip("/"))
         elif parsed.scheme == "file":
             return file_size(str(path).replace("file://", "", 1))
         else:
             raise NotImplementedError(f"file size not implemented for '{parsed.scheme}' files")
     else:
         return os.stat(path).st_size
 
@@ -360,18 +362,22 @@
         parsed = urlparse(str(source))
         if parsed.scheme == "gs":
             return _gcs_get_bytes_range(parsed.netloc, parsed.path.strip("/"), bytes_start, num_bytes)
         elif parsed.scheme in ("s3", "r2"):
             return _s3_get_bytes_range(
                 parsed.scheme, parsed.netloc, parsed.path.strip("/"), bytes_start, num_bytes
             )
+        elif parsed.scheme in ("http", "https"):
+            return _http_get_bytes_range(
+                parsed.scheme, parsed.netloc, parsed.path.strip("/"), bytes_start, num_bytes
+            )
         elif parsed.scheme == "file":
             return get_bytes_range(str(source).replace("file://", "", 1), bytes_start, num_bytes)
         else:
-            raise NotImplementedError(f"file size not implemented for '{parsed.scheme}' files")
+            raise NotImplementedError(f"get bytes range not implemented for '{parsed.scheme}' files")
     else:
         with open(source, "rb") as f:
             f.seek(bytes_start)
             return f.read(num_bytes)
 
 
 def find_latest_checkpoint(dir: PathOrStr) -> Optional[PathOrStr]:
@@ -446,30 +452,30 @@
 def _get_s3_profile_name(scheme: str) -> Optional[str]:
     if scheme == "s3":
         # For backwards compatibility, we assume S3 uses the default profile if S3_PROFILE is not set.
         return os.environ.get("S3_PROFILE")
     if scheme == "r2":
         profile_name = os.environ.get("R2_PROFILE")
         if profile_name is None:
-            raise OlmoEnvironmentError(
+            raise OLMoEnvironmentError(
                 "R2 profile name is not set. Did you forget to set the 'R2_PROFILE' env var?"
             )
 
         return profile_name
 
     raise NotImplementedError(f"Cannot get profile name for scheme {scheme}")
 
 
 def _get_s3_endpoint_url(scheme: str) -> Optional[str]:
     if scheme == "s3":
         return None
     if scheme == "r2":
         r2_endpoint_url = os.environ.get("R2_ENDPOINT_URL")
         if r2_endpoint_url is None:
-            raise OlmoEnvironmentError(
+            raise OLMoEnvironmentError(
                 "R2 endpoint url is not set. Did you forget to set the 'R2_ENDPOINT_URL' env var?"
             )
 
         return r2_endpoint_url
 
     raise NotImplementedError(f"Cannot get endpoint url for scheme {scheme}")
 
@@ -497,47 +503,47 @@
         for attempt in range(1, max_attempts + 1):
             try:
                 _get_s3_client(scheme).head_object(Bucket=bucket_name, Key=key)
                 raise FileExistsError(
                     f"s3://{bucket_name}/{key} already exists. Use save_overwrite to overwrite it."
                 )
             except boto_exceptions.ClientError as e:
-                if int(e.response["Error"]["Code"]) == 404:
+                if e.response["ResponseMetadata"]["HTTPStatusCode"] == 404:
                     err = None
                     break
                 err = e
 
             if attempt < max_attempts:
                 log.warning("%s failed attempt %d with retriable error: %s", _s3_upload.__name__, attempt, err)
                 _wait_before_retry(attempt)
 
         if err is not None:
-            raise OlmoNetworkError("Failed to check object existence during s3 upload") from err
+            raise OLMoNetworkError(f"Failed to check object existence during {scheme} upload") from err
 
     try:
         _get_s3_client(scheme).upload_file(source, bucket_name, key)
     except boto_exceptions.ClientError as e:
-        raise OlmoNetworkError("Failed to upload to s3") from e
+        raise OLMoNetworkError(f"Failed to upload to {scheme}") from e
 
 
 def _s3_file_size(scheme: str, bucket_name: str, key: str, max_attempts: int = 3) -> int:
     err: Optional[Exception] = None
     for attempt in range(1, max_attempts + 1):
         try:
             return _get_s3_client(scheme).head_object(Bucket=bucket_name, Key=key)["ContentLength"]
         except boto_exceptions.ClientError as e:
-            if int(e.response["Error"]["Code"]) == 404:
+            if e.response["ResponseMetadata"]["HTTPStatusCode"] == 404:
                 raise FileNotFoundError(f"s3://{bucket_name}/{key}") from e
             err = e
 
         if attempt < max_attempts:
             log.warning("%s failed attempt %d with retriable error: %s", _s3_file_size.__name__, attempt, err)
             _wait_before_retry(attempt)
 
-    raise OlmoNetworkError("Failed to get s3 file size") from err
+    raise OLMoNetworkError(f"Failed to get {scheme} file size") from err
 
 
 def _s3_get_bytes_range(
     scheme: str, bucket_name: str, key: str, bytes_start: int, num_bytes: int, max_attempts: int = 3
 ) -> bytes:
     err: Optional[Exception] = None
     for attempt in range(1, max_attempts + 1):
@@ -546,16 +552,16 @@
                 _get_s3_client(scheme)
                 .get_object(
                     Bucket=bucket_name, Key=key, Range=f"bytes={bytes_start}-{bytes_start + num_bytes - 1}"
                 )["Body"]
                 .read()
             )
         except boto_exceptions.ClientError as e:
-            if int(e.response["Error"]["Code"]) == 404:
-                raise FileNotFoundError(f"s3://{bucket_name}/{key}") from e
+            if e.response["ResponseMetadata"]["HTTPStatusCode"] == 404:
+                raise FileNotFoundError(f"{scheme}://{bucket_name}/{key}") from e
             err = e
         except (boto_exceptions.HTTPClientError, boto_exceptions.ConnectionError) as e:
             # ResponseStreamingError (subclass of HTTPClientError) can happen as
             # a result of a failed read from the stream (http.client.IncompleteRead).
             # Retrying can help in this case.
             err = e
 
@@ -568,15 +574,15 @@
     # When torch's DataLoader intercepts exceptions, it may try to re-raise them
     # by recalling their constructor with a single message arg. Torch has some
     # logic to deal with the absence of a single-parameter constructor, but it
     # doesn't gracefully handle other possible failures in calling such a constructor
     # This can cause an irrelevant exception (e.g. KeyError: 'error'), resulting
     # in us losing the true exception info. To avoid this, we change the exception
     # to a type that has a single-parameter constructor.
-    raise OlmoNetworkError("Failed to get bytes range from s3") from err
+    raise OLMoNetworkError(f"Failed to get bytes range from {scheme}") from err
 
 
 def _s3_find_latest_checkpoint(scheme: str, bucket_name: str, prefix: str) -> Optional[str]:
     if not prefix.endswith("/"):
         prefix = f"{prefix}/"
     response = _get_s3_client(scheme).list_objects(Bucket=bucket_name, Prefix=prefix, Delimiter="/")
     assert not response["IsTruncated"]  # need to handle this if it happens
@@ -587,21 +593,47 @@
         checkpoint_name = os.path.split(prefix)[-1]
         if not checkpoint_name.startswith("step"):
             continue
         try:
             step = int(checkpoint_name.replace("step", "").replace("-unsharded", ""))
         except ValueError:
             continue
+        # Make sure the checkpoint dir contains a config, otherwise the checkpoint is incomplete
+        # (upload might have have failed part way through).
+        try:
+            _s3_file_size(scheme, bucket_name, f"{prefix}/config.yaml")
+        except FileNotFoundError:
+            continue
         # We prioritize sharded checkpoints over unsharded ones.
         if step > latest_step or (step == latest_step and not checkpoint_name.endswith("-unsharded")):
             latest_step = step
-            latest_checkpoint = f"s3://ai2-llm/{prefix}"
+            latest_checkpoint = f"{scheme}://ai2-llm/{prefix}"
     return latest_checkpoint
 
 
+def _http_file_size(scheme: str, host_name: str, path: str) -> int:
+    import requests
+
+    response = requests.head(f"{scheme}://{host_name}/{path}", allow_redirects=True)
+    return int(response.headers.get("content-length"))
+
+
+def _http_get_bytes_range(scheme: str, host_name: str, path: str, bytes_start: int, num_bytes: int) -> bytes:
+    import requests
+
+    response = requests.get(
+        f"{scheme}://{host_name}/{path}", headers={"Range": f"bytes={bytes_start}-{bytes_start+num_bytes-1}"}
+    )
+    result = response.content
+    assert (
+        len(result) == num_bytes
+    ), f"expected {num_bytes} bytes, got {len(result)}"  # Some web servers silently ignore range requests and send everything
+    return result
+
+
 def default_thread_count() -> int:
     return int(os.environ.get("OLMO_NUM_THREADS") or min(32, (os.cpu_count() or 1) + 4))
 
 
 def pass_through_fn(fn, *args, **kwargs):
     return fn(*args, **kwargs)
 
@@ -622,15 +654,15 @@
 
     thread_name = thread_name or repr(g)
     thread = Thread(name=thread_name, target=fill_queue, daemon=True)
     thread.start()
 
     for x in iter(q.get, sentinel):
         if isinstance(x, Exception):
-            raise OlmoThreadError(f"generator thread {thread_name} failed") from x
+            raise OLMoThreadError(f"generator thread {thread_name} failed") from x
         else:
             yield x
 
 
 def roundrobin(*iterables):
     """
     Call the given iterables in a round-robin fashion. For example:
```

### Comparing `ai2-olmo-0.2.5/pyproject.toml` & `ai2_olmo-0.3.0/pyproject.toml`

 * *Files identical despite different names*


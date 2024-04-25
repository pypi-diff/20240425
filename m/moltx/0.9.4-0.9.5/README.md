# Comparing `tmp/moltx-0.9.4.tar.gz` & `tmp/moltx-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moltx-0.9.4.tar", last modified: Mon Apr 22 13:30:08 2024, max compression
+gzip compressed data, was "moltx-0.9.5.tar", last modified: Thu Apr 25 08:22:17 2024, max compression
```

## Comparing `moltx-0.9.4.tar` & `moltx-0.9.5.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 13:30:08.375759 moltx-0.9.4/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-22 13:29:59.000000 moltx-0.9.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5884 2024-04-22 13:30:08.375759 moltx-0.9.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5273 2024-04-22 13:29:59.000000 moltx-0.9.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 13:30:08.371759 moltx-0.9.4/moltx/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 13:29:59.000000 moltx-0.9.4/moltx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-22 13:29:59.000000 moltx-0.9.4/moltx/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 13:30:08.375759 moltx-0.9.4/moltx/data/
--rw-r--r--   0 runner    (1001) docker     (127)    11088 2024-04-22 13:29:59.000000 moltx-0.9.4/moltx/data/spe_safe.txt
--rw-r--r--   0 runner    (1001) docker     (127)    27879 2024-04-22 13:29:59.000000 moltx-0.9.4/moltx/data/spe_smiles.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5372 2024-04-22 13:29:59.000000 moltx-0.9.4/moltx/data/tks_safe.json
--rw-r--r--   0 runner    (1001) docker     (127)    36304 2024-04-22 13:29:59.000000 moltx-0.9.4/moltx/data/tks_smiles.json
--rw-r--r--   0 runner    (1001) docker     (127)     3377 2024-04-22 13:29:59.000000 moltx-0.9.4/moltx/datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-04-22 13:29:59.000000 moltx-0.9.4/moltx/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     4288 2024-04-22 13:29:59.000000 moltx-0.9.4/moltx/nets.py
--rw-r--r--   0 runner    (1001) docker     (127)     7359 2024-04-22 13:29:59.000000 moltx-0.9.4/moltx/pipelines.py
--rw-r--r--   0 runner    (1001) docker     (127)     8000 2024-04-22 13:29:59.000000 moltx-0.9.4/moltx/tokenizers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 13:30:08.375759 moltx-0.9.4/moltx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5884 2024-04-22 13:30:08.000000 moltx-0.9.4/moltx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-04-22 13:30:08.000000 moltx-0.9.4/moltx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 13:30:08.000000 moltx-0.9.4/moltx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-22 13:30:08.000000 moltx-0.9.4/moltx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-22 13:30:08.000000 moltx-0.9.4/moltx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-22 13:29:59.000000 moltx-0.9.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-04-22 13:30:08.375759 moltx-0.9.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 13:29:59.000000 moltx-0.9.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 13:30:08.375759 moltx-0.9.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-04-22 13:29:59.000000 moltx-0.9.4/tests/test_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2378 2024-04-22 13:29:59.000000 moltx-0.9.4/tests/test_nets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2295 2024-04-22 13:29:59.000000 moltx-0.9.4/tests/test_pipelines.py
--rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-04-22 13:29:59.000000 moltx-0.9.4/tests/test_tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:22:17.423490 moltx-0.9.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-25 08:22:10.000000 moltx-0.9.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5704 2024-04-25 08:22:17.423490 moltx-0.9.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5093 2024-04-25 08:22:10.000000 moltx-0.9.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:22:17.419490 moltx-0.9.5/moltx/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 08:22:10.000000 moltx-0.9.5/moltx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-25 08:22:10.000000 moltx-0.9.5/moltx/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:22:17.419490 moltx-0.9.5/moltx/data/
+-rw-r--r--   0 runner    (1001) docker     (127)    11088 2024-04-25 08:22:10.000000 moltx-0.9.5/moltx/data/spe_safe.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    27879 2024-04-25 08:22:10.000000 moltx-0.9.5/moltx/data/spe_smiles.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5372 2024-04-25 08:22:10.000000 moltx-0.9.5/moltx/data/tks_safe.json
+-rw-r--r--   0 runner    (1001) docker     (127)    36304 2024-04-25 08:22:10.000000 moltx-0.9.5/moltx/data/tks_smiles.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3377 2024-04-25 08:22:10.000000 moltx-0.9.5/moltx/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-04-25 08:22:10.000000 moltx-0.9.5/moltx/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4506 2024-04-25 08:22:10.000000 moltx-0.9.5/moltx/nets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7442 2024-04-25 08:22:10.000000 moltx-0.9.5/moltx/pipelines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8000 2024-04-25 08:22:10.000000 moltx-0.9.5/moltx/tokenizers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:22:17.423490 moltx-0.9.5/moltx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5704 2024-04-25 08:22:17.000000 moltx-0.9.5/moltx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-04-25 08:22:17.000000 moltx-0.9.5/moltx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 08:22:17.000000 moltx-0.9.5/moltx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-25 08:22:17.000000 moltx-0.9.5/moltx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-25 08:22:17.000000 moltx-0.9.5/moltx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-25 08:22:10.000000 moltx-0.9.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-04-25 08:22:17.423490 moltx-0.9.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 08:22:10.000000 moltx-0.9.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:22:17.423490 moltx-0.9.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-04-25 08:22:10.000000 moltx-0.9.5/tests/test_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3113 2024-04-25 08:22:10.000000 moltx-0.9.5/tests/test_nets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-04-25 08:22:10.000000 moltx-0.9.5/tests/test_pipelines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-04-25 08:22:10.000000 moltx-0.9.5/tests/test_tokenizer.py
```

### Comparing `moltx-0.9.4/LICENSE` & `moltx-0.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `moltx-0.9.4/README.md` & `moltx-0.9.5/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,27 @@
+Metadata-Version: 2.1
+Name: moltx
+Version: 0.9.5
+Summary: Molcule Transformer X Model
+Author: Michael Ding
+Author-email: yandy.ding@gmail.com
+License: Apache-2.0
+Keywords: molcule,AI,deep learning,transformer
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Science/Research
+Classifier: Operating System :: POSIX
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Development Status :: 4 - Beta
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: rdkit~=2023.9.1
+Requires-Dist: torch~=2.2.0
+
 # MolTx
 
 [![CI](https://github.com/js-ish/MolTx/actions/workflows/test.yml/badge.svg)](https://github.com/js-ish/MolTx/actions/workflows/test.yml?query=branch%3Amain)
 [![Coverage Status](https://coveralls.io/repos/github/js-ish/MolTx/badge.svg?branch=main)](https://coveralls.io/github/js-ish/MolTx?branch=main)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/moltx)
 
 ## Installation
@@ -27,23 +47,17 @@
 
 # train
 import torch.nn as nn
 from torch.optim import Adam
 from moltx import nets, models
 
 ## use custom config
-conf = nets.AbsPosEncoderDecoderConfig(token_size=512, max_len=256)
+conf = models.AdaMR.CONFIG_LARGE # or models.AdaMR.CONFIG_BASE
 model = models.AdaMR(conf)
 
-## or use default large config
-model = models.AdaMR()
-
-## or use base config
-model = models.AdaMR(models.AdaMR.CONFIG_BASE)
-
 crt = nn.CrossEntropyLoss(ignore_index=0)
 optim = Adam(model.parameters(), lr=0.1)
 
 optim.zero_grad()
 pred = model(src, tgt)
 loss = crt(pred.view(-1, pred.size(-1)), out.view(-1))
 loss.backward()
@@ -64,15 +78,15 @@
 
 ds = datasets.AdaMRClassifier(tokenizer=tk, device=torch.device('cpu'))
 smiles = ["c1cccc1c", "CC[N+](C)(C)Cc1ccccc1Br"]
 labels = [0, 1]
 src, tgt, out = ds(smiles, labels)
 
 from moltx import nets, models
-pretrained_conf = nets.AbsPosEncoderDecoderConfig(token_size=512, max_len=256, ...)
+pretrained_conf = models.AdaMR.CONFIG_LARGE # or models.AdaMR.CONFIG_BASE
 model = models.AdaMRClassifier(num_classes=2, conf=pretrained_conf)
 model.load_ckpt('/path/to/adamr.ckpt')
 crt = nn.CrossEntropyLoss()
 optim = Adam(model.parameters(), lr=0.1)
 
 optim.zero_grad()
 pred = model(src, tgt)
@@ -139,46 +153,46 @@
 ### Inference
 
 ```python
 from moltx import nets, models, pipelines, tokenizers
 tk = tokenizers.MoltxTokenizer.from_jsonfile(spe_codes=True, token_size=512)
 
 # AdaMR
-conf = nets.AbsPosEncoderDecoderConfig(...) # use config matching ckpt
+conf = models.AdaMR.CONFIG_LARGE # or models.AdaMR.CONFIG_BASE
 model = models.AdaMR(conf)
 model.load_ckpt('/path/to/adamr.ckpt')
 pipeline = pipelines.AdaMR(tk, model)
 pipeline("C=CC=CC=C")
 # {"smiles": ["c1ccccc1"], probabilities: [0.9]}
 
 # Classifier
-conf = nets.AbsPosEncoderDecoderConfig(...) # use config matching ckpt
+conf = models.AdaMR.CONFIG_LARGE # or models.AdaMR.CONFIG_BASE
 model = models.AdaMRClassifier(2, conf)
 model.load_ckpt('/path/to/classifier.ckpt')
 pipeline = pipelines.AdaMRClassifier(tk, model)
 pipeline("C=CC=CC=C")
 # {"label": [1], "probability": [0.67]}
 
 # Regression
-conf = nets.AbsPosEncoderDecoderConfig(...) # use config matching ckpt
+conf = models.AdaMR.CONFIG_LARGE # or models.AdaMR.CONFIG_BASE
 model = models.AdaMRRegression(2, conf)
 model.load_ckpt('/path/to/regression.ckpt')
 pipeline = pipelines.AdaMRRegression(tk, model)
 pipeline("C=CC=CC=C")
 # {"value": [0.467], "probability": [0.67]}
 
 # DistGeneration
-conf = nets.AbsPosEncoderDecoderConfig(...) # use config matching ckpt
+conf = models.AdaMR.CONFIG_LARGE # or models.AdaMR.CONFIG_BASE
 model = models.AdaMRDistGeneration(conf)
 model.load_ckpt('/path/to/distgen.ckpt')
 pipeline = pipelines.AdaMRDistGeneration(tk, model)
 pipeline(k=2)
 # {"smiles": ["c1ccccc1", "...."], probabilities: [0.9, 0.1]}
 
 # GoalGeneration
-conf = nets.AbsPosEncoderDecoderConfig(...) # use config matching ckpt
+conf = models.AdaMR.CONFIG_LARGE # or models.AdaMR.CONFIG_BASE
 model = models.AdaMRGoalGeneration(conf)
 model.load_ckpt('/path/to/goalgen.ckpt')
 pipeline = pipelines.AdaMRGoalGeneration(tk, model)
 pipeline(0.48, k=2)
 # {"smiles": ["c1ccccc1", "...."], probabilities: [0.9, 0.1]}
 ```
```

### Comparing `moltx-0.9.4/moltx/data/spe_safe.txt` & `moltx-0.9.5/moltx/data/spe_safe.txt`

 * *Files identical despite different names*

### Comparing `moltx-0.9.4/moltx/data/spe_smiles.txt` & `moltx-0.9.5/moltx/data/spe_smiles.txt`

 * *Files identical despite different names*

### Comparing `moltx-0.9.4/moltx/data/tks_safe.json` & `moltx-0.9.5/moltx/data/tks_safe.json`

 * *Files identical despite different names*

### Comparing `moltx-0.9.4/moltx/data/tks_smiles.json` & `moltx-0.9.5/moltx/data/tks_smiles.json`

 * *Files identical despite different names*

### Comparing `moltx-0.9.4/moltx/datasets.py` & `moltx-0.9.5/moltx/datasets.py`

 * *Files identical despite different names*

### Comparing `moltx-0.9.4/moltx/models.py` & `moltx-0.9.5/moltx/models.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,24 +9,26 @@
         token_size=512,  # max(spe_merge) = 240
         max_len=512,
         d_model=768,
         nhead=12,
         num_encoder_layers=12,
         num_decoder_layers=12,
         dropout=0.1,
+        dtype=torch.bfloat16
     )
 
     CONFIG_BASE = nets.AbsPosEncoderDecoderConfig(
         token_size=512,  # max(spe_merge) = 240
         max_len=512,
         d_model=768,
         nhead=8,
         num_encoder_layers=6,
         num_decoder_layers=6,
         dropout=0.1,
+        dtype=torch.float32
     )
 
     def __init__(self, conf: nets.AbsPosEncoderDecoderConfig = CONFIG_LARGE) -> None:
         super().__init__(conf=conf)
 
     def forward(self, src: torch.Tensor, tgt: torch.Tensor) -> torch.Tensor:
         return super().forward_generation(src, tgt)
@@ -34,18 +36,18 @@
 
 class AdaMRClassifier(AdaMR):
     def __init__(self, num_classes: int, conf: nets.AbsPosEncoderDecoderConfig) -> None:
         super().__init__(conf=conf)
         d_hidden = conf.d_model // 2
         self.fc = nn.Sequential(
             nn.Dropout(conf.dropout),
-            nn.Linear(conf.d_model, d_hidden),
+            nn.Linear(conf.d_model, d_hidden, dtype=conf.dtype),
             nn.Tanh(),
             nn.Dropout(conf.dropout),
-            nn.Linear(d_hidden, num_classes)
+            nn.Linear(d_hidden, num_classes, dtype=conf.dtype)
         )
 
     def load_ckpt(self, ckpt_files: typing.Sequence[str]) -> None:
         self.load_state_dict(torch.load(
             ckpt_files[0], map_location=torch.device('cpu')), strict=False)
 
     def forward(self, src: torch.Tensor, tgt: torch.Tensor) -> torch.Tensor:
@@ -55,18 +57,18 @@
 
 class AdaMRRegression(AdaMR):
     def __init__(self, conf: nets.AbsPosEncoderDecoderConfig) -> None:
         super().__init__(conf=conf)
         d_hidden = conf.d_model // 2
         self.fc = nn.Sequential(
             nn.Dropout(conf.dropout),
-            nn.Linear(conf.d_model, d_hidden),
+            nn.Linear(conf.d_model, d_hidden, dtype=conf.dtype),
             nn.Tanh(),
             nn.Dropout(conf.dropout),
-            nn.Linear(d_hidden, 1)
+            nn.Linear(d_hidden, 1, dtype=conf.dtype)
         )
 
     def load_ckpt(self, *ckpt_files: str) -> None:
         self.load_state_dict(torch.load(
             ckpt_files[0], map_location=torch.device('cpu')), strict=False)
 
     def forward(self, src: torch.Tensor, tgt: torch.Tensor) -> torch.Tensor:
```

### Comparing `moltx-0.9.4/moltx/nets.py` & `moltx-0.9.5/moltx/nets.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import torch
 import torch.nn as nn
 from dataclasses import dataclass
 
 
 class AbsPosEmbedding(nn.Module):
-    def __init__(self, token_size: int, max_len: int, d_model: int, dropout: float = 0.1) -> None:
+    def __init__(self, token_size: int, max_len: int, d_model: int, dropout: float = 0.1, dtype: torch.dtype = torch.float32) -> None:
         super().__init__()
-        self.token_embedding = nn.Embedding(token_size, d_model, padding_idx=0)
-        self.pos_embedding = nn.Embedding(max_len + 1, d_model, padding_idx=0)
+        self.token_embedding = nn.Embedding(token_size, d_model, padding_idx=0, dtype=dtype)
+        self.pos_embedding = nn.Embedding(max_len + 1, d_model, padding_idx=0, dtype=dtype)
         self.dropout = nn.Dropout(dropout)
 
     def forward(self, x: torch.Tensor) -> torch.Tensor:
         xlen = x.size(-1)
         mask = (x > 0).long()
         position = torch.arange(1, xlen + 1).to(x.device)
         position = position * mask
@@ -25,26 +25,27 @@
     token_size: int
     max_len: int = 512
     d_model: int = 768
     nhead: int = 8
     num_encoder_layers: int = 6
     num_decoder_layers: int = 6
     dropout: float = 0.1
+    dtype: torch.dtype = None
 
 
 class AbsPosEncoderDecoder(nn.Module):
     def __init__(self, conf: AbsPosEncoderDecoderConfig) -> None:
         super().__init__()
         self.conf = conf
         self.embedding = AbsPosEmbedding(
-            conf.token_size, conf.max_len, conf.d_model, conf.dropout)
+            conf.token_size, conf.max_len, conf.d_model, conf.dropout, conf.dtype)
         self.transformer = nn.Transformer(
-            conf.d_model, conf.nhead, conf.num_encoder_layers, conf.num_decoder_layers, dropout=conf.dropout, activation='gelu', batch_first=True)
+            conf.d_model, conf.nhead, conf.num_encoder_layers, conf.num_decoder_layers, dropout=conf.dropout, activation='gelu', batch_first=True, dtype=conf.dtype)
         self.token_output = nn.Linear(
-            conf.d_model, conf.token_size, bias=False)
+            conf.d_model, conf.token_size, bias=False, dtype=conf.dtype)
 
     def load_ckpt(self, *ckpt_files: str) -> None:
         self.load_state_dict(torch.load(
             ckpt_files[0], map_location=torch.device('cpu')))
 
     def forward_(self, src: torch.Tensor, tgt: torch.Tensor) -> torch.Tensor:
         mask = nn.Transformer.generate_square_subsequent_mask(
@@ -69,28 +70,29 @@
 class AbsPosEncoderCausalConfig:
     token_size: int
     max_len: int = 256
     d_model: int = 768
     nhead: int = 8
     num_layers: int = 12
     dropout: float = 0.1
+    dtype: torch.dtype = None
 
 
 class AbsPosEncoderCausal(nn.Module):
     def __init__(self, conf: AbsPosEncoderCausalConfig) -> None:
         super().__init__()
         self.conf = conf
         self.embedding = AbsPosEmbedding(
-            conf.token_size, conf.max_len, conf.d_model, conf.dropout)
+            conf.token_size, conf.max_len, conf.d_model, conf.dropout, conf.dtype)
         layer = nn.TransformerEncoderLayer(
-            conf.d_model, conf.nhead, dropout=conf.dropout, batch_first=True, activation='gelu')
+            conf.d_model, conf.nhead, dropout=conf.dropout, batch_first=True, activation='gelu', dtype=conf.dtype)
         self.transformer = nn.TransformerEncoder(
             layer, conf.num_layers, norm=nn.LayerNorm(conf.d_model))
         self.token_output = nn.Linear(
-            conf.d_model, conf.token_size, bias=False)
+            conf.d_model, conf.token_size, bias=False, dtype=conf.dtype)
 
     def load_ckpt(self, *ckpt_files: str) -> None:
         self.load_state_dict(torch.load(
             ckpt_files[0], map_location=torch.device('cpu')))
 
     def forward_(self, x: torch.Tensor) -> torch.Tensor:
         mask = nn.Transformer.generate_square_subsequent_mask(
```

### Comparing `moltx-0.9.4/moltx/pipelines.py` & `moltx-0.9.5/moltx/pipelines.py`

 * *Files 1% similar despite different names*

```diff
@@ -120,17 +120,19 @@
         for _ in range(k):
             smi, prob = self._greedy_search(src=src, tgt=tgt)
             smiles.append(smi)
             probs.append(prob)
         return smiles, probs
 
     def _call_beam(self, src: torch.Tensor, tgt: torch.Tensor, k: int) -> typing.Mapping:
-        src = src.unsqueeze(0).repeat(k, 1)
-        tgt = tgt.unsqueeze(0).repeat(k, 1)
-        return self._beam_search(src=src, tgt=tgt)
+        beam_k = max(k, 3)
+        src = src.unsqueeze(0).repeat(beam_k, 1)
+        tgt = tgt.unsqueeze(0).repeat(beam_k, 1)
+        smiles, probs = self._beam_search(src=src, tgt=tgt)
+        return smiles[:k], probs[:k]
 
 
 class AdaMRClassifier(AdaMR):
     def _model_args(self, smiles: str) -> typing.Tuple[torch.Tensor]:
         return super()._model_args(smiles, f"{smiles}{self.tokenizer.EOS}")
 
     def __call__(self, smiles: str) -> typing.Mapping:
```

### Comparing `moltx-0.9.4/moltx/tokenizers.py` & `moltx-0.9.5/moltx/tokenizers.py`

 * *Files identical despite different names*

### Comparing `moltx-0.9.4/moltx.egg-info/SOURCES.txt` & `moltx-0.9.5/moltx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `moltx-0.9.4/setup.cfg` & `moltx-0.9.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `moltx-0.9.4/tests/test_datasets.py` & `moltx-0.9.5/tests/test_datasets.py`

 * *Files identical despite different names*

### Comparing `moltx-0.9.4/tests/test_nets.py` & `moltx-0.9.5/tests/test_nets.py`

 * *Files 5% similar despite different names*

```diff
@@ -45,14 +45,25 @@
     assert out.shape == (32, 8)
     feat = model.forward_feature(tokens, tokens)
     assert feat.shape == (8,)
     assert feat.eq(out[-1]).all()
     gen = model.forward_generation(tokens, tokens)
     assert gen.shape == (32, 16)
 
+    conf = nets.AbsPosEncoderDecoderConfig(
+        token_size=16, max_len=32, d_model=8, nhead=2,
+        num_encoder_layers=2, num_decoder_layers=2, dtype=torch.bfloat16)
+    model = nets.AbsPosEncoderDecoder(conf=conf)
+    model.eval()
+    model.requires_grad_(False)
+    
+    batch = torch.randint(1, 16, (2, 32))
+    out = model.forward_(batch, batch)
+    assert out.shape == (2, 32, 8)
+
 
 def test_AbsPosEncoderCausal():
     conf = nets.AbsPosEncoderCausalConfig(
         token_size=16, max_len=32, d_model=8, nhead=2, num_layers=2)
     model = nets.AbsPosEncoderCausal(conf=conf)
     model.eval()
     model.requires_grad_(False)
@@ -70,7 +81,17 @@
     out = model.forward_(tokens)
     assert out.shape == (32, 8)
     feat = model.forward_feature(tokens)
     assert feat.shape == (8,)
     assert feat.eq(out[-1]).all()
     gen = model.forward_generation(tokens)
     assert gen.shape == (32, 16)
+
+    conf = nets.AbsPosEncoderCausalConfig(
+        token_size=16, max_len=32, d_model=8, nhead=2, num_layers=2, dtype=torch.bfloat16)
+    model = nets.AbsPosEncoderCausal(conf=conf)
+    model.eval()
+    model.requires_grad_(False)
+
+    batch = torch.randint(1, 16, (2, 32))
+    out = model.forward_(batch)
+    assert out.shape == (2, 32, 8)
```

### Comparing `moltx-0.9.4/tests/test_pipelines.py` & `moltx-0.9.5/tests/test_pipelines.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,20 +5,27 @@
 def test_AdaMR(tokenizer, model_conf):
     pipeline = pipelines.AdaMR(tokenizer, models.AdaMR(model_conf))
     out = pipeline("CC[N+](C)(C)Br", k=1)
     assert 'smiles' in out and 'probabilities' in out
     assert isinstance(out['smiles'], list) and len(out['smiles']) == 1 and isinstance(out['smiles'][0], str)
     assert isinstance(out['probabilities'], list) and len(
         out['probabilities']) == 1
+
     out = pipeline("CC[N+](C)(C)Br", k=2, gentype='beam')
     assert 'smiles' in out and 'probabilities' in out
     assert isinstance(out['smiles'], list) and len(out['smiles']) == 2 and isinstance(out['smiles'][0], str)
     assert isinstance(out['probabilities'], list) and len(
         out['probabilities']) == 2
 
+    out = pipeline("CC[N+](C)(C)Br", k=1, gentype='beam')
+    assert 'smiles' in out and 'probabilities' in out
+    assert isinstance(out['smiles'], list) and len(out['smiles']) == 1 and isinstance(out['smiles'][0], str)
+    assert isinstance(out['probabilities'], list) and len(
+        out['probabilities']) == 1
+
 
 def test_AdaMRClassifier(tokenizer, model_conf):
     pipeline = pipelines.AdaMRClassifier(
         tokenizer, models.AdaMRClassifier(num_classes=2, conf=model_conf))
     out = pipeline("CC[N+](C)(C)Br")
     assert 'label' in out and 'probability' in out
     assert isinstance(out['label'], int) and isinstance(out['probability'], float)
```

### Comparing `moltx-0.9.4/tests/test_tokenizer.py` & `moltx-0.9.5/tests/test_tokenizer.py`

 * *Files identical despite different names*


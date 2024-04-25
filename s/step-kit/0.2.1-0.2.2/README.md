# Comparing `tmp/step_kit-0.2.1.tar.gz` & `tmp/step_kit-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "step_kit-0.2.1.tar", max compression
+gzip compressed data, was "step_kit-0.2.2.tar", max compression
```

## Comparing `step_kit-0.2.1.tar` & `step_kit-0.2.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0    11357 2024-04-14 11:50:19.928369 step_kit-0.2.1/LICENSE
--rw-r--r--   0        0        0     3016 2024-04-16 07:34:41.018373 step_kit-0.2.1/README.md
--rw-r--r--   0        0        0     1737 2024-04-16 08:18:29.082467 step_kit-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      138 2024-04-14 11:50:19.933514 step_kit-0.2.1/step/__init__.py
--rw-r--r--   0        0        0        0 2024-04-14 11:50:19.933611 step_kit-0.2.1/step/functionality/__init__.py
--rw-r--r--   0        0        0     4705 2024-04-15 05:59:16.479789 step_kit-0.2.1/step/functionality/base.py
--rw-r--r--   0        0        0        0 2024-04-14 11:50:19.933908 step_kit-0.2.1/step/functionality/comps/__init__.py
--rw-r--r--   0        0        0    18935 2024-04-14 12:22:44.709635 step_kit-0.2.1/step/functionality/comps/model_ops.py
--rw-r--r--   0        0        0    28629 2024-04-15 05:59:16.480343 step_kit-0.2.1/step/functionality/comps/trainer.py
--rw-r--r--   0        0        0    41985 2024-04-16 07:34:41.020583 step_kit-0.2.1/step/functionality/cross_funcmodel.py
--rw-r--r--   0        0        0    18452 2024-04-15 05:59:16.481504 step_kit-0.2.1/step/functionality/sc_funcmodel.py
--rw-r--r--   0        0        0    19728 2024-04-15 05:59:16.482134 step_kit-0.2.1/step/functionality/st_funcmodel.py
--rw-r--r--   0        0        0    19342 2024-04-14 18:41:45.322451 step_kit-0.2.1/step/integration.py
--rw-r--r--   0        0        0     1151 2024-04-15 05:59:16.482328 step_kit-0.2.1/step/manager/__init__.py
--rw-r--r--   0        0        0     2765 2024-04-15 05:59:16.482478 step_kit-0.2.1/step/manager/save.py
--rwxr-xr-x   0        0        0        0 2024-04-14 11:50:19.935557 step_kit-0.2.1/step/models/__init__.py
--rw-r--r--   0        0        0     1846 2024-04-14 11:50:19.935690 step_kit-0.2.1/step/models/clust.py
--rw-r--r--   0        0        0    14598 2024-04-16 07:34:41.021749 step_kit-0.2.1/step/models/deconv.py
--rw-r--r--   0        0        0    15639 2024-04-14 11:50:19.936096 step_kit-0.2.1/step/models/distributions.py
--rw-r--r--   0        0        0    12710 2024-04-15 05:59:16.483032 step_kit-0.2.1/step/models/extension.py
--rw-r--r--   0        0        0    17561 2024-04-15 05:59:16.483633 step_kit-0.2.1/step/models/geneformer.py
--rw-r--r--   0        0        0     2307 2024-04-14 12:22:44.709047 step_kit-0.2.1/step/models/knn_map.py
--rw-r--r--   0        0        0      678 2024-04-14 11:50:19.936662 step_kit-0.2.1/step/models/nnls.py
--rw-r--r--   0        0        0        0 2024-04-14 11:50:19.936752 step_kit-0.2.1/step/modules/__init__.py
--rw-r--r--   0        0        0     6941 2024-04-16 07:34:41.022554 step_kit-0.2.1/step/modules/decoder.py
--rw-r--r--   0        0        0     1848 2024-04-14 11:50:19.937054 step_kit-0.2.1/step/modules/gnn.py
--rw-r--r--   0        0        0     3090 2024-04-14 11:50:19.937162 step_kit-0.2.1/step/modules/transformer.py
--rw-r--r--   0        0        0    10647 2024-04-15 05:59:16.484405 step_kit-0.2.1/step/scmodel.py
--rw-r--r--   0        0        0    16647 2024-04-14 18:42:53.390640 step_kit-0.2.1/step/stmodel.py
--rw-r--r--   0        0        0        0 2024-04-14 11:50:19.937755 step_kit-0.2.1/step/utils/__init__.py
--rw-r--r--   0        0        0    41256 2024-04-14 12:22:44.708893 step_kit-0.2.1/step/utils/dataset.py
--rw-r--r--   0        0        0     2853 2024-04-15 05:59:16.484585 step_kit-0.2.1/step/utils/gbolt.py
--rw-r--r--   0        0        0     1454 2024-04-14 11:50:19.938205 step_kit-0.2.1/step/utils/metrics.py
--rwxr-xr-x   0        0        0    14616 2024-04-15 06:00:06.656239 step_kit-0.2.1/step/utils/misc.py
--rw-r--r--   0        0        0    16000 2024-04-15 05:59:16.485008 step_kit-0.2.1/step/utils/plotting.py
--rw-r--r--   0        0        0        0 2024-04-14 11:50:19.938694 step_kit-0.2.1/step/utils/synthetics/__init__.py
--rw-r--r--   0        0        0    22670 2024-04-14 12:22:44.700905 step_kit-0.2.1/step/utils/synthetics/pseudo_st.py
--rw-r--r--   0        0        0     4735 1970-01-01 00:00:00.000000 step_kit-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-14 11:50:19.928369 step_kit-0.2.2/LICENSE
+-rw-r--r--   0        0        0     5115 2024-04-25 16:24:13.951115 step_kit-0.2.2/README.md
+-rw-r--r--   0        0        0     1949 2024-04-25 17:05:40.907767 step_kit-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      138 2024-04-14 11:50:19.933514 step_kit-0.2.2/step/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-14 11:50:19.933611 step_kit-0.2.2/step/functionality/__init__.py
+-rw-r--r--   0        0        0     4735 2024-04-23 10:25:22.106565 step_kit-0.2.2/step/functionality/base.py
+-rw-r--r--   0        0        0        0 2024-04-14 11:50:19.933908 step_kit-0.2.2/step/functionality/comps/__init__.py
+-rw-r--r--   0        0        0    18989 2024-04-23 10:25:22.116431 step_kit-0.2.2/step/functionality/comps/model_ops.py
+-rw-r--r--   0        0        0    28677 2024-04-23 10:25:22.118508 step_kit-0.2.2/step/functionality/comps/trainer.py
+-rw-r--r--   0        0        0    41985 2024-04-16 07:34:41.020583 step_kit-0.2.2/step/functionality/cross_funcmodel.py
+-rw-r--r--   0        0        0    18476 2024-04-23 10:25:22.106597 step_kit-0.2.2/step/functionality/sc_funcmodel.py
+-rw-r--r--   0        0        0    19746 2024-04-23 10:21:41.306847 step_kit-0.2.2/step/functionality/st_funcmodel.py
+-rw-r--r--   0        0        0    19342 2024-04-14 18:41:45.322451 step_kit-0.2.2/step/integration.py
+-rw-r--r--   0        0        0     1151 2024-04-15 05:59:16.482328 step_kit-0.2.2/step/manager/__init__.py
+-rw-r--r--   0        0        0     2765 2024-04-15 05:59:16.482478 step_kit-0.2.2/step/manager/save.py
+-rwxr-xr-x   0        0        0        0 2024-04-14 11:50:19.935557 step_kit-0.2.2/step/models/__init__.py
+-rw-r--r--   0        0        0     1846 2024-04-14 11:50:19.935690 step_kit-0.2.2/step/models/clust.py
+-rw-r--r--   0        0        0    14598 2024-04-16 07:34:41.021749 step_kit-0.2.2/step/models/deconv.py
+-rw-r--r--   0        0        0    15639 2024-04-14 11:50:19.936096 step_kit-0.2.2/step/models/distributions.py
+-rw-r--r--   0        0        0    12740 2024-04-23 10:25:22.106158 step_kit-0.2.2/step/models/extension.py
+-rw-r--r--   0        0        0     2307 2024-04-14 12:22:44.709047 step_kit-0.2.2/step/models/knn_map.py
+-rw-r--r--   0        0        0      678 2024-04-14 11:50:19.936662 step_kit-0.2.2/step/models/nnls.py
+-rw-r--r--   0        0        0    17627 2024-04-23 10:25:22.106144 step_kit-0.2.2/step/models/transcriptformer.py
+-rw-r--r--   0        0        0        0 2024-04-14 11:50:19.936752 step_kit-0.2.2/step/modules/__init__.py
+-rw-r--r--   0        0        0     6941 2024-04-16 07:34:41.022554 step_kit-0.2.2/step/modules/decoder.py
+-rw-r--r--   0        0        0     1848 2024-04-14 11:50:19.937054 step_kit-0.2.2/step/modules/gnn.py
+-rw-r--r--   0        0        0     3090 2024-04-14 11:50:19.937162 step_kit-0.2.2/step/modules/transformer.py
+-rw-r--r--   0        0        0    10647 2024-04-15 05:59:16.484405 step_kit-0.2.2/step/scmodel.py
+-rw-r--r--   0        0        0    16647 2024-04-14 18:42:53.390640 step_kit-0.2.2/step/stmodel.py
+-rw-r--r--   0        0        0        0 2024-04-14 11:50:19.937755 step_kit-0.2.2/step/utils/__init__.py
+-rw-r--r--   0        0        0    41256 2024-04-14 12:22:44.708893 step_kit-0.2.2/step/utils/dataset.py
+-rw-r--r--   0        0        0     2853 2024-04-15 05:59:16.484585 step_kit-0.2.2/step/utils/gbolt.py
+-rw-r--r--   0        0        0     1454 2024-04-14 11:50:19.938205 step_kit-0.2.2/step/utils/metrics.py
+-rwxr-xr-x   0        0        0    14616 2024-04-15 06:00:06.656239 step_kit-0.2.2/step/utils/misc.py
+-rw-r--r--   0        0        0    16000 2024-04-15 05:59:16.485008 step_kit-0.2.2/step/utils/plotting.py
+-rw-r--r--   0        0        0        0 2024-04-14 11:50:19.938694 step_kit-0.2.2/step/utils/synthetics/__init__.py
+-rw-r--r--   0        0        0    22670 2024-04-14 12:22:44.700905 step_kit-0.2.2/step/utils/synthetics/pseudo_st.py
+-rw-r--r--   0        0        0     7086 1970-01-01 00:00:00.000000 step_kit-0.2.2/PKG-INFO
```

### Comparing `step_kit-0.2.1/LICENSE` & `step_kit-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `step_kit-0.2.1/pyproject.toml` & `step_kit-0.2.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 [tool.poetry]
 name = "step-kit"
-version = "0.2.1"
+version = "0.2.2"
 description = "STEP, an acronym for Spatial Transcriptomics Embedding Procedure, is a deep learning-based tool for the analysis of single-cell RNA (scRNA-seq) and spatially resolved transcriptomics (SRT) data. STEP introduces a unified approach to process and analyze multiple samples of scRNA-seq data as well as align several sections of SRT data, disregarding location relationships. Furthermore, STEP conducts integrative analysis across different modalities like scRNA-seq and SRT."
 authors = ["SGGb0nd <lilounan1997@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.md"
+repository = "https://github.com/SGGb0nd/step"
+documentation = "https://sggb0nd.github.io/step/"
+keywords = ["spatial transcriptomics", "single-cell RNA-seq", "deep learning", "scRNA-seq", "SRT", "step", "STEP"]
 packages = [
     {include = "step"}
 ]
 
 [tool.poetry.dependencies]
 python = "^3.10"
-torch = "1.13.0"
+torch = "1.13.1"
 scanpy = "^1.10.0rc2"
 einops = "^0.6.0"
 leidenalg = "^0.9.0"
 libpysal = "4.8.1"
 esda = "2.5.1"
 scikit-misc = "*"
 rpy2 = { version = "*", optional = true }
```

### Comparing `step_kit-0.2.1/step/functionality/base.py` & `step_kit-0.2.2/step/functionality/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 import torch
 import torch.utils
 from anndata import AnnData
 
 from step.manager import logger
-from step.models.geneformer import Geneformer
+from step.models.transcriptformer import TranscriptFormer
 from step.utils.dataset import BaseDataset, MaskedDataset
 
 from .comps.model_ops import ModelOps
 from .comps.trainer import Trainer
 
 
 class FunctionalBase(ModelOps, Trainer):
     """
     FunctionalBase is a compound class that combines the ModelOps and Trainer classes.
 
     Attributes:
-        model (Geneformer): The model to be trained.
+        model (TranscriptFormer): The model to be trained.
         split_rate (float): The ratio of validation data to the total data.
         use_earlystop (bool): A flag indicating whether to use early stopping during training.
         device (str): The device to use for training. Defaults to "cuda" if a GPU is available, otherwise "cpu".
     """
 
-    def __init__(self, model: Geneformer, use_earlystop=True, device=None):
+    def __init__(self, model: TranscriptFormer, use_earlystop=True, device=None):
         """Initialize the FunctionalBase.
 
         Args:
-            model (Geneformer): The model to be wrapped.
+            model (TranscriptFormer): The model to be wrapped.
             use_earlystop (bool, optional): A flag indicating whether to use early stopping during training. Defaults to True.
         """
         ModelOps.__init__(self, model=model, device=device)
         Trainer.__init__(self, model=model)
         self.split_rate = 0.0
         self.use_earlystop = use_earlystop
         if device is not None:
```

### Comparing `step_kit-0.2.1/step/functionality/comps/model_ops.py` & `step_kit-0.2.2/step/functionality/comps/model_ops.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,36 +5,36 @@
 import torch.nn.functional as F
 from anndata import AnnData
 from torch.distributions import Poisson
 
 from step.manager import logger
 from step.models.distributions import (NegativeBinomial,
                                        ZeroInflatedNegativeBinomial)
-from step.models.geneformer import Geneformer, Readout
+from step.models.transcriptformer import TranscriptFormer, Readout
 from step.utils.dataset import BaseDataset
 
 
 class ModelOps(object):
-    """A class for wrapping a Geneformer model with useful methods.
+    """A class for wrapping a TranscriptFormer model with useful methods.
 
     Attributes:
-        model (Geneformer): The Geneformer model.
+        model (TranscriptFormer): The TranscriptFormer model.
 
     """
 
     def __init__(
         self,
-        model: Geneformer,
+        model: TranscriptFormer,
         device: str | None,
     ):
         """
-        Take a Geneformer model and wrap it with some useful methods.
+        Take a TranscriptFormer model and wrap it with some useful methods.
 
         Args:
-            model (Geneformer): a Geneformer model
+            model (TranscriptFormer): a TranscriptFormer model
             _factor (float): a factor to scale the loss
             kl_cutoff (float): a cutoff value for the KL loss
         """
         self.model = model
 
         # self._factor = 0.01 if model.decoder_type == 'zinb' else 1e-3
         self._factor = 1e-2
```

### Comparing `step_kit-0.2.1/step/functionality/comps/trainer.py` & `step_kit-0.2.2/step/functionality/comps/trainer.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import torch
 from sklearn.model_selection import train_test_split
 from torch import optim
 from torch.utils.data import DataLoader, random_split
 from tqdm import tqdm
 
 from step.manager import logger
-from step.models.geneformer import Geneformer
+from step.models.transcriptformer import TranscriptFormer
 from step.utils.dataset import BaseDataset, MaskedDataset
 
 
 def train_loop_formatter(train_func):
     """
     A decorator function that formats the training loop.
 
@@ -112,32 +112,32 @@
             self.best_score = score
             self.counter = 0
             self.early_stop = False
 
 
 class Trainer(object):
     """
-    The Trainer class is responsible for training the Geneformer model.
+    The Trainer class is responsible for training the TranscriptFormer model.
 
     Attributes:
-        model (Geneformer): The Geneformer model being trained.
+        model (TranscriptFormer): The TranscriptFormer model being trained.
         optimizer (torch.optim.Adam): The optimizer used for model parameter updates.
         lr_scheduler (torch.optim.lr_scheduler.MultiStepLR): The learning rate scheduler.
         early_stopping (Dict[str, EarlyStopping]): A dictionary of EarlyStopping objects for each loss type.
         lossconfig (dict): A dictionary containing the configuration for different loss types.
         defualt_lcfg (dict): The default configuration for loss types.
 
     """
 
-    def __init__(self, model: Geneformer):
+    def __init__(self, model: TranscriptFormer):
         """
         Initializes the Trainer object.
 
         Args:
-            model (Geneformer): The Geneformer model being trained.
+            model (TranscriptFormer): The TranscriptFormer model being trained.
         """
         self.model = model
         self.init_optimizer()
         self.set_lr_scheduler()
         self.model.train()
         self.early_stopping: Dict[str, EarlyStopping] = {}
         # self.lr_scheduler = kwargs.get('lr_scheduler', defualt_lr_scheduler)
```

### Comparing `step_kit-0.2.1/step/functionality/cross_funcmodel.py` & `step_kit-0.2.2/step/functionality/cross_funcmodel.py`

 * *Files identical despite different names*

### Comparing `step_kit-0.2.1/step/functionality/sc_funcmodel.py` & `step_kit-0.2.2/step/functionality/sc_funcmodel.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 from typing import Literal, Optional
 
 import torch
 import torch.nn.functional as F
 from anndata import AnnData
 
 from step.manager import logger
-from step.models.geneformer import Geneformer
+from step.models.transcriptformer import TranscriptFormer
 from step.utils.dataset import BaseDataset, MaskedDataset, ScDataset
 
 from ..models.extension import NrmlsBC
 from .base import FunctionalBase
 
 
 class scSingleBatch(FunctionalBase):
     """scSingleBatch model for scRNA-seq data.
 
     Attributes:
-        model (Geneformer): The model used for training.
+        model (TranscriptFormer): The model used for training.
     """
 
     def __init__(self, device=None, **kwargs):
-        model = Geneformer(**kwargs)
+        model = TranscriptFormer(**kwargs)
         super().__init__(model, device=device)
 
     def handle_input_tuple(self, input_tuple):
         X = input_tuple
         return self.loss(X.to(self.device))
```

### Comparing `step_kit-0.2.1/step/functionality/st_funcmodel.py` & `step_kit-0.2.2/step/functionality/st_funcmodel.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import numpy as np
 import torch
 import torch.nn.functional as F
 from anndata import AnnData
 from torch.distributions import kl_divergence as kl
 
 from step.manager import logger
-from step.models.geneformer import Geneformer
+from step.models.transcriptformer import TranscriptFormer
 from step.utils.dataset import StDataset
 from step.utils.gbolt import MultiGraphsAllNodesSampler
 from step.utils.misc import generate_adj
 
 from ..models.extension import NrmlsBC
 from .base import FunctionalBase
 
@@ -61,15 +61,15 @@
                 variational=variational,
                 dispersion=dispersion,
                 n_glayers=n_glayers,
                 use_l_scale=use_l_scale,
                 **kwargs
             )
         else:
-            model = Geneformer(variational=variational,
+            model = TranscriptFormer(variational=variational,
                                n_glayers=n_glayers,
                                **kwargs)
 
         model.init_smoother_with_builtin()
         super().__init__(model=model, use_earlystop=use_earlystop, device=device)
         self._factor = beta
         self._num_batches = num_batches
```

### Comparing `step_kit-0.2.1/step/integration.py` & `step_kit-0.2.2/step/integration.py`

 * *Files identical despite different names*

### Comparing `step_kit-0.2.1/step/manager/__init__.py` & `step_kit-0.2.2/step/manager/__init__.py`

 * *Files identical despite different names*

### Comparing `step_kit-0.2.1/step/manager/save.py` & `step_kit-0.2.2/step/manager/save.py`

 * *Files identical despite different names*

### Comparing `step_kit-0.2.1/step/models/clust.py` & `step_kit-0.2.2/step/models/clust.py`

 * *Files identical despite different names*

### Comparing `step_kit-0.2.1/step/models/deconv.py` & `step_kit-0.2.2/step/models/deconv.py`

 * *Files identical despite different names*

### Comparing `step_kit-0.2.1/step/models/distributions.py` & `step_kit-0.2.2/step/models/distributions.py`

 * *Files identical despite different names*

### Comparing `step_kit-0.2.1/step/models/extension.py` & `step_kit-0.2.2/step/models/extension.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from itertools import chain
 from typing import Literal, Optional
 
 import torch
 from einops import repeat
 from torch import nn
 
-from step.models.geneformer import Geneformer
+from step.models.transcriptformer import TranscriptFormer
 
 
 class BatchAwareScale(nn.Module):
     """BatchAwareScale is a module that performs BatchAwareScale introduced in the paper.
 
     Attributes:
         net (nn.Sequential): The neural network.
@@ -70,23 +70,23 @@
     def forward(self, x, batch):
         x = self.layernorm(x)
         mean = self.mean(batch)
         scale = self.scale(batch).exp()
         return self.act(x * scale + mean)
 
 
-class NrmlsBC(Geneformer):
-    """NrmlsBC is an extension of the Geneformer model that supports batch-aware normalization and scaling to eliminate batch effects.
+class NrmlsBC(TranscriptFormer):
+    """NrmlsBC is an extension of the TranscriptFormer model that supports batch-aware normalization and scaling to eliminate batch effects.
 
     Attributes:
         num_batches (int): The number of batches.
         batch_emb_dim (int): The batch embedding dimension.
         smoother (Optional[nn.Module]): The smoother module.
         batch_embedding (nn.Parameter): The batch embedding parameter.
-        moduler (Geneformer): The moduler module.
+        moduler (TranscriptFormer): The moduler module.
         batch_readout (BatchAwareScale): The batch readout module.
         args (Dict[str, Any]): The arguments of the model.
     """
 
     def __init__(self,
                  num_batches: int,
                  num_classes: int = 1,
```

### Comparing `step_kit-0.2.1/step/models/geneformer.py` & `step_kit-0.2.2/step/models/transcriptformer.py`

 * *Files 6% similar despite different names*

```diff
@@ -56,15 +56,15 @@
         affine_out = torch.einsum("bi,ijk->bjk", [x, self.weights])
         if self.bias is not None:
             affine_out = affine_out + self.bias
         return affine_out
 
 
 class Readout(nn.Module):
-    """Readout module for the Geneformer model.
+    """Readout module for the TranscriptFormer model.
 
     Attributes:
         net (nn.Sequential): The sequential neural network.
         variational (bool): Whether to use variational encoding.
         out (nn.Sequential): The sequential neural network for the output.
         mean (nn.Linear): The linear layer for the mean.
         logvar (nn.Linear): The linear layer for the logvar.
@@ -181,34 +181,34 @@
         return unfolded
 
     def random_permute(self, x):
         perm = torch.randperm(self.input_dim)
         return x[:, perm]
 
 
-class Geneformer(nn.Module):
-    """Geneformer is a gene expression model based on the Transformer architecture.
+class TranscriptFormer(nn.Module):
+    """TranscriptFormer is a gene expression model based on the Transformer architecture.
 
     Attributes:
-        input_dim (int): The input dimension of the Geneformer model.
-        module_dim (int): The module dimension of the Geneformer model.
-        hidden_dim (int): The hidden dimension of the Geneformer model.
-        n_modules (int): The number of modules of the Geneformer model.
+        input_dim (int): The input dimension of the TranscriptFormer model.
+        module_dim (int): The module dimension of the TranscriptFormer model.
+        hidden_dim (int): The hidden dimension of the TranscriptFormer model.
+        n_modules (int): The number of modules of the TranscriptFormer model.
         moduler (GeneModuler): The GeneModuler object.
         expand (nn.Linear): The linear layer for expanding the module.
         readout (Readout): The Readout object.
         module (nn.TransformerEncoder): The TransformerEncoder object.
         cls_token (nn.Parameter): The classification token.
         px_r (torch.nn.Parameter): The parameter for the zero-inflated negative binomial distribution.
         decoder (ProbDecoder): The ProbDecoder object.
         decoder_type (str): The type of the decoder.
         _smooth (bool): Whether to use smoothing.
         smoother (GCN): The GCN object for smoothing.
         smoother_type (str): The type of the smoother.
-        args (dict): The arguments for the Geneformer model.
+        args (dict): The arguments for the TranscriptFormer model.
         gargs (dict): The arguments for the GCN object.
     """
 
     def __init__(
         self,
         decoder_type="zinb",
         use_pe=True,
@@ -228,15 +228,15 @@
         dec_hidden_dim=None,
         n_dec_hid_layers: int = 1,
         edge_clip=2,
         use_l_scale: bool = False,
         num_batches: int = 1,
         activation: Literal["softplus", "softmax"] | None = None,
     ):
-        """Initializes the Geneformer model.
+        """Initializes the TranscriptFormer model.
 
         Args:
             grids (None, optional): Grids. Defaults to None.
             decoder_type (str, optional): Decoder type. Defaults to 'zinb'.
             use_pe (bool, optional): Whether to use positional encoding. Defaults to True.
             use_smooth (bool, optional): Whether to use smoothing. Defaults to False.
             use_skip (bool, optional): Whether to use skip connections. Defaults to False.
@@ -251,15 +251,15 @@
             variational (bool, optional): Whether to use variational encoding. Defaults to True.
             smoother (str, optional): Smoother type. Defaults to 'GCN'.
             n_glayers (int, optional): Number of graph layers. Defaults to 3.
             dec_hidden_dim (None, optional): Decoder hidden dimension. Defaults to None.
             n_dec_hid_layers (int, optional): Number of decoder hidden layers. Defaults to 1.
             edge_clip (int, optional): Edge clip value. Defaults to 2.
         """
-        super(Geneformer, self).__init__()
+        super(TranscriptFormer, self).__init__()
         if not variational:
             logger.info("Not using VAE")
         self.input_dim = input_dim
         self.module_dim = module_dim
         self.hidden_dim = hidden_dim
         self.n_modules = n_modules
         if decoder_input_dim is None:
@@ -483,11 +483,11 @@
         if self.decoder_type in ["zinb", "nb"]:
             x_recon, _, _ = self.decoder(h, x)
         else:
             x_recon, _ = self.decoder(h, x)
         return x_recon
 
     def copy(self, with_state=True):
-        new_model = Geneformer(**self.args)
+        new_model = TranscriptFormer(**self.args)
         if with_state:
             new_model.load_state_dict(self.state_dict())
         return new_model
```

### Comparing `step_kit-0.2.1/step/models/knn_map.py` & `step_kit-0.2.2/step/models/knn_map.py`

 * *Files identical despite different names*

### Comparing `step_kit-0.2.1/step/models/nnls.py` & `step_kit-0.2.2/step/models/nnls.py`

 * *Files identical despite different names*

### Comparing `step_kit-0.2.1/step/modules/decoder.py` & `step_kit-0.2.2/step/modules/decoder.py`

 * *Files identical despite different names*

### Comparing `step_kit-0.2.1/step/modules/gnn.py` & `step_kit-0.2.2/step/modules/gnn.py`

 * *Files identical despite different names*

### Comparing `step_kit-0.2.1/step/modules/transformer.py` & `step_kit-0.2.2/step/modules/transformer.py`

 * *Files identical despite different names*

### Comparing `step_kit-0.2.1/step/scmodel.py` & `step_kit-0.2.2/step/scmodel.py`

 * *Files identical despite different names*

### Comparing `step_kit-0.2.1/step/stmodel.py` & `step_kit-0.2.2/step/stmodel.py`

 * *Files identical despite different names*

### Comparing `step_kit-0.2.1/step/utils/dataset.py` & `step_kit-0.2.2/step/utils/dataset.py`

 * *Files identical despite different names*

### Comparing `step_kit-0.2.1/step/utils/gbolt.py` & `step_kit-0.2.2/step/utils/gbolt.py`

 * *Files identical despite different names*

### Comparing `step_kit-0.2.1/step/utils/metrics.py` & `step_kit-0.2.2/step/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `step_kit-0.2.1/step/utils/misc.py` & `step_kit-0.2.2/step/utils/misc.py`

 * *Files identical despite different names*

### Comparing `step_kit-0.2.1/step/utils/plotting.py` & `step_kit-0.2.2/step/utils/plotting.py`

 * *Files identical despite different names*

### Comparing `step_kit-0.2.1/step/utils/synthetics/pseudo_st.py` & `step_kit-0.2.2/step/utils/synthetics/pseudo_st.py`

 * *Files identical despite different names*


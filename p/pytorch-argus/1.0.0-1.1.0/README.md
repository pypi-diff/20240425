# Comparing `tmp/pytorch-argus-1.0.0.tar.gz` & `tmp/pytorch_argus-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytorch-argus-1.0.0.tar", last modified: Tue Nov  9 20:18:45 2021, max compression
+gzip compressed data, was "pytorch_argus-1.1.0.tar", last modified: Thu Apr 25 00:27:55 2024, max compression
```

## Comparing `pytorch-argus-1.0.0.tar` & `pytorch_argus-1.1.0.tar`

### file list

```diff
@@ -1,41 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-09 20:18:45.779556 pytorch-argus-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1080 2021-11-09 20:18:38.000000 pytorch-argus-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       41 2021-11-09 20:18:38.000000 pytorch-argus-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     5038 2021-11-09 20:18:45.783556 pytorch-argus-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3868 2021-11-09 20:18:38.000000 pytorch-argus-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-09 20:18:45.779556 pytorch-argus-1.0.0/argus/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2021-11-09 20:18:38.000000 pytorch-argus-1.0.0/argus/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-09 20:18:45.779556 pytorch-argus-1.0.0/argus/callbacks/
--rw-r--r--   0 runner    (1001) docker     (121)      725 2021-11-09 20:18:38.000000 pytorch-argus-1.0.0/argus/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8593 2021-11-09 20:18:38.000000 pytorch-argus-1.0.0/argus/callbacks/callback.py
--rw-r--r--   0 runner    (1001) docker     (121)     7752 2021-11-09 20:18:38.000000 pytorch-argus-1.0.0/argus/callbacks/checkpoints.py
--rw-r--r--   0 runner    (1001) docker     (121)     2435 2021-11-09 20:18:38.000000 pytorch-argus-1.0.0/argus/callbacks/early_stopping.py
--rw-r--r--   0 runner    (1001) docker     (121)     5446 2021-11-09 20:18:38.000000 pytorch-argus-1.0.0/argus/callbacks/logging.py
--rw-r--r--   0 runner    (1001) docker     (121)    19992 2021-11-09 20:18:38.000000 pytorch-argus-1.0.0/argus/callbacks/lr_schedulers.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-09 20:18:45.779556 pytorch-argus-1.0.0/argus/engine/
--rw-r--r--   0 runner    (1001) docker     (121)       86 2021-11-09 20:18:38.000000 pytorch-argus-1.0.0/argus/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9803 2021-11-09 20:18:38.000000 pytorch-argus-1.0.0/argus/engine/engine.py
--rw-r--r--   0 runner    (1001) docker     (121)      639 2021-11-09 20:18:38.000000 pytorch-argus-1.0.0/argus/loss.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-09 20:18:45.779556 pytorch-argus-1.0.0/argus/metrics/
--rw-r--r--   0 runner    (1001) docker     (121)      123 2021-11-09 20:18:38.000000 pytorch-argus-1.0.0/argus/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      821 2021-11-09 20:18:38.000000 pytorch-argus-1.0.0/argus/metrics/categorical_accuracy.py
--rw-r--r--   0 runner    (1001) docker     (121)      669 2021-11-09 20:18:38.000000 pytorch-argus-1.0.0/argus/metrics/loss.py
--rw-r--r--   0 runner    (1001) docker     (121)     7177 2021-11-09 20:18:38.000000 pytorch-argus-1.0.0/argus/metrics/metric.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-09 20:18:45.779556 pytorch-argus-1.0.0/argus/model/
--rw-r--r--   0 runner    (1001) docker     (121)       76 2021-11-09 20:18:38.000000 pytorch-argus-1.0.0/argus/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11610 2021-11-09 20:18:38.000000 pytorch-argus-1.0.0/argus/model/build.py
--rw-r--r--   0 runner    (1001) docker     (121)     5681 2021-11-09 20:18:38.000000 pytorch-argus-1.0.0/argus/model/load.py
--rw-r--r--   0 runner    (1001) docker     (121)    14359 2021-11-09 20:18:38.000000 pytorch-argus-1.0.0/argus/model/model.py
--rw-r--r--   0 runner    (1001) docker     (121)      704 2021-11-09 20:18:38.000000 pytorch-argus-1.0.0/argus/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (121)      411 2021-11-09 20:18:38.000000 pytorch-argus-1.0.0/argus/types.py
--rw-r--r--   0 runner    (1001) docker     (121)     6661 2021-11-09 20:18:38.000000 pytorch-argus-1.0.0/argus/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-09 20:18:45.779556 pytorch-argus-1.0.0/pytorch_argus.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5038 2021-11-09 20:18:45.000000 pytorch-argus-1.0.0/pytorch_argus.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      787 2021-11-09 20:18:45.000000 pytorch-argus-1.0.0/pytorch_argus.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-09 20:18:45.000000 pytorch-argus-1.0.0/pytorch_argus.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2021-11-09 20:18:45.000000 pytorch-argus-1.0.0/pytorch_argus.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2021-11-09 20:18:45.000000 pytorch-argus-1.0.0/pytorch_argus.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-09 20:18:45.000000 pytorch-argus-1.0.0/pytorch_argus.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       13 2021-11-09 20:18:38.000000 pytorch-argus-1.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      235 2021-11-09 20:18:45.783556 pytorch-argus-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1969 2021-11-09 20:18:38.000000 pytorch-argus-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:27:55.235052 pytorch_argus-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-25 00:27:46.000000 pytorch_argus-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6971 2024-04-25 00:27:55.235052 pytorch_argus-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4028 2024-04-25 00:27:46.000000 pytorch_argus-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:27:55.231052 pytorch_argus-1.1.0/argus/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-25 00:27:46.000000 pytorch_argus-1.1.0/argus/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:27:55.231052 pytorch_argus-1.1.0/argus/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-25 00:27:46.000000 pytorch_argus-1.1.0/argus/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8593 2024-04-25 00:27:46.000000 pytorch_argus-1.1.0/argus/callbacks/callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7752 2024-04-25 00:27:46.000000 pytorch_argus-1.1.0/argus/callbacks/checkpoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-04-25 00:27:46.000000 pytorch_argus-1.1.0/argus/callbacks/early_stopping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5446 2024-04-25 00:27:46.000000 pytorch_argus-1.1.0/argus/callbacks/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19284 2024-04-25 00:27:46.000000 pytorch_argus-1.1.0/argus/callbacks/lr_schedulers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:27:55.231052 pytorch_argus-1.1.0/argus/engine/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-25 00:27:46.000000 pytorch_argus-1.1.0/argus/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9805 2024-04-25 00:27:46.000000 pytorch_argus-1.1.0/argus/engine/engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-25 00:27:46.000000 pytorch_argus-1.1.0/argus/loss.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:27:55.231052 pytorch_argus-1.1.0/argus/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-25 00:27:46.000000 pytorch_argus-1.1.0/argus/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      821 2024-04-25 00:27:46.000000 pytorch_argus-1.1.0/argus/metrics/categorical_accuracy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-25 00:27:46.000000 pytorch_argus-1.1.0/argus/metrics/loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7192 2024-04-25 00:27:46.000000 pytorch_argus-1.1.0/argus/metrics/metric.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:27:55.231052 pytorch_argus-1.1.0/argus/model/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-25 00:27:46.000000 pytorch_argus-1.1.0/argus/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11610 2024-04-25 00:27:46.000000 pytorch_argus-1.1.0/argus/model/build.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5681 2024-04-25 00:27:46.000000 pytorch_argus-1.1.0/argus/model/load.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14558 2024-04-25 00:27:46.000000 pytorch_argus-1.1.0/argus/model/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-25 00:27:46.000000 pytorch_argus-1.1.0/argus/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-25 00:27:46.000000 pytorch_argus-1.1.0/argus/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7340 2024-04-25 00:27:46.000000 pytorch_argus-1.1.0/argus/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-04-25 00:27:46.000000 pytorch_argus-1.1.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:27:55.235052 pytorch_argus-1.1.0/pytorch_argus.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6971 2024-04-25 00:27:55.000000 pytorch_argus-1.1.0/pytorch_argus.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-25 00:27:55.000000 pytorch_argus-1.1.0/pytorch_argus.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 00:27:55.000000 pytorch_argus-1.1.0/pytorch_argus.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-25 00:27:55.000000 pytorch_argus-1.1.0/pytorch_argus.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-25 00:27:55.000000 pytorch_argus-1.1.0/pytorch_argus.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 00:27:55.235052 pytorch_argus-1.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:27:55.235052 pytorch_argus-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-25 00:27:46.000000 pytorch_argus-1.1.0/tests/test_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-25 00:27:46.000000 pytorch_argus-1.1.0/tests/test_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-04-25 00:27:46.000000 pytorch_argus-1.1.0/tests/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4814 2024-04-25 00:27:46.000000 pytorch_argus-1.1.0/tests/test_utils.py
```

### Comparing `pytorch-argus-1.0.0/LICENSE` & `pytorch_argus-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytorch-argus-1.0.0/README.md` & `pytorch_argus-1.1.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -16,35 +16,35 @@
 ## Documentation
 
 https://pytorch-argus.readthedocs.io
 
 ## Installation
 
 Requirements: 
-* torch>=1.1.0
+* torch>=2.0.0
 
 From pip:
 
 ```bash
 pip install pytorch-argus
 ```
 
 From source:
 
 ```bash
-pip install -U git+https://github.com/lRomul/argus.git
+pip install -U git+https://github.com/lRomul/argus.git@dev
 ```
 
 ## Example
 
 Simple image classification example with `create_model` from [pytorch-image-models](https://github.com/rwightman/pytorch-image-models):
 
 ```python
-from torchvision.datasets import MNIST
 from torch.utils.data import DataLoader
+from torchvision.datasets import MNIST
 from torchvision.transforms import Compose, ToTensor, Normalize
 
 import timm
 
 import argus
 from argus.callbacks import MonitorCheckpoint, EarlyStopping, ReduceLROnPlateau
 
@@ -96,14 +96,15 @@
               num_epochs=50,
               metrics=['accuracy'],
               callbacks=callbacks,
               metrics_on_train=True)
 ```
 
 More examples you can find [here](https://pytorch-argus.readthedocs.io/en/latest/examples.html).
+Additional guides on how to customize and use argus component can be found in [Guides](https://pytorch-argus.readthedocs.io/en/latest/guides.html) section.
 
 
 ## Why this name, Argus?
 
 The library name is a reference to a planet from World of Warcraft. 
 Argus is the original homeworld of the eredar (a race of supremely talented magic-wielders), now located within the Twisting Nether. 
 It was once described as a utopian world whose inhabitants were both vastly intelligent and highly gifted in magic.
```

### Comparing `pytorch-argus-1.0.0/argus/callbacks/__init__.py` & `pytorch_argus-1.1.0/argus/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorch-argus-1.0.0/argus/callbacks/callback.py` & `pytorch_argus-1.1.0/argus/callbacks/callback.py`

 * *Files identical despite different names*

### Comparing `pytorch-argus-1.0.0/argus/callbacks/checkpoints.py` & `pytorch_argus-1.1.0/argus/callbacks/checkpoints.py`

 * *Files identical despite different names*

### Comparing `pytorch-argus-1.0.0/argus/callbacks/early_stopping.py` & `pytorch_argus-1.1.0/argus/callbacks/early_stopping.py`

 * *Files identical despite different names*

### Comparing `pytorch-argus-1.0.0/argus/callbacks/logging.py` & `pytorch_argus-1.1.0/argus/callbacks/logging.py`

 * *Files identical despite different names*

### Comparing `pytorch-argus-1.0.0/argus/callbacks/lr_schedulers.py` & `pytorch_argus-1.1.0/argus/callbacks/lr_schedulers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """Wrappers to use learning rate schedulers from PyTorch with argus models.
 
 It enables the PyTorch lr_schedulers to be used as normal argus Callbacks.
 """
 from typing import Optional, Callable, Iterable, Any, Union, List
 
-import torch
 from torch.optim import Optimizer
 from torch.optim import lr_scheduler as _scheduler
 
 from argus.engine import State
 from argus.callbacks.callback import Callback
 from argus.metrics.metric import init_better
 
@@ -204,42 +203,39 @@
         better (str, optional): The metric improvement criterion. Should be
             'min', 'max' or 'auto'. 'auto' means the criterion should be
             taken from the metric itself, which is appropriate behavior in
             most cases. Defaults to 'auto'.
         factor (float, optional): Multiplicative factor. Defaults to 0.1.
         patience (int, optional): Number of training epochs without the
             metric improvement to update the learning rate. Defaults to 10.
-        verbose (bool, optional): Print info on each update to stdout.
-            Defaults to False.
         threshold (float, optional): Threshold for considering the changes
             significant. Defaults to 1e-4.
         threshold_mode (str, optional): Should be 'rel', 'abs'.
             Defaults to 'rel'.
         cooldown (int, optional): Number of epochs to wait before resuming
             normal operation after lr has been updated. Defaults to 0.
         min_lr (float or list of float, optional): Min learning rate.
             Defaults to 0.
         eps (float, optional): Min significant learning rate update.
             Defaults to 1e-8.
 
     """
 
     def __init__(self, monitor='val_loss', better='auto', factor=0.1,
-                 patience=10, verbose=False, threshold=1e-4,
-                 threshold_mode='rel', cooldown=0, min_lr=0, eps=1e-8):
+                 patience=10, threshold=1e-4, threshold_mode='rel',
+                 cooldown=0, min_lr=0, eps=1e-8):
         self.monitor = monitor
         self.patience = patience
         self.better, _, _ = init_better(better, monitor)
 
         super().__init__(
             lambda opt: _scheduler.ReduceLROnPlateau(opt,
                                                      mode=self.better,
                                                      factor=factor,
                                                      patience=patience,
-                                                     verbose=verbose,
                                                      threshold=threshold,
                                                      threshold_mode=threshold_mode,
                                                      cooldown=cooldown,
                                                      min_lr=min_lr,
                                                      eps=eps),
             step_on_iteration=False
         )
@@ -366,24 +362,20 @@
     """
 
     def __init__(self,
                  lr_lambda: Union[Callable[[int], float],
                                   List[Callable[[int], float]]],
                  last_epoch: int = -1,
                  step_on_iteration: bool = False):
-        from distutils.version import LooseVersion
-        if LooseVersion(torch.__version__) >= LooseVersion("1.4.0"):
-            super().__init__(
-                lambda opt: _scheduler.MultiplicativeLR(opt,
-                                                        lr_lambda,
-                                                        last_epoch=last_epoch),
-                step_on_iteration=step_on_iteration
-            )
-        else:
-            raise ImportError("Update torch>=1.4.0 to use 'MultiplicativeLR'")
+        super().__init__(
+            lambda opt: _scheduler.MultiplicativeLR(opt,
+                                                    lr_lambda,
+                                                    last_epoch=last_epoch),
+            step_on_iteration=step_on_iteration
+        )
 
 
 class OneCycleLR(LRScheduler):
     """OneCycleLR scheduler.
 
     Sets the learning rate of each parameter group according to the
     1cycle learning rate policy. The 1cycle policy anneals the learning
@@ -447,27 +439,23 @@
                  anneal_strategy: str = 'cos',
                  cycle_momentum: bool = True,
                  base_momentum: Union[float, List[float]] = 0.85,
                  max_momentum: Union[float, List[float]] = 0.95,
                  div_factor: float = 25.,
                  final_div_factor: float = 1e4,
                  last_epoch: int = -1):
-        from distutils.version import LooseVersion
-        if LooseVersion(torch.__version__) >= LooseVersion("1.3.0"):
-            super().__init__(
-                lambda opt: _scheduler.OneCycleLR(opt,
-                                                  max_lr,
-                                                  total_steps=total_steps,
-                                                  epochs=epochs,
-                                                  steps_per_epoch=steps_per_epoch,
-                                                  pct_start=pct_start,
-                                                  anneal_strategy=anneal_strategy,
-                                                  cycle_momentum=cycle_momentum,
-                                                  base_momentum=base_momentum,
-                                                  max_momentum=max_momentum,
-                                                  div_factor=div_factor,
-                                                  final_div_factor=final_div_factor,
-                                                  last_epoch=last_epoch),
-                step_on_iteration=True
-            )
-        else:
-            raise ImportError("Update torch>=1.3.0 to use 'OneCycleLR'")
+        super().__init__(
+            lambda opt: _scheduler.OneCycleLR(opt,
+                                              max_lr,
+                                              total_steps=total_steps,
+                                              epochs=epochs,
+                                              steps_per_epoch=steps_per_epoch,
+                                              pct_start=pct_start,
+                                              anneal_strategy=anneal_strategy,
+                                              cycle_momentum=cycle_momentum,
+                                              base_momentum=base_momentum,
+                                              max_momentum=max_momentum,
+                                              div_factor=div_factor,
+                                              final_div_factor=final_div_factor,
+                                              last_epoch=last_epoch),
+            step_on_iteration=True
+        )
```

### Comparing `pytorch-argus-1.0.0/argus/engine/engine.py` & `pytorch_argus-1.1.0/argus/engine/engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,16 +14,16 @@
     "Events",
     "State",
     "Engine",
 ]
 
 
 class EventEnum(Enum):
-    """Base class for engine events. User defined custom events should also
-    inherit this class. Example of creating custom events you can find
+    """Base class for engine events. User-defined custom events should also
+    inherit this class. An example of creating custom events is available
     `here <https://github.com/lRomul/argus/blob/master/examples/custom_events.py>`_.
     """
 
 
 class Events(EventEnum):
     """Events that are fired by the :class:`argus.engine.Engine` during
     running.
@@ -111,15 +111,14 @@
         self.iteration: int = 0
         self.epoch: int = 0
         self.step_method, self.model, self.phase = init_step_method(step_method)
         if phase_states is not None:
             phase_states[self.phase] = self
         self.phase_states = phase_states
         self.logger: logging.Logger = self.model.logger
-        self.data_loader: Optional[Iterable] = None
         self.exception: Optional[BaseException] = None
         self.engine: Optional[Engine] = engine
 
         self.batch: Any = None
         self.step_output: Any = None
 
         self.metrics: Dict[str, Any] = dict()
@@ -220,16 +219,15 @@
             start_epoch (int): The first epoch number.
             end_epoch (int): One above the largest epoch number.
 
         Returns:
             State: An engine state.
 
         """
-        self.state.update(data_loader=data_loader,
-                          epoch=start_epoch,
+        self.state.update(epoch=start_epoch,
                           iteration=0,
                           stopped=False)
 
         try:
             self.raise_event(Events.START)
             while self.state.epoch < end_epoch and not self.state.stopped:
                 self.state.iteration = 0
@@ -238,20 +236,23 @@
 
                 for batch in data_loader:
                     self.state.batch = batch
                     self.raise_event(Events.ITERATION_START)
                     self.state.step_output = self.step_method(batch, self.state)
                     self.raise_event(Events.ITERATION_COMPLETE)
                     self.state.step_output = None
+                    self.state.batch = None
+                    del batch
                     if self.state.stopped:
                         break
                     self.state.iteration += 1
 
                 self.raise_event(Events.EPOCH_COMPLETE)
                 self.state.epoch += 1
+            del data_loader
 
             self.raise_event(Events.COMPLETE)
 
         except BaseException as exception:
             if self.state.logger is not None:
                 self.state.logger.exception(exception)
```

### Comparing `pytorch-argus-1.0.0/argus/loss.py` & `pytorch_argus-1.1.0/argus/loss.py`

 * *Files identical despite different names*

### Comparing `pytorch-argus-1.0.0/argus/metrics/categorical_accuracy.py` & `pytorch_argus-1.1.0/argus/metrics/categorical_accuracy.py`

 * *Files identical despite different names*

### Comparing `pytorch-argus-1.0.0/argus/metrics/loss.py` & `pytorch_argus-1.1.0/argus/metrics/loss.py`

 * *Files identical despite different names*

### Comparing `pytorch-argus-1.0.0/argus/metrics/metric.py` & `pytorch_argus-1.1.0/argus/metrics/metric.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import argus
 from argus.callbacks import Callback
 from argus.engine import State, Engine
 
 
 METRIC_REGISTRY: Dict[str, Type['argus.metrics.Metric']] = dict()
 
-__all__ = ["Metric", "attach_metrics"]
+__all__ = ["init_better", "Metric", "attach_metrics"]
 
 
 def init_better(better: str, monitor: str) -> Tuple[str, Callable, float]:
     if better not in ['min', 'max', 'auto']:
         raise ValueError(f"Unknown better option '{better}'")
 
     if better == 'auto':
```

### Comparing `pytorch-argus-1.0.0/argus/model/build.py` & `pytorch_argus-1.1.0/argus/model/build.py`

 * *Files identical despite different names*

### Comparing `pytorch-argus-1.0.0/argus/model/load.py` & `pytorch_argus-1.1.0/argus/model/load.py`

 * *Files identical despite different names*

### Comparing `pytorch-argus-1.0.0/argus/model/model.py` & `pytorch_argus-1.1.0/argus/model/model.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import numbers
 from typing import Iterable, Optional, Union, Dict, List
 
 import torch
 
 import argus
 from argus import types
-from argus.model.build import BuildModel
 from argus.engine import Engine, State
-from argus.callbacks import Callback, attach_callbacks
+from argus.model.build import BuildModel
+from argus.utils import deep_to, deep_detach
 from argus.callbacks.logging import default_logging
+from argus.callbacks import Callback, attach_callbacks
 from argus.metrics.metric import Metric, attach_metrics
 from argus.metrics.loss import Loss
-from argus.utils import deep_to, deep_detach
 
 __all__ = ["Model"]
 
 
 class Model(BuildModel):
     """Argus model is an abstraction of a trainer/predictor that uses:
 
@@ -30,14 +30,16 @@
             multi-GPU mode. To get all devices use
             :meth:`argus.model.Model.get_device` method.
         prediction_transform (Callable): postprocessing function of predictions
             as :class:`Callable` function or object.
 
     Args:
         params (dict): A model parameters.
+        build_order (Iterable[str]): Order of building model attributes. The default
+            order: ('nn_module', 'optimizer', 'loss', 'device', 'prediction_transform').
 
     Examples:
 
         One can use several ways to initialize :class:`argus.model.Model`:
 
         1. Set parameters for each part of the model directly:
 
@@ -79,17 +81,14 @@
                 'device': 'cuda'
             }
 
             model = FlexModel(params)
 
     """
 
-    def __init__(self, params: dict):
-        super().__init__(params)
-
     def train_step(self, batch, state: State) -> dict:
         """Perform a single train step.
 
         The method is used by :class:`argus.engine.Engine`.
         The train step includes input and target tensor transferring to the
         model device, forward pass, loss evaluation, backward pass, and the
         train batch prediction treating with a prediction_transform.
@@ -193,14 +192,17 @@
             callbacks (list of :class:`argus.callbacks.Callback`, optional):
                 List of callbacks to be attached to the training process.
                 Defaults to `None`.
             val_callbacks (list of :class:`argus.callbacks.Callback`, optional):
                 List of callbacks to be attached to the validation process.
                 Defaults to `None`.
 
+        Returns:
+            dict: The metrics dictionary.
+
         """
         self._check_train_ready()
         metrics = [] if metrics is None else metrics
         phase_states = dict()
 
         train_engine = Engine(self.train_step, phase_states=phase_states)
         train_metrics = [Loss()] + metrics if metrics_on_train else [Loss()]
@@ -219,15 +221,16 @@
                 val_state = val_engine.run(val_loader, epoch, epoch + 1)
                 train_state.metrics.update(val_state.metrics)
 
             validation_epoch.attach(train_engine, val_engine, val_loader)
             val_engine.run(val_loader, -1, 0)
 
         attach_callbacks(train_engine, callbacks)
-        train_engine.run(train_loader, 0, num_epochs)
+        state = train_engine.run(train_loader, 0, num_epochs)
+        return state.metrics
 
     def validate(self,
                  val_loader: Iterable,
                  metrics: Optional[List[Union[Metric, str]]] = None,
                  callbacks: Optional[List[Callback]] = None) -> Dict[str, float]:
         """Perform a validation.
```

### Comparing `pytorch-argus-1.0.0/argus/optimizer.py` & `pytorch_argus-1.1.0/argus/optimizer.py`

 * *Files identical despite different names*

### Comparing `pytorch-argus-1.0.0/argus/utils.py` & `pytorch_argus-1.1.0/argus/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-import torch
 import collections
-from functools import partial
+from typing import Any, Set, List, Type, Union
 from tempfile import TemporaryFile
-from typing import List, Union, Type, Set, Any
+from functools import partial
+
+import torch
 
 from argus import types
 
 __all__ = ["deep_to", "deep_detach", "deep_chunk", "AverageMeter"]
 
 
 class Default:
@@ -194,20 +195,36 @@
         device_ids.append(dev.index)
     if len(device_ids) != len(set(device_ids)):
         raise ValueError("CUDA device indices must be unique")
     return device_ids
 
 
 class AverageMeter:
-    """Computes and stores the average by Welford's algorithm"""
+    """Compute and store the average by Welford's algorithm.
+
+    The class instances can be used to compute the average of any sequence of
+    values, for example, to average the loss or metrics over an epoch.
+
+    Use `average` attribute to get the average value. Make sure to check the
+    meter was updated with at least one element by assessing the `count`
+    attribute. Default value of `average` is 0 before updates.
+    """
 
     def __init__(self):
         self.average = 0
         self.count: int = 0
 
     def reset(self):
+        """Reset the average meter."""
         self.average = 0
         self.count = 0
 
     def update(self, value, n: int = 1):
+        """Update the average meter with a new value.
+
+        Args:
+            value: Value to update the average meter with.
+            n (int, optional): Number of elements accumulated by the value.
+                Should be positive. Defaults to 1.
+        """
         self.count += n
-        self.average += (value - self.average) / self.count
+        self.average += (value - self.average * n) / self.count
```

### Comparing `pytorch-argus-1.0.0/pytorch_argus.egg-info/SOURCES.txt` & `pytorch_argus-1.1.0/pytorch_argus.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,10 @@
 LICENSE
-MANIFEST.in
 README.md
-requirements.txt
-setup.cfg
-setup.py
+pyproject.toml
 argus/__init__.py
 argus/loss.py
 argus/optimizer.py
 argus/types.py
 argus/utils.py
 argus/callbacks/__init__.py
 argus/callbacks/callback.py
@@ -26,8 +23,11 @@
 argus/model/load.py
 argus/model/model.py
 pytorch_argus.egg-info/PKG-INFO
 pytorch_argus.egg-info/SOURCES.txt
 pytorch_argus.egg-info/dependency_links.txt
 pytorch_argus.egg-info/requires.txt
 pytorch_argus.egg-info/top_level.txt
-pytorch_argus.egg-info/zip-safe
+tests/test_loss.py
+tests/test_optimizer.py
+tests/test_pipeline.py
+tests/test_utils.py
```


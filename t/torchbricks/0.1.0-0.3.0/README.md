# Comparing `tmp/torchbricks-0.1.0.tar.gz` & `tmp/torchbricks-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchbricks-0.1.0.tar", last modified: Thu Oct  5 07:02:26 2023, max compression
+gzip compressed data, was "torchbricks-0.3.0.tar", last modified: Wed Apr 24 22:54:53 2024, max compression
```

## Comparing `torchbricks-0.1.0.tar` & `torchbricks-0.3.0.tar`

### file list

```diff
@@ -1,36 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 07:02:26.130121 torchbricks-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2023-10-05 07:02:09.000000 torchbricks-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       97 2023-10-05 07:02:09.000000 torchbricks-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    44387 2023-10-05 07:02:26.130121 torchbricks-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    42531 2023-10-05 07:02:09.000000 torchbricks-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2023-10-05 07:02:09.000000 torchbricks-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-05 07:02:26.130121 torchbricks-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 07:02:26.118121 torchbricks-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 07:02:26.126120 torchbricks-0.1.0/src/torchbricks/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2023-10-05 07:02:09.000000 torchbricks-0.1.0/src/torchbricks/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-10-05 07:02:09.000000 torchbricks-0.1.0/src/torchbricks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3142 2023-10-05 07:02:09.000000 torchbricks-0.1.0/src/torchbricks/bag_of_bricks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1871 2023-10-05 07:02:09.000000 torchbricks-0.1.0/src/torchbricks/brick_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6831 2023-10-05 07:02:09.000000 torchbricks-0.1.0/src/torchbricks/brick_visualizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    15457 2023-10-05 07:02:09.000000 torchbricks-0.1.0/src/torchbricks/bricks.py
--rw-r--r--   0 runner    (1001) docker     (127)     3276 2023-10-05 07:02:09.000000 torchbricks-0.1.0/src/torchbricks/bricks_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2023-10-05 07:02:09.000000 torchbricks-0.1.0/src/torchbricks/collection_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1116 2023-10-05 07:02:09.000000 torchbricks-0.1.0/src/torchbricks/custom_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     2613 2023-10-05 07:02:09.000000 torchbricks-0.1.0/src/torchbricks/dag.py
--rw-r--r--   0 runner    (1001) docker     (127)     5391 2023-10-05 07:02:09.000000 torchbricks-0.1.0/src/torchbricks/graph_plotter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3010 2023-10-05 07:02:09.000000 torchbricks-0.1.0/src/torchbricks/tensor_conversions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 07:02:26.126120 torchbricks-0.1.0/src/torchbricks.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    44387 2023-10-05 07:02:26.000000 torchbricks-0.1.0/src/torchbricks.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      834 2023-10-05 07:02:26.000000 torchbricks-0.1.0/src/torchbricks.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-05 07:02:26.000000 torchbricks-0.1.0/src/torchbricks.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2023-10-05 07:02:26.000000 torchbricks-0.1.0/src/torchbricks.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2023-10-05 07:02:26.000000 torchbricks-0.1.0/src/torchbricks.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 07:02:26.130121 torchbricks-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      623 2023-10-05 07:02:09.000000 torchbricks-0.1.0/tests/test_bag_of_bricks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2001 2023-10-05 07:02:09.000000 torchbricks-0.1.0/tests/test_brick_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6663 2023-10-05 07:02:09.000000 torchbricks-0.1.0/tests/test_brick_visualizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    17753 2023-10-05 07:02:09.000000 torchbricks-0.1.0/tests/test_bricks.py
--rw-r--r--   0 runner    (1001) docker     (127)     5460 2023-10-05 07:02:09.000000 torchbricks-0.1.0/tests/test_bricks_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1162 2023-10-05 07:02:09.000000 torchbricks-0.1.0/tests/test_environment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1904 2023-10-05 07:02:09.000000 torchbricks-0.1.0/tests/test_graph_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3473 2023-10-05 07:02:09.000000 torchbricks-0.1.0/tests/test_tensor_conversions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:54:53.601057 torchbricks-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-24 22:54:44.000000 torchbricks-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-24 22:54:44.000000 torchbricks-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    40684 2024-04-24 22:54:53.601057 torchbricks-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    38779 2024-04-24 22:54:44.000000 torchbricks-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-04-24 22:54:44.000000 torchbricks-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 22:54:53.601057 torchbricks-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:54:53.597057 torchbricks-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:54:53.597057 torchbricks-0.3.0/src/torchbricks/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-24 22:54:44.000000 torchbricks-0.3.0/src/torchbricks/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-24 22:54:44.000000 torchbricks-0.3.0/src/torchbricks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:54:53.601057 torchbricks-0.3.0/src/torchbricks/bag_of_bricks/
+-rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-04-24 22:54:44.000000 torchbricks-0.3.0/src/torchbricks/bag_of_bricks/backbones.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6690 2024-04-24 22:54:44.000000 torchbricks-0.3.0/src/torchbricks/bag_of_bricks/brick_visualizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-24 22:54:44.000000 torchbricks-0.3.0/src/torchbricks/bag_of_bricks/custom_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-04-24 22:54:44.000000 torchbricks-0.3.0/src/torchbricks/bag_of_bricks/image_classification.py
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-24 22:54:44.000000 torchbricks-0.3.0/src/torchbricks/bag_of_bricks/preprocessors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-04-24 22:54:44.000000 torchbricks-0.3.0/src/torchbricks/bag_of_bricks/task_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6945 2024-04-24 22:54:44.000000 torchbricks-0.3.0/src/torchbricks/brick_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3799 2024-04-24 22:54:44.000000 torchbricks-0.3.0/src/torchbricks/brick_collection_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-24 22:54:44.000000 torchbricks-0.3.0/src/torchbricks/brick_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9102 2024-04-24 22:54:44.000000 torchbricks-0.3.0/src/torchbricks/bricks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3814 2024-04-24 22:54:44.000000 torchbricks-0.3.0/src/torchbricks/bricks_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-04-24 22:54:44.000000 torchbricks-0.3.0/src/torchbricks/collection_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-04-24 22:54:44.000000 torchbricks-0.3.0/src/torchbricks/dag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5394 2024-04-24 22:54:44.000000 torchbricks-0.3.0/src/torchbricks/graph_plotter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-04-24 22:54:44.000000 torchbricks-0.3.0/src/torchbricks/model_stage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3010 2024-04-24 22:54:44.000000 torchbricks-0.3.0/src/torchbricks/tensor_conversions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:54:53.601057 torchbricks-0.3.0/src/torchbricks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    40684 2024-04-24 22:54:53.000000 torchbricks-0.3.0/src/torchbricks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-04-24 22:54:53.000000 torchbricks-0.3.0/src/torchbricks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 22:54:53.000000 torchbricks-0.3.0/src/torchbricks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-24 22:54:53.000000 torchbricks-0.3.0/src/torchbricks.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-24 22:54:53.000000 torchbricks-0.3.0/src/torchbricks.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:54:53.601057 torchbricks-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    17360 2024-04-24 22:54:44.000000 torchbricks-0.3.0/tests/test_brick_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-04-24 22:54:44.000000 torchbricks-0.3.0/tests/test_brick_collection_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-04-24 22:54:44.000000 torchbricks-0.3.0/tests/test_bricks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5144 2024-04-24 22:54:44.000000 torchbricks-0.3.0/tests/test_bricks_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-24 22:54:44.000000 torchbricks-0.3.0/tests/test_collection_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-24 22:54:44.000000 torchbricks-0.3.0/tests/test_environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-04-24 22:54:44.000000 torchbricks-0.3.0/tests/test_graph_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3473 2024-04-24 22:54:44.000000 torchbricks-0.3.0/tests/test_tensor_conversions.py
```

### Comparing `torchbricks-0.1.0/LICENSE` & `torchbricks-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `torchbricks-0.1.0/PKG-INFO` & `torchbricks-0.3.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: torchbricks
-Version: 0.1.0
-Summary: Decoupled and modular approach to building multi-task ML models
+Version: 0.3.0
+Summary: Decoupled and modular approach to building multi-task ML models using a single model recipe for all model stages
 Author-email: Peter Hviid Christiansen <PeterHviidChristiansen@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Peter Christiansen
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -61,110 +61,114 @@
 
 
 TorchBricks builds pytorch models using small reuseable and decoupled parts - we call them bricks. 
 
 The concept is simple and flexible and allows you to more easily combine, add or swap out parts of the model 
 (preprocessor, backbone, neck, head or post-processor), change the task or extend it with multiple tasks.
 
-TorchBricks is a compact recipe on both *how* model parts are connected and *when* parts are executed 
-during model stages such as training, validation, testing, inference and export.
+TorchBricks is a compact recipe on both *how* model parts are connected and *when* parts should be executed 
+during different model stages such as training, validation, testing, inference and export.
+
+TorchBricks is NOT a framework! - it just a thin abstraction on top of pytorch modules. 
 
 <!-- #region -->
 
 ## Install it with pip
 
 ```bash
 pip install torchbricks
 ```
 <!-- #endregion -->
 
 ## Bricks by example
 
-To demonstrate the the concepts of TorchBricks, we will first specify some dummy parts used of a regular image recognition model: 
+To demonstrate the the concepts of TorchBricks, we will first specify some dummy parts used in a regular image recognition model: 
 A preprocessor, a backbone and a head (in this case a classifier).
 *Note: Don't worry about the actually implementation of these modules - they are just dummy examples.*
 
 ```python
-from typing import Tuple, Any
+from typing import Tuple
+
 import torch
 from torch import nn
+
+
 class PreprocessorDummy(nn.Module):
     def forward(self, raw_input: torch.Tensor) -> torch.Tensor:
-        return raw_input/2
+        return raw_input / 2
+
 
 class TinyModel(nn.Module):
     def __init__(self, n_channels: int, n_features: int) -> None:
         super().__init__()
         self.conv = nn.Conv2d(n_channels, n_features, kernel_size=1)
 
     def forward(self, tensor: torch.Tensor) -> torch.Tensor:
         return self.conv(tensor)
 
+
 class ClassifierDummy(nn.Module):
     def __init__(self, num_classes: int, in_features: int) -> None:
         super().__init__()
         self.fc = nn.Linear(in_features, num_classes)
         self.avgpool = nn.AdaptiveAvgPool2d((1, 1))
         self.softmax = nn.Softmax(dim=1)
 
     def forward(self, tensor: torch.Tensor) -> Tuple[torch.Tensor, torch.Tensor]:
-        logits = self.fc(torch.flatten(self.avgpool(tensor), start_dim = 1))
+        logits = self.fc(torch.flatten(self.avgpool(tensor), start_dim=1))
         return logits, self.softmax(logits)
 ```
 
 
 ## Concept 1: Bricks are connected
 An important concept of TorchBricks is that it defines how modules are connected by specifying input and output names of
 each module similar to a DAG. 
 
 In below code snippet, we demonstrate how this would look for our dummy model. 
 
 ```python
-from torchbricks.bricks import BrickCollection, BrickTrainable, BrickNotTrainable, BrickLoss
-from torchbricks.bricks import Stage
-from torchbricks.graph_plotter import create_mermaid_dag_graph
+from torchbricks.brick_collection import BrickCollection
+from torchbricks.bricks import BrickNotTrainable, BrickTrainable
 
 bricks = {
-    'preprocessor': BrickNotTrainable(PreprocessorDummy(), 
-                                      input_names=['raw_images'], 
-                                      output_names=['processed']),
-    'backbone': BrickTrainable(TinyModel(n_channels=3, n_features=10), 
-                               input_names=['processed'], 
-                               output_names=['embedding']),
-    'head': BrickTrainable(ClassifierDummy(num_classes=3, in_features=10), 
-                           input_names=['embedding'], 
-                           output_names=['logits', "softmaxed"]),
+    "preprocessor": BrickNotTrainable(PreprocessorDummy(), input_names=["raw_images"], output_names=["processed"]),
+    "backbone": BrickTrainable(TinyModel(n_channels=3, n_features=10), input_names=["processed"], output_names=["embedding"]),
+    "head": BrickTrainable(ClassifierDummy(num_classes=3, in_features=10), input_names=["embedding"], output_names=["logits", "softmaxed"]),
 }
 brick_collection = BrickCollection(bricks)
+# print(create_mermaid_dag_graph(brick_collection))
 print(brick_collection)
 ```
 
 Each module is placed in a dictionary with a unique name and wrapped inside a brick with input and output names. 
 Input and output names specifies how outputs of one module is passed to inputs of the next module. 
 
+In above example, we use `BrickNotTrainable` to wrap modules that are shouldn't be trained (weights are fixed) and 
+`BrickTrainable` to wrap modules that are trainable (weights are updated on each training iteration). 
+
 Finally, the dictionary of bricks is passed to a `BrickCollection`. 
 
 Below we visualize how the brick collection connects bricks together. 
 
 
 ```mermaid
 flowchart LR
     %% Brick definitions
-    preprocessor("<strong>BrickNotTrainable</strong><br><strong>preprocessor</strong>: PreprocessorDummy"):::BrickNotTrainable
-    backbone("<strong>BrickTrainable</strong><br><strong>backbone</strong>: TinyModel"):::BrickTrainable
-    head("<strong>BrickTrainable</strong><br><strong>head</strong>: ClassifierDummy"):::BrickTrainable
+    preprocessor(<strong>'preprocessor': PreprocessorDummy</strong><br><i>BrickNotTrainable</i>):::BrickNotTrainable
+    backbone(<strong>'backbone': TinyModel</strong><br><i>BrickTrainable</i>):::BrickTrainable
+    head(<strong>'head': ClassifierDummy</strong><br><i>BrickTrainable</i>):::BrickTrainable
     
     %% Draw input and outputs
     raw_images:::input --> preprocessor
     
     %% Draw nodes and edges
     preprocessor --> |processed| backbone
     backbone --> |embedding| head
-    head --> softmaxed:::output
     head --> logits:::output
+    head --> softmaxed:::output
     
     %% Add styling
     classDef arrow stroke-width:0px,fill-opacity:0.0 
     classDef input stroke-width:0px,fill-opacity:0.3,fill:#22A699 
     classDef output stroke-width:0px,fill-opacity:0.3,fill:#F2BE22 
     classDef BrickNotTrainable stroke-width:0px,fill:#B56576 
     classDef BrickTrainable stroke-width:0px,fill:#6D597A 
@@ -175,26 +179,25 @@
         output(output):::output
     end
 ```
 *Graph is visualized using [mermaid](https://github.com/mermaid-js/mermaid) syntax.*
 *We provide the `create_mermaid_dag_graph`-function to create a brick collection visualization*
 
 
-The `BrickCollection` is used for executing above graph using `named_inputs`. 
-`named_inputs` is simply a dictionary with input name as key and input data as value.
+The `BrickCollection` is used for executing above graph by passing a dictionary with named input data (`named_inputs`). 
 
 For above brick collection, we only expect one named input called `raw_images`. 
 
 ```python
-batch_size=2
+batch_size = 2
 batched_images = torch.rand((batch_size, 3, 100, 200))
-named_inputs = {'raw_images': batched_images}
-named_outputs = brick_collection(named_inputs=named_inputs, stage=Stage.INFERENCE)
+named_inputs = {"raw_images": batched_images}
+named_outputs = brick_collection(named_inputs=named_inputs)
 print("Brick outputs:", named_outputs.keys())
-# Brick outputs: dict_keys(['raw_images', 'stage', 'processed', 'embedding', 'logits', 'softmaxed'])
+# Brick outputs: dict_keys(['raw_images', 'processed', 'embedding', 'logits', 'softmaxed'])
 ```
 
 The brick collection accepts a dictionary and returns a dictionary with all intermediated and resulting tensors. 
 
 Running our models as a brick collection has the following advantages:
 
 - A brick collection act as a regular `nn.Module` with all the familiar features: a `forward`-function, a `to`-function to move 
@@ -202,128 +205,130 @@
 - A brick collection is also a simple DAG, it accepts a dictionary with "named data" (we call this `named_inputs`), 
 executes each bricks and ensures that the outputs are passed to the inputs of other bricks with matching names. 
 Structuring the model as a DAG, makes it easy to add/remove outputs for a given module during development, add new modules to the
 collection and build completely new models from reusable parts. 
 - A brick collection is actually a dictionary (`nn.DictModule`). Allowing you to access, pop and update the 
   collection easily as a regular dictionary. It can also handle nested dictionary, allowing groups of bricks to be added/removed easily. 
 
-Note also that we set `stage=Stage.INFERENCE` to explicitly specify if we are doing training, validation, test or inference.
-Specifying a stage is important, if we want a module to act in a specific way during a specific stages.
 
-Leading us to the next section
+## Concept 2: Bricks are grouped
+Another important concept is that bricks can be executed in groups. 
 
-
-## Concept 2: Bricks can be dead (or alive)
-The second concept is to specify when bricks are alive - meaning we can specify at which stages (train, test, validation, inference 
-and export) a brick is active. 
-
-For other stage the brick will play dead - do nothing / return an empty dictionary. 
-
-Meaning that for different `stages`, we will have the option of creating a unique DAG for each model stage and
-we can control how a brick collection acts during all stages of a model. 
-
-In above example this is not very interesting - because a model will mostly have preprocessor, backbone and head active 
-during all stages.
-
-So we will demonstrate by adding a loss brick (`BrickLoss`) and specifying `alive_stages` for each brick.
+To demonstrate how and why this is useful, we have added the `group` argument to each brick and introduced `BrickLoss` brick.
 
 ```python
-num_classes = 3
+from torchbricks.bricks import BrickLoss
+
 bricks = {
-    'preprocessor': BrickNotTrainable(PreprocessorDummy(), 
-                                      input_names=['raw_images'], 
-                                      output_names=['processed'], 
-                                      alive_stages="all"),
-    'backbone': BrickTrainable(TinyModel(n_channels=num_classes, n_features=10), 
-                               input_names=['processed'], 
-                               output_names=['embedding'], 
-                               alive_stages="all"),
-    'head': BrickTrainable(ClassifierDummy(num_classes=num_classes, in_features=10), 
-                           input_names=['embedding'], 
-                           output_names=['logits', 'softmaxed'], 
-                           alive_stages="all"),
-    'loss': BrickLoss(model=nn.CrossEntropyLoss(), 
-                      input_names=['logits', 'targets'], 
-                      output_names=['loss_ce'], 
-                      alive_stages=[Stage.TRAIN, Stage.VALIDATION, Stage.TEST])
+    "preprocessor": BrickNotTrainable(PreprocessorDummy(), input_names=["raw_images"], output_names=["processed"], group="MODEL"),
+    "backbone": BrickTrainable(
+        TinyModel(n_channels=3, n_features=10), input_names=["processed"], output_names=["embedding"], group="MODEL"
+    ),
+    "head": BrickTrainable(
+        ClassifierDummy(num_classes=3, in_features=10),
+        input_names=["embedding"],
+        output_names=["logits", "softmaxed"],
+        group="MODEL",
+    ),
+    "loss": BrickLoss(model=nn.CrossEntropyLoss(), input_names=["logits", "targets"], output_names=["loss_ce"], group="LOSS"),
 }
 brick_collection = BrickCollection(bricks)
 
 print(brick_collection)
 # BrickCollection(
-#   (preprocessor): BrickNotTrainable(PreprocessorDummy, input_names=['raw_images'], output_names=['processed'], alive_stages=['TRAIN', 'VALIDATION', 'TEST', 'INFERENCE', 'EXPORT'])
-#   (backbone): BrickTrainable(TinyModel, input_names=['processed'], output_names=['embedding'], alive_stages=['TRAIN', 'VALIDATION', 'TEST', 'INFERENCE', 'EXPORT'])
-#   (head): BrickTrainable(ClassifierDummy, input_names=['embedding'], output_names=['logits', 'softmaxed'], alive_stages=['TRAIN', 'VALIDATION', 'TEST', 'INFERENCE', 'EXPORT'])
-#   (loss): BrickLoss(CrossEntropyLoss, input_names=['logits', 'targets'], output_names=['loss_ce'], alive_stages=['TRAIN', 'VALIDATION', 'TEST'])
+#   (preprocessor): BrickNotTrainable(PreprocessorDummy, input_names=['raw_images'], output_names=['processed'], groups={'MODEL'})
+#   (backbone): BrickTrainable(TinyModel, input_names=['processed'], output_names=['embedding'], groups={'MODEL'})
+#   (head): BrickTrainable(ClassifierDummy, input_names=['embedding'], output_names=['logits', 'softmaxed'], groups={'MODEL'})
+#   (loss): BrickLoss(CrossEntropyLoss, input_names=['logits', 'targets'], output_names=['loss_ce'], groups={'LOSS'})
 # )
-print(create_mermaid_dag_graph(brick_collection))
+# print(create_mermaid_dag_graph(brick_collection))
 ```
 
-We set `preprocessor`, `backbone` and `head` to be alive on all stages `alive_stages="all"` - this is the default behavior and
-similar to before. 
- 
-For `loss` we set `alive_stages=[Stage.TRAIN, Stage.VALIDATION, Stage.TEST]` to only calculate loss during train, validation and test
-stages. 
+With group names, it is now possible to execute desired subsets of the model 
+during execution by adding `groups`.
+
+Here is a few examples: 
 
+```python
+named_inputs = {"raw_images": batched_images, "targets": torch.ones((batch_size), dtype=torch.int64)}
 
+# With no groups specified, all bricks are executed
+named_outputs = brick_collection(named_inputs=named_inputs)
 
-**Graph during inference and export:**
+# With groups specified, only bricks in the specified groups are executed
+named_outputs = brick_collection(named_inputs=named_inputs, groups={"MODEL"})
+```
 
-During `Stage.INFERENCE` and `Stage.EXPORT`, the graph will look as before, the loss modules is dead and note only `raw_images` is 
-still the only required input
+Groups are important concept in our model recipe as it allows us to specify how model will act during different model stages. 
 
 
 
+**Brick collection during inference and export:**
 
+During `Inference` and `Export` model stages, we do not have ground truth labels and we wan to skip loss calculations. 
+
+```python
+# Execution only "MODEL" group bricks
+named_outputs = brick_collection(named_inputs=named_inputs, groups={"MODEL"})
+```
+
+The graph will look like this and note that the graph only requires `raw_images` as input:
 ```mermaid
 flowchart LR
     %% Brick definitions
-    preprocessor("<strong>BrickNotTrainable</strong><br><strong>preprocessor</strong>: PreprocessorDummy"):::BrickNotTrainable
-    backbone("<strong>BrickTrainable</strong><br><strong>backbone</strong>: TinyModel"):::BrickTrainable
-    head("<strong>BrickTrainable</strong><br><strong>head</strong>: ClassifierDummy"):::BrickTrainable
+    preprocessor(<strong>'preprocessor': PreprocessorDummy</strong><br><i>BrickNotTrainable</i>):::BrickNotTrainable
+    backbone(<strong>'backbone': TinyModel</strong><br><i>BrickTrainable</i>):::BrickTrainable
+    head(<strong>'head': ClassifierDummy</strong><br><i>BrickTrainable</i>):::BrickTrainable
     
     %% Draw input and outputs
     raw_images:::input --> preprocessor
     
     %% Draw nodes and edges
     preprocessor --> |processed| backbone
     backbone --> |embedding| head
-    head --> softmaxed:::output
     head --> logits:::output
+    head --> softmaxed:::output
     
     %% Add styling
     classDef arrow stroke-width:0px,fill-opacity:0.0 
     classDef input stroke-width:0px,fill-opacity:0.3,fill:#22A699 
     classDef output stroke-width:0px,fill-opacity:0.3,fill:#F2BE22 
     classDef BrickNotTrainable stroke-width:0px,fill:#B56576 
     classDef BrickTrainable stroke-width:0px,fill:#6D597A 
     
     %% Add legends
     subgraph Legends
         input(input):::input
         output(output):::output
-        
     end
 ```
 
 
-**Graph during train, test and validation:**
+**Brick collection during train, test and validation:**
 
-During `Stage.TRAIN`, `Stage.VALIDATION` and `Stage.TEST`, the loss module is alive and note both `raw_images` and `targets` are required as inputs:
+During "Train", "Test" and "Validation", `targets` are available and we want to calculate loss to 
+both improve model and track loss curves. 
 
+```python
+# Execution all groups
+named_outputs = brick_collection(named_inputs=named_inputs)
 
+# Or execute explicitly "MODEL" and "LOSS" group bricks
+named_outputs = brick_collection(named_inputs=named_inputs, groups={"MODEL", "LOSS"})
+```
 
+The graph will look like this and note that the graph now requires `raw_images` and `targets` as input:
 
 ```mermaid
 flowchart LR
     %% Brick definitions
-    preprocessor("<strong>BrickNotTrainable</strong><br><strong>preprocessor</strong>: PreprocessorDummy"):::BrickNotTrainable
-    backbone("<strong>BrickTrainable</strong><br><strong>backbone</strong>: TinyModel"):::BrickTrainable
-    head("<strong>BrickTrainable</strong><br><strong>head</strong>: ClassifierDummy"):::BrickTrainable
-    loss("<strong>BrickLoss</strong><br><strong>loss</strong>: CrossEntropyLoss"):::BrickLoss
+    preprocessor(<strong>'preprocessor': PreprocessorDummy</strong><br><i>BrickNotTrainable</i>):::BrickNotTrainable
+    backbone(<strong>'backbone': TinyModel</strong><br><i>BrickTrainable</i>):::BrickTrainable
+    head(<strong>'head': ClassifierDummy</strong><br><i>BrickTrainable</i>):::BrickTrainable
+    loss(<strong>'loss': CrossEntropyLoss</strong><br><i>BrickLoss</i>):::BrickLoss
     
     %% Draw input and outputs
     raw_images:::input --> preprocessor
     targets:::input --> loss
     
     %% Draw nodes and edges
     preprocessor --> |processed| backbone
@@ -344,21 +349,20 @@
     subgraph Legends
         input(input):::input
         output(output):::output
     end
 ```
 
 
-
 As demonstrated in above example, we can easily change the required inputs by change the model stage.
 That allows us to support two basic use cases:
 
 1) When labels/targets are available, we have the option of getting model prediction along with loss and metrics.
 
-2) When labels/targets are **not** available, we will only do basic model predictions. 
+2) When labels/targets are **not** available, we do only model predictions used for model inference/export.
 
 The mechanism of activating different parts of the model and making loss, metrics and visualizations part of the model recipe, 
 allows us to more easily investigate/debug/visualize model parts in a notebook or scratch scripts.
 
 
 ## Brick features: 
 
@@ -374,59 +378,62 @@
 To calculate metrics across a dataset, we heavily rely on concepts and functions used in the 
 [TorchMetrics](https://torchmetrics.readthedocs.io/en/stable/) library.
 
 The used of TorchMetrics in a brick collection is demonstrated in below code snippet. 
 
 ```python
 import torchvision
-from torchbricks.bag_of_bricks import ImageClassifier, Preprocessor, resnet_to_brick
-from torchbricks.bricks import BrickMetricSingle
+from torchbricks.bag_of_bricks.backbones import resnet_to_brick
+from torchbricks.bag_of_bricks.image_classification import ImageClassifier
+from torchbricks.bag_of_bricks.preprocessors import Preprocessor
+from torchbricks.bricks import BrickLoss, BrickMetricSingle
 from torchmetrics.classification import MulticlassAccuracy
 
 num_classes = 10
 resnet = torchvision.models.resnet18(weights=None, num_classes=num_classes)
-resnet_brick = resnet_to_brick(resnet=resnet,  input_name='normalized', output_name='features')
+resnet_brick = resnet_to_brick(resnet=resnet, input_name="normalized", output_name="features")
 n_features = resnet_brick.model.n_backbone_features
 bricks = {
-    'preprocessor': BrickNotTrainable(Preprocessor(), 
-                                      input_names=['raw'], 
-                                      output_names=['normalized']),
-    'backbone': resnet_brick,
-    'head': BrickTrainable(ImageClassifier(num_classes=num_classes, n_features=n_features),
-                           input_names=['features'], 
-                           output_names=['logits', 'probabilities', 'class_prediction']),
-    'accuracy': BrickMetricSingle(MulticlassAccuracy(num_classes=num_classes), 
-                                  input_names=['class_prediction', 'targets']),
-    'loss': BrickLoss(model=nn.CrossEntropyLoss(), 
-                      input_names=['logits', 'targets'], 
-                      output_names=['loss_ce'])
+    "preprocessor": BrickNotTrainable(Preprocessor(), input_names=["raw"], output_names=["normalized"]),
+    "backbone": resnet_brick,
+    "head": BrickTrainable(
+        ImageClassifier(num_classes=num_classes, n_features=n_features),
+        input_names=["features"],
+        output_names=["logits", "probabilities", "class_prediction"],
+    ),
+    "accuracy": BrickMetricSingle(MulticlassAccuracy(num_classes=num_classes), input_names=["class_prediction", "targets"]),
+    "loss": BrickLoss(model=nn.CrossEntropyLoss(), input_names=["logits", "targets"], output_names=["loss_ce"]),
 }
 brick_collection = BrickCollection(bricks)
 ```
 
-We will now use the brick collection above to simulate how a user can iterate over a dataset and 
-pass batches to the brick collection.
+We will now use the brick collection above to simulate how a user can iterate over a dataset.
 
 ```python
 # Simulate dataloader
 named_input_simulated = {"raw": batched_images, "targets": torch.ones((batch_size), dtype=torch.int64)}
 dataloader_simulated = [named_input_simulated for _ in range(5)]
 
 # Loop over the dataset
-for named_inputs in dataloader_simulated: # Simulates iterating over the dataset
-    named_outputs = brick_collection(named_inputs=named_inputs, stage=Stage.TRAIN)
+for named_inputs in dataloader_simulated:  # Simulates iterating over the dataset
+    named_outputs = brick_collection(named_inputs=named_inputs)
+    named_outputs_losses_only = brick_collection.extract_losses(named_outputs=named_outputs)
 
-metrics = brick_collection.summarize(stage=Stage.TRAIN, reset=True)
+metrics = brick_collection.summarize(reset=True)
 print(f"{named_outputs.keys()=}")
 # named_outputs.keys()=dict_keys(['raw', 'targets', 'stage', 'normalized', 'features', 'logits', 'probabilities', 'class_prediction', 'loss_ce'])
 print(f"{metrics=}")
 # metrics={'MulticlassAccuracy': tensor(0.)}
 ```
 
 For each iteration in our (simulated) dataset, we calculate model outputs, losses and metrics for each batch. 
+
+Losses are calculated and returned in `named_outputs` together with other model outputs. 
+We provide `extract_losses` as simple function to filter `named_outputs` and only return losses in a new dictionary. 
+
 Unlike other bricks, `BrickMetrics` will not (by default) output metrics for each batch. 
 Instead metrics are stored internally in `BrickMetricSingle` and only aggregated and return when
 the `summarize` function is called. In above example, metric is aggregated over 5 batches as summaries to a single value. 
 
 It is important to note that we set `reset=True` to reset the internal aggregation of metrics.  
 
 **Additional notes on metrics**
@@ -481,43 +488,42 @@
 
 ```python
 from typing import Dict
 
 from torchbricks.bricks import BrickInterface
 
 
-def create_image_classification_head(num_classes: int, in_channels: int, features_name: str, targets_name: str) -> Dict[str, BrickInterface]:
-    """Image classifier bricks: Classifier, loss and metrics """
+def create_image_classification_head(
+    num_classes: int, in_channels: int, features_name: str, targets_name: str
+) -> Dict[str, BrickInterface]:
+    """Image classifier bricks: Classifier, loss and metrics"""
     head = {
-        'classify': BrickTrainable(ImageClassifier(num_classes=num_classes, n_features=in_channels),
-                                   input_names=[features_name], 
-                                   output_names=['./logits', './probabilities', './class_prediction']),
-        'accuracy': BrickMetricSingle(MulticlassAccuracy(num_classes=num_classes), 
-                                      input_names=['./class_prediction', targets_name]),
-        'loss': BrickLoss(model=nn.CrossEntropyLoss(),
-                          input_names=['./logits', targets_name], 
-                          output_names=['./loss_ce'])
+        "classify": BrickTrainable(
+            ImageClassifier(num_classes=num_classes, n_features=in_channels),
+            input_names=[features_name],
+            output_names=["./logits", "./probabilities", "./class_prediction"],
+        ),
+        "accuracy": BrickMetricSingle(MulticlassAccuracy(num_classes=num_classes), input_names=["./class_prediction", targets_name]),
+        "loss": BrickLoss(model=nn.CrossEntropyLoss(), input_names=["./logits", targets_name], output_names=["./loss_ce"]),
     }
     return head
-
 ```
 
 We now create the full model containing a `preprocessor`, `backbone` and two independent heads called `head0` and `head1`.
 Each head is a dictionary of bricks, making our brick collection a nested dictionary. 
 
 ```python
+from torchbricks.graph_plotter import create_mermaid_dag_graph
 
 n_features = resnet_brick.model.n_backbone_features
 bricks = {
-    'preprocessor': BrickNotTrainable(Preprocessor(), 
-                                      input_names=['raw'], 
-                                      output_names=['normalized']),
-    'backbone': resnet_brick,
-    'head0': create_image_classification_head(num_classes=3, in_channels=n_features, features_name='features', targets_name='targets0'),
-    'head1': create_image_classification_head(num_classes=5, in_channels=n_features, features_name='features', targets_name='targets1'),
+    "preprocessor": BrickNotTrainable(Preprocessor(), input_names=["raw"], output_names=["normalized"]),
+    "backbone": resnet_brick,
+    "head0": create_image_classification_head(num_classes=3, in_channels=n_features, features_name="features", targets_name="targets0"),
+    "head1": create_image_classification_head(num_classes=5, in_channels=n_features, features_name="features", targets_name="targets1"),
 }
 brick_collections = BrickCollection(bricks)
 print(brick_collections)
 print(create_mermaid_dag_graph(brick_collections))
 ```
 
 Also demonstrated in above example is the use of relative input and output names. 
@@ -529,22 +535,22 @@
 
 We visualize above graph: 
 
 
 ```mermaid
 flowchart LR
     %% Brick definitions
-    preprocessor("<strong>BrickNotTrainable</strong><br><strong>preprocessor</strong>: Preprocessor"):::BrickNotTrainable
-    backbone("<strong>BrickTrainable</strong><br><strong>backbone</strong>: BackboneResnet"):::BrickTrainable
-    head0/classify("<strong>BrickTrainable</strong><br><strong>head0/classify</strong>: ImageClassifier"):::BrickTrainable
-    head0/accuracy("<strong>BrickMetricSingle</strong><br><strong>head0/accuracy</strong>: ['MulticlassAccuracy']"):::BrickMetricSingle
-    head0/loss("<strong>BrickLoss</strong><br><strong>head0/loss</strong>: CrossEntropyLoss"):::BrickLoss
-    head1/classify("<strong>BrickTrainable</strong><br><strong>head1/classify</strong>: ImageClassifier"):::BrickTrainable
-    head1/accuracy("<strong>BrickMetricSingle</strong><br><strong>head1/accuracy</strong>: ['MulticlassAccuracy']"):::BrickMetricSingle
-    head1/loss("<strong>BrickLoss</strong><br><strong>head1/loss</strong>: CrossEntropyLoss"):::BrickLoss
+    preprocessor(<strong>'preprocessor': Preprocessor</strong><br><i>BrickNotTrainable</i>):::BrickNotTrainable
+    backbone(<strong>'backbone': BackboneResnet</strong><br><i>BrickTrainable</i>):::BrickTrainable
+    head0/classify(<strong>'head0/classify': ImageClassifier</strong><br><i>BrickTrainable</i>):::BrickTrainable
+    head0/accuracy(<strong>'head0/accuracy': 'MulticlassAccuracy'</strong><br><i>BrickMetricSingle</i>):::BrickMetricSingle
+    head0/loss(<strong>'head0/loss': CrossEntropyLoss</strong><br><i>BrickLoss</i>):::BrickLoss
+    head1/classify(<strong>'head1/classify': ImageClassifier</strong><br><i>BrickTrainable</i>):::BrickTrainable
+    head1/accuracy(<strong>'head1/accuracy': 'MulticlassAccuracy'</strong><br><i>BrickMetricSingle</i>):::BrickMetricSingle
+    head1/loss(<strong>'head1/loss': CrossEntropyLoss</strong><br><i>BrickLoss</i>):::BrickLoss
     
     %% Draw input and outputs
     raw:::input --> preprocessor
     targets0:::input --> head0/accuracy
     targets0:::input --> head0/loss
     targets1:::input --> head1/accuracy
     targets1:::input --> head1/loss
@@ -579,32 +585,54 @@
     subgraph Legends
         input(input):::input
         output(output):::output
     end
 ```
 
 
+### Brick features: Save and loading bricks
+A brick collection can be saved and loaded as a regular pytorch `nn.Module`. For more information you can look up the official 
+pytorch guide on [Saving and Loading Models](https://pytorch.org/tutorials/beginner/saving_loading_models.html). 
+
+However, we have also added a brick collection specific saving/loading format. It uses a pytorch weight format, 
+but creates a model file for each brick and keeps files in a nested folder structure. 
+
+The idea is that a user can more easily add or remove weights to a specific model by simply moving around model files and folders.
+Time will tell, if this a useful abstraction or dead code. 
+
+But it looks like this: 
+
+```python
+path_model_folder = Path("build/bricks")
+
+# Saving model parameters brick-collection style
+brick_collections.save_bricks(path_model_folder=path_model_folder, exist_ok=True)
+
+print("Model files: ")
+print("\n".join(str(path) for path in path_model_folder.rglob("*.pt")))
+
+# Loading model parameters brick-collection style
+brick_collection.load_bricks(path_model_folder=path_model_folder)
+```
+
 ### Brick features: Export as ONNX
 To export a brick collection as onnx we provide the `export_bricks_as_onnx`-function. 
 
 Pass an example input (`named_input`) to trace a brick collection.
 Set `dynamic_batch_size=True` to support any batch size inputs and here we explicitly set `stage=Stage.EXPORT` - this is also 
 the default.
 
 ```python
-from torchbricks.brick_utils import export_bricks_as_onnx
+from torchbricks.brick_collection_utils import export_bricks_as_onnx
+
 path_build = Path("build")
 path_build.mkdir(exist_ok=True)
 path_onnx = path_build / "readme_model.onnx"
 
-export_bricks_as_onnx(path_onnx=path_onnx, 
-                      brick_collection=brick_collection, 
-                      named_inputs=named_inputs, 
-                      dynamic_batch_size=True, 
-                      stage=Stage.EXPORT)
+export_bricks_as_onnx(path_onnx=path_onnx, brick_collection=brick_collection, named_inputs=named_inputs, dynamic_batch_size=True)
 ```
 
 ### Brick features: Bag of bricks - reusable bricks modules
 Note also in above example we use bag-of-bricks to import commonly used `nn.Module`s 
 
 This includes a `Preprocessor`, `ImageClassifier` and `resnet_to_brick` to convert a torchvision resnet models to a backbone brick 
 without a classifier.
@@ -630,144 +658,126 @@
 as an example for you to use. 
 
 
 ```python
 from functools import partial
 from pathlib import Path
 
-import torchvision
 import pytorch_lightning as pl
-from utils_testing.lightning_module import LightningBrickCollection
+import torchvision
 from utils_testing.datamodule_cifar10 import CIFAR10DataModule
+from utils_testing.lightning_module import LightningBrickCollection
 
-experiment_name="CIFAR10"
+experiment_name = "CIFAR10"
 transform = torchvision.transforms.ToTensor()
-data_module = CIFAR10DataModule(data_dir='data', batch_size=5, num_workers=12, test_transforms=transform, train_transforms=transform)
-create_opimtizer_func = partial(torch.optim.SGD, lr=0.05, momentum=0.9, weight_decay=5e-4)
-bricks_lightning_module = LightningBrickCollection(path_experiments=Path("build") / "experiments",
-                                                   experiment_name=None,
-                                                   brick_collection=brick_collection,
-                                                   create_optimizers_func=create_opimtizer_func)
+data_module = CIFAR10DataModule(data_dir="data", batch_size=5, num_workers=12, test_transforms=transform, train_transforms=transform)
+create_optimizer_func = partial(torch.optim.SGD, lr=0.05, momentum=0.9, weight_decay=5e-4)
+bricks_lightning_module = LightningBrickCollection(
+    path_experiments=Path("build") / "experiments",
+    experiment_name=None,
+    brick_collection=brick_collection,
+    create_optimizers_func=create_optimizer_func,
+)
 
 trainer = pl.Trainer(max_epochs=1, limit_train_batches=2, limit_val_batches=2, limit_test_batches=2)
 # Train and test model by injecting 'bricks_lightning_module'
-# trainer.fit(bricks_lightning_module, datamodule=data_module)
-# trainer.test(bricks_lightning_module, datamodule=data_module)
+trainer.fit(bricks_lightning_module, datamodule=data_module)
+trainer.test(bricks_lightning_module, datamodule=data_module)
 ```
 
 
 ### Brick features: Pass all intermediate tensors to Brick
 By adding `'__all__'` to `input_names`, it is possible to access all tensors as a dictionary inside a brick module. 
 For production code, this may not be the best option, but this feature can be valuable during an exploration phase or 
 when doing some live debugging of a new model/module. 
 
-We will demonstrate in code by introducing a (dummy) module `VisualizeRawAndPreprocessed`.
+We will demonstrate in code by introducing a (dummy) module `MyNewPostProcessor`.
 
 *Note: It is just a dummy class, don't worry to much about the actual implementation.*
 
 The important thing to notice is that `input_names = ['__all__']` is used for our `visualizer`-brick to
 pass all tensors as a dictionary as an argument in the forward call. 
 
 ```python
-class VisualizeRawAndPreprocessed(torch.nn.Module):
+from typing import Any
+
+
+class MyNewPostProcessor(torch.nn.Module):
     def forward(self, named_inputs: Dict[str, Any]):
         ## Here `named_inputs` contains all intermediate tensors
-        image_raw_and_preprocessed = torch.concatenate((named_inputs["raw"], named_inputs["preprocessed"]), dim=3)
-        return image_raw_and_preprocessed
+        assert "raw" in named_inputs
+        assert "embedding" in named_inputs
+        return named_inputs["embedding"]
 
 
 bricks = {
-    'preprocessor': BrickNotTrainable(PreprocessorDummy(), input_names=['raw'],  output_names=['preprocessed']),
-    'backbone': BrickTrainable(TinyModel(n_channels=3, n_features=10), input_names=['preprocessed'], output_names=['embedding']),
-    'visualizer': BrickNotTrainable(VisualizeRawAndPreprocessed(), input_names = ['__all__'], output_names=["visualization"])
+    "backbone": BrickTrainable(TinyModel(n_channels=3, n_features=10), input_names=["raw"], output_names=["embedding"]),
+    "post_processor": BrickNotTrainable(MyNewPostProcessor(), input_names=["__all__"], output_names=["postprocessed"]),
 }
 brick_collection = BrickCollection(bricks)
-named_outputs = brick_collection(named_inputs={'raw': torch.rand((2, 3, 100, 200))}, stage=Stage.INFERENCE)
-```
-
-### Brick features: Using Stage Inside Module
-By passing in `stage` in `input_names` it is possible to change the program flow. 
-
-As demonstrated below want to alway resize the input to a specific size when the model is being exported.
-
-```python
-class Preprocessor(torch.nn.Module):
-    def forward(self, input_image: torch.Tensor, stage: Stage) -> str:
-        if stage in [Stage.EXPORT]:
-            input_image = torch.nn.functional.interpolate(input_image, size=(50,100))
-        return input_image/2
-
-
-brick_collection = BrickCollection({
-        "preprocessor": BrickNotTrainable(Preprocessor(), input_names=['raw', 'stage'], output_names=["processed"])
-    })
-named_inputs = {'raw': torch.rand((2, 3, 100, 200))}
-named_outputs = brick_collection(named_inputs=named_inputs, stage=Stage.EXPORT)
-assert list(named_outputs["processed"].shape[2:]) == [50, 100]
-
-named_outputs = brick_collection(named_inputs=named_inputs, stage=Stage.VALIDATION)
-assert list(named_outputs["processed"].shape[2:]) == [100, 200]
+named_outputs = brick_collection(named_inputs={"raw": torch.rand((2, 3, 100, 200))})
 ```
 
 ### Brick features: Visualizations in TorchBricks
 We provide `BrickPerImageVisualization` as base brick for doing visualizations in a brick collection. 
 The advantage of brick-based visualization is that it can be bundled together with a specific task/head. 
 
-Visualization/drawing functions typically operate on a single image and on non-`torch.Tensor` data types.
+Secondly, visualization/drawing functions typically operate on a single image and on non-`torch.Tensor` data types.
 E.g. Opencv/matplotlib uses `np.array` and pillow using `Image`. 
 
 (Torchvision actually has functions to draw rectangles, key-points and segmentation masks directly on `torch.Tensor`s -
 but it still operates on a single image and it has no option for rendering text).
 
-The goal of `BrickPerImageVisualization` is to convert batched tensors/data to per image data in a desired format
+The goal of `BrickPerImageVisualization` is to convert batched tensors/data to per image data in a desired format/datatype 
 and pass it to a draw function. Look up the documentation of `BrickPerImageVisualization` to see all options.
 
-First we create a callable to do per image visualizations. It can be a simple function, but in this example we create a callable 
-class to pass in class names and initialize font. 
+First we create a callable to do per image visualizations. It can be a simple function, but as demonstrated in below example, it 
+can also be a callable class. 
 
 The callable visualizes image classification predictions using pillow and requires two `np.array`s as input: 
 `input_image` of shape [H, W, C] and `target_prediction` [1].
 
 ```python
-
-from PIL import Image, ImageDraw, ImageFont
 import numpy as np
+from PIL import Image, ImageDraw, ImageFont
 from torchbricks.tensor_conversions import float2uint8
 
+
 class VisualizeImageClassification:
     def __init__(self, class_names: list, font_size: int = 50):
         self.class_names = class_names
-        self.font = ImageFont.truetype('tests/data/font_ASMAN.TTF', size=font_size) 
+        self.font = ImageFont.truetype("tests/data/font_ASMAN.TTF", size=font_size)
 
     def __call__(self, input_image: np.ndarray, target_prediction: np.ndarray) -> Image.Image:
         """Draws image classification results"""
-        assert input_image.ndim == 3 # Converted to single image channel last numpy array [H, W, C]
+        assert input_image.ndim == 3  # Converted to single image channel last numpy array [H, W, C]
         image = Image.fromarray(float2uint8(input_image))
-        draw = ImageDraw.Draw(image) 
-        draw.text((25, 25), text=self.class_names[target_prediction[0]], font = self.font) 
+        draw = ImageDraw.Draw(image)
+        draw.text((25, 25), text=self.class_names[target_prediction[0]], font=self.font)
         return image
 ```
 
-Our new drawing class `VisualizeImageClassification` is not passed to `BrickPerImageVisualization` and used in a brick collection.
+The drawing class `VisualizeImageClassification` is now passed to `BrickPerImageVisualization` and used in a brick collection.
 
 ```python
+from torchbricks.bag_of_bricks.brick_visualizer import BrickPerImageVisualization
 
-from torchbricks.brick_visualizer import BrickPerImageVisualization
 bricks = {
-    'visualizer': BrickPerImageVisualization(callable=VisualizeImageClassification(class_names=["cat", "dog"]), 
-                                          input_names=["input_image", "target"], 
-                                          output_names=["visualization"],
-                                          alive_stages=[Stage.INFERENCE])
+    "visualizer": BrickPerImageVisualization(
+        callable=VisualizeImageClassification(class_names=["cat", "dog"]),
+        input_names=["input_image", "target"],
+        output_names=["visualization"],
+    )
 }
 
-batched_inputs = {'input_image': torch.zeros((2, 3, 100, 200)), 'target': torch.tensor([0, 1], dtype=torch.int64)}
+batched_inputs = {"input_image": torch.zeros((2, 3, 100, 200)), "target": torch.tensor([0, 1], dtype=torch.int64)}
 brick_collection = BrickCollection(bricks)
-outputs = brick_collection(named_inputs=batched_inputs, stage=Stage.INFERENCE)
+outputs = brick_collection(named_inputs=batched_inputs)
 
-display(outputs["visualization"][0],  outputs["visualization"][1])
+display(outputs["visualization"][0], outputs["visualization"][1])
 ```
 
 `BrickPerImageProcessing` will by default convert a batch tensor of shape [B, C, H, W] to a channel last numpy image of shape [H, W, C]. 
 This is the default behavior, and it allows us in the callable of `VisualizeImageClassification` to operate directly on numpy arrays. 
 
 However for `BrickPerImageProcessing` a user has the option for unpacking batch data in a desired way as we will demonstrate in the 
 next example.
@@ -778,37 +788,43 @@
 other options of the `BrickPerImageVisualization` class. 
 
 *It is important to note that `visualize_image_classification_pillow` is passed as a callable, and we do not override functionality of 
 `BrickPerImageVisualization`. We only use it to simplify the constructor of `BrickVisualizeImageClassification`.
 
 ```python
 from typing import List
-from torchbricks.tensor_conversions import unpack_batched_tensor_to_pillow_images, function_composer, torch_to_numpy
+
+from torchbricks.tensor_conversions import function_composer, torch_to_numpy, unpack_batched_tensor_to_pillow_images
 
 
 class BrickVisualizeImageClassification(BrickPerImageVisualization):
     def __init__(self, input_image: str, target_name: str, class_names: List[str], output_name: str):
         self.class_names = class_names
-        self.font = ImageFont.truetype('tests/data/font_ASMAN.TTF', 50) 
-        super().__init__(callable=self.visualize_image_classification_pillow, input_names=[input_image, target_name], output_names=[output_name],
-                         unpack_functions_for_type={torch.Tensor: unpack_batched_tensor_to_pillow_images},
-                         unpack_functions_for_input_name={target_name: function_composer(torch_to_numpy, list)})
+        self.font = ImageFont.truetype("tests/data/font_ASMAN.TTF", 50)
+        super().__init__(
+            callable=self.visualize_image_classification_pillow,
+            input_names=[input_image, target_name],
+            output_names=[output_name],
+            unpack_functions_for_type={torch.Tensor: unpack_batched_tensor_to_pillow_images},
+            unpack_functions_for_input_name={target_name: function_composer(torch_to_numpy, list)},
+        )
 
     def visualize_image_classification_pillow(self, image: Image.Image, target_prediction: np.int64) -> Image.Image:
         """Draws image classification results"""
-        draw = ImageDraw.Draw(image) 
+        draw = ImageDraw.Draw(image)
 
-        draw.text((25, 25), text=self.class_names[target_prediction], font = self.font) 
+        draw.text((25, 25), text=self.class_names[target_prediction], font=self.font)
         return image
 
 
-visualizer = BrickVisualizeImageClassification(input_image="input_image", target_name="target", class_names=["cat", "dog"],
-                                               output_name="VisualizeImageClassification")
-batched_inputs = {'input_image': torch.zeros((2, 3, 100, 200)), 'target': torch.tensor([0, 1], dtype=torch.int64)}
-visualizer(batched_inputs, stage=Stage.INFERENCE)
+visualizer = BrickVisualizeImageClassification(
+    input_image="input_image", target_name="target", class_names=["cat", "dog"], output_name="VisualizeImageClassification"
+)
+batched_inputs = {"input_image": torch.zeros((2, 3, 100, 200)), "target": torch.tensor([0, 1], dtype=torch.int64)}
+visualizer(batched_inputs)
 ```
 
 Not unlike before, the callable (here `visualize_image_classification_pillow`) accepts an `Image.Image` image and an `int64` value directly
 and we are not required to do conversions inside the drawing function. 
 
 This can be achieved by using the two input arguments: 
 - `unpack_functions_for_type: Dict[Type, Callable]` specifying how each type should be unpacked.
@@ -820,95 +836,51 @@
 
 Specifying unpacking by input name (`unpack_functions_for_input_name`) will override the per type unpacking of `unpack_functions_for_type`. 
 
 
 ## Motivation
 
 The main motivation:
-- Sharable models: Packing model parts, metrics, loss-functions and visualization into a single recipe, makes the model more sharable to
-  other projects and supports sharing model for different use cases such as: Only inference, inference+visualizations and 
+- Sharable models: Packing model parts, metrics, loss-functions and visualizations into a single recipe, makes the model more sharable to
+  other projects and supports sharing models for different use cases such as: Only inference, inference+visualizations and 
   training+metrics+losses.
 - Shareable Parts: The brick collection encourage users to decouples parts and making also each part more sharable. 
-- Multiple tasks: Makes it easier to add and remove tasks. Each task can be expressed by model parts in a dictionary, we can easily add/remove them to a brick collection. 
+- Multiple tasks: Makes it easier to add and remove tasks. Each task can be expressed by model parts in a dictionary, 
+  we can easily add/remove them to a brick collection. 
 - By packing model modules, metrics, loss-functions and visualization into a single brick collection, we can more easily 
   inject it into your custom trainer and evaluation without doing per task/model modifications. 
 - Your model is **not** required to only return logits. Some training frameworks expect you to only return logits - values that go into 
   your loss function. Then at inference/test/evaluation you need to do post processing or pass additional outputs to 
   calculate metrics, do visualizations and make prediction human interpretable. It encourage unclear control flow (if/else statements) 
   in the model that depends on model stage. 
 - Using input and output names makes it easier to describe how parts are connected. Internally data is passed between bricks in a 
-  dictionary of any type - making in flexible. But for each module, you can specific and check types hints for input and output data to 
-  both improve readability and more production ready. 
+  dictionary of any type - making in flexible. But for each module, you can specific and add and check type hints for input and output 
+  data to both improve readability and make it more production ready. 
 - When I started making a framework suited for multiple tasks, I would passed dictionaries around to all modules and pull out tensors by
-  name in modules. Changing names would break stuff and it was not production ready. I also started using the typical 
-  backbone(encoder) / head(decoder) separation... But some heads may share a common neck. The decoder might also take different inputs and
+  name in each module. Book keeping names and updating names was messy. 
+  I also started using the typical backbone(encoder) / head(decoder) separation... But some heads may share a common neck. 
+  The decoder might also take different inputs and
   split into different representation and merge again... Also to avoid code duplication, I ended up during 
   multiple layers of inheritance for the decoder, making reuse bad and generally everything became too complicated and a new task would 
   require me to refactor the whole concept. Yes, it was probably not a super great attempt either, but it made me realize it should be 
   easier to make a new task and it should be easier to reuse parts. 
 
 
-
-
-## Why should I explicitly set the train, val or test stage
-
-MISSING
-
-
-
 <!-- #region -->
 ##
 
 ## What are we missing?
-
-
-- [x] ~~Proper~~ Added a link to `LightningBrickCollection` for other people to use
-- [x] Minor: BrickCollections supports passing a dictionary with BrickCollections. But we should also convert a nested dictionary into a nested brick collections
-- [x] Minor: Currently, `input_names` and `output_names` support positional arguments, but we should also support keyword arguments.
-- [x] Minor: Make Brick an abstract class
-- [x] Convert torchvision resnet models to only a backbone brick.
-- [x] Make readme a notebook
-- [x] Automatically convert jupyter notebook to `README.md`
-- [x] Remove README.md header
-- [x] Make an export to onnx function 
-- [x] Make it optional if gradients can be passed through NonTrainableBrick without weights being optimized
-- [x] Refactor Metrics: Create BrickMetricCollection and BrickSingleMetric and create flag to return metrics.
-- [x] Make brick base class with input_names, output_names and alive_stages - inherit this from other bricks. 
-  - Pros: We might include other non-torch modules later. 
-  - Do not necessarily pass a stage-object. Consider also passing it as a string so it can be handled correctly with scripting. 
-- [x] Update README.md to match the new bricks. 
-  - [x] Start with basic bricks example. 
-  - [x] Use loss-function to show that stage decided on what is being executed. 
-  - [x] Introduce metrics by it-self in another example
-- [x] Ensure that all examples in the `README.md` are working with easy to use modules. 
-- [x] Add typeguard
-- [x] Allow a brick to receive all named_inputs and add a test for it.
-- [x] Fix the release process. It should be as simple as running `make release`.
-- [x] Add onnx export example to the README.md
-- [x] Pretty print bricks
-- [x] Relative input/output names
-- [x] Test to verify that environment matches conda lock. The make command 'update-lock-file' should store a copy of 'environment.yml'
-      We will the have a test checking if the copy and the current version of `environment.yml` is the same.
-- [x] Add code coverage and tests passed badges to readme again
-- [x] Create brick-collection visualization tool ("mermaid?")
-- [x] Make DAG like functionality to check if inputs and outputs works for all model stages.
-- [x] Make Base Module PerImageProcessing as the basis for doing visualizations. 
-  - [ ] Consider caching unpacked data
-- [ ] Demonstrate model configuration with hydra
+- [ ] Demonstrate model configuration with hydra in this document
 - [ ] Make common Visualizations with pillow - not opencv to not blow up the required dependencies. ImageClassification, Segmentation, ObjectDetection
   - [ ] VideoModule to store data as a video
   - [ ] DisplayModule to show data
+- [ ] Consider caching unpacked data for `PerImageVisualizer`
 - [ ] Multiple named tensors caching module. 
 - [ ] Use pymy, pyright or pyre to do static code checks. 
-- [ ] Decide: Add stage as an internal state and not in the forward pass:
-  - Minor Pros: Tracing (to get onnx model) requires only torch.Tensors only as input - we avoid making an adapter class. 
-  - Minor Cons: State gets hidden away - implicit instead of explicit.
-  - Minor Pros: Similar to eval/training 
 - [ ] Collection of helper modules. Preprocessors, Backbones, Necks/Upsamplers, ImageClassification, SemanticSegmentation, ObjectDetection
-  - [x] All the modules in the README should be easy to import as actually modules.
   - [ ] Make common brick collections: BricksImageClassification, BricksSegmentation, BricksPointDetection, BricksObjectDetection
 - [ ] Support preparing data in the dataloader?
 - [ ] Support torch.jit.scripting? 
 
 ## How does it really work?
 ????
 
@@ -925,9 +897,7 @@
     poetry install
 
 ### Activating the environment
 
     conda activate torchbricks
 
 <!-- #endregion -->
-
-
```

### Comparing `torchbricks-0.1.0/README.md` & `torchbricks-0.3.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -23,110 +23,114 @@
 
 
 TorchBricks builds pytorch models using small reuseable and decoupled parts - we call them bricks. 
 
 The concept is simple and flexible and allows you to more easily combine, add or swap out parts of the model 
 (preprocessor, backbone, neck, head or post-processor), change the task or extend it with multiple tasks.
 
-TorchBricks is a compact recipe on both *how* model parts are connected and *when* parts are executed 
-during model stages such as training, validation, testing, inference and export.
+TorchBricks is a compact recipe on both *how* model parts are connected and *when* parts should be executed 
+during different model stages such as training, validation, testing, inference and export.
+
+TorchBricks is NOT a framework! - it just a thin abstraction on top of pytorch modules. 
 
 <!-- #region -->
 
 ## Install it with pip
 
 ```bash
 pip install torchbricks
 ```
 <!-- #endregion -->
 
 ## Bricks by example
 
-To demonstrate the the concepts of TorchBricks, we will first specify some dummy parts used of a regular image recognition model: 
+To demonstrate the the concepts of TorchBricks, we will first specify some dummy parts used in a regular image recognition model: 
 A preprocessor, a backbone and a head (in this case a classifier).
 *Note: Don't worry about the actually implementation of these modules - they are just dummy examples.*
 
 ```python
-from typing import Tuple, Any
+from typing import Tuple
+
 import torch
 from torch import nn
+
+
 class PreprocessorDummy(nn.Module):
     def forward(self, raw_input: torch.Tensor) -> torch.Tensor:
-        return raw_input/2
+        return raw_input / 2
+
 
 class TinyModel(nn.Module):
     def __init__(self, n_channels: int, n_features: int) -> None:
         super().__init__()
         self.conv = nn.Conv2d(n_channels, n_features, kernel_size=1)
 
     def forward(self, tensor: torch.Tensor) -> torch.Tensor:
         return self.conv(tensor)
 
+
 class ClassifierDummy(nn.Module):
     def __init__(self, num_classes: int, in_features: int) -> None:
         super().__init__()
         self.fc = nn.Linear(in_features, num_classes)
         self.avgpool = nn.AdaptiveAvgPool2d((1, 1))
         self.softmax = nn.Softmax(dim=1)
 
     def forward(self, tensor: torch.Tensor) -> Tuple[torch.Tensor, torch.Tensor]:
-        logits = self.fc(torch.flatten(self.avgpool(tensor), start_dim = 1))
+        logits = self.fc(torch.flatten(self.avgpool(tensor), start_dim=1))
         return logits, self.softmax(logits)
 ```
 
 
 ## Concept 1: Bricks are connected
 An important concept of TorchBricks is that it defines how modules are connected by specifying input and output names of
 each module similar to a DAG. 
 
 In below code snippet, we demonstrate how this would look for our dummy model. 
 
 ```python
-from torchbricks.bricks import BrickCollection, BrickTrainable, BrickNotTrainable, BrickLoss
-from torchbricks.bricks import Stage
-from torchbricks.graph_plotter import create_mermaid_dag_graph
+from torchbricks.brick_collection import BrickCollection
+from torchbricks.bricks import BrickNotTrainable, BrickTrainable
 
 bricks = {
-    'preprocessor': BrickNotTrainable(PreprocessorDummy(), 
-                                      input_names=['raw_images'], 
-                                      output_names=['processed']),
-    'backbone': BrickTrainable(TinyModel(n_channels=3, n_features=10), 
-                               input_names=['processed'], 
-                               output_names=['embedding']),
-    'head': BrickTrainable(ClassifierDummy(num_classes=3, in_features=10), 
-                           input_names=['embedding'], 
-                           output_names=['logits', "softmaxed"]),
+    "preprocessor": BrickNotTrainable(PreprocessorDummy(), input_names=["raw_images"], output_names=["processed"]),
+    "backbone": BrickTrainable(TinyModel(n_channels=3, n_features=10), input_names=["processed"], output_names=["embedding"]),
+    "head": BrickTrainable(ClassifierDummy(num_classes=3, in_features=10), input_names=["embedding"], output_names=["logits", "softmaxed"]),
 }
 brick_collection = BrickCollection(bricks)
+# print(create_mermaid_dag_graph(brick_collection))
 print(brick_collection)
 ```
 
 Each module is placed in a dictionary with a unique name and wrapped inside a brick with input and output names. 
 Input and output names specifies how outputs of one module is passed to inputs of the next module. 
 
+In above example, we use `BrickNotTrainable` to wrap modules that are shouldn't be trained (weights are fixed) and 
+`BrickTrainable` to wrap modules that are trainable (weights are updated on each training iteration). 
+
 Finally, the dictionary of bricks is passed to a `BrickCollection`. 
 
 Below we visualize how the brick collection connects bricks together. 
 
 
 ```mermaid
 flowchart LR
     %% Brick definitions
-    preprocessor("<strong>BrickNotTrainable</strong><br><strong>preprocessor</strong>: PreprocessorDummy"):::BrickNotTrainable
-    backbone("<strong>BrickTrainable</strong><br><strong>backbone</strong>: TinyModel"):::BrickTrainable
-    head("<strong>BrickTrainable</strong><br><strong>head</strong>: ClassifierDummy"):::BrickTrainable
+    preprocessor(<strong>'preprocessor': PreprocessorDummy</strong><br><i>BrickNotTrainable</i>):::BrickNotTrainable
+    backbone(<strong>'backbone': TinyModel</strong><br><i>BrickTrainable</i>):::BrickTrainable
+    head(<strong>'head': ClassifierDummy</strong><br><i>BrickTrainable</i>):::BrickTrainable
     
     %% Draw input and outputs
     raw_images:::input --> preprocessor
     
     %% Draw nodes and edges
     preprocessor --> |processed| backbone
     backbone --> |embedding| head
-    head --> softmaxed:::output
     head --> logits:::output
+    head --> softmaxed:::output
     
     %% Add styling
     classDef arrow stroke-width:0px,fill-opacity:0.0 
     classDef input stroke-width:0px,fill-opacity:0.3,fill:#22A699 
     classDef output stroke-width:0px,fill-opacity:0.3,fill:#F2BE22 
     classDef BrickNotTrainable stroke-width:0px,fill:#B56576 
     classDef BrickTrainable stroke-width:0px,fill:#6D597A 
@@ -137,26 +141,25 @@
         output(output):::output
     end
 ```
 *Graph is visualized using [mermaid](https://github.com/mermaid-js/mermaid) syntax.*
 *We provide the `create_mermaid_dag_graph`-function to create a brick collection visualization*
 
 
-The `BrickCollection` is used for executing above graph using `named_inputs`. 
-`named_inputs` is simply a dictionary with input name as key and input data as value.
+The `BrickCollection` is used for executing above graph by passing a dictionary with named input data (`named_inputs`). 
 
 For above brick collection, we only expect one named input called `raw_images`. 
 
 ```python
-batch_size=2
+batch_size = 2
 batched_images = torch.rand((batch_size, 3, 100, 200))
-named_inputs = {'raw_images': batched_images}
-named_outputs = brick_collection(named_inputs=named_inputs, stage=Stage.INFERENCE)
+named_inputs = {"raw_images": batched_images}
+named_outputs = brick_collection(named_inputs=named_inputs)
 print("Brick outputs:", named_outputs.keys())
-# Brick outputs: dict_keys(['raw_images', 'stage', 'processed', 'embedding', 'logits', 'softmaxed'])
+# Brick outputs: dict_keys(['raw_images', 'processed', 'embedding', 'logits', 'softmaxed'])
 ```
 
 The brick collection accepts a dictionary and returns a dictionary with all intermediated and resulting tensors. 
 
 Running our models as a brick collection has the following advantages:
 
 - A brick collection act as a regular `nn.Module` with all the familiar features: a `forward`-function, a `to`-function to move 
@@ -164,128 +167,130 @@
 - A brick collection is also a simple DAG, it accepts a dictionary with "named data" (we call this `named_inputs`), 
 executes each bricks and ensures that the outputs are passed to the inputs of other bricks with matching names. 
 Structuring the model as a DAG, makes it easy to add/remove outputs for a given module during development, add new modules to the
 collection and build completely new models from reusable parts. 
 - A brick collection is actually a dictionary (`nn.DictModule`). Allowing you to access, pop and update the 
   collection easily as a regular dictionary. It can also handle nested dictionary, allowing groups of bricks to be added/removed easily. 
 
-Note also that we set `stage=Stage.INFERENCE` to explicitly specify if we are doing training, validation, test or inference.
-Specifying a stage is important, if we want a module to act in a specific way during a specific stages.
-
-Leading us to the next section
-
-
-## Concept 2: Bricks can be dead (or alive)
-The second concept is to specify when bricks are alive - meaning we can specify at which stages (train, test, validation, inference 
-and export) a brick is active. 
-
-For other stage the brick will play dead - do nothing / return an empty dictionary. 
 
-Meaning that for different `stages`, we will have the option of creating a unique DAG for each model stage and
-we can control how a brick collection acts during all stages of a model. 
+## Concept 2: Bricks are grouped
+Another important concept is that bricks can be executed in groups. 
 
-In above example this is not very interesting - because a model will mostly have preprocessor, backbone and head active 
-during all stages.
-
-So we will demonstrate by adding a loss brick (`BrickLoss`) and specifying `alive_stages` for each brick.
+To demonstrate how and why this is useful, we have added the `group` argument to each brick and introduced `BrickLoss` brick.
 
 ```python
-num_classes = 3
+from torchbricks.bricks import BrickLoss
+
 bricks = {
-    'preprocessor': BrickNotTrainable(PreprocessorDummy(), 
-                                      input_names=['raw_images'], 
-                                      output_names=['processed'], 
-                                      alive_stages="all"),
-    'backbone': BrickTrainable(TinyModel(n_channels=num_classes, n_features=10), 
-                               input_names=['processed'], 
-                               output_names=['embedding'], 
-                               alive_stages="all"),
-    'head': BrickTrainable(ClassifierDummy(num_classes=num_classes, in_features=10), 
-                           input_names=['embedding'], 
-                           output_names=['logits', 'softmaxed'], 
-                           alive_stages="all"),
-    'loss': BrickLoss(model=nn.CrossEntropyLoss(), 
-                      input_names=['logits', 'targets'], 
-                      output_names=['loss_ce'], 
-                      alive_stages=[Stage.TRAIN, Stage.VALIDATION, Stage.TEST])
+    "preprocessor": BrickNotTrainable(PreprocessorDummy(), input_names=["raw_images"], output_names=["processed"], group="MODEL"),
+    "backbone": BrickTrainable(
+        TinyModel(n_channels=3, n_features=10), input_names=["processed"], output_names=["embedding"], group="MODEL"
+    ),
+    "head": BrickTrainable(
+        ClassifierDummy(num_classes=3, in_features=10),
+        input_names=["embedding"],
+        output_names=["logits", "softmaxed"],
+        group="MODEL",
+    ),
+    "loss": BrickLoss(model=nn.CrossEntropyLoss(), input_names=["logits", "targets"], output_names=["loss_ce"], group="LOSS"),
 }
 brick_collection = BrickCollection(bricks)
 
 print(brick_collection)
 # BrickCollection(
-#   (preprocessor): BrickNotTrainable(PreprocessorDummy, input_names=['raw_images'], output_names=['processed'], alive_stages=['TRAIN', 'VALIDATION', 'TEST', 'INFERENCE', 'EXPORT'])
-#   (backbone): BrickTrainable(TinyModel, input_names=['processed'], output_names=['embedding'], alive_stages=['TRAIN', 'VALIDATION', 'TEST', 'INFERENCE', 'EXPORT'])
-#   (head): BrickTrainable(ClassifierDummy, input_names=['embedding'], output_names=['logits', 'softmaxed'], alive_stages=['TRAIN', 'VALIDATION', 'TEST', 'INFERENCE', 'EXPORT'])
-#   (loss): BrickLoss(CrossEntropyLoss, input_names=['logits', 'targets'], output_names=['loss_ce'], alive_stages=['TRAIN', 'VALIDATION', 'TEST'])
+#   (preprocessor): BrickNotTrainable(PreprocessorDummy, input_names=['raw_images'], output_names=['processed'], groups={'MODEL'})
+#   (backbone): BrickTrainable(TinyModel, input_names=['processed'], output_names=['embedding'], groups={'MODEL'})
+#   (head): BrickTrainable(ClassifierDummy, input_names=['embedding'], output_names=['logits', 'softmaxed'], groups={'MODEL'})
+#   (loss): BrickLoss(CrossEntropyLoss, input_names=['logits', 'targets'], output_names=['loss_ce'], groups={'LOSS'})
 # )
-print(create_mermaid_dag_graph(brick_collection))
+# print(create_mermaid_dag_graph(brick_collection))
 ```
 
-We set `preprocessor`, `backbone` and `head` to be alive on all stages `alive_stages="all"` - this is the default behavior and
-similar to before. 
- 
-For `loss` we set `alive_stages=[Stage.TRAIN, Stage.VALIDATION, Stage.TEST]` to only calculate loss during train, validation and test
-stages. 
+With group names, it is now possible to execute desired subsets of the model 
+during execution by adding `groups`.
+
+Here is a few examples: 
+
+```python
+named_inputs = {"raw_images": batched_images, "targets": torch.ones((batch_size), dtype=torch.int64)}
+
+# With no groups specified, all bricks are executed
+named_outputs = brick_collection(named_inputs=named_inputs)
 
+# With groups specified, only bricks in the specified groups are executed
+named_outputs = brick_collection(named_inputs=named_inputs, groups={"MODEL"})
+```
 
+Groups are important concept in our model recipe as it allows us to specify how model will act during different model stages. 
 
-**Graph during inference and export:**
 
-During `Stage.INFERENCE` and `Stage.EXPORT`, the graph will look as before, the loss modules is dead and note only `raw_images` is 
-still the only required input
 
+**Brick collection during inference and export:**
 
+During `Inference` and `Export` model stages, we do not have ground truth labels and we wan to skip loss calculations. 
 
+```python
+# Execution only "MODEL" group bricks
+named_outputs = brick_collection(named_inputs=named_inputs, groups={"MODEL"})
+```
 
+The graph will look like this and note that the graph only requires `raw_images` as input:
 ```mermaid
 flowchart LR
     %% Brick definitions
-    preprocessor("<strong>BrickNotTrainable</strong><br><strong>preprocessor</strong>: PreprocessorDummy"):::BrickNotTrainable
-    backbone("<strong>BrickTrainable</strong><br><strong>backbone</strong>: TinyModel"):::BrickTrainable
-    head("<strong>BrickTrainable</strong><br><strong>head</strong>: ClassifierDummy"):::BrickTrainable
+    preprocessor(<strong>'preprocessor': PreprocessorDummy</strong><br><i>BrickNotTrainable</i>):::BrickNotTrainable
+    backbone(<strong>'backbone': TinyModel</strong><br><i>BrickTrainable</i>):::BrickTrainable
+    head(<strong>'head': ClassifierDummy</strong><br><i>BrickTrainable</i>):::BrickTrainable
     
     %% Draw input and outputs
     raw_images:::input --> preprocessor
     
     %% Draw nodes and edges
     preprocessor --> |processed| backbone
     backbone --> |embedding| head
-    head --> softmaxed:::output
     head --> logits:::output
+    head --> softmaxed:::output
     
     %% Add styling
     classDef arrow stroke-width:0px,fill-opacity:0.0 
     classDef input stroke-width:0px,fill-opacity:0.3,fill:#22A699 
     classDef output stroke-width:0px,fill-opacity:0.3,fill:#F2BE22 
     classDef BrickNotTrainable stroke-width:0px,fill:#B56576 
     classDef BrickTrainable stroke-width:0px,fill:#6D597A 
     
     %% Add legends
     subgraph Legends
         input(input):::input
         output(output):::output
-        
     end
 ```
 
 
-**Graph during train, test and validation:**
+**Brick collection during train, test and validation:**
 
-During `Stage.TRAIN`, `Stage.VALIDATION` and `Stage.TEST`, the loss module is alive and note both `raw_images` and `targets` are required as inputs:
+During "Train", "Test" and "Validation", `targets` are available and we want to calculate loss to 
+both improve model and track loss curves. 
 
+```python
+# Execution all groups
+named_outputs = brick_collection(named_inputs=named_inputs)
 
+# Or execute explicitly "MODEL" and "LOSS" group bricks
+named_outputs = brick_collection(named_inputs=named_inputs, groups={"MODEL", "LOSS"})
+```
 
+The graph will look like this and note that the graph now requires `raw_images` and `targets` as input:
 
 ```mermaid
 flowchart LR
     %% Brick definitions
-    preprocessor("<strong>BrickNotTrainable</strong><br><strong>preprocessor</strong>: PreprocessorDummy"):::BrickNotTrainable
-    backbone("<strong>BrickTrainable</strong><br><strong>backbone</strong>: TinyModel"):::BrickTrainable
-    head("<strong>BrickTrainable</strong><br><strong>head</strong>: ClassifierDummy"):::BrickTrainable
-    loss("<strong>BrickLoss</strong><br><strong>loss</strong>: CrossEntropyLoss"):::BrickLoss
+    preprocessor(<strong>'preprocessor': PreprocessorDummy</strong><br><i>BrickNotTrainable</i>):::BrickNotTrainable
+    backbone(<strong>'backbone': TinyModel</strong><br><i>BrickTrainable</i>):::BrickTrainable
+    head(<strong>'head': ClassifierDummy</strong><br><i>BrickTrainable</i>):::BrickTrainable
+    loss(<strong>'loss': CrossEntropyLoss</strong><br><i>BrickLoss</i>):::BrickLoss
     
     %% Draw input and outputs
     raw_images:::input --> preprocessor
     targets:::input --> loss
     
     %% Draw nodes and edges
     preprocessor --> |processed| backbone
@@ -306,21 +311,20 @@
     subgraph Legends
         input(input):::input
         output(output):::output
     end
 ```
 
 
-
 As demonstrated in above example, we can easily change the required inputs by change the model stage.
 That allows us to support two basic use cases:
 
 1) When labels/targets are available, we have the option of getting model prediction along with loss and metrics.
 
-2) When labels/targets are **not** available, we will only do basic model predictions. 
+2) When labels/targets are **not** available, we do only model predictions used for model inference/export.
 
 The mechanism of activating different parts of the model and making loss, metrics and visualizations part of the model recipe, 
 allows us to more easily investigate/debug/visualize model parts in a notebook or scratch scripts.
 
 
 ## Brick features: 
 
@@ -336,59 +340,62 @@
 To calculate metrics across a dataset, we heavily rely on concepts and functions used in the 
 [TorchMetrics](https://torchmetrics.readthedocs.io/en/stable/) library.
 
 The used of TorchMetrics in a brick collection is demonstrated in below code snippet. 
 
 ```python
 import torchvision
-from torchbricks.bag_of_bricks import ImageClassifier, Preprocessor, resnet_to_brick
-from torchbricks.bricks import BrickMetricSingle
+from torchbricks.bag_of_bricks.backbones import resnet_to_brick
+from torchbricks.bag_of_bricks.image_classification import ImageClassifier
+from torchbricks.bag_of_bricks.preprocessors import Preprocessor
+from torchbricks.bricks import BrickLoss, BrickMetricSingle
 from torchmetrics.classification import MulticlassAccuracy
 
 num_classes = 10
 resnet = torchvision.models.resnet18(weights=None, num_classes=num_classes)
-resnet_brick = resnet_to_brick(resnet=resnet,  input_name='normalized', output_name='features')
+resnet_brick = resnet_to_brick(resnet=resnet, input_name="normalized", output_name="features")
 n_features = resnet_brick.model.n_backbone_features
 bricks = {
-    'preprocessor': BrickNotTrainable(Preprocessor(), 
-                                      input_names=['raw'], 
-                                      output_names=['normalized']),
-    'backbone': resnet_brick,
-    'head': BrickTrainable(ImageClassifier(num_classes=num_classes, n_features=n_features),
-                           input_names=['features'], 
-                           output_names=['logits', 'probabilities', 'class_prediction']),
-    'accuracy': BrickMetricSingle(MulticlassAccuracy(num_classes=num_classes), 
-                                  input_names=['class_prediction', 'targets']),
-    'loss': BrickLoss(model=nn.CrossEntropyLoss(), 
-                      input_names=['logits', 'targets'], 
-                      output_names=['loss_ce'])
+    "preprocessor": BrickNotTrainable(Preprocessor(), input_names=["raw"], output_names=["normalized"]),
+    "backbone": resnet_brick,
+    "head": BrickTrainable(
+        ImageClassifier(num_classes=num_classes, n_features=n_features),
+        input_names=["features"],
+        output_names=["logits", "probabilities", "class_prediction"],
+    ),
+    "accuracy": BrickMetricSingle(MulticlassAccuracy(num_classes=num_classes), input_names=["class_prediction", "targets"]),
+    "loss": BrickLoss(model=nn.CrossEntropyLoss(), input_names=["logits", "targets"], output_names=["loss_ce"]),
 }
 brick_collection = BrickCollection(bricks)
 ```
 
-We will now use the brick collection above to simulate how a user can iterate over a dataset and 
-pass batches to the brick collection.
+We will now use the brick collection above to simulate how a user can iterate over a dataset.
 
 ```python
 # Simulate dataloader
 named_input_simulated = {"raw": batched_images, "targets": torch.ones((batch_size), dtype=torch.int64)}
 dataloader_simulated = [named_input_simulated for _ in range(5)]
 
 # Loop over the dataset
-for named_inputs in dataloader_simulated: # Simulates iterating over the dataset
-    named_outputs = brick_collection(named_inputs=named_inputs, stage=Stage.TRAIN)
+for named_inputs in dataloader_simulated:  # Simulates iterating over the dataset
+    named_outputs = brick_collection(named_inputs=named_inputs)
+    named_outputs_losses_only = brick_collection.extract_losses(named_outputs=named_outputs)
 
-metrics = brick_collection.summarize(stage=Stage.TRAIN, reset=True)
+metrics = brick_collection.summarize(reset=True)
 print(f"{named_outputs.keys()=}")
 # named_outputs.keys()=dict_keys(['raw', 'targets', 'stage', 'normalized', 'features', 'logits', 'probabilities', 'class_prediction', 'loss_ce'])
 print(f"{metrics=}")
 # metrics={'MulticlassAccuracy': tensor(0.)}
 ```
 
 For each iteration in our (simulated) dataset, we calculate model outputs, losses and metrics for each batch. 
+
+Losses are calculated and returned in `named_outputs` together with other model outputs. 
+We provide `extract_losses` as simple function to filter `named_outputs` and only return losses in a new dictionary. 
+
 Unlike other bricks, `BrickMetrics` will not (by default) output metrics for each batch. 
 Instead metrics are stored internally in `BrickMetricSingle` and only aggregated and return when
 the `summarize` function is called. In above example, metric is aggregated over 5 batches as summaries to a single value. 
 
 It is important to note that we set `reset=True` to reset the internal aggregation of metrics.  
 
 **Additional notes on metrics**
@@ -443,43 +450,42 @@
 
 ```python
 from typing import Dict
 
 from torchbricks.bricks import BrickInterface
 
 
-def create_image_classification_head(num_classes: int, in_channels: int, features_name: str, targets_name: str) -> Dict[str, BrickInterface]:
-    """Image classifier bricks: Classifier, loss and metrics """
+def create_image_classification_head(
+    num_classes: int, in_channels: int, features_name: str, targets_name: str
+) -> Dict[str, BrickInterface]:
+    """Image classifier bricks: Classifier, loss and metrics"""
     head = {
-        'classify': BrickTrainable(ImageClassifier(num_classes=num_classes, n_features=in_channels),
-                                   input_names=[features_name], 
-                                   output_names=['./logits', './probabilities', './class_prediction']),
-        'accuracy': BrickMetricSingle(MulticlassAccuracy(num_classes=num_classes), 
-                                      input_names=['./class_prediction', targets_name]),
-        'loss': BrickLoss(model=nn.CrossEntropyLoss(),
-                          input_names=['./logits', targets_name], 
-                          output_names=['./loss_ce'])
+        "classify": BrickTrainable(
+            ImageClassifier(num_classes=num_classes, n_features=in_channels),
+            input_names=[features_name],
+            output_names=["./logits", "./probabilities", "./class_prediction"],
+        ),
+        "accuracy": BrickMetricSingle(MulticlassAccuracy(num_classes=num_classes), input_names=["./class_prediction", targets_name]),
+        "loss": BrickLoss(model=nn.CrossEntropyLoss(), input_names=["./logits", targets_name], output_names=["./loss_ce"]),
     }
     return head
-
 ```
 
 We now create the full model containing a `preprocessor`, `backbone` and two independent heads called `head0` and `head1`.
 Each head is a dictionary of bricks, making our brick collection a nested dictionary. 
 
 ```python
+from torchbricks.graph_plotter import create_mermaid_dag_graph
 
 n_features = resnet_brick.model.n_backbone_features
 bricks = {
-    'preprocessor': BrickNotTrainable(Preprocessor(), 
-                                      input_names=['raw'], 
-                                      output_names=['normalized']),
-    'backbone': resnet_brick,
-    'head0': create_image_classification_head(num_classes=3, in_channels=n_features, features_name='features', targets_name='targets0'),
-    'head1': create_image_classification_head(num_classes=5, in_channels=n_features, features_name='features', targets_name='targets1'),
+    "preprocessor": BrickNotTrainable(Preprocessor(), input_names=["raw"], output_names=["normalized"]),
+    "backbone": resnet_brick,
+    "head0": create_image_classification_head(num_classes=3, in_channels=n_features, features_name="features", targets_name="targets0"),
+    "head1": create_image_classification_head(num_classes=5, in_channels=n_features, features_name="features", targets_name="targets1"),
 }
 brick_collections = BrickCollection(bricks)
 print(brick_collections)
 print(create_mermaid_dag_graph(brick_collections))
 ```
 
 Also demonstrated in above example is the use of relative input and output names. 
@@ -491,22 +497,22 @@
 
 We visualize above graph: 
 
 
 ```mermaid
 flowchart LR
     %% Brick definitions
-    preprocessor("<strong>BrickNotTrainable</strong><br><strong>preprocessor</strong>: Preprocessor"):::BrickNotTrainable
-    backbone("<strong>BrickTrainable</strong><br><strong>backbone</strong>: BackboneResnet"):::BrickTrainable
-    head0/classify("<strong>BrickTrainable</strong><br><strong>head0/classify</strong>: ImageClassifier"):::BrickTrainable
-    head0/accuracy("<strong>BrickMetricSingle</strong><br><strong>head0/accuracy</strong>: ['MulticlassAccuracy']"):::BrickMetricSingle
-    head0/loss("<strong>BrickLoss</strong><br><strong>head0/loss</strong>: CrossEntropyLoss"):::BrickLoss
-    head1/classify("<strong>BrickTrainable</strong><br><strong>head1/classify</strong>: ImageClassifier"):::BrickTrainable
-    head1/accuracy("<strong>BrickMetricSingle</strong><br><strong>head1/accuracy</strong>: ['MulticlassAccuracy']"):::BrickMetricSingle
-    head1/loss("<strong>BrickLoss</strong><br><strong>head1/loss</strong>: CrossEntropyLoss"):::BrickLoss
+    preprocessor(<strong>'preprocessor': Preprocessor</strong><br><i>BrickNotTrainable</i>):::BrickNotTrainable
+    backbone(<strong>'backbone': BackboneResnet</strong><br><i>BrickTrainable</i>):::BrickTrainable
+    head0/classify(<strong>'head0/classify': ImageClassifier</strong><br><i>BrickTrainable</i>):::BrickTrainable
+    head0/accuracy(<strong>'head0/accuracy': 'MulticlassAccuracy'</strong><br><i>BrickMetricSingle</i>):::BrickMetricSingle
+    head0/loss(<strong>'head0/loss': CrossEntropyLoss</strong><br><i>BrickLoss</i>):::BrickLoss
+    head1/classify(<strong>'head1/classify': ImageClassifier</strong><br><i>BrickTrainable</i>):::BrickTrainable
+    head1/accuracy(<strong>'head1/accuracy': 'MulticlassAccuracy'</strong><br><i>BrickMetricSingle</i>):::BrickMetricSingle
+    head1/loss(<strong>'head1/loss': CrossEntropyLoss</strong><br><i>BrickLoss</i>):::BrickLoss
     
     %% Draw input and outputs
     raw:::input --> preprocessor
     targets0:::input --> head0/accuracy
     targets0:::input --> head0/loss
     targets1:::input --> head1/accuracy
     targets1:::input --> head1/loss
@@ -541,32 +547,54 @@
     subgraph Legends
         input(input):::input
         output(output):::output
     end
 ```
 
 
+### Brick features: Save and loading bricks
+A brick collection can be saved and loaded as a regular pytorch `nn.Module`. For more information you can look up the official 
+pytorch guide on [Saving and Loading Models](https://pytorch.org/tutorials/beginner/saving_loading_models.html). 
+
+However, we have also added a brick collection specific saving/loading format. It uses a pytorch weight format, 
+but creates a model file for each brick and keeps files in a nested folder structure. 
+
+The idea is that a user can more easily add or remove weights to a specific model by simply moving around model files and folders.
+Time will tell, if this a useful abstraction or dead code. 
+
+But it looks like this: 
+
+```python
+path_model_folder = Path("build/bricks")
+
+# Saving model parameters brick-collection style
+brick_collections.save_bricks(path_model_folder=path_model_folder, exist_ok=True)
+
+print("Model files: ")
+print("\n".join(str(path) for path in path_model_folder.rglob("*.pt")))
+
+# Loading model parameters brick-collection style
+brick_collection.load_bricks(path_model_folder=path_model_folder)
+```
+
 ### Brick features: Export as ONNX
 To export a brick collection as onnx we provide the `export_bricks_as_onnx`-function. 
 
 Pass an example input (`named_input`) to trace a brick collection.
 Set `dynamic_batch_size=True` to support any batch size inputs and here we explicitly set `stage=Stage.EXPORT` - this is also 
 the default.
 
 ```python
-from torchbricks.brick_utils import export_bricks_as_onnx
+from torchbricks.brick_collection_utils import export_bricks_as_onnx
+
 path_build = Path("build")
 path_build.mkdir(exist_ok=True)
 path_onnx = path_build / "readme_model.onnx"
 
-export_bricks_as_onnx(path_onnx=path_onnx, 
-                      brick_collection=brick_collection, 
-                      named_inputs=named_inputs, 
-                      dynamic_batch_size=True, 
-                      stage=Stage.EXPORT)
+export_bricks_as_onnx(path_onnx=path_onnx, brick_collection=brick_collection, named_inputs=named_inputs, dynamic_batch_size=True)
 ```
 
 ### Brick features: Bag of bricks - reusable bricks modules
 Note also in above example we use bag-of-bricks to import commonly used `nn.Module`s 
 
 This includes a `Preprocessor`, `ImageClassifier` and `resnet_to_brick` to convert a torchvision resnet models to a backbone brick 
 without a classifier.
@@ -592,144 +620,126 @@
 as an example for you to use. 
 
 
 ```python
 from functools import partial
 from pathlib import Path
 
-import torchvision
 import pytorch_lightning as pl
-from utils_testing.lightning_module import LightningBrickCollection
+import torchvision
 from utils_testing.datamodule_cifar10 import CIFAR10DataModule
+from utils_testing.lightning_module import LightningBrickCollection
 
-experiment_name="CIFAR10"
+experiment_name = "CIFAR10"
 transform = torchvision.transforms.ToTensor()
-data_module = CIFAR10DataModule(data_dir='data', batch_size=5, num_workers=12, test_transforms=transform, train_transforms=transform)
-create_opimtizer_func = partial(torch.optim.SGD, lr=0.05, momentum=0.9, weight_decay=5e-4)
-bricks_lightning_module = LightningBrickCollection(path_experiments=Path("build") / "experiments",
-                                                   experiment_name=None,
-                                                   brick_collection=brick_collection,
-                                                   create_optimizers_func=create_opimtizer_func)
+data_module = CIFAR10DataModule(data_dir="data", batch_size=5, num_workers=12, test_transforms=transform, train_transforms=transform)
+create_optimizer_func = partial(torch.optim.SGD, lr=0.05, momentum=0.9, weight_decay=5e-4)
+bricks_lightning_module = LightningBrickCollection(
+    path_experiments=Path("build") / "experiments",
+    experiment_name=None,
+    brick_collection=brick_collection,
+    create_optimizers_func=create_optimizer_func,
+)
 
 trainer = pl.Trainer(max_epochs=1, limit_train_batches=2, limit_val_batches=2, limit_test_batches=2)
 # Train and test model by injecting 'bricks_lightning_module'
-# trainer.fit(bricks_lightning_module, datamodule=data_module)
-# trainer.test(bricks_lightning_module, datamodule=data_module)
+trainer.fit(bricks_lightning_module, datamodule=data_module)
+trainer.test(bricks_lightning_module, datamodule=data_module)
 ```
 
 
 ### Brick features: Pass all intermediate tensors to Brick
 By adding `'__all__'` to `input_names`, it is possible to access all tensors as a dictionary inside a brick module. 
 For production code, this may not be the best option, but this feature can be valuable during an exploration phase or 
 when doing some live debugging of a new model/module. 
 
-We will demonstrate in code by introducing a (dummy) module `VisualizeRawAndPreprocessed`.
+We will demonstrate in code by introducing a (dummy) module `MyNewPostProcessor`.
 
 *Note: It is just a dummy class, don't worry to much about the actual implementation.*
 
 The important thing to notice is that `input_names = ['__all__']` is used for our `visualizer`-brick to
 pass all tensors as a dictionary as an argument in the forward call. 
 
 ```python
-class VisualizeRawAndPreprocessed(torch.nn.Module):
+from typing import Any
+
+
+class MyNewPostProcessor(torch.nn.Module):
     def forward(self, named_inputs: Dict[str, Any]):
         ## Here `named_inputs` contains all intermediate tensors
-        image_raw_and_preprocessed = torch.concatenate((named_inputs["raw"], named_inputs["preprocessed"]), dim=3)
-        return image_raw_and_preprocessed
+        assert "raw" in named_inputs
+        assert "embedding" in named_inputs
+        return named_inputs["embedding"]
 
 
 bricks = {
-    'preprocessor': BrickNotTrainable(PreprocessorDummy(), input_names=['raw'],  output_names=['preprocessed']),
-    'backbone': BrickTrainable(TinyModel(n_channels=3, n_features=10), input_names=['preprocessed'], output_names=['embedding']),
-    'visualizer': BrickNotTrainable(VisualizeRawAndPreprocessed(), input_names = ['__all__'], output_names=["visualization"])
+    "backbone": BrickTrainable(TinyModel(n_channels=3, n_features=10), input_names=["raw"], output_names=["embedding"]),
+    "post_processor": BrickNotTrainable(MyNewPostProcessor(), input_names=["__all__"], output_names=["postprocessed"]),
 }
 brick_collection = BrickCollection(bricks)
-named_outputs = brick_collection(named_inputs={'raw': torch.rand((2, 3, 100, 200))}, stage=Stage.INFERENCE)
-```
-
-### Brick features: Using Stage Inside Module
-By passing in `stage` in `input_names` it is possible to change the program flow. 
-
-As demonstrated below want to alway resize the input to a specific size when the model is being exported.
-
-```python
-class Preprocessor(torch.nn.Module):
-    def forward(self, input_image: torch.Tensor, stage: Stage) -> str:
-        if stage in [Stage.EXPORT]:
-            input_image = torch.nn.functional.interpolate(input_image, size=(50,100))
-        return input_image/2
-
-
-brick_collection = BrickCollection({
-        "preprocessor": BrickNotTrainable(Preprocessor(), input_names=['raw', 'stage'], output_names=["processed"])
-    })
-named_inputs = {'raw': torch.rand((2, 3, 100, 200))}
-named_outputs = brick_collection(named_inputs=named_inputs, stage=Stage.EXPORT)
-assert list(named_outputs["processed"].shape[2:]) == [50, 100]
-
-named_outputs = brick_collection(named_inputs=named_inputs, stage=Stage.VALIDATION)
-assert list(named_outputs["processed"].shape[2:]) == [100, 200]
+named_outputs = brick_collection(named_inputs={"raw": torch.rand((2, 3, 100, 200))})
 ```
 
 ### Brick features: Visualizations in TorchBricks
 We provide `BrickPerImageVisualization` as base brick for doing visualizations in a brick collection. 
 The advantage of brick-based visualization is that it can be bundled together with a specific task/head. 
 
-Visualization/drawing functions typically operate on a single image and on non-`torch.Tensor` data types.
+Secondly, visualization/drawing functions typically operate on a single image and on non-`torch.Tensor` data types.
 E.g. Opencv/matplotlib uses `np.array` and pillow using `Image`. 
 
 (Torchvision actually has functions to draw rectangles, key-points and segmentation masks directly on `torch.Tensor`s -
 but it still operates on a single image and it has no option for rendering text).
 
-The goal of `BrickPerImageVisualization` is to convert batched tensors/data to per image data in a desired format
+The goal of `BrickPerImageVisualization` is to convert batched tensors/data to per image data in a desired format/datatype 
 and pass it to a draw function. Look up the documentation of `BrickPerImageVisualization` to see all options.
 
-First we create a callable to do per image visualizations. It can be a simple function, but in this example we create a callable 
-class to pass in class names and initialize font. 
+First we create a callable to do per image visualizations. It can be a simple function, but as demonstrated in below example, it 
+can also be a callable class. 
 
 The callable visualizes image classification predictions using pillow and requires two `np.array`s as input: 
 `input_image` of shape [H, W, C] and `target_prediction` [1].
 
 ```python
-
-from PIL import Image, ImageDraw, ImageFont
 import numpy as np
+from PIL import Image, ImageDraw, ImageFont
 from torchbricks.tensor_conversions import float2uint8
 
+
 class VisualizeImageClassification:
     def __init__(self, class_names: list, font_size: int = 50):
         self.class_names = class_names
-        self.font = ImageFont.truetype('tests/data/font_ASMAN.TTF', size=font_size) 
+        self.font = ImageFont.truetype("tests/data/font_ASMAN.TTF", size=font_size)
 
     def __call__(self, input_image: np.ndarray, target_prediction: np.ndarray) -> Image.Image:
         """Draws image classification results"""
-        assert input_image.ndim == 3 # Converted to single image channel last numpy array [H, W, C]
+        assert input_image.ndim == 3  # Converted to single image channel last numpy array [H, W, C]
         image = Image.fromarray(float2uint8(input_image))
-        draw = ImageDraw.Draw(image) 
-        draw.text((25, 25), text=self.class_names[target_prediction[0]], font = self.font) 
+        draw = ImageDraw.Draw(image)
+        draw.text((25, 25), text=self.class_names[target_prediction[0]], font=self.font)
         return image
 ```
 
-Our new drawing class `VisualizeImageClassification` is not passed to `BrickPerImageVisualization` and used in a brick collection.
+The drawing class `VisualizeImageClassification` is now passed to `BrickPerImageVisualization` and used in a brick collection.
 
 ```python
+from torchbricks.bag_of_bricks.brick_visualizer import BrickPerImageVisualization
 
-from torchbricks.brick_visualizer import BrickPerImageVisualization
 bricks = {
-    'visualizer': BrickPerImageVisualization(callable=VisualizeImageClassification(class_names=["cat", "dog"]), 
-                                          input_names=["input_image", "target"], 
-                                          output_names=["visualization"],
-                                          alive_stages=[Stage.INFERENCE])
+    "visualizer": BrickPerImageVisualization(
+        callable=VisualizeImageClassification(class_names=["cat", "dog"]),
+        input_names=["input_image", "target"],
+        output_names=["visualization"],
+    )
 }
 
-batched_inputs = {'input_image': torch.zeros((2, 3, 100, 200)), 'target': torch.tensor([0, 1], dtype=torch.int64)}
+batched_inputs = {"input_image": torch.zeros((2, 3, 100, 200)), "target": torch.tensor([0, 1], dtype=torch.int64)}
 brick_collection = BrickCollection(bricks)
-outputs = brick_collection(named_inputs=batched_inputs, stage=Stage.INFERENCE)
+outputs = brick_collection(named_inputs=batched_inputs)
 
-display(outputs["visualization"][0],  outputs["visualization"][1])
+display(outputs["visualization"][0], outputs["visualization"][1])
 ```
 
 `BrickPerImageProcessing` will by default convert a batch tensor of shape [B, C, H, W] to a channel last numpy image of shape [H, W, C]. 
 This is the default behavior, and it allows us in the callable of `VisualizeImageClassification` to operate directly on numpy arrays. 
 
 However for `BrickPerImageProcessing` a user has the option for unpacking batch data in a desired way as we will demonstrate in the 
 next example.
@@ -740,37 +750,43 @@
 other options of the `BrickPerImageVisualization` class. 
 
 *It is important to note that `visualize_image_classification_pillow` is passed as a callable, and we do not override functionality of 
 `BrickPerImageVisualization`. We only use it to simplify the constructor of `BrickVisualizeImageClassification`.
 
 ```python
 from typing import List
-from torchbricks.tensor_conversions import unpack_batched_tensor_to_pillow_images, function_composer, torch_to_numpy
+
+from torchbricks.tensor_conversions import function_composer, torch_to_numpy, unpack_batched_tensor_to_pillow_images
 
 
 class BrickVisualizeImageClassification(BrickPerImageVisualization):
     def __init__(self, input_image: str, target_name: str, class_names: List[str], output_name: str):
         self.class_names = class_names
-        self.font = ImageFont.truetype('tests/data/font_ASMAN.TTF', 50) 
-        super().__init__(callable=self.visualize_image_classification_pillow, input_names=[input_image, target_name], output_names=[output_name],
-                         unpack_functions_for_type={torch.Tensor: unpack_batched_tensor_to_pillow_images},
-                         unpack_functions_for_input_name={target_name: function_composer(torch_to_numpy, list)})
+        self.font = ImageFont.truetype("tests/data/font_ASMAN.TTF", 50)
+        super().__init__(
+            callable=self.visualize_image_classification_pillow,
+            input_names=[input_image, target_name],
+            output_names=[output_name],
+            unpack_functions_for_type={torch.Tensor: unpack_batched_tensor_to_pillow_images},
+            unpack_functions_for_input_name={target_name: function_composer(torch_to_numpy, list)},
+        )
 
     def visualize_image_classification_pillow(self, image: Image.Image, target_prediction: np.int64) -> Image.Image:
         """Draws image classification results"""
-        draw = ImageDraw.Draw(image) 
+        draw = ImageDraw.Draw(image)
 
-        draw.text((25, 25), text=self.class_names[target_prediction], font = self.font) 
+        draw.text((25, 25), text=self.class_names[target_prediction], font=self.font)
         return image
 
 
-visualizer = BrickVisualizeImageClassification(input_image="input_image", target_name="target", class_names=["cat", "dog"],
-                                               output_name="VisualizeImageClassification")
-batched_inputs = {'input_image': torch.zeros((2, 3, 100, 200)), 'target': torch.tensor([0, 1], dtype=torch.int64)}
-visualizer(batched_inputs, stage=Stage.INFERENCE)
+visualizer = BrickVisualizeImageClassification(
+    input_image="input_image", target_name="target", class_names=["cat", "dog"], output_name="VisualizeImageClassification"
+)
+batched_inputs = {"input_image": torch.zeros((2, 3, 100, 200)), "target": torch.tensor([0, 1], dtype=torch.int64)}
+visualizer(batched_inputs)
 ```
 
 Not unlike before, the callable (here `visualize_image_classification_pillow`) accepts an `Image.Image` image and an `int64` value directly
 and we are not required to do conversions inside the drawing function. 
 
 This can be achieved by using the two input arguments: 
 - `unpack_functions_for_type: Dict[Type, Callable]` specifying how each type should be unpacked.
@@ -782,95 +798,51 @@
 
 Specifying unpacking by input name (`unpack_functions_for_input_name`) will override the per type unpacking of `unpack_functions_for_type`. 
 
 
 ## Motivation
 
 The main motivation:
-- Sharable models: Packing model parts, metrics, loss-functions and visualization into a single recipe, makes the model more sharable to
-  other projects and supports sharing model for different use cases such as: Only inference, inference+visualizations and 
+- Sharable models: Packing model parts, metrics, loss-functions and visualizations into a single recipe, makes the model more sharable to
+  other projects and supports sharing models for different use cases such as: Only inference, inference+visualizations and 
   training+metrics+losses.
 - Shareable Parts: The brick collection encourage users to decouples parts and making also each part more sharable. 
-- Multiple tasks: Makes it easier to add and remove tasks. Each task can be expressed by model parts in a dictionary, we can easily add/remove them to a brick collection. 
+- Multiple tasks: Makes it easier to add and remove tasks. Each task can be expressed by model parts in a dictionary, 
+  we can easily add/remove them to a brick collection. 
 - By packing model modules, metrics, loss-functions and visualization into a single brick collection, we can more easily 
   inject it into your custom trainer and evaluation without doing per task/model modifications. 
 - Your model is **not** required to only return logits. Some training frameworks expect you to only return logits - values that go into 
   your loss function. Then at inference/test/evaluation you need to do post processing or pass additional outputs to 
   calculate metrics, do visualizations and make prediction human interpretable. It encourage unclear control flow (if/else statements) 
   in the model that depends on model stage. 
 - Using input and output names makes it easier to describe how parts are connected. Internally data is passed between bricks in a 
-  dictionary of any type - making in flexible. But for each module, you can specific and check types hints for input and output data to 
-  both improve readability and more production ready. 
+  dictionary of any type - making in flexible. But for each module, you can specific and add and check type hints for input and output 
+  data to both improve readability and make it more production ready. 
 - When I started making a framework suited for multiple tasks, I would passed dictionaries around to all modules and pull out tensors by
-  name in modules. Changing names would break stuff and it was not production ready. I also started using the typical 
-  backbone(encoder) / head(decoder) separation... But some heads may share a common neck. The decoder might also take different inputs and
+  name in each module. Book keeping names and updating names was messy. 
+  I also started using the typical backbone(encoder) / head(decoder) separation... But some heads may share a common neck. 
+  The decoder might also take different inputs and
   split into different representation and merge again... Also to avoid code duplication, I ended up during 
   multiple layers of inheritance for the decoder, making reuse bad and generally everything became too complicated and a new task would 
   require me to refactor the whole concept. Yes, it was probably not a super great attempt either, but it made me realize it should be 
   easier to make a new task and it should be easier to reuse parts. 
 
 
-
-
-## Why should I explicitly set the train, val or test stage
-
-MISSING
-
-
-
 <!-- #region -->
 ##
 
 ## What are we missing?
-
-
-- [x] ~~Proper~~ Added a link to `LightningBrickCollection` for other people to use
-- [x] Minor: BrickCollections supports passing a dictionary with BrickCollections. But we should also convert a nested dictionary into a nested brick collections
-- [x] Minor: Currently, `input_names` and `output_names` support positional arguments, but we should also support keyword arguments.
-- [x] Minor: Make Brick an abstract class
-- [x] Convert torchvision resnet models to only a backbone brick.
-- [x] Make readme a notebook
-- [x] Automatically convert jupyter notebook to `README.md`
-- [x] Remove README.md header
-- [x] Make an export to onnx function 
-- [x] Make it optional if gradients can be passed through NonTrainableBrick without weights being optimized
-- [x] Refactor Metrics: Create BrickMetricCollection and BrickSingleMetric and create flag to return metrics.
-- [x] Make brick base class with input_names, output_names and alive_stages - inherit this from other bricks. 
-  - Pros: We might include other non-torch modules later. 
-  - Do not necessarily pass a stage-object. Consider also passing it as a string so it can be handled correctly with scripting. 
-- [x] Update README.md to match the new bricks. 
-  - [x] Start with basic bricks example. 
-  - [x] Use loss-function to show that stage decided on what is being executed. 
-  - [x] Introduce metrics by it-self in another example
-- [x] Ensure that all examples in the `README.md` are working with easy to use modules. 
-- [x] Add typeguard
-- [x] Allow a brick to receive all named_inputs and add a test for it.
-- [x] Fix the release process. It should be as simple as running `make release`.
-- [x] Add onnx export example to the README.md
-- [x] Pretty print bricks
-- [x] Relative input/output names
-- [x] Test to verify that environment matches conda lock. The make command 'update-lock-file' should store a copy of 'environment.yml'
-      We will the have a test checking if the copy and the current version of `environment.yml` is the same.
-- [x] Add code coverage and tests passed badges to readme again
-- [x] Create brick-collection visualization tool ("mermaid?")
-- [x] Make DAG like functionality to check if inputs and outputs works for all model stages.
-- [x] Make Base Module PerImageProcessing as the basis for doing visualizations. 
-  - [ ] Consider caching unpacked data
-- [ ] Demonstrate model configuration with hydra
+- [ ] Demonstrate model configuration with hydra in this document
 - [ ] Make common Visualizations with pillow - not opencv to not blow up the required dependencies. ImageClassification, Segmentation, ObjectDetection
   - [ ] VideoModule to store data as a video
   - [ ] DisplayModule to show data
+- [ ] Consider caching unpacked data for `PerImageVisualizer`
 - [ ] Multiple named tensors caching module. 
 - [ ] Use pymy, pyright or pyre to do static code checks. 
-- [ ] Decide: Add stage as an internal state and not in the forward pass:
-  - Minor Pros: Tracing (to get onnx model) requires only torch.Tensors only as input - we avoid making an adapter class. 
-  - Minor Cons: State gets hidden away - implicit instead of explicit.
-  - Minor Pros: Similar to eval/training 
 - [ ] Collection of helper modules. Preprocessors, Backbones, Necks/Upsamplers, ImageClassification, SemanticSegmentation, ObjectDetection
-  - [x] All the modules in the README should be easy to import as actually modules.
   - [ ] Make common brick collections: BricksImageClassification, BricksSegmentation, BricksPointDetection, BricksObjectDetection
 - [ ] Support preparing data in the dataloader?
 - [ ] Support torch.jit.scripting? 
 
 ## How does it really work?
 ????
 
@@ -887,9 +859,7 @@
     poetry install
 
 ### Activating the environment
 
     conda activate torchbricks
 
 <!-- #endregion -->
-
-
```

### Comparing `torchbricks-0.1.0/pyproject.toml` & `torchbricks-0.3.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,16 @@
-[flake8]
-max-line-length = 140
-
 [tool.ruff]
+extend-include = ["*.ipynb"]
 line-length = 140
-select = ["C4", "E", "F","B", "I", "W", "RUF"]
+select = ["C4", "E", "F","B", "I", "W", "RUF", "Q"]
 
 [project]
 name = "torchbricks"
-version = "0.1.0"
-description = "Decoupled and modular approach to building multi-task ML models"
+version = "0.3.0"
+description = "Decoupled and modular approach to building multi-task ML models using a single model recipe for all model stages"
 readme = "README.md"
 authors = [{ name = "Peter Hviid Christiansen", email = "PeterHviidChristiansen@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
@@ -27,15 +25,15 @@
 requires-python = ">=3.7"
 
 [project.urls]
 Homepage = "https://github.com/pete-machine/torchbricks"
 
 # bumpver update --patch | --minor | --major --dry
 [tool.bumpver]
-current_version = "0.1.0"
+current_version = "0.3.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message  = "Bump version {old_version} -> {new_version}"
 commit          = true
 tag             = true
 push            = false
 
 [tool.bumpver.file_patterns]  # Specify all files containging version-numbers
```

### Comparing `torchbricks-0.1.0/src/torchbricks/brick_visualizer.py` & `torchbricks-0.3.0/src/torchbricks/bag_of_bricks/brick_visualizer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,45 +1,50 @@
 from collections import Counter, defaultdict
-from typing import Callable, Dict, List, Optional, Union
+from typing import Callable, Dict, List, Optional, Set, Union
 
 import numpy as np
 import torch
-from typeguard import typechecked
-
-from torchbricks.bricks import BrickModule, Stage, use_default_style
+from torchbricks import brick_group
+from torchbricks.bricks import BrickModule, use_default_style
 from torchbricks.bricks_helper import name_callable_outputs
 from torchbricks.tensor_conversions import unpack_batched_array_to_arrays, unpack_batched_tensor_to_numpy_format
+from typeguard import typechecked
 
 UNPACK_NO_CONVERSION = {
-    torch.Tensor: list, # Unpack as list only [B, C, H, W] -> [C, H, W]
-    np.ndarray: unpack_batched_array_to_arrays, # Unpack as list only [B, H, W, C] -> [H, W, C]
+    torch.Tensor: list,  # Unpack as list only [B, C, H, W] -> [C, H, W]
+    np.ndarray: unpack_batched_array_to_arrays,  # Unpack as list only [B, H, W, C] -> [H, W, C]
 }
 
 UNPACK_TENSORS_TO_NDARRAYS = {
     torch.Tensor: unpack_batched_tensor_to_numpy_format,
     np.ndarray: unpack_batched_array_to_arrays,  # Unpack as list only
 }
 
+
 @typechecked
 class BrickPerImageVisualization(BrickModule):
     """
     Primarily used to visualize data per image.
     The callable-function is called for each image in the batch and the outputs are collected in a list.
 
     Brick to perform operations on a batched input to a list of unbatched inputs.
     Useful when during per image visualization and processing.
     """
-    style: Dict[str, str] = use_default_style({'fill' :'#5C677D'})
-    def __init__(self, callable: Callable,
-                 input_names: Union[List[str], Dict[str, str]],
-                 output_names: List[str],
-                 unpack_functions_for_type: Optional[Dict[type, Optional[Callable]]] = None,
-                 alive_stages: Union[List[Stage], str, None] = None,
-                 unpack_functions_for_input_name: Optional[Dict[str, Optional[Callable]]] = None,
-                 ):
+
+    style: Dict[str, str] = use_default_style({"fill": "#5C677D"})
+
+    def __init__(
+        self,
+        callable: Callable,
+        input_names: Union[List[str], Dict[str, str]],
+        output_names: List[str],
+        unpack_functions_for_type: Optional[Dict[type, Optional[Callable]]] = None,
+        group: Union[Set[str], List[str], str] = brick_group.VISUALIZATION,
+        unpack_functions_for_input_name: Optional[Dict[str, Optional[Callable]]] = None,
+    ):
         """
         Parameters
         ----------
         type_unpack_functions : Dict[type, Callable]
             Specifies type specific functions to unpack data.
             Example: To convert a torch.tensor of shape [B, C, H, W] to numpy.array of shape [B, H, W, C]
                 type_unpack_functions = {
@@ -55,59 +60,61 @@
                Converts a torch.tensor of shape [B, C, H, W] to numpy.array of shape [B, H, W, C]. This is then iterated over
                and the callable-function receives numpy array of shape [H, W, C].
             2) `type_unpack_functions=UNPACK_NO_CONVERSION` to keep torch tensors as they are.
                E.g. A torch tensor of shape [B, C, H, W] will keep type and shape. This is then iterated over
                and the callable-function receives a torch tensor of shape [C, H, W].
 
         """
-        alive_stages = alive_stages or [Stage.INFERENCE]
-        super().__init__(model=self.unpack_data,
-                         input_names=input_names,
-                         output_names=output_names,
-                         loss_output_names=[],
-                         alive_stages=alive_stages,
-                         calculate_gradients=False,
-                         trainable=False)
+        super().__init__(
+            model=self.unpack_data,
+            input_names=input_names,
+            output_names=output_names,
+            loss_output_names=[],
+            group=group,
+            calculate_gradients=False,
+            trainable=False,
+        )
 
         self.type_unpack_functions = unpack_functions_for_type or UNPACK_TENSORS_TO_NDARRAYS
         self.callable = callable
 
         self.input_name_unpack_functions = unpack_functions_for_input_name or {}
         input_names_list = self.input_names_as_list()
         input_names_to_unpack = list(self.input_name_unpack_functions)
-        assert set(input_names_to_unpack).issubset(input_names_list), (f'One or more {input_names_to_unpack=} is not an ',
-                                                              f'`input_names` of brick {input_names_list=}')
+        assert set(input_names_to_unpack).issubset(input_names_list), (
+            f"One or more {input_names_to_unpack=} is not an ",
+            f"`input_names` of brick {input_names_list=}",
+        )
 
     def unpack_data(self, *args, **kwargs):
         uses_keyword_args = len(kwargs) > 0
 
         if uses_keyword_args:
             function_kwargs = kwargs.values()
         else:
             function_kwargs = args
         named_data_batched = dict(zip(self.input_names_as_list(), function_kwargs))
         named_data_unpacked_as_lists = {}
         for input_name, input_to_unpack in named_data_batched.items():
-
             unpack_function = self.type_unpack_functions.get(type(input_to_unpack), None)
             if input_name in self.input_name_unpack_functions:  # input_name unpack functions are prioritized above type unpack functions
                 unpack_function = self.input_name_unpack_functions[input_name]
 
             if unpack_function is not None:
                 input_to_unpack = unpack_function(input_to_unpack)
             named_data_unpacked_as_lists[input_name] = input_to_unpack
 
         unpack_types = (list, tuple)
         batch_sizes = [len(unpacked) for unpacked in named_data_unpacked_as_lists.values() if isinstance(unpacked, unpack_types)]
         if len(batch_sizes) == 0:
-            raise ValueError(f'Can not estimate batch size from these inputs: {self.input_names_as_list()}')
+            raise ValueError(f"Can not estimate batch size from these inputs: {self.input_names_as_list()}")
 
         batch_size_counts = Counter(batch_sizes)
         if len(batch_size_counts) > 1:
-            raise ValueError(f'Batch size is not the same for all inputs: {self.input_names_as_list()}')
+            raise ValueError(f"Batch size is not the same for all inputs: {self.input_names_as_list()}")
 
         batch_size = batch_size_counts.most_common(1)[0][0]
         per_image_data = defaultdict(dict)
         for input_name, input_unpacked_as_list in named_data_unpacked_as_lists.items():
             safe_to_unpack = isinstance(input_unpacked_as_list, unpack_types) and (len(input_unpacked_as_list) == batch_size)
             if safe_to_unpack:
                 for i_image, function_kwargs in enumerate(input_unpacked_as_list):
```

### Comparing `torchbricks-0.1.0/src/torchbricks/bricks_helper.py` & `torchbricks-0.3.0/src/torchbricks/bricks_helper.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,66 +1,88 @@
 from typing import Any, Callable, Dict, List, Union
 
 import torch
 from typeguard import typechecked
 
-__ALL__ = '__all__'
+__ALL__ = "__all__"
 
-def check_input_names(named_inputs: Dict[str, Any],
-                      input_names: List[str]):
+
+def check_input_names(named_inputs: Dict[str, Any], input_names: List[str]):
     expected_names = [*list(named_inputs), __ALL__]
     is_subset = set(input_names).issubset(expected_names)
-    assert is_subset, (f'Not all `{input_names=}` exists in `named_inputs={list(named_inputs)}`. The following expected names '
-                       f'{list(set(input_names).difference(named_inputs))} does not exist in the dictionary of `named_inputs`')
+    assert is_subset, (
+        f"Not all `{input_names=}` exists in `named_inputs={list(named_inputs)}`. The following expected names "
+        f"{list(set(input_names).difference(named_inputs))} does not exist in the dictionary of `named_inputs`"
+    )
 
 
 def positional_arguments_from_list_input_names(named_inputs: Dict[str, Any], input_names: List[str]) -> List:
     check_input_names(named_inputs=named_inputs, input_names=input_names)
     selected_inputs = [named_inputs if name == __ALL__ else named_inputs[name] for name in input_names]
     return selected_inputs
 
+
 def keyword_arguments_from_dict_input_names(named_inputs, input_names):
     input_name_keys = list(input_names.values())
     selected_inputs = positional_arguments_from_list_input_names(named_inputs, input_names=input_name_keys)
     argument_names_callable = list(input_names)
     arguments_and_values = dict(zip(argument_names_callable, selected_inputs))
     return arguments_and_values
 
 
-def name_callable_outputs(outputs: Any,
-                          output_names: List[str]) -> Dict[str, Any]:
+def name_callable_outputs(outputs: Any, output_names: List[str]) -> Dict[str, Any]:
     if outputs is None:
         if len(output_names) == 0:
             return {}
         else:
-            raise ValueError(f'No outputs was returned {outputs=} and we expected '
-                             f'"len(output_names)==0". However the following {output_names=} was specified')
+            raise ValueError(
+                f"No outputs was returned {outputs=} and we expected "
+                f'"len(output_names)==0". However the following {output_names=} was specified'
+            )
 
     if not isinstance(outputs, tuple):
-        outputs = (outputs, )
-    assert len(outputs) == len(output_names), (f'The number of specified output names {output_names=} '
-                                               f'does not match the actual number of outputs `{len(outputs)=}`')
+        outputs = (outputs,)
+    assert len(outputs) == len(output_names), (
+        f"The number of specified output names {output_names=} " f"does not match the actual number of outputs `{len(outputs)=}`"
+    )
     return dict(zip(output_names, outputs))
 
 
 @typechecked
-def named_input_and_outputs_callable(callable: Callable,
-                                     named_inputs: Dict[str, Any],
-                                     input_names: Union[List[str], Dict[str, str]],
-                                     output_names: List[str],
-                                     calculate_gradients: bool = True) -> Dict[str, Any]:
-
+def named_input_and_outputs_callable(
+    callable: Callable,
+    named_inputs: Dict[str, Any],
+    input_names: Union[List[str], Dict[str, str]],
+    output_names: List[str],
+    calculate_gradients: bool = True,
+) -> Dict[str, Any]:
     if isinstance(input_names, list):
         selected_inputs = positional_arguments_from_list_input_names(named_inputs, input_names=input_names)
         outputs = callable(*selected_inputs)
     elif isinstance(input_names, dict):
         arguments_and_values = keyword_arguments_from_dict_input_names(named_inputs, input_names)
         outputs = callable(**arguments_and_values)
     else:
-        raise ValueError(f'`input_names` is not as expected `{input_names=}` should be a list of input names `List[str]`, a mapping from '
-                         'input names to function arguments `Dict[str, str]` or `all`')
+        raise ValueError(
+            f"`input_names` is not as expected `{input_names=}` should be a list of input names `List[str]`, a mapping from "
+            "input names to function arguments `Dict[str, str]` or `all`"
+        )
     if calculate_gradients:
         outputs = name_callable_outputs(outputs=outputs, output_names=output_names)
     else:
         with torch.no_grad():
             outputs = name_callable_outputs(outputs=outputs, output_names=output_names)
     return outputs
+
+
+@typechecked
+def parse_argument_loss_output_name_indices(loss_output_names: Union[List[str], str], available_output_names: List[str]) -> List[int]:
+    if loss_output_names == "all":
+        loss_output_names = available_output_names
+    elif loss_output_names == "none":
+        loss_output_names = []
+
+    assert isinstance(loss_output_names, List), f"`loss_output_names` should be `all`, `none` or a list of strings. {loss_output_names=}"
+    assert set(loss_output_names).issubset(available_output_names), (
+        f"One or more {loss_output_names=} is not an " "`output_names` of brick {output_names=}"
+    )
+    return [available_output_names.index(loss_output_name) for loss_output_name in loss_output_names]
```

### Comparing `torchbricks-0.1.0/src/torchbricks/collection_utils.py` & `torchbricks-0.3.0/src/torchbricks/collection_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,27 @@
-
-
 from collections.abc import MutableMapping
 from typing import Any, Dict, Optional
 
-from torchbricks.bricks import BrickCollection
+from torchbricks.brick_collection import BrickCollection
 
 
 def _flatten_dict_gen(d, parent_key, sep):
     for k, v in d.items():
         new_key = parent_key + sep + k if parent_key else k
         if isinstance(v, BrickCollection):
             yield from flatten_dict(v, new_key, sep=sep).items()
         else:
             yield new_key, v
 
 
-def flatten_dict(d: MutableMapping, parent_key: str = '', sep: str = '.'):
+def flatten_dict(d: MutableMapping, parent_key: str = "", sep: str = "."):
     return dict(_flatten_dict_gen(d, parent_key, sep))
 
 
-def unflatten(d: Dict[str, Any], base: Optional[Dict[str, Any]] = None, sep: str = '/') -> Dict[str, Any]:
+def unflatten(d: Dict[str, Any], base: Optional[Dict[str, Any]] = None, sep: str = "/") -> Dict[str, Any]:
     """
     Convert any keys containing dotted paths to nested dicts
     https://stackoverflow.com/a/55545369
     """
     if base is None:
         base = {}
 
@@ -34,12 +32,12 @@
             *parts, key = key.split(sep)
 
             for part in parts:
                 root.setdefault(part, {})
                 root = root[part]
 
         if isinstance(value, dict):
-            value = unflatten(value, root.get(key, {}))
+            value = unflatten(value, root.get(key, {}), sep=sep)
 
         root[key] = value
 
     return base
```

### Comparing `torchbricks-0.1.0/src/torchbricks/custom_metrics.py` & `torchbricks-0.3.0/src/torchbricks/bag_of_bricks/custom_metrics.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 from torchmetrics import Metric
 from torchmetrics.utilities.data import dim_zero_cat
 from typeguard import typechecked
 
 
 @typechecked
 class ConcatenatePredictionAndTarget(Metric):
-    full_state_update = False  # Maybe this should be False?!
+    full_state_update = False  # https://lightning.ai/docs/torchmetrics/stable/pages/implement.html#internal-implementation-details
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
-        self.add_state('predictions', default=[], dist_reduce_fx='cat')
-        self.add_state('targets', default=[], dist_reduce_fx='cat')
+        self.add_state("predictions", default=[], dist_reduce_fx="cat")
+        self.add_state("targets", default=[], dist_reduce_fx="cat")
 
     def update(self, preds: torch.Tensor, target: torch.Tensor):
         assert preds.shape[0] == target.shape[0]  # Potentially remove this assertion if it is in your way.
 
         self.predictions.append(preds)
         self.targets.append(target)
```

### Comparing `torchbricks-0.1.0/src/torchbricks/dag.py` & `torchbricks-0.3.0/src/torchbricks/dag.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from dataclasses import dataclass
 from typing import Dict, List, Optional
 
-from torchbricks.bricks import BrickCollection, BrickInterface
+from torchbricks.brick_collection import BrickCollection
+from torchbricks.bricks import BrickInterface
 from torchbricks.collection_utils import flatten_dict
 
 
 @dataclass
 class NodeEdge:
     name: str
     to_node: Optional[str]
@@ -23,20 +24,20 @@
 class Dag:
     nodes: Dict[str, Node]
     inputs: List[NodeEdge]
     outputs: List[NodeEdge]
 
 
 def brick_collection_as_dag(brick_collections: BrickCollection) -> Dag:
-    brick_collections_flat = flatten_dict(brick_collections, sep = '/')
+    brick_collections_flat = flatten_dict(brick_collections, sep="/")
     all_input_names = set()
     all_output_names = set()
     dag_nodes = {}
     for node_name, node in brick_collections_flat.items():
-        dag_nodes[node_name] = Node(name=node_name, brick=node, edges = [])
+        dag_nodes[node_name] = Node(name=node_name, brick=node, edges=[])
         all_input_names = all_input_names.union(node.input_names)
         all_output_names = all_output_names.union(node.output_names)
 
     # Expected inputs and outputs
     only_input_names = all_input_names.difference(all_output_names)
     only_output_names = all_output_names.difference(all_input_names)
```

### Comparing `torchbricks-0.1.0/src/torchbricks/graph_plotter.py` & `torchbricks-0.3.0/src/torchbricks/graph_plotter.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,124 +1,122 @@
-
 from typing import Dict, Union
 
-from torchbricks.bricks import BrickCollection
+from torchbricks.brick_collection import BrickCollection
 from torchbricks.collection_utils import unflatten
 from torchbricks.dag import Dag, Node, brick_collection_as_dag
 
 
 def create_mermaid_dag_graph(brick_collection: BrickCollection, add_legends: bool = True) -> str:
     dag = brick_collection_as_dag(brick_collection)
     dag_builder = MermaidDagBuilder()
     dag_builder.start_graph()
-    dag_builder.add_comment('Brick definitions')
+    dag_builder.add_comment("Brick definitions")
     for node in dag.nodes.values():
         dag_builder.define_node(node)
 
     dag_builder.add_empty_line()
-    dag_builder.add_comment('Draw input and outputs')
+    dag_builder.add_comment("Draw input and outputs")
     for dag_input in dag.inputs:
-        string = f'{dag_input.name}:::input --> {dag_input.to_node}'
+        string = f"{dag_input.name}:::input --> {dag_input.to_node}"
         dag_builder.add_string(string=string)
 
     dag_builder.add_empty_line()
-    dag_builder.add_comment('Draw nodes and edges')
+    dag_builder.add_comment("Draw nodes and edges")
     dag_builder.draw_nodes_and_connections(dag_nodes=dag.nodes)
 
-
     dag_builder.add_empty_line()
-    dag_builder.add_comment('Add styling')
-    dag_builder.add_style_from_string(style_name='arrow', style='stroke-width:0px,fill-opacity:0.0', add_to_legends=False)
-    dag_builder.add_style_from_string(style_name='input', style='stroke-width:0px,fill-opacity:0.3,fill:#22A699')
-    dag_builder.add_style_from_string(style_name='output', style='stroke-width:0px,fill-opacity:0.3,fill:#F2BE22')
+    dag_builder.add_comment("Add styling")
+    dag_builder.add_style_from_string(style_name="arrow", style="stroke-width:0px,fill-opacity:0.0", add_to_legends=False)
+    dag_builder.add_style_from_string(style_name="input", style="stroke-width:0px,fill-opacity:0.3,fill:#22A699")
+    dag_builder.add_style_from_string(style_name="output", style="stroke-width:0px,fill-opacity:0.3,fill:#F2BE22")
     dag_builder.add_node_styles(dag=dag)
 
     if add_legends:
         dag_builder.add_empty_line()
-        dag_builder.add_comment('Add legends')
+        dag_builder.add_comment("Add legends")
         dag_builder.add_legends()
     return dag_builder.build()
 
 
 class MermaidDagBuilder:  # Pipeline pattern
     def __init__(self) -> None:
         self._graph_lines = []
         self._indent_level = 0
-        self._indent_char = '    '
+        self._indent_char = "    "
         self._added_legends = []
 
     def add_string(self, string: str, increase_indent_level: bool = False, decrease_indent_level: bool = False):
         if decrease_indent_level:
-            self._indent_level = self._indent_level-1
+            self._indent_level = self._indent_level - 1
 
-        indent_chars = self._indent_char*self._indent_level
+        indent_chars = self._indent_char * self._indent_level
         self._graph_lines.append(indent_chars + string)
         if increase_indent_level:
-            self._indent_level = self._indent_level+1
+            self._indent_level = self._indent_level + 1
 
     def add_empty_line(self):
-        self.add_string(string='')
+        self.add_string(string="")
 
     def add_comment(self, string: str):
-        self.add_string(f'%% {string}')
+        self.add_string(f"%% {string}")
 
     def start_graph(self):
-        self.add_string('flowchart LR', increase_indent_level=True)
+        self.add_string("flowchart LR", increase_indent_level=True)
 
     def define_node(self, brick: Node):
         module_name = brick.brick.get_module_name()
         style = brick.brick.get_brick_type()
-        brick_string = f'{brick.name}("<strong>{style}</strong><br><strong>{brick.name}</strong>: {module_name}"):::{style}'
+        brick_string = f"{brick.name}(<strong>'{brick.name}': {module_name}</strong><br><i>{style}</i>):::{style}"
         self.add_string(brick_string)
 
     def draw_nodes_and_connections(self, dag_nodes: Dict[str, Node]):
         nodes_nested = unflatten(dag_nodes)
         self._draw_nested_nodes_recursive(nodes_nested)
 
     def build(self, markdown=True) -> str:
         graph_lines = list(self._graph_lines)
         if markdown:
-            graph_lines.insert(0, '```mermaid')
-            graph_lines.append('```')
-        mermaid_str = '\n'.join(graph_lines)
+            graph_lines.insert(0, "```mermaid")
+            graph_lines.append("```")
+        mermaid_str = "\n".join(graph_lines)
         return mermaid_str
 
     def _draw_nested_nodes_recursive(self, nodes_nested: Dict[str, Union[Node, Dict]]):
         for node_or_subgraph_name, node_or_subgraph in nodes_nested.items():
             if isinstance(node_or_subgraph, dict):
                 subgraph = node_or_subgraph
-                self.add_string(f'subgraph {node_or_subgraph_name}', increase_indent_level=True)
+                self.add_string(f"subgraph {node_or_subgraph_name}", increase_indent_level=True)
                 self._draw_nested_nodes_recursive(subgraph)
-                self.add_string('end', decrease_indent_level=True)
+                self.add_string("end", decrease_indent_level=True)
             else:
                 node: Node = node_or_subgraph
                 for brick_connection in node.edges:
                     if brick_connection.to_node is None:
-                        string = f'{node.name} --> {brick_connection.name}:::output'
+                        string = f"{node.name} --> {brick_connection.name}:::output"
                     else:
-                        string = f'{node.name} --> |{brick_connection.name}| {brick_connection.to_node}'
+                        string = f"{node.name} --> |{brick_connection.name}| {brick_connection.to_node}"
                     self.add_string(string=string)
 
-    def add_style_from_string(self, style: str, style_name: str, add_to_legends: bool = True ):
+    def add_style_from_string(self, style: str, style_name: str, add_to_legends: bool = True):
         if add_to_legends:
             self._added_legends.append(style_name)
-        self.add_string(f'classDef {style_name} {style} ')
+        self.add_string(f"classDef {style_name} {style} ")
 
     def add_style_from_dict(self, style: Dict[str, str], style_name: str, add_to_legends: bool = True):
-        html_style = ','.join([f'{style_attr_name}:{style_attr_value}' for style_attr_name, style_attr_value in style.items()])
+        html_style = ",".join([f"{style_attr_name}:{style_attr_value}" for style_attr_name, style_attr_value in style.items()])
         self.add_style_from_string(style=html_style, style_name=style_name, add_to_legends=add_to_legends)
 
     def add_node_styles(self, dag: Dag, add_to_legends: bool = False):
         node_styles = set()
         for node in dag.nodes.values():
             style_name = node.brick.get_brick_type()
             if style_name in node_styles:
                 continue
             node_styles.add(style_name)
             style_name = node.brick.get_brick_type()
             self.add_style_from_dict(style=node.brick.style, style_name=style_name, add_to_legends=add_to_legends)
 
     def add_legends(self):
-        self.add_string('subgraph Legends', increase_indent_level=True)
+        self.add_string("subgraph Legends", increase_indent_level=True)
         for style in self._added_legends:
-            self.add_string(f'{style}({style}):::{style}')
-        self.add_string('end', decrease_indent_level=True)
+            self.add_string(f"{style}({style}):::{style}")
+        self.add_string("end", decrease_indent_level=True)
```

### Comparing `torchbricks-0.1.0/src/torchbricks/tensor_conversions.py` & `torchbricks-0.3.0/src/torchbricks/tensor_conversions.py`

 * *Files 5% similar despite different names*

```diff
@@ -46,16 +46,16 @@
 def unpack_batched_tensor_to_pillow_images(batched_tensor: torch.Tensor) -> List[Image.Image]:
     """
     Converts a batched tensor to list of pillow images
 
     Examples:
     - [B, 3, H, W] to list of Images
     """
-    assert batched_tensor.ndim == 4, f'Expected 4 dimensions, got {batched_tensor.ndim}'
-    assert batched_tensor.shape[1] == 3, f'Expected 3 channels, got {batched_tensor.shape[1]}'
+    assert batched_tensor.ndim == 4, f"Expected 4 dimensions, got {batched_tensor.ndim}"
+    assert batched_tensor.shape[1] == 3, f"Expected 3 channels, got {batched_tensor.shape[1]}"
     np_array = batched_tensor_to_batched_np_array_channel_last(batched_tensor)
     return [Image.fromarray(float2uint8(np_array)) for np_array in np_array]
 
 
 @typechecked
 def unpack_batched_array_to_arrays(array: np.ndarray) -> List[np.ndarray]:
     """
```

### Comparing `torchbricks-0.1.0/src/torchbricks.egg-info/PKG-INFO` & `torchbricks-0.3.0/src/torchbricks.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: torchbricks
-Version: 0.1.0
-Summary: Decoupled and modular approach to building multi-task ML models
+Version: 0.3.0
+Summary: Decoupled and modular approach to building multi-task ML models using a single model recipe for all model stages
 Author-email: Peter Hviid Christiansen <PeterHviidChristiansen@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Peter Christiansen
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -61,110 +61,114 @@
 
 
 TorchBricks builds pytorch models using small reuseable and decoupled parts - we call them bricks. 
 
 The concept is simple and flexible and allows you to more easily combine, add or swap out parts of the model 
 (preprocessor, backbone, neck, head or post-processor), change the task or extend it with multiple tasks.
 
-TorchBricks is a compact recipe on both *how* model parts are connected and *when* parts are executed 
-during model stages such as training, validation, testing, inference and export.
+TorchBricks is a compact recipe on both *how* model parts are connected and *when* parts should be executed 
+during different model stages such as training, validation, testing, inference and export.
+
+TorchBricks is NOT a framework! - it just a thin abstraction on top of pytorch modules. 
 
 <!-- #region -->
 
 ## Install it with pip
 
 ```bash
 pip install torchbricks
 ```
 <!-- #endregion -->
 
 ## Bricks by example
 
-To demonstrate the the concepts of TorchBricks, we will first specify some dummy parts used of a regular image recognition model: 
+To demonstrate the the concepts of TorchBricks, we will first specify some dummy parts used in a regular image recognition model: 
 A preprocessor, a backbone and a head (in this case a classifier).
 *Note: Don't worry about the actually implementation of these modules - they are just dummy examples.*
 
 ```python
-from typing import Tuple, Any
+from typing import Tuple
+
 import torch
 from torch import nn
+
+
 class PreprocessorDummy(nn.Module):
     def forward(self, raw_input: torch.Tensor) -> torch.Tensor:
-        return raw_input/2
+        return raw_input / 2
+
 
 class TinyModel(nn.Module):
     def __init__(self, n_channels: int, n_features: int) -> None:
         super().__init__()
         self.conv = nn.Conv2d(n_channels, n_features, kernel_size=1)
 
     def forward(self, tensor: torch.Tensor) -> torch.Tensor:
         return self.conv(tensor)
 
+
 class ClassifierDummy(nn.Module):
     def __init__(self, num_classes: int, in_features: int) -> None:
         super().__init__()
         self.fc = nn.Linear(in_features, num_classes)
         self.avgpool = nn.AdaptiveAvgPool2d((1, 1))
         self.softmax = nn.Softmax(dim=1)
 
     def forward(self, tensor: torch.Tensor) -> Tuple[torch.Tensor, torch.Tensor]:
-        logits = self.fc(torch.flatten(self.avgpool(tensor), start_dim = 1))
+        logits = self.fc(torch.flatten(self.avgpool(tensor), start_dim=1))
         return logits, self.softmax(logits)
 ```
 
 
 ## Concept 1: Bricks are connected
 An important concept of TorchBricks is that it defines how modules are connected by specifying input and output names of
 each module similar to a DAG. 
 
 In below code snippet, we demonstrate how this would look for our dummy model. 
 
 ```python
-from torchbricks.bricks import BrickCollection, BrickTrainable, BrickNotTrainable, BrickLoss
-from torchbricks.bricks import Stage
-from torchbricks.graph_plotter import create_mermaid_dag_graph
+from torchbricks.brick_collection import BrickCollection
+from torchbricks.bricks import BrickNotTrainable, BrickTrainable
 
 bricks = {
-    'preprocessor': BrickNotTrainable(PreprocessorDummy(), 
-                                      input_names=['raw_images'], 
-                                      output_names=['processed']),
-    'backbone': BrickTrainable(TinyModel(n_channels=3, n_features=10), 
-                               input_names=['processed'], 
-                               output_names=['embedding']),
-    'head': BrickTrainable(ClassifierDummy(num_classes=3, in_features=10), 
-                           input_names=['embedding'], 
-                           output_names=['logits', "softmaxed"]),
+    "preprocessor": BrickNotTrainable(PreprocessorDummy(), input_names=["raw_images"], output_names=["processed"]),
+    "backbone": BrickTrainable(TinyModel(n_channels=3, n_features=10), input_names=["processed"], output_names=["embedding"]),
+    "head": BrickTrainable(ClassifierDummy(num_classes=3, in_features=10), input_names=["embedding"], output_names=["logits", "softmaxed"]),
 }
 brick_collection = BrickCollection(bricks)
+# print(create_mermaid_dag_graph(brick_collection))
 print(brick_collection)
 ```
 
 Each module is placed in a dictionary with a unique name and wrapped inside a brick with input and output names. 
 Input and output names specifies how outputs of one module is passed to inputs of the next module. 
 
+In above example, we use `BrickNotTrainable` to wrap modules that are shouldn't be trained (weights are fixed) and 
+`BrickTrainable` to wrap modules that are trainable (weights are updated on each training iteration). 
+
 Finally, the dictionary of bricks is passed to a `BrickCollection`. 
 
 Below we visualize how the brick collection connects bricks together. 
 
 
 ```mermaid
 flowchart LR
     %% Brick definitions
-    preprocessor("<strong>BrickNotTrainable</strong><br><strong>preprocessor</strong>: PreprocessorDummy"):::BrickNotTrainable
-    backbone("<strong>BrickTrainable</strong><br><strong>backbone</strong>: TinyModel"):::BrickTrainable
-    head("<strong>BrickTrainable</strong><br><strong>head</strong>: ClassifierDummy"):::BrickTrainable
+    preprocessor(<strong>'preprocessor': PreprocessorDummy</strong><br><i>BrickNotTrainable</i>):::BrickNotTrainable
+    backbone(<strong>'backbone': TinyModel</strong><br><i>BrickTrainable</i>):::BrickTrainable
+    head(<strong>'head': ClassifierDummy</strong><br><i>BrickTrainable</i>):::BrickTrainable
     
     %% Draw input and outputs
     raw_images:::input --> preprocessor
     
     %% Draw nodes and edges
     preprocessor --> |processed| backbone
     backbone --> |embedding| head
-    head --> softmaxed:::output
     head --> logits:::output
+    head --> softmaxed:::output
     
     %% Add styling
     classDef arrow stroke-width:0px,fill-opacity:0.0 
     classDef input stroke-width:0px,fill-opacity:0.3,fill:#22A699 
     classDef output stroke-width:0px,fill-opacity:0.3,fill:#F2BE22 
     classDef BrickNotTrainable stroke-width:0px,fill:#B56576 
     classDef BrickTrainable stroke-width:0px,fill:#6D597A 
@@ -175,26 +179,25 @@
         output(output):::output
     end
 ```
 *Graph is visualized using [mermaid](https://github.com/mermaid-js/mermaid) syntax.*
 *We provide the `create_mermaid_dag_graph`-function to create a brick collection visualization*
 
 
-The `BrickCollection` is used for executing above graph using `named_inputs`. 
-`named_inputs` is simply a dictionary with input name as key and input data as value.
+The `BrickCollection` is used for executing above graph by passing a dictionary with named input data (`named_inputs`). 
 
 For above brick collection, we only expect one named input called `raw_images`. 
 
 ```python
-batch_size=2
+batch_size = 2
 batched_images = torch.rand((batch_size, 3, 100, 200))
-named_inputs = {'raw_images': batched_images}
-named_outputs = brick_collection(named_inputs=named_inputs, stage=Stage.INFERENCE)
+named_inputs = {"raw_images": batched_images}
+named_outputs = brick_collection(named_inputs=named_inputs)
 print("Brick outputs:", named_outputs.keys())
-# Brick outputs: dict_keys(['raw_images', 'stage', 'processed', 'embedding', 'logits', 'softmaxed'])
+# Brick outputs: dict_keys(['raw_images', 'processed', 'embedding', 'logits', 'softmaxed'])
 ```
 
 The brick collection accepts a dictionary and returns a dictionary with all intermediated and resulting tensors. 
 
 Running our models as a brick collection has the following advantages:
 
 - A brick collection act as a regular `nn.Module` with all the familiar features: a `forward`-function, a `to`-function to move 
@@ -202,128 +205,130 @@
 - A brick collection is also a simple DAG, it accepts a dictionary with "named data" (we call this `named_inputs`), 
 executes each bricks and ensures that the outputs are passed to the inputs of other bricks with matching names. 
 Structuring the model as a DAG, makes it easy to add/remove outputs for a given module during development, add new modules to the
 collection and build completely new models from reusable parts. 
 - A brick collection is actually a dictionary (`nn.DictModule`). Allowing you to access, pop and update the 
   collection easily as a regular dictionary. It can also handle nested dictionary, allowing groups of bricks to be added/removed easily. 
 
-Note also that we set `stage=Stage.INFERENCE` to explicitly specify if we are doing training, validation, test or inference.
-Specifying a stage is important, if we want a module to act in a specific way during a specific stages.
 
-Leading us to the next section
+## Concept 2: Bricks are grouped
+Another important concept is that bricks can be executed in groups. 
 
-
-## Concept 2: Bricks can be dead (or alive)
-The second concept is to specify when bricks are alive - meaning we can specify at which stages (train, test, validation, inference 
-and export) a brick is active. 
-
-For other stage the brick will play dead - do nothing / return an empty dictionary. 
-
-Meaning that for different `stages`, we will have the option of creating a unique DAG for each model stage and
-we can control how a brick collection acts during all stages of a model. 
-
-In above example this is not very interesting - because a model will mostly have preprocessor, backbone and head active 
-during all stages.
-
-So we will demonstrate by adding a loss brick (`BrickLoss`) and specifying `alive_stages` for each brick.
+To demonstrate how and why this is useful, we have added the `group` argument to each brick and introduced `BrickLoss` brick.
 
 ```python
-num_classes = 3
+from torchbricks.bricks import BrickLoss
+
 bricks = {
-    'preprocessor': BrickNotTrainable(PreprocessorDummy(), 
-                                      input_names=['raw_images'], 
-                                      output_names=['processed'], 
-                                      alive_stages="all"),
-    'backbone': BrickTrainable(TinyModel(n_channels=num_classes, n_features=10), 
-                               input_names=['processed'], 
-                               output_names=['embedding'], 
-                               alive_stages="all"),
-    'head': BrickTrainable(ClassifierDummy(num_classes=num_classes, in_features=10), 
-                           input_names=['embedding'], 
-                           output_names=['logits', 'softmaxed'], 
-                           alive_stages="all"),
-    'loss': BrickLoss(model=nn.CrossEntropyLoss(), 
-                      input_names=['logits', 'targets'], 
-                      output_names=['loss_ce'], 
-                      alive_stages=[Stage.TRAIN, Stage.VALIDATION, Stage.TEST])
+    "preprocessor": BrickNotTrainable(PreprocessorDummy(), input_names=["raw_images"], output_names=["processed"], group="MODEL"),
+    "backbone": BrickTrainable(
+        TinyModel(n_channels=3, n_features=10), input_names=["processed"], output_names=["embedding"], group="MODEL"
+    ),
+    "head": BrickTrainable(
+        ClassifierDummy(num_classes=3, in_features=10),
+        input_names=["embedding"],
+        output_names=["logits", "softmaxed"],
+        group="MODEL",
+    ),
+    "loss": BrickLoss(model=nn.CrossEntropyLoss(), input_names=["logits", "targets"], output_names=["loss_ce"], group="LOSS"),
 }
 brick_collection = BrickCollection(bricks)
 
 print(brick_collection)
 # BrickCollection(
-#   (preprocessor): BrickNotTrainable(PreprocessorDummy, input_names=['raw_images'], output_names=['processed'], alive_stages=['TRAIN', 'VALIDATION', 'TEST', 'INFERENCE', 'EXPORT'])
-#   (backbone): BrickTrainable(TinyModel, input_names=['processed'], output_names=['embedding'], alive_stages=['TRAIN', 'VALIDATION', 'TEST', 'INFERENCE', 'EXPORT'])
-#   (head): BrickTrainable(ClassifierDummy, input_names=['embedding'], output_names=['logits', 'softmaxed'], alive_stages=['TRAIN', 'VALIDATION', 'TEST', 'INFERENCE', 'EXPORT'])
-#   (loss): BrickLoss(CrossEntropyLoss, input_names=['logits', 'targets'], output_names=['loss_ce'], alive_stages=['TRAIN', 'VALIDATION', 'TEST'])
+#   (preprocessor): BrickNotTrainable(PreprocessorDummy, input_names=['raw_images'], output_names=['processed'], groups={'MODEL'})
+#   (backbone): BrickTrainable(TinyModel, input_names=['processed'], output_names=['embedding'], groups={'MODEL'})
+#   (head): BrickTrainable(ClassifierDummy, input_names=['embedding'], output_names=['logits', 'softmaxed'], groups={'MODEL'})
+#   (loss): BrickLoss(CrossEntropyLoss, input_names=['logits', 'targets'], output_names=['loss_ce'], groups={'LOSS'})
 # )
-print(create_mermaid_dag_graph(brick_collection))
+# print(create_mermaid_dag_graph(brick_collection))
 ```
 
-We set `preprocessor`, `backbone` and `head` to be alive on all stages `alive_stages="all"` - this is the default behavior and
-similar to before. 
- 
-For `loss` we set `alive_stages=[Stage.TRAIN, Stage.VALIDATION, Stage.TEST]` to only calculate loss during train, validation and test
-stages. 
+With group names, it is now possible to execute desired subsets of the model 
+during execution by adding `groups`.
+
+Here is a few examples: 
 
+```python
+named_inputs = {"raw_images": batched_images, "targets": torch.ones((batch_size), dtype=torch.int64)}
 
+# With no groups specified, all bricks are executed
+named_outputs = brick_collection(named_inputs=named_inputs)
 
-**Graph during inference and export:**
+# With groups specified, only bricks in the specified groups are executed
+named_outputs = brick_collection(named_inputs=named_inputs, groups={"MODEL"})
+```
 
-During `Stage.INFERENCE` and `Stage.EXPORT`, the graph will look as before, the loss modules is dead and note only `raw_images` is 
-still the only required input
+Groups are important concept in our model recipe as it allows us to specify how model will act during different model stages. 
 
 
 
+**Brick collection during inference and export:**
 
+During `Inference` and `Export` model stages, we do not have ground truth labels and we wan to skip loss calculations. 
+
+```python
+# Execution only "MODEL" group bricks
+named_outputs = brick_collection(named_inputs=named_inputs, groups={"MODEL"})
+```
+
+The graph will look like this and note that the graph only requires `raw_images` as input:
 ```mermaid
 flowchart LR
     %% Brick definitions
-    preprocessor("<strong>BrickNotTrainable</strong><br><strong>preprocessor</strong>: PreprocessorDummy"):::BrickNotTrainable
-    backbone("<strong>BrickTrainable</strong><br><strong>backbone</strong>: TinyModel"):::BrickTrainable
-    head("<strong>BrickTrainable</strong><br><strong>head</strong>: ClassifierDummy"):::BrickTrainable
+    preprocessor(<strong>'preprocessor': PreprocessorDummy</strong><br><i>BrickNotTrainable</i>):::BrickNotTrainable
+    backbone(<strong>'backbone': TinyModel</strong><br><i>BrickTrainable</i>):::BrickTrainable
+    head(<strong>'head': ClassifierDummy</strong><br><i>BrickTrainable</i>):::BrickTrainable
     
     %% Draw input and outputs
     raw_images:::input --> preprocessor
     
     %% Draw nodes and edges
     preprocessor --> |processed| backbone
     backbone --> |embedding| head
-    head --> softmaxed:::output
     head --> logits:::output
+    head --> softmaxed:::output
     
     %% Add styling
     classDef arrow stroke-width:0px,fill-opacity:0.0 
     classDef input stroke-width:0px,fill-opacity:0.3,fill:#22A699 
     classDef output stroke-width:0px,fill-opacity:0.3,fill:#F2BE22 
     classDef BrickNotTrainable stroke-width:0px,fill:#B56576 
     classDef BrickTrainable stroke-width:0px,fill:#6D597A 
     
     %% Add legends
     subgraph Legends
         input(input):::input
         output(output):::output
-        
     end
 ```
 
 
-**Graph during train, test and validation:**
+**Brick collection during train, test and validation:**
 
-During `Stage.TRAIN`, `Stage.VALIDATION` and `Stage.TEST`, the loss module is alive and note both `raw_images` and `targets` are required as inputs:
+During "Train", "Test" and "Validation", `targets` are available and we want to calculate loss to 
+both improve model and track loss curves. 
 
+```python
+# Execution all groups
+named_outputs = brick_collection(named_inputs=named_inputs)
 
+# Or execute explicitly "MODEL" and "LOSS" group bricks
+named_outputs = brick_collection(named_inputs=named_inputs, groups={"MODEL", "LOSS"})
+```
 
+The graph will look like this and note that the graph now requires `raw_images` and `targets` as input:
 
 ```mermaid
 flowchart LR
     %% Brick definitions
-    preprocessor("<strong>BrickNotTrainable</strong><br><strong>preprocessor</strong>: PreprocessorDummy"):::BrickNotTrainable
-    backbone("<strong>BrickTrainable</strong><br><strong>backbone</strong>: TinyModel"):::BrickTrainable
-    head("<strong>BrickTrainable</strong><br><strong>head</strong>: ClassifierDummy"):::BrickTrainable
-    loss("<strong>BrickLoss</strong><br><strong>loss</strong>: CrossEntropyLoss"):::BrickLoss
+    preprocessor(<strong>'preprocessor': PreprocessorDummy</strong><br><i>BrickNotTrainable</i>):::BrickNotTrainable
+    backbone(<strong>'backbone': TinyModel</strong><br><i>BrickTrainable</i>):::BrickTrainable
+    head(<strong>'head': ClassifierDummy</strong><br><i>BrickTrainable</i>):::BrickTrainable
+    loss(<strong>'loss': CrossEntropyLoss</strong><br><i>BrickLoss</i>):::BrickLoss
     
     %% Draw input and outputs
     raw_images:::input --> preprocessor
     targets:::input --> loss
     
     %% Draw nodes and edges
     preprocessor --> |processed| backbone
@@ -344,21 +349,20 @@
     subgraph Legends
         input(input):::input
         output(output):::output
     end
 ```
 
 
-
 As demonstrated in above example, we can easily change the required inputs by change the model stage.
 That allows us to support two basic use cases:
 
 1) When labels/targets are available, we have the option of getting model prediction along with loss and metrics.
 
-2) When labels/targets are **not** available, we will only do basic model predictions. 
+2) When labels/targets are **not** available, we do only model predictions used for model inference/export.
 
 The mechanism of activating different parts of the model and making loss, metrics and visualizations part of the model recipe, 
 allows us to more easily investigate/debug/visualize model parts in a notebook or scratch scripts.
 
 
 ## Brick features: 
 
@@ -374,59 +378,62 @@
 To calculate metrics across a dataset, we heavily rely on concepts and functions used in the 
 [TorchMetrics](https://torchmetrics.readthedocs.io/en/stable/) library.
 
 The used of TorchMetrics in a brick collection is demonstrated in below code snippet. 
 
 ```python
 import torchvision
-from torchbricks.bag_of_bricks import ImageClassifier, Preprocessor, resnet_to_brick
-from torchbricks.bricks import BrickMetricSingle
+from torchbricks.bag_of_bricks.backbones import resnet_to_brick
+from torchbricks.bag_of_bricks.image_classification import ImageClassifier
+from torchbricks.bag_of_bricks.preprocessors import Preprocessor
+from torchbricks.bricks import BrickLoss, BrickMetricSingle
 from torchmetrics.classification import MulticlassAccuracy
 
 num_classes = 10
 resnet = torchvision.models.resnet18(weights=None, num_classes=num_classes)
-resnet_brick = resnet_to_brick(resnet=resnet,  input_name='normalized', output_name='features')
+resnet_brick = resnet_to_brick(resnet=resnet, input_name="normalized", output_name="features")
 n_features = resnet_brick.model.n_backbone_features
 bricks = {
-    'preprocessor': BrickNotTrainable(Preprocessor(), 
-                                      input_names=['raw'], 
-                                      output_names=['normalized']),
-    'backbone': resnet_brick,
-    'head': BrickTrainable(ImageClassifier(num_classes=num_classes, n_features=n_features),
-                           input_names=['features'], 
-                           output_names=['logits', 'probabilities', 'class_prediction']),
-    'accuracy': BrickMetricSingle(MulticlassAccuracy(num_classes=num_classes), 
-                                  input_names=['class_prediction', 'targets']),
-    'loss': BrickLoss(model=nn.CrossEntropyLoss(), 
-                      input_names=['logits', 'targets'], 
-                      output_names=['loss_ce'])
+    "preprocessor": BrickNotTrainable(Preprocessor(), input_names=["raw"], output_names=["normalized"]),
+    "backbone": resnet_brick,
+    "head": BrickTrainable(
+        ImageClassifier(num_classes=num_classes, n_features=n_features),
+        input_names=["features"],
+        output_names=["logits", "probabilities", "class_prediction"],
+    ),
+    "accuracy": BrickMetricSingle(MulticlassAccuracy(num_classes=num_classes), input_names=["class_prediction", "targets"]),
+    "loss": BrickLoss(model=nn.CrossEntropyLoss(), input_names=["logits", "targets"], output_names=["loss_ce"]),
 }
 brick_collection = BrickCollection(bricks)
 ```
 
-We will now use the brick collection above to simulate how a user can iterate over a dataset and 
-pass batches to the brick collection.
+We will now use the brick collection above to simulate how a user can iterate over a dataset.
 
 ```python
 # Simulate dataloader
 named_input_simulated = {"raw": batched_images, "targets": torch.ones((batch_size), dtype=torch.int64)}
 dataloader_simulated = [named_input_simulated for _ in range(5)]
 
 # Loop over the dataset
-for named_inputs in dataloader_simulated: # Simulates iterating over the dataset
-    named_outputs = brick_collection(named_inputs=named_inputs, stage=Stage.TRAIN)
+for named_inputs in dataloader_simulated:  # Simulates iterating over the dataset
+    named_outputs = brick_collection(named_inputs=named_inputs)
+    named_outputs_losses_only = brick_collection.extract_losses(named_outputs=named_outputs)
 
-metrics = brick_collection.summarize(stage=Stage.TRAIN, reset=True)
+metrics = brick_collection.summarize(reset=True)
 print(f"{named_outputs.keys()=}")
 # named_outputs.keys()=dict_keys(['raw', 'targets', 'stage', 'normalized', 'features', 'logits', 'probabilities', 'class_prediction', 'loss_ce'])
 print(f"{metrics=}")
 # metrics={'MulticlassAccuracy': tensor(0.)}
 ```
 
 For each iteration in our (simulated) dataset, we calculate model outputs, losses and metrics for each batch. 
+
+Losses are calculated and returned in `named_outputs` together with other model outputs. 
+We provide `extract_losses` as simple function to filter `named_outputs` and only return losses in a new dictionary. 
+
 Unlike other bricks, `BrickMetrics` will not (by default) output metrics for each batch. 
 Instead metrics are stored internally in `BrickMetricSingle` and only aggregated and return when
 the `summarize` function is called. In above example, metric is aggregated over 5 batches as summaries to a single value. 
 
 It is important to note that we set `reset=True` to reset the internal aggregation of metrics.  
 
 **Additional notes on metrics**
@@ -481,43 +488,42 @@
 
 ```python
 from typing import Dict
 
 from torchbricks.bricks import BrickInterface
 
 
-def create_image_classification_head(num_classes: int, in_channels: int, features_name: str, targets_name: str) -> Dict[str, BrickInterface]:
-    """Image classifier bricks: Classifier, loss and metrics """
+def create_image_classification_head(
+    num_classes: int, in_channels: int, features_name: str, targets_name: str
+) -> Dict[str, BrickInterface]:
+    """Image classifier bricks: Classifier, loss and metrics"""
     head = {
-        'classify': BrickTrainable(ImageClassifier(num_classes=num_classes, n_features=in_channels),
-                                   input_names=[features_name], 
-                                   output_names=['./logits', './probabilities', './class_prediction']),
-        'accuracy': BrickMetricSingle(MulticlassAccuracy(num_classes=num_classes), 
-                                      input_names=['./class_prediction', targets_name]),
-        'loss': BrickLoss(model=nn.CrossEntropyLoss(),
-                          input_names=['./logits', targets_name], 
-                          output_names=['./loss_ce'])
+        "classify": BrickTrainable(
+            ImageClassifier(num_classes=num_classes, n_features=in_channels),
+            input_names=[features_name],
+            output_names=["./logits", "./probabilities", "./class_prediction"],
+        ),
+        "accuracy": BrickMetricSingle(MulticlassAccuracy(num_classes=num_classes), input_names=["./class_prediction", targets_name]),
+        "loss": BrickLoss(model=nn.CrossEntropyLoss(), input_names=["./logits", targets_name], output_names=["./loss_ce"]),
     }
     return head
-
 ```
 
 We now create the full model containing a `preprocessor`, `backbone` and two independent heads called `head0` and `head1`.
 Each head is a dictionary of bricks, making our brick collection a nested dictionary. 
 
 ```python
+from torchbricks.graph_plotter import create_mermaid_dag_graph
 
 n_features = resnet_brick.model.n_backbone_features
 bricks = {
-    'preprocessor': BrickNotTrainable(Preprocessor(), 
-                                      input_names=['raw'], 
-                                      output_names=['normalized']),
-    'backbone': resnet_brick,
-    'head0': create_image_classification_head(num_classes=3, in_channels=n_features, features_name='features', targets_name='targets0'),
-    'head1': create_image_classification_head(num_classes=5, in_channels=n_features, features_name='features', targets_name='targets1'),
+    "preprocessor": BrickNotTrainable(Preprocessor(), input_names=["raw"], output_names=["normalized"]),
+    "backbone": resnet_brick,
+    "head0": create_image_classification_head(num_classes=3, in_channels=n_features, features_name="features", targets_name="targets0"),
+    "head1": create_image_classification_head(num_classes=5, in_channels=n_features, features_name="features", targets_name="targets1"),
 }
 brick_collections = BrickCollection(bricks)
 print(brick_collections)
 print(create_mermaid_dag_graph(brick_collections))
 ```
 
 Also demonstrated in above example is the use of relative input and output names. 
@@ -529,22 +535,22 @@
 
 We visualize above graph: 
 
 
 ```mermaid
 flowchart LR
     %% Brick definitions
-    preprocessor("<strong>BrickNotTrainable</strong><br><strong>preprocessor</strong>: Preprocessor"):::BrickNotTrainable
-    backbone("<strong>BrickTrainable</strong><br><strong>backbone</strong>: BackboneResnet"):::BrickTrainable
-    head0/classify("<strong>BrickTrainable</strong><br><strong>head0/classify</strong>: ImageClassifier"):::BrickTrainable
-    head0/accuracy("<strong>BrickMetricSingle</strong><br><strong>head0/accuracy</strong>: ['MulticlassAccuracy']"):::BrickMetricSingle
-    head0/loss("<strong>BrickLoss</strong><br><strong>head0/loss</strong>: CrossEntropyLoss"):::BrickLoss
-    head1/classify("<strong>BrickTrainable</strong><br><strong>head1/classify</strong>: ImageClassifier"):::BrickTrainable
-    head1/accuracy("<strong>BrickMetricSingle</strong><br><strong>head1/accuracy</strong>: ['MulticlassAccuracy']"):::BrickMetricSingle
-    head1/loss("<strong>BrickLoss</strong><br><strong>head1/loss</strong>: CrossEntropyLoss"):::BrickLoss
+    preprocessor(<strong>'preprocessor': Preprocessor</strong><br><i>BrickNotTrainable</i>):::BrickNotTrainable
+    backbone(<strong>'backbone': BackboneResnet</strong><br><i>BrickTrainable</i>):::BrickTrainable
+    head0/classify(<strong>'head0/classify': ImageClassifier</strong><br><i>BrickTrainable</i>):::BrickTrainable
+    head0/accuracy(<strong>'head0/accuracy': 'MulticlassAccuracy'</strong><br><i>BrickMetricSingle</i>):::BrickMetricSingle
+    head0/loss(<strong>'head0/loss': CrossEntropyLoss</strong><br><i>BrickLoss</i>):::BrickLoss
+    head1/classify(<strong>'head1/classify': ImageClassifier</strong><br><i>BrickTrainable</i>):::BrickTrainable
+    head1/accuracy(<strong>'head1/accuracy': 'MulticlassAccuracy'</strong><br><i>BrickMetricSingle</i>):::BrickMetricSingle
+    head1/loss(<strong>'head1/loss': CrossEntropyLoss</strong><br><i>BrickLoss</i>):::BrickLoss
     
     %% Draw input and outputs
     raw:::input --> preprocessor
     targets0:::input --> head0/accuracy
     targets0:::input --> head0/loss
     targets1:::input --> head1/accuracy
     targets1:::input --> head1/loss
@@ -579,32 +585,54 @@
     subgraph Legends
         input(input):::input
         output(output):::output
     end
 ```
 
 
+### Brick features: Save and loading bricks
+A brick collection can be saved and loaded as a regular pytorch `nn.Module`. For more information you can look up the official 
+pytorch guide on [Saving and Loading Models](https://pytorch.org/tutorials/beginner/saving_loading_models.html). 
+
+However, we have also added a brick collection specific saving/loading format. It uses a pytorch weight format, 
+but creates a model file for each brick and keeps files in a nested folder structure. 
+
+The idea is that a user can more easily add or remove weights to a specific model by simply moving around model files and folders.
+Time will tell, if this a useful abstraction or dead code. 
+
+But it looks like this: 
+
+```python
+path_model_folder = Path("build/bricks")
+
+# Saving model parameters brick-collection style
+brick_collections.save_bricks(path_model_folder=path_model_folder, exist_ok=True)
+
+print("Model files: ")
+print("\n".join(str(path) for path in path_model_folder.rglob("*.pt")))
+
+# Loading model parameters brick-collection style
+brick_collection.load_bricks(path_model_folder=path_model_folder)
+```
+
 ### Brick features: Export as ONNX
 To export a brick collection as onnx we provide the `export_bricks_as_onnx`-function. 
 
 Pass an example input (`named_input`) to trace a brick collection.
 Set `dynamic_batch_size=True` to support any batch size inputs and here we explicitly set `stage=Stage.EXPORT` - this is also 
 the default.
 
 ```python
-from torchbricks.brick_utils import export_bricks_as_onnx
+from torchbricks.brick_collection_utils import export_bricks_as_onnx
+
 path_build = Path("build")
 path_build.mkdir(exist_ok=True)
 path_onnx = path_build / "readme_model.onnx"
 
-export_bricks_as_onnx(path_onnx=path_onnx, 
-                      brick_collection=brick_collection, 
-                      named_inputs=named_inputs, 
-                      dynamic_batch_size=True, 
-                      stage=Stage.EXPORT)
+export_bricks_as_onnx(path_onnx=path_onnx, brick_collection=brick_collection, named_inputs=named_inputs, dynamic_batch_size=True)
 ```
 
 ### Brick features: Bag of bricks - reusable bricks modules
 Note also in above example we use bag-of-bricks to import commonly used `nn.Module`s 
 
 This includes a `Preprocessor`, `ImageClassifier` and `resnet_to_brick` to convert a torchvision resnet models to a backbone brick 
 without a classifier.
@@ -630,144 +658,126 @@
 as an example for you to use. 
 
 
 ```python
 from functools import partial
 from pathlib import Path
 
-import torchvision
 import pytorch_lightning as pl
-from utils_testing.lightning_module import LightningBrickCollection
+import torchvision
 from utils_testing.datamodule_cifar10 import CIFAR10DataModule
+from utils_testing.lightning_module import LightningBrickCollection
 
-experiment_name="CIFAR10"
+experiment_name = "CIFAR10"
 transform = torchvision.transforms.ToTensor()
-data_module = CIFAR10DataModule(data_dir='data', batch_size=5, num_workers=12, test_transforms=transform, train_transforms=transform)
-create_opimtizer_func = partial(torch.optim.SGD, lr=0.05, momentum=0.9, weight_decay=5e-4)
-bricks_lightning_module = LightningBrickCollection(path_experiments=Path("build") / "experiments",
-                                                   experiment_name=None,
-                                                   brick_collection=brick_collection,
-                                                   create_optimizers_func=create_opimtizer_func)
+data_module = CIFAR10DataModule(data_dir="data", batch_size=5, num_workers=12, test_transforms=transform, train_transforms=transform)
+create_optimizer_func = partial(torch.optim.SGD, lr=0.05, momentum=0.9, weight_decay=5e-4)
+bricks_lightning_module = LightningBrickCollection(
+    path_experiments=Path("build") / "experiments",
+    experiment_name=None,
+    brick_collection=brick_collection,
+    create_optimizers_func=create_optimizer_func,
+)
 
 trainer = pl.Trainer(max_epochs=1, limit_train_batches=2, limit_val_batches=2, limit_test_batches=2)
 # Train and test model by injecting 'bricks_lightning_module'
-# trainer.fit(bricks_lightning_module, datamodule=data_module)
-# trainer.test(bricks_lightning_module, datamodule=data_module)
+trainer.fit(bricks_lightning_module, datamodule=data_module)
+trainer.test(bricks_lightning_module, datamodule=data_module)
 ```
 
 
 ### Brick features: Pass all intermediate tensors to Brick
 By adding `'__all__'` to `input_names`, it is possible to access all tensors as a dictionary inside a brick module. 
 For production code, this may not be the best option, but this feature can be valuable during an exploration phase or 
 when doing some live debugging of a new model/module. 
 
-We will demonstrate in code by introducing a (dummy) module `VisualizeRawAndPreprocessed`.
+We will demonstrate in code by introducing a (dummy) module `MyNewPostProcessor`.
 
 *Note: It is just a dummy class, don't worry to much about the actual implementation.*
 
 The important thing to notice is that `input_names = ['__all__']` is used for our `visualizer`-brick to
 pass all tensors as a dictionary as an argument in the forward call. 
 
 ```python
-class VisualizeRawAndPreprocessed(torch.nn.Module):
+from typing import Any
+
+
+class MyNewPostProcessor(torch.nn.Module):
     def forward(self, named_inputs: Dict[str, Any]):
         ## Here `named_inputs` contains all intermediate tensors
-        image_raw_and_preprocessed = torch.concatenate((named_inputs["raw"], named_inputs["preprocessed"]), dim=3)
-        return image_raw_and_preprocessed
+        assert "raw" in named_inputs
+        assert "embedding" in named_inputs
+        return named_inputs["embedding"]
 
 
 bricks = {
-    'preprocessor': BrickNotTrainable(PreprocessorDummy(), input_names=['raw'],  output_names=['preprocessed']),
-    'backbone': BrickTrainable(TinyModel(n_channels=3, n_features=10), input_names=['preprocessed'], output_names=['embedding']),
-    'visualizer': BrickNotTrainable(VisualizeRawAndPreprocessed(), input_names = ['__all__'], output_names=["visualization"])
+    "backbone": BrickTrainable(TinyModel(n_channels=3, n_features=10), input_names=["raw"], output_names=["embedding"]),
+    "post_processor": BrickNotTrainable(MyNewPostProcessor(), input_names=["__all__"], output_names=["postprocessed"]),
 }
 brick_collection = BrickCollection(bricks)
-named_outputs = brick_collection(named_inputs={'raw': torch.rand((2, 3, 100, 200))}, stage=Stage.INFERENCE)
-```
-
-### Brick features: Using Stage Inside Module
-By passing in `stage` in `input_names` it is possible to change the program flow. 
-
-As demonstrated below want to alway resize the input to a specific size when the model is being exported.
-
-```python
-class Preprocessor(torch.nn.Module):
-    def forward(self, input_image: torch.Tensor, stage: Stage) -> str:
-        if stage in [Stage.EXPORT]:
-            input_image = torch.nn.functional.interpolate(input_image, size=(50,100))
-        return input_image/2
-
-
-brick_collection = BrickCollection({
-        "preprocessor": BrickNotTrainable(Preprocessor(), input_names=['raw', 'stage'], output_names=["processed"])
-    })
-named_inputs = {'raw': torch.rand((2, 3, 100, 200))}
-named_outputs = brick_collection(named_inputs=named_inputs, stage=Stage.EXPORT)
-assert list(named_outputs["processed"].shape[2:]) == [50, 100]
-
-named_outputs = brick_collection(named_inputs=named_inputs, stage=Stage.VALIDATION)
-assert list(named_outputs["processed"].shape[2:]) == [100, 200]
+named_outputs = brick_collection(named_inputs={"raw": torch.rand((2, 3, 100, 200))})
 ```
 
 ### Brick features: Visualizations in TorchBricks
 We provide `BrickPerImageVisualization` as base brick for doing visualizations in a brick collection. 
 The advantage of brick-based visualization is that it can be bundled together with a specific task/head. 
 
-Visualization/drawing functions typically operate on a single image and on non-`torch.Tensor` data types.
+Secondly, visualization/drawing functions typically operate on a single image and on non-`torch.Tensor` data types.
 E.g. Opencv/matplotlib uses `np.array` and pillow using `Image`. 
 
 (Torchvision actually has functions to draw rectangles, key-points and segmentation masks directly on `torch.Tensor`s -
 but it still operates on a single image and it has no option for rendering text).
 
-The goal of `BrickPerImageVisualization` is to convert batched tensors/data to per image data in a desired format
+The goal of `BrickPerImageVisualization` is to convert batched tensors/data to per image data in a desired format/datatype 
 and pass it to a draw function. Look up the documentation of `BrickPerImageVisualization` to see all options.
 
-First we create a callable to do per image visualizations. It can be a simple function, but in this example we create a callable 
-class to pass in class names and initialize font. 
+First we create a callable to do per image visualizations. It can be a simple function, but as demonstrated in below example, it 
+can also be a callable class. 
 
 The callable visualizes image classification predictions using pillow and requires two `np.array`s as input: 
 `input_image` of shape [H, W, C] and `target_prediction` [1].
 
 ```python
-
-from PIL import Image, ImageDraw, ImageFont
 import numpy as np
+from PIL import Image, ImageDraw, ImageFont
 from torchbricks.tensor_conversions import float2uint8
 
+
 class VisualizeImageClassification:
     def __init__(self, class_names: list, font_size: int = 50):
         self.class_names = class_names
-        self.font = ImageFont.truetype('tests/data/font_ASMAN.TTF', size=font_size) 
+        self.font = ImageFont.truetype("tests/data/font_ASMAN.TTF", size=font_size)
 
     def __call__(self, input_image: np.ndarray, target_prediction: np.ndarray) -> Image.Image:
         """Draws image classification results"""
-        assert input_image.ndim == 3 # Converted to single image channel last numpy array [H, W, C]
+        assert input_image.ndim == 3  # Converted to single image channel last numpy array [H, W, C]
         image = Image.fromarray(float2uint8(input_image))
-        draw = ImageDraw.Draw(image) 
-        draw.text((25, 25), text=self.class_names[target_prediction[0]], font = self.font) 
+        draw = ImageDraw.Draw(image)
+        draw.text((25, 25), text=self.class_names[target_prediction[0]], font=self.font)
         return image
 ```
 
-Our new drawing class `VisualizeImageClassification` is not passed to `BrickPerImageVisualization` and used in a brick collection.
+The drawing class `VisualizeImageClassification` is now passed to `BrickPerImageVisualization` and used in a brick collection.
 
 ```python
+from torchbricks.bag_of_bricks.brick_visualizer import BrickPerImageVisualization
 
-from torchbricks.brick_visualizer import BrickPerImageVisualization
 bricks = {
-    'visualizer': BrickPerImageVisualization(callable=VisualizeImageClassification(class_names=["cat", "dog"]), 
-                                          input_names=["input_image", "target"], 
-                                          output_names=["visualization"],
-                                          alive_stages=[Stage.INFERENCE])
+    "visualizer": BrickPerImageVisualization(
+        callable=VisualizeImageClassification(class_names=["cat", "dog"]),
+        input_names=["input_image", "target"],
+        output_names=["visualization"],
+    )
 }
 
-batched_inputs = {'input_image': torch.zeros((2, 3, 100, 200)), 'target': torch.tensor([0, 1], dtype=torch.int64)}
+batched_inputs = {"input_image": torch.zeros((2, 3, 100, 200)), "target": torch.tensor([0, 1], dtype=torch.int64)}
 brick_collection = BrickCollection(bricks)
-outputs = brick_collection(named_inputs=batched_inputs, stage=Stage.INFERENCE)
+outputs = brick_collection(named_inputs=batched_inputs)
 
-display(outputs["visualization"][0],  outputs["visualization"][1])
+display(outputs["visualization"][0], outputs["visualization"][1])
 ```
 
 `BrickPerImageProcessing` will by default convert a batch tensor of shape [B, C, H, W] to a channel last numpy image of shape [H, W, C]. 
 This is the default behavior, and it allows us in the callable of `VisualizeImageClassification` to operate directly on numpy arrays. 
 
 However for `BrickPerImageProcessing` a user has the option for unpacking batch data in a desired way as we will demonstrate in the 
 next example.
@@ -778,37 +788,43 @@
 other options of the `BrickPerImageVisualization` class. 
 
 *It is important to note that `visualize_image_classification_pillow` is passed as a callable, and we do not override functionality of 
 `BrickPerImageVisualization`. We only use it to simplify the constructor of `BrickVisualizeImageClassification`.
 
 ```python
 from typing import List
-from torchbricks.tensor_conversions import unpack_batched_tensor_to_pillow_images, function_composer, torch_to_numpy
+
+from torchbricks.tensor_conversions import function_composer, torch_to_numpy, unpack_batched_tensor_to_pillow_images
 
 
 class BrickVisualizeImageClassification(BrickPerImageVisualization):
     def __init__(self, input_image: str, target_name: str, class_names: List[str], output_name: str):
         self.class_names = class_names
-        self.font = ImageFont.truetype('tests/data/font_ASMAN.TTF', 50) 
-        super().__init__(callable=self.visualize_image_classification_pillow, input_names=[input_image, target_name], output_names=[output_name],
-                         unpack_functions_for_type={torch.Tensor: unpack_batched_tensor_to_pillow_images},
-                         unpack_functions_for_input_name={target_name: function_composer(torch_to_numpy, list)})
+        self.font = ImageFont.truetype("tests/data/font_ASMAN.TTF", 50)
+        super().__init__(
+            callable=self.visualize_image_classification_pillow,
+            input_names=[input_image, target_name],
+            output_names=[output_name],
+            unpack_functions_for_type={torch.Tensor: unpack_batched_tensor_to_pillow_images},
+            unpack_functions_for_input_name={target_name: function_composer(torch_to_numpy, list)},
+        )
 
     def visualize_image_classification_pillow(self, image: Image.Image, target_prediction: np.int64) -> Image.Image:
         """Draws image classification results"""
-        draw = ImageDraw.Draw(image) 
+        draw = ImageDraw.Draw(image)
 
-        draw.text((25, 25), text=self.class_names[target_prediction], font = self.font) 
+        draw.text((25, 25), text=self.class_names[target_prediction], font=self.font)
         return image
 
 
-visualizer = BrickVisualizeImageClassification(input_image="input_image", target_name="target", class_names=["cat", "dog"],
-                                               output_name="VisualizeImageClassification")
-batched_inputs = {'input_image': torch.zeros((2, 3, 100, 200)), 'target': torch.tensor([0, 1], dtype=torch.int64)}
-visualizer(batched_inputs, stage=Stage.INFERENCE)
+visualizer = BrickVisualizeImageClassification(
+    input_image="input_image", target_name="target", class_names=["cat", "dog"], output_name="VisualizeImageClassification"
+)
+batched_inputs = {"input_image": torch.zeros((2, 3, 100, 200)), "target": torch.tensor([0, 1], dtype=torch.int64)}
+visualizer(batched_inputs)
 ```
 
 Not unlike before, the callable (here `visualize_image_classification_pillow`) accepts an `Image.Image` image and an `int64` value directly
 and we are not required to do conversions inside the drawing function. 
 
 This can be achieved by using the two input arguments: 
 - `unpack_functions_for_type: Dict[Type, Callable]` specifying how each type should be unpacked.
@@ -820,95 +836,51 @@
 
 Specifying unpacking by input name (`unpack_functions_for_input_name`) will override the per type unpacking of `unpack_functions_for_type`. 
 
 
 ## Motivation
 
 The main motivation:
-- Sharable models: Packing model parts, metrics, loss-functions and visualization into a single recipe, makes the model more sharable to
-  other projects and supports sharing model for different use cases such as: Only inference, inference+visualizations and 
+- Sharable models: Packing model parts, metrics, loss-functions and visualizations into a single recipe, makes the model more sharable to
+  other projects and supports sharing models for different use cases such as: Only inference, inference+visualizations and 
   training+metrics+losses.
 - Shareable Parts: The brick collection encourage users to decouples parts and making also each part more sharable. 
-- Multiple tasks: Makes it easier to add and remove tasks. Each task can be expressed by model parts in a dictionary, we can easily add/remove them to a brick collection. 
+- Multiple tasks: Makes it easier to add and remove tasks. Each task can be expressed by model parts in a dictionary, 
+  we can easily add/remove them to a brick collection. 
 - By packing model modules, metrics, loss-functions and visualization into a single brick collection, we can more easily 
   inject it into your custom trainer and evaluation without doing per task/model modifications. 
 - Your model is **not** required to only return logits. Some training frameworks expect you to only return logits - values that go into 
   your loss function. Then at inference/test/evaluation you need to do post processing or pass additional outputs to 
   calculate metrics, do visualizations and make prediction human interpretable. It encourage unclear control flow (if/else statements) 
   in the model that depends on model stage. 
 - Using input and output names makes it easier to describe how parts are connected. Internally data is passed between bricks in a 
-  dictionary of any type - making in flexible. But for each module, you can specific and check types hints for input and output data to 
-  both improve readability and more production ready. 
+  dictionary of any type - making in flexible. But for each module, you can specific and add and check type hints for input and output 
+  data to both improve readability and make it more production ready. 
 - When I started making a framework suited for multiple tasks, I would passed dictionaries around to all modules and pull out tensors by
-  name in modules. Changing names would break stuff and it was not production ready. I also started using the typical 
-  backbone(encoder) / head(decoder) separation... But some heads may share a common neck. The decoder might also take different inputs and
+  name in each module. Book keeping names and updating names was messy. 
+  I also started using the typical backbone(encoder) / head(decoder) separation... But some heads may share a common neck. 
+  The decoder might also take different inputs and
   split into different representation and merge again... Also to avoid code duplication, I ended up during 
   multiple layers of inheritance for the decoder, making reuse bad and generally everything became too complicated and a new task would 
   require me to refactor the whole concept. Yes, it was probably not a super great attempt either, but it made me realize it should be 
   easier to make a new task and it should be easier to reuse parts. 
 
 
-
-
-## Why should I explicitly set the train, val or test stage
-
-MISSING
-
-
-
 <!-- #region -->
 ##
 
 ## What are we missing?
-
-
-- [x] ~~Proper~~ Added a link to `LightningBrickCollection` for other people to use
-- [x] Minor: BrickCollections supports passing a dictionary with BrickCollections. But we should also convert a nested dictionary into a nested brick collections
-- [x] Minor: Currently, `input_names` and `output_names` support positional arguments, but we should also support keyword arguments.
-- [x] Minor: Make Brick an abstract class
-- [x] Convert torchvision resnet models to only a backbone brick.
-- [x] Make readme a notebook
-- [x] Automatically convert jupyter notebook to `README.md`
-- [x] Remove README.md header
-- [x] Make an export to onnx function 
-- [x] Make it optional if gradients can be passed through NonTrainableBrick without weights being optimized
-- [x] Refactor Metrics: Create BrickMetricCollection and BrickSingleMetric and create flag to return metrics.
-- [x] Make brick base class with input_names, output_names and alive_stages - inherit this from other bricks. 
-  - Pros: We might include other non-torch modules later. 
-  - Do not necessarily pass a stage-object. Consider also passing it as a string so it can be handled correctly with scripting. 
-- [x] Update README.md to match the new bricks. 
-  - [x] Start with basic bricks example. 
-  - [x] Use loss-function to show that stage decided on what is being executed. 
-  - [x] Introduce metrics by it-self in another example
-- [x] Ensure that all examples in the `README.md` are working with easy to use modules. 
-- [x] Add typeguard
-- [x] Allow a brick to receive all named_inputs and add a test for it.
-- [x] Fix the release process. It should be as simple as running `make release`.
-- [x] Add onnx export example to the README.md
-- [x] Pretty print bricks
-- [x] Relative input/output names
-- [x] Test to verify that environment matches conda lock. The make command 'update-lock-file' should store a copy of 'environment.yml'
-      We will the have a test checking if the copy and the current version of `environment.yml` is the same.
-- [x] Add code coverage and tests passed badges to readme again
-- [x] Create brick-collection visualization tool ("mermaid?")
-- [x] Make DAG like functionality to check if inputs and outputs works for all model stages.
-- [x] Make Base Module PerImageProcessing as the basis for doing visualizations. 
-  - [ ] Consider caching unpacked data
-- [ ] Demonstrate model configuration with hydra
+- [ ] Demonstrate model configuration with hydra in this document
 - [ ] Make common Visualizations with pillow - not opencv to not blow up the required dependencies. ImageClassification, Segmentation, ObjectDetection
   - [ ] VideoModule to store data as a video
   - [ ] DisplayModule to show data
+- [ ] Consider caching unpacked data for `PerImageVisualizer`
 - [ ] Multiple named tensors caching module. 
 - [ ] Use pymy, pyright or pyre to do static code checks. 
-- [ ] Decide: Add stage as an internal state and not in the forward pass:
-  - Minor Pros: Tracing (to get onnx model) requires only torch.Tensors only as input - we avoid making an adapter class. 
-  - Minor Cons: State gets hidden away - implicit instead of explicit.
-  - Minor Pros: Similar to eval/training 
 - [ ] Collection of helper modules. Preprocessors, Backbones, Necks/Upsamplers, ImageClassification, SemanticSegmentation, ObjectDetection
-  - [x] All the modules in the README should be easy to import as actually modules.
   - [ ] Make common brick collections: BricksImageClassification, BricksSegmentation, BricksPointDetection, BricksObjectDetection
 - [ ] Support preparing data in the dataloader?
 - [ ] Support torch.jit.scripting? 
 
 ## How does it really work?
 ????
 
@@ -925,9 +897,7 @@
     poetry install
 
 ### Activating the environment
 
     conda activate torchbricks
 
 <!-- #endregion -->
-
-
```

### Comparing `torchbricks-0.1.0/tests/test_brick_utils.py` & `torchbricks-0.3.0/tests/test_brick_collection_utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 from pathlib import Path
 
 import onnx
 import pytest
 import torch
-from torchbricks.brick_utils import export_bricks_as_onnx
-from torchbricks.bricks import BrickCollection, Stage
-from utils_testing.utils_testing import create_brick_collection
+from torchbricks import model_stage
+from torchbricks.brick_collection import BrickCollection
+from torchbricks.brick_collection_utils import export_bricks_as_onnx
+from utils_testing.utils_testing import create_dummy_brick_collection
 
 
 def test_export_onnx_trace(tmp_path: Path):
     num_classes = 3
-    brick_collection = create_brick_collection(num_classes=num_classes, num_backbone_featues=10)
+    brick_collection = create_dummy_brick_collection(num_classes=num_classes, num_backbone_featues=10)
     model = BrickCollection(brick_collection)
-    named_inputs = {'raw': torch.zeros((1, 3, 64, 64))}
+    named_inputs = {"raw": torch.zeros((1, 3, 64, 64))}
 
-    stage = Stage.EXPORT
-    named_outputs = model(named_inputs, stage=stage, return_inputs=False)
+    named_outputs = model(named_inputs, groups=model_stage.EXPORT, return_inputs=False)
     # remove_from_outputs = ["stage"] + list(named_inputs)
     expected_input = list(named_inputs)
     expected_outputs = list(named_outputs)
 
-    path_onnx = Path(tmp_path / 'model.onnx')
+    path_onnx = Path(tmp_path / "model.onnx")
 
     dynamic_batch_size_configs = [False, True]
     for dynamic_batch_size in dynamic_batch_size_configs:
-        export_bricks_as_onnx(brick_collection=model, named_inputs=named_inputs, path_onnx=path_onnx, stage=stage,
-                       dynamic_batch_size=dynamic_batch_size)
+        export_bricks_as_onnx(brick_collection=model, named_inputs=named_inputs, path_onnx=path_onnx, dynamic_batch_size=dynamic_batch_size)
 
         assert path_onnx.exists()
         onnx_model = onnx.load(path_onnx)
 
         output_names_graph = {output.name for output in onnx_model.graph.output}
         assert set(expected_outputs) == output_names_graph
 
@@ -38,18 +37,18 @@
 
         onnx.checker.check_model(onnx_model)
 
 
 @pytest.mark.xfail
 def test_export_torch_jit_script(tmp_path: Path):
     num_classes = 3
-    brick_collection = create_brick_collection(num_classes=num_classes, num_backbone_featues=10)
-    model = BrickCollection(brick_collection)
-    named_inputs = {'raw': torch.zeros((1, 3, 64, 64))}
+    brick_collection = create_dummy_brick_collection(num_classes=num_classes, num_backbone_featues=10)
+
+    model = BrickCollection(brick_collection).to_sub_collection(groups=model_stage.EXPORT)
+    named_inputs = {"raw": torch.zeros((1, 3, 64, 64))}
 
-    stage = Stage.EXPORT
-    named_outputs = model(named_inputs, stage=stage, return_inputs=False)
+    named_outputs = model(named_inputs, return_inputs=False)
     # remove_from_outputs = ["stage"] + list(named_inputs)
     list(named_inputs)
     list(named_outputs)
 
     torch.jit.script(model)
```

### Comparing `torchbricks-0.1.0/tests/test_environment.py` & `torchbricks-0.3.0/tests/test_environment.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,14 +11,14 @@
 
     When we run `make update-lock-file` we will create a conda-lock file (`[repo]/conda-linux-64.lock`) and then make a copy of
     `[repo]/environement.yml` to `[repo]/tests/data/copy_lock_filed_environment.yml`.
 
     If `[repo]/environement.yml` and `[repo]/tests/data/copy_lock_filed_environment.yml` are not equal we expected the lock file to be
     outdated.
     """
-    path_current_env_file = path_repo_root() / 'environment.yml'
-    path_env_file_locked = path_repo_root() / 'tests' / 'data' / 'copy_lock_filed_environment.yml'
+    path_current_env_file = path_repo_root() / "environment.yml"
+    path_env_file_locked = path_repo_root() / "tests" / "data" / "copy_lock_filed_environment.yml"
 
     is_env_updated = filecmp.cmp(path_current_env_file, path_env_file_locked)
     assert is_env_updated, ("The 'environment.yml'-file have been updated and you need to update the environement lock-file. \n"
-                            f"Run 'make update-lock-file' to ensure {path_current_env_file} matches our env lock"
+                            f"Run 'make env-create-lock-file' to ensure {path_current_env_file} matches our env lock"
                             "file 'conda-linux-64.lock'")
```

### Comparing `torchbricks-0.1.0/tests/test_graph_builder.py` & `torchbricks-0.3.0/tests/test_graph_builder.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,39 +1,36 @@
-
 from typing import Dict
 
 from torch import nn
-from torchbricks.bag_of_bricks import ImageClassifier, Preprocessor
-from torchbricks.bricks import BrickCollection, BrickInterface, BrickLoss, BrickMetricSingle, BrickNotTrainable, BrickTrainable
+from torchbricks.bag_of_bricks.image_classification import ImageClassifier
+from torchbricks.bag_of_bricks.preprocessors import Preprocessor
+from torchbricks.brick_collection import BrickCollection
+from torchbricks.bricks import BrickInterface, BrickLoss, BrickMetricSingle, BrickNotTrainable, BrickTrainable
 from torchbricks.graph_plotter import create_mermaid_dag_graph
 from torchmetrics.classification import MulticlassAccuracy
 
 
 def test_graph_builder():
     def image_classifier_head(num_classes: int, in_channels: int, input_name: str) -> Dict[str, BrickInterface]:
-        """Image classifier bricks: Classifier, loss and metrics """
+        """Image classifier bricks: Classifier, loss and metrics"""
         head = {
-            'classify': BrickTrainable(ImageClassifier(num_classes=num_classes, n_features=in_channels),
-                                    input_names=[input_name],
-                                    output_names=['./logits', './probabilities', './class_prediction']),
-            'accuracy': BrickMetricSingle(MulticlassAccuracy(num_classes=num_classes),
-                                        input_names=['./class_prediction', 'targets']),
-            'loss': BrickLoss(model=nn.CrossEntropyLoss(),
-                            input_names=['./logits', 'targets'],
-                            output_names=['./loss_ce'])
+            "classify": BrickTrainable(
+                ImageClassifier(num_classes=num_classes, n_features=in_channels),
+                input_names=[input_name],
+                output_names=["./logits", "./probabilities", "./class_prediction"],
+            ),
+            "accuracy": BrickMetricSingle(MulticlassAccuracy(num_classes=num_classes), input_names=["./class_prediction", "targets"]),
+            "loss": BrickLoss(model=nn.CrossEntropyLoss(), input_names=["./logits", "targets"], output_names=["./loss_ce"]),
         }
         return head
 
     n_features = 5
     bricks = {
-        'preprocessor': BrickNotTrainable(Preprocessor(),
-                                        input_names=['raw'],
-                                        output_names=['normalized']),
-        'backbone': BrickTrainable(nn.Identity(), input_names=['normalized'], output_names=['features']),
-        'head0': image_classifier_head(num_classes=3, in_channels=n_features, input_name='features'),
-        'head1': image_classifier_head(num_classes=5, in_channels=n_features, input_name='features'),
+        "preprocessor": BrickNotTrainable(Preprocessor(), input_names=["raw"], output_names=["normalized"]),
+        "backbone": BrickTrainable(nn.Identity(), input_names=["normalized"], output_names=["features"]),
+        "head0": image_classifier_head(num_classes=3, in_channels=n_features, input_name="features"),
+        "head1": image_classifier_head(num_classes=5, in_channels=n_features, input_name="features"),
     }
 
     brick_collection = BrickCollection(bricks)
-
     print(create_mermaid_dag_graph(brick_collection))
     print()
```

### Comparing `torchbricks-0.1.0/tests/test_tensor_conversions.py` & `torchbricks-0.3.0/tests/test_tensor_conversions.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,26 +7,26 @@
     function_composer,
     unpack_batched_tensor_to_numpy_format,
     unpack_batched_tensor_to_pillow_images,
     unpack_batched_tensor_to_torchvision_format,
 )
 
 
-@pytest.mark.parametrize(['tensor_shape', 'tensor_shape_expected'],
+@pytest.mark.parametrize(["tensor_shape", "tensor_shape_expected"],
                          [((5,), (5,)),  # Same shape
                           ((5, 3), (5, 3)),  # Same shape
                           ((5, 3, 10), (5, 10, 3)),
                           ((5, 3, 10, 20), (5, 10, 20, 3)),
                           ((5, 3, 10, 20, 30), (5, 10, 20, 30, 3))])
 def test_batched_tensor_to_channel_last(tensor_shape, tensor_shape_expected):
     tensor = torch.ones(tensor_shape)
     result = batched_tensor_to_channel_last(tensor)
     assert result.shape == tensor_shape_expected
 
-@pytest.mark.parametrize(['tensor_shape', 'tensor_full_shape_expected'],
+@pytest.mark.parametrize(["tensor_shape", "tensor_full_shape_expected"],
                          [((5,), (5,)),  # Same shape
                           ((5, 3), (5, 3)),  # Same shape
                           ((5, 3, 10), (5, 10, 3)),
                           ((5, 3, 10, 20), (5, 10, 20, 3)),
                           ((5, 3, 10, 20, 30), (5, 10, 20, 30, 3))])
 def test_unpack_batched_tensor_to_numpy_format(tensor_shape, tensor_full_shape_expected):
     tensor = torch.ones(tensor_shape)
@@ -35,15 +35,15 @@
     if len(tensor_full_shape_expected) == 1:
         tensor_shape_expected = (1, )
     else:
         tensor_shape_expected = tensor_full_shape_expected[1:]
     assert result[0].shape == tensor_shape_expected
     assert isinstance(result[0], np.ndarray)
 
-@pytest.mark.parametrize(['tensor_shape', 'tensor_full_shape_expected'],
+@pytest.mark.parametrize(["tensor_shape", "tensor_full_shape_expected"],
                          [((5,), (5,)),  # Same shape
                           ((5, 3), (5, 3)),  # Same shape
                           ((5, 3, 10), (5, 3, 10)),
                           ((5, 3, 10, 20), (5, 3, 10, 20)),
                           ((5, 3, 10, 20, 30), (5, 3, 10, 20, 30))])
 def test_unpack_batched_tensor_to_torchvision_format(tensor_shape, tensor_full_shape_expected):
     tensor = torch.ones(tensor_shape)
@@ -60,15 +60,15 @@
     tensor_full_shape_expected = (5, 10, 20, 3)
     tensor = torch.ones(tensor_shape)
     result = unpack_batched_tensor_to_pillow_images(tensor)
     assert len(result) == tensor_full_shape_expected[0]
     assert isinstance(result[0], Image.Image)
     assert (result[0].height, result[0].width) == tensor_full_shape_expected[1:3]
 
-@pytest.mark.parametrize('tensor_shape', [(5, 3, 10), (5, 4, 10, 20)])
+@pytest.mark.parametrize("tensor_shape", [(5, 3, 10), (5, 4, 10, 20)])
 def test_unpack_batched_tensor_to_pillow_images_fail(tensor_shape):
     tensor = torch.ones(tensor_shape)
 
     with pytest.raises(AssertionError):
         unpack_batched_tensor_to_pillow_images(tensor)
 
 def test_function_composer():
```


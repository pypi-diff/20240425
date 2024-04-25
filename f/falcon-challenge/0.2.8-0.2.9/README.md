# Comparing `tmp/falcon_challenge-0.2.8.tar.gz` & `tmp/falcon_challenge-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "falcon_challenge-0.2.8.tar", last modified: Wed Apr 10 11:08:30 2024, max compression
+gzip compressed data, was "falcon_challenge-0.2.9.tar", last modified: Thu Apr 25 16:36:54 2024, max compression
```

## Comparing `falcon_challenge-0.2.8.tar` & `falcon_challenge-0.2.9.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:08:30.013023 falcon_challenge-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-10 11:08:21.000000 falcon_challenge-0.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4880 2024-04-10 11:08:30.013023 falcon_challenge-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4420 2024-04-10 11:08:21.000000 falcon_challenge-0.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:08:30.009023 falcon_challenge-0.2.8/decoder_demos/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 11:08:21.000000 falcon_challenge-0.2.8/decoder_demos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-04-10 11:08:21.000000 falcon_challenge-0.2.8/decoder_demos/decoding_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8406 2024-04-10 11:08:21.000000 falcon_challenge-0.2.8/decoder_demos/filtering.py
--rw-r--r--   0 runner    (1001) docker     (127)     4869 2024-04-10 11:08:21.000000 falcon_challenge-0.2.8/decoder_demos/ndt2_decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-04-10 11:08:21.000000 falcon_challenge-0.2.8/decoder_demos/ndt2_sample.py
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-10 11:08:21.000000 falcon_challenge-0.2.8/decoder_demos/random_decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-10 11:08:21.000000 falcon_challenge-0.2.8/decoder_demos/rnn_decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)    11789 2024-04-10 11:08:21.000000 falcon_challenge-0.2.8/decoder_demos/sklearn_decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-10 11:08:21.000000 falcon_challenge-0.2.8/decoder_demos/sklearn_sample.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:08:30.009023 falcon_challenge-0.2.8/falcon_challenge/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 11:08:21.000000 falcon_challenge-0.2.8/falcon_challenge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-10 11:08:21.000000 falcon_challenge-0.2.8/falcon_challenge/challenge_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-04-10 11:08:21.000000 falcon_challenge-0.2.8/falcon_challenge/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7992 2024-04-10 11:08:21.000000 falcon_challenge-0.2.8/falcon_challenge/dataloaders.py
--rw-r--r--   0 runner    (1001) docker     (127)    17333 2024-04-10 11:08:21.000000 falcon_challenge-0.2.8/falcon_challenge/evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-04-10 11:08:21.000000 falcon_challenge-0.2.8/falcon_challenge/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:08:30.009023 falcon_challenge-0.2.8/falcon_challenge.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4880 2024-04-10 11:08:29.000000 falcon_challenge-0.2.8/falcon_challenge.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-04-10 11:08:30.000000 falcon_challenge-0.2.8/falcon_challenge.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 11:08:29.000000 falcon_challenge-0.2.8/falcon_challenge.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-10 11:08:29.000000 falcon_challenge-0.2.8/falcon_challenge.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-10 11:08:29.000000 falcon_challenge-0.2.8/falcon_challenge.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:08:30.009023 falcon_challenge-0.2.8/preproc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 11:08:21.000000 falcon_challenge-0.2.8/preproc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-10 11:08:21.000000 falcon_challenge-0.2.8/preproc/assemble_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     8389 2024-04-10 11:08:21.000000 falcon_challenge-0.2.8/preproc/filtering.py
--rw-r--r--   0 runner    (1001) docker     (127)     6319 2024-04-10 11:08:21.000000 falcon_challenge-0.2.8/preproc/h2_preproc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4049 2024-04-10 11:08:21.000000 falcon_challenge-0.2.8/preproc/m1_fewshot_trial_counts.py
--rw-r--r--   0 runner    (1001) docker     (127)    23601 2024-04-10 11:08:21.000000 falcon_challenge-0.2.8/preproc/m1_reachgrasp_preprocv2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-04-10 11:08:21.000000 falcon_challenge-0.2.8/preproc/m2_fewshot_trial_counts.py
--rw-r--r--   0 runner    (1001) docker     (127)    13083 2024-04-10 11:08:21.000000 falcon_challenge-0.2.8/preproc/m2_preproc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-04-10 11:08:21.000000 falcon_challenge-0.2.8/preproc/merge_answers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-04-10 11:08:21.000000 falcon_challenge-0.2.8/preproc/nwb_create_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-10 11:08:21.000000 falcon_challenge-0.2.8/preproc/wrapper_convert_batch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-04-10 11:08:21.000000 falcon_challenge-0.2.8/preproc/zip_data.py
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-10 11:08:21.000000 falcon_challenge-0.2.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 11:08:30.013023 falcon_challenge-0.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-10 11:08:21.000000 falcon_challenge-0.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:36:54.377393 falcon_challenge-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-25 16:36:50.000000 falcon_challenge-0.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4930 2024-04-25 16:36:54.377393 falcon_challenge-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4420 2024-04-25 16:36:50.000000 falcon_challenge-0.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:36:54.373393 falcon_challenge-0.2.9/decoder_demos/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 16:36:50.000000 falcon_challenge-0.2.9/decoder_demos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-04-25 16:36:50.000000 falcon_challenge-0.2.9/decoder_demos/decoding_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8568 2024-04-25 16:36:50.000000 falcon_challenge-0.2.9/decoder_demos/filtering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5854 2024-04-25 16:36:50.000000 falcon_challenge-0.2.9/decoder_demos/ndt2_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-04-25 16:36:50.000000 falcon_challenge-0.2.9/decoder_demos/ndt2_sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-25 16:36:50.000000 falcon_challenge-0.2.9/decoder_demos/random_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-25 16:36:50.000000 falcon_challenge-0.2.9/decoder_demos/rnn_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13336 2024-04-25 16:36:50.000000 falcon_challenge-0.2.9/decoder_demos/sklearn_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-04-25 16:36:50.000000 falcon_challenge-0.2.9/decoder_demos/sklearn_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:36:54.373393 falcon_challenge-0.2.9/falcon_challenge/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 16:36:50.000000 falcon_challenge-0.2.9/falcon_challenge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-25 16:36:50.000000 falcon_challenge-0.2.9/falcon_challenge/challenge_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3762 2024-04-25 16:36:50.000000 falcon_challenge-0.2.9/falcon_challenge/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8214 2024-04-25 16:36:50.000000 falcon_challenge-0.2.9/falcon_challenge/dataloaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25871 2024-04-25 16:36:50.000000 falcon_challenge-0.2.9/falcon_challenge/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2317 2024-04-25 16:36:50.000000 falcon_challenge-0.2.9/falcon_challenge/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:36:54.377393 falcon_challenge-0.2.9/falcon_challenge.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4930 2024-04-25 16:36:54.000000 falcon_challenge-0.2.9/falcon_challenge.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-04-25 16:36:54.000000 falcon_challenge-0.2.9/falcon_challenge.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 16:36:54.000000 falcon_challenge-0.2.9/falcon_challenge.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-25 16:36:54.000000 falcon_challenge-0.2.9/falcon_challenge.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-25 16:36:54.000000 falcon_challenge-0.2.9/falcon_challenge.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:36:54.377393 falcon_challenge-0.2.9/preproc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 16:36:50.000000 falcon_challenge-0.2.9/preproc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-25 16:36:50.000000 falcon_challenge-0.2.9/preproc/assemble_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8389 2024-04-25 16:36:50.000000 falcon_challenge-0.2.9/preproc/filtering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6319 2024-04-25 16:36:50.000000 falcon_challenge-0.2.9/preproc/h2_preproc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4049 2024-04-25 16:36:50.000000 falcon_challenge-0.2.9/preproc/m1_fewshot_trial_counts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23601 2024-04-25 16:36:50.000000 falcon_challenge-0.2.9/preproc/m1_reachgrasp_preprocv2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-04-25 16:36:50.000000 falcon_challenge-0.2.9/preproc/m2_fewshot_trial_counts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16660 2024-04-25 16:36:50.000000 falcon_challenge-0.2.9/preproc/m2_preproc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-04-25 16:36:50.000000 falcon_challenge-0.2.9/preproc/merge_answers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-04-25 16:36:50.000000 falcon_challenge-0.2.9/preproc/nwb_create_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-25 16:36:50.000000 falcon_challenge-0.2.9/preproc/wrapper_convert_batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-04-25 16:36:50.000000 falcon_challenge-0.2.9/preproc/zip_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-25 16:36:50.000000 falcon_challenge-0.2.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 16:36:54.377393 falcon_challenge-0.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-25 16:36:50.000000 falcon_challenge-0.2.9/setup.py
```

### Comparing `falcon_challenge-0.2.8/LICENSE` & `falcon_challenge-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.2.8/PKG-INFO` & `falcon_challenge-0.2.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: falcon_challenge
-Version: 0.2.8
+Version: 0.2.9
 Home-page: https://github.com/snel-repo/stability-benchmark
 Author: Joel Ye
 Author-email: joelye9@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: hydra-core
@@ -12,14 +12,16 @@
 Requires-Dist: tqdm
 Requires-Dist: scipy
 Requires-Dist: pandas
 Requires-Dist: seaborn
 Requires-Dist: scikit-learn
 Requires-Dist: pynwb
 Requires-Dist: torch
+Requires-Dist: edit_distance
+Requires-Dist: dandi
 
 # FALCON Benchmark and Challenge
 
 This package contains core code for submitting decoders to the FALCON challenge. Full github contains additional examples and documentation.
 
 ## Installation
 Install `falcon_challenge` with:
```

### Comparing `falcon_challenge-0.2.8/README.md` & `falcon_challenge-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.2.8/decoder_demos/decoding_utils.py` & `falcon_challenge-0.2.9/decoder_demos/decoding_utils.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.2.8/decoder_demos/filtering.py` & `falcon_challenge-0.2.9/preproc/filtering.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import torch.nn.functional as F
 
 r"""
     H1 filtering
 """
 NEURAL_TAU_MS = 240. # exponential filter from H1 Lab
 def apply_exponential_filter(
-        x, tau=NEURAL_TAU_MS, bin_size=20, extent: int=1
+        x, tau=NEURAL_TAU_MS, bin_size=10, extent: int=1
     ):
     """
     Apply a **causal** exponential filter to the neural signal.
 
     :param x: NumPy array of shape (time, channels)
     :param tau: Decay rate (time constant) of the exponential filter
     :param bin_size: Bin size in ms (default is 10ms)
@@ -27,29 +27,28 @@
     kernel = np.exp(-t / tau)
     kernel /= np.sum(kernel)
     # Apply the filter
     filtered_signal = np.array([signal.convolve(x[:, ch], kernel, mode='full')[:len(x)] for ch in range(x.shape[1])]).T
     return filtered_signal
 
 
-
 def gaussian_kernel(size, sigma):
     """
     Create a 1D Gaussian kernel.
     """
     size = int(size)
     x = np.linspace(-size // 2, size // 2, size)
     kernel = np.exp(-0.5 * (x / sigma) ** 2)
     kernel /= kernel.sum()
     return kernel
 
 def smooth(position, kernel_size: int, sigma: float):
     """
     Apply Gaussian smoothing on the position data (dim 0)
-    kernel_size: size of the kernel (in input bins)
+    kernel_size: size of the kernel
     sigma: standard deviation of the Gaussian kernel
     """
     kernel = gaussian_kernel(kernel_size, sigma)
     pad_total = kernel_size - 1
     pad_left = pad_total // 2
     pad_right = pad_total - pad_left
```

### Comparing `falcon_challenge-0.2.8/decoder_demos/ndt2_decoder.py` & `falcon_challenge-0.2.9/decoder_demos/ndt2_decoder.py`

 * *Files 20% similar despite different names*

```diff
@@ -33,21 +33,22 @@
 
     def __init__(
             self,
             task_config: FalconConfig,
             model_ckpt_path: str,
             model_cfg_stem: str,
             zscore_path: str,
-            dataset_handles: List[str] = []
+            dataset_handles: List[str] = [],
+            batch_size: int = 1
         ):
         r"""
             Loading NDT2 requires both weights and model config. Weight loading through a checkpoint is standard.
             Model config is typically stored on wandb, but this is not portable enough. Instead, directly reference the model config file.
         """
-        self._task_config = task_config
+        super().__init__(task_config=task_config, batch_size=batch_size)
         self.exp_task = getattr(ExperimentalTask, f'falcon_{task_config.task.name}')
         try:
             initialize_config_module(
                 config_module="context_general_bci.config",
                 job_name="falcon",
                 version_base="1.3",
             )
@@ -67,48 +68,63 @@
             MetaKey.subject.name: [self.subject],
             MetaKey.session.name: sorted([self._task_config.hash_dataset(handle) for handle in dataset_handles]),
             MetaKey.task.name: [self.exp_task],
         }
         data_attrs = DataAttrs.from_config(cfg.dataset, context=ContextAttrs(**context_idx))
         cfg.model.task.decode_normalizer = zscore_path
         model = load_from_checkpoint(model_ckpt_path, cfg=cfg.model, data_attrs=data_attrs)
-        model = transfer_model(model, cfg.model, data_attrs)
+        model = transfer_model(model, cfg.model, data_attrs, batch_size=batch_size)
         self.model = model.to('cuda:0')
         self.model.eval()
 
         assert task_config.bin_size_ms == cfg.dataset.bin_size_ms, "Bin size mismatch, transform not implemented."
-        self.observation_buffer = torch.zeros((cfg.dataset.max_length_ms // task_config.bin_size_ms, task_config.n_channels), dtype=torch.uint8, device='cuda:0')
+        self.observation_buffer = torch.zeros((
+            cfg.dataset.max_length_ms // task_config.bin_size_ms, 
+            self.batch_size,
+            task_config.n_channels
+        ), dtype=torch.uint8, device='cuda:0')
 
-    def reset(self, dataset: Path = ""):
-        dataset_tag = dataset.stem
+    def reset(self, dataset_tags: List[Path] = [""]):
         self.set_steps = 0
         self.observation_buffer.zero_()
-        self.meta_key = torch.tensor([
-            self.model.data_attrs.context.session.index(
-                self._task_config.hash_dataset(dataset_tag)
-            )], device='cuda:0')
+        dataset_tags = [self._task_config.hash_dataset(dset.stem) for dset in dataset_tags]
+        meta_keys = []
+        for dataset_tag in dataset_tags:
+            if dataset_tag not in self.model.data_attrs.context.session:
+                raise ValueError(f"Dataset tag {dataset_tag} not found in calibration sets {self.model.data_attrs.context.session} - did you calibrate on this dataset?")
+            meta_keys.append(self.model.data_attrs.context.session.index(dataset_tag))
+        self.meta_key = torch.tensor(meta_keys, device='cuda:0')
 
     def predict(self, neural_observations: np.ndarray):
         r"""
-            neural_observations: array of shape (n_channels), binned spike counts
+            neural_observations: array of shape (batch, n_channels), binned spike counts
+            
+            return:
+                out: (batch, n_dims)
         """
         self.observe(neural_observations)
-        decoder_in = rearrange(self.observation_buffer[-self.set_steps:], 't c -> 1 t c 1')
-        out = self.model(decoder_in, self.meta_key) # Remove batch dim
-        return out[0].cpu().numpy()
+        decoder_in = rearrange(self.observation_buffer[-self.set_steps:], 't b c -> b t c 1')
+        out = self.model(decoder_in, self.meta_key)
+        return out.cpu().numpy()
+
     
     def observe(self, neural_observations: np.ndarray):
         r"""
-            neural_observations: array of shape (n_channels), binned spike counts
+            neural_observations: array of shape (batch, n_channels), binned spike counts
             - for timestamps where we don't want predictions but neural data may be informative (start of trial)
         """
+        if neural_observations.shape[0] < self.batch_size:
+            neural_observations = np.pad(neural_observations, ((0, self.batch_size - neural_observations.shape[0]), (0, 0)))
         self.set_steps += 1
         self.observation_buffer = torch.roll(self.observation_buffer, -1, dims=0)
+        # self.observation_buffer[-1] = neural_observations # , dtype=torch.uint8, device='cuda:0')
         self.observation_buffer[-1] = torch.as_tensor(neural_observations, dtype=torch.uint8, device='cuda:0')
 
-    def on_trial_end(self):
+    def on_dones(self, dones: np.ndarray):
         # reset - for some reason m1 benefits from this
         self.set_steps = 0
-        self.observation_buffer.zero_()
+        if dones.shape[0] < self.batch_size:
+            dones = np.pad(dones, (0, self.batch_size - dones.shape[0]))
+        self.observation_buffer[:, dones].zero_()
 
 if __name__ == "__main__":
     print(f"No train/calibration capabilities in {__file__}, use `context_general_bci` codebase.")
```

### Comparing `falcon_challenge-0.2.8/decoder_demos/ndt2_sample.py` & `falcon_challenge-0.2.9/decoder_demos/ndt2_sample.py`

 * *Files 9% similar despite different names*

```diff
@@ -30,29 +30,33 @@
     )
     parser.add_argument(
         '--split', type=str, choices=['h1', 'h2', 'm1', 'm2'], default='h1',
     )
     parser.add_argument(
         '--phase', choices=['minival', 'test'], default='minival'
     )
+    parser.add_argument(
+        '--batch-size', type=int, default=1
+    )
     args = parser.parse_args()
 
     evaluator = FalconEvaluator(
         eval_remote=args.evaluation == "remote",
         split=args.split)
 
     task = getattr(FalconTask, args.split)
     config = FalconConfig(task=task)
 
     decoder = NDT2Decoder(
         task_config=config,
         model_ckpt_path=args.model_path,
         model_cfg_stem=args.config_stem,
         zscore_path=args.zscore_path,
-        dataset_handles=[x.stem for x in evaluator.get_eval_files(phase=args.phase)]
+        dataset_handles=[x.stem for x in evaluator.get_eval_files(phase=args.phase)],
+        batch_size=args.batch_size
     )
 
 
     evaluator.evaluate(decoder, phase=args.phase)
 
 
 if __name__ == "__main__":
```

### Comparing `falcon_challenge-0.2.8/decoder_demos/random_decoder.py` & `falcon_challenge-0.2.9/decoder_demos/random_decoder.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.2.8/decoder_demos/rnn_decoder.py` & `falcon_challenge-0.2.9/decoder_demos/rnn_decoder.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.2.8/decoder_demos/sklearn_decoder.py` & `falcon_challenge-0.2.9/decoder_demos/sklearn_decoder.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 r"""
     Load an sklearn decoder.
     To train, for example:
-    `python decoder_demos/sklearn_decoder.py --training_dir data/h1/held_in_calib --calibration_dir data/h1/held_out_calib --mode all`
+    `python decoder_demos/sklearn_decoder.py --training_dir data/h1/held_in_calib --calibration_dir data/h1/held_out_calib --mode all --task h1`
     To evaluate, see `sklearn_sample.py`
 """
 from typing import List, Union, Optional
 import argparse
 import pickle
 import numpy as np
 from pathlib import Path
@@ -25,28 +25,32 @@
 )
 
 def prepare_train_test(
         binned_spikes: np.ndarray,
         targets: np.ndarray,
         blacklist: Optional[np.ndarray]=None,
         history: int=0,
+        mask_still_times: bool=True
         ):
     signal = apply_exponential_filter(binned_spikes)
 
-    # Remove timepoints where nothing is happening in the kinematics
-    still_times = np.all(np.abs(targets) < 0.001, axis=1)
-    if blacklist is not None:
-        blacklist = still_times | blacklist
+    # Remove timepoints where nothing is happening in the kinematics (relevant esp for H1)
+    if mask_still_times:
+        still_times = np.all(np.abs(targets) < 0.001, axis=1)
+        if blacklist is not None:
+            blacklist = still_times | blacklist
+        else:
+            blacklist = still_times
     else:
-        blacklist = still_times
+        if blacklist is None:
+            blacklist = np.zeros(targets.shape[0], dtype=bool)
 
     train_x, test_x = np.split(signal, [int(TRAIN_TEST[0] * signal.shape[0])])
     train_y, test_y = np.split(targets, [int(TRAIN_TEST[0] * targets.shape[0])])
     train_blacklist, test_blacklist = np.split(blacklist, [int(TRAIN_TEST[0] * blacklist.shape[0])])
-
     x_mean, x_std = np.nanmean(train_x, axis=0), np.nanstd(train_x, axis=0)
     x_std[x_std == 0] = 1
     y_mean, y_std = np.nanmean(train_y[~train_blacklist], axis=0), np.nanstd(train_y[~train_blacklist], axis=0)
     y_std[y_std == 0] = 1
     train_x = (train_x - x_mean) / x_std
     test_x = (test_x - x_mean) / x_std
     # train_y = (train_y - y_mean) / y_std # don't standardize y if using var weighted r2
@@ -76,66 +80,85 @@
 
     return train_x, train_y, test_x, test_y, x_mean, x_std, y_mean, y_std
 
 class SKLearnDecoder(BCIDecoder):
     r"""
         Load an sklearn decoder. Assumes the dimensionality is correct.
     """
-    def __init__(self, task_config: FalconConfig, model_path: str):
+    def __init__(self, task_config: FalconConfig, model_path: str, batch_size: int = 1):
+        super().__init__(task_config=task_config, batch_size=batch_size)
         self._task_config = task_config
+        self.batch_size = batch_size
         with open(model_path, 'rb') as f:
             payload = pickle.load(f)
             assert payload['task'] == task_config.task
             self.clf = payload['decoder']
             self.history = payload['history'] + 1
             MAX_HISTORY = int(NEURAL_TAU_MS / task_config.bin_size_ms) * 5 # bin size ms
             self.x_mean = payload['x_mean']
             self.x_std = payload['x_std']
-            self.raw_history_buffer = np.zeros((MAX_HISTORY, task_config.n_channels))
-            self.observation_buffer = np.zeros((self.history, task_config.n_channels))
+            self.raw_history_buffer = np.zeros((MAX_HISTORY, batch_size, task_config.n_channels))
+            self.observation_buffer = np.zeros((self.history, batch_size, task_config.n_channels))
 
-    def reset(self, dataset: Path = ""):
+    def reset(self, dataset_tags: List[Path] = [""]):
         if isinstance(self.x_mean, dict):
-            dataset_tag =  self._task_config.hash_dataset(dataset.stem)
-            if dataset_tag not in self.x_mean:
-                raise ValueError(f"Dataset tag {dataset_tag} not found in calibration set {self.x_mean.keys()} - did you calibrate on this dataset?")
-            self.local_x_mean = self.x_mean[dataset_tag]
-            self.local_x_std = self.x_std[dataset_tag]
+            # TODO retrieve a list of x_means
+            dataset_tags = [self._task_config.hash_dataset(dset.stem) for dset in dataset_tags]
+            for dataset_tag in dataset_tags:
+                if dataset_tag not in self.x_mean:
+                    raise ValueError(f"Dataset tag {dataset_tag} not found in calibration set {self.x_mean.keys()} - did you calibrate on this dataset?")
+            self.local_x_mean = [self.x_mean[dset_tag] for dset_tag in dataset_tags]
+            self.local_x_std = [self.x_std[dset_tag] for dset_tag in dataset_tags]
         else:
             self.local_x_mean = self.x_mean
             self.local_x_std = self.x_std
+        # TODO this one too...
         if isinstance(self.clf, dict):
-            dataset_tag =  self._task_config.hash_dataset(dataset.stem)
-            if dataset_tag not in self.clf:
-                raise ValueError(f"Dataset tag {dataset_tag} not found decoder set {self.clf.keys()}")
-            self.local_clf = self.clf[dataset_tag]
+            dataset_tags = [self._task_config.hash_dataset(dset.stem) for dset in dataset_tags]
+            for dataset_tag in dataset_tags:
+                if dataset_tag not in self.clf:
+                    raise ValueError(f"Dataset tag {dataset_tag} not found decoder set {self.clf.keys()}")
+            self.local_clf = [self.clf[dataset_tag] for dataset_tag in dataset_tags]
         else:
             self.local_clf = self.clf
         self.raw_history_buffer = np.zeros_like(self.raw_history_buffer)
         self.observation_buffer = np.zeros_like(self.observation_buffer)
 
     def predict(self, neural_observations: np.ndarray):
         r"""
-            neural_observations: array of shape (n_channels), binned spike counts
+            neural_observations: array of shape (batch, n_channels), binned spike counts
+            
+            return: array of shape (batch, n_features), predicted kinematics
         """
         self.observe(neural_observations)
-        decoder_in = self.observation_buffer[::-1].copy().flatten().reshape(1, -1) # Reverse since this happens to be how the lagged matrix is formatted
-        out = self.local_clf.predict(decoder_in)[0]
-        return out
+        decoder_in = self.observation_buffer[::-1].copy().transpose(  # Reverse since this happens to be how the lagged matrix is formatted
+            1, 0, 2 # batch, history, channels
+        ).reshape(self.observation_buffer.shape[1], -1)
+        if isinstance(self.clf, dict):
+            out = []
+            for idx in range(len(self.local_clf)):
+                out.append(self.local_clf[idx].predict(decoder_in[idx:idx+1])[0]) # needs batch=1 dim
+            return np.stack(out, 0)
+        else:
+            return self.local_clf.predict(decoder_in[:neural_observations.shape[0]])
 
     def observe(self, neural_observations: np.ndarray):
         r"""
-            neural_observations: array of shape (n_channels), binned spike counts
+            neural_observations: array of shape (batch, n_channels), binned spike counts
             - for timestamps where we don't want predictions but neural data may be informative (start of trial)
         """
+        # pad neural observation to batch size
+        if neural_observations.shape[0] < self.batch_size:
+            neural_observations = np.pad(neural_observations, ((0, self.batch_size - neural_observations.shape[0]), (0, 0)))
         self.raw_history_buffer = np.roll(self.raw_history_buffer, -1, axis=0)
         self.raw_history_buffer[-1] = neural_observations
-        smth_history = apply_exponential_filter(self.raw_history_buffer, NEURAL_TAU_MS)
         self.observation_buffer = np.roll(self.observation_buffer, -1, axis=0)
-        self.observation_buffer[-1] = (smth_history[-1] - self.local_x_mean) / self.local_x_std
+        for idx in range(len(self.local_x_mean)):
+            smth_history_idx = apply_exponential_filter(self.raw_history_buffer[:, idx], NEURAL_TAU_MS)
+            self.observation_buffer[-1, idx] = (smth_history_idx[-1] - self.local_x_mean[idx]) / self.local_x_std[idx]
 
 def fit_sklearn_decoder(
     datafiles: List[Path],
     calibration_datafiles: List[Path],
     task_config: FalconConfig,
     save_path: Path,
     history = 0,
@@ -158,15 +181,15 @@
         train_y,
         test_x,
         test_y,
         x_mean,
         x_std,
         y_mean,
         y_std
-    ) = prepare_train_test(all_neural_data, all_covariates, ~all_eval_mask, history=history)
+    ) = prepare_train_test(all_neural_data, all_covariates, ~all_eval_mask, history=history, mask_still_times=task_config.task == FalconTask.h1)
     score, decoder = fit_and_eval_decoder(train_x, train_y, test_x, test_y)
     print(f"CV Fit score: {score:.2f}")
     (
         cal_neural_data,
         _,
         _,
         _,
```

### Comparing `falcon_challenge-0.2.8/decoder_demos/sklearn_sample.py` & `falcon_challenge-0.2.9/decoder_demos/sklearn_sample.py`

 * *Files 16% similar despite different names*

```diff
@@ -18,22 +18,23 @@
     )
     parser.add_argument(
         '--split', type=str, choices=['h1', 'h2', 'm1', 'm2'], default='h1',
     )
     parser.add_argument(
         '--phase', choices=['minival', 'test'], default='minival'
     )
+    parser.add_argument('--batch-size', type=int, help='size of batch for evaluation', default=1)
     args = parser.parse_args()
 
     task = getattr(FalconTask, args.split)
     config = FalconConfig(
         task=task,
     )
 
-    decoder = SKLearnDecoder(task_config=config, model_path=args.model_path)
+    decoder = SKLearnDecoder(task_config=config, model_path=args.model_path, batch_size=args.batch_size)
 
     evaluator = FalconEvaluator(
         eval_remote=args.evaluation == "remote",
         split=args.split,
     )
     evaluator.evaluate(decoder, phase=args.phase)
```

### Comparing `falcon_challenge-0.2.8/falcon_challenge/config.py` & `falcon_challenge-0.2.9/falcon_challenge/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,13 @@
+from __future__ import annotations
+
 import enum
 from typing import Union
 from pathlib import Path
+import datetime
 from dataclasses import dataclass, field
 
 from hydra.core.config_store import ConfigStore
 from hydra.core.config_search_path import ConfigSearchPath
 from hydra.plugins.search_path_plugin import SearchPathPlugin
 
 
@@ -69,19 +72,27 @@
             # remove split and set information
             # pieces = handle.split('_')
             # for piece in pieces:
                 # if piece[0].lower() == 's' and piece != 'set':
                     # return piece
             raise ValueError(f"Could not find session in {handle}.")
         elif self.task == FalconTask.h2:
-            return handle.split('_')[-1].split('-')[-1]
+            return handle.split('_')[1]
         elif self.task == FalconTask.m1: # return date
             # sub-MonkeyL-held-in-minival_ses-20120924_behavior+ecephys.nwb
             # or L_20120924_held_in_eval.nwb
             if 'behavior+ecephys' in handle:
                 return handle.split('_')[-2].split('-')[-1]
             return handle.split('_')[1]
         elif self.task == FalconTask.m2:
-            raise NotImplementedError("M2 not implemented.")
+            if 'behavior+ecephys' in handle: # public sub-MonkeyN-held-in-calib_ses-2020-10-19-Run1_behavior+ecephys.nwb
+                return handle.split('_')[-2][4:] # -> 2020-10-19-Run1
+            # sub-MonkeyNRun1_20201019_held_in_eval.nwb 
+            run_str = handle.split('_')[0][-4:]
+            date_str = handle.split('_')[1]
+            date = datetime.datetime.strptime(date_str, '%Y%m%d')
+            date_str_fmt = date.strftime('%Y-%m-%d')
+            return f'{date_str_fmt}-{run_str}'
+            
 
 cs = ConfigStore.instance()
 cs.store(name="falcon_config", node=FalconConfig)
```

### Comparing `falcon_challenge-0.2.8/falcon_challenge/dataloaders.py` & `falcon_challenge-0.2.9/falcon_challenge/dataloaders.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,16 @@
         else:
             bin_end_timestamps = bin_timestamps
         # Check contiguous else force cropping for even bins
         gaps = np.diff(bin_end_timestamps)
         if (gaps <= 0).any():
             raise ValueError("bin_end_timestamps must be monotonically increasing.")
         if not np.allclose(gaps, bin_size_s):
-            print(f"Warning: Input timestamps not spaced like requested {bin_size_s}. Outputting proximal bin spikes.")
+            not_close = (~np.isclose(gaps, bin_size_s)).sum()
+            print(f"Warning: Input has {not_close} timestamps not spaced like requested {bin_size_s}. Outputting proximal bin spikes.")
             # Adjust bin_end_timestamps to include bins at the end of discontinuities
             new_bin_ends = [bin_end_timestamps[0]]
             bin_mask = [True] # bool, True if bin ending at this timepoint should be included post mask (not padding)
             for i, gap in enumerate(gaps):
                 if not np.isclose(gap, bin_size_s) and gap > bin_size_s:
                     cur_bin_end = bin_end_timestamps[i+1]
                     new_bin_ends.extend([cur_bin_end - bin_size_s, cur_bin_end])
@@ -100,15 +101,18 @@
             binned_spikes = nwbfile.acquisition['binned_spikes'].data[()]
             time = nwbfile.acquisition['binned_spikes'].timestamps[()]
             eval_mask = nwbfile.acquisition['eval_mask'].data[()].astype(bool)
             trial_info = (
                 nwbfile.trials.to_dataframe()
                 .reset_index()
             )
-            return binned_spikes, trial_info.cue.values, np.concatenate([[False], np.diff(time) > 0.02]), eval_mask
+            targets = []
+            for _, row in trial_info.iterrows():
+                targets.append(np.array([ord(c) for c in row.cue], dtype=np.int32))
+            return binned_spikes, targets, np.concatenate([np.diff(time) > 0.021, [True]]), eval_mask
         elif dataset == FalconTask.m1:
             units = nwbfile.units.to_dataframe()
             raw_emg = nwbfile.acquisition['preprocessed_emg']
             muscles = [ts for ts in raw_emg.time_series]
             emg_data = []
             emg_timestamps = []
             for m in muscles:
```

### Comparing `falcon_challenge-0.2.8/falcon_challenge.egg-info/PKG-INFO` & `falcon_challenge-0.2.9/falcon_challenge.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: falcon_challenge
-Version: 0.2.8
+Version: 0.2.9
 Home-page: https://github.com/snel-repo/stability-benchmark
 Author: Joel Ye
 Author-email: joelye9@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: hydra-core
@@ -12,14 +12,16 @@
 Requires-Dist: tqdm
 Requires-Dist: scipy
 Requires-Dist: pandas
 Requires-Dist: seaborn
 Requires-Dist: scikit-learn
 Requires-Dist: pynwb
 Requires-Dist: torch
+Requires-Dist: edit_distance
+Requires-Dist: dandi
 
 # FALCON Benchmark and Challenge
 
 This package contains core code for submitting decoders to the FALCON challenge. Full github contains additional examples and documentation.
 
 ## Installation
 Install `falcon_challenge` with:
```

### Comparing `falcon_challenge-0.2.8/falcon_challenge.egg-info/SOURCES.txt` & `falcon_challenge-0.2.9/falcon_challenge.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.2.8/preproc/assemble_data.py` & `falcon_challenge-0.2.9/preproc/assemble_data.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.2.8/preproc/filtering.py` & `falcon_challenge-0.2.9/decoder_demos/filtering.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,51 +4,55 @@
 import torch.nn.functional as F
 
 r"""
     H1 filtering
 """
 NEURAL_TAU_MS = 240. # exponential filter from H1 Lab
 def apply_exponential_filter(
-        x, tau=NEURAL_TAU_MS, bin_size=10, extent: int=1
+        x, tau=NEURAL_TAU_MS, bin_size=20, extent: int=1
     ):
     """
     Apply a **causal** exponential filter to the neural signal.
 
     :param x: NumPy array of shape (time, channels)
     :param tau: Decay rate (time constant) of the exponential filter
     :param bin_size: Bin size in ms (default is 10ms)
     :return: Filtered signal
     :param extent: Number of time constants to extend the filter kernel
 
     Implementation notes:
     # extent should be 3 for reporting parity, but reference hardcodes a kernel that's equivalent to extent=1
     """
+    assert len(x.shape) == 2, "Still need to implement 3D convolve..."
     t = np.arange(0, extent * tau, bin_size)
     # Exponential filter kernel
     kernel = np.exp(-t / tau)
     kernel /= np.sum(kernel)
+    # if len(x.shape) == 3: # This seems wrong
+        # kernel = kernel[:, np.newaxis]
     # Apply the filter
-    filtered_signal = np.array([signal.convolve(x[:, ch], kernel, mode='full')[:len(x)] for ch in range(x.shape[1])]).T
+    filtered_signal = np.array([signal.convolve(x[..., ch], kernel, mode='full')[:len(x)] for ch in range(x.shape[-1])]).T
     return filtered_signal
 
 
+
 def gaussian_kernel(size, sigma):
     """
     Create a 1D Gaussian kernel.
     """
     size = int(size)
     x = np.linspace(-size // 2, size // 2, size)
     kernel = np.exp(-0.5 * (x / sigma) ** 2)
     kernel /= kernel.sum()
     return kernel
 
 def smooth(position, kernel_size: int, sigma: float):
     """
     Apply Gaussian smoothing on the position data (dim 0)
-    kernel_size: size of the kernel
+    kernel_size: size of the kernel (in input bins)
     sigma: standard deviation of the Gaussian kernel
     """
     kernel = gaussian_kernel(kernel_size, sigma)
     pad_total = kernel_size - 1
     pad_left = pad_total // 2
     pad_right = pad_total - pad_left
```

### Comparing `falcon_challenge-0.2.8/preproc/h2_preproc.py` & `falcon_challenge-0.2.9/preproc/h2_preproc.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.2.8/preproc/m1_fewshot_trial_counts.py` & `falcon_challenge-0.2.9/preproc/m1_fewshot_trial_counts.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.2.8/preproc/m1_reachgrasp_preprocv2.py` & `falcon_challenge-0.2.9/preproc/m1_reachgrasp_preprocv2.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.2.8/preproc/m2_fewshot_trial_counts.py` & `falcon_challenge-0.2.9/preproc/m2_fewshot_trial_counts.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.2.8/preproc/m2_preproc.py` & `falcon_challenge-0.2.9/preproc/m2_preproc.py`

 * *Files 24% similar despite different names*

```diff
@@ -73,46 +73,51 @@
     'Z_Joker_2020-11-18_Run-001': 1,
     'Z_Joker_2020-11-19_Run-001': 1,
     'Z_Joker_2020-11-24_Run-001': 1,
     'Z_Joker_2020-11-24_Run-002': 2
 }
 # Note that intertrial spikes are not available
 #%%
-def create_nwb_shell(path: Path, split, suffix='full'):
+def create_nwb_shell(path: Path, split, suffix='full', extra_note=""):
     start_date = path.stem.split('_')[2] # YYYY-MM-DD
     session_start_time = datetime.strptime(start_date, '%Y-%m-%d')
     # inject arbitrary hour to distinguish sets
     session_start_time = session_start_time.replace(hour=12 + DATA_RUN_SET[path.stem])
-    hash = '_'.join(path.stem.split('_')[2:])
+    # hash = '_'.join(path.stem.split('_')[2:]) # includes date and run, remap run
+    session_hash = start_date + '_' + f'Run{DATA_RUN_SET[path.stem]}'
+    # breakpoint()
     subject = pynwb.file.Subject(
         subject_id=f'MonkeyN-{split}-{suffix}',
-        description='MonkeyN, Chestek Lab, number indicates experimental set from day',
+        description=f'MonkeyN, Chestek Lab, number indicates experimental set from day.{extra_note}',
         species='Rhesus macaque',
         sex='M',
         age='P8Y',
     )
+    file_id = f'MonkeyN_{session_start_time.strftime("%m-%d-%H:%M")}_{split}'
+    # file_id = f'MonkeyN_{session_start_time.strftime("%m-%d-%H:%M")}_run{DATA_RUN_SET[path.stem]}_{split}'
     f = NWBFile(
         session_description='M2 data',
-        identifier=f'MonkeyN_{start_date}_{split}',
+        identifier=file_id,
         subject=subject,
-        session_start_time=datetime.strptime(start_date, '%Y-%m-%d'),
-        experimenter='Samuel R. Nason and Matthew J. Mender',
+        session_start_time=session_start_time,
+        experimenter='Samuel R. Nason-Tomaszewski and Matthew J. Mender',
         lab='Chestek Lab',
-        institution='University of Michicgan',
-        experiment_description='Two finger group movement in NHP',
-        session_id=hash
+        institution='University of Michigan',
+        experiment_description='Two finger group movement in NHP. Behavior provided in 20ms bins, observation interval at trial ends may include a bit of neural data from partial bin.',
+        session_id=session_hash # determines the fn
     )
-    device = f.create_device(name='Blackrock Utah Array', description='96-channel array')
+    device = f.create_device(name='Blackrock Utah Array', description='2x64-channel array, 96 active')
     main_group = f.create_electrode_group(
         name='M1_array',
-        description='Hand area 96-channel array',
+        description='Hand area 2x64-channel array (96 active channels in recording system)',
         location='M1',
         device=device,
     )
     f.add_trial_column(name="tgt_loc", description="location of target (0-1 AU)")
+    f.add_trial_column(name="trial_num", description="trial number as in experiment")
     for i in range(CHANNEL_EXPECTATION):
         f.add_electrode(
             id=i,
             x=np.nan, y=np.nan, z=np.nan,
             imp=np.nan,
             location='M1',
             group=main_group,
@@ -123,112 +128,155 @@
 def filt_single_trial(trial):
     # reduce raw
     assert len(trial['Channel']) == CHANNEL_EXPECTATION
     return {
         'fingers': trial['FingerAnglesTIMRL'][:, TARGET_FINGERS],
         'spikes': trial['Channel'], # spike time to nearest ms
         'time': trial['ExperimentTime'], # Clock time since start of block. 0 on first step i.e. start of bin.
-        'target': trial['TargetPos'][TARGET_FINGERS]
+        'target': trial['TargetPos'][TARGET_FINGERS],
+        'trial_num': trial['TrialNumber'],
     }
 
 def to_nwb(path: Path, ):
     full_payload = loadmat(str(path), simplify_cells=True)['z']
     # Skip trial 0 - no data, used for block setup
     full_payload = full_payload[1:]
     full_payload = [i for i in full_payload if not i['BlankTrial']] # 1 if screen was off, no trial run
     full_payload = list(map(filt_single_trial, full_payload))
-
     def create_and_write(
         payload, suffix
     ):
-        nwbfile = create_nwb_shell(path, DATA_SPLITS[path.stem], suffix=suffix)
-        all_bhvr = []
-        all_vel = []
+        extra_note = ""
+        if path.stem == 'Z_Joker_2020-10-19_Run-002' and suffix in ['calib', 'full', 'in_day_oracle']:
+            extra_note = " Dropped trial in this file, see trial dataframe." # Cannot edit description after creation.
+        nwbfile = create_nwb_shell(path, DATA_SPLITS[path.stem], suffix=suffix, extra_note=extra_note)
+        cont_bhvr = []
+        # cont_vel = []
         all_spikes = [[] for _ in range(CHANNEL_EXPECTATION)]
-        all_time = []
+        cont_time = []
         start_time = 0
+        # breakpoint()
         for i, trial_data in enumerate(payload):
-            time = trial_data['time'].astype(float) / 1000 # To ms
+            time = (trial_data['time'].astype(float) / 1000) # To ms
             if not start_time:
                 start_time = time[0]
             time -= start_time
             nwbfile.add_trial(
                 start_time=time[0],
                 stop_time=time[-1],
                 tgt_loc=trial_data['target'],
+                trial_num = trial_data['trial_num']
             )
 
-            # Downsample to 20ms
-            time = time[::math.ceil(FS * BIN_SIZE_MS / 1000)] # This effectively rounds up
             bhvr = trial_data['fingers']
-            EDGE_PAD = 160 # reduce edge ringing, in ms
-            y_padded = np.pad(bhvr, ((EDGE_PAD, EDGE_PAD), (0, 0)), mode='edge',)
-            y_padded = smooth(y_padded, 120, 40) # TODO ask Sam what to use instead of this Gaussian
-
-            y_resampled_padded = resample_poly(y_padded, math.ceil(FS / BIN_SIZE_MS), 1000)
-            bhvr = y_resampled_padded[int(EDGE_PAD / BIN_SIZE_MS):int(-EDGE_PAD / BIN_SIZE_MS)]
-            all_bhvr.append(bhvr)
-            all_vel.append(np.gradient(bhvr, axis=0))
-            assert np.isclose(np.diff(time), BIN_SIZE_S).all(), "Expecting timestamps to be about 20ms apart"
-            all_time.append(time)
+            
+            # Per-trial Downsample to 20ms
+            # time = time[::math.ceil(FS * BIN_SIZE_MS / 1000)] # This effectively rounds up
+            # EDGE_PAD = 160 # reduce edge ringing, in ms
+            # y_padded = np.pad(bhvr, ((EDGE_PAD, EDGE_PAD), (0, 0)), mode='edge',)
+            # y_padded = smooth(y_padded, 120, 40) # Sam says Gaussian is fine
+
+            # y_resampled_padded = resample_poly(y_padded, math.ceil(FS / BIN_SIZE_MS), 1000)
+            # bhvr = y_resampled_padded[int(EDGE_PAD / BIN_SIZE_MS):int(-EDGE_PAD / BIN_SIZE_MS)]
+            cont_bhvr.append(bhvr)
+            # all_vel.append(np.gradient(bhvr, axis=0))
+            # assert np.isclose(np.diff(time), BIN_SIZE_S).all(), "Expecting timestamps to be about 20ms apart"
+            cont_time.append(time)
 
             for j, spike in enumerate(trial_data['spikes']):
                 spike_data = spike['SpikeTimes']
                 if isinstance(spike_data, int):
                     spike_data = [spike_data]
                 all_spikes[j].extend(spike_data)
 
         for i, spikes in enumerate(all_spikes):
             nwbfile.add_unit(
                 id=i,
                 spike_times=np.array(spikes) / 1000 - start_time,
                 electrodes=[i],
-                obs_intervals=[[i[0], i[-1] + BIN_SIZE_S] for i in all_time]
+                obs_intervals=[[0., cont_time[-1][-1]]]
+                # obs_intervals=[[i[0], i[-1] + BIN_SIZE_S] for i in all_time]
             )
-            # OK...
         # trial_diffs = [all_time[i+1][0] - all_time[i][-1] for i in range(len(all_time) - 1)]
-        all_time = np.concatenate(all_time, axis=0)
-        diff_check = np.diff(all_time).max()
-        assert (diff_check > 0), "Expecting time to be monotonically increasing across trials."
-        print(f"Max diff b/n consecutive timebins: {diff_check}")
-
+        # trial_diff_raw = [payload[i+1]['time'][0] - payload[i]['time'][-1] for i in range(len(payload) - 1)]
+        # print(f"Max diff b/n consecutive trials: {max(trial_diffs):.4f}")
+        # print(f"Max diff b/n consecutive trials (raw): {max(trial_diff_raw):.4f}")
+        # Note there's one long drop in `20201019`
+        # if max(trial_diff_raw) > 3:
+            # breakpoint()
+        # all_time = np.concatenate(all_time, axis=0)
+        # diff_check = np.diff(all_time).max()
+        # assert (diff_check > 0), "Expecting time to be monotonically increasing across trials."
+        # print(f"Max diff b/n consecutive timebins: {diff_check}")
         
+        # Form continuous behavior and time
+        cat_bhvr = np.concatenate(cont_bhvr, axis=0)
+        cat_time = np.concatenate(cont_time, axis=0).round(3)
+        assert np.diff(cat_time).min() > 0, "Expecting time to be monotonically increasing."
+        interp_time = np.arange(cat_time[0], cat_time[-1], 0.001)
+        cat_mask = np.zeros_like(interp_time, dtype=bool)
+        for interval in cont_time:
+            cat_mask[(interp_time >= interval[0]) & (interp_time <= interval[-1])] = True
+        interp_bhvrs = [np.interp(interp_time, cat_time, y) for y in cat_bhvr.T]
+        interp_bhvr = np.stack(interp_bhvrs, axis=1)
+        # smooth and downsample
+        EDGE_PAD = 160 # reduce edge ringing, in ms
+        downsample_ratio = math.ceil(FS * BIN_SIZE_MS / 1000)
+        def get_reshape(vec: np.ndarray, downsample_ratio: int):
+            if len(vec) % downsample_ratio:
+                vec = vec[:-(len(vec) % downsample_ratio)]
+            vec = vec.reshape(-1, downsample_ratio)
+            return vec
+        downsampled_time = get_reshape(interp_time, downsample_ratio)[:, -1] # Get RHS of bin
+        pad_bhvr = np.pad(interp_bhvr, ((EDGE_PAD, EDGE_PAD), (0, 0)), mode='edge',)
+        smth_bhvr = smooth(pad_bhvr, 120, 40) # Sam says Gaussian is fine
+        resampled_bhvr = resample_poly(smth_bhvr, math.ceil(FS / BIN_SIZE_MS), 1000)
+        downsampled_bhvr = resampled_bhvr[int(EDGE_PAD / BIN_SIZE_MS):int(-EDGE_PAD / BIN_SIZE_MS)]
+        if smth_bhvr.shape[0] % downsample_ratio:
+            downsampled_bhvr = downsampled_bhvr[1:] # Right bias on extra bin from resample
+        downsampled_vel = np.gradient(downsampled_bhvr, axis=0)
+        downsampled_mask = get_reshape(cat_mask, downsample_ratio).mean(axis=1).round().astype(bool)
+        # assert downsampled_mask.all(), "Expecting mask to be all true."
+        if downsampled_bhvr.shape[0] != downsampled_time.shape[0]:
+            breakpoint()
         ts = create_multichannel_timeseries(
             data_name='finger_pos',
             chan_names=KIN_LABELS,
-            data=np.concatenate(all_bhvr, axis=0),
-            timestamps=all_time, # timestamps denote wall-clock sample is drawn - not evenly spaced
+            data=downsampled_bhvr,
+            # data=np.concatenate(downsampled_bhvr, axis=0),
+            timestamps=downsampled_time, # timestamps denote wall-clock sample is drawn - not evenly spaced
             unit='AU'
         )
         nwbfile.add_acquisition(ts)
 
         ts = create_multichannel_timeseries(
             data_name='finger_vel',
             chan_names=KIN_LABELS,
-            data=np.concatenate(all_vel, axis=0),
-            timestamps=all_time,
+            data=downsampled_vel,
+            # data=np.concatenate(downsampled_vel, axis=0),
+            timestamps=downsampled_time,
             unit='AU'
         )
         nwbfile.add_acquisition(ts)
 
         nwbfile.add_acquisition(
             TimeSeries(
                 name='eval_mask',
                 description='Timesteps to keep covariates (for training, eval).',
-                timestamps=all_time,
-                data=np.ones_like(all_time, dtype=bool),
+                timestamps=downsampled_time,
+                data=downsampled_mask,
+                # data=np.ones_like(downsampled_time, dtype=bool),
                 unit='bool'
             )
         )
         date_str = path.stem.split('_')[2].replace('-', '')
         run = DATA_RUN_SET[path.stem]
         new_prefix = f'sub-MonkeyNRun{run}_{date_str}_{DATA_SPLITS[path.stem]}'
         write_to_nwb(nwbfile, out_root / DATA_SPLITS[path.stem] / f"{new_prefix}_{suffix}.nwb")
-        print(f"Written {path.stem}_{suffix}.nwb")
-
+        print(f"Written ", out_root / DATA_SPLITS[path.stem] / f"{new_prefix}_{suffix}.nwb")
     eval_num = int(len(full_payload) * EVAL_RATIO)
     eval_trials = full_payload[-eval_num:]
     create_and_write(eval_trials, 'eval')
     create_and_write(full_payload, 'full')
     in_day_full_trials = full_payload[:-eval_num]
     if DATA_SPLITS[path.stem] == 'held_in':
         create_and_write(in_day_full_trials, 'calib')
```

### Comparing `falcon_challenge-0.2.8/preproc/merge_answers.py` & `falcon_challenge-0.2.9/preproc/merge_answers.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 #%%
 
-# Realizing now that I need to pull together a separate file for all answers.
+# Flow on EvalAI is; worker runs the container, which should output predictions at submission/submission.csv
+# Worker will compare against ground truth specified in the challenge config repo.
+# Answers thus need to be pushed to challenge config repo.
 # Need a minival.pkl, and a test.pkl
 # needs to be a dict of all split targets
 from falcon_challenge.config import FalconTask, FalconConfig
 from falcon_challenge.dataloaders import load_nwb
 from pathlib import Path
 import pickle
 
@@ -19,24 +21,28 @@
         }
     }
 """
 
 def assemble_phase_answer_key(phase='minival', answer_key_dir='./data/answer_key'):
     annotations = {}
     for dataset in ['h1', 'h2', 'm1', 'm2']:
+        print(f'Loading {dataset} {phase}')
         annotations[dataset] = {}
         dataset_path = Path(answer_key_dir) / dataset / phase
         dataset_files = list(dataset_path.rglob(f'*{phase}*.nwb'))
         task = getattr(FalconTask, dataset)
         config = FalconConfig(task)
         for d in dataset_files:
-            print(d.stem)
             neural_data, decoding_targets, trial_change, eval_mask = load_nwb(d, dataset=task)
+            if dataset == 'h2':
+                eval_targets = decoding_targets
+            else:
+                eval_targets = decoding_targets[eval_mask]
             annotations[dataset][config.hash_dataset(d.stem)] = {
-                'data': decoding_targets[eval_mask],
+                'data': eval_targets,
                 'mask': eval_mask
             }
         print(annotations[dataset].keys())
     return annotations
 
 minival_annotations = assemble_phase_answer_key('minival')
 eval_annotations = assemble_phase_answer_key('eval')
```

### Comparing `falcon_challenge-0.2.8/preproc/nwb_create_utils.py` & `falcon_challenge-0.2.9/preproc/nwb_create_utils.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.2.8/preproc/zip_data.py` & `falcon_challenge-0.2.9/preproc/zip_data.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.2.8/setup.py` & `falcon_challenge-0.2.9/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='falcon_challenge',
-    version='0.2.8',
+    version='0.2.9',
 
     url='https://github.com/snel-repo/stability-benchmark',
     author='Joel Ye',
     author_email='joelye9@gmail.com',
 
     packages=find_packages(exclude=['data_demos', 'data']),
     install_requires=[
@@ -16,11 +16,13 @@
         'tqdm',
         'scipy',
         'pandas',
         'seaborn',
         'scikit-learn',
         'pynwb',
         'torch',
+        'edit_distance',
+        'dandi',
     ],
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
-)
+)
```


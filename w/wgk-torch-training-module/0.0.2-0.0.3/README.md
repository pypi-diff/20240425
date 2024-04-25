# Comparing `tmp/wgk-torch-training-module-0.0.2.tar.gz` & `tmp/wgk_torch_training_module-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wgk-torch-training-module-0.0.2.tar", last modified: Sat Apr 13 05:33:49 2024, max compression
+gzip compressed data, was "wgk_torch_training_module-0.0.3.tar", last modified: Thu Apr 25 01:57:42 2024, max compression
```

## Comparing `wgk-torch-training-module-0.0.2.tar` & `wgk_torch_training_module-0.0.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 gook       (501) staff       (20)        0 2024-04-13 05:33:49.905298 wgk-torch-training-module-0.0.2/
--rw-r--r--   0 gook       (501) staff       (20)       26 2024-04-13 04:56:31.000000 wgk-torch-training-module-0.0.2/LICENSE.txt
--rw-r--r--   0 gook       (501) staff       (20)      431 2024-04-13 05:33:49.905229 wgk-torch-training-module-0.0.2/PKG-INFO
--rw-r--r--   0 gook       (501) staff       (20)       38 2024-04-13 05:03:57.000000 wgk-torch-training-module-0.0.2/README.md
--rw-r--r--   0 gook       (501) staff       (20)      118 2024-04-13 05:13:35.000000 wgk-torch-training-module-0.0.2/pyproject.toml
--rw-r--r--   0 gook       (501) staff       (20)      303 2024-04-13 05:33:49.905509 wgk-torch-training-module-0.0.2/setup.cfg
--rw-r--r--   0 gook       (501) staff       (20)      661 2024-04-13 05:33:26.000000 wgk-torch-training-module-0.0.2/setup.py
-drwxr-xr-x   0 gook       (501) staff       (20)        0 2024-04-13 05:33:49.900776 wgk-torch-training-module-0.0.2/src/
-drwxr-xr-x   0 gook       (501) staff       (20)        0 2024-04-13 05:33:49.904000 wgk-torch-training-module-0.0.2/src/TrainModule/
--rw-r--r--   0 gook       (501) staff       (20)     1460 2024-04-13 04:51:39.000000 wgk-torch-training-module-0.0.2/src/TrainModule/Evaluation.py
--rw-r--r--   0 gook       (501) staff       (20)     6467 2024-04-13 04:51:39.000000 wgk-torch-training-module-0.0.2/src/TrainModule/Experiment.py
--rw-r--r--   0 gook       (501) staff       (20)    11181 2024-04-13 04:51:39.000000 wgk-torch-training-module-0.0.2/src/TrainModule/Trainer.py
--rw-r--r--   0 gook       (501) staff       (20)      176 2024-04-13 05:31:10.000000 wgk-torch-training-module-0.0.2/src/TrainModule/__init__.py
--rw-r--r--   0 gook       (501) staff       (20)      916 2024-04-13 04:51:39.000000 wgk-torch-training-module-0.0.2/src/TrainModule/backup.py
--rw-r--r--   0 gook       (501) staff       (20)     5073 2024-04-13 04:51:39.000000 wgk-torch-training-module-0.0.2/src/TrainModule/checkpoint.py
--rw-r--r--   0 gook       (501) staff       (20)     2474 2024-04-13 04:51:39.000000 wgk-torch-training-module-0.0.2/src/TrainModule/progress.py
-drwxr-xr-x   0 gook       (501) staff       (20)        0 2024-04-13 05:33:49.905033 wgk-torch-training-module-0.0.2/src/wgk_torch_training_module.egg-info/
--rw-r--r--   0 gook       (501) staff       (20)      431 2024-04-13 05:33:49.000000 wgk-torch-training-module-0.0.2/src/wgk_torch_training_module.egg-info/PKG-INFO
--rw-r--r--   0 gook       (501) staff       (20)      466 2024-04-13 05:33:49.000000 wgk-torch-training-module-0.0.2/src/wgk_torch_training_module.egg-info/SOURCES.txt
--rw-r--r--   0 gook       (501) staff       (20)        1 2024-04-13 05:33:49.000000 wgk-torch-training-module-0.0.2/src/wgk_torch_training_module.egg-info/dependency_links.txt
--rw-r--r--   0 gook       (501) staff       (20)       12 2024-04-13 05:33:49.000000 wgk-torch-training-module-0.0.2/src/wgk_torch_training_module.egg-info/top_level.txt
+drwxr-xr-x   0 gook       (501) staff       (20)        0 2024-04-25 01:57:42.490431 wgk_torch_training_module-0.0.3/
+-rw-r--r--   0 gook       (501) staff       (20)       26 2024-04-13 04:56:31.000000 wgk_torch_training_module-0.0.3/LICENSE.txt
+-rw-r--r--   0 gook       (501) staff       (20)      431 2024-04-25 01:57:42.490368 wgk_torch_training_module-0.0.3/PKG-INFO
+-rw-r--r--   0 gook       (501) staff       (20)       38 2024-04-13 05:03:57.000000 wgk_torch_training_module-0.0.3/README.md
+-rw-r--r--   0 gook       (501) staff       (20)      118 2024-04-13 05:13:35.000000 wgk_torch_training_module-0.0.3/pyproject.toml
+-rw-r--r--   0 gook       (501) staff       (20)      303 2024-04-25 01:57:42.490628 wgk_torch_training_module-0.0.3/setup.cfg
+-rw-r--r--   0 gook       (501) staff       (20)      661 2024-04-25 01:56:42.000000 wgk_torch_training_module-0.0.3/setup.py
+drwxr-xr-x   0 gook       (501) staff       (20)        0 2024-04-25 01:57:42.486741 wgk_torch_training_module-0.0.3/src/
+drwxr-xr-x   0 gook       (501) staff       (20)        0 2024-04-25 01:57:42.489328 wgk_torch_training_module-0.0.3/src/TrainModule/
+-rw-r--r--   0 gook       (501) staff       (20)     1460 2024-04-13 04:51:39.000000 wgk_torch_training_module-0.0.3/src/TrainModule/Evaluation.py
+-rw-r--r--   0 gook       (501) staff       (20)     6467 2024-04-13 04:51:39.000000 wgk_torch_training_module-0.0.3/src/TrainModule/Experiment.py
+-rw-r--r--   0 gook       (501) staff       (20)    11181 2024-04-25 01:55:54.000000 wgk_torch_training_module-0.0.3/src/TrainModule/Trainer.py
+-rw-r--r--   0 gook       (501) staff       (20)      176 2024-04-13 05:31:10.000000 wgk_torch_training_module-0.0.3/src/TrainModule/__init__.py
+-rw-r--r--   0 gook       (501) staff       (20)      916 2024-04-13 04:51:39.000000 wgk_torch_training_module-0.0.3/src/TrainModule/backup.py
+-rw-r--r--   0 gook       (501) staff       (20)     5073 2024-04-13 04:51:39.000000 wgk_torch_training_module-0.0.3/src/TrainModule/checkpoint.py
+-rw-r--r--   0 gook       (501) staff       (20)     2561 2024-04-25 01:55:40.000000 wgk_torch_training_module-0.0.3/src/TrainModule/progress.py
+drwxr-xr-x   0 gook       (501) staff       (20)        0 2024-04-25 01:57:42.490191 wgk_torch_training_module-0.0.3/src/wgk_torch_training_module.egg-info/
+-rw-r--r--   0 gook       (501) staff       (20)      431 2024-04-25 01:57:42.000000 wgk_torch_training_module-0.0.3/src/wgk_torch_training_module.egg-info/PKG-INFO
+-rw-r--r--   0 gook       (501) staff       (20)      466 2024-04-25 01:57:42.000000 wgk_torch_training_module-0.0.3/src/wgk_torch_training_module.egg-info/SOURCES.txt
+-rw-r--r--   0 gook       (501) staff       (20)        1 2024-04-25 01:57:42.000000 wgk_torch_training_module-0.0.3/src/wgk_torch_training_module.egg-info/dependency_links.txt
+-rw-r--r--   0 gook       (501) staff       (20)       12 2024-04-25 01:57:42.000000 wgk_torch_training_module-0.0.3/src/wgk_torch_training_module.egg-info/top_level.txt
```

### Comparing `wgk-torch-training-module-0.0.2/setup.py` & `wgk_torch_training_module-0.0.3/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="wgk-torch-training-module",
-    version="0.0.2",
+    version="0.0.3",
     author="WonGook",
     author_email="onlyworld94@naver.com",
     description="wgk torch training module",
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
         "Programming Language :: Python :: 3",
```

### Comparing `wgk-torch-training-module-0.0.2/src/TrainModule/Evaluation.py` & `wgk_torch_training_module-0.0.3/src/TrainModule/Evaluation.py`

 * *Files identical despite different names*

### Comparing `wgk-torch-training-module-0.0.2/src/TrainModule/Experiment.py` & `wgk_torch_training_module-0.0.3/src/TrainModule/Experiment.py`

 * *Files identical despite different names*

### Comparing `wgk-torch-training-module-0.0.2/src/TrainModule/Trainer.py` & `wgk_torch_training_module-0.0.3/src/TrainModule/Trainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,15 +101,15 @@
                 if self.step%self.gradient_accumulate_every == 0:
                     self.task.amp_scaler.unscale_(self.task.optimizer)
                     torch.nn.utils.clip_grad_norm_(self.task.parameters(), 5)
                     self.task.amp_scaler.step(self.task.optimizer)
                     self.task.amp_scaler.update()
                     self.task.optimizer.zero_grad()
             self._lr_update(self.task.scheduler)
-            self._progress.on_training_end(output['loss'])
+            self._progress.on_training_end(output['tqdm'])
 
             self.task.training_step_end(self.train_outputs)
             self.log(self.task.logs)
             self.reset_log('epoch')
 
             if dist.get_rank() == 0:
                 if self.step != 0 and self.step % self.save_ckpt == 0:
```

### Comparing `wgk-torch-training-module-0.0.2/src/TrainModule/backup.py` & `wgk_torch_training_module-0.0.3/src/TrainModule/backup.py`

 * *Files identical despite different names*

### Comparing `wgk-torch-training-module-0.0.2/src/TrainModule/checkpoint.py` & `wgk_torch_training_module-0.0.3/src/TrainModule/checkpoint.py`

 * *Files identical despite different names*

### Comparing `wgk-torch-training-module-0.0.2/src/TrainModule/progress.py` & `wgk_torch_training_module-0.0.3/src/TrainModule/progress.py`

 * *Files 18% similar despite different names*

```diff
@@ -37,21 +37,23 @@
         #                  )
 
     def on_training_start(self):
         self.cur_step += 1
         self.Training_bar.display()
 
     def on_training_end(self, output):
-        if type(output) in [list, tuple]:
-            self.loss = [round(op.detach().item(), 4) for op in output]
-        else:
-            self.loss = output.detach().item()
+        for k in output.keys():
+            output[k] = round(output[k].detach().item(), 4)
+        # if type(output) in [list, tuple]:
+        #     self.loss = [round(op.detach().item(), 4) for op in output]
+        # else:
+        #     self.loss = output.detach().item()
         self.Training_bar.update(1)
         self.Training_bar.set_description('Training step {}'.format(self.cur_step))
-        self.Training_bar.set_postfix({'loss': self.loss})
+        self.Training_bar.set_postfix(output)
 
     def on_train_batch_end(self, output):
         self.loss = output.detach().item()
 
 
 
     def on_validation_start(self):
```


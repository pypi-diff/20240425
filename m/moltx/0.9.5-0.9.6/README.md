# Comparing `tmp/moltx-0.9.5.tar.gz` & `tmp/moltx-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moltx-0.9.5.tar", last modified: Thu Apr 25 08:22:17 2024, max compression
+gzip compressed data, was "moltx-0.9.6.tar", last modified: Thu Apr 25 08:47:59 2024, max compression
```

## Comparing `moltx-0.9.5.tar` & `moltx-0.9.6.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:22:17.423490 moltx-0.9.5/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-25 08:22:10.000000 moltx-0.9.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5704 2024-04-25 08:22:17.423490 moltx-0.9.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5093 2024-04-25 08:22:10.000000 moltx-0.9.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:22:17.419490 moltx-0.9.5/moltx/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 08:22:10.000000 moltx-0.9.5/moltx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-25 08:22:10.000000 moltx-0.9.5/moltx/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:22:17.419490 moltx-0.9.5/moltx/data/
--rw-r--r--   0 runner    (1001) docker     (127)    11088 2024-04-25 08:22:10.000000 moltx-0.9.5/moltx/data/spe_safe.txt
--rw-r--r--   0 runner    (1001) docker     (127)    27879 2024-04-25 08:22:10.000000 moltx-0.9.5/moltx/data/spe_smiles.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5372 2024-04-25 08:22:10.000000 moltx-0.9.5/moltx/data/tks_safe.json
--rw-r--r--   0 runner    (1001) docker     (127)    36304 2024-04-25 08:22:10.000000 moltx-0.9.5/moltx/data/tks_smiles.json
--rw-r--r--   0 runner    (1001) docker     (127)     3377 2024-04-25 08:22:10.000000 moltx-0.9.5/moltx/datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-04-25 08:22:10.000000 moltx-0.9.5/moltx/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     4506 2024-04-25 08:22:10.000000 moltx-0.9.5/moltx/nets.py
--rw-r--r--   0 runner    (1001) docker     (127)     7442 2024-04-25 08:22:10.000000 moltx-0.9.5/moltx/pipelines.py
--rw-r--r--   0 runner    (1001) docker     (127)     8000 2024-04-25 08:22:10.000000 moltx-0.9.5/moltx/tokenizers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:22:17.423490 moltx-0.9.5/moltx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5704 2024-04-25 08:22:17.000000 moltx-0.9.5/moltx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-04-25 08:22:17.000000 moltx-0.9.5/moltx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 08:22:17.000000 moltx-0.9.5/moltx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-25 08:22:17.000000 moltx-0.9.5/moltx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-25 08:22:17.000000 moltx-0.9.5/moltx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-25 08:22:10.000000 moltx-0.9.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-04-25 08:22:17.423490 moltx-0.9.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 08:22:10.000000 moltx-0.9.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:22:17.423490 moltx-0.9.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-04-25 08:22:10.000000 moltx-0.9.5/tests/test_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     3113 2024-04-25 08:22:10.000000 moltx-0.9.5/tests/test_nets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-04-25 08:22:10.000000 moltx-0.9.5/tests/test_pipelines.py
--rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-04-25 08:22:10.000000 moltx-0.9.5/tests/test_tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:47:59.628718 moltx-0.9.6/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-25 08:47:53.000000 moltx-0.9.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5704 2024-04-25 08:47:59.628718 moltx-0.9.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5093 2024-04-25 08:47:53.000000 moltx-0.9.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:47:59.624717 moltx-0.9.6/moltx/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 08:47:53.000000 moltx-0.9.6/moltx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-25 08:47:53.000000 moltx-0.9.6/moltx/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:47:59.624717 moltx-0.9.6/moltx/data/
+-rw-r--r--   0 runner    (1001) docker     (127)    11088 2024-04-25 08:47:53.000000 moltx-0.9.6/moltx/data/spe_safe.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    27879 2024-04-25 08:47:53.000000 moltx-0.9.6/moltx/data/spe_smiles.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5372 2024-04-25 08:47:53.000000 moltx-0.9.6/moltx/data/tks_safe.json
+-rw-r--r--   0 runner    (1001) docker     (127)    36304 2024-04-25 08:47:53.000000 moltx-0.9.6/moltx/data/tks_smiles.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3377 2024-04-25 08:47:53.000000 moltx-0.9.6/moltx/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-04-25 08:47:53.000000 moltx-0.9.6/moltx/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4506 2024-04-25 08:47:53.000000 moltx-0.9.6/moltx/nets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7447 2024-04-25 08:47:53.000000 moltx-0.9.6/moltx/pipelines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8000 2024-04-25 08:47:53.000000 moltx-0.9.6/moltx/tokenizers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:47:59.628718 moltx-0.9.6/moltx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5704 2024-04-25 08:47:59.000000 moltx-0.9.6/moltx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-04-25 08:47:59.000000 moltx-0.9.6/moltx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 08:47:59.000000 moltx-0.9.6/moltx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-25 08:47:59.000000 moltx-0.9.6/moltx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-25 08:47:59.000000 moltx-0.9.6/moltx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-25 08:47:53.000000 moltx-0.9.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-04-25 08:47:59.628718 moltx-0.9.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 08:47:53.000000 moltx-0.9.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:47:59.628718 moltx-0.9.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-04-25 08:47:53.000000 moltx-0.9.6/tests/test_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3113 2024-04-25 08:47:53.000000 moltx-0.9.6/tests/test_nets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-04-25 08:47:53.000000 moltx-0.9.6/tests/test_pipelines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-04-25 08:47:53.000000 moltx-0.9.6/tests/test_tokenizer.py
```

### Comparing `moltx-0.9.5/LICENSE` & `moltx-0.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `moltx-0.9.5/PKG-INFO` & `moltx-0.9.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moltx
-Version: 0.9.5
+Version: 0.9.6
 Summary: Molcule Transformer X Model
 Author: Michael Ding
 Author-email: yandy.ding@gmail.com
 License: Apache-2.0
 Keywords: molcule,AI,deep learning,transformer
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
```

### Comparing `moltx-0.9.5/README.md` & `moltx-0.9.6/README.md`

 * *Files identical despite different names*

### Comparing `moltx-0.9.5/moltx/data/spe_safe.txt` & `moltx-0.9.6/moltx/data/spe_safe.txt`

 * *Files identical despite different names*

### Comparing `moltx-0.9.5/moltx/data/spe_smiles.txt` & `moltx-0.9.6/moltx/data/spe_smiles.txt`

 * *Files identical despite different names*

### Comparing `moltx-0.9.5/moltx/data/tks_safe.json` & `moltx-0.9.6/moltx/data/tks_safe.json`

 * *Files identical despite different names*

### Comparing `moltx-0.9.5/moltx/data/tks_smiles.json` & `moltx-0.9.6/moltx/data/tks_smiles.json`

 * *Files identical despite different names*

### Comparing `moltx-0.9.5/moltx/datasets.py` & `moltx-0.9.6/moltx/datasets.py`

 * *Files identical despite different names*

### Comparing `moltx-0.9.5/moltx/models.py` & `moltx-0.9.6/moltx/models.py`

 * *Files identical despite different names*

### Comparing `moltx-0.9.5/moltx/nets.py` & `moltx-0.9.6/moltx/nets.py`

 * *Files identical despite different names*

### Comparing `moltx-0.9.5/moltx/pipelines.py` & `moltx-0.9.6/moltx/pipelines.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,17 +84,17 @@
             if meet_end.all():
                 break
         probs = log_probs.squeeze().exp().tolist()
         smiles = []
         for line in tgt:
             idx = (line == eos).nonzero(as_tuple=True)[0]
             if idx.numel() > 0:
-                smiles.append(self.tokenizer.decode(line[:idx[0]].tolist()))
+                smiles.append(self.tokenizer.decode(line[1:idx[0]].tolist()))
             else:
-                smiles.append(self.tokenizer.decode(line.tolist()))
+                smiles.append(self.tokenizer.decode(line[1:].tolist()))
         return smiles, probs
 
 
 class AdaMR(Base):
 
     def _model_args(self, s1: str, s2: typing.Optional[str] = None) -> typing.Tuple[torch.Tensor]:
         src = self._tokenize(s1)
```

### Comparing `moltx-0.9.5/moltx/tokenizers.py` & `moltx-0.9.6/moltx/tokenizers.py`

 * *Files identical despite different names*

### Comparing `moltx-0.9.5/moltx.egg-info/PKG-INFO` & `moltx-0.9.6/moltx.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moltx
-Version: 0.9.5
+Version: 0.9.6
 Summary: Molcule Transformer X Model
 Author: Michael Ding
 Author-email: yandy.ding@gmail.com
 License: Apache-2.0
 Keywords: molcule,AI,deep learning,transformer
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
```

### Comparing `moltx-0.9.5/moltx.egg-info/SOURCES.txt` & `moltx-0.9.6/moltx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `moltx-0.9.5/setup.cfg` & `moltx-0.9.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `moltx-0.9.5/tests/test_datasets.py` & `moltx-0.9.6/tests/test_datasets.py`

 * *Files identical despite different names*

### Comparing `moltx-0.9.5/tests/test_nets.py` & `moltx-0.9.6/tests/test_nets.py`

 * *Files identical despite different names*

### Comparing `moltx-0.9.5/tests/test_pipelines.py` & `moltx-0.9.6/tests/test_pipelines.py`

 * *Files identical despite different names*

### Comparing `moltx-0.9.5/tests/test_tokenizer.py` & `moltx-0.9.6/tests/test_tokenizer.py`

 * *Files identical despite different names*


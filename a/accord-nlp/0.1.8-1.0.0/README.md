# Comparing `tmp/accord_nlp-0.1.8.tar.gz` & `tmp/accord_nlp-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "accord_nlp-0.1.8.tar", last modified: Thu Aug 31 07:14:01 2023, max compression
+gzip compressed data, was "accord_nlp-1.0.0.tar", last modified: Thu Apr 25 19:47:33 2024, max compression
```

## Comparing `accord_nlp-0.1.8.tar` & `accord_nlp-1.0.0.tar`

### file list

```diff
@@ -1,37 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-31 07:14:01.920873 accord_nlp-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (999)    11357 2023-08-31 07:13:51.000000 accord_nlp-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (999)      610 2023-08-31 07:14:01.920873 accord_nlp-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)       15 2023-08-31 07:13:51.000000 accord_nlp-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-31 07:14:01.920873 accord_nlp-0.1.8/accord_nlp/
--rw-r--r--   0 runner    (1001) docker     (999)      116 2023-08-31 07:13:51.000000 accord_nlp-0.1.8/accord_nlp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-31 07:14:01.920873 accord_nlp-0.1.8/accord_nlp/information_extraction/
--rw-r--r--   0 runner    (1001) docker     (999)        2 2023-08-31 07:13:51.000000 accord_nlp-0.1.8/accord_nlp/information_extraction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     7539 2023-08-31 07:13:51.000000 accord_nlp-0.1.8/accord_nlp/information_extraction/convertor.py
--rw-r--r--   0 runner    (1001) docker     (999)     2756 2023-08-31 07:13:51.000000 accord_nlp-0.1.8/accord_nlp/information_extraction/ie_pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-31 07:14:01.920873 accord_nlp-0.1.8/accord_nlp/text_classification/
--rw-r--r--   0 runner    (1001) docker     (999)        2 2023-08-31 07:13:51.000000 accord_nlp-0.1.8/accord_nlp/text_classification/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-31 07:14:01.920873 accord_nlp-0.1.8/accord_nlp/text_classification/config/
--rw-r--r--   0 runner    (1001) docker     (999)        2 2023-08-31 07:13:51.000000 accord_nlp-0.1.8/accord_nlp/text_classification/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     5718 2023-08-31 07:13:51.000000 accord_nlp-0.1.8/accord_nlp/text_classification/config/model_args.py
--rw-r--r--   0 runner    (1001) docker     (999)      347 2023-08-31 07:13:51.000000 accord_nlp-0.1.8/accord_nlp/text_classification/config/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-31 07:14:01.920873 accord_nlp-0.1.8/accord_nlp/text_classification/ner/
--rw-r--r--   0 runner    (1001) docker     (999)        2 2023-08-31 07:13:51.000000 accord_nlp-0.1.8/accord_nlp/text_classification/ner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)    61904 2023-08-31 07:13:51.000000 accord_nlp-0.1.8/accord_nlp/text_classification/ner/ner_model.py
--rw-r--r--   0 runner    (1001) docker     (999)    16501 2023-08-31 07:13:51.000000 accord_nlp-0.1.8/accord_nlp/text_classification/ner/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-31 07:14:01.920873 accord_nlp-0.1.8/accord_nlp/text_classification/relation_extraction/
--rw-r--r--   0 runner    (1001) docker     (999)        2 2023-08-31 07:13:51.000000 accord_nlp-0.1.8/accord_nlp/text_classification/relation_extraction/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-31 07:14:01.920873 accord_nlp-0.1.8/accord_nlp/text_classification/relation_extraction/models/
--rw-r--r--   0 runner    (1001) docker     (999)        2 2023-08-31 07:13:51.000000 accord_nlp-0.1.8/accord_nlp/text_classification/relation_extraction/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     4777 2023-08-31 07:13:51.000000 accord_nlp-0.1.8/accord_nlp/text_classification/relation_extraction/models/albert_model.py
--rw-r--r--   0 runner    (1001) docker     (999)     4721 2023-08-31 07:13:51.000000 accord_nlp-0.1.8/accord_nlp/text_classification/relation_extraction/models/bert_model.py
--rw-r--r--   0 runner    (1001) docker     (999)     5629 2023-08-31 07:13:51.000000 accord_nlp-0.1.8/accord_nlp/text_classification/relation_extraction/models/roberta_model.py
--rw-r--r--   0 runner    (1001) docker     (999)    74565 2023-08-31 07:13:51.000000 accord_nlp-0.1.8/accord_nlp/text_classification/relation_extraction/re_model.py
--rw-r--r--   0 runner    (1001) docker     (999)    28346 2023-08-31 07:13:51.000000 accord_nlp-0.1.8/accord_nlp/text_classification/relation_extraction/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-31 07:14:01.920873 accord_nlp-0.1.8/accord_nlp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (999)      610 2023-08-31 07:14:01.000000 accord_nlp-0.1.8/accord_nlp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)     1178 2023-08-31 07:14:01.000000 accord_nlp-0.1.8/accord_nlp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (999)        1 2023-08-31 07:14:01.000000 accord_nlp-0.1.8/accord_nlp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (999)      121 2023-08-31 07:14:01.000000 accord_nlp-0.1.8/accord_nlp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (999)       11 2023-08-31 07:14:01.000000 accord_nlp-0.1.8/accord_nlp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (999)      102 2023-08-31 07:14:01.920873 accord_nlp-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (999)     1164 2023-08-31 07:13:51.000000 accord_nlp-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:47:33.751783 accord_nlp-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-25 19:47:25.000000 accord_nlp-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8723 2024-04-25 19:47:33.751783 accord_nlp-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7768 2024-04-25 19:47:25.000000 accord_nlp-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:47:33.743783 accord_nlp-1.0.0/accord_nlp/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-25 19:47:25.000000 accord_nlp-1.0.0/accord_nlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3269 2024-04-25 19:47:25.000000 accord_nlp-1.0.0/accord_nlp/data_augmentation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:47:33.747783 accord_nlp-1.0.0/accord_nlp/information_extraction/
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-04-25 19:47:25.000000 accord_nlp-1.0.0/accord_nlp/information_extraction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7539 2024-04-25 19:47:25.000000 accord_nlp-1.0.0/accord_nlp/information_extraction/convertor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3141 2024-04-25 19:47:25.000000 accord_nlp-1.0.0/accord_nlp/information_extraction/ie_pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:47:33.747783 accord_nlp-1.0.0/accord_nlp/text_classification/
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-04-25 19:47:25.000000 accord_nlp-1.0.0/accord_nlp/text_classification/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:47:33.747783 accord_nlp-1.0.0/accord_nlp/text_classification/config/
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-04-25 19:47:25.000000 accord_nlp-1.0.0/accord_nlp/text_classification/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6285 2024-04-25 19:47:25.000000 accord_nlp-1.0.0/accord_nlp/text_classification/config/model_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-04-25 19:47:25.000000 accord_nlp-1.0.0/accord_nlp/text_classification/config/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:47:33.747783 accord_nlp-1.0.0/accord_nlp/text_classification/language_modelling/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-25 19:47:25.000000 accord_nlp-1.0.0/accord_nlp/text_classification/language_modelling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28179 2024-04-25 19:47:25.000000 accord_nlp-1.0.0/accord_nlp/text_classification/language_modelling/custom_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    69606 2024-04-25 19:47:25.000000 accord_nlp-1.0.0/accord_nlp/text_classification/language_modelling/lm_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7576 2024-04-25 19:47:25.000000 accord_nlp-1.0.0/accord_nlp/text_classification/language_modelling/lm_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:47:33.747783 accord_nlp-1.0.0/accord_nlp/text_classification/ner/
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-04-25 19:47:25.000000 accord_nlp-1.0.0/accord_nlp/text_classification/ner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62413 2024-04-25 19:47:25.000000 accord_nlp-1.0.0/accord_nlp/text_classification/ner/ner_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16501 2024-04-25 19:47:25.000000 accord_nlp-1.0.0/accord_nlp/text_classification/ner/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:47:33.747783 accord_nlp-1.0.0/accord_nlp/text_classification/relation_extraction/
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-04-25 19:47:25.000000 accord_nlp-1.0.0/accord_nlp/text_classification/relation_extraction/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:47:33.751783 accord_nlp-1.0.0/accord_nlp/text_classification/relation_extraction/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-04-25 19:47:25.000000 accord_nlp-1.0.0/accord_nlp/text_classification/relation_extraction/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4777 2024-04-25 19:47:25.000000 accord_nlp-1.0.0/accord_nlp/text_classification/relation_extraction/models/albert_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4721 2024-04-25 19:47:25.000000 accord_nlp-1.0.0/accord_nlp/text_classification/relation_extraction/models/bert_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5629 2024-04-25 19:47:25.000000 accord_nlp-1.0.0/accord_nlp/text_classification/relation_extraction/models/roberta_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    74586 2024-04-25 19:47:25.000000 accord_nlp-1.0.0/accord_nlp/text_classification/relation_extraction/re_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28346 2024-04-25 19:47:25.000000 accord_nlp-1.0.0/accord_nlp/text_classification/relation_extraction/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:47:33.751783 accord_nlp-1.0.0/accord_nlp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8723 2024-04-25 19:47:33.000000 accord_nlp-1.0.0/accord_nlp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-04-25 19:47:33.000000 accord_nlp-1.0.0/accord_nlp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 19:47:33.000000 accord_nlp-1.0.0/accord_nlp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-25 19:47:33.000000 accord_nlp-1.0.0/accord_nlp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-25 19:47:33.000000 accord_nlp-1.0.0/accord_nlp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-25 19:47:33.751783 accord_nlp-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-04-25 19:47:25.000000 accord_nlp-1.0.0/setup.py
```

### Comparing `accord_nlp-0.1.8/LICENSE` & `accord_nlp-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `accord_nlp-0.1.8/accord_nlp/information_extraction/convertor.py` & `accord_nlp-1.0.0/accord_nlp/information_extraction/convertor.py`

 * *Files identical despite different names*

### Comparing `accord_nlp-0.1.8/accord_nlp/information_extraction/ie_pipeline.py` & `accord_nlp-1.0.0/accord_nlp/information_extraction/ie_pipeline.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,50 +1,56 @@
 # Created by Hansi at 28/08/2023
-
 # import nltk
 # nltk.download('punkt')
 # nltk.download('averaged_perceptron_tagger')
+import logging
 
 import torch
 from nltk import word_tokenize
 
 from accord_nlp.information_extraction.convertor import entity_pairing, graph_building
 from accord_nlp.text_classification.ner.ner_model import NERModel
 from accord_nlp.text_classification.relation_extraction.re_model import REModel
 
-SEED = 157
-
-ner_args = {
-    "labels_list": ["O", "B-quality", "B-property", "I-property", "I-quality", "B-object", "I-object", "B-value", "I-value"],
-}
-
-re_args = {
-    "labels_list": ["selection", "necessity", "none", "greater", "part-of", "equal", "greater-equal", "less-equal", "not-part-of", "less"],
-    "special_tags": ["<e1>", "<e2>"],  # Should be either begin_tag or end_tag
-}
+logger = logging.getLogger(__name__)
 
 
 class InformationExtractor:
     def __init__(
             self,
-            ner_model_info=('roberta', 'ACCORD-NLP/ner-roberta-large', ner_args),
-            re_model_info=('roberta', 'ACCORD-NLP/re-roberta-large', re_args),
-            cuda_device=0):
+            ner_model_info=('roberta', 'ACCORD-NLP/ner-roberta-large'),
+            re_model_info=('roberta', 'ACCORD-NLP/re-roberta-large'),
+            cuda_device=0,
+            debug=False):
 
-        self.ner_model = NERModel(ner_model_info[0], ner_model_info[1], labels=ner_model_info[2]['labels_list'],
-                                  use_cuda=torch.cuda.is_available(), cuda_device=cuda_device, args=ner_model_info[2])
+        """
+        Initialise an information extraction pipeline
+
+        :param ner_model_info: tuple
+            (<model_type>, <model_name>) OR (<model_type>, <model_name>, <args as a dictionary>)
+        :param re_model_info: tuple
+            (<model_type>, <model_name>) OR (<model_type>, <model_name>, <args as a dictionary>)
+        :param cuda_device: int (optional)
+        :param debug: boolean (optional)
+            If debug=True, intermediate outputs will be logged
+        """
+
+        self.debug = debug
+        if self.debug:
+            logging.basicConfig(level=logging.INFO)
+
+        self.ner_model = NERModel(ner_model_info[0], ner_model_info[1], use_cuda=torch.cuda.is_available(),
+                                  cuda_device=cuda_device, args=ner_model_info[2] if len(ner_model_info) > 2 else None)
 
         self.re_model = REModel(re_model_info[0], re_model_info[1], use_cuda=torch.cuda.is_available(),
-                                cuda_device=cuda_device, args=re_model_info[2])
+                                cuda_device=cuda_device, args=re_model_info[2] if len(re_model_info) > 2 else None)
 
     def preprocess(self, sentence):
-        # remove white spaces at the beginning and end of the text
-        sentence = sentence.strip()
-        # tokenise
-        sentence = ' '.join(word_tokenize(sentence))
+        sentence = sentence.strip()  # remove white spaces at the beginning and end of the text
+        sentence = ' '.join(word_tokenize(sentence))  # tokenise the sentence
         return sentence
 
     def sentence_to_graph(self, sentence):
         """
         Generate a graph based on the information contained in a sentence
             graph nodes - entities
             graph edges - relations between entities
@@ -53,25 +59,25 @@
         :return: graphviz graph
         """
         # preprocess
         sentence = self.preprocess(sentence)
 
         # NER
         ner_predictions, ner_raw_outputs = self.ner_model.predict([sentence])
+        if self.debug:
+            logger.info(f'Entity predictions: {ner_predictions}')
 
         # pair entities to predict their relations
         entity_pair_df = entity_pairing(sentence, ner_predictions[0])
 
         # relation extraction
         re_predictions, re_raw_outputs = self.re_model.predict(entity_pair_df['output'].tolist())
         entity_pair_df['prediction'] = re_predictions
+        if self.debug:
+            logger.info('Relation predictions:')
+            for pred, sample in zip(re_predictions, entity_pair_df['output']):
+                logger.info(f'{sample}: {pred}')
 
         # build graph
-        graph = graph_building(entity_pair_df, view=False)
+        graph = graph_building(entity_pair_df, view=True)
 
         return graph
-
-
-# if __name__ == '__main__':
-#     sentence = 'Perimeter insulation should be continuous and have a minimum thickness of 25mm.'
-#     ie = InformationExtractor()
-#     ie.sentence_to_graph(sentence)
```

### Comparing `accord_nlp-0.1.8/accord_nlp/text_classification/config/model_args.py` & `accord_nlp-1.0.0/accord_nlp/text_classification/config/model_args.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # Created by Hansi at 28/06/2023
 
 import json
 import os
 import sys
-from dataclasses import asdict, dataclass, field, fields
+from dataclasses import asdict, dataclass, field
 from multiprocessing import cpu_count
-import warnings
 
 from torch.utils.data import Dataset
 
 
 def get_default_process_count():
     process_count = cpu_count() - 2 if cpu_count() > 2 else 1
     if sys.platform == "win32":
@@ -152,36 +151,39 @@
     tie_generator_and_discriminator_embeddings: bool = True
     tokenizer_name: str = None
     vocab_size: int = None
     clean_text: bool = True
     handle_chinese_chars: bool = True
     strip_accents: bool = True
     local_rank: int = -1
+    use_hf_datasets: bool = False
+    optimizer: str = "AdamW"
+    adam_betas: tuple = field(default_factory=lambda: (0.9, 0.999))
+    scheduler: str = "linear_schedule_with_warmup"
+
 
 @dataclass
 class REArgs(ModelArgs):
     """
     Model args for a RE_Model
     """
 
     model_class: str = "REModel"
-    labels_list: list = field(default_factory=list)
+    # added to support huggingface models, and needs to be changed if a different labels list is used
+    labels_list: list = field(
+        default_factory=lambda: ["selection", "necessity", "none", "greater", "part-of", "equal", "greater-equal",
+                                 "less-equal", "not-part-of", "less"])
     labels_map: dict = field(default_factory=dict)
     lazy_delimiter: str = "\t"
     lazy_labels_column: int = 1
     lazy_loading: bool = False
     lazy_loading_start_line: int = 1
     lazy_text_a_column: bool = None
     lazy_text_b_column: bool = None
     lazy_text_column: int = 0
     onnx: bool = False
     regression: bool = False
     sliding_window: bool = False
     stride: float = 0.8
     tie_value: int = 1
-    special_tags: list = None
-
-
-
-
-
-
+    # added to support huggingface models, and needs to be changed if a different special tags are used
+    special_tags: list = field(default_factory=lambda: ["<e1>", "<e2>"])
```

### Comparing `accord_nlp-0.1.8/accord_nlp/text_classification/ner/ner_model.py` & `accord_nlp-1.0.0/accord_nlp/text_classification/ner/ner_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 # adapted from - https://github.com/TharinduDR/MUDES
 from __future__ import absolute_import, division, print_function
 
 import glob
 import logging
 import math
+import numbers
 import os
 import random
 import shutil
 import warnings
 from dataclasses import asdict
 import tempfile
 from pathlib import Path
@@ -78,26 +79,26 @@
 class NERModel:
     def __init__(
             self,
             model_type,
             model_name,
             labels=None,
             args=None,
-            use_cuda=True,
+            use_cuda=torch.cuda.is_available(),
             cuda_device=-1,
             onnx_execution_provider=None,
             **kwargs,
     ):
         """
         Initializes a NERModel
 
         Args:
             model_type: The type of model (bert, roberta)
             model_name: Default Transformer model name or path to a directory containing Transformer model file (pytorch_model.bin).
-            labels (optional): A list of all Named Entity labels.  If not given, ["O", "B-MISC", "I-MISC",  "B-PER", "I-PER", "B-ORG", "I-ORG", "B-LOC", "I-LOC"] will be used.
+            labels (optional): A list of all Named Entity labels.  If not given, ["O", "B-quality", "B-property", "I-property", "I-quality", "B-object", "I-object", "B-value", "I-value"] will be used.
             args (optional): Default args will be used if this parameter is not provided. If provided, it should be a dict containing the args that should be changed in the default args.
             use_cuda (optional): Use GPU if available. Setting to False will force model to use CPU only.
             cuda_device (optional): Specific GPU that should be used. Will use the first available GPU by default.
             **kwargs (optional): For providing proxies, force_download, resume_download, cache_dir and other options specific to the 'from_pretrained' implementation where this will be supplied.
         """  # noqa: ignore flake8"
 
         MODEL_CLASSES = {
@@ -144,25 +145,23 @@
         #     self.args.labels_list = labels
 
         if labels is not None:
             self.args.labels_list = labels
         elif self.args.labels_list:
             pass
         else:
-            self.args.labels_list = [
-                "O",
-                "B-MISC",
-                "I-MISC",
-                "B-PER",
-                "I-PER",
-                "B-ORG",
-                "I-ORG",
-                "B-LOC",
-                "I-LOC",
-            ]
+            self.args.labels_list = ["O",
+                                     "B-quality",
+                                     "B-property",
+                                     "I-property",
+                                     "I-quality",
+                                     "B-object",
+                                     "I-object",
+                                     "B-value",
+                                     "I-value"]
         self.num_labels = len(self.args.labels_list)
 
         config_class, model_class, tokenizer_class = MODEL_CLASSES[model_type]
         if self.num_labels:
             self.config = config_class.from_pretrained(model_name, num_labels=self.num_labels, **self.args.config)
             self.num_labels = self.num_labels
         else:
@@ -553,23 +552,25 @@
                             eval_data,
                             verbose=verbose and args.evaluate_during_training_verbose,
                             wandb_log=False,
                             output_dir=output_dir_current,
                             **kwargs,
                         )
                         for key, value in results.items():
-                            tb_writer.add_scalar("eval_{}".format(key), value, global_step)
+                            if isinstance(value, numbers.Number):
+                                tb_writer.add_scalar("eval_{}".format(key), value, global_step)
 
                         if args.save_eval_checkpoints:
                             self.save_model(output_dir_current, optimizer, scheduler, model=model, results=results)
 
                         training_progress_scores["global_step"].append(global_step)
                         training_progress_scores["train_loss"].append(current_loss)
                         for key in results:
-                            training_progress_scores[key].append(results[key])
+                            if isinstance(results[key], numbers.Number):
+                                training_progress_scores[key].append(results[key])
                         report = pd.DataFrame(training_progress_scores)
                         report.to_csv(
                             os.path.join(args.output_dir, "training_progress_scores.csv"), index=False,
                         )
 
                         if args.wandb_project or self.is_sweeping:
                             wandb.log(self._get_last_metrics(training_progress_scores))
@@ -657,15 +658,16 @@
                 )
 
                 self.save_model(output_dir_current, optimizer, scheduler, results=results)
 
                 training_progress_scores["global_step"].append(global_step)
                 training_progress_scores["train_loss"].append(current_loss)
                 for key in results:
-                    training_progress_scores[key].append(results[key])
+                    if isinstance(results[key], numbers.Number):
+                        training_progress_scores[key].append(results[key])
                 report = pd.DataFrame(training_progress_scores)
                 report.to_csv(os.path.join(args.output_dir, "training_progress_scores.csv"), index=False)
 
                 if args.wandb_project or self.is_sweeping:
                     wandb.log(self._get_last_metrics(training_progress_scores))
 
                 if not best_eval_metric:
@@ -870,30 +872,31 @@
             "recall": recall_score(out_label_list, preds_list, average="macro"),
             "f1_score": f1_score(out_label_list, preds_list, average="macro"),
             "precision_strict": precision_score(out_label_list, preds_list, average="macro", mode="strict", scheme=IOB2),
             "recall_strict": recall_score(out_label_list, preds_list, average="macro", mode="strict",
                                                 scheme=IOB2),
             "f1_score_strict": f1_score(out_label_list, preds_list, average="macro", mode="strict",
                                                 scheme=IOB2),
+
             **extra_metrics,
         }
 
         results.update(result)
 
         os.makedirs(eval_output_dir, exist_ok=True)
         output_eval_file = os.path.join(eval_output_dir, "eval_results.txt")
         with open(output_eval_file, "w") as writer:
             # if args.classification_report:
-            writer.write("Default classification report:\n")
-            cls_report = classification_report(out_label_list, preds_list)
-            writer.write("{}\n".format(cls_report))
-
-            writer.write("Strict classification report:\n")
-            cls_report_strict = classification_report(out_label_list, preds_list, mode="strict", scheme=IOB2)
-            writer.write("{}\n".format(cls_report_strict))
+            # writer.write("Default classification report:\n")
+            # cls_report = classification_report(out_label_list, preds_list, digits=4)
+            # writer.write("{}\n".format(cls_report))
+            #
+            # writer.write("Strict classification report:\n")
+            # cls_report_strict = classification_report(out_label_list, preds_list, mode="strict", scheme=IOB2, digits=4)
+            # writer.write("{}\n".format(cls_report_strict))
 
             for key in sorted(result.keys()):
                 writer.write("{} = {}\n".format(key, str(result[key])))
 
         if self.args.wandb_project and wandb_log:
             wandb.init(project=args.wandb_project, config={**asdict(args)}, **args.wandb_kwargs)
 
@@ -1283,15 +1286,15 @@
 
         if self.args.model_type == "layoutlm":
             inputs["bbox"] = batch[4]
 
         return inputs
 
     def _create_training_progress_scores(self, **kwargs):
-        extra_metrics = {key: [] for key in kwargs}
+        extra_metrics = {key: [] for key in kwargs if 'report' not in key}
         training_progress_scores = {
             "global_step": [],
             "precision": [],
             "recall": [],
             "f1_score": [],
             "train_loss": [],
             "eval_loss": [],
```

### Comparing `accord_nlp-0.1.8/accord_nlp/text_classification/ner/utils.py` & `accord_nlp-1.0.0/accord_nlp/text_classification/ner/utils.py`

 * *Files identical despite different names*

### Comparing `accord_nlp-0.1.8/accord_nlp/text_classification/relation_extraction/models/albert_model.py` & `accord_nlp-1.0.0/accord_nlp/text_classification/relation_extraction/models/albert_model.py`

 * *Files identical despite different names*

### Comparing `accord_nlp-0.1.8/accord_nlp/text_classification/relation_extraction/models/bert_model.py` & `accord_nlp-1.0.0/accord_nlp/text_classification/relation_extraction/models/bert_model.py`

 * *Files identical despite different names*

### Comparing `accord_nlp-0.1.8/accord_nlp/text_classification/relation_extraction/models/roberta_model.py` & `accord_nlp-1.0.0/accord_nlp/text_classification/relation_extraction/models/roberta_model.py`

 * *Files identical despite different names*

### Comparing `accord_nlp-0.1.8/accord_nlp/text_classification/relation_extraction/re_model.py` & `accord_nlp-1.0.0/accord_nlp/text_classification/relation_extraction/re_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,15 @@
     def __init__(
             self,
             model_type,
             model_name,
             num_labels=None,
             weight=None,
             args=None,
-            use_cuda=True,
+            use_cuda=torch.cuda.is_available(),
             cuda_device=-1,
             onnx_execution_provider=None,
             merge_type=None,
             merge_n=2,
             **kwargs,
     ):
```

### Comparing `accord_nlp-0.1.8/accord_nlp/text_classification/relation_extraction/utils.py` & `accord_nlp-1.0.0/accord_nlp/text_classification/relation_extraction/utils.py`

 * *Files identical despite different names*

### Comparing `accord_nlp-0.1.8/accord_nlp.egg-info/SOURCES.txt` & `accord_nlp-1.0.0/accord_nlp.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 LICENSE
 README.md
 setup.cfg
 setup.py
 accord_nlp/__init__.py
+accord_nlp/data_augmentation.py
 accord_nlp.egg-info/PKG-INFO
 accord_nlp.egg-info/SOURCES.txt
 accord_nlp.egg-info/dependency_links.txt
 accord_nlp.egg-info/requires.txt
 accord_nlp.egg-info/top_level.txt
 accord_nlp/information_extraction/__init__.py
 accord_nlp/information_extraction/convertor.py
 accord_nlp/information_extraction/ie_pipeline.py
 accord_nlp/text_classification/__init__.py
 accord_nlp/text_classification/config/__init__.py
 accord_nlp/text_classification/config/model_args.py
 accord_nlp/text_classification/config/utils.py
+accord_nlp/text_classification/language_modelling/__init__.py
+accord_nlp/text_classification/language_modelling/custom_models.py
+accord_nlp/text_classification/language_modelling/lm_model.py
+accord_nlp/text_classification/language_modelling/lm_utils.py
 accord_nlp/text_classification/ner/__init__.py
 accord_nlp/text_classification/ner/ner_model.py
 accord_nlp/text_classification/ner/utils.py
 accord_nlp/text_classification/relation_extraction/__init__.py
 accord_nlp/text_classification/relation_extraction/re_model.py
 accord_nlp/text_classification/relation_extraction/utils.py
 accord_nlp/text_classification/relation_extraction/models/__init__.py
```


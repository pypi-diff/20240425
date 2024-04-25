# Comparing `tmp/languagemodels-0.8.0rc1.tar.gz` & `tmp/languagemodels-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "languagemodels-0.8.0rc1.tar", last modified: Fri Aug  4 19:46:21 2023, max compression
+gzip compressed data, was "languagemodels-0.9.0.tar", last modified: Sat Oct  7 21:24:11 2023, max compression
```

## Comparing `languagemodels-0.8.0rc1.tar` & `languagemodels-0.9.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 jncraton  (1000) jncraton  (1000)        0 2023-08-04 19:46:21.669079 languagemodels-0.8.0rc1/
--rw-r--r--   0 jncraton  (1000) jncraton  (1000)     9977 2023-08-04 19:46:21.669079 languagemodels-0.8.0rc1/PKG-INFO
-drwxr-xr-x   0 jncraton  (1000) jncraton  (1000)        0 2023-08-04 19:46:21.669079 languagemodels-0.8.0rc1/languagemodels/
--rw-r--r--   0 jncraton  (1000) jncraton  (1000)    12249 2023-07-28 16:09:19.000000 languagemodels-0.8.0rc1/languagemodels/__init__.py
--rw-r--r--   0 jncraton  (1000) jncraton  (1000)    10131 2023-08-04 19:35:02.000000 languagemodels-0.8.0rc1/languagemodels/config.py
--rw-r--r--   0 jncraton  (1000) jncraton  (1000)     8157 2023-07-23 12:54:43.000000 languagemodels-0.8.0rc1/languagemodels/embeddings.py
--rw-r--r--   0 jncraton  (1000) jncraton  (1000)    10112 2023-08-04 19:34:11.000000 languagemodels-0.8.0rc1/languagemodels/inference.py
--rw-r--r--   0 jncraton  (1000) jncraton  (1000)     3758 2023-08-04 19:35:02.000000 languagemodels-0.8.0rc1/languagemodels/models.py
-drwxr-xr-x   0 jncraton  (1000) jncraton  (1000)        0 2023-08-04 19:46:21.669079 languagemodels-0.8.0rc1/languagemodels.egg-info/
--rw-r--r--   0 jncraton  (1000) jncraton  (1000)     9977 2023-08-04 19:46:21.000000 languagemodels-0.8.0rc1/languagemodels.egg-info/PKG-INFO
--rw-r--r--   0 jncraton  (1000) jncraton  (1000)      331 2023-08-04 19:46:21.000000 languagemodels-0.8.0rc1/languagemodels.egg-info/SOURCES.txt
--rw-r--r--   0 jncraton  (1000) jncraton  (1000)        1 2023-08-04 19:46:21.000000 languagemodels-0.8.0rc1/languagemodels.egg-info/dependency_links.txt
--rw-r--r--   0 jncraton  (1000) jncraton  (1000)       47 2023-08-04 19:46:21.000000 languagemodels-0.8.0rc1/languagemodels.egg-info/requires.txt
--rw-r--r--   0 jncraton  (1000) jncraton  (1000)       15 2023-08-04 19:46:21.000000 languagemodels-0.8.0rc1/languagemodels.egg-info/top_level.txt
--rw-r--r--   0 jncraton  (1000) jncraton  (1000)       38 2023-08-04 19:46:21.669079 languagemodels-0.8.0rc1/setup.cfg
--rw-r--r--   0 jncraton  (1000) jncraton  (1000)      778 2023-08-04 19:45:50.000000 languagemodels-0.8.0rc1/setup.py
+drwxrwxr-x   0 jncraton  (1000) jncraton  (1000)        0 2023-10-07 21:24:11.570630 languagemodels-0.9.0/
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     9974 2023-10-07 21:24:11.570630 languagemodels-0.9.0/PKG-INFO
+drwxrwxr-x   0 jncraton  (1000) jncraton  (1000)        0 2023-10-07 21:24:11.570630 languagemodels-0.9.0/languagemodels/
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)    12346 2023-10-07 21:23:20.000000 languagemodels-0.9.0/languagemodels/__init__.py
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)    12790 2023-10-07 21:23:20.000000 languagemodels-0.9.0/languagemodels/config.py
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     8590 2023-10-07 21:23:20.000000 languagemodels-0.9.0/languagemodels/embeddings.py
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)    10116 2023-10-07 21:23:20.000000 languagemodels-0.9.0/languagemodels/inference.py
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     3758 2023-08-19 18:43:38.000000 languagemodels-0.9.0/languagemodels/models.py
+drwxrwxr-x   0 jncraton  (1000) jncraton  (1000)        0 2023-10-07 21:24:11.570630 languagemodels-0.9.0/languagemodels.egg-info/
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     9974 2023-10-07 21:24:11.000000 languagemodels-0.9.0/languagemodels.egg-info/PKG-INFO
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)      331 2023-10-07 21:24:11.000000 languagemodels-0.9.0/languagemodels.egg-info/SOURCES.txt
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)        1 2023-10-07 21:24:11.000000 languagemodels-0.9.0/languagemodels.egg-info/dependency_links.txt
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)       47 2023-10-07 21:24:11.000000 languagemodels-0.9.0/languagemodels.egg-info/requires.txt
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)       15 2023-10-07 21:24:11.000000 languagemodels-0.9.0/languagemodels.egg-info/top_level.txt
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)       38 2023-10-07 21:24:11.570630 languagemodels-0.9.0/setup.cfg
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)      775 2023-10-07 21:23:20.000000 languagemodels-0.9.0/setup.py
```

### Comparing `languagemodels-0.8.0rc1/PKG-INFO` & `languagemodels-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: languagemodels
-Version: 0.8.0rc1
+Version: 0.9.0
 Summary: Simple inference for large language models
 Home-page: https://github.com/jncraton/languagemodels
 Author: Jon Craton
 Author-email: jon@joncraton.com
 License: UNKNOWN
 Description: Language Models
         ===============
```

### Comparing `languagemodels-0.8.0rc1/languagemodels/__init__.py` & `languagemodels-0.9.0/languagemodels/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -337,16 +337,17 @@
             "External_links",
         ]
 
         for cutoff in cutoffs:
             summary = summary.split(f'<span id="{cutoff}">', 1)[0]
 
         summary = re.sub(r"<p>", "\n\n", summary, flags=re.I)
-        summary = re.sub(r"\s*[\n\r]+\s*", "\n\n", summary, flags=re.I)
+        summary = re.sub(r"<!\-\-.*?\-\->", "", summary, flags=re.I | re.DOTALL)
         summary = re.sub(r"<.*?>", "", summary, flags=re.I)
+        summary = re.sub(r"\s*[\n\r]+\s*[\r\n]+[\s\r\n]*", "\n\n", summary, flags=re.I)
         summary = summary.strip()
         return summary
     else:
         return "No matching wiki page found."
 
 
 def get_weather(latitude, longitude):
```

### Comparing `languagemodels-0.8.0rc1/languagemodels/config.py` & `languagemodels-0.9.0/languagemodels/config.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+"""Global model and inference configuration
+
+This module manages the global configuration object shared between other
+modules in the package. It implements a dictionary with data validation
+on the keys and values.
+
+Note that this module provides access to many implementation details
+that are not expected to be used by average users. Specific models that
+have never been the default for the package may be removed at any time.
+"""
+
 import re
 import os
 from collections import namedtuple
 
 ConfigItem = namedtuple("ConfigItem", "initfn default")
 
 
@@ -101,14 +112,27 @@
         "params": 248e6,
         "quantization": "int8",
         "backend": "ct2",
         "architecture": "encoder-decoder-transformer",
         "license": "apache-2.0",
     },
     {
+        "name": "dialogstudio-t5-base-v1.0",
+        "tuning": "instruct",
+        "datasets": ["c4", "flan", "dialogstudio"],
+        "params": 248e6,
+        "quantization": "int8",
+        "backend": "ct2",
+        "architecture": "encoder-decoder-transformer",
+        "license": "apache-2.0",
+        "prompt_fmt": (
+            "Instruction: Answer honestly and helpfully. <USER> {instruction}"
+        ),
+    },
+    {
         "name": "LaMini-Flan-T5-77M",
         "tuning": "instruct",
         "datasets": ["c4", "flan", "lamini"],
         "params": 77e6,
         "backend": "ct2",
         "quantization": "int8",
         "architecture": "encoder-decoder-transformer",
@@ -121,32 +145,66 @@
         "params": 77e6,
         "quantization": "int8",
         "backend": "ct2",
         "architecture": "encoder-decoder-transformer",
         "license": "apache-2.0",
     },
     {
+        "name": "phi-1_5",
+        "tuning": "instruct",
+        "datasets": ["phi-1_5"],
+        "params": 14e8,
+        "quantization": "int8",
+        "backend": "ct2",
+        "architecture": "decoder-only-transformer",
+        "license": "other",
+    },
+    {
         "name": "LaMini-GPT-774M",
         "tuning": "instruct",
         "datasets": ["webtext", "lamini"],
         "params": 774e6,
         "quantization": "int8",
         "backend": "ct2",
         "architecture": "decoder-only-transformer",
         "license": "mit",
+        "prompt_fmt": (
+            "Below is an instruction that describes a task.\n"
+            "Write a response that completes the request.\n\n"
+            "### Instruction:\n{instruction}\n\n### Response:"
+        ),
     },
     {
         "name": "LaMini-GPT-124M",
         "tuning": "instruct",
         "datasets": ["webtext", "lamini"],
         "params": 124e6,
         "quantization": "int8",
         "backend": "ct2",
         "architecture": "decoder-only-transformer",
         "license": "mit",
+        "prompt_fmt": (
+            "Below is an instruction that describes a task.\n"
+            "Write a response that completes the request.\n\n"
+            "### Instruction:\n{instruction}\n\n### Response:"
+        ),
+    },
+    {
+        "name": "TinyLlama-1.1B-Chat-v0.3",
+        "tuning": "instruct",
+        "datasets": ["slimpajama", "starcoderdata"],
+        "params": 1.1e9,
+        "quantization": "int8",
+        "backend": "ct2",
+        "architecture": "decoder-only-transformer",
+        "license": "mit",
+        "prompt_fmt": (
+            "<|im_start|>user\n{instruction} <|im_end|> <|im_start|>assistant\n"
+        ),
+        "support": "deprecated",
     },
     {
         "name": "codet5p-770m-py",
         "tuning": "code",
         "datasets": ["github-code"],
         "params": 770e6,
         "quantization": "int8",
@@ -163,23 +221,45 @@
         "backend": "ct2",
         "architecture": "encoder-decoder-transformer",
         "license": "bsd-3-clause",
     },
     {
         "name": "all-MiniLM-L6-v2",
         "tuning": "embedding",
+        "query_prefix": "",
         "params": 22e6,
         "quantization": "int8",
         "backend": "ct2",
         "architecture": "encoder-only-transformer",
         "license": "apache-2.0",
     },
     {
+        "name": "gte-small",
+        "tuning": "embedding",
+        "query_prefix": "",
+        "params": 33e6,
+        "quantization": "int8",
+        "backend": "ct2",
+        "architecture": "encoder-only-transformer",
+        "license": "mit",
+    },
+    {
+        "name": "bge-small-en",
+        "tuning": "embedding",
+        "query_prefix": "Represent this sentence for searching relevant passages: ",
+        "params": 33e6,
+        "quantization": "int8",
+        "backend": "ct2",
+        "architecture": "encoder-only-transformer",
+        "license": "mit",
+    },
+    {
         "name": "e5-small-v2",
         "tuning": "embedding",
+        "query_prefix": "",
         "params": 33e6,
         "quantization": "int8",
         "backend": "ct2",
         "architecture": "encoder-only-transformer",
         "license": "mit",
     },
 ]
```

### Comparing `languagemodels-0.8.0rc1/languagemodels/embeddings.py` & `languagemodels-0.9.0/languagemodels/embeddings.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,46 @@
 import numpy as np
 
-from languagemodels.models import get_model
+from languagemodels.models import get_model, get_model_info
 
 
-def embed(doc):
-    """Gets embeddings for a document
+def embed(docs):
+    """Get embeddings for a batch of documents
 
-    >>> embed("I love Python!")[-3:]
+    >>> embed(["I love Python!"])[0].shape
+    (384,)
+
+    >>> embed(["I love Python!"])[0][-3:]
     array([0.1..., 0.1..., 0.0...], dtype=float32)
     """
+
     tokenizer, model = get_model("embedding")
 
-    tokens = tokenizer.encode(doc).ids
-    output = model.forward_batch([tokens[:512]])
-    embedding = np.mean(np.array(output.last_hidden_state), axis=1)[0]
-    embedding = embedding / np.linalg.norm(embedding)
-    return embedding
+    tokens = [tokenizer.encode(doc).ids[:512] for doc in docs]
+    outputs = model.forward_batch(tokens)
+
+    def mean_pool(last_hidden_state):
+        embedding = np.mean(last_hidden_state, axis=0)
+        embedding = embedding / np.linalg.norm(embedding)
+        return embedding
+
+    return [mean_pool(lhs) for lhs in np.array(outputs.last_hidden_state)]
 
 
 def search(query, docs):
     """Return docs sorted by match against query
 
     :param query: Input to match in search
     :param docs: List of docs to search against
     :return: List of (doc_num, score) tuples sorted by score descending
     """
 
-    query_embedding = embed(query)
+    prefix = get_model_info("embedding")["query_prefix"]
+
+    query_embedding = embed([f"{prefix}{query}"])[0]
 
     scores = [np.dot(query_embedding, d.embedding) for d in docs]
 
     return sorted(enumerate(scores), key=lambda x: x[1], reverse=True)
 
 
 def get_token_ids(doc):
@@ -147,17 +157,17 @@
     """
     A document used for semantic search
 
     Documents have content and an embedding that is used to match the content
     against other semantically similar documents.
     """
 
-    def __init__(self, content, name=""):
+    def __init__(self, content, name="", embedding=None):
         self.content = content
-        self.embedding = embed(content)
+        self.embedding = embedding if embedding is not None else embed([content])[0]
         self.name = name
 
 
 class RetrievalContext:
     """
     Provides a context for document retrieval
 
@@ -252,16 +262,18 @@
         if doc not in self.docs:
             self.docs.append(Document(doc))
             self.store_chunks(doc, name)
 
     def store_chunks(self, doc, name=""):
         chunks = chunk_doc(doc, name, self.chunk_size, self.chunk_overlap)
 
-        for chunk in chunks:
-            self.chunks.append(Document(chunk))
+        embeddings = embed(chunks)
+
+        for embedding, chunk in zip(embeddings, chunks):
+            self.chunks.append(Document(chunk, embedding=embedding))
 
     def get_context(self, query, max_tokens=128):
         """Gets context matching a query
 
         Context is capped by token length and is retrieved from stored
         document chunks
         """
```

### Comparing `languagemodels-0.8.0rc1/languagemodels/inference.py` & `languagemodels-0.9.0/languagemodels/inference.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import requests
 import re
 import os
 
-from languagemodels.models import get_model
+from languagemodels.models import get_model, get_model_info
 
 
 class InferenceException(Exception):
     pass
 
 
 def list_tokens(prompt):
@@ -107,15 +107,15 @@
     try:
         return resp["choices"][0]["message"]["content"]
     except KeyError:
         raise InferenceException(f"OpenAI error: {resp}")
 
 
 def generate_instruct(
-    prompt,
+    instruction,
     max_tokens=200,
     temperature=0.1,
     topk=1,
     repetition_penalty=1.3,
     prefix="",
     suppress=[],
 ):
@@ -123,23 +123,29 @@
 
     This may use a local model, or it may make an API call to an external
     model if API keys are available.
     """
     if os.environ.get("LANGUAGEMODELS_TS_KEY") or os.environ.get(
         "LANGUAGEMODELS_TS_SERVER"
     ):
-        return generate_ts("flan_t5_xxl_q4", prompt, max_tokens).strip()
+        return generate_ts("flan_t5_xxl_q4", instruction, max_tokens).strip()
 
     if os.environ.get("LANGUAGEMODELS_OA_KEY"):
-        return chat_oa("gpt-3.5-turbo", prompt, max_tokens).strip()
+        return chat_oa("gpt-3.5-turbo", instruction, max_tokens).strip()
 
     tokenizer, model = get_model("instruct")
 
     suppress = [tokenizer.encode(s, add_special_tokens=False).tokens for s in suppress]
 
+    model_info = get_model_info("instruct")
+
+    fmt = model_info.get("prompt_fmt", "{instruction}")
+
+    prompt = fmt.replace("{instruction}", instruction)
+
     if hasattr(model, "translate_batch"):
         results = model.translate_batch(
             [tokenizer.encode(prompt).tokens],
             target_prefix=[tokenizer.encode(prefix, add_special_tokens=False).tokens],
             repetition_penalty=repetition_penalty,
             max_decoding_length=max_tokens,
             sampling_temperature=temperature,
@@ -147,25 +153,21 @@
             suppress_sequences=suppress,
             beam_size=1,
         )
         output_tokens = results[0].hypotheses[0]
         output_ids = [tokenizer.token_to_id(t) for t in output_tokens]
         text = tokenizer.decode(output_ids, skip_special_tokens=True)
     else:
-        prompt = (
-            "Below is an instruction that describes a task.\n"
-            "Write a response that appropriately completes the request.\n\n"
-            f"### Instruction:{prompt}\n\n### Response:"
-        )
         results = model.generate_batch(
             [tokenizer.encode(prompt).tokens],
             repetition_penalty=repetition_penalty,
             max_length=max_tokens,
             sampling_temperature=temperature,
             sampling_topk=topk,
+            suppress_sequences=suppress,
             beam_size=1,
         )
         output_ids = results[0].sequences_ids[0]
         text = tokenizer.decode(output_ids, skip_special_tokens=True)
         text = text[len(prompt) :]
 
     return text
```

### Comparing `languagemodels-0.8.0rc1/languagemodels/models.py` & `languagemodels-0.9.0/languagemodels/models.py`

 * *Files identical despite different names*

### Comparing `languagemodels-0.8.0rc1/languagemodels.egg-info/PKG-INFO` & `languagemodels-0.9.0/languagemodels.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: languagemodels
-Version: 0.8.0rc1
+Version: 0.9.0
 Summary: Simple inference for large language models
 Home-page: https://github.com/jncraton/languagemodels
 Author: Jon Craton
 Author-email: jon@joncraton.com
 License: UNKNOWN
 Description: Language Models
         ===============
```


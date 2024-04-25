# Comparing `tmp/dblcsgen-0.2.3.tar.gz` & `tmp/dblcsgen-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dblcsgen-0.2.3.tar", last modified: Tue Apr 23 09:51:20 2024, max compression
+gzip compressed data, was "dblcsgen-0.2.4.tar", last modified: Thu Apr 25 16:22:05 2024, max compression
```

## Comparing `dblcsgen-0.2.3.tar` & `dblcsgen-0.2.4.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 09:51:20.839537 dblcsgen-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-23 09:51:18.000000 dblcsgen-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    28296 2024-04-23 09:51:20.839537 dblcsgen-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14259 2024-04-23 09:51:18.000000 dblcsgen-0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 09:51:20.839537 dblcsgen-0.2.3/dblcsgen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    28296 2024-04-23 09:51:20.000000 dblcsgen-0.2.3/dblcsgen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-04-23 09:51:20.000000 dblcsgen-0.2.3/dblcsgen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 09:51:20.000000 dblcsgen-0.2.3/dblcsgen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-23 09:51:20.000000 dblcsgen-0.2.3/dblcsgen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-23 09:51:20.000000 dblcsgen-0.2.3/dblcsgen.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-23 09:51:15.000000 dblcsgen-0.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 09:51:20.839537 dblcsgen-0.2.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 09:51:20.827537 dblcsgen-0.2.3/sglang/
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-23 09:51:15.000000 dblcsgen-0.2.3/sglang/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4443 2024-04-23 09:51:15.000000 dblcsgen-0.2.3/sglang/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 09:51:20.827537 dblcsgen-0.2.3/sglang/backend/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 09:51:15.000000 dblcsgen-0.2.3/sglang/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-04-23 09:51:15.000000 dblcsgen-0.2.3/sglang/backend/base_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     8319 2024-04-23 09:51:15.000000 dblcsgen-0.2.3/sglang/backend/runtime_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-23 09:51:15.000000 dblcsgen-0.2.3/sglang/global_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 09:51:20.827537 dblcsgen-0.2.3/sglang/lang/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 09:51:15.000000 dblcsgen-0.2.3/sglang/lang/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10476 2024-04-23 09:51:15.000000 dblcsgen-0.2.3/sglang/lang/chat_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     7527 2024-04-23 09:51:15.000000 dblcsgen-0.2.3/sglang/lang/compiler.py
--rw-r--r--   0 runner    (1001) docker     (127)    27168 2024-04-23 09:51:15.000000 dblcsgen-0.2.3/sglang/lang/interpreter.py
--rw-r--r--   0 runner    (1001) docker     (127)    13320 2024-04-23 09:51:15.000000 dblcsgen-0.2.3/sglang/lang/ir.py
--rw-r--r--   0 runner    (1001) docker     (127)     8260 2024-04-23 09:51:15.000000 dblcsgen-0.2.3/sglang/lang/tracer.py
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-23 09:51:15.000000 dblcsgen-0.2.3/sglang/launch_server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 09:51:20.831537 dblcsgen-0.2.3/sglang/srt/
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-23 09:51:15.000000 dblcsgen-0.2.3/sglang/srt/backend_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 09:51:20.831537 dblcsgen-0.2.3/sglang/srt/constrained/
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-04-23 09:51:15.000000 dblcsgen-0.2.3/sglang/srt/constrained/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-04-23 09:51:15.000000 dblcsgen-0.2.3/sglang/srt/constrained/base_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-04-23 09:51:15.000000 dblcsgen-0.2.3/sglang/srt/constrained/fsm_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     2482 2024-04-23 09:51:15.000000 dblcsgen-0.2.3/sglang/srt/constrained/jump_forward.py
--rw-r--r--   0 runner    (1001) docker     (127)    15496 2024-04-23 09:51:15.000000 dblcsgen-0.2.3/sglang/srt/conversation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5285 2024-04-23 09:51:15.000000 dblcsgen-0.2.3/sglang/srt/hf_transformers_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 09:51:20.831537 dblcsgen-0.2.3/sglang/srt/layers/
--rw-r--r--   0 runner    (1001) docker     (127)     5209 2024-04-23 09:51:15.000000 dblcsgen-0.2.3/sglang/srt/layers/context_flashattention_nopad.py
--rw-r--r--   0 runner    (1001) docker     (127)    12622 2024-04-23 09:51:15.000000 dblcsgen-0.2.3/sglang/srt/layers/extend_attention.py
--rw-r--r--   0 runner    (1001) docker     (127)     6887 2024-04-23 09:51:15.000000 dblcsgen-0.2.3/sglang/srt/layers/logits_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     5597 2024-04-23 09:51:15.000000 dblcsgen-0.2.3/sglang/srt/layers/radix_attention.py
--rw-r--r--   0 runner    (1001) docker     (127)     8516 2024-04-23 09:51:15.000000 dblcsgen-0.2.3/sglang/srt/layers/token_attention.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 09:51:20.835537 dblcsgen-0.2.3/sglang/srt/managers/
--rw-r--r--   0 runner    (1001) docker     (127)     3292 2024-04-23 09:51:15.000000 dblcsgen-0.2.3/sglang/srt/managers/detokenizer_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     3670 2024-04-23 09:51:15.000000 dblcsgen-0.2.3/sglang/srt/managers/io_struct.py
--rw-r--r--   0 runner    (1001) docker     (127)     4563 2024-04-23 09:51:15.000000 dblcsgen-0.2.3/sglang/srt/managers/openai_protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 09:51:20.835537 dblcsgen-0.2.3/sglang/srt/managers/router/
--rw-r--r--   0 runner    (1001) docker     (127)    19922 2024-04-23 09:51:15.000000 dblcsgen-0.2.3/sglang/srt/managers/router/infer_batch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2682 2024-04-23 09:51:15.000000 dblcsgen-0.2.3/sglang/srt/managers/router/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    28007 2024-04-23 09:51:15.000000 dblcsgen-0.2.3/sglang/srt/managers/router/model_rpc.py
--rw-r--r--   0 runner    (1001) docker     (127)    16926 2024-04-23 09:51:15.000000 dblcsgen-0.2.3/sglang/srt/managers/router/model_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     6524 2024-04-23 09:51:15.000000 dblcsgen-0.2.3/sglang/srt/managers/router/radix_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-04-23 09:51:15.000000 dblcsgen-0.2.3/sglang/srt/managers/router/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)     9743 2024-04-23 09:51:15.000000 dblcsgen-0.2.3/sglang/srt/managers/tokenizer_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     3609 2024-04-23 09:51:15.000000 dblcsgen-0.2.3/sglang/srt/memory_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)     8889 2024-04-23 09:51:15.000000 dblcsgen-0.2.3/sglang/srt/mm_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-04-23 09:51:15.000000 dblcsgen-0.2.3/sglang/srt/model_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 09:51:20.835537 dblcsgen-0.2.3/sglang/srt/models/
--rw-r--r--   0 runner    (1001) docker     (127)    14112 2024-04-23 09:51:15.000000 dblcsgen-0.2.3/sglang/srt/models/dbrx.py
--rw-r--r--   0 runner    (1001) docker     (127)    11071 2024-04-23 09:51:15.000000 dblcsgen-0.2.3/sglang/srt/models/dbrx_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    11587 2024-04-23 09:51:15.000000 dblcsgen-0.2.3/sglang/srt/models/gemma.py
--rw-r--r--   0 runner    (1001) docker     (127)    11611 2024-04-23 09:51:15.000000 dblcsgen-0.2.3/sglang/srt/models/llama2.py
--rw-r--r--   0 runner    (1001) docker     (127)    14922 2024-04-23 09:51:15.000000 dblcsgen-0.2.3/sglang/srt/models/llava.py
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-23 09:51:15.000000 dblcsgen-0.2.3/sglang/srt/models/mistral.py
--rw-r--r--   0 runner    (1001) docker     (127)    13915 2024-04-23 09:51:15.000000 dblcsgen-0.2.3/sglang/srt/models/mixtral.py
--rw-r--r--   0 runner    (1001) docker     (127)     9225 2024-04-23 09:51:15.000000 dblcsgen-0.2.3/sglang/srt/models/qwen.py
--rw-r--r--   0 runner    (1001) docker     (127)    11307 2024-04-23 09:51:15.000000 dblcsgen-0.2.3/sglang/srt/models/qwen2.py
--rw-r--r--   0 runner    (1001) docker     (127)    10816 2024-04-23 09:51:15.000000 dblcsgen-0.2.3/sglang/srt/models/stablelm.py
--rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-04-23 09:51:15.000000 dblcsgen-0.2.3/sglang/srt/models/yivl.py
--rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-04-23 09:51:15.000000 dblcsgen-0.2.3/sglang/srt/sampling_params.py
--rw-r--r--   0 runner    (1001) docker     (127)    27702 2024-04-23 09:51:15.000000 dblcsgen-0.2.3/sglang/srt/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     9143 2024-04-23 09:51:15.000000 dblcsgen-0.2.3/sglang/srt/server_args.py
--rw-r--r--   0 runner    (1001) docker     (127)     7582 2024-04-23 09:51:15.000000 dblcsgen-0.2.3/sglang/srt/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 09:51:20.839537 dblcsgen-0.2.3/sglang/test/
--rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-04-23 09:51:15.000000 dblcsgen-0.2.3/sglang/test/test_conversation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-04-23 09:51:15.000000 dblcsgen-0.2.3/sglang/test/test_openai_protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)    11421 2024-04-23 09:51:15.000000 dblcsgen-0.2.3/sglang/test/test_programs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4830 2024-04-23 09:51:15.000000 dblcsgen-0.2.3/sglang/test/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6237 2024-04-23 09:51:15.000000 dblcsgen-0.2.3/sglang/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:22:05.767481 dblcsgen-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-25 16:22:03.000000 dblcsgen-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    28296 2024-04-25 16:22:05.767481 dblcsgen-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14259 2024-04-25 16:22:03.000000 dblcsgen-0.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:22:05.763481 dblcsgen-0.2.4/dblcsgen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    28296 2024-04-25 16:22:05.000000 dblcsgen-0.2.4/dblcsgen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-04-25 16:22:05.000000 dblcsgen-0.2.4/dblcsgen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 16:22:05.000000 dblcsgen-0.2.4/dblcsgen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-25 16:22:05.000000 dblcsgen-0.2.4/dblcsgen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-25 16:22:05.000000 dblcsgen-0.2.4/dblcsgen.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-25 16:22:00.000000 dblcsgen-0.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 16:22:05.767481 dblcsgen-0.2.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:22:05.751481 dblcsgen-0.2.4/sglang/
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-25 16:22:00.000000 dblcsgen-0.2.4/sglang/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4443 2024-04-25 16:22:00.000000 dblcsgen-0.2.4/sglang/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:22:05.751481 dblcsgen-0.2.4/sglang/backend/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 16:22:00.000000 dblcsgen-0.2.4/sglang/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-04-25 16:22:00.000000 dblcsgen-0.2.4/sglang/backend/base_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8319 2024-04-25 16:22:00.000000 dblcsgen-0.2.4/sglang/backend/runtime_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-25 16:22:00.000000 dblcsgen-0.2.4/sglang/global_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:22:05.755481 dblcsgen-0.2.4/sglang/lang/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 16:22:00.000000 dblcsgen-0.2.4/sglang/lang/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10476 2024-04-25 16:22:00.000000 dblcsgen-0.2.4/sglang/lang/chat_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7527 2024-04-25 16:22:00.000000 dblcsgen-0.2.4/sglang/lang/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27168 2024-04-25 16:22:00.000000 dblcsgen-0.2.4/sglang/lang/interpreter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13320 2024-04-25 16:22:00.000000 dblcsgen-0.2.4/sglang/lang/ir.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8260 2024-04-25 16:22:00.000000 dblcsgen-0.2.4/sglang/lang/tracer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-25 16:22:00.000000 dblcsgen-0.2.4/sglang/launch_server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:22:05.755481 dblcsgen-0.2.4/sglang/srt/
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-25 16:22:00.000000 dblcsgen-0.2.4/sglang/srt/backend_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:22:05.755481 dblcsgen-0.2.4/sglang/srt/constrained/
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-04-25 16:22:00.000000 dblcsgen-0.2.4/sglang/srt/constrained/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-04-25 16:22:00.000000 dblcsgen-0.2.4/sglang/srt/constrained/base_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-04-25 16:22:00.000000 dblcsgen-0.2.4/sglang/srt/constrained/fsm_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2482 2024-04-25 16:22:00.000000 dblcsgen-0.2.4/sglang/srt/constrained/jump_forward.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15496 2024-04-25 16:22:00.000000 dblcsgen-0.2.4/sglang/srt/conversation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5285 2024-04-25 16:22:00.000000 dblcsgen-0.2.4/sglang/srt/hf_transformers_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:22:05.759481 dblcsgen-0.2.4/sglang/srt/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)     5209 2024-04-25 16:22:00.000000 dblcsgen-0.2.4/sglang/srt/layers/context_flashattention_nopad.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12622 2024-04-25 16:22:00.000000 dblcsgen-0.2.4/sglang/srt/layers/extend_attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6887 2024-04-25 16:22:00.000000 dblcsgen-0.2.4/sglang/srt/layers/logits_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5597 2024-04-25 16:22:00.000000 dblcsgen-0.2.4/sglang/srt/layers/radix_attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8516 2024-04-25 16:22:00.000000 dblcsgen-0.2.4/sglang/srt/layers/token_attention.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:22:05.759481 dblcsgen-0.2.4/sglang/srt/managers/
+-rw-r--r--   0 runner    (1001) docker     (127)     3292 2024-04-25 16:22:00.000000 dblcsgen-0.2.4/sglang/srt/managers/detokenizer_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3670 2024-04-25 16:22:00.000000 dblcsgen-0.2.4/sglang/srt/managers/io_struct.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4563 2024-04-25 16:22:00.000000 dblcsgen-0.2.4/sglang/srt/managers/openai_protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:22:05.759481 dblcsgen-0.2.4/sglang/srt/managers/router/
+-rw-r--r--   0 runner    (1001) docker     (127)    19922 2024-04-25 16:22:00.000000 dblcsgen-0.2.4/sglang/srt/managers/router/infer_batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2682 2024-04-25 16:22:00.000000 dblcsgen-0.2.4/sglang/srt/managers/router/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28072 2024-04-25 16:22:00.000000 dblcsgen-0.2.4/sglang/srt/managers/router/model_rpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16926 2024-04-25 16:22:00.000000 dblcsgen-0.2.4/sglang/srt/managers/router/model_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6524 2024-04-25 16:22:00.000000 dblcsgen-0.2.4/sglang/srt/managers/router/radix_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-04-25 16:22:00.000000 dblcsgen-0.2.4/sglang/srt/managers/router/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9743 2024-04-25 16:22:00.000000 dblcsgen-0.2.4/sglang/srt/managers/tokenizer_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3609 2024-04-25 16:22:00.000000 dblcsgen-0.2.4/sglang/srt/memory_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8889 2024-04-25 16:22:00.000000 dblcsgen-0.2.4/sglang/srt/mm_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-04-25 16:22:00.000000 dblcsgen-0.2.4/sglang/srt/model_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:22:05.763481 dblcsgen-0.2.4/sglang/srt/models/
+-rw-r--r--   0 runner    (1001) docker     (127)    14112 2024-04-25 16:22:00.000000 dblcsgen-0.2.4/sglang/srt/models/dbrx.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11071 2024-04-25 16:22:00.000000 dblcsgen-0.2.4/sglang/srt/models/dbrx_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11587 2024-04-25 16:22:00.000000 dblcsgen-0.2.4/sglang/srt/models/gemma.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11611 2024-04-25 16:22:00.000000 dblcsgen-0.2.4/sglang/srt/models/llama2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14922 2024-04-25 16:22:00.000000 dblcsgen-0.2.4/sglang/srt/models/llava.py
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-25 16:22:00.000000 dblcsgen-0.2.4/sglang/srt/models/mistral.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13915 2024-04-25 16:22:00.000000 dblcsgen-0.2.4/sglang/srt/models/mixtral.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9225 2024-04-25 16:22:00.000000 dblcsgen-0.2.4/sglang/srt/models/qwen.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11307 2024-04-25 16:22:00.000000 dblcsgen-0.2.4/sglang/srt/models/qwen2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10816 2024-04-25 16:22:00.000000 dblcsgen-0.2.4/sglang/srt/models/stablelm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-04-25 16:22:00.000000 dblcsgen-0.2.4/sglang/srt/models/yivl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-04-25 16:22:00.000000 dblcsgen-0.2.4/sglang/srt/sampling_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27702 2024-04-25 16:22:00.000000 dblcsgen-0.2.4/sglang/srt/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9143 2024-04-25 16:22:00.000000 dblcsgen-0.2.4/sglang/srt/server_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7582 2024-04-25 16:22:00.000000 dblcsgen-0.2.4/sglang/srt/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:22:05.763481 dblcsgen-0.2.4/sglang/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-04-25 16:22:00.000000 dblcsgen-0.2.4/sglang/test/test_conversation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-04-25 16:22:00.000000 dblcsgen-0.2.4/sglang/test/test_openai_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11421 2024-04-25 16:22:00.000000 dblcsgen-0.2.4/sglang/test/test_programs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4830 2024-04-25 16:22:00.000000 dblcsgen-0.2.4/sglang/test/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6237 2024-04-25 16:22:00.000000 dblcsgen-0.2.4/sglang/utils.py
```

### Comparing `dblcsgen-0.2.3/LICENSE` & `dblcsgen-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.3/PKG-INFO` & `dblcsgen-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dblcsgen
-Version: 0.2.3
+Version: 0.2.4
 Summary: DBLC Fast Structured Generation
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `dblcsgen-0.2.3/README.md` & `dblcsgen-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.3/dblcsgen.egg-info/PKG-INFO` & `dblcsgen-0.2.4/dblcsgen.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dblcsgen
-Version: 0.2.3
+Version: 0.2.4
 Summary: DBLC Fast Structured Generation
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `dblcsgen-0.2.3/dblcsgen.egg-info/SOURCES.txt` & `dblcsgen-0.2.4/dblcsgen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.3/pyproject.toml` & `dblcsgen-0.2.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dblcsgen"
-version = "0.2.3"
+version = "0.2.4"
 description = "DBLC Fast Structured Generation"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {file = "LICENSE"}
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
```

### Comparing `dblcsgen-0.2.3/sglang/api.py` & `dblcsgen-0.2.4/sglang/api.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.3/sglang/backend/base_backend.py` & `dblcsgen-0.2.4/sglang/backend/base_backend.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.3/sglang/backend/runtime_endpoint.py` & `dblcsgen-0.2.4/sglang/backend/runtime_endpoint.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.3/sglang/global_config.py` & `dblcsgen-0.2.4/sglang/global_config.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.3/sglang/lang/chat_template.py` & `dblcsgen-0.2.4/sglang/lang/chat_template.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.3/sglang/lang/compiler.py` & `dblcsgen-0.2.4/sglang/lang/compiler.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.3/sglang/lang/interpreter.py` & `dblcsgen-0.2.4/sglang/lang/interpreter.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.3/sglang/lang/ir.py` & `dblcsgen-0.2.4/sglang/lang/ir.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.3/sglang/lang/tracer.py` & `dblcsgen-0.2.4/sglang/lang/tracer.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.3/sglang/srt/constrained/__init__.py` & `dblcsgen-0.2.4/sglang/srt/constrained/__init__.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.3/sglang/srt/constrained/base_cache.py` & `dblcsgen-0.2.4/sglang/srt/constrained/base_cache.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.3/sglang/srt/constrained/fsm_cache.py` & `dblcsgen-0.2.4/sglang/srt/constrained/fsm_cache.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.3/sglang/srt/constrained/jump_forward.py` & `dblcsgen-0.2.4/sglang/srt/constrained/jump_forward.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.3/sglang/srt/conversation.py` & `dblcsgen-0.2.4/sglang/srt/conversation.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.3/sglang/srt/hf_transformers_utils.py` & `dblcsgen-0.2.4/sglang/srt/hf_transformers_utils.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.3/sglang/srt/layers/context_flashattention_nopad.py` & `dblcsgen-0.2.4/sglang/srt/layers/context_flashattention_nopad.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.3/sglang/srt/layers/extend_attention.py` & `dblcsgen-0.2.4/sglang/srt/layers/extend_attention.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.3/sglang/srt/layers/logits_processor.py` & `dblcsgen-0.2.4/sglang/srt/layers/logits_processor.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.3/sglang/srt/layers/radix_attention.py` & `dblcsgen-0.2.4/sglang/srt/layers/radix_attention.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.3/sglang/srt/layers/token_attention.py` & `dblcsgen-0.2.4/sglang/srt/layers/token_attention.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.3/sglang/srt/managers/detokenizer_manager.py` & `dblcsgen-0.2.4/sglang/srt/managers/detokenizer_manager.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.3/sglang/srt/managers/io_struct.py` & `dblcsgen-0.2.4/sglang/srt/managers/io_struct.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.3/sglang/srt/managers/openai_protocol.py` & `dblcsgen-0.2.4/sglang/srt/managers/openai_protocol.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.3/sglang/srt/managers/router/infer_batch.py` & `dblcsgen-0.2.4/sglang/srt/managers/router/infer_batch.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.3/sglang/srt/managers/router/manager.py` & `dblcsgen-0.2.4/sglang/srt/managers/router/manager.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.3/sglang/srt/managers/router/model_rpc.py` & `dblcsgen-0.2.4/sglang/srt/managers/router/model_rpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -343,23 +343,25 @@
                 if not (
                     req.extend_input_len + req.max_new_tokens() + new_batch_total_tokens
                     < available_size
                 ):
                     # Undo the insertion
                     delta = self.tree_cache.dec_ref_counter(req.last_node)
                     available_size += delta
+                    break
                 else:
                     # Add this request to the running batch
                     self.token_to_kv_pool.add_refs(req.prefix_indices)
                     can_run_list.append(req)
                     new_batch_total_tokens += (
                         req.extend_input_len + req.max_new_tokens()
                     )
                     new_batch_input_tokens += req.extend_input_len
-
+            else:
+                break
         if len(can_run_list) == 0:
             return None
 
         if self.tp_rank == 0:
             running_req = (
                 0 if self.running_batch is None else len(self.running_batch.reqs)
             )
```

### Comparing `dblcsgen-0.2.3/sglang/srt/managers/router/model_runner.py` & `dblcsgen-0.2.4/sglang/srt/managers/router/model_runner.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.3/sglang/srt/managers/router/radix_cache.py` & `dblcsgen-0.2.4/sglang/srt/managers/router/radix_cache.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.3/sglang/srt/managers/router/scheduler.py` & `dblcsgen-0.2.4/sglang/srt/managers/router/scheduler.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.3/sglang/srt/managers/tokenizer_manager.py` & `dblcsgen-0.2.4/sglang/srt/managers/tokenizer_manager.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.3/sglang/srt/memory_pool.py` & `dblcsgen-0.2.4/sglang/srt/memory_pool.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.3/sglang/srt/mm_utils.py` & `dblcsgen-0.2.4/sglang/srt/mm_utils.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.3/sglang/srt/model_config.py` & `dblcsgen-0.2.4/sglang/srt/model_config.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.3/sglang/srt/models/dbrx.py` & `dblcsgen-0.2.4/sglang/srt/models/dbrx.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.3/sglang/srt/models/dbrx_config.py` & `dblcsgen-0.2.4/sglang/srt/models/dbrx_config.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.3/sglang/srt/models/gemma.py` & `dblcsgen-0.2.4/sglang/srt/models/gemma.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.3/sglang/srt/models/llama2.py` & `dblcsgen-0.2.4/sglang/srt/models/llama2.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.3/sglang/srt/models/llava.py` & `dblcsgen-0.2.4/sglang/srt/models/llava.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.3/sglang/srt/models/mixtral.py` & `dblcsgen-0.2.4/sglang/srt/models/mixtral.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.3/sglang/srt/models/qwen.py` & `dblcsgen-0.2.4/sglang/srt/models/qwen.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.3/sglang/srt/models/qwen2.py` & `dblcsgen-0.2.4/sglang/srt/models/qwen2.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.3/sglang/srt/models/stablelm.py` & `dblcsgen-0.2.4/sglang/srt/models/stablelm.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.3/sglang/srt/models/yivl.py` & `dblcsgen-0.2.4/sglang/srt/models/yivl.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.3/sglang/srt/sampling_params.py` & `dblcsgen-0.2.4/sglang/srt/sampling_params.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.3/sglang/srt/server.py` & `dblcsgen-0.2.4/sglang/srt/server.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.3/sglang/srt/server_args.py` & `dblcsgen-0.2.4/sglang/srt/server_args.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.3/sglang/srt/utils.py` & `dblcsgen-0.2.4/sglang/srt/utils.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.3/sglang/test/test_conversation.py` & `dblcsgen-0.2.4/sglang/test/test_conversation.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.3/sglang/test/test_openai_protocol.py` & `dblcsgen-0.2.4/sglang/test/test_openai_protocol.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.3/sglang/test/test_programs.py` & `dblcsgen-0.2.4/sglang/test/test_programs.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.3/sglang/test/test_utils.py` & `dblcsgen-0.2.4/sglang/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.3/sglang/utils.py` & `dblcsgen-0.2.4/sglang/utils.py`

 * *Files identical despite different names*


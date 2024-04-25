# Comparing `tmp/ipex_llm-2.1.0b20240423-py3-none-win_amd64.whl.zip` & `tmp/ipex_llm-2.1.0b20240424-py3-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 5263783 bytes, number of entries: 186
+Zip file size: 5267978 bytes, number of entries: 187
 -rw-------  2.0 unx     1898 b- defN 24-Mar-25 11:36 ipex_llm/__init__.py
 -rw-------  2.0 unx     6816 b- defN 24-Mar-25 11:36 ipex_llm/convert_model.py
 -rw-------  2.0 unx     3091 b- defN 24-Apr-17 15:07 ipex_llm/llm_patching.py
 -rw-------  2.0 unx     1177 b- defN 24-Mar-25 11:36 ipex_llm/models.py
 -rw-------  2.0 unx    12404 b- defN 24-Apr-18 12:34 ipex_llm/optimize.py
 -rw-------  2.0 unx     2769 b- defN 24-Mar-25 11:36 ipex_llm/cli/llm-chat.ps1
 -rwx------  2.0 unx     3009 b- defN 24-Mar-25 11:36 ipex_llm/cli/llm-cli.ps1
@@ -38,59 +38,59 @@
 -rw-------  2.0 unx     1189 b- defN 24-Mar-25 11:36 ipex_llm/langchain/embeddings/__init__.py
 -rw-------  2.0 unx    13589 b- defN 24-Mar-25 11:36 ipex_llm/langchain/embeddings/bigdlllm.py
 -rw-------  2.0 unx     7225 b- defN 24-Mar-25 11:36 ipex_llm/langchain/embeddings/transformersembeddings.py
 -rw-------  2.0 unx     1636 b- defN 24-Mar-25 11:36 ipex_llm/langchain/llms/__init__.py
 -rw-------  2.0 unx    24438 b- defN 24-Mar-25 11:36 ipex_llm/langchain/llms/bigdlllm.py
 -rw-------  2.0 unx    10576 b- defN 24-Apr-03 15:07 ipex_llm/langchain/llms/transformersllm.py
 -rw-------  2.0 unx     7379 b- defN 24-Mar-25 11:36 ipex_llm/langchain/llms/transformerspipelinellm.py
--rw-------  2.0 unx        0 b- defN 24-Apr-23 15:08 ipex_llm/libs/__init__.py
--rw-------  2.0 unx    36352 b- defN 24-Apr-23 15:08 ipex_llm/libs/bloom-api.dll
--rw-------  2.0 unx   460288 b- defN 24-Apr-23 15:08 ipex_llm/libs/bloom.dll
--rw-------  2.0 unx   852992 b- defN 24-Apr-23 15:08 ipex_llm/libs/chatglm_C.cp310-win_amd64.pyd
--rw-------  2.0 unx   856064 b- defN 24-Apr-23 15:08 ipex_llm/libs/chatglm_C.cp311-win_amd64.pyd
--rw-------  2.0 unx   843776 b- defN 24-Apr-23 15:08 ipex_llm/libs/chatglm_C.cp39-win_amd64.pyd
--rw-------  2.0 unx    24576 b- defN 24-Apr-23 15:08 ipex_llm/libs/gptneox-api.dll
--rw-------  2.0 unx   520192 b- defN 24-Apr-23 15:08 ipex_llm/libs/gptneox.dll
--rw-------  2.0 unx   485888 b- defN 24-Apr-23 15:08 ipex_llm/libs/libbloom_avx.dll
--rw-------  2.0 unx   460800 b- defN 24-Apr-23 15:08 ipex_llm/libs/libbloom_vnni.dll
--rw-------  2.0 unx   545792 b- defN 24-Apr-23 15:08 ipex_llm/libs/libgptneox_avx.dll
--rw-------  2.0 unx   520704 b- defN 24-Apr-23 15:08 ipex_llm/libs/libgptneox_vnni.dll
--rw-------  2.0 unx   540160 b- defN 24-Apr-23 15:08 ipex_llm/libs/libllama_avx.dll
--rw-------  2.0 unx   515072 b- defN 24-Apr-23 15:08 ipex_llm/libs/libllama_vnni.dll
--rw-------  2.0 unx   577024 b- defN 24-Apr-23 15:08 ipex_llm/libs/libstarcoder_avx.dll
--rw-------  2.0 unx   551936 b- defN 24-Apr-23 15:08 ipex_llm/libs/libstarcoder_vnni.dll
--rw-------  2.0 unx    25088 b- defN 24-Apr-23 15:08 ipex_llm/libs/llama-api.dll
--rw-------  2.0 unx   514560 b- defN 24-Apr-23 15:08 ipex_llm/libs/llama.dll
--rw-------  2.0 unx   103424 b- defN 24-Apr-23 15:08 ipex_llm/libs/main-bloom.exe
--rw-------  2.0 unx   726016 b- defN 24-Apr-23 15:08 ipex_llm/libs/main-chatglm_vnni.exe
--rw-------  2.0 unx    98816 b- defN 24-Apr-23 15:08 ipex_llm/libs/main-gptneox.exe
--rw-------  2.0 unx    99840 b- defN 24-Apr-23 15:08 ipex_llm/libs/main-llama.exe
--rw-------  2.0 unx   157696 b- defN 24-Apr-23 15:08 ipex_llm/libs/main-starcoder.exe
--rw-------  2.0 unx   125952 b- defN 24-Apr-23 15:08 ipex_llm/libs/quantize-bloom.exe
--rw-------  2.0 unx   127488 b- defN 24-Apr-23 15:08 ipex_llm/libs/quantize-bloom_vnni.exe
--rw-------  2.0 unx   103936 b- defN 24-Apr-23 15:08 ipex_llm/libs/quantize-gptneox.exe
--rw-------  2.0 unx   104448 b- defN 24-Apr-23 15:08 ipex_llm/libs/quantize-gptneox_vnni.exe
--rw-------  2.0 unx   109056 b- defN 24-Apr-23 15:08 ipex_llm/libs/quantize-llama.exe
--rw-------  2.0 unx   110080 b- defN 24-Apr-23 15:08 ipex_llm/libs/quantize-llama_vnni.exe
--rw-------  2.0 unx   126976 b- defN 24-Apr-23 15:08 ipex_llm/libs/quantize-starcoder.exe
--rw-------  2.0 unx   128000 b- defN 24-Apr-23 15:08 ipex_llm/libs/quantize-starcoder_vnni.exe
--rw-------  2.0 unx    21504 b- defN 24-Apr-23 15:08 ipex_llm/libs/starcoder-api.dll
--rw-------  2.0 unx   551424 b- defN 24-Apr-23 15:08 ipex_llm/libs/starcoder.dll
+-rw-------  2.0 unx        0 b- defN 24-Apr-24 15:08 ipex_llm/libs/__init__.py
+-rw-------  2.0 unx    36352 b- defN 24-Apr-24 15:08 ipex_llm/libs/bloom-api.dll
+-rw-------  2.0 unx   460288 b- defN 24-Apr-24 15:08 ipex_llm/libs/bloom.dll
+-rw-------  2.0 unx   852992 b- defN 24-Apr-24 15:08 ipex_llm/libs/chatglm_C.cp310-win_amd64.pyd
+-rw-------  2.0 unx   856064 b- defN 24-Apr-24 15:08 ipex_llm/libs/chatglm_C.cp311-win_amd64.pyd
+-rw-------  2.0 unx   843776 b- defN 24-Apr-24 15:08 ipex_llm/libs/chatglm_C.cp39-win_amd64.pyd
+-rw-------  2.0 unx    24576 b- defN 24-Apr-24 15:08 ipex_llm/libs/gptneox-api.dll
+-rw-------  2.0 unx   520192 b- defN 24-Apr-24 15:08 ipex_llm/libs/gptneox.dll
+-rw-------  2.0 unx   485888 b- defN 24-Apr-24 15:08 ipex_llm/libs/libbloom_avx.dll
+-rw-------  2.0 unx   460800 b- defN 24-Apr-24 15:08 ipex_llm/libs/libbloom_vnni.dll
+-rw-------  2.0 unx   545792 b- defN 24-Apr-24 15:08 ipex_llm/libs/libgptneox_avx.dll
+-rw-------  2.0 unx   520704 b- defN 24-Apr-24 15:08 ipex_llm/libs/libgptneox_vnni.dll
+-rw-------  2.0 unx   540160 b- defN 24-Apr-24 15:08 ipex_llm/libs/libllama_avx.dll
+-rw-------  2.0 unx   515072 b- defN 24-Apr-24 15:08 ipex_llm/libs/libllama_vnni.dll
+-rw-------  2.0 unx   577024 b- defN 24-Apr-24 15:08 ipex_llm/libs/libstarcoder_avx.dll
+-rw-------  2.0 unx   551936 b- defN 24-Apr-24 15:08 ipex_llm/libs/libstarcoder_vnni.dll
+-rw-------  2.0 unx    25088 b- defN 24-Apr-24 15:08 ipex_llm/libs/llama-api.dll
+-rw-------  2.0 unx   514560 b- defN 24-Apr-24 15:08 ipex_llm/libs/llama.dll
+-rw-------  2.0 unx   103424 b- defN 24-Apr-24 15:08 ipex_llm/libs/main-bloom.exe
+-rw-------  2.0 unx   726016 b- defN 24-Apr-24 15:08 ipex_llm/libs/main-chatglm_vnni.exe
+-rw-------  2.0 unx    98816 b- defN 24-Apr-24 15:08 ipex_llm/libs/main-gptneox.exe
+-rw-------  2.0 unx    99840 b- defN 24-Apr-24 15:08 ipex_llm/libs/main-llama.exe
+-rw-------  2.0 unx   157696 b- defN 24-Apr-24 15:08 ipex_llm/libs/main-starcoder.exe
+-rw-------  2.0 unx   125952 b- defN 24-Apr-24 15:08 ipex_llm/libs/quantize-bloom.exe
+-rw-------  2.0 unx   127488 b- defN 24-Apr-24 15:08 ipex_llm/libs/quantize-bloom_vnni.exe
+-rw-------  2.0 unx   103936 b- defN 24-Apr-24 15:08 ipex_llm/libs/quantize-gptneox.exe
+-rw-------  2.0 unx   104448 b- defN 24-Apr-24 15:08 ipex_llm/libs/quantize-gptneox_vnni.exe
+-rw-------  2.0 unx   109056 b- defN 24-Apr-24 15:08 ipex_llm/libs/quantize-llama.exe
+-rw-------  2.0 unx   110080 b- defN 24-Apr-24 15:08 ipex_llm/libs/quantize-llama_vnni.exe
+-rw-------  2.0 unx   126976 b- defN 24-Apr-24 15:08 ipex_llm/libs/quantize-starcoder.exe
+-rw-------  2.0 unx   128000 b- defN 24-Apr-24 15:08 ipex_llm/libs/quantize-starcoder_vnni.exe
+-rw-------  2.0 unx    21504 b- defN 24-Apr-24 15:08 ipex_llm/libs/starcoder-api.dll
+-rw-------  2.0 unx   551424 b- defN 24-Apr-24 15:08 ipex_llm/libs/starcoder.dll
 -rw-------  2.0 unx      874 b- defN 24-Mar-25 11:36 ipex_llm/llamaindex/__init__.py
 -rw-------  2.0 unx     1139 b- defN 24-Apr-07 15:05 ipex_llm/llamaindex/llms/__init__.py
 -rw-------  2.0 unx    26314 b- defN 24-Apr-07 15:05 ipex_llm/llamaindex/llms/bigdlllm.py
 -rw-------  2.0 unx      586 b- defN 24-Mar-25 11:36 ipex_llm/serving/__init__.py
 -rw-------  2.0 unx      586 b- defN 24-Mar-25 11:36 ipex_llm/serving/fastchat/__init__.py
 -rw-------  2.0 unx    10084 b- defN 24-Mar-25 11:36 ipex_llm/serving/fastchat/bigdl_llm_model.py
 -rw-------  2.0 unx    11371 b- defN 24-Mar-27 11:49 ipex_llm/serving/fastchat/ipex_llm_worker.py
 -rw-------  2.0 unx    16649 b- defN 24-Mar-25 11:36 ipex_llm/serving/fastchat/model_worker.py
 -rw-------  2.0 unx    11232 b- defN 24-Apr-22 15:07 ipex_llm/serving/fastchat/vllm_worker.py
 -rw-------  2.0 unx     1005 b- defN 24-Mar-25 11:36 ipex_llm/transformers/__init__.py
 -rw-------  2.0 unx     1213 b- defN 24-Mar-25 11:36 ipex_llm/transformers/bmm.py
--rw-------  2.0 unx    70437 b- defN 24-Apr-22 15:07 ipex_llm/transformers/convert.py
+-rw-------  2.0 unx    71241 b- defN 24-Apr-24 15:07 ipex_llm/transformers/convert.py
 -rw-------  2.0 unx    14334 b- defN 24-Apr-22 15:07 ipex_llm/transformers/convert_ipex.py
 -rw-------  2.0 unx     4613 b- defN 24-Mar-25 11:36 ipex_llm/transformers/embedding.py
 -rw-------  2.0 unx     4533 b- defN 24-Apr-03 15:07 ipex_llm/transformers/kv.py
 -rw-------  2.0 unx     3289 b- defN 24-Apr-18 12:34 ipex_llm/transformers/lisa.py
 -rw-------  2.0 unx     5429 b- defN 24-Mar-25 11:36 ipex_llm/transformers/loader.py
 -rw-------  2.0 unx    14775 b- defN 24-Apr-22 15:07 ipex_llm/transformers/lookup.py
 -rw-------  2.0 unx    38388 b- defN 24-Apr-18 12:34 ipex_llm/transformers/low_bit_linear.py
@@ -142,29 +142,30 @@
 -rw-------  2.0 unx     8654 b- defN 24-Apr-16 15:08 ipex_llm/transformers/models/decilm.py
 -rw-------  2.0 unx    33549 b- defN 24-Apr-16 15:08 ipex_llm/transformers/models/falcon.py
 -rw-------  2.0 unx    12310 b- defN 24-Apr-19 15:09 ipex_llm/transformers/models/gemma.py
 -rw-------  2.0 unx     4342 b- defN 24-Mar-25 11:36 ipex_llm/transformers/models/gptbigcode.py
 -rw-------  2.0 unx    17973 b- defN 24-Apr-16 15:08 ipex_llm/transformers/models/gptj.py
 -rw-------  2.0 unx     6219 b- defN 24-Apr-16 15:08 ipex_llm/transformers/models/gptneox.py
 -rw-------  2.0 unx    11647 b- defN 24-Apr-16 15:08 ipex_llm/transformers/models/internlm.py
--rw-------  2.0 unx    97944 b- defN 24-Apr-23 15:07 ipex_llm/transformers/models/llama.py
--rw-------  2.0 unx    45181 b- defN 24-Apr-18 12:34 ipex_llm/transformers/models/mistral.py
+-rw-------  2.0 unx    97964 b- defN 24-Apr-24 15:07 ipex_llm/transformers/models/llama.py
+-rw-------  2.0 unx    45217 b- defN 24-Apr-24 15:07 ipex_llm/transformers/models/mistral.py
 -rw-------  2.0 unx    27294 b- defN 24-Apr-23 15:07 ipex_llm/transformers/models/mixtral.py
 -rw-------  2.0 unx     9540 b- defN 24-Apr-16 15:08 ipex_llm/transformers/models/mpt.py
 -rw-------  2.0 unx     7685 b- defN 24-Apr-22 15:07 ipex_llm/transformers/models/phi.py
+-rw-------  2.0 unx     7835 b- defN 24-Apr-24 15:07 ipex_llm/transformers/models/phi3.py
 -rw-------  2.0 unx     6268 b- defN 24-Apr-18 12:34 ipex_llm/transformers/models/phixtral.py
 -rw-------  2.0 unx    32349 b- defN 24-Apr-18 12:34 ipex_llm/transformers/models/qwen.py
 -rw-------  2.0 unx    32725 b- defN 24-Apr-18 12:34 ipex_llm/transformers/models/qwen2.py
--rw-------  2.0 unx    30334 b- defN 24-Apr-18 12:34 ipex_llm/transformers/models/qwen2_moe.py
+-rw-------  2.0 unx    38558 b- defN 24-Apr-24 15:07 ipex_llm/transformers/models/qwen2_moe.py
 -rw-------  2.0 unx    11832 b- defN 24-Apr-18 12:34 ipex_llm/transformers/models/qwen_vl.py
 -rw-------  2.0 unx     6135 b- defN 24-Mar-29 11:38 ipex_llm/transformers/models/rwkv4.py
 -rw-------  2.0 unx    10722 b- defN 24-Apr-09 15:06 ipex_llm/transformers/models/rwkv5.py
 -rw-------  2.0 unx    21125 b- defN 24-Apr-16 15:08 ipex_llm/transformers/models/stablelm.py
 -rw-------  2.0 unx     8822 b- defN 24-Apr-03 15:07 ipex_llm/transformers/models/starcoder2.py
--rw-------  2.0 unx    18248 b- defN 24-Apr-18 12:34 ipex_llm/transformers/models/utils.py
+-rw-------  2.0 unx    19678 b- defN 24-Apr-24 15:07 ipex_llm/transformers/models/utils.py
 -rw-------  2.0 unx    20278 b- defN 24-Apr-18 12:34 ipex_llm/transformers/models/yuan.py
 -rw-------  2.0 unx      874 b- defN 24-Mar-25 11:36 ipex_llm/utils/__init__.py
 -rw-------  2.0 unx    18074 b- defN 24-Mar-25 11:36 ipex_llm/utils/convert_chatglm.py
 -rw-------  2.0 unx    72612 b- defN 24-Mar-25 11:36 ipex_llm/utils/convert_util.py
 -rw-------  2.0 unx     2093 b- defN 24-Mar-25 11:36 ipex_llm/utils/glibc_checker.py
 -rw-------  2.0 unx     2477 b- defN 24-Mar-25 11:36 ipex_llm/utils/ipex_importer.py
 -rw-------  2.0 unx     2259 b- defN 24-Mar-25 11:36 ipex_llm/utils/isa_checker.py
@@ -174,15 +175,15 @@
 -rw-------  2.0 unx     2872 b- defN 24-Mar-25 11:36 ipex_llm/utils/common/lazyimport.py
 -rw-------  2.0 unx     1763 b- defN 24-Mar-25 11:36 ipex_llm/utils/common/log4Error.py
 -rw-------  2.0 unx      585 b- defN 24-Apr-22 15:07 ipex_llm/vllm/__init__.py
 -rw-------  2.0 unx     7208 b- defN 24-Apr-22 15:07 ipex_llm/vllm/model_convert.py
 -rw-------  2.0 unx      747 b- defN 24-Apr-22 15:07 ipex_llm/vllm/engine/__init__.py
 -rw-------  2.0 unx     5714 b- defN 24-Apr-22 15:07 ipex_llm/vllm/engine/engine.py
 -rw-------  2.0 unx    10564 b- defN 24-Apr-22 15:07 ipex_llm/vllm/entrypoints/openai/api_server.py
--rwxr-xr-x  2.0 unx     2769 b- defN 24-Mar-25 11:36 ipex_llm-2.1.0b20240423.data/scripts/llm-chat.ps1
--rwxr-xr-x  2.0 unx     3009 b- defN 24-Mar-25 11:36 ipex_llm-2.1.0b20240423.data/scripts/llm-cli.ps1
--rw-------  2.0 unx     5125 b- defN 24-Apr-23 15:08 ipex_llm-2.1.0b20240423.dist-info/METADATA
--rw-------  2.0 unx       98 b- defN 24-Apr-23 15:08 ipex_llm-2.1.0b20240423.dist-info/WHEEL
--rw-------  2.0 unx       61 b- defN 24-Apr-23 15:08 ipex_llm-2.1.0b20240423.dist-info/entry_points.txt
--rw-------  2.0 unx        9 b- defN 24-Apr-23 15:08 ipex_llm-2.1.0b20240423.dist-info/top_level.txt
--rw-rw-r--  2.0 unx    17635 b- defN 24-Apr-23 15:08 ipex_llm-2.1.0b20240423.dist-info/RECORD
-186 files, 12789983 bytes uncompressed, 5235603 bytes compressed:  59.1%
+-rwxr-xr-x  2.0 unx     2769 b- defN 24-Mar-25 11:36 ipex_llm-2.1.0b20240424.data/scripts/llm-chat.ps1
+-rwxr-xr-x  2.0 unx     3009 b- defN 24-Mar-25 11:36 ipex_llm-2.1.0b20240424.data/scripts/llm-cli.ps1
+-rw-------  2.0 unx     5125 b- defN 24-Apr-24 15:08 ipex_llm-2.1.0b20240424.dist-info/METADATA
+-rw-------  2.0 unx       98 b- defN 24-Apr-24 15:08 ipex_llm-2.1.0b20240424.dist-info/WHEEL
+-rw-------  2.0 unx       61 b- defN 24-Apr-24 15:08 ipex_llm-2.1.0b20240424.dist-info/entry_points.txt
+-rw-------  2.0 unx        9 b- defN 24-Apr-24 15:08 ipex_llm-2.1.0b20240424.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx    17728 b- defN 24-Apr-24 15:08 ipex_llm-2.1.0b20240424.dist-info/RECORD
+187 files, 12808425 bytes uncompressed, 5239650 bytes compressed:  59.1%
```

## zipnote {}

```diff
@@ -450,14 +450,17 @@
 
 Filename: ipex_llm/transformers/models/mpt.py
 Comment: 
 
 Filename: ipex_llm/transformers/models/phi.py
 Comment: 
 
+Filename: ipex_llm/transformers/models/phi3.py
+Comment: 
+
 Filename: ipex_llm/transformers/models/phixtral.py
 Comment: 
 
 Filename: ipex_llm/transformers/models/qwen.py
 Comment: 
 
 Filename: ipex_llm/transformers/models/qwen2.py
@@ -531,29 +534,29 @@
 
 Filename: ipex_llm/vllm/engine/engine.py
 Comment: 
 
 Filename: ipex_llm/vllm/entrypoints/openai/api_server.py
 Comment: 
 
-Filename: ipex_llm-2.1.0b20240423.data/scripts/llm-chat.ps1
+Filename: ipex_llm-2.1.0b20240424.data/scripts/llm-chat.ps1
 Comment: 
 
-Filename: ipex_llm-2.1.0b20240423.data/scripts/llm-cli.ps1
+Filename: ipex_llm-2.1.0b20240424.data/scripts/llm-cli.ps1
 Comment: 
 
-Filename: ipex_llm-2.1.0b20240423.dist-info/METADATA
+Filename: ipex_llm-2.1.0b20240424.dist-info/METADATA
 Comment: 
 
-Filename: ipex_llm-2.1.0b20240423.dist-info/WHEEL
+Filename: ipex_llm-2.1.0b20240424.dist-info/WHEEL
 Comment: 
 
-Filename: ipex_llm-2.1.0b20240423.dist-info/entry_points.txt
+Filename: ipex_llm-2.1.0b20240424.dist-info/entry_points.txt
 Comment: 
 
-Filename: ipex_llm-2.1.0b20240423.dist-info/top_level.txt
+Filename: ipex_llm-2.1.0b20240424.dist-info/top_level.txt
 Comment: 
 
-Filename: ipex_llm-2.1.0b20240423.dist-info/RECORD
+Filename: ipex_llm-2.1.0b20240424.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ipex_llm/libs/bloom-api.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x00000001800036cc
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Tue Apr 23 15:02:42 2024
+Time/Date		Wed Apr 24 15:02:45 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000003200
 SizeOfInitializedData	0000000000005e00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	00000000000036cc
@@ -6375,19 +6375,17 @@
    180005621:	push   %rdx
    180005622:	add    %al,0x1(%rax)
    180005628:	pop    %rax
    180005629:	push   %rdx
    18000562a:	add    %al,0x1(%rax)
    180005630:	add    %al,(%rax)
    180005632:	add    %al,(%rax)
-   180005634:	xchg   %eax,%edx
-   180005635:	int    $0x27
-   180005637:	data16 add %al,(%rax)
-   18000563a:	add    %al,(%rax)
-   18000563c:	or     $0xe0000000,%eax
+   180005634:	adc    $0x66291f,%eax
+   180005639:	add    %al,(%rax)
+   18000563b:	add    %cl,-0x20000000(%rip)        # 0x160005641
    180005641:	add    (%rax),%al
    180005643:	add    %cl,(%rcx,%rbx,2)
    180005646:	add    %al,(%rax)
    180005648:	or     $0x3f,%al
 	...
    18000567e:	add    %al,(%rax)
    180005680:	add    %eax,(%rax)
```

## ipex_llm/libs/bloom.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180052e48
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Tue Apr 23 15:02:42 2024
+Time/Date		Wed Apr 24 15:02:45 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000053400
 SizeOfInitializedData	00000000000bee00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000052e48
@@ -109410,15 +109410,15 @@
    18005c7ba:	add    $0x180,%eax
    18005c7bf:	add    %dh,0x56(%rax)
    18005c7c2:	add    $0x180,%eax
    18005c7c7:	add    %bh,0x56(%rax)
    18005c7ca:	add    $0x180,%eax
    18005c7cf:	add    %al,(%rax)
    18005c7d1:	add    %al,(%rax)
-   18005c7d3:	add    %dl,0x6627cd(%rdx)
+   18005c7d3:	add    %dl,0x66291f(%rip)        # 0x1806bf0f8
    18005c7d9:	add    %al,(%rax)
    18005c7db:	add    %cl,0x50000000(%rip)        # 0x1d005c7e1
    18005c7e1:	add    (%rax),%eax
    18005c7e3:	add    %ah,-0x5ffffa2f(%rax)
    18005c7e9:	mov    $0x5,%ecx
 	...
    18005c7fe:	add    %al,(%rax)
```

## ipex_llm/libs/gptneox-api.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180002cbc
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Tue Apr 23 15:02:42 2024
+Time/Date		Wed Apr 24 15:02:45 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000002600
 SizeOfInitializedData	0000000000003e00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000002cbc
@@ -5058,19 +5058,17 @@
    1800049c0:	cmp    %al,0x0(%rdx)
    1800049c3:	addb   $0x0,(%rcx)
    1800049c6:	add    %al,(%rax)
    1800049c8:	rex
    1800049c9:	rex.X add %al,0x1(%rax)
    1800049d0:	add    %al,(%rax)
    1800049d2:	add    %al,(%rax)
-   1800049d4:	xchg   %eax,%edx
-   1800049d5:	int    $0x27
-   1800049d7:	data16 add %al,(%rax)
-   1800049da:	add    %al,(%rax)
-   1800049dc:	or     $0xe0000000,%eax
+   1800049d4:	adc    $0x66291f,%eax
+   1800049d9:	add    %al,(%rax)
+   1800049db:	add    %cl,-0x20000000(%rip)        # 0x1600049e1
    1800049e1:	add    (%rax),%al
    1800049e3:	add    %ah,0x0(%rsp,%rcx,2)
    1800049e7:	add    %ah,0x0(%rsi,%rsi,1)
 	...
    1800049ff:	add    %al,(%rcx)
 	...
    180004a09:	add    %al,(%rax)
```

## ipex_llm/libs/gptneox.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x000000018005a5a8
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Tue Apr 23 15:02:43 2024
+Time/Date		Wed Apr 24 15:02:46 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		000000000005ae00
 SizeOfInitializedData	00000000000c6000
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000005a5a8
@@ -120845,19 +120845,19 @@
    18006307d:	add    %al,(%rax)
    18006307f:	add    %bh,0x18005c6(%rax)
    180063085:	add    %al,(%rax)
    180063087:	add    %al,%al
    180063089:	movb   $0x0,0x180(%rip)        # 0x180063210
    180063090:	add    %al,(%rax)
    180063092:	add    %al,(%rax)
-   180063094:	xchg   %eax,%ebx
-   180063095:	int    $0x27
-   180063097:	data16 add %al,(%rax)
-   18006309a:	add    %al,(%rax)
-   18006309c:	or     $0x50000000,%eax
+   180063094:	(bad)
+   180063095:	(bad)
+   180063096:	sub    %esp,0x0(%rsi)
+   180063099:	add    %al,(%rax)
+   18006309b:	add    %cl,0x50000000(%rip)        # 0x1d00630a1
    1800630a1:	add    (%rax),%eax
    1800630a3:	add    %al,0x2f040006(,%rdi,1)
    1800630aa:	(bad)
 	...
    1800630ff:	add    %bh,0x40(%rax)
    180063102:	(bad)
    180063103:	addb   $0x0,(%rcx)
```

## ipex_llm/libs/libbloom_avx.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180058c38
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Tue Apr 23 15:03:45 2024
+Time/Date		Wed Apr 24 15:07:18 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000059200
 SizeOfInitializedData	00000000000bf400
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000058c38
@@ -114727,16 +114727,16 @@
    1800626ed:	add    %al,(%rax)
    1800626ef:	add    %dh,-0x4a(%rax)
    1800626f2:	add    $0x180,%eax
    1800626f7:	add    %bh,-0x4a(%rax)
    1800626fa:	add    $0x180,%eax
    1800626ff:	add    %al,(%rax)
    180062701:	add    %al,(%rax)
-   180062703:	add    %dl,%cl
-   180062705:	int    $0x27
+   180062703:	add    %ah,(%rsi)
+   180062705:	and    %ch,(%rcx)
    180062707:	data16 add %al,(%rax)
    18006270a:	add    %al,(%rax)
    18006270c:	or     $0x50000000,%eax
    180062711:	add    (%rax),%eax
    180062713:	add    %ah,(%rax)
    180062715:	xor    %eax,(%rsi)
    180062717:	add    %ah,(%rax)
```

## ipex_llm/libs/libbloom_vnni.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180053058
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Tue Apr 23 15:04:44 2024
+Time/Date		Wed Apr 24 15:03:51 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000053600
 SizeOfInitializedData	00000000000bee00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000053058
@@ -109461,19 +109461,18 @@
    18005c79a:	add    $0x180,%eax
    18005c79f:	add    %dh,0x56(%rax)
    18005c7a2:	add    $0x180,%eax
    18005c7a7:	add    %bh,0x56(%rax)
    18005c7aa:	add    $0x180,%eax
    18005c7af:	add    %al,(%rax)
    18005c7b1:	add    %al,(%rax)
-   18005c7b3:	add    %cl,(%rsi,%rcx,8)
-   18005c7b6:	(bad)
-   18005c7b7:	data16 add %al,(%rax)
-   18005c7ba:	add    %al,(%rax)
-   18005c7bc:	or     $0x50000000,%eax
+   18005c7b3:	add    %dl,0x1f(%rdi)
+   18005c7b6:	sub    %esp,0x0(%rsi)
+   18005c7b9:	add    %al,(%rax)
+   18005c7bb:	add    %cl,0x50000000(%rip)        # 0x1d005c7c1
    18005c7c1:	add    (%rax),%eax
    18005c7c3:	add    %ah,-0x5ffffa2f(%rax)
    18005c7c9:	mov    $0x5,%ebx
 	...
    18005c7fe:	add    %al,(%rax)
    18005c800:	adc    %dl,%ch
    18005c802:	add    $0x180,%eax
```

## ipex_llm/libs/libgptneox_avx.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180060428
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Tue Apr 23 15:03:45 2024
+Time/Date		Wed Apr 24 15:07:19 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000060c00
 SizeOfInitializedData	00000000000c6600
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000060428
@@ -126192,16 +126192,16 @@
    180068fb5:	add    %al,(%rax)
    180068fb7:	add    %al,%al
    180068fb9:	es (bad)
    180068fbb:	addb   $0x0,(%rcx)
    180068fbe:	add    %al,(%rax)
    180068fc0:	add    %al,(%rax)
    180068fc2:	add    %al,(%rax)
-   180068fc4:	ror    $1,%ebp
-   180068fc6:	(bad)
+   180068fc4:	(bad)
+   180068fc5:	and    %ch,(%rcx)
    180068fc7:	data16 add %al,(%rax)
    180068fca:	add    %al,(%rax)
    180068fcc:	or     $0x50000000,%eax
    180068fd1:	add    (%rax),%eax
    180068fd3:	add    %al,(%rsp,%rbx,4)
    180068fd6:	(bad)
    180068fd7:	add    %al,(%rsp,%rcx,4)
```

## ipex_llm/libs/libgptneox_vnni.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x000000018005a7b8
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Tue Apr 23 15:04:44 2024
+Time/Date		Wed Apr 24 15:03:52 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		000000000005b000
 SizeOfInitializedData	00000000000c6000
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000005a7b8
@@ -121007,19 +121007,19 @@
    18006305d:	add    %al,(%rax)
    18006305f:	add    %bh,0x18005c6(%rax)
    180063065:	add    %al,(%rax)
    180063067:	add    %al,%al
    180063069:	movb   $0x0,0x180(%rip)        # 0x1800631f0
    180063070:	add    %al,(%rax)
    180063072:	add    %al,(%rax)
-   180063074:	or     $0xce,%al
-   180063076:	(bad)
-   180063077:	data16 add %al,(%rax)
-   18006307a:	add    %al,(%rax)
-   18006307c:	or     $0x50000000,%eax
+   180063074:	pop    %rax
+   180063075:	(bad)
+   180063076:	sub    %esp,0x0(%rsi)
+   180063079:	add    %al,(%rax)
+   18006307b:	add    %cl,0x50000000(%rip)        # 0x1d0063081
    180063081:	add    (%rax),%eax
    180063083:	add    %al,0x31040006(,%rdi,1)
    18006308a:	(bad)
 	...
    1800630ff:	add    %bh,0x40(%rax)
    180063102:	(bad)
    180063103:	addb   $0x0,(%rcx)
```

## ipex_llm/libs/libllama_avx.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x000000018005f138
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Tue Apr 23 15:03:46 2024
+Time/Date		Wed Apr 24 15:07:19 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		000000000005f800
 SizeOfInitializedData	00000000000c6400
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000005f138
@@ -124880,16 +124880,16 @@
    180068096:	add    %al,(%rax)
    180068098:	rclb   $1,(%rsi)
    18006809a:	(bad)
    18006809b:	addb   $0x0,(%rcx)
    18006809e:	add    %al,(%rax)
    1800680a0:	add    %al,(%rax)
    1800680a2:	add    %al,(%rax)
-   1800680a4:	ror    %cl,%ch
-   1800680a6:	(bad)
+   1800680a4:	(bad)
+   1800680a5:	and    %ch,(%rcx)
    1800680a7:	data16 add %al,(%rax)
    1800680aa:	add    %al,(%rax)
    1800680ac:	or     $0x50000000,%eax
    1800680b1:	add    (%rax),%eax
    1800680b3:	add    %al,(%rax)
    1800680b5:	lea    (%rsi),%eax
    1800680b7:	add    %al,(%rax)
```

## ipex_llm/libs/libllama_vnni.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x00000001800594c8
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Tue Apr 23 15:04:44 2024
+Time/Date		Wed Apr 24 15:03:52 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000059c00
 SizeOfInitializedData	00000000000c5e00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	00000000000594c8
@@ -119683,19 +119683,19 @@
    180062140:	enter  $0x5b6,$0x80
    180062144:	add    %eax,(%rax)
    180062146:	add    %al,(%rax)
    180062148:	shlb   $1,0x18005(%rsi)
    18006214e:	add    %al,(%rax)
    180062150:	add    %al,(%rax)
    180062152:	add    %al,(%rax)
-   180062154:	or     $0xce,%al
-   180062156:	(bad)
-   180062157:	data16 add %al,(%rax)
-   18006215a:	add    %al,(%rax)
-   18006215c:	or     $0x50000000,%eax
+   180062154:	pop    %rax
+   180062155:	(bad)
+   180062156:	sub    %esp,0x0(%rsi)
+   180062159:	add    %al,(%rax)
+   18006215b:	add    %cl,0x50000000(%rip)        # 0x1d0062161
    180062161:	add    (%rax),%eax
    180062163:	add    %al,-0x7ffff9d3(%rax)
    180062169:	sbb    $0x6,%eax
 	...
    18006217e:	add    %al,(%rax)
    180062180:	lock xor %al,(%rsi)
    180062183:	addb   $0x0,(%rcx)
```

## ipex_llm/libs/libstarcoder_avx.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180066598
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Tue Apr 23 15:03:45 2024
+Time/Date		Wed Apr 24 15:07:18 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000066c00
 SizeOfInitializedData	00000000000c8000
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000066598
@@ -135439,16 +135439,15 @@
    18006fbe5:	add    %al,(%rax)
    18006fbe7:	add    %al,%al
    18006fbe9:	xchg   %al,(%rsi)
    18006fbeb:	addb   $0x0,(%rcx)
    18006fbee:	add    %al,(%rax)
    18006fbf0:	add    %al,(%rax)
    18006fbf2:	add    %al,(%rax)
-   18006fbf4:	ror    $1,%ebp
-   18006fbf6:	(bad)
+   18006fbf4:	es and %ch,(%rcx)
    18006fbf7:	data16 add %al,(%rax)
    18006fbfa:	add    %al,(%rax)
    18006fbfc:	or     $0x50000000,%eax
    18006fc01:	add    (%rax),%eax
    18006fc03:	add    %dl,%al
    18006fc05:	or     $0xfdd00007,%eax
    18006fc0a:	(bad)
```

## ipex_llm/libs/libstarcoder_vnni.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x00000001800609b8
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Tue Apr 23 15:04:44 2024
+Time/Date		Wed Apr 24 15:03:51 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000061000
 SizeOfInitializedData	00000000000c7a00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	00000000000609b8
@@ -130151,19 +130151,19 @@
    180069cb5:	add    %al,(%rax)
    180069cb7:	add    %al,%al
    180069cb9:	es (bad)
    180069cbb:	addb   $0x0,(%rcx)
    180069cbe:	add    %al,(%rax)
    180069cc0:	add    %al,(%rax)
    180069cc2:	add    %al,(%rax)
-   180069cc4:	or     $0xce,%al
-   180069cc6:	(bad)
-   180069cc7:	data16 add %al,(%rax)
-   180069cca:	add    %al,(%rax)
-   180069ccc:	or     $0x50000000,%eax
+   180069cc4:	push   %rdi
+   180069cc5:	(bad)
+   180069cc6:	sub    %esp,0x0(%rsi)
+   180069cc9:	add    %al,(%rax)
+   180069ccb:	add    %cl,0x50000000(%rip)        # 0x1d0069cd1
    180069cd1:	add    (%rax),%eax
    180069cd3:	add    %dl,-0x52(%rax)
    180069cd6:	(bad)
    180069cd7:	add    %dl,-0x5e(%rax)
    180069cda:	(bad)
 	...
    180069cff:	add    %al,%al
```

## ipex_llm/libs/llama-api.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180002dac
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Tue Apr 23 15:02:42 2024
+Time/Date		Wed Apr 24 15:02:45 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000002800
 SizeOfInitializedData	0000000000003e00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000002dac
@@ -5355,19 +5355,17 @@
    180004a20:	cmp    %al,0x0(%rdx)
    180004a23:	addb   $0x0,(%rcx)
    180004a26:	add    %al,(%rax)
    180004a28:	rex
    180004a29:	rex.X add %al,0x1(%rax)
    180004a30:	add    %al,(%rax)
    180004a32:	add    %al,(%rax)
-   180004a34:	xchg   %eax,%edx
-   180004a35:	int    $0x27
-   180004a37:	data16 add %al,(%rax)
-   180004a3a:	add    %al,(%rax)
-   180004a3c:	or     $0xe0000000,%eax
+   180004a34:	adc    $0x66291f,%eax
+   180004a39:	add    %al,(%rax)
+   180004a3b:	add    %cl,-0x20000000(%rip)        # 0x160004a41
    180004a41:	add    (%rax),%al
    180004a43:	add    %ah,%ah
    180004a45:	rex.WR add %r8b,(%rax)
    180004a48:	in     $0x38,%al
 	...
    180004a7e:	add    %al,(%rax)
    180004a80:	add    %eax,(%rax)
```

## ipex_llm/libs/llama.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x00000001800592b8
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Tue Apr 23 15:02:43 2024
+Time/Date		Wed Apr 24 15:02:45 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000059a00
 SizeOfInitializedData	00000000000c5e00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	00000000000592b8
@@ -119535,19 +119535,17 @@
    180062160:	enter  $0x5b6,$0x80
    180062164:	add    %eax,(%rax)
    180062166:	add    %al,(%rax)
    180062168:	shlb   $1,0x18005(%rsi)
    18006216e:	add    %al,(%rax)
    180062170:	add    %al,(%rax)
    180062172:	add    %al,(%rax)
-   180062174:	xchg   %eax,%ebx
-   180062175:	int    $0x27
-   180062177:	data16 add %al,(%rax)
-   18006217a:	add    %al,(%rax)
-   18006217c:	or     $0x50000000,%eax
+   180062174:	adc    $0x66291f,%eax
+   180062179:	add    %al,(%rax)
+   18006217b:	add    %cl,0x50000000(%rip)        # 0x1d0062181
    180062181:	add    (%rax),%eax
    180062183:	add    %al,(%rax)
    180062185:	cs (bad)
    180062187:	add    %al,(%rax)
    180062189:	sbb    $0x6,%al
 	...
    1800621ff:	add    %dh,0x31(%rax)
```

## ipex_llm/libs/main-bloom.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x000000014001045c
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Tue Apr 23 15:02:42 2024
+Time/Date		Wed Apr 24 15:02:45 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000010800
 SizeOfInitializedData	0000000000008e00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000001045c
@@ -25509,19 +25509,17 @@
    140014ab0:	enter  $0x125,$0x40
    140014ab4:	add    %eax,(%rax)
    140014ab6:	add    %al,(%rax)
    140014ab8:	shlb   $1,0x14001(%rip)        # 0x140028abf
    140014abe:	add    %al,(%rax)
    140014ac0:	add    %al,(%rax)
    140014ac2:	add    %al,(%rax)
-   140014ac4:	xchg   %eax,%edx
-   140014ac5:	int    $0x27
-   140014ac7:	data16 add %al,(%rax)
-   140014aca:	add    %al,(%rax)
-   140014acc:	or     $0x20000000,%eax
+   140014ac4:	adc    $0x66291f,%eax
+   140014ac9:	add    %al,(%rax)
+   140014acb:	add    %cl,0x20000000(%rip)        # 0x160014ad1
    140014ad1:	add    (%rax),%eax
    140014ad3:	add    %cl,%ah
    140014ad5:	push   %rsp
    140014ad6:	add    %eax,(%rax)
    140014ad8:	int3
    140014ad9:	rex add %eax,(%rax)
 	...
```

## ipex_llm/libs/main-chatglm_vnni.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x00000001400836cc
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Tue Apr 23 15:05:10 2024
+Time/Date		Wed Apr 24 15:04:19 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000087c00
 SizeOfInitializedData	00000000000cbe00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	00000000000836cc
@@ -189024,20 +189024,18 @@
    140093ea5:	add    %al,(%rax)
    140093ea7:	add    %al,(%rax)
    140093ea9:	cltd
    140093eaa:	or     %al,0x1(%rax)
    140093ead:	add    %al,(%rax)
    140093eaf:	add    %al,(%rax)
    140093eb1:	add    %al,(%rax)
-   140093eb3:	add    %ah,(%rsi)
-   140093eb5:	(bad)
-   140093eb6:	(bad)
-   140093eb7:	data16 add %al,(%rax)
-   140093eba:	add    %al,(%rax)
-   140093ebc:	or     $0xcc000000,%eax
+   140093eb3:	add    %dh,0x1f(%rbx)
+   140093eb6:	sub    %esp,0x0(%rsi)
+   140093eb9:	add    %al,(%rax)
+   140093ebb:	add    %cl,-0x34000000(%rip)        # 0x10c093ec1
    140093ec1:	add    (%rax),%eax
    140093ec3:	add    %dl,(%rax)
    140093ec5:	jae    0x140093ed0
    140093ec7:	add    %dl,(%rax)
    140093ec9:	movsxd (%rcx),%ecx
 	...
    140093eff:	add    %al,(%rax)
```

## ipex_llm/libs/main-gptneox.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x000000014000ef6c
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Tue Apr 23 15:02:42 2024
+Time/Date		Wed Apr 24 15:02:45 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		000000000000f200
 SizeOfInitializedData	0000000000009400
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000000ef6c
@@ -24136,19 +24136,17 @@
    140013edf:	add    %ch,%al
    140013ee1:	adc    $0x14001,%eax
    140013ee6:	add    %al,(%rax)
    140013ee8:	lock adc $0x14001,%eax
    140013eee:	add    %al,(%rax)
    140013ef0:	add    %al,(%rax)
    140013ef2:	add    %al,(%rax)
-   140013ef4:	xchg   %eax,%edx
-   140013ef5:	int    $0x27
-   140013ef7:	data16 add %al,(%rax)
-   140013efa:	add    %al,(%rax)
-   140013efc:	or     $0x90000000,%eax
+   140013ef4:	adc    $0x66291f,%eax
+   140013ef9:	add    %al,(%rax)
+   140013efb:	add    %cl,-0x70000000(%rip)        # 0xd0013f01
    140013f01:	add    (%rax),%eax
    140013f03:	add    %ch,0x1(%rcx,%rcx,2)
    140013f07:	add    %ch,0x1(%rdi,%rbp,1)
 	...
    140013f7f:	add    %ah,(%rax)
    140013f81:	add    %r8,0x1(%r8)
    140013f85:	add    %al,(%rax)
```

## ipex_llm/libs/main-llama.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x000000014000f32c
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Tue Apr 23 15:02:42 2024
+Time/Date		Wed Apr 24 15:02:45 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		000000000000f600
 SizeOfInitializedData	0000000000009400
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000000f32c
@@ -24679,19 +24679,17 @@
    140013faf:	add    %ch,%al
    140013fb1:	adc    $0x14001,%eax
    140013fb6:	add    %al,(%rax)
    140013fb8:	lock adc $0x14001,%eax
    140013fbe:	add    %al,(%rax)
    140013fc0:	add    %al,(%rax)
    140013fc2:	add    %al,(%rax)
-   140013fc4:	xchg   %eax,%edx
-   140013fc5:	int    $0x27
-   140013fc7:	data16 add %al,(%rax)
-   140013fca:	add    %al,(%rax)
-   140013fcc:	or     $0x90000000,%eax
+   140013fc4:	adc    $0x66291f,%eax
+   140013fc9:	add    %al,(%rax)
+   140013fcb:	add    %cl,-0x70000000(%rip)        # 0xd0013fd1
    140013fd1:	add    (%rax),%eax
    140013fd3:	add    %ch,%ah
    140013fd5:	add    %rax,(%r8)
    140013fd8:	in     (%dx),%al
    140013fd9:	xor    (%rcx),%eax
 	...
    140013fff:	add    %ah,0x140014d(%rax)
```

## ipex_llm/libs/main-starcoder.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x000000014001a85c
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Tue Apr 23 15:02:42 2024
+Time/Date		Wed Apr 24 15:02:45 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		000000000001b000
 SizeOfInitializedData	000000000000bc00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000001a85c
@@ -40341,15 +40341,15 @@
    14001f111:	movb   $0x40,(%rcx)
    14001f114:	add    %eax,(%rax)
    14001f116:	add    %al,(%rax)
    14001f118:	push   $0x14001c6
    14001f11d:	add    %al,(%rax)
    14001f11f:	add    %al,(%rax)
    14001f121:	add    %al,(%rax)
-   14001f123:	add    %dl,0x6627cd(%rdx)
+   14001f123:	add    %dl,0x66291f(%rip)        # 0x140681a48
    14001f129:	add    %al,(%rax)
    14001f12b:	add    %cl,0x20000000(%rip)        # 0x16001f131
    14001f131:	add    (%rax),%eax
    14001f133:	add    %dl,(%rbx,%rax,1)
    14001f136:	add    (%rax),%al
    14001f138:	adc    $0xf7,%al
    14001f13a:	add    %eax,(%rax)
```

## ipex_llm/libs/quantize-bloom.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x0000000140013918
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Tue Apr 23 15:02:42 2024
+Time/Date		Wed Apr 24 15:02:45 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000013a00
 SizeOfInitializedData	00000000000acc00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000013918
@@ -32227,15 +32227,15 @@
    1400191a5:	add    %al,(%rax)
    1400191a7:	add    %al,(%rax)
    1400191a9:	push   %rbp
    1400191aa:	add    %eax,0x1(%rax)
    1400191ad:	add    %al,(%rax)
    1400191af:	add    %al,(%rax)
    1400191b1:	add    %al,(%rax)
-   1400191b3:	add    %dl,0x6627cd(%rdx)
+   1400191b3:	add    %dl,0x66291f(%rip)        # 0x14067bad8
    1400191b9:	add    %al,(%rax)
    1400191bb:	add    %cl,0x20000000(%rip)        # 0x1600191c1
    1400191c1:	add    (%rax),%eax
    1400191c3:	add    %dh,-0x5f(%rax)
    1400191c6:	add    %eax,(%rax)
    1400191c8:	jo     0x140019159
    1400191ca:	add    %eax,(%rax)
```

## ipex_llm/libs/quantize-bloom_vnni.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x0000000140013b28
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Tue Apr 23 15:04:44 2024
+Time/Date		Wed Apr 24 15:03:52 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000013c00
 SizeOfInitializedData	00000000000ad000
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000013b28
@@ -32344,19 +32344,18 @@
    140019185:	add    %al,(%rax)
    140019187:	add    %al,(%rax)
    140019189:	push   %rbp
    14001918a:	add    %eax,0x1(%rax)
    14001918d:	add    %al,(%rax)
    14001918f:	add    %al,(%rax)
    140019191:	add    %al,(%rax)
-   140019193:	add    %cl,(%rsi,%rcx,8)
-   140019196:	(bad)
-   140019197:	data16 add %al,(%rax)
-   14001919a:	add    %al,(%rax)
-   14001919c:	or     $0x20000000,%eax
+   140019193:	add    %bl,0x1f(%rax)
+   140019196:	sub    %esp,0x0(%rsi)
+   140019199:	add    %al,(%rax)
+   14001919b:	add    %cl,0x20000000(%rip)        # 0x1600191a1
    1400191a1:	add    (%rax),%eax
    1400191a3:	add    %dh,-0x5f(%rax)
    1400191a6:	add    %eax,(%rax)
    1400191a8:	jo     0x14001913b
    1400191aa:	add    %eax,(%rax)
 	...
    140019200:	add    %eax,(%rax)
```

## ipex_llm/libs/quantize-gptneox.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x0000000140010988
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Tue Apr 23 15:02:41 2024
+Time/Date		Wed Apr 24 15:02:44 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000010a00
 SizeOfInitializedData	00000000000aa600
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000010988
@@ -27188,15 +27188,16 @@
    140015f80:	push   $0x1400123
    140015f85:	add    %al,(%rax)
    140015f87:	add    %dh,0x23(%rax)
    140015f8a:	add    %eax,0x1(%rax)
    140015f8d:	add    %al,(%rax)
    140015f8f:	add    %al,(%rax)
    140015f91:	add    %al,(%rax)
-   140015f93:	add    %dl,0x6627cd(%rcx)
+   140015f93:	add    %dl,(%rdi,%rbx,1)
+   140015f96:	sub    %esp,0x0(%rsi)
    140015f99:	add    %al,(%rax)
    140015f9b:	add    %cl,-0x70000000(%rip)        # 0xd0015fa1
    140015fa1:	add    (%rax),%eax
    140015fa3:	add    %ch,0x65(%rax)
    140015fa6:	add    %eax,(%rax)
    140015fa8:	push   $0x153
 	...
```

## ipex_llm/libs/quantize-gptneox_vnni.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x0000000140010b98
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Tue Apr 23 15:04:43 2024
+Time/Date		Wed Apr 24 15:03:51 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000010c00
 SizeOfInitializedData	00000000000aa600
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000010b98
@@ -27296,20 +27296,18 @@
    140015f60:	push   $0x1400123
    140015f65:	add    %al,(%rax)
    140015f67:	add    %dh,0x23(%rax)
    140015f6a:	add    %eax,0x1(%rax)
    140015f6d:	add    %al,(%rax)
    140015f6f:	add    %al,(%rax)
    140015f71:	add    %al,(%rax)
-   140015f73:	add    %cl,(%rbx)
-   140015f75:	(bad)
-   140015f76:	(bad)
-   140015f77:	data16 add %al,(%rax)
-   140015f7a:	add    %al,(%rax)
-   140015f7c:	or     $0x90000000,%eax
+   140015f73:	add    %dl,0x1f(%rdi)
+   140015f76:	sub    %esp,0x0(%rsi)
+   140015f79:	add    %al,(%rax)
+   140015f7b:	add    %cl,-0x70000000(%rip)        # 0xd0015f81
    140015f81:	add    (%rax),%eax
    140015f83:	add    %ch,0x65(%rax)
    140015f86:	add    %eax,(%rax)
    140015f88:	push   $0x155
 	...
    140015ffd:	add    %al,(%rax)
    140015fff:	add    %bl,(%rax)
```

## ipex_llm/libs/quantize-llama.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x00000001400118e8
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Tue Apr 23 15:02:41 2024
+Time/Date		Wed Apr 24 15:02:44 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000011800
 SizeOfInitializedData	00000000000aac00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	00000000000118e8
@@ -28454,15 +28454,16 @@
    14001706d:	add    %al,(%rax)
    14001706f:	add    %cl,0x1400133(%rax)
    140017075:	add    %al,(%rax)
    140017077:	add    %dl,0x1400133(%rax)
    14001707d:	add    %al,(%rax)
    14001707f:	add    %al,(%rax)
    140017081:	add    %al,(%rax)
-   140017083:	add    %dl,0x6627cd(%rcx)
+   140017083:	add    %dl,(%rdi,%rbx,1)
+   140017086:	sub    %esp,0x0(%rsi)
    140017089:	add    %al,(%rax)
    14001708b:	add    %cl,-0x70000000(%rip)        # 0xd0017091
    140017091:	add    (%rax),%eax
    140017093:	add    %ch,0x1(%rsi,%rsi,2)
    140017097:	add    %ch,0x1(%rdx,%riz,2)
 	...
    1400170ff:	add    %ah,(%rax)
```

## ipex_llm/libs/quantize-llama_vnni.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x0000000140011af8
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Tue Apr 23 15:04:43 2024
+Time/Date		Wed Apr 24 15:03:51 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000011c00
 SizeOfInitializedData	00000000000aac00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000011af8
@@ -28600,20 +28600,18 @@
    14001704d:	add    %al,(%rax)
    14001704f:	add    %cl,0x1400133(%rax)
    140017055:	add    %al,(%rax)
    140017057:	add    %dl,0x1400133(%rax)
    14001705d:	add    %al,(%rax)
    14001705f:	add    %al,(%rax)
    140017061:	add    %al,(%rax)
-   140017063:	add    %cl,(%rbx)
-   140017065:	(bad)
-   140017066:	(bad)
-   140017067:	data16 add %al,(%rax)
-   14001706a:	add    %al,(%rax)
-   14001706c:	or     $0x90000000,%eax
+   140017063:	add    %dl,0x1f(%rdi)
+   140017066:	sub    %esp,0x0(%rsi)
+   140017069:	add    %al,(%rax)
+   14001706b:	add    %cl,-0x70000000(%rip)        # 0xd0017071
    140017071:	add    (%rax),%eax
    140017073:	add    %ch,%ah
    140017075:	jne    0x140017078
    140017077:	add    %ch,%ah
    140017079:	add    %eax,%gs:(%rax)
    14001707c:	add    %al,(%rax)
    14001707e:	add    %al,(%rax)
```

## ipex_llm/libs/quantize-starcoder.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x0000000140013c70
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Tue Apr 23 15:02:42 2024
+Time/Date		Wed Apr 24 15:02:45 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000013c00
 SizeOfInitializedData	00000000000ace00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000013c70
@@ -32545,15 +32545,15 @@
    1400192a5:	add    %al,(%rax)
    1400192a7:	add    %al,(%rax)
    1400192a9:	push   %rbp
    1400192aa:	add    %eax,0x1(%rax)
    1400192ad:	add    %al,(%rax)
    1400192af:	add    %al,(%rax)
    1400192b1:	add    %al,(%rax)
-   1400192b3:	add    %dl,0x6627cd(%rdx)
+   1400192b3:	add    %dl,0x66291f(%rip)        # 0x14067bbd8
    1400192b9:	add    %al,(%rax)
    1400192bb:	add    %cl,0x20000000(%rip)        # 0x1600192c1
    1400192c1:	add    (%rax),%eax
    1400192c3:	add    %bh,0x1(%rdx,%riz,4)
    1400192c7:	add    %bh,0x1(%rdx,%rdx,4)
 	...
    1400192ff:	add    %al,(%rcx)
```

## ipex_llm/libs/quantize-starcoder_vnni.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x0000000140013e80
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Tue Apr 23 15:04:44 2024
+Time/Date		Wed Apr 24 15:03:51 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000013e00
 SizeOfInitializedData	00000000000ad000
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000013e80
@@ -32652,19 +32652,18 @@
    140019285:	add    %al,(%rax)
    140019287:	add    %al,(%rax)
    140019289:	push   %rbp
    14001928a:	add    %eax,0x1(%rax)
    14001928d:	add    %al,(%rax)
    14001928f:	add    %al,(%rax)
    140019291:	add    %al,(%rax)
-   140019293:	add    %cl,(%rsi,%rcx,8)
-   140019296:	(bad)
-   140019297:	data16 add %al,(%rax)
-   14001929a:	add    %al,(%rax)
-   14001929c:	or     $0x20000000,%eax
+   140019293:	add    %dl,0x1f(%rdi)
+   140019296:	sub    %esp,0x0(%rsi)
+   140019299:	add    %al,(%rax)
+   14001929b:	add    %cl,0x20000000(%rip)        # 0x1600192a1
    1400192a1:	add    (%rax),%eax
    1400192a3:	add    %bh,0x1(%rdx,%riz,4)
    1400192a7:	add    %bh,0x1(%rsp,%rdx,4)
 	...
    1400192ff:	add    %al,(%rcx)
 	...
    140019309:	add    %al,(%rax)
```

## ipex_llm/libs/starcoder-api.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x000000018000277c
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Tue Apr 23 15:02:42 2024
+Time/Date		Wed Apr 24 15:02:45 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000002200
 SizeOfInitializedData	0000000000003400
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000000277c
@@ -4028,19 +4028,17 @@
    1800045f0:	cmp    %al,0x0(%rdx)
    1800045f3:	addb   $0x0,(%rcx)
    1800045f6:	add    %al,(%rax)
    1800045f8:	rex
    1800045f9:	rex.X add %al,0x1(%rax)
    180004600:	add    %al,(%rax)
    180004602:	add    %al,(%rax)
-   180004604:	xchg   %eax,%edx
-   180004605:	int    $0x27
-   180004607:	data16 add %al,(%rax)
-   18000460a:	add    %al,(%rax)
-   18000460c:	or     $0xe0000000,%eax
+   180004604:	adc    $0x66291f,%eax
+   180004609:	add    %al,(%rax)
+   18000460b:	add    %cl,-0x20000000(%rip)        # 0x160004611
    180004611:	add    (%rax),%al
    180004613:	add    %ah,%ah
    180004615:	rex.W add %al,(%rax)
    180004618:	in     $0x2e,%al
 	...
    18000467e:	add    %al,(%rax)
    180004680:	add    %eax,(%rax)
```

## ipex_llm/libs/starcoder.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x00000001800607a8
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Tue Apr 23 15:02:42 2024
+Time/Date		Wed Apr 24 15:02:45 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000060e00
 SizeOfInitializedData	00000000000c7a00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	00000000000607a8
@@ -129991,19 +129991,17 @@
    180069cd5:	add    %al,(%rax)
    180069cd7:	add    %al,%al
    180069cd9:	es (bad)
    180069cdb:	addb   $0x0,(%rcx)
    180069cde:	add    %al,(%rax)
    180069ce0:	add    %al,(%rax)
    180069ce2:	add    %al,(%rax)
-   180069ce4:	xchg   %eax,%edx
-   180069ce5:	int    $0x27
-   180069ce7:	data16 add %al,(%rax)
-   180069cea:	add    %al,(%rax)
-   180069cec:	or     $0x50000000,%eax
+   180069ce4:	adc    $0x66291f,%eax
+   180069ce9:	add    %al,(%rax)
+   180069ceb:	add    %cl,0x50000000(%rip)        # 0x1d0069cf1
    180069cf1:	add    (%rax),%eax
    180069cf3:	add    %dl,-0x52(%rax)
    180069cf6:	(bad)
    180069cf7:	add    %dl,-0x60(%rax)
    180069cfa:	(bad)
    180069cfb:	add    %al,(%rax)
    180069cfd:	add    %al,(%rax)
```

## ipex_llm/transformers/convert.py

```diff
@@ -649,14 +649,17 @@
     # for starcoder2
     if model.config.model_type == "starcoder2":
         from ipex_llm.transformers.models.starcoder2 import merge_qkv
         model.apply(merge_qkv)
     if model.config.model_type == "phi":
         from ipex_llm.transformers.models.phi import merge_qkv
         model.apply(merge_qkv)
+    if model.config.model_type == "phi3":
+        from ipex_llm.transformers.models.phi3 import split_mlp
+        model.apply(split_mlp)
     if model.config.model_type == "qwen":
         rope_base = model.config.rotary_emb_base
         from accelerate.big_modeling import init_empty_weights
 
         def split_qkv_proj_func(module):
             if "QWenAttention" in module.__class__.__name__:
                 c_attn_weight = module.c_attn.weight.data
@@ -1422,14 +1425,25 @@
         # for phi-2
         modeling_module_name = model.__class__.__module__
         module = importlib.import_module(modeling_module_name)
         from ipex_llm.transformers.models.phi import attention_forward
         from ipex_llm.transformers.models.phi import model_forward
         convert_forward(model, module.PhiAttention, attention_forward)
         convert_forward(model, module.PhiModel, model_forward)
+    elif model.config.model_type == "phi3":
+        # for phi-3
+        modeling_module_name = model.__class__.__module__
+        module = importlib.import_module(modeling_module_name)
+        from ipex_llm.transformers.models.phi3 import attention_forward
+        convert_forward(model, module.Phi3Attention, attention_forward)
+        from ipex_llm.transformers.models.phi3 import mlp_forward
+        convert_forward(model, module.Phi3MLP, mlp_forward)
+        from ipex_llm.transformers.models.phi3 import model_forward_wrapper
+        model_forward = model_forward_wrapper(module.Phi3Model.forward)
+        convert_forward(model, module.Phi3Model, model_forward)
     elif model.config.model_type == 'yuan':
         modeling_module_name = model.__class__.__module__
         module = importlib.import_module(modeling_module_name)
         from ipex_llm.transformers.models.yuan import yuan_attention_forward
         # from ipex_llm.transformers.models.yuan import yuan_mlp_forward
         convert_forward(model,
                         module.YuanAttention,
```

## ipex_llm/transformers/models/llama.py

```diff
@@ -42,15 +42,16 @@
 from ipex_llm.transformers.models.utils import init_kv_cache, extend_kv_cache, append_kv_cache
 from ipex_llm.transformers.models.utils import SILU
 from ipex_llm.transformers.models.utils import init_fp8_kv_cache, append_fp8_kv_cache, \
     restore_fp8_kv_cache, use_quantize_kv_cache
 from ipex_llm.transformers.models.utils import is_enough_kv_cache_room_4_31, \
     apply_rotary_pos_emb, is_enough_kv_cache_room_4_36
 from ipex_llm.transformers.models.utils import apply_rotary_pos_emb_no_cache_xpu
-from ipex_llm.transformers.models.utils import use_flash_attention, use_esimd_sdp
+from ipex_llm.transformers.models.utils import use_flash_attention, use_new_esimd_sdp_fp16, \
+    use_sdp_fp8
 from ipex_llm.transformers.models.utils import mlp_fusion_check, fp16_fusion_check
 from ipex_llm.transformers.models.utils import use_decoding_fast_path
 from transformers.modeling_outputs import BaseModelOutputWithPast
 from transformers.models.llama.modeling_llama import LlamaModel
 from ipex_llm.transformers.low_bit_linear import SYM_INT4, FP8E5, IQ2_XXS, FP4
 from ipex_llm.ggml.quantize import ggml_tensor_qtype
 from ipex_llm.utils.common import invalidInputError
@@ -445,15 +446,15 @@
     else:
         k_cache, v_cache = past_key_value
         key_states, value_states = append_fp8_kv_cache(k_cache, v_cache,
                                                        key_states, value_states, new_layout=True)
         kv_seq_len = key_states.shape[-2]
         past_key_value = (key_states, value_states)
 
-        if query_states.size(2) != 1 or query_states.device.type != 'xpu':
+        if not use_sdp_fp8(q_len, key_states.shape[2], query_states):
             key_states, value_states = restore_fp8_kv_cache(key_states, value_states,
                                                             query_states.dtype)
             # repeat k/v heads if n_kv_heads < n_heads
             key_states = repeat_kv(key_states, self.num_key_value_groups)
             value_states = repeat_kv(value_states, self.num_key_value_groups)
             attn_output, attn_weights = native_sdp(query_states, key_states, value_states,
                                                    attention_mask,
@@ -662,15 +663,15 @@
         value_states = repeat_kv(value_states, self.num_key_value_groups)
         attn_output = F.scaled_dot_product_attention(query_states.to(device, dtype=torch.float16),
                                                      key_states.to(device, dtype=torch.float16),
                                                      value_states.to(device, dtype=torch.float16),
                                                      is_causal=True)
         attn_weights = None
     elif not self.training and not hidden_states.requires_grad and \
-            use_esimd_sdp(q_len, key_states.shape[2], self.head_dim, query_states, attention_mask):
+            use_new_esimd_sdp_fp16(q_len, key_states.shape[2], self.head_dim, query_states):
         import linear_q4_0
         attn_output = linear_q4_0.sdp_fp16(query_states, key_states, value_states, attention_mask)
         attn_output = attn_output.view(query_states.shape)
         attn_weights = None
     else:
         # repeat k/v heads if n_kv_heads < n_heads
         key_states = repeat_kv(key_states, self.num_key_value_groups)
@@ -1070,15 +1071,15 @@
                                                              new_layout=True)
     else:
         cache_kwargs = None  # Specific to RoPE models
         key_states, value_states = past_key_value.update(key_states, value_states,
                                                          self.layer_idx, cache_kwargs,
                                                          new_layout=True)
         kv_seq_len = key_states.shape[-2]
-        if query_states.size(2) != 1 or query_states.device.type != 'xpu':
+        if not use_sdp_fp8(q_len, key_states.shape[2], query_states):
             key_states, value_states = restore_fp8_kv_cache(key_states, value_states,
                                                             query_states.dtype)
             key_states = repeat_kv(key_states, self.num_key_value_groups)\
                 .to(device, dtype=query_states.dtype)
             value_states = repeat_kv(value_states, self.num_key_value_groups)\
                 .to(device, dtype=query_states.dtype)
             attn_weights = torch.matmul(query_states, key_states.transpose(2, 3))
@@ -1338,15 +1339,15 @@
         # now only use flash attention for first token
         attn_output = F.scaled_dot_product_attention(query_states.to(device, dtype=torch.float16),
                                                      key_states.to(device, dtype=torch.float16),
                                                      value_states.to(device, dtype=torch.float16),
                                                      is_causal=True)
         attn_weights = None
     elif not self.training and not hidden_states.requires_grad and \
-            use_esimd_sdp(q_len, key_states.shape[2], self.head_dim, query_states):
+            use_new_esimd_sdp_fp16(q_len, key_states.shape[2], self.head_dim, query_states):
         import linear_q4_0
         attn_output = linear_q4_0.sdp_fp16(query_states, key_states, value_states, attention_mask)
         attn_output = attn_output.view(query_states.shape)
         attn_weights = None
     else:
         # repeat k/v heads if n_kv_heads < n_heads
         key_states = repeat_kv(key_states, self.num_key_value_groups)
```

## ipex_llm/transformers/models/mistral.py

```diff
@@ -48,15 +48,16 @@
 from ipex_llm.transformers.models.utils import init_fp8_kv_cache, append_fp8_kv_cache, \
     restore_fp8_kv_cache, use_quantize_kv_cache
 from ipex_llm.transformers.models.utils import apply_rotary_pos_emb, \
     apply_rotary_pos_emb_no_cache_xpu
 from ipex_llm.transformers.models.utils import is_enough_kv_cache_room_4_31, \
     is_enough_kv_cache_room_4_36
 from ipex_llm.transformers.low_bit_linear import SYM_INT4, FP8E5, IQ2_XXS
-from ipex_llm.transformers.models.utils import use_flash_attention, use_esimd_sdp
+from ipex_llm.transformers.models.utils import use_flash_attention, use_new_esimd_sdp_fp16, \
+    use_sdp_fp8
 from ipex_llm.transformers.models.utils import use_decoding_fast_path
 from ipex_llm.transformers.models.llama import llama_decoding_fast_path_qtype_check
 from ipex_llm.transformers.models.llama import should_use_xetla_mm_qkv
 from ipex_llm.transformers.models.llama import fuse_qkv_weight_xetla
 try:
     from transformers.cache_utils import Cache
 except ImportError:
@@ -306,15 +307,15 @@
     else:
         k_cache, v_cache = past_key_value
         key_states, value_states = append_fp8_kv_cache(k_cache, v_cache,
                                                        key_states, value_states, new_layout=True)
         kv_seq_len = key_states.shape[-2]
         past_key_value = (key_states, value_states)
 
-        if query_states.size(2) != 1 or query_states.device.type != 'xpu':
+        if not use_sdp_fp8(q_len, key_states.shape[2], query_states):
             key_states, value_states = restore_fp8_kv_cache(key_states, value_states,
                                                             query_states.dtype)
             attn_weights = torch.matmul(query_states, key_states.transpose(2, 3))
 
             attn_weights = attn_weights / math.sqrt(self.head_dim)
 
             if attn_weights.size() != (bsz, self.num_heads, q_len, kv_seq_len):
@@ -499,15 +500,15 @@
         attn_output = F.scaled_dot_product_attention(query_states.to(dtype=attention_dtype),
                                                      key_states,
                                                      value_states,
                                                      is_causal=True)
         attn_weights = None
         attn_output = attn_output.transpose(1, 2).contiguous()
         attn_output = attn_output.reshape(bsz, q_len, self.hidden_size)
-    elif use_esimd_sdp(q_len, key_states.shape[2], self.head_dim, query_states):
+    elif use_new_esimd_sdp_fp16(q_len, key_states.shape[2], self.head_dim, query_states):
         # new fp16 sdp doesn't require repeat_kv
         import linear_q4_0
         attn_output = linear_q4_0.sdp_fp16(query_states, key_states, value_states, attention_mask)
         attn_output = attn_output.view(query_states.shape)
         attn_weights = None
         attn_output = attn_output.transpose(1, 2).contiguous()
         attn_output = attn_output.reshape(bsz, q_len, self.hidden_size)
@@ -683,15 +684,15 @@
                                                              new_layout=True)
     else:
         cache_kwargs = None  # Specific to RoPE models
         key_states, value_states = past_key_value.update(key_states, value_states,
                                                          self.layer_idx, cache_kwargs,
                                                          new_layout=True)
         kv_seq_len = key_states.shape[-2]
-        if query_states.size(2) != 1 or query_states.device.type != 'xpu':
+        if not use_sdp_fp8(q_len, key_states.shape[2], query_states):
             key_states, value_states = restore_fp8_kv_cache(key_states, value_states,
                                                             query_states.dtype)
             attn_weights = torch.matmul(query_states, key_states.transpose(2, 3))
 
             attn_weights = attn_weights / math.sqrt(self.head_dim)
 
             if attn_weights.size() != (bsz, self.num_heads, q_len, kv_seq_len):
@@ -892,15 +893,15 @@
         attn_output = F.scaled_dot_product_attention(query_states.to(dtype=attention_dtype),
                                                      key_states,
                                                      value_states,
                                                      is_causal=True)
         attn_weights = None
         attn_output = attn_output.transpose(1, 2).contiguous()
         attn_output = attn_output.reshape(bsz, q_len, self.hidden_size)
-    elif use_esimd_sdp(q_len, key_states.shape[2], self.head_dim, query_states):
+    elif use_new_esimd_sdp_fp16(q_len, key_states.shape[2], self.head_dim, query_states):
         # new fp16 sdp doesn't require repeat_kv
         import linear_q4_0
         attn_output = linear_q4_0.sdp_fp16(query_states, key_states, value_states, attention_mask)
         attn_output = attn_output.view(query_states.shape)
         attn_weights = None
         attn_output = attn_output.transpose(1, 2).contiguous()
         attn_output = attn_output.reshape(bsz, q_len, self.hidden_size)
```

## ipex_llm/transformers/models/qwen2_moe.py

```diff
@@ -57,14 +57,28 @@
 from ipex_llm.transformers.models.utils import use_quantize_kv_cache, restore_fp8_kv_cache
 from ipex_llm.transformers.kv import DynamicFp8Cache
 
 import os
 
 KV_CACHE_ALLOC_BLOCK_LENGTH = int(os.environ.get("KV_CACHE_ALLOC_BLOCK_LENGTH", 256))
 
+from transformers.models.qwen2.modeling_qwen2 import _prepare_4d_causal_attention_mask_for_sdpa
+from transformers.models.qwen2.modeling_qwen2 import _prepare_4d_causal_attention_mask
+from transformers.modeling_outputs import MoeModelOutputWithPast
+
+try:
+    from transformers.cache_utils import Cache, DynamicCache
+except ImportError:
+    Cache = Tuple[torch.Tensor]
+import logging
+from transformers import logging
+
+
+logger = logging.get_logger(__name__)
+
 
 def qwen2moe_model_forward(
     self,
     input_ids: torch.LongTensor = None,
     attention_mask: Optional[torch.Tensor] = None,
     position_ids: Optional[torch.LongTensor] = None,
     past_key_values: Optional[List[torch.FloatTensor]] = None,
@@ -75,29 +89,211 @@
     output_router_logits: Optional[bool] = None,
     return_dict: Optional[bool] = None,
 ):
     use_cache = use_cache if use_cache is not None else self.config.use_cache
     if use_cache and use_quantize_kv_cache(self.layers[0].mlp.shared_expert.up_proj, input_ids):
         if not isinstance(past_key_values, DynamicFp8Cache):
             past_key_values = DynamicFp8Cache.from_legacy_cache(past_key_values)
-    return Qwen2MoeModel.forward(
+    return qwen2_moe_model_forward_internal(
         self=self,
         input_ids=input_ids,
         attention_mask=attention_mask,
         position_ids=position_ids,
         past_key_values=past_key_values,
         inputs_embeds=inputs_embeds,
         use_cache=use_cache,
         output_attentions=output_attentions,
         output_hidden_states=output_hidden_states,
         output_router_logits=output_router_logits,
         return_dict=return_dict,
     )
 
 
+def qwen2_moe_model_forward_internal(
+        self,
+        input_ids: torch.LongTensor = None,
+        attention_mask: Optional[torch.Tensor] = None,
+        position_ids: Optional[torch.LongTensor] = None,
+        past_key_values: Optional[List[torch.FloatTensor]] = None,
+        inputs_embeds: Optional[torch.FloatTensor] = None,
+        use_cache: Optional[bool] = None,
+        output_attentions: Optional[bool] = None,
+        output_hidden_states: Optional[bool] = None,
+        output_router_logits: Optional[bool] = None,
+        return_dict: Optional[bool] = None,
+) -> Union[Tuple, MoeModelOutputWithPast]:
+        output_attentions = output_attentions if output_attentions is not None \
+            else self.config.output_attentions
+        output_router_logits = (
+            output_router_logits if output_router_logits is not None else
+            self.config.output_router_logits
+        )
+        output_hidden_states = (
+            output_hidden_states if output_hidden_states is not None else
+            self.config.output_hidden_states
+        )
+        use_cache = use_cache if use_cache is not None else self.config.use_cache
+
+        return_dict = return_dict if return_dict is not None else self.config.use_return_dict
+
+        # retrieve input_ids and inputs_embeds
+        if input_ids is not None and inputs_embeds is not None:
+            invalidInputError(False, "You cannot specify both decoder_input_ids and "
+                              "decoder_inputs_embeds at the same time")
+        elif input_ids is not None:
+            batch_size, seq_length = input_ids.shape
+        elif inputs_embeds is not None:
+            batch_size, seq_length, _ = inputs_embeds.shape
+        else:
+            invalidInputError(False,
+                              "You have to specify decoder_input_ids or decoder_inputs_embeds")
+
+        if self.gradient_checkpointing and self.training:
+            if use_cache:
+                logger.warning_once(
+                    "`use_cache=True` is incompatible with gradient checkpointing."
+                    " Setting `use_cache=False`..."
+                )
+                use_cache = False
+
+        past_key_values_length = 0
+
+        if use_cache:
+            use_legacy_cache = not isinstance(past_key_values, Cache)
+            if use_legacy_cache:
+                past_key_values = DynamicCache.from_legacy_cache(past_key_values)
+            past_key_values_length = past_key_values.get_usable_length(seq_length)
+
+        if position_ids is None:
+            device = input_ids.device if input_ids is not None else inputs_embeds.device
+            position_ids = torch.arange(
+                past_key_values_length, seq_length + past_key_values_length,
+                dtype=torch.long, device=device
+            )
+            position_ids = position_ids.unsqueeze(0).view(-1, seq_length)
+        else:
+            position_ids = position_ids.view(-1, seq_length).long()
+
+        if inputs_embeds is None:
+            inputs_embeds = self.embed_tokens(input_ids)
+
+        if attention_mask is not None and self._attn_implementation == "flash_attention_2" \
+                and use_cache:
+            is_padding_right = attention_mask[:, -1].sum().item() != batch_size
+            if is_padding_right:
+                invalidInputError(
+                    False,
+                    "You are attempting to perform batched generation with padding_side='right'"
+                    " this may lead to unexpected behaviour for Flash Attention version of"
+                    " Qwen2MoE. Make sure to call `tokenizer.padding_side='left'`"
+                    " before tokenizing the input."
+                )
+
+        if self._attn_implementation == "flash_attention_2":
+            # 2d mask is passed through the layers
+            attention_mask = attention_mask if (attention_mask is not None and
+                                                0 in attention_mask) else None
+        elif self._attn_implementation == "sdpa" and not output_attentions:
+            # output_attentions=True can not be supported when using SDPA, and we fall back on
+            # the manual implementation that requires a 4D causal mask in all cases.
+            attention_mask = _prepare_4d_causal_attention_mask_for_sdpa(
+                attention_mask,
+                (batch_size, seq_length),
+                inputs_embeds,
+                past_key_values_length,
+                sliding_window=self.config.sliding_window,
+            )
+        else:
+            # 4d mask is passed through the layers
+            attention_mask = _prepare_4d_causal_attention_mask(
+                attention_mask,
+                (batch_size, seq_length),
+                inputs_embeds,
+                past_key_values_length,
+                sliding_window=self.config.sliding_window,
+            )
+
+        hidden_states = inputs_embeds
+
+        # decoder layers
+        all_hidden_states = () if output_hidden_states else None
+        all_self_attns = () if output_attentions else None
+        all_router_logits = () if output_router_logits else None
+        next_decoder_cache = None
+
+        for decoder_layer in self.layers:
+            if output_hidden_states:
+                all_hidden_states += (hidden_states,)
+
+            if self.gradient_checkpointing and self.training:
+                layer_outputs = self._gradient_checkpointing_func(
+                    decoder_layer.__call__,
+                    hidden_states,
+                    attention_mask,
+                    position_ids,
+                    past_key_values,
+                    output_attentions,
+                    output_router_logits,
+                    use_cache,
+                )
+            else:
+                # ipex-llm changes
+                curr_device = decoder_layer.input_layernorm.weight.device
+                if attention_mask is not None:
+                    attention_mask = attention_mask.to(curr_device)
+                if position_ids is not None:
+                    position_ids = position_ids.to(curr_device)
+                # ipex-llm changes end
+                layer_outputs = decoder_layer(
+                    hidden_states,
+                    attention_mask=attention_mask,
+                    position_ids=position_ids,
+                    past_key_value=past_key_values,
+                    output_attentions=output_attentions,
+                    output_router_logits=output_router_logits,
+                    use_cache=use_cache,
+                )
+
+            hidden_states = layer_outputs[0]
+
+            if use_cache:
+                next_decoder_cache = layer_outputs[2 if output_attentions else 1]
+
+            if output_attentions:
+                all_self_attns += (layer_outputs[1],)
+
+            if output_router_logits and layer_outputs[-1] is not None:
+                all_router_logits += (layer_outputs[-1],)
+
+        hidden_states = self.norm(hidden_states)
+
+        # add hidden states from the last decoder layer
+        if output_hidden_states:
+            all_hidden_states += (hidden_states,)
+
+        next_cache = None
+        if use_cache:
+            next_cache = next_decoder_cache.to_legacy_cache() if use_legacy_cache \
+                else next_decoder_cache
+
+        if not return_dict:
+            return tuple(
+                v
+                for v in [hidden_states, next_cache, all_hidden_states, all_self_attns,
+                          all_router_logits] if v is not None
+            )
+        return MoeModelOutputWithPast(
+            last_hidden_state=hidden_states,
+            past_key_values=next_cache,
+            hidden_states=all_hidden_states,
+            attentions=all_self_attns,
+            router_logits=all_router_logits,
+        )
+
+
 def qwen2moe_attention_forward(
     self,
     hidden_states: torch.Tensor,
     attention_mask: Optional[torch.Tensor] = None,
     position_ids: Optional[torch.LongTensor] = None,
     past_key_value: Optional[Tuple[torch.Tensor]] = None,
     output_attentions: bool = False,
```

## ipex_llm/transformers/models/utils.py

```diff
@@ -163,14 +163,22 @@
 def rotate_every_two(x):
     x1 = x[:, :, :, ::2]
     x2 = x[:, :, :, 1::2]
     x = torch.stack((-x2, x1), dim=-1)
     return x.flatten(-2)  # in einsum notation: rearrange(x, '... d j -> ... (d j)')
 
 
+def should_use_fuse_rope(hidden_states, position_ids, training):
+    return (
+        hidden_states.device.type == "xpu"
+        and not training and not hidden_states.requires_grad
+        and position_ids is not None
+    )
+
+
 def apply_rotary_pos_emb(q, k, cos, sin, position_ids, model_family):
     if model_family in ["llama", "baichuan", "internlm", "aquila", "gpt_neox", "mistral",
                         "mixtral", "qwen2", "yuan", "stablelm", "qwen2_moe"]:
         # The first two dimensions of cos and sin are always 1, so we can `squeeze` them.
         cos = cos.squeeze(1).squeeze(0)  # [seq_len, dim]
         sin = sin.squeeze(1).squeeze(0)  # [seq_len, dim]
         cos = cos[position_ids].unsqueeze(1)  # [bs, 1, seq_len, dim]
@@ -230,15 +238,15 @@
         cos = cos.to(q.dtype)
         sin = sin.to(q.dtype)
         cos = cos.squeeze(1).squeeze(0)  # [seq_len, dim]
         sin = sin.squeeze(1).squeeze(0)  # [seq_len, dim]
         cos = cos[position_ids].unsqueeze(1)  # [bs, 1, seq_len, dim]
         sin = sin[position_ids].unsqueeze(1)  # [bs, 1, seq_len, dim]
         linear_q4_0.apply_rotary_embedding_half_q_and_k_cache_freq(q, k, sin, cos, q_embed, k_embed)
-    elif model_family in ["gemma"]:
+    elif model_family in ["gemma", "phi3"]:
         cos = cos.unsqueeze(1)
         sin = sin.unsqueeze(1)
         linear_q4_0.apply_rotary_embedding_half_q_and_k_cache_freq(q, k, sin, cos, q_embed, k_embed)
     else:
         invalidInputError(False,
                           f"{model_family} is not supported.")
     return q_embed, k_embed
@@ -313,15 +321,15 @@
 
 
 def use_esimd_sdp(q_len, k_len, head_dim, query_states, attention_mask=None):
     if head_dim != 128:
         # esimd_sdp only support head_dim = 128 now
         return False
     elif q_len != 1:
-        # esimd_sdp only support rest token now
+        # esimd_sdp only support rest token and q_len == 1 now
         return False
     elif k_len < 8:
         # esimd_sdp will cause wrong output when k_len < 8
         return False
     elif query_states.device.type != "xpu":
         # esimd_sdp only support GPU now
         return False
@@ -351,14 +359,50 @@
         # TODO: this check needs some time
         if not torch.all(attention_mask.eq(0)):
             return False
 
     return True
 
 
+def use_new_esimd_sdp_fp16(q_len, k_len, head_dim, query_states):
+    if query_states.device.type != "xpu":
+        # esimd_sdp only support GPU now
+        return False
+    elif query_states.dtype != torch.float16:
+        # esimd_sdp only has optimization for FP16 now
+        return False
+    elif head_dim != 128 and head_dim != 64:
+        # esimd_sdp only support head_dim = 128 and 64 now
+        return False
+    elif q_len == k_len:
+        # new sdp_fp16 only support rest token now
+        return False
+    elif q_len > 32:
+        # Use new sdp_fp16 only when q_len <= 32
+        return False
+
+    device_name = torch.xpu.get_device_name(query_states.device.index)
+    if query_states.shape[0] > 1 and device_name.startswith("Intel(R) Arc(TM) A") \
+            and is_deepspeed_available:
+        # It seems there is an issue in DeepSpeed AutoTP when multi-card inference,
+        # Disable new sdp_fp16 for now
+        return False
+
+    return True
+
+
+def use_sdp_fp8(q_len, k_len, query_states):
+    if query_states.device.type != "xpu":
+        return False
+    if q_len == k_len:
+        # sdp_fp8 only support rest token now
+        return False
+    return True
+
+
 def mlp_fusion_check(x, qtype, training):
     invalidInputError(x.dim() == 2,
                       "Here input x's dim should be 2.")
     if x.shape[0] != 1:
         return False
     if x.device.type != 'xpu':
         return False
```

## Comparing `ipex_llm-2.1.0b20240423.data/scripts/llm-chat.ps1` & `ipex_llm-2.1.0b20240424.data/scripts/llm-chat.ps1`

 * *Files identical despite different names*

## Comparing `ipex_llm-2.1.0b20240423.data/scripts/llm-cli.ps1` & `ipex_llm-2.1.0b20240424.data/scripts/llm-cli.ps1`

 * *Files identical despite different names*

## Comparing `ipex_llm-2.1.0b20240423.dist-info/METADATA` & `ipex_llm-2.1.0b20240424.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipex-llm
-Version: 2.1.0b20240423
+Version: 2.1.0b20240424
 Summary: Large Language Model Develop Toolkit
 Home-page: https://github.com/intel-analytics/BigDL
 Author: BigDL Authors
 Author-email: bigdl-user-group@googlegroups.com
 License: Apache License, Version 2.0
 Platform: windows
 Classifier: License :: OSI Approved :: Apache Software License
@@ -21,15 +21,15 @@
 Requires-Dist: transformers (==4.31.0) ; extra == 'all'
 Requires-Dist: sentencepiece ; extra == 'all'
 Requires-Dist: tokenizers (==0.13.3) ; extra == 'all'
 Requires-Dist: accelerate (==0.21.0) ; extra == 'all'
 Requires-Dist: tabulate ; extra == 'all'
 Requires-Dist: intel-openmp ; (platform_machine == "x86_64" or platform_machine == "AMD64") and extra == 'all'
 Provides-Extra: cpp
-Requires-Dist: bigdl-core-cpp (==2.5.0b20240423) ; extra == 'cpp'
+Requires-Dist: bigdl-core-cpp (==2.5.0b20240424) ; extra == 'cpp'
 Provides-Extra: llama-index
 Requires-Dist: py-cpuinfo ; extra == 'llama-index'
 Requires-Dist: protobuf ; extra == 'llama-index'
 Requires-Dist: mpmath (==1.3.0) ; extra == 'llama-index'
 Requires-Dist: numpy (==1.26.4) ; extra == 'llama-index'
 Requires-Dist: sentencepiece ; extra == 'llama-index'
 Requires-Dist: accelerate (==0.21.0) ; extra == 'llama-index'
@@ -51,47 +51,47 @@
 Requires-Dist: sentencepiece ; extra == 'xpu'
 Requires-Dist: tokenizers (==0.13.3) ; extra == 'xpu'
 Requires-Dist: accelerate (==0.21.0) ; extra == 'xpu'
 Requires-Dist: tabulate ; extra == 'xpu'
 Requires-Dist: torch (==2.1.0a0) ; extra == 'xpu'
 Requires-Dist: torchvision (==0.16.0a0) ; extra == 'xpu'
 Requires-Dist: intel-extension-for-pytorch (==2.1.10+xpu) ; extra == 'xpu'
-Requires-Dist: bigdl-core-xe-21 (==2.5.0b20240423) ; extra == 'xpu'
-Requires-Dist: bigdl-core-xe-esimd-21 (==2.5.0b20240423) ; extra == 'xpu'
+Requires-Dist: bigdl-core-xe-21 (==2.5.0b20240424) ; extra == 'xpu'
+Requires-Dist: bigdl-core-xe-esimd-21 (==2.5.0b20240424) ; extra == 'xpu'
 Provides-Extra: xpu-2-0
 Requires-Dist: py-cpuinfo ; extra == 'xpu-2-0'
 Requires-Dist: protobuf ; extra == 'xpu-2-0'
 Requires-Dist: mpmath (==1.3.0) ; extra == 'xpu-2-0'
 Requires-Dist: numpy (==1.26.4) ; extra == 'xpu-2-0'
 Requires-Dist: transformers (==4.31.0) ; extra == 'xpu-2-0'
 Requires-Dist: sentencepiece ; extra == 'xpu-2-0'
 Requires-Dist: tokenizers (==0.13.3) ; extra == 'xpu-2-0'
 Requires-Dist: accelerate (==0.21.0) ; extra == 'xpu-2-0'
 Requires-Dist: tabulate ; extra == 'xpu-2-0'
 Requires-Dist: intel-openmp ; (platform_machine == "x86_64" or platform_machine == "AMD64") and extra == 'xpu-2-0'
 Requires-Dist: torch (==2.0.1a0) ; (platform_system == "Linux") and extra == 'xpu-2-0'
 Requires-Dist: torchvision (==0.15.2a0) ; (platform_system == "Linux") and extra == 'xpu-2-0'
 Requires-Dist: intel-extension-for-pytorch (==2.0.110+xpu) ; (platform_system == "Linux") and extra == 'xpu-2-0'
-Requires-Dist: bigdl-core-xe (==2.5.0b20240423) ; (platform_system == "Linux") and extra == 'xpu-2-0'
-Requires-Dist: bigdl-core-xe-esimd (==2.5.0b20240423) ; (platform_system == "Linux") and extra == 'xpu-2-0'
+Requires-Dist: bigdl-core-xe (==2.5.0b20240424) ; (platform_system == "Linux") and extra == 'xpu-2-0'
+Requires-Dist: bigdl-core-xe-esimd (==2.5.0b20240424) ; (platform_system == "Linux") and extra == 'xpu-2-0'
 Provides-Extra: xpu-2-1
 Requires-Dist: py-cpuinfo ; extra == 'xpu-2-1'
 Requires-Dist: protobuf ; extra == 'xpu-2-1'
 Requires-Dist: mpmath (==1.3.0) ; extra == 'xpu-2-1'
 Requires-Dist: numpy (==1.26.4) ; extra == 'xpu-2-1'
 Requires-Dist: transformers (==4.31.0) ; extra == 'xpu-2-1'
 Requires-Dist: sentencepiece ; extra == 'xpu-2-1'
 Requires-Dist: tokenizers (==0.13.3) ; extra == 'xpu-2-1'
 Requires-Dist: accelerate (==0.21.0) ; extra == 'xpu-2-1'
 Requires-Dist: tabulate ; extra == 'xpu-2-1'
 Requires-Dist: torch (==2.1.0a0) ; extra == 'xpu-2-1'
 Requires-Dist: torchvision (==0.16.0a0) ; extra == 'xpu-2-1'
 Requires-Dist: intel-extension-for-pytorch (==2.1.10+xpu) ; extra == 'xpu-2-1'
-Requires-Dist: bigdl-core-xe-21 (==2.5.0b20240423) ; extra == 'xpu-2-1'
-Requires-Dist: bigdl-core-xe-esimd-21 (==2.5.0b20240423) ; extra == 'xpu-2-1'
+Requires-Dist: bigdl-core-xe-21 (==2.5.0b20240424) ; extra == 'xpu-2-1'
+Requires-Dist: bigdl-core-xe-esimd-21 (==2.5.0b20240424) ; extra == 'xpu-2-1'
 Requires-Dist: intel-openmp ; (platform_machine == "x86_64" or platform_machine == "AMD64") and extra == 'xpu-2-1'
 Requires-Dist: intel-openmp ; (platform_machine == "x86_64" or platform_machine == "AMD64") and extra == 'xpu'
 
 
 IPEX LLM
```

## Comparing `ipex_llm-2.1.0b20240423.dist-info/RECORD` & `ipex_llm-2.1.0b20240424.dist-info/RECORD`

 * *Files 3% similar despite different names*

```diff
@@ -38,58 +38,58 @@
 ipex_llm/langchain/embeddings/bigdlllm.py,sha256=auNueZ-S5RQrngss_huXlYdWImX2vPYfuEVOZsx35rk,13589
 ipex_llm/langchain/embeddings/transformersembeddings.py,sha256=hBtqBfGmGg_xjb4Us7hLNfyvbLMo5mJk9a0iooOWtPM,7225
 ipex_llm/langchain/llms/__init__.py,sha256=vBCl9JF45vnk9CWBG1k8lp8J6F8OCR9UY2E-idkkm5Y,1636
 ipex_llm/langchain/llms/bigdlllm.py,sha256=FAZG6cAIJhRgbxm16gMq-cyBwLe-u165zE7yyxD7r9E,24438
 ipex_llm/langchain/llms/transformersllm.py,sha256=7eaIkJi1CbTCSgNxBCoZTe-o_5FYjD1GTYPWpn0Ccr4,10576
 ipex_llm/langchain/llms/transformerspipelinellm.py,sha256=vm522YPPwWxxAPVvQBtxRfBinC4hIbXdKW6VjHDaFXY,7379
 ipex_llm/libs/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-ipex_llm/libs/bloom-api.dll,sha256=eK0yOpMXs6TQx_DNBnd8jy9miD03Hed7qBNfyezZ1ws,36352
-ipex_llm/libs/bloom.dll,sha256=bXzOUTvrfuoEk5olYCIoqAqatFbm9aDXv2Mm_C97_1U,460288
-ipex_llm/libs/chatglm_C.cp310-win_amd64.pyd,sha256=hDbTXpKRmCA4nL2FZOKN-JCqFoxRecwS7WTpX7hqfXQ,852992
-ipex_llm/libs/chatglm_C.cp311-win_amd64.pyd,sha256=otaopmTJIKsoCDVSg2LisUNunmPUc8vVgw2T0k5Jcw0,856064
-ipex_llm/libs/chatglm_C.cp39-win_amd64.pyd,sha256=dX8I__emwV8RCv01-WzJ2pkjWdx15ZcvTGRbsb-Q_Nw,843776
-ipex_llm/libs/gptneox-api.dll,sha256=tsK4ofR1IYgVvvO4UDCDAfB5qbKEWQw76cAJb950ouc,24576
-ipex_llm/libs/gptneox.dll,sha256=0p7t74OFQWD4RBMK2uqfdXxAasXmKTL3D-N6hF-rtUA,520192
-ipex_llm/libs/libbloom_avx.dll,sha256=4OaC5wsiEfSFCaKHqRKwIJTbQOl6ONgOSSo7aY37Xno,485888
-ipex_llm/libs/libbloom_vnni.dll,sha256=nUSzgIC83FEZHjayFFoFcCBQS-pepNSfkz8aDydsK3M,460800
-ipex_llm/libs/libgptneox_avx.dll,sha256=XxJXiVQ9poiIytU5e4xu_6E-nmUoSgx8dabdzCvZYc4,545792
-ipex_llm/libs/libgptneox_vnni.dll,sha256=ToLxjGVmKboym6b7WDRmABcXM3AjHDE_NkRjvzk9cXU,520704
-ipex_llm/libs/libllama_avx.dll,sha256=0_s3OSjq3C7OPo-Ay4jBgrf9kNrGUukvUacjj9GJVPE,540160
-ipex_llm/libs/libllama_vnni.dll,sha256=tV88Q_Xt5QV89vZQJolecyHGyXyBw1DKpV78nFhaV2Y,515072
-ipex_llm/libs/libstarcoder_avx.dll,sha256=8KK38-q9lw2yswlS7ocJ3OILsnhMQKIK0fWRyjBlRxo,577024
-ipex_llm/libs/libstarcoder_vnni.dll,sha256=lrIWp5skULzieCQHhKbA3pOQylP7QtHzBiUcJTAQZGw,551936
-ipex_llm/libs/llama-api.dll,sha256=xwTkZKorXq99kKPCufIFFRSAou40e2_I0Gcux6ZFCns,25088
-ipex_llm/libs/llama.dll,sha256=R8SePR7ze0RR-_ODaMKdrystu8HOmcXodwbk32BnPT0,514560
-ipex_llm/libs/main-bloom.exe,sha256=2aiEBPQi6c_HR0lu_xBAmFyY3_ijPQfsy2uAOLfGOZs,103424
-ipex_llm/libs/main-chatglm_vnni.exe,sha256=V8MCTcrJpSq9bPtK9B-ATBCDZjsm0jMdSaFhdVOQ4uc,726016
-ipex_llm/libs/main-gptneox.exe,sha256=BkbSwOWcbEU2tO4b3wcXruhKVn9OqN-Wn19g3C9CE9I,98816
-ipex_llm/libs/main-llama.exe,sha256=gUS9ernU1-WM9QTIzrHWBnWmKctvd_FMBFtdPdriNVc,99840
-ipex_llm/libs/main-starcoder.exe,sha256=hmd2dI8f8XQpeGYEQepuMIWnAHpuxSUo4mJoxD6mVxU,157696
-ipex_llm/libs/quantize-bloom.exe,sha256=tg-Ry4xOlGAE-rmZ2JNvZreWaokxXgTknF7mzH5lHuI,125952
-ipex_llm/libs/quantize-bloom_vnni.exe,sha256=ZxO93hQoVmYI2_UTBoRd37raTjSNyqwsR0-3CXNR0Ro,127488
-ipex_llm/libs/quantize-gptneox.exe,sha256=nhuszKDXw8nxyAQVyCNmHSZSNyRtvxnpxWUlm_AhR-c,103936
-ipex_llm/libs/quantize-gptneox_vnni.exe,sha256=5GfM_csnOp2hlRtzP2zf4I8XoQFPTlwmQEjC98CqTfY,104448
-ipex_llm/libs/quantize-llama.exe,sha256=OBfvPTl1Lk_yvKkrvXLFbIVKt7CN1iqSQYrAESR55ss,109056
-ipex_llm/libs/quantize-llama_vnni.exe,sha256=zQxMJRbqJyq3CqxXRD07y9OaPffDZ9OiDzY31QNauB4,110080
-ipex_llm/libs/quantize-starcoder.exe,sha256=mNJtrvdMyFeMFadP1f_AhHeocMPoCR9DlI3NLd2O64Q,126976
-ipex_llm/libs/quantize-starcoder_vnni.exe,sha256=tdIP1vK1V0MHG15QdjikibaLNwMOKbw1ewuChm_UVhw,128000
-ipex_llm/libs/starcoder-api.dll,sha256=lnj9xS_KKSCeteSNtEKAxPp5aOMTbaOkp7IzWrhxcak,21504
-ipex_llm/libs/starcoder.dll,sha256=L1zov-MYHLOl146NeoAumMUzb_NLZEaTDY7mQ2BH4Ik,551424
+ipex_llm/libs/bloom-api.dll,sha256=51693emI_SijSD_iVNP7sL5cDVjB2i-W48Fh9j1mypE,36352
+ipex_llm/libs/bloom.dll,sha256=9HHXSdR2Dxav8O5j4Ftnh6vxsiRedSPY5UFgBziHU4s,460288
+ipex_llm/libs/chatglm_C.cp310-win_amd64.pyd,sha256=ZzBEI-4BXqR5e8WNTnbEI04pSDOu1W4uGe8iAzvkVTo,852992
+ipex_llm/libs/chatglm_C.cp311-win_amd64.pyd,sha256=Jw0sCvZ_f_4GQVUFedBaqHMCHZSleAy2NS9BcrZpmpU,856064
+ipex_llm/libs/chatglm_C.cp39-win_amd64.pyd,sha256=zLbMaCUG1FtvNGM2VIWm89N67ifEAdRdX_w-WSyfA5w,843776
+ipex_llm/libs/gptneox-api.dll,sha256=T1KDtnFvGmGqIx_NapiaqSY49V2G97bFCHH-NHa6CNk,24576
+ipex_llm/libs/gptneox.dll,sha256=6zKIreIOn79EQVB2R8yXW025ec2daFeGB_HfnB6n6MU,520192
+ipex_llm/libs/libbloom_avx.dll,sha256=CKrRbZmNkDbwPI1SS5bZ_DXB2Q0e1siU0GfazL2omvw,485888
+ipex_llm/libs/libbloom_vnni.dll,sha256=unSvNOSZbK6W46q_Uq55fZYyH02pX_Q0_YSkvkqWx84,460800
+ipex_llm/libs/libgptneox_avx.dll,sha256=aSY3F0HOeXPnjPndFB6hk5jip6hlyd2ZorsUxiwIuLg,545792
+ipex_llm/libs/libgptneox_vnni.dll,sha256=jvcPmHjS9pSSi9R6_ZE693I9yJXiaMHueQZ2wl0xrhA,520704
+ipex_llm/libs/libllama_avx.dll,sha256=AGBk1OizYr4lhoxaPvcaq4fxBe8qL05uCew2ktIxGcI,540160
+ipex_llm/libs/libllama_vnni.dll,sha256=m5B0B95-XDbX5nk5bS4YaJaFG1DZShbrLrTos_pdAB0,515072
+ipex_llm/libs/libstarcoder_avx.dll,sha256=AkeKuA_1-WMLpPwQV3vdmHft5EsInXpnMK-fiwcVPMQ,577024
+ipex_llm/libs/libstarcoder_vnni.dll,sha256=yWulfpUW6kL7ZmB6_fzS3wpUXf5uSp0vBPvIAtSbhY4,551936
+ipex_llm/libs/llama-api.dll,sha256=3-D847W8taKmkvDxpeGUC_DHQ1N0eMkn1FBV0NpOgBM,25088
+ipex_llm/libs/llama.dll,sha256=dOewyJ9NEKeAAR4LJuFVMNEa_NwVdnN2Vv0v-FsuxmA,514560
+ipex_llm/libs/main-bloom.exe,sha256=Dv7V9th92e9YU8lfIu9RunZC7UfZ4FmwcZ-5pr2KPpU,103424
+ipex_llm/libs/main-chatglm_vnni.exe,sha256=oS-OUDGJoe_kEtmDAXLzN8UNcIZ-9jQGIYthwzY-XPQ,726016
+ipex_llm/libs/main-gptneox.exe,sha256=o-CisrdWExpi8p7uaNmyQkzMqwKevYEdcN_XerAsep8,98816
+ipex_llm/libs/main-llama.exe,sha256=wM536dvoiNmBNEqT8xl2zWEVO2VxSDZhMgaYCFMk_6I,99840
+ipex_llm/libs/main-starcoder.exe,sha256=n31RW5_xlhRlEModJ5pSovmE5B3dpgLN-lx3B1jkPO0,157696
+ipex_llm/libs/quantize-bloom.exe,sha256=R3tr_uaFP98JqHtoTYqcsCyhzfjvy2wzKlMHugkSPww,125952
+ipex_llm/libs/quantize-bloom_vnni.exe,sha256=YPz8c25ZmfGOJBJnqj403KFJo2Nq3UQPB9qc9aQ89aQ,127488
+ipex_llm/libs/quantize-gptneox.exe,sha256=PNp_U7WuSvuNMSQ32Yy2shzdBxF42H7duA6rmPXn9Sw,103936
+ipex_llm/libs/quantize-gptneox_vnni.exe,sha256=fm2pxmU_iVGx43BqRg_KZb15BpzCr6W7lWCc2x9woF8,104448
+ipex_llm/libs/quantize-llama.exe,sha256=Av_qCF-hL1Jdoj7xSuEW9HpURyzkLQLt2zNXHy1wlPM,109056
+ipex_llm/libs/quantize-llama_vnni.exe,sha256=hUKm_lsH8Zrw1Ly1Sa7vArGYBQMLqY6Z2jJwO31TH6I,110080
+ipex_llm/libs/quantize-starcoder.exe,sha256=pDtASf0AX8w5kZf81W-k65XsSEmwiJgaoMaUHJKx53Y,126976
+ipex_llm/libs/quantize-starcoder_vnni.exe,sha256=zeF60jDhTltWjT3JK17HstyP0xvJt4CESJ-CAGL_NTU,128000
+ipex_llm/libs/starcoder-api.dll,sha256=q4iTkD36JO7FieLEcfN7yK3WLSvLwk_E79hpUY1EAt0,21504
+ipex_llm/libs/starcoder.dll,sha256=pU4SwKtyO4DbiQwsURIdpWvEV9bjf3t1pfJ1ZoBAOmA,551424
 ipex_llm/llamaindex/__init__.py,sha256=T-EbRT6GJ_8RCu-iLmSzcftOimXSPQf2d5X72AUAy2Y,874
 ipex_llm/llamaindex/llms/__init__.py,sha256=KP1lEdGqDuxPoxL1ZSH25Pm2kKMPJBWUTLR0ckSLMIU,1139
 ipex_llm/llamaindex/llms/bigdlllm.py,sha256=FQBzq1KOjfc6uofTXAha3O7TqpJkNfOFepXQmOVlbnI,26314
 ipex_llm/serving/__init__.py,sha256=b2IXvVqQ5cItki021h8s3ymW12RPu8QNPprq4Mn3bDM,586
 ipex_llm/serving/fastchat/__init__.py,sha256=b2IXvVqQ5cItki021h8s3ymW12RPu8QNPprq4Mn3bDM,586
 ipex_llm/serving/fastchat/bigdl_llm_model.py,sha256=NXEN_3EPmcP3dDnvug4MokEXXE2zVUnENgBYxfubqic,10084
 ipex_llm/serving/fastchat/ipex_llm_worker.py,sha256=LNMHFYgJqna-4TfIYH7zfKElUXIYMqE0J0ICHpvMGPk,11371
 ipex_llm/serving/fastchat/model_worker.py,sha256=qJSLyWNkP6z70ysq4AV5SqHzXPJJiX2tz7AORB6jEvM,16649
 ipex_llm/serving/fastchat/vllm_worker.py,sha256=AKQSXstaNztTViXnWFVwgH_EmPsQzdTSuijNFldOnDk,11232
 ipex_llm/transformers/__init__.py,sha256=8zrY1AGBb2_AeKGDWHY4PCJyzelYA4KwahD54jPoiPg,1005
 ipex_llm/transformers/bmm.py,sha256=BlYrXqeJuw-m136Nf_ST9i6WtZrX6BiTG_psTe1M3Y0,1213
-ipex_llm/transformers/convert.py,sha256=Pel8w2gQdL5Cj0WHj_RRx7HhpzmZ3xyRoYbWFBl2D80,70437
+ipex_llm/transformers/convert.py,sha256=_2PATbcTEqJL8hv-18ENQ1tRdOQ8I6xAaj3DvoUUdkg,71241
 ipex_llm/transformers/convert_ipex.py,sha256=34aAqZ_TXrdu-Pf4eWebSxvbnu4lg3pJEc5Wd_KA0aQ,14334
 ipex_llm/transformers/embedding.py,sha256=f3crD31fEq0pT-d4FV_fS_9uLhgW64BofAxhHSO1QbE,4613
 ipex_llm/transformers/kv.py,sha256=rllcXh7wQAtyLsXWg8BxAYJuIwTBp9aRElnKifCFWRg,4533
 ipex_llm/transformers/lisa.py,sha256=F5WxbtXQ7RdKulj83h_2DnEIgKiKGZf7zvOmg6QBl2s,3289
 ipex_llm/transformers/loader.py,sha256=mC9-RuJGIvpSdP0eyDQ3OY2q1SFTwM-TDlcv2ZSVNIo,5429
 ipex_llm/transformers/lookup.py,sha256=dvQkkovR6DvoEuaHzgyFHPmeS0Yk3Gm-T2Nm0QirywE,14775
 ipex_llm/transformers/low_bit_linear.py,sha256=ifclEZ2AAh5ZN3G6fHy-8K9NgRRHJcg6rg0z7lZwaZw,38388
@@ -141,29 +141,30 @@
 ipex_llm/transformers/models/decilm.py,sha256=oAKyfB2_9GWheuqi3SyQXCBcRd6ixr6jeuYhN1z_d6A,8654
 ipex_llm/transformers/models/falcon.py,sha256=f5BzMbv4E-R5Pete8zBscbgiueXGIaWGs-5RbcMlUo4,33549
 ipex_llm/transformers/models/gemma.py,sha256=ZMn_BizM1ekqZ3erJep8L_QNLSEDgJNrUm1hEJWsQLQ,12310
 ipex_llm/transformers/models/gptbigcode.py,sha256=93l2PRLk1aLEhCGpio_7Y93amALS4SPrD5VXWiRl6hs,4342
 ipex_llm/transformers/models/gptj.py,sha256=TTIx461X2nOcIkrAcZhEf7d7mjJ3yvEC9KLVc1-hrpc,17973
 ipex_llm/transformers/models/gptneox.py,sha256=MVVdTbxV2oGzpCCzBMUy6oysVlnMtohJkl7SiC0xMAA,6219
 ipex_llm/transformers/models/internlm.py,sha256=mHyKQswtAHpT8R44gVvH7N57jjbk_GNtxjZWJy7ioog,11647
-ipex_llm/transformers/models/llama.py,sha256=RTG7JLLplwDTlijomZHQzky9HjNJDtFpOCzVeiSQcps,97944
-ipex_llm/transformers/models/mistral.py,sha256=GC0qaiQ1P-eOOmbvHoiaDziB2LFjhf8srll0fkr7c6M,45181
+ipex_llm/transformers/models/llama.py,sha256=o9tY4R5yKk_16Rn7if7kpSWiLe8jxj3P8fMPOHgTl2Y,97964
+ipex_llm/transformers/models/mistral.py,sha256=S77H3fkMstwbZMAxzb4oWKldT_Gfn1YxO6Y01WkSfWU,45217
 ipex_llm/transformers/models/mixtral.py,sha256=lO7R_Aa5GP4WPb64laSykOBfL4lvQz9RLmx2MVIANKA,27294
 ipex_llm/transformers/models/mpt.py,sha256=z02NwHogJZVh-Mk4sYoIzR90SFIKhoNN_-ifsD907TQ,9540
 ipex_llm/transformers/models/phi.py,sha256=i2IWpShCej-da32iZWTYVYVT5WuEqKVYFfiaiqDOYJg,7685
+ipex_llm/transformers/models/phi3.py,sha256=kMtUNl1Yrb8P6xwVIlxEu-xXTjhWvslyUV8pbLN1ug4,7835
 ipex_llm/transformers/models/phixtral.py,sha256=4B_2iE26GlzTVdaemd6mwYQ8mp4Yo4Yq9DgSFkF0yvc,6268
 ipex_llm/transformers/models/qwen.py,sha256=JLUFrgJ3cD_2iG_pqov5zZmkZDhZUZ9Lg9bgQYJCcWk,32349
 ipex_llm/transformers/models/qwen2.py,sha256=NFLzgdvBcj5cdmCeJi0lqXz4c0JfBioZK_im2Ysynac,32725
-ipex_llm/transformers/models/qwen2_moe.py,sha256=Wv9oU1vOx087DeC4BSVLtrAAdKKnyk2y1czzhfG7ncc,30334
+ipex_llm/transformers/models/qwen2_moe.py,sha256=Vt3mJfxJKkeochTG23_PE5g4lDzJApvGyfe-q6KPkA4,38558
 ipex_llm/transformers/models/qwen_vl.py,sha256=8uu4OS-KipkMxUZxCnjjx28LfIwdqz2ue-Ul1ZwtdO0,11832
 ipex_llm/transformers/models/rwkv4.py,sha256=Kzu6QlEi0KDXiJrfoZ71TI_D2nju2-sOeaKSZqdJz8U,6135
 ipex_llm/transformers/models/rwkv5.py,sha256=nNtWQROVAUc82SClzHrbaYVsr6CALnlVos0I2TX0YUc,10722
 ipex_llm/transformers/models/stablelm.py,sha256=xmupwXKzswNhDQRLJcuVMzBM86v0JqNX3_Wn7tKKRng,21125
 ipex_llm/transformers/models/starcoder2.py,sha256=gQSoT4T3lM8Ve1A7CiOlIp7PMwKF2fyD2uCMQUvrY1I,8822
-ipex_llm/transformers/models/utils.py,sha256=Uz9j935JfvcUlZ7OVfhszc54r1c0PB6ZZvYy_cdC5bk,18248
+ipex_llm/transformers/models/utils.py,sha256=pEJm7CDGSueuhPEVMSM7blnfC9RA7iH36JzNyx_xOuE,19678
 ipex_llm/transformers/models/yuan.py,sha256=Cus4rqN0Xq6NfqOIWkilnSzB17nNPzM2gsWlDrMp-_M,20278
 ipex_llm/utils/__init__.py,sha256=T-EbRT6GJ_8RCu-iLmSzcftOimXSPQf2d5X72AUAy2Y,874
 ipex_llm/utils/convert_chatglm.py,sha256=YLbpJIbqnQOd8aJSijG5q4xBudNi_QR5sYVjCtYoVkY,18074
 ipex_llm/utils/convert_util.py,sha256=X1eLTdF9crlca6jPEQKymEITRx_57i_87dhl1htPEhc,72612
 ipex_llm/utils/glibc_checker.py,sha256=bm6kN6gbpA7GKtnUgsCE6K16iZZyil-Ylp55SoRvHG8,2093
 ipex_llm/utils/ipex_importer.py,sha256=sZro19_QZGr7oKiTq4P_i0CMUrDFlQkc7Ple9mV38CA,2477
 ipex_llm/utils/isa_checker.py,sha256=SisZ32B1G7meZvgRKZcani1WevIhMwum7nilZ3sHgXY,2259
@@ -173,14 +174,14 @@
 ipex_llm/utils/common/lazyimport.py,sha256=AOxkmsRnqpr9zEGA5_0baqrWGhdWBmIgyKO8cwF33u4,2872
 ipex_llm/utils/common/log4Error.py,sha256=8UgIpEJYQasQO4gMOWO22nsOgr14w1emAJy4ts1VOb0,1763
 ipex_llm/vllm/__init__.py,sha256=zBSG6nzrVF5QnpR6_f7kPhBFeowTE9gaZ7D5m98E7_w,585
 ipex_llm/vllm/model_convert.py,sha256=jbsUSUAeVHm24CokIiLdyv6ubd_HuCrN_pnF3cLhhWE,7208
 ipex_llm/vllm/engine/__init__.py,sha256=mzPVAyZdbvfzBQi-wxZh1sbme_NElPMmtrJ9C2zh8Us,747
 ipex_llm/vllm/engine/engine.py,sha256=G6Zyvl2vYVQD_WodYiPxKPkkG6iVxF_EeB4bNtUPCyY,5714
 ipex_llm/vllm/entrypoints/openai/api_server.py,sha256=luEdC8lW0UZuFx_cWF13Yz7s1wUrvNhHnhAW_rHa1Ps,10564
-ipex_llm-2.1.0b20240423.data/scripts/llm-chat.ps1,sha256=6qrs-hGVAV8IKh7Jx8nq_XrnZcjd7qGU5wndArM7Yag,2769
-ipex_llm-2.1.0b20240423.data/scripts/llm-cli.ps1,sha256=3qBtTLs_EjYDnM8YyCpJhzLnGCKTEGssu9UNqfkjVXs,3009
-ipex_llm-2.1.0b20240423.dist-info/METADATA,sha256=sYLKFoqxx3oE0_axQ4rB3OHZaQuuNW1bjszRrl_tQK0,5125
-ipex_llm-2.1.0b20240423.dist-info/WHEEL,sha256=bC8mYJUOJCh5KnyEeT6W_BCQYi3v39D3z64Vy_sFvVg,98
-ipex_llm-2.1.0b20240423.dist-info/entry_points.txt,sha256=TiUyBB2MRmfF3ko-pyAEzqeBCRnyhu27bNOAsWPp3e8,61
-ipex_llm-2.1.0b20240423.dist-info/top_level.txt,sha256=CGCMHM-SyqUabU4h8RqJ2KTYckQUO3LvIWwmUQ6Qbzw,9
-ipex_llm-2.1.0b20240423.dist-info/RECORD,,
+ipex_llm-2.1.0b20240424.data/scripts/llm-chat.ps1,sha256=6qrs-hGVAV8IKh7Jx8nq_XrnZcjd7qGU5wndArM7Yag,2769
+ipex_llm-2.1.0b20240424.data/scripts/llm-cli.ps1,sha256=3qBtTLs_EjYDnM8YyCpJhzLnGCKTEGssu9UNqfkjVXs,3009
+ipex_llm-2.1.0b20240424.dist-info/METADATA,sha256=YyZbVGzUQ7f0R2dIbW-FaGTOy_iB2VbGxrjtvz34khI,5125
+ipex_llm-2.1.0b20240424.dist-info/WHEEL,sha256=bC8mYJUOJCh5KnyEeT6W_BCQYi3v39D3z64Vy_sFvVg,98
+ipex_llm-2.1.0b20240424.dist-info/entry_points.txt,sha256=TiUyBB2MRmfF3ko-pyAEzqeBCRnyhu27bNOAsWPp3e8,61
+ipex_llm-2.1.0b20240424.dist-info/top_level.txt,sha256=CGCMHM-SyqUabU4h8RqJ2KTYckQUO3LvIWwmUQ6Qbzw,9
+ipex_llm-2.1.0b20240424.dist-info/RECORD,,
```


# Comparing `tmp/adapters-0.1.2.tar.gz` & `tmp/adapters-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adapters-0.1.2.tar", last modified: Wed Feb 28 21:03:33 2024, max compression
+gzip compressed data, was "adapters-0.2.0.tar", last modified: Thu Apr 25 13:46:39 2024, max compression
```

## Comparing `adapters-0.1.2.tar` & `adapters-0.2.0.tar`

### file list

```diff
@@ -1,183 +1,185 @@
-drwxrwxrwx   0        0        0        0 2024-02-28 21:03:33.689225 adapters-0.1.2/
--rw-rw-rw-   0        0        0    11623 2024-01-27 12:24:34.000000 adapters-0.1.2/LICENSE
--rw-rw-rw-   0        0        0       17 2023-08-25 14:36:57.000000 adapters-0.1.2/MANIFEST.in
--rw-rw-rw-   0        0        0    10911 2024-02-28 21:03:33.690226 adapters-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     9474 2024-01-13 14:43:58.000000 adapters-0.1.2/README.md
--rw-rw-rw-   0        0        0       60 2023-09-09 08:43:00.000000 adapters-0.1.2/pyproject.toml
--rw-rw-rw-   0        0        0      875 2024-02-28 21:03:33.696239 adapters-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     4941 2024-02-28 21:02:36.000000 adapters-0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-02-28 21:03:32.909849 adapters-0.1.2/src/
-drwxrwxrwx   0        0        0        0 2024-02-28 21:03:32.975365 adapters-0.1.2/src/adapters/
--rw-rw-rw-   0        0        0     7343 2024-02-28 20:59:10.000000 adapters-0.1.2/src/adapters/__init__.py
--rw-rw-rw-   0        0        0     9546 2024-02-04 15:11:48.000000 adapters-0.1.2/src/adapters/composition.py
-drwxrwxrwx   0        0        0        0 2024-02-28 21:03:33.037364 adapters-0.1.2/src/adapters/configuration/
--rw-rw-rw-   0        0        0      156 2023-08-25 14:37:02.000000 adapters-0.1.2/src/adapters/configuration/__init__.py
--rw-rw-rw-   0        0        0    27034 2023-12-02 11:06:42.000000 adapters-0.1.2/src/adapters/configuration/adapter_config.py
--rw-rw-rw-   0        0        0     2743 2023-11-19 13:39:54.000000 adapters-0.1.2/src/adapters/configuration/adapter_fusion_config.py
--rw-rw-rw-   0        0        0     9999 2023-11-19 13:39:54.000000 adapters-0.1.2/src/adapters/configuration/model_adapters_config.py
--rw-rw-rw-   0        0        0     5038 2023-11-20 14:39:51.000000 adapters-0.1.2/src/adapters/context.py
--rw-rw-rw-   0        0        0    21274 2024-02-04 15:11:48.000000 adapters-0.1.2/src/adapters/head_utils.py
-drwxrwxrwx   0        0        0        0 2024-02-28 21:03:33.058366 adapters-0.1.2/src/adapters/heads/
--rw-rw-rw-   0        0        0      212 2024-02-17 10:34:53.000000 adapters-0.1.2/src/adapters/heads/__init__.py
--rw-rw-rw-   0        0        0    19353 2024-02-17 10:34:53.000000 adapters-0.1.2/src/adapters/heads/base.py
--rw-rw-rw-   0        0        0     6337 2023-11-20 14:39:51.000000 adapters-0.1.2/src/adapters/heads/dependency_parsing.py
--rw-rw-rw-   0        0        0     7658 2023-11-20 14:39:51.000000 adapters-0.1.2/src/adapters/heads/language_modeling.py
--rw-rw-rw-   0        0        0    31796 2024-02-17 10:34:53.000000 adapters-0.1.2/src/adapters/heads/model_mixin.py
--rw-rw-rw-   0        0        0     9600 2023-12-13 19:31:54.000000 adapters-0.1.2/src/adapters/hub_mixin.py
--rw-rw-rw-   0        0        0    40478 2024-02-04 15:11:48.000000 adapters-0.1.2/src/adapters/loading.py
-drwxrwxrwx   0        0        0        0 2024-02-28 21:03:33.086365 adapters-0.1.2/src/adapters/methods/
--rw-rw-rw-   0        0        0        0 2023-11-14 20:50:28.000000 adapters-0.1.2/src/adapters/methods/__init__.py
--rw-rw-rw-   0        0        0    20372 2023-11-20 14:39:51.000000 adapters-0.1.2/src/adapters/methods/adapter_layer_base.py
--rw-rw-rw-   0        0        0    16815 2023-11-14 20:50:28.000000 adapters-0.1.2/src/adapters/methods/bottleneck.py
--rw-rw-rw-   0        0        0    25234 2023-11-19 13:40:10.000000 adapters-0.1.2/src/adapters/methods/lora.py
--rw-rw-rw-   0        0        0    31612 2023-11-14 20:50:28.000000 adapters-0.1.2/src/adapters/methods/modeling.py
--rw-rw-rw-   0        0        0    24239 2024-01-27 12:24:34.000000 adapters-0.1.2/src/adapters/methods/prefix_tuning.py
--rw-rw-rw-   0        0        0     9516 2023-11-20 14:39:51.000000 adapters-0.1.2/src/adapters/methods/prompt_tuning.py
--rw-rw-rw-   0        0        0    68806 2024-01-27 12:24:34.000000 adapters-0.1.2/src/adapters/model_mixin.py
-drwxrwxrwx   0        0        0        0 2024-02-28 21:03:33.088859 adapters-0.1.2/src/adapters/models/
--rw-rw-rw-   0        0        0     3858 2024-02-04 15:11:48.000000 adapters-0.1.2/src/adapters/models/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-28 21:03:33.095365 adapters-0.1.2/src/adapters/models/albert/
--rw-rw-rw-   0        0        0     1142 2023-08-25 14:37:00.000000 adapters-0.1.2/src/adapters/models/albert/__init__.py
--rw-rw-rw-   0        0        0     3921 2024-02-17 10:34:53.000000 adapters-0.1.2/src/adapters/models/albert/adapter_model.py
--rw-rw-rw-   0        0        0     2668 2023-11-20 14:39:51.000000 adapters-0.1.2/src/adapters/models/albert/mixin_albert.py
--rw-rw-rw-   0        0        0     6063 2023-11-20 14:39:51.000000 adapters-0.1.2/src/adapters/models/albert/modeling_albert.py
-drwxrwxrwx   0        0        0        0 2024-02-28 21:03:33.102365 adapters-0.1.2/src/adapters/models/auto/
--rw-rw-rw-   0        0        0     1251 2024-02-12 21:24:12.000000 adapters-0.1.2/src/adapters/models/auto/__init__.py
--rw-rw-rw-   0        0        0     1542 2024-02-12 21:24:12.000000 adapters-0.1.2/src/adapters/models/auto/adapter_model.py
--rw-rw-rw-   0        0        0      543 2024-02-12 21:24:12.000000 adapters-0.1.2/src/adapters/models/auto/auto_factory.py
-drwxrwxrwx   0        0        0        0 2024-02-28 21:03:33.115364 adapters-0.1.2/src/adapters/models/bart/
--rw-rw-rw-   0        0        0     1138 2023-08-28 09:38:56.000000 adapters-0.1.2/src/adapters/models/bart/__init__.py
--rw-rw-rw-   0        0        0     5848 2024-02-17 10:34:53.000000 adapters-0.1.2/src/adapters/models/bart/adapter_model.py
--rw-rw-rw-   0        0        0     4319 2023-11-20 14:39:51.000000 adapters-0.1.2/src/adapters/models/bart/mixin_bart.py
--rw-rw-rw-   0        0        0    26766 2024-02-17 10:34:53.000000 adapters-0.1.2/src/adapters/models/bart/modeling_bart.py
-drwxrwxrwx   0        0        0        0 2024-02-28 21:03:33.132367 adapters-0.1.2/src/adapters/models/beit/
--rw-rw-rw-   0        0        0     1138 2023-08-25 14:37:00.000000 adapters-0.1.2/src/adapters/models/beit/__init__.py
--rw-rw-rw-   0        0        0     3121 2024-02-17 10:34:53.000000 adapters-0.1.2/src/adapters/models/beit/adapter_model.py
--rw-rw-rw-   0        0        0     2333 2024-02-17 10:34:53.000000 adapters-0.1.2/src/adapters/models/beit/mixin_beit.py
--rw-rw-rw-   0        0        0     5036 2023-11-14 20:50:28.000000 adapters-0.1.2/src/adapters/models/beit/modeling_beit.py
-drwxrwxrwx   0        0        0        0 2024-02-28 21:03:33.142392 adapters-0.1.2/src/adapters/models/bert/
--rw-rw-rw-   0        0        0     1138 2023-08-28 09:38:56.000000 adapters-0.1.2/src/adapters/models/bert/__init__.py
--rw-rw-rw-   0        0        0     4663 2024-02-17 10:34:53.000000 adapters-0.1.2/src/adapters/models/bert/adapter_model.py
--rw-rw-rw-   0        0        0     3489 2023-11-20 14:39:51.000000 adapters-0.1.2/src/adapters/models/bert/mixin_bert.py
--rw-rw-rw-   0        0        0     8251 2023-11-20 14:39:51.000000 adapters-0.1.2/src/adapters/models/bert/modeling_bert.py
-drwxrwxrwx   0        0        0        0 2024-02-28 21:03:33.178907 adapters-0.1.2/src/adapters/models/bert_generation/
--rw-rw-rw-   0        0        0     1547 2023-08-25 14:37:00.000000 adapters-0.1.2/src/adapters/models/bert_generation/__init__.py
--rw-rw-rw-   0        0        0     4734 2024-02-17 10:34:53.000000 adapters-0.1.2/src/adapters/models/bert_generation/adapter_model.py
--rw-rw-rw-   0        0        0     8635 2023-11-20 14:39:51.000000 adapters-0.1.2/src/adapters/models/bert_generation/modeling_bert_generation.py
-drwxrwxrwx   0        0        0        0 2024-02-28 21:03:33.193910 adapters-0.1.2/src/adapters/models/clip/
--rw-rw-rw-   0        0        0     1138 2023-08-25 14:37:00.000000 adapters-0.1.2/src/adapters/models/clip/__init__.py
--rw-rw-rw-   0        0        0     2785 2023-11-20 14:39:51.000000 adapters-0.1.2/src/adapters/models/clip/adapter_model.py
--rw-rw-rw-   0        0        0     4501 2023-11-20 14:39:51.000000 adapters-0.1.2/src/adapters/models/clip/mixin_clip.py
--rw-rw-rw-   0        0        0     6801 2023-11-07 17:45:30.000000 adapters-0.1.2/src/adapters/models/clip/modeling_clip.py
-drwxrwxrwx   0        0        0        0 2024-02-28 21:03:33.205910 adapters-0.1.2/src/adapters/models/deberta/
--rw-rw-rw-   0        0        0     1144 2023-08-25 14:37:00.000000 adapters-0.1.2/src/adapters/models/deberta/__init__.py
--rw-rw-rw-   0        0        0     3673 2024-02-17 10:34:53.000000 adapters-0.1.2/src/adapters/models/deberta/adapter_model.py
--rw-rw-rw-   0        0        0      557 2023-11-19 13:40:10.000000 adapters-0.1.2/src/adapters/models/deberta/mixin_deberta.py
--rw-rw-rw-   0        0        0     7288 2023-11-20 14:39:51.000000 adapters-0.1.2/src/adapters/models/deberta/modeling_deberta.py
-drwxrwxrwx   0        0        0        0 2024-02-28 21:03:33.224909 adapters-0.1.2/src/adapters/models/deberta_v2/
--rw-rw-rw-   0        0        0     1148 2023-08-25 14:37:00.000000 adapters-0.1.2/src/adapters/models/deberta_v2/__init__.py
--rw-rw-rw-   0        0        0     3698 2024-02-17 10:34:53.000000 adapters-0.1.2/src/adapters/models/deberta_v2/adapter_model.py
--rw-rw-rw-   0        0        0      795 2023-11-19 13:40:10.000000 adapters-0.1.2/src/adapters/models/deberta_v2/mixin_deberta_v2.py
--rw-rw-rw-   0        0        0     7388 2023-11-20 14:39:51.000000 adapters-0.1.2/src/adapters/models/deberta_v2/modeling_deberta_v2.py
-drwxrwxrwx   0        0        0        0 2024-02-28 21:03:33.237909 adapters-0.1.2/src/adapters/models/distilbert/
--rw-rw-rw-   0        0        0     1150 2023-08-25 14:37:00.000000 adapters-0.1.2/src/adapters/models/distilbert/__init__.py
--rw-rw-rw-   0        0        0     4876 2024-02-17 10:34:53.000000 adapters-0.1.2/src/adapters/models/distilbert/adapter_model.py
--rw-rw-rw-   0        0        0     2274 2023-11-20 14:39:51.000000 adapters-0.1.2/src/adapters/models/distilbert/mixin_distilbert.py
--rw-rw-rw-   0        0        0     6356 2023-11-20 14:39:51.000000 adapters-0.1.2/src/adapters/models/distilbert/modeling_distilbert.py
-drwxrwxrwx   0        0        0        0 2024-02-28 21:03:33.241943 adapters-0.1.2/src/adapters/models/electra/
--rw-rw-rw-   0        0        0     1144 2023-11-14 20:50:28.000000 adapters-0.1.2/src/adapters/models/electra/__init__.py
--rw-rw-rw-   0        0        0     4429 2024-02-17 10:34:53.000000 adapters-0.1.2/src/adapters/models/electra/adapter_model.py
--rw-rw-rw-   0        0        0     7523 2023-11-20 14:39:51.000000 adapters-0.1.2/src/adapters/models/electra/modeling_electra.py
-drwxrwxrwx   0        0        0        0 2024-02-28 21:03:33.257946 adapters-0.1.2/src/adapters/models/gpt2/
--rw-rw-rw-   0        0        0     1138 2023-08-28 09:38:56.000000 adapters-0.1.2/src/adapters/models/gpt2/__init__.py
--rw-rw-rw-   0        0        0     5832 2024-02-17 10:34:53.000000 adapters-0.1.2/src/adapters/models/gpt2/adapter_model.py
--rw-rw-rw-   0        0        0     2504 2023-11-20 14:39:51.000000 adapters-0.1.2/src/adapters/models/gpt2/mixin_gpt2.py
--rw-rw-rw-   0        0        0     6480 2023-11-14 20:50:28.000000 adapters-0.1.2/src/adapters/models/gpt2/modeling_gpt2.py
-drwxrwxrwx   0        0        0        0 2024-02-28 21:03:33.263944 adapters-0.1.2/src/adapters/models/gptj/
--rw-rw-rw-   0        0        0     1138 2023-08-25 14:37:00.000000 adapters-0.1.2/src/adapters/models/gptj/__init__.py
--rw-rw-rw-   0        0        0     5645 2024-02-17 10:34:53.000000 adapters-0.1.2/src/adapters/models/gptj/adapter_model.py
--rw-rw-rw-   0        0        0     2302 2023-11-20 14:39:51.000000 adapters-0.1.2/src/adapters/models/gptj/mixin_gptj.py
--rw-rw-rw-   0        0        0     6291 2023-11-19 13:40:10.000000 adapters-0.1.2/src/adapters/models/gptj/modeling_gptj.py
-drwxrwxrwx   0        0        0        0 2024-02-28 21:03:33.276944 adapters-0.1.2/src/adapters/models/llama/
--rw-rw-rw-   0        0        0     1140 2023-08-25 14:37:02.000000 adapters-0.1.2/src/adapters/models/llama/__init__.py
--rw-rw-rw-   0        0        0     5792 2024-02-17 10:34:53.000000 adapters-0.1.2/src/adapters/models/llama/adapter_model.py
--rw-rw-rw-   0        0        0     2027 2023-11-20 14:39:51.000000 adapters-0.1.2/src/adapters/models/llama/mixin_llama.py
--rw-rw-rw-   0        0        0    19828 2024-02-17 10:34:53.000000 adapters-0.1.2/src/adapters/models/llama/modeling_llama.py
-drwxrwxrwx   0        0        0        0 2024-02-28 21:03:33.289942 adapters-0.1.2/src/adapters/models/mbart/
--rw-rw-rw-   0        0        0     1140 2023-08-28 09:38:56.000000 adapters-0.1.2/src/adapters/models/mbart/__init__.py
--rw-rw-rw-   0        0        0     6319 2024-02-17 10:34:53.000000 adapters-0.1.2/src/adapters/models/mbart/adapter_model.py
--rw-rw-rw-   0        0        0    15256 2023-11-19 13:40:10.000000 adapters-0.1.2/src/adapters/models/mbart/modeling_mbart.py
-drwxrwxrwx   0        0        0        0 2024-02-28 21:03:33.305945 adapters-0.1.2/src/adapters/models/mt5/
--rw-rw-rw-   0        0        0     1136 2024-02-04 15:11:48.000000 adapters-0.1.2/src/adapters/models/mt5/__init__.py
--rw-rw-rw-   0        0        0     7911 2024-02-17 10:34:53.000000 adapters-0.1.2/src/adapters/models/mt5/adapter_model.py
--rw-rw-rw-   0        0        0    21626 2024-02-04 15:11:48.000000 adapters-0.1.2/src/adapters/models/mt5/modeling_mt5.py
-drwxrwxrwx   0        0        0        0 2024-02-28 21:03:33.321493 adapters-0.1.2/src/adapters/models/roberta/
--rw-rw-rw-   0        0        0     1144 2023-08-28 09:38:56.000000 adapters-0.1.2/src/adapters/models/roberta/__init__.py
--rw-rw-rw-   0        0        0     4710 2024-02-17 10:34:53.000000 adapters-0.1.2/src/adapters/models/roberta/adapter_model.py
--rw-rw-rw-   0        0        0     8512 2023-11-20 14:39:51.000000 adapters-0.1.2/src/adapters/models/roberta/modeling_roberta.py
-drwxrwxrwx   0        0        0        0 2024-02-28 21:03:33.439112 adapters-0.1.2/src/adapters/models/t5/
--rw-rw-rw-   0        0        0     1134 2023-08-25 14:37:00.000000 adapters-0.1.2/src/adapters/models/t5/__init__.py
--rw-rw-rw-   0        0        0     7872 2024-02-17 10:34:53.000000 adapters-0.1.2/src/adapters/models/t5/adapter_model.py
--rw-rw-rw-   0        0        0     5011 2023-11-20 14:39:51.000000 adapters-0.1.2/src/adapters/models/t5/mixin_t5.py
--rw-rw-rw-   0        0        0    21603 2023-11-20 14:39:51.000000 adapters-0.1.2/src/adapters/models/t5/modeling_t5.py
-drwxrwxrwx   0        0        0        0 2024-02-28 21:03:33.461713 adapters-0.1.2/src/adapters/models/vit/
--rw-rw-rw-   0        0        0     1136 2023-08-25 14:37:00.000000 adapters-0.1.2/src/adapters/models/vit/__init__.py
--rw-rw-rw-   0        0        0     2984 2024-02-17 10:34:53.000000 adapters-0.1.2/src/adapters/models/vit/adapter_model.py
--rw-rw-rw-   0        0        0     2227 2023-11-20 14:39:51.000000 adapters-0.1.2/src/adapters/models/vit/mixin_vit.py
--rw-rw-rw-   0        0        0     4697 2023-11-19 13:40:10.000000 adapters-0.1.2/src/adapters/models/vit/modeling_vit.py
-drwxrwxrwx   0        0        0        0 2024-02-28 21:03:33.466712 adapters-0.1.2/src/adapters/models/xlm_roberta/
--rw-rw-rw-   0        0        0     1150 2023-08-28 09:38:56.000000 adapters-0.1.2/src/adapters/models/xlm_roberta/__init__.py
--rw-rw-rw-   0        0        0     4760 2024-02-17 10:34:53.000000 adapters-0.1.2/src/adapters/models/xlm_roberta/adapter_model.py
--rw-rw-rw-   0        0        0     8644 2023-11-20 14:39:51.000000 adapters-0.1.2/src/adapters/models/xlm_roberta/modeling_xlm_roberta.py
-drwxrwxrwx   0        0        0        0 2024-02-28 21:03:33.514225 adapters-0.1.2/src/adapters/models/xmod/
--rw-rw-rw-   0        0        0     1138 2023-11-14 20:50:28.000000 adapters-0.1.2/src/adapters/models/xmod/__init__.py
--rw-rw-rw-   0        0        0     5218 2024-02-17 10:34:53.000000 adapters-0.1.2/src/adapters/models/xmod/adapter_model.py
--rw-rw-rw-   0        0        0     2687 2023-11-20 14:39:51.000000 adapters-0.1.2/src/adapters/models/xmod/mixin_xmod.py
--rw-rw-rw-   0        0        0     8460 2023-11-20 14:39:51.000000 adapters-0.1.2/src/adapters/models/xmod/modeling_xmod.py
--rw-rw-rw-   0        0        0    11982 2023-11-20 14:39:51.000000 adapters-0.1.2/src/adapters/trainer.py
--rw-rw-rw-   0        0        0     4193 2023-11-19 13:39:55.000000 adapters-0.1.2/src/adapters/training.py
--rw-rw-rw-   0        0        0    34524 2023-11-20 14:39:51.000000 adapters-0.1.2/src/adapters/utils.py
-drwxrwxrwx   0        0        0        0 2024-02-28 21:03:33.531226 adapters-0.1.2/src/adapters/wrappers/
--rw-rw-rw-   0        0        0     1212 2023-08-25 14:37:02.000000 adapters-0.1.2/src/adapters/wrappers/__init__.py
--rw-rw-rw-   0        0        0     3962 2024-01-05 22:29:03.000000 adapters-0.1.2/src/adapters/wrappers/configuration.py
--rw-rw-rw-   0        0        0     5279 2023-09-09 08:42:47.000000 adapters-0.1.2/src/adapters/wrappers/model.py
-drwxrwxrwx   0        0        0        0 2024-02-28 21:03:33.013364 adapters-0.1.2/src/adapters.egg-info/
--rw-rw-rw-   0        0        0    10911 2024-02-28 21:03:31.000000 adapters-0.1.2/src/adapters.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     5364 2024-02-28 21:03:31.000000 adapters-0.1.2/src/adapters.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-28 21:03:31.000000 adapters-0.1.2/src/adapters.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-08-04 20:36:09.000000 adapters-0.1.2/src/adapters.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0     1476 2024-02-28 21:03:31.000000 adapters-0.1.2/src/adapters.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-02-28 21:03:31.000000 adapters-0.1.2/src/adapters.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-02-28 21:03:33.688225 adapters-0.1.2/tests/
--rw-rw-rw-   0        0        0     4838 2023-12-02 11:06:43.000000 adapters-0.1.2/tests/test_adapter.py
--rw-rw-rw-   0        0        0     1847 2023-11-20 14:39:51.000000 adapters-0.1.2/tests/test_adapter_backward_compability.py
--rw-rw-rw-   0        0        0     5523 2023-11-20 14:39:51.000000 adapters-0.1.2/tests/test_adapter_config.py
--rw-rw-rw-   0        0        0    10792 2023-11-20 14:39:51.000000 adapters-0.1.2/tests/test_adapter_conversion.py
--rw-rw-rw-   0        0        0     3425 2023-11-20 14:39:51.000000 adapters-0.1.2/tests/test_adapter_custom_head.py
--rw-rw-rw-   0        0        0     6423 2023-11-20 14:39:51.000000 adapters-0.1.2/tests/test_adapter_embeddings.py
--rw-rw-rw-   0        0        0     9165 2023-11-20 14:39:51.000000 adapters-0.1.2/tests/test_adapter_fusion_common.py
--rw-rw-rw-   0        0        0     1249 2023-11-20 14:39:51.000000 adapters-0.1.2/tests/test_adapter_fusion_config.py
--rw-rw-rw-   0        0        0    19179 2024-02-17 10:34:53.000000 adapters-0.1.2/tests/test_adapter_heads.py
--rw-rw-rw-   0        0        0     7249 2023-11-20 14:39:51.000000 adapters-0.1.2/tests/test_adapter_hub.py
--rw-rw-rw-   0        0        0     4133 2023-11-20 14:39:51.000000 adapters-0.1.2/tests/test_adapter_save_id2label.py
--rw-rw-rw-   0        0        0    21978 2023-11-20 14:39:51.000000 adapters-0.1.2/tests/test_adapter_trainer.py
--rw-rw-rw-   0        0        0     2012 2023-12-02 11:06:43.000000 adapters-0.1.2/tests/test_albert.py
--rw-rw-rw-   0        0        0     1774 2023-11-20 14:39:51.000000 adapters-0.1.2/tests/test_bart.py
--rw-rw-rw-   0        0        0     1472 2023-11-20 14:39:51.000000 adapters-0.1.2/tests/test_beit.py
--rw-rw-rw-   0        0        0     1745 2023-11-20 14:39:51.000000 adapters-0.1.2/tests/test_bert.py
--rw-rw-rw-   0        0        0     3535 2023-11-20 14:39:51.000000 adapters-0.1.2/tests/test_bert_generation.py
--rw-rw-rw-   0        0        0     6003 2023-11-20 14:39:51.000000 adapters-0.1.2/tests/test_clip.py
--rw-rw-rw-   0        0        0     1866 2023-11-20 14:39:51.000000 adapters-0.1.2/tests/test_deberta.py
--rw-rw-rw-   0        0        0     1885 2023-11-20 14:39:51.000000 adapters-0.1.2/tests/test_debertaV2.py
--rw-rw-rw-   0        0        0     1763 2023-11-20 14:39:51.000000 adapters-0.1.2/tests/test_distilbert.py
--rw-rw-rw-   0        0        0     1806 2023-11-20 14:39:51.000000 adapters-0.1.2/tests/test_electra.py
--rw-rw-rw-   0        0        0     3216 2023-11-20 14:39:51.000000 adapters-0.1.2/tests/test_encoder_decoder.py
--rw-rw-rw-   0        0        0     1685 2023-11-20 14:39:51.000000 adapters-0.1.2/tests/test_gpt2.py
--rw-rw-rw-   0        0        0     1747 2023-11-20 14:39:51.000000 adapters-0.1.2/tests/test_gptj.py
--rw-rw-rw-   0        0        0     1734 2024-02-17 10:34:53.000000 adapters-0.1.2/tests/test_llama.py
--rw-rw-rw-   0        0        0     1497 2023-11-20 14:39:51.000000 adapters-0.1.2/tests/test_mbart.py
--rw-rw-rw-   0        0        0     1660 2023-11-20 14:39:51.000000 adapters-0.1.2/tests/test_roberta.py
--rw-rw-rw-   0        0        0     1671 2023-11-20 14:39:51.000000 adapters-0.1.2/tests/test_t5.py
--rw-rw-rw-   0        0        0     1622 2023-11-20 14:39:51.000000 adapters-0.1.2/tests/test_vit.py
--rw-rw-rw-   0        0        0     1293 2023-11-20 14:39:51.000000 adapters-0.1.2/tests/test_xlm_roberta.py
--rw-rw-rw-   0        0        0     1617 2023-11-20 14:39:51.000000 adapters-0.1.2/tests/test_xmod.py
+drwxrwxrwx   0        0        0        0 2024-04-25 13:46:39.923250 adapters-0.2.0/
+-rw-rw-rw-   0        0        0    11623 2024-01-27 12:24:34.000000 adapters-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0       17 2023-08-25 14:36:57.000000 adapters-0.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0    11450 2024-04-25 13:46:39.923250 adapters-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0    10020 2024-04-25 13:45:33.000000 adapters-0.2.0/README.md
+-rw-rw-rw-   0        0        0       60 2023-09-09 08:43:00.000000 adapters-0.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0      875 2024-04-25 13:46:39.925251 adapters-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     4960 2024-04-25 13:45:33.000000 adapters-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-25 13:46:38.010967 adapters-0.2.0/src/
+drwxrwxrwx   0        0        0        0 2024-04-25 13:46:38.170973 adapters-0.2.0/src/adapters/
+-rw-rw-rw-   0        0        0     7343 2024-04-25 13:45:33.000000 adapters-0.2.0/src/adapters/__init__.py
+-rw-rw-rw-   0        0        0     9546 2024-02-04 15:11:48.000000 adapters-0.2.0/src/adapters/composition.py
+drwxrwxrwx   0        0        0        0 2024-04-25 13:46:38.309251 adapters-0.2.0/src/adapters/configuration/
+-rw-rw-rw-   0        0        0      156 2023-08-25 14:37:02.000000 adapters-0.2.0/src/adapters/configuration/__init__.py
+-rw-rw-rw-   0        0        0    27171 2024-04-24 20:20:10.000000 adapters-0.2.0/src/adapters/configuration/adapter_config.py
+-rw-rw-rw-   0        0        0     2743 2023-11-19 13:39:54.000000 adapters-0.2.0/src/adapters/configuration/adapter_fusion_config.py
+-rw-rw-rw-   0        0        0     9999 2023-11-19 13:39:54.000000 adapters-0.2.0/src/adapters/configuration/model_adapters_config.py
+-rw-rw-rw-   0        0        0     5038 2023-11-20 14:39:51.000000 adapters-0.2.0/src/adapters/context.py
+-rw-rw-rw-   0        0        0    21553 2024-04-20 14:48:45.000000 adapters-0.2.0/src/adapters/head_utils.py
+drwxrwxrwx   0        0        0        0 2024-04-25 13:46:38.359250 adapters-0.2.0/src/adapters/heads/
+-rw-rw-rw-   0        0        0      212 2024-02-17 10:34:53.000000 adapters-0.2.0/src/adapters/heads/__init__.py
+-rw-rw-rw-   0        0        0    19702 2024-04-25 13:45:33.000000 adapters-0.2.0/src/adapters/heads/base.py
+-rw-rw-rw-   0        0        0     6341 2024-04-25 13:45:33.000000 adapters-0.2.0/src/adapters/heads/dependency_parsing.py
+-rw-rw-rw-   0        0        0     7658 2023-11-20 14:39:51.000000 adapters-0.2.0/src/adapters/heads/language_modeling.py
+-rw-rw-rw-   0        0        0    31796 2024-02-17 10:34:53.000000 adapters-0.2.0/src/adapters/heads/model_mixin.py
+-rw-rw-rw-   0        0        0     9657 2024-04-20 14:48:45.000000 adapters-0.2.0/src/adapters/hub_mixin.py
+-rw-rw-rw-   0        0        0    40478 2024-02-04 15:11:48.000000 adapters-0.2.0/src/adapters/loading.py
+drwxrwxrwx   0        0        0        0 2024-04-25 13:46:38.433251 adapters-0.2.0/src/adapters/methods/
+-rw-rw-rw-   0        0        0        0 2023-11-14 20:50:28.000000 adapters-0.2.0/src/adapters/methods/__init__.py
+-rw-rw-rw-   0        0        0    20866 2024-04-24 20:20:10.000000 adapters-0.2.0/src/adapters/methods/adapter_layer_base.py
+-rw-rw-rw-   0        0        0    17156 2024-04-24 20:20:10.000000 adapters-0.2.0/src/adapters/methods/bottleneck.py
+-rw-rw-rw-   0        0        0    30112 2024-04-25 13:45:33.000000 adapters-0.2.0/src/adapters/methods/lora.py
+-rw-rw-rw-   0        0        0    31696 2024-04-20 14:48:45.000000 adapters-0.2.0/src/adapters/methods/modeling.py
+-rw-rw-rw-   0        0        0    24359 2024-04-20 14:48:45.000000 adapters-0.2.0/src/adapters/methods/prefix_tuning.py
+-rw-rw-rw-   0        0        0     9516 2023-11-20 14:39:51.000000 adapters-0.2.0/src/adapters/methods/prompt_tuning.py
+-rw-rw-rw-   0        0        0     1878 2024-04-25 13:45:33.000000 adapters-0.2.0/src/adapters/methods/utils.py
+-rw-rw-rw-   0        0        0    69255 2024-04-25 13:45:33.000000 adapters-0.2.0/src/adapters/model_mixin.py
+drwxrwxrwx   0        0        0        0 2024-04-25 13:46:38.442249 adapters-0.2.0/src/adapters/models/
+-rw-rw-rw-   0        0        0     3969 2024-04-20 14:48:45.000000 adapters-0.2.0/src/adapters/models/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-25 13:46:38.483251 adapters-0.2.0/src/adapters/models/albert/
+-rw-rw-rw-   0        0        0     1142 2023-08-25 14:37:00.000000 adapters-0.2.0/src/adapters/models/albert/__init__.py
+-rw-rw-rw-   0        0        0     3921 2024-02-17 10:34:53.000000 adapters-0.2.0/src/adapters/models/albert/adapter_model.py
+-rw-rw-rw-   0        0        0     2760 2024-04-25 13:45:33.000000 adapters-0.2.0/src/adapters/models/albert/mixin_albert.py
+-rw-rw-rw-   0        0        0     6063 2023-11-20 14:39:51.000000 adapters-0.2.0/src/adapters/models/albert/modeling_albert.py
+drwxrwxrwx   0        0        0        0 2024-04-25 13:46:38.508249 adapters-0.2.0/src/adapters/models/auto/
+-rw-rw-rw-   0        0        0     1251 2024-04-24 20:33:19.000000 adapters-0.2.0/src/adapters/models/auto/__init__.py
+-rw-rw-rw-   0        0        0     1542 2024-04-24 20:33:19.000000 adapters-0.2.0/src/adapters/models/auto/adapter_model.py
+-rw-rw-rw-   0        0        0      543 2024-04-24 20:33:19.000000 adapters-0.2.0/src/adapters/models/auto/auto_factory.py
+drwxrwxrwx   0        0        0        0 2024-04-25 13:46:38.546249 adapters-0.2.0/src/adapters/models/bart/
+-rw-rw-rw-   0        0        0     1138 2023-08-28 09:38:56.000000 adapters-0.2.0/src/adapters/models/bart/__init__.py
+-rw-rw-rw-   0        0        0     5848 2024-04-20 14:48:45.000000 adapters-0.2.0/src/adapters/models/bart/adapter_model.py
+-rw-rw-rw-   0        0        0     4500 2024-04-25 13:45:33.000000 adapters-0.2.0/src/adapters/models/bart/mixin_bart.py
+-rw-rw-rw-   0        0        0    26766 2024-02-17 10:34:53.000000 adapters-0.2.0/src/adapters/models/bart/modeling_bart.py
+drwxrwxrwx   0        0        0        0 2024-04-25 13:46:38.583253 adapters-0.2.0/src/adapters/models/beit/
+-rw-rw-rw-   0        0        0     1138 2023-08-25 14:37:00.000000 adapters-0.2.0/src/adapters/models/beit/__init__.py
+-rw-rw-rw-   0        0        0     3121 2024-02-17 10:34:53.000000 adapters-0.2.0/src/adapters/models/beit/adapter_model.py
+-rw-rw-rw-   0        0        0     2424 2024-04-25 13:45:33.000000 adapters-0.2.0/src/adapters/models/beit/mixin_beit.py
+-rw-rw-rw-   0        0        0     5036 2023-11-14 20:50:28.000000 adapters-0.2.0/src/adapters/models/beit/modeling_beit.py
+drwxrwxrwx   0        0        0        0 2024-04-25 13:46:38.625250 adapters-0.2.0/src/adapters/models/bert/
+-rw-rw-rw-   0        0        0     1138 2023-08-28 09:38:56.000000 adapters-0.2.0/src/adapters/models/bert/__init__.py
+-rw-rw-rw-   0        0        0     4663 2024-02-17 10:34:53.000000 adapters-0.2.0/src/adapters/models/bert/adapter_model.py
+-rw-rw-rw-   0        0        0     3608 2024-04-25 13:45:33.000000 adapters-0.2.0/src/adapters/models/bert/mixin_bert.py
+-rw-rw-rw-   0        0        0     8251 2023-11-20 14:39:51.000000 adapters-0.2.0/src/adapters/models/bert/modeling_bert.py
+drwxrwxrwx   0        0        0        0 2024-04-25 13:46:38.655253 adapters-0.2.0/src/adapters/models/bert_generation/
+-rw-rw-rw-   0        0        0     1547 2023-08-25 14:37:00.000000 adapters-0.2.0/src/adapters/models/bert_generation/__init__.py
+-rw-rw-rw-   0        0        0     4734 2024-02-17 10:34:53.000000 adapters-0.2.0/src/adapters/models/bert_generation/adapter_model.py
+-rw-rw-rw-   0        0        0     8635 2023-11-20 14:39:51.000000 adapters-0.2.0/src/adapters/models/bert_generation/modeling_bert_generation.py
+drwxrwxrwx   0        0        0        0 2024-04-25 13:46:38.745252 adapters-0.2.0/src/adapters/models/clip/
+-rw-rw-rw-   0        0        0     1138 2023-08-25 14:37:00.000000 adapters-0.2.0/src/adapters/models/clip/__init__.py
+-rw-rw-rw-   0        0        0     2785 2023-11-20 14:39:51.000000 adapters-0.2.0/src/adapters/models/clip/adapter_model.py
+-rw-rw-rw-   0        0        0     4593 2024-04-25 13:45:33.000000 adapters-0.2.0/src/adapters/models/clip/mixin_clip.py
+-rw-rw-rw-   0        0        0     6843 2024-04-20 14:48:45.000000 adapters-0.2.0/src/adapters/models/clip/modeling_clip.py
+drwxrwxrwx   0        0        0        0 2024-04-25 13:46:38.826252 adapters-0.2.0/src/adapters/models/deberta/
+-rw-rw-rw-   0        0        0     1144 2023-08-25 14:37:00.000000 adapters-0.2.0/src/adapters/models/deberta/__init__.py
+-rw-rw-rw-   0        0        0     3673 2024-02-17 10:34:53.000000 adapters-0.2.0/src/adapters/models/deberta/adapter_model.py
+-rw-rw-rw-   0        0        0      620 2024-04-25 13:45:33.000000 adapters-0.2.0/src/adapters/models/deberta/mixin_deberta.py
+-rw-rw-rw-   0        0        0     7288 2023-11-20 14:39:51.000000 adapters-0.2.0/src/adapters/models/deberta/modeling_deberta.py
+drwxrwxrwx   0        0        0        0 2024-04-25 13:46:38.861251 adapters-0.2.0/src/adapters/models/deberta_v2/
+-rw-rw-rw-   0        0        0     1148 2023-08-25 14:37:00.000000 adapters-0.2.0/src/adapters/models/deberta_v2/__init__.py
+-rw-rw-rw-   0        0        0     3698 2024-02-17 10:34:53.000000 adapters-0.2.0/src/adapters/models/deberta_v2/adapter_model.py
+-rw-rw-rw-   0        0        0      858 2024-04-25 13:45:33.000000 adapters-0.2.0/src/adapters/models/deberta_v2/mixin_deberta_v2.py
+-rw-rw-rw-   0        0        0     7388 2023-11-20 14:39:51.000000 adapters-0.2.0/src/adapters/models/deberta_v2/modeling_deberta_v2.py
+drwxrwxrwx   0        0        0        0 2024-04-25 13:46:38.899253 adapters-0.2.0/src/adapters/models/distilbert/
+-rw-rw-rw-   0        0        0     1150 2023-08-25 14:37:00.000000 adapters-0.2.0/src/adapters/models/distilbert/__init__.py
+-rw-rw-rw-   0        0        0     4876 2024-02-17 10:34:53.000000 adapters-0.2.0/src/adapters/models/distilbert/adapter_model.py
+-rw-rw-rw-   0        0        0     2455 2024-04-25 13:45:33.000000 adapters-0.2.0/src/adapters/models/distilbert/mixin_distilbert.py
+-rw-rw-rw-   0        0        0     6356 2023-11-20 14:39:51.000000 adapters-0.2.0/src/adapters/models/distilbert/modeling_distilbert.py
+drwxrwxrwx   0        0        0        0 2024-04-25 13:46:38.925250 adapters-0.2.0/src/adapters/models/electra/
+-rw-rw-rw-   0        0        0     1144 2023-11-14 20:50:28.000000 adapters-0.2.0/src/adapters/models/electra/__init__.py
+-rw-rw-rw-   0        0        0     4429 2024-02-17 10:34:53.000000 adapters-0.2.0/src/adapters/models/electra/adapter_model.py
+-rw-rw-rw-   0        0        0     7523 2023-11-20 14:39:51.000000 adapters-0.2.0/src/adapters/models/electra/modeling_electra.py
+drwxrwxrwx   0        0        0        0 2024-04-25 13:46:39.010251 adapters-0.2.0/src/adapters/models/gpt2/
+-rw-rw-rw-   0        0        0     1138 2023-08-28 09:38:56.000000 adapters-0.2.0/src/adapters/models/gpt2/__init__.py
+-rw-rw-rw-   0        0        0     5832 2024-02-17 10:34:53.000000 adapters-0.2.0/src/adapters/models/gpt2/adapter_model.py
+-rw-rw-rw-   0        0        0     2597 2024-04-25 13:45:33.000000 adapters-0.2.0/src/adapters/models/gpt2/mixin_gpt2.py
+-rw-rw-rw-   0        0        0     6480 2023-11-14 20:50:28.000000 adapters-0.2.0/src/adapters/models/gpt2/modeling_gpt2.py
+drwxrwxrwx   0        0        0        0 2024-04-25 13:46:39.049253 adapters-0.2.0/src/adapters/models/gptj/
+-rw-rw-rw-   0        0        0     1138 2023-08-25 14:37:00.000000 adapters-0.2.0/src/adapters/models/gptj/__init__.py
+-rw-rw-rw-   0        0        0     5645 2024-02-17 10:34:53.000000 adapters-0.2.0/src/adapters/models/gptj/adapter_model.py
+-rw-rw-rw-   0        0        0     2394 2024-04-25 13:45:33.000000 adapters-0.2.0/src/adapters/models/gptj/mixin_gptj.py
+-rw-rw-rw-   0        0        0     6291 2023-11-19 13:40:10.000000 adapters-0.2.0/src/adapters/models/gptj/modeling_gptj.py
+drwxrwxrwx   0        0        0        0 2024-04-25 13:46:39.092251 adapters-0.2.0/src/adapters/models/llama/
+-rw-rw-rw-   0        0        0     1140 2023-08-25 14:37:02.000000 adapters-0.2.0/src/adapters/models/llama/__init__.py
+-rw-rw-rw-   0        0        0     5922 2024-04-20 14:48:45.000000 adapters-0.2.0/src/adapters/models/llama/adapter_model.py
+-rw-rw-rw-   0        0        0     2493 2024-04-25 13:45:33.000000 adapters-0.2.0/src/adapters/models/llama/mixin_llama.py
+-rw-rw-rw-   0        0        0    18419 2024-04-25 13:45:33.000000 adapters-0.2.0/src/adapters/models/llama/modeling_llama.py
+drwxrwxrwx   0        0        0        0 2024-04-25 13:46:39.122249 adapters-0.2.0/src/adapters/models/mbart/
+-rw-rw-rw-   0        0        0     1140 2023-08-28 09:38:56.000000 adapters-0.2.0/src/adapters/models/mbart/__init__.py
+-rw-rw-rw-   0        0        0     6319 2024-02-17 10:34:53.000000 adapters-0.2.0/src/adapters/models/mbart/adapter_model.py
+-rw-rw-rw-   0        0        0    15256 2023-11-19 13:40:10.000000 adapters-0.2.0/src/adapters/models/mbart/modeling_mbart.py
+drwxrwxrwx   0        0        0        0 2024-04-25 13:46:39.154252 adapters-0.2.0/src/adapters/models/mt5/
+-rw-rw-rw-   0        0        0     1136 2024-02-04 15:11:48.000000 adapters-0.2.0/src/adapters/models/mt5/__init__.py
+-rw-rw-rw-   0        0        0     7911 2024-02-17 10:34:53.000000 adapters-0.2.0/src/adapters/models/mt5/adapter_model.py
+-rw-rw-rw-   0        0        0    21626 2024-02-04 15:11:48.000000 adapters-0.2.0/src/adapters/models/mt5/modeling_mt5.py
+drwxrwxrwx   0        0        0        0 2024-04-25 13:46:39.300252 adapters-0.2.0/src/adapters/models/roberta/
+-rw-rw-rw-   0        0        0     1144 2023-08-28 09:38:56.000000 adapters-0.2.0/src/adapters/models/roberta/__init__.py
+-rw-rw-rw-   0        0        0     4710 2024-02-17 10:34:53.000000 adapters-0.2.0/src/adapters/models/roberta/adapter_model.py
+-rw-rw-rw-   0        0        0     8512 2023-11-20 14:39:51.000000 adapters-0.2.0/src/adapters/models/roberta/modeling_roberta.py
+drwxrwxrwx   0        0        0        0 2024-04-25 13:46:39.360253 adapters-0.2.0/src/adapters/models/t5/
+-rw-rw-rw-   0        0        0     1134 2023-08-25 14:37:00.000000 adapters-0.2.0/src/adapters/models/t5/__init__.py
+-rw-rw-rw-   0        0        0     7872 2024-02-17 10:34:53.000000 adapters-0.2.0/src/adapters/models/t5/adapter_model.py
+-rw-rw-rw-   0        0        0     5158 2024-04-25 13:45:33.000000 adapters-0.2.0/src/adapters/models/t5/mixin_t5.py
+-rw-rw-rw-   0        0        0    22273 2024-04-20 14:48:45.000000 adapters-0.2.0/src/adapters/models/t5/modeling_t5.py
+drwxrwxrwx   0        0        0        0 2024-04-25 13:46:39.428254 adapters-0.2.0/src/adapters/models/vit/
+-rw-rw-rw-   0        0        0     1136 2023-08-25 14:37:00.000000 adapters-0.2.0/src/adapters/models/vit/__init__.py
+-rw-rw-rw-   0        0        0     2984 2024-02-17 10:34:53.000000 adapters-0.2.0/src/adapters/models/vit/adapter_model.py
+-rw-rw-rw-   0        0        0     2347 2024-04-25 13:45:33.000000 adapters-0.2.0/src/adapters/models/vit/mixin_vit.py
+-rw-rw-rw-   0        0        0     4697 2023-11-19 13:40:10.000000 adapters-0.2.0/src/adapters/models/vit/modeling_vit.py
+drwxrwxrwx   0        0        0        0 2024-04-25 13:46:39.460251 adapters-0.2.0/src/adapters/models/xlm_roberta/
+-rw-rw-rw-   0        0        0     1150 2023-08-28 09:38:56.000000 adapters-0.2.0/src/adapters/models/xlm_roberta/__init__.py
+-rw-rw-rw-   0        0        0     4760 2024-02-17 10:34:53.000000 adapters-0.2.0/src/adapters/models/xlm_roberta/adapter_model.py
+-rw-rw-rw-   0        0        0     8644 2023-11-20 14:39:51.000000 adapters-0.2.0/src/adapters/models/xlm_roberta/modeling_xlm_roberta.py
+drwxrwxrwx   0        0        0        0 2024-04-25 13:46:39.500250 adapters-0.2.0/src/adapters/models/xmod/
+-rw-rw-rw-   0        0        0     1138 2023-11-14 20:50:28.000000 adapters-0.2.0/src/adapters/models/xmod/__init__.py
+-rw-rw-rw-   0        0        0     5218 2024-02-17 10:34:53.000000 adapters-0.2.0/src/adapters/models/xmod/adapter_model.py
+-rw-rw-rw-   0        0        0     2687 2023-11-20 14:39:51.000000 adapters-0.2.0/src/adapters/models/xmod/mixin_xmod.py
+-rw-rw-rw-   0        0        0     8460 2023-11-20 14:39:51.000000 adapters-0.2.0/src/adapters/models/xmod/modeling_xmod.py
+-rw-rw-rw-   0        0        0    11982 2023-11-20 14:39:51.000000 adapters-0.2.0/src/adapters/trainer.py
+-rw-rw-rw-   0        0        0     4193 2023-11-19 13:39:55.000000 adapters-0.2.0/src/adapters/training.py
+-rw-rw-rw-   0        0        0    35223 2024-04-25 13:45:33.000000 adapters-0.2.0/src/adapters/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-25 13:46:39.544251 adapters-0.2.0/src/adapters/wrappers/
+-rw-rw-rw-   0        0        0     1212 2023-08-25 14:37:02.000000 adapters-0.2.0/src/adapters/wrappers/__init__.py
+-rw-rw-rw-   0        0        0     3962 2024-01-05 22:29:03.000000 adapters-0.2.0/src/adapters/wrappers/configuration.py
+-rw-rw-rw-   0        0        0     5279 2023-09-09 08:42:47.000000 adapters-0.2.0/src/adapters/wrappers/model.py
+drwxrwxrwx   0        0        0        0 2024-04-25 13:46:38.260967 adapters-0.2.0/src/adapters.egg-info/
+-rw-rw-rw-   0        0        0    11450 2024-04-25 13:46:37.000000 adapters-0.2.0/src/adapters.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     5412 2024-04-25 13:46:37.000000 adapters-0.2.0/src/adapters.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 13:46:37.000000 adapters-0.2.0/src/adapters.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-08-04 20:36:09.000000 adapters-0.2.0/src/adapters.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0     1534 2024-04-25 13:46:37.000000 adapters-0.2.0/src/adapters.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-25 13:46:37.000000 adapters-0.2.0/src/adapters.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-25 13:46:39.922255 adapters-0.2.0/tests/
+-rw-rw-rw-   0        0        0     4871 2024-04-20 14:48:45.000000 adapters-0.2.0/tests/test_adapter.py
+-rw-rw-rw-   0        0        0     1847 2023-11-20 14:39:51.000000 adapters-0.2.0/tests/test_adapter_backward_compability.py
+-rw-rw-rw-   0        0        0     5523 2023-11-20 14:39:51.000000 adapters-0.2.0/tests/test_adapter_config.py
+-rw-rw-rw-   0        0        0    10792 2023-11-20 14:39:51.000000 adapters-0.2.0/tests/test_adapter_conversion.py
+-rw-rw-rw-   0        0        0     3425 2023-11-20 14:39:51.000000 adapters-0.2.0/tests/test_adapter_custom_head.py
+-rw-rw-rw-   0        0        0     6882 2024-04-06 16:40:46.000000 adapters-0.2.0/tests/test_adapter_embeddings.py
+-rw-rw-rw-   0        0        0     9165 2023-11-20 14:39:51.000000 adapters-0.2.0/tests/test_adapter_fusion_common.py
+-rw-rw-rw-   0        0        0     1249 2023-11-20 14:39:51.000000 adapters-0.2.0/tests/test_adapter_fusion_config.py
+-rw-rw-rw-   0        0        0    19179 2024-02-17 10:34:53.000000 adapters-0.2.0/tests/test_adapter_heads.py
+-rw-rw-rw-   0        0        0     7249 2023-11-20 14:39:51.000000 adapters-0.2.0/tests/test_adapter_hub.py
+-rw-rw-rw-   0        0        0     4133 2023-11-20 14:39:51.000000 adapters-0.2.0/tests/test_adapter_save_id2label.py
+-rw-rw-rw-   0        0        0    21978 2023-11-20 14:39:51.000000 adapters-0.2.0/tests/test_adapter_trainer.py
+-rw-rw-rw-   0        0        0     2012 2023-12-02 11:06:43.000000 adapters-0.2.0/tests/test_albert.py
+-rw-rw-rw-   0        0        0     1774 2023-11-20 14:39:51.000000 adapters-0.2.0/tests/test_bart.py
+-rw-rw-rw-   0        0        0     1472 2023-11-20 14:39:51.000000 adapters-0.2.0/tests/test_beit.py
+-rw-rw-rw-   0        0        0     1745 2023-11-20 14:39:51.000000 adapters-0.2.0/tests/test_bert.py
+-rw-rw-rw-   0        0        0     3535 2023-11-20 14:39:51.000000 adapters-0.2.0/tests/test_bert_generation.py
+-rw-rw-rw-   0        0        0     6026 2024-04-20 14:48:45.000000 adapters-0.2.0/tests/test_clip.py
+-rw-rw-rw-   0        0        0     1866 2023-11-20 14:39:51.000000 adapters-0.2.0/tests/test_deberta.py
+-rw-rw-rw-   0        0        0     1885 2023-11-20 14:39:51.000000 adapters-0.2.0/tests/test_debertaV2.py
+-rw-rw-rw-   0        0        0     1763 2023-11-20 14:39:51.000000 adapters-0.2.0/tests/test_distilbert.py
+-rw-rw-rw-   0        0        0     1806 2023-11-20 14:39:51.000000 adapters-0.2.0/tests/test_electra.py
+-rw-rw-rw-   0        0        0     3216 2023-11-20 14:39:51.000000 adapters-0.2.0/tests/test_encoder_decoder.py
+-rw-rw-rw-   0        0        0     1685 2023-11-20 14:39:51.000000 adapters-0.2.0/tests/test_gpt2.py
+-rw-rw-rw-   0        0        0     1747 2023-11-20 14:39:51.000000 adapters-0.2.0/tests/test_gptj.py
+-rw-rw-rw-   0        0        0     1816 2024-04-25 13:45:33.000000 adapters-0.2.0/tests/test_llama.py
+-rw-rw-rw-   0        0        0     1497 2023-11-20 14:39:51.000000 adapters-0.2.0/tests/test_mbart.py
+-rw-rw-rw-   0        0        0     1687 2024-02-04 15:11:48.000000 adapters-0.2.0/tests/test_mt5.py
+-rw-rw-rw-   0        0        0     1660 2023-11-20 14:39:51.000000 adapters-0.2.0/tests/test_roberta.py
+-rw-rw-rw-   0        0        0     1671 2023-11-20 14:39:51.000000 adapters-0.2.0/tests/test_t5.py
+-rw-rw-rw-   0        0        0     1622 2023-11-20 14:39:51.000000 adapters-0.2.0/tests/test_vit.py
+-rw-rw-rw-   0        0        0     1293 2023-11-20 14:39:51.000000 adapters-0.2.0/tests/test_xlm_roberta.py
+-rw-rw-rw-   0        0        0     1617 2023-11-20 14:39:51.000000 adapters-0.2.0/tests/test_xmod.py
```

### Comparing `adapters-0.1.2/LICENSE` & `adapters-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `adapters-0.1.2/PKG-INFO` & `adapters-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,682 +1,716 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310d 0a4e 616d 653a 2061 6461  : 2.1..Name: ada
 00000020: 7074 6572 730d 0a56 6572 7369 6f6e 3a20  pters..Version: 
-00000030: 302e 312e 320d 0a53 756d 6d61 7279 3a20  0.1.2..Summary: 
+00000030: 302e 322e 300d 0a53 756d 6d61 7279 3a20  0.2.0..Summary: 
 00000040: 4120 556e 6966 6965 6420 4c69 6272 6172  A Unified Librar
 00000050: 7920 666f 7220 5061 7261 6d65 7465 722d  y for Parameter-
 00000060: 4566 6669 6369 656e 7420 616e 6420 4d6f  Efficient and Mo
 00000070: 6475 6c61 7220 5472 616e 7366 6572 204c  dular Transfer L
 00000080: 6561 726e 696e 670d 0a48 6f6d 652d 7061  earning..Home-pa
 00000090: 6765 3a20 6874 7470 733a 2f2f 6769 7468  ge: https://gith
 000000a0: 7562 2e63 6f6d 2f61 6461 7074 6572 2d68  ub.com/adapter-h
 000000b0: 7562 2f61 6461 7074 6572 730d 0a41 7574  ub/adapters..Aut
 000000c0: 686f 723a 2054 6865 2041 6461 7074 6572  hor: The Adapter
 000000d0: 4875 6220 7465 616d 2061 6e64 2063 6f6d  Hub team and com
 000000e0: 6d75 6e69 7479 2063 6f6e 7472 6962 7574  munity contribut
 000000f0: 6f72 730d 0a41 7574 686f 722d 656d 6169  ors..Author-emai
-00000100: 6c3a 2070 6665 6966 6665 7240 756b 702e  l: pfeiffer@ukp.
-00000110: 7475 2d64 6172 6d73 7461 6474 2e64 650d  tu-darmstadt.de.
-00000120: 0a4c 6963 656e 7365 3a20 4170 6163 6865  .License: Apache
-00000130: 0d0a 4b65 7977 6f72 6473 3a20 4e4c 5020  ..Keywords: NLP 
-00000140: 6465 6570 206c 6561 726e 696e 6720 7472  deep learning tr
-00000150: 616e 7366 6f72 6d65 7220 7079 746f 7263  ansformer pytorc
-00000160: 6820 4245 5254 2061 6461 7074 6572 730d  h BERT adapters.
-00000170: 0a43 6c61 7373 6966 6965 723a 2044 6576  .Classifier: Dev
-00000180: 656c 6f70 6d65 6e74 2053 7461 7475 7320  elopment Status 
-00000190: 3a3a 2034 202d 2042 6574 610d 0a43 6c61  :: 4 - Beta..Cla
-000001a0: 7373 6966 6965 723a 2049 6e74 656e 6465  ssifier: Intende
-000001b0: 6420 4175 6469 656e 6365 203a 3a20 4465  d Audience :: De
-000001c0: 7665 6c6f 7065 7273 0d0a 436c 6173 7369  velopers..Classi
-000001d0: 6669 6572 3a20 496e 7465 6e64 6564 2041  fier: Intended A
-000001e0: 7564 6965 6e63 6520 3a3a 2045 6475 6361  udience :: Educa
-000001f0: 7469 6f6e 0d0a 436c 6173 7369 6669 6572  tion..Classifier
-00000200: 3a20 496e 7465 6e64 6564 2041 7564 6965  : Intended Audie
-00000210: 6e63 6520 3a3a 2053 6369 656e 6365 2f52  nce :: Science/R
-00000220: 6573 6561 7263 680d 0a43 6c61 7373 6966  esearch..Classif
-00000230: 6965 723a 204c 6963 656e 7365 203a 3a20  ier: License :: 
-00000240: 4f53 4920 4170 7072 6f76 6564 203a 3a20  OSI Approved :: 
-00000250: 4170 6163 6865 2053 6f66 7477 6172 6520  Apache Software 
-00000260: 4c69 6365 6e73 650d 0a43 6c61 7373 6966  License..Classif
-00000270: 6965 723a 204f 7065 7261 7469 6e67 2053  ier: Operating S
-00000280: 7973 7465 6d20 3a3a 204f 5320 496e 6465  ystem :: OS Inde
-00000290: 7065 6e64 656e 740d 0a43 6c61 7373 6966  pendent..Classif
-000002a0: 6965 723a 2050 726f 6772 616d 6d69 6e67  ier: Programming
-000002b0: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
-000002c0: 686f 6e20 3a3a 2033 0d0a 436c 6173 7369  hon :: 3..Classi
-000002d0: 6669 6572 3a20 5072 6f67 7261 6d6d 696e  fier: Programmin
-000002e0: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
-000002f0: 7468 6f6e 203a 3a20 332e 380d 0a43 6c61  thon :: 3.8..Cla
-00000300: 7373 6966 6965 723a 2050 726f 6772 616d  ssifier: Program
-00000310: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
-00000320: 2050 7974 686f 6e20 3a3a 2033 2e39 0d0a   Python :: 3.9..
-00000330: 436c 6173 7369 6669 6572 3a20 5072 6f67  Classifier: Prog
-00000340: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
-00000350: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
-00000360: 3130 0d0a 436c 6173 7369 6669 6572 3a20  10..Classifier: 
-00000370: 546f 7069 6320 3a3a 2053 6369 656e 7469  Topic :: Scienti
-00000380: 6669 632f 456e 6769 6e65 6572 696e 6720  fic/Engineering 
-00000390: 3a3a 2041 7274 6966 6963 6961 6c20 496e  :: Artificial In
-000003a0: 7465 6c6c 6967 656e 6365 0d0a 5265 7175  telligence..Requ
-000003b0: 6972 6573 2d50 7974 686f 6e3a 203e 3d33  ires-Python: >=3
-000003c0: 2e38 2e30 0d0a 4465 7363 7269 7074 696f  .8.0..Descriptio
-000003d0: 6e2d 436f 6e74 656e 742d 5479 7065 3a20  n-Content-Type: 
-000003e0: 7465 7874 2f6d 6172 6b64 6f77 6e0d 0a50  text/markdown..P
-000003f0: 726f 7669 6465 732d 4578 7472 613a 2073  rovides-Extra: s
-00000400: 6b6c 6561 726e 0d0a 5072 6f76 6964 6573  klearn..Provides
-00000410: 2d45 7874 7261 3a20 746f 7263 680d 0a50  -Extra: torch..P
-00000420: 726f 7669 6465 732d 4578 7472 613a 206f  rovides-Extra: o
-00000430: 6e6e 7872 756e 7469 6d65 0d0a 5072 6f76  nnxruntime..Prov
-00000440: 6964 6573 2d45 7874 7261 3a20 7365 6e74  ides-Extra: sent
-00000450: 656e 6365 7069 6563 650d 0a50 726f 7669  encepiece..Provi
-00000460: 6465 732d 4578 7472 613a 2074 6573 7469  des-Extra: testi
-00000470: 6e67 0d0a 5072 6f76 6964 6573 2d45 7874  ng..Provides-Ext
-00000480: 7261 3a20 7175 616c 6974 790d 0a50 726f  ra: quality..Pro
-00000490: 7669 6465 732d 4578 7472 613a 2064 6f63  vides-Extra: doc
-000004a0: 730d 0a50 726f 7669 6465 732d 4578 7472  s..Provides-Extr
-000004b0: 613a 2064 6576 0d0a 4c69 6365 6e73 652d  a: dev..License-
-000004c0: 4669 6c65 3a20 4c49 4345 4e53 450d 0a0d  File: LICENSE...
-000004d0: 0a3c 212d 2d2d 0d0a 436f 7079 7269 6768  .<!---..Copyrigh
-000004e0: 7420 3230 3230 2054 6865 2041 6461 7074  t 2020 The Adapt
-000004f0: 6572 4875 6220 5465 616d 2e20 416c 6c20  erHub Team. All 
-00000500: 7269 6768 7473 2072 6573 6572 7665 642e  rights reserved.
-00000510: 0d0a 0d0a 4c69 6365 6e73 6564 2075 6e64  ....Licensed und
-00000520: 6572 2074 6865 2041 7061 6368 6520 4c69  er the Apache Li
-00000530: 6365 6e73 652c 2056 6572 7369 6f6e 2032  cense, Version 2
-00000540: 2e30 2028 7468 6520 224c 6963 656e 7365  .0 (the "License
-00000550: 2229 3b0d 0a79 6f75 206d 6179 206e 6f74  ");..you may not
-00000560: 2075 7365 2074 6869 7320 6669 6c65 2065   use this file e
-00000570: 7863 6570 7420 696e 2063 6f6d 706c 6961  xcept in complia
-00000580: 6e63 6520 7769 7468 2074 6865 204c 6963  nce with the Lic
-00000590: 656e 7365 2e0d 0a59 6f75 206d 6179 206f  ense...You may o
-000005a0: 6274 6169 6e20 6120 636f 7079 206f 6620  btain a copy of 
-000005b0: 7468 6520 4c69 6365 6e73 6520 6174 0d0a  the License at..
-000005c0: 0d0a 2020 2020 6874 7470 3a2f 2f77 7777  ..    http://www
-000005d0: 2e61 7061 6368 652e 6f72 672f 6c69 6365  .apache.org/lice
-000005e0: 6e73 6573 2f4c 4943 454e 5345 2d32 2e30  nses/LICENSE-2.0
-000005f0: 0d0a 0d0a 556e 6c65 7373 2072 6571 7569  ....Unless requi
-00000600: 7265 6420 6279 2061 7070 6c69 6361 626c  red by applicabl
-00000610: 6520 6c61 7720 6f72 2061 6772 6565 6420  e law or agreed 
-00000620: 746f 2069 6e20 7772 6974 696e 672c 2073  to in writing, s
-00000630: 6f66 7477 6172 650d 0a64 6973 7472 6962  oftware..distrib
-00000640: 7574 6564 2075 6e64 6572 2074 6865 204c  uted under the L
-00000650: 6963 656e 7365 2069 7320 6469 7374 7269  icense is distri
-00000660: 6275 7465 6420 6f6e 2061 6e20 2241 5320  buted on an "AS 
-00000670: 4953 2220 4241 5349 532c 0d0a 5749 5448  IS" BASIS,..WITH
-00000680: 4f55 5420 5741 5252 414e 5449 4553 204f  OUT WARRANTIES O
-00000690: 5220 434f 4e44 4954 494f 4e53 204f 4620  R CONDITIONS OF 
-000006a0: 414e 5920 4b49 4e44 2c20 6569 7468 6572  ANY KIND, either
-000006b0: 2065 7870 7265 7373 206f 7220 696d 706c   express or impl
-000006c0: 6965 642e 0d0a 5365 6520 7468 6520 4c69  ied...See the Li
-000006d0: 6365 6e73 6520 666f 7220 7468 6520 7370  cense for the sp
-000006e0: 6563 6966 6963 206c 616e 6775 6167 6520  ecific language 
-000006f0: 676f 7665 726e 696e 6720 7065 726d 6973  governing permis
-00000700: 7369 6f6e 7320 616e 640d 0a6c 696d 6974  sions and..limit
-00000710: 6174 696f 6e73 2075 6e64 6572 2074 6865  ations under the
-00000720: 204c 6963 656e 7365 2e0d 0a2d 2d3e 0d0a   License...-->..
-00000730: 0d0a 3e20 2a2a 4e6f 7465 2a2a 3a20 5468  ..> **Note**: Th
-00000740: 6973 2072 6570 6f73 6974 6f72 7920 686f  is repository ho
-00000750: 6c64 7320 7468 6520 636f 6465 6261 7365  lds the codebase
-00000760: 206f 6620 7468 6520 5f41 6461 7074 6572   of the _Adapter
-00000770: 735f 206c 6962 7261 7279 2c20 7768 6963  s_ library, whic
-00000780: 6820 6861 7320 7265 706c 6163 6564 2060  h has replaced `
-00000790: 6164 6170 7465 722d 7472 616e 7366 6f72  adapter-transfor
-000007a0: 6d65 7273 602e 2046 6f72 2074 6865 206c  mers`. For the l
-000007b0: 6567 6163 7920 636f 6465 6261 7365 2c20  egacy codebase, 
-000007c0: 676f 2074 6f3a 2068 7474 7073 3a2f 2f67  go to: https://g
-000007d0: 6974 6875 622e 636f 6d2f 6164 6170 7465  ithub.com/adapte
-000007e0: 722d 6875 622f 6164 6170 7465 722d 7472  r-hub/adapter-tr
-000007f0: 616e 7366 6f72 6d65 7273 2d6c 6567 6163  ansformers-legac
-00000800: 792e 0d0a 0d0a 3c70 2061 6c69 676e 3d22  y.....<p align="
-00000810: 6365 6e74 6572 223e 0d0a 3c69 6d67 2073  center">..<img s
-00000820: 7479 6c65 3d22 7665 7274 6963 616c 2d61  tyle="vertical-a
-00000830: 6c69 676e 3a6d 6964 646c 6522 2073 7263  lign:middle" src
-00000840: 3d22 6874 7470 733a 2f2f 7261 772e 6769  ="https://raw.gi
-00000850: 7468 7562 7573 6572 636f 6e74 656e 742e  thubusercontent.
-00000860: 636f 6d2f 4164 6170 7465 722d 4875 622f  com/Adapter-Hub/
-00000870: 6164 6170 7465 7273 2f6d 6169 6e2f 646f  adapters/main/do
-00000880: 6373 2f6c 6f67 6f2e 706e 6722 202f 3e0d  cs/logo.png" />.
-00000890: 0a3c 2f70 3e0d 0a3c 6831 2061 6c69 676e  .</p>..<h1 align
-000008a0: 3d22 6365 6e74 6572 223e 0d0a 3c73 7061  ="center">..<spa
-000008b0: 6e3e 3c69 3e41 6461 7074 6572 733c 2f69  n><i>Adapters</i
-000008c0: 3e3c 2f73 7061 6e3e 0d0a 3c2f 6831 3e0d  ></span>..</h1>.
-000008d0: 0a0d 0a3c 6833 2061 6c69 676e 3d22 6365  ...<h3 align="ce
-000008e0: 6e74 6572 223e 0d0a 4120 556e 6966 6965  nter">..A Unifie
-000008f0: 6420 4c69 6272 6172 7920 666f 7220 5061  d Library for Pa
-00000900: 7261 6d65 7465 722d 4566 6669 6369 656e  rameter-Efficien
-00000910: 7420 616e 6420 4d6f 6475 6c61 7220 5472  t and Modular Tr
-00000920: 616e 7366 6572 204c 6561 726e 696e 670d  ansfer Learning.
-00000930: 0a3c 2f68 333e 0d0a 0d0a 215b 5465 7374  .</h3>....![Test
-00000940: 735d 2868 7474 7073 3a2f 2f67 6974 6875  s](https://githu
-00000950: 622e 636f 6d2f 4164 6170 7465 722d 4875  b.com/Adapter-Hu
-00000960: 622f 6164 6170 7465 7273 2f77 6f72 6b66  b/adapters/workf
-00000970: 6c6f 7773 2f54 6573 7473 2f62 6164 6765  lows/Tests/badge
-00000980: 2e73 7667 3f62 7261 6e63 683d 6164 6170  .svg?branch=adap
-00000990: 7465 7273 290d 0a5b 215b 4769 7448 7562  ters)..[![GitHub
-000009a0: 5d28 6874 7470 733a 2f2f 696d 672e 7368  ](https://img.sh
-000009b0: 6965 6c64 732e 696f 2f67 6974 6875 622f  ields.io/github/
-000009c0: 6c69 6365 6e73 652f 6164 6170 7465 722d  license/adapter-
-000009d0: 6875 622f 6164 6170 7465 7273 2e73 7667  hub/adapters.svg
-000009e0: 3f63 6f6c 6f72 3d62 6c75 6529 5d28 6874  ?color=blue)](ht
-000009f0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000a00: 2f61 6461 7074 6572 2d68 7562 2f61 6461  /adapter-hub/ada
-00000a10: 7074 6572 732f 626c 6f62 2f6d 6169 6e2f  pters/blob/main/
-00000a20: 4c49 4345 4e53 4529 0d0a 5b21 5b50 7950  LICENSE)..[![PyP
-00000a30: 495d 2868 7474 7073 3a2f 2f69 6d67 2e73  I](https://img.s
-00000a40: 6869 656c 6473 2e69 6f2f 7079 7069 2f76  hields.io/pypi/v
-00000a50: 2f61 6461 7074 6572 7329 5d28 6874 7470  /adapters)](http
-00000a60: 733a 2f2f 7079 7069 2e6f 7267 2f70 726f  s://pypi.org/pro
-00000a70: 6a65 6374 2f61 6461 7074 6572 732f 290d  ject/adapters/).
-00000a80: 0a0d 0a60 6164 6170 7465 7273 6020 6973  ...`adapters` is
-00000a90: 2061 6e20 6164 642d 6f6e 2074 6f20 5b48   an add-on to [H
-00000aa0: 7567 6769 6e67 4661 6365 2773 2054 7261  uggingFace's Tra
-00000ab0: 6e73 666f 726d 6572 735d 2868 7474 7073  nsformers](https
-00000ac0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6875  ://github.com/hu
-00000ad0: 6767 696e 6766 6163 652f 7472 616e 7366  ggingface/transf
-00000ae0: 6f72 6d65 7273 2920 6c69 6272 6172 792c  ormers) library,
-00000af0: 2069 6e74 6567 7261 7469 6e67 2061 6461   integrating ada
-00000b00: 7074 6572 7320 696e 746f 2073 7461 7465  pters into state
-00000b10: 2d6f 662d 7468 652d 6172 7420 6c61 6e67  -of-the-art lang
-00000b20: 7561 6765 206d 6f64 656c 7320 6279 2069  uage models by i
-00000b30: 6e63 6f72 706f 7261 7469 6e67 202a 2a5b  ncorporating **[
-00000b40: 4164 6170 7465 7248 7562 5d28 6874 7470  AdapterHub](http
-00000b50: 733a 2f2f 6164 6170 7465 7268 7562 2e6d  s://adapterhub.m
-00000b60: 6c29 2a2a 2c20 6120 6365 6e74 7261 6c20  l)**, a central 
-00000b70: 7265 706f 7369 746f 7279 2066 6f72 2070  repository for p
-00000b80: 7265 2d74 7261 696e 6564 2061 6461 7074  re-trained adapt
-00000b90: 6572 206d 6f64 756c 6573 2e0d 0a0d 0a23  er modules.....#
-00000ba0: 2320 496e 7374 616c 6c61 7469 6f6e 0d0a  # Installation..
-00000bb0: 0d0a 6061 6461 7074 6572 7360 2063 7572  ..`adapters` cur
-00000bc0: 7265 6e74 6c79 2073 7570 706f 7274 7320  rently supports 
-00000bd0: 2a2a 5079 7468 6f6e 2033 2e38 2b2a 2a20  **Python 3.8+** 
-00000be0: 616e 6420 2a2a 5079 546f 7263 6820 312e  and **PyTorch 1.
-00000bf0: 3130 2b2a 2a2e 0d0a 4166 7465 7220 5b69  10+**...After [i
-00000c00: 6e73 7461 6c6c 696e 6720 5079 546f 7263  nstalling PyTorc
-00000c10: 685d 2868 7474 7073 3a2f 2f70 7974 6f72  h](https://pytor
-00000c20: 6368 2e6f 7267 2f67 6574 2d73 7461 7274  ch.org/get-start
-00000c30: 6564 2f6c 6f63 616c 6c79 2f29 2c20 796f  ed/locally/), yo
-00000c40: 7520 6361 6e20 696e 7374 616c 6c20 6061  u can install `a
-00000c50: 6461 7074 6572 7360 2066 726f 6d20 5079  dapters` from Py
-00000c60: 5049 202e 2e2e 0d0a 0d0a 6060 600d 0a70  PI .......```..p
-00000c70: 6970 2069 6e73 7461 6c6c 202d 5520 6164  ip install -U ad
-00000c80: 6170 7465 7273 0d0a 6060 600d 0a0d 0a2e  apters..```.....
-00000c90: 2e2e 206f 7220 6672 6f6d 2073 6f75 7263  .. or from sourc
-00000ca0: 6520 6279 2063 6c6f 6e69 6e67 2074 6865  e by cloning the
-00000cb0: 2072 6570 6f73 6974 6f72 793a 0d0a 0d0a   repository:....
-00000cc0: 6060 600d 0a67 6974 2063 6c6f 6e65 2068  ```..git clone h
-00000cd0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000ce0: 6d2f 6164 6170 7465 722d 6875 622f 6164  m/adapter-hub/ad
-00000cf0: 6170 7465 7273 2e67 6974 0d0a 6364 2061  apters.git..cd a
-00000d00: 6461 7074 6572 730d 0a70 6970 2069 6e73  dapters..pip ins
-00000d10: 7461 6c6c 202e 0d0a 6060 600d 0a0d 0a23  tall ...```....#
-00000d20: 2320 5175 6963 6b20 546f 7572 0d0a 0d0a  # Quick Tour....
-00000d30: 2323 2323 204c 6f61 6420 7072 652d 7472  #### Load pre-tr
-00000d40: 6169 6e65 6420 6164 6170 7465 7273 3a0d  ained adapters:.
-00000d50: 0a0d 0a60 6060 7079 7468 6f6e 0d0a 6672  ...```python..fr
-00000d60: 6f6d 2061 6461 7074 6572 7320 696d 706f  om adapters impo
-00000d70: 7274 2041 7574 6f41 6461 7074 6572 4d6f  rt AutoAdapterMo
-00000d80: 6465 6c0d 0a66 726f 6d20 7472 616e 7366  del..from transf
-00000d90: 6f72 6d65 7273 2069 6d70 6f72 7420 4175  ormers import Au
-00000da0: 746f 546f 6b65 6e69 7a65 720d 0a0d 0a6d  toTokenizer....m
-00000db0: 6f64 656c 203d 2041 7574 6f41 6461 7074  odel = AutoAdapt
-00000dc0: 6572 4d6f 6465 6c2e 6672 6f6d 5f70 7265  erModel.from_pre
-00000dd0: 7472 6169 6e65 6428 2272 6f62 6572 7461  trained("roberta
-00000de0: 2d62 6173 6522 290d 0a74 6f6b 656e 697a  -base")..tokeniz
-00000df0: 6572 203d 2041 7574 6f54 6f6b 656e 697a  er = AutoTokeniz
-00000e00: 6572 2e66 726f 6d5f 7072 6574 7261 696e  er.from_pretrain
-00000e10: 6564 2822 726f 6265 7274 612d 6261 7365  ed("roberta-base
-00000e20: 2229 0d0a 0d0a 6d6f 6465 6c2e 6c6f 6164  ")....model.load
-00000e30: 5f61 6461 7074 6572 2822 4164 6170 7465  _adapter("Adapte
-00000e40: 7248 7562 2f72 6f62 6572 7461 2d62 6173  rHub/roberta-bas
-00000e50: 652d 7066 2d69 6d64 6222 2c20 736f 7572  e-pf-imdb", sour
-00000e60: 6365 3d22 6866 222c 2073 6574 5f61 6374  ce="hf", set_act
-00000e70: 6976 653d 5472 7565 290d 0a0d 0a70 7269  ive=True)....pri
-00000e80: 6e74 286d 6f64 656c 282a 2a74 6f6b 656e  nt(model(**token
-00000e90: 697a 6572 2822 5468 6973 2077 6f72 6b73  izer("This works
-00000ea0: 2067 7265 6174 2122 2c20 7265 7475 726e   great!", return
-00000eb0: 5f74 656e 736f 7273 3d22 7074 2229 292e  _tensors="pt")).
-00000ec0: 6c6f 6769 7473 290d 0a60 6060 0d0a 0d0a  logits)..```....
-00000ed0: 2a2a 5b4c 6561 726e 204d 6f72 655d 2868  **[Learn More](h
-00000ee0: 7474 7073 3a2f 2f64 6f63 732e 6164 6170  ttps://docs.adap
-00000ef0: 7465 7268 7562 2e6d 6c2f 6c6f 6164 696e  terhub.ml/loadin
-00000f00: 672e 6874 6d6c 292a 2a0d 0a0d 0a23 2323  g.html)**....###
-00000f10: 2320 4164 6170 7420 6578 6973 7469 6e67  # Adapt existing
-00000f20: 206d 6f64 656c 2073 6574 7570 733a 0d0a   model setups:..
-00000f30: 0d0a 6060 6070 7974 686f 6e0d 0a69 6d70  ..```python..imp
-00000f40: 6f72 7420 6164 6170 7465 7273 0d0a 6672  ort adapters..fr
-00000f50: 6f6d 2074 7261 6e73 666f 726d 6572 7320  om transformers 
-00000f60: 696d 706f 7274 2041 7574 6f4d 6f64 656c  import AutoModel
-00000f70: 466f 7253 6571 7565 6e63 6543 6c61 7373  ForSequenceClass
-00000f80: 6966 6963 6174 696f 6e0d 0a0d 0a6d 6f64  ification....mod
-00000f90: 656c 203d 2041 7574 6f4d 6f64 656c 466f  el = AutoModelFo
-00000fa0: 7253 6571 7565 6e63 6543 6c61 7373 6966  rSequenceClassif
-00000fb0: 6963 6174 696f 6e2e 6672 6f6d 5f70 7265  ication.from_pre
-00000fc0: 7472 6169 6e65 6428 2274 352d 6261 7365  trained("t5-base
-00000fd0: 2229 0d0a 0d0a 6164 6170 7465 7273 2e69  ")....adapters.i
-00000fe0: 6e69 7428 6d6f 6465 6c29 0d0a 0d0a 6d6f  nit(model)....mo
-00000ff0: 6465 6c2e 6164 645f 6164 6170 7465 7228  del.add_adapter(
-00001000: 226d 795f 6c6f 7261 5f61 6461 7074 6572  "my_lora_adapter
-00001010: 222c 2063 6f6e 6669 673d 226c 6f72 6122  ", config="lora"
-00001020: 290d 0a6d 6f64 656c 2e74 7261 696e 5f61  )..model.train_a
-00001030: 6461 7074 6572 2822 6d79 5f6c 6f72 615f  dapter("my_lora_
-00001040: 6164 6170 7465 7222 290d 0a0d 0a23 2059  adapter")....# Y
-00001050: 6f75 7220 7265 6775 6c61 7220 7472 6169  our regular trai
-00001060: 6e69 6e67 206c 6f6f 702e 2e2e 0d0a 6060  ning loop.....``
-00001070: 600d 0a0d 0a2a 2a5b 4c65 6172 6e20 4d6f  `....**[Learn Mo
-00001080: 7265 5d28 6874 7470 733a 2f2f 646f 6373  re](https://docs
-00001090: 2e61 6461 7074 6572 6875 622e 6d6c 2f71  .adapterhub.ml/q
-000010a0: 7569 636b 7374 6172 742e 6874 6d6c 292a  uickstart.html)*
-000010b0: 2a0d 0a0d 0a23 2323 2320 466c 6578 6962  *....#### Flexib
-000010c0: 6c79 2063 6f6e 6669 6775 7265 2061 6461  ly configure ada
-000010d0: 7074 6572 733a 0d0a 0d0a 6060 6070 7974  pters:....```pyt
-000010e0: 686f 6e0d 0a66 726f 6d20 6164 6170 7465  hon..from adapte
-000010f0: 7273 2069 6d70 6f72 7420 436f 6e66 6967  rs import Config
-00001100: 556e 696f 6e2c 2050 7265 6669 7854 756e  Union, PrefixTun
-00001110: 696e 6743 6f6e 6669 672c 2050 6172 426e  ingConfig, ParBn
-00001120: 436f 6e66 6967 2c20 4175 746f 4164 6170  Config, AutoAdap
-00001130: 7465 724d 6f64 656c 0d0a 0d0a 6d6f 6465  terModel....mode
-00001140: 6c20 3d20 4175 746f 4164 6170 7465 724d  l = AutoAdapterM
-00001150: 6f64 656c 2e66 726f 6d5f 7072 6574 7261  odel.from_pretra
-00001160: 696e 6564 2822 6d69 6372 6f73 6f66 742f  ined("microsoft/
-00001170: 6465 6265 7274 612d 7633 2d62 6173 6522  deberta-v3-base"
-00001180: 290d 0a0d 0a61 6461 7074 6572 5f63 6f6e  )....adapter_con
-00001190: 6669 6720 3d20 436f 6e66 6967 556e 696f  fig = ConfigUnio
-000011a0: 6e28 0d0a 2020 2020 5072 6566 6978 5475  n(..    PrefixTu
-000011b0: 6e69 6e67 436f 6e66 6967 2870 7265 6669  ningConfig(prefi
-000011c0: 785f 6c65 6e67 7468 3d32 3029 2c0d 0a20  x_length=20),.. 
-000011d0: 2020 2050 6172 426e 436f 6e66 6967 2872     ParBnConfig(r
-000011e0: 6564 7563 7469 6f6e 5f66 6163 746f 723d  eduction_factor=
-000011f0: 3429 2c0d 0a29 0d0a 6d6f 6465 6c2e 6164  4),..)..model.ad
-00001200: 645f 6164 6170 7465 7228 226d 795f 6164  d_adapter("my_ad
-00001210: 6170 7465 7222 2c20 636f 6e66 6967 3d61  apter", config=a
-00001220: 6461 7074 6572 5f63 6f6e 6669 672c 2073  dapter_config, s
-00001230: 6574 5f61 6374 6976 653d 5472 7565 290d  et_active=True).
-00001240: 0a60 6060 0d0a 0d0a 2a2a 5b4c 6561 726e  .```....**[Learn
-00001250: 204d 6f72 655d 2868 7474 7073 3a2f 2f64   More](https://d
-00001260: 6f63 732e 6164 6170 7465 7268 7562 2e6d  ocs.adapterhub.m
-00001270: 6c2f 6f76 6572 7669 6577 2e68 746d 6c29  l/overview.html)
-00001280: 2a2a 0d0a 0d0a 2323 2323 2045 6173 696c  **....#### Easil
-00001290: 7920 636f 6d70 6f73 6520 6164 6170 7465  y compose adapte
-000012a0: 7273 2069 6e20 6120 7369 6e67 6c65 206d  rs in a single m
-000012b0: 6f64 656c 3a0d 0a0d 0a60 6060 7079 7468  odel:....```pyth
-000012c0: 6f6e 0d0a 6672 6f6d 2061 6461 7074 6572  on..from adapter
-000012d0: 7320 696d 706f 7274 2041 6461 7074 6572  s import Adapter
-000012e0: 5365 7475 702c 2041 7574 6f41 6461 7074  Setup, AutoAdapt
-000012f0: 6572 4d6f 6465 6c0d 0a69 6d70 6f72 7420  erModel..import 
-00001300: 6164 6170 7465 7273 2e63 6f6d 706f 7369  adapters.composi
-00001310: 7469 6f6e 2061 7320 6163 0d0a 0d0a 6d6f  tion as ac....mo
-00001320: 6465 6c20 3d20 4175 746f 4164 6170 7465  del = AutoAdapte
-00001330: 724d 6f64 656c 2e66 726f 6d5f 7072 6574  rModel.from_pret
-00001340: 7261 696e 6564 2822 726f 6265 7274 612d  rained("roberta-
-00001350: 6261 7365 2229 0d0a 0d0a 7163 203d 206d  base")....qc = m
-00001360: 6f64 656c 2e6c 6f61 645f 6164 6170 7465  odel.load_adapte
-00001370: 7228 2241 6461 7074 6572 4875 622f 726f  r("AdapterHub/ro
-00001380: 6265 7274 612d 6261 7365 2d70 662d 7472  berta-base-pf-tr
-00001390: 6563 2229 0d0a 7365 6e74 203d 206d 6f64  ec")..sent = mod
-000013a0: 656c 2e6c 6f61 645f 6164 6170 7465 7228  el.load_adapter(
-000013b0: 2241 6461 7074 6572 4875 622f 726f 6265  "AdapterHub/robe
-000013c0: 7274 612d 6261 7365 2d70 662d 696d 6462  rta-base-pf-imdb
-000013d0: 2229 0d0a 0d0a 7769 7468 2041 6461 7074  ")....with Adapt
-000013e0: 6572 5365 7475 7028 6163 2e50 6172 616c  erSetup(ac.Paral
-000013f0: 6c65 6c28 7163 2c20 7365 6e74 2929 3a0d  lel(qc, sent)):.
-00001400: 0a20 2020 2070 7269 6e74 286d 6f64 656c  .    print(model
-00001410: 282a 2a74 6f6b 656e 697a 6572 2822 5768  (**tokenizer("Wh
-00001420: 6174 2069 7320 4164 6170 7465 7248 7562  at is AdapterHub
-00001430: 3f22 2c20 7265 7475 726e 5f74 656e 736f  ?", return_tenso
-00001440: 7273 3d22 7074 2229 2929 0d0a 6060 600d  rs="pt")))..```.
-00001450: 0a0d 0a2a 2a5b 4c65 6172 6e20 4d6f 7265  ...**[Learn More
-00001460: 5d28 6874 7470 733a 2f2f 646f 6373 2e61  ](https://docs.a
-00001470: 6461 7074 6572 6875 622e 6d6c 2f61 6461  dapterhub.ml/ada
-00001480: 7074 6572 5f63 6f6d 706f 7369 7469 6f6e  pter_composition
-00001490: 2e68 746d 6c29 2a2a 0d0a 0d0a 2323 2055  .html)**....## U
-000014a0: 7365 6675 6c20 5265 736f 7572 6365 730d  seful Resources.
-000014b0: 0a0d 0a48 7567 6769 6e67 4661 6365 2773  ...HuggingFace's
-000014c0: 2067 7265 6174 2064 6f63 756d 656e 7461   great documenta
-000014d0: 7469 6f6e 206f 6e20 6765 7474 696e 6720  tion on getting 
-000014e0: 7374 6172 7465 6420 7769 7468 205f 5472  started with _Tr
-000014f0: 616e 7366 6f72 6d65 7273 5f20 6361 6e20  ansformers_ can 
-00001500: 6265 2066 6f75 6e64 205b 6865 7265 5d28  be found [here](
-00001510: 6874 7470 733a 2f2f 6875 6767 696e 6766  https://huggingf
-00001520: 6163 652e 636f 2f74 7261 6e73 666f 726d  ace.co/transform
-00001530: 6572 732f 696e 6465 782e 6874 6d6c 292e  ers/index.html).
-00001540: 2060 6164 6170 7465 7273 6020 6973 2066   `adapters` is f
-00001550: 756c 6c79 2063 6f6d 7061 7469 626c 6520  ully compatible 
-00001560: 7769 7468 205f 5472 616e 7366 6f72 6d65  with _Transforme
-00001570: 7273 5f2e 0d0a 0d0a 546f 2067 6574 2073  rs_.....To get s
-00001580: 7461 7274 6564 2077 6974 6820 6164 6170  tarted with adap
-00001590: 7465 7273 2c20 7265 6665 7220 746f 2074  ters, refer to t
-000015a0: 6865 7365 206c 6f63 6174 696f 6e73 3a0d  hese locations:.
-000015b0: 0a0d 0a2d 202a 2a5b 436f 6c61 6220 6e6f  ...- **[Colab no
-000015c0: 7465 626f 6f6b 2074 7574 6f72 6961 6c73  tebook tutorials
-000015d0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-000015e0: 2e63 6f6d 2f41 6461 7074 6572 2d48 7562  .com/Adapter-Hub
-000015f0: 2f61 6461 7074 6572 732f 7472 6565 2f6d  /adapters/tree/m
-00001600: 6169 6e2f 6e6f 7465 626f 6f6b 7329 2a2a  ain/notebooks)**
-00001610: 2c20 6120 7365 7269 6573 206e 6f74 6562  , a series noteb
-00001620: 6f6f 6b73 2070 726f 7669 6469 6e67 2061  ooks providing a
-00001630: 6e20 696e 7472 6f64 7563 7469 6f6e 2074  n introduction t
-00001640: 6f20 616c 6c20 7468 6520 6d61 696e 2063  o all the main c
-00001650: 6f6e 6365 7074 7320 6f66 2028 6164 6170  oncepts of (adap
-00001660: 7465 722d 2974 7261 6e73 666f 726d 6572  ter-)transformer
-00001670: 7320 616e 6420 4164 6170 7465 7248 7562  s and AdapterHub
-00001680: 0d0a 2d20 2a2a 6874 7470 733a 2f2f 646f  ..- **https://do
-00001690: 6373 2e61 6461 7074 6572 6875 622e 6d6c  cs.adapterhub.ml
-000016a0: 2a2a 2c20 6f75 7220 646f 6375 6d65 6e74  **, our document
-000016b0: 6174 696f 6e20 6f6e 2074 7261 696e 696e  ation on trainin
-000016c0: 6720 616e 6420 7573 696e 6720 6164 6170  g and using adap
-000016d0: 7465 7273 2077 6974 6820 5f61 6461 7074  ters with _adapt
-000016e0: 6572 735f 0d0a 2d20 2a2a 6874 7470 733a  ers_..- **https:
-000016f0: 2f2f 6164 6170 7465 7268 7562 2e6d 6c2a  //adapterhub.ml*
-00001700: 2a20 746f 2065 7870 6c6f 7265 2061 7661  * to explore ava
-00001710: 696c 6162 6c65 2070 7265 2d74 7261 696e  ilable pre-train
-00001720: 6564 2061 6461 7074 6572 206d 6f64 756c  ed adapter modul
-00001730: 6573 2061 6e64 2073 6861 7265 2079 6f75  es and share you
-00001740: 7220 6f77 6e20 6164 6170 7465 7273 0d0a  r own adapters..
-00001750: 2d20 2a2a 5b45 7861 6d70 6c65 7320 666f  - **[Examples fo
-00001760: 6c64 6572 5d28 6874 7470 733a 2f2f 6769  lder](https://gi
-00001770: 7468 7562 2e63 6f6d 2f41 6461 7074 6572  thub.com/Adapter
-00001780: 2d48 7562 2f61 6461 7074 6572 732f 7472  -Hub/adapters/tr
-00001790: 6565 2f6d 6169 6e2f 6578 616d 706c 6573  ee/main/examples
-000017a0: 2f70 7974 6f72 6368 292a 2a20 6f66 2074  /pytorch)** of t
-000017b0: 6869 7320 7265 706f 7369 746f 7279 2063  his repository c
-000017c0: 6f6e 7461 696e 696e 6720 4875 6767 696e  ontaining Huggin
-000017d0: 6746 6163 6527 7320 6578 616d 706c 6520  gFace's example 
-000017e0: 7472 6169 6e69 6e67 2073 6372 6970 7473  training scripts
-000017f0: 2c20 6d61 6e79 2061 6461 7074 6564 2066  , many adapted f
-00001800: 6f72 2074 7261 696e 696e 6720 6164 6170  or training adap
-00001810: 7465 7273 0d0a 0d0a 2323 2049 6d70 6c65  ters....## Imple
-00001820: 6d65 6e74 6564 204d 6574 686f 6473 0d0a  mented Methods..
-00001830: 0d0a 4375 7272 656e 746c 792c 2061 6461  ..Currently, ada
-00001840: 7074 6572 7320 696e 7465 6772 6174 6573  pters integrates
-00001850: 2061 6c6c 2061 7263 6869 7465 6374 7572   all architectur
-00001860: 6573 2061 6e64 206d 6574 686f 6473 206c  es and methods l
-00001870: 6973 7465 6420 6265 6c6f 773a 0d0a 0d0a  isted below:....
-00001880: 7c20 4d65 7468 6f64 207c 2050 6170 6572  | Method | Paper
-00001890: 2873 2920 7c20 5175 6963 6b20 4c69 6e6b  (s) | Quick Link
-000018a0: 7320 7c0d 0a7c 202d 2d2d 207c 202d 2d2d  s |..| --- | ---
-000018b0: 207c 202d 2d2d 207c 0d0a 7c20 426f 7474   | --- |..| Bott
-000018c0: 6c65 6e65 636b 2061 6461 7074 6572 7320  leneck adapters 
-000018d0: 7c20 5b48 6f75 6c73 6279 2065 7420 616c  | [Houlsby et al
-000018e0: 2e20 2832 3031 3929 5d28 6874 7470 733a  . (2019)](https:
-000018f0: 2f2f 6172 7869 762e 6f72 672f 7064 662f  //arxiv.org/pdf/
-00001900: 3139 3032 2e30 3037 3531 2e70 6466 293c  1902.00751.pdf)<
-00001910: 6272 3e20 5b42 6170 6e61 2061 6e64 2046  br> [Bapna and F
-00001920: 6972 6174 2028 3230 3139 295d 2868 7474  irat (2019)](htt
-00001930: 7073 3a2f 2f61 7278 6976 2e6f 7267 2f70  ps://arxiv.org/p
-00001940: 6466 2f31 3930 392e 3038 3437 382e 7064  df/1909.08478.pd
-00001950: 6629 207c 205b 5175 6963 6b73 7461 7274  f) | [Quickstart
-00001960: 5d28 6874 7470 733a 2f2f 646f 6373 2e61  ](https://docs.a
-00001970: 6461 7074 6572 6875 622e 6d6c 2f71 7569  dapterhub.ml/qui
-00001980: 636b 7374 6172 742e 6874 6d6c 292c 205b  ckstart.html), [
-00001990: 4e6f 7465 626f 6f6b 5d28 6874 7470 733a  Notebook](https:
-000019a0: 2f2f 636f 6c61 622e 7265 7365 6172 6368  //colab.research
-000019b0: 2e67 6f6f 676c 652e 636f 6d2f 6769 7468  .google.com/gith
-000019c0: 7562 2f41 6461 7074 6572 2d48 7562 2f61  ub/Adapter-Hub/a
-000019d0: 6461 7074 6572 732f 626c 6f62 2f6d 6169  dapters/blob/mai
-000019e0: 6e2f 6e6f 7465 626f 6f6b 732f 3031 5f41  n/notebooks/01_A
-000019f0: 6461 7074 6572 5f54 7261 696e 696e 672e  dapter_Training.
-00001a00: 6970 796e 6229 207c 0d0a 7c20 4164 6170  ipynb) |..| Adap
-00001a10: 7465 7246 7573 696f 6e20 7c20 5b50 6665  terFusion | [Pfe
-00001a20: 6966 6665 7220 6574 2061 6c2e 2028 3230  iffer et al. (20
-00001a30: 3231 295d 2868 7474 7073 3a2f 2f61 636c  21)](https://acl
-00001a40: 616e 7468 6f6c 6f67 792e 6f72 672f 3230  anthology.org/20
-00001a50: 3231 2e65 6163 6c2d 6d61 696e 2e33 392e  21.eacl-main.39.
-00001a60: 7064 6629 207c 205b 446f 6373 3a20 5472  pdf) | [Docs: Tr
-00001a70: 6169 6e69 6e67 5d28 6874 7470 733a 2f2f  aining](https://
-00001a80: 646f 6373 2e61 6461 7074 6572 6875 622e  docs.adapterhub.
-00001a90: 6d6c 2f74 7261 696e 696e 672e 6874 6d6c  ml/training.html
-00001aa0: 2374 7261 696e 2d61 6461 7074 6572 6675  #train-adapterfu
-00001ab0: 7369 6f6e 292c 205b 4e6f 7465 626f 6f6b  sion), [Notebook
-00001ac0: 5d28 6874 7470 733a 2f2f 636f 6c61 622e  ](https://colab.
-00001ad0: 7265 7365 6172 6368 2e67 6f6f 676c 652e  research.google.
-00001ae0: 636f 6d2f 6769 7468 7562 2f41 6461 7074  com/github/Adapt
-00001af0: 6572 2d48 7562 2f61 6461 7074 6572 732f  er-Hub/adapters/
-00001b00: 626c 6f62 2f6d 6169 6e2f 6e6f 7465 626f  blob/main/notebo
-00001b10: 6f6b 732f 3033 5f41 6461 7074 6572 5f46  oks/03_Adapter_F
-00001b20: 7573 696f 6e2e 6970 796e 6229 207c 0d0a  usion.ipynb) |..
-00001b30: 7c20 4d41 442d 582c 3c62 723e 2049 6e76  | MAD-X,<br> Inv
-00001b40: 6572 7469 626c 6520 6164 6170 7465 7273  ertible adapters
-00001b50: 207c 205b 5066 6569 6666 6572 2065 7420   | [Pfeiffer et 
-00001b60: 616c 2e20 2832 3032 3029 5d28 6874 7470  al. (2020)](http
-00001b70: 733a 2f2f 6163 6c61 6e74 686f 6c6f 6779  s://aclanthology
-00001b80: 2e6f 7267 2f32 3032 302e 656d 6e6c 702d  .org/2020.emnlp-
-00001b90: 6d61 696e 2e36 3137 2f29 207c 205b 4e6f  main.617/) | [No
-00001ba0: 7465 626f 6f6b 5d28 6874 7470 733a 2f2f  tebook](https://
-00001bb0: 636f 6c61 622e 7265 7365 6172 6368 2e67  colab.research.g
-00001bc0: 6f6f 676c 652e 636f 6d2f 6769 7468 7562  oogle.com/github
-00001bd0: 2f41 6461 7074 6572 2d48 7562 2f61 6461  /Adapter-Hub/ada
-00001be0: 7074 6572 732f 626c 6f62 2f6d 6169 6e2f  pters/blob/main/
-00001bf0: 6e6f 7465 626f 6f6b 732f 3034 5f43 726f  notebooks/04_Cro
-00001c00: 7373 5f4c 696e 6775 616c 5f54 7261 6e73  ss_Lingual_Trans
-00001c10: 6665 722e 6970 796e 6229 207c 0d0a 7c20  fer.ipynb) |..| 
-00001c20: 4164 6170 7465 7244 726f 7020 7c20 5b52  AdapterDrop | [R
-00001c30: c3bc 636b 6cc3 a920 6574 2061 6c2e 2028  ..ckl.. et al. (
-00001c40: 3230 3231 295d 2868 7474 7073 3a2f 2f61  2021)](https://a
-00001c50: 7278 6976 2e6f 7267 2f70 6466 2f32 3031  rxiv.org/pdf/201
-00001c60: 302e 3131 3931 382e 7064 6629 207c 205b  0.11918.pdf) | [
-00001c70: 4e6f 7465 626f 6f6b 5d28 6874 7470 733a  Notebook](https:
-00001c80: 2f2f 636f 6c61 622e 7265 7365 6172 6368  //colab.research
-00001c90: 2e67 6f6f 676c 652e 636f 6d2f 6769 7468  .google.com/gith
-00001ca0: 7562 2f41 6461 7074 6572 2d48 7562 2f61  ub/Adapter-Hub/a
-00001cb0: 6461 7074 6572 732f 626c 6f62 2f6d 6169  dapters/blob/mai
-00001cc0: 6e2f 6e6f 7465 626f 6f6b 732f 3035 5f41  n/notebooks/05_A
-00001cd0: 6461 7074 6572 5f44 726f 705f 5472 6169  dapter_Drop_Trai
-00001ce0: 6e69 6e67 2e69 7079 6e62 2920 7c0d 0a7c  ning.ipynb) |..|
-00001cf0: 204d 4144 2d58 2032 2e30 2c3c 6272 3e20   MAD-X 2.0,<br> 
-00001d00: 456d 6265 6464 696e 6720 7472 6169 6e69  Embedding traini
-00001d10: 6e67 207c 205b 5066 6569 6666 6572 2065  ng | [Pfeiffer e
-00001d20: 7420 616c 2e20 2832 3032 3129 5d28 6874  t al. (2021)](ht
-00001d30: 7470 733a 2f2f 6172 7869 762e 6f72 672f  tps://arxiv.org/
-00001d40: 7064 662f 3230 3132 2e31 3535 3632 2e70  pdf/2012.15562.p
-00001d50: 6466 2920 7c20 5b44 6f63 733a 2045 6d62  df) | [Docs: Emb
-00001d60: 6564 6469 6e67 735d 2868 7474 7073 3a2f  eddings](https:/
-00001d70: 2f64 6f63 732e 6164 6170 7465 7268 7562  /docs.adapterhub
-00001d80: 2e6d 6c2f 656d 6265 6464 696e 6773 2e68  .ml/embeddings.h
-00001d90: 746d 6c29 2c20 5b4e 6f74 6562 6f6f 6b5d  tml), [Notebook]
-00001da0: 2868 7474 7073 3a2f 2f63 6f6c 6162 2e72  (https://colab.r
-00001db0: 6573 6561 7263 682e 676f 6f67 6c65 2e63  esearch.google.c
-00001dc0: 6f6d 2f67 6974 6875 622f 4164 6170 7465  om/github/Adapte
-00001dd0: 722d 4875 622f 6164 6170 7465 7273 2f62  r-Hub/adapters/b
-00001de0: 6c6f 622f 6d61 696e 2f6e 6f74 6562 6f6f  lob/main/noteboo
-00001df0: 6b73 2f30 385f 4e45 525f 5769 6b69 616e  ks/08_NER_Wikian
-00001e00: 6e2e 6970 796e 6229 207c 0d0a 7c20 5072  n.ipynb) |..| Pr
-00001e10: 6566 6978 2054 756e 696e 6720 7c20 5b4c  efix Tuning | [L
-00001e20: 6920 616e 6420 4c69 616e 6720 2832 3032  i and Liang (202
-00001e30: 3129 5d28 6874 7470 733a 2f2f 6172 7869  1)](https://arxi
-00001e40: 762e 6f72 672f 7064 662f 3231 3031 2e30  v.org/pdf/2101.0
-00001e50: 3031 3930 2e70 6466 2920 7c20 5b44 6f63  0190.pdf) | [Doc
-00001e60: 735d 2868 7474 7073 3a2f 2f64 6f63 732e  s](https://docs.
-00001e70: 6164 6170 7465 7268 7562 2e6d 6c2f 6d65  adapterhub.ml/me
-00001e80: 7468 6f64 732e 6874 6d6c 2370 7265 6669  thods.html#prefi
-00001e90: 782d 7475 6e69 6e67 2920 7c0d 0a7c 2050  x-tuning) |..| P
-00001ea0: 6172 616c 6c65 6c20 6164 6170 7465 7273  arallel adapters
-00001eb0: 2c3c 6272 3e20 4d69 782d 616e 642d 4d61  ,<br> Mix-and-Ma
-00001ec0: 7463 6820 6164 6170 7465 7273 207c 205b  tch adapters | [
-00001ed0: 4865 2065 7420 616c 2e20 2832 3032 3129  He et al. (2021)
-00001ee0: 5d28 6874 7470 733a 2f2f 6172 7869 762e  ](https://arxiv.
-00001ef0: 6f72 672f 7064 662f 3231 3130 2e30 3433  org/pdf/2110.043
-00001f00: 3636 2e70 6466 2920 7c20 5b44 6f63 735d  66.pdf) | [Docs]
-00001f10: 2868 7474 7073 3a2f 2f64 6f63 732e 6164  (https://docs.ad
-00001f20: 6170 7465 7268 7562 2e6d 6c2f 6d65 7468  apterhub.ml/meth
-00001f30: 6f64 5f63 6f6d 6269 6e61 7469 6f6e 732e  od_combinations.
-00001f40: 6874 6d6c 236d 6978 2d61 6e64 2d6d 6174  html#mix-and-mat
-00001f50: 6368 2d61 6461 7074 6572 7329 207c 0d0a  ch-adapters) |..
-00001f60: 7c20 436f 6d70 6163 7465 7220 7c20 5b4d  | Compacter | [M
-00001f70: 6168 6162 6164 6920 6574 2061 6c2e 2028  ahabadi et al. (
-00001f80: 3230 3231 295d 2868 7474 7073 3a2f 2f61  2021)](https://a
-00001f90: 7278 6976 2e6f 7267 2f70 6466 2f32 3130  rxiv.org/pdf/210
-00001fa0: 362e 3034 3634 372e 7064 6629 207c 205b  6.04647.pdf) | [
-00001fb0: 446f 6373 5d28 6874 7470 733a 2f2f 646f  Docs](https://do
-00001fc0: 6373 2e61 6461 7074 6572 6875 622e 6d6c  cs.adapterhub.ml
-00001fd0: 2f6d 6574 686f 6473 2e68 746d 6c23 636f  /methods.html#co
-00001fe0: 6d70 6163 7465 7229 207c 0d0a 7c20 4c6f  mpacter) |..| Lo
-00001ff0: 5241 207c 205b 4875 2065 7420 616c 2e20  RA | [Hu et al. 
-00002000: 2832 3032 3129 5d28 6874 7470 733a 2f2f  (2021)](https://
-00002010: 6172 7869 762e 6f72 672f 7064 662f 3231  arxiv.org/pdf/21
-00002020: 3036 2e30 3936 3835 2e70 6466 2920 7c20  06.09685.pdf) | 
-00002030: 5b44 6f63 735d 2868 7474 7073 3a2f 2f64  [Docs](https://d
-00002040: 6f63 732e 6164 6170 7465 7268 7562 2e6d  ocs.adapterhub.m
-00002050: 6c2f 6d65 7468 6f64 732e 6874 6d6c 236c  l/methods.html#l
-00002060: 6f72 6129 207c 0d0a 7c20 2849 4129 5e33  ora) |..| (IA)^3
-00002070: 207c 205b 4c69 7520 6574 2061 6c2e 2028   | [Liu et al. (
-00002080: 3230 3232 295d 2868 7474 7073 3a2f 2f61  2022)](https://a
-00002090: 7278 6976 2e6f 7267 2f70 6466 2f32 3230  rxiv.org/pdf/220
-000020a0: 352e 3035 3633 382e 7064 6629 207c 205b  5.05638.pdf) | [
-000020b0: 446f 6373 5d28 6874 7470 733a 2f2f 646f  Docs](https://do
-000020c0: 6373 2e61 6461 7074 6572 6875 622e 6d6c  cs.adapterhub.ml
-000020d0: 2f6d 6574 686f 6473 2e68 746d 6c23 6961  /methods.html#ia
-000020e0: 2d33 2920 7c0d 0a7c 2055 6e69 5045 4c54  -3) |..| UniPELT
-000020f0: 207c 205b 4d61 6f20 6574 2061 6c2e 2028   | [Mao et al. (
-00002100: 3230 3232 295d 2868 7474 7073 3a2f 2f61  2022)](https://a
-00002110: 7278 6976 2e6f 7267 2f70 6466 2f32 3131  rxiv.org/pdf/211
-00002120: 302e 3037 3537 372e 7064 6629 207c 205b  0.07577.pdf) | [
-00002130: 446f 6373 5d28 6874 7470 733a 2f2f 646f  Docs](https://do
-00002140: 6373 2e61 6461 7074 6572 6875 622e 6d6c  cs.adapterhub.ml
-00002150: 2f6d 6574 686f 645f 636f 6d62 696e 6174  /method_combinat
-00002160: 696f 6e73 2e68 746d 6c23 756e 6970 656c  ions.html#unipel
-00002170: 7429 207c 0d0a 7c20 5072 6f6d 7074 2054  t) |..| Prompt T
-00002180: 756e 696e 6720 7c20 5b4c 6573 7465 7220  uning | [Lester 
-00002190: 6574 2061 6c2e 2028 3230 3231 295d 2868  et al. (2021)](h
-000021a0: 7474 7073 3a2f 2f61 636c 616e 7468 6f6c  ttps://aclanthol
-000021b0: 6f67 792e 6f72 672f 3230 3231 2e65 6d6e  ogy.org/2021.emn
-000021c0: 6c70 2d6d 6169 6e2e 3234 332f 2920 7c20  lp-main.243/) | 
-000021d0: 5b44 6f63 735d 2868 7474 7073 3a2f 2f64  [Docs](https://d
-000021e0: 6f63 732e 6164 6170 7465 7268 7562 2e6d  ocs.adapterhub.m
-000021f0: 6c2f 6d65 7468 6f64 732e 6874 6d6c 2370  l/methods.html#p
-00002200: 726f 6d70 742d 7475 6e69 6e67 2920 7c0d  rompt-tuning) |.
-00002210: 0a0d 0a23 2320 5375 7070 6f72 7465 6420  ...## Supported 
-00002220: 4d6f 6465 6c73 0d0a 0d0a 5765 2063 7572  Models....We cur
-00002230: 7265 6e74 6c79 2073 7570 706f 7274 2074  rently support t
-00002240: 6865 2050 7954 6f72 6368 2076 6572 7369  he PyTorch versi
-00002250: 6f6e 7320 6f66 2061 6c6c 206d 6f64 656c  ons of all model
-00002260: 7320 6c69 7374 6564 206f 6e20 7468 6520  s listed on the 
-00002270: 2a2a 5b4d 6f64 656c 204f 7665 7276 6965  **[Model Overvie
-00002280: 775d 2868 7474 7073 3a2f 2f64 6f63 732e  w](https://docs.
-00002290: 6164 6170 7465 7268 7562 2e6d 6c2f 6d6f  adapterhub.ml/mo
-000022a0: 6465 6c5f 6f76 6572 7669 6577 2e68 746d  del_overview.htm
-000022b0: 6c29 2070 6167 652a 2a20 696e 206f 7572  l) page** in our
-000022c0: 2064 6f63 756d 656e 7461 7469 6f6e 2e0d   documentation..
-000022d0: 0a0d 0a23 2320 4465 7665 6c6f 7069 6e67  ...## Developing
-000022e0: 2026 2043 6f6e 7472 6962 7574 696e 670d   & Contributing.
-000022f0: 0a0d 0a54 6f20 6765 7420 7374 6172 7465  ...To get starte
-00002300: 6420 7769 7468 2064 6576 656c 6f70 696e  d with developin
-00002310: 6720 6f6e 205f 4164 6170 7465 7273 5f20  g on _Adapters_ 
-00002320: 796f 7572 7365 6c66 2061 6e64 206c 6561  yourself and lea
-00002330: 726e 206d 6f72 6520 6162 6f75 7420 7761  rn more about wa
-00002340: 7973 2074 6f20 636f 6e74 7269 6275 7465  ys to contribute
-00002350: 2c20 706c 6561 7365 2073 6565 2068 7474  , please see htt
-00002360: 7073 3a2f 2f64 6f63 732e 6164 6170 7465  ps://docs.adapte
-00002370: 7268 7562 2e6d 6c2f 636f 6e74 7269 6275  rhub.ml/contribu
-00002380: 7469 6e67 2e68 746d 6c2e 0d0a 0d0a 2323  ting.html.....##
-00002390: 2043 6974 6174 696f 6e0d 0a0d 0a49 6620   Citation....If 
-000023a0: 796f 7520 7573 6520 5f41 6461 7074 6572  you use _Adapter
-000023b0: 735f 2069 6e20 796f 7572 2077 6f72 6b2c  s_ in your work,
-000023c0: 2070 6c65 6173 6520 636f 6e73 6964 6572   please consider
-000023d0: 2063 6974 696e 6720 6f75 7220 6c69 6272   citing our libr
-000023e0: 6172 7920 7061 7065 723a 205b 4164 6170  ary paper: [Adap
-000023f0: 7465 7273 3a20 4120 556e 6966 6965 6420  ters: A Unified 
-00002400: 4c69 6272 6172 7920 666f 7220 5061 7261  Library for Para
-00002410: 6d65 7465 722d 4566 6669 6369 656e 7420  meter-Efficient 
-00002420: 616e 6420 4d6f 6475 6c61 7220 5472 616e  and Modular Tran
-00002430: 7366 6572 204c 6561 726e 696e 675d 2868  sfer Learning](h
-00002440: 7474 7073 3a2f 2f61 7278 6976 2e6f 7267  ttps://arxiv.org
-00002450: 2f61 6273 2f32 3331 312e 3131 3037 3729  /abs/2311.11077)
-00002460: 0d0a 0d0a 6060 600d 0a40 696e 7072 6f63  ....```..@inproc
-00002470: 6565 6469 6e67 737b 706f 7468 2d65 7461  eedings{poth-eta
-00002480: 6c2d 3230 3233 2d61 6461 7074 6572 732c  l-2023-adapters,
-00002490: 0d0a 2020 2020 7469 746c 6520 3d20 2241  ..    title = "A
-000024a0: 6461 7074 6572 733a 2041 2055 6e69 6669  dapters: A Unifi
-000024b0: 6564 204c 6962 7261 7279 2066 6f72 2050  ed Library for P
-000024c0: 6172 616d 6574 6572 2d45 6666 6963 6965  arameter-Efficie
-000024d0: 6e74 2061 6e64 204d 6f64 756c 6172 2054  nt and Modular T
-000024e0: 7261 6e73 6665 7220 4c65 6172 6e69 6e67  ransfer Learning
-000024f0: 222c 0d0a 2020 2020 6175 7468 6f72 203d  ",..    author =
-00002500: 207b 506f 7468 2c20 436c 6966 746f 6e20   {Poth, Clifton 
-00002510: 2061 6e64 0d0a 2020 2020 2020 5374 6572   and..      Ster
-00002520: 7a2c 2048 616e 6e61 6820 2061 6e64 0d0a  z, Hannah  and..
-00002530: 2020 2020 2020 5061 756c 2c20 496e 6472        Paul, Indr
-00002540: 616e 6569 6c20 2061 6e64 0d0a 2020 2020  aneil  and..    
-00002550: 2020 5075 726b 6179 6173 7468 612c 2053    Purkayastha, S
-00002560: 756b 616e 6e79 6120 2061 6e64 0d0a 2020  ukannya  and..  
-00002570: 2020 2020 456e 676c 7b5c 2261 7d6e 6465      Engl{\"a}nde
-00002580: 722c 204c 656f 6e20 2061 6e64 0d0a 2020  r, Leon  and..  
-00002590: 2020 2020 496d 686f 662c 2054 696d 6f20      Imhof, Timo 
-000025a0: 2061 6e64 0d0a 2020 2020 2020 5675 6c69   and..      Vuli
-000025b0: 7b5c 2763 7d2c 2049 7661 6e20 2061 6e64  {\'c}, Ivan  and
-000025c0: 0d0a 2020 2020 2020 5275 6465 722c 2053  ..      Ruder, S
-000025d0: 6562 6173 7469 616e 2020 616e 640d 0a20  ebastian  and.. 
-000025e0: 2020 2020 2047 7572 6576 7963 682c 2049       Gurevych, I
-000025f0: 7279 6e61 2020 616e 640d 0a20 2020 2020  ryna  and..     
-00002600: 2050 6665 6966 6665 722c 204a 6f6e 6173   Pfeiffer, Jonas
-00002610: 7d2c 0d0a 2020 2020 626f 6f6b 7469 746c  },..    booktitl
-00002620: 6520 3d20 2250 726f 6365 6564 696e 6773  e = "Proceedings
-00002630: 206f 6620 7468 6520 3230 3233 2043 6f6e   of the 2023 Con
-00002640: 6665 7265 6e63 6520 6f6e 2045 6d70 6972  ference on Empir
-00002650: 6963 616c 204d 6574 686f 6473 2069 6e20  ical Methods in 
-00002660: 4e61 7475 7261 6c20 4c61 6e67 7561 6765  Natural Language
-00002670: 2050 726f 6365 7373 696e 673a 2053 7973   Processing: Sys
-00002680: 7465 6d20 4465 6d6f 6e73 7472 6174 696f  tem Demonstratio
-00002690: 6e73 222c 0d0a 2020 2020 6d6f 6e74 6820  ns",..    month 
-000026a0: 3d20 6465 632c 0d0a 2020 2020 7965 6172  = dec,..    year
-000026b0: 203d 2022 3230 3233 222c 0d0a 2020 2020   = "2023",..    
-000026c0: 6164 6472 6573 7320 3d20 2253 696e 6761  address = "Singa
-000026d0: 706f 7265 222c 0d0a 2020 2020 7075 626c  pore",..    publ
-000026e0: 6973 6865 7220 3d20 2241 7373 6f63 6961  isher = "Associa
-000026f0: 7469 6f6e 2066 6f72 2043 6f6d 7075 7461  tion for Computa
-00002700: 7469 6f6e 616c 204c 696e 6775 6973 7469  tional Linguisti
-00002710: 6373 222c 0d0a 2020 2020 7572 6c20 3d20  cs",..    url = 
-00002720: 2268 7474 7073 3a2f 2f61 636c 616e 7468  "https://aclanth
-00002730: 6f6c 6f67 792e 6f72 672f 3230 3233 2e65  ology.org/2023.e
-00002740: 6d6e 6c70 2d64 656d 6f2e 3133 222c 0d0a  mnlp-demo.13",..
-00002750: 2020 2020 7061 6765 7320 3d20 2231 3439      pages = "149
-00002760: 2d2d 3136 3022 2c0d 0a7d 0d0a 6060 600d  --160",..}..```.
-00002770: 0a0d 0a41 6c74 6572 6e61 7469 7665 6c79  ...Alternatively
-00002780: 2c20 666f 7220 7468 6520 7072 6564 6563  , for the predec
-00002790: 6573 736f 7220 6061 6461 7074 6572 2d74  essor `adapter-t
-000027a0: 7261 6e73 666f 726d 6572 7360 2c20 7468  ransformers`, th
-000027b0: 6520 4875 6220 696e 6672 6173 7472 7563  e Hub infrastruc
-000027c0: 7475 7265 2061 6e64 2061 6461 7074 6572  ture and adapter
-000027d0: 7320 7570 6c6f 6164 6564 2062 7920 7468  s uploaded by th
-000027e0: 6520 4164 6170 7465 7248 7562 2074 6561  e AdapterHub tea
-000027f0: 6d2c 2070 6c65 6173 6520 636f 6e73 6964  m, please consid
-00002800: 6572 2063 6974 696e 6720 6f75 7220 696e  er citing our in
-00002810: 6974 6961 6c20 7061 7065 723a 205b 4164  itial paper: [Ad
-00002820: 6170 7465 7248 7562 3a20 4120 4672 616d  apterHub: A Fram
-00002830: 6577 6f72 6b20 666f 7220 4164 6170 7469  ework for Adapti
-00002840: 6e67 2054 7261 6e73 666f 726d 6572 735d  ng Transformers]
-00002850: 2868 7474 7073 3a2f 2f61 7278 6976 2e6f  (https://arxiv.o
-00002860: 7267 2f61 6273 2f32 3030 372e 3037 3737  rg/abs/2007.0777
-00002870: 3929 0d0a 0d0a 6060 600d 0a40 696e 7072  9)....```..@inpr
-00002880: 6f63 6565 6469 6e67 737b 7066 6569 6666  oceedings{pfeiff
-00002890: 6572 3230 3230 4164 6170 7465 7248 7562  er2020AdapterHub
-000028a0: 2c0d 0a20 2020 2074 6974 6c65 3d7b 4164  ,..    title={Ad
-000028b0: 6170 7465 7248 7562 3a20 4120 4672 616d  apterHub: A Fram
-000028c0: 6577 6f72 6b20 666f 7220 4164 6170 7469  ework for Adapti
-000028d0: 6e67 2054 7261 6e73 666f 726d 6572 737d  ng Transformers}
-000028e0: 2c0d 0a20 2020 2061 7574 686f 723d 7b50  ,..    author={P
-000028f0: 6665 6966 6665 722c 204a 6f6e 6173 2061  feiffer, Jonas a
-00002900: 6e64 0d0a 2020 2020 2020 2020 2020 2020  nd..            
-00002910: 527b 5c22 757d 636b 6c7b 5c27 657d 2c20  R{\"u}ckl{\'e}, 
-00002920: 416e 6472 6561 7320 616e 640d 0a20 2020  Andreas and..   
-00002930: 2020 2020 2020 2020 2050 6f74 682c 2043           Poth, C
-00002940: 6c69 6674 6f6e 2061 6e64 0d0a 2020 2020  lifton and..    
-00002950: 2020 2020 2020 2020 4b61 6d61 7468 2c20          Kamath, 
-00002960: 4169 7368 7761 7279 6120 616e 640d 0a20  Aishwarya and.. 
-00002970: 2020 2020 2020 2020 2020 2056 756c 697b             Vuli{
-00002980: 5c27 637d 2c20 4976 616e 2061 6e64 0d0a  \'c}, Ivan and..
-00002990: 2020 2020 2020 2020 2020 2020 5275 6465              Rude
-000029a0: 722c 2053 6562 6173 7469 616e 2061 6e64  r, Sebastian and
-000029b0: 0d0a 2020 2020 2020 2020 2020 2020 4368  ..            Ch
-000029c0: 6f2c 204b 7975 6e67 6879 756e 2061 6e64  o, Kyunghyun and
-000029d0: 0d0a 2020 2020 2020 2020 2020 2020 4775  ..            Gu
-000029e0: 7265 7679 6368 2c20 4972 796e 617d 2c0d  revych, Iryna},.
-000029f0: 0a20 2020 2062 6f6f 6b74 6974 6c65 3d7b  .    booktitle={
-00002a00: 5072 6f63 6565 6469 6e67 7320 6f66 2074  Proceedings of t
-00002a10: 6865 2032 3032 3020 436f 6e66 6572 656e  he 2020 Conferen
-00002a20: 6365 206f 6e20 456d 7069 7269 6361 6c20  ce on Empirical 
-00002a30: 4d65 7468 6f64 7320 696e 204e 6174 7572  Methods in Natur
-00002a40: 616c 204c 616e 6775 6167 6520 5072 6f63  al Language Proc
-00002a50: 6573 7369 6e67 3a20 5379 7374 656d 2044  essing: System D
-00002a60: 656d 6f6e 7374 7261 7469 6f6e 737d 2c0d  emonstrations},.
-00002a70: 0a20 2020 2070 6167 6573 3d7b 3436 2d2d  .    pages={46--
-00002a80: 3534 7d2c 0d0a 2020 2020 7965 6172 3d7b  54},..    year={
-00002a90: 3230 3230 7d0d 0a7d 0d0a 6060 600d 0a    2020}..}..```..
+00000100: 6c3a 2063 616c 7074 406d 6169 6c2e 6465  l: calpt@mail.de
+00000110: 0d0a 4c69 6365 6e73 653a 2041 7061 6368  ..License: Apach
+00000120: 650d 0a4b 6579 776f 7264 733a 204e 4c50  e..Keywords: NLP
+00000130: 2064 6565 7020 6c65 6172 6e69 6e67 2074   deep learning t
+00000140: 7261 6e73 666f 726d 6572 2070 7974 6f72  ransformer pytor
+00000150: 6368 2042 4552 5420 6164 6170 7465 7273  ch BERT adapters
+00000160: 0d0a 436c 6173 7369 6669 6572 3a20 4465  ..Classifier: De
+00000170: 7665 6c6f 706d 656e 7420 5374 6174 7573  velopment Status
+00000180: 203a 3a20 3420 2d20 4265 7461 0d0a 436c   :: 4 - Beta..Cl
+00000190: 6173 7369 6669 6572 3a20 496e 7465 6e64  assifier: Intend
+000001a0: 6564 2041 7564 6965 6e63 6520 3a3a 2044  ed Audience :: D
+000001b0: 6576 656c 6f70 6572 730d 0a43 6c61 7373  evelopers..Class
+000001c0: 6966 6965 723a 2049 6e74 656e 6465 6420  ifier: Intended 
+000001d0: 4175 6469 656e 6365 203a 3a20 4564 7563  Audience :: Educ
+000001e0: 6174 696f 6e0d 0a43 6c61 7373 6966 6965  ation..Classifie
+000001f0: 723a 2049 6e74 656e 6465 6420 4175 6469  r: Intended Audi
+00000200: 656e 6365 203a 3a20 5363 6965 6e63 652f  ence :: Science/
+00000210: 5265 7365 6172 6368 0d0a 436c 6173 7369  Research..Classi
+00000220: 6669 6572 3a20 4c69 6365 6e73 6520 3a3a  fier: License ::
+00000230: 204f 5349 2041 7070 726f 7665 6420 3a3a   OSI Approved ::
+00000240: 2041 7061 6368 6520 536f 6674 7761 7265   Apache Software
+00000250: 204c 6963 656e 7365 0d0a 436c 6173 7369   License..Classi
+00000260: 6669 6572 3a20 4f70 6572 6174 696e 6720  fier: Operating 
+00000270: 5379 7374 656d 203a 3a20 4f53 2049 6e64  System :: OS Ind
+00000280: 6570 656e 6465 6e74 0d0a 436c 6173 7369  ependent..Classi
+00000290: 6669 6572 3a20 5072 6f67 7261 6d6d 696e  fier: Programmin
+000002a0: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
+000002b0: 7468 6f6e 203a 3a20 330d 0a43 6c61 7373  thon :: 3..Class
+000002c0: 6966 6965 723a 2050 726f 6772 616d 6d69  ifier: Programmi
+000002d0: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
+000002e0: 7974 686f 6e20 3a3a 2033 2e38 0d0a 436c  ython :: 3.8..Cl
+000002f0: 6173 7369 6669 6572 3a20 5072 6f67 7261  assifier: Progra
+00000300: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
+00000310: 3a20 5079 7468 6f6e 203a 3a20 332e 390d  : Python :: 3.9.
+00000320: 0a43 6c61 7373 6966 6965 723a 2050 726f  .Classifier: Pro
+00000330: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
+00000340: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
+00000350: 2e31 300d 0a43 6c61 7373 6966 6965 723a  .10..Classifier:
+00000360: 2054 6f70 6963 203a 3a20 5363 6965 6e74   Topic :: Scient
+00000370: 6966 6963 2f45 6e67 696e 6565 7269 6e67  ific/Engineering
+00000380: 203a 3a20 4172 7469 6669 6369 616c 2049   :: Artificial I
+00000390: 6e74 656c 6c69 6765 6e63 650d 0a52 6571  ntelligence..Req
+000003a0: 7569 7265 732d 5079 7468 6f6e 3a20 3e3d  uires-Python: >=
+000003b0: 332e 382e 300d 0a44 6573 6372 6970 7469  3.8.0..Descripti
+000003c0: 6f6e 2d43 6f6e 7465 6e74 2d54 7970 653a  on-Content-Type:
+000003d0: 2074 6578 742f 6d61 726b 646f 776e 0d0a   text/markdown..
+000003e0: 5072 6f76 6964 6573 2d45 7874 7261 3a20  Provides-Extra: 
+000003f0: 736b 6c65 6172 6e0d 0a50 726f 7669 6465  sklearn..Provide
+00000400: 732d 4578 7472 613a 2074 6f72 6368 0d0a  s-Extra: torch..
+00000410: 5072 6f76 6964 6573 2d45 7874 7261 3a20  Provides-Extra: 
+00000420: 6f6e 6e78 7275 6e74 696d 650d 0a50 726f  onnxruntime..Pro
+00000430: 7669 6465 732d 4578 7472 613a 2073 656e  vides-Extra: sen
+00000440: 7465 6e63 6570 6965 6365 0d0a 5072 6f76  tencepiece..Prov
+00000450: 6964 6573 2d45 7874 7261 3a20 7465 7374  ides-Extra: test
+00000460: 696e 670d 0a50 726f 7669 6465 732d 4578  ing..Provides-Ex
+00000470: 7472 613a 2071 7561 6c69 7479 0d0a 5072  tra: quality..Pr
+00000480: 6f76 6964 6573 2d45 7874 7261 3a20 646f  ovides-Extra: do
+00000490: 6373 0d0a 5072 6f76 6964 6573 2d45 7874  cs..Provides-Ext
+000004a0: 7261 3a20 6465 760d 0a4c 6963 656e 7365  ra: dev..License
+000004b0: 2d46 696c 653a 204c 4943 454e 5345 0d0a  -File: LICENSE..
+000004c0: 0d0a 3c21 2d2d 2d0d 0a43 6f70 7972 6967  ..<!---..Copyrig
+000004d0: 6874 2032 3032 3020 5468 6520 4164 6170  ht 2020 The Adap
+000004e0: 7465 7248 7562 2054 6561 6d2e 2041 6c6c  terHub Team. All
+000004f0: 2072 6967 6874 7320 7265 7365 7276 6564   rights reserved
+00000500: 2e0d 0a0d 0a4c 6963 656e 7365 6420 756e  .....Licensed un
+00000510: 6465 7220 7468 6520 4170 6163 6865 204c  der the Apache L
+00000520: 6963 656e 7365 2c20 5665 7273 696f 6e20  icense, Version 
+00000530: 322e 3020 2874 6865 2022 4c69 6365 6e73  2.0 (the "Licens
+00000540: 6522 293b 0d0a 796f 7520 6d61 7920 6e6f  e");..you may no
+00000550: 7420 7573 6520 7468 6973 2066 696c 6520  t use this file 
+00000560: 6578 6365 7074 2069 6e20 636f 6d70 6c69  except in compli
+00000570: 616e 6365 2077 6974 6820 7468 6520 4c69  ance with the Li
+00000580: 6365 6e73 652e 0d0a 596f 7520 6d61 7920  cense...You may 
+00000590: 6f62 7461 696e 2061 2063 6f70 7920 6f66  obtain a copy of
+000005a0: 2074 6865 204c 6963 656e 7365 2061 740d   the License at.
+000005b0: 0a0d 0a20 2020 2068 7474 703a 2f2f 7777  ...    http://ww
+000005c0: 772e 6170 6163 6865 2e6f 7267 2f6c 6963  w.apache.org/lic
+000005d0: 656e 7365 732f 4c49 4345 4e53 452d 322e  enses/LICENSE-2.
+000005e0: 300d 0a0d 0a55 6e6c 6573 7320 7265 7175  0....Unless requ
+000005f0: 6972 6564 2062 7920 6170 706c 6963 6162  ired by applicab
+00000600: 6c65 206c 6177 206f 7220 6167 7265 6564  le law or agreed
+00000610: 2074 6f20 696e 2077 7269 7469 6e67 2c20   to in writing, 
+00000620: 736f 6674 7761 7265 0d0a 6469 7374 7269  software..distri
+00000630: 6275 7465 6420 756e 6465 7220 7468 6520  buted under the 
+00000640: 4c69 6365 6e73 6520 6973 2064 6973 7472  License is distr
+00000650: 6962 7574 6564 206f 6e20 616e 2022 4153  ibuted on an "AS
+00000660: 2049 5322 2042 4153 4953 2c0d 0a57 4954   IS" BASIS,..WIT
+00000670: 484f 5554 2057 4152 5241 4e54 4945 5320  HOUT WARRANTIES 
+00000680: 4f52 2043 4f4e 4449 5449 4f4e 5320 4f46  OR CONDITIONS OF
+00000690: 2041 4e59 204b 494e 442c 2065 6974 6865   ANY KIND, eithe
+000006a0: 7220 6578 7072 6573 7320 6f72 2069 6d70  r express or imp
+000006b0: 6c69 6564 2e0d 0a53 6565 2074 6865 204c  lied...See the L
+000006c0: 6963 656e 7365 2066 6f72 2074 6865 2073  icense for the s
+000006d0: 7065 6369 6669 6320 6c61 6e67 7561 6765  pecific language
+000006e0: 2067 6f76 6572 6e69 6e67 2070 6572 6d69   governing permi
+000006f0: 7373 696f 6e73 2061 6e64 0d0a 6c69 6d69  ssions and..limi
+00000700: 7461 7469 6f6e 7320 756e 6465 7220 7468  tations under th
+00000710: 6520 4c69 6365 6e73 652e 0d0a 2d2d 3e0d  e License...-->.
+00000720: 0a0d 0a3c 7020 616c 6967 6e3d 2263 656e  ...<p align="cen
+00000730: 7465 7222 3e0d 0a3c 696d 6720 7374 796c  ter">..<img styl
+00000740: 653d 2276 6572 7469 6361 6c2d 616c 6967  e="vertical-alig
+00000750: 6e3a 6d69 6464 6c65 2220 7372 633d 2268  n:middle" src="h
+00000760: 7474 7073 3a2f 2f72 6177 2e67 6974 6875  ttps://raw.githu
+00000770: 6275 7365 7263 6f6e 7465 6e74 2e63 6f6d  busercontent.com
+00000780: 2f41 6461 7074 6572 2d48 7562 2f61 6461  /Adapter-Hub/ada
+00000790: 7074 6572 732f 6d61 696e 2f64 6f63 732f  pters/main/docs/
+000007a0: 696d 672f 6164 6170 7465 722d 6265 7274  img/adapter-bert
+000007b0: 2e70 6e67 2220 7769 6474 683d 2238 3022  .png" width="80"
+000007c0: 202f 3e0d 0a3c 2f70 3e0d 0a3c 6831 2061   />..</p>..<h1 a
+000007d0: 6c69 676e 3d22 6365 6e74 6572 223e 0d0a  lign="center">..
+000007e0: 3c73 7061 6e3e 3c69 3e41 6461 7074 6572  <span><i>Adapter
+000007f0: 733c 2f69 3e3c 2f73 7061 6e3e 0d0a 3c2f  s</i></span>..</
+00000800: 6831 3e0d 0a0d 0a3c 6833 2061 6c69 676e  h1>....<h3 align
+00000810: 3d22 6365 6e74 6572 223e 0d0a 4120 556e  ="center">..A Un
+00000820: 6966 6965 6420 4c69 6272 6172 7920 666f  ified Library fo
+00000830: 7220 5061 7261 6d65 7465 722d 4566 6669  r Parameter-Effi
+00000840: 6369 656e 7420 616e 6420 4d6f 6475 6c61  cient and Modula
+00000850: 7220 5472 616e 7366 6572 204c 6561 726e  r Transfer Learn
+00000860: 696e 670d 0a3c 2f68 333e 0d0a 3c68 3320  ing..</h3>..<h3 
+00000870: 616c 6967 6e3d 2263 656e 7465 7222 3e0d  align="center">.
+00000880: 0a20 2020 203c 6120 6872 6566 3d22 6874  .    <a href="ht
+00000890: 7470 733a 2f2f 6164 6170 7465 7268 7562  tps://adapterhub
+000008a0: 2e6d 6c22 3e57 6562 7369 7465 3c2f 613e  .ml">Website</a>
+000008b0: 0d0a 2020 2020 266e 6273 703b 20e2 80a2  ..    &nbsp; ...
+000008c0: 2026 6e62 7370 3b0d 0a20 2020 203c 6120   &nbsp;..    <a 
+000008d0: 6872 6566 3d22 6874 7470 733a 2f2f 646f  href="https://do
+000008e0: 6373 2e61 6461 7074 6572 6875 622e 6d6c  cs.adapterhub.ml
+000008f0: 223e 446f 6375 6d65 6e74 6174 696f 6e3c  ">Documentation<
+00000900: 2f61 3e0d 0a20 2020 2026 6e62 7370 3b20  /a>..    &nbsp; 
+00000910: e280 a220 266e 6273 703b 0d0a 2020 2020  ... &nbsp;..    
+00000920: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
+00000930: 2f61 7278 6976 2e6f 7267 2f61 6273 2f32  /arxiv.org/abs/2
+00000940: 3331 312e 3131 3037 3722 3e50 6170 6572  311.11077">Paper
+00000950: 3c2f 613e 0d0a 3c2f 6833 3e0d 0a0d 0a21  </a>..</h3>....!
+00000960: 5b54 6573 7473 5d28 6874 7470 733a 2f2f  [Tests](https://
+00000970: 6769 7468 7562 2e63 6f6d 2f41 6461 7074  github.com/Adapt
+00000980: 6572 2d48 7562 2f61 6461 7074 6572 732f  er-Hub/adapters/
+00000990: 776f 726b 666c 6f77 732f 5465 7374 732f  workflows/Tests/
+000009a0: 6261 6467 652e 7376 673f 6272 616e 6368  badge.svg?branch
+000009b0: 3d61 6461 7074 6572 7329 0d0a 5b21 5b47  =adapters)..[![G
+000009c0: 6974 4875 625d 2868 7474 7073 3a2f 2f69  itHub](https://i
+000009d0: 6d67 2e73 6869 656c 6473 2e69 6f2f 6769  mg.shields.io/gi
+000009e0: 7468 7562 2f6c 6963 656e 7365 2f61 6461  thub/license/ada
+000009f0: 7074 6572 2d68 7562 2f61 6461 7074 6572  pter-hub/adapter
+00000a00: 732e 7376 673f 636f 6c6f 723d 626c 7565  s.svg?color=blue
+00000a10: 295d 2868 7474 7073 3a2f 2f67 6974 6875  )](https://githu
+00000a20: 622e 636f 6d2f 6164 6170 7465 722d 6875  b.com/adapter-hu
+00000a30: 622f 6164 6170 7465 7273 2f62 6c6f 622f  b/adapters/blob/
+00000a40: 6d61 696e 2f4c 4943 454e 5345 290d 0a5b  main/LICENSE)..[
+00000a50: 215b 5079 5049 5d28 6874 7470 733a 2f2f  ![PyPI](https://
+00000a60: 696d 672e 7368 6965 6c64 732e 696f 2f70  img.shields.io/p
+00000a70: 7970 692f 762f 6164 6170 7465 7273 295d  ypi/v/adapters)]
+00000a80: 2868 7474 7073 3a2f 2f70 7970 692e 6f72  (https://pypi.or
+00000a90: 672f 7072 6f6a 6563 742f 6164 6170 7465  g/project/adapte
+00000aa0: 7273 2f29 0d0a 0d0a 5f41 6461 7074 6572  rs/)...._Adapter
+00000ab0: 735f 2069 7320 616e 2061 6464 2d6f 6e20  s_ is an add-on 
+00000ac0: 6c69 6272 6172 7920 746f 205b 4875 6767  library to [Hugg
+00000ad0: 696e 6746 6163 6527 7320 5472 616e 7366  ingFace's Transf
+00000ae0: 6f72 6d65 7273 5d28 6874 7470 733a 2f2f  ormers](https://
+00000af0: 6769 7468 7562 2e63 6f6d 2f68 7567 6769  github.com/huggi
+00000b00: 6e67 6661 6365 2f74 7261 6e73 666f 726d  ngface/transform
+00000b10: 6572 7329 2c20 696e 7465 6772 6174 696e  ers), integratin
+00000b20: 6720 5b76 6172 696f 7573 2061 6461 7074  g [various adapt
+00000b30: 6572 206d 6574 686f 6473 5d28 6874 7470  er methods](http
+00000b40: 733a 2f2f 646f 6373 2e61 6461 7074 6572  s://docs.adapter
+00000b50: 6875 622e 6d6c 2f6f 7665 7276 6965 772e  hub.ml/overview.
+00000b60: 6874 6d6c 2920 696e 746f 205b 7374 6174  html) into [stat
+00000b70: 652d 6f66 2d74 6865 2d61 7274 2070 7265  e-of-the-art pre
+00000b80: 2d74 7261 696e 6564 206c 616e 6775 6167  -trained languag
+00000b90: 6520 6d6f 6465 6c73 5d28 6874 7470 733a  e models](https:
+00000ba0: 2f2f 646f 6373 2e61 6461 7074 6572 6875  //docs.adapterhu
+00000bb0: 622e 6d6c 2f6d 6f64 656c 5f6f 7665 7276  b.ml/model_overv
+00000bc0: 6965 772e 6874 6d6c 2920 7769 7468 206d  iew.html) with m
+00000bd0: 696e 696d 616c 2063 6f64 696e 6720 6f76  inimal coding ov
+00000be0: 6572 6865 6164 2066 6f72 2074 7261 696e  erhead for train
+00000bf0: 696e 6720 616e 6420 696e 6665 7265 6e63  ing and inferenc
+00000c00: 652e 0d0a 0d0a 3e20 2a2a 4e6f 7465 2a2a  e.....> **Note**
+00000c10: 3a20 5468 6520 5f41 6461 7074 6572 735f  : The _Adapters_
+00000c20: 206c 6962 7261 7279 2068 6173 2072 6570   library has rep
+00000c30: 6c61 6365 6420 7468 6520 6061 6461 7074  laced the `adapt
+00000c40: 6572 2d74 7261 6e73 666f 726d 6572 7360  er-transformers`
+00000c50: 2070 6163 6b61 6765 2e20 416c 6c20 7072   package. All pr
+00000c60: 6576 696f 7573 6c79 2074 7261 696e 6564  eviously trained
+00000c70: 2061 6461 7074 6572 7320 6172 6520 636f   adapters are co
+00000c80: 6d70 6174 6962 6c65 2077 6974 6820 7468  mpatible with th
+00000c90: 6520 6e65 7720 6c69 6272 6172 792e 2046  e new library. F
+00000ca0: 6f72 2074 7261 6e73 6974 696f 6e69 6e67  or transitioning
+00000cb0: 2c20 706c 6561 7365 2072 6561 643a 2068  , please read: h
+00000cc0: 7474 7073 3a2f 2f64 6f63 732e 6164 6170  ttps://docs.adap
+00000cd0: 7465 7268 7562 2e6d 6c2f 7472 616e 7369  terhub.ml/transi
+00000ce0: 7469 6f6e 696e 672e 6874 6d6c 2e0d 0a0d  tioning.html....
+00000cf0: 0a23 2320 496e 7374 616c 6c61 7469 6f6e  .## Installation
+00000d00: 0d0a 0d0a 6061 6461 7074 6572 7360 2063  ....`adapters` c
+00000d10: 7572 7265 6e74 6c79 2073 7570 706f 7274  urrently support
+00000d20: 7320 2a2a 5079 7468 6f6e 2033 2e38 2b2a  s **Python 3.8+*
+00000d30: 2a20 616e 6420 2a2a 5079 546f 7263 6820  * and **PyTorch 
+00000d40: 312e 3130 2b2a 2a2e 0d0a 4166 7465 7220  1.10+**...After 
+00000d50: 5b69 6e73 7461 6c6c 696e 6720 5079 546f  [installing PyTo
+00000d60: 7263 685d 2868 7474 7073 3a2f 2f70 7974  rch](https://pyt
+00000d70: 6f72 6368 2e6f 7267 2f67 6574 2d73 7461  orch.org/get-sta
+00000d80: 7274 6564 2f6c 6f63 616c 6c79 2f29 2c20  rted/locally/), 
+00000d90: 796f 7520 6361 6e20 696e 7374 616c 6c20  you can install 
+00000da0: 6061 6461 7074 6572 7360 2066 726f 6d20  `adapters` from 
+00000db0: 5079 5049 202e 2e2e 0d0a 0d0a 6060 600d  PyPI .......```.
+00000dc0: 0a70 6970 2069 6e73 7461 6c6c 202d 5520  .pip install -U 
+00000dd0: 6164 6170 7465 7273 0d0a 6060 600d 0a0d  adapters..```...
+00000de0: 0a2e 2e2e 206f 7220 6672 6f6d 2073 6f75  .... or from sou
+00000df0: 7263 6520 6279 2063 6c6f 6e69 6e67 2074  rce by cloning t
+00000e00: 6865 2072 6570 6f73 6974 6f72 793a 0d0a  he repository:..
+00000e10: 0d0a 6060 600d 0a67 6974 2063 6c6f 6e65  ..```..git clone
+00000e20: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
+00000e30: 636f 6d2f 6164 6170 7465 722d 6875 622f  com/adapter-hub/
+00000e40: 6164 6170 7465 7273 2e67 6974 0d0a 6364  adapters.git..cd
+00000e50: 2061 6461 7074 6572 730d 0a70 6970 2069   adapters..pip i
+00000e60: 6e73 7461 6c6c 202e 0d0a 6060 600d 0a0d  nstall ...```...
+00000e70: 0a23 2320 5175 6963 6b20 546f 7572 0d0a  .## Quick Tour..
+00000e80: 0d0a 2323 2323 204c 6f61 6420 7072 652d  ..#### Load pre-
+00000e90: 7472 6169 6e65 6420 6164 6170 7465 7273  trained adapters
+00000ea0: 3a0d 0a0d 0a60 6060 7079 7468 6f6e 0d0a  :....```python..
+00000eb0: 6672 6f6d 2061 6461 7074 6572 7320 696d  from adapters im
+00000ec0: 706f 7274 2041 7574 6f41 6461 7074 6572  port AutoAdapter
+00000ed0: 4d6f 6465 6c0d 0a66 726f 6d20 7472 616e  Model..from tran
+00000ee0: 7366 6f72 6d65 7273 2069 6d70 6f72 7420  sformers import 
+00000ef0: 4175 746f 546f 6b65 6e69 7a65 720d 0a0d  AutoTokenizer...
+00000f00: 0a6d 6f64 656c 203d 2041 7574 6f41 6461  .model = AutoAda
+00000f10: 7074 6572 4d6f 6465 6c2e 6672 6f6d 5f70  pterModel.from_p
+00000f20: 7265 7472 6169 6e65 6428 2272 6f62 6572  retrained("rober
+00000f30: 7461 2d62 6173 6522 290d 0a74 6f6b 656e  ta-base")..token
+00000f40: 697a 6572 203d 2041 7574 6f54 6f6b 656e  izer = AutoToken
+00000f50: 697a 6572 2e66 726f 6d5f 7072 6574 7261  izer.from_pretra
+00000f60: 696e 6564 2822 726f 6265 7274 612d 6261  ined("roberta-ba
+00000f70: 7365 2229 0d0a 0d0a 6d6f 6465 6c2e 6c6f  se")....model.lo
+00000f80: 6164 5f61 6461 7074 6572 2822 4164 6170  ad_adapter("Adap
+00000f90: 7465 7248 7562 2f72 6f62 6572 7461 2d62  terHub/roberta-b
+00000fa0: 6173 652d 7066 2d69 6d64 6222 2c20 736f  ase-pf-imdb", so
+00000fb0: 7572 6365 3d22 6866 222c 2073 6574 5f61  urce="hf", set_a
+00000fc0: 6374 6976 653d 5472 7565 290d 0a0d 0a70  ctive=True)....p
+00000fd0: 7269 6e74 286d 6f64 656c 282a 2a74 6f6b  rint(model(**tok
+00000fe0: 656e 697a 6572 2822 5468 6973 2077 6f72  enizer("This wor
+00000ff0: 6b73 2067 7265 6174 2122 2c20 7265 7475  ks great!", retu
+00001000: 726e 5f74 656e 736f 7273 3d22 7074 2229  rn_tensors="pt")
+00001010: 292e 6c6f 6769 7473 290d 0a60 6060 0d0a  ).logits)..```..
+00001020: 0d0a 2a2a 5b4c 6561 726e 204d 6f72 655d  ..**[Learn More]
+00001030: 2868 7474 7073 3a2f 2f64 6f63 732e 6164  (https://docs.ad
+00001040: 6170 7465 7268 7562 2e6d 6c2f 6c6f 6164  apterhub.ml/load
+00001050: 696e 672e 6874 6d6c 292a 2a0d 0a0d 0a23  ing.html)**....#
+00001060: 2323 2320 4164 6170 7420 6578 6973 7469  ### Adapt existi
+00001070: 6e67 206d 6f64 656c 2073 6574 7570 733a  ng model setups:
+00001080: 0d0a 0d0a 6060 6070 7974 686f 6e0d 0a69  ....```python..i
+00001090: 6d70 6f72 7420 6164 6170 7465 7273 0d0a  mport adapters..
+000010a0: 6672 6f6d 2074 7261 6e73 666f 726d 6572  from transformer
+000010b0: 7320 696d 706f 7274 2041 7574 6f4d 6f64  s import AutoMod
+000010c0: 656c 466f 7253 6571 7565 6e63 6543 6c61  elForSequenceCla
+000010d0: 7373 6966 6963 6174 696f 6e0d 0a0d 0a6d  ssification....m
+000010e0: 6f64 656c 203d 2041 7574 6f4d 6f64 656c  odel = AutoModel
+000010f0: 466f 7253 6571 7565 6e63 6543 6c61 7373  ForSequenceClass
+00001100: 6966 6963 6174 696f 6e2e 6672 6f6d 5f70  ification.from_p
+00001110: 7265 7472 6169 6e65 6428 2274 352d 6261  retrained("t5-ba
+00001120: 7365 2229 0d0a 0d0a 6164 6170 7465 7273  se")....adapters
+00001130: 2e69 6e69 7428 6d6f 6465 6c29 0d0a 0d0a  .init(model)....
+00001140: 6d6f 6465 6c2e 6164 645f 6164 6170 7465  model.add_adapte
+00001150: 7228 226d 795f 6c6f 7261 5f61 6461 7074  r("my_lora_adapt
+00001160: 6572 222c 2063 6f6e 6669 673d 226c 6f72  er", config="lor
+00001170: 6122 290d 0a6d 6f64 656c 2e74 7261 696e  a")..model.train
+00001180: 5f61 6461 7074 6572 2822 6d79 5f6c 6f72  _adapter("my_lor
+00001190: 615f 6164 6170 7465 7222 290d 0a0d 0a23  a_adapter")....#
+000011a0: 2059 6f75 7220 7265 6775 6c61 7220 7472   Your regular tr
+000011b0: 6169 6e69 6e67 206c 6f6f 702e 2e2e 0d0a  aining loop.....
+000011c0: 6060 600d 0a0d 0a2a 2a5b 4c65 6172 6e20  ```....**[Learn 
+000011d0: 4d6f 7265 5d28 6874 7470 733a 2f2f 646f  More](https://do
+000011e0: 6373 2e61 6461 7074 6572 6875 622e 6d6c  cs.adapterhub.ml
+000011f0: 2f71 7569 636b 7374 6172 742e 6874 6d6c  /quickstart.html
+00001200: 292a 2a0d 0a0d 0a23 2323 2320 466c 6578  )**....#### Flex
+00001210: 6962 6c79 2063 6f6e 6669 6775 7265 2061  ibly configure a
+00001220: 6461 7074 6572 733a 0d0a 0d0a 6060 6070  dapters:....```p
+00001230: 7974 686f 6e0d 0a66 726f 6d20 6164 6170  ython..from adap
+00001240: 7465 7273 2069 6d70 6f72 7420 436f 6e66  ters import Conf
+00001250: 6967 556e 696f 6e2c 2050 7265 6669 7854  igUnion, PrefixT
+00001260: 756e 696e 6743 6f6e 6669 672c 2050 6172  uningConfig, Par
+00001270: 426e 436f 6e66 6967 2c20 4175 746f 4164  BnConfig, AutoAd
+00001280: 6170 7465 724d 6f64 656c 0d0a 0d0a 6d6f  apterModel....mo
+00001290: 6465 6c20 3d20 4175 746f 4164 6170 7465  del = AutoAdapte
+000012a0: 724d 6f64 656c 2e66 726f 6d5f 7072 6574  rModel.from_pret
+000012b0: 7261 696e 6564 2822 6d69 6372 6f73 6f66  rained("microsof
+000012c0: 742f 6465 6265 7274 612d 7633 2d62 6173  t/deberta-v3-bas
+000012d0: 6522 290d 0a0d 0a61 6461 7074 6572 5f63  e")....adapter_c
+000012e0: 6f6e 6669 6720 3d20 436f 6e66 6967 556e  onfig = ConfigUn
+000012f0: 696f 6e28 0d0a 2020 2020 5072 6566 6978  ion(..    Prefix
+00001300: 5475 6e69 6e67 436f 6e66 6967 2870 7265  TuningConfig(pre
+00001310: 6669 785f 6c65 6e67 7468 3d32 3029 2c0d  fix_length=20),.
+00001320: 0a20 2020 2050 6172 426e 436f 6e66 6967  .    ParBnConfig
+00001330: 2872 6564 7563 7469 6f6e 5f66 6163 746f  (reduction_facto
+00001340: 723d 3429 2c0d 0a29 0d0a 6d6f 6465 6c2e  r=4),..)..model.
+00001350: 6164 645f 6164 6170 7465 7228 226d 795f  add_adapter("my_
+00001360: 6164 6170 7465 7222 2c20 636f 6e66 6967  adapter", config
+00001370: 3d61 6461 7074 6572 5f63 6f6e 6669 672c  =adapter_config,
+00001380: 2073 6574 5f61 6374 6976 653d 5472 7565   set_active=True
+00001390: 290d 0a60 6060 0d0a 0d0a 2a2a 5b4c 6561  )..```....**[Lea
+000013a0: 726e 204d 6f72 655d 2868 7474 7073 3a2f  rn More](https:/
+000013b0: 2f64 6f63 732e 6164 6170 7465 7268 7562  /docs.adapterhub
+000013c0: 2e6d 6c2f 6f76 6572 7669 6577 2e68 746d  .ml/overview.htm
+000013d0: 6c29 2a2a 0d0a 0d0a 2323 2323 2045 6173  l)**....#### Eas
+000013e0: 696c 7920 636f 6d70 6f73 6520 6164 6170  ily compose adap
+000013f0: 7465 7273 2069 6e20 6120 7369 6e67 6c65  ters in a single
+00001400: 206d 6f64 656c 3a0d 0a0d 0a60 6060 7079   model:....```py
+00001410: 7468 6f6e 0d0a 6672 6f6d 2061 6461 7074  thon..from adapt
+00001420: 6572 7320 696d 706f 7274 2041 6461 7074  ers import Adapt
+00001430: 6572 5365 7475 702c 2041 7574 6f41 6461  erSetup, AutoAda
+00001440: 7074 6572 4d6f 6465 6c0d 0a69 6d70 6f72  pterModel..impor
+00001450: 7420 6164 6170 7465 7273 2e63 6f6d 706f  t adapters.compo
+00001460: 7369 7469 6f6e 2061 7320 6163 0d0a 0d0a  sition as ac....
+00001470: 6d6f 6465 6c20 3d20 4175 746f 4164 6170  model = AutoAdap
+00001480: 7465 724d 6f64 656c 2e66 726f 6d5f 7072  terModel.from_pr
+00001490: 6574 7261 696e 6564 2822 726f 6265 7274  etrained("robert
+000014a0: 612d 6261 7365 2229 0d0a 0d0a 7163 203d  a-base")....qc =
+000014b0: 206d 6f64 656c 2e6c 6f61 645f 6164 6170   model.load_adap
+000014c0: 7465 7228 2241 6461 7074 6572 4875 622f  ter("AdapterHub/
+000014d0: 726f 6265 7274 612d 6261 7365 2d70 662d  roberta-base-pf-
+000014e0: 7472 6563 2229 0d0a 7365 6e74 203d 206d  trec")..sent = m
+000014f0: 6f64 656c 2e6c 6f61 645f 6164 6170 7465  odel.load_adapte
+00001500: 7228 2241 6461 7074 6572 4875 622f 726f  r("AdapterHub/ro
+00001510: 6265 7274 612d 6261 7365 2d70 662d 696d  berta-base-pf-im
+00001520: 6462 2229 0d0a 0d0a 7769 7468 2041 6461  db")....with Ada
+00001530: 7074 6572 5365 7475 7028 6163 2e50 6172  pterSetup(ac.Par
+00001540: 616c 6c65 6c28 7163 2c20 7365 6e74 2929  allel(qc, sent))
+00001550: 3a0d 0a20 2020 2070 7269 6e74 286d 6f64  :..    print(mod
+00001560: 656c 282a 2a74 6f6b 656e 697a 6572 2822  el(**tokenizer("
+00001570: 5768 6174 2069 7320 4164 6170 7465 7248  What is AdapterH
+00001580: 7562 3f22 2c20 7265 7475 726e 5f74 656e  ub?", return_ten
+00001590: 736f 7273 3d22 7074 2229 2929 0d0a 6060  sors="pt")))..``
+000015a0: 600d 0a0d 0a2a 2a5b 4c65 6172 6e20 4d6f  `....**[Learn Mo
+000015b0: 7265 5d28 6874 7470 733a 2f2f 646f 6373  re](https://docs
+000015c0: 2e61 6461 7074 6572 6875 622e 6d6c 2f61  .adapterhub.ml/a
+000015d0: 6461 7074 6572 5f63 6f6d 706f 7369 7469  dapter_compositi
+000015e0: 6f6e 2e68 746d 6c29 2a2a 0d0a 0d0a 2323  on.html)**....##
+000015f0: 2055 7365 6675 6c20 5265 736f 7572 6365   Useful Resource
+00001600: 730d 0a0d 0a48 7567 6769 6e67 4661 6365  s....HuggingFace
+00001610: 2773 2067 7265 6174 2064 6f63 756d 656e  's great documen
+00001620: 7461 7469 6f6e 206f 6e20 6765 7474 696e  tation on gettin
+00001630: 6720 7374 6172 7465 6420 7769 7468 205f  g started with _
+00001640: 5472 616e 7366 6f72 6d65 7273 5f20 6361  Transformers_ ca
+00001650: 6e20 6265 2066 6f75 6e64 205b 6865 7265  n be found [here
+00001660: 5d28 6874 7470 733a 2f2f 6875 6767 696e  ](https://huggin
+00001670: 6766 6163 652e 636f 2f74 7261 6e73 666f  gface.co/transfo
+00001680: 726d 6572 732f 696e 6465 782e 6874 6d6c  rmers/index.html
+00001690: 292e 2060 6164 6170 7465 7273 6020 6973  ). `adapters` is
+000016a0: 2066 756c 6c79 2063 6f6d 7061 7469 626c   fully compatibl
+000016b0: 6520 7769 7468 205f 5472 616e 7366 6f72  e with _Transfor
+000016c0: 6d65 7273 5f2e 0d0a 0d0a 546f 2067 6574  mers_.....To get
+000016d0: 2073 7461 7274 6564 2077 6974 6820 6164   started with ad
+000016e0: 6170 7465 7273 2c20 7265 6665 7220 746f  apters, refer to
+000016f0: 2074 6865 7365 206c 6f63 6174 696f 6e73   these locations
+00001700: 3a0d 0a0d 0a2d 202a 2a5b 436f 6c61 6220  :....- **[Colab 
+00001710: 6e6f 7465 626f 6f6b 2074 7574 6f72 6961  notebook tutoria
+00001720: 6c73 5d28 6874 7470 733a 2f2f 6769 7468  ls](https://gith
+00001730: 7562 2e63 6f6d 2f41 6461 7074 6572 2d48  ub.com/Adapter-H
+00001740: 7562 2f61 6461 7074 6572 732f 7472 6565  ub/adapters/tree
+00001750: 2f6d 6169 6e2f 6e6f 7465 626f 6f6b 7329  /main/notebooks)
+00001760: 2a2a 2c20 6120 7365 7269 6573 206e 6f74  **, a series not
+00001770: 6562 6f6f 6b73 2070 726f 7669 6469 6e67  ebooks providing
+00001780: 2061 6e20 696e 7472 6f64 7563 7469 6f6e   an introduction
+00001790: 2074 6f20 616c 6c20 7468 6520 6d61 696e   to all the main
+000017a0: 2063 6f6e 6365 7074 7320 6f66 2028 6164   concepts of (ad
+000017b0: 6170 7465 722d 2974 7261 6e73 666f 726d  apter-)transform
+000017c0: 6572 7320 616e 6420 4164 6170 7465 7248  ers and AdapterH
+000017d0: 7562 0d0a 2d20 2a2a 6874 7470 733a 2f2f  ub..- **https://
+000017e0: 646f 6373 2e61 6461 7074 6572 6875 622e  docs.adapterhub.
+000017f0: 6d6c 2a2a 2c20 6f75 7220 646f 6375 6d65  ml**, our docume
+00001800: 6e74 6174 696f 6e20 6f6e 2074 7261 696e  ntation on train
+00001810: 696e 6720 616e 6420 7573 696e 6720 6164  ing and using ad
+00001820: 6170 7465 7273 2077 6974 6820 5f61 6461  apters with _ada
+00001830: 7074 6572 735f 0d0a 2d20 2a2a 6874 7470  pters_..- **http
+00001840: 733a 2f2f 6164 6170 7465 7268 7562 2e6d  s://adapterhub.m
+00001850: 6c2a 2a20 746f 2065 7870 6c6f 7265 2061  l** to explore a
+00001860: 7661 696c 6162 6c65 2070 7265 2d74 7261  vailable pre-tra
+00001870: 696e 6564 2061 6461 7074 6572 206d 6f64  ined adapter mod
+00001880: 756c 6573 2061 6e64 2073 6861 7265 2079  ules and share y
+00001890: 6f75 7220 6f77 6e20 6164 6170 7465 7273  our own adapters
+000018a0: 0d0a 2d20 2a2a 5b45 7861 6d70 6c65 7320  ..- **[Examples 
+000018b0: 666f 6c64 6572 5d28 6874 7470 733a 2f2f  folder](https://
+000018c0: 6769 7468 7562 2e63 6f6d 2f41 6461 7074  github.com/Adapt
+000018d0: 6572 2d48 7562 2f61 6461 7074 6572 732f  er-Hub/adapters/
+000018e0: 7472 6565 2f6d 6169 6e2f 6578 616d 706c  tree/main/exampl
+000018f0: 6573 2f70 7974 6f72 6368 292a 2a20 6f66  es/pytorch)** of
+00001900: 2074 6869 7320 7265 706f 7369 746f 7279   this repository
+00001910: 2063 6f6e 7461 696e 696e 6720 4875 6767   containing Hugg
+00001920: 696e 6746 6163 6527 7320 6578 616d 706c  ingFace's exampl
+00001930: 6520 7472 6169 6e69 6e67 2073 6372 6970  e training scrip
+00001940: 7473 2c20 6d61 6e79 2061 6461 7074 6564  ts, many adapted
+00001950: 2066 6f72 2074 7261 696e 696e 6720 6164   for training ad
+00001960: 6170 7465 7273 0d0a 0d0a 2323 2049 6d70  apters....## Imp
+00001970: 6c65 6d65 6e74 6564 204d 6574 686f 6473  lemented Methods
+00001980: 0d0a 0d0a 4375 7272 656e 746c 792c 2061  ....Currently, a
+00001990: 6461 7074 6572 7320 696e 7465 6772 6174  dapters integrat
+000019a0: 6573 2061 6c6c 2061 7263 6869 7465 6374  es all architect
+000019b0: 7572 6573 2061 6e64 206d 6574 686f 6473  ures and methods
+000019c0: 206c 6973 7465 6420 6265 6c6f 773a 0d0a   listed below:..
+000019d0: 0d0a 7c20 4d65 7468 6f64 207c 2050 6170  ..| Method | Pap
+000019e0: 6572 2873 2920 7c20 5175 6963 6b20 4c69  er(s) | Quick Li
+000019f0: 6e6b 7320 7c0d 0a7c 202d 2d2d 207c 202d  nks |..| --- | -
+00001a00: 2d2d 207c 202d 2d2d 207c 0d0a 7c20 426f  -- | --- |..| Bo
+00001a10: 7474 6c65 6e65 636b 2061 6461 7074 6572  ttleneck adapter
+00001a20: 7320 7c20 5b48 6f75 6c73 6279 2065 7420  s | [Houlsby et 
+00001a30: 616c 2e20 2832 3031 3929 5d28 6874 7470  al. (2019)](http
+00001a40: 733a 2f2f 6172 7869 762e 6f72 672f 7064  s://arxiv.org/pd
+00001a50: 662f 3139 3032 2e30 3037 3531 2e70 6466  f/1902.00751.pdf
+00001a60: 293c 6272 3e20 5b42 6170 6e61 2061 6e64  )<br> [Bapna and
+00001a70: 2046 6972 6174 2028 3230 3139 295d 2868   Firat (2019)](h
+00001a80: 7474 7073 3a2f 2f61 7278 6976 2e6f 7267  ttps://arxiv.org
+00001a90: 2f70 6466 2f31 3930 392e 3038 3437 382e  /pdf/1909.08478.
+00001aa0: 7064 6629 207c 205b 5175 6963 6b73 7461  pdf) | [Quicksta
+00001ab0: 7274 5d28 6874 7470 733a 2f2f 646f 6373  rt](https://docs
+00001ac0: 2e61 6461 7074 6572 6875 622e 6d6c 2f71  .adapterhub.ml/q
+00001ad0: 7569 636b 7374 6172 742e 6874 6d6c 292c  uickstart.html),
+00001ae0: 205b 4e6f 7465 626f 6f6b 5d28 6874 7470   [Notebook](http
+00001af0: 733a 2f2f 636f 6c61 622e 7265 7365 6172  s://colab.resear
+00001b00: 6368 2e67 6f6f 676c 652e 636f 6d2f 6769  ch.google.com/gi
+00001b10: 7468 7562 2f41 6461 7074 6572 2d48 7562  thub/Adapter-Hub
+00001b20: 2f61 6461 7074 6572 732f 626c 6f62 2f6d  /adapters/blob/m
+00001b30: 6169 6e2f 6e6f 7465 626f 6f6b 732f 3031  ain/notebooks/01
+00001b40: 5f41 6461 7074 6572 5f54 7261 696e 696e  _Adapter_Trainin
+00001b50: 672e 6970 796e 6229 207c 0d0a 7c20 4164  g.ipynb) |..| Ad
+00001b60: 6170 7465 7246 7573 696f 6e20 7c20 5b50  apterFusion | [P
+00001b70: 6665 6966 6665 7220 6574 2061 6c2e 2028  feiffer et al. (
+00001b80: 3230 3231 295d 2868 7474 7073 3a2f 2f61  2021)](https://a
+00001b90: 636c 616e 7468 6f6c 6f67 792e 6f72 672f  clanthology.org/
+00001ba0: 3230 3231 2e65 6163 6c2d 6d61 696e 2e33  2021.eacl-main.3
+00001bb0: 392e 7064 6629 207c 205b 446f 6373 3a20  9.pdf) | [Docs: 
+00001bc0: 5472 6169 6e69 6e67 5d28 6874 7470 733a  Training](https:
+00001bd0: 2f2f 646f 6373 2e61 6461 7074 6572 6875  //docs.adapterhu
+00001be0: 622e 6d6c 2f74 7261 696e 696e 672e 6874  b.ml/training.ht
+00001bf0: 6d6c 2374 7261 696e 2d61 6461 7074 6572  ml#train-adapter
+00001c00: 6675 7369 6f6e 292c 205b 4e6f 7465 626f  fusion), [Notebo
+00001c10: 6f6b 5d28 6874 7470 733a 2f2f 636f 6c61  ok](https://cola
+00001c20: 622e 7265 7365 6172 6368 2e67 6f6f 676c  b.research.googl
+00001c30: 652e 636f 6d2f 6769 7468 7562 2f41 6461  e.com/github/Ada
+00001c40: 7074 6572 2d48 7562 2f61 6461 7074 6572  pter-Hub/adapter
+00001c50: 732f 626c 6f62 2f6d 6169 6e2f 6e6f 7465  s/blob/main/note
+00001c60: 626f 6f6b 732f 3033 5f41 6461 7074 6572  books/03_Adapter
+00001c70: 5f46 7573 696f 6e2e 6970 796e 6229 207c  _Fusion.ipynb) |
+00001c80: 0d0a 7c20 4d41 442d 582c 3c62 723e 2049  ..| MAD-X,<br> I
+00001c90: 6e76 6572 7469 626c 6520 6164 6170 7465  nvertible adapte
+00001ca0: 7273 207c 205b 5066 6569 6666 6572 2065  rs | [Pfeiffer e
+00001cb0: 7420 616c 2e20 2832 3032 3029 5d28 6874  t al. (2020)](ht
+00001cc0: 7470 733a 2f2f 6163 6c61 6e74 686f 6c6f  tps://aclantholo
+00001cd0: 6779 2e6f 7267 2f32 3032 302e 656d 6e6c  gy.org/2020.emnl
+00001ce0: 702d 6d61 696e 2e36 3137 2f29 207c 205b  p-main.617/) | [
+00001cf0: 4e6f 7465 626f 6f6b 5d28 6874 7470 733a  Notebook](https:
+00001d00: 2f2f 636f 6c61 622e 7265 7365 6172 6368  //colab.research
+00001d10: 2e67 6f6f 676c 652e 636f 6d2f 6769 7468  .google.com/gith
+00001d20: 7562 2f41 6461 7074 6572 2d48 7562 2f61  ub/Adapter-Hub/a
+00001d30: 6461 7074 6572 732f 626c 6f62 2f6d 6169  dapters/blob/mai
+00001d40: 6e2f 6e6f 7465 626f 6f6b 732f 3034 5f43  n/notebooks/04_C
+00001d50: 726f 7373 5f4c 696e 6775 616c 5f54 7261  ross_Lingual_Tra
+00001d60: 6e73 6665 722e 6970 796e 6229 207c 0d0a  nsfer.ipynb) |..
+00001d70: 7c20 4164 6170 7465 7244 726f 7020 7c20  | AdapterDrop | 
+00001d80: 5b52 c3bc 636b 6cc3 a920 6574 2061 6c2e  [R..ckl.. et al.
+00001d90: 2028 3230 3231 295d 2868 7474 7073 3a2f   (2021)](https:/
+00001da0: 2f61 7278 6976 2e6f 7267 2f70 6466 2f32  /arxiv.org/pdf/2
+00001db0: 3031 302e 3131 3931 382e 7064 6629 207c  010.11918.pdf) |
+00001dc0: 205b 4e6f 7465 626f 6f6b 5d28 6874 7470   [Notebook](http
+00001dd0: 733a 2f2f 636f 6c61 622e 7265 7365 6172  s://colab.resear
+00001de0: 6368 2e67 6f6f 676c 652e 636f 6d2f 6769  ch.google.com/gi
+00001df0: 7468 7562 2f41 6461 7074 6572 2d48 7562  thub/Adapter-Hub
+00001e00: 2f61 6461 7074 6572 732f 626c 6f62 2f6d  /adapters/blob/m
+00001e10: 6169 6e2f 6e6f 7465 626f 6f6b 732f 3035  ain/notebooks/05
+00001e20: 5f41 6461 7074 6572 5f44 726f 705f 5472  _Adapter_Drop_Tr
+00001e30: 6169 6e69 6e67 2e69 7079 6e62 2920 7c0d  aining.ipynb) |.
+00001e40: 0a7c 204d 4144 2d58 2032 2e30 2c3c 6272  .| MAD-X 2.0,<br
+00001e50: 3e20 456d 6265 6464 696e 6720 7472 6169  > Embedding trai
+00001e60: 6e69 6e67 207c 205b 5066 6569 6666 6572  ning | [Pfeiffer
+00001e70: 2065 7420 616c 2e20 2832 3032 3129 5d28   et al. (2021)](
+00001e80: 6874 7470 733a 2f2f 6172 7869 762e 6f72  https://arxiv.or
+00001e90: 672f 7064 662f 3230 3132 2e31 3535 3632  g/pdf/2012.15562
+00001ea0: 2e70 6466 2920 7c20 5b44 6f63 733a 2045  .pdf) | [Docs: E
+00001eb0: 6d62 6564 6469 6e67 735d 2868 7474 7073  mbeddings](https
+00001ec0: 3a2f 2f64 6f63 732e 6164 6170 7465 7268  ://docs.adapterh
+00001ed0: 7562 2e6d 6c2f 656d 6265 6464 696e 6773  ub.ml/embeddings
+00001ee0: 2e68 746d 6c29 2c20 5b4e 6f74 6562 6f6f  .html), [Noteboo
+00001ef0: 6b5d 2868 7474 7073 3a2f 2f63 6f6c 6162  k](https://colab
+00001f00: 2e72 6573 6561 7263 682e 676f 6f67 6c65  .research.google
+00001f10: 2e63 6f6d 2f67 6974 6875 622f 4164 6170  .com/github/Adap
+00001f20: 7465 722d 4875 622f 6164 6170 7465 7273  ter-Hub/adapters
+00001f30: 2f62 6c6f 622f 6d61 696e 2f6e 6f74 6562  /blob/main/noteb
+00001f40: 6f6f 6b73 2f30 385f 4e45 525f 5769 6b69  ooks/08_NER_Wiki
+00001f50: 616e 6e2e 6970 796e 6229 207c 0d0a 7c20  ann.ipynb) |..| 
+00001f60: 5072 6566 6978 2054 756e 696e 6720 7c20  Prefix Tuning | 
+00001f70: 5b4c 6920 616e 6420 4c69 616e 6720 2832  [Li and Liang (2
+00001f80: 3032 3129 5d28 6874 7470 733a 2f2f 6172  021)](https://ar
+00001f90: 7869 762e 6f72 672f 7064 662f 3231 3031  xiv.org/pdf/2101
+00001fa0: 2e30 3031 3930 2e70 6466 2920 7c20 5b44  .00190.pdf) | [D
+00001fb0: 6f63 735d 2868 7474 7073 3a2f 2f64 6f63  ocs](https://doc
+00001fc0: 732e 6164 6170 7465 7268 7562 2e6d 6c2f  s.adapterhub.ml/
+00001fd0: 6d65 7468 6f64 732e 6874 6d6c 2370 7265  methods.html#pre
+00001fe0: 6669 782d 7475 6e69 6e67 2920 7c0d 0a7c  fix-tuning) |..|
+00001ff0: 2050 6172 616c 6c65 6c20 6164 6170 7465   Parallel adapte
+00002000: 7273 2c3c 6272 3e20 4d69 782d 616e 642d  rs,<br> Mix-and-
+00002010: 4d61 7463 6820 6164 6170 7465 7273 207c  Match adapters |
+00002020: 205b 4865 2065 7420 616c 2e20 2832 3032   [He et al. (202
+00002030: 3129 5d28 6874 7470 733a 2f2f 6172 7869  1)](https://arxi
+00002040: 762e 6f72 672f 7064 662f 3231 3130 2e30  v.org/pdf/2110.0
+00002050: 3433 3636 2e70 6466 2920 7c20 5b44 6f63  4366.pdf) | [Doc
+00002060: 735d 2868 7474 7073 3a2f 2f64 6f63 732e  s](https://docs.
+00002070: 6164 6170 7465 7268 7562 2e6d 6c2f 6d65  adapterhub.ml/me
+00002080: 7468 6f64 5f63 6f6d 6269 6e61 7469 6f6e  thod_combination
+00002090: 732e 6874 6d6c 236d 6978 2d61 6e64 2d6d  s.html#mix-and-m
+000020a0: 6174 6368 2d61 6461 7074 6572 7329 207c  atch-adapters) |
+000020b0: 0d0a 7c20 436f 6d70 6163 7465 7220 7c20  ..| Compacter | 
+000020c0: 5b4d 6168 6162 6164 6920 6574 2061 6c2e  [Mahabadi et al.
+000020d0: 2028 3230 3231 295d 2868 7474 7073 3a2f   (2021)](https:/
+000020e0: 2f61 7278 6976 2e6f 7267 2f70 6466 2f32  /arxiv.org/pdf/2
+000020f0: 3130 362e 3034 3634 372e 7064 6629 207c  106.04647.pdf) |
+00002100: 205b 446f 6373 5d28 6874 7470 733a 2f2f   [Docs](https://
+00002110: 646f 6373 2e61 6461 7074 6572 6875 622e  docs.adapterhub.
+00002120: 6d6c 2f6d 6574 686f 6473 2e68 746d 6c23  ml/methods.html#
+00002130: 636f 6d70 6163 7465 7229 207c 0d0a 7c20  compacter) |..| 
+00002140: 4c6f 5241 207c 205b 4875 2065 7420 616c  LoRA | [Hu et al
+00002150: 2e20 2832 3032 3129 5d28 6874 7470 733a  . (2021)](https:
+00002160: 2f2f 6172 7869 762e 6f72 672f 7064 662f  //arxiv.org/pdf/
+00002170: 3231 3036 2e30 3936 3835 2e70 6466 2920  2106.09685.pdf) 
+00002180: 7c20 5b44 6f63 735d 2868 7474 7073 3a2f  | [Docs](https:/
+00002190: 2f64 6f63 732e 6164 6170 7465 7268 7562  /docs.adapterhub
+000021a0: 2e6d 6c2f 6d65 7468 6f64 732e 6874 6d6c  .ml/methods.html
+000021b0: 236c 6f72 6129 207c 0d0a 7c20 2849 4129  #lora) |..| (IA)
+000021c0: 5e33 207c 205b 4c69 7520 6574 2061 6c2e  ^3 | [Liu et al.
+000021d0: 2028 3230 3232 295d 2868 7474 7073 3a2f   (2022)](https:/
+000021e0: 2f61 7278 6976 2e6f 7267 2f70 6466 2f32  /arxiv.org/pdf/2
+000021f0: 3230 352e 3035 3633 382e 7064 6629 207c  205.05638.pdf) |
+00002200: 205b 446f 6373 5d28 6874 7470 733a 2f2f   [Docs](https://
+00002210: 646f 6373 2e61 6461 7074 6572 6875 622e  docs.adapterhub.
+00002220: 6d6c 2f6d 6574 686f 6473 2e68 746d 6c23  ml/methods.html#
+00002230: 6961 2d33 2920 7c0d 0a7c 2055 6e69 5045  ia-3) |..| UniPE
+00002240: 4c54 207c 205b 4d61 6f20 6574 2061 6c2e  LT | [Mao et al.
+00002250: 2028 3230 3232 295d 2868 7474 7073 3a2f   (2022)](https:/
+00002260: 2f61 7278 6976 2e6f 7267 2f70 6466 2f32  /arxiv.org/pdf/2
+00002270: 3131 302e 3037 3537 372e 7064 6629 207c  110.07577.pdf) |
+00002280: 205b 446f 6373 5d28 6874 7470 733a 2f2f   [Docs](https://
+00002290: 646f 6373 2e61 6461 7074 6572 6875 622e  docs.adapterhub.
+000022a0: 6d6c 2f6d 6574 686f 645f 636f 6d62 696e  ml/method_combin
+000022b0: 6174 696f 6e73 2e68 746d 6c23 756e 6970  ations.html#unip
+000022c0: 656c 7429 207c 0d0a 7c20 5072 6f6d 7074  elt) |..| Prompt
+000022d0: 2054 756e 696e 6720 7c20 5b4c 6573 7465   Tuning | [Leste
+000022e0: 7220 6574 2061 6c2e 2028 3230 3231 295d  r et al. (2021)]
+000022f0: 2868 7474 7073 3a2f 2f61 636c 616e 7468  (https://aclanth
+00002300: 6f6c 6f67 792e 6f72 672f 3230 3231 2e65  ology.org/2021.e
+00002310: 6d6e 6c70 2d6d 6169 6e2e 3234 332f 2920  mnlp-main.243/) 
+00002320: 7c20 5b44 6f63 735d 2868 7474 7073 3a2f  | [Docs](https:/
+00002330: 2f64 6f63 732e 6164 6170 7465 7268 7562  /docs.adapterhub
+00002340: 2e6d 6c2f 6d65 7468 6f64 732e 6874 6d6c  .ml/methods.html
+00002350: 2370 726f 6d70 742d 7475 6e69 6e67 2920  #prompt-tuning) 
+00002360: 7c0d 0a7c 2051 4c6f 5241 207c 205b 4465  |..| QLoRA | [De
+00002370: 7474 6d65 7273 2065 7420 616c 2e20 2832  ttmers et al. (2
+00002380: 3032 3329 5d28 6874 7470 733a 2f2f 6172  023)](https://ar
+00002390: 7869 762e 6f72 672f 7064 662f 3233 3035  xiv.org/pdf/2305
+000023a0: 2e31 3433 3134 2e70 6466 2920 7c20 5b4e  .14314.pdf) | [N
+000023b0: 6f74 6562 6f6f 6b5d 2868 7474 7073 3a2f  otebook](https:/
+000023c0: 2f63 6f6c 6162 2e72 6573 6561 7263 682e  /colab.research.
+000023d0: 676f 6f67 6c65 2e63 6f6d 2f67 6974 6875  google.com/githu
+000023e0: 622f 4164 6170 7465 722d 4875 622f 6164  b/Adapter-Hub/ad
+000023f0: 6170 7465 7273 2f62 6c6f 622f 6d61 696e  apters/blob/main
+00002400: 2f6e 6f74 6562 6f6f 6b73 2f51 4c6f 5241  /notebooks/QLoRA
+00002410: 5f4c 6c61 6d61 5f46 696e 6574 756e 696e  _Llama_Finetunin
+00002420: 672e 6970 796e 6229 207c 0d0a 0d0a 2323  g.ipynb) |....##
+00002430: 2053 7570 706f 7274 6564 204d 6f64 656c   Supported Model
+00002440: 730d 0a0d 0a57 6520 6375 7272 656e 746c  s....We currentl
+00002450: 7920 7375 7070 6f72 7420 7468 6520 5079  y support the Py
+00002460: 546f 7263 6820 7665 7273 696f 6e73 206f  Torch versions o
+00002470: 6620 616c 6c20 6d6f 6465 6c73 206c 6973  f all models lis
+00002480: 7465 6420 6f6e 2074 6865 202a 2a5b 4d6f  ted on the **[Mo
+00002490: 6465 6c20 4f76 6572 7669 6577 5d28 6874  del Overview](ht
+000024a0: 7470 733a 2f2f 646f 6373 2e61 6461 7074  tps://docs.adapt
+000024b0: 6572 6875 622e 6d6c 2f6d 6f64 656c 5f6f  erhub.ml/model_o
+000024c0: 7665 7276 6965 772e 6874 6d6c 2920 7061  verview.html) pa
+000024d0: 6765 2a2a 2069 6e20 6f75 7220 646f 6375  ge** in our docu
+000024e0: 6d65 6e74 6174 696f 6e2e 0d0a 0d0a 2323  mentation.....##
+000024f0: 2044 6576 656c 6f70 696e 6720 2620 436f   Developing & Co
+00002500: 6e74 7269 6275 7469 6e67 0d0a 0d0a 546f  ntributing....To
+00002510: 2067 6574 2073 7461 7274 6564 2077 6974   get started wit
+00002520: 6820 6465 7665 6c6f 7069 6e67 206f 6e20  h developing on 
+00002530: 5f41 6461 7074 6572 735f 2079 6f75 7273  _Adapters_ yours
+00002540: 656c 6620 616e 6420 6c65 6172 6e20 6d6f  elf and learn mo
+00002550: 7265 2061 626f 7574 2077 6179 7320 746f  re about ways to
+00002560: 2063 6f6e 7472 6962 7574 652c 2070 6c65   contribute, ple
+00002570: 6173 6520 7365 6520 6874 7470 733a 2f2f  ase see https://
+00002580: 646f 6373 2e61 6461 7074 6572 6875 622e  docs.adapterhub.
+00002590: 6d6c 2f63 6f6e 7472 6962 7574 696e 672e  ml/contributing.
+000025a0: 6874 6d6c 2e0d 0a0d 0a23 2320 4369 7461  html.....## Cita
+000025b0: 7469 6f6e 0d0a 0d0a 4966 2079 6f75 2075  tion....If you u
+000025c0: 7365 205f 4164 6170 7465 7273 5f20 696e  se _Adapters_ in
+000025d0: 2079 6f75 7220 776f 726b 2c20 706c 6561   your work, plea
+000025e0: 7365 2063 6f6e 7369 6465 7220 6369 7469  se consider citi
+000025f0: 6e67 206f 7572 206c 6962 7261 7279 2070  ng our library p
+00002600: 6170 6572 3a20 5b41 6461 7074 6572 733a  aper: [Adapters:
+00002610: 2041 2055 6e69 6669 6564 204c 6962 7261   A Unified Libra
+00002620: 7279 2066 6f72 2050 6172 616d 6574 6572  ry for Parameter
+00002630: 2d45 6666 6963 6965 6e74 2061 6e64 204d  -Efficient and M
+00002640: 6f64 756c 6172 2054 7261 6e73 6665 7220  odular Transfer 
+00002650: 4c65 6172 6e69 6e67 5d28 6874 7470 733a  Learning](https:
+00002660: 2f2f 6172 7869 762e 6f72 672f 6162 732f  //arxiv.org/abs/
+00002670: 3233 3131 2e31 3130 3737 290d 0a0d 0a60  2311.11077)....`
+00002680: 6060 0d0a 4069 6e70 726f 6365 6564 696e  ``..@inproceedin
+00002690: 6773 7b70 6f74 682d 6574 616c 2d32 3032  gs{poth-etal-202
+000026a0: 332d 6164 6170 7465 7273 2c0d 0a20 2020  3-adapters,..   
+000026b0: 2074 6974 6c65 203d 2022 4164 6170 7465   title = "Adapte
+000026c0: 7273 3a20 4120 556e 6966 6965 6420 4c69  rs: A Unified Li
+000026d0: 6272 6172 7920 666f 7220 5061 7261 6d65  brary for Parame
+000026e0: 7465 722d 4566 6669 6369 656e 7420 616e  ter-Efficient an
+000026f0: 6420 4d6f 6475 6c61 7220 5472 616e 7366  d Modular Transf
+00002700: 6572 204c 6561 726e 696e 6722 2c0d 0a20  er Learning",.. 
+00002710: 2020 2061 7574 686f 7220 3d20 7b50 6f74     author = {Pot
+00002720: 682c 2043 6c69 6674 6f6e 2020 616e 640d  h, Clifton  and.
+00002730: 0a20 2020 2020 2053 7465 727a 2c20 4861  .      Sterz, Ha
+00002740: 6e6e 6168 2020 616e 640d 0a20 2020 2020  nnah  and..     
+00002750: 2050 6175 6c2c 2049 6e64 7261 6e65 696c   Paul, Indraneil
+00002760: 2020 616e 640d 0a20 2020 2020 2050 7572    and..      Pur
+00002770: 6b61 7961 7374 6861 2c20 5375 6b61 6e6e  kayastha, Sukann
+00002780: 7961 2020 616e 640d 0a20 2020 2020 2045  ya  and..      E
+00002790: 6e67 6c7b 5c22 617d 6e64 6572 2c20 4c65  ngl{\"a}nder, Le
+000027a0: 6f6e 2020 616e 640d 0a20 2020 2020 2049  on  and..      I
+000027b0: 6d68 6f66 2c20 5469 6d6f 2020 616e 640d  mhof, Timo  and.
+000027c0: 0a20 2020 2020 2056 756c 697b 5c27 637d  .      Vuli{\'c}
+000027d0: 2c20 4976 616e 2020 616e 640d 0a20 2020  , Ivan  and..   
+000027e0: 2020 2052 7564 6572 2c20 5365 6261 7374     Ruder, Sebast
+000027f0: 6961 6e20 2061 6e64 0d0a 2020 2020 2020  ian  and..      
+00002800: 4775 7265 7679 6368 2c20 4972 796e 6120  Gurevych, Iryna 
+00002810: 2061 6e64 0d0a 2020 2020 2020 5066 6569   and..      Pfei
+00002820: 6666 6572 2c20 4a6f 6e61 737d 2c0d 0a20  ffer, Jonas},.. 
+00002830: 2020 2062 6f6f 6b74 6974 6c65 203d 2022     booktitle = "
+00002840: 5072 6f63 6565 6469 6e67 7320 6f66 2074  Proceedings of t
+00002850: 6865 2032 3032 3320 436f 6e66 6572 656e  he 2023 Conferen
+00002860: 6365 206f 6e20 456d 7069 7269 6361 6c20  ce on Empirical 
+00002870: 4d65 7468 6f64 7320 696e 204e 6174 7572  Methods in Natur
+00002880: 616c 204c 616e 6775 6167 6520 5072 6f63  al Language Proc
+00002890: 6573 7369 6e67 3a20 5379 7374 656d 2044  essing: System D
+000028a0: 656d 6f6e 7374 7261 7469 6f6e 7322 2c0d  emonstrations",.
+000028b0: 0a20 2020 206d 6f6e 7468 203d 2064 6563  .    month = dec
+000028c0: 2c0d 0a20 2020 2079 6561 7220 3d20 2232  ,..    year = "2
+000028d0: 3032 3322 2c0d 0a20 2020 2061 6464 7265  023",..    addre
+000028e0: 7373 203d 2022 5369 6e67 6170 6f72 6522  ss = "Singapore"
+000028f0: 2c0d 0a20 2020 2070 7562 6c69 7368 6572  ,..    publisher
+00002900: 203d 2022 4173 736f 6369 6174 696f 6e20   = "Association 
+00002910: 666f 7220 436f 6d70 7574 6174 696f 6e61  for Computationa
+00002920: 6c20 4c69 6e67 7569 7374 6963 7322 2c0d  l Linguistics",.
+00002930: 0a20 2020 2075 726c 203d 2022 6874 7470  .    url = "http
+00002940: 733a 2f2f 6163 6c61 6e74 686f 6c6f 6779  s://aclanthology
+00002950: 2e6f 7267 2f32 3032 332e 656d 6e6c 702d  .org/2023.emnlp-
+00002960: 6465 6d6f 2e31 3322 2c0d 0a20 2020 2070  demo.13",..    p
+00002970: 6167 6573 203d 2022 3134 392d 2d31 3630  ages = "149--160
+00002980: 222c 0d0a 7d0d 0a60 6060 0d0a 0d0a 416c  ",..}..```....Al
+00002990: 7465 726e 6174 6976 656c 792c 2066 6f72  ternatively, for
+000029a0: 2074 6865 2070 7265 6465 6365 7373 6f72   the predecessor
+000029b0: 2060 6164 6170 7465 722d 7472 616e 7366   `adapter-transf
+000029c0: 6f72 6d65 7273 602c 2074 6865 2048 7562  ormers`, the Hub
+000029d0: 2069 6e66 7261 7374 7275 6374 7572 6520   infrastructure 
+000029e0: 616e 6420 6164 6170 7465 7273 2075 706c  and adapters upl
+000029f0: 6f61 6465 6420 6279 2074 6865 2041 6461  oaded by the Ada
+00002a00: 7074 6572 4875 6220 7465 616d 2c20 706c  pterHub team, pl
+00002a10: 6561 7365 2063 6f6e 7369 6465 7220 6369  ease consider ci
+00002a20: 7469 6e67 206f 7572 2069 6e69 7469 616c  ting our initial
+00002a30: 2070 6170 6572 3a20 5b41 6461 7074 6572   paper: [Adapter
+00002a40: 4875 623a 2041 2046 7261 6d65 776f 726b  Hub: A Framework
+00002a50: 2066 6f72 2041 6461 7074 696e 6720 5472   for Adapting Tr
+00002a60: 616e 7366 6f72 6d65 7273 5d28 6874 7470  ansformers](http
+00002a70: 733a 2f2f 6172 7869 762e 6f72 672f 6162  s://arxiv.org/ab
+00002a80: 732f 3230 3037 2e30 3737 3739 290d 0a0d  s/2007.07779)...
+00002a90: 0a60 6060 0d0a 4069 6e70 726f 6365 6564  .```..@inproceed
+00002aa0: 696e 6773 7b70 6665 6966 6665 7232 3032  ings{pfeiffer202
+00002ab0: 3041 6461 7074 6572 4875 622c 0d0a 2020  0AdapterHub,..  
+00002ac0: 2020 7469 746c 653d 7b41 6461 7074 6572    title={Adapter
+00002ad0: 4875 623a 2041 2046 7261 6d65 776f 726b  Hub: A Framework
+00002ae0: 2066 6f72 2041 6461 7074 696e 6720 5472   for Adapting Tr
+00002af0: 616e 7366 6f72 6d65 7273 7d2c 0d0a 2020  ansformers},..  
+00002b00: 2020 6175 7468 6f72 3d7b 5066 6569 6666    author={Pfeiff
+00002b10: 6572 2c20 4a6f 6e61 7320 616e 640d 0a20  er, Jonas and.. 
+00002b20: 2020 2020 2020 2020 2020 2052 7b5c 2275             R{\"u
+00002b30: 7d63 6b6c 7b5c 2765 7d2c 2041 6e64 7265  }ckl{\'e}, Andre
+00002b40: 6173 2061 6e64 0d0a 2020 2020 2020 2020  as and..        
+00002b50: 2020 2020 506f 7468 2c20 436c 6966 746f      Poth, Clifto
+00002b60: 6e20 616e 640d 0a20 2020 2020 2020 2020  n and..         
+00002b70: 2020 204b 616d 6174 682c 2041 6973 6877     Kamath, Aishw
+00002b80: 6172 7961 2061 6e64 0d0a 2020 2020 2020  arya and..      
+00002b90: 2020 2020 2020 5675 6c69 7b5c 2763 7d2c        Vuli{\'c},
+00002ba0: 2049 7661 6e20 616e 640d 0a20 2020 2020   Ivan and..     
+00002bb0: 2020 2020 2020 2052 7564 6572 2c20 5365         Ruder, Se
+00002bc0: 6261 7374 6961 6e20 616e 640d 0a20 2020  bastian and..   
+00002bd0: 2020 2020 2020 2020 2043 686f 2c20 4b79           Cho, Ky
+00002be0: 756e 6768 7975 6e20 616e 640d 0a20 2020  unghyun and..   
+00002bf0: 2020 2020 2020 2020 2047 7572 6576 7963           Gurevyc
+00002c00: 682c 2049 7279 6e61 7d2c 0d0a 2020 2020  h, Iryna},..    
+00002c10: 626f 6f6b 7469 746c 653d 7b50 726f 6365  booktitle={Proce
+00002c20: 6564 696e 6773 206f 6620 7468 6520 3230  edings of the 20
+00002c30: 3230 2043 6f6e 6665 7265 6e63 6520 6f6e  20 Conference on
+00002c40: 2045 6d70 6972 6963 616c 204d 6574 686f   Empirical Metho
+00002c50: 6473 2069 6e20 4e61 7475 7261 6c20 4c61  ds in Natural La
+00002c60: 6e67 7561 6765 2050 726f 6365 7373 696e  nguage Processin
+00002c70: 673a 2053 7973 7465 6d20 4465 6d6f 6e73  g: System Demons
+00002c80: 7472 6174 696f 6e73 7d2c 0d0a 2020 2020  trations},..    
+00002c90: 7061 6765 733d 7b34 362d 2d35 347d 2c0d  pages={46--54},.
+00002ca0: 0a20 2020 2079 6561 723d 7b32 3032 307d  .    year={2020}
+00002cb0: 0d0a 7d0d 0a60 6060 0d0a                 ..}..```..
```

### Comparing `adapters-0.1.2/README.md` & `adapters-0.2.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -31,563 +31,597 @@
 000001e0: 696d 706c 6965 642e 0a53 6565 2074 6865  implied..See the
 000001f0: 204c 6963 656e 7365 2066 6f72 2074 6865   License for the
 00000200: 2073 7065 6369 6669 6320 6c61 6e67 7561   specific langua
 00000210: 6765 2067 6f76 6572 6e69 6e67 2070 6572  ge governing per
 00000220: 6d69 7373 696f 6e73 2061 6e64 0a6c 696d  missions and.lim
 00000230: 6974 6174 696f 6e73 2075 6e64 6572 2074  itations under t
 00000240: 6865 204c 6963 656e 7365 2e0a 2d2d 3e0a  he License..-->.
-00000250: 0a3e 202a 2a4e 6f74 652a 2a3a 2054 6869  .> **Note**: Thi
-00000260: 7320 7265 706f 7369 746f 7279 2068 6f6c  s repository hol
-00000270: 6473 2074 6865 2063 6f64 6562 6173 6520  ds the codebase 
-00000280: 6f66 2074 6865 205f 4164 6170 7465 7273  of the _Adapters
-00000290: 5f20 6c69 6272 6172 792c 2077 6869 6368  _ library, which
-000002a0: 2068 6173 2072 6570 6c61 6365 6420 6061   has replaced `a
-000002b0: 6461 7074 6572 2d74 7261 6e73 666f 726d  dapter-transform
-000002c0: 6572 7360 2e20 466f 7220 7468 6520 6c65  ers`. For the le
-000002d0: 6761 6379 2063 6f64 6562 6173 652c 2067  gacy codebase, g
-000002e0: 6f20 746f 3a20 6874 7470 733a 2f2f 6769  o to: https://gi
-000002f0: 7468 7562 2e63 6f6d 2f61 6461 7074 6572  thub.com/adapter
-00000300: 2d68 7562 2f61 6461 7074 6572 2d74 7261  -hub/adapter-tra
-00000310: 6e73 666f 726d 6572 732d 6c65 6761 6379  nsformers-legacy
-00000320: 2e0a 0a3c 7020 616c 6967 6e3d 2263 656e  ...<p align="cen
-00000330: 7465 7222 3e0a 3c69 6d67 2073 7479 6c65  ter">.<img style
-00000340: 3d22 7665 7274 6963 616c 2d61 6c69 676e  ="vertical-align
-00000350: 3a6d 6964 646c 6522 2073 7263 3d22 6874  :middle" src="ht
-00000360: 7470 733a 2f2f 7261 772e 6769 7468 7562  tps://raw.github
-00000370: 7573 6572 636f 6e74 656e 742e 636f 6d2f  usercontent.com/
-00000380: 4164 6170 7465 722d 4875 622f 6164 6170  Adapter-Hub/adap
-00000390: 7465 7273 2f6d 6169 6e2f 646f 6373 2f6c  ters/main/docs/l
-000003a0: 6f67 6f2e 706e 6722 202f 3e0a 3c2f 703e  ogo.png" />.</p>
-000003b0: 0a3c 6831 2061 6c69 676e 3d22 6365 6e74  .<h1 align="cent
-000003c0: 6572 223e 0a3c 7370 616e 3e3c 693e 4164  er">.<span><i>Ad
-000003d0: 6170 7465 7273 3c2f 693e 3c2f 7370 616e  apters</i></span
-000003e0: 3e0a 3c2f 6831 3e0a 0a3c 6833 2061 6c69  >.</h1>..<h3 ali
-000003f0: 676e 3d22 6365 6e74 6572 223e 0a41 2055  gn="center">.A U
-00000400: 6e69 6669 6564 204c 6962 7261 7279 2066  nified Library f
-00000410: 6f72 2050 6172 616d 6574 6572 2d45 6666  or Parameter-Eff
-00000420: 6963 6965 6e74 2061 6e64 204d 6f64 756c  icient and Modul
-00000430: 6172 2054 7261 6e73 6665 7220 4c65 6172  ar Transfer Lear
-00000440: 6e69 6e67 0a3c 2f68 333e 0a0a 215b 5465  ning.</h3>..![Te
-00000450: 7374 735d 2868 7474 7073 3a2f 2f67 6974  sts](https://git
-00000460: 6875 622e 636f 6d2f 4164 6170 7465 722d  hub.com/Adapter-
-00000470: 4875 622f 6164 6170 7465 7273 2f77 6f72  Hub/adapters/wor
-00000480: 6b66 6c6f 7773 2f54 6573 7473 2f62 6164  kflows/Tests/bad
-00000490: 6765 2e73 7667 3f62 7261 6e63 683d 6164  ge.svg?branch=ad
-000004a0: 6170 7465 7273 290a 5b21 5b47 6974 4875  apters).[![GitHu
-000004b0: 625d 2868 7474 7073 3a2f 2f69 6d67 2e73  b](https://img.s
-000004c0: 6869 656c 6473 2e69 6f2f 6769 7468 7562  hields.io/github
-000004d0: 2f6c 6963 656e 7365 2f61 6461 7074 6572  /license/adapter
-000004e0: 2d68 7562 2f61 6461 7074 6572 732e 7376  -hub/adapters.sv
-000004f0: 673f 636f 6c6f 723d 626c 7565 295d 2868  g?color=blue)](h
-00000500: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000510: 6d2f 6164 6170 7465 722d 6875 622f 6164  m/adapter-hub/ad
-00000520: 6170 7465 7273 2f62 6c6f 622f 6d61 696e  apters/blob/main
-00000530: 2f4c 4943 454e 5345 290a 5b21 5b50 7950  /LICENSE).[![PyP
-00000540: 495d 2868 7474 7073 3a2f 2f69 6d67 2e73  I](https://img.s
-00000550: 6869 656c 6473 2e69 6f2f 7079 7069 2f76  hields.io/pypi/v
-00000560: 2f61 6461 7074 6572 7329 5d28 6874 7470  /adapters)](http
-00000570: 733a 2f2f 7079 7069 2e6f 7267 2f70 726f  s://pypi.org/pro
-00000580: 6a65 6374 2f61 6461 7074 6572 732f 290a  ject/adapters/).
-00000590: 0a60 6164 6170 7465 7273 6020 6973 2061  .`adapters` is a
-000005a0: 6e20 6164 642d 6f6e 2074 6f20 5b48 7567  n add-on to [Hug
-000005b0: 6769 6e67 4661 6365 2773 2054 7261 6e73  gingFace's Trans
-000005c0: 666f 726d 6572 735d 2868 7474 7073 3a2f  formers](https:/
-000005d0: 2f67 6974 6875 622e 636f 6d2f 6875 6767  /github.com/hugg
-000005e0: 696e 6766 6163 652f 7472 616e 7366 6f72  ingface/transfor
-000005f0: 6d65 7273 2920 6c69 6272 6172 792c 2069  mers) library, i
-00000600: 6e74 6567 7261 7469 6e67 2061 6461 7074  ntegrating adapt
-00000610: 6572 7320 696e 746f 2073 7461 7465 2d6f  ers into state-o
-00000620: 662d 7468 652d 6172 7420 6c61 6e67 7561  f-the-art langua
-00000630: 6765 206d 6f64 656c 7320 6279 2069 6e63  ge models by inc
-00000640: 6f72 706f 7261 7469 6e67 202a 2a5b 4164  orporating **[Ad
-00000650: 6170 7465 7248 7562 5d28 6874 7470 733a  apterHub](https:
-00000660: 2f2f 6164 6170 7465 7268 7562 2e6d 6c29  //adapterhub.ml)
-00000670: 2a2a 2c20 6120 6365 6e74 7261 6c20 7265  **, a central re
-00000680: 706f 7369 746f 7279 2066 6f72 2070 7265  pository for pre
-00000690: 2d74 7261 696e 6564 2061 6461 7074 6572  -trained adapter
-000006a0: 206d 6f64 756c 6573 2e0a 0a23 2320 496e   modules...## In
-000006b0: 7374 616c 6c61 7469 6f6e 0a0a 6061 6461  stallation..`ada
-000006c0: 7074 6572 7360 2063 7572 7265 6e74 6c79  pters` currently
-000006d0: 2073 7570 706f 7274 7320 2a2a 5079 7468   supports **Pyth
-000006e0: 6f6e 2033 2e38 2b2a 2a20 616e 6420 2a2a  on 3.8+** and **
-000006f0: 5079 546f 7263 6820 312e 3130 2b2a 2a2e  PyTorch 1.10+**.
-00000700: 0a41 6674 6572 205b 696e 7374 616c 6c69  .After [installi
-00000710: 6e67 2050 7954 6f72 6368 5d28 6874 7470  ng PyTorch](http
-00000720: 733a 2f2f 7079 746f 7263 682e 6f72 672f  s://pytorch.org/
-00000730: 6765 742d 7374 6172 7465 642f 6c6f 6361  get-started/loca
-00000740: 6c6c 792f 292c 2079 6f75 2063 616e 2069  lly/), you can i
-00000750: 6e73 7461 6c6c 2060 6164 6170 7465 7273  nstall `adapters
-00000760: 6020 6672 6f6d 2050 7950 4920 2e2e 2e0a  ` from PyPI ....
-00000770: 0a60 6060 0a70 6970 2069 6e73 7461 6c6c  .```.pip install
-00000780: 202d 5520 6164 6170 7465 7273 0a60 6060   -U adapters.```
-00000790: 0a0a 2e2e 2e20 6f72 2066 726f 6d20 736f  ..... or from so
-000007a0: 7572 6365 2062 7920 636c 6f6e 696e 6720  urce by cloning 
-000007b0: 7468 6520 7265 706f 7369 746f 7279 3a0a  the repository:.
-000007c0: 0a60 6060 0a67 6974 2063 6c6f 6e65 2068  .```.git clone h
-000007d0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-000007e0: 6d2f 6164 6170 7465 722d 6875 622f 6164  m/adapter-hub/ad
-000007f0: 6170 7465 7273 2e67 6974 0a63 6420 6164  apters.git.cd ad
-00000800: 6170 7465 7273 0a70 6970 2069 6e73 7461  apters.pip insta
-00000810: 6c6c 202e 0a60 6060 0a0a 2323 2051 7569  ll ..```..## Qui
-00000820: 636b 2054 6f75 720a 0a23 2323 2320 4c6f  ck Tour..#### Lo
-00000830: 6164 2070 7265 2d74 7261 696e 6564 2061  ad pre-trained a
-00000840: 6461 7074 6572 733a 0a0a 6060 6070 7974  dapters:..```pyt
-00000850: 686f 6e0a 6672 6f6d 2061 6461 7074 6572  hon.from adapter
-00000860: 7320 696d 706f 7274 2041 7574 6f41 6461  s import AutoAda
-00000870: 7074 6572 4d6f 6465 6c0a 6672 6f6d 2074  pterModel.from t
-00000880: 7261 6e73 666f 726d 6572 7320 696d 706f  ransformers impo
-00000890: 7274 2041 7574 6f54 6f6b 656e 697a 6572  rt AutoTokenizer
-000008a0: 0a0a 6d6f 6465 6c20 3d20 4175 746f 4164  ..model = AutoAd
-000008b0: 6170 7465 724d 6f64 656c 2e66 726f 6d5f  apterModel.from_
-000008c0: 7072 6574 7261 696e 6564 2822 726f 6265  pretrained("robe
-000008d0: 7274 612d 6261 7365 2229 0a74 6f6b 656e  rta-base").token
-000008e0: 697a 6572 203d 2041 7574 6f54 6f6b 656e  izer = AutoToken
-000008f0: 697a 6572 2e66 726f 6d5f 7072 6574 7261  izer.from_pretra
-00000900: 696e 6564 2822 726f 6265 7274 612d 6261  ined("roberta-ba
-00000910: 7365 2229 0a0a 6d6f 6465 6c2e 6c6f 6164  se")..model.load
-00000920: 5f61 6461 7074 6572 2822 4164 6170 7465  _adapter("Adapte
-00000930: 7248 7562 2f72 6f62 6572 7461 2d62 6173  rHub/roberta-bas
-00000940: 652d 7066 2d69 6d64 6222 2c20 736f 7572  e-pf-imdb", sour
-00000950: 6365 3d22 6866 222c 2073 6574 5f61 6374  ce="hf", set_act
-00000960: 6976 653d 5472 7565 290a 0a70 7269 6e74  ive=True)..print
-00000970: 286d 6f64 656c 282a 2a74 6f6b 656e 697a  (model(**tokeniz
-00000980: 6572 2822 5468 6973 2077 6f72 6b73 2067  er("This works g
-00000990: 7265 6174 2122 2c20 7265 7475 726e 5f74  reat!", return_t
-000009a0: 656e 736f 7273 3d22 7074 2229 292e 6c6f  ensors="pt")).lo
-000009b0: 6769 7473 290a 6060 600a 0a2a 2a5b 4c65  gits).```..**[Le
-000009c0: 6172 6e20 4d6f 7265 5d28 6874 7470 733a  arn More](https:
-000009d0: 2f2f 646f 6373 2e61 6461 7074 6572 6875  //docs.adapterhu
-000009e0: 622e 6d6c 2f6c 6f61 6469 6e67 2e68 746d  b.ml/loading.htm
-000009f0: 6c29 2a2a 0a0a 2323 2323 2041 6461 7074  l)**..#### Adapt
-00000a00: 2065 7869 7374 696e 6720 6d6f 6465 6c20   existing model 
-00000a10: 7365 7475 7073 3a0a 0a60 6060 7079 7468  setups:..```pyth
-00000a20: 6f6e 0a69 6d70 6f72 7420 6164 6170 7465  on.import adapte
-00000a30: 7273 0a66 726f 6d20 7472 616e 7366 6f72  rs.from transfor
-00000a40: 6d65 7273 2069 6d70 6f72 7420 4175 746f  mers import Auto
-00000a50: 4d6f 6465 6c46 6f72 5365 7175 656e 6365  ModelForSequence
-00000a60: 436c 6173 7369 6669 6361 7469 6f6e 0a0a  Classification..
-00000a70: 6d6f 6465 6c20 3d20 4175 746f 4d6f 6465  model = AutoMode
-00000a80: 6c46 6f72 5365 7175 656e 6365 436c 6173  lForSequenceClas
-00000a90: 7369 6669 6361 7469 6f6e 2e66 726f 6d5f  sification.from_
-00000aa0: 7072 6574 7261 696e 6564 2822 7435 2d62  pretrained("t5-b
-00000ab0: 6173 6522 290a 0a61 6461 7074 6572 732e  ase")..adapters.
-00000ac0: 696e 6974 286d 6f64 656c 290a 0a6d 6f64  init(model)..mod
-00000ad0: 656c 2e61 6464 5f61 6461 7074 6572 2822  el.add_adapter("
-00000ae0: 6d79 5f6c 6f72 615f 6164 6170 7465 7222  my_lora_adapter"
-00000af0: 2c20 636f 6e66 6967 3d22 6c6f 7261 2229  , config="lora")
-00000b00: 0a6d 6f64 656c 2e74 7261 696e 5f61 6461  .model.train_ada
-00000b10: 7074 6572 2822 6d79 5f6c 6f72 615f 6164  pter("my_lora_ad
-00000b20: 6170 7465 7222 290a 0a23 2059 6f75 7220  apter")..# Your 
-00000b30: 7265 6775 6c61 7220 7472 6169 6e69 6e67  regular training
-00000b40: 206c 6f6f 702e 2e2e 0a60 6060 0a0a 2a2a   loop....```..**
-00000b50: 5b4c 6561 726e 204d 6f72 655d 2868 7474  [Learn More](htt
-00000b60: 7073 3a2f 2f64 6f63 732e 6164 6170 7465  ps://docs.adapte
-00000b70: 7268 7562 2e6d 6c2f 7175 6963 6b73 7461  rhub.ml/quicksta
-00000b80: 7274 2e68 746d 6c29 2a2a 0a0a 2323 2323  rt.html)**..####
-00000b90: 2046 6c65 7869 626c 7920 636f 6e66 6967   Flexibly config
-00000ba0: 7572 6520 6164 6170 7465 7273 3a0a 0a60  ure adapters:..`
-00000bb0: 6060 7079 7468 6f6e 0a66 726f 6d20 6164  ``python.from ad
-00000bc0: 6170 7465 7273 2069 6d70 6f72 7420 436f  apters import Co
-00000bd0: 6e66 6967 556e 696f 6e2c 2050 7265 6669  nfigUnion, Prefi
-00000be0: 7854 756e 696e 6743 6f6e 6669 672c 2050  xTuningConfig, P
-00000bf0: 6172 426e 436f 6e66 6967 2c20 4175 746f  arBnConfig, Auto
-00000c00: 4164 6170 7465 724d 6f64 656c 0a0a 6d6f  AdapterModel..mo
-00000c10: 6465 6c20 3d20 4175 746f 4164 6170 7465  del = AutoAdapte
-00000c20: 724d 6f64 656c 2e66 726f 6d5f 7072 6574  rModel.from_pret
-00000c30: 7261 696e 6564 2822 6d69 6372 6f73 6f66  rained("microsof
-00000c40: 742f 6465 6265 7274 612d 7633 2d62 6173  t/deberta-v3-bas
-00000c50: 6522 290a 0a61 6461 7074 6572 5f63 6f6e  e")..adapter_con
-00000c60: 6669 6720 3d20 436f 6e66 6967 556e 696f  fig = ConfigUnio
-00000c70: 6e28 0a20 2020 2050 7265 6669 7854 756e  n(.    PrefixTun
-00000c80: 696e 6743 6f6e 6669 6728 7072 6566 6978  ingConfig(prefix
-00000c90: 5f6c 656e 6774 683d 3230 292c 0a20 2020  _length=20),.   
-00000ca0: 2050 6172 426e 436f 6e66 6967 2872 6564   ParBnConfig(red
-00000cb0: 7563 7469 6f6e 5f66 6163 746f 723d 3429  uction_factor=4)
-00000cc0: 2c0a 290a 6d6f 6465 6c2e 6164 645f 6164  ,.).model.add_ad
-00000cd0: 6170 7465 7228 226d 795f 6164 6170 7465  apter("my_adapte
-00000ce0: 7222 2c20 636f 6e66 6967 3d61 6461 7074  r", config=adapt
-00000cf0: 6572 5f63 6f6e 6669 672c 2073 6574 5f61  er_config, set_a
-00000d00: 6374 6976 653d 5472 7565 290a 6060 600a  ctive=True).```.
-00000d10: 0a2a 2a5b 4c65 6172 6e20 4d6f 7265 5d28  .**[Learn More](
-00000d20: 6874 7470 733a 2f2f 646f 6373 2e61 6461  https://docs.ada
-00000d30: 7074 6572 6875 622e 6d6c 2f6f 7665 7276  pterhub.ml/overv
-00000d40: 6965 772e 6874 6d6c 292a 2a0a 0a23 2323  iew.html)**..###
-00000d50: 2320 4561 7369 6c79 2063 6f6d 706f 7365  # Easily compose
-00000d60: 2061 6461 7074 6572 7320 696e 2061 2073   adapters in a s
-00000d70: 696e 676c 6520 6d6f 6465 6c3a 0a0a 6060  ingle model:..``
-00000d80: 6070 7974 686f 6e0a 6672 6f6d 2061 6461  `python.from ada
-00000d90: 7074 6572 7320 696d 706f 7274 2041 6461  pters import Ada
-00000da0: 7074 6572 5365 7475 702c 2041 7574 6f41  pterSetup, AutoA
-00000db0: 6461 7074 6572 4d6f 6465 6c0a 696d 706f  dapterModel.impo
-00000dc0: 7274 2061 6461 7074 6572 732e 636f 6d70  rt adapters.comp
-00000dd0: 6f73 6974 696f 6e20 6173 2061 630a 0a6d  osition as ac..m
-00000de0: 6f64 656c 203d 2041 7574 6f41 6461 7074  odel = AutoAdapt
-00000df0: 6572 4d6f 6465 6c2e 6672 6f6d 5f70 7265  erModel.from_pre
-00000e00: 7472 6169 6e65 6428 2272 6f62 6572 7461  trained("roberta
-00000e10: 2d62 6173 6522 290a 0a71 6320 3d20 6d6f  -base")..qc = mo
-00000e20: 6465 6c2e 6c6f 6164 5f61 6461 7074 6572  del.load_adapter
-00000e30: 2822 4164 6170 7465 7248 7562 2f72 6f62  ("AdapterHub/rob
-00000e40: 6572 7461 2d62 6173 652d 7066 2d74 7265  erta-base-pf-tre
-00000e50: 6322 290a 7365 6e74 203d 206d 6f64 656c  c").sent = model
-00000e60: 2e6c 6f61 645f 6164 6170 7465 7228 2241  .load_adapter("A
-00000e70: 6461 7074 6572 4875 622f 726f 6265 7274  dapterHub/robert
-00000e80: 612d 6261 7365 2d70 662d 696d 6462 2229  a-base-pf-imdb")
-00000e90: 0a0a 7769 7468 2041 6461 7074 6572 5365  ..with AdapterSe
-00000ea0: 7475 7028 6163 2e50 6172 616c 6c65 6c28  tup(ac.Parallel(
-00000eb0: 7163 2c20 7365 6e74 2929 3a0a 2020 2020  qc, sent)):.    
-00000ec0: 7072 696e 7428 6d6f 6465 6c28 2a2a 746f  print(model(**to
-00000ed0: 6b65 6e69 7a65 7228 2257 6861 7420 6973  kenizer("What is
-00000ee0: 2041 6461 7074 6572 4875 623f 222c 2072   AdapterHub?", r
-00000ef0: 6574 7572 6e5f 7465 6e73 6f72 733d 2270  eturn_tensors="p
-00000f00: 7422 2929 290a 6060 600a 0a2a 2a5b 4c65  t"))).```..**[Le
-00000f10: 6172 6e20 4d6f 7265 5d28 6874 7470 733a  arn More](https:
-00000f20: 2f2f 646f 6373 2e61 6461 7074 6572 6875  //docs.adapterhu
-00000f30: 622e 6d6c 2f61 6461 7074 6572 5f63 6f6d  b.ml/adapter_com
-00000f40: 706f 7369 7469 6f6e 2e68 746d 6c29 2a2a  position.html)**
-00000f50: 0a0a 2323 2055 7365 6675 6c20 5265 736f  ..## Useful Reso
-00000f60: 7572 6365 730a 0a48 7567 6769 6e67 4661  urces..HuggingFa
-00000f70: 6365 2773 2067 7265 6174 2064 6f63 756d  ce's great docum
-00000f80: 656e 7461 7469 6f6e 206f 6e20 6765 7474  entation on gett
-00000f90: 696e 6720 7374 6172 7465 6420 7769 7468  ing started with
-00000fa0: 205f 5472 616e 7366 6f72 6d65 7273 5f20   _Transformers_ 
-00000fb0: 6361 6e20 6265 2066 6f75 6e64 205b 6865  can be found [he
-00000fc0: 7265 5d28 6874 7470 733a 2f2f 6875 6767  re](https://hugg
-00000fd0: 696e 6766 6163 652e 636f 2f74 7261 6e73  ingface.co/trans
-00000fe0: 666f 726d 6572 732f 696e 6465 782e 6874  formers/index.ht
-00000ff0: 6d6c 292e 2060 6164 6170 7465 7273 6020  ml). `adapters` 
-00001000: 6973 2066 756c 6c79 2063 6f6d 7061 7469  is fully compati
-00001010: 626c 6520 7769 7468 205f 5472 616e 7366  ble with _Transf
-00001020: 6f72 6d65 7273 5f2e 0a0a 546f 2067 6574  ormers_...To get
-00001030: 2073 7461 7274 6564 2077 6974 6820 6164   started with ad
-00001040: 6170 7465 7273 2c20 7265 6665 7220 746f  apters, refer to
-00001050: 2074 6865 7365 206c 6f63 6174 696f 6e73   these locations
-00001060: 3a0a 0a2d 202a 2a5b 436f 6c61 6220 6e6f  :..- **[Colab no
-00001070: 7465 626f 6f6b 2074 7574 6f72 6961 6c73  tebook tutorials
-00001080: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-00001090: 2e63 6f6d 2f41 6461 7074 6572 2d48 7562  .com/Adapter-Hub
-000010a0: 2f61 6461 7074 6572 732f 7472 6565 2f6d  /adapters/tree/m
-000010b0: 6169 6e2f 6e6f 7465 626f 6f6b 7329 2a2a  ain/notebooks)**
-000010c0: 2c20 6120 7365 7269 6573 206e 6f74 6562  , a series noteb
-000010d0: 6f6f 6b73 2070 726f 7669 6469 6e67 2061  ooks providing a
-000010e0: 6e20 696e 7472 6f64 7563 7469 6f6e 2074  n introduction t
-000010f0: 6f20 616c 6c20 7468 6520 6d61 696e 2063  o all the main c
-00001100: 6f6e 6365 7074 7320 6f66 2028 6164 6170  oncepts of (adap
-00001110: 7465 722d 2974 7261 6e73 666f 726d 6572  ter-)transformer
-00001120: 7320 616e 6420 4164 6170 7465 7248 7562  s and AdapterHub
-00001130: 0a2d 202a 2a68 7474 7073 3a2f 2f64 6f63  .- **https://doc
-00001140: 732e 6164 6170 7465 7268 7562 2e6d 6c2a  s.adapterhub.ml*
-00001150: 2a2c 206f 7572 2064 6f63 756d 656e 7461  *, our documenta
-00001160: 7469 6f6e 206f 6e20 7472 6169 6e69 6e67  tion on training
-00001170: 2061 6e64 2075 7369 6e67 2061 6461 7074   and using adapt
-00001180: 6572 7320 7769 7468 205f 6164 6170 7465  ers with _adapte
-00001190: 7273 5f0a 2d20 2a2a 6874 7470 733a 2f2f  rs_.- **https://
-000011a0: 6164 6170 7465 7268 7562 2e6d 6c2a 2a20  adapterhub.ml** 
-000011b0: 746f 2065 7870 6c6f 7265 2061 7661 696c  to explore avail
-000011c0: 6162 6c65 2070 7265 2d74 7261 696e 6564  able pre-trained
-000011d0: 2061 6461 7074 6572 206d 6f64 756c 6573   adapter modules
-000011e0: 2061 6e64 2073 6861 7265 2079 6f75 7220   and share your 
-000011f0: 6f77 6e20 6164 6170 7465 7273 0a2d 202a  own adapters.- *
-00001200: 2a5b 4578 616d 706c 6573 2066 6f6c 6465  *[Examples folde
-00001210: 725d 2868 7474 7073 3a2f 2f67 6974 6875  r](https://githu
-00001220: 622e 636f 6d2f 4164 6170 7465 722d 4875  b.com/Adapter-Hu
-00001230: 622f 6164 6170 7465 7273 2f74 7265 652f  b/adapters/tree/
-00001240: 6d61 696e 2f65 7861 6d70 6c65 732f 7079  main/examples/py
-00001250: 746f 7263 6829 2a2a 206f 6620 7468 6973  torch)** of this
-00001260: 2072 6570 6f73 6974 6f72 7920 636f 6e74   repository cont
-00001270: 6169 6e69 6e67 2048 7567 6769 6e67 4661  aining HuggingFa
-00001280: 6365 2773 2065 7861 6d70 6c65 2074 7261  ce's example tra
-00001290: 696e 696e 6720 7363 7269 7074 732c 206d  ining scripts, m
-000012a0: 616e 7920 6164 6170 7465 6420 666f 7220  any adapted for 
-000012b0: 7472 6169 6e69 6e67 2061 6461 7074 6572  training adapter
-000012c0: 730a 0a23 2320 496d 706c 656d 656e 7465  s..## Implemente
-000012d0: 6420 4d65 7468 6f64 730a 0a43 7572 7265  d Methods..Curre
-000012e0: 6e74 6c79 2c20 6164 6170 7465 7273 2069  ntly, adapters i
-000012f0: 6e74 6567 7261 7465 7320 616c 6c20 6172  ntegrates all ar
-00001300: 6368 6974 6563 7475 7265 7320 616e 6420  chitectures and 
-00001310: 6d65 7468 6f64 7320 6c69 7374 6564 2062  methods listed b
-00001320: 656c 6f77 3a0a 0a7c 204d 6574 686f 6420  elow:..| Method 
-00001330: 7c20 5061 7065 7228 7329 207c 2051 7569  | Paper(s) | Qui
-00001340: 636b 204c 696e 6b73 207c 0a7c 202d 2d2d  ck Links |.| ---
-00001350: 207c 202d 2d2d 207c 202d 2d2d 207c 0a7c   | --- | --- |.|
-00001360: 2042 6f74 746c 656e 6563 6b20 6164 6170   Bottleneck adap
-00001370: 7465 7273 207c 205b 486f 756c 7362 7920  ters | [Houlsby 
-00001380: 6574 2061 6c2e 2028 3230 3139 295d 2868  et al. (2019)](h
-00001390: 7474 7073 3a2f 2f61 7278 6976 2e6f 7267  ttps://arxiv.org
-000013a0: 2f70 6466 2f31 3930 322e 3030 3735 312e  /pdf/1902.00751.
-000013b0: 7064 6629 3c62 723e 205b 4261 706e 6120  pdf)<br> [Bapna 
-000013c0: 616e 6420 4669 7261 7420 2832 3031 3929  and Firat (2019)
-000013d0: 5d28 6874 7470 733a 2f2f 6172 7869 762e  ](https://arxiv.
-000013e0: 6f72 672f 7064 662f 3139 3039 2e30 3834  org/pdf/1909.084
-000013f0: 3738 2e70 6466 2920 7c20 5b51 7569 636b  78.pdf) | [Quick
-00001400: 7374 6172 745d 2868 7474 7073 3a2f 2f64  start](https://d
-00001410: 6f63 732e 6164 6170 7465 7268 7562 2e6d  ocs.adapterhub.m
-00001420: 6c2f 7175 6963 6b73 7461 7274 2e68 746d  l/quickstart.htm
-00001430: 6c29 2c20 5b4e 6f74 6562 6f6f 6b5d 2868  l), [Notebook](h
-00001440: 7474 7073 3a2f 2f63 6f6c 6162 2e72 6573  ttps://colab.res
-00001450: 6561 7263 682e 676f 6f67 6c65 2e63 6f6d  earch.google.com
-00001460: 2f67 6974 6875 622f 4164 6170 7465 722d  /github/Adapter-
-00001470: 4875 622f 6164 6170 7465 7273 2f62 6c6f  Hub/adapters/blo
-00001480: 622f 6d61 696e 2f6e 6f74 6562 6f6f 6b73  b/main/notebooks
-00001490: 2f30 315f 4164 6170 7465 725f 5472 6169  /01_Adapter_Trai
-000014a0: 6e69 6e67 2e69 7079 6e62 2920 7c0a 7c20  ning.ipynb) |.| 
-000014b0: 4164 6170 7465 7246 7573 696f 6e20 7c20  AdapterFusion | 
-000014c0: 5b50 6665 6966 6665 7220 6574 2061 6c2e  [Pfeiffer et al.
-000014d0: 2028 3230 3231 295d 2868 7474 7073 3a2f   (2021)](https:/
-000014e0: 2f61 636c 616e 7468 6f6c 6f67 792e 6f72  /aclanthology.or
-000014f0: 672f 3230 3231 2e65 6163 6c2d 6d61 696e  g/2021.eacl-main
-00001500: 2e33 392e 7064 6629 207c 205b 446f 6373  .39.pdf) | [Docs
-00001510: 3a20 5472 6169 6e69 6e67 5d28 6874 7470  : Training](http
-00001520: 733a 2f2f 646f 6373 2e61 6461 7074 6572  s://docs.adapter
-00001530: 6875 622e 6d6c 2f74 7261 696e 696e 672e  hub.ml/training.
-00001540: 6874 6d6c 2374 7261 696e 2d61 6461 7074  html#train-adapt
-00001550: 6572 6675 7369 6f6e 292c 205b 4e6f 7465  erfusion), [Note
-00001560: 626f 6f6b 5d28 6874 7470 733a 2f2f 636f  book](https://co
-00001570: 6c61 622e 7265 7365 6172 6368 2e67 6f6f  lab.research.goo
-00001580: 676c 652e 636f 6d2f 6769 7468 7562 2f41  gle.com/github/A
-00001590: 6461 7074 6572 2d48 7562 2f61 6461 7074  dapter-Hub/adapt
-000015a0: 6572 732f 626c 6f62 2f6d 6169 6e2f 6e6f  ers/blob/main/no
-000015b0: 7465 626f 6f6b 732f 3033 5f41 6461 7074  tebooks/03_Adapt
-000015c0: 6572 5f46 7573 696f 6e2e 6970 796e 6229  er_Fusion.ipynb)
-000015d0: 207c 0a7c 204d 4144 2d58 2c3c 6272 3e20   |.| MAD-X,<br> 
-000015e0: 496e 7665 7274 6962 6c65 2061 6461 7074  Invertible adapt
-000015f0: 6572 7320 7c20 5b50 6665 6966 6665 7220  ers | [Pfeiffer 
-00001600: 6574 2061 6c2e 2028 3230 3230 295d 2868  et al. (2020)](h
-00001610: 7474 7073 3a2f 2f61 636c 616e 7468 6f6c  ttps://aclanthol
-00001620: 6f67 792e 6f72 672f 3230 3230 2e65 6d6e  ogy.org/2020.emn
-00001630: 6c70 2d6d 6169 6e2e 3631 372f 2920 7c20  lp-main.617/) | 
-00001640: 5b4e 6f74 6562 6f6f 6b5d 2868 7474 7073  [Notebook](https
-00001650: 3a2f 2f63 6f6c 6162 2e72 6573 6561 7263  ://colab.researc
-00001660: 682e 676f 6f67 6c65 2e63 6f6d 2f67 6974  h.google.com/git
-00001670: 6875 622f 4164 6170 7465 722d 4875 622f  hub/Adapter-Hub/
-00001680: 6164 6170 7465 7273 2f62 6c6f 622f 6d61  adapters/blob/ma
-00001690: 696e 2f6e 6f74 6562 6f6f 6b73 2f30 345f  in/notebooks/04_
-000016a0: 4372 6f73 735f 4c69 6e67 7561 6c5f 5472  Cross_Lingual_Tr
-000016b0: 616e 7366 6572 2e69 7079 6e62 2920 7c0a  ansfer.ipynb) |.
-000016c0: 7c20 4164 6170 7465 7244 726f 7020 7c20  | AdapterDrop | 
-000016d0: 5b52 c3bc 636b 6cc3 a920 6574 2061 6c2e  [R..ckl.. et al.
-000016e0: 2028 3230 3231 295d 2868 7474 7073 3a2f   (2021)](https:/
-000016f0: 2f61 7278 6976 2e6f 7267 2f70 6466 2f32  /arxiv.org/pdf/2
-00001700: 3031 302e 3131 3931 382e 7064 6629 207c  010.11918.pdf) |
-00001710: 205b 4e6f 7465 626f 6f6b 5d28 6874 7470   [Notebook](http
-00001720: 733a 2f2f 636f 6c61 622e 7265 7365 6172  s://colab.resear
-00001730: 6368 2e67 6f6f 676c 652e 636f 6d2f 6769  ch.google.com/gi
-00001740: 7468 7562 2f41 6461 7074 6572 2d48 7562  thub/Adapter-Hub
-00001750: 2f61 6461 7074 6572 732f 626c 6f62 2f6d  /adapters/blob/m
-00001760: 6169 6e2f 6e6f 7465 626f 6f6b 732f 3035  ain/notebooks/05
-00001770: 5f41 6461 7074 6572 5f44 726f 705f 5472  _Adapter_Drop_Tr
-00001780: 6169 6e69 6e67 2e69 7079 6e62 2920 7c0a  aining.ipynb) |.
-00001790: 7c20 4d41 442d 5820 322e 302c 3c62 723e  | MAD-X 2.0,<br>
-000017a0: 2045 6d62 6564 6469 6e67 2074 7261 696e   Embedding train
-000017b0: 696e 6720 7c20 5b50 6665 6966 6665 7220  ing | [Pfeiffer 
-000017c0: 6574 2061 6c2e 2028 3230 3231 295d 2868  et al. (2021)](h
-000017d0: 7474 7073 3a2f 2f61 7278 6976 2e6f 7267  ttps://arxiv.org
-000017e0: 2f70 6466 2f32 3031 322e 3135 3536 322e  /pdf/2012.15562.
-000017f0: 7064 6629 207c 205b 446f 6373 3a20 456d  pdf) | [Docs: Em
-00001800: 6265 6464 696e 6773 5d28 6874 7470 733a  beddings](https:
-00001810: 2f2f 646f 6373 2e61 6461 7074 6572 6875  //docs.adapterhu
-00001820: 622e 6d6c 2f65 6d62 6564 6469 6e67 732e  b.ml/embeddings.
-00001830: 6874 6d6c 292c 205b 4e6f 7465 626f 6f6b  html), [Notebook
-00001840: 5d28 6874 7470 733a 2f2f 636f 6c61 622e  ](https://colab.
-00001850: 7265 7365 6172 6368 2e67 6f6f 676c 652e  research.google.
-00001860: 636f 6d2f 6769 7468 7562 2f41 6461 7074  com/github/Adapt
-00001870: 6572 2d48 7562 2f61 6461 7074 6572 732f  er-Hub/adapters/
-00001880: 626c 6f62 2f6d 6169 6e2f 6e6f 7465 626f  blob/main/notebo
-00001890: 6f6b 732f 3038 5f4e 4552 5f57 696b 6961  oks/08_NER_Wikia
-000018a0: 6e6e 2e69 7079 6e62 2920 7c0a 7c20 5072  nn.ipynb) |.| Pr
-000018b0: 6566 6978 2054 756e 696e 6720 7c20 5b4c  efix Tuning | [L
-000018c0: 6920 616e 6420 4c69 616e 6720 2832 3032  i and Liang (202
-000018d0: 3129 5d28 6874 7470 733a 2f2f 6172 7869  1)](https://arxi
-000018e0: 762e 6f72 672f 7064 662f 3231 3031 2e30  v.org/pdf/2101.0
-000018f0: 3031 3930 2e70 6466 2920 7c20 5b44 6f63  0190.pdf) | [Doc
-00001900: 735d 2868 7474 7073 3a2f 2f64 6f63 732e  s](https://docs.
-00001910: 6164 6170 7465 7268 7562 2e6d 6c2f 6d65  adapterhub.ml/me
-00001920: 7468 6f64 732e 6874 6d6c 2370 7265 6669  thods.html#prefi
-00001930: 782d 7475 6e69 6e67 2920 7c0a 7c20 5061  x-tuning) |.| Pa
-00001940: 7261 6c6c 656c 2061 6461 7074 6572 732c  rallel adapters,
-00001950: 3c62 723e 204d 6978 2d61 6e64 2d4d 6174  <br> Mix-and-Mat
-00001960: 6368 2061 6461 7074 6572 7320 7c20 5b48  ch adapters | [H
-00001970: 6520 6574 2061 6c2e 2028 3230 3231 295d  e et al. (2021)]
-00001980: 2868 7474 7073 3a2f 2f61 7278 6976 2e6f  (https://arxiv.o
-00001990: 7267 2f70 6466 2f32 3131 302e 3034 3336  rg/pdf/2110.0436
-000019a0: 362e 7064 6629 207c 205b 446f 6373 5d28  6.pdf) | [Docs](
-000019b0: 6874 7470 733a 2f2f 646f 6373 2e61 6461  https://docs.ada
-000019c0: 7074 6572 6875 622e 6d6c 2f6d 6574 686f  pterhub.ml/metho
-000019d0: 645f 636f 6d62 696e 6174 696f 6e73 2e68  d_combinations.h
-000019e0: 746d 6c23 6d69 782d 616e 642d 6d61 7463  tml#mix-and-matc
-000019f0: 682d 6164 6170 7465 7273 2920 7c0a 7c20  h-adapters) |.| 
-00001a00: 436f 6d70 6163 7465 7220 7c20 5b4d 6168  Compacter | [Mah
-00001a10: 6162 6164 6920 6574 2061 6c2e 2028 3230  abadi et al. (20
-00001a20: 3231 295d 2868 7474 7073 3a2f 2f61 7278  21)](https://arx
-00001a30: 6976 2e6f 7267 2f70 6466 2f32 3130 362e  iv.org/pdf/2106.
-00001a40: 3034 3634 372e 7064 6629 207c 205b 446f  04647.pdf) | [Do
-00001a50: 6373 5d28 6874 7470 733a 2f2f 646f 6373  cs](https://docs
-00001a60: 2e61 6461 7074 6572 6875 622e 6d6c 2f6d  .adapterhub.ml/m
-00001a70: 6574 686f 6473 2e68 746d 6c23 636f 6d70  ethods.html#comp
-00001a80: 6163 7465 7229 207c 0a7c 204c 6f52 4120  acter) |.| LoRA 
-00001a90: 7c20 5b48 7520 6574 2061 6c2e 2028 3230  | [Hu et al. (20
-00001aa0: 3231 295d 2868 7474 7073 3a2f 2f61 7278  21)](https://arx
-00001ab0: 6976 2e6f 7267 2f70 6466 2f32 3130 362e  iv.org/pdf/2106.
-00001ac0: 3039 3638 352e 7064 6629 207c 205b 446f  09685.pdf) | [Do
-00001ad0: 6373 5d28 6874 7470 733a 2f2f 646f 6373  cs](https://docs
-00001ae0: 2e61 6461 7074 6572 6875 622e 6d6c 2f6d  .adapterhub.ml/m
-00001af0: 6574 686f 6473 2e68 746d 6c23 6c6f 7261  ethods.html#lora
-00001b00: 2920 7c0a 7c20 2849 4129 5e33 207c 205b  ) |.| (IA)^3 | [
-00001b10: 4c69 7520 6574 2061 6c2e 2028 3230 3232  Liu et al. (2022
-00001b20: 295d 2868 7474 7073 3a2f 2f61 7278 6976  )](https://arxiv
-00001b30: 2e6f 7267 2f70 6466 2f32 3230 352e 3035  .org/pdf/2205.05
-00001b40: 3633 382e 7064 6629 207c 205b 446f 6373  638.pdf) | [Docs
-00001b50: 5d28 6874 7470 733a 2f2f 646f 6373 2e61  ](https://docs.a
-00001b60: 6461 7074 6572 6875 622e 6d6c 2f6d 6574  dapterhub.ml/met
-00001b70: 686f 6473 2e68 746d 6c23 6961 2d33 2920  hods.html#ia-3) 
-00001b80: 7c0a 7c20 556e 6950 454c 5420 7c20 5b4d  |.| UniPELT | [M
-00001b90: 616f 2065 7420 616c 2e20 2832 3032 3229  ao et al. (2022)
-00001ba0: 5d28 6874 7470 733a 2f2f 6172 7869 762e  ](https://arxiv.
-00001bb0: 6f72 672f 7064 662f 3231 3130 2e30 3735  org/pdf/2110.075
-00001bc0: 3737 2e70 6466 2920 7c20 5b44 6f63 735d  77.pdf) | [Docs]
-00001bd0: 2868 7474 7073 3a2f 2f64 6f63 732e 6164  (https://docs.ad
-00001be0: 6170 7465 7268 7562 2e6d 6c2f 6d65 7468  apterhub.ml/meth
-00001bf0: 6f64 5f63 6f6d 6269 6e61 7469 6f6e 732e  od_combinations.
-00001c00: 6874 6d6c 2375 6e69 7065 6c74 2920 7c0a  html#unipelt) |.
-00001c10: 7c20 5072 6f6d 7074 2054 756e 696e 6720  | Prompt Tuning 
-00001c20: 7c20 5b4c 6573 7465 7220 6574 2061 6c2e  | [Lester et al.
-00001c30: 2028 3230 3231 295d 2868 7474 7073 3a2f   (2021)](https:/
-00001c40: 2f61 636c 616e 7468 6f6c 6f67 792e 6f72  /aclanthology.or
-00001c50: 672f 3230 3231 2e65 6d6e 6c70 2d6d 6169  g/2021.emnlp-mai
-00001c60: 6e2e 3234 332f 2920 7c20 5b44 6f63 735d  n.243/) | [Docs]
-00001c70: 2868 7474 7073 3a2f 2f64 6f63 732e 6164  (https://docs.ad
-00001c80: 6170 7465 7268 7562 2e6d 6c2f 6d65 7468  apterhub.ml/meth
-00001c90: 6f64 732e 6874 6d6c 2370 726f 6d70 742d  ods.html#prompt-
-00001ca0: 7475 6e69 6e67 2920 7c0a 0a23 2320 5375  tuning) |..## Su
-00001cb0: 7070 6f72 7465 6420 4d6f 6465 6c73 0a0a  pported Models..
-00001cc0: 5765 2063 7572 7265 6e74 6c79 2073 7570  We currently sup
-00001cd0: 706f 7274 2074 6865 2050 7954 6f72 6368  port the PyTorch
-00001ce0: 2076 6572 7369 6f6e 7320 6f66 2061 6c6c   versions of all
-00001cf0: 206d 6f64 656c 7320 6c69 7374 6564 206f   models listed o
-00001d00: 6e20 7468 6520 2a2a 5b4d 6f64 656c 204f  n the **[Model O
-00001d10: 7665 7276 6965 775d 2868 7474 7073 3a2f  verview](https:/
-00001d20: 2f64 6f63 732e 6164 6170 7465 7268 7562  /docs.adapterhub
-00001d30: 2e6d 6c2f 6d6f 6465 6c5f 6f76 6572 7669  .ml/model_overvi
-00001d40: 6577 2e68 746d 6c29 2070 6167 652a 2a20  ew.html) page** 
-00001d50: 696e 206f 7572 2064 6f63 756d 656e 7461  in our documenta
-00001d60: 7469 6f6e 2e0a 0a23 2320 4465 7665 6c6f  tion...## Develo
-00001d70: 7069 6e67 2026 2043 6f6e 7472 6962 7574  ping & Contribut
-00001d80: 696e 670a 0a54 6f20 6765 7420 7374 6172  ing..To get star
-00001d90: 7465 6420 7769 7468 2064 6576 656c 6f70  ted with develop
-00001da0: 696e 6720 6f6e 205f 4164 6170 7465 7273  ing on _Adapters
-00001db0: 5f20 796f 7572 7365 6c66 2061 6e64 206c  _ yourself and l
-00001dc0: 6561 726e 206d 6f72 6520 6162 6f75 7420  earn more about 
-00001dd0: 7761 7973 2074 6f20 636f 6e74 7269 6275  ways to contribu
-00001de0: 7465 2c20 706c 6561 7365 2073 6565 2068  te, please see h
-00001df0: 7474 7073 3a2f 2f64 6f63 732e 6164 6170  ttps://docs.adap
-00001e00: 7465 7268 7562 2e6d 6c2f 636f 6e74 7269  terhub.ml/contri
-00001e10: 6275 7469 6e67 2e68 746d 6c2e 0a0a 2323  buting.html...##
-00001e20: 2043 6974 6174 696f 6e0a 0a49 6620 796f   Citation..If yo
-00001e30: 7520 7573 6520 5f41 6461 7074 6572 735f  u use _Adapters_
-00001e40: 2069 6e20 796f 7572 2077 6f72 6b2c 2070   in your work, p
-00001e50: 6c65 6173 6520 636f 6e73 6964 6572 2063  lease consider c
-00001e60: 6974 696e 6720 6f75 7220 6c69 6272 6172  iting our librar
-00001e70: 7920 7061 7065 723a 205b 4164 6170 7465  y paper: [Adapte
-00001e80: 7273 3a20 4120 556e 6966 6965 6420 4c69  rs: A Unified Li
-00001e90: 6272 6172 7920 666f 7220 5061 7261 6d65  brary for Parame
-00001ea0: 7465 722d 4566 6669 6369 656e 7420 616e  ter-Efficient an
-00001eb0: 6420 4d6f 6475 6c61 7220 5472 616e 7366  d Modular Transf
-00001ec0: 6572 204c 6561 726e 696e 675d 2868 7474  er Learning](htt
-00001ed0: 7073 3a2f 2f61 7278 6976 2e6f 7267 2f61  ps://arxiv.org/a
-00001ee0: 6273 2f32 3331 312e 3131 3037 3729 0a0a  bs/2311.11077)..
-00001ef0: 6060 600a 4069 6e70 726f 6365 6564 696e  ```.@inproceedin
-00001f00: 6773 7b70 6f74 682d 6574 616c 2d32 3032  gs{poth-etal-202
-00001f10: 332d 6164 6170 7465 7273 2c0a 2020 2020  3-adapters,.    
-00001f20: 7469 746c 6520 3d20 2241 6461 7074 6572  title = "Adapter
-00001f30: 733a 2041 2055 6e69 6669 6564 204c 6962  s: A Unified Lib
-00001f40: 7261 7279 2066 6f72 2050 6172 616d 6574  rary for Paramet
-00001f50: 6572 2d45 6666 6963 6965 6e74 2061 6e64  er-Efficient and
-00001f60: 204d 6f64 756c 6172 2054 7261 6e73 6665   Modular Transfe
-00001f70: 7220 4c65 6172 6e69 6e67 222c 0a20 2020  r Learning",.   
-00001f80: 2061 7574 686f 7220 3d20 7b50 6f74 682c   author = {Poth,
-00001f90: 2043 6c69 6674 6f6e 2020 616e 640a 2020   Clifton  and.  
-00001fa0: 2020 2020 5374 6572 7a2c 2048 616e 6e61      Sterz, Hanna
-00001fb0: 6820 2061 6e64 0a20 2020 2020 2050 6175  h  and.      Pau
-00001fc0: 6c2c 2049 6e64 7261 6e65 696c 2020 616e  l, Indraneil  an
-00001fd0: 640a 2020 2020 2020 5075 726b 6179 6173  d.      Purkayas
-00001fe0: 7468 612c 2053 756b 616e 6e79 6120 2061  tha, Sukannya  a
-00001ff0: 6e64 0a20 2020 2020 2045 6e67 6c7b 5c22  nd.      Engl{\"
-00002000: 617d 6e64 6572 2c20 4c65 6f6e 2020 616e  a}nder, Leon  an
-00002010: 640a 2020 2020 2020 496d 686f 662c 2054  d.      Imhof, T
-00002020: 696d 6f20 2061 6e64 0a20 2020 2020 2056  imo  and.      V
-00002030: 756c 697b 5c27 637d 2c20 4976 616e 2020  uli{\'c}, Ivan  
-00002040: 616e 640a 2020 2020 2020 5275 6465 722c  and.      Ruder,
-00002050: 2053 6562 6173 7469 616e 2020 616e 640a   Sebastian  and.
-00002060: 2020 2020 2020 4775 7265 7679 6368 2c20        Gurevych, 
-00002070: 4972 796e 6120 2061 6e64 0a20 2020 2020  Iryna  and.     
-00002080: 2050 6665 6966 6665 722c 204a 6f6e 6173   Pfeiffer, Jonas
-00002090: 7d2c 0a20 2020 2062 6f6f 6b74 6974 6c65  },.    booktitle
-000020a0: 203d 2022 5072 6f63 6565 6469 6e67 7320   = "Proceedings 
-000020b0: 6f66 2074 6865 2032 3032 3320 436f 6e66  of the 2023 Conf
-000020c0: 6572 656e 6365 206f 6e20 456d 7069 7269  erence on Empiri
-000020d0: 6361 6c20 4d65 7468 6f64 7320 696e 204e  cal Methods in N
-000020e0: 6174 7572 616c 204c 616e 6775 6167 6520  atural Language 
-000020f0: 5072 6f63 6573 7369 6e67 3a20 5379 7374  Processing: Syst
-00002100: 656d 2044 656d 6f6e 7374 7261 7469 6f6e  em Demonstration
-00002110: 7322 2c0a 2020 2020 6d6f 6e74 6820 3d20  s",.    month = 
-00002120: 6465 632c 0a20 2020 2079 6561 7220 3d20  dec,.    year = 
-00002130: 2232 3032 3322 2c0a 2020 2020 6164 6472  "2023",.    addr
-00002140: 6573 7320 3d20 2253 696e 6761 706f 7265  ess = "Singapore
-00002150: 222c 0a20 2020 2070 7562 6c69 7368 6572  ",.    publisher
-00002160: 203d 2022 4173 736f 6369 6174 696f 6e20   = "Association 
-00002170: 666f 7220 436f 6d70 7574 6174 696f 6e61  for Computationa
-00002180: 6c20 4c69 6e67 7569 7374 6963 7322 2c0a  l Linguistics",.
-00002190: 2020 2020 7572 6c20 3d20 2268 7474 7073      url = "https
-000021a0: 3a2f 2f61 636c 616e 7468 6f6c 6f67 792e  ://aclanthology.
-000021b0: 6f72 672f 3230 3233 2e65 6d6e 6c70 2d64  org/2023.emnlp-d
-000021c0: 656d 6f2e 3133 222c 0a20 2020 2070 6167  emo.13",.    pag
-000021d0: 6573 203d 2022 3134 392d 2d31 3630 222c  es = "149--160",
-000021e0: 0a7d 0a60 6060 0a0a 416c 7465 726e 6174  .}.```..Alternat
-000021f0: 6976 656c 792c 2066 6f72 2074 6865 2070  ively, for the p
-00002200: 7265 6465 6365 7373 6f72 2060 6164 6170  redecessor `adap
-00002210: 7465 722d 7472 616e 7366 6f72 6d65 7273  ter-transformers
-00002220: 602c 2074 6865 2048 7562 2069 6e66 7261  `, the Hub infra
-00002230: 7374 7275 6374 7572 6520 616e 6420 6164  structure and ad
-00002240: 6170 7465 7273 2075 706c 6f61 6465 6420  apters uploaded 
-00002250: 6279 2074 6865 2041 6461 7074 6572 4875  by the AdapterHu
-00002260: 6220 7465 616d 2c20 706c 6561 7365 2063  b team, please c
-00002270: 6f6e 7369 6465 7220 6369 7469 6e67 206f  onsider citing o
-00002280: 7572 2069 6e69 7469 616c 2070 6170 6572  ur initial paper
-00002290: 3a20 5b41 6461 7074 6572 4875 623a 2041  : [AdapterHub: A
-000022a0: 2046 7261 6d65 776f 726b 2066 6f72 2041   Framework for A
-000022b0: 6461 7074 696e 6720 5472 616e 7366 6f72  dapting Transfor
-000022c0: 6d65 7273 5d28 6874 7470 733a 2f2f 6172  mers](https://ar
-000022d0: 7869 762e 6f72 672f 6162 732f 3230 3037  xiv.org/abs/2007
-000022e0: 2e30 3737 3739 290a 0a60 6060 0a40 696e  .07779)..```.@in
-000022f0: 7072 6f63 6565 6469 6e67 737b 7066 6569  proceedings{pfei
-00002300: 6666 6572 3230 3230 4164 6170 7465 7248  ffer2020AdapterH
-00002310: 7562 2c0a 2020 2020 7469 746c 653d 7b41  ub,.    title={A
-00002320: 6461 7074 6572 4875 623a 2041 2046 7261  dapterHub: A Fra
-00002330: 6d65 776f 726b 2066 6f72 2041 6461 7074  mework for Adapt
-00002340: 696e 6720 5472 616e 7366 6f72 6d65 7273  ing Transformers
-00002350: 7d2c 0a20 2020 2061 7574 686f 723d 7b50  },.    author={P
-00002360: 6665 6966 6665 722c 204a 6f6e 6173 2061  feiffer, Jonas a
-00002370: 6e64 0a20 2020 2020 2020 2020 2020 2052  nd.            R
-00002380: 7b5c 2275 7d63 6b6c 7b5c 2765 7d2c 2041  {\"u}ckl{\'e}, A
-00002390: 6e64 7265 6173 2061 6e64 0a20 2020 2020  ndreas and.     
-000023a0: 2020 2020 2020 2050 6f74 682c 2043 6c69         Poth, Cli
-000023b0: 6674 6f6e 2061 6e64 0a20 2020 2020 2020  fton and.       
-000023c0: 2020 2020 204b 616d 6174 682c 2041 6973       Kamath, Ais
-000023d0: 6877 6172 7961 2061 6e64 0a20 2020 2020  hwarya and.     
-000023e0: 2020 2020 2020 2056 756c 697b 5c27 637d         Vuli{\'c}
-000023f0: 2c20 4976 616e 2061 6e64 0a20 2020 2020  , Ivan and.     
-00002400: 2020 2020 2020 2052 7564 6572 2c20 5365         Ruder, Se
-00002410: 6261 7374 6961 6e20 616e 640a 2020 2020  bastian and.    
-00002420: 2020 2020 2020 2020 4368 6f2c 204b 7975          Cho, Kyu
-00002430: 6e67 6879 756e 2061 6e64 0a20 2020 2020  nghyun and.     
-00002440: 2020 2020 2020 2047 7572 6576 7963 682c         Gurevych,
-00002450: 2049 7279 6e61 7d2c 0a20 2020 2062 6f6f   Iryna},.    boo
-00002460: 6b74 6974 6c65 3d7b 5072 6f63 6565 6469  ktitle={Proceedi
-00002470: 6e67 7320 6f66 2074 6865 2032 3032 3020  ngs of the 2020 
-00002480: 436f 6e66 6572 656e 6365 206f 6e20 456d  Conference on Em
-00002490: 7069 7269 6361 6c20 4d65 7468 6f64 7320  pirical Methods 
-000024a0: 696e 204e 6174 7572 616c 204c 616e 6775  in Natural Langu
-000024b0: 6167 6520 5072 6f63 6573 7369 6e67 3a20  age Processing: 
-000024c0: 5379 7374 656d 2044 656d 6f6e 7374 7261  System Demonstra
-000024d0: 7469 6f6e 737d 2c0a 2020 2020 7061 6765  tions},.    page
-000024e0: 733d 7b34 362d 2d35 347d 2c0a 2020 2020  s={46--54},.    
-000024f0: 7965 6172 3d7b 3230 3230 7d0a 7d0a 6060  year={2020}.}.``
-00002500: 600a                                     `.
+00000250: 0a3c 7020 616c 6967 6e3d 2263 656e 7465  .<p align="cente
+00000260: 7222 3e0a 3c69 6d67 2073 7479 6c65 3d22  r">.<img style="
+00000270: 7665 7274 6963 616c 2d61 6c69 676e 3a6d  vertical-align:m
+00000280: 6964 646c 6522 2073 7263 3d22 6874 7470  iddle" src="http
+00000290: 733a 2f2f 7261 772e 6769 7468 7562 7573  s://raw.githubus
+000002a0: 6572 636f 6e74 656e 742e 636f 6d2f 4164  ercontent.com/Ad
+000002b0: 6170 7465 722d 4875 622f 6164 6170 7465  apter-Hub/adapte
+000002c0: 7273 2f6d 6169 6e2f 646f 6373 2f69 6d67  rs/main/docs/img
+000002d0: 2f61 6461 7074 6572 2d62 6572 742e 706e  /adapter-bert.pn
+000002e0: 6722 2077 6964 7468 3d22 3830 2220 2f3e  g" width="80" />
+000002f0: 0a3c 2f70 3e0a 3c68 3120 616c 6967 6e3d  .</p>.<h1 align=
+00000300: 2263 656e 7465 7222 3e0a 3c73 7061 6e3e  "center">.<span>
+00000310: 3c69 3e41 6461 7074 6572 733c 2f69 3e3c  <i>Adapters</i><
+00000320: 2f73 7061 6e3e 0a3c 2f68 313e 0a0a 3c68  /span>.</h1>..<h
+00000330: 3320 616c 6967 6e3d 2263 656e 7465 7222  3 align="center"
+00000340: 3e0a 4120 556e 6966 6965 6420 4c69 6272  >.A Unified Libr
+00000350: 6172 7920 666f 7220 5061 7261 6d65 7465  ary for Paramete
+00000360: 722d 4566 6669 6369 656e 7420 616e 6420  r-Efficient and 
+00000370: 4d6f 6475 6c61 7220 5472 616e 7366 6572  Modular Transfer
+00000380: 204c 6561 726e 696e 670a 3c2f 6833 3e0a   Learning.</h3>.
+00000390: 3c68 3320 616c 6967 6e3d 2263 656e 7465  <h3 align="cente
+000003a0: 7222 3e0a 2020 2020 3c61 2068 7265 663d  r">.    <a href=
+000003b0: 2268 7474 7073 3a2f 2f61 6461 7074 6572  "https://adapter
+000003c0: 6875 622e 6d6c 223e 5765 6273 6974 653c  hub.ml">Website<
+000003d0: 2f61 3e0a 2020 2020 266e 6273 703b 20e2  /a>.    &nbsp; .
+000003e0: 80a2 2026 6e62 7370 3b0a 2020 2020 3c61  .. &nbsp;.    <a
+000003f0: 2068 7265 663d 2268 7474 7073 3a2f 2f64   href="https://d
+00000400: 6f63 732e 6164 6170 7465 7268 7562 2e6d  ocs.adapterhub.m
+00000410: 6c22 3e44 6f63 756d 656e 7461 7469 6f6e  l">Documentation
+00000420: 3c2f 613e 0a20 2020 2026 6e62 7370 3b20  </a>.    &nbsp; 
+00000430: e280 a220 266e 6273 703b 0a20 2020 203c  ... &nbsp;.    <
+00000440: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
+00000450: 6172 7869 762e 6f72 672f 6162 732f 3233  arxiv.org/abs/23
+00000460: 3131 2e31 3130 3737 223e 5061 7065 723c  11.11077">Paper<
+00000470: 2f61 3e0a 3c2f 6833 3e0a 0a21 5b54 6573  /a>.</h3>..![Tes
+00000480: 7473 5d28 6874 7470 733a 2f2f 6769 7468  ts](https://gith
+00000490: 7562 2e63 6f6d 2f41 6461 7074 6572 2d48  ub.com/Adapter-H
+000004a0: 7562 2f61 6461 7074 6572 732f 776f 726b  ub/adapters/work
+000004b0: 666c 6f77 732f 5465 7374 732f 6261 6467  flows/Tests/badg
+000004c0: 652e 7376 673f 6272 616e 6368 3d61 6461  e.svg?branch=ada
+000004d0: 7074 6572 7329 0a5b 215b 4769 7448 7562  pters).[![GitHub
+000004e0: 5d28 6874 7470 733a 2f2f 696d 672e 7368  ](https://img.sh
+000004f0: 6965 6c64 732e 696f 2f67 6974 6875 622f  ields.io/github/
+00000500: 6c69 6365 6e73 652f 6164 6170 7465 722d  license/adapter-
+00000510: 6875 622f 6164 6170 7465 7273 2e73 7667  hub/adapters.svg
+00000520: 3f63 6f6c 6f72 3d62 6c75 6529 5d28 6874  ?color=blue)](ht
+00000530: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000540: 2f61 6461 7074 6572 2d68 7562 2f61 6461  /adapter-hub/ada
+00000550: 7074 6572 732f 626c 6f62 2f6d 6169 6e2f  pters/blob/main/
+00000560: 4c49 4345 4e53 4529 0a5b 215b 5079 5049  LICENSE).[![PyPI
+00000570: 5d28 6874 7470 733a 2f2f 696d 672e 7368  ](https://img.sh
+00000580: 6965 6c64 732e 696f 2f70 7970 692f 762f  ields.io/pypi/v/
+00000590: 6164 6170 7465 7273 295d 2868 7474 7073  adapters)](https
+000005a0: 3a2f 2f70 7970 692e 6f72 672f 7072 6f6a  ://pypi.org/proj
+000005b0: 6563 742f 6164 6170 7465 7273 2f29 0a0a  ect/adapters/)..
+000005c0: 5f41 6461 7074 6572 735f 2069 7320 616e  _Adapters_ is an
+000005d0: 2061 6464 2d6f 6e20 6c69 6272 6172 7920   add-on library 
+000005e0: 746f 205b 4875 6767 696e 6746 6163 6527  to [HuggingFace'
+000005f0: 7320 5472 616e 7366 6f72 6d65 7273 5d28  s Transformers](
+00000600: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000610: 6f6d 2f68 7567 6769 6e67 6661 6365 2f74  om/huggingface/t
+00000620: 7261 6e73 666f 726d 6572 7329 2c20 696e  ransformers), in
+00000630: 7465 6772 6174 696e 6720 5b76 6172 696f  tegrating [vario
+00000640: 7573 2061 6461 7074 6572 206d 6574 686f  us adapter metho
+00000650: 6473 5d28 6874 7470 733a 2f2f 646f 6373  ds](https://docs
+00000660: 2e61 6461 7074 6572 6875 622e 6d6c 2f6f  .adapterhub.ml/o
+00000670: 7665 7276 6965 772e 6874 6d6c 2920 696e  verview.html) in
+00000680: 746f 205b 7374 6174 652d 6f66 2d74 6865  to [state-of-the
+00000690: 2d61 7274 2070 7265 2d74 7261 696e 6564  -art pre-trained
+000006a0: 206c 616e 6775 6167 6520 6d6f 6465 6c73   language models
+000006b0: 5d28 6874 7470 733a 2f2f 646f 6373 2e61  ](https://docs.a
+000006c0: 6461 7074 6572 6875 622e 6d6c 2f6d 6f64  dapterhub.ml/mod
+000006d0: 656c 5f6f 7665 7276 6965 772e 6874 6d6c  el_overview.html
+000006e0: 2920 7769 7468 206d 696e 696d 616c 2063  ) with minimal c
+000006f0: 6f64 696e 6720 6f76 6572 6865 6164 2066  oding overhead f
+00000700: 6f72 2074 7261 696e 696e 6720 616e 6420  or training and 
+00000710: 696e 6665 7265 6e63 652e 0a0a 3e20 2a2a  inference...> **
+00000720: 4e6f 7465 2a2a 3a20 5468 6520 5f41 6461  Note**: The _Ada
+00000730: 7074 6572 735f 206c 6962 7261 7279 2068  pters_ library h
+00000740: 6173 2072 6570 6c61 6365 6420 7468 6520  as replaced the 
+00000750: 6061 6461 7074 6572 2d74 7261 6e73 666f  `adapter-transfo
+00000760: 726d 6572 7360 2070 6163 6b61 6765 2e20  rmers` package. 
+00000770: 416c 6c20 7072 6576 696f 7573 6c79 2074  All previously t
+00000780: 7261 696e 6564 2061 6461 7074 6572 7320  rained adapters 
+00000790: 6172 6520 636f 6d70 6174 6962 6c65 2077  are compatible w
+000007a0: 6974 6820 7468 6520 6e65 7720 6c69 6272  ith the new libr
+000007b0: 6172 792e 2046 6f72 2074 7261 6e73 6974  ary. For transit
+000007c0: 696f 6e69 6e67 2c20 706c 6561 7365 2072  ioning, please r
+000007d0: 6561 643a 2068 7474 7073 3a2f 2f64 6f63  ead: https://doc
+000007e0: 732e 6164 6170 7465 7268 7562 2e6d 6c2f  s.adapterhub.ml/
+000007f0: 7472 616e 7369 7469 6f6e 696e 672e 6874  transitioning.ht
+00000800: 6d6c 2e0a 0a23 2320 496e 7374 616c 6c61  ml...## Installa
+00000810: 7469 6f6e 0a0a 6061 6461 7074 6572 7360  tion..`adapters`
+00000820: 2063 7572 7265 6e74 6c79 2073 7570 706f   currently suppo
+00000830: 7274 7320 2a2a 5079 7468 6f6e 2033 2e38  rts **Python 3.8
+00000840: 2b2a 2a20 616e 6420 2a2a 5079 546f 7263  +** and **PyTorc
+00000850: 6820 312e 3130 2b2a 2a2e 0a41 6674 6572  h 1.10+**..After
+00000860: 205b 696e 7374 616c 6c69 6e67 2050 7954   [installing PyT
+00000870: 6f72 6368 5d28 6874 7470 733a 2f2f 7079  orch](https://py
+00000880: 746f 7263 682e 6f72 672f 6765 742d 7374  torch.org/get-st
+00000890: 6172 7465 642f 6c6f 6361 6c6c 792f 292c  arted/locally/),
+000008a0: 2079 6f75 2063 616e 2069 6e73 7461 6c6c   you can install
+000008b0: 2060 6164 6170 7465 7273 6020 6672 6f6d   `adapters` from
+000008c0: 2050 7950 4920 2e2e 2e0a 0a60 6060 0a70   PyPI .....```.p
+000008d0: 6970 2069 6e73 7461 6c6c 202d 5520 6164  ip install -U ad
+000008e0: 6170 7465 7273 0a60 6060 0a0a 2e2e 2e20  apters.```..... 
+000008f0: 6f72 2066 726f 6d20 736f 7572 6365 2062  or from source b
+00000900: 7920 636c 6f6e 696e 6720 7468 6520 7265  y cloning the re
+00000910: 706f 7369 746f 7279 3a0a 0a60 6060 0a67  pository:..```.g
+00000920: 6974 2063 6c6f 6e65 2068 7474 7073 3a2f  it clone https:/
+00000930: 2f67 6974 6875 622e 636f 6d2f 6164 6170  /github.com/adap
+00000940: 7465 722d 6875 622f 6164 6170 7465 7273  ter-hub/adapters
+00000950: 2e67 6974 0a63 6420 6164 6170 7465 7273  .git.cd adapters
+00000960: 0a70 6970 2069 6e73 7461 6c6c 202e 0a60  .pip install ..`
+00000970: 6060 0a0a 2323 2051 7569 636b 2054 6f75  ``..## Quick Tou
+00000980: 720a 0a23 2323 2320 4c6f 6164 2070 7265  r..#### Load pre
+00000990: 2d74 7261 696e 6564 2061 6461 7074 6572  -trained adapter
+000009a0: 733a 0a0a 6060 6070 7974 686f 6e0a 6672  s:..```python.fr
+000009b0: 6f6d 2061 6461 7074 6572 7320 696d 706f  om adapters impo
+000009c0: 7274 2041 7574 6f41 6461 7074 6572 4d6f  rt AutoAdapterMo
+000009d0: 6465 6c0a 6672 6f6d 2074 7261 6e73 666f  del.from transfo
+000009e0: 726d 6572 7320 696d 706f 7274 2041 7574  rmers import Aut
+000009f0: 6f54 6f6b 656e 697a 6572 0a0a 6d6f 6465  oTokenizer..mode
+00000a00: 6c20 3d20 4175 746f 4164 6170 7465 724d  l = AutoAdapterM
+00000a10: 6f64 656c 2e66 726f 6d5f 7072 6574 7261  odel.from_pretra
+00000a20: 696e 6564 2822 726f 6265 7274 612d 6261  ined("roberta-ba
+00000a30: 7365 2229 0a74 6f6b 656e 697a 6572 203d  se").tokenizer =
+00000a40: 2041 7574 6f54 6f6b 656e 697a 6572 2e66   AutoTokenizer.f
+00000a50: 726f 6d5f 7072 6574 7261 696e 6564 2822  rom_pretrained("
+00000a60: 726f 6265 7274 612d 6261 7365 2229 0a0a  roberta-base")..
+00000a70: 6d6f 6465 6c2e 6c6f 6164 5f61 6461 7074  model.load_adapt
+00000a80: 6572 2822 4164 6170 7465 7248 7562 2f72  er("AdapterHub/r
+00000a90: 6f62 6572 7461 2d62 6173 652d 7066 2d69  oberta-base-pf-i
+00000aa0: 6d64 6222 2c20 736f 7572 6365 3d22 6866  mdb", source="hf
+00000ab0: 222c 2073 6574 5f61 6374 6976 653d 5472  ", set_active=Tr
+00000ac0: 7565 290a 0a70 7269 6e74 286d 6f64 656c  ue)..print(model
+00000ad0: 282a 2a74 6f6b 656e 697a 6572 2822 5468  (**tokenizer("Th
+00000ae0: 6973 2077 6f72 6b73 2067 7265 6174 2122  is works great!"
+00000af0: 2c20 7265 7475 726e 5f74 656e 736f 7273  , return_tensors
+00000b00: 3d22 7074 2229 292e 6c6f 6769 7473 290a  ="pt")).logits).
+00000b10: 6060 600a 0a2a 2a5b 4c65 6172 6e20 4d6f  ```..**[Learn Mo
+00000b20: 7265 5d28 6874 7470 733a 2f2f 646f 6373  re](https://docs
+00000b30: 2e61 6461 7074 6572 6875 622e 6d6c 2f6c  .adapterhub.ml/l
+00000b40: 6f61 6469 6e67 2e68 746d 6c29 2a2a 0a0a  oading.html)**..
+00000b50: 2323 2323 2041 6461 7074 2065 7869 7374  #### Adapt exist
+00000b60: 696e 6720 6d6f 6465 6c20 7365 7475 7073  ing model setups
+00000b70: 3a0a 0a60 6060 7079 7468 6f6e 0a69 6d70  :..```python.imp
+00000b80: 6f72 7420 6164 6170 7465 7273 0a66 726f  ort adapters.fro
+00000b90: 6d20 7472 616e 7366 6f72 6d65 7273 2069  m transformers i
+00000ba0: 6d70 6f72 7420 4175 746f 4d6f 6465 6c46  mport AutoModelF
+00000bb0: 6f72 5365 7175 656e 6365 436c 6173 7369  orSequenceClassi
+00000bc0: 6669 6361 7469 6f6e 0a0a 6d6f 6465 6c20  fication..model 
+00000bd0: 3d20 4175 746f 4d6f 6465 6c46 6f72 5365  = AutoModelForSe
+00000be0: 7175 656e 6365 436c 6173 7369 6669 6361  quenceClassifica
+00000bf0: 7469 6f6e 2e66 726f 6d5f 7072 6574 7261  tion.from_pretra
+00000c00: 696e 6564 2822 7435 2d62 6173 6522 290a  ined("t5-base").
+00000c10: 0a61 6461 7074 6572 732e 696e 6974 286d  .adapters.init(m
+00000c20: 6f64 656c 290a 0a6d 6f64 656c 2e61 6464  odel)..model.add
+00000c30: 5f61 6461 7074 6572 2822 6d79 5f6c 6f72  _adapter("my_lor
+00000c40: 615f 6164 6170 7465 7222 2c20 636f 6e66  a_adapter", conf
+00000c50: 6967 3d22 6c6f 7261 2229 0a6d 6f64 656c  ig="lora").model
+00000c60: 2e74 7261 696e 5f61 6461 7074 6572 2822  .train_adapter("
+00000c70: 6d79 5f6c 6f72 615f 6164 6170 7465 7222  my_lora_adapter"
+00000c80: 290a 0a23 2059 6f75 7220 7265 6775 6c61  )..# Your regula
+00000c90: 7220 7472 6169 6e69 6e67 206c 6f6f 702e  r training loop.
+00000ca0: 2e2e 0a60 6060 0a0a 2a2a 5b4c 6561 726e  ...```..**[Learn
+00000cb0: 204d 6f72 655d 2868 7474 7073 3a2f 2f64   More](https://d
+00000cc0: 6f63 732e 6164 6170 7465 7268 7562 2e6d  ocs.adapterhub.m
+00000cd0: 6c2f 7175 6963 6b73 7461 7274 2e68 746d  l/quickstart.htm
+00000ce0: 6c29 2a2a 0a0a 2323 2323 2046 6c65 7869  l)**..#### Flexi
+00000cf0: 626c 7920 636f 6e66 6967 7572 6520 6164  bly configure ad
+00000d00: 6170 7465 7273 3a0a 0a60 6060 7079 7468  apters:..```pyth
+00000d10: 6f6e 0a66 726f 6d20 6164 6170 7465 7273  on.from adapters
+00000d20: 2069 6d70 6f72 7420 436f 6e66 6967 556e   import ConfigUn
+00000d30: 696f 6e2c 2050 7265 6669 7854 756e 696e  ion, PrefixTunin
+00000d40: 6743 6f6e 6669 672c 2050 6172 426e 436f  gConfig, ParBnCo
+00000d50: 6e66 6967 2c20 4175 746f 4164 6170 7465  nfig, AutoAdapte
+00000d60: 724d 6f64 656c 0a0a 6d6f 6465 6c20 3d20  rModel..model = 
+00000d70: 4175 746f 4164 6170 7465 724d 6f64 656c  AutoAdapterModel
+00000d80: 2e66 726f 6d5f 7072 6574 7261 696e 6564  .from_pretrained
+00000d90: 2822 6d69 6372 6f73 6f66 742f 6465 6265  ("microsoft/debe
+00000da0: 7274 612d 7633 2d62 6173 6522 290a 0a61  rta-v3-base")..a
+00000db0: 6461 7074 6572 5f63 6f6e 6669 6720 3d20  dapter_config = 
+00000dc0: 436f 6e66 6967 556e 696f 6e28 0a20 2020  ConfigUnion(.   
+00000dd0: 2050 7265 6669 7854 756e 696e 6743 6f6e   PrefixTuningCon
+00000de0: 6669 6728 7072 6566 6978 5f6c 656e 6774  fig(prefix_lengt
+00000df0: 683d 3230 292c 0a20 2020 2050 6172 426e  h=20),.    ParBn
+00000e00: 436f 6e66 6967 2872 6564 7563 7469 6f6e  Config(reduction
+00000e10: 5f66 6163 746f 723d 3429 2c0a 290a 6d6f  _factor=4),.).mo
+00000e20: 6465 6c2e 6164 645f 6164 6170 7465 7228  del.add_adapter(
+00000e30: 226d 795f 6164 6170 7465 7222 2c20 636f  "my_adapter", co
+00000e40: 6e66 6967 3d61 6461 7074 6572 5f63 6f6e  nfig=adapter_con
+00000e50: 6669 672c 2073 6574 5f61 6374 6976 653d  fig, set_active=
+00000e60: 5472 7565 290a 6060 600a 0a2a 2a5b 4c65  True).```..**[Le
+00000e70: 6172 6e20 4d6f 7265 5d28 6874 7470 733a  arn More](https:
+00000e80: 2f2f 646f 6373 2e61 6461 7074 6572 6875  //docs.adapterhu
+00000e90: 622e 6d6c 2f6f 7665 7276 6965 772e 6874  b.ml/overview.ht
+00000ea0: 6d6c 292a 2a0a 0a23 2323 2320 4561 7369  ml)**..#### Easi
+00000eb0: 6c79 2063 6f6d 706f 7365 2061 6461 7074  ly compose adapt
+00000ec0: 6572 7320 696e 2061 2073 696e 676c 6520  ers in a single 
+00000ed0: 6d6f 6465 6c3a 0a0a 6060 6070 7974 686f  model:..```pytho
+00000ee0: 6e0a 6672 6f6d 2061 6461 7074 6572 7320  n.from adapters 
+00000ef0: 696d 706f 7274 2041 6461 7074 6572 5365  import AdapterSe
+00000f00: 7475 702c 2041 7574 6f41 6461 7074 6572  tup, AutoAdapter
+00000f10: 4d6f 6465 6c0a 696d 706f 7274 2061 6461  Model.import ada
+00000f20: 7074 6572 732e 636f 6d70 6f73 6974 696f  pters.compositio
+00000f30: 6e20 6173 2061 630a 0a6d 6f64 656c 203d  n as ac..model =
+00000f40: 2041 7574 6f41 6461 7074 6572 4d6f 6465   AutoAdapterMode
+00000f50: 6c2e 6672 6f6d 5f70 7265 7472 6169 6e65  l.from_pretraine
+00000f60: 6428 2272 6f62 6572 7461 2d62 6173 6522  d("roberta-base"
+00000f70: 290a 0a71 6320 3d20 6d6f 6465 6c2e 6c6f  )..qc = model.lo
+00000f80: 6164 5f61 6461 7074 6572 2822 4164 6170  ad_adapter("Adap
+00000f90: 7465 7248 7562 2f72 6f62 6572 7461 2d62  terHub/roberta-b
+00000fa0: 6173 652d 7066 2d74 7265 6322 290a 7365  ase-pf-trec").se
+00000fb0: 6e74 203d 206d 6f64 656c 2e6c 6f61 645f  nt = model.load_
+00000fc0: 6164 6170 7465 7228 2241 6461 7074 6572  adapter("Adapter
+00000fd0: 4875 622f 726f 6265 7274 612d 6261 7365  Hub/roberta-base
+00000fe0: 2d70 662d 696d 6462 2229 0a0a 7769 7468  -pf-imdb")..with
+00000ff0: 2041 6461 7074 6572 5365 7475 7028 6163   AdapterSetup(ac
+00001000: 2e50 6172 616c 6c65 6c28 7163 2c20 7365  .Parallel(qc, se
+00001010: 6e74 2929 3a0a 2020 2020 7072 696e 7428  nt)):.    print(
+00001020: 6d6f 6465 6c28 2a2a 746f 6b65 6e69 7a65  model(**tokenize
+00001030: 7228 2257 6861 7420 6973 2041 6461 7074  r("What is Adapt
+00001040: 6572 4875 623f 222c 2072 6574 7572 6e5f  erHub?", return_
+00001050: 7465 6e73 6f72 733d 2270 7422 2929 290a  tensors="pt"))).
+00001060: 6060 600a 0a2a 2a5b 4c65 6172 6e20 4d6f  ```..**[Learn Mo
+00001070: 7265 5d28 6874 7470 733a 2f2f 646f 6373  re](https://docs
+00001080: 2e61 6461 7074 6572 6875 622e 6d6c 2f61  .adapterhub.ml/a
+00001090: 6461 7074 6572 5f63 6f6d 706f 7369 7469  dapter_compositi
+000010a0: 6f6e 2e68 746d 6c29 2a2a 0a0a 2323 2055  on.html)**..## U
+000010b0: 7365 6675 6c20 5265 736f 7572 6365 730a  seful Resources.
+000010c0: 0a48 7567 6769 6e67 4661 6365 2773 2067  .HuggingFace's g
+000010d0: 7265 6174 2064 6f63 756d 656e 7461 7469  reat documentati
+000010e0: 6f6e 206f 6e20 6765 7474 696e 6720 7374  on on getting st
+000010f0: 6172 7465 6420 7769 7468 205f 5472 616e  arted with _Tran
+00001100: 7366 6f72 6d65 7273 5f20 6361 6e20 6265  sformers_ can be
+00001110: 2066 6f75 6e64 205b 6865 7265 5d28 6874   found [here](ht
+00001120: 7470 733a 2f2f 6875 6767 696e 6766 6163  tps://huggingfac
+00001130: 652e 636f 2f74 7261 6e73 666f 726d 6572  e.co/transformer
+00001140: 732f 696e 6465 782e 6874 6d6c 292e 2060  s/index.html). `
+00001150: 6164 6170 7465 7273 6020 6973 2066 756c  adapters` is ful
+00001160: 6c79 2063 6f6d 7061 7469 626c 6520 7769  ly compatible wi
+00001170: 7468 205f 5472 616e 7366 6f72 6d65 7273  th _Transformers
+00001180: 5f2e 0a0a 546f 2067 6574 2073 7461 7274  _...To get start
+00001190: 6564 2077 6974 6820 6164 6170 7465 7273  ed with adapters
+000011a0: 2c20 7265 6665 7220 746f 2074 6865 7365  , refer to these
+000011b0: 206c 6f63 6174 696f 6e73 3a0a 0a2d 202a   locations:..- *
+000011c0: 2a5b 436f 6c61 6220 6e6f 7465 626f 6f6b  *[Colab notebook
+000011d0: 2074 7574 6f72 6961 6c73 5d28 6874 7470   tutorials](http
+000011e0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f41  s://github.com/A
+000011f0: 6461 7074 6572 2d48 7562 2f61 6461 7074  dapter-Hub/adapt
+00001200: 6572 732f 7472 6565 2f6d 6169 6e2f 6e6f  ers/tree/main/no
+00001210: 7465 626f 6f6b 7329 2a2a 2c20 6120 7365  tebooks)**, a se
+00001220: 7269 6573 206e 6f74 6562 6f6f 6b73 2070  ries notebooks p
+00001230: 726f 7669 6469 6e67 2061 6e20 696e 7472  roviding an intr
+00001240: 6f64 7563 7469 6f6e 2074 6f20 616c 6c20  oduction to all 
+00001250: 7468 6520 6d61 696e 2063 6f6e 6365 7074  the main concept
+00001260: 7320 6f66 2028 6164 6170 7465 722d 2974  s of (adapter-)t
+00001270: 7261 6e73 666f 726d 6572 7320 616e 6420  ransformers and 
+00001280: 4164 6170 7465 7248 7562 0a2d 202a 2a68  AdapterHub.- **h
+00001290: 7474 7073 3a2f 2f64 6f63 732e 6164 6170  ttps://docs.adap
+000012a0: 7465 7268 7562 2e6d 6c2a 2a2c 206f 7572  terhub.ml**, our
+000012b0: 2064 6f63 756d 656e 7461 7469 6f6e 206f   documentation o
+000012c0: 6e20 7472 6169 6e69 6e67 2061 6e64 2075  n training and u
+000012d0: 7369 6e67 2061 6461 7074 6572 7320 7769  sing adapters wi
+000012e0: 7468 205f 6164 6170 7465 7273 5f0a 2d20  th _adapters_.- 
+000012f0: 2a2a 6874 7470 733a 2f2f 6164 6170 7465  **https://adapte
+00001300: 7268 7562 2e6d 6c2a 2a20 746f 2065 7870  rhub.ml** to exp
+00001310: 6c6f 7265 2061 7661 696c 6162 6c65 2070  lore available p
+00001320: 7265 2d74 7261 696e 6564 2061 6461 7074  re-trained adapt
+00001330: 6572 206d 6f64 756c 6573 2061 6e64 2073  er modules and s
+00001340: 6861 7265 2079 6f75 7220 6f77 6e20 6164  hare your own ad
+00001350: 6170 7465 7273 0a2d 202a 2a5b 4578 616d  apters.- **[Exam
+00001360: 706c 6573 2066 6f6c 6465 725d 2868 7474  ples folder](htt
+00001370: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00001380: 4164 6170 7465 722d 4875 622f 6164 6170  Adapter-Hub/adap
+00001390: 7465 7273 2f74 7265 652f 6d61 696e 2f65  ters/tree/main/e
+000013a0: 7861 6d70 6c65 732f 7079 746f 7263 6829  xamples/pytorch)
+000013b0: 2a2a 206f 6620 7468 6973 2072 6570 6f73  ** of this repos
+000013c0: 6974 6f72 7920 636f 6e74 6169 6e69 6e67  itory containing
+000013d0: 2048 7567 6769 6e67 4661 6365 2773 2065   HuggingFace's e
+000013e0: 7861 6d70 6c65 2074 7261 696e 696e 6720  xample training 
+000013f0: 7363 7269 7074 732c 206d 616e 7920 6164  scripts, many ad
+00001400: 6170 7465 6420 666f 7220 7472 6169 6e69  apted for traini
+00001410: 6e67 2061 6461 7074 6572 730a 0a23 2320  ng adapters..## 
+00001420: 496d 706c 656d 656e 7465 6420 4d65 7468  Implemented Meth
+00001430: 6f64 730a 0a43 7572 7265 6e74 6c79 2c20  ods..Currently, 
+00001440: 6164 6170 7465 7273 2069 6e74 6567 7261  adapters integra
+00001450: 7465 7320 616c 6c20 6172 6368 6974 6563  tes all architec
+00001460: 7475 7265 7320 616e 6420 6d65 7468 6f64  tures and method
+00001470: 7320 6c69 7374 6564 2062 656c 6f77 3a0a  s listed below:.
+00001480: 0a7c 204d 6574 686f 6420 7c20 5061 7065  .| Method | Pape
+00001490: 7228 7329 207c 2051 7569 636b 204c 696e  r(s) | Quick Lin
+000014a0: 6b73 207c 0a7c 202d 2d2d 207c 202d 2d2d  ks |.| --- | ---
+000014b0: 207c 202d 2d2d 207c 0a7c 2042 6f74 746c   | --- |.| Bottl
+000014c0: 656e 6563 6b20 6164 6170 7465 7273 207c  eneck adapters |
+000014d0: 205b 486f 756c 7362 7920 6574 2061 6c2e   [Houlsby et al.
+000014e0: 2028 3230 3139 295d 2868 7474 7073 3a2f   (2019)](https:/
+000014f0: 2f61 7278 6976 2e6f 7267 2f70 6466 2f31  /arxiv.org/pdf/1
+00001500: 3930 322e 3030 3735 312e 7064 6629 3c62  902.00751.pdf)<b
+00001510: 723e 205b 4261 706e 6120 616e 6420 4669  r> [Bapna and Fi
+00001520: 7261 7420 2832 3031 3929 5d28 6874 7470  rat (2019)](http
+00001530: 733a 2f2f 6172 7869 762e 6f72 672f 7064  s://arxiv.org/pd
+00001540: 662f 3139 3039 2e30 3834 3738 2e70 6466  f/1909.08478.pdf
+00001550: 2920 7c20 5b51 7569 636b 7374 6172 745d  ) | [Quickstart]
+00001560: 2868 7474 7073 3a2f 2f64 6f63 732e 6164  (https://docs.ad
+00001570: 6170 7465 7268 7562 2e6d 6c2f 7175 6963  apterhub.ml/quic
+00001580: 6b73 7461 7274 2e68 746d 6c29 2c20 5b4e  kstart.html), [N
+00001590: 6f74 6562 6f6f 6b5d 2868 7474 7073 3a2f  otebook](https:/
+000015a0: 2f63 6f6c 6162 2e72 6573 6561 7263 682e  /colab.research.
+000015b0: 676f 6f67 6c65 2e63 6f6d 2f67 6974 6875  google.com/githu
+000015c0: 622f 4164 6170 7465 722d 4875 622f 6164  b/Adapter-Hub/ad
+000015d0: 6170 7465 7273 2f62 6c6f 622f 6d61 696e  apters/blob/main
+000015e0: 2f6e 6f74 6562 6f6f 6b73 2f30 315f 4164  /notebooks/01_Ad
+000015f0: 6170 7465 725f 5472 6169 6e69 6e67 2e69  apter_Training.i
+00001600: 7079 6e62 2920 7c0a 7c20 4164 6170 7465  pynb) |.| Adapte
+00001610: 7246 7573 696f 6e20 7c20 5b50 6665 6966  rFusion | [Pfeif
+00001620: 6665 7220 6574 2061 6c2e 2028 3230 3231  fer et al. (2021
+00001630: 295d 2868 7474 7073 3a2f 2f61 636c 616e  )](https://aclan
+00001640: 7468 6f6c 6f67 792e 6f72 672f 3230 3231  thology.org/2021
+00001650: 2e65 6163 6c2d 6d61 696e 2e33 392e 7064  .eacl-main.39.pd
+00001660: 6629 207c 205b 446f 6373 3a20 5472 6169  f) | [Docs: Trai
+00001670: 6e69 6e67 5d28 6874 7470 733a 2f2f 646f  ning](https://do
+00001680: 6373 2e61 6461 7074 6572 6875 622e 6d6c  cs.adapterhub.ml
+00001690: 2f74 7261 696e 696e 672e 6874 6d6c 2374  /training.html#t
+000016a0: 7261 696e 2d61 6461 7074 6572 6675 7369  rain-adapterfusi
+000016b0: 6f6e 292c 205b 4e6f 7465 626f 6f6b 5d28  on), [Notebook](
+000016c0: 6874 7470 733a 2f2f 636f 6c61 622e 7265  https://colab.re
+000016d0: 7365 6172 6368 2e67 6f6f 676c 652e 636f  search.google.co
+000016e0: 6d2f 6769 7468 7562 2f41 6461 7074 6572  m/github/Adapter
+000016f0: 2d48 7562 2f61 6461 7074 6572 732f 626c  -Hub/adapters/bl
+00001700: 6f62 2f6d 6169 6e2f 6e6f 7465 626f 6f6b  ob/main/notebook
+00001710: 732f 3033 5f41 6461 7074 6572 5f46 7573  s/03_Adapter_Fus
+00001720: 696f 6e2e 6970 796e 6229 207c 0a7c 204d  ion.ipynb) |.| M
+00001730: 4144 2d58 2c3c 6272 3e20 496e 7665 7274  AD-X,<br> Invert
+00001740: 6962 6c65 2061 6461 7074 6572 7320 7c20  ible adapters | 
+00001750: 5b50 6665 6966 6665 7220 6574 2061 6c2e  [Pfeiffer et al.
+00001760: 2028 3230 3230 295d 2868 7474 7073 3a2f   (2020)](https:/
+00001770: 2f61 636c 616e 7468 6f6c 6f67 792e 6f72  /aclanthology.or
+00001780: 672f 3230 3230 2e65 6d6e 6c70 2d6d 6169  g/2020.emnlp-mai
+00001790: 6e2e 3631 372f 2920 7c20 5b4e 6f74 6562  n.617/) | [Noteb
+000017a0: 6f6f 6b5d 2868 7474 7073 3a2f 2f63 6f6c  ook](https://col
+000017b0: 6162 2e72 6573 6561 7263 682e 676f 6f67  ab.research.goog
+000017c0: 6c65 2e63 6f6d 2f67 6974 6875 622f 4164  le.com/github/Ad
+000017d0: 6170 7465 722d 4875 622f 6164 6170 7465  apter-Hub/adapte
+000017e0: 7273 2f62 6c6f 622f 6d61 696e 2f6e 6f74  rs/blob/main/not
+000017f0: 6562 6f6f 6b73 2f30 345f 4372 6f73 735f  ebooks/04_Cross_
+00001800: 4c69 6e67 7561 6c5f 5472 616e 7366 6572  Lingual_Transfer
+00001810: 2e69 7079 6e62 2920 7c0a 7c20 4164 6170  .ipynb) |.| Adap
+00001820: 7465 7244 726f 7020 7c20 5b52 c3bc 636b  terDrop | [R..ck
+00001830: 6cc3 a920 6574 2061 6c2e 2028 3230 3231  l.. et al. (2021
+00001840: 295d 2868 7474 7073 3a2f 2f61 7278 6976  )](https://arxiv
+00001850: 2e6f 7267 2f70 6466 2f32 3031 302e 3131  .org/pdf/2010.11
+00001860: 3931 382e 7064 6629 207c 205b 4e6f 7465  918.pdf) | [Note
+00001870: 626f 6f6b 5d28 6874 7470 733a 2f2f 636f  book](https://co
+00001880: 6c61 622e 7265 7365 6172 6368 2e67 6f6f  lab.research.goo
+00001890: 676c 652e 636f 6d2f 6769 7468 7562 2f41  gle.com/github/A
+000018a0: 6461 7074 6572 2d48 7562 2f61 6461 7074  dapter-Hub/adapt
+000018b0: 6572 732f 626c 6f62 2f6d 6169 6e2f 6e6f  ers/blob/main/no
+000018c0: 7465 626f 6f6b 732f 3035 5f41 6461 7074  tebooks/05_Adapt
+000018d0: 6572 5f44 726f 705f 5472 6169 6e69 6e67  er_Drop_Training
+000018e0: 2e69 7079 6e62 2920 7c0a 7c20 4d41 442d  .ipynb) |.| MAD-
+000018f0: 5820 322e 302c 3c62 723e 2045 6d62 6564  X 2.0,<br> Embed
+00001900: 6469 6e67 2074 7261 696e 696e 6720 7c20  ding training | 
+00001910: 5b50 6665 6966 6665 7220 6574 2061 6c2e  [Pfeiffer et al.
+00001920: 2028 3230 3231 295d 2868 7474 7073 3a2f   (2021)](https:/
+00001930: 2f61 7278 6976 2e6f 7267 2f70 6466 2f32  /arxiv.org/pdf/2
+00001940: 3031 322e 3135 3536 322e 7064 6629 207c  012.15562.pdf) |
+00001950: 205b 446f 6373 3a20 456d 6265 6464 696e   [Docs: Embeddin
+00001960: 6773 5d28 6874 7470 733a 2f2f 646f 6373  gs](https://docs
+00001970: 2e61 6461 7074 6572 6875 622e 6d6c 2f65  .adapterhub.ml/e
+00001980: 6d62 6564 6469 6e67 732e 6874 6d6c 292c  mbeddings.html),
+00001990: 205b 4e6f 7465 626f 6f6b 5d28 6874 7470   [Notebook](http
+000019a0: 733a 2f2f 636f 6c61 622e 7265 7365 6172  s://colab.resear
+000019b0: 6368 2e67 6f6f 676c 652e 636f 6d2f 6769  ch.google.com/gi
+000019c0: 7468 7562 2f41 6461 7074 6572 2d48 7562  thub/Adapter-Hub
+000019d0: 2f61 6461 7074 6572 732f 626c 6f62 2f6d  /adapters/blob/m
+000019e0: 6169 6e2f 6e6f 7465 626f 6f6b 732f 3038  ain/notebooks/08
+000019f0: 5f4e 4552 5f57 696b 6961 6e6e 2e69 7079  _NER_Wikiann.ipy
+00001a00: 6e62 2920 7c0a 7c20 5072 6566 6978 2054  nb) |.| Prefix T
+00001a10: 756e 696e 6720 7c20 5b4c 6920 616e 6420  uning | [Li and 
+00001a20: 4c69 616e 6720 2832 3032 3129 5d28 6874  Liang (2021)](ht
+00001a30: 7470 733a 2f2f 6172 7869 762e 6f72 672f  tps://arxiv.org/
+00001a40: 7064 662f 3231 3031 2e30 3031 3930 2e70  pdf/2101.00190.p
+00001a50: 6466 2920 7c20 5b44 6f63 735d 2868 7474  df) | [Docs](htt
+00001a60: 7073 3a2f 2f64 6f63 732e 6164 6170 7465  ps://docs.adapte
+00001a70: 7268 7562 2e6d 6c2f 6d65 7468 6f64 732e  rhub.ml/methods.
+00001a80: 6874 6d6c 2370 7265 6669 782d 7475 6e69  html#prefix-tuni
+00001a90: 6e67 2920 7c0a 7c20 5061 7261 6c6c 656c  ng) |.| Parallel
+00001aa0: 2061 6461 7074 6572 732c 3c62 723e 204d   adapters,<br> M
+00001ab0: 6978 2d61 6e64 2d4d 6174 6368 2061 6461  ix-and-Match ada
+00001ac0: 7074 6572 7320 7c20 5b48 6520 6574 2061  pters | [He et a
+00001ad0: 6c2e 2028 3230 3231 295d 2868 7474 7073  l. (2021)](https
+00001ae0: 3a2f 2f61 7278 6976 2e6f 7267 2f70 6466  ://arxiv.org/pdf
+00001af0: 2f32 3131 302e 3034 3336 362e 7064 6629  /2110.04366.pdf)
+00001b00: 207c 205b 446f 6373 5d28 6874 7470 733a   | [Docs](https:
+00001b10: 2f2f 646f 6373 2e61 6461 7074 6572 6875  //docs.adapterhu
+00001b20: 622e 6d6c 2f6d 6574 686f 645f 636f 6d62  b.ml/method_comb
+00001b30: 696e 6174 696f 6e73 2e68 746d 6c23 6d69  inations.html#mi
+00001b40: 782d 616e 642d 6d61 7463 682d 6164 6170  x-and-match-adap
+00001b50: 7465 7273 2920 7c0a 7c20 436f 6d70 6163  ters) |.| Compac
+00001b60: 7465 7220 7c20 5b4d 6168 6162 6164 6920  ter | [Mahabadi 
+00001b70: 6574 2061 6c2e 2028 3230 3231 295d 2868  et al. (2021)](h
+00001b80: 7474 7073 3a2f 2f61 7278 6976 2e6f 7267  ttps://arxiv.org
+00001b90: 2f70 6466 2f32 3130 362e 3034 3634 372e  /pdf/2106.04647.
+00001ba0: 7064 6629 207c 205b 446f 6373 5d28 6874  pdf) | [Docs](ht
+00001bb0: 7470 733a 2f2f 646f 6373 2e61 6461 7074  tps://docs.adapt
+00001bc0: 6572 6875 622e 6d6c 2f6d 6574 686f 6473  erhub.ml/methods
+00001bd0: 2e68 746d 6c23 636f 6d70 6163 7465 7229  .html#compacter)
+00001be0: 207c 0a7c 204c 6f52 4120 7c20 5b48 7520   |.| LoRA | [Hu 
+00001bf0: 6574 2061 6c2e 2028 3230 3231 295d 2868  et al. (2021)](h
+00001c00: 7474 7073 3a2f 2f61 7278 6976 2e6f 7267  ttps://arxiv.org
+00001c10: 2f70 6466 2f32 3130 362e 3039 3638 352e  /pdf/2106.09685.
+00001c20: 7064 6629 207c 205b 446f 6373 5d28 6874  pdf) | [Docs](ht
+00001c30: 7470 733a 2f2f 646f 6373 2e61 6461 7074  tps://docs.adapt
+00001c40: 6572 6875 622e 6d6c 2f6d 6574 686f 6473  erhub.ml/methods
+00001c50: 2e68 746d 6c23 6c6f 7261 2920 7c0a 7c20  .html#lora) |.| 
+00001c60: 2849 4129 5e33 207c 205b 4c69 7520 6574  (IA)^3 | [Liu et
+00001c70: 2061 6c2e 2028 3230 3232 295d 2868 7474   al. (2022)](htt
+00001c80: 7073 3a2f 2f61 7278 6976 2e6f 7267 2f70  ps://arxiv.org/p
+00001c90: 6466 2f32 3230 352e 3035 3633 382e 7064  df/2205.05638.pd
+00001ca0: 6629 207c 205b 446f 6373 5d28 6874 7470  f) | [Docs](http
+00001cb0: 733a 2f2f 646f 6373 2e61 6461 7074 6572  s://docs.adapter
+00001cc0: 6875 622e 6d6c 2f6d 6574 686f 6473 2e68  hub.ml/methods.h
+00001cd0: 746d 6c23 6961 2d33 2920 7c0a 7c20 556e  tml#ia-3) |.| Un
+00001ce0: 6950 454c 5420 7c20 5b4d 616f 2065 7420  iPELT | [Mao et 
+00001cf0: 616c 2e20 2832 3032 3229 5d28 6874 7470  al. (2022)](http
+00001d00: 733a 2f2f 6172 7869 762e 6f72 672f 7064  s://arxiv.org/pd
+00001d10: 662f 3231 3130 2e30 3735 3737 2e70 6466  f/2110.07577.pdf
+00001d20: 2920 7c20 5b44 6f63 735d 2868 7474 7073  ) | [Docs](https
+00001d30: 3a2f 2f64 6f63 732e 6164 6170 7465 7268  ://docs.adapterh
+00001d40: 7562 2e6d 6c2f 6d65 7468 6f64 5f63 6f6d  ub.ml/method_com
+00001d50: 6269 6e61 7469 6f6e 732e 6874 6d6c 2375  binations.html#u
+00001d60: 6e69 7065 6c74 2920 7c0a 7c20 5072 6f6d  nipelt) |.| Prom
+00001d70: 7074 2054 756e 696e 6720 7c20 5b4c 6573  pt Tuning | [Les
+00001d80: 7465 7220 6574 2061 6c2e 2028 3230 3231  ter et al. (2021
+00001d90: 295d 2868 7474 7073 3a2f 2f61 636c 616e  )](https://aclan
+00001da0: 7468 6f6c 6f67 792e 6f72 672f 3230 3231  thology.org/2021
+00001db0: 2e65 6d6e 6c70 2d6d 6169 6e2e 3234 332f  .emnlp-main.243/
+00001dc0: 2920 7c20 5b44 6f63 735d 2868 7474 7073  ) | [Docs](https
+00001dd0: 3a2f 2f64 6f63 732e 6164 6170 7465 7268  ://docs.adapterh
+00001de0: 7562 2e6d 6c2f 6d65 7468 6f64 732e 6874  ub.ml/methods.ht
+00001df0: 6d6c 2370 726f 6d70 742d 7475 6e69 6e67  ml#prompt-tuning
+00001e00: 2920 7c0a 7c20 514c 6f52 4120 7c20 5b44  ) |.| QLoRA | [D
+00001e10: 6574 746d 6572 7320 6574 2061 6c2e 2028  ettmers et al. (
+00001e20: 3230 3233 295d 2868 7474 7073 3a2f 2f61  2023)](https://a
+00001e30: 7278 6976 2e6f 7267 2f70 6466 2f32 3330  rxiv.org/pdf/230
+00001e40: 352e 3134 3331 342e 7064 6629 207c 205b  5.14314.pdf) | [
+00001e50: 4e6f 7465 626f 6f6b 5d28 6874 7470 733a  Notebook](https:
+00001e60: 2f2f 636f 6c61 622e 7265 7365 6172 6368  //colab.research
+00001e70: 2e67 6f6f 676c 652e 636f 6d2f 6769 7468  .google.com/gith
+00001e80: 7562 2f41 6461 7074 6572 2d48 7562 2f61  ub/Adapter-Hub/a
+00001e90: 6461 7074 6572 732f 626c 6f62 2f6d 6169  dapters/blob/mai
+00001ea0: 6e2f 6e6f 7465 626f 6f6b 732f 514c 6f52  n/notebooks/QLoR
+00001eb0: 415f 4c6c 616d 615f 4669 6e65 7475 6e69  A_Llama_Finetuni
+00001ec0: 6e67 2e69 7079 6e62 2920 7c0a 0a23 2320  ng.ipynb) |..## 
+00001ed0: 5375 7070 6f72 7465 6420 4d6f 6465 6c73  Supported Models
+00001ee0: 0a0a 5765 2063 7572 7265 6e74 6c79 2073  ..We currently s
+00001ef0: 7570 706f 7274 2074 6865 2050 7954 6f72  upport the PyTor
+00001f00: 6368 2076 6572 7369 6f6e 7320 6f66 2061  ch versions of a
+00001f10: 6c6c 206d 6f64 656c 7320 6c69 7374 6564  ll models listed
+00001f20: 206f 6e20 7468 6520 2a2a 5b4d 6f64 656c   on the **[Model
+00001f30: 204f 7665 7276 6965 775d 2868 7474 7073   Overview](https
+00001f40: 3a2f 2f64 6f63 732e 6164 6170 7465 7268  ://docs.adapterh
+00001f50: 7562 2e6d 6c2f 6d6f 6465 6c5f 6f76 6572  ub.ml/model_over
+00001f60: 7669 6577 2e68 746d 6c29 2070 6167 652a  view.html) page*
+00001f70: 2a20 696e 206f 7572 2064 6f63 756d 656e  * in our documen
+00001f80: 7461 7469 6f6e 2e0a 0a23 2320 4465 7665  tation...## Deve
+00001f90: 6c6f 7069 6e67 2026 2043 6f6e 7472 6962  loping & Contrib
+00001fa0: 7574 696e 670a 0a54 6f20 6765 7420 7374  uting..To get st
+00001fb0: 6172 7465 6420 7769 7468 2064 6576 656c  arted with devel
+00001fc0: 6f70 696e 6720 6f6e 205f 4164 6170 7465  oping on _Adapte
+00001fd0: 7273 5f20 796f 7572 7365 6c66 2061 6e64  rs_ yourself and
+00001fe0: 206c 6561 726e 206d 6f72 6520 6162 6f75   learn more abou
+00001ff0: 7420 7761 7973 2074 6f20 636f 6e74 7269  t ways to contri
+00002000: 6275 7465 2c20 706c 6561 7365 2073 6565  bute, please see
+00002010: 2068 7474 7073 3a2f 2f64 6f63 732e 6164   https://docs.ad
+00002020: 6170 7465 7268 7562 2e6d 6c2f 636f 6e74  apterhub.ml/cont
+00002030: 7269 6275 7469 6e67 2e68 746d 6c2e 0a0a  ributing.html...
+00002040: 2323 2043 6974 6174 696f 6e0a 0a49 6620  ## Citation..If 
+00002050: 796f 7520 7573 6520 5f41 6461 7074 6572  you use _Adapter
+00002060: 735f 2069 6e20 796f 7572 2077 6f72 6b2c  s_ in your work,
+00002070: 2070 6c65 6173 6520 636f 6e73 6964 6572   please consider
+00002080: 2063 6974 696e 6720 6f75 7220 6c69 6272   citing our libr
+00002090: 6172 7920 7061 7065 723a 205b 4164 6170  ary paper: [Adap
+000020a0: 7465 7273 3a20 4120 556e 6966 6965 6420  ters: A Unified 
+000020b0: 4c69 6272 6172 7920 666f 7220 5061 7261  Library for Para
+000020c0: 6d65 7465 722d 4566 6669 6369 656e 7420  meter-Efficient 
+000020d0: 616e 6420 4d6f 6475 6c61 7220 5472 616e  and Modular Tran
+000020e0: 7366 6572 204c 6561 726e 696e 675d 2868  sfer Learning](h
+000020f0: 7474 7073 3a2f 2f61 7278 6976 2e6f 7267  ttps://arxiv.org
+00002100: 2f61 6273 2f32 3331 312e 3131 3037 3729  /abs/2311.11077)
+00002110: 0a0a 6060 600a 4069 6e70 726f 6365 6564  ..```.@inproceed
+00002120: 696e 6773 7b70 6f74 682d 6574 616c 2d32  ings{poth-etal-2
+00002130: 3032 332d 6164 6170 7465 7273 2c0a 2020  023-adapters,.  
+00002140: 2020 7469 746c 6520 3d20 2241 6461 7074    title = "Adapt
+00002150: 6572 733a 2041 2055 6e69 6669 6564 204c  ers: A Unified L
+00002160: 6962 7261 7279 2066 6f72 2050 6172 616d  ibrary for Param
+00002170: 6574 6572 2d45 6666 6963 6965 6e74 2061  eter-Efficient a
+00002180: 6e64 204d 6f64 756c 6172 2054 7261 6e73  nd Modular Trans
+00002190: 6665 7220 4c65 6172 6e69 6e67 222c 0a20  fer Learning",. 
+000021a0: 2020 2061 7574 686f 7220 3d20 7b50 6f74     author = {Pot
+000021b0: 682c 2043 6c69 6674 6f6e 2020 616e 640a  h, Clifton  and.
+000021c0: 2020 2020 2020 5374 6572 7a2c 2048 616e        Sterz, Han
+000021d0: 6e61 6820 2061 6e64 0a20 2020 2020 2050  nah  and.      P
+000021e0: 6175 6c2c 2049 6e64 7261 6e65 696c 2020  aul, Indraneil  
+000021f0: 616e 640a 2020 2020 2020 5075 726b 6179  and.      Purkay
+00002200: 6173 7468 612c 2053 756b 616e 6e79 6120  astha, Sukannya 
+00002210: 2061 6e64 0a20 2020 2020 2045 6e67 6c7b   and.      Engl{
+00002220: 5c22 617d 6e64 6572 2c20 4c65 6f6e 2020  \"a}nder, Leon  
+00002230: 616e 640a 2020 2020 2020 496d 686f 662c  and.      Imhof,
+00002240: 2054 696d 6f20 2061 6e64 0a20 2020 2020   Timo  and.     
+00002250: 2056 756c 697b 5c27 637d 2c20 4976 616e   Vuli{\'c}, Ivan
+00002260: 2020 616e 640a 2020 2020 2020 5275 6465    and.      Rude
+00002270: 722c 2053 6562 6173 7469 616e 2020 616e  r, Sebastian  an
+00002280: 640a 2020 2020 2020 4775 7265 7679 6368  d.      Gurevych
+00002290: 2c20 4972 796e 6120 2061 6e64 0a20 2020  , Iryna  and.   
+000022a0: 2020 2050 6665 6966 6665 722c 204a 6f6e     Pfeiffer, Jon
+000022b0: 6173 7d2c 0a20 2020 2062 6f6f 6b74 6974  as},.    booktit
+000022c0: 6c65 203d 2022 5072 6f63 6565 6469 6e67  le = "Proceeding
+000022d0: 7320 6f66 2074 6865 2032 3032 3320 436f  s of the 2023 Co
+000022e0: 6e66 6572 656e 6365 206f 6e20 456d 7069  nference on Empi
+000022f0: 7269 6361 6c20 4d65 7468 6f64 7320 696e  rical Methods in
+00002300: 204e 6174 7572 616c 204c 616e 6775 6167   Natural Languag
+00002310: 6520 5072 6f63 6573 7369 6e67 3a20 5379  e Processing: Sy
+00002320: 7374 656d 2044 656d 6f6e 7374 7261 7469  stem Demonstrati
+00002330: 6f6e 7322 2c0a 2020 2020 6d6f 6e74 6820  ons",.    month 
+00002340: 3d20 6465 632c 0a20 2020 2079 6561 7220  = dec,.    year 
+00002350: 3d20 2232 3032 3322 2c0a 2020 2020 6164  = "2023",.    ad
+00002360: 6472 6573 7320 3d20 2253 696e 6761 706f  dress = "Singapo
+00002370: 7265 222c 0a20 2020 2070 7562 6c69 7368  re",.    publish
+00002380: 6572 203d 2022 4173 736f 6369 6174 696f  er = "Associatio
+00002390: 6e20 666f 7220 436f 6d70 7574 6174 696f  n for Computatio
+000023a0: 6e61 6c20 4c69 6e67 7569 7374 6963 7322  nal Linguistics"
+000023b0: 2c0a 2020 2020 7572 6c20 3d20 2268 7474  ,.    url = "htt
+000023c0: 7073 3a2f 2f61 636c 616e 7468 6f6c 6f67  ps://aclantholog
+000023d0: 792e 6f72 672f 3230 3233 2e65 6d6e 6c70  y.org/2023.emnlp
+000023e0: 2d64 656d 6f2e 3133 222c 0a20 2020 2070  -demo.13",.    p
+000023f0: 6167 6573 203d 2022 3134 392d 2d31 3630  ages = "149--160
+00002400: 222c 0a7d 0a60 6060 0a0a 416c 7465 726e  ",.}.```..Altern
+00002410: 6174 6976 656c 792c 2066 6f72 2074 6865  atively, for the
+00002420: 2070 7265 6465 6365 7373 6f72 2060 6164   predecessor `ad
+00002430: 6170 7465 722d 7472 616e 7366 6f72 6d65  apter-transforme
+00002440: 7273 602c 2074 6865 2048 7562 2069 6e66  rs`, the Hub inf
+00002450: 7261 7374 7275 6374 7572 6520 616e 6420  rastructure and 
+00002460: 6164 6170 7465 7273 2075 706c 6f61 6465  adapters uploade
+00002470: 6420 6279 2074 6865 2041 6461 7074 6572  d by the Adapter
+00002480: 4875 6220 7465 616d 2c20 706c 6561 7365  Hub team, please
+00002490: 2063 6f6e 7369 6465 7220 6369 7469 6e67   consider citing
+000024a0: 206f 7572 2069 6e69 7469 616c 2070 6170   our initial pap
+000024b0: 6572 3a20 5b41 6461 7074 6572 4875 623a  er: [AdapterHub:
+000024c0: 2041 2046 7261 6d65 776f 726b 2066 6f72   A Framework for
+000024d0: 2041 6461 7074 696e 6720 5472 616e 7366   Adapting Transf
+000024e0: 6f72 6d65 7273 5d28 6874 7470 733a 2f2f  ormers](https://
+000024f0: 6172 7869 762e 6f72 672f 6162 732f 3230  arxiv.org/abs/20
+00002500: 3037 2e30 3737 3739 290a 0a60 6060 0a40  07.07779)..```.@
+00002510: 696e 7072 6f63 6565 6469 6e67 737b 7066  inproceedings{pf
+00002520: 6569 6666 6572 3230 3230 4164 6170 7465  eiffer2020Adapte
+00002530: 7248 7562 2c0a 2020 2020 7469 746c 653d  rHub,.    title=
+00002540: 7b41 6461 7074 6572 4875 623a 2041 2046  {AdapterHub: A F
+00002550: 7261 6d65 776f 726b 2066 6f72 2041 6461  ramework for Ada
+00002560: 7074 696e 6720 5472 616e 7366 6f72 6d65  pting Transforme
+00002570: 7273 7d2c 0a20 2020 2061 7574 686f 723d  rs},.    author=
+00002580: 7b50 6665 6966 6665 722c 204a 6f6e 6173  {Pfeiffer, Jonas
+00002590: 2061 6e64 0a20 2020 2020 2020 2020 2020   and.           
+000025a0: 2052 7b5c 2275 7d63 6b6c 7b5c 2765 7d2c   R{\"u}ckl{\'e},
+000025b0: 2041 6e64 7265 6173 2061 6e64 0a20 2020   Andreas and.   
+000025c0: 2020 2020 2020 2020 2050 6f74 682c 2043           Poth, C
+000025d0: 6c69 6674 6f6e 2061 6e64 0a20 2020 2020  lifton and.     
+000025e0: 2020 2020 2020 204b 616d 6174 682c 2041         Kamath, A
+000025f0: 6973 6877 6172 7961 2061 6e64 0a20 2020  ishwarya and.   
+00002600: 2020 2020 2020 2020 2056 756c 697b 5c27           Vuli{\'
+00002610: 637d 2c20 4976 616e 2061 6e64 0a20 2020  c}, Ivan and.   
+00002620: 2020 2020 2020 2020 2052 7564 6572 2c20           Ruder, 
+00002630: 5365 6261 7374 6961 6e20 616e 640a 2020  Sebastian and.  
+00002640: 2020 2020 2020 2020 2020 4368 6f2c 204b            Cho, K
+00002650: 7975 6e67 6879 756e 2061 6e64 0a20 2020  yunghyun and.   
+00002660: 2020 2020 2020 2020 2047 7572 6576 7963           Gurevyc
+00002670: 682c 2049 7279 6e61 7d2c 0a20 2020 2062  h, Iryna},.    b
+00002680: 6f6f 6b74 6974 6c65 3d7b 5072 6f63 6565  ooktitle={Procee
+00002690: 6469 6e67 7320 6f66 2074 6865 2032 3032  dings of the 202
+000026a0: 3020 436f 6e66 6572 656e 6365 206f 6e20  0 Conference on 
+000026b0: 456d 7069 7269 6361 6c20 4d65 7468 6f64  Empirical Method
+000026c0: 7320 696e 204e 6174 7572 616c 204c 616e  s in Natural Lan
+000026d0: 6775 6167 6520 5072 6f63 6573 7369 6e67  guage Processing
+000026e0: 3a20 5379 7374 656d 2044 656d 6f6e 7374  : System Demonst
+000026f0: 7261 7469 6f6e 737d 2c0a 2020 2020 7061  rations},.    pa
+00002700: 6765 733d 7b34 362d 2d35 347d 2c0a 2020  ges={46--54},.  
+00002710: 2020 7965 6172 3d7b 3230 3230 7d0a 7d0a    year={2020}.}.
+00002720: 6060 600a                                ```.
```

### Comparing `adapters-0.1.2/setup.cfg` & `adapters-0.2.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `adapters-0.1.2/setup.py` & `adapters-0.2.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2020 The AdapterHub Team. All rights reserved.
+# Copyright 2020-2024 The AdapterHub Team. All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -47,24 +47,24 @@
     "myst-parser",
     "rjieba",
     "rouge-score!=0.0.7,!=0.0.8,!=0.1,!=0.1.1",
     "sacrebleu>=1.4.12,<2.0.0",
     "sacremoses",
     "scikit-learn",
     "sentencepiece>=0.1.91,!=0.1.92",
-    "sphinx-copybutton",
-    "sphinx-markdown-tables",
+    "sphinx-copybutton==0.5.2",
+    "sphinx-markdown-tables==0.0.17",
     "sphinx-rtd-theme==0.4.3",  # sphinx-rtd-theme==0.5.0 introduced big changes in the style.
-    "sphinx==3.2.1",
+    "sphinx==5.0.2",
     "sphinxext-opengraph==0.4.1",
-    "sphinx-intl",
-    "sphinx-multiversion",
+    "sphinx-intl==2.1.0",
+    "sphinx-multiversion==0.2.4",
     "timeout-decorator",
     "torch>=1.10,!=1.12.0",
-    "transformers~=4.36.0",
+    "transformers~=4.39.3",
 ]
 
 
 # this is a lookup table with items like:
 #
 # tokenizers: "tokenizers==0.9.4"
 # packaging: "packaging"
@@ -138,17 +138,17 @@
 # when modifying the following list, make sure to update src/transformers/dependency_versions_check.py
 install_requires = [
     deps["transformers"],
 ]
 
 setup(
     name="adapters",
-    version="0.1.2",
+    version="0.2.0",
     author="The AdapterHub team and community contributors",
-    author_email="pfeiffer@ukp.tu-darmstadt.de",
+    author_email="calpt@mail.de",
     description="A Unified Library for Parameter-Efficient and Modular Transfer Learning",
     long_description=open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     keywords="NLP deep learning transformer pytorch BERT adapters",
     license="Apache",
     url="https://github.com/adapter-hub/adapters",
     package_dir={"": "src"},
```

### Comparing `adapters-0.1.2/src/adapters/__init__.py` & `adapters-0.2.0/src/adapters/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.1.2"
+__version__ = "0.2.0"
 
 from typing import TYPE_CHECKING
 
 from transformers.utils import _LazyModule
 
 
 _import_structure = {
```

### Comparing `adapters-0.1.2/src/adapters/composition.py` & `adapters-0.2.0/src/adapters/composition.py`

 * *Files identical despite different names*

### Comparing `adapters-0.1.2/src/adapters/configuration/adapter_config.py` & `adapters-0.2.0/src/adapters/configuration/adapter_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -178,14 +178,15 @@
             The reduction to use within the invertible adapter modules. Only applicable if :obj:`inv_adapter` is not
             None.
         cross_adapter (:obj:`bool`, optional):
             If True, add adapter modules after the cross attention block of each decoder layer in an encoder-decoder
             model. Defaults to False.
         leave_out (:obj:`List[int]`, optional):
             The IDs of the layers (starting at 0) where NO adapter modules should be added.
+        dropout (:obj:`float`, optional): The dropout rate used in the adapter layer. Defaults to 0.0.
         phm_layer (:obj:`bool`, optional): If True the down and up projection layers are a PHMLayer.
             Defaults to False
         phm_dim (:obj:`int`, optional): The dimension of the phm matrix.
             Only applicable if `phm_layer` is set to `True`. Defaults to 4.
         shared_phm_rule (:obj:`bool`, optional): Whether the phm matrix is shared across all layers.
             Defaults to True
         factorized_phm_rule (:obj:`bool`, optional):
@@ -230,14 +231,15 @@
     use_gating: bool = False
     residual_before_ln: Union[bool, str] = True
     adapter_residual_before_ln: bool = False
     inv_adapter: Optional[str] = None
     inv_adapter_reduction_factor: Optional[float] = None
     cross_adapter: bool = False
     leave_out: List[int] = field(default_factory=list)
+    dropout: float = 0.0
     phm_layer: bool = False
     phm_dim: int = 4
     factorized_phm_W: Optional[bool] = True
     shared_W_phm: Optional[bool] = False
     shared_phm_rule: Optional[bool] = True
     factorized_phm_rule: Optional[bool] = False
     phm_c_init: Optional[str] = "normal"
@@ -615,15 +617,15 @@
         prefix_tuning: Optional[PrefixTuningConfig] = None,
         adapter: Optional[BnConfig] = None,
         lora: Optional[LoRAConfig] = None,
     ):
         components = [
             prefix_tuning or PrefixTuningConfig(prefix_length=10),
             adapter or SeqBnConfig(reduction_factor=16),
-            lora or LoRAConfig(r=8),
+            lora or LoRAConfig(r=8, alpha=2),
         ]
 
         super().__init__(*[c.replace(use_gating=True) for c in components])
 
 
 # IMPORTANT: When adding a new config here, also add it to docs/overview.md!
 ADAPTER_CONFIG_MAP = {
```

### Comparing `adapters-0.1.2/src/adapters/configuration/adapter_fusion_config.py` & `adapters-0.2.0/src/adapters/configuration/adapter_fusion_config.py`

 * *Files identical despite different names*

### Comparing `adapters-0.1.2/src/adapters/configuration/model_adapters_config.py` & `adapters-0.2.0/src/adapters/configuration/model_adapters_config.py`

 * *Files identical despite different names*

### Comparing `adapters-0.1.2/src/adapters/context.py` & `adapters-0.2.0/src/adapters/context.py`

 * *Files identical despite different names*

### Comparing `adapters-0.1.2/src/adapters/head_utils.py` & `adapters-0.2.0/src/adapters/head_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -494,14 +494,15 @@
         "config": {
             "head_type": "question_answering",
             "layers": 1,
             "activation_function": None,
         },
         "layers": [None, "qa_outputs"],
     },
+    # T5
     "T5ForConditionalGeneration": {
         "config": {
             "head_type": "seq2seq_lm",
         },
         "layers": ["lm_head"],
     },
     "T5ForQuestionAnswering": {
@@ -522,14 +523,15 @@
             None,
             "classification_head.dense",
             None,
             None,
             "classification_head.out_proj",
         ],
     },
+    # DeBERTaV2
     "DebertaV2ForSequenceClassification": {
         "config": {
             "head_type": "classification",
             "layers": 2,
             "activation_function": "gelu",
             "use_pooler": False,
         },
@@ -571,14 +573,15 @@
             "head_type": "multiple_choice",
             "layers": 2,
             "activation_function": "gelu",
             "use_pooler": False,
         },
         "layers": [None, "pooler.dense", None, None, "classifier"],
     },
+    # DeBERTa
     "DebertaForSequenceClassification": {
         "config": {
             "head_type": "classification",
             "layers": 2,
             "activation_function": "gelu",
             "use_pooler": False,
         },
@@ -637,14 +640,23 @@
     },
     "LlamaForCausalLM": {
         "config": {
             "head_type": "causal_lm",
         },
         "layers": ["lm_head"],
     },
+    "LlamaForQuestionAnswering": {
+        "config": {
+            "head_type": "question_answering",
+            "layers": 1,
+            "activation_function": None,
+        },
+        "layers": [None, "qa_outputs"],
+    },
+    # Electra
     "ElectraForTokenClassification": {
         "config": {
             "head_type": "tagging",
             "layers": 1,
             "activation_function": None,
         },
         "layers": [None, "classifier"],
```

### Comparing `adapters-0.1.2/src/adapters/heads/base.py` & `adapters-0.2.0/src/adapters/heads/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,23 +61,31 @@
 # Let this class inherit from nn.Sequential to provide iterable access as before
 class PredictionHead(nn.Sequential):
     def __init__(self, name):
         super().__init__()
         self.config = {}
         self.name = name
 
-    def build(self, model):
-        model_config = model.config
-        pred_head = []
+    def _get_dropout_prob(self, model_config):
+        # try to infer dropout prob from various sources, default to 0.0
         if "dropout_prob" in self.config and self.config["dropout_prob"] is not None:
             dropout_prob = self.config["dropout_prob"]
         elif hasattr(model_config, "classifier_dropout") and model_config.classifier_dropout is not None:
             dropout_prob = model_config.classifier_dropout
-        else:
+        elif hasattr(model_config, "hidden_dropout_prob") and model_config.hidden_dropout_prob is not None:
             dropout_prob = model_config.hidden_dropout_prob
+        else:
+            dropout_prob = 0.0
+
+        return dropout_prob
+
+    def build(self, model):
+        model_config = model.config
+        pred_head = []
+        dropout_prob = self._get_dropout_prob(model_config)
         bias = self.config.get("bias", True)
         for l_id in range(self.config["layers"]):
             pred_head.append(nn.Dropout(dropout_prob))
             if l_id < self.config["layers"] - 1:
                 pred_head.append(nn.Linear(model_config.hidden_size, model_config.hidden_size))
                 if self.config["activation_function"]:
                     pred_head.append(Activation_Function_Class(self.config["activation_function"]))
```

### Comparing `adapters-0.1.2/src/adapters/heads/dependency_parsing.py` & `adapters-0.2.0/src/adapters/heads/dependency_parsing.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,15 +77,15 @@
 
     def build(self, model):
         self.biaffine_arcs = Biaffine(n_in=model.config.hidden_size, bias_x=True, bias_y=False)
         self.biaffine_rels = Biaffine(
             n_in=model.config.hidden_size, n_out=self.config["num_labels"], bias_x=True, bias_y=True
         )
 
-        self.dropout = nn.Dropout(model.config.hidden_dropout_prob)
+        self.dropout = nn.Dropout(self._get_dropout_prob(model.config))
 
         self.loss_fn = CrossEntropyLoss()
 
         self.train(model.training)  # make sure training mode is consistent
 
     def forward(
         self,
```

### Comparing `adapters-0.1.2/src/adapters/heads/language_modeling.py` & `adapters-0.2.0/src/adapters/heads/language_modeling.py`

 * *Files identical despite different names*

### Comparing `adapters-0.1.2/src/adapters/heads/model_mixin.py` & `adapters-0.2.0/src/adapters/heads/model_mixin.py`

 * *Files identical despite different names*

### Comparing `adapters-0.1.2/src/adapters/hub_mixin.py` & `adapters-0.2.0/src/adapters/hub_mixin.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,16 @@
         datasets_tag: Optional[str] = None,
         tags: Optional[List[str]] = None,
         language: Optional[str] = None,
         license: Optional[str] = None,
         metrics: Optional[List[str]] = None,
         **kwargs
     ):
-        all_tags = {"adapter-transformers"}  # TODO: change this tag once changed on HF side
+        # Key remains "adapter-transformers", see: https://github.com/huggingface/huggingface.js/pull/459
+        all_tags = {"adapter-transformers"}
         datasets = set()
         # Dataset/ Task info
         dataset_name = None
         if adapterhub_tag is None and datasets_tag is None:
             raise ValueError("Either adapterhub_tag or datasets_tag must be specified.")
         if datasets_tag is not None:
             dataset_name = f"[{datasets_tag}](https://huggingface.co/datasets/{datasets_tag}/)"
```

### Comparing `adapters-0.1.2/src/adapters/loading.py` & `adapters-0.2.0/src/adapters/loading.py`

 * *Files identical despite different names*

### Comparing `adapters-0.1.2/src/adapters/methods/adapter_layer_base.py` & `adapters-0.2.0/src/adapters/methods/adapter_layer_base.py`

 * *Files 6% similar despite different names*

```diff
@@ -159,23 +159,28 @@
     allow_multi_parallelize = False
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self._init_mapping()
 
     def _init_mapping(self):
+        # Mapping between composition block types and names of composition functions
         self.composition_to_func_map = {
-            Stack: self.compose_stack,
-            Fuse: self.compose_fuse,
-            Split: self.compose_split,
-            BatchSplit: self.compose_batch_split,
-            Parallel: self.compose_parallel,
-            Average: self.compose_average,
+            Stack: "compose_stack",
+            Fuse: "compose_fuse",
+            Split: "compose_split",
+            BatchSplit: "compose_batch_split",
+            Parallel: "compose_parallel",
+            Average: "compose_average",
         }
 
+    def _get_compose_func(self, composition_type: type) -> callable:
+        """Retrieves the correct composition function based on the mapping in 'composition_to_func_map'."""
+        return getattr(self, self.composition_to_func_map[composition_type])
+
     # START CUSTOMIZABLE METHODS #
     # The following methods should be implemented in derived classes.
 
     def _bsz(self, state: NamedTuple) -> int:
         """
         Returns the batch size of the given state.
         """
@@ -297,41 +302,43 @@
     def compose_stack(self, adapter_setup: Stack, state: NamedTuple, lvl: int = 0) -> NamedTuple:
         """
         For sequentially stacking multiple adapters.
         """
         for i, adapter_stack_layer in enumerate(adapter_setup):
             if isinstance(adapter_stack_layer, AdapterCompositionBlock):
                 self.check_composition_valid(adapter_setup, adapter_stack_layer, lvl)
-                composition_func = self.composition_to_func_map[type(adapter_stack_layer)]
+                composition_func = self._get_compose_func(type(adapter_stack_layer))
                 state = composition_func(adapter_stack_layer, state, lvl=lvl + 1)
             elif adapter_stack_layer in self.adapter_modules:
                 state = self.pre_block(adapter_stack_layer, state)
                 state = self.compose_single(adapter_stack_layer, state, lvl=lvl + 1)
             else:
-                raise ValueError(
-                    "Invalid adapter setup: {} is not a valid adapter name or composition block.".format(
-                        adapter_stack_layer.__class__.__name__
-                    )
-                )
+                pass
 
         return state
 
     def compose_fuse(self, adapter_setup: Fuse, state: NamedTuple, lvl: int = 0):
         """
         For fusing multiple adapters using adapter fusion. NOTE: This method has no default implementation.
         """
         # Fuse is currently only applicable to bottleneck adapters, thus don't provide a default implementation
+        # If the adapter setup does not contain any of the adapter modules, return without doing anything
+        if set(self.adapter_modules.keys()).isdisjoint(adapter_setup.flatten()):
+            return state
         raise NotImplementedError()
 
     def compose_split(self, adapter_setup: Split, state: NamedTuple, lvl: int = 0):
         """
         For splitting to multiple adapters along the sequence length dimension. NOTE: This method has no default
         implementation.
         """
         # Split is currently only applicable to bottleneck adapters, thus don't provide a default implementation
+        # If the adapter setup does not contain any of the adapter modules, return without doing anything
+        if set(self.adapter_modules.keys()).isdisjoint(adapter_setup.flatten()):
+            return state
         raise NotImplementedError()
 
     def compose_batch_split(self, adapter_setup: BatchSplit, state: NamedTuple, lvl: int = 0):
         """
         For splitting to multiple adapters along the batch size dimension.
         """
         if sum(adapter_setup.batch_sizes) != self._bsz(state):
@@ -349,15 +356,15 @@
             # compute ids of sequences that should be passed to the ith adapter
             batch_idx = (
                 sum(adapter_setup.batch_sizes[:i]),
                 sum(adapter_setup.batch_sizes[: i + 1]),
             )
             if isinstance(child, AdapterCompositionBlock):
                 self.check_composition_valid(adapter_setup, child, lvl)
-                composition_func = self.composition_to_func_map[type(child)]
+                composition_func = self._get_compose_func(type(child))
                 child_state = composition_func(
                     child,
                     self.vslice(state, slice(*batch_idx)),
                     lvl=lvl + 1,
                 )
                 children_states.append(child_state)
             elif child in self.adapter_modules:
@@ -406,15 +413,15 @@
         state = self.pre_block(adapter_setup, state)
 
         # sequentially feed different parts of the blown-up batch into different adapters
         children_states = []
         for i, child in enumerate(adapter_setup):
             if isinstance(child, AdapterCompositionBlock):
                 self.check_composition_valid(adapter_setup, child, lvl)
-                composition_func = self.composition_to_func_map[type(child)]
+                composition_func = self._get_compose_func(type(child))
                 child_state = composition_func(
                     child,
                     self.vslice(state, slice(i * orig_batch_size, (i + 1) * orig_batch_size)),
                     lvl=lvl + 1,
                 )
                 children_states.append(child_state)
             elif child in self.adapter_modules:
@@ -438,15 +445,15 @@
 
         state = self.pre_block(adapter_setup, state)
 
         children_states = []
         for i, child in enumerate(adapter_setup):
             if isinstance(child, AdapterCompositionBlock):
                 self.check_composition_valid(adapter_setup, child, lvl)
-                composition_func = self.composition_to_func_map[type(child)]
+                composition_func = self._get_compose_func(type(child))
                 child_state = composition_func(child, state, lvl=lvl + 1)
                 children_states.append(child_state)
             elif child in self.adapter_modules:
                 child_state = self.compose_single(child, state, lvl=lvl + 1)
                 children_states.append(child_state)
             else:
                 pass
@@ -464,15 +471,15 @@
             adapter_setup (Union[AdapterCompositionBlock, str]): The adapter setup to be used.
             state (NamedTuple): The current state.
 
         Returns:
             NamedTuple: The state after forwarding through the adapter setup.
         """
         if isinstance(adapter_setup, AdapterCompositionBlock):
-            composition_func = self.composition_to_func_map[type(adapter_setup)]
+            composition_func = self._get_compose_func(type(adapter_setup))
             state = composition_func(adapter_setup, state, lvl=0)
         elif adapter_setup in self.adapter_modules:
             state = self.compose_single(adapter_setup, state, lvl=0)
         else:
             raise ValueError(
                 "Invalid adapter setup: {} is not a valid adapter name or composition block.".format(
                     adapter_setup.__class__.__name__
```

### Comparing `adapters-0.1.2/src/adapters/methods/bottleneck.py` & `adapters-0.2.0/src/adapters/methods/bottleneck.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,21 +26,23 @@
     Args:
         hidden_states (torch.Tensor): The layer input/ output hidden states.
         input_tensor (torch.Tensor): The Transformer sub-block residual connection inputs.
         adapter_residual (torch.Tensor): The adapter residual connection inputs.
         layer_norm (torch.nn.Module, optional): The Transformer layer norm module.
         bottleneck_up (torch.Tensor, optional):
             The up-projected bottleneck MLP output. This is only for Fuse compositions.
+        last (str, optional): Name of the last adapter applied in the composition.
     """
 
     hidden_states: torch.Tensor
     input_tensor: torch.Tensor
     adapter_residual: torch.Tensor
     layer_norm: Optional[torch.nn.Module]
     bottleneck_up: Optional[torch.Tensor] = None
+    last: Optional[str] = None
 
 
 class BottleneckLayer(ComposableAdapterLayerBase, nn.Module):
     adapter_modules_name = "adapters"
     supported_compositions = [Stack, Fuse, Split, Parallel, BatchSplit, Average]
 
     def __init__(self, location_key: str):
@@ -189,77 +191,82 @@
     def vslice(self, state: BottleneckState, slice_obj: slice) -> BottleneckState:
         return BottleneckState(
             state.hidden_states[slice_obj],
             state.input_tensor[slice_obj],
             state.adapter_residual[slice_obj],
             state.layer_norm,
             state.bottleneck_up[slice_obj] if state.bottleneck_up is not None else None,
+            state.last,
         )
 
     def pad_and_concat(self, states: List[BottleneckState]) -> BottleneckState:
         return BottleneckState(
             torch.cat([state.hidden_states for state in states], dim=0),
             torch.cat([state.input_tensor for state in states], dim=0),
             torch.cat([state.adapter_residual for state in states], dim=0),
             states[0].layer_norm,
             torch.cat([state.bottleneck_up for state in states], dim=0)
             if states[0].bottleneck_up is not None
             else None,
+            states[-1].last,
         )
 
     def repeat(self, state: BottleneckState, channels: int) -> BottleneckState:
         return BottleneckState(
             state.hidden_states.repeat(channels, 1, 1),
             state.input_tensor.repeat(channels, 1, 1),
             state.adapter_residual.repeat(channels, 1, 1),
             state.layer_norm,
             state.bottleneck_up.repeat(channels, 1, 1) if state.bottleneck_up is not None else None,
+            state.last,
         )
 
     def mean(self, states: List[BottleneckState], weights: torch.Tensor) -> BottleneckState:
         return BottleneckState(
             torch.mean(torch.stack([s.hidden_states for s in states], 0) * weights, dim=0),
             states[0].input_tensor,
             states[0].adapter_residual,
             states[0].layer_norm,
             states[0].bottleneck_up,
+            states[-1].last,
         )
 
     def compose_single(self, adapter_setup: str, state: BottleneckState, lvl: int = 0) -> BottleneckState:
         adapter_layer = self.adapters[adapter_setup]
         context = ForwardContext.get_context()
         layer_output = adapter_layer(
             state.hidden_states,
             residual_input=state.adapter_residual,
             output_gating=context.output_adapter_gating_scores,
         )
         hidden_states, up = layer_output[0], layer_output[2]
         self._store_gating_score(adapter_setup, layer_output[-1])
 
-        return BottleneckState(hidden_states, state.input_tensor, state.adapter_residual, state.layer_norm, up)
+        return state._replace(hidden_states=hidden_states, bottleneck_up=up, last=adapter_setup)
 
     def compose_fuse(self, adapter_setup: Fuse, state: BottleneckState, lvl: int = 0):
         """
         Performs adapter fusion with the given adapters for the given input.
         """
         context = ForwardContext.get_context()
 
         # config of _last_ fused adapter is significant
         fusion_config = self.adapters_config.get_fusion(adapter_setup.name)
-        last_adapter = self.adapters[adapter_setup.last()]
+        last = adapter_setup.last()
+        last_adapter = self.adapters[last]
         hidden_states, query, residual = last_adapter.pre_forward(
             state.hidden_states, state.input_tensor, state.layer_norm, fusion_config=fusion_config
         )
         state = state._replace(hidden_states=hidden_states, adapter_residual=residual)
 
         children_states = []
         for child in adapter_setup:
             if isinstance(child, AdapterCompositionBlock):
                 self.check_composition_valid(adapter_setup, child, lvl)
-                composition_func = self.composition_to_func_map[type(child)]
+                composition_func = self._get_compose_func(type(child))
                 child_state = composition_func(child, state, lvl=lvl + 1)
                 children_states.append(child_state)
             elif child in self.adapter_modules:
                 child_state = self.compose_single(child, state, lvl=lvl + 1)
                 children_states.append(child_state)
             else:
                 pass
@@ -277,15 +284,15 @@
             )
             if context.output_adapter_fusion_attentions:
                 hidden_states = fusion_output[0]
                 self._store_fusion_attentions(adapter_setup.name, fusion_output[-1])
             else:
                 hidden_states = fusion_output
 
-        return state._replace(hidden_states=hidden_states)
+        return state._replace(hidden_states=hidden_states, last=last)
 
     def compose_split(self, adapter_setup: Split, state: BottleneckState, lvl: int = 0):
         """
         Splits the given input between the given adapters.
         """
         if sum(adapter_setup.splits) != state.hidden_states.shape[1]:
             raise IndexError(
@@ -293,39 +300,42 @@
                     state.hidden_states.shape[1], adapter_setup.splits
                 )
             )
 
         state = self.pre_block(adapter_setup, state)
 
         children_states = []
+        last = None
         for i, child in enumerate(adapter_setup):
             batch_idx = (
                 sum(adapter_setup.splits[:i]),
                 sum(adapter_setup.splits[: i + 1]),
             )
             child_state = BottleneckState(
                 state.hidden_states[:, batch_idx[0] : batch_idx[1], :],
                 state.input_tensor[:, batch_idx[0] : batch_idx[1], :],
                 state.adapter_residual[:, batch_idx[0] : batch_idx[1], :],
                 state.layer_norm,
                 state.bottleneck_up[:, batch_idx[0] : batch_idx[1], :] if state.bottleneck_up is not None else None,
             )
             if isinstance(child, AdapterCompositionBlock):
                 self.check_composition_valid(adapter_setup, child, lvl)
-                composition_func = self.composition_to_func_map[type(child)]
+                composition_func = self._get_compose_func(type(child))
                 child_state = composition_func(child, child_state, lvl=lvl + 1)
                 children_states.append(child_state)
+                last = child_state.last or last
             elif child in self.adapter_modules:
                 child_state = self.compose_single(child, child_state, lvl=lvl + 1)
                 children_states.append(child_state)
+                last = child_state.last or last
             else:
                 pass
 
         hidden_states = torch.cat([child.hidden_states for child in children_states], dim=1)
-        return state._replace(hidden_states=hidden_states)
+        return state._replace(hidden_states=hidden_states, last=last)
 
     def bottleneck_layer_forward(self, hidden_states, residual_input, layer_norm):
         """Forward pass through the adapter layer.
         NOTE: This method should only be called if the calling module directly inherits from BottleneckLayer.
         Otherwise, call the regular forward() method.
 
         Args:
@@ -342,17 +352,17 @@
         (hidden_states,) = adjust_tensors_for_parallel(residual_input, hidden_states)
         adapter_setup = self.get_active_setup()
         if adapter_setup is not None:
             input_hidden_states = hidden_states
 
             state = BottleneckState(hidden_states, residual_input, residual_input, layer_norm)
             state = self.compose(adapter_setup, state)
-            hidden_states, residual_input, _, _, _ = state
+            hidden_states, residual_input, _, _, _, last = state
 
-            last_adapter = self.adapters[adapter_setup.last()]
+            last_adapter = self.adapters[last]
             hidden_states = last_adapter.post_forward(hidden_states, input_hidden_states, residual_input, layer_norm)
 
         elif layer_norm:
             hidden_states = layer_norm(hidden_states + residual_input)
         else:
             hidden_states = hidden_states + residual_input
```

### Comparing `adapters-0.1.2/src/adapters/methods/lora.py` & `adapters-0.2.0/src/adapters/methods/lora.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,16 +13,24 @@
 
 from transformers.configuration_utils import PretrainedConfig
 from transformers.pytorch_utils import Conv1D
 
 from ..composition import AdapterCompositionBlock, Average, BatchSplit, Parallel, Stack
 from ..configuration import LoRAConfig, ModelAdaptersConfig
 from .adapter_layer_base import AdapterLayerBase, ComposableAdapterLayerBase
+from .utils import dequantize_bnb_weight
 
 
+try:
+    from bitsandbytes.nn import Int8Params, Linear4bit, Linear8bitLt, Params4bit
+
+    bitsandbytes_available = True
+except ImportError:
+    bitsandbytes_available = False
+
 logger = logging.getLogger(__name__)
 
 
 class LoRA(nn.Module):
     def __init__(
         self,
         lora_A_shape,
@@ -206,14 +214,15 @@
                 raise ValueError(f"Unknown composition_mode: {lora_config.composition_mode}")
             lora = lora_cls(
                 *self._get_lora_shapes(lora_config),
                 lora_config,
                 gating_heads=self.get_n_heads(lora_config),
             )
             lora.train(self.training)
+            lora = lora.to(self.weight.device)
             self.loras[adapter_name] = lora
             return True
 
         return False
 
     def average_adapter(self, adapter_name: str, input_adapters: Dict[str, float]) -> bool:
         # add new adapter
@@ -272,22 +281,24 @@
 
     Args:
         layer_input (torch.Tensor): The input states to the adapted layer.
         hidden_states (Optional[torch.Tensor]):
             The hidden states of the adaptation module. These can be None before passing through the first LoRA/ IA3
             module.
         layer_output (torch.Tensor): The output states of the original layer without adaptation.
+        last (str, optional): Name of the last adapter applied in the composition.
     """
 
     layer_input: torch.Tensor
     hidden_states: Optional[torch.Tensor]
     layer_output: torch.Tensor
+    last: Optional[str]
 
 
-class LoRALinear(LoRALayer, ComposableAdapterLayerBase, nn.Linear):
+class LoRALinear(LoRALayer, ComposableAdapterLayerBase):
     """
     LoRA implementation for Linear layer. This layer supports composition.
 
     Args:
         fan_in_fan_out (bool, optional):
             Set this to True if the layer to replace stores weight like (fan_in, fan_out). Defaults to False.
         no_init_bias (bool, optional): Use this to add a bias that is not initialized by PyTorch. Defaults to False.
@@ -327,131 +338,232 @@
         location_key: str,
         model_config: PretrainedConfig,
         adapters_config: ModelAdaptersConfig,
         attn_key: str = None,
         **kwargs
     ):
         if isinstance(module, Conv1D):
-            new_module = cls(
+            new_module = LoRALinearTorch(
                 module.weight.shape[0],
                 module.weight.shape[1],
                 location_key,
                 model_config,
                 adapters_config,
                 attn_key=attn_key,
                 **kwargs,
             )
         else:
+            if bitsandbytes_available and isinstance(module, Linear4bit):
+                cls = LoRALinear4bit
+            elif bitsandbytes_available and isinstance(module, Linear8bitLt):
+                cls = LoRALinear8bitLt
+            else:
+                cls = LoRALinearTorch
             # Make sure that the bias is not added if the original module does not have one
             if "bias" not in kwargs:
                 kwargs["bias"] = hasattr(module, "bias") and module.bias is not None
             new_module = cls(
                 module.in_features,
                 module.out_features,
                 location_key,
                 model_config,
                 adapters_config,
                 attn_key=attn_key,
                 **kwargs,
             )
-        new_module.weight.data = module.weight.data
-        if module.bias is not None:
-            new_module.bias.data = module.bias.data
+        new_module.copy_from(module)
 
         return new_module
 
+    def copy_from(self, module: nn.Linear):
+        self.weight = module.weight
+        if module.bias is not None:
+            self.bias = module.bias
+
     def _check_lora_location(self, config: LoRAConfig):
         return self.attn_key is None or self.attn_key in config.attn_matrices
 
     def _get_lora_shapes(self, config: LoRAConfig):
         return (config.r, self.in_features), (self.out_features, config.r)
 
     def maybe_t(self, w):
         return torch.t(w) if self.fan_in_fan_out else w
 
-    def reset_adapter(self):
-        if self.merged:
-            lora = self.loras[self.merged]
-            # Make sure that the weights are not merged
-            delta_w = self.maybe_t(lora.delta_w)
-            self.weight.data = lora.com_inv(self.weight.data, delta_w)
-            self.merged = None
-
     def merge_adapter(self, name: str):
         if name in self.loras:
             if self.merged == name:
                 return  # already merged
             elif not self.merged:
                 lora = self.loras[name]
                 if lora.use_gating:
                     raise ValueError("Cannot merge LoRA layer with gating.")
                 delta_w = self.maybe_t(lora.delta_w)
                 self.weight.data = lora.com(self.weight.data, delta_w)
                 self.merged = name
             elif self.merged != name:
                 raise ValueError("LoRALayer already has a merged LoRA module. Please reset it first.")
 
+    def reset_adapter(self):
+        if self.merged:
+            lora = self.loras[self.merged]
+            # Make sure that the weights are not merged
+            delta_w = self.maybe_t(lora.delta_w)
+            self.weight.data = lora.com_inv(self.weight.data, delta_w)
+            self.merged = None
+
     def vslice(self, state: LoRAState, slice_obj: slice) -> LoRAState:
         return LoRAState(
             state.layer_input[slice_obj],
             state.hidden_states[slice_obj] if state.hidden_states is not None else None,
             state.layer_output[slice_obj],
+            state.last,
         )
 
     def pad_and_concat(self, states: List[LoRAState]) -> LoRAState:
         return LoRAState(
             torch.cat([s.layer_input for s in states], dim=0),
             torch.cat([s.hidden_states for s in states], dim=0) if states[0].hidden_states is not None else None,
             torch.cat([s.layer_output for s in states], dim=0),
+            states[-1].last,
         )
 
     def repeat(self, state: LoRAState, channels: int) -> LoRAState:
         return LoRAState(
             state.layer_input.repeat(channels, 1, 1),
             state.hidden_states.repeat(channels, 1, 1) if state.hidden_states is not None else None,
             state.layer_output.repeat(channels, 1, 1),
+            state.last,
         )
 
     def mean(self, states: List[LoRAState], weights: torch.Tensor) -> LoRAState:
         return LoRAState(
             states[0].layer_input,
             torch.mean(torch.stack([s.hidden_states for s in states], dim=0) * weights, dim=0)
             if states[0].hidden_states is not None
             else None,
             states[0].layer_output,
+            states[-1].last,
         )
 
     def compose_single(self, adapter_setup: str, state: LoRAState, lvl: int = 0) -> LoRAState:
         lora = self.loras[adapter_setup]
         hidden_states, gate = lora(state.hidden_states, state.layer_input)
         if gate is not None:
             self._store_gating_score(adapter_setup, gate)
 
-        return state._replace(hidden_states=hidden_states)
+        return state._replace(hidden_states=hidden_states, last=adapter_setup)
 
     def forward(self, input_states: torch.Tensor):
-        weight = torch.transpose(self.weight, -2, -1) if self.fan_in_fan_out else self.weight
-        # result shape: <batch_size> x <seq_len> x <head_dim>
-        layer_output = F.linear(input_states, weight, bias=self.bias)
+        if self.fan_in_fan_out:
+            weight = torch.transpose(self.weight, -2, -1) if self.fan_in_fan_out else self.weight
+            # result shape: <batch_size> x <seq_len> x <head_dim>
+            layer_output = F.linear(input_states, weight, bias=self.bias)
+        else:
+            layer_output = super().forward(input_states)
 
         if not self.merged:
             adapter_setup = self.get_active_setup()
             if adapter_setup is not None:
-                state = LoRAState(input_states, None, layer_output)
+                state = LoRAState(input_states, None, layer_output, None)
                 state = self.compose(adapter_setup, state)
-                _, hidden_states, layer_output = state
+                _, hidden_states, layer_output, last = state
 
-                last_lora = self.loras[adapter_setup.last()]
+                last_lora = self.loras[last]
                 layer_output = last_lora.com(
                     layer_output, hidden_states, scaling=1.0
                 )  # scaling already applied in compose
 
         return layer_output
 
 
+class LoRALinearTorch(LoRALinear, nn.Linear):
+    pass
+
+
+if bitsandbytes_available:
+
+    class LoRALinear4bit(LoRALinear, Linear4bit):
+        def copy_from(self, module: Linear4bit):
+            self.weight = module.weight
+            if module.bias is not None:
+                self.bias = module.bias
+            self.compute_dtype = module.compute_dtype
+            self.compute_type_is_set = module.compute_type_is_set
+            self.quant_state = module.quant_state
+            self.quant_storage = module.quant_storage
+
+        def merge_adapter(self, name: str):
+            if name in self.loras:
+                if self.merged == name:
+                    return  # already merged
+                elif not self.merged:
+                    lora = self.loras[name]
+                    if lora.use_gating:
+                        raise ValueError("Cannot merge LoRA layer with gating.")
+                    delta_w = self.maybe_t(lora.delta_w)
+                    layer_weight = dequantize_bnb_weight(self.weight, state=self.quant_state)
+                    kwargs = self.weight.__dict__
+                    merged_weight = lora.com(layer_weight, delta_w)
+                    self.weight = Params4bit(merged_weight.to("cpu"), requires_grad=False, **kwargs).to(
+                        self.weight.device
+                    )
+                    self.merged = name
+                elif self.merged != name:
+                    raise ValueError("LoRALayer already has a merged LoRA module. Please reset it first.")
+
+        def reset_adapter(self):
+            if self.merged:
+                lora = self.loras[self.merged]
+                delta_w = self.maybe_t(lora.delta_w)
+                merged_weight = dequantize_bnb_weight(self.weight, state=self.quant_state)
+                kwargs = self.weight.__dict__
+                layer_weight = lora.com_inv(merged_weight, delta_w)
+                self.weight = Params4bit(layer_weight.to("cpu"), requires_grad=False, **kwargs).to(self.weight.device)
+                self.merged = None
+
+    class LoRALinear8bitLt(LoRALinear, Linear8bitLt):
+        def copy_from(self, module: Linear8bitLt):
+            self.weight = module.weight
+            if module.bias is not None:
+                self.bias = module.bias
+            self.state = module.state
+            self.index = module.index
+
+        def merge_adapter(self, name: str):
+            if name in self.loras:
+                if self.merged == name:
+                    return  # already merged
+                elif not self.merged:
+                    lora = self.loras[name]
+                    if lora.use_gating:
+                        raise ValueError("Cannot merge LoRA layer with gating.")
+                    delta_w = self.maybe_t(lora.delta_w)
+                    layer_weight = dequantize_bnb_weight(self.weight, state=self.state)
+                    merged_weight = lora.com(layer_weight, delta_w)
+                    self.weight = Int8Params(
+                        merged_weight.to("cpu"), requires_grad=False, has_fp16_weights=self.weight.has_fp16_weights
+                    ).to(self.weight.device)
+                    self.state.reset_grads()
+                    self.merged = name
+                elif self.merged != name:
+                    raise ValueError("LoRALayer already has a merged LoRA module. Please reset it first.")
+
+        def reset_adapter(self):
+            if self.merged:
+                lora = self.loras[self.merged]
+                delta_w = self.maybe_t(lora.delta_w)
+                merged_weight = dequantize_bnb_weight(self.weight, state=self.state)
+                layer_weight = lora.com_inv(merged_weight, delta_w)
+                self.weight = Int8Params(
+                    layer_weight.to("cpu"), requires_grad=False, has_fp16_weights=self.weight.has_fp16_weights
+                ).to(self.weight.device)
+                self.state.reset_grads()
+                self.merged = None
+
+
 class LoRAMergedLinear(LoRALayer, nn.Linear):
     """
     LoRA implementation for merged attention layer, as used by some model implementations (e.g. GPT-2). This layer
     currently does not support composition.
 
     Args:
         fan_in_fan_out (bool, optional):
@@ -494,17 +606,17 @@
             new_module = cls(
                 module.weight.shape[0], module.weight.shape[1], location_key, model_config, adapters_config, **kwargs
             )
         else:
             new_module = cls(
                 module.in_features, module.out_features, location_key, model_config, adapters_config, **kwargs
             )
-        new_module.weight.data = module.weight.data
+        new_module.weight = module.weight
         if module.bias is not None:
-            new_module.bias.data = module.bias.data
+            new_module.bias = module.bias
 
         return new_module
 
     def get_n_heads(self, lora: Union[LoRA, IA3, LoRAConfig]):
         return len(set(lora.attn_matrices))
 
     def _get_lora_shapes(self, config: LoRAConfig):
```

### Comparing `adapters-0.1.2/src/adapters/methods/modeling.py` & `adapters-0.2.0/src/adapters/methods/modeling.py`

 * *Files 0% similar despite different names*

```diff
@@ -104,14 +104,16 @@
         # This means that we learn a new output layer norm, which replaces another layer norm learned in the bert layer
         if self.add_layer_norm_after:
             self.adapter_norm_after = nn.LayerNorm(self.input_size)
 
         if self.use_gating:
             self.gate = nn.Linear(self.input_size, 1)
 
+        self.dropout = nn.Dropout(p=config["dropout"])
+
         # if we want to initialize with the bert strategy then this function is called for all the linear layers
         if config["init_weights"] == "bert":
             self.adapter_down.apply(self.init_bert_weights)
             self.adapter_up.apply(self.init_bert_weights)
             if self.use_gating:
                 self.gate.apply(self.init_bert_weights)
         elif config["init_weights"] == "mam_adapter":
@@ -169,15 +171,15 @@
         return hidden_states, query, residual
 
     def forward(self, x, residual_input, output_gating=False):
         down = self.adapter_down(x)
 
         up = self.adapter_up(down)
         up = up * self.scaling
-        output = up
+        output = self.dropout(up)
 
         if self.use_gating:
             # x.shape = (batch_size, seq_len, hidden_size)
             gate = torch.sigmoid(self.gate(x))
             gate = torch.mean(gate, dim=1).unsqueeze(-1)
             output = output * gate
 
@@ -267,15 +269,15 @@
 
     def forward(self, x, residual_input, output_gating=False):
         down = self.adapter_down(x)
 
         up = self.adapter_up(down)
         up = up * self.scaling
 
-        output = up
+        output = self.dropout(up)
 
         if self.use_gating:
             # x.shape = (batch_size, seq_len, hidden_size)
             gate = torch.sigmoid(self.gate(x))
             gate = torch.mean(gate, dim=1).unsqueeze(-1)
             output = output * gate
```

### Comparing `adapters-0.1.2/src/adapters/methods/prefix_tuning.py` & `adapters-0.2.0/src/adapters/methods/prefix_tuning.py`

 * *Files 1% similar despite different names*

```diff
@@ -515,18 +515,20 @@
         # Replicate for Parallel block
         prefix_keys, prefix_values = adjust_tensors_for_parallel(state.key_states, prefix_keys, prefix_values)
 
         key_states = torch.cat([prefix_keys, state.key_states], dim=2)
         value_states = torch.cat([prefix_values, state.value_states], dim=2)
         if state.attention_mask is not None:
             if state.attention_mask.dim() == 2:  # e.g. for DistilBERT, attention_mask has shape (batch_size, seq_len)
-                prefix_mask = torch.ones(batch_size, prefix_keys.size(2)).to(state.attention_mask.device)
+                prefix_mask = torch.ones(batch_size, prefix_keys.size(2)).to(
+                    device=state.attention_mask.device, dtype=state.attention_mask.dtype
+                )
             else:
                 prefix_mask = torch.ones(batch_size, 1, state.attention_mask.size(2), prefix_keys.size(2)).to(
-                    state.attention_mask.device
+                    device=state.attention_mask.device, dtype=state.attention_mask.dtype
                 )
             if state.invert_mask:
                 prefix_mask = 1.0 - prefix_mask
             (prefix_mask,) = adjust_tensors_for_parallel(state.attention_mask, prefix_mask)
             attention_mask = torch.cat([prefix_mask, state.attention_mask], dim=-1)
         else:
             attention_mask = None
```

### Comparing `adapters-0.1.2/src/adapters/methods/prompt_tuning.py` & `adapters-0.2.0/src/adapters/methods/prompt_tuning.py`

 * *Files identical despite different names*

### Comparing `adapters-0.1.2/src/adapters/model_mixin.py` & `adapters-0.2.0/src/adapters/model_mixin.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from .loading import AdapterFusionLoader, AdapterLoader, PredictionHeadLoader, WeightsLoader
 from .methods.adapter_layer_base import AdapterLayerBase
 from .methods.bottleneck import BottleneckLayer
 from .methods.lora import LoRALayer
 from .methods.modeling import Adapter, GLOWCouplingBlock, NICECouplingBlock, init_shared_parameters
 from .methods.prefix_tuning import PrefixTuningLayer, PrefixTuningPool
 from .methods.prompt_tuning import PromptTuningLayer
-from .utils import EMBEDDING_FILE, TOKENIZER_PATH, get_adapter_config_hash, inherit_doc
+from .utils import EMBEDDING_FILE, TOKENIZER_PATH, get_adapter_config_hash, inherit_doc, patch_forward
 from .wrappers.configuration import SUBMODEL_NAMES, init_adapters_config
 
 
 logger = logging.getLogger(__name__)
 
 
 class InvertibleAdaptersMixin:
@@ -463,14 +463,15 @@
 
         if isinstance(self, InvertibleAdaptersMixin) or isinstance(self, InvertibleAdaptersWrapperMixin):
             self.enable_invertible_adapters(adapter_setup.flatten())
         # use the adapters to be trained by default in every forward pass
         self.set_active_adapters(adapter_setup)
         if train_embeddings:
             self.get_input_embeddings().train()
+            self.get_input_embeddings().weight.requires_grad = True
 
     def train_fusion(self, adapter_setup: Union[list, AdapterCompositionBlock], unfreeze_adapters=False):
         """Sets the model into mode for training of adapter fusion determined by a list of adapter names."""
         warnings.warn(
             "add_fusion() has been deprecated in favor of add_adapter_fusion(). Please use the newer method instead.",
             FutureWarning,
         )
@@ -1253,14 +1254,19 @@
         del self.config.adapters
 
 
 @inherit_doc
 class ModelBaseAdaptersMixin(ModelAdaptersMixin):
     add_base_adapters = True
 
+    def init_adapters(self, model_config, adapters_config, add_prefix_tuning_pool=True):
+        super().init_adapters(model_config, adapters_config, add_prefix_tuning_pool)
+
+        patch_forward(self)
+
     def post_embedding_forward(self, module, args, embedding_output):
         if isinstance(self, InvertibleAdaptersMixin) or isinstance(self, InvertibleAdaptersWrapperMixin):
             embedding_output = self.invertible_adapters_forward(embedding_output)
 
         embedding_output = self.prompt_tuning.forward(embedding_output)
 
         return embedding_output
@@ -1352,15 +1358,19 @@
         Sets the model into mode for training the given adapters. If self.base_model is self, must inherit from a class
         that implements this method, to preclude infinite recursion
         """
         if self.base_model is self:
             super().train_adapter(adapter_setup, train_embeddings)
         else:
             self.base_model.train_adapter(adapter_setup, train_embeddings)
-        self.freeze_embeddings()
+        if not train_embeddings:
+            self.freeze_embeddings()
+
+        # Hack to prevent HF Trainer from throwing an error due to peft missing.
+        self._hf_peft_config_loaded = True
 
     def train_adapter_fusion(self, adapter_setup: Union[list, AdapterCompositionBlock], unfreeze_adapters=False):
         """
         Sets the model into mode for training of adapter fusion determined by a list of adapter names. If
         self.base_model is self, must inherit from a class that implements this method, to preclude infinite recursion
         """
         if self.base_model is self:
```

### Comparing `adapters-0.1.2/src/adapters/models/__init__.py` & `adapters-0.2.0/src/adapters/models/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     CLIPTextModelAdaptersMixin,
     CLIPTextTransformerAdaptersMixin,
     CLIPVisionModelAdaptersMixin,
 )
 from .distilbert.mixin_distilbert import DistilBertModelAdaptersMixin, DistilBertTransformerAdaptersMixin
 from .gpt2.mixin_gpt2 import GPT2ModelAdapterMixin
 from .gptj.mixin_gptj import GPTJMLPAdaptersMixin, GPTJModelAdapterMixin
-from .llama.mixin_llama import LlamaModelAdapterMixin
+from .llama.mixin_llama import LlamaForQuestionAnsweringAdapterMixin, LlamaModelAdapterMixin
 from .t5.mixin_t5 import (
     T5BlockAdaptersMixin,
     T5ForCondiditionalGenerationWithHeadsMixin,
     T5ForQuestionAnsweringWithHeadsMixin,
     T5ModelAdaptersMixin,
 )
 from .vit.mixin_vit import ViTIntermediateAdaptersMixin, ViTModelAdaptersMixin
@@ -79,8 +79,9 @@
     "DebertaModel": BertModelAdaptersMixin,
     "DebertaLayer": BertLayerAdaptersMixin,
     "DebertaV2Model": BertModelAdaptersMixin,
     "DebertaV2Layer": BertLayerAdaptersMixin,
     "BertGenerationEncoder": BertModelAdaptersMixin,
     "BertGenerationLayer": BertLayerAdaptersMixin,
     "LlamaModel": LlamaModelAdapterMixin,
+    "LlamaForQuestionAnswering": LlamaForQuestionAnsweringAdapterMixin,
 }
```

### Comparing `adapters-0.1.2/src/adapters/models/albert/__init__.py` & `adapters-0.2.0/src/adapters/models/albert/__init__.py`

 * *Files identical despite different names*

### Comparing `adapters-0.1.2/src/adapters/models/albert/adapter_model.py` & `adapters-0.2.0/src/adapters/models/albert/adapter_model.py`

 * *Files identical despite different names*

### Comparing `adapters-0.1.2/src/adapters/models/albert/mixin_albert.py` & `adapters-0.2.0/src/adapters/models/albert/mixin_albert.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import torch.nn as nn
 
 from ...composition import adjust_tensors_for_parallel_
 from ...methods.bottleneck import BottleneckLayer
 from ...methods.lora import LoRALinear
 from ...methods.prefix_tuning import PrefixTuningLayer
 from ...model_mixin import EmbeddingAdaptersMixin, InvertibleAdaptersMixin, ModelBaseAdaptersMixin
+from ...utils import patch_forward
 
 
 class AlbertAttentionAdaptersMixin:
     """Adds adapters to the AlbertAttention module of ALBERT."""
 
     def init_adapters(self, model_config, adapters_config):
         # Wrap layers for LoRA
@@ -19,14 +20,15 @@
         self.value = LoRALinear.wrap(self.value, "selfattn", model_config, adapters_config, attn_key="v")
 
         self.attention_adapters = BottleneckLayer("mh_adapter")
 
         self.prefix_tuning = PrefixTuningLayer(
             self.location_key + "_prefix" if self.location_key else None, model_config, adapters_config
         )
+        patch_forward(self)
 
 
 class AlbertEncoderLayerAdaptersMixin:
     """Adds adapters to the AlbertLayer module."""
 
     def init_adapters(self, model_config, adapters_config):
         # Wrap layers for LoRA
@@ -36,14 +38,16 @@
         # Set location keys for prefix tuning
         self.location_key = "output_adapter"
 
         self.output_adapters = BottleneckLayer("output_adapter")
 
         self.attention.location_key = "self"
 
+        patch_forward(self)
+
 
 class AlbertModelAdaptersMixin(EmbeddingAdaptersMixin, InvertibleAdaptersMixin, ModelBaseAdaptersMixin):
     """Adds adapters to the AlbertModel module."""
 
     def init_adapters(self, model_config, adapters_config):
         super().init_adapters(model_config, adapters_config)
```

### Comparing `adapters-0.1.2/src/adapters/models/albert/modeling_albert.py` & `adapters-0.2.0/src/adapters/models/albert/modeling_albert.py`

 * *Files identical despite different names*

### Comparing `adapters-0.1.2/src/adapters/models/auto/__init__.py` & `adapters-0.2.0/src/adapters/models/auto/__init__.py`

 * *Files identical despite different names*

### Comparing `adapters-0.1.2/src/adapters/models/auto/adapter_model.py` & `adapters-0.2.0/src/adapters/models/auto/adapter_model.py`

 * *Files identical despite different names*

### Comparing `adapters-0.1.2/src/adapters/models/auto/auto_factory.py` & `adapters-0.2.0/src/adapters/models/auto/auto_factory.py`

 * *Files identical despite different names*

### Comparing `adapters-0.1.2/src/adapters/models/bart/__init__.py` & `adapters-0.2.0/src/adapters/models/bart/__init__.py`

 * *Files identical despite different names*

### Comparing `adapters-0.1.2/src/adapters/models/bart/adapter_model.py` & `adapters-0.2.0/src/adapters/models/bart/adapter_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import torch
 
 from transformers.models.bart.modeling_bart import (
     BART_INPUTS_DOCSTRING,
     BART_START_DOCSTRING,
     BartConfig,
     BartModel,
-    BartPretrainedModel,
+    BartPreTrainedModel,
     shift_tokens_right,
 )
 from transformers.utils import add_start_docstrings, add_start_docstrings_to_model_forward
 
 from ...heads import ModelWithFlexibleHeadsAdaptersMixin
 from ...model_mixin import EmbeddingAdaptersWrapperMixin
 from ...wrappers import init
 
 
 @add_start_docstrings(
     "BART Model with the option to add multiple flexible prediction heads on top.", BART_START_DOCSTRING
 )
-class BartAdapterModel(EmbeddingAdaptersWrapperMixin, ModelWithFlexibleHeadsAdaptersMixin, BartPretrainedModel):
+class BartAdapterModel(EmbeddingAdaptersWrapperMixin, ModelWithFlexibleHeadsAdaptersMixin, BartPreTrainedModel):
     _tied_weights_keys = [
         "encoder.embed_tokens.weight",
         "decoder.embed_tokens.weight",
     ]
 
     head_types = [
         "classification",
```

### Comparing `adapters-0.1.2/src/adapters/models/bart/mixin_bart.py` & `adapters-0.2.0/src/adapters/models/bart/mixin_bart.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,28 +10,30 @@
 from ...model_mixin import (
     EmbeddingAdaptersMixin,
     EmbeddingAdaptersWrapperMixin,
     InvertibleAdaptersMixin,
     InvertibleAdaptersWrapperMixin,
     ModelBaseAdaptersMixin,
 )
+from ...utils import patch_forward
 
 
 class BartAttentionAdaptersMixin:
     """Adds adapters to the BartAttention module."""
 
     def init_adapters(self, model_config, adapters_config):
         # Wrap layers for LoRA
         self.k_proj = LoRALinear.wrap(self.k_proj, "selfattn", model_config, adapters_config, attn_key="k")
         self.v_proj = LoRALinear.wrap(self.v_proj, "selfattn", model_config, adapters_config, attn_key="v")
         self.q_proj = LoRALinear.wrap(self.q_proj, "selfattn", model_config, adapters_config, attn_key="q")
 
         self.prefix_tuning = PrefixTuningLayer(
             self.location_key + "_prefix" if self.location_key else None, model_config, adapters_config
         )
+        patch_forward(self)
 
 
 class BartEncoderLayerAdaptersMixin:
     """Adds adapters to the BartEncoderLayer module of BART."""
 
     def init_adapters(self, model_config, adapters_config):
         self.adapters_config = adapters_config
@@ -40,14 +42,16 @@
         self.fc2 = LoRALinear.wrap(self.fc2, "output", model_config, adapters_config)
 
         # Set attention layer location key for prefix tuning
         self.self_attn.location_key = "encoder"
         self.attention_adapters = BottleneckLayer("mh_adapter")
         self.output_adapters = BottleneckLayer("output_adapter")
 
+        patch_forward(self)
+
 
 class BartDecoderLayerAdaptersMixin(BartEncoderLayerAdaptersMixin):
     """Adds adapters to the BartDecoderLayer module of BART."""
 
     def init_adapters(self, model_config, adapters_config):
         super().init_adapters(model_config, adapters_config)
         # Set attention layer location key for prefix tuning
@@ -61,14 +65,17 @@
 
     pass
 
 
 class BartDecoderAdaptersMixin:
     """Adds adapters to the BartDecoder module of BART."""
 
+    def init_adapters(self, model_config, adapters_config):
+        patch_forward(self)
+
     def forward(
         self, input_ids: torch.LongTensor = None, encoder_hidden_states: Optional[torch.FloatTensor] = None, **kwargs
     ):
         (input_ids,) = adjust_tensors_for_parallel(encoder_hidden_states, input_ids)
         return super().forward(input_ids=input_ids, encoder_hidden_states=encoder_hidden_states, **kwargs)
```

### Comparing `adapters-0.1.2/src/adapters/models/bart/modeling_bart.py` & `adapters-0.2.0/src/adapters/models/bart/modeling_bart.py`

 * *Files identical despite different names*

### Comparing `adapters-0.1.2/src/adapters/models/beit/__init__.py` & `adapters-0.2.0/src/adapters/models/beit/__init__.py`

 * *Files identical despite different names*

### Comparing `adapters-0.1.2/src/adapters/models/beit/adapter_model.py` & `adapters-0.2.0/src/adapters/models/beit/adapter_model.py`

 * *Files identical despite different names*

### Comparing `adapters-0.1.2/src/adapters/models/beit/mixin_beit.py` & `adapters-0.2.0/src/adapters/models/vit/mixin_vit.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,60 +2,64 @@
 
 import torch.nn as nn
 
 from ...methods.bottleneck import BottleneckLayer
 from ...methods.lora import LoRALinear
 from ...methods.prefix_tuning import PrefixTuningLayer
 from ...model_mixin import ModelBaseAdaptersMixin
+from ...utils import patch_forward
 
 
-class BeitSelfAttentionAdaptersMixin:
+class ViTSelfAttentionAdaptersMixin:
     def init_adapters(self, model_config, adapters_config):
         self.location_key = "self"
 
         # Wrap layers for LoRA
         self.query = LoRALinear.wrap(self.query, "selfattn", model_config, adapters_config, attn_key="q")
         self.key = LoRALinear.wrap(self.key, "selfattn", model_config, adapters_config, attn_key="k")
         self.value = LoRALinear.wrap(self.value, "selfattn", model_config, adapters_config, attn_key="v")
 
         self.prefix_tuning = PrefixTuningLayer(
             self.location_key + "_prefix" if self.location_key else None, model_config, adapters_config
         )
+        patch_forward(self)
 
 
-class BeitIntermediateAdaptersMixin:
+class ViTIntermediateAdaptersMixin:
     def init_adapters(self, model_config, adapters_config):
         # Wrap layers for LoRA
         self.dense = LoRALinear.wrap(self.dense, "intermediate", model_config, adapters_config)
 
 
-class BeitOutputAdaptersMixin:
+class ViTOutputAdaptersMixin:
+    """Adds adapters to the ViTOutput module."""
+
     def init_adapters(self, model_config, adapters_config):
+        self.output_adapters = BottleneckLayer("output_adapter")
+
         # Wrap layers for LoRA
         self.dense = LoRALinear.wrap(self.dense, "output", model_config, adapters_config)
 
+        patch_forward(self)
+
 
-class BeitLayerAdaptersMixin:
-    """Adds adapters to the BeitLayer module."""
+# Unlike BERT, self attention adapters are added to Layer module in ViT
+class ViTLayerAdaptersMixin:
+    """Adds adapters to the ViTSelfOutput module."""
 
     def init_adapters(self, model_config, adapters_config):
         self.attention_adapters = BottleneckLayer("mh_adapter")
-        self.output_adapters = BottleneckLayer("output_adapter")
+        patch_forward(self)
 
 
-class BeitModelAdaptersMixin(ModelBaseAdaptersMixin):
-    """Adds adapters to the BeitModel module."""
+class ViTModelAdaptersMixin(ModelBaseAdaptersMixin):
+    """Adds adapters to the ViTModel class."""
 
     def init_adapters(self, model_config, adapters_config):
         super().init_adapters(model_config, adapters_config)
+
+        # Register hook for post embedding forward
         self.embeddings.register_forward_hook(self.post_embedding_forward)
 
     def iter_layers(self) -> Iterable[Tuple[int, nn.Module]]:
         for i, layer in enumerate(self.encoder.layer):
             yield i, layer
-
-    def set_input_embeddings(self, value):
-        self.embeddings.patch_embeddings = value
-
-    def post_embedding_forward(self, module, args, outputs):
-        embedding_output, tup = outputs
-        return super().post_embedding_forward(module, args, embedding_output), tup
```

### Comparing `adapters-0.1.2/src/adapters/models/beit/modeling_beit.py` & `adapters-0.2.0/src/adapters/models/beit/modeling_beit.py`

 * *Files identical despite different names*

### Comparing `adapters-0.1.2/src/adapters/models/bert/__init__.py` & `adapters-0.2.0/src/adapters/models/bert/__init__.py`

 * *Files identical despite different names*

### Comparing `adapters-0.1.2/src/adapters/models/bert/adapter_model.py` & `adapters-0.2.0/src/adapters/models/bert/adapter_model.py`

 * *Files identical despite different names*

### Comparing `adapters-0.1.2/src/adapters/models/bert/mixin_bert.py` & `adapters-0.2.0/src/adapters/models/bert/mixin_bert.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import torch.nn as nn
 
 from ...composition import adjust_tensors_for_parallel_
 from ...methods.bottleneck import BottleneckLayer
 from ...methods.lora import LoRALinear
 from ...methods.prefix_tuning import PrefixTuningLayer
 from ...model_mixin import EmbeddingAdaptersMixin, InvertibleAdaptersMixin, ModelBaseAdaptersMixin
+from ...utils import patch_forward
 
 
 logger = logging.getLogger(__name__)
 
 
 class BertSelfAttentionAdaptersMixin:
     """Adds adapters to the BertSelfAttention module."""
@@ -21,38 +22,41 @@
         self.query = LoRALinear.wrap(self.query, "selfattn", model_config, adapters_config, attn_key="q")
         self.key = LoRALinear.wrap(self.key, "selfattn", model_config, adapters_config, attn_key="k")
         self.value = LoRALinear.wrap(self.value, "selfattn", model_config, adapters_config, attn_key="v")
 
         self.prefix_tuning = PrefixTuningLayer(
             self.location_key + "_prefix" if self.location_key else None, model_config, adapters_config
         )
+        patch_forward(self)
 
 
 # For backwards compatibility, BertSelfOutput inherits directly from BottleneckLayer
 class BertSelfOutputAdaptersMixin(BottleneckLayer):
     """Adds adapters to the BertSelfOutput module."""
 
     def __init__(self):
         super().__init__("mh_adapter")
 
     def init_adapters(self, model_config, adapters_config):
         self.location_key = "mh_adapter"
         super().init_adapters(model_config, adapters_config)
+        patch_forward(self)
 
 
 # For backwards compatibility, BertOutput inherits directly from BottleneckLayer
 class BertOutputAdaptersMixin(BottleneckLayer):
     """Adds adapters to the BertOutput module."""
 
     def __init__(self):
         super().__init__("output_adapter")
 
     def init_adapters(self, model_config, adapters_config):
         self.location_key = "output_adapter"
         super().init_adapters(model_config, adapters_config)
+        patch_forward(self)
 
 
 class BertLayerAdaptersMixin:
     """Adds adapters to the BertLayer module."""
 
     def init_adapters(self, model_config, adapters_config):
         # Wrap layers for LoRA
```

### Comparing `adapters-0.1.2/src/adapters/models/bert/modeling_bert.py` & `adapters-0.2.0/src/adapters/models/bert/modeling_bert.py`

 * *Files identical despite different names*

### Comparing `adapters-0.1.2/src/adapters/models/bert_generation/__init__.py` & `adapters-0.2.0/src/adapters/models/bert_generation/__init__.py`

 * *Files identical despite different names*

### Comparing `adapters-0.1.2/src/adapters/models/bert_generation/adapter_model.py` & `adapters-0.2.0/src/adapters/models/bert_generation/adapter_model.py`

 * *Files identical despite different names*

### Comparing `adapters-0.1.2/src/adapters/models/bert_generation/modeling_bert_generation.py` & `adapters-0.2.0/src/adapters/models/bert_generation/modeling_bert_generation.py`

 * *Files identical despite different names*

### Comparing `adapters-0.1.2/src/adapters/models/clip/__init__.py` & `adapters-0.2.0/src/adapters/models/clip/__init__.py`

 * *Files identical despite different names*

### Comparing `adapters-0.1.2/src/adapters/models/clip/adapter_model.py` & `adapters-0.2.0/src/adapters/models/clip/adapter_model.py`

 * *Files identical despite different names*

### Comparing `adapters-0.1.2/src/adapters/models/clip/mixin_clip.py` & `adapters-0.2.0/src/adapters/models/clip/mixin_clip.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,41 +9,45 @@
 from ...model_mixin import (
     EmbeddingAdaptersMixin,
     EmbeddingAdaptersWrapperMixin,
     InvertibleAdaptersMixin,
     InvertibleAdaptersWrapperMixin,
     ModelBaseAdaptersMixin,
 )
+from ...utils import patch_forward
 
 
 class CLIPAttentionAdaptersMixin:
     """Adds adapters to the CLIPAttention module."""
 
     def init_adapters(self, model_config, adapters_config):
         # Wrap layers for LoRA
         self.q_proj = LoRALinear.wrap(self.q_proj, "selfattn", model_config, adapters_config, attn_key="q")
         self.k_proj = LoRALinear.wrap(self.k_proj, "selfattn", model_config, adapters_config, attn_key="k")
         self.v_proj = LoRALinear.wrap(self.v_proj, "selfattn", model_config, adapters_config, attn_key="v")
 
         self.prefix_tuning = PrefixTuningLayer(
             "self_prefix", model_config, adapters_config, add_model_type_to_key=True
         )
+        patch_forward(self)
 
 
 class CLIPEncoderLayerAdaptersMixin:
     """Adds adapters to the CLIPEncoderLayer module of CLIP."""
 
     def init_adapters(self, model_config, adapters_config):
         # Wrap layers for LoRA
         self.mlp.fc1 = LoRALinear.wrap(self.mlp.fc1, "intermediate", model_config, adapters_config)
         self.mlp.fc2 = LoRALinear.wrap(self.mlp.fc2, "output", model_config, adapters_config)
 
         self.attention_adapters = BottleneckLayer("mh_adapter")
         self.output_adapters = BottleneckLayer("output_adapter")
 
+        patch_forward(self)
+
 
 class CLIPEncoderAdaptersMixin:
     """Adds adapters to the CLIPEncoder module of CLIP."""
 
     def init_adapters(self, model_config, adapters_config):
         # Set hook for parallel composition
         for layer in self.layers:
```

### Comparing `adapters-0.1.2/src/adapters/models/clip/modeling_clip.py` & `adapters-0.2.0/src/adapters/models/clip/modeling_clip.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,15 +62,15 @@
                 f" {attn_weights.size()}"
             )
 
         # apply the causal_attention_mask first
         if causal_attention_mask is not None:
             prefix_mask = torch.ones(
                 bsz, 1, causal_attention_mask.size(2), src_len - causal_attention_mask.size(-1)
-            ).to(causal_attention_mask.device)
+            ).to(device=causal_attention_mask.device, dtype=causal_attention_mask.dtype)
             causal_attention_mask = torch.cat([prefix_mask, causal_attention_mask], dim=-1)
             if causal_attention_mask.size() != (bsz, 1, tgt_len, src_len):
                 raise ValueError(
                     f"Attention mask should be of size {(bsz, 1, tgt_len, src_len)}, but is"
                     f" {causal_attention_mask.size()}"
                 )
             attn_weights = attn_weights.view(bsz, self.num_heads, tgt_len, src_len) + causal_attention_mask
```

### Comparing `adapters-0.1.2/src/adapters/models/deberta/__init__.py` & `adapters-0.2.0/src/adapters/models/deberta/__init__.py`

 * *Files identical despite different names*

### Comparing `adapters-0.1.2/src/adapters/models/deberta/adapter_model.py` & `adapters-0.2.0/src/adapters/models/deberta/adapter_model.py`

 * *Files identical despite different names*

### Comparing `adapters-0.1.2/src/adapters/models/deberta/mixin_deberta.py` & `adapters-0.2.0/src/adapters/models/deberta/mixin_deberta.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from ...methods.lora import LoRAMergedLinear
 from ...methods.prefix_tuning import PrefixTuningLayer
+from ...utils import patch_forward
 
 
 class DebertaSelfAttentionAdaptersMixin:
     """Adds adapters to the BertSelfAttention module."""
 
     def init_adapters(self, model_config, adapters_config):
         # Wrap layers for LoRA
         self.in_proj = LoRAMergedLinear.wrap(self.in_proj, "selfattn", model_config, adapters_config)
 
         self.prefix_tuning = PrefixTuningLayer(
             self.location_key + "_prefix" if self.location_key else None, model_config, adapters_config
         )
+        patch_forward(self)
```

### Comparing `adapters-0.1.2/src/adapters/models/deberta/modeling_deberta.py` & `adapters-0.2.0/src/adapters/models/deberta/modeling_deberta.py`

 * *Files identical despite different names*

### Comparing `adapters-0.1.2/src/adapters/models/deberta_v2/__init__.py` & `adapters-0.2.0/src/adapters/models/deberta_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `adapters-0.1.2/src/adapters/models/deberta_v2/adapter_model.py` & `adapters-0.2.0/src/adapters/models/deberta_v2/adapter_model.py`

 * *Files identical despite different names*

### Comparing `adapters-0.1.2/src/adapters/models/deberta_v2/mixin_deberta_v2.py` & `adapters-0.2.0/src/adapters/models/deberta_v2/mixin_deberta_v2.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from ...methods.lora import LoRALinear
 from ...methods.prefix_tuning import PrefixTuningLayer
+from ...utils import patch_forward
 
 
 class DebertaV2SelfAttentionAdaptersMixin:
     """Adds adapters to the BertSelfAttention module."""
 
     def init_adapters(self, model_config, adapters_config):
         # Wrap layers for LoRA
         self.query_proj = LoRALinear.wrap(self.query_proj, "selfattn", model_config, adapters_config, attn_key="q")
         self.key_proj = LoRALinear.wrap(self.key_proj, "selfattn", model_config, adapters_config, attn_key="k")
         self.value_proj = LoRALinear.wrap(self.value_proj, "selfattn", model_config, adapters_config, attn_key="v")
 
         self.prefix_tuning = PrefixTuningLayer(
             self.location_key + "_prefix" if self.location_key else None, model_config, adapters_config
         )
+        patch_forward(self)
```

### Comparing `adapters-0.1.2/src/adapters/models/deberta_v2/modeling_deberta_v2.py` & `adapters-0.2.0/src/adapters/models/deberta_v2/modeling_deberta_v2.py`

 * *Files identical despite different names*

### Comparing `adapters-0.1.2/src/adapters/models/distilbert/__init__.py` & `adapters-0.2.0/src/adapters/models/distilbert/__init__.py`

 * *Files identical despite different names*

### Comparing `adapters-0.1.2/src/adapters/models/distilbert/adapter_model.py` & `adapters-0.2.0/src/adapters/models/distilbert/adapter_model.py`

 * *Files identical despite different names*

### Comparing `adapters-0.1.2/src/adapters/models/distilbert/mixin_distilbert.py` & `adapters-0.2.0/src/adapters/models/distilbert/mixin_distilbert.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,43 +2,50 @@
 
 import torch.nn as nn
 
 from ...methods.bottleneck import BottleneckLayer
 from ...methods.lora import LoRALinear
 from ...methods.prefix_tuning import PrefixTuningLayer
 from ...model_mixin import EmbeddingAdaptersMixin, InvertibleAdaptersMixin, ModelBaseAdaptersMixin
+from ...utils import patch_forward
 
 
 class DistilBertMultiHeadSelfAttentionMixin:
     """Adds adapters to the MultiHeadSelfAttention module of DistilBert."""
 
     def init_adapters(self, model_config, adapters_config):
         # Wrap layers for LoRA
         self.q_lin = LoRALinear.wrap(self.q_lin, "selfattn", model_config, adapters_config, attn_key="q")
         self.k_lin = LoRALinear.wrap(self.k_lin, "selfattn", model_config, adapters_config, attn_key="k")
         self.v_lin = LoRALinear.wrap(self.v_lin, "selfattn", model_config, adapters_config, attn_key="v")
 
         self.prefix_tuning = PrefixTuningLayer("self", model_config, adapters_config)
+        patch_forward(self)
 
 
 class DistilBertTransfomerBlockAdaptersMixin:
     """Adds adapters to the TransformerBlock module of DistilBert."""
 
     def init_adapters(self, model_config, adapters_config):
         # Wrap layers for LoRA
         self.ffn.lin1 = LoRALinear.wrap(self.ffn.lin1, "intermediate", model_config, adapters_config)
         self.ffn.lin2 = LoRALinear.wrap(self.ffn.lin2, "output", model_config, adapters_config)
 
         self.attention_adapters = BottleneckLayer("mh_adapter")
         self.output_adapters = BottleneckLayer("output_adapter")
 
+        patch_forward(self)
+
 
 class DistilBertTransformerAdaptersMixin:
     """Adds adapters to the Transformer module of DistilBert."""
 
+    def init_adapters(self, model_config, adapters_config):
+        patch_forward(self)
+
     def forward(self, *args, **kwargs):
         if hasattr(self, "pre_forward_fn"):
             kwargs["x"] = self.pre_forward_fn(self, kwargs["x"])
         return super().forward(*args, **kwargs)
 
 
 class DistilBertModelAdaptersMixin(EmbeddingAdaptersMixin, InvertibleAdaptersMixin, ModelBaseAdaptersMixin):
```

### Comparing `adapters-0.1.2/src/adapters/models/distilbert/modeling_distilbert.py` & `adapters-0.2.0/src/adapters/models/distilbert/modeling_distilbert.py`

 * *Files identical despite different names*

### Comparing `adapters-0.1.2/src/adapters/models/electra/__init__.py` & `adapters-0.2.0/src/adapters/models/electra/__init__.py`

 * *Files identical despite different names*

### Comparing `adapters-0.1.2/src/adapters/models/electra/adapter_model.py` & `adapters-0.2.0/src/adapters/models/electra/adapter_model.py`

 * *Files identical despite different names*

### Comparing `adapters-0.1.2/src/adapters/models/electra/modeling_electra.py` & `adapters-0.2.0/src/adapters/models/electra/modeling_electra.py`

 * *Files identical despite different names*

### Comparing `adapters-0.1.2/src/adapters/models/gpt2/__init__.py` & `adapters-0.2.0/src/adapters/models/gpt2/__init__.py`

 * *Files identical despite different names*

### Comparing `adapters-0.1.2/src/adapters/models/gpt2/adapter_model.py` & `adapters-0.2.0/src/adapters/models/gpt2/adapter_model.py`

 * *Files identical despite different names*

### Comparing `adapters-0.1.2/src/adapters/models/gpt2/mixin_gpt2.py` & `adapters-0.2.0/src/adapters/models/gpt2/mixin_gpt2.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import torch.nn as nn
 
 from ...methods.bottleneck import BottleneckLayer
 from ...methods.lora import LoRALinear, LoRAMergedLinear
 from ...methods.prefix_tuning import PrefixTuningLayer
 from ...model_mixin import EmbeddingAdaptersMixin, InvertibleAdaptersMixin, ModelBaseAdaptersMixin
+from ...utils import patch_forward
 
 
 class GPT2AttentionAdaptersMixin:
     """Adds adapters to the Attention module of GPT2."""
 
     def init_adapters(self, model_config, adapters_config):
         # Wrap layers for LoRA
@@ -22,14 +23,16 @@
                 fan_in_fan_out=True,
                 no_init_bias=True,
             )
 
         location_key = "cross_prefix" if self.is_cross_attention else "self_prefix"
         self.prefix_tuning = PrefixTuningLayer(location_key, model_config, adapters_config)
 
+        patch_forward(self)
+
 
 class GPT2DecoderBlockAdaptersMixin:
     """Adds adapters to the TransformerBlock module of DistilBert."""
 
     def init_adapters(self, model_config, adapters_config):
         # Wrap layers for LoRA
         self.mlp.c_fc = LoRALinear.wrap(
@@ -48,14 +51,16 @@
             fan_in_fan_out=True,
             no_init_bias=True,
         )
 
         self.attention_adapters = BottleneckLayer("mh_adapter")
         self.output_adapters = BottleneckLayer("output_adapter")
 
+        patch_forward(self)
+
 
 class GPT2ModelAdapterMixin(EmbeddingAdaptersMixin, InvertibleAdaptersMixin, ModelBaseAdaptersMixin):
     support_prompt_tuning = False
 
     def init_adapters(self, model_config, adapters_config):
         super().init_adapters(model_config, adapters_config)
```

### Comparing `adapters-0.1.2/src/adapters/models/gpt2/modeling_gpt2.py` & `adapters-0.2.0/src/adapters/models/gpt2/modeling_gpt2.py`

 * *Files identical despite different names*

### Comparing `adapters-0.1.2/src/adapters/models/gptj/__init__.py` & `adapters-0.2.0/src/adapters/models/gptj/__init__.py`

 * *Files identical despite different names*

### Comparing `adapters-0.1.2/src/adapters/models/gptj/adapter_model.py` & `adapters-0.2.0/src/adapters/models/gptj/adapter_model.py`

 * *Files identical despite different names*

### Comparing `adapters-0.1.2/src/adapters/models/gptj/mixin_gptj.py` & `adapters-0.2.0/src/adapters/models/gptj/mixin_gptj.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,28 +2,30 @@
 
 import torch.nn as nn
 
 from ...methods.bottleneck import BottleneckLayer
 from ...methods.lora import LoRALinear
 from ...methods.prefix_tuning import PrefixTuningLayer
 from ...model_mixin import EmbeddingAdaptersMixin, InvertibleAdaptersMixin, ModelBaseAdaptersMixin
+from ...utils import patch_forward
 
 
 class GPTJAttentionAdaptersMixin:
     def init_adapters(self, model_config, adapters_config):
         self.location_key = "self"
 
         # Wrap layers for LoRA
         self.q_proj = LoRALinear.wrap(self.q_proj, "selfattn", model_config, adapters_config, attn_key="q")
         self.k_proj = LoRALinear.wrap(self.k_proj, "selfattn", model_config, adapters_config, attn_key="k")
         self.v_proj = LoRALinear.wrap(self.v_proj, "selfattn", model_config, adapters_config, attn_key="v")
 
         self.prefix_tuning = PrefixTuningLayer(
             self.location_key + "_prefix" if self.location_key else None, model_config, adapters_config
         )
+        patch_forward(self)
 
 
 class GPTJMLPAdaptersMixin:
     def init_adapters(self, model_config, adapters_config):
         # Wrap layers for LoRA
         self.fc_in = LoRALinear.wrap(self.fc_in, "intermediate", model_config, adapters_config)
         self.fc_out = LoRALinear.wrap(self.fc_out, "output", model_config, adapters_config)
@@ -32,14 +34,16 @@
 class GPTJDecoderBlockAdaptersMixin:
     """Adds adapters to the TransformerBlock module of GPTJ."""
 
     def init_adapters(self, model_config, adapters_config):
         self.attention_adapters = BottleneckLayer("mh_adapter")
         self.output_adapters = BottleneckLayer("output_adapter")
 
+        patch_forward(self)
+
 
 class GPTJModelAdapterMixin(EmbeddingAdaptersMixin, InvertibleAdaptersMixin, ModelBaseAdaptersMixin):
     support_prompt_tuning = False
 
     def init_adapters(self, model_config, adapters_config):
         super().init_adapters(model_config, adapters_config)
```

### Comparing `adapters-0.1.2/src/adapters/models/gptj/modeling_gptj.py` & `adapters-0.2.0/src/adapters/models/gptj/modeling_gptj.py`

 * *Files identical despite different names*

### Comparing `adapters-0.1.2/src/adapters/models/llama/__init__.py` & `adapters-0.2.0/src/adapters/models/llama/__init__.py`

 * *Files identical despite different names*

### Comparing `adapters-0.1.2/src/adapters/models/llama/adapter_model.py` & `adapters-0.2.0/src/adapters/models/llama/adapter_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import logging
+from typing import Optional
 
 import torch
 
 from transformers.models.llama.modeling_llama import LLAMA_START_DOCSTRING, LlamaModel, LlamaPreTrainedModel
 from transformers.utils import add_start_docstrings
 
 from ...composition import adjust_tensors_for_parallel
@@ -54,14 +55,15 @@
         self,
         input_ids=None,
         attention_mask=None,
         position_ids=None,
         past_key_values=None,
         inputs_embeds=None,
         use_cache=None,
+        cache_position: Optional[torch.LongTensor] = None,
         output_attentions=None,
         output_hidden_states=None,
         return_dict=None,
         head=None,
         output_adapter_gating_scores=False,
         output_adapter_fusion_attentions=False,
         **kwargs
@@ -75,14 +77,15 @@
         outputs, context = self.model(
             input_ids,
             past_key_values=past_key_values,
             attention_mask=attention_mask,
             position_ids=position_ids,
             inputs_embeds=inputs_embeds,
             use_cache=use_cache,
+            cache_position=cache_position,
             output_attentions=output_attentions,
             return_dict=return_dict,
             output_hidden_states=output_hidden_states,
             output_adapter_gating_scores=output_adapter_gating_scores,
             output_adapter_fusion_attentions=output_adapter_fusion_attentions,
             adapter_input_parallelized=kwargs.pop("adapter_input_parallelized", False),
             output_context=True,
```

### Comparing `adapters-0.1.2/src/adapters/models/llama/mixin_llama.py` & `adapters-0.2.0/src/adapters/models/beit/mixin_beit.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,46 +1,64 @@
 from typing import Iterable, Tuple
 
 import torch.nn as nn
 
 from ...methods.bottleneck import BottleneckLayer
 from ...methods.lora import LoRALinear
 from ...methods.prefix_tuning import PrefixTuningLayer
-from ...model_mixin import EmbeddingAdaptersMixin, InvertibleAdaptersMixin, ModelBaseAdaptersMixin
+from ...model_mixin import ModelBaseAdaptersMixin
+from ...utils import patch_forward
 
 
-class LlamaAttentionMixin:
+class BeitSelfAttentionAdaptersMixin:
     def init_adapters(self, model_config, adapters_config):
-        self.q_proj = LoRALinear.wrap(self.q_proj, "selfattn", model_config, adapters_config, attn_key="q")
-        self.k_proj = LoRALinear.wrap(self.k_proj, "selfattn", model_config, adapters_config, attn_key="k")
-        self.v_proj = LoRALinear.wrap(self.v_proj, "selfattn", model_config, adapters_config, attn_key="v")
+        self.location_key = "self"
 
-        self.prefix_tuning = PrefixTuningLayer("self_prefix", model_config, adapters_config)
+        # Wrap layers for LoRA
+        self.query = LoRALinear.wrap(self.query, "selfattn", model_config, adapters_config, attn_key="q")
+        self.key = LoRALinear.wrap(self.key, "selfattn", model_config, adapters_config, attn_key="k")
+        self.value = LoRALinear.wrap(self.value, "selfattn", model_config, adapters_config, attn_key="v")
+
+        self.prefix_tuning = PrefixTuningLayer(
+            self.location_key + "_prefix" if self.location_key else None, model_config, adapters_config
+        )
+        patch_forward(self)
+
+
+class BeitIntermediateAdaptersMixin:
+    def init_adapters(self, model_config, adapters_config):
+        # Wrap layers for LoRA
+        self.dense = LoRALinear.wrap(self.dense, "intermediate", model_config, adapters_config)
 
 
-class LlamaDecoderLayerMixin:
+class BeitOutputAdaptersMixin:
     def init_adapters(self, model_config, adapters_config):
         # Wrap layers for LoRA
-        self.mlp.down_proj = LoRALinear.wrap(self.mlp.down_proj, "intermediate", model_config, adapters_config)
-        self.mlp.up_proj = LoRALinear.wrap(self.mlp.up_proj, "output", model_config, adapters_config)
+        self.dense = LoRALinear.wrap(self.dense, "output", model_config, adapters_config)
 
+
+class BeitLayerAdaptersMixin:
+    """Adds adapters to the BeitLayer module."""
+
+    def init_adapters(self, model_config, adapters_config):
         self.attention_adapters = BottleneckLayer("mh_adapter")
         self.output_adapters = BottleneckLayer("output_adapter")
+        patch_forward(self)
 
 
-class LlamaModelAdapterMixin(EmbeddingAdaptersMixin, InvertibleAdaptersMixin, ModelBaseAdaptersMixin):
-    support_prompt_tuning = False
+class BeitModelAdaptersMixin(ModelBaseAdaptersMixin):
+    """Adds adapters to the BeitModel module."""
 
     def init_adapters(self, model_config, adapters_config):
         super().init_adapters(model_config, adapters_config)
-
-        # Register hook for post embedding forward
-        self.embed_tokens.register_forward_hook(self.post_embedding_forward)
+        self.embeddings.register_forward_hook(self.post_embedding_forward)
 
     def iter_layers(self) -> Iterable[Tuple[int, nn.Module]]:
-        for i, layer in enumerate(self.layers):
+        for i, layer in enumerate(self.encoder.layer):
             yield i, layer
 
-    def post_embedding_forward(self, module, args, embedding_output):
-        embedding_output = self.invertible_adapters_forward(embedding_output)
-        # Prompt tuning not yet supported
-        return embedding_output
+    def set_input_embeddings(self, value):
+        self.embeddings.patch_embeddings = value
+
+    def post_embedding_forward(self, module, args, outputs):
+        embedding_output, tup = outputs
+        return super().post_embedding_forward(module, args, embedding_output), tup
```

### Comparing `adapters-0.1.2/src/adapters/models/llama/modeling_llama.py` & `adapters-0.2.0/src/adapters/models/llama/modeling_llama.py`

 * *Files 12% similar despite different names*

```diff
@@ -23,19 +23,15 @@
 from typing import Optional, Tuple
 
 import torch
 import torch.nn.functional as F
 import torch.utils.checkpoint
 from torch import nn
 
-from adapters.composition import (
-    adjust_tensors_for_parallel,
-    adjust_tensors_for_parallel_,
-    match_attn_matrices_for_parallel,
-)
+from adapters.composition import adjust_tensors_for_parallel, match_attn_matrices_for_parallel
 from transformers.cache_utils import Cache
 from transformers.models.llama.modeling_llama import LlamaAttention, LlamaDecoderLayer, apply_rotary_pos_emb, repeat_kv
 from transformers.utils import logging
 
 from .mixin_llama import LlamaAttentionMixin, LlamaDecoderLayerMixin
 
 
@@ -49,22 +45,17 @@
         self,
         hidden_states: torch.Tensor,
         attention_mask: Optional[torch.Tensor] = None,
         position_ids: Optional[torch.LongTensor] = None,
         past_key_value: Optional[Cache] = None,
         output_attentions: bool = False,
         use_cache: bool = False,
+        cache_position: Optional[torch.LongTensor] = None,
         **kwargs,
     ) -> Tuple[torch.Tensor, Optional[torch.Tensor], Optional[Tuple[torch.Tensor]]]:
-        if "padding_mask" in kwargs:
-            warnings.warn(
-                "Passing `padding_mask` is deprecated and will be removed in v4.37. Please make sure use"
-                " `attention_mask` instead.`"
-            )
-
         bsz, q_len, _ = hidden_states.size()
 
         if self.config.pretraining_tp > 1:
             key_value_slicing = (self.num_key_value_heads * self.head_dim) // self.config.pretraining_tp
             query_slices = self.q_proj.weight.split(
                 (self.num_heads * self.head_dim) // self.config.pretraining_tp, dim=0
             )
@@ -90,56 +81,38 @@
         value_states = value_states.view(bsz, q_len, self.num_key_value_heads, self.head_dim).transpose(1, 2)
 
         query_states, key_states, value_states = match_attn_matrices_for_parallel(
             query_states, key_states, value_states
         )
         (attention_mask,) = adjust_tensors_for_parallel(query_states, attention_mask)
 
-        kv_seq_len = key_states.shape[-2]
-        if past_key_value is not None:
-            if self.layer_idx is None:
-                raise ValueError(
-                    "The cache structure has changed since version v4.36. If you are using"
-                    f" {self.__class__.__name__} for auto-regressive decoding with k/v caching, please make sure to"
-                    " initialize the attention class with a layer index."
-                )
-            kv_seq_len += past_key_value.get_usable_length(kv_seq_len, self.layer_idx)
-        cos, sin = self.rotary_emb(value_states, seq_len=kv_seq_len)
-        query_states, key_states = apply_rotary_pos_emb(query_states, key_states, cos, sin, position_ids)
+        past_key_value = getattr(self, "past_key_value", past_key_value)
+        cos, sin = self.rotary_emb(value_states, position_ids)
+        query_states, key_states = apply_rotary_pos_emb(query_states, key_states, cos, sin)
 
         if past_key_value is not None:
-            cache_kwargs = {"sin": sin, "cos": cos}  # Specific to RoPE models
+            # sin and cos are specific to RoPE models; cache_position needed for the static cache
+            cache_kwargs = {"sin": sin, "cos": cos, "cache_position": cache_position}
             key_states, value_states = past_key_value.update(key_states, value_states, self.layer_idx, cache_kwargs)
 
         key_states = repeat_kv(key_states, self.num_key_value_groups)
         value_states = repeat_kv(value_states, self.num_key_value_groups)
 
         key_states, value_states, attention_mask = self.prefix_tuning(
             key_states, value_states, hidden_states, attention_mask
         )
         (query_states,) = adjust_tensors_for_parallel(key_states, query_states)
 
         attn_weights = torch.matmul(query_states, key_states.transpose(2, 3)) / math.sqrt(self.head_dim)
 
-        # Make adjustments since (parallel) prefix tuning changes the attention mask
-        kv_seq_len = key_states.shape[-2]
         bsz = key_states.shape[0]
 
-        if attn_weights.size() != (bsz, self.num_heads, q_len, kv_seq_len):
-            raise ValueError(
-                f"Attention weights should be of size {(bsz, self.num_heads, q_len, kv_seq_len)}, but is"
-                f" {attn_weights.size()}"
-            )
-
-        if attention_mask is not None:
-            if attention_mask.size() != (bsz, 1, q_len, kv_seq_len):
-                raise ValueError(
-                    f"Attention mask should be of size {(bsz, 1, q_len, kv_seq_len)}, but is {attention_mask.size()}"
-                )
-            attn_weights = attn_weights + attention_mask
+        if attention_mask is not None:  # no matter the length, we just slice it
+            causal_mask = attention_mask[:, :, :, : key_states.shape[-2]]
+            attn_weights = attn_weights + causal_mask
 
         # upcast attention to fp32
         attn_weights = nn.functional.softmax(attn_weights, dim=-1, dtype=torch.float32).to(query_states.dtype)
         attn_weights = nn.functional.dropout(attn_weights, p=self.attention_dropout, training=self.training)
         attn_output = torch.matmul(attn_weights, value_states)
 
         if attn_output.size() != (bsz, self.num_heads, q_len, self.head_dim):
@@ -170,26 +143,17 @@
         self,
         hidden_states: torch.Tensor,
         attention_mask: Optional[torch.LongTensor] = None,
         position_ids: Optional[torch.LongTensor] = None,
         past_key_value: Optional[Cache] = None,
         output_attentions: bool = False,
         use_cache: bool = False,
+        cache_position: Optional[torch.LongTensor] = None,
         **kwargs,
     ) -> Tuple[torch.Tensor, Optional[torch.Tensor], Optional[Tuple[torch.Tensor]]]:
-        # LlamaFlashAttention2 attention does not support output_attentions
-        if "padding_mask" in kwargs:
-            warnings.warn(
-                "Passing `padding_mask` is deprecated and will be removed in v4.37. Please make sure use"
-                " `attention_mask` instead.`"
-            )
-
-            # overwrite attention_mask with padding_mask
-            attention_mask = kwargs.pop("padding_mask")
-
         output_attentions = False
 
         bsz, q_len, _ = hidden_states.size()
 
         query_states = self.q_proj(hidden_states)
         key_states = self.k_proj(hidden_states)
         value_states = self.v_proj(hidden_states)
@@ -202,31 +166,29 @@
         value_states = value_states.view(bsz, q_len, self.num_key_value_heads, self.head_dim).transpose(1, 2)
 
         query_states, key_states, value_states = match_attn_matrices_for_parallel(
             query_states, key_states, value_states
         )
         (attention_mask,) = adjust_tensors_for_parallel(query_states, attention_mask)
 
-        kv_seq_len = key_states.shape[-2]
-        if past_key_value is not None:
-            kv_seq_len += past_key_value.get_usable_length(kv_seq_len, self.layer_idx)
-        cos, sin = self.rotary_emb(value_states, seq_len=kv_seq_len)
-        query_states, key_states = apply_rotary_pos_emb(query_states, key_states, cos, sin, position_ids)
+        cos, sin = self.rotary_emb(value_states, position_ids)
+        query_states, key_states = apply_rotary_pos_emb(query_states, key_states, cos, sin)
 
         key_states, value_states, attention_mask = self.prefix_tuning(
             key_states, value_states, hidden_states, attention_mask
         )
         (query_states,) = adjust_tensors_for_parallel(key_states, query_states)
 
-        # Make adjustments since (parallel) prefix tuning changes the attention mask
-        kv_seq_len = key_states.shape[-2]
         bsz = key_states.shape[0]
 
+        past_key_value = getattr(self, "past_key_value", past_key_value)
+
         if past_key_value is not None:
-            cache_kwargs = {"sin": sin, "cos": cos}  # Specific to RoPE models
+            # sin and cos are specific to RoPE models; cache_position needed for the static cache
+            cache_kwargs = {"sin": sin, "cos": cos, "cache_position": cache_position}
             key_states, value_states = past_key_value.update(key_states, value_states, self.layer_idx, cache_kwargs)
 
         # TODO: These transpose are quite inefficient but Flash Attention requires the layout [batch_size, sequence_length, num_heads, head_dim]. We would need to refactor the KV cache
         # to be able to avoid many of these transpose/reshape/view.
         query_states = query_states.transpose(1, 2)
         key_states = key_states.transpose(1, 2)
         value_states = value_states.transpose(1, 2)
@@ -237,16 +199,18 @@
         # therefore the input hidden states gets silently casted in float32. Hence, we need
         # cast them back in the correct dtype just to be sure everything works as expected.
         # This might slowdown training & inference so it is recommended to not cast the LayerNorms
         # in fp32. (LlamaRMSNorm handles it correctly)
 
         input_dtype = query_states.dtype
         if input_dtype == torch.float32:
+            if torch.is_autocast_enabled():
+                target_dtype = torch.get_autocast_gpu_dtype()
             # Handle the case where the model is quantized
-            if hasattr(self.config, "_pre_quantization_dtype"):
+            elif hasattr(self.config, "_pre_quantization_dtype"):
                 target_dtype = self.config._pre_quantization_dtype
             else:
                 target_dtype = self.q_proj.weight.dtype
 
             logger.warning_once(
                 "The input hidden states seems to be silently casted in float32, this might be related to the fact"
                 " you have upcasted embedding or layer norm layers in float32. We will cast back the input in"
@@ -277,14 +241,15 @@
         self,
         hidden_states: torch.Tensor,
         attention_mask: Optional[torch.Tensor] = None,
         position_ids: Optional[torch.LongTensor] = None,
         past_key_value: Optional[Cache] = None,
         output_attentions: bool = False,
         use_cache: bool = False,
+        cache_position: Optional[torch.LongTensor] = None,
     ) -> Tuple[torch.Tensor, Optional[torch.Tensor], Optional[Tuple[torch.Tensor]]]:
         if output_attentions:
             # TODO: Improve this warning with e.g. `model.config.attn_implementation = "manual"` once this is implemented.
             logger.warning_once(
                 "LlamaModel is using LlamaSdpaAttention, but `torch.nn.functional.scaled_dot_product_attention` does"
                 " not support `output_attentions=True`. Falling back to the manual attention implementation, but"
                 " specifying the manual implementation will be required from Transformers version v5.0.0 onwards. This"
@@ -293,14 +258,15 @@
             return super().forward(
                 hidden_states=hidden_states,
                 attention_mask=attention_mask,
                 position_ids=position_ids,
                 past_key_value=past_key_value,
                 output_attentions=output_attentions,
                 use_cache=use_cache,
+                cache_position=cache_position,
             )
 
         bsz, q_len, _ = hidden_states.size()
 
         query_states = self.q_proj(hidden_states)
         key_states = self.k_proj(hidden_states)
         value_states = self.v_proj(hidden_states)
@@ -310,62 +276,57 @@
         value_states = value_states.view(bsz, q_len, self.num_key_value_heads, self.head_dim).transpose(1, 2)
 
         query_states, key_states, value_states = match_attn_matrices_for_parallel(
             query_states, key_states, value_states
         )
         (attention_mask,) = adjust_tensors_for_parallel(query_states, attention_mask)
 
-        kv_seq_len = key_states.shape[-2]
-        if past_key_value is not None:
-            kv_seq_len += past_key_value.get_usable_length(kv_seq_len, self.layer_idx)
-        cos, sin = self.rotary_emb(value_states, seq_len=kv_seq_len)
+        cos, sin = self.rotary_emb(value_states, position_ids)
+        query_states, key_states = apply_rotary_pos_emb(query_states, key_states, cos, sin)
 
-        query_states, key_states = apply_rotary_pos_emb(query_states, key_states, cos, sin, position_ids)
+        # In case static cache is used, it is an instance attribute.
+        past_key_value = getattr(self, "past_key_value", past_key_value)
 
         if past_key_value is not None:
-            cache_kwargs = {"sin": sin, "cos": cos}  # Specific to RoPE models
+            # sin and cos are specific to RoPE models; cache_position needed for the static cache
+            cache_kwargs = {"sin": sin, "cos": cos, "cache_position": cache_position}
             key_states, value_states = past_key_value.update(key_states, value_states, self.layer_idx, cache_kwargs)
 
         key_states = repeat_kv(key_states, self.num_key_value_groups)
         value_states = repeat_kv(value_states, self.num_key_value_groups)
 
         key_states, value_states, attention_mask = self.prefix_tuning(
             key_states, value_states, hidden_states, attention_mask
         )
         (query_states,) = adjust_tensors_for_parallel(key_states, query_states)
 
-        # Make adjustments since (parallel) prefix tuning changes the attention mask
-        kv_seq_len = key_states.shape[-2]
         bsz = key_states.shape[0]
 
+        causal_mask = attention_mask
+        # if attention_mask is not None and cache_position is not None:
         if attention_mask is not None:
-            if attention_mask.size() != (bsz, 1, q_len, kv_seq_len):
-                raise ValueError(
-                    f"Attention mask should be of size {(bsz, 1, q_len, kv_seq_len)}, but is {attention_mask.size()}"
-                )
+            causal_mask = causal_mask[:, :, :, : key_states.shape[-2]]
 
         # SDPA with memory-efficient backend is currently (torch==2.1.2) bugged with non-contiguous inputs with custom attn_mask,
         # Reference: https://github.com/pytorch/pytorch/issues/112577.
-        if query_states.device.type == "cuda" and attention_mask is not None:
+        if query_states.device.type == "cuda" and causal_mask is not None:
             query_states = query_states.contiguous()
             key_states = key_states.contiguous()
             value_states = value_states.contiguous()
 
         attn_output = torch.nn.functional.scaled_dot_product_attention(
             query_states,
             key_states,
             value_states,
-            attn_mask=attention_mask,
+            attn_mask=causal_mask,
             dropout_p=self.attention_dropout if self.training else 0.0,
-            # The q_len > 1 is necessary to match with AttentionMaskConverter.to_causal_4d that does not create a causal mask in case q_len == 1.
-            is_causal=self.is_causal and attention_mask is None and q_len > 1,
         )
 
         attn_output = attn_output.transpose(1, 2).contiguous()
-        attn_output = attn_output.reshape(bsz, q_len, self.hidden_size)
+        attn_output = attn_output.view(bsz, q_len, self.hidden_size)
 
         attn_output = self.o_proj(attn_output)
 
         return attn_output, None, past_key_value
 
 
 class LlamaDecoderLayerWithAdapters(LlamaDecoderLayerMixin, LlamaDecoderLayer):
@@ -373,42 +334,51 @@
         self,
         hidden_states: torch.Tensor,
         attention_mask: Optional[torch.Tensor] = None,
         position_ids: Optional[torch.LongTensor] = None,
         past_key_value: Optional[Tuple[torch.Tensor]] = None,
         output_attentions: Optional[bool] = False,
         use_cache: Optional[bool] = False,
+        cache_position: Optional[torch.LongTensor] = None,
+        **kwargs,
     ) -> Tuple[torch.FloatTensor, Optional[Tuple[torch.FloatTensor, torch.FloatTensor]]]:
         """
         Args:
             hidden_states (`torch.FloatTensor`): input to the layer of shape `(batch, seq_len, embed_dim)`
-            attention_mask (`torch.FloatTensor`, *optional*): attention mask of size
-                `(batch, 1, tgt_len, src_len)` where padding elements are indicated by very large negative values.
+            attention_mask (`torch.FloatTensor`, *optional*):
+                attention mask of size `(batch_size, sequence_length)` if flash attention is used or `(batch_size, 1,
+                query_sequence_length, key_sequence_length)` if default attention is used.
             output_attentions (`bool`, *optional*):
                 Whether or not to return the attentions tensors of all attention layers. See `attentions` under
                 returned tensors for more detail.
             use_cache (`bool`, *optional*):
                 If set to `True`, `past_key_values` key value states are returned and can be used to speed up decoding
                 (see `past_key_values`).
             past_key_value (`Tuple(torch.FloatTensor)`, *optional*): cached past key and value projection states
         """
+        if "padding_mask" in kwargs:
+            warnings.warn(
+                "Passing `padding_mask` is deprecated and will be removed in v4.37. Please make sure use"
+                " `attention_mask` instead.`"
+            )
 
-        adjust_tensors_for_parallel_(hidden_states, attention_mask, position_ids)
         residual = hidden_states
 
         hidden_states = self.input_layernorm(hidden_states)
 
         # Self Attention
         hidden_states, self_attn_weights, present_key_value = self.self_attn(
             hidden_states=hidden_states,
             attention_mask=attention_mask,
             position_ids=position_ids,
             past_key_value=past_key_value,
             output_attentions=output_attentions,
             use_cache=use_cache,
+            cache_position=cache_position,
+            **kwargs,
         )
         hidden_states = self.attention_adapters(hidden_states, residual, None)
 
         # Fully Connected
         residual = hidden_states
         hidden_states = self.post_attention_layernorm(hidden_states)
         hidden_states = self.mlp(hidden_states)
```

### Comparing `adapters-0.1.2/src/adapters/models/mbart/__init__.py` & `adapters-0.2.0/src/adapters/models/mbart/__init__.py`

 * *Files identical despite different names*

### Comparing `adapters-0.1.2/src/adapters/models/mbart/adapter_model.py` & `adapters-0.2.0/src/adapters/models/mbart/adapter_model.py`

 * *Files identical despite different names*

### Comparing `adapters-0.1.2/src/adapters/models/mbart/modeling_mbart.py` & `adapters-0.2.0/src/adapters/models/mbart/modeling_mbart.py`

 * *Files identical despite different names*

### Comparing `adapters-0.1.2/src/adapters/models/mt5/__init__.py` & `adapters-0.2.0/src/adapters/models/mt5/__init__.py`

 * *Files identical despite different names*

### Comparing `adapters-0.1.2/src/adapters/models/mt5/adapter_model.py` & `adapters-0.2.0/src/adapters/models/mt5/adapter_model.py`

 * *Files identical despite different names*

### Comparing `adapters-0.1.2/src/adapters/models/mt5/modeling_mt5.py` & `adapters-0.2.0/src/adapters/models/mt5/modeling_mt5.py`

 * *Files identical despite different names*

### Comparing `adapters-0.1.2/src/adapters/models/roberta/__init__.py` & `adapters-0.2.0/src/adapters/models/roberta/__init__.py`

 * *Files identical despite different names*

### Comparing `adapters-0.1.2/src/adapters/models/roberta/adapter_model.py` & `adapters-0.2.0/src/adapters/models/roberta/adapter_model.py`

 * *Files identical despite different names*

### Comparing `adapters-0.1.2/src/adapters/models/roberta/modeling_roberta.py` & `adapters-0.2.0/src/adapters/models/roberta/modeling_roberta.py`

 * *Files identical despite different names*

### Comparing `adapters-0.1.2/src/adapters/models/t5/__init__.py` & `adapters-0.2.0/src/adapters/models/t5/__init__.py`

 * *Files identical despite different names*

### Comparing `adapters-0.1.2/src/adapters/models/t5/adapter_model.py` & `adapters-0.2.0/src/adapters/models/t5/adapter_model.py`

 * *Files identical despite different names*

### Comparing `adapters-0.1.2/src/adapters/models/t5/mixin_t5.py` & `adapters-0.2.0/src/adapters/models/t5/mixin_t5.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,47 +9,51 @@
 from ...model_mixin import (
     EmbeddingAdaptersMixin,
     InvertibleAdaptersMixin,
     InvertibleAdaptersWrapperMixin,
     ModelBaseAdaptersMixin,
     ModelWithHeadsAdaptersMixin,
 )
+from ...utils import patch_forward
 
 
 class T5AttentionAdaptersMixin:
     """Adds adapters to the T5Attention module."""
 
     def init_adapters(self, model_config, adapters_config):
         # Wrap layers for LoRA
         self.q = LoRALinear.wrap(self.q, "selfattn", model_config, adapters_config, attn_key="q", bias=False)
         self.k = LoRALinear.wrap(self.k, "selfattn", model_config, adapters_config, attn_key="k", bias=False)
         self.v = LoRALinear.wrap(self.v, "selfattn", model_config, adapters_config, attn_key="v", bias=False)
 
         self.prefix_tuning = PrefixTuningLayer(
             self.location_key + "_prefix" if self.location_key else None, model_config, adapters_config
         )
+        patch_forward(self)
 
 
 class T5SelfAttentionLayerAdaptersMixin(BottleneckLayer):
     def __init__(self):
         super().__init__("mh_adapter", None)
 
     def init_adapters(self, model_config, adapters_config):
         self.location_key = "mh_adapter"
         super().init_adapters(model_config, adapters_config)
+        patch_forward(self)
 
 
 class T5CrossAttentionLayerAdaptersMixin(BottleneckLayer):
     def __init__(self):
         super().__init__("cross_adapter", None)
 
     def init_adapters(self, model_config, adapters_config):
         self.location_key = "cross_adapter"
         self.EncDecAttention.location_key = "cross"
         super().init_adapters(model_config, adapters_config)
+        patch_forward(self)
 
 
 class T5FFLayerAdaptersMixin(BottleneckLayer):
     def __init__(self):
         super().__init__("output_adapter", None)
 
     def init_adapters(self, model_config, adapters_config):
@@ -78,14 +82,15 @@
 
 class T5StackAdaptersMixin(InvertibleAdaptersMixin):
     """Adds adapters to the T5Stack module."""
 
     def init_adapters(self, model_config, adapters_config):
         if not self.is_decoder:
             InvertibleAdaptersMixin.init_adapters(self, self.config, adapters_config)
+        patch_forward(self)
 
     def post_embedding_forward(self, embedding_output):
         embedding_output = self.invertible_adapters_forward(embedding_output)
         # Prompt tuning not yet supported
         return embedding_output
```

### Comparing `adapters-0.1.2/src/adapters/models/t5/modeling_t5.py` & `adapters-0.2.0/src/adapters/models/t5/modeling_t5.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,15 @@
         batch_size, seq_length = hidden_states.shape[:2]
 
         real_seq_length = seq_length
 
         if past_key_value is not None:
             assert (
                 len(past_key_value) == 2
-            ), f"past_key_value should have 2 past states: keys and values. Got { len(past_key_value)} past states"
+            ), f"past_key_value should have 2 past states: keys and values. Got {len(past_key_value)} past states"
             real_seq_length += past_key_value[0].shape[2] if query_length is None else query_length
 
         key_length = real_seq_length if key_value_states is None else key_value_states.shape[1]
 
         def shape(states):
             """projection"""
             return states.view(batch_size, -1, self.n_heads, self.key_value_proj_dim).transpose(1, 2)
@@ -140,15 +140,21 @@
         batch_size, key_length = key_states.shape[0], key_states.shape[2]
 
         # compute scores
         scores = torch.matmul(
             query_states, key_states.transpose(3, 2)
         )  # equivalent of torch.einsum("bnqd,bnkd->bnqk", query_states, key_states), compatible with onnx op>9
 
-        if position_bias is None:
+        # For Prefix Tuning, when training with AdapterDrop, we must additionally check that the sequence lengths of
+        # both positional encoding and the scores account for the prefix tokens.
+        # This is because the positional encoding is calculated only once in the beginning and then used for all layers.
+        # However, if the encoding was calculated without the prefix tokens due to AdapterDrop having dropped an
+        # adapter layer in the beginning, the positional encoding will be shorter than the scores, resulting in a
+        # dimension mismatch when adding the positional encoding to the scores.
+        if position_bias is None or position_bias.shape[3] != scores.shape[3]:
             if not self.has_relative_attention_bias:
                 position_bias = torch.zeros(
                     (1, self.n_heads, real_seq_length, key_length), device=scores.device, dtype=scores.dtype
                 )
                 if self.gradient_checkpointing and self.training:
                     position_bias.requires_grad = True
             else:
```

### Comparing `adapters-0.1.2/src/adapters/models/vit/__init__.py` & `adapters-0.2.0/src/adapters/models/vit/__init__.py`

 * *Files identical despite different names*

### Comparing `adapters-0.1.2/src/adapters/models/vit/adapter_model.py` & `adapters-0.2.0/src/adapters/models/vit/adapter_model.py`

 * *Files identical despite different names*

### Comparing `adapters-0.1.2/src/adapters/models/vit/modeling_vit.py` & `adapters-0.2.0/src/adapters/models/vit/modeling_vit.py`

 * *Files identical despite different names*

### Comparing `adapters-0.1.2/src/adapters/models/xlm_roberta/__init__.py` & `adapters-0.2.0/src/adapters/models/xlm_roberta/__init__.py`

 * *Files identical despite different names*

### Comparing `adapters-0.1.2/src/adapters/models/xlm_roberta/adapter_model.py` & `adapters-0.2.0/src/adapters/models/xlm_roberta/adapter_model.py`

 * *Files identical despite different names*

### Comparing `adapters-0.1.2/src/adapters/models/xlm_roberta/modeling_xlm_roberta.py` & `adapters-0.2.0/src/adapters/models/xlm_roberta/modeling_xlm_roberta.py`

 * *Files identical despite different names*

### Comparing `adapters-0.1.2/src/adapters/models/xmod/__init__.py` & `adapters-0.2.0/src/adapters/models/xmod/__init__.py`

 * *Files identical despite different names*

### Comparing `adapters-0.1.2/src/adapters/models/xmod/adapter_model.py` & `adapters-0.2.0/src/adapters/models/xmod/adapter_model.py`

 * *Files identical despite different names*

### Comparing `adapters-0.1.2/src/adapters/models/xmod/mixin_xmod.py` & `adapters-0.2.0/src/adapters/models/xmod/mixin_xmod.py`

 * *Files identical despite different names*

### Comparing `adapters-0.1.2/src/adapters/models/xmod/modeling_xmod.py` & `adapters-0.2.0/src/adapters/models/xmod/modeling_xmod.py`

 * *Files identical despite different names*

### Comparing `adapters-0.1.2/src/adapters/trainer.py` & `adapters-0.2.0/src/adapters/trainer.py`

 * *Files identical despite different names*

### Comparing `adapters-0.1.2/src/adapters/training.py` & `adapters-0.2.0/src/adapters/training.py`

 * *Files identical despite different names*

### Comparing `adapters-0.1.2/src/adapters/utils.py` & `adapters-0.2.0/src/adapters/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,14 @@
     EntryNotFoundError,
     RepositoryNotFoundError,
     RevisionNotFoundError,
     hf_raise_for_status,
 )
 from requests.exceptions import HTTPError
 from transformers.utils import http_user_agent, is_remote_url
-from transformers.utils.hub import torch_cache_home
 
 from . import __version__
 from .context import ForwardContext
 
 
 logger = logging.getLogger(__name__)
 
@@ -55,14 +54,17 @@
 ADAPTER_HUB_URL = "https://raw.githubusercontent.com/Adapter-Hub/Hub/master/dist/v2/"
 ADAPTER_HUB_INDEX_FILE = ADAPTER_HUB_URL + "index/{}.json"
 ADAPTER_HUB_CONFIG_FILE = ADAPTER_HUB_URL + "architectures.json"
 ADAPTER_HUB_ALL_FILE = ADAPTER_HUB_URL + "all.json"
 ADAPTER_HUB_ADAPTER_ENTRY_JSON = ADAPTER_HUB_URL + "adapters/{}/{}.json"
 
 # the download cache
+torch_cache_home = os.getenv(
+    "TORCH_HOME", os.path.join(os.getenv("XDG_CACHE_HOME", os.path.expanduser("~/.cache")), "torch")
+)
 ADAPTER_CACHE = join(torch_cache_home, "adapters")
 
 # these keys are ignored when calculating the config hash
 ADAPTER_CONFIG_HASH_IGNORE = []
 
 # old: new
 ACTIVATION_RENAME = {
@@ -713,23 +715,23 @@
         return pull_from_hub(
             adapter_name_or_path, model_name, adapter_config=adapter_config, version=version, **kwargs
         )
     elif source == "hf":
         return pull_from_hf_model_hub(adapter_name_or_path, version=version, **kwargs)
     elif source is None:
         try:
-            logger.info("Attempting to load adapter from source 'ah'...")
-            return pull_from_hub(
-                adapter_name_or_path, model_name, adapter_config=adapter_config, version=version, **kwargs
-            )
-        except EnvironmentError as ex:
-            logger.info(ex)
             logger.info("Attempting to load adapter from source 'hf'...")
+            return pull_from_hf_model_hub(adapter_name_or_path, version=version, **kwargs)
+        except (EnvironmentError, ValueError) as ex:
+            logger.info(ex)
+            logger.info("Attempting to load adapter from source 'ah'...")
             try:
-                return pull_from_hf_model_hub(adapter_name_or_path, version=version, **kwargs)
+                return pull_from_hub(
+                    adapter_name_or_path, model_name, adapter_config=adapter_config, version=version, **kwargs
+                )
             except Exception as ex:
                 logger.info(ex)
                 raise EnvironmentError(
                     "Unable to load adapter {} from any source. Please check the name of the adapter or the source."
                     .format(adapter_name_or_path)
                 )
     else:
@@ -833,16 +835,16 @@
             The attention mask to add the prefix to.
         dim (int):
             The dimension along which to concatenate the prefix_attention_mask. Defaults to 3.
         prefix_value (int):
             The value to use for the prefix_attention_mask. Defaults to 0, however some models, e.g. DistilBert, use
             different values. BERT like models invert their extended_attention_mask, hence they use 0 as value for not
             masked tokens. This inversion is usually done in the forward method of the model in 2 different ways:
-                1) by calling self.invert_attention_mask, as BERT does 2) by doing the inversion manually, e.g. ALBERT
-                does: `extended_attention_mask = (1.0 - extended_attention_mask) * torch.finfo(self.dtype).min`
+            1) by calling self.invert_attention_mask, as BERT does 2) by doing the inversion manually, e.g. ALBERT
+            does: `extended_attention_mask = (1.0 - extended_attention_mask) * torch.finfo(self.dtype).min`
     """
 
     forward_context = ForwardContext.get_context()
 
     if (
         attention_mask is not None
         and forward_context is not None
@@ -858,7 +860,16 @@
             dtype=attention_mask.dtype,
         ).to(attention_mask.device)
 
         # Concatenate the prefix_attention_mask along the specified dimension
         attention_mask = torch.cat((prefix_attention_mask, attention_mask), dim=dim)
 
     return attention_mask
+
+
+def patch_forward(module: torch.nn.Module):
+    # HF Accelerate's `add_hook_to_module()` replaces the module forward method with a wrapper
+    # and stores the original forward method in `_old_forward`. For this to work with Adapters' post-hook wrapping,
+    # we need to explicitly set to potentially overriden forward methods on adapter init.
+    # The `add_hook_to_module()` method is e.g. used for `device_map="auto"` in the `PreTrainedModel.from_pretrained()` method.
+    if hasattr(module, "_old_forward"):
+        module._old_forward = module.__class__.forward.__get__(module, module.__class__)
```

### Comparing `adapters-0.1.2/src/adapters/wrappers/__init__.py` & `adapters-0.2.0/src/adapters/wrappers/__init__.py`

 * *Files identical despite different names*

### Comparing `adapters-0.1.2/src/adapters/wrappers/configuration.py` & `adapters-0.2.0/src/adapters/wrappers/configuration.py`

 * *Files identical despite different names*

### Comparing `adapters-0.1.2/src/adapters/wrappers/model.py` & `adapters-0.2.0/src/adapters/wrappers/model.py`

 * *Files identical despite different names*

### Comparing `adapters-0.1.2/src/adapters.egg-info/PKG-INFO` & `adapters-0.2.0/src/adapters.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,682 +1,716 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310d 0a4e 616d 653a 2061 6461  : 2.1..Name: ada
 00000020: 7074 6572 730d 0a56 6572 7369 6f6e 3a20  pters..Version: 
-00000030: 302e 312e 320d 0a53 756d 6d61 7279 3a20  0.1.2..Summary: 
+00000030: 302e 322e 300d 0a53 756d 6d61 7279 3a20  0.2.0..Summary: 
 00000040: 4120 556e 6966 6965 6420 4c69 6272 6172  A Unified Librar
 00000050: 7920 666f 7220 5061 7261 6d65 7465 722d  y for Parameter-
 00000060: 4566 6669 6369 656e 7420 616e 6420 4d6f  Efficient and Mo
 00000070: 6475 6c61 7220 5472 616e 7366 6572 204c  dular Transfer L
 00000080: 6561 726e 696e 670d 0a48 6f6d 652d 7061  earning..Home-pa
 00000090: 6765 3a20 6874 7470 733a 2f2f 6769 7468  ge: https://gith
 000000a0: 7562 2e63 6f6d 2f61 6461 7074 6572 2d68  ub.com/adapter-h
 000000b0: 7562 2f61 6461 7074 6572 730d 0a41 7574  ub/adapters..Aut
 000000c0: 686f 723a 2054 6865 2041 6461 7074 6572  hor: The Adapter
 000000d0: 4875 6220 7465 616d 2061 6e64 2063 6f6d  Hub team and com
 000000e0: 6d75 6e69 7479 2063 6f6e 7472 6962 7574  munity contribut
 000000f0: 6f72 730d 0a41 7574 686f 722d 656d 6169  ors..Author-emai
-00000100: 6c3a 2070 6665 6966 6665 7240 756b 702e  l: pfeiffer@ukp.
-00000110: 7475 2d64 6172 6d73 7461 6474 2e64 650d  tu-darmstadt.de.
-00000120: 0a4c 6963 656e 7365 3a20 4170 6163 6865  .License: Apache
-00000130: 0d0a 4b65 7977 6f72 6473 3a20 4e4c 5020  ..Keywords: NLP 
-00000140: 6465 6570 206c 6561 726e 696e 6720 7472  deep learning tr
-00000150: 616e 7366 6f72 6d65 7220 7079 746f 7263  ansformer pytorc
-00000160: 6820 4245 5254 2061 6461 7074 6572 730d  h BERT adapters.
-00000170: 0a43 6c61 7373 6966 6965 723a 2044 6576  .Classifier: Dev
-00000180: 656c 6f70 6d65 6e74 2053 7461 7475 7320  elopment Status 
-00000190: 3a3a 2034 202d 2042 6574 610d 0a43 6c61  :: 4 - Beta..Cla
-000001a0: 7373 6966 6965 723a 2049 6e74 656e 6465  ssifier: Intende
-000001b0: 6420 4175 6469 656e 6365 203a 3a20 4465  d Audience :: De
-000001c0: 7665 6c6f 7065 7273 0d0a 436c 6173 7369  velopers..Classi
-000001d0: 6669 6572 3a20 496e 7465 6e64 6564 2041  fier: Intended A
-000001e0: 7564 6965 6e63 6520 3a3a 2045 6475 6361  udience :: Educa
-000001f0: 7469 6f6e 0d0a 436c 6173 7369 6669 6572  tion..Classifier
-00000200: 3a20 496e 7465 6e64 6564 2041 7564 6965  : Intended Audie
-00000210: 6e63 6520 3a3a 2053 6369 656e 6365 2f52  nce :: Science/R
-00000220: 6573 6561 7263 680d 0a43 6c61 7373 6966  esearch..Classif
-00000230: 6965 723a 204c 6963 656e 7365 203a 3a20  ier: License :: 
-00000240: 4f53 4920 4170 7072 6f76 6564 203a 3a20  OSI Approved :: 
-00000250: 4170 6163 6865 2053 6f66 7477 6172 6520  Apache Software 
-00000260: 4c69 6365 6e73 650d 0a43 6c61 7373 6966  License..Classif
-00000270: 6965 723a 204f 7065 7261 7469 6e67 2053  ier: Operating S
-00000280: 7973 7465 6d20 3a3a 204f 5320 496e 6465  ystem :: OS Inde
-00000290: 7065 6e64 656e 740d 0a43 6c61 7373 6966  pendent..Classif
-000002a0: 6965 723a 2050 726f 6772 616d 6d69 6e67  ier: Programming
-000002b0: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
-000002c0: 686f 6e20 3a3a 2033 0d0a 436c 6173 7369  hon :: 3..Classi
-000002d0: 6669 6572 3a20 5072 6f67 7261 6d6d 696e  fier: Programmin
-000002e0: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
-000002f0: 7468 6f6e 203a 3a20 332e 380d 0a43 6c61  thon :: 3.8..Cla
-00000300: 7373 6966 6965 723a 2050 726f 6772 616d  ssifier: Program
-00000310: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
-00000320: 2050 7974 686f 6e20 3a3a 2033 2e39 0d0a   Python :: 3.9..
-00000330: 436c 6173 7369 6669 6572 3a20 5072 6f67  Classifier: Prog
-00000340: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
-00000350: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
-00000360: 3130 0d0a 436c 6173 7369 6669 6572 3a20  10..Classifier: 
-00000370: 546f 7069 6320 3a3a 2053 6369 656e 7469  Topic :: Scienti
-00000380: 6669 632f 456e 6769 6e65 6572 696e 6720  fic/Engineering 
-00000390: 3a3a 2041 7274 6966 6963 6961 6c20 496e  :: Artificial In
-000003a0: 7465 6c6c 6967 656e 6365 0d0a 5265 7175  telligence..Requ
-000003b0: 6972 6573 2d50 7974 686f 6e3a 203e 3d33  ires-Python: >=3
-000003c0: 2e38 2e30 0d0a 4465 7363 7269 7074 696f  .8.0..Descriptio
-000003d0: 6e2d 436f 6e74 656e 742d 5479 7065 3a20  n-Content-Type: 
-000003e0: 7465 7874 2f6d 6172 6b64 6f77 6e0d 0a50  text/markdown..P
-000003f0: 726f 7669 6465 732d 4578 7472 613a 2073  rovides-Extra: s
-00000400: 6b6c 6561 726e 0d0a 5072 6f76 6964 6573  klearn..Provides
-00000410: 2d45 7874 7261 3a20 746f 7263 680d 0a50  -Extra: torch..P
-00000420: 726f 7669 6465 732d 4578 7472 613a 206f  rovides-Extra: o
-00000430: 6e6e 7872 756e 7469 6d65 0d0a 5072 6f76  nnxruntime..Prov
-00000440: 6964 6573 2d45 7874 7261 3a20 7365 6e74  ides-Extra: sent
-00000450: 656e 6365 7069 6563 650d 0a50 726f 7669  encepiece..Provi
-00000460: 6465 732d 4578 7472 613a 2074 6573 7469  des-Extra: testi
-00000470: 6e67 0d0a 5072 6f76 6964 6573 2d45 7874  ng..Provides-Ext
-00000480: 7261 3a20 7175 616c 6974 790d 0a50 726f  ra: quality..Pro
-00000490: 7669 6465 732d 4578 7472 613a 2064 6f63  vides-Extra: doc
-000004a0: 730d 0a50 726f 7669 6465 732d 4578 7472  s..Provides-Extr
-000004b0: 613a 2064 6576 0d0a 4c69 6365 6e73 652d  a: dev..License-
-000004c0: 4669 6c65 3a20 4c49 4345 4e53 450d 0a0d  File: LICENSE...
-000004d0: 0a3c 212d 2d2d 0d0a 436f 7079 7269 6768  .<!---..Copyrigh
-000004e0: 7420 3230 3230 2054 6865 2041 6461 7074  t 2020 The Adapt
-000004f0: 6572 4875 6220 5465 616d 2e20 416c 6c20  erHub Team. All 
-00000500: 7269 6768 7473 2072 6573 6572 7665 642e  rights reserved.
-00000510: 0d0a 0d0a 4c69 6365 6e73 6564 2075 6e64  ....Licensed und
-00000520: 6572 2074 6865 2041 7061 6368 6520 4c69  er the Apache Li
-00000530: 6365 6e73 652c 2056 6572 7369 6f6e 2032  cense, Version 2
-00000540: 2e30 2028 7468 6520 224c 6963 656e 7365  .0 (the "License
-00000550: 2229 3b0d 0a79 6f75 206d 6179 206e 6f74  ");..you may not
-00000560: 2075 7365 2074 6869 7320 6669 6c65 2065   use this file e
-00000570: 7863 6570 7420 696e 2063 6f6d 706c 6961  xcept in complia
-00000580: 6e63 6520 7769 7468 2074 6865 204c 6963  nce with the Lic
-00000590: 656e 7365 2e0d 0a59 6f75 206d 6179 206f  ense...You may o
-000005a0: 6274 6169 6e20 6120 636f 7079 206f 6620  btain a copy of 
-000005b0: 7468 6520 4c69 6365 6e73 6520 6174 0d0a  the License at..
-000005c0: 0d0a 2020 2020 6874 7470 3a2f 2f77 7777  ..    http://www
-000005d0: 2e61 7061 6368 652e 6f72 672f 6c69 6365  .apache.org/lice
-000005e0: 6e73 6573 2f4c 4943 454e 5345 2d32 2e30  nses/LICENSE-2.0
-000005f0: 0d0a 0d0a 556e 6c65 7373 2072 6571 7569  ....Unless requi
-00000600: 7265 6420 6279 2061 7070 6c69 6361 626c  red by applicabl
-00000610: 6520 6c61 7720 6f72 2061 6772 6565 6420  e law or agreed 
-00000620: 746f 2069 6e20 7772 6974 696e 672c 2073  to in writing, s
-00000630: 6f66 7477 6172 650d 0a64 6973 7472 6962  oftware..distrib
-00000640: 7574 6564 2075 6e64 6572 2074 6865 204c  uted under the L
-00000650: 6963 656e 7365 2069 7320 6469 7374 7269  icense is distri
-00000660: 6275 7465 6420 6f6e 2061 6e20 2241 5320  buted on an "AS 
-00000670: 4953 2220 4241 5349 532c 0d0a 5749 5448  IS" BASIS,..WITH
-00000680: 4f55 5420 5741 5252 414e 5449 4553 204f  OUT WARRANTIES O
-00000690: 5220 434f 4e44 4954 494f 4e53 204f 4620  R CONDITIONS OF 
-000006a0: 414e 5920 4b49 4e44 2c20 6569 7468 6572  ANY KIND, either
-000006b0: 2065 7870 7265 7373 206f 7220 696d 706c   express or impl
-000006c0: 6965 642e 0d0a 5365 6520 7468 6520 4c69  ied...See the Li
-000006d0: 6365 6e73 6520 666f 7220 7468 6520 7370  cense for the sp
-000006e0: 6563 6966 6963 206c 616e 6775 6167 6520  ecific language 
-000006f0: 676f 7665 726e 696e 6720 7065 726d 6973  governing permis
-00000700: 7369 6f6e 7320 616e 640d 0a6c 696d 6974  sions and..limit
-00000710: 6174 696f 6e73 2075 6e64 6572 2074 6865  ations under the
-00000720: 204c 6963 656e 7365 2e0d 0a2d 2d3e 0d0a   License...-->..
-00000730: 0d0a 3e20 2a2a 4e6f 7465 2a2a 3a20 5468  ..> **Note**: Th
-00000740: 6973 2072 6570 6f73 6974 6f72 7920 686f  is repository ho
-00000750: 6c64 7320 7468 6520 636f 6465 6261 7365  lds the codebase
-00000760: 206f 6620 7468 6520 5f41 6461 7074 6572   of the _Adapter
-00000770: 735f 206c 6962 7261 7279 2c20 7768 6963  s_ library, whic
-00000780: 6820 6861 7320 7265 706c 6163 6564 2060  h has replaced `
-00000790: 6164 6170 7465 722d 7472 616e 7366 6f72  adapter-transfor
-000007a0: 6d65 7273 602e 2046 6f72 2074 6865 206c  mers`. For the l
-000007b0: 6567 6163 7920 636f 6465 6261 7365 2c20  egacy codebase, 
-000007c0: 676f 2074 6f3a 2068 7474 7073 3a2f 2f67  go to: https://g
-000007d0: 6974 6875 622e 636f 6d2f 6164 6170 7465  ithub.com/adapte
-000007e0: 722d 6875 622f 6164 6170 7465 722d 7472  r-hub/adapter-tr
-000007f0: 616e 7366 6f72 6d65 7273 2d6c 6567 6163  ansformers-legac
-00000800: 792e 0d0a 0d0a 3c70 2061 6c69 676e 3d22  y.....<p align="
-00000810: 6365 6e74 6572 223e 0d0a 3c69 6d67 2073  center">..<img s
-00000820: 7479 6c65 3d22 7665 7274 6963 616c 2d61  tyle="vertical-a
-00000830: 6c69 676e 3a6d 6964 646c 6522 2073 7263  lign:middle" src
-00000840: 3d22 6874 7470 733a 2f2f 7261 772e 6769  ="https://raw.gi
-00000850: 7468 7562 7573 6572 636f 6e74 656e 742e  thubusercontent.
-00000860: 636f 6d2f 4164 6170 7465 722d 4875 622f  com/Adapter-Hub/
-00000870: 6164 6170 7465 7273 2f6d 6169 6e2f 646f  adapters/main/do
-00000880: 6373 2f6c 6f67 6f2e 706e 6722 202f 3e0d  cs/logo.png" />.
-00000890: 0a3c 2f70 3e0d 0a3c 6831 2061 6c69 676e  .</p>..<h1 align
-000008a0: 3d22 6365 6e74 6572 223e 0d0a 3c73 7061  ="center">..<spa
-000008b0: 6e3e 3c69 3e41 6461 7074 6572 733c 2f69  n><i>Adapters</i
-000008c0: 3e3c 2f73 7061 6e3e 0d0a 3c2f 6831 3e0d  ></span>..</h1>.
-000008d0: 0a0d 0a3c 6833 2061 6c69 676e 3d22 6365  ...<h3 align="ce
-000008e0: 6e74 6572 223e 0d0a 4120 556e 6966 6965  nter">..A Unifie
-000008f0: 6420 4c69 6272 6172 7920 666f 7220 5061  d Library for Pa
-00000900: 7261 6d65 7465 722d 4566 6669 6369 656e  rameter-Efficien
-00000910: 7420 616e 6420 4d6f 6475 6c61 7220 5472  t and Modular Tr
-00000920: 616e 7366 6572 204c 6561 726e 696e 670d  ansfer Learning.
-00000930: 0a3c 2f68 333e 0d0a 0d0a 215b 5465 7374  .</h3>....![Test
-00000940: 735d 2868 7474 7073 3a2f 2f67 6974 6875  s](https://githu
-00000950: 622e 636f 6d2f 4164 6170 7465 722d 4875  b.com/Adapter-Hu
-00000960: 622f 6164 6170 7465 7273 2f77 6f72 6b66  b/adapters/workf
-00000970: 6c6f 7773 2f54 6573 7473 2f62 6164 6765  lows/Tests/badge
-00000980: 2e73 7667 3f62 7261 6e63 683d 6164 6170  .svg?branch=adap
-00000990: 7465 7273 290d 0a5b 215b 4769 7448 7562  ters)..[![GitHub
-000009a0: 5d28 6874 7470 733a 2f2f 696d 672e 7368  ](https://img.sh
-000009b0: 6965 6c64 732e 696f 2f67 6974 6875 622f  ields.io/github/
-000009c0: 6c69 6365 6e73 652f 6164 6170 7465 722d  license/adapter-
-000009d0: 6875 622f 6164 6170 7465 7273 2e73 7667  hub/adapters.svg
-000009e0: 3f63 6f6c 6f72 3d62 6c75 6529 5d28 6874  ?color=blue)](ht
-000009f0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000a00: 2f61 6461 7074 6572 2d68 7562 2f61 6461  /adapter-hub/ada
-00000a10: 7074 6572 732f 626c 6f62 2f6d 6169 6e2f  pters/blob/main/
-00000a20: 4c49 4345 4e53 4529 0d0a 5b21 5b50 7950  LICENSE)..[![PyP
-00000a30: 495d 2868 7474 7073 3a2f 2f69 6d67 2e73  I](https://img.s
-00000a40: 6869 656c 6473 2e69 6f2f 7079 7069 2f76  hields.io/pypi/v
-00000a50: 2f61 6461 7074 6572 7329 5d28 6874 7470  /adapters)](http
-00000a60: 733a 2f2f 7079 7069 2e6f 7267 2f70 726f  s://pypi.org/pro
-00000a70: 6a65 6374 2f61 6461 7074 6572 732f 290d  ject/adapters/).
-00000a80: 0a0d 0a60 6164 6170 7465 7273 6020 6973  ...`adapters` is
-00000a90: 2061 6e20 6164 642d 6f6e 2074 6f20 5b48   an add-on to [H
-00000aa0: 7567 6769 6e67 4661 6365 2773 2054 7261  uggingFace's Tra
-00000ab0: 6e73 666f 726d 6572 735d 2868 7474 7073  nsformers](https
-00000ac0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6875  ://github.com/hu
-00000ad0: 6767 696e 6766 6163 652f 7472 616e 7366  ggingface/transf
-00000ae0: 6f72 6d65 7273 2920 6c69 6272 6172 792c  ormers) library,
-00000af0: 2069 6e74 6567 7261 7469 6e67 2061 6461   integrating ada
-00000b00: 7074 6572 7320 696e 746f 2073 7461 7465  pters into state
-00000b10: 2d6f 662d 7468 652d 6172 7420 6c61 6e67  -of-the-art lang
-00000b20: 7561 6765 206d 6f64 656c 7320 6279 2069  uage models by i
-00000b30: 6e63 6f72 706f 7261 7469 6e67 202a 2a5b  ncorporating **[
-00000b40: 4164 6170 7465 7248 7562 5d28 6874 7470  AdapterHub](http
-00000b50: 733a 2f2f 6164 6170 7465 7268 7562 2e6d  s://adapterhub.m
-00000b60: 6c29 2a2a 2c20 6120 6365 6e74 7261 6c20  l)**, a central 
-00000b70: 7265 706f 7369 746f 7279 2066 6f72 2070  repository for p
-00000b80: 7265 2d74 7261 696e 6564 2061 6461 7074  re-trained adapt
-00000b90: 6572 206d 6f64 756c 6573 2e0d 0a0d 0a23  er modules.....#
-00000ba0: 2320 496e 7374 616c 6c61 7469 6f6e 0d0a  # Installation..
-00000bb0: 0d0a 6061 6461 7074 6572 7360 2063 7572  ..`adapters` cur
-00000bc0: 7265 6e74 6c79 2073 7570 706f 7274 7320  rently supports 
-00000bd0: 2a2a 5079 7468 6f6e 2033 2e38 2b2a 2a20  **Python 3.8+** 
-00000be0: 616e 6420 2a2a 5079 546f 7263 6820 312e  and **PyTorch 1.
-00000bf0: 3130 2b2a 2a2e 0d0a 4166 7465 7220 5b69  10+**...After [i
-00000c00: 6e73 7461 6c6c 696e 6720 5079 546f 7263  nstalling PyTorc
-00000c10: 685d 2868 7474 7073 3a2f 2f70 7974 6f72  h](https://pytor
-00000c20: 6368 2e6f 7267 2f67 6574 2d73 7461 7274  ch.org/get-start
-00000c30: 6564 2f6c 6f63 616c 6c79 2f29 2c20 796f  ed/locally/), yo
-00000c40: 7520 6361 6e20 696e 7374 616c 6c20 6061  u can install `a
-00000c50: 6461 7074 6572 7360 2066 726f 6d20 5079  dapters` from Py
-00000c60: 5049 202e 2e2e 0d0a 0d0a 6060 600d 0a70  PI .......```..p
-00000c70: 6970 2069 6e73 7461 6c6c 202d 5520 6164  ip install -U ad
-00000c80: 6170 7465 7273 0d0a 6060 600d 0a0d 0a2e  apters..```.....
-00000c90: 2e2e 206f 7220 6672 6f6d 2073 6f75 7263  .. or from sourc
-00000ca0: 6520 6279 2063 6c6f 6e69 6e67 2074 6865  e by cloning the
-00000cb0: 2072 6570 6f73 6974 6f72 793a 0d0a 0d0a   repository:....
-00000cc0: 6060 600d 0a67 6974 2063 6c6f 6e65 2068  ```..git clone h
-00000cd0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000ce0: 6d2f 6164 6170 7465 722d 6875 622f 6164  m/adapter-hub/ad
-00000cf0: 6170 7465 7273 2e67 6974 0d0a 6364 2061  apters.git..cd a
-00000d00: 6461 7074 6572 730d 0a70 6970 2069 6e73  dapters..pip ins
-00000d10: 7461 6c6c 202e 0d0a 6060 600d 0a0d 0a23  tall ...```....#
-00000d20: 2320 5175 6963 6b20 546f 7572 0d0a 0d0a  # Quick Tour....
-00000d30: 2323 2323 204c 6f61 6420 7072 652d 7472  #### Load pre-tr
-00000d40: 6169 6e65 6420 6164 6170 7465 7273 3a0d  ained adapters:.
-00000d50: 0a0d 0a60 6060 7079 7468 6f6e 0d0a 6672  ...```python..fr
-00000d60: 6f6d 2061 6461 7074 6572 7320 696d 706f  om adapters impo
-00000d70: 7274 2041 7574 6f41 6461 7074 6572 4d6f  rt AutoAdapterMo
-00000d80: 6465 6c0d 0a66 726f 6d20 7472 616e 7366  del..from transf
-00000d90: 6f72 6d65 7273 2069 6d70 6f72 7420 4175  ormers import Au
-00000da0: 746f 546f 6b65 6e69 7a65 720d 0a0d 0a6d  toTokenizer....m
-00000db0: 6f64 656c 203d 2041 7574 6f41 6461 7074  odel = AutoAdapt
-00000dc0: 6572 4d6f 6465 6c2e 6672 6f6d 5f70 7265  erModel.from_pre
-00000dd0: 7472 6169 6e65 6428 2272 6f62 6572 7461  trained("roberta
-00000de0: 2d62 6173 6522 290d 0a74 6f6b 656e 697a  -base")..tokeniz
-00000df0: 6572 203d 2041 7574 6f54 6f6b 656e 697a  er = AutoTokeniz
-00000e00: 6572 2e66 726f 6d5f 7072 6574 7261 696e  er.from_pretrain
-00000e10: 6564 2822 726f 6265 7274 612d 6261 7365  ed("roberta-base
-00000e20: 2229 0d0a 0d0a 6d6f 6465 6c2e 6c6f 6164  ")....model.load
-00000e30: 5f61 6461 7074 6572 2822 4164 6170 7465  _adapter("Adapte
-00000e40: 7248 7562 2f72 6f62 6572 7461 2d62 6173  rHub/roberta-bas
-00000e50: 652d 7066 2d69 6d64 6222 2c20 736f 7572  e-pf-imdb", sour
-00000e60: 6365 3d22 6866 222c 2073 6574 5f61 6374  ce="hf", set_act
-00000e70: 6976 653d 5472 7565 290d 0a0d 0a70 7269  ive=True)....pri
-00000e80: 6e74 286d 6f64 656c 282a 2a74 6f6b 656e  nt(model(**token
-00000e90: 697a 6572 2822 5468 6973 2077 6f72 6b73  izer("This works
-00000ea0: 2067 7265 6174 2122 2c20 7265 7475 726e   great!", return
-00000eb0: 5f74 656e 736f 7273 3d22 7074 2229 292e  _tensors="pt")).
-00000ec0: 6c6f 6769 7473 290d 0a60 6060 0d0a 0d0a  logits)..```....
-00000ed0: 2a2a 5b4c 6561 726e 204d 6f72 655d 2868  **[Learn More](h
-00000ee0: 7474 7073 3a2f 2f64 6f63 732e 6164 6170  ttps://docs.adap
-00000ef0: 7465 7268 7562 2e6d 6c2f 6c6f 6164 696e  terhub.ml/loadin
-00000f00: 672e 6874 6d6c 292a 2a0d 0a0d 0a23 2323  g.html)**....###
-00000f10: 2320 4164 6170 7420 6578 6973 7469 6e67  # Adapt existing
-00000f20: 206d 6f64 656c 2073 6574 7570 733a 0d0a   model setups:..
-00000f30: 0d0a 6060 6070 7974 686f 6e0d 0a69 6d70  ..```python..imp
-00000f40: 6f72 7420 6164 6170 7465 7273 0d0a 6672  ort adapters..fr
-00000f50: 6f6d 2074 7261 6e73 666f 726d 6572 7320  om transformers 
-00000f60: 696d 706f 7274 2041 7574 6f4d 6f64 656c  import AutoModel
-00000f70: 466f 7253 6571 7565 6e63 6543 6c61 7373  ForSequenceClass
-00000f80: 6966 6963 6174 696f 6e0d 0a0d 0a6d 6f64  ification....mod
-00000f90: 656c 203d 2041 7574 6f4d 6f64 656c 466f  el = AutoModelFo
-00000fa0: 7253 6571 7565 6e63 6543 6c61 7373 6966  rSequenceClassif
-00000fb0: 6963 6174 696f 6e2e 6672 6f6d 5f70 7265  ication.from_pre
-00000fc0: 7472 6169 6e65 6428 2274 352d 6261 7365  trained("t5-base
-00000fd0: 2229 0d0a 0d0a 6164 6170 7465 7273 2e69  ")....adapters.i
-00000fe0: 6e69 7428 6d6f 6465 6c29 0d0a 0d0a 6d6f  nit(model)....mo
-00000ff0: 6465 6c2e 6164 645f 6164 6170 7465 7228  del.add_adapter(
-00001000: 226d 795f 6c6f 7261 5f61 6461 7074 6572  "my_lora_adapter
-00001010: 222c 2063 6f6e 6669 673d 226c 6f72 6122  ", config="lora"
-00001020: 290d 0a6d 6f64 656c 2e74 7261 696e 5f61  )..model.train_a
-00001030: 6461 7074 6572 2822 6d79 5f6c 6f72 615f  dapter("my_lora_
-00001040: 6164 6170 7465 7222 290d 0a0d 0a23 2059  adapter")....# Y
-00001050: 6f75 7220 7265 6775 6c61 7220 7472 6169  our regular trai
-00001060: 6e69 6e67 206c 6f6f 702e 2e2e 0d0a 6060  ning loop.....``
-00001070: 600d 0a0d 0a2a 2a5b 4c65 6172 6e20 4d6f  `....**[Learn Mo
-00001080: 7265 5d28 6874 7470 733a 2f2f 646f 6373  re](https://docs
-00001090: 2e61 6461 7074 6572 6875 622e 6d6c 2f71  .adapterhub.ml/q
-000010a0: 7569 636b 7374 6172 742e 6874 6d6c 292a  uickstart.html)*
-000010b0: 2a0d 0a0d 0a23 2323 2320 466c 6578 6962  *....#### Flexib
-000010c0: 6c79 2063 6f6e 6669 6775 7265 2061 6461  ly configure ada
-000010d0: 7074 6572 733a 0d0a 0d0a 6060 6070 7974  pters:....```pyt
-000010e0: 686f 6e0d 0a66 726f 6d20 6164 6170 7465  hon..from adapte
-000010f0: 7273 2069 6d70 6f72 7420 436f 6e66 6967  rs import Config
-00001100: 556e 696f 6e2c 2050 7265 6669 7854 756e  Union, PrefixTun
-00001110: 696e 6743 6f6e 6669 672c 2050 6172 426e  ingConfig, ParBn
-00001120: 436f 6e66 6967 2c20 4175 746f 4164 6170  Config, AutoAdap
-00001130: 7465 724d 6f64 656c 0d0a 0d0a 6d6f 6465  terModel....mode
-00001140: 6c20 3d20 4175 746f 4164 6170 7465 724d  l = AutoAdapterM
-00001150: 6f64 656c 2e66 726f 6d5f 7072 6574 7261  odel.from_pretra
-00001160: 696e 6564 2822 6d69 6372 6f73 6f66 742f  ined("microsoft/
-00001170: 6465 6265 7274 612d 7633 2d62 6173 6522  deberta-v3-base"
-00001180: 290d 0a0d 0a61 6461 7074 6572 5f63 6f6e  )....adapter_con
-00001190: 6669 6720 3d20 436f 6e66 6967 556e 696f  fig = ConfigUnio
-000011a0: 6e28 0d0a 2020 2020 5072 6566 6978 5475  n(..    PrefixTu
-000011b0: 6e69 6e67 436f 6e66 6967 2870 7265 6669  ningConfig(prefi
-000011c0: 785f 6c65 6e67 7468 3d32 3029 2c0d 0a20  x_length=20),.. 
-000011d0: 2020 2050 6172 426e 436f 6e66 6967 2872     ParBnConfig(r
-000011e0: 6564 7563 7469 6f6e 5f66 6163 746f 723d  eduction_factor=
-000011f0: 3429 2c0d 0a29 0d0a 6d6f 6465 6c2e 6164  4),..)..model.ad
-00001200: 645f 6164 6170 7465 7228 226d 795f 6164  d_adapter("my_ad
-00001210: 6170 7465 7222 2c20 636f 6e66 6967 3d61  apter", config=a
-00001220: 6461 7074 6572 5f63 6f6e 6669 672c 2073  dapter_config, s
-00001230: 6574 5f61 6374 6976 653d 5472 7565 290d  et_active=True).
-00001240: 0a60 6060 0d0a 0d0a 2a2a 5b4c 6561 726e  .```....**[Learn
-00001250: 204d 6f72 655d 2868 7474 7073 3a2f 2f64   More](https://d
-00001260: 6f63 732e 6164 6170 7465 7268 7562 2e6d  ocs.adapterhub.m
-00001270: 6c2f 6f76 6572 7669 6577 2e68 746d 6c29  l/overview.html)
-00001280: 2a2a 0d0a 0d0a 2323 2323 2045 6173 696c  **....#### Easil
-00001290: 7920 636f 6d70 6f73 6520 6164 6170 7465  y compose adapte
-000012a0: 7273 2069 6e20 6120 7369 6e67 6c65 206d  rs in a single m
-000012b0: 6f64 656c 3a0d 0a0d 0a60 6060 7079 7468  odel:....```pyth
-000012c0: 6f6e 0d0a 6672 6f6d 2061 6461 7074 6572  on..from adapter
-000012d0: 7320 696d 706f 7274 2041 6461 7074 6572  s import Adapter
-000012e0: 5365 7475 702c 2041 7574 6f41 6461 7074  Setup, AutoAdapt
-000012f0: 6572 4d6f 6465 6c0d 0a69 6d70 6f72 7420  erModel..import 
-00001300: 6164 6170 7465 7273 2e63 6f6d 706f 7369  adapters.composi
-00001310: 7469 6f6e 2061 7320 6163 0d0a 0d0a 6d6f  tion as ac....mo
-00001320: 6465 6c20 3d20 4175 746f 4164 6170 7465  del = AutoAdapte
-00001330: 724d 6f64 656c 2e66 726f 6d5f 7072 6574  rModel.from_pret
-00001340: 7261 696e 6564 2822 726f 6265 7274 612d  rained("roberta-
-00001350: 6261 7365 2229 0d0a 0d0a 7163 203d 206d  base")....qc = m
-00001360: 6f64 656c 2e6c 6f61 645f 6164 6170 7465  odel.load_adapte
-00001370: 7228 2241 6461 7074 6572 4875 622f 726f  r("AdapterHub/ro
-00001380: 6265 7274 612d 6261 7365 2d70 662d 7472  berta-base-pf-tr
-00001390: 6563 2229 0d0a 7365 6e74 203d 206d 6f64  ec")..sent = mod
-000013a0: 656c 2e6c 6f61 645f 6164 6170 7465 7228  el.load_adapter(
-000013b0: 2241 6461 7074 6572 4875 622f 726f 6265  "AdapterHub/robe
-000013c0: 7274 612d 6261 7365 2d70 662d 696d 6462  rta-base-pf-imdb
-000013d0: 2229 0d0a 0d0a 7769 7468 2041 6461 7074  ")....with Adapt
-000013e0: 6572 5365 7475 7028 6163 2e50 6172 616c  erSetup(ac.Paral
-000013f0: 6c65 6c28 7163 2c20 7365 6e74 2929 3a0d  lel(qc, sent)):.
-00001400: 0a20 2020 2070 7269 6e74 286d 6f64 656c  .    print(model
-00001410: 282a 2a74 6f6b 656e 697a 6572 2822 5768  (**tokenizer("Wh
-00001420: 6174 2069 7320 4164 6170 7465 7248 7562  at is AdapterHub
-00001430: 3f22 2c20 7265 7475 726e 5f74 656e 736f  ?", return_tenso
-00001440: 7273 3d22 7074 2229 2929 0d0a 6060 600d  rs="pt")))..```.
-00001450: 0a0d 0a2a 2a5b 4c65 6172 6e20 4d6f 7265  ...**[Learn More
-00001460: 5d28 6874 7470 733a 2f2f 646f 6373 2e61  ](https://docs.a
-00001470: 6461 7074 6572 6875 622e 6d6c 2f61 6461  dapterhub.ml/ada
-00001480: 7074 6572 5f63 6f6d 706f 7369 7469 6f6e  pter_composition
-00001490: 2e68 746d 6c29 2a2a 0d0a 0d0a 2323 2055  .html)**....## U
-000014a0: 7365 6675 6c20 5265 736f 7572 6365 730d  seful Resources.
-000014b0: 0a0d 0a48 7567 6769 6e67 4661 6365 2773  ...HuggingFace's
-000014c0: 2067 7265 6174 2064 6f63 756d 656e 7461   great documenta
-000014d0: 7469 6f6e 206f 6e20 6765 7474 696e 6720  tion on getting 
-000014e0: 7374 6172 7465 6420 7769 7468 205f 5472  started with _Tr
-000014f0: 616e 7366 6f72 6d65 7273 5f20 6361 6e20  ansformers_ can 
-00001500: 6265 2066 6f75 6e64 205b 6865 7265 5d28  be found [here](
-00001510: 6874 7470 733a 2f2f 6875 6767 696e 6766  https://huggingf
-00001520: 6163 652e 636f 2f74 7261 6e73 666f 726d  ace.co/transform
-00001530: 6572 732f 696e 6465 782e 6874 6d6c 292e  ers/index.html).
-00001540: 2060 6164 6170 7465 7273 6020 6973 2066   `adapters` is f
-00001550: 756c 6c79 2063 6f6d 7061 7469 626c 6520  ully compatible 
-00001560: 7769 7468 205f 5472 616e 7366 6f72 6d65  with _Transforme
-00001570: 7273 5f2e 0d0a 0d0a 546f 2067 6574 2073  rs_.....To get s
-00001580: 7461 7274 6564 2077 6974 6820 6164 6170  tarted with adap
-00001590: 7465 7273 2c20 7265 6665 7220 746f 2074  ters, refer to t
-000015a0: 6865 7365 206c 6f63 6174 696f 6e73 3a0d  hese locations:.
-000015b0: 0a0d 0a2d 202a 2a5b 436f 6c61 6220 6e6f  ...- **[Colab no
-000015c0: 7465 626f 6f6b 2074 7574 6f72 6961 6c73  tebook tutorials
-000015d0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-000015e0: 2e63 6f6d 2f41 6461 7074 6572 2d48 7562  .com/Adapter-Hub
-000015f0: 2f61 6461 7074 6572 732f 7472 6565 2f6d  /adapters/tree/m
-00001600: 6169 6e2f 6e6f 7465 626f 6f6b 7329 2a2a  ain/notebooks)**
-00001610: 2c20 6120 7365 7269 6573 206e 6f74 6562  , a series noteb
-00001620: 6f6f 6b73 2070 726f 7669 6469 6e67 2061  ooks providing a
-00001630: 6e20 696e 7472 6f64 7563 7469 6f6e 2074  n introduction t
-00001640: 6f20 616c 6c20 7468 6520 6d61 696e 2063  o all the main c
-00001650: 6f6e 6365 7074 7320 6f66 2028 6164 6170  oncepts of (adap
-00001660: 7465 722d 2974 7261 6e73 666f 726d 6572  ter-)transformer
-00001670: 7320 616e 6420 4164 6170 7465 7248 7562  s and AdapterHub
-00001680: 0d0a 2d20 2a2a 6874 7470 733a 2f2f 646f  ..- **https://do
-00001690: 6373 2e61 6461 7074 6572 6875 622e 6d6c  cs.adapterhub.ml
-000016a0: 2a2a 2c20 6f75 7220 646f 6375 6d65 6e74  **, our document
-000016b0: 6174 696f 6e20 6f6e 2074 7261 696e 696e  ation on trainin
-000016c0: 6720 616e 6420 7573 696e 6720 6164 6170  g and using adap
-000016d0: 7465 7273 2077 6974 6820 5f61 6461 7074  ters with _adapt
-000016e0: 6572 735f 0d0a 2d20 2a2a 6874 7470 733a  ers_..- **https:
-000016f0: 2f2f 6164 6170 7465 7268 7562 2e6d 6c2a  //adapterhub.ml*
-00001700: 2a20 746f 2065 7870 6c6f 7265 2061 7661  * to explore ava
-00001710: 696c 6162 6c65 2070 7265 2d74 7261 696e  ilable pre-train
-00001720: 6564 2061 6461 7074 6572 206d 6f64 756c  ed adapter modul
-00001730: 6573 2061 6e64 2073 6861 7265 2079 6f75  es and share you
-00001740: 7220 6f77 6e20 6164 6170 7465 7273 0d0a  r own adapters..
-00001750: 2d20 2a2a 5b45 7861 6d70 6c65 7320 666f  - **[Examples fo
-00001760: 6c64 6572 5d28 6874 7470 733a 2f2f 6769  lder](https://gi
-00001770: 7468 7562 2e63 6f6d 2f41 6461 7074 6572  thub.com/Adapter
-00001780: 2d48 7562 2f61 6461 7074 6572 732f 7472  -Hub/adapters/tr
-00001790: 6565 2f6d 6169 6e2f 6578 616d 706c 6573  ee/main/examples
-000017a0: 2f70 7974 6f72 6368 292a 2a20 6f66 2074  /pytorch)** of t
-000017b0: 6869 7320 7265 706f 7369 746f 7279 2063  his repository c
-000017c0: 6f6e 7461 696e 696e 6720 4875 6767 696e  ontaining Huggin
-000017d0: 6746 6163 6527 7320 6578 616d 706c 6520  gFace's example 
-000017e0: 7472 6169 6e69 6e67 2073 6372 6970 7473  training scripts
-000017f0: 2c20 6d61 6e79 2061 6461 7074 6564 2066  , many adapted f
-00001800: 6f72 2074 7261 696e 696e 6720 6164 6170  or training adap
-00001810: 7465 7273 0d0a 0d0a 2323 2049 6d70 6c65  ters....## Imple
-00001820: 6d65 6e74 6564 204d 6574 686f 6473 0d0a  mented Methods..
-00001830: 0d0a 4375 7272 656e 746c 792c 2061 6461  ..Currently, ada
-00001840: 7074 6572 7320 696e 7465 6772 6174 6573  pters integrates
-00001850: 2061 6c6c 2061 7263 6869 7465 6374 7572   all architectur
-00001860: 6573 2061 6e64 206d 6574 686f 6473 206c  es and methods l
-00001870: 6973 7465 6420 6265 6c6f 773a 0d0a 0d0a  isted below:....
-00001880: 7c20 4d65 7468 6f64 207c 2050 6170 6572  | Method | Paper
-00001890: 2873 2920 7c20 5175 6963 6b20 4c69 6e6b  (s) | Quick Link
-000018a0: 7320 7c0d 0a7c 202d 2d2d 207c 202d 2d2d  s |..| --- | ---
-000018b0: 207c 202d 2d2d 207c 0d0a 7c20 426f 7474   | --- |..| Bott
-000018c0: 6c65 6e65 636b 2061 6461 7074 6572 7320  leneck adapters 
-000018d0: 7c20 5b48 6f75 6c73 6279 2065 7420 616c  | [Houlsby et al
-000018e0: 2e20 2832 3031 3929 5d28 6874 7470 733a  . (2019)](https:
-000018f0: 2f2f 6172 7869 762e 6f72 672f 7064 662f  //arxiv.org/pdf/
-00001900: 3139 3032 2e30 3037 3531 2e70 6466 293c  1902.00751.pdf)<
-00001910: 6272 3e20 5b42 6170 6e61 2061 6e64 2046  br> [Bapna and F
-00001920: 6972 6174 2028 3230 3139 295d 2868 7474  irat (2019)](htt
-00001930: 7073 3a2f 2f61 7278 6976 2e6f 7267 2f70  ps://arxiv.org/p
-00001940: 6466 2f31 3930 392e 3038 3437 382e 7064  df/1909.08478.pd
-00001950: 6629 207c 205b 5175 6963 6b73 7461 7274  f) | [Quickstart
-00001960: 5d28 6874 7470 733a 2f2f 646f 6373 2e61  ](https://docs.a
-00001970: 6461 7074 6572 6875 622e 6d6c 2f71 7569  dapterhub.ml/qui
-00001980: 636b 7374 6172 742e 6874 6d6c 292c 205b  ckstart.html), [
-00001990: 4e6f 7465 626f 6f6b 5d28 6874 7470 733a  Notebook](https:
-000019a0: 2f2f 636f 6c61 622e 7265 7365 6172 6368  //colab.research
-000019b0: 2e67 6f6f 676c 652e 636f 6d2f 6769 7468  .google.com/gith
-000019c0: 7562 2f41 6461 7074 6572 2d48 7562 2f61  ub/Adapter-Hub/a
-000019d0: 6461 7074 6572 732f 626c 6f62 2f6d 6169  dapters/blob/mai
-000019e0: 6e2f 6e6f 7465 626f 6f6b 732f 3031 5f41  n/notebooks/01_A
-000019f0: 6461 7074 6572 5f54 7261 696e 696e 672e  dapter_Training.
-00001a00: 6970 796e 6229 207c 0d0a 7c20 4164 6170  ipynb) |..| Adap
-00001a10: 7465 7246 7573 696f 6e20 7c20 5b50 6665  terFusion | [Pfe
-00001a20: 6966 6665 7220 6574 2061 6c2e 2028 3230  iffer et al. (20
-00001a30: 3231 295d 2868 7474 7073 3a2f 2f61 636c  21)](https://acl
-00001a40: 616e 7468 6f6c 6f67 792e 6f72 672f 3230  anthology.org/20
-00001a50: 3231 2e65 6163 6c2d 6d61 696e 2e33 392e  21.eacl-main.39.
-00001a60: 7064 6629 207c 205b 446f 6373 3a20 5472  pdf) | [Docs: Tr
-00001a70: 6169 6e69 6e67 5d28 6874 7470 733a 2f2f  aining](https://
-00001a80: 646f 6373 2e61 6461 7074 6572 6875 622e  docs.adapterhub.
-00001a90: 6d6c 2f74 7261 696e 696e 672e 6874 6d6c  ml/training.html
-00001aa0: 2374 7261 696e 2d61 6461 7074 6572 6675  #train-adapterfu
-00001ab0: 7369 6f6e 292c 205b 4e6f 7465 626f 6f6b  sion), [Notebook
-00001ac0: 5d28 6874 7470 733a 2f2f 636f 6c61 622e  ](https://colab.
-00001ad0: 7265 7365 6172 6368 2e67 6f6f 676c 652e  research.google.
-00001ae0: 636f 6d2f 6769 7468 7562 2f41 6461 7074  com/github/Adapt
-00001af0: 6572 2d48 7562 2f61 6461 7074 6572 732f  er-Hub/adapters/
-00001b00: 626c 6f62 2f6d 6169 6e2f 6e6f 7465 626f  blob/main/notebo
-00001b10: 6f6b 732f 3033 5f41 6461 7074 6572 5f46  oks/03_Adapter_F
-00001b20: 7573 696f 6e2e 6970 796e 6229 207c 0d0a  usion.ipynb) |..
-00001b30: 7c20 4d41 442d 582c 3c62 723e 2049 6e76  | MAD-X,<br> Inv
-00001b40: 6572 7469 626c 6520 6164 6170 7465 7273  ertible adapters
-00001b50: 207c 205b 5066 6569 6666 6572 2065 7420   | [Pfeiffer et 
-00001b60: 616c 2e20 2832 3032 3029 5d28 6874 7470  al. (2020)](http
-00001b70: 733a 2f2f 6163 6c61 6e74 686f 6c6f 6779  s://aclanthology
-00001b80: 2e6f 7267 2f32 3032 302e 656d 6e6c 702d  .org/2020.emnlp-
-00001b90: 6d61 696e 2e36 3137 2f29 207c 205b 4e6f  main.617/) | [No
-00001ba0: 7465 626f 6f6b 5d28 6874 7470 733a 2f2f  tebook](https://
-00001bb0: 636f 6c61 622e 7265 7365 6172 6368 2e67  colab.research.g
-00001bc0: 6f6f 676c 652e 636f 6d2f 6769 7468 7562  oogle.com/github
-00001bd0: 2f41 6461 7074 6572 2d48 7562 2f61 6461  /Adapter-Hub/ada
-00001be0: 7074 6572 732f 626c 6f62 2f6d 6169 6e2f  pters/blob/main/
-00001bf0: 6e6f 7465 626f 6f6b 732f 3034 5f43 726f  notebooks/04_Cro
-00001c00: 7373 5f4c 696e 6775 616c 5f54 7261 6e73  ss_Lingual_Trans
-00001c10: 6665 722e 6970 796e 6229 207c 0d0a 7c20  fer.ipynb) |..| 
-00001c20: 4164 6170 7465 7244 726f 7020 7c20 5b52  AdapterDrop | [R
-00001c30: c3bc 636b 6cc3 a920 6574 2061 6c2e 2028  ..ckl.. et al. (
-00001c40: 3230 3231 295d 2868 7474 7073 3a2f 2f61  2021)](https://a
-00001c50: 7278 6976 2e6f 7267 2f70 6466 2f32 3031  rxiv.org/pdf/201
-00001c60: 302e 3131 3931 382e 7064 6629 207c 205b  0.11918.pdf) | [
-00001c70: 4e6f 7465 626f 6f6b 5d28 6874 7470 733a  Notebook](https:
-00001c80: 2f2f 636f 6c61 622e 7265 7365 6172 6368  //colab.research
-00001c90: 2e67 6f6f 676c 652e 636f 6d2f 6769 7468  .google.com/gith
-00001ca0: 7562 2f41 6461 7074 6572 2d48 7562 2f61  ub/Adapter-Hub/a
-00001cb0: 6461 7074 6572 732f 626c 6f62 2f6d 6169  dapters/blob/mai
-00001cc0: 6e2f 6e6f 7465 626f 6f6b 732f 3035 5f41  n/notebooks/05_A
-00001cd0: 6461 7074 6572 5f44 726f 705f 5472 6169  dapter_Drop_Trai
-00001ce0: 6e69 6e67 2e69 7079 6e62 2920 7c0d 0a7c  ning.ipynb) |..|
-00001cf0: 204d 4144 2d58 2032 2e30 2c3c 6272 3e20   MAD-X 2.0,<br> 
-00001d00: 456d 6265 6464 696e 6720 7472 6169 6e69  Embedding traini
-00001d10: 6e67 207c 205b 5066 6569 6666 6572 2065  ng | [Pfeiffer e
-00001d20: 7420 616c 2e20 2832 3032 3129 5d28 6874  t al. (2021)](ht
-00001d30: 7470 733a 2f2f 6172 7869 762e 6f72 672f  tps://arxiv.org/
-00001d40: 7064 662f 3230 3132 2e31 3535 3632 2e70  pdf/2012.15562.p
-00001d50: 6466 2920 7c20 5b44 6f63 733a 2045 6d62  df) | [Docs: Emb
-00001d60: 6564 6469 6e67 735d 2868 7474 7073 3a2f  eddings](https:/
-00001d70: 2f64 6f63 732e 6164 6170 7465 7268 7562  /docs.adapterhub
-00001d80: 2e6d 6c2f 656d 6265 6464 696e 6773 2e68  .ml/embeddings.h
-00001d90: 746d 6c29 2c20 5b4e 6f74 6562 6f6f 6b5d  tml), [Notebook]
-00001da0: 2868 7474 7073 3a2f 2f63 6f6c 6162 2e72  (https://colab.r
-00001db0: 6573 6561 7263 682e 676f 6f67 6c65 2e63  esearch.google.c
-00001dc0: 6f6d 2f67 6974 6875 622f 4164 6170 7465  om/github/Adapte
-00001dd0: 722d 4875 622f 6164 6170 7465 7273 2f62  r-Hub/adapters/b
-00001de0: 6c6f 622f 6d61 696e 2f6e 6f74 6562 6f6f  lob/main/noteboo
-00001df0: 6b73 2f30 385f 4e45 525f 5769 6b69 616e  ks/08_NER_Wikian
-00001e00: 6e2e 6970 796e 6229 207c 0d0a 7c20 5072  n.ipynb) |..| Pr
-00001e10: 6566 6978 2054 756e 696e 6720 7c20 5b4c  efix Tuning | [L
-00001e20: 6920 616e 6420 4c69 616e 6720 2832 3032  i and Liang (202
-00001e30: 3129 5d28 6874 7470 733a 2f2f 6172 7869  1)](https://arxi
-00001e40: 762e 6f72 672f 7064 662f 3231 3031 2e30  v.org/pdf/2101.0
-00001e50: 3031 3930 2e70 6466 2920 7c20 5b44 6f63  0190.pdf) | [Doc
-00001e60: 735d 2868 7474 7073 3a2f 2f64 6f63 732e  s](https://docs.
-00001e70: 6164 6170 7465 7268 7562 2e6d 6c2f 6d65  adapterhub.ml/me
-00001e80: 7468 6f64 732e 6874 6d6c 2370 7265 6669  thods.html#prefi
-00001e90: 782d 7475 6e69 6e67 2920 7c0d 0a7c 2050  x-tuning) |..| P
-00001ea0: 6172 616c 6c65 6c20 6164 6170 7465 7273  arallel adapters
-00001eb0: 2c3c 6272 3e20 4d69 782d 616e 642d 4d61  ,<br> Mix-and-Ma
-00001ec0: 7463 6820 6164 6170 7465 7273 207c 205b  tch adapters | [
-00001ed0: 4865 2065 7420 616c 2e20 2832 3032 3129  He et al. (2021)
-00001ee0: 5d28 6874 7470 733a 2f2f 6172 7869 762e  ](https://arxiv.
-00001ef0: 6f72 672f 7064 662f 3231 3130 2e30 3433  org/pdf/2110.043
-00001f00: 3636 2e70 6466 2920 7c20 5b44 6f63 735d  66.pdf) | [Docs]
-00001f10: 2868 7474 7073 3a2f 2f64 6f63 732e 6164  (https://docs.ad
-00001f20: 6170 7465 7268 7562 2e6d 6c2f 6d65 7468  apterhub.ml/meth
-00001f30: 6f64 5f63 6f6d 6269 6e61 7469 6f6e 732e  od_combinations.
-00001f40: 6874 6d6c 236d 6978 2d61 6e64 2d6d 6174  html#mix-and-mat
-00001f50: 6368 2d61 6461 7074 6572 7329 207c 0d0a  ch-adapters) |..
-00001f60: 7c20 436f 6d70 6163 7465 7220 7c20 5b4d  | Compacter | [M
-00001f70: 6168 6162 6164 6920 6574 2061 6c2e 2028  ahabadi et al. (
-00001f80: 3230 3231 295d 2868 7474 7073 3a2f 2f61  2021)](https://a
-00001f90: 7278 6976 2e6f 7267 2f70 6466 2f32 3130  rxiv.org/pdf/210
-00001fa0: 362e 3034 3634 372e 7064 6629 207c 205b  6.04647.pdf) | [
-00001fb0: 446f 6373 5d28 6874 7470 733a 2f2f 646f  Docs](https://do
-00001fc0: 6373 2e61 6461 7074 6572 6875 622e 6d6c  cs.adapterhub.ml
-00001fd0: 2f6d 6574 686f 6473 2e68 746d 6c23 636f  /methods.html#co
-00001fe0: 6d70 6163 7465 7229 207c 0d0a 7c20 4c6f  mpacter) |..| Lo
-00001ff0: 5241 207c 205b 4875 2065 7420 616c 2e20  RA | [Hu et al. 
-00002000: 2832 3032 3129 5d28 6874 7470 733a 2f2f  (2021)](https://
-00002010: 6172 7869 762e 6f72 672f 7064 662f 3231  arxiv.org/pdf/21
-00002020: 3036 2e30 3936 3835 2e70 6466 2920 7c20  06.09685.pdf) | 
-00002030: 5b44 6f63 735d 2868 7474 7073 3a2f 2f64  [Docs](https://d
-00002040: 6f63 732e 6164 6170 7465 7268 7562 2e6d  ocs.adapterhub.m
-00002050: 6c2f 6d65 7468 6f64 732e 6874 6d6c 236c  l/methods.html#l
-00002060: 6f72 6129 207c 0d0a 7c20 2849 4129 5e33  ora) |..| (IA)^3
-00002070: 207c 205b 4c69 7520 6574 2061 6c2e 2028   | [Liu et al. (
-00002080: 3230 3232 295d 2868 7474 7073 3a2f 2f61  2022)](https://a
-00002090: 7278 6976 2e6f 7267 2f70 6466 2f32 3230  rxiv.org/pdf/220
-000020a0: 352e 3035 3633 382e 7064 6629 207c 205b  5.05638.pdf) | [
-000020b0: 446f 6373 5d28 6874 7470 733a 2f2f 646f  Docs](https://do
-000020c0: 6373 2e61 6461 7074 6572 6875 622e 6d6c  cs.adapterhub.ml
-000020d0: 2f6d 6574 686f 6473 2e68 746d 6c23 6961  /methods.html#ia
-000020e0: 2d33 2920 7c0d 0a7c 2055 6e69 5045 4c54  -3) |..| UniPELT
-000020f0: 207c 205b 4d61 6f20 6574 2061 6c2e 2028   | [Mao et al. (
-00002100: 3230 3232 295d 2868 7474 7073 3a2f 2f61  2022)](https://a
-00002110: 7278 6976 2e6f 7267 2f70 6466 2f32 3131  rxiv.org/pdf/211
-00002120: 302e 3037 3537 372e 7064 6629 207c 205b  0.07577.pdf) | [
-00002130: 446f 6373 5d28 6874 7470 733a 2f2f 646f  Docs](https://do
-00002140: 6373 2e61 6461 7074 6572 6875 622e 6d6c  cs.adapterhub.ml
-00002150: 2f6d 6574 686f 645f 636f 6d62 696e 6174  /method_combinat
-00002160: 696f 6e73 2e68 746d 6c23 756e 6970 656c  ions.html#unipel
-00002170: 7429 207c 0d0a 7c20 5072 6f6d 7074 2054  t) |..| Prompt T
-00002180: 756e 696e 6720 7c20 5b4c 6573 7465 7220  uning | [Lester 
-00002190: 6574 2061 6c2e 2028 3230 3231 295d 2868  et al. (2021)](h
-000021a0: 7474 7073 3a2f 2f61 636c 616e 7468 6f6c  ttps://aclanthol
-000021b0: 6f67 792e 6f72 672f 3230 3231 2e65 6d6e  ogy.org/2021.emn
-000021c0: 6c70 2d6d 6169 6e2e 3234 332f 2920 7c20  lp-main.243/) | 
-000021d0: 5b44 6f63 735d 2868 7474 7073 3a2f 2f64  [Docs](https://d
-000021e0: 6f63 732e 6164 6170 7465 7268 7562 2e6d  ocs.adapterhub.m
-000021f0: 6c2f 6d65 7468 6f64 732e 6874 6d6c 2370  l/methods.html#p
-00002200: 726f 6d70 742d 7475 6e69 6e67 2920 7c0d  rompt-tuning) |.
-00002210: 0a0d 0a23 2320 5375 7070 6f72 7465 6420  ...## Supported 
-00002220: 4d6f 6465 6c73 0d0a 0d0a 5765 2063 7572  Models....We cur
-00002230: 7265 6e74 6c79 2073 7570 706f 7274 2074  rently support t
-00002240: 6865 2050 7954 6f72 6368 2076 6572 7369  he PyTorch versi
-00002250: 6f6e 7320 6f66 2061 6c6c 206d 6f64 656c  ons of all model
-00002260: 7320 6c69 7374 6564 206f 6e20 7468 6520  s listed on the 
-00002270: 2a2a 5b4d 6f64 656c 204f 7665 7276 6965  **[Model Overvie
-00002280: 775d 2868 7474 7073 3a2f 2f64 6f63 732e  w](https://docs.
-00002290: 6164 6170 7465 7268 7562 2e6d 6c2f 6d6f  adapterhub.ml/mo
-000022a0: 6465 6c5f 6f76 6572 7669 6577 2e68 746d  del_overview.htm
-000022b0: 6c29 2070 6167 652a 2a20 696e 206f 7572  l) page** in our
-000022c0: 2064 6f63 756d 656e 7461 7469 6f6e 2e0d   documentation..
-000022d0: 0a0d 0a23 2320 4465 7665 6c6f 7069 6e67  ...## Developing
-000022e0: 2026 2043 6f6e 7472 6962 7574 696e 670d   & Contributing.
-000022f0: 0a0d 0a54 6f20 6765 7420 7374 6172 7465  ...To get starte
-00002300: 6420 7769 7468 2064 6576 656c 6f70 696e  d with developin
-00002310: 6720 6f6e 205f 4164 6170 7465 7273 5f20  g on _Adapters_ 
-00002320: 796f 7572 7365 6c66 2061 6e64 206c 6561  yourself and lea
-00002330: 726e 206d 6f72 6520 6162 6f75 7420 7761  rn more about wa
-00002340: 7973 2074 6f20 636f 6e74 7269 6275 7465  ys to contribute
-00002350: 2c20 706c 6561 7365 2073 6565 2068 7474  , please see htt
-00002360: 7073 3a2f 2f64 6f63 732e 6164 6170 7465  ps://docs.adapte
-00002370: 7268 7562 2e6d 6c2f 636f 6e74 7269 6275  rhub.ml/contribu
-00002380: 7469 6e67 2e68 746d 6c2e 0d0a 0d0a 2323  ting.html.....##
-00002390: 2043 6974 6174 696f 6e0d 0a0d 0a49 6620   Citation....If 
-000023a0: 796f 7520 7573 6520 5f41 6461 7074 6572  you use _Adapter
-000023b0: 735f 2069 6e20 796f 7572 2077 6f72 6b2c  s_ in your work,
-000023c0: 2070 6c65 6173 6520 636f 6e73 6964 6572   please consider
-000023d0: 2063 6974 696e 6720 6f75 7220 6c69 6272   citing our libr
-000023e0: 6172 7920 7061 7065 723a 205b 4164 6170  ary paper: [Adap
-000023f0: 7465 7273 3a20 4120 556e 6966 6965 6420  ters: A Unified 
-00002400: 4c69 6272 6172 7920 666f 7220 5061 7261  Library for Para
-00002410: 6d65 7465 722d 4566 6669 6369 656e 7420  meter-Efficient 
-00002420: 616e 6420 4d6f 6475 6c61 7220 5472 616e  and Modular Tran
-00002430: 7366 6572 204c 6561 726e 696e 675d 2868  sfer Learning](h
-00002440: 7474 7073 3a2f 2f61 7278 6976 2e6f 7267  ttps://arxiv.org
-00002450: 2f61 6273 2f32 3331 312e 3131 3037 3729  /abs/2311.11077)
-00002460: 0d0a 0d0a 6060 600d 0a40 696e 7072 6f63  ....```..@inproc
-00002470: 6565 6469 6e67 737b 706f 7468 2d65 7461  eedings{poth-eta
-00002480: 6c2d 3230 3233 2d61 6461 7074 6572 732c  l-2023-adapters,
-00002490: 0d0a 2020 2020 7469 746c 6520 3d20 2241  ..    title = "A
-000024a0: 6461 7074 6572 733a 2041 2055 6e69 6669  dapters: A Unifi
-000024b0: 6564 204c 6962 7261 7279 2066 6f72 2050  ed Library for P
-000024c0: 6172 616d 6574 6572 2d45 6666 6963 6965  arameter-Efficie
-000024d0: 6e74 2061 6e64 204d 6f64 756c 6172 2054  nt and Modular T
-000024e0: 7261 6e73 6665 7220 4c65 6172 6e69 6e67  ransfer Learning
-000024f0: 222c 0d0a 2020 2020 6175 7468 6f72 203d  ",..    author =
-00002500: 207b 506f 7468 2c20 436c 6966 746f 6e20   {Poth, Clifton 
-00002510: 2061 6e64 0d0a 2020 2020 2020 5374 6572   and..      Ster
-00002520: 7a2c 2048 616e 6e61 6820 2061 6e64 0d0a  z, Hannah  and..
-00002530: 2020 2020 2020 5061 756c 2c20 496e 6472        Paul, Indr
-00002540: 616e 6569 6c20 2061 6e64 0d0a 2020 2020  aneil  and..    
-00002550: 2020 5075 726b 6179 6173 7468 612c 2053    Purkayastha, S
-00002560: 756b 616e 6e79 6120 2061 6e64 0d0a 2020  ukannya  and..  
-00002570: 2020 2020 456e 676c 7b5c 2261 7d6e 6465      Engl{\"a}nde
-00002580: 722c 204c 656f 6e20 2061 6e64 0d0a 2020  r, Leon  and..  
-00002590: 2020 2020 496d 686f 662c 2054 696d 6f20      Imhof, Timo 
-000025a0: 2061 6e64 0d0a 2020 2020 2020 5675 6c69   and..      Vuli
-000025b0: 7b5c 2763 7d2c 2049 7661 6e20 2061 6e64  {\'c}, Ivan  and
-000025c0: 0d0a 2020 2020 2020 5275 6465 722c 2053  ..      Ruder, S
-000025d0: 6562 6173 7469 616e 2020 616e 640d 0a20  ebastian  and.. 
-000025e0: 2020 2020 2047 7572 6576 7963 682c 2049       Gurevych, I
-000025f0: 7279 6e61 2020 616e 640d 0a20 2020 2020  ryna  and..     
-00002600: 2050 6665 6966 6665 722c 204a 6f6e 6173   Pfeiffer, Jonas
-00002610: 7d2c 0d0a 2020 2020 626f 6f6b 7469 746c  },..    booktitl
-00002620: 6520 3d20 2250 726f 6365 6564 696e 6773  e = "Proceedings
-00002630: 206f 6620 7468 6520 3230 3233 2043 6f6e   of the 2023 Con
-00002640: 6665 7265 6e63 6520 6f6e 2045 6d70 6972  ference on Empir
-00002650: 6963 616c 204d 6574 686f 6473 2069 6e20  ical Methods in 
-00002660: 4e61 7475 7261 6c20 4c61 6e67 7561 6765  Natural Language
-00002670: 2050 726f 6365 7373 696e 673a 2053 7973   Processing: Sys
-00002680: 7465 6d20 4465 6d6f 6e73 7472 6174 696f  tem Demonstratio
-00002690: 6e73 222c 0d0a 2020 2020 6d6f 6e74 6820  ns",..    month 
-000026a0: 3d20 6465 632c 0d0a 2020 2020 7965 6172  = dec,..    year
-000026b0: 203d 2022 3230 3233 222c 0d0a 2020 2020   = "2023",..    
-000026c0: 6164 6472 6573 7320 3d20 2253 696e 6761  address = "Singa
-000026d0: 706f 7265 222c 0d0a 2020 2020 7075 626c  pore",..    publ
-000026e0: 6973 6865 7220 3d20 2241 7373 6f63 6961  isher = "Associa
-000026f0: 7469 6f6e 2066 6f72 2043 6f6d 7075 7461  tion for Computa
-00002700: 7469 6f6e 616c 204c 696e 6775 6973 7469  tional Linguisti
-00002710: 6373 222c 0d0a 2020 2020 7572 6c20 3d20  cs",..    url = 
-00002720: 2268 7474 7073 3a2f 2f61 636c 616e 7468  "https://aclanth
-00002730: 6f6c 6f67 792e 6f72 672f 3230 3233 2e65  ology.org/2023.e
-00002740: 6d6e 6c70 2d64 656d 6f2e 3133 222c 0d0a  mnlp-demo.13",..
-00002750: 2020 2020 7061 6765 7320 3d20 2231 3439      pages = "149
-00002760: 2d2d 3136 3022 2c0d 0a7d 0d0a 6060 600d  --160",..}..```.
-00002770: 0a0d 0a41 6c74 6572 6e61 7469 7665 6c79  ...Alternatively
-00002780: 2c20 666f 7220 7468 6520 7072 6564 6563  , for the predec
-00002790: 6573 736f 7220 6061 6461 7074 6572 2d74  essor `adapter-t
-000027a0: 7261 6e73 666f 726d 6572 7360 2c20 7468  ransformers`, th
-000027b0: 6520 4875 6220 696e 6672 6173 7472 7563  e Hub infrastruc
-000027c0: 7475 7265 2061 6e64 2061 6461 7074 6572  ture and adapter
-000027d0: 7320 7570 6c6f 6164 6564 2062 7920 7468  s uploaded by th
-000027e0: 6520 4164 6170 7465 7248 7562 2074 6561  e AdapterHub tea
-000027f0: 6d2c 2070 6c65 6173 6520 636f 6e73 6964  m, please consid
-00002800: 6572 2063 6974 696e 6720 6f75 7220 696e  er citing our in
-00002810: 6974 6961 6c20 7061 7065 723a 205b 4164  itial paper: [Ad
-00002820: 6170 7465 7248 7562 3a20 4120 4672 616d  apterHub: A Fram
-00002830: 6577 6f72 6b20 666f 7220 4164 6170 7469  ework for Adapti
-00002840: 6e67 2054 7261 6e73 666f 726d 6572 735d  ng Transformers]
-00002850: 2868 7474 7073 3a2f 2f61 7278 6976 2e6f  (https://arxiv.o
-00002860: 7267 2f61 6273 2f32 3030 372e 3037 3737  rg/abs/2007.0777
-00002870: 3929 0d0a 0d0a 6060 600d 0a40 696e 7072  9)....```..@inpr
-00002880: 6f63 6565 6469 6e67 737b 7066 6569 6666  oceedings{pfeiff
-00002890: 6572 3230 3230 4164 6170 7465 7248 7562  er2020AdapterHub
-000028a0: 2c0d 0a20 2020 2074 6974 6c65 3d7b 4164  ,..    title={Ad
-000028b0: 6170 7465 7248 7562 3a20 4120 4672 616d  apterHub: A Fram
-000028c0: 6577 6f72 6b20 666f 7220 4164 6170 7469  ework for Adapti
-000028d0: 6e67 2054 7261 6e73 666f 726d 6572 737d  ng Transformers}
-000028e0: 2c0d 0a20 2020 2061 7574 686f 723d 7b50  ,..    author={P
-000028f0: 6665 6966 6665 722c 204a 6f6e 6173 2061  feiffer, Jonas a
-00002900: 6e64 0d0a 2020 2020 2020 2020 2020 2020  nd..            
-00002910: 527b 5c22 757d 636b 6c7b 5c27 657d 2c20  R{\"u}ckl{\'e}, 
-00002920: 416e 6472 6561 7320 616e 640d 0a20 2020  Andreas and..   
-00002930: 2020 2020 2020 2020 2050 6f74 682c 2043           Poth, C
-00002940: 6c69 6674 6f6e 2061 6e64 0d0a 2020 2020  lifton and..    
-00002950: 2020 2020 2020 2020 4b61 6d61 7468 2c20          Kamath, 
-00002960: 4169 7368 7761 7279 6120 616e 640d 0a20  Aishwarya and.. 
-00002970: 2020 2020 2020 2020 2020 2056 756c 697b             Vuli{
-00002980: 5c27 637d 2c20 4976 616e 2061 6e64 0d0a  \'c}, Ivan and..
-00002990: 2020 2020 2020 2020 2020 2020 5275 6465              Rude
-000029a0: 722c 2053 6562 6173 7469 616e 2061 6e64  r, Sebastian and
-000029b0: 0d0a 2020 2020 2020 2020 2020 2020 4368  ..            Ch
-000029c0: 6f2c 204b 7975 6e67 6879 756e 2061 6e64  o, Kyunghyun and
-000029d0: 0d0a 2020 2020 2020 2020 2020 2020 4775  ..            Gu
-000029e0: 7265 7679 6368 2c20 4972 796e 617d 2c0d  revych, Iryna},.
-000029f0: 0a20 2020 2062 6f6f 6b74 6974 6c65 3d7b  .    booktitle={
-00002a00: 5072 6f63 6565 6469 6e67 7320 6f66 2074  Proceedings of t
-00002a10: 6865 2032 3032 3020 436f 6e66 6572 656e  he 2020 Conferen
-00002a20: 6365 206f 6e20 456d 7069 7269 6361 6c20  ce on Empirical 
-00002a30: 4d65 7468 6f64 7320 696e 204e 6174 7572  Methods in Natur
-00002a40: 616c 204c 616e 6775 6167 6520 5072 6f63  al Language Proc
-00002a50: 6573 7369 6e67 3a20 5379 7374 656d 2044  essing: System D
-00002a60: 656d 6f6e 7374 7261 7469 6f6e 737d 2c0d  emonstrations},.
-00002a70: 0a20 2020 2070 6167 6573 3d7b 3436 2d2d  .    pages={46--
-00002a80: 3534 7d2c 0d0a 2020 2020 7965 6172 3d7b  54},..    year={
-00002a90: 3230 3230 7d0d 0a7d 0d0a 6060 600d 0a    2020}..}..```..
+00000100: 6c3a 2063 616c 7074 406d 6169 6c2e 6465  l: calpt@mail.de
+00000110: 0d0a 4c69 6365 6e73 653a 2041 7061 6368  ..License: Apach
+00000120: 650d 0a4b 6579 776f 7264 733a 204e 4c50  e..Keywords: NLP
+00000130: 2064 6565 7020 6c65 6172 6e69 6e67 2074   deep learning t
+00000140: 7261 6e73 666f 726d 6572 2070 7974 6f72  ransformer pytor
+00000150: 6368 2042 4552 5420 6164 6170 7465 7273  ch BERT adapters
+00000160: 0d0a 436c 6173 7369 6669 6572 3a20 4465  ..Classifier: De
+00000170: 7665 6c6f 706d 656e 7420 5374 6174 7573  velopment Status
+00000180: 203a 3a20 3420 2d20 4265 7461 0d0a 436c   :: 4 - Beta..Cl
+00000190: 6173 7369 6669 6572 3a20 496e 7465 6e64  assifier: Intend
+000001a0: 6564 2041 7564 6965 6e63 6520 3a3a 2044  ed Audience :: D
+000001b0: 6576 656c 6f70 6572 730d 0a43 6c61 7373  evelopers..Class
+000001c0: 6966 6965 723a 2049 6e74 656e 6465 6420  ifier: Intended 
+000001d0: 4175 6469 656e 6365 203a 3a20 4564 7563  Audience :: Educ
+000001e0: 6174 696f 6e0d 0a43 6c61 7373 6966 6965  ation..Classifie
+000001f0: 723a 2049 6e74 656e 6465 6420 4175 6469  r: Intended Audi
+00000200: 656e 6365 203a 3a20 5363 6965 6e63 652f  ence :: Science/
+00000210: 5265 7365 6172 6368 0d0a 436c 6173 7369  Research..Classi
+00000220: 6669 6572 3a20 4c69 6365 6e73 6520 3a3a  fier: License ::
+00000230: 204f 5349 2041 7070 726f 7665 6420 3a3a   OSI Approved ::
+00000240: 2041 7061 6368 6520 536f 6674 7761 7265   Apache Software
+00000250: 204c 6963 656e 7365 0d0a 436c 6173 7369   License..Classi
+00000260: 6669 6572 3a20 4f70 6572 6174 696e 6720  fier: Operating 
+00000270: 5379 7374 656d 203a 3a20 4f53 2049 6e64  System :: OS Ind
+00000280: 6570 656e 6465 6e74 0d0a 436c 6173 7369  ependent..Classi
+00000290: 6669 6572 3a20 5072 6f67 7261 6d6d 696e  fier: Programmin
+000002a0: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
+000002b0: 7468 6f6e 203a 3a20 330d 0a43 6c61 7373  thon :: 3..Class
+000002c0: 6966 6965 723a 2050 726f 6772 616d 6d69  ifier: Programmi
+000002d0: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
+000002e0: 7974 686f 6e20 3a3a 2033 2e38 0d0a 436c  ython :: 3.8..Cl
+000002f0: 6173 7369 6669 6572 3a20 5072 6f67 7261  assifier: Progra
+00000300: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
+00000310: 3a20 5079 7468 6f6e 203a 3a20 332e 390d  : Python :: 3.9.
+00000320: 0a43 6c61 7373 6966 6965 723a 2050 726f  .Classifier: Pro
+00000330: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
+00000340: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
+00000350: 2e31 300d 0a43 6c61 7373 6966 6965 723a  .10..Classifier:
+00000360: 2054 6f70 6963 203a 3a20 5363 6965 6e74   Topic :: Scient
+00000370: 6966 6963 2f45 6e67 696e 6565 7269 6e67  ific/Engineering
+00000380: 203a 3a20 4172 7469 6669 6369 616c 2049   :: Artificial I
+00000390: 6e74 656c 6c69 6765 6e63 650d 0a52 6571  ntelligence..Req
+000003a0: 7569 7265 732d 5079 7468 6f6e 3a20 3e3d  uires-Python: >=
+000003b0: 332e 382e 300d 0a44 6573 6372 6970 7469  3.8.0..Descripti
+000003c0: 6f6e 2d43 6f6e 7465 6e74 2d54 7970 653a  on-Content-Type:
+000003d0: 2074 6578 742f 6d61 726b 646f 776e 0d0a   text/markdown..
+000003e0: 5072 6f76 6964 6573 2d45 7874 7261 3a20  Provides-Extra: 
+000003f0: 736b 6c65 6172 6e0d 0a50 726f 7669 6465  sklearn..Provide
+00000400: 732d 4578 7472 613a 2074 6f72 6368 0d0a  s-Extra: torch..
+00000410: 5072 6f76 6964 6573 2d45 7874 7261 3a20  Provides-Extra: 
+00000420: 6f6e 6e78 7275 6e74 696d 650d 0a50 726f  onnxruntime..Pro
+00000430: 7669 6465 732d 4578 7472 613a 2073 656e  vides-Extra: sen
+00000440: 7465 6e63 6570 6965 6365 0d0a 5072 6f76  tencepiece..Prov
+00000450: 6964 6573 2d45 7874 7261 3a20 7465 7374  ides-Extra: test
+00000460: 696e 670d 0a50 726f 7669 6465 732d 4578  ing..Provides-Ex
+00000470: 7472 613a 2071 7561 6c69 7479 0d0a 5072  tra: quality..Pr
+00000480: 6f76 6964 6573 2d45 7874 7261 3a20 646f  ovides-Extra: do
+00000490: 6373 0d0a 5072 6f76 6964 6573 2d45 7874  cs..Provides-Ext
+000004a0: 7261 3a20 6465 760d 0a4c 6963 656e 7365  ra: dev..License
+000004b0: 2d46 696c 653a 204c 4943 454e 5345 0d0a  -File: LICENSE..
+000004c0: 0d0a 3c21 2d2d 2d0d 0a43 6f70 7972 6967  ..<!---..Copyrig
+000004d0: 6874 2032 3032 3020 5468 6520 4164 6170  ht 2020 The Adap
+000004e0: 7465 7248 7562 2054 6561 6d2e 2041 6c6c  terHub Team. All
+000004f0: 2072 6967 6874 7320 7265 7365 7276 6564   rights reserved
+00000500: 2e0d 0a0d 0a4c 6963 656e 7365 6420 756e  .....Licensed un
+00000510: 6465 7220 7468 6520 4170 6163 6865 204c  der the Apache L
+00000520: 6963 656e 7365 2c20 5665 7273 696f 6e20  icense, Version 
+00000530: 322e 3020 2874 6865 2022 4c69 6365 6e73  2.0 (the "Licens
+00000540: 6522 293b 0d0a 796f 7520 6d61 7920 6e6f  e");..you may no
+00000550: 7420 7573 6520 7468 6973 2066 696c 6520  t use this file 
+00000560: 6578 6365 7074 2069 6e20 636f 6d70 6c69  except in compli
+00000570: 616e 6365 2077 6974 6820 7468 6520 4c69  ance with the Li
+00000580: 6365 6e73 652e 0d0a 596f 7520 6d61 7920  cense...You may 
+00000590: 6f62 7461 696e 2061 2063 6f70 7920 6f66  obtain a copy of
+000005a0: 2074 6865 204c 6963 656e 7365 2061 740d   the License at.
+000005b0: 0a0d 0a20 2020 2068 7474 703a 2f2f 7777  ...    http://ww
+000005c0: 772e 6170 6163 6865 2e6f 7267 2f6c 6963  w.apache.org/lic
+000005d0: 656e 7365 732f 4c49 4345 4e53 452d 322e  enses/LICENSE-2.
+000005e0: 300d 0a0d 0a55 6e6c 6573 7320 7265 7175  0....Unless requ
+000005f0: 6972 6564 2062 7920 6170 706c 6963 6162  ired by applicab
+00000600: 6c65 206c 6177 206f 7220 6167 7265 6564  le law or agreed
+00000610: 2074 6f20 696e 2077 7269 7469 6e67 2c20   to in writing, 
+00000620: 736f 6674 7761 7265 0d0a 6469 7374 7269  software..distri
+00000630: 6275 7465 6420 756e 6465 7220 7468 6520  buted under the 
+00000640: 4c69 6365 6e73 6520 6973 2064 6973 7472  License is distr
+00000650: 6962 7574 6564 206f 6e20 616e 2022 4153  ibuted on an "AS
+00000660: 2049 5322 2042 4153 4953 2c0d 0a57 4954   IS" BASIS,..WIT
+00000670: 484f 5554 2057 4152 5241 4e54 4945 5320  HOUT WARRANTIES 
+00000680: 4f52 2043 4f4e 4449 5449 4f4e 5320 4f46  OR CONDITIONS OF
+00000690: 2041 4e59 204b 494e 442c 2065 6974 6865   ANY KIND, eithe
+000006a0: 7220 6578 7072 6573 7320 6f72 2069 6d70  r express or imp
+000006b0: 6c69 6564 2e0d 0a53 6565 2074 6865 204c  lied...See the L
+000006c0: 6963 656e 7365 2066 6f72 2074 6865 2073  icense for the s
+000006d0: 7065 6369 6669 6320 6c61 6e67 7561 6765  pecific language
+000006e0: 2067 6f76 6572 6e69 6e67 2070 6572 6d69   governing permi
+000006f0: 7373 696f 6e73 2061 6e64 0d0a 6c69 6d69  ssions and..limi
+00000700: 7461 7469 6f6e 7320 756e 6465 7220 7468  tations under th
+00000710: 6520 4c69 6365 6e73 652e 0d0a 2d2d 3e0d  e License...-->.
+00000720: 0a0d 0a3c 7020 616c 6967 6e3d 2263 656e  ...<p align="cen
+00000730: 7465 7222 3e0d 0a3c 696d 6720 7374 796c  ter">..<img styl
+00000740: 653d 2276 6572 7469 6361 6c2d 616c 6967  e="vertical-alig
+00000750: 6e3a 6d69 6464 6c65 2220 7372 633d 2268  n:middle" src="h
+00000760: 7474 7073 3a2f 2f72 6177 2e67 6974 6875  ttps://raw.githu
+00000770: 6275 7365 7263 6f6e 7465 6e74 2e63 6f6d  busercontent.com
+00000780: 2f41 6461 7074 6572 2d48 7562 2f61 6461  /Adapter-Hub/ada
+00000790: 7074 6572 732f 6d61 696e 2f64 6f63 732f  pters/main/docs/
+000007a0: 696d 672f 6164 6170 7465 722d 6265 7274  img/adapter-bert
+000007b0: 2e70 6e67 2220 7769 6474 683d 2238 3022  .png" width="80"
+000007c0: 202f 3e0d 0a3c 2f70 3e0d 0a3c 6831 2061   />..</p>..<h1 a
+000007d0: 6c69 676e 3d22 6365 6e74 6572 223e 0d0a  lign="center">..
+000007e0: 3c73 7061 6e3e 3c69 3e41 6461 7074 6572  <span><i>Adapter
+000007f0: 733c 2f69 3e3c 2f73 7061 6e3e 0d0a 3c2f  s</i></span>..</
+00000800: 6831 3e0d 0a0d 0a3c 6833 2061 6c69 676e  h1>....<h3 align
+00000810: 3d22 6365 6e74 6572 223e 0d0a 4120 556e  ="center">..A Un
+00000820: 6966 6965 6420 4c69 6272 6172 7920 666f  ified Library fo
+00000830: 7220 5061 7261 6d65 7465 722d 4566 6669  r Parameter-Effi
+00000840: 6369 656e 7420 616e 6420 4d6f 6475 6c61  cient and Modula
+00000850: 7220 5472 616e 7366 6572 204c 6561 726e  r Transfer Learn
+00000860: 696e 670d 0a3c 2f68 333e 0d0a 3c68 3320  ing..</h3>..<h3 
+00000870: 616c 6967 6e3d 2263 656e 7465 7222 3e0d  align="center">.
+00000880: 0a20 2020 203c 6120 6872 6566 3d22 6874  .    <a href="ht
+00000890: 7470 733a 2f2f 6164 6170 7465 7268 7562  tps://adapterhub
+000008a0: 2e6d 6c22 3e57 6562 7369 7465 3c2f 613e  .ml">Website</a>
+000008b0: 0d0a 2020 2020 266e 6273 703b 20e2 80a2  ..    &nbsp; ...
+000008c0: 2026 6e62 7370 3b0d 0a20 2020 203c 6120   &nbsp;..    <a 
+000008d0: 6872 6566 3d22 6874 7470 733a 2f2f 646f  href="https://do
+000008e0: 6373 2e61 6461 7074 6572 6875 622e 6d6c  cs.adapterhub.ml
+000008f0: 223e 446f 6375 6d65 6e74 6174 696f 6e3c  ">Documentation<
+00000900: 2f61 3e0d 0a20 2020 2026 6e62 7370 3b20  /a>..    &nbsp; 
+00000910: e280 a220 266e 6273 703b 0d0a 2020 2020  ... &nbsp;..    
+00000920: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
+00000930: 2f61 7278 6976 2e6f 7267 2f61 6273 2f32  /arxiv.org/abs/2
+00000940: 3331 312e 3131 3037 3722 3e50 6170 6572  311.11077">Paper
+00000950: 3c2f 613e 0d0a 3c2f 6833 3e0d 0a0d 0a21  </a>..</h3>....!
+00000960: 5b54 6573 7473 5d28 6874 7470 733a 2f2f  [Tests](https://
+00000970: 6769 7468 7562 2e63 6f6d 2f41 6461 7074  github.com/Adapt
+00000980: 6572 2d48 7562 2f61 6461 7074 6572 732f  er-Hub/adapters/
+00000990: 776f 726b 666c 6f77 732f 5465 7374 732f  workflows/Tests/
+000009a0: 6261 6467 652e 7376 673f 6272 616e 6368  badge.svg?branch
+000009b0: 3d61 6461 7074 6572 7329 0d0a 5b21 5b47  =adapters)..[![G
+000009c0: 6974 4875 625d 2868 7474 7073 3a2f 2f69  itHub](https://i
+000009d0: 6d67 2e73 6869 656c 6473 2e69 6f2f 6769  mg.shields.io/gi
+000009e0: 7468 7562 2f6c 6963 656e 7365 2f61 6461  thub/license/ada
+000009f0: 7074 6572 2d68 7562 2f61 6461 7074 6572  pter-hub/adapter
+00000a00: 732e 7376 673f 636f 6c6f 723d 626c 7565  s.svg?color=blue
+00000a10: 295d 2868 7474 7073 3a2f 2f67 6974 6875  )](https://githu
+00000a20: 622e 636f 6d2f 6164 6170 7465 722d 6875  b.com/adapter-hu
+00000a30: 622f 6164 6170 7465 7273 2f62 6c6f 622f  b/adapters/blob/
+00000a40: 6d61 696e 2f4c 4943 454e 5345 290d 0a5b  main/LICENSE)..[
+00000a50: 215b 5079 5049 5d28 6874 7470 733a 2f2f  ![PyPI](https://
+00000a60: 696d 672e 7368 6965 6c64 732e 696f 2f70  img.shields.io/p
+00000a70: 7970 692f 762f 6164 6170 7465 7273 295d  ypi/v/adapters)]
+00000a80: 2868 7474 7073 3a2f 2f70 7970 692e 6f72  (https://pypi.or
+00000a90: 672f 7072 6f6a 6563 742f 6164 6170 7465  g/project/adapte
+00000aa0: 7273 2f29 0d0a 0d0a 5f41 6461 7074 6572  rs/)...._Adapter
+00000ab0: 735f 2069 7320 616e 2061 6464 2d6f 6e20  s_ is an add-on 
+00000ac0: 6c69 6272 6172 7920 746f 205b 4875 6767  library to [Hugg
+00000ad0: 696e 6746 6163 6527 7320 5472 616e 7366  ingFace's Transf
+00000ae0: 6f72 6d65 7273 5d28 6874 7470 733a 2f2f  ormers](https://
+00000af0: 6769 7468 7562 2e63 6f6d 2f68 7567 6769  github.com/huggi
+00000b00: 6e67 6661 6365 2f74 7261 6e73 666f 726d  ngface/transform
+00000b10: 6572 7329 2c20 696e 7465 6772 6174 696e  ers), integratin
+00000b20: 6720 5b76 6172 696f 7573 2061 6461 7074  g [various adapt
+00000b30: 6572 206d 6574 686f 6473 5d28 6874 7470  er methods](http
+00000b40: 733a 2f2f 646f 6373 2e61 6461 7074 6572  s://docs.adapter
+00000b50: 6875 622e 6d6c 2f6f 7665 7276 6965 772e  hub.ml/overview.
+00000b60: 6874 6d6c 2920 696e 746f 205b 7374 6174  html) into [stat
+00000b70: 652d 6f66 2d74 6865 2d61 7274 2070 7265  e-of-the-art pre
+00000b80: 2d74 7261 696e 6564 206c 616e 6775 6167  -trained languag
+00000b90: 6520 6d6f 6465 6c73 5d28 6874 7470 733a  e models](https:
+00000ba0: 2f2f 646f 6373 2e61 6461 7074 6572 6875  //docs.adapterhu
+00000bb0: 622e 6d6c 2f6d 6f64 656c 5f6f 7665 7276  b.ml/model_overv
+00000bc0: 6965 772e 6874 6d6c 2920 7769 7468 206d  iew.html) with m
+00000bd0: 696e 696d 616c 2063 6f64 696e 6720 6f76  inimal coding ov
+00000be0: 6572 6865 6164 2066 6f72 2074 7261 696e  erhead for train
+00000bf0: 696e 6720 616e 6420 696e 6665 7265 6e63  ing and inferenc
+00000c00: 652e 0d0a 0d0a 3e20 2a2a 4e6f 7465 2a2a  e.....> **Note**
+00000c10: 3a20 5468 6520 5f41 6461 7074 6572 735f  : The _Adapters_
+00000c20: 206c 6962 7261 7279 2068 6173 2072 6570   library has rep
+00000c30: 6c61 6365 6420 7468 6520 6061 6461 7074  laced the `adapt
+00000c40: 6572 2d74 7261 6e73 666f 726d 6572 7360  er-transformers`
+00000c50: 2070 6163 6b61 6765 2e20 416c 6c20 7072   package. All pr
+00000c60: 6576 696f 7573 6c79 2074 7261 696e 6564  eviously trained
+00000c70: 2061 6461 7074 6572 7320 6172 6520 636f   adapters are co
+00000c80: 6d70 6174 6962 6c65 2077 6974 6820 7468  mpatible with th
+00000c90: 6520 6e65 7720 6c69 6272 6172 792e 2046  e new library. F
+00000ca0: 6f72 2074 7261 6e73 6974 696f 6e69 6e67  or transitioning
+00000cb0: 2c20 706c 6561 7365 2072 6561 643a 2068  , please read: h
+00000cc0: 7474 7073 3a2f 2f64 6f63 732e 6164 6170  ttps://docs.adap
+00000cd0: 7465 7268 7562 2e6d 6c2f 7472 616e 7369  terhub.ml/transi
+00000ce0: 7469 6f6e 696e 672e 6874 6d6c 2e0d 0a0d  tioning.html....
+00000cf0: 0a23 2320 496e 7374 616c 6c61 7469 6f6e  .## Installation
+00000d00: 0d0a 0d0a 6061 6461 7074 6572 7360 2063  ....`adapters` c
+00000d10: 7572 7265 6e74 6c79 2073 7570 706f 7274  urrently support
+00000d20: 7320 2a2a 5079 7468 6f6e 2033 2e38 2b2a  s **Python 3.8+*
+00000d30: 2a20 616e 6420 2a2a 5079 546f 7263 6820  * and **PyTorch 
+00000d40: 312e 3130 2b2a 2a2e 0d0a 4166 7465 7220  1.10+**...After 
+00000d50: 5b69 6e73 7461 6c6c 696e 6720 5079 546f  [installing PyTo
+00000d60: 7263 685d 2868 7474 7073 3a2f 2f70 7974  rch](https://pyt
+00000d70: 6f72 6368 2e6f 7267 2f67 6574 2d73 7461  orch.org/get-sta
+00000d80: 7274 6564 2f6c 6f63 616c 6c79 2f29 2c20  rted/locally/), 
+00000d90: 796f 7520 6361 6e20 696e 7374 616c 6c20  you can install 
+00000da0: 6061 6461 7074 6572 7360 2066 726f 6d20  `adapters` from 
+00000db0: 5079 5049 202e 2e2e 0d0a 0d0a 6060 600d  PyPI .......```.
+00000dc0: 0a70 6970 2069 6e73 7461 6c6c 202d 5520  .pip install -U 
+00000dd0: 6164 6170 7465 7273 0d0a 6060 600d 0a0d  adapters..```...
+00000de0: 0a2e 2e2e 206f 7220 6672 6f6d 2073 6f75  .... or from sou
+00000df0: 7263 6520 6279 2063 6c6f 6e69 6e67 2074  rce by cloning t
+00000e00: 6865 2072 6570 6f73 6974 6f72 793a 0d0a  he repository:..
+00000e10: 0d0a 6060 600d 0a67 6974 2063 6c6f 6e65  ..```..git clone
+00000e20: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
+00000e30: 636f 6d2f 6164 6170 7465 722d 6875 622f  com/adapter-hub/
+00000e40: 6164 6170 7465 7273 2e67 6974 0d0a 6364  adapters.git..cd
+00000e50: 2061 6461 7074 6572 730d 0a70 6970 2069   adapters..pip i
+00000e60: 6e73 7461 6c6c 202e 0d0a 6060 600d 0a0d  nstall ...```...
+00000e70: 0a23 2320 5175 6963 6b20 546f 7572 0d0a  .## Quick Tour..
+00000e80: 0d0a 2323 2323 204c 6f61 6420 7072 652d  ..#### Load pre-
+00000e90: 7472 6169 6e65 6420 6164 6170 7465 7273  trained adapters
+00000ea0: 3a0d 0a0d 0a60 6060 7079 7468 6f6e 0d0a  :....```python..
+00000eb0: 6672 6f6d 2061 6461 7074 6572 7320 696d  from adapters im
+00000ec0: 706f 7274 2041 7574 6f41 6461 7074 6572  port AutoAdapter
+00000ed0: 4d6f 6465 6c0d 0a66 726f 6d20 7472 616e  Model..from tran
+00000ee0: 7366 6f72 6d65 7273 2069 6d70 6f72 7420  sformers import 
+00000ef0: 4175 746f 546f 6b65 6e69 7a65 720d 0a0d  AutoTokenizer...
+00000f00: 0a6d 6f64 656c 203d 2041 7574 6f41 6461  .model = AutoAda
+00000f10: 7074 6572 4d6f 6465 6c2e 6672 6f6d 5f70  pterModel.from_p
+00000f20: 7265 7472 6169 6e65 6428 2272 6f62 6572  retrained("rober
+00000f30: 7461 2d62 6173 6522 290d 0a74 6f6b 656e  ta-base")..token
+00000f40: 697a 6572 203d 2041 7574 6f54 6f6b 656e  izer = AutoToken
+00000f50: 697a 6572 2e66 726f 6d5f 7072 6574 7261  izer.from_pretra
+00000f60: 696e 6564 2822 726f 6265 7274 612d 6261  ined("roberta-ba
+00000f70: 7365 2229 0d0a 0d0a 6d6f 6465 6c2e 6c6f  se")....model.lo
+00000f80: 6164 5f61 6461 7074 6572 2822 4164 6170  ad_adapter("Adap
+00000f90: 7465 7248 7562 2f72 6f62 6572 7461 2d62  terHub/roberta-b
+00000fa0: 6173 652d 7066 2d69 6d64 6222 2c20 736f  ase-pf-imdb", so
+00000fb0: 7572 6365 3d22 6866 222c 2073 6574 5f61  urce="hf", set_a
+00000fc0: 6374 6976 653d 5472 7565 290d 0a0d 0a70  ctive=True)....p
+00000fd0: 7269 6e74 286d 6f64 656c 282a 2a74 6f6b  rint(model(**tok
+00000fe0: 656e 697a 6572 2822 5468 6973 2077 6f72  enizer("This wor
+00000ff0: 6b73 2067 7265 6174 2122 2c20 7265 7475  ks great!", retu
+00001000: 726e 5f74 656e 736f 7273 3d22 7074 2229  rn_tensors="pt")
+00001010: 292e 6c6f 6769 7473 290d 0a60 6060 0d0a  ).logits)..```..
+00001020: 0d0a 2a2a 5b4c 6561 726e 204d 6f72 655d  ..**[Learn More]
+00001030: 2868 7474 7073 3a2f 2f64 6f63 732e 6164  (https://docs.ad
+00001040: 6170 7465 7268 7562 2e6d 6c2f 6c6f 6164  apterhub.ml/load
+00001050: 696e 672e 6874 6d6c 292a 2a0d 0a0d 0a23  ing.html)**....#
+00001060: 2323 2320 4164 6170 7420 6578 6973 7469  ### Adapt existi
+00001070: 6e67 206d 6f64 656c 2073 6574 7570 733a  ng model setups:
+00001080: 0d0a 0d0a 6060 6070 7974 686f 6e0d 0a69  ....```python..i
+00001090: 6d70 6f72 7420 6164 6170 7465 7273 0d0a  mport adapters..
+000010a0: 6672 6f6d 2074 7261 6e73 666f 726d 6572  from transformer
+000010b0: 7320 696d 706f 7274 2041 7574 6f4d 6f64  s import AutoMod
+000010c0: 656c 466f 7253 6571 7565 6e63 6543 6c61  elForSequenceCla
+000010d0: 7373 6966 6963 6174 696f 6e0d 0a0d 0a6d  ssification....m
+000010e0: 6f64 656c 203d 2041 7574 6f4d 6f64 656c  odel = AutoModel
+000010f0: 466f 7253 6571 7565 6e63 6543 6c61 7373  ForSequenceClass
+00001100: 6966 6963 6174 696f 6e2e 6672 6f6d 5f70  ification.from_p
+00001110: 7265 7472 6169 6e65 6428 2274 352d 6261  retrained("t5-ba
+00001120: 7365 2229 0d0a 0d0a 6164 6170 7465 7273  se")....adapters
+00001130: 2e69 6e69 7428 6d6f 6465 6c29 0d0a 0d0a  .init(model)....
+00001140: 6d6f 6465 6c2e 6164 645f 6164 6170 7465  model.add_adapte
+00001150: 7228 226d 795f 6c6f 7261 5f61 6461 7074  r("my_lora_adapt
+00001160: 6572 222c 2063 6f6e 6669 673d 226c 6f72  er", config="lor
+00001170: 6122 290d 0a6d 6f64 656c 2e74 7261 696e  a")..model.train
+00001180: 5f61 6461 7074 6572 2822 6d79 5f6c 6f72  _adapter("my_lor
+00001190: 615f 6164 6170 7465 7222 290d 0a0d 0a23  a_adapter")....#
+000011a0: 2059 6f75 7220 7265 6775 6c61 7220 7472   Your regular tr
+000011b0: 6169 6e69 6e67 206c 6f6f 702e 2e2e 0d0a  aining loop.....
+000011c0: 6060 600d 0a0d 0a2a 2a5b 4c65 6172 6e20  ```....**[Learn 
+000011d0: 4d6f 7265 5d28 6874 7470 733a 2f2f 646f  More](https://do
+000011e0: 6373 2e61 6461 7074 6572 6875 622e 6d6c  cs.adapterhub.ml
+000011f0: 2f71 7569 636b 7374 6172 742e 6874 6d6c  /quickstart.html
+00001200: 292a 2a0d 0a0d 0a23 2323 2320 466c 6578  )**....#### Flex
+00001210: 6962 6c79 2063 6f6e 6669 6775 7265 2061  ibly configure a
+00001220: 6461 7074 6572 733a 0d0a 0d0a 6060 6070  dapters:....```p
+00001230: 7974 686f 6e0d 0a66 726f 6d20 6164 6170  ython..from adap
+00001240: 7465 7273 2069 6d70 6f72 7420 436f 6e66  ters import Conf
+00001250: 6967 556e 696f 6e2c 2050 7265 6669 7854  igUnion, PrefixT
+00001260: 756e 696e 6743 6f6e 6669 672c 2050 6172  uningConfig, Par
+00001270: 426e 436f 6e66 6967 2c20 4175 746f 4164  BnConfig, AutoAd
+00001280: 6170 7465 724d 6f64 656c 0d0a 0d0a 6d6f  apterModel....mo
+00001290: 6465 6c20 3d20 4175 746f 4164 6170 7465  del = AutoAdapte
+000012a0: 724d 6f64 656c 2e66 726f 6d5f 7072 6574  rModel.from_pret
+000012b0: 7261 696e 6564 2822 6d69 6372 6f73 6f66  rained("microsof
+000012c0: 742f 6465 6265 7274 612d 7633 2d62 6173  t/deberta-v3-bas
+000012d0: 6522 290d 0a0d 0a61 6461 7074 6572 5f63  e")....adapter_c
+000012e0: 6f6e 6669 6720 3d20 436f 6e66 6967 556e  onfig = ConfigUn
+000012f0: 696f 6e28 0d0a 2020 2020 5072 6566 6978  ion(..    Prefix
+00001300: 5475 6e69 6e67 436f 6e66 6967 2870 7265  TuningConfig(pre
+00001310: 6669 785f 6c65 6e67 7468 3d32 3029 2c0d  fix_length=20),.
+00001320: 0a20 2020 2050 6172 426e 436f 6e66 6967  .    ParBnConfig
+00001330: 2872 6564 7563 7469 6f6e 5f66 6163 746f  (reduction_facto
+00001340: 723d 3429 2c0d 0a29 0d0a 6d6f 6465 6c2e  r=4),..)..model.
+00001350: 6164 645f 6164 6170 7465 7228 226d 795f  add_adapter("my_
+00001360: 6164 6170 7465 7222 2c20 636f 6e66 6967  adapter", config
+00001370: 3d61 6461 7074 6572 5f63 6f6e 6669 672c  =adapter_config,
+00001380: 2073 6574 5f61 6374 6976 653d 5472 7565   set_active=True
+00001390: 290d 0a60 6060 0d0a 0d0a 2a2a 5b4c 6561  )..```....**[Lea
+000013a0: 726e 204d 6f72 655d 2868 7474 7073 3a2f  rn More](https:/
+000013b0: 2f64 6f63 732e 6164 6170 7465 7268 7562  /docs.adapterhub
+000013c0: 2e6d 6c2f 6f76 6572 7669 6577 2e68 746d  .ml/overview.htm
+000013d0: 6c29 2a2a 0d0a 0d0a 2323 2323 2045 6173  l)**....#### Eas
+000013e0: 696c 7920 636f 6d70 6f73 6520 6164 6170  ily compose adap
+000013f0: 7465 7273 2069 6e20 6120 7369 6e67 6c65  ters in a single
+00001400: 206d 6f64 656c 3a0d 0a0d 0a60 6060 7079   model:....```py
+00001410: 7468 6f6e 0d0a 6672 6f6d 2061 6461 7074  thon..from adapt
+00001420: 6572 7320 696d 706f 7274 2041 6461 7074  ers import Adapt
+00001430: 6572 5365 7475 702c 2041 7574 6f41 6461  erSetup, AutoAda
+00001440: 7074 6572 4d6f 6465 6c0d 0a69 6d70 6f72  pterModel..impor
+00001450: 7420 6164 6170 7465 7273 2e63 6f6d 706f  t adapters.compo
+00001460: 7369 7469 6f6e 2061 7320 6163 0d0a 0d0a  sition as ac....
+00001470: 6d6f 6465 6c20 3d20 4175 746f 4164 6170  model = AutoAdap
+00001480: 7465 724d 6f64 656c 2e66 726f 6d5f 7072  terModel.from_pr
+00001490: 6574 7261 696e 6564 2822 726f 6265 7274  etrained("robert
+000014a0: 612d 6261 7365 2229 0d0a 0d0a 7163 203d  a-base")....qc =
+000014b0: 206d 6f64 656c 2e6c 6f61 645f 6164 6170   model.load_adap
+000014c0: 7465 7228 2241 6461 7074 6572 4875 622f  ter("AdapterHub/
+000014d0: 726f 6265 7274 612d 6261 7365 2d70 662d  roberta-base-pf-
+000014e0: 7472 6563 2229 0d0a 7365 6e74 203d 206d  trec")..sent = m
+000014f0: 6f64 656c 2e6c 6f61 645f 6164 6170 7465  odel.load_adapte
+00001500: 7228 2241 6461 7074 6572 4875 622f 726f  r("AdapterHub/ro
+00001510: 6265 7274 612d 6261 7365 2d70 662d 696d  berta-base-pf-im
+00001520: 6462 2229 0d0a 0d0a 7769 7468 2041 6461  db")....with Ada
+00001530: 7074 6572 5365 7475 7028 6163 2e50 6172  pterSetup(ac.Par
+00001540: 616c 6c65 6c28 7163 2c20 7365 6e74 2929  allel(qc, sent))
+00001550: 3a0d 0a20 2020 2070 7269 6e74 286d 6f64  :..    print(mod
+00001560: 656c 282a 2a74 6f6b 656e 697a 6572 2822  el(**tokenizer("
+00001570: 5768 6174 2069 7320 4164 6170 7465 7248  What is AdapterH
+00001580: 7562 3f22 2c20 7265 7475 726e 5f74 656e  ub?", return_ten
+00001590: 736f 7273 3d22 7074 2229 2929 0d0a 6060  sors="pt")))..``
+000015a0: 600d 0a0d 0a2a 2a5b 4c65 6172 6e20 4d6f  `....**[Learn Mo
+000015b0: 7265 5d28 6874 7470 733a 2f2f 646f 6373  re](https://docs
+000015c0: 2e61 6461 7074 6572 6875 622e 6d6c 2f61  .adapterhub.ml/a
+000015d0: 6461 7074 6572 5f63 6f6d 706f 7369 7469  dapter_compositi
+000015e0: 6f6e 2e68 746d 6c29 2a2a 0d0a 0d0a 2323  on.html)**....##
+000015f0: 2055 7365 6675 6c20 5265 736f 7572 6365   Useful Resource
+00001600: 730d 0a0d 0a48 7567 6769 6e67 4661 6365  s....HuggingFace
+00001610: 2773 2067 7265 6174 2064 6f63 756d 656e  's great documen
+00001620: 7461 7469 6f6e 206f 6e20 6765 7474 696e  tation on gettin
+00001630: 6720 7374 6172 7465 6420 7769 7468 205f  g started with _
+00001640: 5472 616e 7366 6f72 6d65 7273 5f20 6361  Transformers_ ca
+00001650: 6e20 6265 2066 6f75 6e64 205b 6865 7265  n be found [here
+00001660: 5d28 6874 7470 733a 2f2f 6875 6767 696e  ](https://huggin
+00001670: 6766 6163 652e 636f 2f74 7261 6e73 666f  gface.co/transfo
+00001680: 726d 6572 732f 696e 6465 782e 6874 6d6c  rmers/index.html
+00001690: 292e 2060 6164 6170 7465 7273 6020 6973  ). `adapters` is
+000016a0: 2066 756c 6c79 2063 6f6d 7061 7469 626c   fully compatibl
+000016b0: 6520 7769 7468 205f 5472 616e 7366 6f72  e with _Transfor
+000016c0: 6d65 7273 5f2e 0d0a 0d0a 546f 2067 6574  mers_.....To get
+000016d0: 2073 7461 7274 6564 2077 6974 6820 6164   started with ad
+000016e0: 6170 7465 7273 2c20 7265 6665 7220 746f  apters, refer to
+000016f0: 2074 6865 7365 206c 6f63 6174 696f 6e73   these locations
+00001700: 3a0d 0a0d 0a2d 202a 2a5b 436f 6c61 6220  :....- **[Colab 
+00001710: 6e6f 7465 626f 6f6b 2074 7574 6f72 6961  notebook tutoria
+00001720: 6c73 5d28 6874 7470 733a 2f2f 6769 7468  ls](https://gith
+00001730: 7562 2e63 6f6d 2f41 6461 7074 6572 2d48  ub.com/Adapter-H
+00001740: 7562 2f61 6461 7074 6572 732f 7472 6565  ub/adapters/tree
+00001750: 2f6d 6169 6e2f 6e6f 7465 626f 6f6b 7329  /main/notebooks)
+00001760: 2a2a 2c20 6120 7365 7269 6573 206e 6f74  **, a series not
+00001770: 6562 6f6f 6b73 2070 726f 7669 6469 6e67  ebooks providing
+00001780: 2061 6e20 696e 7472 6f64 7563 7469 6f6e   an introduction
+00001790: 2074 6f20 616c 6c20 7468 6520 6d61 696e   to all the main
+000017a0: 2063 6f6e 6365 7074 7320 6f66 2028 6164   concepts of (ad
+000017b0: 6170 7465 722d 2974 7261 6e73 666f 726d  apter-)transform
+000017c0: 6572 7320 616e 6420 4164 6170 7465 7248  ers and AdapterH
+000017d0: 7562 0d0a 2d20 2a2a 6874 7470 733a 2f2f  ub..- **https://
+000017e0: 646f 6373 2e61 6461 7074 6572 6875 622e  docs.adapterhub.
+000017f0: 6d6c 2a2a 2c20 6f75 7220 646f 6375 6d65  ml**, our docume
+00001800: 6e74 6174 696f 6e20 6f6e 2074 7261 696e  ntation on train
+00001810: 696e 6720 616e 6420 7573 696e 6720 6164  ing and using ad
+00001820: 6170 7465 7273 2077 6974 6820 5f61 6461  apters with _ada
+00001830: 7074 6572 735f 0d0a 2d20 2a2a 6874 7470  pters_..- **http
+00001840: 733a 2f2f 6164 6170 7465 7268 7562 2e6d  s://adapterhub.m
+00001850: 6c2a 2a20 746f 2065 7870 6c6f 7265 2061  l** to explore a
+00001860: 7661 696c 6162 6c65 2070 7265 2d74 7261  vailable pre-tra
+00001870: 696e 6564 2061 6461 7074 6572 206d 6f64  ined adapter mod
+00001880: 756c 6573 2061 6e64 2073 6861 7265 2079  ules and share y
+00001890: 6f75 7220 6f77 6e20 6164 6170 7465 7273  our own adapters
+000018a0: 0d0a 2d20 2a2a 5b45 7861 6d70 6c65 7320  ..- **[Examples 
+000018b0: 666f 6c64 6572 5d28 6874 7470 733a 2f2f  folder](https://
+000018c0: 6769 7468 7562 2e63 6f6d 2f41 6461 7074  github.com/Adapt
+000018d0: 6572 2d48 7562 2f61 6461 7074 6572 732f  er-Hub/adapters/
+000018e0: 7472 6565 2f6d 6169 6e2f 6578 616d 706c  tree/main/exampl
+000018f0: 6573 2f70 7974 6f72 6368 292a 2a20 6f66  es/pytorch)** of
+00001900: 2074 6869 7320 7265 706f 7369 746f 7279   this repository
+00001910: 2063 6f6e 7461 696e 696e 6720 4875 6767   containing Hugg
+00001920: 696e 6746 6163 6527 7320 6578 616d 706c  ingFace's exampl
+00001930: 6520 7472 6169 6e69 6e67 2073 6372 6970  e training scrip
+00001940: 7473 2c20 6d61 6e79 2061 6461 7074 6564  ts, many adapted
+00001950: 2066 6f72 2074 7261 696e 696e 6720 6164   for training ad
+00001960: 6170 7465 7273 0d0a 0d0a 2323 2049 6d70  apters....## Imp
+00001970: 6c65 6d65 6e74 6564 204d 6574 686f 6473  lemented Methods
+00001980: 0d0a 0d0a 4375 7272 656e 746c 792c 2061  ....Currently, a
+00001990: 6461 7074 6572 7320 696e 7465 6772 6174  dapters integrat
+000019a0: 6573 2061 6c6c 2061 7263 6869 7465 6374  es all architect
+000019b0: 7572 6573 2061 6e64 206d 6574 686f 6473  ures and methods
+000019c0: 206c 6973 7465 6420 6265 6c6f 773a 0d0a   listed below:..
+000019d0: 0d0a 7c20 4d65 7468 6f64 207c 2050 6170  ..| Method | Pap
+000019e0: 6572 2873 2920 7c20 5175 6963 6b20 4c69  er(s) | Quick Li
+000019f0: 6e6b 7320 7c0d 0a7c 202d 2d2d 207c 202d  nks |..| --- | -
+00001a00: 2d2d 207c 202d 2d2d 207c 0d0a 7c20 426f  -- | --- |..| Bo
+00001a10: 7474 6c65 6e65 636b 2061 6461 7074 6572  ttleneck adapter
+00001a20: 7320 7c20 5b48 6f75 6c73 6279 2065 7420  s | [Houlsby et 
+00001a30: 616c 2e20 2832 3031 3929 5d28 6874 7470  al. (2019)](http
+00001a40: 733a 2f2f 6172 7869 762e 6f72 672f 7064  s://arxiv.org/pd
+00001a50: 662f 3139 3032 2e30 3037 3531 2e70 6466  f/1902.00751.pdf
+00001a60: 293c 6272 3e20 5b42 6170 6e61 2061 6e64  )<br> [Bapna and
+00001a70: 2046 6972 6174 2028 3230 3139 295d 2868   Firat (2019)](h
+00001a80: 7474 7073 3a2f 2f61 7278 6976 2e6f 7267  ttps://arxiv.org
+00001a90: 2f70 6466 2f31 3930 392e 3038 3437 382e  /pdf/1909.08478.
+00001aa0: 7064 6629 207c 205b 5175 6963 6b73 7461  pdf) | [Quicksta
+00001ab0: 7274 5d28 6874 7470 733a 2f2f 646f 6373  rt](https://docs
+00001ac0: 2e61 6461 7074 6572 6875 622e 6d6c 2f71  .adapterhub.ml/q
+00001ad0: 7569 636b 7374 6172 742e 6874 6d6c 292c  uickstart.html),
+00001ae0: 205b 4e6f 7465 626f 6f6b 5d28 6874 7470   [Notebook](http
+00001af0: 733a 2f2f 636f 6c61 622e 7265 7365 6172  s://colab.resear
+00001b00: 6368 2e67 6f6f 676c 652e 636f 6d2f 6769  ch.google.com/gi
+00001b10: 7468 7562 2f41 6461 7074 6572 2d48 7562  thub/Adapter-Hub
+00001b20: 2f61 6461 7074 6572 732f 626c 6f62 2f6d  /adapters/blob/m
+00001b30: 6169 6e2f 6e6f 7465 626f 6f6b 732f 3031  ain/notebooks/01
+00001b40: 5f41 6461 7074 6572 5f54 7261 696e 696e  _Adapter_Trainin
+00001b50: 672e 6970 796e 6229 207c 0d0a 7c20 4164  g.ipynb) |..| Ad
+00001b60: 6170 7465 7246 7573 696f 6e20 7c20 5b50  apterFusion | [P
+00001b70: 6665 6966 6665 7220 6574 2061 6c2e 2028  feiffer et al. (
+00001b80: 3230 3231 295d 2868 7474 7073 3a2f 2f61  2021)](https://a
+00001b90: 636c 616e 7468 6f6c 6f67 792e 6f72 672f  clanthology.org/
+00001ba0: 3230 3231 2e65 6163 6c2d 6d61 696e 2e33  2021.eacl-main.3
+00001bb0: 392e 7064 6629 207c 205b 446f 6373 3a20  9.pdf) | [Docs: 
+00001bc0: 5472 6169 6e69 6e67 5d28 6874 7470 733a  Training](https:
+00001bd0: 2f2f 646f 6373 2e61 6461 7074 6572 6875  //docs.adapterhu
+00001be0: 622e 6d6c 2f74 7261 696e 696e 672e 6874  b.ml/training.ht
+00001bf0: 6d6c 2374 7261 696e 2d61 6461 7074 6572  ml#train-adapter
+00001c00: 6675 7369 6f6e 292c 205b 4e6f 7465 626f  fusion), [Notebo
+00001c10: 6f6b 5d28 6874 7470 733a 2f2f 636f 6c61  ok](https://cola
+00001c20: 622e 7265 7365 6172 6368 2e67 6f6f 676c  b.research.googl
+00001c30: 652e 636f 6d2f 6769 7468 7562 2f41 6461  e.com/github/Ada
+00001c40: 7074 6572 2d48 7562 2f61 6461 7074 6572  pter-Hub/adapter
+00001c50: 732f 626c 6f62 2f6d 6169 6e2f 6e6f 7465  s/blob/main/note
+00001c60: 626f 6f6b 732f 3033 5f41 6461 7074 6572  books/03_Adapter
+00001c70: 5f46 7573 696f 6e2e 6970 796e 6229 207c  _Fusion.ipynb) |
+00001c80: 0d0a 7c20 4d41 442d 582c 3c62 723e 2049  ..| MAD-X,<br> I
+00001c90: 6e76 6572 7469 626c 6520 6164 6170 7465  nvertible adapte
+00001ca0: 7273 207c 205b 5066 6569 6666 6572 2065  rs | [Pfeiffer e
+00001cb0: 7420 616c 2e20 2832 3032 3029 5d28 6874  t al. (2020)](ht
+00001cc0: 7470 733a 2f2f 6163 6c61 6e74 686f 6c6f  tps://aclantholo
+00001cd0: 6779 2e6f 7267 2f32 3032 302e 656d 6e6c  gy.org/2020.emnl
+00001ce0: 702d 6d61 696e 2e36 3137 2f29 207c 205b  p-main.617/) | [
+00001cf0: 4e6f 7465 626f 6f6b 5d28 6874 7470 733a  Notebook](https:
+00001d00: 2f2f 636f 6c61 622e 7265 7365 6172 6368  //colab.research
+00001d10: 2e67 6f6f 676c 652e 636f 6d2f 6769 7468  .google.com/gith
+00001d20: 7562 2f41 6461 7074 6572 2d48 7562 2f61  ub/Adapter-Hub/a
+00001d30: 6461 7074 6572 732f 626c 6f62 2f6d 6169  dapters/blob/mai
+00001d40: 6e2f 6e6f 7465 626f 6f6b 732f 3034 5f43  n/notebooks/04_C
+00001d50: 726f 7373 5f4c 696e 6775 616c 5f54 7261  ross_Lingual_Tra
+00001d60: 6e73 6665 722e 6970 796e 6229 207c 0d0a  nsfer.ipynb) |..
+00001d70: 7c20 4164 6170 7465 7244 726f 7020 7c20  | AdapterDrop | 
+00001d80: 5b52 c3bc 636b 6cc3 a920 6574 2061 6c2e  [R..ckl.. et al.
+00001d90: 2028 3230 3231 295d 2868 7474 7073 3a2f   (2021)](https:/
+00001da0: 2f61 7278 6976 2e6f 7267 2f70 6466 2f32  /arxiv.org/pdf/2
+00001db0: 3031 302e 3131 3931 382e 7064 6629 207c  010.11918.pdf) |
+00001dc0: 205b 4e6f 7465 626f 6f6b 5d28 6874 7470   [Notebook](http
+00001dd0: 733a 2f2f 636f 6c61 622e 7265 7365 6172  s://colab.resear
+00001de0: 6368 2e67 6f6f 676c 652e 636f 6d2f 6769  ch.google.com/gi
+00001df0: 7468 7562 2f41 6461 7074 6572 2d48 7562  thub/Adapter-Hub
+00001e00: 2f61 6461 7074 6572 732f 626c 6f62 2f6d  /adapters/blob/m
+00001e10: 6169 6e2f 6e6f 7465 626f 6f6b 732f 3035  ain/notebooks/05
+00001e20: 5f41 6461 7074 6572 5f44 726f 705f 5472  _Adapter_Drop_Tr
+00001e30: 6169 6e69 6e67 2e69 7079 6e62 2920 7c0d  aining.ipynb) |.
+00001e40: 0a7c 204d 4144 2d58 2032 2e30 2c3c 6272  .| MAD-X 2.0,<br
+00001e50: 3e20 456d 6265 6464 696e 6720 7472 6169  > Embedding trai
+00001e60: 6e69 6e67 207c 205b 5066 6569 6666 6572  ning | [Pfeiffer
+00001e70: 2065 7420 616c 2e20 2832 3032 3129 5d28   et al. (2021)](
+00001e80: 6874 7470 733a 2f2f 6172 7869 762e 6f72  https://arxiv.or
+00001e90: 672f 7064 662f 3230 3132 2e31 3535 3632  g/pdf/2012.15562
+00001ea0: 2e70 6466 2920 7c20 5b44 6f63 733a 2045  .pdf) | [Docs: E
+00001eb0: 6d62 6564 6469 6e67 735d 2868 7474 7073  mbeddings](https
+00001ec0: 3a2f 2f64 6f63 732e 6164 6170 7465 7268  ://docs.adapterh
+00001ed0: 7562 2e6d 6c2f 656d 6265 6464 696e 6773  ub.ml/embeddings
+00001ee0: 2e68 746d 6c29 2c20 5b4e 6f74 6562 6f6f  .html), [Noteboo
+00001ef0: 6b5d 2868 7474 7073 3a2f 2f63 6f6c 6162  k](https://colab
+00001f00: 2e72 6573 6561 7263 682e 676f 6f67 6c65  .research.google
+00001f10: 2e63 6f6d 2f67 6974 6875 622f 4164 6170  .com/github/Adap
+00001f20: 7465 722d 4875 622f 6164 6170 7465 7273  ter-Hub/adapters
+00001f30: 2f62 6c6f 622f 6d61 696e 2f6e 6f74 6562  /blob/main/noteb
+00001f40: 6f6f 6b73 2f30 385f 4e45 525f 5769 6b69  ooks/08_NER_Wiki
+00001f50: 616e 6e2e 6970 796e 6229 207c 0d0a 7c20  ann.ipynb) |..| 
+00001f60: 5072 6566 6978 2054 756e 696e 6720 7c20  Prefix Tuning | 
+00001f70: 5b4c 6920 616e 6420 4c69 616e 6720 2832  [Li and Liang (2
+00001f80: 3032 3129 5d28 6874 7470 733a 2f2f 6172  021)](https://ar
+00001f90: 7869 762e 6f72 672f 7064 662f 3231 3031  xiv.org/pdf/2101
+00001fa0: 2e30 3031 3930 2e70 6466 2920 7c20 5b44  .00190.pdf) | [D
+00001fb0: 6f63 735d 2868 7474 7073 3a2f 2f64 6f63  ocs](https://doc
+00001fc0: 732e 6164 6170 7465 7268 7562 2e6d 6c2f  s.adapterhub.ml/
+00001fd0: 6d65 7468 6f64 732e 6874 6d6c 2370 7265  methods.html#pre
+00001fe0: 6669 782d 7475 6e69 6e67 2920 7c0d 0a7c  fix-tuning) |..|
+00001ff0: 2050 6172 616c 6c65 6c20 6164 6170 7465   Parallel adapte
+00002000: 7273 2c3c 6272 3e20 4d69 782d 616e 642d  rs,<br> Mix-and-
+00002010: 4d61 7463 6820 6164 6170 7465 7273 207c  Match adapters |
+00002020: 205b 4865 2065 7420 616c 2e20 2832 3032   [He et al. (202
+00002030: 3129 5d28 6874 7470 733a 2f2f 6172 7869  1)](https://arxi
+00002040: 762e 6f72 672f 7064 662f 3231 3130 2e30  v.org/pdf/2110.0
+00002050: 3433 3636 2e70 6466 2920 7c20 5b44 6f63  4366.pdf) | [Doc
+00002060: 735d 2868 7474 7073 3a2f 2f64 6f63 732e  s](https://docs.
+00002070: 6164 6170 7465 7268 7562 2e6d 6c2f 6d65  adapterhub.ml/me
+00002080: 7468 6f64 5f63 6f6d 6269 6e61 7469 6f6e  thod_combination
+00002090: 732e 6874 6d6c 236d 6978 2d61 6e64 2d6d  s.html#mix-and-m
+000020a0: 6174 6368 2d61 6461 7074 6572 7329 207c  atch-adapters) |
+000020b0: 0d0a 7c20 436f 6d70 6163 7465 7220 7c20  ..| Compacter | 
+000020c0: 5b4d 6168 6162 6164 6920 6574 2061 6c2e  [Mahabadi et al.
+000020d0: 2028 3230 3231 295d 2868 7474 7073 3a2f   (2021)](https:/
+000020e0: 2f61 7278 6976 2e6f 7267 2f70 6466 2f32  /arxiv.org/pdf/2
+000020f0: 3130 362e 3034 3634 372e 7064 6629 207c  106.04647.pdf) |
+00002100: 205b 446f 6373 5d28 6874 7470 733a 2f2f   [Docs](https://
+00002110: 646f 6373 2e61 6461 7074 6572 6875 622e  docs.adapterhub.
+00002120: 6d6c 2f6d 6574 686f 6473 2e68 746d 6c23  ml/methods.html#
+00002130: 636f 6d70 6163 7465 7229 207c 0d0a 7c20  compacter) |..| 
+00002140: 4c6f 5241 207c 205b 4875 2065 7420 616c  LoRA | [Hu et al
+00002150: 2e20 2832 3032 3129 5d28 6874 7470 733a  . (2021)](https:
+00002160: 2f2f 6172 7869 762e 6f72 672f 7064 662f  //arxiv.org/pdf/
+00002170: 3231 3036 2e30 3936 3835 2e70 6466 2920  2106.09685.pdf) 
+00002180: 7c20 5b44 6f63 735d 2868 7474 7073 3a2f  | [Docs](https:/
+00002190: 2f64 6f63 732e 6164 6170 7465 7268 7562  /docs.adapterhub
+000021a0: 2e6d 6c2f 6d65 7468 6f64 732e 6874 6d6c  .ml/methods.html
+000021b0: 236c 6f72 6129 207c 0d0a 7c20 2849 4129  #lora) |..| (IA)
+000021c0: 5e33 207c 205b 4c69 7520 6574 2061 6c2e  ^3 | [Liu et al.
+000021d0: 2028 3230 3232 295d 2868 7474 7073 3a2f   (2022)](https:/
+000021e0: 2f61 7278 6976 2e6f 7267 2f70 6466 2f32  /arxiv.org/pdf/2
+000021f0: 3230 352e 3035 3633 382e 7064 6629 207c  205.05638.pdf) |
+00002200: 205b 446f 6373 5d28 6874 7470 733a 2f2f   [Docs](https://
+00002210: 646f 6373 2e61 6461 7074 6572 6875 622e  docs.adapterhub.
+00002220: 6d6c 2f6d 6574 686f 6473 2e68 746d 6c23  ml/methods.html#
+00002230: 6961 2d33 2920 7c0d 0a7c 2055 6e69 5045  ia-3) |..| UniPE
+00002240: 4c54 207c 205b 4d61 6f20 6574 2061 6c2e  LT | [Mao et al.
+00002250: 2028 3230 3232 295d 2868 7474 7073 3a2f   (2022)](https:/
+00002260: 2f61 7278 6976 2e6f 7267 2f70 6466 2f32  /arxiv.org/pdf/2
+00002270: 3131 302e 3037 3537 372e 7064 6629 207c  110.07577.pdf) |
+00002280: 205b 446f 6373 5d28 6874 7470 733a 2f2f   [Docs](https://
+00002290: 646f 6373 2e61 6461 7074 6572 6875 622e  docs.adapterhub.
+000022a0: 6d6c 2f6d 6574 686f 645f 636f 6d62 696e  ml/method_combin
+000022b0: 6174 696f 6e73 2e68 746d 6c23 756e 6970  ations.html#unip
+000022c0: 656c 7429 207c 0d0a 7c20 5072 6f6d 7074  elt) |..| Prompt
+000022d0: 2054 756e 696e 6720 7c20 5b4c 6573 7465   Tuning | [Leste
+000022e0: 7220 6574 2061 6c2e 2028 3230 3231 295d  r et al. (2021)]
+000022f0: 2868 7474 7073 3a2f 2f61 636c 616e 7468  (https://aclanth
+00002300: 6f6c 6f67 792e 6f72 672f 3230 3231 2e65  ology.org/2021.e
+00002310: 6d6e 6c70 2d6d 6169 6e2e 3234 332f 2920  mnlp-main.243/) 
+00002320: 7c20 5b44 6f63 735d 2868 7474 7073 3a2f  | [Docs](https:/
+00002330: 2f64 6f63 732e 6164 6170 7465 7268 7562  /docs.adapterhub
+00002340: 2e6d 6c2f 6d65 7468 6f64 732e 6874 6d6c  .ml/methods.html
+00002350: 2370 726f 6d70 742d 7475 6e69 6e67 2920  #prompt-tuning) 
+00002360: 7c0d 0a7c 2051 4c6f 5241 207c 205b 4465  |..| QLoRA | [De
+00002370: 7474 6d65 7273 2065 7420 616c 2e20 2832  ttmers et al. (2
+00002380: 3032 3329 5d28 6874 7470 733a 2f2f 6172  023)](https://ar
+00002390: 7869 762e 6f72 672f 7064 662f 3233 3035  xiv.org/pdf/2305
+000023a0: 2e31 3433 3134 2e70 6466 2920 7c20 5b4e  .14314.pdf) | [N
+000023b0: 6f74 6562 6f6f 6b5d 2868 7474 7073 3a2f  otebook](https:/
+000023c0: 2f63 6f6c 6162 2e72 6573 6561 7263 682e  /colab.research.
+000023d0: 676f 6f67 6c65 2e63 6f6d 2f67 6974 6875  google.com/githu
+000023e0: 622f 4164 6170 7465 722d 4875 622f 6164  b/Adapter-Hub/ad
+000023f0: 6170 7465 7273 2f62 6c6f 622f 6d61 696e  apters/blob/main
+00002400: 2f6e 6f74 6562 6f6f 6b73 2f51 4c6f 5241  /notebooks/QLoRA
+00002410: 5f4c 6c61 6d61 5f46 696e 6574 756e 696e  _Llama_Finetunin
+00002420: 672e 6970 796e 6229 207c 0d0a 0d0a 2323  g.ipynb) |....##
+00002430: 2053 7570 706f 7274 6564 204d 6f64 656c   Supported Model
+00002440: 730d 0a0d 0a57 6520 6375 7272 656e 746c  s....We currentl
+00002450: 7920 7375 7070 6f72 7420 7468 6520 5079  y support the Py
+00002460: 546f 7263 6820 7665 7273 696f 6e73 206f  Torch versions o
+00002470: 6620 616c 6c20 6d6f 6465 6c73 206c 6973  f all models lis
+00002480: 7465 6420 6f6e 2074 6865 202a 2a5b 4d6f  ted on the **[Mo
+00002490: 6465 6c20 4f76 6572 7669 6577 5d28 6874  del Overview](ht
+000024a0: 7470 733a 2f2f 646f 6373 2e61 6461 7074  tps://docs.adapt
+000024b0: 6572 6875 622e 6d6c 2f6d 6f64 656c 5f6f  erhub.ml/model_o
+000024c0: 7665 7276 6965 772e 6874 6d6c 2920 7061  verview.html) pa
+000024d0: 6765 2a2a 2069 6e20 6f75 7220 646f 6375  ge** in our docu
+000024e0: 6d65 6e74 6174 696f 6e2e 0d0a 0d0a 2323  mentation.....##
+000024f0: 2044 6576 656c 6f70 696e 6720 2620 436f   Developing & Co
+00002500: 6e74 7269 6275 7469 6e67 0d0a 0d0a 546f  ntributing....To
+00002510: 2067 6574 2073 7461 7274 6564 2077 6974   get started wit
+00002520: 6820 6465 7665 6c6f 7069 6e67 206f 6e20  h developing on 
+00002530: 5f41 6461 7074 6572 735f 2079 6f75 7273  _Adapters_ yours
+00002540: 656c 6620 616e 6420 6c65 6172 6e20 6d6f  elf and learn mo
+00002550: 7265 2061 626f 7574 2077 6179 7320 746f  re about ways to
+00002560: 2063 6f6e 7472 6962 7574 652c 2070 6c65   contribute, ple
+00002570: 6173 6520 7365 6520 6874 7470 733a 2f2f  ase see https://
+00002580: 646f 6373 2e61 6461 7074 6572 6875 622e  docs.adapterhub.
+00002590: 6d6c 2f63 6f6e 7472 6962 7574 696e 672e  ml/contributing.
+000025a0: 6874 6d6c 2e0d 0a0d 0a23 2320 4369 7461  html.....## Cita
+000025b0: 7469 6f6e 0d0a 0d0a 4966 2079 6f75 2075  tion....If you u
+000025c0: 7365 205f 4164 6170 7465 7273 5f20 696e  se _Adapters_ in
+000025d0: 2079 6f75 7220 776f 726b 2c20 706c 6561   your work, plea
+000025e0: 7365 2063 6f6e 7369 6465 7220 6369 7469  se consider citi
+000025f0: 6e67 206f 7572 206c 6962 7261 7279 2070  ng our library p
+00002600: 6170 6572 3a20 5b41 6461 7074 6572 733a  aper: [Adapters:
+00002610: 2041 2055 6e69 6669 6564 204c 6962 7261   A Unified Libra
+00002620: 7279 2066 6f72 2050 6172 616d 6574 6572  ry for Parameter
+00002630: 2d45 6666 6963 6965 6e74 2061 6e64 204d  -Efficient and M
+00002640: 6f64 756c 6172 2054 7261 6e73 6665 7220  odular Transfer 
+00002650: 4c65 6172 6e69 6e67 5d28 6874 7470 733a  Learning](https:
+00002660: 2f2f 6172 7869 762e 6f72 672f 6162 732f  //arxiv.org/abs/
+00002670: 3233 3131 2e31 3130 3737 290d 0a0d 0a60  2311.11077)....`
+00002680: 6060 0d0a 4069 6e70 726f 6365 6564 696e  ``..@inproceedin
+00002690: 6773 7b70 6f74 682d 6574 616c 2d32 3032  gs{poth-etal-202
+000026a0: 332d 6164 6170 7465 7273 2c0d 0a20 2020  3-adapters,..   
+000026b0: 2074 6974 6c65 203d 2022 4164 6170 7465   title = "Adapte
+000026c0: 7273 3a20 4120 556e 6966 6965 6420 4c69  rs: A Unified Li
+000026d0: 6272 6172 7920 666f 7220 5061 7261 6d65  brary for Parame
+000026e0: 7465 722d 4566 6669 6369 656e 7420 616e  ter-Efficient an
+000026f0: 6420 4d6f 6475 6c61 7220 5472 616e 7366  d Modular Transf
+00002700: 6572 204c 6561 726e 696e 6722 2c0d 0a20  er Learning",.. 
+00002710: 2020 2061 7574 686f 7220 3d20 7b50 6f74     author = {Pot
+00002720: 682c 2043 6c69 6674 6f6e 2020 616e 640d  h, Clifton  and.
+00002730: 0a20 2020 2020 2053 7465 727a 2c20 4861  .      Sterz, Ha
+00002740: 6e6e 6168 2020 616e 640d 0a20 2020 2020  nnah  and..     
+00002750: 2050 6175 6c2c 2049 6e64 7261 6e65 696c   Paul, Indraneil
+00002760: 2020 616e 640d 0a20 2020 2020 2050 7572    and..      Pur
+00002770: 6b61 7961 7374 6861 2c20 5375 6b61 6e6e  kayastha, Sukann
+00002780: 7961 2020 616e 640d 0a20 2020 2020 2045  ya  and..      E
+00002790: 6e67 6c7b 5c22 617d 6e64 6572 2c20 4c65  ngl{\"a}nder, Le
+000027a0: 6f6e 2020 616e 640d 0a20 2020 2020 2049  on  and..      I
+000027b0: 6d68 6f66 2c20 5469 6d6f 2020 616e 640d  mhof, Timo  and.
+000027c0: 0a20 2020 2020 2056 756c 697b 5c27 637d  .      Vuli{\'c}
+000027d0: 2c20 4976 616e 2020 616e 640d 0a20 2020  , Ivan  and..   
+000027e0: 2020 2052 7564 6572 2c20 5365 6261 7374     Ruder, Sebast
+000027f0: 6961 6e20 2061 6e64 0d0a 2020 2020 2020  ian  and..      
+00002800: 4775 7265 7679 6368 2c20 4972 796e 6120  Gurevych, Iryna 
+00002810: 2061 6e64 0d0a 2020 2020 2020 5066 6569   and..      Pfei
+00002820: 6666 6572 2c20 4a6f 6e61 737d 2c0d 0a20  ffer, Jonas},.. 
+00002830: 2020 2062 6f6f 6b74 6974 6c65 203d 2022     booktitle = "
+00002840: 5072 6f63 6565 6469 6e67 7320 6f66 2074  Proceedings of t
+00002850: 6865 2032 3032 3320 436f 6e66 6572 656e  he 2023 Conferen
+00002860: 6365 206f 6e20 456d 7069 7269 6361 6c20  ce on Empirical 
+00002870: 4d65 7468 6f64 7320 696e 204e 6174 7572  Methods in Natur
+00002880: 616c 204c 616e 6775 6167 6520 5072 6f63  al Language Proc
+00002890: 6573 7369 6e67 3a20 5379 7374 656d 2044  essing: System D
+000028a0: 656d 6f6e 7374 7261 7469 6f6e 7322 2c0d  emonstrations",.
+000028b0: 0a20 2020 206d 6f6e 7468 203d 2064 6563  .    month = dec
+000028c0: 2c0d 0a20 2020 2079 6561 7220 3d20 2232  ,..    year = "2
+000028d0: 3032 3322 2c0d 0a20 2020 2061 6464 7265  023",..    addre
+000028e0: 7373 203d 2022 5369 6e67 6170 6f72 6522  ss = "Singapore"
+000028f0: 2c0d 0a20 2020 2070 7562 6c69 7368 6572  ,..    publisher
+00002900: 203d 2022 4173 736f 6369 6174 696f 6e20   = "Association 
+00002910: 666f 7220 436f 6d70 7574 6174 696f 6e61  for Computationa
+00002920: 6c20 4c69 6e67 7569 7374 6963 7322 2c0d  l Linguistics",.
+00002930: 0a20 2020 2075 726c 203d 2022 6874 7470  .    url = "http
+00002940: 733a 2f2f 6163 6c61 6e74 686f 6c6f 6779  s://aclanthology
+00002950: 2e6f 7267 2f32 3032 332e 656d 6e6c 702d  .org/2023.emnlp-
+00002960: 6465 6d6f 2e31 3322 2c0d 0a20 2020 2070  demo.13",..    p
+00002970: 6167 6573 203d 2022 3134 392d 2d31 3630  ages = "149--160
+00002980: 222c 0d0a 7d0d 0a60 6060 0d0a 0d0a 416c  ",..}..```....Al
+00002990: 7465 726e 6174 6976 656c 792c 2066 6f72  ternatively, for
+000029a0: 2074 6865 2070 7265 6465 6365 7373 6f72   the predecessor
+000029b0: 2060 6164 6170 7465 722d 7472 616e 7366   `adapter-transf
+000029c0: 6f72 6d65 7273 602c 2074 6865 2048 7562  ormers`, the Hub
+000029d0: 2069 6e66 7261 7374 7275 6374 7572 6520   infrastructure 
+000029e0: 616e 6420 6164 6170 7465 7273 2075 706c  and adapters upl
+000029f0: 6f61 6465 6420 6279 2074 6865 2041 6461  oaded by the Ada
+00002a00: 7074 6572 4875 6220 7465 616d 2c20 706c  pterHub team, pl
+00002a10: 6561 7365 2063 6f6e 7369 6465 7220 6369  ease consider ci
+00002a20: 7469 6e67 206f 7572 2069 6e69 7469 616c  ting our initial
+00002a30: 2070 6170 6572 3a20 5b41 6461 7074 6572   paper: [Adapter
+00002a40: 4875 623a 2041 2046 7261 6d65 776f 726b  Hub: A Framework
+00002a50: 2066 6f72 2041 6461 7074 696e 6720 5472   for Adapting Tr
+00002a60: 616e 7366 6f72 6d65 7273 5d28 6874 7470  ansformers](http
+00002a70: 733a 2f2f 6172 7869 762e 6f72 672f 6162  s://arxiv.org/ab
+00002a80: 732f 3230 3037 2e30 3737 3739 290d 0a0d  s/2007.07779)...
+00002a90: 0a60 6060 0d0a 4069 6e70 726f 6365 6564  .```..@inproceed
+00002aa0: 696e 6773 7b70 6665 6966 6665 7232 3032  ings{pfeiffer202
+00002ab0: 3041 6461 7074 6572 4875 622c 0d0a 2020  0AdapterHub,..  
+00002ac0: 2020 7469 746c 653d 7b41 6461 7074 6572    title={Adapter
+00002ad0: 4875 623a 2041 2046 7261 6d65 776f 726b  Hub: A Framework
+00002ae0: 2066 6f72 2041 6461 7074 696e 6720 5472   for Adapting Tr
+00002af0: 616e 7366 6f72 6d65 7273 7d2c 0d0a 2020  ansformers},..  
+00002b00: 2020 6175 7468 6f72 3d7b 5066 6569 6666    author={Pfeiff
+00002b10: 6572 2c20 4a6f 6e61 7320 616e 640d 0a20  er, Jonas and.. 
+00002b20: 2020 2020 2020 2020 2020 2052 7b5c 2275             R{\"u
+00002b30: 7d63 6b6c 7b5c 2765 7d2c 2041 6e64 7265  }ckl{\'e}, Andre
+00002b40: 6173 2061 6e64 0d0a 2020 2020 2020 2020  as and..        
+00002b50: 2020 2020 506f 7468 2c20 436c 6966 746f      Poth, Clifto
+00002b60: 6e20 616e 640d 0a20 2020 2020 2020 2020  n and..         
+00002b70: 2020 204b 616d 6174 682c 2041 6973 6877     Kamath, Aishw
+00002b80: 6172 7961 2061 6e64 0d0a 2020 2020 2020  arya and..      
+00002b90: 2020 2020 2020 5675 6c69 7b5c 2763 7d2c        Vuli{\'c},
+00002ba0: 2049 7661 6e20 616e 640d 0a20 2020 2020   Ivan and..     
+00002bb0: 2020 2020 2020 2052 7564 6572 2c20 5365         Ruder, Se
+00002bc0: 6261 7374 6961 6e20 616e 640d 0a20 2020  bastian and..   
+00002bd0: 2020 2020 2020 2020 2043 686f 2c20 4b79           Cho, Ky
+00002be0: 756e 6768 7975 6e20 616e 640d 0a20 2020  unghyun and..   
+00002bf0: 2020 2020 2020 2020 2047 7572 6576 7963           Gurevyc
+00002c00: 682c 2049 7279 6e61 7d2c 0d0a 2020 2020  h, Iryna},..    
+00002c10: 626f 6f6b 7469 746c 653d 7b50 726f 6365  booktitle={Proce
+00002c20: 6564 696e 6773 206f 6620 7468 6520 3230  edings of the 20
+00002c30: 3230 2043 6f6e 6665 7265 6e63 6520 6f6e  20 Conference on
+00002c40: 2045 6d70 6972 6963 616c 204d 6574 686f   Empirical Metho
+00002c50: 6473 2069 6e20 4e61 7475 7261 6c20 4c61  ds in Natural La
+00002c60: 6e67 7561 6765 2050 726f 6365 7373 696e  nguage Processin
+00002c70: 673a 2053 7973 7465 6d20 4465 6d6f 6e73  g: System Demons
+00002c80: 7472 6174 696f 6e73 7d2c 0d0a 2020 2020  trations},..    
+00002c90: 7061 6765 733d 7b34 362d 2d35 347d 2c0d  pages={46--54},.
+00002ca0: 0a20 2020 2079 6561 723d 7b32 3032 307d  .    year={2020}
+00002cb0: 0d0a 7d0d 0a60 6060 0d0a                 ..}..```..
```

### Comparing `adapters-0.1.2/src/adapters.egg-info/SOURCES.txt` & `adapters-0.2.0/src/adapters.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 src/adapters/methods/__init__.py
 src/adapters/methods/adapter_layer_base.py
 src/adapters/methods/bottleneck.py
 src/adapters/methods/lora.py
 src/adapters/methods/modeling.py
 src/adapters/methods/prefix_tuning.py
 src/adapters/methods/prompt_tuning.py
+src/adapters/methods/utils.py
 src/adapters/models/__init__.py
 src/adapters/models/albert/__init__.py
 src/adapters/models/albert/adapter_model.py
 src/adapters/models/albert/mixin_albert.py
 src/adapters/models/albert/modeling_albert.py
 src/adapters/models/auto/__init__.py
 src/adapters/models/auto/adapter_model.py
@@ -140,12 +141,13 @@
 tests/test_distilbert.py
 tests/test_electra.py
 tests/test_encoder_decoder.py
 tests/test_gpt2.py
 tests/test_gptj.py
 tests/test_llama.py
 tests/test_mbart.py
+tests/test_mt5.py
 tests/test_roberta.py
 tests/test_t5.py
 tests/test_vit.py
 tests/test_xlm_roberta.py
 tests/test_xmod.py
```

### Comparing `adapters-0.1.2/src/adapters.egg-info/requires.txt` & `adapters-0.2.0/src/adapters.egg-info/requires.txt`

 * *Files 27% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-transformers~=4.36.0
+transformers~=4.39.3
 
 [dev]
 pytest<8.0.0,>=7.2.0
 pytest-subtests
 pytest-xdist
 timeout-decorator
 parameterized
@@ -26,37 +26,37 @@
 protobuf
 isort>=5.5.4
 flake8>=3.8.3
 docutils==0.16.0
 Jinja2==2.11.3
 markupsafe==2.0.1
 myst-parser
-sphinx==3.2.1
-sphinx-markdown-tables
+sphinx==5.0.2
+sphinx-markdown-tables==0.0.17
 sphinx-rtd-theme==0.4.3
-sphinx-copybutton
+sphinx-copybutton==0.5.2
 sphinxext-opengraph==0.4.1
-sphinx-intl
-sphinx-multiversion
+sphinx-intl==2.1.0
+sphinx-multiversion==0.2.4
 scikit-learn
 onnxruntime>=1.4.0
 onnxruntime-tools>=1.4.2
 
 [docs]
 docutils==0.16.0
 Jinja2==2.11.3
 markupsafe==2.0.1
 myst-parser
-sphinx==3.2.1
-sphinx-markdown-tables
+sphinx==5.0.2
+sphinx-markdown-tables==0.0.17
 sphinx-rtd-theme==0.4.3
-sphinx-copybutton
+sphinx-copybutton==0.5.2
 sphinxext-opengraph==0.4.1
-sphinx-intl
-sphinx-multiversion
+sphinx-intl==2.1.0
+sphinx-multiversion==0.2.4
 
 [onnxruntime]
 onnxruntime>=1.4.0
 onnxruntime-tools>=1.4.2
 
 [quality]
 black==22.3
```

### Comparing `adapters-0.1.2/tests/test_adapter.py` & `adapters-0.2.0/tests/test_adapter.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
             model = AutoAdapterModel.from_config(self.config())
         else:
             model = self.model_class(self.config())
             adapters.init(model)
         model.to(torch_device)
         return model
 
-    def get_input_samples(self, shape=None, vocab_size=5000, config=None):
+    def get_input_samples(self, shape=None, vocab_size=5000, config=None, **kwargs):
         shape = shape or self.default_input_samples_shape
         total_dims = 1
         for dim in shape:
             total_dims *= dim
 
         values = []
         for _ in range(total_dims):
@@ -92,23 +92,23 @@
         self.assertFalse(adapter_name in model.adapters_config)
         self.assertEqual(len(model.get_adapter(adapter_name)), 0)
 
 
 class VisionAdapterTestBase(AdapterTestBase):
     default_input_samples_shape = (3, 3, 224, 224)
 
-    def get_input_samples(self, shape=None, config=None):
+    def get_input_samples(self, shape=None, config=None, dtype=torch.float, **kwargs):
         shape = shape or self.default_input_samples_shape
         total_dims = 1
         for dim in shape:
             total_dims *= dim
         values = []
         for _ in range(total_dims):
             values.append(random.random())
-        pixel_values = torch.tensor(data=values, dtype=torch.float, device=torch_device).view(shape).contiguous()
+        pixel_values = torch.tensor(data=values, dtype=dtype, device=torch_device).view(shape).contiguous()
         in_data = {"pixel_values": pixel_values}
 
         return in_data
 
     def add_head(self, model, name, **kwargs):
         if "num_labels" not in kwargs:
             kwargs["num_labels"] = 10
```

### Comparing `adapters-0.1.2/tests/test_adapter_backward_compability.py` & `adapters-0.2.0/tests/test_adapter_backward_compability.py`

 * *Files identical despite different names*

### Comparing `adapters-0.1.2/tests/test_adapter_config.py` & `adapters-0.2.0/tests/test_adapter_config.py`

 * *Files identical despite different names*

### Comparing `adapters-0.1.2/tests/test_adapter_conversion.py` & `adapters-0.2.0/tests/test_adapter_conversion.py`

 * *Files identical despite different names*

### Comparing `adapters-0.1.2/tests/test_adapter_custom_head.py` & `adapters-0.2.0/tests/test_adapter_custom_head.py`

 * *Files identical despite different names*

### Comparing `adapters-0.1.2/tests/test_adapter_embeddings.py` & `adapters-0.2.0/tests/test_adapter_embeddings.py`

 * *Files 10% similar despite different names*

```diff
@@ -92,16 +92,18 @@
         self.add_head(model, "test")
         model.train_adapter("test", train_embeddings=True)
 
         for k, v in filter_parameters(model, "adapters.test.").items():
             self.assertTrue(v.requires_grad, k)
 
         self.assertTrue(model.get_input_embeddings().train)
+        self.assertTrue(model.get_input_embeddings().weight.requires_grad)
 
         state_dict_pre = copy.deepcopy(model.state_dict())
+        initial_embedding = model.get_input_embeddings().weight.clone()
 
         train_dataset = self.dataset()
         training_args = TrainingArguments(
             output_dir="./examples",
             do_train=True,
             learning_rate=0.4,
             max_steps=15,
@@ -114,26 +116,34 @@
         trainer = Trainer(
             model=model,
             args=training_args,
             train_dataset=train_dataset,
         )
         trainer.train()
 
+        trained_embedding = model.get_input_embeddings().weight.clone()
+
+        self.assertFalse(torch.equal(initial_embedding, trained_embedding))
+
         self.assertFalse(
             all(
                 torch.equal(v1, v2)
                 for ((k1, v1), (k2, v2)) in zip(state_dict_pre.items(), model.state_dict().items())
                 if "test" in k1
             )
         )
         self.assertTrue(
             all(
                 torch.equal(v1, v2)
                 for ((k1, v1), (k2, v2)) in zip(state_dict_pre.items(), model.state_dict().items())
                 if "test" not in k1
+                and "embedding" not in k1
+                and "embed_tokens" not in k1
+                and "shared" not in k1
+                and "wte" not in k1
             )
         )
 
     def test_reference_embedding(self):
         model = AutoAdapterModel.from_config(self.config())  # self.get_model()
         tokenizer = AutoTokenizer.from_pretrained(self.tokenizer_name, use_fast=False)
         if tokenizer.pad_token is None:
```

### Comparing `adapters-0.1.2/tests/test_adapter_fusion_common.py` & `adapters-0.2.0/tests/test_adapter_fusion_common.py`

 * *Files identical despite different names*

### Comparing `adapters-0.1.2/tests/test_adapter_fusion_config.py` & `adapters-0.2.0/tests/test_adapter_fusion_config.py`

 * *Files identical despite different names*

### Comparing `adapters-0.1.2/tests/test_adapter_heads.py` & `adapters-0.2.0/tests/test_adapter_heads.py`

 * *Files identical despite different names*

### Comparing `adapters-0.1.2/tests/test_adapter_hub.py` & `adapters-0.2.0/tests/test_adapter_hub.py`

 * *Files identical despite different names*

### Comparing `adapters-0.1.2/tests/test_adapter_save_id2label.py` & `adapters-0.2.0/tests/test_adapter_save_id2label.py`

 * *Files identical despite different names*

### Comparing `adapters-0.1.2/tests/test_adapter_trainer.py` & `adapters-0.2.0/tests/test_adapter_trainer.py`

 * *Files identical despite different names*

### Comparing `adapters-0.1.2/tests/test_albert.py` & `adapters-0.2.0/tests/test_albert.py`

 * *Files identical despite different names*

### Comparing `adapters-0.1.2/tests/test_bart.py` & `adapters-0.2.0/tests/test_bart.py`

 * *Files identical despite different names*

### Comparing `adapters-0.1.2/tests/test_beit.py` & `adapters-0.2.0/tests/test_beit.py`

 * *Files identical despite different names*

### Comparing `adapters-0.1.2/tests/test_bert.py` & `adapters-0.2.0/tests/test_bert.py`

 * *Files identical despite different names*

### Comparing `adapters-0.1.2/tests/test_bert_generation.py` & `adapters-0.2.0/tests/test_bert_generation.py`

 * *Files identical despite different names*

### Comparing `adapters-0.1.2/tests/test_clip.py` & `adapters-0.2.0/tests/test_clip.py`

 * *Files 1% similar despite different names*

```diff
@@ -166,15 +166,15 @@
     )
     tokenizer_name = "openai/clip-vit-base-patch32"
     # Default shape of inputs to use
     default_text_input_samples_shape = (3, 64)
     default_vision_input_samples_shape = (3, 3, 224, 224)
     do_run_train_tests = False
 
-    def get_input_samples(self, vocab_size=5000, config=None):
+    def get_input_samples(self, vocab_size=5000, config=None, dtype=torch.float, **kwargs):
         # text inputs
         shape = self.default_text_input_samples_shape
         total_dims = 1
         for dim in shape:
             total_dims *= dim
         values = []
         for _ in range(total_dims):
@@ -190,15 +190,15 @@
         shape = self.default_vision_input_samples_shape
         total_dims = 1
         for dim in shape:
             total_dims *= dim
         values = []
         for _ in range(total_dims):
             values.append(random.random())
-        pixel_values = torch.tensor(data=values, dtype=torch.float, device=torch_device).view(shape).contiguous()
+        pixel_values = torch.tensor(data=values, dtype=dtype, device=torch_device).view(shape).contiguous()
         in_data["pixel_values"] = pixel_values
 
         return in_data
 
     def add_head(self, *args, **kwargs):
         pass
```

### Comparing `adapters-0.1.2/tests/test_deberta.py` & `adapters-0.2.0/tests/test_deberta.py`

 * *Files identical despite different names*

### Comparing `adapters-0.1.2/tests/test_debertaV2.py` & `adapters-0.2.0/tests/test_debertaV2.py`

 * *Files identical despite different names*

### Comparing `adapters-0.1.2/tests/test_distilbert.py` & `adapters-0.2.0/tests/test_distilbert.py`

 * *Files identical despite different names*

### Comparing `adapters-0.1.2/tests/test_electra.py` & `adapters-0.2.0/tests/test_electra.py`

 * *Files identical despite different names*

### Comparing `adapters-0.1.2/tests/test_encoder_decoder.py` & `adapters-0.2.0/tests/test_encoder_decoder.py`

 * *Files identical despite different names*

### Comparing `adapters-0.1.2/tests/test_gpt2.py` & `adapters-0.2.0/tests/test_gpt2.py`

 * *Files identical despite different names*

### Comparing `adapters-0.1.2/tests/test_gptj.py` & `adapters-0.2.0/tests/test_gptj.py`

 * *Files identical despite different names*

### Comparing `adapters-0.1.2/tests/test_llama.py` & `adapters-0.2.0/tests/test_llama.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,15 +25,14 @@
     config = make_config(
         LlamaConfig,
         hidden_size=32,
         num_hidden_layers=5,
         num_attention_heads=4,
         intermediate_size=37,
         hidden_act="gelu",
-        hidden_dropout_prob=0.1,
         pad_token_id=0,
     )
     tokenizer_name = "openlm-research/open_llama_13b"
 
 
 @require_torch
 class LlamaAdapterTest(
@@ -57,8 +56,9 @@
 
 @require_torch
 class LlamaClassConversionTest(
     ModelClassConversionTestMixin,
     LlamaAdapterTestBase,
     unittest.TestCase,
 ):
-    pass
+    def test_conversion_question_answering_model(self):
+        raise self.skipTest("We don't support the Llama QA model.")
```

### Comparing `adapters-0.1.2/tests/test_mbart.py` & `adapters-0.2.0/tests/test_mbart.py`

 * *Files identical despite different names*

### Comparing `adapters-0.1.2/tests/test_roberta.py` & `adapters-0.2.0/tests/test_roberta.py`

 * *Files identical despite different names*

### Comparing `adapters-0.1.2/tests/test_t5.py` & `adapters-0.2.0/tests/test_t5.py`

 * *Files identical despite different names*

### Comparing `adapters-0.1.2/tests/test_vit.py` & `adapters-0.2.0/tests/test_vit.py`

 * *Files identical despite different names*

### Comparing `adapters-0.1.2/tests/test_xlm_roberta.py` & `adapters-0.2.0/tests/test_xlm_roberta.py`

 * *Files identical despite different names*

### Comparing `adapters-0.1.2/tests/test_xmod.py` & `adapters-0.2.0/tests/test_xmod.py`

 * *Files identical despite different names*


# Comparing `tmp/caikit-nlp-0.4.8.tar.gz` & `tmp/caikit_nlp-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caikit-nlp-0.4.8.tar", last modified: Wed Apr  3 19:16:29 2024, max compression
+gzip compressed data, was "caikit_nlp-0.4.9.tar", last modified: Thu Apr 25 04:47:13 2024, max compression
```

## Comparing `caikit-nlp-0.4.8.tar` & `caikit_nlp-0.4.9.tar`

### file list

```diff
@@ -1,183 +1,183 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:16:29.669224 caikit-nlp-0.4.8/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/.dockerignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:16:29.641224 caikit-nlp-0.4.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:16:29.641224 caikit-nlp-0.4.8/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      676 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/.github/ISSUE_TEMPLATE/user_story.md
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:16:29.645224 caikit-nlp-0.4.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/.github/workflows/build-image.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/.github/workflows/build-library.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/.github/workflows/lint-code.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/.github/workflows/publish-library.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2157 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/.prettierignore
--rw-r--r--   0 runner    (1001) docker     (127)    21457 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/.whitesource
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (127)     7191 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    11424 2024-04-03 19:16:29.669224 caikit-nlp-0.4.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10588 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/SECURITY.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:16:29.645224 caikit-nlp-0.4.8/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/benchmarks/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:16:29.633224 caikit-nlp-0.4.8/benchmarks/logs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:16:29.645224 caikit-nlp-0.4.8/benchmarks/logs/llama2-7b/
--rw-r--r--   0 runner    (1001) docker     (127)     4288 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/benchmarks/logs/llama2-7b/20230905_183655.output
--rw-r--r--   0 runner    (1001) docker     (127)     4288 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/benchmarks/logs/llama2-7b/20230905_184809.output
--rw-r--r--   0 runner    (1001) docker     (127)     9795 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/benchmarks/logs/llama2-7b/20230905_191650.output
--rw-r--r--   0 runner    (1001) docker     (127)     4286 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/benchmarks/logs/llama2-7b/20230905_194133.output
--rw-r--r--   0 runner    (1001) docker     (127)     4286 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/benchmarks/logs/llama2-7b/20230906_135211.output
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:16:29.645224 caikit-nlp-0.4.8/caikit_nlp/
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/caikit_nlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-03 19:16:29.000000 caikit-nlp-0.4.8/caikit_nlp/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:16:29.645224 caikit-nlp-0.4.8/caikit_nlp/config/
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/caikit_nlp/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2211 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/caikit_nlp/config/config.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:16:29.645224 caikit-nlp-0.4.8/caikit_nlp/data_model/
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/caikit_nlp/data_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2956 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/caikit_nlp/data_model/generation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:16:29.649224 caikit-nlp-0.4.8/caikit_nlp/model_management/
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/caikit_nlp/model_management/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5168 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/caikit_nlp/model_management/tgis_auto_finder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:16:29.649224 caikit-nlp-0.4.8/caikit_nlp/modules/
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/caikit_nlp/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:16:29.649224 caikit-nlp-0.4.8/caikit_nlp/modules/text_classification/
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/caikit_nlp/modules/text_classification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7859 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/caikit_nlp/modules/text_classification/sequence_classification.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:16:29.649224 caikit-nlp-0.4.8/caikit_nlp/modules/text_embedding/
--rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/caikit_nlp/modules/text_embedding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    40080 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/caikit_nlp/modules/text_embedding/embedding.py
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/caikit_nlp/modules/text_embedding/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:16:29.649224 caikit-nlp-0.4.8/caikit_nlp/modules/text_generation/
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/caikit_nlp/modules/text_generation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8496 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/caikit_nlp/modules/text_generation/peft_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    51230 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/caikit_nlp/modules/text_generation/peft_prompt_tuning.py
--rw-r--r--   0 runner    (1001) docker     (127)    12248 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/caikit_nlp/modules/text_generation/peft_tgis_remote.py
--rw-r--r--   0 runner    (1001) docker     (127)    26132 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/caikit_nlp/modules/text_generation/text_generation_local.py
--rw-r--r--   0 runner    (1001) docker     (127)    12610 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/caikit_nlp/modules/text_generation/text_generation_tgis.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:16:29.649224 caikit-nlp-0.4.8/caikit_nlp/modules/token_classification/
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/caikit_nlp/modules/token_classification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16150 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/caikit_nlp/modules/token_classification/filtered_span_classification.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:16:29.649224 caikit-nlp-0.4.8/caikit_nlp/modules/tokenization/
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/caikit_nlp/modules/tokenization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3917 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/caikit_nlp/modules/tokenization/regex_sentence_splitter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:16:29.649224 caikit-nlp-0.4.8/caikit_nlp/resources/
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/caikit_nlp/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:16:29.653224 caikit-nlp-0.4.8/caikit_nlp/resources/pretrained_model/
--rw-r--r--   0 runner    (1001) docker     (127)      840 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/caikit_nlp/resources/pretrained_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15732 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/caikit_nlp/resources/pretrained_model/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    21429 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/caikit_nlp/resources/pretrained_model/hf_auto_causal_lm.py
--rw-r--r--   0 runner    (1001) docker     (127)     6778 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/caikit_nlp/resources/pretrained_model/hf_auto_seq2seq_lm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/caikit_nlp/resources/pretrained_model/hf_auto_seq_classifier.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:16:29.653224 caikit-nlp-0.4.8/caikit_nlp/toolkit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/caikit_nlp/toolkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3285 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/caikit_nlp/toolkit/data_stream_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/caikit_nlp/toolkit/data_type_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/caikit_nlp/toolkit/task_specific_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:16:29.653224 caikit-nlp-0.4.8/caikit_nlp/toolkit/text_generation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/caikit_nlp/toolkit/text_generation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16766 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/caikit_nlp/toolkit/text_generation/model_run_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    19662 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/caikit_nlp/toolkit/text_generation/tgis_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3335 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/caikit_nlp/toolkit/torch_run.py
--rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/caikit_nlp/toolkit/trainer_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3986 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/caikit_nlp/toolkit/verbalizer_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/caikit_nlp/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:16:29.669224 caikit-nlp-0.4.8/caikit_nlp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11424 2024-04-03 19:16:29.000000 caikit-nlp-0.4.8/caikit_nlp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5729 2024-04-03 19:16:29.000000 caikit-nlp-0.4.8/caikit_nlp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 19:16:29.000000 caikit-nlp-0.4.8/caikit_nlp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-03 19:16:29.000000 caikit-nlp-0.4.8/caikit_nlp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-03 19:16:29.000000 caikit-nlp-0.4.8/caikit_nlp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/code-of-conduct.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:16:29.653224 caikit-nlp-0.4.8/examples/
--rw-r--r--   0 runner    (1001) docker     (127)    55479 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/examples/Caikit_Getting_Started.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/examples/compare_local_vs_tgis_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     7104 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/examples/evaluate_model.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      404 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/examples/kill-text-generation-launcher.sh
--rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/examples/load_and_run_distributed_peft.py
--rw-r--r--   0 runner    (1001) docker     (127)    13678 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/examples/run_fine_tuning.py
--rw-r--r--   0 runner    (1001) docker     (127)    15840 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/examples/run_peft_tuning.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1992 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/examples/text-generation-launcher
--rw-r--r--   0 runner    (1001) docker     (127)    15815 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/examples/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6158 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/prompt_tuning_parameter_selection.md
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/runtime_config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:16:29.657224 caikit-nlp-0.4.8/runtime_template/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1252 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/runtime_template/run_with_gateway.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:16:29.657224 caikit-nlp-0.4.8/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (127)      657 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/scripts/dump_apis.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      720 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/scripts/fmt.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      231 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/scripts/run_local.sh
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 19:16:29.669224 caikit-nlp-0.4.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/setup_requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:16:29.657224 caikit-nlp-0.4.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:16:29.657224 caikit-nlp-0.4.8/tests/data_model/
--rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/tests/data_model/test_generation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:16:29.657224 caikit-nlp-0.4.8/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)    11719 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/tests/fixtures/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:16:29.657224 caikit-nlp-0.4.8/tests/fixtures/data_model/
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/tests/fixtures/data_model/sample_objects.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:16:29.657224 caikit-nlp-0.4.8/tests/fixtures/tiny_models/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:16:29.661224 caikit-nlp-0.4.8/tests/fixtures/tiny_models/BertForSequenceClassification/
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/tests/fixtures/tiny_models/BertForSequenceClassification/config.json
--rw-r--r--   0 runner    (1001) docker     (127)   384767 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/tests/fixtures/tiny_models/BertForSequenceClassification/pytorch_model.bin
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/tests/fixtures/tiny_models/BertForSequenceClassification/special_tokens_map.json
--rw-r--r--   0 runner    (1001) docker     (127)   481096 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/tests/fixtures/tiny_models/BertForSequenceClassification/tf_model.h5
--rw-r--r--   0 runner    (1001) docker     (127)    23061 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/tests/fixtures/tiny_models/BertForSequenceClassification/tokenizer.json
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/tests/fixtures/tiny_models/BertForSequenceClassification/tokenizer_config.json
--rw-r--r--   0 runner    (1001) docker     (127)     4679 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/tests/fixtures/tiny_models/BertForSequenceClassification/vocab.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:16:29.661224 caikit-nlp-0.4.8/tests/fixtures/tiny_models/BloomForCausalLM/
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/tests/fixtures/tiny_models/BloomForCausalLM/config.json
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/tests/fixtures/tiny_models/BloomForCausalLM/generation_config.json
--rw-r--r--   0 runner    (1001) docker     (127)   406260 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/tests/fixtures/tiny_models/BloomForCausalLM/pytorch_model.bin
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/tests/fixtures/tiny_models/BloomForCausalLM/special_tokens_map.json
--rw-r--r--   0 runner    (1001) docker     (127)    33054 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/tests/fixtures/tiny_models/BloomForCausalLM/tokenizer.json
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/tests/fixtures/tiny_models/BloomForCausalLM/tokenizer_config.json
--rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/tests/fixtures/tiny_models/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:16:29.665224 caikit-nlp-0.4.8/tests/fixtures/tiny_models/T5ForConditionalGeneration/
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/tests/fixtures/tiny_models/T5ForConditionalGeneration/config.json
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/tests/fixtures/tiny_models/T5ForConditionalGeneration/generation_config.json
--rw-r--r--   0 runner    (1001) docker     (127)   546693 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/tests/fixtures/tiny_models/T5ForConditionalGeneration/pytorch_model.bin
--rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/tests/fixtures/tiny_models/T5ForConditionalGeneration/special_tokens_map.json
--rw-r--r--   0 runner    (1001) docker     (127)   382892 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/tests/fixtures/tiny_models/T5ForConditionalGeneration/tokenizer.json
--rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/tests/fixtures/tiny_models/T5ForConditionalGeneration/tokenizer_config.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:16:29.665224 caikit-nlp-0.4.8/tests/model_management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/tests/model_management/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9024 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/tests/model_management/test_tgis_auto_finder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:16:29.665224 caikit-nlp-0.4.8/tests/modules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/tests/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:16:29.665224 caikit-nlp-0.4.8/tests/modules/text_classification/
--rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/tests/modules/text_classification/test_sequence_classification.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:16:29.665224 caikit-nlp-0.4.8/tests/modules/text_embedding/
--rw-r--r--   0 runner    (1001) docker     (127)    37559 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/tests/modules/text_embedding/test_embedding.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:16:29.665224 caikit-nlp-0.4.8/tests/modules/text_generation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/tests/modules/text_generation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3501 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/tests/modules/text_generation/test_peft_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    25729 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/tests/modules/text_generation/test_peft_prompt_tuning.py
--rw-r--r--   0 runner    (1001) docker     (127)     6540 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/tests/modules/text_generation/test_peft_tgis_remote.py
--rw-r--r--   0 runner    (1001) docker     (127)     7254 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/tests/modules/text_generation/test_text_generation_local.py
--rw-r--r--   0 runner    (1001) docker     (127)     8300 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/tests/modules/text_generation/test_text_generation_tgis.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:16:29.665224 caikit-nlp-0.4.8/tests/modules/token_classification/
--rw-r--r--   0 runner    (1001) docker     (127)    18398 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/tests/modules/token_classification/test_filtered_span_classification.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:16:29.665224 caikit-nlp-0.4.8/tests/modules/tokenization/
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/tests/modules/tokenization/test_regex_sentence_splitter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:16:29.665224 caikit-nlp-0.4.8/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/tests/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16904 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/tests/resources/test_pretrained_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:16:29.669224 caikit-nlp-0.4.8/tests/toolkit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/tests/toolkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4087 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/tests/toolkit/test_data_stream_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/tests/toolkit/test_data_type_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2363 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/tests/toolkit/test_task_specific_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3650 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/tests/toolkit/test_verbalizers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:16:29.669224 caikit-nlp-0.4.8/tests/toolkit/text_generation/
--rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/tests/toolkit/text_generation/test_model_run_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:47:13.746450 caikit_nlp-0.4.9/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-25 04:47:06.000000 caikit_nlp-0.4.9/.dockerignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:47:13.722450 caikit_nlp-0.4.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:47:13.722450 caikit_nlp-0.4.9/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-04-25 04:47:06.000000 caikit_nlp-0.4.9/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-25 04:47:06.000000 caikit_nlp-0.4.9/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-25 04:47:06.000000 caikit_nlp-0.4.9/.github/ISSUE_TEMPLATE/user_story.md
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-25 04:47:06.000000 caikit_nlp-0.4.9/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:47:13.722450 caikit_nlp-0.4.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-04-25 04:47:06.000000 caikit_nlp-0.4.9/.github/workflows/build-image.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-25 04:47:06.000000 caikit_nlp-0.4.9/.github/workflows/build-library.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-04-25 04:47:06.000000 caikit_nlp-0.4.9/.github/workflows/lint-code.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-25 04:47:06.000000 caikit_nlp-0.4.9/.github/workflows/publish-library.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2157 2024-04-25 04:47:06.000000 caikit_nlp-0.4.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-25 04:47:06.000000 caikit_nlp-0.4.9/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-25 04:47:06.000000 caikit_nlp-0.4.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-25 04:47:06.000000 caikit_nlp-0.4.9/.prettierignore
+-rw-r--r--   0 runner    (1001) docker     (127)    21457 2024-04-25 04:47:06.000000 caikit_nlp-0.4.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-25 04:47:06.000000 caikit_nlp-0.4.9/.whitesource
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-25 04:47:06.000000 caikit_nlp-0.4.9/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (127)     7191 2024-04-25 04:47:06.000000 caikit_nlp-0.4.9/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-04-25 04:47:06.000000 caikit_nlp-0.4.9/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-04-25 04:47:06.000000 caikit_nlp-0.4.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11431 2024-04-25 04:47:13.746450 caikit_nlp-0.4.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10588 2024-04-25 04:47:06.000000 caikit_nlp-0.4.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-25 04:47:06.000000 caikit_nlp-0.4.9/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:47:13.722450 caikit_nlp-0.4.9/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-04-25 04:47:06.000000 caikit_nlp-0.4.9/benchmarks/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:47:13.714450 caikit_nlp-0.4.9/benchmarks/logs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:47:13.722450 caikit_nlp-0.4.9/benchmarks/logs/llama2-7b/
+-rw-r--r--   0 runner    (1001) docker     (127)     4288 2024-04-25 04:47:06.000000 caikit_nlp-0.4.9/benchmarks/logs/llama2-7b/20230905_183655.output
+-rw-r--r--   0 runner    (1001) docker     (127)     4288 2024-04-25 04:47:06.000000 caikit_nlp-0.4.9/benchmarks/logs/llama2-7b/20230905_184809.output
+-rw-r--r--   0 runner    (1001) docker     (127)     9795 2024-04-25 04:47:06.000000 caikit_nlp-0.4.9/benchmarks/logs/llama2-7b/20230905_191650.output
+-rw-r--r--   0 runner    (1001) docker     (127)     4286 2024-04-25 04:47:06.000000 caikit_nlp-0.4.9/benchmarks/logs/llama2-7b/20230905_194133.output
+-rw-r--r--   0 runner    (1001) docker     (127)     4286 2024-04-25 04:47:06.000000 caikit_nlp-0.4.9/benchmarks/logs/llama2-7b/20230906_135211.output
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:47:13.726450 caikit_nlp-0.4.9/caikit_nlp/
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-25 04:47:06.000000 caikit_nlp-0.4.9/caikit_nlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-25 04:47:13.000000 caikit_nlp-0.4.9/caikit_nlp/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:47:13.726450 caikit_nlp-0.4.9/caikit_nlp/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-25 04:47:06.000000 caikit_nlp-0.4.9/caikit_nlp/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2211 2024-04-25 04:47:06.000000 caikit_nlp-0.4.9/caikit_nlp/config/config.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:47:13.726450 caikit_nlp-0.4.9/caikit_nlp/data_model/
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-25 04:47:06.000000 caikit_nlp-0.4.9/caikit_nlp/data_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2956 2024-04-25 04:47:06.000000 caikit_nlp-0.4.9/caikit_nlp/data_model/generation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:47:13.726450 caikit_nlp-0.4.9/caikit_nlp/model_management/
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-25 04:47:06.000000 caikit_nlp-0.4.9/caikit_nlp/model_management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5168 2024-04-25 04:47:06.000000 caikit_nlp-0.4.9/caikit_nlp/model_management/tgis_auto_finder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:47:13.726450 caikit_nlp-0.4.9/caikit_nlp/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-04-25 04:47:06.000000 caikit_nlp-0.4.9/caikit_nlp/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:47:13.726450 caikit_nlp-0.4.9/caikit_nlp/modules/text_classification/
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-25 04:47:06.000000 caikit_nlp-0.4.9/caikit_nlp/modules/text_classification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7859 2024-04-25 04:47:06.000000 caikit_nlp-0.4.9/caikit_nlp/modules/text_classification/sequence_classification.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:47:13.726450 caikit_nlp-0.4.9/caikit_nlp/modules/text_embedding/
+-rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-04-25 04:47:06.000000 caikit_nlp-0.4.9/caikit_nlp/modules/text_embedding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40080 2024-04-25 04:47:06.000000 caikit_nlp-0.4.9/caikit_nlp/modules/text_embedding/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-25 04:47:06.000000 caikit_nlp-0.4.9/caikit_nlp/modules/text_embedding/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:47:13.730450 caikit_nlp-0.4.9/caikit_nlp/modules/text_generation/
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-25 04:47:06.000000 caikit_nlp-0.4.9/caikit_nlp/modules/text_generation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8496 2024-04-25 04:47:06.000000 caikit_nlp-0.4.9/caikit_nlp/modules/text_generation/peft_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51705 2024-04-25 04:47:06.000000 caikit_nlp-0.4.9/caikit_nlp/modules/text_generation/peft_prompt_tuning.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12248 2024-04-25 04:47:06.000000 caikit_nlp-0.4.9/caikit_nlp/modules/text_generation/peft_tgis_remote.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26640 2024-04-25 04:47:06.000000 caikit_nlp-0.4.9/caikit_nlp/modules/text_generation/text_generation_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12610 2024-04-25 04:47:06.000000 caikit_nlp-0.4.9/caikit_nlp/modules/text_generation/text_generation_tgis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:47:13.730450 caikit_nlp-0.4.9/caikit_nlp/modules/token_classification/
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-25 04:47:06.000000 caikit_nlp-0.4.9/caikit_nlp/modules/token_classification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16150 2024-04-25 04:47:06.000000 caikit_nlp-0.4.9/caikit_nlp/modules/token_classification/filtered_span_classification.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:47:13.730450 caikit_nlp-0.4.9/caikit_nlp/modules/tokenization/
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-25 04:47:06.000000 caikit_nlp-0.4.9/caikit_nlp/modules/tokenization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3917 2024-04-25 04:47:06.000000 caikit_nlp-0.4.9/caikit_nlp/modules/tokenization/regex_sentence_splitter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:47:13.730450 caikit_nlp-0.4.9/caikit_nlp/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-04-25 04:47:06.000000 caikit_nlp-0.4.9/caikit_nlp/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:47:13.730450 caikit_nlp-0.4.9/caikit_nlp/resources/pretrained_model/
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-04-25 04:47:06.000000 caikit_nlp-0.4.9/caikit_nlp/resources/pretrained_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15732 2024-04-25 04:47:06.000000 caikit_nlp-0.4.9/caikit_nlp/resources/pretrained_model/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21429 2024-04-25 04:47:06.000000 caikit_nlp-0.4.9/caikit_nlp/resources/pretrained_model/hf_auto_causal_lm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6778 2024-04-25 04:47:06.000000 caikit_nlp-0.4.9/caikit_nlp/resources/pretrained_model/hf_auto_seq2seq_lm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-04-25 04:47:06.000000 caikit_nlp-0.4.9/caikit_nlp/resources/pretrained_model/hf_auto_seq_classifier.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:47:13.730450 caikit_nlp-0.4.9/caikit_nlp/toolkit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:47:06.000000 caikit_nlp-0.4.9/caikit_nlp/toolkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3285 2024-04-25 04:47:06.000000 caikit_nlp-0.4.9/caikit_nlp/toolkit/data_stream_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-04-25 04:47:06.000000 caikit_nlp-0.4.9/caikit_nlp/toolkit/data_type_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-04-25 04:47:06.000000 caikit_nlp-0.4.9/caikit_nlp/toolkit/task_specific_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:47:13.734450 caikit_nlp-0.4.9/caikit_nlp/toolkit/text_generation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:47:06.000000 caikit_nlp-0.4.9/caikit_nlp/toolkit/text_generation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16766 2024-04-25 04:47:06.000000 caikit_nlp-0.4.9/caikit_nlp/toolkit/text_generation/model_run_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19662 2024-04-25 04:47:06.000000 caikit_nlp-0.4.9/caikit_nlp/toolkit/text_generation/tgis_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-04-25 04:47:06.000000 caikit_nlp-0.4.9/caikit_nlp/toolkit/torch_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-04-25 04:47:06.000000 caikit_nlp-0.4.9/caikit_nlp/toolkit/trainer_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3986 2024-04-25 04:47:06.000000 caikit_nlp-0.4.9/caikit_nlp/toolkit/verbalizer_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-25 04:47:06.000000 caikit_nlp-0.4.9/caikit_nlp/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:47:13.746450 caikit_nlp-0.4.9/caikit_nlp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11431 2024-04-25 04:47:13.000000 caikit_nlp-0.4.9/caikit_nlp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5729 2024-04-25 04:47:13.000000 caikit_nlp-0.4.9/caikit_nlp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 04:47:13.000000 caikit_nlp-0.4.9/caikit_nlp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-25 04:47:13.000000 caikit_nlp-0.4.9/caikit_nlp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-25 04:47:13.000000 caikit_nlp-0.4.9/caikit_nlp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-25 04:47:06.000000 caikit_nlp-0.4.9/code-of-conduct.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:47:13.734450 caikit_nlp-0.4.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)    55479 2024-04-25 04:47:06.000000 caikit_nlp-0.4.9/examples/Caikit_Getting_Started.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-04-25 04:47:06.000000 caikit_nlp-0.4.9/examples/compare_local_vs_tgis_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7104 2024-04-25 04:47:06.000000 caikit_nlp-0.4.9/examples/evaluate_model.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      404 2024-04-25 04:47:06.000000 caikit_nlp-0.4.9/examples/kill-text-generation-launcher.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-04-25 04:47:06.000000 caikit_nlp-0.4.9/examples/load_and_run_distributed_peft.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13678 2024-04-25 04:47:06.000000 caikit_nlp-0.4.9/examples/run_fine_tuning.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15840 2024-04-25 04:47:06.000000 caikit_nlp-0.4.9/examples/run_peft_tuning.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1992 2024-04-25 04:47:06.000000 caikit_nlp-0.4.9/examples/text-generation-launcher
+-rw-r--r--   0 runner    (1001) docker     (127)    15815 2024-04-25 04:47:06.000000 caikit_nlp-0.4.9/examples/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6158 2024-04-25 04:47:06.000000 caikit_nlp-0.4.9/prompt_tuning_parameter_selection.md
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-25 04:47:06.000000 caikit_nlp-0.4.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-04-25 04:47:06.000000 caikit_nlp-0.4.9/runtime_config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:47:13.734450 caikit_nlp-0.4.9/runtime_template/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1252 2024-04-25 04:47:06.000000 caikit_nlp-0.4.9/runtime_template/run_with_gateway.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:47:13.734450 caikit_nlp-0.4.9/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      657 2024-04-25 04:47:06.000000 caikit_nlp-0.4.9/scripts/dump_apis.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      720 2024-04-25 04:47:06.000000 caikit_nlp-0.4.9/scripts/fmt.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      231 2024-04-25 04:47:06.000000 caikit_nlp-0.4.9/scripts/run_local.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 04:47:13.746450 caikit_nlp-0.4.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-25 04:47:06.000000 caikit_nlp-0.4.9/setup_requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:47:13.734450 caikit_nlp-0.4.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:47:06.000000 caikit_nlp-0.4.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-04-25 04:47:06.000000 caikit_nlp-0.4.9/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:47:13.734450 caikit_nlp-0.4.9/tests/data_model/
+-rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-04-25 04:47:06.000000 caikit_nlp-0.4.9/tests/data_model/test_generation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:47:13.734450 caikit_nlp-0.4.9/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)    11719 2024-04-25 04:47:06.000000 caikit_nlp-0.4.9/tests/fixtures/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:47:13.734450 caikit_nlp-0.4.9/tests/fixtures/data_model/
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-25 04:47:06.000000 caikit_nlp-0.4.9/tests/fixtures/data_model/sample_objects.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:47:13.734450 caikit_nlp-0.4.9/tests/fixtures/tiny_models/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:47:13.738450 caikit_nlp-0.4.9/tests/fixtures/tiny_models/BertForSequenceClassification/
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-25 04:47:06.000000 caikit_nlp-0.4.9/tests/fixtures/tiny_models/BertForSequenceClassification/config.json
+-rw-r--r--   0 runner    (1001) docker     (127)   384767 2024-04-25 04:47:06.000000 caikit_nlp-0.4.9/tests/fixtures/tiny_models/BertForSequenceClassification/pytorch_model.bin
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-25 04:47:06.000000 caikit_nlp-0.4.9/tests/fixtures/tiny_models/BertForSequenceClassification/special_tokens_map.json
+-rw-r--r--   0 runner    (1001) docker     (127)   481096 2024-04-25 04:47:06.000000 caikit_nlp-0.4.9/tests/fixtures/tiny_models/BertForSequenceClassification/tf_model.h5
+-rw-r--r--   0 runner    (1001) docker     (127)    23061 2024-04-25 04:47:06.000000 caikit_nlp-0.4.9/tests/fixtures/tiny_models/BertForSequenceClassification/tokenizer.json
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-25 04:47:06.000000 caikit_nlp-0.4.9/tests/fixtures/tiny_models/BertForSequenceClassification/tokenizer_config.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4679 2024-04-25 04:47:06.000000 caikit_nlp-0.4.9/tests/fixtures/tiny_models/BertForSequenceClassification/vocab.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:47:13.742450 caikit_nlp-0.4.9/tests/fixtures/tiny_models/BloomForCausalLM/
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-25 04:47:06.000000 caikit_nlp-0.4.9/tests/fixtures/tiny_models/BloomForCausalLM/config.json
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-25 04:47:06.000000 caikit_nlp-0.4.9/tests/fixtures/tiny_models/BloomForCausalLM/generation_config.json
+-rw-r--r--   0 runner    (1001) docker     (127)   406260 2024-04-25 04:47:06.000000 caikit_nlp-0.4.9/tests/fixtures/tiny_models/BloomForCausalLM/pytorch_model.bin
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-25 04:47:06.000000 caikit_nlp-0.4.9/tests/fixtures/tiny_models/BloomForCausalLM/special_tokens_map.json
+-rw-r--r--   0 runner    (1001) docker     (127)    33054 2024-04-25 04:47:06.000000 caikit_nlp-0.4.9/tests/fixtures/tiny_models/BloomForCausalLM/tokenizer.json
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-25 04:47:06.000000 caikit_nlp-0.4.9/tests/fixtures/tiny_models/BloomForCausalLM/tokenizer_config.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-04-25 04:47:06.000000 caikit_nlp-0.4.9/tests/fixtures/tiny_models/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:47:13.742450 caikit_nlp-0.4.9/tests/fixtures/tiny_models/T5ForConditionalGeneration/
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-25 04:47:06.000000 caikit_nlp-0.4.9/tests/fixtures/tiny_models/T5ForConditionalGeneration/config.json
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-25 04:47:06.000000 caikit_nlp-0.4.9/tests/fixtures/tiny_models/T5ForConditionalGeneration/generation_config.json
+-rw-r--r--   0 runner    (1001) docker     (127)   546693 2024-04-25 04:47:06.000000 caikit_nlp-0.4.9/tests/fixtures/tiny_models/T5ForConditionalGeneration/pytorch_model.bin
+-rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-04-25 04:47:06.000000 caikit_nlp-0.4.9/tests/fixtures/tiny_models/T5ForConditionalGeneration/special_tokens_map.json
+-rw-r--r--   0 runner    (1001) docker     (127)   382892 2024-04-25 04:47:06.000000 caikit_nlp-0.4.9/tests/fixtures/tiny_models/T5ForConditionalGeneration/tokenizer.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-04-25 04:47:06.000000 caikit_nlp-0.4.9/tests/fixtures/tiny_models/T5ForConditionalGeneration/tokenizer_config.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:47:13.742450 caikit_nlp-0.4.9/tests/model_management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:47:06.000000 caikit_nlp-0.4.9/tests/model_management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9024 2024-04-25 04:47:06.000000 caikit_nlp-0.4.9/tests/model_management/test_tgis_auto_finder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:47:13.742450 caikit_nlp-0.4.9/tests/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:47:06.000000 caikit_nlp-0.4.9/tests/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:47:13.742450 caikit_nlp-0.4.9/tests/modules/text_classification/
+-rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-04-25 04:47:06.000000 caikit_nlp-0.4.9/tests/modules/text_classification/test_sequence_classification.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:47:13.742450 caikit_nlp-0.4.9/tests/modules/text_embedding/
+-rw-r--r--   0 runner    (1001) docker     (127)    39151 2024-04-25 04:47:06.000000 caikit_nlp-0.4.9/tests/modules/text_embedding/test_embedding.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:47:13.746450 caikit_nlp-0.4.9/tests/modules/text_generation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:47:06.000000 caikit_nlp-0.4.9/tests/modules/text_generation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3501 2024-04-25 04:47:06.000000 caikit_nlp-0.4.9/tests/modules/text_generation/test_peft_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25997 2024-04-25 04:47:06.000000 caikit_nlp-0.4.9/tests/modules/text_generation/test_peft_prompt_tuning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6540 2024-04-25 04:47:06.000000 caikit_nlp-0.4.9/tests/modules/text_generation/test_peft_tgis_remote.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7458 2024-04-25 04:47:06.000000 caikit_nlp-0.4.9/tests/modules/text_generation/test_text_generation_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8300 2024-04-25 04:47:06.000000 caikit_nlp-0.4.9/tests/modules/text_generation/test_text_generation_tgis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:47:13.746450 caikit_nlp-0.4.9/tests/modules/token_classification/
+-rw-r--r--   0 runner    (1001) docker     (127)    18398 2024-04-25 04:47:06.000000 caikit_nlp-0.4.9/tests/modules/token_classification/test_filtered_span_classification.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:47:13.746450 caikit_nlp-0.4.9/tests/modules/tokenization/
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-04-25 04:47:06.000000 caikit_nlp-0.4.9/tests/modules/tokenization/test_regex_sentence_splitter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:47:13.746450 caikit_nlp-0.4.9/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:47:06.000000 caikit_nlp-0.4.9/tests/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16904 2024-04-25 04:47:06.000000 caikit_nlp-0.4.9/tests/resources/test_pretrained_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:47:13.746450 caikit_nlp-0.4.9/tests/toolkit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 04:47:06.000000 caikit_nlp-0.4.9/tests/toolkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4087 2024-04-25 04:47:06.000000 caikit_nlp-0.4.9/tests/toolkit/test_data_stream_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-04-25 04:47:06.000000 caikit_nlp-0.4.9/tests/toolkit/test_data_type_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2363 2024-04-25 04:47:06.000000 caikit_nlp-0.4.9/tests/toolkit/test_task_specific_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3650 2024-04-25 04:47:06.000000 caikit_nlp-0.4.9/tests/toolkit/test_verbalizers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 04:47:13.746450 caikit_nlp-0.4.9/tests/toolkit/text_generation/
+-rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-04-25 04:47:06.000000 caikit_nlp-0.4.9/tests/toolkit/text_generation/test_model_run_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-25 04:47:06.000000 caikit_nlp-0.4.9/tox.ini
```

### Comparing `caikit-nlp-0.4.8/.github/ISSUE_TEMPLATE/bug_report.md` & `caikit_nlp-0.4.9/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.8/.github/ISSUE_TEMPLATE/feature_request.md` & `caikit_nlp-0.4.9/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.8/.github/ISSUE_TEMPLATE/user_story.md` & `caikit_nlp-0.4.9/.github/ISSUE_TEMPLATE/user_story.md`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.8/.github/workflows/build-image.yml` & `caikit_nlp-0.4.9/.github/workflows/build-image.yml`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.8/.github/workflows/build-library.yml` & `caikit_nlp-0.4.9/.github/workflows/build-library.yml`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.8/.github/workflows/lint-code.yml` & `caikit_nlp-0.4.9/.github/workflows/lint-code.yml`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.8/.github/workflows/publish-library.yml` & `caikit_nlp-0.4.9/.github/workflows/publish-library.yml`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.8/.gitignore` & `caikit_nlp-0.4.9/.gitignore`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.8/.pylintrc` & `caikit_nlp-0.4.9/.pylintrc`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.8/CONTRIBUTING.md` & `caikit_nlp-0.4.9/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.8/Dockerfile` & `caikit_nlp-0.4.9/Dockerfile`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.8/LICENSE` & `caikit_nlp-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.8/PKG-INFO` & `caikit_nlp-0.4.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caikit-nlp
-Version: 0.4.8
+Version: 0.4.9
 Summary: Caikit NLP
 License: Apache-2.0
 Project-URL: Source, https://github.com/caikit/caikit-nlp
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: ~=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -15,15 +15,15 @@
 Requires-Dist: huggingface-hub
 Requires-Dist: numpy>=1.22.4
 Requires-Dist: pandas>=1.5.0
 Requires-Dist: scikit-learn>=1.1
 Requires-Dist: scipy>=1.8.1
 Requires-Dist: sentence-transformers<2.4.0,>=2.3.1
 Requires-Dist: tokenizers>=0.13.3
-Requires-Dist: torch>=2.0.1
+Requires-Dist: torch<2.3.0,>=2.0.1
 Requires-Dist: tqdm>=4.65.0
 Requires-Dist: transformers>=4.32.0
 Requires-Dist: peft==0.6.0
 
 # Caikit NLP
 
 Caikit-NLP is a python library providing various Natural Language Processing (NLP) capabilities built on top of [caikit](https://github.com/caikit/caikit) framework.
```

### Comparing `caikit-nlp-0.4.8/README.md` & `caikit_nlp-0.4.9/README.md`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.8/benchmarks/README.md` & `caikit_nlp-0.4.9/benchmarks/README.md`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.8/benchmarks/logs/llama2-7b/20230905_183655.output` & `caikit_nlp-0.4.9/benchmarks/logs/llama2-7b/20230905_183655.output`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.8/benchmarks/logs/llama2-7b/20230905_184809.output` & `caikit_nlp-0.4.9/benchmarks/logs/llama2-7b/20230905_184809.output`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.8/benchmarks/logs/llama2-7b/20230905_191650.output` & `caikit_nlp-0.4.9/benchmarks/logs/llama2-7b/20230905_191650.output`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.8/benchmarks/logs/llama2-7b/20230905_194133.output` & `caikit_nlp-0.4.9/benchmarks/logs/llama2-7b/20230905_194133.output`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.8/benchmarks/logs/llama2-7b/20230906_135211.output` & `caikit_nlp-0.4.9/benchmarks/logs/llama2-7b/20230906_135211.output`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.8/caikit_nlp/__init__.py` & `caikit_nlp-0.4.9/caikit_nlp/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.8/caikit_nlp/config/__init__.py` & `caikit_nlp-0.4.9/caikit_nlp/config/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.8/caikit_nlp/config/config.yml` & `caikit_nlp-0.4.9/caikit_nlp/config/config.yml`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.8/caikit_nlp/data_model/__init__.py` & `caikit_nlp-0.4.9/caikit_nlp/data_model/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.8/caikit_nlp/data_model/generation.py` & `caikit_nlp-0.4.9/caikit_nlp/data_model/generation.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.8/caikit_nlp/model_management/__init__.py` & `caikit_nlp-0.4.9/caikit_nlp/model_management/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.8/caikit_nlp/model_management/tgis_auto_finder.py` & `caikit_nlp-0.4.9/caikit_nlp/model_management/tgis_auto_finder.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.8/caikit_nlp/modules/__init__.py` & `caikit_nlp-0.4.9/caikit_nlp/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.8/caikit_nlp/modules/text_classification/__init__.py` & `caikit_nlp-0.4.9/caikit_nlp/modules/text_classification/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.8/caikit_nlp/modules/text_classification/sequence_classification.py` & `caikit_nlp-0.4.9/caikit_nlp/modules/text_classification/sequence_classification.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.8/caikit_nlp/modules/text_embedding/__init__.py` & `caikit_nlp-0.4.9/caikit_nlp/modules/text_embedding/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.8/caikit_nlp/modules/text_embedding/embedding.py` & `caikit_nlp-0.4.9/caikit_nlp/modules/text_embedding/embedding.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.8/caikit_nlp/modules/text_embedding/utils.py` & `caikit_nlp-0.4.9/caikit_nlp/modules/text_embedding/utils.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.8/caikit_nlp/modules/text_generation/__init__.py` & `caikit_nlp-0.4.9/caikit_nlp/modules/text_generation/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.8/caikit_nlp/modules/text_generation/peft_config.py` & `caikit_nlp-0.4.9/caikit_nlp/modules/text_generation/peft_config.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.8/caikit_nlp/modules/text_generation/peft_prompt_tuning.py` & `caikit_nlp-0.4.9/caikit_nlp/modules/text_generation/peft_prompt_tuning.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,16 +44,17 @@
 from caikit.core.data_model import DataStream
 from caikit.core.exceptions import error_handler
 from caikit.core.modules import ModuleBase, ModuleConfig, ModuleSaver, module
 from caikit.interfaces.nlp.data_model import (
     ClassificationTrainRecord,
     GeneratedTextResult,
     GeneratedTextStreamResult,
+    TokenizationResults,
 )
-from caikit.interfaces.nlp.tasks import TextGenerationTask
+from caikit.interfaces.nlp.tasks import TextGenerationTask, TokenizationTask
 import alog
 
 # Local
 from ...data_model import (
     ExponentialDecayLengthPenalty,
     GenerationTrainRecord,
     PromptOutputModelType,
@@ -83,15 +84,15 @@
 
 # TODO: try to refactor this into a smaller module
 # pylint: disable=too-many-lines,too-many-instance-attributes
 @module(
     id="6655831b-960a-4dc5-8df4-867026e2cd41",
     name="Peft generation",
     version="0.1.0",
-    task=TextGenerationTask,
+    tasks=[TextGenerationTask, TokenizationTask],
 )
 class PeftPromptTuning(ModuleBase):
 
     _DETECT_DEVICE = "__DETECT__"
     _ENCODER_KEY = PromptOutputModelType.ENCODER
     _DECODER_KEY = PromptOutputModelType.DECODER
     _ADAPTER_NAME = "default"
@@ -270,14 +271,30 @@
             seed=seed,
             repetition_penalty=repetition_penalty,
             max_time=max_time,
             exponential_decay_length_penalty=exponential_decay_length_penalty,
             stop_sequences=stop_sequences,
         )
 
+    @TokenizationTask.taskmethod()
+    def run_tokenizer(
+        self,
+        text: str,
+    ) -> TokenizationResults:
+        """Run tokenization task against the model
+
+        Args:
+           text: str
+                Text to tokenize
+        Returns:
+            TokenizationResults
+                The token count
+        """
+        raise NotImplementedError("Tokenization not implemented for local")
+
     @classmethod
     def train(
         cls,
         base_model: str,  # TODO: Union[str, PretrainedModelBase]
         train_stream: Union[
             DataStream[GenerationTrainRecord],
             DataStream[ClassificationTrainRecord],
```

### Comparing `caikit-nlp-0.4.8/caikit_nlp/modules/text_generation/peft_tgis_remote.py` & `caikit_nlp-0.4.9/caikit_nlp/modules/text_generation/peft_tgis_remote.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.8/caikit_nlp/modules/text_generation/text_generation_local.py` & `caikit_nlp-0.4.9/caikit_nlp/modules/text_generation/text_generation_local.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,16 +27,16 @@
 import torch
 
 # First Party
 from caikit import get_config
 from caikit.core.data_model import DataStream
 from caikit.core.exceptions import error_handler
 from caikit.core.modules import ModuleBase, ModuleConfig, ModuleSaver, module
-from caikit.interfaces.nlp.data_model import GeneratedTextResult
-from caikit.interfaces.nlp.tasks import TextGenerationTask
+from caikit.interfaces.nlp.data_model import GeneratedTextResult, TokenizationResults
+from caikit.interfaces.nlp.tasks import TextGenerationTask, TokenizationTask
 import alog
 
 # Local
 from ...data_model import GenerationTrainRecord
 from ...resources.pretrained_model import (
     HFAutoCausalLM,
     HFAutoSeq2SeqLM,
@@ -56,15 +56,15 @@
 TRAINING_LOSS_LOG_FILENAME = "training_logs.jsonl"
 
 # pylint: disable=too-many-lines,too-many-instance-attributes
 @module(
     id="f9181353-4ccf-4572-bd1e-f12bcda26792",
     name="Text Generation",
     version="0.1.0",
-    task=TextGenerationTask,
+    tasks=[TextGenerationTask, TokenizationTask],
 )
 class TextGeneration(ModuleBase):
     """Module to provide text generation capabilities"""
 
     RANDOM_SEED = 73
     supported_resources = [HFAutoCausalLM, HFAutoSeq2SeqLM]
 
@@ -517,14 +517,15 @@
                     encoding="utf-8",
                 ) as f:
                     for loss_log in loss_log_lines:
                         loss_log = {"name": "loss", "data": loss_log}
                         json.dump(loss_log, f)
                         f.write("\n")
 
+    @TextGenerationTask.taskmethod()
     def run(
         self,
         text: str,
         max_new_tokens: Optional[int] = 20,
         min_new_tokens: Optional[int] = 0,
         truncate_input_tokens: Optional[int] = 0,
         decoding_method: Optional[str] = "GREEDY",
@@ -571,14 +572,30 @@
             repetition_penalty=repetition_penalty,
             max_time=max_time,
             preserve_input_text=preserve_input_text,
             task_type=self.model.TASK_TYPE,
             **kwargs,
         )
 
+    @TokenizationTask.taskmethod()
+    def run_tokenizer(
+        self,
+        text: str,
+    ) -> TokenizationResults:
+        """Run tokenization task against the model
+
+        Args:
+           text: str
+                Text to tokenize
+        Returns:
+            TokenizationResults
+                The token count
+        """
+        raise NotImplementedError("Tokenization not implemented for local")
+
     ################################## Private Functions ######################################
 
     @staticmethod
     def _preprocess_function(
         base_model: PretrainedModelBase,
         train_stream: DataStream[GenerationTrainRecord],
         tokenizer: AutoTokenizer,
```

### Comparing `caikit-nlp-0.4.8/caikit_nlp/modules/text_generation/text_generation_tgis.py` & `caikit_nlp-0.4.9/caikit_nlp/modules/text_generation/text_generation_tgis.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.8/caikit_nlp/modules/token_classification/__init__.py` & `caikit_nlp-0.4.9/caikit_nlp/modules/token_classification/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.8/caikit_nlp/modules/token_classification/filtered_span_classification.py` & `caikit_nlp-0.4.9/caikit_nlp/modules/token_classification/filtered_span_classification.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.8/caikit_nlp/modules/tokenization/__init__.py` & `caikit_nlp-0.4.9/caikit_nlp/modules/tokenization/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.8/caikit_nlp/modules/tokenization/regex_sentence_splitter.py` & `caikit_nlp-0.4.9/caikit_nlp/modules/tokenization/regex_sentence_splitter.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.8/caikit_nlp/resources/__init__.py` & `caikit_nlp-0.4.9/caikit_nlp/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.8/caikit_nlp/resources/pretrained_model/__init__.py` & `caikit_nlp-0.4.9/caikit_nlp/resources/pretrained_model/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.8/caikit_nlp/resources/pretrained_model/base.py` & `caikit_nlp-0.4.9/caikit_nlp/resources/pretrained_model/base.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.8/caikit_nlp/resources/pretrained_model/hf_auto_causal_lm.py` & `caikit_nlp-0.4.9/caikit_nlp/resources/pretrained_model/hf_auto_causal_lm.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.8/caikit_nlp/resources/pretrained_model/hf_auto_seq2seq_lm.py` & `caikit_nlp-0.4.9/caikit_nlp/resources/pretrained_model/hf_auto_seq2seq_lm.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.8/caikit_nlp/resources/pretrained_model/hf_auto_seq_classifier.py` & `caikit_nlp-0.4.9/caikit_nlp/resources/pretrained_model/hf_auto_seq_classifier.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.8/caikit_nlp/toolkit/data_stream_wrapper.py` & `caikit_nlp-0.4.9/caikit_nlp/toolkit/data_stream_wrapper.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.8/caikit_nlp/toolkit/data_type_utils.py` & `caikit_nlp-0.4.9/caikit_nlp/toolkit/data_type_utils.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.8/caikit_nlp/toolkit/task_specific_utils.py` & `caikit_nlp-0.4.9/caikit_nlp/toolkit/task_specific_utils.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.8/caikit_nlp/toolkit/text_generation/model_run_utils.py` & `caikit_nlp-0.4.9/caikit_nlp/toolkit/text_generation/model_run_utils.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.8/caikit_nlp/toolkit/text_generation/tgis_utils.py` & `caikit_nlp-0.4.9/caikit_nlp/toolkit/text_generation/tgis_utils.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.8/caikit_nlp/toolkit/torch_run.py` & `caikit_nlp-0.4.9/caikit_nlp/toolkit/torch_run.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,15 +20,16 @@
 """
 
 # Standard
 import os
 
 # Third Party
 from torch import cuda
-from torch.distributed.launcher.api import LaunchConfig, Std
+from torch.distributed.elastic.multiprocessing.api import Std
+from torch.distributed.launcher.api import LaunchConfig
 import torch.distributed as dist
 
 # First Party
 import alog
 
 log = alog.use_channel("TRCH_RN")
```

### Comparing `caikit-nlp-0.4.8/caikit_nlp/toolkit/trainer_utils.py` & `caikit_nlp-0.4.9/caikit_nlp/toolkit/trainer_utils.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.8/caikit_nlp/toolkit/verbalizer_utils.py` & `caikit_nlp-0.4.9/caikit_nlp/toolkit/verbalizer_utils.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.8/caikit_nlp.egg-info/PKG-INFO` & `caikit_nlp-0.4.9/caikit_nlp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caikit-nlp
-Version: 0.4.8
+Version: 0.4.9
 Summary: Caikit NLP
 License: Apache-2.0
 Project-URL: Source, https://github.com/caikit/caikit-nlp
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: ~=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -15,15 +15,15 @@
 Requires-Dist: huggingface-hub
 Requires-Dist: numpy>=1.22.4
 Requires-Dist: pandas>=1.5.0
 Requires-Dist: scikit-learn>=1.1
 Requires-Dist: scipy>=1.8.1
 Requires-Dist: sentence-transformers<2.4.0,>=2.3.1
 Requires-Dist: tokenizers>=0.13.3
-Requires-Dist: torch>=2.0.1
+Requires-Dist: torch<2.3.0,>=2.0.1
 Requires-Dist: tqdm>=4.65.0
 Requires-Dist: transformers>=4.32.0
 Requires-Dist: peft==0.6.0
 
 # Caikit NLP
 
 Caikit-NLP is a python library providing various Natural Language Processing (NLP) capabilities built on top of [caikit](https://github.com/caikit/caikit) framework.
```

### Comparing `caikit-nlp-0.4.8/caikit_nlp.egg-info/SOURCES.txt` & `caikit_nlp-0.4.9/caikit_nlp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.8/examples/Caikit_Getting_Started.ipynb` & `caikit_nlp-0.4.9/examples/Caikit_Getting_Started.ipynb`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.8/examples/compare_local_vs_tgis_models.py` & `caikit_nlp-0.4.9/examples/compare_local_vs_tgis_models.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.8/examples/evaluate_model.py` & `caikit_nlp-0.4.9/examples/evaluate_model.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.8/examples/load_and_run_distributed_peft.py` & `caikit_nlp-0.4.9/examples/load_and_run_distributed_peft.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.8/examples/run_fine_tuning.py` & `caikit_nlp-0.4.9/examples/run_fine_tuning.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.8/examples/run_peft_tuning.py` & `caikit_nlp-0.4.9/examples/run_peft_tuning.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.8/examples/text-generation-launcher` & `caikit_nlp-0.4.9/examples/text-generation-launcher`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.8/examples/utils.py` & `caikit_nlp-0.4.9/examples/utils.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.8/prompt_tuning_parameter_selection.md` & `caikit_nlp-0.4.9/prompt_tuning_parameter_selection.md`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.8/pyproject.toml` & `caikit_nlp-0.4.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     "huggingface-hub",
     "numpy>=1.22.4",
     "pandas>=1.5.0",
     "scikit-learn>=1.1",
     "scipy>=1.8.1",
     "sentence-transformers>=2.3.1,<2.4.0",
     "tokenizers>=0.13.3",
-    "torch>=2.0.1",
+    "torch>=2.0.1,<2.3.0",
     "tqdm>=4.65.0",
     "transformers>=4.32.0",
     "peft==0.6.0",
 ]
 
 [tool.setuptools.packages.find]
 exclude = ["tests", "tests.*"]
```

### Comparing `caikit-nlp-0.4.8/runtime_config.yaml` & `caikit_nlp-0.4.9/runtime_config.yaml`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.8/runtime_template/run_with_gateway.sh` & `caikit_nlp-0.4.9/runtime_template/run_with_gateway.sh`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.8/scripts/dump_apis.sh` & `caikit_nlp-0.4.9/scripts/dump_apis.sh`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.8/scripts/fmt.sh` & `caikit_nlp-0.4.9/scripts/fmt.sh`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.8/tests/conftest.py` & `caikit_nlp-0.4.9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.8/tests/data_model/test_generation.py` & `caikit_nlp-0.4.9/tests/data_model/test_generation.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.8/tests/fixtures/__init__.py` & `caikit_nlp-0.4.9/tests/fixtures/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.8/tests/fixtures/data_model/sample_objects.py` & `caikit_nlp-0.4.9/tests/fixtures/data_model/sample_objects.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.8/tests/fixtures/tiny_models/BertForSequenceClassification/config.json` & `caikit_nlp-0.4.9/tests/fixtures/tiny_models/BertForSequenceClassification/config.json`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.8/tests/fixtures/tiny_models/BertForSequenceClassification/pytorch_model.bin` & `caikit_nlp-0.4.9/tests/fixtures/tiny_models/BertForSequenceClassification/pytorch_model.bin`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.8/tests/fixtures/tiny_models/BertForSequenceClassification/tf_model.h5` & `caikit_nlp-0.4.9/tests/fixtures/tiny_models/BertForSequenceClassification/tf_model.h5`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.8/tests/fixtures/tiny_models/BertForSequenceClassification/tokenizer.json` & `caikit_nlp-0.4.9/tests/fixtures/tiny_models/BertForSequenceClassification/tokenizer.json`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.8/tests/fixtures/tiny_models/BertForSequenceClassification/vocab.txt` & `caikit_nlp-0.4.9/tests/fixtures/tiny_models/BertForSequenceClassification/vocab.txt`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.8/tests/fixtures/tiny_models/BloomForCausalLM/config.json` & `caikit_nlp-0.4.9/tests/fixtures/tiny_models/BloomForCausalLM/config.json`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.8/tests/fixtures/tiny_models/BloomForCausalLM/pytorch_model.bin` & `caikit_nlp-0.4.9/tests/fixtures/tiny_models/BloomForCausalLM/pytorch_model.bin`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.8/tests/fixtures/tiny_models/BloomForCausalLM/tokenizer.json` & `caikit_nlp-0.4.9/tests/fixtures/tiny_models/BloomForCausalLM/tokenizer.json`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.8/tests/fixtures/tiny_models/README.md` & `caikit_nlp-0.4.9/tests/fixtures/tiny_models/README.md`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.8/tests/fixtures/tiny_models/T5ForConditionalGeneration/config.json` & `caikit_nlp-0.4.9/tests/fixtures/tiny_models/T5ForConditionalGeneration/config.json`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.8/tests/fixtures/tiny_models/T5ForConditionalGeneration/pytorch_model.bin` & `caikit_nlp-0.4.9/tests/fixtures/tiny_models/T5ForConditionalGeneration/pytorch_model.bin`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.8/tests/fixtures/tiny_models/T5ForConditionalGeneration/special_tokens_map.json` & `caikit_nlp-0.4.9/tests/fixtures/tiny_models/T5ForConditionalGeneration/special_tokens_map.json`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.8/tests/fixtures/tiny_models/T5ForConditionalGeneration/tokenizer.json` & `caikit_nlp-0.4.9/tests/fixtures/tiny_models/T5ForConditionalGeneration/tokenizer.json`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.8/tests/fixtures/tiny_models/T5ForConditionalGeneration/tokenizer_config.json` & `caikit_nlp-0.4.9/tests/fixtures/tiny_models/T5ForConditionalGeneration/tokenizer_config.json`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.8/tests/model_management/test_tgis_auto_finder.py` & `caikit_nlp-0.4.9/tests/model_management/test_tgis_auto_finder.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.8/tests/modules/text_classification/test_sequence_classification.py` & `caikit_nlp-0.4.9/tests/modules/text_classification/test_sequence_classification.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.8/tests/modules/text_embedding/test_embedding.py` & `caikit_nlp-0.4.9/tests/modules/text_embedding/test_embedding.py`

 * *Files 4% similar despite different names*

```diff
@@ -1050,7 +1050,47 @@
         truncate_input_tokens=123,
         implicit_truncation_errors=False,
     )
     assert isinstance(ret, np.ndarray)
     BOOTSTRAPPED_MODEL._encode_with_retry(
         "text here"
     )  # and no KeyError trying to remove non-existing keys
+
+
+@pytest.mark.parametrize(
+    "truncate_input_tokens",
+    [0, 1, 2, 3, 4, 5, 99, 100, 101, 300, 510, 511, 512, 513, 1000, -1],
+)
+def test_same_same(loaded_model: EmbeddingModule, truncate_input_tokens):
+    """Confirm that same text gives same results"""
+
+    inputs = ["What is generative ai?", "What is generative ai?", "different"]
+
+    # First ensuring that batch input vs loop over inputs is the same
+    separate_embeddings = [
+        loaded_model.run_embedding(text=i, truncate_input_tokens=truncate_input_tokens)
+        for i in inputs
+    ]
+    combined_embeddings = loaded_model.run_embeddings(
+        texts=inputs, truncate_input_tokens=truncate_input_tokens
+    )
+
+    separate_vectors = [
+        e.to_dict()["result"]["data"]["values"] for e in separate_embeddings
+    ]
+    combined_vectors = [
+        e["data"]["values"] for e in combined_embeddings.to_dict()["results"]["vectors"]
+    ]
+
+    assert len(separate_vectors) == len(
+        combined_vectors
+    ), "expected the same number separate and combined embeddings"
+
+    # test order by comparing value of individual embeddings in sequence
+    for i, e in enumerate(separate_vectors):
+        assert np.allclose(e, combined_vectors[i])
+
+    # Next ensuring that the two identical sentences yield identical results (and 3rd does not)
+    assert np.array_equal(combined_vectors[0], combined_vectors[1])
+    assert not np.array_equal(combined_vectors[1], combined_vectors[2])
+    assert np.array_equal(separate_vectors[0], separate_vectors[1])
+    assert not np.array_equal(separate_vectors[1], separate_vectors[2])
```

### Comparing `caikit-nlp-0.4.8/tests/modules/text_generation/test_peft_config.py` & `caikit_nlp-0.4.9/tests/modules/text_generation/test_peft_config.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.8/tests/modules/text_generation/test_peft_prompt_tuning.py` & `caikit_nlp-0.4.9/tests/modules/text_generation/test_peft_prompt_tuning.py`

 * *Files 2% similar despite different names*

```diff
@@ -425,14 +425,22 @@
         decoding_method="GREEDY",
         stop_sequences=["Foo", "bar"],
         exponential_decay_length_penalty=penalty,
     )
     assert isinstance(pred, GeneratedTextResult)
 
 
+def test_run_tokenizer_not_implemented(causal_lm_dummy_model):
+    with pytest.raises(NotImplementedError):
+        causal_lm_dummy_model.run_tokenizer("This text doesn't matter")
+
+
+######################## Test train ###############################################
+
+
 def test_train_with_data_validation_raises(causal_lm_train_kwargs, set_cpu_device):
     """Check if we are able to throw error for when number of examples are more than configured limit"""
     patch_kwargs = {
         "num_epochs": 1,
         "verbalizer": "Tweet text : {{input}} Label : ",
         "train_stream": caikit.core.data_model.DataStream.from_iterable(
             [
```

### Comparing `caikit-nlp-0.4.8/tests/modules/text_generation/test_peft_tgis_remote.py` & `caikit_nlp-0.4.9/tests/modules/text_generation/test_peft_tgis_remote.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.8/tests/modules/text_generation/test_text_generation_local.py` & `caikit_nlp-0.4.9/tests/modules/text_generation/test_text_generation_local.py`

 * *Files 3% similar despite different names*

```diff
@@ -205,7 +205,13 @@
                 ),
             ]
         ),
         "torch_dtype": torch.float32,
     }
     model = TextGeneration.train(**train_kwargs)
     assert isinstance(model.model, HFAutoSeq2SeqLM)
+
+
+def test_run_tokenizer_not_implemented():
+    with pytest.raises(NotImplementedError):
+        model = TextGeneration.bootstrap(SEQ2SEQ_LM_MODEL)
+        model.run_tokenizer("This text doesn't matter")
```

### Comparing `caikit-nlp-0.4.8/tests/modules/text_generation/test_text_generation_tgis.py` & `caikit_nlp-0.4.9/tests/modules/text_generation/test_text_generation_tgis.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.8/tests/modules/token_classification/test_filtered_span_classification.py` & `caikit_nlp-0.4.9/tests/modules/token_classification/test_filtered_span_classification.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.8/tests/modules/tokenization/test_regex_sentence_splitter.py` & `caikit_nlp-0.4.9/tests/modules/tokenization/test_regex_sentence_splitter.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.8/tests/resources/test_pretrained_model.py` & `caikit_nlp-0.4.9/tests/resources/test_pretrained_model.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.8/tests/toolkit/test_data_stream_wrapper.py` & `caikit_nlp-0.4.9/tests/toolkit/test_data_stream_wrapper.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.8/tests/toolkit/test_data_type_utils.py` & `caikit_nlp-0.4.9/tests/toolkit/test_data_type_utils.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.8/tests/toolkit/test_task_specific_utils.py` & `caikit_nlp-0.4.9/tests/toolkit/test_task_specific_utils.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.8/tests/toolkit/test_verbalizers.py` & `caikit_nlp-0.4.9/tests/toolkit/test_verbalizers.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.8/tests/toolkit/text_generation/test_model_run_utils.py` & `caikit_nlp-0.4.9/tests/toolkit/text_generation/test_model_run_utils.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.8/tox.ini` & `caikit_nlp-0.4.9/tox.ini`

 * *Files identical despite different names*


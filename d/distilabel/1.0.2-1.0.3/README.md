# Comparing `tmp/distilabel-1.0.2.tar.gz` & `tmp/distilabel-1.0.3.tar.gz`

## Comparing `distilabel-1.0.2.tar` & `distilabel-1.0.3.tar`

### file list

```diff
@@ -1,256 +1,256 @@
--rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 distilabel-1.0.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 distilabel-1.0.2/Makefile
--rw-r--r--   0        0        0     5115 2020-02-02 00:00:00.000000 distilabel-1.0.2/mkdocs.yml
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 distilabel-1.0.2/.github/ISSUE_TEMPLATE/blank-issue-template.md
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 distilabel-1.0.2/.github/ISSUE_TEMPLATE/🆕-feature-request.md
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 distilabel-1.0.2/.github/ISSUE_TEMPLATE/🐛-bug-report.md
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 distilabel-1.0.2/.github/ISSUE_TEMPLATE/📚-documentation-update.md
--rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 distilabel-1.0.2/.github/workflows/docs.yml
--rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 distilabel-1.0.2/.github/workflows/release.yml
--rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 distilabel-1.0.2/.github/workflows/test.yml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/CNAME
--rw-r--r--   0        0        0     3503 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/index.md
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/overview.md
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/api/cli.md
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/api/llms/anthropic.md
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/api/llms/anyscale.md
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/api/llms/azure.md
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/api/llms/huggingface.md
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/api/llms/index.md
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/api/llms/litellm.md
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/api/llms/llamacpp.md
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/api/llms/mistral.md
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/api/llms/ollama.md
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/api/llms/openai.md
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/api/llms/together.md
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/api/llms/vertexai.md
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/api/llms/vllm.md
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/api/pipeline/pipeline.md
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/api/steps/argilla.md
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/api/steps/decorator.md
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/api/steps/extra.md
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/api/steps/index.md
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/api/steps/generator_steps/generator_steps.md
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/api/steps/global_steps/global_steps.md
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/api/steps/tasks/embeddings.md
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/api/steps/tasks/preference_tasks.md
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/api/steps/tasks/text_generation.md
--rw-r--r--   0        0        0    16279 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/assets/distilabel-badge-dark.png
--rw-r--r--   0        0        0    15551 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/assets/distilabel-badge-light.png
--rw-r--r--   0        0        0    11187 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/assets/distilabel-black.png
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/assets/distilabel-icon.svg
--rw-r--r--   0        0        0     7678 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/assets/distilabel-white.png
--rw-r--r--   0        0        0     3431 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/assets/logo.svg
--rw-r--r--   0        0        0    47284 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/assets/images/distilabel-diagram-dark.svg
--rw-r--r--   0        0        0    47244 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/assets/images/distilabel-diagram.svg
--rw-r--r--   0        0        0   301103 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/assets/images/sections/caching/caching_pipe_1.png
--rw-r--r--   0        0        0   329256 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/assets/images/sections/caching/caching_pipe_2.png
--rw-r--r--   0        0        0   129190 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/assets/images/sections/caching/caching_pipe_3.png
--rw-r--r--   0        0        0    24695 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/assets/images/sections/caching/caching_pipe_4.png
--rw-r--r--   0        0        0   368245 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/assets/images/sections/cli/cli_pipe.png
--rw-r--r--   0        0        0  1290074 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/assets/images/sections/learn/steps/argilla/preference.png
--rw-r--r--   0        0        0  1014081 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/assets/images/sections/learn/steps/argilla/text_generation.png
--rw-r--r--   0        0        0   173971 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/assets/tutorials-assets/instrucion_dataset_notus_ui.png
--rw-r--r--   0        0        0   356586 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/assets/tutorials-assets/preference_dataset_notus_ui.png
--rw-r--r--   0        0        0    19151 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/assets/tutorials-assets/deita/datasets.png
--rw-r--r--   0        0        0    96338 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/assets/tutorials-assets/deita/diversity.png
--rw-r--r--   0        0        0   191403 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/assets/tutorials-assets/deita/overview.png
--rw-r--r--   0        0        0    94813 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/assets/tutorials-assets/deita/results.png
--rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/scripts/gen_ref_pages.py
--rw-r--r--   0        0        0     4117 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/sections/learn/caching.md
--rw-r--r--   0        0        0     7963 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/sections/learn/cli.md
--rw-r--r--   0        0        0     2921 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/sections/learn/distiset.md
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/sections/learn/index.md
--rw-r--r--   0        0        0     7708 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/sections/learn/llms/index.md
--rw-r--r--   0        0        0    14701 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/sections/learn/pipelines/index.md
--rw-r--r--   0        0        0     7914 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/sections/learn/steps/argilla.md
--rw-r--r--   0        0        0     8669 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/sections/learn/steps/general_steps.md
--rw-r--r--   0        0        0     6941 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/sections/learn/steps/generator_steps.md
--rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/sections/learn/steps/global_steps.md
--rw-r--r--   0        0        0     8491 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/sections/learn/steps/index.md
--rw-r--r--   0        0        0     7803 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/sections/learn/tasks/feedback_tasks.md
--rw-r--r--   0        0        0    10710 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/sections/learn/tasks/index.md
--rw-r--r--   0        0        0     5887 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/sections/learn/tasks/special_tasks.md
--rw-r--r--   0        0        0    16125 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/sections/learn/tasks/text_generation.md
--rw-r--r--   0        0        0    21822 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/sections/papers/deita.md
--rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/sections/papers/index.md
--rw-r--r--   0        0        0     5921 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/sections/papers/instruction_backtranslation.md
--rw-r--r--   0        0        0     6730 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/sections/papers/ultrafeedback.md
--rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 distilabel-1.0.2/docs/stylesheets/extra.css
--rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/__init__.py
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/__main__.py
--rw-r--r--   0        0        0     9461 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/distiset.py
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/cli/__init__.py
--rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/cli/app.py
--rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/cli/pipeline/__init__.py
--rw-r--r--   0        0        0     3277 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/cli/pipeline/app.py
--rw-r--r--   0        0        0     8197 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/cli/pipeline/utils.py
--rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/llms/__init__.py
--rw-r--r--   0        0        0     9236 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/llms/anthropic.py
--rw-r--r--   0        0        0     2436 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/llms/anyscale.py
--rw-r--r--   0        0        0     4125 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/llms/azure.py
--rw-r--r--   0        0        0    10588 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/llms/base.py
--rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/llms/chat_templates.py
--rw-r--r--   0        0        0     9147 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/llms/cohere.py
--rw-r--r--   0        0        0     8176 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/llms/litellm.py
--rw-r--r--   0        0        0     5275 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/llms/llamacpp.py
--rw-r--r--   0        0        0     7427 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/llms/mistral.py
--rw-r--r--   0        0        0     8783 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/llms/mixins.py
--rw-r--r--   0        0        0     4956 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/llms/ollama.py
--rw-r--r--   0        0        0     6609 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/llms/openai.py
--rw-r--r--   0        0        0     2393 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/llms/together.py
--rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/llms/typing.py
--rw-r--r--   0        0        0     6905 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/llms/vertexai.py
--rw-r--r--   0        0        0     7200 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/llms/vllm.py
--rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/llms/huggingface/__init__.py
--rw-r--r--   0        0        0    15916 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/llms/huggingface/inference_endpoints.py
--rw-r--r--   0        0        0     9033 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/llms/huggingface/transformers.py
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/mixins/__init__.py
--rw-r--r--   0        0        0     7026 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/mixins/runtime_parameters.py
--rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/pipeline/__init__.py
--rw-r--r--   0        0        0    18795 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/pipeline/_dag.py
--rw-r--r--   0        0        0    37076 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/pipeline/base.py
--rw-r--r--   0        0        0    32476 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/pipeline/local.py
--rw-r--r--   0        0        0     1930 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/pipeline/utils.py
--rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/steps/__init__.py
--rw-r--r--   0        0        0    19355 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/steps/base.py
--rw-r--r--   0        0        0     2776 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/steps/combine.py
--rw-r--r--   0        0        0     1917 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/steps/conversation.py
--rw-r--r--   0        0        0     7016 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/steps/decorator.py
--rw-r--r--   0        0        0     9152 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/steps/deita.py
--rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/steps/expand.py
--rw-r--r--   0        0        0     2518 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/steps/keep.py
--rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/steps/typing.py
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/steps/argilla/__init__.py
--rw-r--r--   0        0        0     5690 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/steps/argilla/base.py
--rw-r--r--   0        0        0    10934 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/steps/argilla/preference.py
--rw-r--r--   0        0        0     6705 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/steps/argilla/text_generation.py
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/steps/generators/__init__.py
--rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/steps/generators/data.py
--rw-r--r--   0        0        0     7256 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/steps/generators/huggingface.py
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/steps/globals/__init__.py
--rw-r--r--   0        0        0     4322 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/steps/globals/huggingface.py
--rw-r--r--   0        0        0     2045 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/steps/tasks/__init__.py
--rw-r--r--   0        0        0     6966 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/steps/tasks/base.py
--rw-r--r--   0        0        0     3174 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/steps/tasks/complexity_scorer.py
--rw-r--r--   0        0        0     3780 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/steps/tasks/generate_embeddings.py
--rw-r--r--   0        0        0     3821 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/steps/tasks/instruction_backtranslation.py
--rw-r--r--   0        0        0     4770 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/steps/tasks/pair_rm.py
--rw-r--r--   0        0        0     4523 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/steps/tasks/quality_scorer.py
--rw-r--r--   0        0        0     4747 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/steps/tasks/self_instruct.py
--rw-r--r--   0        0        0     2670 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/steps/tasks/text_generation.py
--rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/steps/tasks/typing.py
--rw-r--r--   0        0        0     9452 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/steps/tasks/ultrafeedback.py
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/steps/tasks/evol_instruct/__init__.py
--rw-r--r--   0        0        0    12081 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/steps/tasks/evol_instruct/base.py
--rw-r--r--   0        0        0    10714 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/steps/tasks/evol_instruct/english_nouns.txt
--rw-r--r--   0        0        0    12857 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/steps/tasks/evol_instruct/generator.py
--rw-r--r--   0        0        0     3671 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/steps/tasks/evol_instruct/utils.py
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/steps/tasks/evol_instruct/evol_complexity/__init__.py
--rw-r--r--   0        0        0     2834 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/steps/tasks/evol_instruct/evol_complexity/base.py
--rw-r--r--   0        0        0     2880 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/steps/tasks/evol_instruct/evol_complexity/generator.py
--rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/steps/tasks/evol_instruct/evol_complexity/utils.py
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/steps/tasks/evol_quality/__init__.py
--rw-r--r--   0        0        0     9098 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/steps/tasks/evol_quality/base.py
--rw-r--r--   0        0        0     2096 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/steps/tasks/evol_quality/utils.py
--rw-r--r--   0        0        0     2383 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/steps/tasks/templates/instruction-backtranslation.jinja2
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/steps/tasks/templates/self-instruct.jinja2
--rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/steps/tasks/templates/ultrafeedback/helpfulness.jinja2
--rw-r--r--   0        0        0     2045 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/steps/tasks/templates/ultrafeedback/honesty.jinja2
--rw-r--r--   0        0        0     1270 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/steps/tasks/templates/ultrafeedback/instruction-following.jinja2
--rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/steps/tasks/templates/ultrafeedback/overall-rating.jinja2
--rw-r--r--   0        0        0     2004 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/steps/tasks/templates/ultrafeedback/truthfulness.jinja2
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/utils/__init__.py
--rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/utils/chat.py
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/utils/dicts.py
--rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/utils/docstring.py
--rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/utils/files.py
--rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/utils/itertools.py
--rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/utils/lists.py
--rw-r--r--   0        0        0     2585 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/utils/logging.py
--rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/utils/notebook.py
--rw-r--r--   0        0        0    10480 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/utils/serialization.py
--rw-r--r--   0        0        0     1361 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/utils/typing_.py
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/utils/card/__init__.py
--rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/utils/card/dataset_card.py
--rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 distilabel-1.0.2/src/distilabel/utils/card/distilabel_template.md
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/__init__.py
--rw-r--r--   0        0        0     2901 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/integration/test_pipe_llms.py
--rw-r--r--   0        0        0     6603 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/integration/test_pipe_simple.py
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/__init__.py
--rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/test_distiset.py
--rw-r--r--   0        0        0     1930 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/test_imports.py
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/cli/__init__.py
--rw-r--r--   0        0        0     8444 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/cli/test_pipeline.yaml
--rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/cli/utils.py
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/cli/pipeline/__init__.py
--rw-r--r--   0        0        0     4559 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/cli/pipeline/test_app.py
--rw-r--r--   0        0        0     2574 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/cli/pipeline/utils.py
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/llms/__init__.py
--rw-r--r--   0        0        0     3194 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/llms/test_anthropic.py
--rw-r--r--   0        0        0     2060 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/llms/test_anyscale.py
--rw-r--r--   0        0        0     2795 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/llms/test_azure.py
--rw-r--r--   0        0        0     3711 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/llms/test_cohere.py
--rw-r--r--   0        0        0     3000 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/llms/test_litellm.py
--rw-r--r--   0        0        0     1896 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/llms/test_llamacpp.py
--rw-r--r--   0        0        0     3415 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/llms/test_mistral.py
--rw-r--r--   0        0        0     5748 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/llms/test_mixins.py
--rw-r--r--   0        0        0     2894 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/llms/test_ollama.py
--rw-r--r--   0        0        0     3671 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/llms/test_openai.py
--rw-r--r--   0        0        0     2050 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/llms/test_together.py
--rw-r--r--   0        0        0     4472 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/llms/test_vertexai.py
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/llms/huggingface/__init__.py
--rw-r--r--   0        0        0     6669 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/llms/huggingface/test_inference_endpoints.py
--rw-r--r--   0        0        0     2292 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/llms/huggingface/test_transformers.py
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/mixins/__init__.py
--rw-r--r--   0        0        0     3562 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/mixins/test_runtime_parameters.py
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/pipeline/__init__.py
--rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/pipeline/conftest.py
--rw-r--r--   0        0        0    44539 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/pipeline/test_base.py
--rw-r--r--   0        0        0    18140 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/pipeline/test_dag.py
--rw-r--r--   0        0        0     4510 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/pipeline/test_local.py
--rw-r--r--   0        0        0     2270 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/pipeline/utils.py
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/steps/__init__.py
--rw-r--r--   0        0        0     9554 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/steps/test_base.py
--rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/steps/test_combine.py
--rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/steps/test_conversation.py
--rw-r--r--   0        0        0     4545 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/steps/test_decorator.py
--rw-r--r--   0        0        0     2234 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/steps/test_deita.py
--rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/steps/test_expand.py
--rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/steps/test_keep.py
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/steps/argilla/__init__.py
--rw-r--r--   0        0        0     5814 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/steps/argilla/test_base.py
--rw-r--r--   0        0        0     5725 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/steps/argilla/test_preference.py
--rw-r--r--   0        0        0     4417 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/steps/argilla/test_text_generation.py
--rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/steps/generators/test_data.py
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/steps/tasks/__init__.py
--rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/steps/tasks/conftest.py
--rw-r--r--   0        0        0     8172 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/steps/tasks/test_base.py
--rw-r--r--   0        0        0     2654 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/steps/tasks/test_complexity_scorer.py
--rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/steps/tasks/test_generate_embeddings.py
--rw-r--r--   0        0        0     5289 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/steps/tasks/test_instruction_backtranslation.py
--rw-r--r--   0        0        0     2444 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/steps/tasks/test_pair_rm.py
--rw-r--r--   0        0        0     2996 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/steps/tasks/test_quality_scorer.py
--rw-r--r--   0        0        0     2384 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/steps/tasks/test_self_instruct.py
--rw-r--r--   0        0        0     2186 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/steps/tasks/test_text_generation.py
--rw-r--r--   0        0        0     2933 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/steps/tasks/test_ultrafeedback.py
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/steps/tasks/utils.py
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/steps/tasks/evol_instruct/__init__.py
--rw-r--r--   0        0        0    11232 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/steps/tasks/evol_instruct/test_base.py
--rw-r--r--   0        0        0    11530 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/steps/tasks/evol_instruct/test_generator.py
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/steps/tasks/evol_instruct/evol_complexity.py/__init__.py
--rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/steps/tasks/evol_instruct/evol_complexity.py/test_base.py
--rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/steps/tasks/evol_instruct/evol_complexity.py/test_generator.py
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/steps/tasks/evol_quality/__init__.py
--rw-r--r--   0        0        0     5168 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/steps/tasks/evol_quality/test_base.py
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/utils/__init__.py
--rw-r--r--   0        0        0     2171 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/utils/test_chat.py
--rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/utils/test_docstring.py
--rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/utils/test_lists.py
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 distilabel-1.0.2/tests/unit/utils/test_typing.py
--rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 distilabel-1.0.2/.gitignore
--rw-r--r--   0        0        0    11355 2020-02-02 00:00:00.000000 distilabel-1.0.2/LICENSE
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 distilabel-1.0.2/LICENSE_HEADER
--rw-r--r--   0        0        0     8989 2020-02-02 00:00:00.000000 distilabel-1.0.2/README.md
--rw-r--r--   0        0        0     2536 2020-02-02 00:00:00.000000 distilabel-1.0.2/pyproject.toml
--rw-r--r--   0        0        0    12184 2020-02-02 00:00:00.000000 distilabel-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 distilabel-1.0.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 distilabel-1.0.3/Makefile
+-rw-r--r--   0        0        0     5115 2020-02-02 00:00:00.000000 distilabel-1.0.3/mkdocs.yml
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 distilabel-1.0.3/.github/ISSUE_TEMPLATE/blank-issue-template.md
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 distilabel-1.0.3/.github/ISSUE_TEMPLATE/🆕-feature-request.md
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 distilabel-1.0.3/.github/ISSUE_TEMPLATE/🐛-bug-report.md
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 distilabel-1.0.3/.github/ISSUE_TEMPLATE/📚-documentation-update.md
+-rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 distilabel-1.0.3/.github/workflows/docs.yml
+-rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 distilabel-1.0.3/.github/workflows/release.yml
+-rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 distilabel-1.0.3/.github/workflows/test.yml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/CNAME
+-rw-r--r--   0        0        0     3503 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/index.md
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/overview.md
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/api/cli.md
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/api/llms/anthropic.md
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/api/llms/anyscale.md
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/api/llms/azure.md
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/api/llms/huggingface.md
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/api/llms/index.md
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/api/llms/litellm.md
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/api/llms/llamacpp.md
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/api/llms/mistral.md
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/api/llms/ollama.md
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/api/llms/openai.md
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/api/llms/together.md
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/api/llms/vertexai.md
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/api/llms/vllm.md
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/api/pipeline/pipeline.md
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/api/steps/argilla.md
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/api/steps/decorator.md
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/api/steps/extra.md
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/api/steps/index.md
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/api/steps/generator_steps/generator_steps.md
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/api/steps/global_steps/global_steps.md
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/api/steps/tasks/embeddings.md
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/api/steps/tasks/preference_tasks.md
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/api/steps/tasks/text_generation.md
+-rw-r--r--   0        0        0    16279 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/assets/distilabel-badge-dark.png
+-rw-r--r--   0        0        0    15551 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/assets/distilabel-badge-light.png
+-rw-r--r--   0        0        0    11187 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/assets/distilabel-black.png
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/assets/distilabel-icon.svg
+-rw-r--r--   0        0        0     7678 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/assets/distilabel-white.png
+-rw-r--r--   0        0        0     3431 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/assets/logo.svg
+-rw-r--r--   0        0        0    47284 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/assets/images/distilabel-diagram-dark.svg
+-rw-r--r--   0        0        0    47244 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/assets/images/distilabel-diagram.svg
+-rw-r--r--   0        0        0   301103 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/assets/images/sections/caching/caching_pipe_1.png
+-rw-r--r--   0        0        0   329256 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/assets/images/sections/caching/caching_pipe_2.png
+-rw-r--r--   0        0        0   129190 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/assets/images/sections/caching/caching_pipe_3.png
+-rw-r--r--   0        0        0    24695 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/assets/images/sections/caching/caching_pipe_4.png
+-rw-r--r--   0        0        0   368245 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/assets/images/sections/cli/cli_pipe.png
+-rw-r--r--   0        0        0  1290074 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/assets/images/sections/learn/steps/argilla/preference.png
+-rw-r--r--   0        0        0  1014081 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/assets/images/sections/learn/steps/argilla/text_generation.png
+-rw-r--r--   0        0        0   173971 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/assets/tutorials-assets/instrucion_dataset_notus_ui.png
+-rw-r--r--   0        0        0   356586 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/assets/tutorials-assets/preference_dataset_notus_ui.png
+-rw-r--r--   0        0        0    19151 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/assets/tutorials-assets/deita/datasets.png
+-rw-r--r--   0        0        0    96338 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/assets/tutorials-assets/deita/diversity.png
+-rw-r--r--   0        0        0   191403 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/assets/tutorials-assets/deita/overview.png
+-rw-r--r--   0        0        0    94813 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/assets/tutorials-assets/deita/results.png
+-rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/scripts/gen_ref_pages.py
+-rw-r--r--   0        0        0     4117 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/sections/learn/caching.md
+-rw-r--r--   0        0        0     7963 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/sections/learn/cli.md
+-rw-r--r--   0        0        0     2921 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/sections/learn/distiset.md
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/sections/learn/index.md
+-rw-r--r--   0        0        0     7708 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/sections/learn/llms/index.md
+-rw-r--r--   0        0        0    14701 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/sections/learn/pipelines/index.md
+-rw-r--r--   0        0        0     7914 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/sections/learn/steps/argilla.md
+-rw-r--r--   0        0        0     8669 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/sections/learn/steps/general_steps.md
+-rw-r--r--   0        0        0     6941 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/sections/learn/steps/generator_steps.md
+-rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/sections/learn/steps/global_steps.md
+-rw-r--r--   0        0        0     8491 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/sections/learn/steps/index.md
+-rw-r--r--   0        0        0     7803 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/sections/learn/tasks/feedback_tasks.md
+-rw-r--r--   0        0        0    10710 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/sections/learn/tasks/index.md
+-rw-r--r--   0        0        0     5887 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/sections/learn/tasks/special_tasks.md
+-rw-r--r--   0        0        0    16125 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/sections/learn/tasks/text_generation.md
+-rw-r--r--   0        0        0    21822 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/sections/papers/deita.md
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/sections/papers/index.md
+-rw-r--r--   0        0        0     5921 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/sections/papers/instruction_backtranslation.md
+-rw-r--r--   0        0        0     6730 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/sections/papers/ultrafeedback.md
+-rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/stylesheets/extra.css
+-rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/__init__.py
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/__main__.py
+-rw-r--r--   0        0        0     9461 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/distiset.py
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/cli/__init__.py
+-rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/cli/app.py
+-rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/cli/pipeline/__init__.py
+-rw-r--r--   0        0        0     3277 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/cli/pipeline/app.py
+-rw-r--r--   0        0        0     8197 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/cli/pipeline/utils.py
+-rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/llms/__init__.py
+-rw-r--r--   0        0        0     9236 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/llms/anthropic.py
+-rw-r--r--   0        0        0     2436 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/llms/anyscale.py
+-rw-r--r--   0        0        0     4125 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/llms/azure.py
+-rw-r--r--   0        0        0    10588 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/llms/base.py
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/llms/chat_templates.py
+-rw-r--r--   0        0        0     9147 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/llms/cohere.py
+-rw-r--r--   0        0        0     8176 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/llms/litellm.py
+-rw-r--r--   0        0        0     5275 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/llms/llamacpp.py
+-rw-r--r--   0        0        0     7427 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/llms/mistral.py
+-rw-r--r--   0        0        0     8783 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/llms/mixins.py
+-rw-r--r--   0        0        0     4956 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/llms/ollama.py
+-rw-r--r--   0        0        0     6861 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/llms/openai.py
+-rw-r--r--   0        0        0     2393 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/llms/together.py
+-rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/llms/typing.py
+-rw-r--r--   0        0        0     6905 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/llms/vertexai.py
+-rw-r--r--   0        0        0     7201 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/llms/vllm.py
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/llms/huggingface/__init__.py
+-rw-r--r--   0        0        0    16868 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/llms/huggingface/inference_endpoints.py
+-rw-r--r--   0        0        0     9033 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/llms/huggingface/transformers.py
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/mixins/__init__.py
+-rw-r--r--   0        0        0     7026 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/mixins/runtime_parameters.py
+-rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/pipeline/__init__.py
+-rw-r--r--   0        0        0    18795 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/pipeline/_dag.py
+-rw-r--r--   0        0        0    37076 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/pipeline/base.py
+-rw-r--r--   0        0        0    32476 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/pipeline/local.py
+-rw-r--r--   0        0        0     1930 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/pipeline/utils.py
+-rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/steps/__init__.py
+-rw-r--r--   0        0        0    19355 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/steps/base.py
+-rw-r--r--   0        0        0     2776 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/steps/combine.py
+-rw-r--r--   0        0        0     1917 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/steps/conversation.py
+-rw-r--r--   0        0        0     7016 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/steps/decorator.py
+-rw-r--r--   0        0        0     9152 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/steps/deita.py
+-rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/steps/expand.py
+-rw-r--r--   0        0        0     2518 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/steps/keep.py
+-rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/steps/typing.py
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/steps/argilla/__init__.py
+-rw-r--r--   0        0        0     5690 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/steps/argilla/base.py
+-rw-r--r--   0        0        0    10934 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/steps/argilla/preference.py
+-rw-r--r--   0        0        0     6705 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/steps/argilla/text_generation.py
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/steps/generators/__init__.py
+-rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/steps/generators/data.py
+-rw-r--r--   0        0        0     7256 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/steps/generators/huggingface.py
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/steps/globals/__init__.py
+-rw-r--r--   0        0        0     4322 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/steps/globals/huggingface.py
+-rw-r--r--   0        0        0     2045 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/steps/tasks/__init__.py
+-rw-r--r--   0        0        0     6966 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/steps/tasks/base.py
+-rw-r--r--   0        0        0     3174 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/steps/tasks/complexity_scorer.py
+-rw-r--r--   0        0        0     3780 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/steps/tasks/generate_embeddings.py
+-rw-r--r--   0        0        0     3821 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/steps/tasks/instruction_backtranslation.py
+-rw-r--r--   0        0        0     4770 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/steps/tasks/pair_rm.py
+-rw-r--r--   0        0        0     4523 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/steps/tasks/quality_scorer.py
+-rw-r--r--   0        0        0     4747 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/steps/tasks/self_instruct.py
+-rw-r--r--   0        0        0     2670 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/steps/tasks/text_generation.py
+-rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/steps/tasks/typing.py
+-rw-r--r--   0        0        0     9452 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/steps/tasks/ultrafeedback.py
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/steps/tasks/evol_instruct/__init__.py
+-rw-r--r--   0        0        0    12081 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/steps/tasks/evol_instruct/base.py
+-rw-r--r--   0        0        0    10714 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/steps/tasks/evol_instruct/english_nouns.txt
+-rw-r--r--   0        0        0    12857 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/steps/tasks/evol_instruct/generator.py
+-rw-r--r--   0        0        0     3671 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/steps/tasks/evol_instruct/utils.py
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/steps/tasks/evol_instruct/evol_complexity/__init__.py
+-rw-r--r--   0        0        0     2834 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/steps/tasks/evol_instruct/evol_complexity/base.py
+-rw-r--r--   0        0        0     2880 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/steps/tasks/evol_instruct/evol_complexity/generator.py
+-rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/steps/tasks/evol_instruct/evol_complexity/utils.py
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/steps/tasks/evol_quality/__init__.py
+-rw-r--r--   0        0        0     9098 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/steps/tasks/evol_quality/base.py
+-rw-r--r--   0        0        0     2096 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/steps/tasks/evol_quality/utils.py
+-rw-r--r--   0        0        0     2383 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/steps/tasks/templates/instruction-backtranslation.jinja2
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/steps/tasks/templates/self-instruct.jinja2
+-rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/steps/tasks/templates/ultrafeedback/helpfulness.jinja2
+-rw-r--r--   0        0        0     2045 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/steps/tasks/templates/ultrafeedback/honesty.jinja2
+-rw-r--r--   0        0        0     1270 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/steps/tasks/templates/ultrafeedback/instruction-following.jinja2
+-rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/steps/tasks/templates/ultrafeedback/overall-rating.jinja2
+-rw-r--r--   0        0        0     2004 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/steps/tasks/templates/ultrafeedback/truthfulness.jinja2
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/utils/__init__.py
+-rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/utils/chat.py
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/utils/dicts.py
+-rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/utils/docstring.py
+-rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/utils/files.py
+-rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/utils/itertools.py
+-rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/utils/lists.py
+-rw-r--r--   0        0        0     2585 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/utils/logging.py
+-rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/utils/notebook.py
+-rw-r--r--   0        0        0    10480 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/utils/serialization.py
+-rw-r--r--   0        0        0     1361 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/utils/typing_.py
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/utils/card/__init__.py
+-rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/utils/card/dataset_card.py
+-rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/utils/card/distilabel_template.md
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/__init__.py
+-rw-r--r--   0        0        0     2901 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/integration/test_pipe_llms.py
+-rw-r--r--   0        0        0     6603 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/integration/test_pipe_simple.py
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/__init__.py
+-rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/test_distiset.py
+-rw-r--r--   0        0        0     1930 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/test_imports.py
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/cli/__init__.py
+-rw-r--r--   0        0        0     8444 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/cli/test_pipeline.yaml
+-rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/cli/utils.py
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/cli/pipeline/__init__.py
+-rw-r--r--   0        0        0     4559 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/cli/pipeline/test_app.py
+-rw-r--r--   0        0        0     2574 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/cli/pipeline/utils.py
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/llms/__init__.py
+-rw-r--r--   0        0        0     3194 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/llms/test_anthropic.py
+-rw-r--r--   0        0        0     2060 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/llms/test_anyscale.py
+-rw-r--r--   0        0        0     2795 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/llms/test_azure.py
+-rw-r--r--   0        0        0     3711 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/llms/test_cohere.py
+-rw-r--r--   0        0        0     3000 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/llms/test_litellm.py
+-rw-r--r--   0        0        0     1896 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/llms/test_llamacpp.py
+-rw-r--r--   0        0        0     3415 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/llms/test_mistral.py
+-rw-r--r--   0        0        0     5748 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/llms/test_mixins.py
+-rw-r--r--   0        0        0     2894 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/llms/test_ollama.py
+-rw-r--r--   0        0        0     3671 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/llms/test_openai.py
+-rw-r--r--   0        0        0     2050 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/llms/test_together.py
+-rw-r--r--   0        0        0     4472 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/llms/test_vertexai.py
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/llms/huggingface/__init__.py
+-rw-r--r--   0        0        0     6669 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/llms/huggingface/test_inference_endpoints.py
+-rw-r--r--   0        0        0     2292 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/llms/huggingface/test_transformers.py
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/mixins/__init__.py
+-rw-r--r--   0        0        0     3562 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/mixins/test_runtime_parameters.py
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/pipeline/__init__.py
+-rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/pipeline/conftest.py
+-rw-r--r--   0        0        0    44539 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/pipeline/test_base.py
+-rw-r--r--   0        0        0    18140 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/pipeline/test_dag.py
+-rw-r--r--   0        0        0     4510 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/pipeline/test_local.py
+-rw-r--r--   0        0        0     2270 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/pipeline/utils.py
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/steps/__init__.py
+-rw-r--r--   0        0        0     9554 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/steps/test_base.py
+-rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/steps/test_combine.py
+-rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/steps/test_conversation.py
+-rw-r--r--   0        0        0     4545 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/steps/test_decorator.py
+-rw-r--r--   0        0        0     2234 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/steps/test_deita.py
+-rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/steps/test_expand.py
+-rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/steps/test_keep.py
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/steps/argilla/__init__.py
+-rw-r--r--   0        0        0     5814 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/steps/argilla/test_base.py
+-rw-r--r--   0        0        0     5725 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/steps/argilla/test_preference.py
+-rw-r--r--   0        0        0     4417 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/steps/argilla/test_text_generation.py
+-rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/steps/generators/test_data.py
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/steps/tasks/__init__.py
+-rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/steps/tasks/conftest.py
+-rw-r--r--   0        0        0     8172 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/steps/tasks/test_base.py
+-rw-r--r--   0        0        0     2654 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/steps/tasks/test_complexity_scorer.py
+-rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/steps/tasks/test_generate_embeddings.py
+-rw-r--r--   0        0        0     5289 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/steps/tasks/test_instruction_backtranslation.py
+-rw-r--r--   0        0        0     2444 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/steps/tasks/test_pair_rm.py
+-rw-r--r--   0        0        0     2996 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/steps/tasks/test_quality_scorer.py
+-rw-r--r--   0        0        0     2384 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/steps/tasks/test_self_instruct.py
+-rw-r--r--   0        0        0     2186 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/steps/tasks/test_text_generation.py
+-rw-r--r--   0        0        0     2933 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/steps/tasks/test_ultrafeedback.py
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/steps/tasks/utils.py
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/steps/tasks/evol_instruct/__init__.py
+-rw-r--r--   0        0        0    11232 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/steps/tasks/evol_instruct/test_base.py
+-rw-r--r--   0        0        0    11530 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/steps/tasks/evol_instruct/test_generator.py
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/steps/tasks/evol_instruct/evol_complexity.py/__init__.py
+-rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/steps/tasks/evol_instruct/evol_complexity.py/test_base.py
+-rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/steps/tasks/evol_instruct/evol_complexity.py/test_generator.py
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/steps/tasks/evol_quality/__init__.py
+-rw-r--r--   0        0        0     5168 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/steps/tasks/evol_quality/test_base.py
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/utils/__init__.py
+-rw-r--r--   0        0        0     2171 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/utils/test_chat.py
+-rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/utils/test_docstring.py
+-rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/utils/test_lists.py
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/utils/test_typing.py
+-rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 distilabel-1.0.3/.gitignore
+-rw-r--r--   0        0        0    11355 2020-02-02 00:00:00.000000 distilabel-1.0.3/LICENSE
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 distilabel-1.0.3/LICENSE_HEADER
+-rw-r--r--   0        0        0     8989 2020-02-02 00:00:00.000000 distilabel-1.0.3/README.md
+-rw-r--r--   0        0        0     2536 2020-02-02 00:00:00.000000 distilabel-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0    12184 2020-02-02 00:00:00.000000 distilabel-1.0.3/PKG-INFO
```

### Comparing `distilabel-1.0.2/.pre-commit-config.yaml` & `distilabel-1.0.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/mkdocs.yml` & `distilabel-1.0.3/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/.github/ISSUE_TEMPLATE/🆕-feature-request.md` & `distilabel-1.0.3/.github/ISSUE_TEMPLATE/🆕-feature-request.md`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/.github/ISSUE_TEMPLATE/🐛-bug-report.md` & `distilabel-1.0.3/.github/ISSUE_TEMPLATE/🐛-bug-report.md`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/.github/ISSUE_TEMPLATE/📚-documentation-update.md` & `distilabel-1.0.3/.github/ISSUE_TEMPLATE/📚-documentation-update.md`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/.github/workflows/docs.yml` & `distilabel-1.0.3/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/.github/workflows/release.yml` & `distilabel-1.0.3/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/.github/workflows/test.yml` & `distilabel-1.0.3/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/docs/index.md` & `distilabel-1.0.3/docs/index.md`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/docs/api/steps/tasks/text_generation.md` & `distilabel-1.0.3/docs/api/steps/tasks/text_generation.md`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/docs/assets/distilabel-badge-dark.png` & `distilabel-1.0.3/docs/assets/distilabel-badge-dark.png`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/docs/assets/distilabel-badge-light.png` & `distilabel-1.0.3/docs/assets/distilabel-badge-light.png`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/docs/assets/distilabel-black.png` & `distilabel-1.0.3/docs/assets/distilabel-black.png`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/docs/assets/distilabel-icon.svg` & `distilabel-1.0.3/docs/assets/distilabel-icon.svg`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/docs/assets/distilabel-white.png` & `distilabel-1.0.3/docs/assets/distilabel-white.png`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/docs/assets/logo.svg` & `distilabel-1.0.3/docs/assets/logo.svg`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/docs/assets/images/distilabel-diagram-dark.svg` & `distilabel-1.0.3/docs/assets/images/distilabel-diagram-dark.svg`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/docs/assets/images/distilabel-diagram.svg` & `distilabel-1.0.3/docs/assets/images/distilabel-diagram.svg`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/docs/assets/images/sections/caching/caching_pipe_1.png` & `distilabel-1.0.3/docs/assets/images/sections/caching/caching_pipe_1.png`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/docs/assets/images/sections/caching/caching_pipe_2.png` & `distilabel-1.0.3/docs/assets/images/sections/caching/caching_pipe_2.png`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/docs/assets/images/sections/caching/caching_pipe_3.png` & `distilabel-1.0.3/docs/assets/images/sections/caching/caching_pipe_3.png`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/docs/assets/images/sections/caching/caching_pipe_4.png` & `distilabel-1.0.3/docs/assets/images/sections/caching/caching_pipe_4.png`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/docs/assets/images/sections/cli/cli_pipe.png` & `distilabel-1.0.3/docs/assets/images/sections/cli/cli_pipe.png`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/docs/assets/images/sections/learn/steps/argilla/preference.png` & `distilabel-1.0.3/docs/assets/images/sections/learn/steps/argilla/preference.png`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/docs/assets/images/sections/learn/steps/argilla/text_generation.png` & `distilabel-1.0.3/docs/assets/images/sections/learn/steps/argilla/text_generation.png`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/docs/assets/tutorials-assets/instrucion_dataset_notus_ui.png` & `distilabel-1.0.3/docs/assets/tutorials-assets/instrucion_dataset_notus_ui.png`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/docs/assets/tutorials-assets/preference_dataset_notus_ui.png` & `distilabel-1.0.3/docs/assets/tutorials-assets/preference_dataset_notus_ui.png`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/docs/assets/tutorials-assets/deita/datasets.png` & `distilabel-1.0.3/docs/assets/tutorials-assets/deita/datasets.png`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/docs/assets/tutorials-assets/deita/diversity.png` & `distilabel-1.0.3/docs/assets/tutorials-assets/deita/diversity.png`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/docs/assets/tutorials-assets/deita/overview.png` & `distilabel-1.0.3/docs/assets/tutorials-assets/deita/overview.png`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/docs/assets/tutorials-assets/deita/results.png` & `distilabel-1.0.3/docs/assets/tutorials-assets/deita/results.png`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/docs/scripts/gen_ref_pages.py` & `distilabel-1.0.3/docs/scripts/gen_ref_pages.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/docs/sections/learn/caching.md` & `distilabel-1.0.3/docs/sections/learn/caching.md`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/docs/sections/learn/cli.md` & `distilabel-1.0.3/docs/sections/learn/cli.md`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/docs/sections/learn/distiset.md` & `distilabel-1.0.3/docs/sections/learn/distiset.md`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/docs/sections/learn/llms/index.md` & `distilabel-1.0.3/docs/sections/learn/llms/index.md`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/docs/sections/learn/pipelines/index.md` & `distilabel-1.0.3/docs/sections/learn/pipelines/index.md`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/docs/sections/learn/steps/argilla.md` & `distilabel-1.0.3/docs/sections/learn/steps/argilla.md`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/docs/sections/learn/steps/general_steps.md` & `distilabel-1.0.3/docs/sections/learn/steps/general_steps.md`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/docs/sections/learn/steps/generator_steps.md` & `distilabel-1.0.3/docs/sections/learn/steps/generator_steps.md`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/docs/sections/learn/steps/global_steps.md` & `distilabel-1.0.3/docs/sections/learn/steps/global_steps.md`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/docs/sections/learn/steps/index.md` & `distilabel-1.0.3/docs/sections/learn/steps/index.md`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/docs/sections/learn/tasks/feedback_tasks.md` & `distilabel-1.0.3/docs/sections/learn/tasks/feedback_tasks.md`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/docs/sections/learn/tasks/index.md` & `distilabel-1.0.3/docs/sections/learn/tasks/index.md`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/docs/sections/learn/tasks/special_tasks.md` & `distilabel-1.0.3/docs/sections/learn/tasks/special_tasks.md`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/docs/sections/learn/tasks/text_generation.md` & `distilabel-1.0.3/docs/sections/learn/tasks/text_generation.md`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/docs/sections/papers/deita.md` & `distilabel-1.0.3/docs/sections/papers/deita.md`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/docs/sections/papers/instruction_backtranslation.md` & `distilabel-1.0.3/docs/sections/papers/instruction_backtranslation.md`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/docs/sections/papers/ultrafeedback.md` & `distilabel-1.0.3/docs/sections/papers/ultrafeedback.md`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/src/distilabel/__init__.py` & `distilabel-1.0.3/src/distilabel/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,10 +10,10 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from rich import traceback as rich_traceback
 
-__version__ = "1.0.2"
+__version__ = "1.0.3"
 
 rich_traceback.install(show_locals=True)
```

### Comparing `distilabel-1.0.2/src/distilabel/__main__.py` & `distilabel-1.0.3/src/distilabel/__main__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/src/distilabel/distiset.py` & `distilabel-1.0.3/src/distilabel/distiset.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/src/distilabel/cli/__init__.py` & `distilabel-1.0.3/src/distilabel/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/src/distilabel/cli/app.py` & `distilabel-1.0.3/src/distilabel/cli/app.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/src/distilabel/cli/pipeline/__init__.py` & `distilabel-1.0.3/src/distilabel/cli/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/src/distilabel/cli/pipeline/app.py` & `distilabel-1.0.3/src/distilabel/cli/pipeline/app.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/src/distilabel/cli/pipeline/utils.py` & `distilabel-1.0.3/src/distilabel/cli/pipeline/utils.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/src/distilabel/llms/__init__.py` & `distilabel-1.0.3/src/distilabel/llms/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/src/distilabel/llms/anthropic.py` & `distilabel-1.0.3/src/distilabel/llms/anthropic.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/src/distilabel/llms/anyscale.py` & `distilabel-1.0.3/src/distilabel/llms/anyscale.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/src/distilabel/llms/azure.py` & `distilabel-1.0.3/src/distilabel/llms/azure.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/src/distilabel/llms/base.py` & `distilabel-1.0.3/src/distilabel/llms/base.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/src/distilabel/llms/chat_templates.py` & `distilabel-1.0.3/src/distilabel/llms/chat_templates.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/src/distilabel/llms/cohere.py` & `distilabel-1.0.3/src/distilabel/llms/cohere.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/src/distilabel/llms/litellm.py` & `distilabel-1.0.3/src/distilabel/llms/litellm.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/src/distilabel/llms/llamacpp.py` & `distilabel-1.0.3/src/distilabel/llms/llamacpp.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/src/distilabel/llms/mistral.py` & `distilabel-1.0.3/src/distilabel/llms/mistral.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/src/distilabel/llms/mixins.py` & `distilabel-1.0.3/src/distilabel/llms/mixins.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/src/distilabel/llms/ollama.py` & `distilabel-1.0.3/src/distilabel/llms/ollama.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/src/distilabel/llms/openai.py` & `distilabel-1.0.3/src/distilabel/llms/openai.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import os
-from typing import TYPE_CHECKING, Optional
+from typing import TYPE_CHECKING, List, Optional, Union
 
 from pydantic import Field, PrivateAttr, SecretStr, validate_call
 
 from distilabel.llms.base import AsyncLLM
 from distilabel.llms.typing import GenerateOutput
 from distilabel.mixins.runtime_parameters import RuntimeParameter
 from distilabel.steps.tasks.typing import ChatType
@@ -97,15 +97,15 @@
                 f"To use `{self.__class__.__name__}` an API key must be provided via `api_key`"
                 f" attribute or runtime parameter, or set the environment variable `{self._api_key_env_var}`."
             )
 
         self._aclient = AsyncOpenAI(
             base_url=self.base_url,
             api_key=self.api_key.get_secret_value(),
-            max_retries=self.max_retries,
+            max_retries=self.max_retries,  # type: ignore
             timeout=self.timeout,
         )
 
     @property
     def model_name(self) -> str:
         """Returns the model name used for the LLM."""
         return self.model
@@ -116,14 +116,15 @@
         input: ChatType,
         num_generations: int = 1,
         max_new_tokens: int = 128,
         frequency_penalty: float = 0.0,
         presence_penalty: float = 0.0,
         temperature: float = 1.0,
         top_p: float = 1.0,
+        stop: Optional[Union[str, List[str]]] = None,
     ) -> GenerateOutput:
         """Generates `num_generations` responses for the given input using the OpenAI async
         client.
 
         Args:
             input: a single input in chat format to generate responses for.
             num_generations: the number of generations to create per input. Defaults to
@@ -132,31 +133,34 @@
                 Defaults to `128`.
             frequency_penalty: the repetition penalty to use for the generation. Defaults
                 to `0.0`.
             presence_penalty: the presence penalty to use for the generation. Defaults to
                 `0.0`.
             temperature: the temperature to use for the generation. Defaults to `0.1`.
             top_p: the top-p value to use for the generation. Defaults to `1.0`.
+            stop: a string or a list of strings to use as a stop sequence for the generation.
+                Defaults to `None`.
 
         Returns:
             A list of lists of strings containing the generated responses for each input.
         """
         completion = await self._aclient.chat.completions.create(  # type: ignore
             messages=input,  # type: ignore
             model=self.model,
             max_tokens=max_new_tokens,
             n=num_generations,
             frequency_penalty=frequency_penalty,
             presence_penalty=presence_penalty,
             temperature=temperature,
             top_p=top_p,
+            stop=stop,
             timeout=50,
         )
         generations = []
         for choice in completion.choices:
             if (content := choice.message.content) is None:
-                self._logger.warning(
+                self._logger.warning(  # type: ignore
                     f"Received no response using OpenAI client (model: '{self.model}')."
                     f" Finish reason was: {choice.finish_reason}"
                 )
             generations.append(content)
         return generations
```

### Comparing `distilabel-1.0.2/src/distilabel/llms/together.py` & `distilabel-1.0.3/src/distilabel/llms/together.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/src/distilabel/llms/typing.py` & `distilabel-1.0.3/src/distilabel/llms/typing.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/src/distilabel/llms/vertexai.py` & `distilabel-1.0.3/src/distilabel/llms/vertexai.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/src/distilabel/llms/vllm.py` & `distilabel-1.0.3/src/distilabel/llms/vllm.py`

 * *Files 0% similar despite different names*

```diff
@@ -145,14 +145,15 @@
                 the `SamplingParams` class from `vllm`.
 
         Returns:
             A list of lists of strings containing the generated responses for each input.
         """
         if extra_sampling_params is None:
             extra_sampling_params = {}
+
         sampling_params = SamplingParams(  # type: ignore
             n=num_generations,
             presence_penalty=presence_penalty,
             frequency_penalty=frequency_penalty,
             temperature=temperature,
             top_p=top_p,
             top_k=top_k,
```

### Comparing `distilabel-1.0.2/src/distilabel/llms/huggingface/__init__.py` & `distilabel-1.0.3/src/distilabel/llms/huggingface/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/src/distilabel/llms/huggingface/inference_endpoints.py` & `distilabel-1.0.3/src/distilabel/llms/huggingface/inference_endpoints.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import asyncio
 import os
 import random
+import warnings
 from typing import TYPE_CHECKING, Any, List, Optional, Union
 
 from pydantic import (
     Field,
     PrivateAttr,
     SecretStr,
     ValidationError,
@@ -258,29 +259,31 @@
         self,
         input: "ChatType",
         max_new_tokens: int = 128,
         frequency_penalty: float = 0.0,
         presence_penalty: float = 0.0,
         temperature: float = 1.0,
         top_p: Optional[float] = None,
+        stop: Optional[Union[str, List[str]]] = None,
     ) -> GenerateOutput:
         """Generates completions for the given input using the OpenAI async client."""
         completion = await self._aclient.chat.completions.create(  # type: ignore
             messages=input,  # type: ignore
             model="tgi",
             max_tokens=max_new_tokens,
             n=1,
             frequency_penalty=frequency_penalty,
             presence_penalty=presence_penalty,
             temperature=temperature,
             top_p=top_p,
+            stop=stop,
             timeout=50,
         )
         if completion.choices[0].message.content is None:
-            self._logger.warning(
+            self._logger.warning(  # type: ignore
                 f"⚠️ Received no response using OpenAI client (model: '{self.model_name}')."
                 f" Finish reason was: {completion.choices[0].finish_reason}"
             )
         return [completion.choices[0].message.content]
 
     # TODO: add `num_generations` parameter once either TGI or `AsyncInferenceClient` allows `n` parameter
     @validate_call
@@ -292,14 +295,15 @@
         presence_penalty: float = 0.0,
         repetition_penalty: Optional[float] = None,
         temperature: float = 1.0,
         do_sample: bool = False,
         top_k: Optional[int] = None,
         top_p: Optional[float] = None,
         typical_p: Optional[float] = None,
+        stop_sequences: Optional[Union[str, List[str]]] = None,
     ) -> "GenerateOutput":
         """Generates completions for the given input using the OpenAI async client.
 
         Args:
             input: a single input in chat format to generate responses for.
             max_new_tokens: the maximum number of new tokens that the model will generate.
                 Defaults to `128`.
@@ -312,27 +316,41 @@
             temperature: the temperature to use for the generation. Defaults to `1.0`.
             do_sample: whether to use sampling for the generation. Defaults to `False`.
                 Only applies if `use_openai_client=False`.
             top_k: the top-k value to use for the generation. Defaults to `0.8`, since neither
                 `0.0` nor `1.0` are valid values in TGI.
             top_p: the top-p value to use for the generation. Defaults to `1.0`.
             typical_p: the typical-p value to use for the generation. Defaults to `0.5`.
+            stop_sequences: either a single string or a list of strings containing the sequences
+                to stop the generation at. Defaults to `None`, but will be set to the
+                `tokenizer.eos_token` if available.
 
         Returns:
             A list of lists of strings containing the generated responses for each input.
         """
+        if stop_sequences is not None:
+            if isinstance(stop_sequences, str):
+                stop_sequences = [stop_sequences]
+            if len(stop_sequences) > 4:
+                warnings.warn(
+                    "Only up to 4 stop sequences are allowed, so keeping the first 4 items only.",
+                    UserWarning,
+                    stacklevel=2,
+                )
+                stop_sequences = stop_sequences[:4]
 
         if self.use_openai_client:
             return await self._openai_agenerate(
                 input=input,
                 max_new_tokens=max_new_tokens,
                 frequency_penalty=frequency_penalty,
                 presence_penalty=presence_penalty,
                 temperature=temperature,
                 top_p=top_p,
+                stop=stop_sequences,
             )
 
         if self._tokenizer is not None:
             prompt = self._tokenizer.apply_chat_template(  # type: ignore
                 conversation=input,  # type: ignore
                 tokenize=False,
                 add_generation_prompt=True,
@@ -349,18 +367,19 @@
                 repetition_penalty=repetition_penalty,
                 temperature=temperature,
                 top_p=top_p,
                 top_k=top_k,
                 # NOTE: here to ensure that the cache is not used and a different response is
                 # generated every time
                 seed=random.randint(0, 2147483647),
+                stop_sequences=stop_sequences,
             )
             return [completion]
         except Exception as e:
-            self._logger.warning(
+            self._logger.warning(  # type: ignore
                 f"⚠️ Received no response using Inference Client (model: '{self.model_name}')."
                 f" Finish reason was: {e}"
             )
             return [None]
 
     # TODO: remove this function once `AsyncInferenceClient` allows `n` parameter
     @override
```

### Comparing `distilabel-1.0.2/src/distilabel/llms/huggingface/transformers.py` & `distilabel-1.0.3/src/distilabel/llms/huggingface/transformers.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/src/distilabel/mixins/__init__.py` & `distilabel-1.0.3/src/distilabel/mixins/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/src/distilabel/mixins/runtime_parameters.py` & `distilabel-1.0.3/src/distilabel/mixins/runtime_parameters.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/src/distilabel/pipeline/__init__.py` & `distilabel-1.0.3/src/distilabel/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/src/distilabel/pipeline/_dag.py` & `distilabel-1.0.3/src/distilabel/pipeline/_dag.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/src/distilabel/pipeline/base.py` & `distilabel-1.0.3/src/distilabel/pipeline/base.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/src/distilabel/pipeline/local.py` & `distilabel-1.0.3/src/distilabel/pipeline/local.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/src/distilabel/pipeline/utils.py` & `distilabel-1.0.3/src/distilabel/pipeline/utils.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/src/distilabel/steps/__init__.py` & `distilabel-1.0.3/src/distilabel/steps/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/src/distilabel/steps/base.py` & `distilabel-1.0.3/src/distilabel/steps/base.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/src/distilabel/steps/combine.py` & `distilabel-1.0.3/src/distilabel/steps/combine.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/src/distilabel/steps/conversation.py` & `distilabel-1.0.3/src/distilabel/steps/conversation.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/src/distilabel/steps/decorator.py` & `distilabel-1.0.3/src/distilabel/steps/decorator.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/src/distilabel/steps/deita.py` & `distilabel-1.0.3/src/distilabel/steps/deita.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/src/distilabel/steps/expand.py` & `distilabel-1.0.3/src/distilabel/steps/expand.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/src/distilabel/steps/keep.py` & `distilabel-1.0.3/src/distilabel/steps/keep.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/src/distilabel/steps/typing.py` & `distilabel-1.0.3/src/distilabel/steps/typing.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/src/distilabel/steps/argilla/__init__.py` & `distilabel-1.0.3/src/distilabel/steps/argilla/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/src/distilabel/steps/argilla/base.py` & `distilabel-1.0.3/src/distilabel/steps/argilla/base.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/src/distilabel/steps/argilla/preference.py` & `distilabel-1.0.3/src/distilabel/steps/argilla/preference.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/src/distilabel/steps/argilla/text_generation.py` & `distilabel-1.0.3/src/distilabel/steps/argilla/text_generation.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/src/distilabel/steps/generators/__init__.py` & `distilabel-1.0.3/src/distilabel/steps/generators/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/src/distilabel/steps/generators/data.py` & `distilabel-1.0.3/src/distilabel/steps/generators/data.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/src/distilabel/steps/generators/huggingface.py` & `distilabel-1.0.3/src/distilabel/steps/generators/huggingface.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/src/distilabel/steps/globals/__init__.py` & `distilabel-1.0.3/src/distilabel/steps/globals/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/src/distilabel/steps/globals/huggingface.py` & `distilabel-1.0.3/src/distilabel/steps/globals/huggingface.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/src/distilabel/steps/tasks/__init__.py` & `distilabel-1.0.3/src/distilabel/steps/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/src/distilabel/steps/tasks/base.py` & `distilabel-1.0.3/src/distilabel/steps/tasks/base.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/src/distilabel/steps/tasks/complexity_scorer.py` & `distilabel-1.0.3/src/distilabel/steps/tasks/complexity_scorer.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/src/distilabel/steps/tasks/generate_embeddings.py` & `distilabel-1.0.3/src/distilabel/steps/tasks/generate_embeddings.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/src/distilabel/steps/tasks/instruction_backtranslation.py` & `distilabel-1.0.3/src/distilabel/steps/tasks/instruction_backtranslation.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/src/distilabel/steps/tasks/pair_rm.py` & `distilabel-1.0.3/src/distilabel/steps/tasks/pair_rm.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/src/distilabel/steps/tasks/quality_scorer.py` & `distilabel-1.0.3/src/distilabel/steps/tasks/quality_scorer.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/src/distilabel/steps/tasks/self_instruct.py` & `distilabel-1.0.3/src/distilabel/steps/tasks/self_instruct.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/src/distilabel/steps/tasks/text_generation.py` & `distilabel-1.0.3/src/distilabel/steps/tasks/text_generation.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/src/distilabel/steps/tasks/typing.py` & `distilabel-1.0.3/src/distilabel/steps/tasks/typing.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/src/distilabel/steps/tasks/ultrafeedback.py` & `distilabel-1.0.3/src/distilabel/steps/tasks/ultrafeedback.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/src/distilabel/steps/tasks/evol_instruct/__init__.py` & `distilabel-1.0.3/src/distilabel/steps/tasks/evol_instruct/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/src/distilabel/steps/tasks/evol_instruct/base.py` & `distilabel-1.0.3/src/distilabel/steps/tasks/evol_instruct/base.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/src/distilabel/steps/tasks/evol_instruct/english_nouns.txt` & `distilabel-1.0.3/src/distilabel/steps/tasks/evol_instruct/english_nouns.txt`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/src/distilabel/steps/tasks/evol_instruct/generator.py` & `distilabel-1.0.3/src/distilabel/steps/tasks/evol_instruct/generator.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/src/distilabel/steps/tasks/evol_instruct/utils.py` & `distilabel-1.0.3/src/distilabel/steps/tasks/evol_instruct/utils.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/src/distilabel/steps/tasks/evol_instruct/evol_complexity/__init__.py` & `distilabel-1.0.3/src/distilabel/steps/tasks/evol_instruct/evol_complexity/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/src/distilabel/steps/tasks/evol_instruct/evol_complexity/base.py` & `distilabel-1.0.3/src/distilabel/steps/tasks/evol_instruct/evol_complexity/base.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/src/distilabel/steps/tasks/evol_instruct/evol_complexity/generator.py` & `distilabel-1.0.3/src/distilabel/steps/tasks/evol_instruct/evol_complexity/generator.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/src/distilabel/steps/tasks/evol_instruct/evol_complexity/utils.py` & `distilabel-1.0.3/src/distilabel/steps/tasks/evol_instruct/evol_complexity/utils.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/src/distilabel/steps/tasks/evol_quality/__init__.py` & `distilabel-1.0.3/src/distilabel/steps/tasks/evol_quality/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/src/distilabel/steps/tasks/evol_quality/base.py` & `distilabel-1.0.3/src/distilabel/steps/tasks/evol_quality/base.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/src/distilabel/steps/tasks/evol_quality/utils.py` & `distilabel-1.0.3/src/distilabel/steps/tasks/evol_quality/utils.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/src/distilabel/steps/tasks/templates/instruction-backtranslation.jinja2` & `distilabel-1.0.3/src/distilabel/steps/tasks/templates/instruction-backtranslation.jinja2`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/src/distilabel/steps/tasks/templates/ultrafeedback/helpfulness.jinja2` & `distilabel-1.0.3/src/distilabel/steps/tasks/templates/ultrafeedback/helpfulness.jinja2`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/src/distilabel/steps/tasks/templates/ultrafeedback/honesty.jinja2` & `distilabel-1.0.3/src/distilabel/steps/tasks/templates/ultrafeedback/honesty.jinja2`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/src/distilabel/steps/tasks/templates/ultrafeedback/instruction-following.jinja2` & `distilabel-1.0.3/src/distilabel/steps/tasks/templates/ultrafeedback/instruction-following.jinja2`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/src/distilabel/steps/tasks/templates/ultrafeedback/overall-rating.jinja2` & `distilabel-1.0.3/src/distilabel/steps/tasks/templates/ultrafeedback/overall-rating.jinja2`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/src/distilabel/steps/tasks/templates/ultrafeedback/truthfulness.jinja2` & `distilabel-1.0.3/src/distilabel/steps/tasks/templates/ultrafeedback/truthfulness.jinja2`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/src/distilabel/utils/__init__.py` & `distilabel-1.0.3/src/distilabel/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/src/distilabel/utils/chat.py` & `distilabel-1.0.3/src/distilabel/utils/chat.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/src/distilabel/utils/dicts.py` & `distilabel-1.0.3/src/distilabel/utils/dicts.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/src/distilabel/utils/docstring.py` & `distilabel-1.0.3/src/distilabel/utils/docstring.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/src/distilabel/utils/files.py` & `distilabel-1.0.3/src/distilabel/utils/files.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/src/distilabel/utils/itertools.py` & `distilabel-1.0.3/src/distilabel/utils/itertools.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/src/distilabel/utils/lists.py` & `distilabel-1.0.3/src/distilabel/utils/lists.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/src/distilabel/utils/logging.py` & `distilabel-1.0.3/src/distilabel/utils/logging.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/src/distilabel/utils/notebook.py` & `distilabel-1.0.3/src/distilabel/utils/notebook.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/src/distilabel/utils/serialization.py` & `distilabel-1.0.3/src/distilabel/utils/serialization.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/src/distilabel/utils/typing_.py` & `distilabel-1.0.3/src/distilabel/utils/typing_.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/src/distilabel/utils/card/__init__.py` & `distilabel-1.0.3/src/distilabel/utils/card/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/src/distilabel/utils/card/dataset_card.py` & `distilabel-1.0.3/src/distilabel/utils/card/dataset_card.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/src/distilabel/utils/card/distilabel_template.md` & `distilabel-1.0.3/src/distilabel/utils/card/distilabel_template.md`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/tests/__init__.py` & `distilabel-1.0.3/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/tests/integration/test_pipe_llms.py` & `distilabel-1.0.3/tests/integration/test_pipe_llms.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/tests/integration/test_pipe_simple.py` & `distilabel-1.0.3/tests/integration/test_pipe_simple.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/tests/unit/__init__.py` & `distilabel-1.0.3/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/tests/unit/test_distiset.py` & `distilabel-1.0.3/tests/unit/test_distiset.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/tests/unit/test_imports.py` & `distilabel-1.0.3/tests/unit/test_imports.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/tests/unit/cli/__init__.py` & `distilabel-1.0.3/tests/unit/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/tests/unit/cli/test_pipeline.yaml` & `distilabel-1.0.3/tests/unit/cli/test_pipeline.yaml`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/tests/unit/cli/utils.py` & `distilabel-1.0.3/tests/unit/cli/utils.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/tests/unit/cli/pipeline/__init__.py` & `distilabel-1.0.3/tests/unit/cli/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/tests/unit/cli/pipeline/test_app.py` & `distilabel-1.0.3/tests/unit/cli/pipeline/test_app.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/tests/unit/cli/pipeline/utils.py` & `distilabel-1.0.3/tests/unit/cli/pipeline/utils.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/tests/unit/llms/__init__.py` & `distilabel-1.0.3/tests/unit/llms/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/tests/unit/llms/test_anthropic.py` & `distilabel-1.0.3/tests/unit/llms/test_anthropic.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/tests/unit/llms/test_anyscale.py` & `distilabel-1.0.3/tests/unit/llms/test_anyscale.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/tests/unit/llms/test_azure.py` & `distilabel-1.0.3/tests/unit/llms/test_azure.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/tests/unit/llms/test_cohere.py` & `distilabel-1.0.3/tests/unit/llms/test_cohere.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/tests/unit/llms/test_litellm.py` & `distilabel-1.0.3/tests/unit/llms/test_litellm.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/tests/unit/llms/test_llamacpp.py` & `distilabel-1.0.3/tests/unit/llms/test_llamacpp.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/tests/unit/llms/test_mistral.py` & `distilabel-1.0.3/tests/unit/llms/test_mistral.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/tests/unit/llms/test_mixins.py` & `distilabel-1.0.3/tests/unit/llms/test_mixins.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/tests/unit/llms/test_ollama.py` & `distilabel-1.0.3/tests/unit/llms/test_ollama.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/tests/unit/llms/test_openai.py` & `distilabel-1.0.3/tests/unit/llms/test_openai.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/tests/unit/llms/test_together.py` & `distilabel-1.0.3/tests/unit/llms/test_together.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/tests/unit/llms/test_vertexai.py` & `distilabel-1.0.3/tests/unit/llms/test_vertexai.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/tests/unit/llms/huggingface/__init__.py` & `distilabel-1.0.3/tests/unit/llms/huggingface/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/tests/unit/llms/huggingface/test_inference_endpoints.py` & `distilabel-1.0.3/tests/unit/llms/huggingface/test_inference_endpoints.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/tests/unit/llms/huggingface/test_transformers.py` & `distilabel-1.0.3/tests/unit/llms/huggingface/test_transformers.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/tests/unit/mixins/__init__.py` & `distilabel-1.0.3/tests/unit/mixins/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/tests/unit/mixins/test_runtime_parameters.py` & `distilabel-1.0.3/tests/unit/mixins/test_runtime_parameters.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/tests/unit/pipeline/__init__.py` & `distilabel-1.0.3/tests/unit/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/tests/unit/pipeline/conftest.py` & `distilabel-1.0.3/tests/unit/pipeline/conftest.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/tests/unit/pipeline/test_base.py` & `distilabel-1.0.3/tests/unit/pipeline/test_base.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/tests/unit/pipeline/test_dag.py` & `distilabel-1.0.3/tests/unit/pipeline/test_dag.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/tests/unit/pipeline/test_local.py` & `distilabel-1.0.3/tests/unit/pipeline/test_local.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/tests/unit/pipeline/utils.py` & `distilabel-1.0.3/tests/unit/pipeline/utils.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/tests/unit/steps/__init__.py` & `distilabel-1.0.3/tests/unit/steps/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/tests/unit/steps/test_base.py` & `distilabel-1.0.3/tests/unit/steps/test_base.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/tests/unit/steps/test_combine.py` & `distilabel-1.0.3/tests/unit/steps/test_combine.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/tests/unit/steps/test_conversation.py` & `distilabel-1.0.3/tests/unit/steps/test_conversation.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/tests/unit/steps/test_decorator.py` & `distilabel-1.0.3/tests/unit/steps/test_decorator.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/tests/unit/steps/test_deita.py` & `distilabel-1.0.3/tests/unit/steps/test_deita.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/tests/unit/steps/test_expand.py` & `distilabel-1.0.3/tests/unit/steps/test_expand.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/tests/unit/steps/test_keep.py` & `distilabel-1.0.3/tests/unit/steps/test_keep.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/tests/unit/steps/argilla/__init__.py` & `distilabel-1.0.3/tests/unit/steps/argilla/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/tests/unit/steps/argilla/test_base.py` & `distilabel-1.0.3/tests/unit/steps/argilla/test_base.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/tests/unit/steps/argilla/test_preference.py` & `distilabel-1.0.3/tests/unit/steps/argilla/test_preference.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/tests/unit/steps/argilla/test_text_generation.py` & `distilabel-1.0.3/tests/unit/steps/argilla/test_text_generation.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/tests/unit/steps/generators/test_data.py` & `distilabel-1.0.3/tests/unit/steps/generators/test_data.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/tests/unit/steps/tasks/__init__.py` & `distilabel-1.0.3/tests/unit/steps/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/tests/unit/steps/tasks/conftest.py` & `distilabel-1.0.3/tests/unit/steps/tasks/conftest.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/tests/unit/steps/tasks/test_base.py` & `distilabel-1.0.3/tests/unit/steps/tasks/test_base.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/tests/unit/steps/tasks/test_complexity_scorer.py` & `distilabel-1.0.3/tests/unit/steps/tasks/test_complexity_scorer.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/tests/unit/steps/tasks/test_generate_embeddings.py` & `distilabel-1.0.3/tests/unit/steps/tasks/test_generate_embeddings.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/tests/unit/steps/tasks/test_instruction_backtranslation.py` & `distilabel-1.0.3/tests/unit/steps/tasks/test_instruction_backtranslation.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/tests/unit/steps/tasks/test_pair_rm.py` & `distilabel-1.0.3/tests/unit/steps/tasks/test_pair_rm.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/tests/unit/steps/tasks/test_quality_scorer.py` & `distilabel-1.0.3/tests/unit/steps/tasks/test_quality_scorer.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/tests/unit/steps/tasks/test_self_instruct.py` & `distilabel-1.0.3/tests/unit/steps/tasks/test_self_instruct.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/tests/unit/steps/tasks/test_text_generation.py` & `distilabel-1.0.3/tests/unit/steps/tasks/test_text_generation.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/tests/unit/steps/tasks/test_ultrafeedback.py` & `distilabel-1.0.3/tests/unit/steps/tasks/test_ultrafeedback.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/tests/unit/steps/tasks/utils.py` & `distilabel-1.0.3/tests/unit/steps/tasks/utils.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/tests/unit/steps/tasks/evol_instruct/__init__.py` & `distilabel-1.0.3/tests/unit/steps/tasks/evol_instruct/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/tests/unit/steps/tasks/evol_instruct/test_base.py` & `distilabel-1.0.3/tests/unit/steps/tasks/evol_instruct/test_base.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/tests/unit/steps/tasks/evol_instruct/test_generator.py` & `distilabel-1.0.3/tests/unit/steps/tasks/evol_instruct/test_generator.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/tests/unit/steps/tasks/evol_instruct/evol_complexity.py/__init__.py` & `distilabel-1.0.3/tests/unit/steps/tasks/evol_instruct/evol_complexity.py/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/tests/unit/steps/tasks/evol_instruct/evol_complexity.py/test_base.py` & `distilabel-1.0.3/tests/unit/steps/tasks/evol_instruct/evol_complexity.py/test_base.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/tests/unit/steps/tasks/evol_instruct/evol_complexity.py/test_generator.py` & `distilabel-1.0.3/tests/unit/steps/tasks/evol_instruct/evol_complexity.py/test_generator.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/tests/unit/steps/tasks/evol_quality/__init__.py` & `distilabel-1.0.3/tests/unit/steps/tasks/evol_quality/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/tests/unit/steps/tasks/evol_quality/test_base.py` & `distilabel-1.0.3/tests/unit/steps/tasks/evol_quality/test_base.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/tests/unit/utils/__init__.py` & `distilabel-1.0.3/tests/unit/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/tests/unit/utils/test_chat.py` & `distilabel-1.0.3/tests/unit/utils/test_chat.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/tests/unit/utils/test_docstring.py` & `distilabel-1.0.3/tests/unit/utils/test_docstring.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/tests/unit/utils/test_lists.py` & `distilabel-1.0.3/tests/unit/utils/test_lists.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/tests/unit/utils/test_typing.py` & `distilabel-1.0.3/tests/unit/utils/test_typing.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/.gitignore` & `distilabel-1.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/LICENSE` & `distilabel-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/LICENSE_HEADER` & `distilabel-1.0.3/LICENSE_HEADER`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/README.md` & `distilabel-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/pyproject.toml` & `distilabel-1.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.2/PKG-INFO` & `distilabel-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: distilabel
-Version: 1.0.2
+Version: 1.0.3
 Summary: AI Feedback (AIF) framework
 Project-URL: Documentation, https://distilabel.argilla.io/
 Project-URL: Issues, https://github.com/argilla/distilabel/issues
 Project-URL: Source, https://github.com/argilla/distilabel
 Author-email: Argilla <admin@argilla.io>
 License-Expression: MIT
 License-File: LICENSE
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_066q_nfa_/tmp3tvbb7_c_TarContainer/0/255", line 85, column 75: Levels of opening and closing headings don't match*

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.3 Name: distilabel Version: 1.0.2 Summary: AI Feedback
+Metadata-Version: 2.3 Name: distilabel Version: 1.0.3 Summary: AI Feedback
 (AIF) framework Project-URL: Documentation, https://distilabel.argilla.io/
 Project-URL: Issues, https://github.com/argilla/distilabel/issues Project-URL:
 Source, https://github.com/argilla/distilabel Author-email: Argilla
 argilla.io> License-Expression: MIT License-File: LICENSE License-File:
 LICENSE_HEADER Keywords: alignment,annotation,data,llm,rlaif,synthetic
 Classifier: Development Status :: 4 - Beta Classifier: Programming Language ::
 Python Classifier: Programming Language :: Python :: 3.8 Classifier:
```


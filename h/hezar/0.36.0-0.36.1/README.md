# Comparing `tmp/hezar-0.36.0.tar.gz` & `tmp/hezar-0.36.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hezar-0.36.0.tar", max compression
+gzip compressed data, was "hezar-0.36.1.tar", max compression
```

## Comparing `hezar-0.36.0.tar` & `hezar-0.36.1.tar`

### file list

```diff
@@ -1,136 +1,136 @@
--rw-r--r--   0        0        0    11337 2024-02-08 09:18:49.117827 hezar-0.36.0/LICENSE
--rw-r--r--   0        0        0    14243 2024-02-08 09:18:49.117827 hezar-0.36.0/README.md
--rw-r--r--   0        0        0      623 2024-02-08 09:18:49.121827 hezar-0.36.0/hezar/__init__.py
--rw-r--r--   0        0        0     5651 2024-02-08 09:18:49.121827 hezar-0.36.0/hezar/builders.py
--rw-r--r--   0        0        0    16833 2024-02-08 09:18:49.121827 hezar-0.36.0/hezar/configs.py
--rw-r--r--   0        0        0     4738 2024-02-08 09:18:49.121827 hezar-0.36.0/hezar/constants.py
--rw-r--r--   0        0        0       54 2024-02-08 09:18:49.121827 hezar-0.36.0/hezar/data/__init__.py
--rw-r--r--   0        0        0    13746 2024-02-08 09:18:49.121827 hezar-0.36.0/hezar/data/data_collators.py
--rw-r--r--   0        0        0      634 2024-02-08 09:18:49.121827 hezar-0.36.0/hezar/data/datasets/__init__.py
--rw-r--r--   0        0        0     3279 2024-02-08 09:18:49.121827 hezar-0.36.0/hezar/data/datasets/dataset.py
--rw-r--r--   0        0        0     3727 2024-02-08 09:18:49.121827 hezar-0.36.0/hezar/data/datasets/image_captioning_dataset.py
--rw-r--r--   0        0        0     7384 2024-02-08 09:18:49.121827 hezar-0.36.0/hezar/data/datasets/ocr_dataset.py
--rw-r--r--   0        0        0     5923 2024-02-08 09:18:49.121827 hezar-0.36.0/hezar/data/datasets/sequence_labeling_dataset.py
--rw-r--r--   0        0        0     3030 2024-02-08 09:18:49.121827 hezar-0.36.0/hezar/data/datasets/speech_recognition_dataset.py
--rw-r--r--   0        0        0     4498 2024-02-08 09:18:49.121827 hezar-0.36.0/hezar/data/datasets/text_classification_dataset.py
--rw-r--r--   0        0        0     4820 2024-02-08 09:18:49.121827 hezar-0.36.0/hezar/data/datasets/text_summarization_dataset.py
--rw-r--r--   0        0        0      202 2024-02-08 09:18:49.121827 hezar-0.36.0/hezar/embeddings/__init__.py
--rw-r--r--   0        0        0    11544 2024-02-08 09:18:49.121827 hezar-0.36.0/hezar/embeddings/embedding.py
--rw-r--r--   0        0        0     7171 2024-02-08 09:18:49.121827 hezar-0.36.0/hezar/embeddings/fasttext.py
--rw-r--r--   0        0        0     7668 2024-02-08 09:18:49.121827 hezar-0.36.0/hezar/embeddings/word2vec.py
--rw-r--r--   0        0        0      444 2024-02-08 09:18:49.121827 hezar-0.36.0/hezar/metrics/__init__.py
--rw-r--r--   0        0        0     2285 2024-02-08 09:18:49.121827 hezar-0.36.0/hezar/metrics/accuracy.py
--rw-r--r--   0        0        0     2484 2024-02-08 09:18:49.121827 hezar-0.36.0/hezar/metrics/bleu.py
--rw-r--r--   0        0        0     3711 2024-02-08 09:18:49.121827 hezar-0.36.0/hezar/metrics/cer.py
--rw-r--r--   0        0        0     3209 2024-02-08 09:18:49.121827 hezar-0.36.0/hezar/metrics/f1.py
--rw-r--r--   0        0        0     1302 2024-02-08 09:18:49.121827 hezar-0.36.0/hezar/metrics/metric.py
--rw-r--r--   0        0        0     3566 2024-02-08 09:18:49.121827 hezar-0.36.0/hezar/metrics/precision.py
--rw-r--r--   0        0        0     3509 2024-02-08 09:18:49.121827 hezar-0.36.0/hezar/metrics/recall.py
--rw-r--r--   0        0        0     3155 2024-02-08 09:18:49.121827 hezar-0.36.0/hezar/metrics/rouge.py
--rw-r--r--   0        0        0     4029 2024-02-08 09:18:49.121827 hezar-0.36.0/hezar/metrics/seqeval.py
--rw-r--r--   0        0        0     2950 2024-02-08 09:18:49.121827 hezar-0.36.0/hezar/metrics/wer.py
--rw-r--r--   0        0        0      333 2024-02-08 09:18:49.121827 hezar-0.36.0/hezar/models/__init__.py
--rw-r--r--   0        0        0       88 2024-02-08 09:18:49.121827 hezar-0.36.0/hezar/models/backbone/__init__.py
--rw-r--r--   0        0        0       35 2024-02-08 09:18:49.121827 hezar-0.36.0/hezar/models/backbone/bert/__init__.py
--rw-r--r--   0        0        0     2787 2024-02-08 09:18:49.121827 hezar-0.36.0/hezar/models/backbone/bert/bert.py
--rw-r--r--   0        0        0      743 2024-02-08 09:18:49.121827 hezar-0.36.0/hezar/models/backbone/bert/bert_config.py
--rw-r--r--   0        0        0       53 2024-02-08 09:18:49.121827 hezar-0.36.0/hezar/models/backbone/distilbert/__init__.py
--rw-r--r--   0        0        0     2288 2024-02-08 09:18:49.121827 hezar-0.36.0/hezar/models/backbone/distilbert/distilbert.py
--rw-r--r--   0        0        0      618 2024-02-08 09:18:49.121827 hezar-0.36.0/hezar/models/backbone/distilbert/distilbert_config.py
--rw-r--r--   0        0        0       44 2024-02-08 09:18:49.121827 hezar-0.36.0/hezar/models/backbone/roberta/__init__.py
--rw-r--r--   0        0        0     2788 2024-02-08 09:18:49.121827 hezar-0.36.0/hezar/models/backbone/roberta/roberta.py
--rw-r--r--   0        0        0      812 2024-02-08 09:18:49.121827 hezar-0.36.0/hezar/models/backbone/roberta/roberta_config.py
--rw-r--r--   0        0        0       55 2024-02-08 09:18:49.121827 hezar-0.36.0/hezar/models/backbone/vit/__init__.py
--rw-r--r--   0        0        0     2170 2024-02-08 09:18:49.121827 hezar-0.36.0/hezar/models/backbone/vit/vit.py
--rw-r--r--   0        0        0      572 2024-02-08 09:18:49.121827 hezar-0.36.0/hezar/models/backbone/vit/vit_config.py
--rw-r--r--   0        0        0      120 2024-02-08 09:18:49.121827 hezar-0.36.0/hezar/models/image2text/__init__.py
--rw-r--r--   0        0        0      131 2024-02-08 09:18:49.121827 hezar-0.36.0/hezar/models/image2text/beit_roberta/__init__.py
--rw-r--r--   0        0        0     3491 2024-02-08 09:18:49.121827 hezar-0.36.0/hezar/models/image2text/beit_roberta/beit_roberta_image2text.py
--rw-r--r--   0        0        0     2376 2024-02-08 09:18:49.121827 hezar-0.36.0/hezar/models/image2text/beit_roberta/beit_roberta_image2text_config.py
--rw-r--r--   0        0        0      101 2024-02-08 09:18:49.121827 hezar-0.36.0/hezar/models/image2text/crnn/__init__.py
--rw-r--r--   0        0        0     1106 2024-02-08 09:18:49.121827 hezar-0.36.0/hezar/models/image2text/crnn/crnn_decode_utils.py
--rw-r--r--   0        0        0     4645 2024-02-08 09:18:49.121827 hezar-0.36.0/hezar/models/image2text/crnn/crnn_image2text.py
--rw-r--r--   0        0        0      478 2024-02-08 09:18:49.121827 hezar-0.36.0/hezar/models/image2text/crnn/crnn_image2text_config.py
--rw-r--r--   0        0        0      105 2024-02-08 09:18:49.121827 hezar-0.36.0/hezar/models/image2text/trocr/__init__.py
--rw-r--r--   0        0        0     3428 2024-02-08 09:18:49.121827 hezar-0.36.0/hezar/models/image2text/trocr/trocr_image2text.py
--rw-r--r--   0        0        0     1899 2024-02-08 09:18:49.121827 hezar-0.36.0/hezar/models/image2text/trocr/trocr_image2text_config.py
--rw-r--r--   0        0        0      115 2024-02-08 09:18:49.121827 hezar-0.36.0/hezar/models/image2text/vit_gpt2/__init__.py
--rw-r--r--   0        0        0     3461 2024-02-08 09:18:49.121827 hezar-0.36.0/hezar/models/image2text/vit_gpt2/vit_gpt2_image2text.py
--rw-r--r--   0        0        0     1872 2024-02-08 09:18:49.121827 hezar-0.36.0/hezar/models/image2text/vit_gpt2/vit_gpt2_image2text_config.py
--rw-r--r--   0        0        0      127 2024-02-08 09:18:49.121827 hezar-0.36.0/hezar/models/image2text/vit_roberta/__init__.py
--rw-r--r--   0        0        0     3862 2024-02-08 09:18:49.121827 hezar-0.36.0/hezar/models/image2text/vit_roberta/vit_roberta_image2text.py
--rw-r--r--   0        0        0     1952 2024-02-08 09:18:49.121827 hezar-0.36.0/hezar/models/image2text/vit_roberta/vit_roberta_image2text_config.py
--rw-r--r--   0        0        0       69 2024-02-08 09:18:49.121827 hezar-0.36.0/hezar/models/mask_filling/__init__.py
--rw-r--r--   0        0        0      107 2024-02-08 09:18:49.121827 hezar-0.36.0/hezar/models/mask_filling/bert/__init__.py
--rw-r--r--   0        0        0     4328 2024-02-08 09:18:49.121827 hezar-0.36.0/hezar/models/mask_filling/bert/bert_mask_filling.py
--rw-r--r--   0        0        0      771 2024-02-08 09:18:49.121827 hezar-0.36.0/hezar/models/mask_filling/bert/bert_mask_filling_config.py
--rw-r--r--   0        0        0      131 2024-02-08 09:18:49.121827 hezar-0.36.0/hezar/models/mask_filling/distilbert/__init__.py
--rw-r--r--   0        0        0     3929 2024-02-08 09:18:49.121827 hezar-0.36.0/hezar/models/mask_filling/distilbert/distilbert_mask_filling.py
--rw-r--r--   0        0        0      637 2024-02-08 09:18:49.121827 hezar-0.36.0/hezar/models/mask_filling/distilbert/distilbert_mask_filling_config.py
--rw-r--r--   0        0        0      119 2024-02-08 09:18:49.125827 hezar-0.36.0/hezar/models/mask_filling/roberta/__init__.py
--rw-r--r--   0        0        0     4392 2024-02-08 09:18:49.125827 hezar-0.36.0/hezar/models/mask_filling/roberta/roberta_mask_filling.py
--rw-r--r--   0        0        0      831 2024-02-08 09:18:49.125827 hezar-0.36.0/hezar/models/mask_filling/roberta/roberta_mask_filling_config.py
--rw-r--r--   0        0        0    20158 2024-02-08 09:18:49.125827 hezar-0.36.0/hezar/models/model.py
--rw-r--r--   0        0        0     2146 2024-02-08 09:18:49.125827 hezar-0.36.0/hezar/models/model_outputs.py
--rw-r--r--   0        0        0       69 2024-02-08 09:18:49.125827 hezar-0.36.0/hezar/models/sequence_labeling/__init__.py
--rw-r--r--   0        0        0      127 2024-02-08 09:18:49.125827 hezar-0.36.0/hezar/models/sequence_labeling/bert/__init__.py
--rw-r--r--   0        0        0     5118 2024-02-08 09:18:49.125827 hezar-0.36.0/hezar/models/sequence_labeling/bert/bert_sequence_labeling.py
--rw-r--r--   0        0        0      931 2024-02-08 09:18:49.125827 hezar-0.36.0/hezar/models/sequence_labeling/bert/bert_sequence_labeling_config.py
--rw-r--r--   0        0        0      151 2024-02-08 09:18:49.125827 hezar-0.36.0/hezar/models/sequence_labeling/distilbert/__init__.py
--rw-r--r--   0        0        0     5172 2024-02-08 09:18:49.125827 hezar-0.36.0/hezar/models/sequence_labeling/distilbert/distilbert_sequence_labeling.py
--rw-r--r--   0        0        0      872 2024-02-08 09:18:49.125827 hezar-0.36.0/hezar/models/sequence_labeling/distilbert/distilbert_sequence_labeling_config.py
--rw-r--r--   0        0        0      139 2024-02-08 09:18:49.125827 hezar-0.36.0/hezar/models/sequence_labeling/roberta/__init__.py
--rw-r--r--   0        0        0     5821 2024-02-08 09:18:49.125827 hezar-0.36.0/hezar/models/sequence_labeling/roberta/roberta_sequence_labeling.py
--rw-r--r--   0        0        0     1025 2024-02-08 09:18:49.125827 hezar-0.36.0/hezar/models/sequence_labeling/roberta/roberta_sequence_labeling_config.py
--rw-r--r--   0        0        0       23 2024-02-08 09:18:49.125827 hezar-0.36.0/hezar/models/speech_recognition/__init__.py
--rw-r--r--   0        0        0      306 2024-02-08 09:18:49.125827 hezar-0.36.0/hezar/models/speech_recognition/whisper/__init__.py
--rw-r--r--   0        0        0     7713 2024-02-08 09:18:49.125827 hezar-0.36.0/hezar/models/speech_recognition/whisper/whisper_feature_extractor.py
--rw-r--r--   0        0        0     6195 2024-02-08 09:18:49.125827 hezar-0.36.0/hezar/models/speech_recognition/whisper/whisper_speech_recognition.py
--rw-r--r--   0        0        0     1572 2024-02-08 09:18:49.125827 hezar-0.36.0/hezar/models/speech_recognition/whisper/whisper_speech_recognition_config.py
--rw-r--r--   0        0        0    26128 2024-02-08 09:18:49.125827 hezar-0.36.0/hezar/models/speech_recognition/whisper/whisper_tokenizer.py
--rw-r--r--   0        0        0       69 2024-02-08 09:18:49.125827 hezar-0.36.0/hezar/models/text_classification/__init__.py
--rw-r--r--   0        0        0      135 2024-02-08 09:18:49.125827 hezar-0.36.0/hezar/models/text_classification/bert/__init__.py
--rw-r--r--   0        0        0     4796 2024-02-08 09:18:49.125827 hezar-0.36.0/hezar/models/text_classification/bert/bert_text_classification.py
--rw-r--r--   0        0        0      845 2024-02-08 09:18:49.125827 hezar-0.36.0/hezar/models/text_classification/bert/bert_text_classification_config.py
--rw-r--r--   0        0        0      159 2024-02-08 09:18:49.125827 hezar-0.36.0/hezar/models/text_classification/distilbert/__init__.py
--rw-r--r--   0        0        0     4357 2024-02-08 09:18:49.125827 hezar-0.36.0/hezar/models/text_classification/distilbert/distilbert_text_classification.py
--rw-r--r--   0        0        0      748 2024-02-08 09:18:49.125827 hezar-0.36.0/hezar/models/text_classification/distilbert/distilbert_text_classification_config.py
--rw-r--r--   0        0        0      147 2024-02-08 09:18:49.125827 hezar-0.36.0/hezar/models/text_classification/roberta/__init__.py
--rw-r--r--   0        0        0     4963 2024-02-08 09:18:49.125827 hezar-0.36.0/hezar/models/text_classification/roberta/roberta_text_classification.py
--rw-r--r--   0        0        0      942 2024-02-08 09:18:49.125827 hezar-0.36.0/hezar/models/text_classification/roberta/roberta_text_classification_config.py
--rw-r--r--   0        0        0        0 2024-02-08 09:18:49.125827 hezar-0.36.0/hezar/models/text_embedding/__init__.py
--rw-r--r--   0        0        0       38 2024-02-08 09:18:49.125827 hezar-0.36.0/hezar/models/text_generation/__init__.py
--rw-r--r--   0        0        0      119 2024-02-08 09:18:49.125827 hezar-0.36.0/hezar/models/text_generation/gpt2/__init__.py
--rw-r--r--   0        0        0     3322 2024-02-08 09:18:49.125827 hezar-0.36.0/hezar/models/text_generation/gpt2/gpt2_text_generation.py
--rw-r--r--   0        0        0     1148 2024-02-08 09:18:49.125827 hezar-0.36.0/hezar/models/text_generation/gpt2/gpt2_text_generation_config.py
--rw-r--r--   0        0        0      111 2024-02-08 09:18:49.125827 hezar-0.36.0/hezar/models/text_generation/t5/__init__.py
--rw-r--r--   0        0        0     4051 2024-02-08 09:18:49.125827 hezar-0.36.0/hezar/models/text_generation/t5/t5_text_generation.py
--rw-r--r--   0        0        0      837 2024-02-08 09:18:49.125827 hezar-0.36.0/hezar/models/text_generation/t5/t5_text_generation_config.py
--rw-r--r--   0        0        0      390 2024-02-08 09:18:49.125827 hezar-0.36.0/hezar/preprocessors/__init__.py
--rw-r--r--   0        0        0    13309 2024-02-08 09:18:49.125827 hezar-0.36.0/hezar/preprocessors/audio_feature_extractor.py
--rw-r--r--   0        0        0     8292 2024-02-08 09:18:49.125827 hezar-0.36.0/hezar/preprocessors/image_processor.py
--rw-r--r--   0        0        0     5043 2024-02-08 09:18:49.125827 hezar-0.36.0/hezar/preprocessors/preprocessor.py
--rw-r--r--   0        0        0     4635 2024-02-08 09:18:49.125827 hezar-0.36.0/hezar/preprocessors/text_normalizer.py
--rw-r--r--   0        0        0      337 2024-02-08 09:18:49.125827 hezar-0.36.0/hezar/preprocessors/tokenizers/__init__.py
--rw-r--r--   0        0        0     3973 2024-02-08 09:18:49.125827 hezar-0.36.0/hezar/preprocessors/tokenizers/bpe.py
--rw-r--r--   0        0        0     4181 2024-02-08 09:18:49.125827 hezar-0.36.0/hezar/preprocessors/tokenizers/sentencepiece_bpe.py
--rw-r--r--   0        0        0     4102 2024-02-08 09:18:49.125827 hezar-0.36.0/hezar/preprocessors/tokenizers/sentencepiece_unigram.py
--rw-r--r--   0        0        0    27637 2024-02-08 09:18:49.125827 hezar-0.36.0/hezar/preprocessors/tokenizers/tokenizer.py
--rw-r--r--   0        0        0     3537 2024-02-08 09:18:49.125827 hezar-0.36.0/hezar/preprocessors/tokenizers/wordpiece.py
--rw-r--r--   0        0        0     6584 2024-02-08 09:18:49.125827 hezar-0.36.0/hezar/registry.py
--rw-r--r--   0        0        0      113 2024-02-08 09:18:49.125827 hezar-0.36.0/hezar/trainer/__init__.py
--rw-r--r--   0        0        0     7097 2024-02-08 09:18:49.125827 hezar-0.36.0/hezar/trainer/metrics_handlers.py
--rw-r--r--   0        0        0    30236 2024-02-08 09:18:49.125827 hezar-0.36.0/hezar/trainer/trainer.py
--rw-r--r--   0        0        0     4963 2024-02-08 09:18:49.125827 hezar-0.36.0/hezar/trainer/trainer_utils.py
--rw-r--r--   0        0        0      245 2024-02-08 09:18:49.125827 hezar-0.36.0/hezar/utils/__init__.py
--rw-r--r--   0        0        0    23979 2024-02-08 09:18:49.125827 hezar-0.36.0/hezar/utils/audio_utils.py
--rw-r--r--   0        0        0     3955 2024-02-08 09:18:49.125827 hezar-0.36.0/hezar/utils/common_utils.py
--rw-r--r--   0        0        0     6884 2024-02-08 09:18:49.125827 hezar-0.36.0/hezar/utils/data_utils.py
--rw-r--r--   0        0        0      976 2024-02-08 09:18:49.125827 hezar-0.36.0/hezar/utils/file_utils.py
--rw-r--r--   0        0        0     4982 2024-02-08 09:18:49.125827 hezar-0.36.0/hezar/utils/hub_utils.py
--rw-r--r--   0        0        0     7352 2024-02-08 09:18:49.125827 hezar-0.36.0/hezar/utils/image_utils.py
--rw-r--r--   0        0        0     1376 2024-02-08 09:18:49.125827 hezar-0.36.0/hezar/utils/integration_utils.py
--rw-r--r--   0        0        0      622 2024-02-08 09:18:49.125827 hezar-0.36.0/hezar/utils/logging.py
--rw-r--r--   0        0        0     4498 2024-02-08 09:18:49.125827 hezar-0.36.0/hezar/utils/registry_utils.py
--rw-r--r--   0        0        0     2572 2024-02-08 09:18:49.125827 hezar-0.36.0/pyproject.toml
--rw-r--r--   0        0        0    16785 1970-01-01 00:00:00.000000 hezar-0.36.0/PKG-INFO
+-rw-r--r--   0        0        0    11337 2024-04-25 07:35:04.374585 hezar-0.36.1/LICENSE
+-rw-r--r--   0        0        0    14442 2024-04-25 07:35:04.374585 hezar-0.36.1/README.md
+-rw-r--r--   0        0        0      623 2024-04-25 07:35:04.378585 hezar-0.36.1/hezar/__init__.py
+-rw-r--r--   0        0        0     5651 2024-04-25 07:35:04.378585 hezar-0.36.1/hezar/builders.py
+-rw-r--r--   0        0        0    16908 2024-04-25 07:35:04.378585 hezar-0.36.1/hezar/configs.py
+-rw-r--r--   0        0        0     4712 2024-04-25 07:35:04.378585 hezar-0.36.1/hezar/constants.py
+-rw-r--r--   0        0        0       54 2024-04-25 07:35:04.378585 hezar-0.36.1/hezar/data/__init__.py
+-rw-r--r--   0        0        0    13746 2024-04-25 07:35:04.378585 hezar-0.36.1/hezar/data/data_collators.py
+-rw-r--r--   0        0        0      634 2024-04-25 07:35:04.378585 hezar-0.36.1/hezar/data/datasets/__init__.py
+-rw-r--r--   0        0        0     3279 2024-04-25 07:35:04.378585 hezar-0.36.1/hezar/data/datasets/dataset.py
+-rw-r--r--   0        0        0     3727 2024-04-25 07:35:04.378585 hezar-0.36.1/hezar/data/datasets/image_captioning_dataset.py
+-rw-r--r--   0        0        0     7384 2024-04-25 07:35:04.378585 hezar-0.36.1/hezar/data/datasets/ocr_dataset.py
+-rw-r--r--   0        0        0     5923 2024-04-25 07:35:04.378585 hezar-0.36.1/hezar/data/datasets/sequence_labeling_dataset.py
+-rw-r--r--   0        0        0     3030 2024-04-25 07:35:04.378585 hezar-0.36.1/hezar/data/datasets/speech_recognition_dataset.py
+-rw-r--r--   0        0        0     4498 2024-04-25 07:35:04.378585 hezar-0.36.1/hezar/data/datasets/text_classification_dataset.py
+-rw-r--r--   0        0        0     4820 2024-04-25 07:35:04.378585 hezar-0.36.1/hezar/data/datasets/text_summarization_dataset.py
+-rw-r--r--   0        0        0      202 2024-04-25 07:35:04.378585 hezar-0.36.1/hezar/embeddings/__init__.py
+-rw-r--r--   0        0        0    11544 2024-04-25 07:35:04.378585 hezar-0.36.1/hezar/embeddings/embedding.py
+-rw-r--r--   0        0        0     7171 2024-04-25 07:35:04.378585 hezar-0.36.1/hezar/embeddings/fasttext.py
+-rw-r--r--   0        0        0     7668 2024-04-25 07:35:04.378585 hezar-0.36.1/hezar/embeddings/word2vec.py
+-rw-r--r--   0        0        0      444 2024-04-25 07:35:04.378585 hezar-0.36.1/hezar/metrics/__init__.py
+-rw-r--r--   0        0        0     2285 2024-04-25 07:35:04.378585 hezar-0.36.1/hezar/metrics/accuracy.py
+-rw-r--r--   0        0        0     2484 2024-04-25 07:35:04.378585 hezar-0.36.1/hezar/metrics/bleu.py
+-rw-r--r--   0        0        0     3711 2024-04-25 07:35:04.378585 hezar-0.36.1/hezar/metrics/cer.py
+-rw-r--r--   0        0        0     3209 2024-04-25 07:35:04.378585 hezar-0.36.1/hezar/metrics/f1.py
+-rw-r--r--   0        0        0     1302 2024-04-25 07:35:04.378585 hezar-0.36.1/hezar/metrics/metric.py
+-rw-r--r--   0        0        0     3566 2024-04-25 07:35:04.378585 hezar-0.36.1/hezar/metrics/precision.py
+-rw-r--r--   0        0        0     3509 2024-04-25 07:35:04.378585 hezar-0.36.1/hezar/metrics/recall.py
+-rw-r--r--   0        0        0     3155 2024-04-25 07:35:04.378585 hezar-0.36.1/hezar/metrics/rouge.py
+-rw-r--r--   0        0        0     4029 2024-04-25 07:35:04.378585 hezar-0.36.1/hezar/metrics/seqeval.py
+-rw-r--r--   0        0        0     2950 2024-04-25 07:35:04.378585 hezar-0.36.1/hezar/metrics/wer.py
+-rw-r--r--   0        0        0      333 2024-04-25 07:35:04.378585 hezar-0.36.1/hezar/models/__init__.py
+-rw-r--r--   0        0        0       88 2024-04-25 07:35:04.378585 hezar-0.36.1/hezar/models/backbone/__init__.py
+-rw-r--r--   0        0        0       35 2024-04-25 07:35:04.378585 hezar-0.36.1/hezar/models/backbone/bert/__init__.py
+-rw-r--r--   0        0        0     2787 2024-04-25 07:35:04.378585 hezar-0.36.1/hezar/models/backbone/bert/bert.py
+-rw-r--r--   0        0        0      743 2024-04-25 07:35:04.378585 hezar-0.36.1/hezar/models/backbone/bert/bert_config.py
+-rw-r--r--   0        0        0       53 2024-04-25 07:35:04.378585 hezar-0.36.1/hezar/models/backbone/distilbert/__init__.py
+-rw-r--r--   0        0        0     2288 2024-04-25 07:35:04.378585 hezar-0.36.1/hezar/models/backbone/distilbert/distilbert.py
+-rw-r--r--   0        0        0      618 2024-04-25 07:35:04.378585 hezar-0.36.1/hezar/models/backbone/distilbert/distilbert_config.py
+-rw-r--r--   0        0        0       44 2024-04-25 07:35:04.378585 hezar-0.36.1/hezar/models/backbone/roberta/__init__.py
+-rw-r--r--   0        0        0     2788 2024-04-25 07:35:04.378585 hezar-0.36.1/hezar/models/backbone/roberta/roberta.py
+-rw-r--r--   0        0        0      812 2024-04-25 07:35:04.378585 hezar-0.36.1/hezar/models/backbone/roberta/roberta_config.py
+-rw-r--r--   0        0        0       55 2024-04-25 07:35:04.378585 hezar-0.36.1/hezar/models/backbone/vit/__init__.py
+-rw-r--r--   0        0        0     2172 2024-04-25 07:35:04.378585 hezar-0.36.1/hezar/models/backbone/vit/vit.py
+-rw-r--r--   0        0        0      572 2024-04-25 07:35:04.378585 hezar-0.36.1/hezar/models/backbone/vit/vit_config.py
+-rw-r--r--   0        0        0      120 2024-04-25 07:35:04.378585 hezar-0.36.1/hezar/models/image2text/__init__.py
+-rw-r--r--   0        0        0      131 2024-04-25 07:35:04.378585 hezar-0.36.1/hezar/models/image2text/beit_roberta/__init__.py
+-rw-r--r--   0        0        0     3493 2024-04-25 07:35:04.378585 hezar-0.36.1/hezar/models/image2text/beit_roberta/beit_roberta_image2text.py
+-rw-r--r--   0        0        0     2376 2024-04-25 07:35:04.378585 hezar-0.36.1/hezar/models/image2text/beit_roberta/beit_roberta_image2text_config.py
+-rw-r--r--   0        0        0      101 2024-04-25 07:35:04.378585 hezar-0.36.1/hezar/models/image2text/crnn/__init__.py
+-rw-r--r--   0        0        0     1106 2024-04-25 07:35:04.378585 hezar-0.36.1/hezar/models/image2text/crnn/crnn_decode_utils.py
+-rw-r--r--   0        0        0     4649 2024-04-25 07:35:04.378585 hezar-0.36.1/hezar/models/image2text/crnn/crnn_image2text.py
+-rw-r--r--   0        0        0      478 2024-04-25 07:35:04.378585 hezar-0.36.1/hezar/models/image2text/crnn/crnn_image2text_config.py
+-rw-r--r--   0        0        0      105 2024-04-25 07:35:04.378585 hezar-0.36.1/hezar/models/image2text/trocr/__init__.py
+-rw-r--r--   0        0        0     3430 2024-04-25 07:35:04.378585 hezar-0.36.1/hezar/models/image2text/trocr/trocr_image2text.py
+-rw-r--r--   0        0        0     1899 2024-04-25 07:35:04.378585 hezar-0.36.1/hezar/models/image2text/trocr/trocr_image2text_config.py
+-rw-r--r--   0        0        0      115 2024-04-25 07:35:04.378585 hezar-0.36.1/hezar/models/image2text/vit_gpt2/__init__.py
+-rw-r--r--   0        0        0     3463 2024-04-25 07:35:04.378585 hezar-0.36.1/hezar/models/image2text/vit_gpt2/vit_gpt2_image2text.py
+-rw-r--r--   0        0        0     1872 2024-04-25 07:35:04.378585 hezar-0.36.1/hezar/models/image2text/vit_gpt2/vit_gpt2_image2text_config.py
+-rw-r--r--   0        0        0      127 2024-04-25 07:35:04.378585 hezar-0.36.1/hezar/models/image2text/vit_roberta/__init__.py
+-rw-r--r--   0        0        0     3864 2024-04-25 07:35:04.378585 hezar-0.36.1/hezar/models/image2text/vit_roberta/vit_roberta_image2text.py
+-rw-r--r--   0        0        0     1952 2024-04-25 07:35:04.378585 hezar-0.36.1/hezar/models/image2text/vit_roberta/vit_roberta_image2text_config.py
+-rw-r--r--   0        0        0       69 2024-04-25 07:35:04.378585 hezar-0.36.1/hezar/models/mask_filling/__init__.py
+-rw-r--r--   0        0        0      107 2024-04-25 07:35:04.378585 hezar-0.36.1/hezar/models/mask_filling/bert/__init__.py
+-rw-r--r--   0        0        0     4320 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/models/mask_filling/bert/bert_mask_filling.py
+-rw-r--r--   0        0        0      771 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/models/mask_filling/bert/bert_mask_filling_config.py
+-rw-r--r--   0        0        0      131 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/models/mask_filling/distilbert/__init__.py
+-rw-r--r--   0        0        0     3921 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/models/mask_filling/distilbert/distilbert_mask_filling.py
+-rw-r--r--   0        0        0      637 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/models/mask_filling/distilbert/distilbert_mask_filling_config.py
+-rw-r--r--   0        0        0      119 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/models/mask_filling/roberta/__init__.py
+-rw-r--r--   0        0        0     4384 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/models/mask_filling/roberta/roberta_mask_filling.py
+-rw-r--r--   0        0        0      831 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/models/mask_filling/roberta/roberta_mask_filling_config.py
+-rw-r--r--   0        0        0    20158 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/models/model.py
+-rw-r--r--   0        0        0     2141 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/models/model_outputs.py
+-rw-r--r--   0        0        0       69 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/models/sequence_labeling/__init__.py
+-rw-r--r--   0        0        0      127 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/models/sequence_labeling/bert/__init__.py
+-rw-r--r--   0        0        0     5118 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/models/sequence_labeling/bert/bert_sequence_labeling.py
+-rw-r--r--   0        0        0      931 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/models/sequence_labeling/bert/bert_sequence_labeling_config.py
+-rw-r--r--   0        0        0      151 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/models/sequence_labeling/distilbert/__init__.py
+-rw-r--r--   0        0        0     5172 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/models/sequence_labeling/distilbert/distilbert_sequence_labeling.py
+-rw-r--r--   0        0        0      872 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/models/sequence_labeling/distilbert/distilbert_sequence_labeling_config.py
+-rw-r--r--   0        0        0      139 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/models/sequence_labeling/roberta/__init__.py
+-rw-r--r--   0        0        0     5821 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/models/sequence_labeling/roberta/roberta_sequence_labeling.py
+-rw-r--r--   0        0        0     1025 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/models/sequence_labeling/roberta/roberta_sequence_labeling_config.py
+-rw-r--r--   0        0        0       23 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/models/speech_recognition/__init__.py
+-rw-r--r--   0        0        0      306 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/models/speech_recognition/whisper/__init__.py
+-rw-r--r--   0        0        0     7713 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/models/speech_recognition/whisper/whisper_feature_extractor.py
+-rw-r--r--   0        0        0     6197 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/models/speech_recognition/whisper/whisper_speech_recognition.py
+-rw-r--r--   0        0        0     1572 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/models/speech_recognition/whisper/whisper_speech_recognition_config.py
+-rw-r--r--   0        0        0    26128 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/models/speech_recognition/whisper/whisper_tokenizer.py
+-rw-r--r--   0        0        0       69 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/models/text_classification/__init__.py
+-rw-r--r--   0        0        0      135 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/models/text_classification/bert/__init__.py
+-rw-r--r--   0        0        0     4796 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/models/text_classification/bert/bert_text_classification.py
+-rw-r--r--   0        0        0      845 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/models/text_classification/bert/bert_text_classification_config.py
+-rw-r--r--   0        0        0      159 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/models/text_classification/distilbert/__init__.py
+-rw-r--r--   0        0        0     4357 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/models/text_classification/distilbert/distilbert_text_classification.py
+-rw-r--r--   0        0        0      748 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/models/text_classification/distilbert/distilbert_text_classification_config.py
+-rw-r--r--   0        0        0      147 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/models/text_classification/roberta/__init__.py
+-rw-r--r--   0        0        0     4963 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/models/text_classification/roberta/roberta_text_classification.py
+-rw-r--r--   0        0        0      942 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/models/text_classification/roberta/roberta_text_classification_config.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/models/text_embedding/__init__.py
+-rw-r--r--   0        0        0       38 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/models/text_generation/__init__.py
+-rw-r--r--   0        0        0      119 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/models/text_generation/gpt2/__init__.py
+-rw-r--r--   0        0        0     3324 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/models/text_generation/gpt2/gpt2_text_generation.py
+-rw-r--r--   0        0        0     1148 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/models/text_generation/gpt2/gpt2_text_generation_config.py
+-rw-r--r--   0        0        0      111 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/models/text_generation/t5/__init__.py
+-rw-r--r--   0        0        0     4053 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/models/text_generation/t5/t5_text_generation.py
+-rw-r--r--   0        0        0      837 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/models/text_generation/t5/t5_text_generation_config.py
+-rw-r--r--   0        0        0      390 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/preprocessors/__init__.py
+-rw-r--r--   0        0        0    13309 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/preprocessors/audio_feature_extractor.py
+-rw-r--r--   0        0        0     8292 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/preprocessors/image_processor.py
+-rw-r--r--   0        0        0     5043 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/preprocessors/preprocessor.py
+-rw-r--r--   0        0        0     4635 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/preprocessors/text_normalizer.py
+-rw-r--r--   0        0        0      337 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/preprocessors/tokenizers/__init__.py
+-rw-r--r--   0        0        0     3973 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/preprocessors/tokenizers/bpe.py
+-rw-r--r--   0        0        0     4181 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/preprocessors/tokenizers/sentencepiece_bpe.py
+-rw-r--r--   0        0        0     4102 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/preprocessors/tokenizers/sentencepiece_unigram.py
+-rw-r--r--   0        0        0    27637 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/preprocessors/tokenizers/tokenizer.py
+-rw-r--r--   0        0        0     3537 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/preprocessors/tokenizers/wordpiece.py
+-rw-r--r--   0        0        0     6584 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/registry.py
+-rw-r--r--   0        0        0      113 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/trainer/__init__.py
+-rw-r--r--   0        0        0     7097 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/trainer/metrics_handlers.py
+-rw-r--r--   0        0        0    30740 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/trainer/trainer.py
+-rw-r--r--   0        0        0     4963 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/trainer/trainer_utils.py
+-rw-r--r--   0        0        0      245 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/utils/__init__.py
+-rw-r--r--   0        0        0    23979 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/utils/audio_utils.py
+-rw-r--r--   0        0        0     3955 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/utils/common_utils.py
+-rw-r--r--   0        0        0     6884 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/utils/data_utils.py
+-rw-r--r--   0        0        0      976 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/utils/file_utils.py
+-rw-r--r--   0        0        0     4903 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/utils/hub_utils.py
+-rw-r--r--   0        0        0     7352 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/utils/image_utils.py
+-rw-r--r--   0        0        0     1376 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/utils/integration_utils.py
+-rw-r--r--   0        0        0      622 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/utils/logging.py
+-rw-r--r--   0        0        0     4498 2024-04-25 07:35:04.382585 hezar-0.36.1/hezar/utils/registry_utils.py
+-rw-r--r--   0        0        0     2632 2024-04-25 07:35:04.386585 hezar-0.36.1/pyproject.toml
+-rw-r--r--   0        0        0    17058 1970-01-01 00:00:00.000000 hezar-0.36.1/PKG-INFO
```

### Comparing `hezar-0.36.0/LICENSE` & `hezar-0.36.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hezar-0.36.0/README.md` & `hezar-0.36.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -214,14 +214,16 @@
 ```python
 from hezar.data import Dataset
 
 sentiment_dataset = Dataset.load("hezarai/sentiment-dksf")  # A TextClassificationDataset instance
 lscp_dataset = Dataset.load("hezarai/lscp-pos-500k")  # A SequenceLabelingDataset instance
 xlsum_dataset = Dataset.load("hezarai/xlsum-fa")  # A TextSummarizationDataset instance
 alpr_ocr_dataset = Dataset.load("hezarai/persian-license-plate-v1")  # An OCRDataset instance
+flickr30k_dataset = Dataset.load("hezarai/flickr30k-fa")  # An ImageCaptioningDataset instance
+commonvoice_dataset = Dataset.load("hezarai/common-voice-13-fa")  # A SpeechRecognitionDataset instance
 ...
 ```
 The returned dataset objects from `load()` are PyTorch Dataset wrappers for specific tasks and can be used by a data loader out-of-the-box!
 
 You can also load Hezar's datasets using 🤗Datasets:
 ```python
 from datasets import load_dataset
```

### Comparing `hezar-0.36.0/hezar/__init__.py` & `hezar-0.36.1/hezar/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.36.0"
+__version__ = "0.36.1"
```

### Comparing `hezar-0.36.0/hezar/builders.py` & `hezar-0.36.1/hezar/builders.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.0/hezar/configs.py` & `hezar-0.36.1/hezar/configs.py`

 * *Files 0% similar despite different names*

```diff
@@ -419,14 +419,16 @@
     config_type: str = field(init=False, default=ConfigType.TRAINER)
     output_dir: str
     task: str | TaskType
     device: str = "cuda"
     num_epochs: int = None
     init_weights_from: str = None
     num_dataloader_workers: int = 0
+    dataloader_drop_last: bool = False
+    dataloader_shuffle: bool = True
     seed: int = 42
     optimizer: str | OptimizerType = None
     learning_rate: float = 2e-5
     weight_decay: float = 0.0
     lr_scheduler: str | LRSchedulerType = None
     lr_scheduler_kwargs: Dict[str, Any] = None
     batch_size: int = None
```

### Comparing `hezar-0.36.0/hezar/constants.py` & `hezar-0.36.1/hezar/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,14 @@
     WANDB = "wandb"
     GENSIM = "gensim"
     PILLOW = "PIL"
     JIWER = "jiwer"
     NLTK = "nltk"
     SCIKIT = "sklearn"
     SEQEVAL = "seqeval"
-    EVALUATE = "evaluate"
     ROUGE = "rouge_score"
 
 
 class TaskType(ExplicitEnum):
     AUDIO_CLASSIFICATION = "audio_classification"
     BACKBONE = "backbone"
     IMAGE2TEXT = "image2text"
```

### Comparing `hezar-0.36.0/hezar/data/data_collators.py` & `hezar-0.36.1/hezar/data/data_collators.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.0/hezar/data/datasets/__init__.py` & `hezar-0.36.1/hezar/data/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.0/hezar/data/datasets/dataset.py` & `hezar-0.36.1/hezar/data/datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.0/hezar/data/datasets/image_captioning_dataset.py` & `hezar-0.36.1/hezar/data/datasets/image_captioning_dataset.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.0/hezar/data/datasets/ocr_dataset.py` & `hezar-0.36.1/hezar/data/datasets/ocr_dataset.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.0/hezar/data/datasets/sequence_labeling_dataset.py` & `hezar-0.36.1/hezar/data/datasets/sequence_labeling_dataset.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.0/hezar/data/datasets/speech_recognition_dataset.py` & `hezar-0.36.1/hezar/data/datasets/speech_recognition_dataset.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.0/hezar/data/datasets/text_classification_dataset.py` & `hezar-0.36.1/hezar/data/datasets/text_classification_dataset.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.0/hezar/data/datasets/text_summarization_dataset.py` & `hezar-0.36.1/hezar/data/datasets/text_summarization_dataset.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.0/hezar/embeddings/embedding.py` & `hezar-0.36.1/hezar/embeddings/embedding.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.0/hezar/embeddings/fasttext.py` & `hezar-0.36.1/hezar/embeddings/fasttext.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.0/hezar/embeddings/word2vec.py` & `hezar-0.36.1/hezar/embeddings/word2vec.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.0/hezar/metrics/accuracy.py` & `hezar-0.36.1/hezar/metrics/accuracy.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.0/hezar/metrics/bleu.py` & `hezar-0.36.1/hezar/metrics/bleu.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.0/hezar/metrics/cer.py` & `hezar-0.36.1/hezar/metrics/cer.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.0/hezar/metrics/f1.py` & `hezar-0.36.1/hezar/metrics/f1.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.0/hezar/metrics/metric.py` & `hezar-0.36.1/hezar/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.0/hezar/metrics/precision.py` & `hezar-0.36.1/hezar/metrics/precision.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.0/hezar/metrics/recall.py` & `hezar-0.36.1/hezar/metrics/recall.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.0/hezar/metrics/rouge.py` & `hezar-0.36.1/hezar/metrics/rouge.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.0/hezar/metrics/seqeval.py` & `hezar-0.36.1/hezar/metrics/seqeval.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.0/hezar/metrics/wer.py` & `hezar-0.36.1/hezar/metrics/wer.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.0/hezar/models/backbone/bert/bert.py` & `hezar-0.36.1/hezar/models/backbone/bert/bert.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.0/hezar/models/backbone/bert/bert_config.py` & `hezar-0.36.1/hezar/models/backbone/bert/bert_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.0/hezar/models/backbone/distilbert/distilbert.py` & `hezar-0.36.1/hezar/models/backbone/distilbert/distilbert.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.0/hezar/models/backbone/distilbert/distilbert_config.py` & `hezar-0.36.1/hezar/models/backbone/distilbert/distilbert_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.0/hezar/models/backbone/roberta/roberta.py` & `hezar-0.36.1/hezar/models/backbone/roberta/roberta.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.0/hezar/models/backbone/roberta/roberta_config.py` & `hezar-0.36.1/hezar/models/backbone/roberta/roberta_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.0/hezar/models/backbone/vit/vit.py` & `hezar-0.36.1/hezar/models/backbone/vit/vit.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 _required_backends = [Backends.TRANSFORMERS, Backends.TOKENIZERS, Backends.PILLOW]
 
 
 @register_model("vit", config_class=ViTConfig)
 class ViT(Model):
     required_backends = _required_backends
     image_processor = "image_processor"
-    loss_fn_name = "cross_entropy"
+    loss_func_name = "cross_entropy"
 
     def __init__(self, config: ViTConfig, **kwargs):
         super().__init__(config=config, **kwargs)
         self.vit = ViTModel(ViTConfig_(**self.config))
 
     def forward(
         self,
```

### Comparing `hezar-0.36.0/hezar/models/backbone/vit/vit_config.py` & `hezar-0.36.1/hezar/models/backbone/vit/vit_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.0/hezar/models/image2text/beit_roberta/beit_roberta_image2text.py` & `hezar-0.36.1/hezar/models/image2text/beit_roberta/beit_roberta_image2text.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     BEiT + RoBERTa for image to text
     """
 
     is_generative = True
     required_backends = _required_backends
     image_processor = "image_processor"
     tokenizer_name = "bpe_tokenizer"
-    loss_fn_name = "cross_entropy"
+    loss_func_name = "cross_entropy"
 
     def __init__(self, config: BeitRobertaImage2TextConfig, **kwargs):
         super().__init__(config, **kwargs)
         encoder = BeitModel(config=BeitConfig(**self.config.encoder))
         decoder = RobertaForCausalLM(config=RobertaConfig(**self.config.decoder))
         self.beit_roberta = VisionEncoderDecoderModel(encoder=encoder, decoder=decoder)
 
@@ -72,15 +72,15 @@
             output_attentions=output_attentions,
             output_hidden_states=output_hidden_states,
         )
 
         return outputs
 
     def compute_loss(self, logits: torch.Tensor, labels: torch.Tensor) -> torch.Tensor:
-        loss = self.criterion(logits.reshape(-1, self.beit_roberta.decoder.config.vocab_size), labels.reshape(-1))
+        loss = self.loss_func(logits.reshape(-1, self.beit_roberta.decoder.config.vocab_size), labels.reshape(-1))
         return loss
 
     def generate(self, pixel_values, generation_config=None, **kwargs):
         if generation_config is None:
             generation_config = self.config.dict()["generation"]
         generation_config = GenerationConfig(**generation_config)
         outputs = self.beit_roberta.generate(inputs=pixel_values, generation_config=generation_config, **kwargs)
```

### Comparing `hezar-0.36.0/hezar/models/image2text/beit_roberta/beit_roberta_image2text_config.py` & `hezar-0.36.1/hezar/models/image2text/beit_roberta/beit_roberta_image2text_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.0/hezar/models/image2text/crnn/crnn_decode_utils.py` & `hezar-0.36.1/hezar/models/image2text/crnn/crnn_decode_utils.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.0/hezar/models/image2text/crnn/crnn_image2text.py` & `hezar-0.36.1/hezar/models/image2text/crnn/crnn_image2text.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 class CRNNImage2Text(Model):
     """
     A robust CRNN model for character level OCR based on the original paper.
     """
 
     is_generative = True
     image_processor = "image_processor"
-    loss_fn_name = "ctc"
-    loss_fn_kwargs = {"zero_infinity": True}
+    loss_func_name = "ctc"
+    loss_func_kwargs = {"zero_infinity": True}
 
     def __init__(self, config: CRNNImage2TextConfig, **kwargs):
         super().__init__(config=config, **kwargs)
         self.cnn = nn.Sequential(
             ConvBlock(self.config.n_channels, 64, 3, 1, 1),
             nn.MaxPool2d(kernel_size=2, stride=2),
             ConvBlock(64, 128, 3, 1, 1),
@@ -60,15 +60,15 @@
 
     def compute_loss(self, logits: torch.Tensor, labels: torch.Tensor):
         batch_size = logits.size(1)
         labels_lengths = torch.count_nonzero(labels, dim=1).flatten()
         labels = labels[labels != self.config.blank_id]
         input_lengths = torch.LongTensor([logits.size(0)] * batch_size)
 
-        loss = self.criterion(logits, labels, input_lengths, labels_lengths)
+        loss = self.loss_func(logits, labels, input_lengths, labels_lengths)
 
         return loss
 
     def generate(self, pixel_values):
         logits = self(pixel_values)["logits"]
         output_ids = ctc_decode(logits, blank=self.config.blank_id)
         probs, values = logits.permute(1, 0, 2).softmax(2).max(2)
```

### Comparing `hezar-0.36.0/hezar/models/image2text/trocr/trocr_image2text.py` & `hezar-0.36.1/hezar/models/image2text/trocr/trocr_image2text.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     TrOCR for optical character recognition
     """
 
     is_generative = True
     required_backends = _required_backends
     image_processor = "image_processor"
     tokenizer_name = "bpe_tokenizer"
-    loss_fn_name = "cross_entropy"
+    loss_func_name = "cross_entropy"
 
     def __init__(self, config: TrOCRImage2TextConfig, **kwargs):
         super().__init__(config, **kwargs)
         encoder = ViTModel(config=ViTConfig(**self.config.encoder))
         decoder = RobertaForCausalLM(config=RobertaConfig(**self.config.decoder))
         self.trocr = VisionEncoderDecoderModel(encoder=encoder, decoder=decoder)
 
@@ -72,15 +72,15 @@
             output_attentions=output_attentions,
             output_hidden_states=output_hidden_states,
         )
 
         return outputs
 
     def compute_loss(self, logits: torch.Tensor, labels: torch.Tensor) -> torch.Tensor:
-        loss = self.criterion(logits.reshape(-1, self.trocr.decoder.config.vocab_size), labels.reshape(-1))
+        loss = self.loss_func(logits.reshape(-1, self.trocr.decoder.config.vocab_size), labels.reshape(-1))
         return loss
 
     def generate(self, pixel_values, generation_config=None, **kwargs):
         if generation_config is None:
             generation_config = self.config.dict()["generation"]
         generation_config = GenerationConfig(**generation_config)
         outputs = self.trocr.generate(inputs=pixel_values, generation_config=generation_config, **kwargs)
```

### Comparing `hezar-0.36.0/hezar/models/image2text/trocr/trocr_image2text_config.py` & `hezar-0.36.1/hezar/models/image2text/trocr/trocr_image2text_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.0/hezar/models/image2text/vit_gpt2/vit_gpt2_image2text.py` & `hezar-0.36.1/hezar/models/image2text/vit_gpt2/vit_gpt2_image2text.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     ViT + GPT2 for image to text generation (image captioning)
     """
 
     is_generative = True
     required_backends = _required_backends
     image_processor = "image_processor"
     tokenizer_name = "bpe_tokenizer"
-    loss_fn_name = "cross_entropy"
+    loss_func_name = "cross_entropy"
 
     def __init__(self, config: ViTGPT2Image2TextConfig, **kwargs):
         super().__init__(config, **kwargs)
         encoder = ViTModel(config=ViTConfig(**self.config.encoder))
         decoder = GPT2LMHeadModel(config=GPT2Config(**self.config.decoder))
         self.vit_gpt2 = VisionEncoderDecoderModel(encoder=encoder, decoder=decoder)
 
@@ -72,15 +72,15 @@
             output_attentions=output_attentions,
             output_hidden_states=output_hidden_states,
         )
 
         return outputs
 
     def compute_loss(self, logits: torch.Tensor, labels: torch.Tensor) -> torch.Tensor:
-        loss = self.criterion(logits.reshape(-1, self.vit_gpt2.decoder.config.vocab_size), labels.reshape(-1))
+        loss = self.loss_func(logits.reshape(-1, self.vit_gpt2.decoder.config.vocab_size), labels.reshape(-1))
         return loss
 
     def generate(self, pixel_values, generation_config=None, **kwargs):
         if generation_config is None:
             generation_config = self.config.dict()["generation"]
         generation_config = GenerationConfig(**generation_config)
         outputs = self.vit_gpt2.generate(inputs=pixel_values, generation_config=generation_config, **kwargs)
```

### Comparing `hezar-0.36.0/hezar/models/image2text/vit_gpt2/vit_gpt2_image2text_config.py` & `hezar-0.36.1/hezar/models/image2text/vit_gpt2/vit_gpt2_image2text_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.0/hezar/models/image2text/vit_roberta/vit_roberta_image2text.py` & `hezar-0.36.1/hezar/models/image2text/vit_roberta/vit_roberta_image2text.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     ViT + RoBERTa for image to text
     """
 
     is_generative = True
     required_backends = _required_backends
     image_processor = "image_processor"
     tokenizer_name = "bpe_tokenizer"
-    loss_fn_name = "cross_entropy"
+    loss_func_name = "cross_entropy"
 
     def __init__(self, config: ViTRobertaImage2TextConfig, **kwargs):
         super().__init__(config, **kwargs)
         encoder = ViTModel(config=ViTConfig(**self.config.encoder))
         decoder = RobertaForCausalLM(config=RobertaConfig(**self.config.decoder))
         self.vit_roberta = VisionEncoderDecoderModel(encoder=encoder, decoder=decoder)
 
@@ -72,16 +72,16 @@
             output_attentions=output_attentions,
             output_hidden_states=output_hidden_states,
         )
 
         return dict(outputs)
 
     def compute_loss(self, logits: torch.Tensor, labels: torch.Tensor) -> torch.Tensor:
-        self.criterion.ignore_index = self.config.decoder["pad_token_id"]
-        loss = self.criterion(logits.reshape(-1, self.vit_roberta.decoder.config.vocab_size), labels.reshape(-1))
+        self.loss_func.ignore_index = self.config.decoder["pad_token_id"]
+        loss = self.loss_func(logits.reshape(-1, self.vit_roberta.decoder.config.vocab_size), labels.reshape(-1))
         return loss
 
     def generate(self, pixel_values, generation_config=None, **kwargs):
         tokenizer = self.preprocessor["bpe_tokenizer"]
         if generation_config is None:
             generation_config = self.config.dict()["generation"]
             generation_config["decoder_start_token_id"] = tokenizer.pad_token_id
```

### Comparing `hezar-0.36.0/hezar/models/image2text/vit_roberta/vit_roberta_image2text_config.py` & `hezar-0.36.1/hezar/models/image2text/vit_roberta/vit_roberta_image2text_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.0/hezar/models/mask_filling/bert/bert_mask_filling.py` & `hezar-0.36.1/hezar/models/mask_filling/bert/bert_mask_filling.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import torch
 
 from ....constants import Backends
 from ....models import Model
 from ....registry import register_model
 from ....utils import is_backend_available
-from ...model_outputs import LanguageModelingOutput
+from ...model_outputs import MaskFillingOutput
 from .bert_mask_filling_config import BertMaskFillingConfig
 
 
 if is_backend_available(Backends.TRANSFORMERS):
     from transformers import BertConfig, BertForMaskedLM
 
 _required_backends = [
@@ -22,15 +22,15 @@
 
 
 @register_model("bert_mask_filling", config_class=BertMaskFillingConfig)
 class BertMaskFilling(Model):
     required_backends = _required_backends
     tokenizer_name = "wordpiece_tokenizer"
     skip_keys_on_load = ["model.embeddings.position_ids", "bert.embeddings.position_ids"]  # For older versions
-    loss_fn_name = "cross_entropy"
+    loss_func_name = "cross_entropy"
 
     def __init__(self, config, **kwargs):
         super().__init__(config=config, **kwargs)
         self.bert_mask_filling = BertForMaskedLM(BertConfig(**self.config))
 
     def forward(
         self,
@@ -61,15 +61,15 @@
             return_dict=True,
         )
         outputs["token_ids"] = token_ids  # needed for post-process
 
         return outputs
 
     def compute_loss(self, logits: torch.Tensor, labels: torch.Tensor) -> torch.Tensor:
-        loss = self.criterion(logits.view(-1, self.config.vocab_size), labels.view(-1))
+        loss = self.loss_func(logits.view(-1, self.config.vocab_size), labels.view(-1))
         return loss
 
     def preprocess(self, inputs: str | List[str], **kwargs):
         if isinstance(inputs, str):
             inputs = [inputs]
 
         tokenizer = self.preprocessor[self.tokenizer_name]
@@ -104,15 +104,15 @@
                 top_fill_token_ids = top_fill_token_ids.squeeze()
 
             row = []
             for i, (prob, token_id) in enumerate(zip(probs, top_fill_token_ids)):
                 candidate = unfilled_token_ids[batch_i].copy()
                 candidate[masked_index.item()] = token_id
                 row.append(
-                    LanguageModelingOutput(
+                    MaskFillingOutput(
                         token=tokenizer.decode([token_id.item()])[0].strip(),
                         sequence=tokenizer.decode(candidate.tolist())[0],
                         token_id=token_id.item(),
                         score=prob.item(),
                     )
                 )
             outputs.append(row)
```

### Comparing `hezar-0.36.0/hezar/models/mask_filling/bert/bert_mask_filling_config.py` & `hezar-0.36.1/hezar/models/mask_filling/bert/bert_mask_filling_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.0/hezar/models/mask_filling/distilbert/distilbert_mask_filling.py` & `hezar-0.36.1/hezar/models/mask_filling/distilbert/distilbert_mask_filling.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import torch
 
 from ....constants import Backends
 from ....models import Model
 from ....registry import register_model
 from ....utils import is_backend_available
-from ...model_outputs import LanguageModelingOutput
+from ...model_outputs import MaskFillingOutput
 from .distilbert_mask_filling_config import DistilBertMaskFillingConfig
 
 
 if is_backend_available(Backends.TRANSFORMERS):
     from transformers import DistilBertConfig, DistilBertForMaskedLM
 
 _required_backends = [
@@ -21,15 +21,15 @@
 ]
 
 
 @register_model("distilbert_mask_filling", config_class=DistilBertMaskFillingConfig)
 class DistilBertMaskFilling(Model):
     required_backends = _required_backends
     tokenizer_name = "wordpiece_tokenizer"
-    loss_fn_name = "cross_entropy"
+    loss_func_name = "cross_entropy"
 
     def __init__(self, config, **kwargs):
         super().__init__(config=config, **kwargs)
         self.distilbert_mask_filling = DistilBertForMaskedLM(DistilBertConfig(**self.config))
 
     def forward(
         self,
@@ -53,15 +53,15 @@
         )
 
         outputs["token_ids"] = token_ids
 
         return outputs
 
     def compute_loss(self, logits: torch.Tensor, labels: torch.Tensor) -> torch.Tensor:
-        loss = self.criterion(logits.view(-1, self.config.vocab_size), labels.view(-1))
+        loss = self.loss_func(logits.view(-1, self.config.vocab_size), labels.view(-1))
         return loss
 
     def preprocess(self, inputs: str | List[str], **kwargs):
         if isinstance(inputs, str):
             inputs = [inputs]
 
         tokenizer = self.preprocessor[self.tokenizer_name]
@@ -96,15 +96,15 @@
                 top_fill_token_ids = top_fill_token_ids.squeeze()
 
             row = []
             for i, (prob, token_id) in enumerate(zip(probs, top_fill_token_ids)):
                 candidate = unfilled_token_ids[batch_i].copy()
                 candidate[masked_index.item()] = token_id
                 row.append(
-                    LanguageModelingOutput(
+                    MaskFillingOutput(
                         token=tokenizer.decode([token_id.item()])[0].strip(),
                         sequence=tokenizer.decode(candidate.tolist())[0],
                         token_id=token_id.item(),
                         score=prob.item(),
                     )
                 )
             outputs.append(row)
```

### Comparing `hezar-0.36.0/hezar/models/mask_filling/distilbert/distilbert_mask_filling_config.py` & `hezar-0.36.1/hezar/models/mask_filling/distilbert/distilbert_mask_filling_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.0/hezar/models/mask_filling/roberta/roberta_mask_filling.py` & `hezar-0.36.1/hezar/models/mask_filling/roberta/roberta_mask_filling.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 import torch
 
 from ....constants import Backends
 from ....models import Model
 from ....registry import register_model
 from ....utils import is_backend_available
-from ...model_outputs import LanguageModelingOutput
+from ...model_outputs import MaskFillingOutput
 from .roberta_mask_filling_config import RobertaMaskFillingConfig
 
 
 if is_backend_available(Backends.TRANSFORMERS):
     from transformers import RobertaConfig, RobertaForMaskedLM
 
 _required_backends = [
@@ -25,15 +25,15 @@
 
 
 @register_model("roberta_mask_filling", config_class=RobertaMaskFillingConfig)
 class RobertaMaskFilling(Model):
     required_backends = _required_backends
     tokenizer_name = "bpe_tokenizer"
     skip_keys_on_load = ["model.embeddings.position_ids", "roberta.embeddings.position_ids"]  # For older versions
-    loss_fn_name = "cross_entropy"
+    loss_func_name = "cross_entropy"
 
     def __init__(self, config, **kwargs):
         super().__init__(config=config, **kwargs)
         self.roberta_mask_filling = RobertaForMaskedLM(RobertaConfig(**self.config))
 
     def forward(
         self,
@@ -63,15 +63,15 @@
             output_hidden_states=output_hidden_states,
         )
         outputs["token_ids"] = token_ids
 
         return outputs
 
     def compute_loss(self, logits: torch.Tensor, labels: torch.Tensor) -> torch.Tensor:
-        loss = self.criterion(logits.view(-1, self.config.vocab_size), labels.view(-1))
+        loss = self.loss_func(logits.view(-1, self.config.vocab_size), labels.view(-1))
         return loss
 
     def preprocess(self, inputs: str | List[str], **kwargs):
         if isinstance(inputs, str):
             inputs = [inputs]
 
         tokenizer = self.preprocessor[self.tokenizer_name]
@@ -106,15 +106,15 @@
                 top_fill_token_ids = top_fill_token_ids.squeeze()
 
             row = []
             for i, (prob, token_id) in enumerate(zip(probs, top_fill_token_ids)):
                 candidate = unfilled_token_ids[batch_i].copy()
                 candidate[masked_index.item()] = token_id
                 row.append(
-                    LanguageModelingOutput(
+                    MaskFillingOutput(
                         token=tokenizer.decode([token_id.item()])[0].strip(),
                         sequence=tokenizer.decode(candidate.tolist())[0],
                         token_id=token_id.item(),
                         score=prob.item(),
                     )
                 )
             outputs.append(row)
```

### Comparing `hezar-0.36.0/hezar/models/mask_filling/roberta/roberta_mask_filling_config.py` & `hezar-0.36.1/hezar/models/mask_filling/roberta/roberta_mask_filling_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.0/hezar/models/model.py` & `hezar-0.36.1/hezar/models/model.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 )
 from ..preprocessors import Preprocessor, PreprocessorsContainer
 from ..utils import Logger, get_module_class, sanitize_function_parameters, verify_dependencies
 
 
 logger = Logger(__name__)
 
-criterions_mapping = {
+losses_mapping = {
     LossType.L1: nn.L1Loss,
     LossType.NLL: nn.NLLLoss,
     LossType.NLL_2D: nn.NLLLoss2d,
     LossType.POISSON_NLL: nn.PoissonNLLLoss,
     LossType.GAUSSIAN_NLL: nn.GaussianNLLLoss,
     LossType.MSE: nn.MSELoss,
     LossType.BCE: nn.BCELoss,
@@ -66,35 +66,35 @@
     # Specify if the model is a generative model. If True, the model must also implement the `generate` method
     is_generative: bool = False
 
     # Keys to ignore on loading state dicts
     skip_keys_on_load = []
 
     # Loss function name
-    loss_fn_name: str | LossType = LossType.CROSS_ENTROPY
-    loss_fn_kwargs: Dict[str, Any] = {}
+    loss_func_name: str | LossType = LossType.CROSS_ENTROPY
+    loss_func_kwargs: Dict[str, Any] = {}
 
     def __init__(self, config: ModelConfig, *args, **kwargs):
         verify_dependencies(self, self.required_backends)
         super().__init__()
         self.config = config.update(kwargs)
         self._preprocessor = None
-        self._criterion = self._set_criterion(self.loss_fn_name, **self.loss_fn_kwargs)
+        self._loss_func = self._set_loss_func(self.loss_func_name, **self.loss_func_kwargs)
 
     def __repr__(self):
         representation = super().__repr__()
         pattern = r"\('?_criterion'?\): [^\)]+\)\s*"
         representation = re.sub(pattern, '', representation)
         return representation
 
     @staticmethod
-    def _set_criterion(loss_fn_name: str, **loss_fn_kwargs: Dict[str, Any]):
-        if loss_fn_name not in criterions_mapping:
-            raise ValueError(f"Invalid criterion name `{loss_fn_name}`. Available: {list(criterions_mapping.keys())}")
-        loss_fn = criterions_mapping[loss_fn_name](**loss_fn_kwargs)
+    def _set_loss_func(loss_func_name: str, **loss_fn_kwargs: Dict[str, Any]):
+        if loss_func_name not in losses_mapping:
+            raise ValueError(f"Invalid loss_func_name `{loss_func_name}`. Available: {list(losses_mapping.keys())}")
+        loss_fn = losses_mapping[loss_func_name](**loss_fn_kwargs)
         return loss_fn
 
     @classmethod
     def load(
         cls,
         hub_or_local_path: str | os.PathLike,
         load_locally: Optional[bool] = False,
@@ -473,23 +473,23 @@
     def device(self):
         """
         Get the model's device. This method is only safe when all weights of the model are on the same device.
         """
         return next(self.parameters()).device
 
     @property
-    def criterion(self):
-        return self._criterion
+    def loss_func(self):
+        return self._loss_func
 
-    @criterion.setter
-    def criterion(self, value):
+    @loss_func.setter
+    def loss_func(self, value):
         if isinstance(value, str):
-            self._criterion = self._set_criterion(value)
+            self._loss_func = self._set_loss_func(value)
         elif isinstance(value, nn.Module):
-            self._criterion = value
+            self._loss_func = value
         else:
             raise ValueError(f"Criterion value must be either a name or a PyTorch `nn.Module`, got {type(value)}!")
 
     @property
     def preprocessor(self) -> PreprocessorsContainer:
         return self._preprocessor
```

### Comparing `hezar-0.36.0/hezar/models/model_outputs.py` & `hezar-0.36.1/hezar/models/model_outputs.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         return list(self.dict().values())
 
     def items(self):
         return self.dict().items()
 
 
 @dataclass(repr=False)
-class LanguageModelingOutput(ModelOutput):
+class MaskFillingOutput(ModelOutput):
     token: Optional[int] = None
     sequence: Optional[str] = None
     token_id: Optional[str] = None
     score: Optional[float] = None
 
 
 @dataclass(repr=False)
```

### Comparing `hezar-0.36.0/hezar/models/sequence_labeling/bert/bert_sequence_labeling.py` & `hezar-0.36.1/hezar/models/sequence_labeling/bert/bert_sequence_labeling.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.0/hezar/models/sequence_labeling/bert/bert_sequence_labeling_config.py` & `hezar-0.36.1/hezar/models/sequence_labeling/bert/bert_sequence_labeling_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.0/hezar/models/sequence_labeling/distilbert/distilbert_sequence_labeling.py` & `hezar-0.36.1/hezar/models/sequence_labeling/distilbert/distilbert_sequence_labeling.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.0/hezar/models/sequence_labeling/distilbert/distilbert_sequence_labeling_config.py` & `hezar-0.36.1/hezar/models/sequence_labeling/distilbert/distilbert_sequence_labeling_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.0/hezar/models/sequence_labeling/roberta/roberta_sequence_labeling.py` & `hezar-0.36.1/hezar/models/sequence_labeling/roberta/roberta_sequence_labeling.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.0/hezar/models/sequence_labeling/roberta/roberta_sequence_labeling_config.py` & `hezar-0.36.1/hezar/models/sequence_labeling/roberta/roberta_sequence_labeling_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.0/hezar/models/speech_recognition/whisper/whisper_feature_extractor.py` & `hezar-0.36.1/hezar/models/speech_recognition/whisper/whisper_feature_extractor.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.0/hezar/models/speech_recognition/whisper/whisper_speech_recognition.py` & `hezar-0.36.1/hezar/models/speech_recognition/whisper/whisper_speech_recognition.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     Whisper model for automatic speech recognition
     """
 
     is_generative = True
     required_backends = _required_backends
     feature_extractor_name = "whisper_feature_extractor"
     tokenizer_name = "whisper_bpe_tokenizer"
-    loss_fn_name = "cross_entropy"
+    loss_func_name = "cross_entropy"
 
     def __init__(self, config: WhisperSpeechRecognitionConfig, **kwargs):
         super().__init__(config, **kwargs)
         self.whisper = WhisperForConditionalGeneration(WhisperConfig(**self.config))
 
     def forward(
         self,
@@ -80,15 +80,15 @@
         )
 
         return dict(outputs)
 
     def compute_loss(self, logits: torch.Tensor, labels: torch.Tensor) -> torch.Tensor:
         labels = copy.deepcopy(labels)
         labels[labels == self.config.pad_token_id] = -100
-        loss = self.criterion(logits.view(-1, self.config.vocab_size), labels.view(-1))
+        loss = self.loss_func(logits.view(-1, self.config.vocab_size), labels.view(-1))
         return loss
 
     def generate(
         self,
         input_features,
         forced_decoder_ids=None,
         generation_config=None,
```

### Comparing `hezar-0.36.0/hezar/models/speech_recognition/whisper/whisper_speech_recognition_config.py` & `hezar-0.36.1/hezar/models/speech_recognition/whisper/whisper_speech_recognition_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.0/hezar/models/speech_recognition/whisper/whisper_tokenizer.py` & `hezar-0.36.1/hezar/models/speech_recognition/whisper/whisper_tokenizer.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.0/hezar/models/text_classification/bert/bert_text_classification.py` & `hezar-0.36.1/hezar/models/text_classification/bert/bert_text_classification.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.0/hezar/models/text_classification/bert/bert_text_classification_config.py` & `hezar-0.36.1/hezar/models/text_classification/bert/bert_text_classification_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.0/hezar/models/text_classification/distilbert/distilbert_text_classification.py` & `hezar-0.36.1/hezar/models/text_classification/distilbert/distilbert_text_classification.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.0/hezar/models/text_classification/distilbert/distilbert_text_classification_config.py` & `hezar-0.36.1/hezar/models/text_classification/distilbert/distilbert_text_classification_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.0/hezar/models/text_classification/roberta/roberta_text_classification.py` & `hezar-0.36.1/hezar/models/text_classification/roberta/roberta_text_classification.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.0/hezar/models/text_classification/roberta/roberta_text_classification_config.py` & `hezar-0.36.1/hezar/models/text_classification/roberta/roberta_text_classification_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.0/hezar/models/text_generation/gpt2/gpt2_text_generation.py` & `hezar-0.36.1/hezar/models/text_generation/gpt2/gpt2_text_generation.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 
 @register_model("gpt2_text_generation", config_class=GPT2TextGenerationConfig)
 class GPT2TextGeneration(Model):
     is_generative = True
     tokenizer_name = "bpe_tokenizer"
     required_backends = _required_backends
-    loss_fn_name = "cross_entropy"
+    loss_func_name = "cross_entropy"
 
     def __init__(self, config: GPT2TextGenerationConfig, **kwargs):
         super().__init__(config, **kwargs)
         self.gpt2 = GPT2LMHeadModel(config=GPT2Config(**self.config))
 
     def forward(
         self,
@@ -70,15 +70,15 @@
 
     def compute_loss(self, logits: torch.Tensor, labels: torch.Tensor) -> torch.Tensor:
         labels = labels.to(logits.device)
         # Shift so that tokens < n predict n
         shift_logits = logits[..., :-1, :].contiguous()
         shift_labels = labels[..., 1:].contiguous()
         # Compute loss
-        loss = self.criterion(shift_logits.view(-1, shift_logits.size(-1)), shift_labels.view(-1))
+        loss = self.loss_func(shift_logits.view(-1, shift_logits.size(-1)), shift_labels.view(-1))
         return loss
 
     def generate(self, token_ids, **kwargs):
         self.config.generation.update(kwargs or {})
         generation_config = GenerationConfig(**self.config.generation)
         generated_ids = self.gpt2.generate(token_ids, generation_config=generation_config)
         return generated_ids
```

### Comparing `hezar-0.36.0/hezar/models/text_generation/gpt2/gpt2_text_generation_config.py` & `hezar-0.36.1/hezar/models/text_generation/gpt2/gpt2_text_generation_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.0/hezar/models/text_generation/t5/t5_text_generation.py` & `hezar-0.36.1/hezar/models/text_generation/t5/t5_text_generation.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     """
     T5 for text to text generation
     """
 
     is_generative = True
     required_backends = _required_backends
     tokenizer_name = "sentencepiece_unigram_tokenizer"
-    loss_fn_name = "cross_entropy"
+    loss_func_name = "cross_entropy"
 
     def __init__(self, config: T5TextGenerationConfig, **kwargs):
         super().__init__(config=config, **kwargs)
 
         self.t5 = T5ForConditionalGeneration(T5Config(**self.config))
 
     def forward(
@@ -83,15 +83,15 @@
 
     def _shift_right(self, input_ids):
         return self.t5._shift_right(input_ids)
 
     def compute_loss(self, logits: torch.Tensor, labels: torch.Tensor) -> torch.Tensor:
         labels = labels.clone()
         labels[labels == self.config.pad_token_id] = -100
-        loss = self.criterion(logits.view(-1, logits.size(-1)), labels.view(-1))
+        loss = self.loss_func(logits.view(-1, logits.size(-1)), labels.view(-1))
         return loss
 
     def generate(self, token_ids, attention_mask=None, **kwargs):
         # TODO Merge kwargs into generation config so users can control generation from kwargs
         model_inputs = {"input_ids": token_ids, "attention_mask": attention_mask}
         generation_kwargs = {"min_length": self.config.min_length, "max_length": self.config.max_length}
         output_ids = self.t5.generate(**model_inputs, **generation_kwargs)
```

### Comparing `hezar-0.36.0/hezar/models/text_generation/t5/t5_text_generation_config.py` & `hezar-0.36.1/hezar/models/text_generation/t5/t5_text_generation_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.0/hezar/preprocessors/audio_feature_extractor.py` & `hezar-0.36.1/hezar/preprocessors/audio_feature_extractor.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.0/hezar/preprocessors/image_processor.py` & `hezar-0.36.1/hezar/preprocessors/image_processor.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.0/hezar/preprocessors/preprocessor.py` & `hezar-0.36.1/hezar/preprocessors/preprocessor.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.0/hezar/preprocessors/text_normalizer.py` & `hezar-0.36.1/hezar/preprocessors/text_normalizer.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.0/hezar/preprocessors/tokenizers/bpe.py` & `hezar-0.36.1/hezar/preprocessors/tokenizers/bpe.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.0/hezar/preprocessors/tokenizers/sentencepiece_bpe.py` & `hezar-0.36.1/hezar/preprocessors/tokenizers/sentencepiece_bpe.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.0/hezar/preprocessors/tokenizers/sentencepiece_unigram.py` & `hezar-0.36.1/hezar/preprocessors/tokenizers/sentencepiece_unigram.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.0/hezar/preprocessors/tokenizers/tokenizer.py` & `hezar-0.36.1/hezar/preprocessors/tokenizers/tokenizer.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.0/hezar/preprocessors/tokenizers/wordpiece.py` & `hezar-0.36.1/hezar/preprocessors/tokenizers/wordpiece.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.0/hezar/registry.py` & `hezar-0.36.1/hezar/registry.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.0/hezar/trainer/metrics_handlers.py` & `hezar-0.36.1/hezar/trainer/metrics_handlers.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.0/hezar/trainer/trainer.py` & `hezar-0.36.1/hezar/trainer/trainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     LRSchedulerType,
     OptimizerType,
     TaskType,
 )
 from ..data.datasets import Dataset
 from ..models import Model
 from ..preprocessors import Preprocessor, PreprocessorsContainer
-from ..utils import Logger, colorize_text, is_backend_available, sanitize_function_parameters
+from ..utils import Logger, colorize_text, is_backend_available, sanitize_function_parameters, verify_dependencies
 
 if TYPE_CHECKING:
     from accelerate import Accelerator
 
 logger = Logger(__name__)
 
 optimizers = {
@@ -90,31 +90,35 @@
         accelerator (Accelerator) : Accelerator object for a customized distributed environment
     """
 
     trainer_subfolder = DEFAULT_TRAINER_SUBFOLDER
     trainer_config_file = DEFAULT_TRAINER_CONFIG_FILE
     trainer_csv_log_file = DEFAULT_TRAINER_CSV_LOG_FILE
     dataset_config_file = DEFAULT_DATASET_CONFIG_FILE
-    default_trainer_state_file = DEFAULT_TRAINER_STATE_FILE
+    trainer_state_file = DEFAULT_TRAINER_STATE_FILE
     default_optimizer = OptimizerType.ADAM
     default_lr_scheduler = None
+    _required_backends = []
 
     def __init__(
         self,
         model: Model = None,
         config: TrainerConfig = None,
         train_dataset: Dataset = None,
         eval_dataset: Dataset = None,
         data_collator: Callable = None,
         preprocessor: Preprocessor | PreprocessorsContainer = None,
         metrics_handler: MetricsHandler = None,
         optimizer: torch.optim.Optimizer = None,
         lr_scheduler=None,
         accelerator: "Accelerator" = None,
     ):
+        # Check if all required dependencies are installed
+        verify_dependencies(self._required_backends)
+
         self.config = config
         self.device = "cuda" if torch.cuda.is_available() and not self.config.use_cpu else "cpu"
 
         # Set determinism
         self._set_seed(self.config.seed)
 
         # Setup model and preprocessor(s)
@@ -206,27 +210,27 @@
         """
         if self.train_dataset is not None:
             train_dataloader = DataLoader(
                 dataset=self.train_dataset,
                 batch_size=self.config.batch_size,
                 collate_fn=self.data_collator,
                 num_workers=self.config.num_dataloader_workers,
-                drop_last=True,
-                shuffle=True,
+                drop_last=self.config.dataloader_drop_last,
+                shuffle=self.config.dataloader_shuffle,
             )
         else:
             raise ValueError("Cannot create train dataloader because `train_dataset` is not given!")
         if self.eval_dataset is not None:
             eval_dataloader = DataLoader(
                 dataset=self.eval_dataset,
                 batch_size=self.config.eval_batch_size or self.config.batch_size,
                 collate_fn=self.data_collator,
                 num_workers=self.config.num_dataloader_workers,
-                drop_last=True,
-                shuffle=True,
+                drop_last=self.config.dataloader_drop_last,
+                shuffle=self.config.dataloader_shuffle,
             )
         else:
             logger.warning(
                 "Cannot create eval dataloader because `eval_dataset` is not given to the Trainer! "
                 "Setting eval_dataloader to None..."
             )
             eval_dataloader = None
@@ -304,15 +308,15 @@
         Args:
             checkpoint: Path to checkpoint directory
             load_best: Whether to load the best checkpoint or not, if False, loads the latest checkpoint
         """
         if os.path.isdir(checkpoint) and load_best:
             logger.warning("The `load_best` parameter has no effect when `checkpoint` is a path!")
 
-        self.state = TrainerState.load(os.path.join(self.checkpoints_dir, self.default_trainer_state_file))
+        self.state = TrainerState.load(os.path.join(self.checkpoints_dir, self.trainer_state_file))
         if isinstance(checkpoint, bool):
             if load_best:
                 checkpoint = os.path.join(self.checkpoints_dir, str(self.state.best_checkpoint))
             else:
                 checkpoint = os.path.join(self.checkpoints_dir, str(self.state.epoch))
         if os.path.isdir(checkpoint):
             # Figure out the epoch number
@@ -340,15 +344,15 @@
         Load the CSV log file
         Args:
             logs_dir: Path to logs directory, defaults to self.config.logs_dir
 
         Returns:
             Logs dictionary
         """
-        logs_dir = logs_dir or self.config.logs_dir
+        logs_dir = logs_dir or self.logs_dir
         csv_path = os.path.join(logs_dir, self.trainer_csv_log_file)
         logs = pd.read_csv(csv_path)
         return logs.to_dict()
 
     def prepare_input_batch(self, input_batch) -> Dict[str, torch.Tensor]:
         """
         Every operation required to prepare the inputs for model forward like moving to device, permutations, etc.
@@ -673,15 +677,15 @@
         # Log to CSV
         self.csv_logger.write({**train_logs, **evaluation_logs}, step)
 
         # Save trainer state
         self.state.save(
             os.path.join(
                 self.checkpoints_dir,
-                self.default_trainer_state_file,
+                self.trainer_state_file,
             )
         )
 
     def save(
         self,
         path: str,
         config_filename=None,
@@ -705,15 +709,21 @@
         """
         config_filename = config_filename or self.trainer_config_file
         subfolder = subfolder or self.trainer_subfolder
         dataset_config_file = dataset_config_file or self.dataset_config_file
 
         self.config.save(path, filename=config_filename, subfolder=subfolder)
         self.model.save(path, filename=model_filename, config_filename=model_config_filename)
-        self.train_dataset.config.save(path, filename=dataset_config_file, subfolder=subfolder)
+        if isinstance(self.train_dataset, Dataset):
+            self.train_dataset.config.save(path, filename=dataset_config_file, subfolder=subfolder)
+        else:
+            logger.warning(
+                f"The dataset passed to the Trainer is not a `hezar.data.Dataset` instance so that no dataset config"
+                f" will be saved!"
+            )
 
     def push_to_hub(
         self,
         repo_id: str,
         config_filename: str = None,
         push_model: bool = True,
         push_logs: bool = True,
```

### Comparing `hezar-0.36.0/hezar/trainer/trainer_utils.py` & `hezar-0.36.1/hezar/trainer/trainer_utils.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.0/hezar/utils/audio_utils.py` & `hezar-0.36.1/hezar/utils/audio_utils.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.0/hezar/utils/common_utils.py` & `hezar-0.36.1/hezar/utils/common_utils.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.0/hezar/utils/data_utils.py` & `hezar-0.36.1/hezar/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.0/hezar/utils/file_utils.py` & `hezar-0.36.1/hezar/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.0/hezar/utils/hub_utils.py` & `hezar-0.36.1/hezar/utils/hub_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -111,26 +111,22 @@
 
     Returns:
         A list of all file names
     """
     if os.path.isdir(hub_or_local_path):
         files_itr = os.walk(hub_or_local_path)
         files = []
-        for r, d, f in files_itr:
-            if r == hub_or_local_path:
-                files.append(f)
-            else:
-                for x in f:
-                    files.append(f"{r.replace(f'{hub_or_local_path}/', '')}/{x}")
+        for root, dirs, files_ in files_itr:
+            for file in files_:
+                files.append(os.path.relpath(os.path.join(root, file), hub_or_local_path))
     else:
         files = HfApi().list_repo_files(hub_or_local_path, repo_type=str(RepoType.MODEL))
 
-    if subfolder is not None:
-        files = [x.replace(f"{subfolder}/", "") for x in files if subfolder in x]
-
+    if subfolder:
+        files = [os.path.relpath(f, subfolder) for f in files if subfolder in f]
     return files
 
 
 def get_state_dict_from_hub(hub_id, filename, subfolder=None):
     """
     Load a state dict from a repo on the HF Hub. Works on any repo no matter the library.
```

### Comparing `hezar-0.36.0/hezar/utils/image_utils.py` & `hezar-0.36.1/hezar/utils/image_utils.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.0/hezar/utils/integration_utils.py` & `hezar-0.36.1/hezar/utils/integration_utils.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.0/hezar/utils/logging.py` & `hezar-0.36.1/hezar/utils/logging.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.0/hezar/utils/registry_utils.py` & `hezar-0.36.1/hezar/utils/registry_utils.py`

 * *Files identical despite different names*

### Comparing `hezar-0.36.0/pyproject.toml` & `hezar-0.36.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "hezar"
-version = "0.36.0"
+version = "0.36.1"
 packages = [{ include = "hezar" }]
 description = "Hezar: The all-in-one AI library for Persian, supporting a wide variety of tasks and modalities!"
 license = "Apache-2.0"
 authors = ["Aryan Shekarlaban <arxyzan@gmail.com>"]
 maintainers = ["Aryan Shekarlaban <arxyzan@gmail.com>"]
 repository = "https://github.com/hezarai/hezar"
 homepage = "https://github.com/hezarai"
@@ -39,30 +39,31 @@
 tokenizers = ">=0.13.0"
 datasets = ">=2.9.0"
 huggingface_hub = ">=0.12.0"
 tensorboard = ">=2.10.0"
 scikit-learn = ">=1.0.0"
 accelerate = {version="*", optional=true}
 numpy = {version="1.24.*", optional=true}
+scipy = {version="1.11.4", optional=true}
 gensim = {version="4.3.2", optional=true}
 seqeval = {version=">=1.2.0", optional=true}
 jiwer = {version=">=3.*", optional=true}
 soundfile = {version=">=0.12.0", optional=true}
 librosa = {version=">=0.10.0", optional=true}
 pillow = {version=">=9.*,<=10.*", optional=true}
 nltk = {version=">=3.8.0", optional=true}
 rouge_score = {version="*", optional=true}
 
 [tool.poetry.extras]
 nlp = ["seqeval", "jiwer", "nltk", "rouge_score"]
 audio = ["soundfile", "librosa", "jiwer"]
 vision = ["pillow"]
-embeddings = ["gensim", "numpy"]
+embeddings = ["gensim", "numpy", "scipy"]
 dev = ["pytest", "ruff", "sphinx", "myst-parser", "furo", "sphinx-copybutton"]
-all = ["numpy", "gensim", "accelerate", "seqeval", "jiwer", "soundfile", "librosa", "pillow", "nltk", "rouge_score"]
+all = ["numpy", "gensim", "accelerate", "seqeval", "jiwer", "soundfile", "librosa", "pillow", "nltk", "rouge_score", "scipy"]
 
 [tool.black]
 line-length = 120
 target-version = ['py39', 'py310', 'py311']
 
 [tool.ruff]
 ignore = ["C901", "E501", "E741", "W605", "F403", "F405"]
```

### Comparing `hezar-0.36.0/PKG-INFO` & `hezar-0.36.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hezar
-Version: 0.36.0
+Version: 0.36.1
 Summary: Hezar: The all-in-one AI library for Persian, supporting a wide variety of tasks and modalities!
 Home-page: https://github.com/hezarai
 License: Apache-2.0
 Keywords: packaging,poetry
 Author: Aryan Shekarlaban
 Author-email: arxyzan@gmail.com
 Maintainer: Aryan Shekarlaban
@@ -40,14 +40,15 @@
 Requires-Dist: librosa (>=0.10.0) ; extra == "audio" or extra == "all"
 Requires-Dist: nltk (>=3.8.0) ; extra == "nlp" or extra == "all"
 Requires-Dist: numpy (==1.24.*) ; extra == "embeddings" or extra == "all"
 Requires-Dist: omegaconf (>=2.3.0)
 Requires-Dist: pillow (>=9,<=10) ; extra == "vision" or extra == "all"
 Requires-Dist: rouge_score ; extra == "nlp" or extra == "all"
 Requires-Dist: scikit-learn (>=1.0.0)
+Requires-Dist: scipy (==1.11.4) ; extra == "embeddings" or extra == "all"
 Requires-Dist: seqeval (>=1.2.0) ; extra == "nlp" or extra == "all"
 Requires-Dist: soundfile (>=0.12.0) ; extra == "audio" or extra == "all"
 Requires-Dist: tensorboard (>=2.10.0)
 Requires-Dist: tokenizers (>=0.13.0)
 Requires-Dist: torch (>=1.10.0)
 Requires-Dist: transformers (>=4.28.0)
 Project-URL: Documentation, https://hezarai.github.io/hezar/
@@ -270,14 +271,16 @@
 ```python
 from hezar.data import Dataset
 
 sentiment_dataset = Dataset.load("hezarai/sentiment-dksf")  # A TextClassificationDataset instance
 lscp_dataset = Dataset.load("hezarai/lscp-pos-500k")  # A SequenceLabelingDataset instance
 xlsum_dataset = Dataset.load("hezarai/xlsum-fa")  # A TextSummarizationDataset instance
 alpr_ocr_dataset = Dataset.load("hezarai/persian-license-plate-v1")  # An OCRDataset instance
+flickr30k_dataset = Dataset.load("hezarai/flickr30k-fa")  # An ImageCaptioningDataset instance
+commonvoice_dataset = Dataset.load("hezarai/common-voice-13-fa")  # A SpeechRecognitionDataset instance
 ...
 ```
 The returned dataset objects from `load()` are PyTorch Dataset wrappers for specific tasks and can be used by a data loader out-of-the-box!
 
 You can also load Hezar's datasets using 🤗Datasets:
 ```python
 from datasets import load_dataset
```


# Comparing `tmp/nyckel-0.4.7.tar.gz` & `tmp/nyckel-0.4.8.tar.gz`

## Comparing `nyckel-0.4.7.tar` & `nyckel-0.4.8.tar`

### file list

```diff
@@ -1,75 +1,75 @@
--rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 nyckel-0.4.7/mkdocs.yml
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 nyckel-0.4.7/requirements.txt
--rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 nyckel-0.4.7/.github/workflows/build.yml
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 nyckel-0.4.7/.github/workflows/docs.yml
--rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 nyckel-0.4.7/.github/workflows/test.yml
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 nyckel-0.4.7/.vscode/extensions.json
--rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 nyckel-0.4.7/.vscode/settings.json
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 nyckel-0.4.7/docs/copy_function.md
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 nyckel-0.4.7/docs/credentials.md
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 nyckel-0.4.7/docs/data_classes.md
--rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 nyckel-0.4.7/docs/delete_label.md
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 nyckel-0.4.7/docs/delete_samples.md
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 nyckel-0.4.7/docs/image_classification.md
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 nyckel-0.4.7/docs/image_tags.md
--rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 nyckel-0.4.7/docs/index.md
--rw-r--r--   0        0        0    15763 2020-02-02 00:00:00.000000 nyckel-0.4.7/docs/is_toxic_cm.png
--rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 nyckel-0.4.7/docs/merge_labels.md
--rw-r--r--   0        0        0     3541 2020-02-02 00:00:00.000000 nyckel-0.4.7/docs/multimodal_classification.md
--rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 nyckel-0.4.7/docs/quickstart.md
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 nyckel-0.4.7/docs/requirements.txt
--rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 nyckel-0.4.7/docs/sklearn_analytics.md
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 nyckel-0.4.7/docs/tabular_classification.md
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 nyckel-0.4.7/docs/tabular_tags.md
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 nyckel-0.4.7/docs/text_classification.md
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 nyckel-0.4.7/docs/text_tags.md
--rw-r--r--   0        0        0     2013 2020-02-02 00:00:00.000000 nyckel-0.4.7/docs/assets/favicon.ico
--rw-r--r--   0        0        0     5903 2020-02-02 00:00:00.000000 nyckel-0.4.7/docs/assets/nyckel-logo.png
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 nyckel-0.4.7/docs/stylesheets/extra.css
--rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 nyckel-0.4.7/src/nyckel/__init__.py
--rw-r--r--   0        0        0     2307 2020-02-02 00:00:00.000000 nyckel-0.4.7/src/nyckel/auth.py
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 nyckel-0.4.7/src/nyckel/config.py
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 nyckel-0.4.7/src/nyckel/data_classes.py
--rw-r--r--   0        0        0     4337 2020-02-02 00:00:00.000000 nyckel-0.4.7/src/nyckel/image_processing.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nyckel-0.4.7/src/nyckel/py.typed
--rw-r--r--   0        0        0     5973 2020-02-02 00:00:00.000000 nyckel-0.4.7/src/nyckel/request_utils.py
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 nyckel-0.4.7/src/nyckel/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nyckel-0.4.7/src/nyckel/functions/__init__.py
--rw-r--r--   0        0        0     2963 2020-02-02 00:00:00.000000 nyckel-0.4.7/src/nyckel/functions/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nyckel-0.4.7/src/nyckel/functions/classification/__init__.py
--rw-r--r--   0        0        0     4576 2020-02-02 00:00:00.000000 nyckel-0.4.7/src/nyckel/functions/classification/classification.py
--rw-r--r--   0        0        0     2535 2020-02-02 00:00:00.000000 nyckel-0.4.7/src/nyckel/functions/classification/factory.py
--rw-r--r--   0        0        0     3708 2020-02-02 00:00:00.000000 nyckel-0.4.7/src/nyckel/functions/classification/function_handler.py
--rw-r--r--   0        0        0     9213 2020-02-02 00:00:00.000000 nyckel-0.4.7/src/nyckel/functions/classification/image_classification.py
--rw-r--r--   0        0        0     4434 2020-02-02 00:00:00.000000 nyckel-0.4.7/src/nyckel/functions/classification/label_handler.py
--rw-r--r--   0        0        0     6630 2020-02-02 00:00:00.000000 nyckel-0.4.7/src/nyckel/functions/classification/sample_handler.py
--rw-r--r--   0        0        0    14225 2020-02-02 00:00:00.000000 nyckel-0.4.7/src/nyckel/functions/classification/tabular_classification.py
--rw-r--r--   0        0        0     8162 2020-02-02 00:00:00.000000 nyckel-0.4.7/src/nyckel/functions/classification/text_classification.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nyckel-0.4.7/src/nyckel/functions/tags/__init__.py
--rw-r--r--   0        0        0    10187 2020-02-02 00:00:00.000000 nyckel-0.4.7/src/nyckel/functions/tags/image_tags.py
--rw-r--r--   0        0        0    13116 2020-02-02 00:00:00.000000 nyckel-0.4.7/src/nyckel/functions/tags/tabular_tags.py
--rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 nyckel-0.4.7/src/nyckel/functions/tags/tags.py
--rw-r--r--   0        0        0     2300 2020-02-02 00:00:00.000000 nyckel-0.4.7/src/nyckel/functions/tags/tags_function_factory.py
--rw-r--r--   0        0        0     3656 2020-02-02 00:00:00.000000 nyckel-0.4.7/src/nyckel/functions/tags/tags_function_handler.py
--rw-r--r--   0        0        0     6726 2020-02-02 00:00:00.000000 nyckel-0.4.7/src/nyckel/functions/tags/tags_sample_handler.py
--rw-r--r--   0        0        0     8190 2020-02-02 00:00:00.000000 nyckel-0.4.7/src/nyckel/functions/tags/text_tags.py
--rw-r--r--   0        0        0     8217 2020-02-02 00:00:00.000000 nyckel-0.4.7/tests/conftest.py
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 nyckel-0.4.7/tests/test_duplicates_handling.py
--rw-r--r--   0        0        0     1272 2020-02-02 00:00:00.000000 nyckel-0.4.7/tests/test_field_handler.py
--rw-r--r--   0        0        0     5272 2020-02-02 00:00:00.000000 nyckel-0.4.7/tests/test_image_classification_function.py
--rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 nyckel-0.4.7/tests/test_image_decoder.py
--rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 nyckel-0.4.7/tests/test_image_tags_function.py
--rw-r--r--   0        0        0     2767 2020-02-02 00:00:00.000000 nyckel-0.4.7/tests/test_label_handler.py
--rw-r--r--   0        0        0     2828 2020-02-02 00:00:00.000000 nyckel-0.4.7/tests/test_sample_handler.py
--rw-r--r--   0        0        0     7597 2020-02-02 00:00:00.000000 nyckel-0.4.7/tests/test_tabular_classification_function.py
--rw-r--r--   0        0        0     3137 2020-02-02 00:00:00.000000 nyckel-0.4.7/tests/test_tabular_tags_function.py
--rw-r--r--   0        0        0    10974 2020-02-02 00:00:00.000000 nyckel-0.4.7/tests/test_tags_shared.py
--rw-r--r--   0        0        0     3325 2020-02-02 00:00:00.000000 nyckel-0.4.7/tests/test_text_classification_function.py
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 nyckel-0.4.7/tests/test_white_background.py
--rw-r--r--   0        0        0   107239 2020-02-02 00:00:00.000000 nyckel-0.4.7/tests/fixtures/flower.jpg
--rw-r--r--   0        0        0    26189 2020-02-02 00:00:00.000000 nyckel-0.4.7/tests/fixtures/mixed-alpha-background.png
--rw-r--r--   0        0        0     3095 2020-02-02 00:00:00.000000 nyckel-0.4.7/.gitignore
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 nyckel-0.4.7/LICENSE
--rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 nyckel-0.4.7/README.md
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 nyckel-0.4.7/pyproject.toml
--rw-r--r--   0        0        0     2124 2020-02-02 00:00:00.000000 nyckel-0.4.7/PKG-INFO
+-rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 nyckel-0.4.8/mkdocs.yml
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 nyckel-0.4.8/requirements.txt
+-rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 nyckel-0.4.8/.github/workflows/build.yml
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 nyckel-0.4.8/.github/workflows/docs.yml
+-rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 nyckel-0.4.8/.github/workflows/test.yml
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 nyckel-0.4.8/.vscode/extensions.json
+-rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 nyckel-0.4.8/.vscode/settings.json
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 nyckel-0.4.8/docs/copy_function.md
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 nyckel-0.4.8/docs/credentials.md
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 nyckel-0.4.8/docs/data_classes.md
+-rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 nyckel-0.4.8/docs/delete_label.md
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 nyckel-0.4.8/docs/delete_samples.md
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 nyckel-0.4.8/docs/image_classification.md
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 nyckel-0.4.8/docs/image_tags.md
+-rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 nyckel-0.4.8/docs/index.md
+-rw-r--r--   0        0        0    15763 2020-02-02 00:00:00.000000 nyckel-0.4.8/docs/is_toxic_cm.png
+-rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 nyckel-0.4.8/docs/merge_labels.md
+-rw-r--r--   0        0        0     3541 2020-02-02 00:00:00.000000 nyckel-0.4.8/docs/multimodal_classification.md
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 nyckel-0.4.8/docs/quickstart.md
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 nyckel-0.4.8/docs/requirements.txt
+-rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 nyckel-0.4.8/docs/sklearn_analytics.md
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 nyckel-0.4.8/docs/tabular_classification.md
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 nyckel-0.4.8/docs/tabular_tags.md
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 nyckel-0.4.8/docs/text_classification.md
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 nyckel-0.4.8/docs/text_tags.md
+-rw-r--r--   0        0        0     2013 2020-02-02 00:00:00.000000 nyckel-0.4.8/docs/assets/favicon.ico
+-rw-r--r--   0        0        0     5903 2020-02-02 00:00:00.000000 nyckel-0.4.8/docs/assets/nyckel-logo.png
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 nyckel-0.4.8/docs/stylesheets/extra.css
+-rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 nyckel-0.4.8/src/nyckel/__init__.py
+-rw-r--r--   0        0        0     2307 2020-02-02 00:00:00.000000 nyckel-0.4.8/src/nyckel/auth.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 nyckel-0.4.8/src/nyckel/config.py
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 nyckel-0.4.8/src/nyckel/data_classes.py
+-rw-r--r--   0        0        0     4337 2020-02-02 00:00:00.000000 nyckel-0.4.8/src/nyckel/image_processing.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nyckel-0.4.8/src/nyckel/py.typed
+-rw-r--r--   0        0        0     5973 2020-02-02 00:00:00.000000 nyckel-0.4.8/src/nyckel/request_utils.py
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 nyckel-0.4.8/src/nyckel/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nyckel-0.4.8/src/nyckel/functions/__init__.py
+-rw-r--r--   0        0        0     2963 2020-02-02 00:00:00.000000 nyckel-0.4.8/src/nyckel/functions/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nyckel-0.4.8/src/nyckel/functions/classification/__init__.py
+-rw-r--r--   0        0        0     4576 2020-02-02 00:00:00.000000 nyckel-0.4.8/src/nyckel/functions/classification/classification.py
+-rw-r--r--   0        0        0     2535 2020-02-02 00:00:00.000000 nyckel-0.4.8/src/nyckel/functions/classification/factory.py
+-rw-r--r--   0        0        0     3708 2020-02-02 00:00:00.000000 nyckel-0.4.8/src/nyckel/functions/classification/function_handler.py
+-rw-r--r--   0        0        0     9213 2020-02-02 00:00:00.000000 nyckel-0.4.8/src/nyckel/functions/classification/image_classification.py
+-rw-r--r--   0        0        0     4434 2020-02-02 00:00:00.000000 nyckel-0.4.8/src/nyckel/functions/classification/label_handler.py
+-rw-r--r--   0        0        0     6630 2020-02-02 00:00:00.000000 nyckel-0.4.8/src/nyckel/functions/classification/sample_handler.py
+-rw-r--r--   0        0        0    14225 2020-02-02 00:00:00.000000 nyckel-0.4.8/src/nyckel/functions/classification/tabular_classification.py
+-rw-r--r--   0        0        0     8162 2020-02-02 00:00:00.000000 nyckel-0.4.8/src/nyckel/functions/classification/text_classification.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nyckel-0.4.8/src/nyckel/functions/tags/__init__.py
+-rw-r--r--   0        0        0    10187 2020-02-02 00:00:00.000000 nyckel-0.4.8/src/nyckel/functions/tags/image_tags.py
+-rw-r--r--   0        0        0    13116 2020-02-02 00:00:00.000000 nyckel-0.4.8/src/nyckel/functions/tags/tabular_tags.py
+-rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 nyckel-0.4.8/src/nyckel/functions/tags/tags.py
+-rw-r--r--   0        0        0     2300 2020-02-02 00:00:00.000000 nyckel-0.4.8/src/nyckel/functions/tags/tags_function_factory.py
+-rw-r--r--   0        0        0     3656 2020-02-02 00:00:00.000000 nyckel-0.4.8/src/nyckel/functions/tags/tags_function_handler.py
+-rw-r--r--   0        0        0     6706 2020-02-02 00:00:00.000000 nyckel-0.4.8/src/nyckel/functions/tags/tags_sample_handler.py
+-rw-r--r--   0        0        0     8190 2020-02-02 00:00:00.000000 nyckel-0.4.8/src/nyckel/functions/tags/text_tags.py
+-rw-r--r--   0        0        0     8217 2020-02-02 00:00:00.000000 nyckel-0.4.8/tests/conftest.py
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 nyckel-0.4.8/tests/test_duplicates_handling.py
+-rw-r--r--   0        0        0     1272 2020-02-02 00:00:00.000000 nyckel-0.4.8/tests/test_field_handler.py
+-rw-r--r--   0        0        0     5272 2020-02-02 00:00:00.000000 nyckel-0.4.8/tests/test_image_classification_function.py
+-rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 nyckel-0.4.8/tests/test_image_decoder.py
+-rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 nyckel-0.4.8/tests/test_image_tags_function.py
+-rw-r--r--   0        0        0     2767 2020-02-02 00:00:00.000000 nyckel-0.4.8/tests/test_label_handler.py
+-rw-r--r--   0        0        0     2828 2020-02-02 00:00:00.000000 nyckel-0.4.8/tests/test_sample_handler.py
+-rw-r--r--   0        0        0     7597 2020-02-02 00:00:00.000000 nyckel-0.4.8/tests/test_tabular_classification_function.py
+-rw-r--r--   0        0        0     3137 2020-02-02 00:00:00.000000 nyckel-0.4.8/tests/test_tabular_tags_function.py
+-rw-r--r--   0        0        0    10974 2020-02-02 00:00:00.000000 nyckel-0.4.8/tests/test_tags_shared.py
+-rw-r--r--   0        0        0     3325 2020-02-02 00:00:00.000000 nyckel-0.4.8/tests/test_text_classification_function.py
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 nyckel-0.4.8/tests/test_white_background.py
+-rw-r--r--   0        0        0   107239 2020-02-02 00:00:00.000000 nyckel-0.4.8/tests/fixtures/flower.jpg
+-rw-r--r--   0        0        0    26189 2020-02-02 00:00:00.000000 nyckel-0.4.8/tests/fixtures/mixed-alpha-background.png
+-rw-r--r--   0        0        0     3095 2020-02-02 00:00:00.000000 nyckel-0.4.8/.gitignore
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 nyckel-0.4.8/LICENSE
+-rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 nyckel-0.4.8/README.md
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 nyckel-0.4.8/pyproject.toml
+-rw-r--r--   0        0        0     2124 2020-02-02 00:00:00.000000 nyckel-0.4.8/PKG-INFO
```

### Comparing `nyckel-0.4.7/mkdocs.yml` & `nyckel-0.4.8/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.7/.github/workflows/build.yml` & `nyckel-0.4.8/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.7/.github/workflows/docs.yml` & `nyckel-0.4.8/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.7/.github/workflows/test.yml` & `nyckel-0.4.8/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.7/.vscode/settings.json` & `nyckel-0.4.8/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.7/docs/copy_function.md` & `nyckel-0.4.8/docs/copy_function.md`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.7/docs/delete_label.md` & `nyckel-0.4.8/docs/delete_label.md`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.7/docs/delete_samples.md` & `nyckel-0.4.8/docs/delete_samples.md`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.7/docs/index.md` & `nyckel-0.4.8/docs/index.md`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.7/docs/is_toxic_cm.png` & `nyckel-0.4.8/docs/is_toxic_cm.png`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.7/docs/merge_labels.md` & `nyckel-0.4.8/docs/merge_labels.md`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.7/docs/multimodal_classification.md` & `nyckel-0.4.8/docs/multimodal_classification.md`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.7/docs/quickstart.md` & `nyckel-0.4.8/docs/quickstart.md`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.7/docs/sklearn_analytics.md` & `nyckel-0.4.8/docs/sklearn_analytics.md`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.7/docs/assets/favicon.ico` & `nyckel-0.4.8/docs/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.7/docs/assets/nyckel-logo.png` & `nyckel-0.4.8/docs/assets/nyckel-logo.png`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.7/src/nyckel/__init__.py` & `nyckel-0.4.8/src/nyckel/__init__.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.7/src/nyckel/auth.py` & `nyckel-0.4.8/src/nyckel/auth.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.7/src/nyckel/image_processing.py` & `nyckel-0.4.8/src/nyckel/image_processing.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.7/src/nyckel/request_utils.py` & `nyckel-0.4.8/src/nyckel/request_utils.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.7/src/nyckel/functions/utils.py` & `nyckel-0.4.8/src/nyckel/functions/utils.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.7/src/nyckel/functions/classification/classification.py` & `nyckel-0.4.8/src/nyckel/functions/classification/classification.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.7/src/nyckel/functions/classification/factory.py` & `nyckel-0.4.8/src/nyckel/functions/classification/factory.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.7/src/nyckel/functions/classification/function_handler.py` & `nyckel-0.4.8/src/nyckel/functions/classification/function_handler.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.7/src/nyckel/functions/classification/image_classification.py` & `nyckel-0.4.8/src/nyckel/functions/classification/image_classification.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.7/src/nyckel/functions/classification/label_handler.py` & `nyckel-0.4.8/src/nyckel/functions/classification/label_handler.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.7/src/nyckel/functions/classification/sample_handler.py` & `nyckel-0.4.8/src/nyckel/functions/classification/sample_handler.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.7/src/nyckel/functions/classification/tabular_classification.py` & `nyckel-0.4.8/src/nyckel/functions/classification/tabular_classification.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.7/src/nyckel/functions/classification/text_classification.py` & `nyckel-0.4.8/src/nyckel/functions/classification/text_classification.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.7/src/nyckel/functions/tags/image_tags.py` & `nyckel-0.4.8/src/nyckel/functions/tags/image_tags.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.7/src/nyckel/functions/tags/tabular_tags.py` & `nyckel-0.4.8/src/nyckel/functions/tags/tabular_tags.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.7/src/nyckel/functions/tags/tags.py` & `nyckel-0.4.8/src/nyckel/functions/tags/tags.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.7/src/nyckel/functions/tags/tags_function_factory.py` & `nyckel-0.4.8/src/nyckel/functions/tags/tags_function_factory.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.7/src/nyckel/functions/tags/tags_function_handler.py` & `nyckel-0.4.8/src/nyckel/functions/tags/tags_function_handler.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.7/src/nyckel/functions/tags/tags_sample_handler.py` & `nyckel-0.4.8/src/nyckel/functions/tags/tags_sample_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,23 +119,23 @@
             ),
         )(tqdm(total=sample_count, ncols=80, desc="Listing samples"))
 
         return samples_dict_list
 
     def read_sample(self, sample_id: str) -> Dict:
         session = self._credentials.get_session()
-        response = session.get(self._url_handler.api_endpoint(path=f"samples/{sample_id}", api_version="v0.9"))
+        url = self._url_handler.api_endpoint(path=f"samples/{sample_id}", api_version="v0.9")
+        response = session.get(url)
         if response.status_code == 404:
             # If calling read right after create, the resource is not available yet. Sleep and retry once.
             time.sleep(1)
             response = session.get(self._url_handler.api_endpoint(path=f"samples/{sample_id}"))
         if not response.status_code == 200:
             raise RuntimeError(
-                f"{response.status_code=}, {response.text=}. Unable to fetch sample {sample_id} "
-                f"from {self._url_handler.train_page}"
+                f"{response.status_code=}, {response.text=}. Unable to fetch sample {sample_id} " f"from {url   }"
             )
         return response.json()
 
     def update_annotation(self, sample: Union[TextTagsSample, ImageTagsSample]) -> None:
         session = self._credentials.get_session()
         assert sample.annotation
         response = session.put(
```

### Comparing `nyckel-0.4.7/src/nyckel/functions/tags/text_tags.py` & `nyckel-0.4.8/src/nyckel/functions/tags/text_tags.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.7/tests/conftest.py` & `nyckel-0.4.8/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.7/tests/test_duplicates_handling.py` & `nyckel-0.4.8/tests/test_duplicates_handling.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.7/tests/test_field_handler.py` & `nyckel-0.4.8/tests/test_field_handler.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.7/tests/test_image_classification_function.py` & `nyckel-0.4.8/tests/test_image_classification_function.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.7/tests/test_image_decoder.py` & `nyckel-0.4.8/tests/test_image_decoder.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.7/tests/test_image_tags_function.py` & `nyckel-0.4.8/tests/test_image_tags_function.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.7/tests/test_label_handler.py` & `nyckel-0.4.8/tests/test_label_handler.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.7/tests/test_sample_handler.py` & `nyckel-0.4.8/tests/test_sample_handler.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.7/tests/test_tabular_classification_function.py` & `nyckel-0.4.8/tests/test_tabular_classification_function.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.7/tests/test_tabular_tags_function.py` & `nyckel-0.4.8/tests/test_tabular_tags_function.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.7/tests/test_tags_shared.py` & `nyckel-0.4.8/tests/test_tags_shared.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.7/tests/test_text_classification_function.py` & `nyckel-0.4.8/tests/test_text_classification_function.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.7/tests/test_white_background.py` & `nyckel-0.4.8/tests/test_white_background.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.7/tests/fixtures/flower.jpg` & `nyckel-0.4.8/tests/fixtures/flower.jpg`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.7/tests/fixtures/mixed-alpha-background.png` & `nyckel-0.4.8/tests/fixtures/mixed-alpha-background.png`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.7/.gitignore` & `nyckel-0.4.8/.gitignore`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.7/LICENSE` & `nyckel-0.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.7/README.md` & `nyckel-0.4.8/README.md`

 * *Files identical despite different names*

### Comparing `nyckel-0.4.7/pyproject.toml` & `nyckel-0.4.8/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/nyckel"]
 
 [project]
 name = "nyckel"
-version = "0.4.7"
+version = "0.4.8"
 authors = [{ name = "Oscar Beijbom", email = "oscar@nyckel.com" }]
 description = "Python package for the Nyckel API"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: MIT License",
```

### Comparing `nyckel-0.4.7/PKG-INFO` & `nyckel-0.4.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: nyckel
-Version: 0.4.7
+Version: 0.4.8
 Summary: Python package for the Nyckel API
 Project-URL: Homepage, https://github.com/NyckelAI/python-sdk
 Author-email: Oscar Beijbom <oscar@nyckel.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```


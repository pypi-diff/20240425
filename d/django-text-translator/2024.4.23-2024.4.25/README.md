# Comparing `tmp/django_text_translator-2024.4.23.tar.gz` & `tmp/django_text_translator-2024.4.25.tar.gz`

## Comparing `django_text_translator-2024.4.23.tar` & `django_text_translator-2024.4.25.tar`

### file list

```diff
@@ -1,53 +1,57 @@
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 django_text_translator-2024.4.23/.github/FUNDING.yml
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 django_text_translator-2024.4.23/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_text_translator-2024.4.23/django_text_translator/__init__.py
--rw-r--r--   0        0        0     5528 2020-02-02 00:00:00.000000 django_text_translator-2024.4.23/django_text_translator/admin.py
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 django_text_translator-2024.4.23/django_text_translator/apps.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 django_text_translator-2024.4.23/django_text_translator/tests.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_text_translator-2024.4.23/django_text_translator/views.py
--rw-r--r--   0        0        0     3310 2020-02-02 00:00:00.000000 django_text_translator-2024.4.23/django_text_translator/migrations/0001_initial.py
--rw-r--r--   0        0        0     1454 2020-02-02 00:00:00.000000 django_text_translator-2024.4.23/django_text_translator/migrations/0002_openaitranslator_base_url_and_more.py
--rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 django_text_translator-2024.4.23/django_text_translator/migrations/0003_azureaitranslator_openaitranslator_frequency_penalty_and_more.py
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 django_text_translator-2024.4.23/django_text_translator/migrations/0004_alter_openaitranslator_model.py
--rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 django_text_translator-2024.4.23/django_text_translator/migrations/0005_caiyuntranslator_deeplxtranslator.py
--rw-r--r--   0        0        0     1216 2020-02-02 00:00:00.000000 django_text_translator-2024.4.23/django_text_translator/migrations/0006_testtranslator_alter_openaitranslator_prompt.py
--rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 django_text_translator-2024.4.23/django_text_translator/migrations/0007_caiyuntranslator_max_characters_and_more.py
--rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 django_text_translator-2024.4.23/django_text_translator/migrations/0008_geminitranslator.py
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 django_text_translator-2024.4.23/django_text_translator/migrations/0009_deepltranslator_proxy_deepltranslator_server_url.py
--rw-r--r--   0        0        0     1891 2020-02-02 00:00:00.000000 django_text_translator-2024.4.23/django_text_translator/migrations/0010_claudetranslator.py
--rw-r--r--   0        0        0     1363 2020-02-02 00:00:00.000000 django_text_translator-2024.4.23/django_text_translator/migrations/0011_googletranslatewebtranslator_and_more.py
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 django_text_translator-2024.4.23/django_text_translator/migrations/0012_geminitranslator_interval.py
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 django_text_translator-2024.4.23/django_text_translator/migrations/0013_deeplwebtranslator.py
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 django_text_translator-2024.4.23/django_text_translator/migrations/0014_testtranslator_interval.py
--rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 django_text_translator-2024.4.23/django_text_translator/migrations/0015_googletranslatewebtranslator_max_characters.py
--rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 django_text_translator-2024.4.23/django_text_translator/migrations/0016_alter_deeplwebtranslator_max_characters_and_more.py
--rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 django_text_translator-2024.4.23/django_text_translator/migrations/0017_remove_translated_content_id_and_more.py
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 django_text_translator-2024.4.23/django_text_translator/migrations/0018_alter_claudetranslator_model.py
--rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 django_text_translator-2024.4.23/django_text_translator/migrations/0019_alter_openaitranslator_model.py
--rw-r--r--   0        0        0     2567 2020-02-02 00:00:00.000000 django_text_translator-2024.4.23/django_text_translator/migrations/0020_moonshotaitranslator.py
--rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 django_text_translator-2024.4.23/django_text_translator/migrations/0021_alter_claudetranslator_model.py
--rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 django_text_translator-2024.4.23/django_text_translator/migrations/0022_alter_geminitranslator_model.py
--rw-r--r--   0        0        0     2200 2020-02-02 00:00:00.000000 django_text_translator-2024.4.23/django_text_translator/migrations/0023_azureaitranslator_summary_prompt_and_more.py
--rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 django_text_translator-2024.4.23/django_text_translator/migrations/0024_alter_claudetranslator_model_and_more.py
--rw-r--r--   0        0        0     6438 2020-02-02 00:00:00.000000 django_text_translator-2024.4.23/django_text_translator/migrations/0025_remove_azureaitranslator_deloyment_name_and_more.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_text_translator-2024.4.23/django_text_translator/migrations/__init__.py
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 django_text_translator-2024.4.23/django_text_translator/models/__init__.py
--rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 django_text_translator-2024.4.23/django_text_translator/models/azureai.py
--rw-r--r--   0        0        0     6427 2020-02-02 00:00:00.000000 django_text_translator-2024.4.23/django_text_translator/models/base.py
--rw-r--r--   0        0        0     2100 2020-02-02 00:00:00.000000 django_text_translator-2024.4.23/django_text_translator/models/caiyun.py
--rw-r--r--   0        0        0     3269 2020-02-02 00:00:00.000000 django_text_translator-2024.4.23/django_text_translator/models/claude.py
--rw-r--r--   0        0        0     2391 2020-02-02 00:00:00.000000 django_text_translator-2024.4.23/django_text_translator/models/deepl.py
--rw-r--r--   0        0        0     2182 2020-02-02 00:00:00.000000 django_text_translator-2024.4.23/django_text_translator/models/deeplweb.py
--rw-r--r--   0        0        0     2478 2020-02-02 00:00:00.000000 django_text_translator-2024.4.23/django_text_translator/models/deeplx.py
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 django_text_translator-2024.4.23/django_text_translator/models/dev.py
--rw-r--r--   0        0        0     3574 2020-02-02 00:00:00.000000 django_text_translator-2024.4.23/django_text_translator/models/gemini.py
--rw-r--r--   0        0        0     2611 2020-02-02 00:00:00.000000 django_text_translator-2024.4.23/django_text_translator/models/google_translate_web.py
--rw-r--r--   0        0        0     2906 2020-02-02 00:00:00.000000 django_text_translator-2024.4.23/django_text_translator/models/microsoft_translate.py
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 django_text_translator-2024.4.23/django_text_translator/models/moonshotai.py
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 django_text_translator-2024.4.23/django_text_translator/models/openai.py
--rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 django_text_translator-2024.4.23/django_text_translator/static/img/icon-loading.svg
--rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 django_text_translator-2024.4.23/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 django_text_translator-2024.4.23/LICENSE
--rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 django_text_translator-2024.4.23/README.md
--rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 django_text_translator-2024.4.23/pyproject.toml
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 django_text_translator-2024.4.23/PKG-INFO
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 django_text_translator-2024.4.25/.github/FUNDING.yml
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 django_text_translator-2024.4.25/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_text_translator-2024.4.25/django_text_translator/__init__.py
+-rw-r--r--   0        0        0     6748 2020-02-02 00:00:00.000000 django_text_translator-2024.4.25/django_text_translator/admin.py
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 django_text_translator-2024.4.25/django_text_translator/apps.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 django_text_translator-2024.4.25/django_text_translator/tests.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_text_translator-2024.4.25/django_text_translator/views.py
+-rw-r--r--   0        0        0     3310 2020-02-02 00:00:00.000000 django_text_translator-2024.4.25/django_text_translator/migrations/0001_initial.py
+-rw-r--r--   0        0        0     1454 2020-02-02 00:00:00.000000 django_text_translator-2024.4.25/django_text_translator/migrations/0002_openaitranslator_base_url_and_more.py
+-rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 django_text_translator-2024.4.25/django_text_translator/migrations/0003_azureaitranslator_openaitranslator_frequency_penalty_and_more.py
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 django_text_translator-2024.4.25/django_text_translator/migrations/0004_alter_openaitranslator_model.py
+-rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 django_text_translator-2024.4.25/django_text_translator/migrations/0005_caiyuntranslator_deeplxtranslator.py
+-rw-r--r--   0        0        0     1216 2020-02-02 00:00:00.000000 django_text_translator-2024.4.25/django_text_translator/migrations/0006_testtranslator_alter_openaitranslator_prompt.py
+-rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 django_text_translator-2024.4.25/django_text_translator/migrations/0007_caiyuntranslator_max_characters_and_more.py
+-rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 django_text_translator-2024.4.25/django_text_translator/migrations/0008_geminitranslator.py
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 django_text_translator-2024.4.25/django_text_translator/migrations/0009_deepltranslator_proxy_deepltranslator_server_url.py
+-rw-r--r--   0        0        0     1891 2020-02-02 00:00:00.000000 django_text_translator-2024.4.25/django_text_translator/migrations/0010_claudetranslator.py
+-rw-r--r--   0        0        0     1363 2020-02-02 00:00:00.000000 django_text_translator-2024.4.25/django_text_translator/migrations/0011_googletranslatewebtranslator_and_more.py
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 django_text_translator-2024.4.25/django_text_translator/migrations/0012_geminitranslator_interval.py
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 django_text_translator-2024.4.25/django_text_translator/migrations/0013_deeplwebtranslator.py
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 django_text_translator-2024.4.25/django_text_translator/migrations/0014_testtranslator_interval.py
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 django_text_translator-2024.4.25/django_text_translator/migrations/0015_googletranslatewebtranslator_max_characters.py
+-rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 django_text_translator-2024.4.25/django_text_translator/migrations/0016_alter_deeplwebtranslator_max_characters_and_more.py
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 django_text_translator-2024.4.25/django_text_translator/migrations/0017_remove_translated_content_id_and_more.py
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 django_text_translator-2024.4.25/django_text_translator/migrations/0018_alter_claudetranslator_model.py
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 django_text_translator-2024.4.25/django_text_translator/migrations/0019_alter_openaitranslator_model.py
+-rw-r--r--   0        0        0     2567 2020-02-02 00:00:00.000000 django_text_translator-2024.4.25/django_text_translator/migrations/0020_moonshotaitranslator.py
+-rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 django_text_translator-2024.4.25/django_text_translator/migrations/0021_alter_claudetranslator_model.py
+-rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 django_text_translator-2024.4.25/django_text_translator/migrations/0022_alter_geminitranslator_model.py
+-rw-r--r--   0        0        0     2200 2020-02-02 00:00:00.000000 django_text_translator-2024.4.25/django_text_translator/migrations/0023_azureaitranslator_summary_prompt_and_more.py
+-rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 django_text_translator-2024.4.25/django_text_translator/migrations/0024_alter_claudetranslator_model_and_more.py
+-rw-r--r--   0        0        0     6438 2020-02-02 00:00:00.000000 django_text_translator-2024.4.25/django_text_translator/migrations/0025_remove_azureaitranslator_deloyment_name_and_more.py
+-rw-r--r--   0        0        0     5119 2020-02-02 00:00:00.000000 django_text_translator-2024.4.25/django_text_translator/migrations/0026_groqtranslator_openrouteraitranslator_and_more.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_text_translator-2024.4.25/django_text_translator/migrations/__init__.py
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 django_text_translator-2024.4.25/django_text_translator/models/__init__.py
+-rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 django_text_translator-2024.4.25/django_text_translator/models/azureai.py
+-rw-r--r--   0        0        0     6427 2020-02-02 00:00:00.000000 django_text_translator-2024.4.25/django_text_translator/models/base.py
+-rw-r--r--   0        0        0     2100 2020-02-02 00:00:00.000000 django_text_translator-2024.4.25/django_text_translator/models/caiyun.py
+-rw-r--r--   0        0        0     3269 2020-02-02 00:00:00.000000 django_text_translator-2024.4.25/django_text_translator/models/claude.py
+-rw-r--r--   0        0        0     2391 2020-02-02 00:00:00.000000 django_text_translator-2024.4.25/django_text_translator/models/deepl.py
+-rw-r--r--   0        0        0     2182 2020-02-02 00:00:00.000000 django_text_translator-2024.4.25/django_text_translator/models/deeplweb.py
+-rw-r--r--   0        0        0     2478 2020-02-02 00:00:00.000000 django_text_translator-2024.4.25/django_text_translator/models/deeplx.py
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 django_text_translator-2024.4.25/django_text_translator/models/dev.py
+-rw-r--r--   0        0        0     3574 2020-02-02 00:00:00.000000 django_text_translator-2024.4.25/django_text_translator/models/gemini.py
+-rw-r--r--   0        0        0     2611 2020-02-02 00:00:00.000000 django_text_translator-2024.4.25/django_text_translator/models/google_translate_web.py
+-rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 django_text_translator-2024.4.25/django_text_translator/models/groq.py
+-rw-r--r--   0        0        0     2906 2020-02-02 00:00:00.000000 django_text_translator-2024.4.25/django_text_translator/models/microsoft_translate.py
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 django_text_translator-2024.4.25/django_text_translator/models/moonshotai.py
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 django_text_translator-2024.4.25/django_text_translator/models/openai.py
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 django_text_translator-2024.4.25/django_text_translator/models/openrouterai.py
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 django_text_translator-2024.4.25/django_text_translator/models/togetherai.py
+-rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 django_text_translator-2024.4.25/django_text_translator/static/img/icon-loading.svg
+-rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 django_text_translator-2024.4.25/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 django_text_translator-2024.4.25/LICENSE
+-rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 django_text_translator-2024.4.25/README.md
+-rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 django_text_translator-2024.4.25/pyproject.toml
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 django_text_translator-2024.4.25/PKG-INFO
```

### Comparing `django_text_translator-2024.4.23/.github/workflows/python-publish.yml` & `django_text_translator-2024.4.25/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `django_text_translator-2024.4.23/django_text_translator/admin.py` & `django_text_translator-2024.4.25/django_text_translator/admin.py`

 * *Files 16% similar despite different names*

```diff
@@ -101,14 +101,33 @@
 
 @admin.register(MoonshotAITranslator)
 class MoonshotAITranslatorAdmin(BaseTranslatorAdmin):
     fields = ["name", "api_key", "base_url", "model", "translate_prompt", "summary_prompt", "temperature", "top_p", "frequency_penalty",
               "presence_penalty", "max_tokens"]
     list_display = ["name", "is_valid", "masked_api_key", "model", "translate_prompt", "summary_prompt", "max_tokens", "base_url"]
 
+@admin.register(TogetherAITranslator)
+class TogetherAITranslatorAdmin(BaseTranslatorAdmin):
+    fields = ["name", "api_key", "base_url", "model", "translate_prompt", "summary_prompt", "temperature", "top_p", "frequency_penalty",
+              "presence_penalty", "max_tokens"]
+    list_display = ["name", "is_valid", "masked_api_key", "model", "translate_prompt", "summary_prompt", "max_tokens", "base_url"]
+
+@admin.register(OpenRouterAITranslator)
+class OpenRouterAITranslatorAdmin(BaseTranslatorAdmin):
+    fields = ["name", "api_key", "base_url", "model", "translate_prompt", "summary_prompt", "temperature", "top_p", "frequency_penalty",
+              "presence_penalty", "max_tokens"]
+    list_display = ["name", "is_valid", "masked_api_key", "model", "translate_prompt", "summary_prompt", "max_tokens", "base_url"]
+
+@admin.register(GroqTranslator)
+class GroqTranslatorAdmin(BaseTranslatorAdmin):
+    fields = ["name", "api_key", "base_url", "model", "translate_prompt", "summary_prompt", "temperature", "top_p", "frequency_penalty",
+              "presence_penalty", "max_tokens"]
+    list_display = ["name", "is_valid", "masked_api_key", "model", "translate_prompt", "summary_prompt", "max_tokens", "base_url"]
+
+
 if settings.DEBUG:
     @admin.register(Translated_Content)
     class Translated_ContentAdmin(admin.ModelAdmin):
         fields = ["original_content", "translated_content", "translated_language", "tokens", "characters"]
         list_display = ["original_content", "translated_language", "translated_content", "tokens", "characters"]
     
         # def has_change_permission(self, request, obj=None):
```

### Comparing `django_text_translator-2024.4.23/django_text_translator/migrations/0001_initial.py` & `django_text_translator-2024.4.25/django_text_translator/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_text_translator-2024.4.23/django_text_translator/migrations/0002_openaitranslator_base_url_and_more.py` & `django_text_translator-2024.4.25/django_text_translator/migrations/0002_openaitranslator_base_url_and_more.py`

 * *Files identical despite different names*

### Comparing `django_text_translator-2024.4.23/django_text_translator/migrations/0003_azureaitranslator_openaitranslator_frequency_penalty_and_more.py` & `django_text_translator-2024.4.25/django_text_translator/migrations/0003_azureaitranslator_openaitranslator_frequency_penalty_and_more.py`

 * *Files identical despite different names*

### Comparing `django_text_translator-2024.4.23/django_text_translator/migrations/0004_alter_openaitranslator_model.py` & `django_text_translator-2024.4.25/django_text_translator/migrations/0004_alter_openaitranslator_model.py`

 * *Files identical despite different names*

### Comparing `django_text_translator-2024.4.23/django_text_translator/migrations/0005_caiyuntranslator_deeplxtranslator.py` & `django_text_translator-2024.4.25/django_text_translator/migrations/0005_caiyuntranslator_deeplxtranslator.py`

 * *Files identical despite different names*

### Comparing `django_text_translator-2024.4.23/django_text_translator/migrations/0006_testtranslator_alter_openaitranslator_prompt.py` & `django_text_translator-2024.4.25/django_text_translator/migrations/0006_testtranslator_alter_openaitranslator_prompt.py`

 * *Files identical despite different names*

### Comparing `django_text_translator-2024.4.23/django_text_translator/migrations/0007_caiyuntranslator_max_characters_and_more.py` & `django_text_translator-2024.4.25/django_text_translator/migrations/0007_caiyuntranslator_max_characters_and_more.py`

 * *Files identical despite different names*

### Comparing `django_text_translator-2024.4.23/django_text_translator/migrations/0008_geminitranslator.py` & `django_text_translator-2024.4.25/django_text_translator/migrations/0008_geminitranslator.py`

 * *Files identical despite different names*

### Comparing `django_text_translator-2024.4.23/django_text_translator/migrations/0009_deepltranslator_proxy_deepltranslator_server_url.py` & `django_text_translator-2024.4.25/django_text_translator/migrations/0009_deepltranslator_proxy_deepltranslator_server_url.py`

 * *Files identical despite different names*

### Comparing `django_text_translator-2024.4.23/django_text_translator/migrations/0010_claudetranslator.py` & `django_text_translator-2024.4.25/django_text_translator/migrations/0010_claudetranslator.py`

 * *Files identical despite different names*

### Comparing `django_text_translator-2024.4.23/django_text_translator/migrations/0011_googletranslatewebtranslator_and_more.py` & `django_text_translator-2024.4.25/django_text_translator/migrations/0011_googletranslatewebtranslator_and_more.py`

 * *Files identical despite different names*

### Comparing `django_text_translator-2024.4.23/django_text_translator/migrations/0013_deeplwebtranslator.py` & `django_text_translator-2024.4.25/django_text_translator/migrations/0013_deeplwebtranslator.py`

 * *Files identical despite different names*

### Comparing `django_text_translator-2024.4.23/django_text_translator/migrations/0016_alter_deeplwebtranslator_max_characters_and_more.py` & `django_text_translator-2024.4.25/django_text_translator/migrations/0016_alter_deeplwebtranslator_max_characters_and_more.py`

 * *Files identical despite different names*

### Comparing `django_text_translator-2024.4.23/django_text_translator/migrations/0017_remove_translated_content_id_and_more.py` & `django_text_translator-2024.4.25/django_text_translator/migrations/0017_remove_translated_content_id_and_more.py`

 * *Files identical despite different names*

### Comparing `django_text_translator-2024.4.23/django_text_translator/migrations/0018_alter_claudetranslator_model.py` & `django_text_translator-2024.4.25/django_text_translator/migrations/0018_alter_claudetranslator_model.py`

 * *Files identical despite different names*

### Comparing `django_text_translator-2024.4.23/django_text_translator/migrations/0019_alter_openaitranslator_model.py` & `django_text_translator-2024.4.25/django_text_translator/migrations/0019_alter_openaitranslator_model.py`

 * *Files identical despite different names*

### Comparing `django_text_translator-2024.4.23/django_text_translator/migrations/0020_moonshotaitranslator.py` & `django_text_translator-2024.4.25/django_text_translator/migrations/0020_moonshotaitranslator.py`

 * *Files identical despite different names*

### Comparing `django_text_translator-2024.4.23/django_text_translator/migrations/0021_alter_claudetranslator_model.py` & `django_text_translator-2024.4.25/django_text_translator/migrations/0021_alter_claudetranslator_model.py`

 * *Files identical despite different names*

### Comparing `django_text_translator-2024.4.23/django_text_translator/migrations/0023_azureaitranslator_summary_prompt_and_more.py` & `django_text_translator-2024.4.25/django_text_translator/migrations/0023_azureaitranslator_summary_prompt_and_more.py`

 * *Files identical despite different names*

### Comparing `django_text_translator-2024.4.23/django_text_translator/migrations/0024_alter_claudetranslator_model_and_more.py` & `django_text_translator-2024.4.25/django_text_translator/migrations/0024_alter_claudetranslator_model_and_more.py`

 * *Files identical despite different names*

### Comparing `django_text_translator-2024.4.23/django_text_translator/migrations/0025_remove_azureaitranslator_deloyment_name_and_more.py` & `django_text_translator-2024.4.25/django_text_translator/migrations/0025_remove_azureaitranslator_deloyment_name_and_more.py`

 * *Files identical despite different names*

### Comparing `django_text_translator-2024.4.23/django_text_translator/models/__init__.py` & `django_text_translator-2024.4.25/django_text_translator/models/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,8 +6,13 @@
 from .deeplx import DeepLXTranslator
 from .deeplweb import DeepLWebTranslator
 from .gemini import GeminiTranslator
 from .google_translate_web import GoogleTranslateWebTranslator
 from .microsoft_translate import MicrosoftTranslator
 from .moonshotai import MoonshotAITranslator
 from .openai import OpenAITranslator
+from .togetherai import TogetherAITranslator
+from .openrouterai import OpenRouterAITranslator
+from .groq import GroqTranslator
+
+
 from .dev import TestTranslator
```

### Comparing `django_text_translator-2024.4.23/django_text_translator/models/azureai.py` & `django_text_translator-2024.4.25/django_text_translator/models/azureai.py`

 * *Files identical despite different names*

### Comparing `django_text_translator-2024.4.23/django_text_translator/models/base.py` & `django_text_translator-2024.4.25/django_text_translator/models/base.py`

 * *Files identical despite different names*

### Comparing `django_text_translator-2024.4.23/django_text_translator/models/caiyun.py` & `django_text_translator-2024.4.25/django_text_translator/models/caiyun.py`

 * *Files identical despite different names*

### Comparing `django_text_translator-2024.4.23/django_text_translator/models/claude.py` & `django_text_translator-2024.4.25/django_text_translator/models/claude.py`

 * *Files identical despite different names*

### Comparing `django_text_translator-2024.4.23/django_text_translator/models/deepl.py` & `django_text_translator-2024.4.25/django_text_translator/models/deepl.py`

 * *Files identical despite different names*

### Comparing `django_text_translator-2024.4.23/django_text_translator/models/deeplweb.py` & `django_text_translator-2024.4.25/django_text_translator/models/deeplweb.py`

 * *Files identical despite different names*

### Comparing `django_text_translator-2024.4.23/django_text_translator/models/deeplx.py` & `django_text_translator-2024.4.25/django_text_translator/models/deeplx.py`

 * *Files identical despite different names*

### Comparing `django_text_translator-2024.4.23/django_text_translator/models/dev.py` & `django_text_translator-2024.4.25/django_text_translator/models/dev.py`

 * *Files identical despite different names*

### Comparing `django_text_translator-2024.4.23/django_text_translator/models/gemini.py` & `django_text_translator-2024.4.25/django_text_translator/models/gemini.py`

 * *Files identical despite different names*

### Comparing `django_text_translator-2024.4.23/django_text_translator/models/google_translate_web.py` & `django_text_translator-2024.4.25/django_text_translator/models/google_translate_web.py`

 * *Files identical despite different names*

### Comparing `django_text_translator-2024.4.23/django_text_translator/models/microsoft_translate.py` & `django_text_translator-2024.4.25/django_text_translator/models/microsoft_translate.py`

 * *Files identical despite different names*

### Comparing `django_text_translator-2024.4.23/django_text_translator/models/moonshotai.py` & `django_text_translator-2024.4.25/django_text_translator/models/moonshotai.py`

 * *Files identical despite different names*

### Comparing `django_text_translator-2024.4.23/django_text_translator/static/img/icon-loading.svg` & `django_text_translator-2024.4.25/django_text_translator/static/img/icon-loading.svg`

 * *Files identical despite different names*

### Comparing `django_text_translator-2024.4.23/LICENSE` & `django_text_translator-2024.4.25/LICENSE`

 * *Files identical despite different names*

### Comparing `django_text_translator-2024.4.23/README.md` & `django_text_translator-2024.4.25/README.md`

 * *Files identical despite different names*

### Comparing `django_text_translator-2024.4.23/pyproject.toml` & `django_text_translator-2024.4.25/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 [tool.hatch.build.targets.wheel]
 packages = ["./"]
 
 [project]
 name = "django-text-translator"
-version = "2024.4.23"
+version = "2024.4.25"
 authors = [
   { name="Versun", email="django-text-translator@versun.me" },
 ]
 description = "A Django application that supports adding multiple third-party engines for text translation."
 readme = "README.md"
 requires-python = ">=3.10"
 license = {text = "MIT License"}
```

### Comparing `django_text_translator-2024.4.23/PKG-INFO` & `django_text_translator-2024.4.25/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: django-text-translator
-Version: 2024.4.23
+Version: 2024.4.25
 Summary: A Django application that supports adding multiple third-party engines for text translation.
 Project-URL: Homepage, https://github.com/rss-translator/django-text-translator
 Project-URL: Repository, https://github.com/rss-translator/django-text-translator.git
 Project-URL: Issues, https://github.com/rss-translator/django-text-translator/issues
 Author-email: Versun <django-text-translator@versun.me>
 License: MIT License
 License-File: LICENSE
```


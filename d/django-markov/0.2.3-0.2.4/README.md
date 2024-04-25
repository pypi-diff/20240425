# Comparing `tmp/django_markov-0.2.3.tar.gz` & `tmp/django_markov-0.2.4.tar.gz`

## Comparing `django_markov-0.2.3.tar` & `django_markov-0.2.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 django_markov-0.2.3/src/django_markov/__init__.py
--rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 django_markov-0.2.3/src/django_markov/admin.py
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 django_markov-0.2.3/src/django_markov/apps.py
--rw-r--r--   0        0        0    12168 2020-02-02 00:00:00.000000 django_markov-0.2.3/src/django_markov/models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_markov-0.2.3/src/django_markov/py.typed
--rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 django_markov-0.2.3/src/django_markov/text_models.py
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 django_markov-0.2.3/src/django_markov/urls.py
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 django_markov-0.2.3/src/django_markov/views.py
--rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 django_markov-0.2.3/src/django_markov/migrations/0001_initial.py
--rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 django_markov-0.2.3/src/django_markov/migrations/0002_alter_markovtextmodel_created_and_more.py
--rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 django_markov-0.2.3/src/django_markov/migrations/0003_markovtextmodel_compiled.py
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 django_markov-0.2.3/src/django_markov/migrations/0004_remove_markovtextmodel_compiled.py
--rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 django_markov-0.2.3/src/django_markov/migrations/0005_alter_markovtextmodel_data.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_markov-0.2.3/src/django_markov/migrations/__init__.py
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 django_markov-0.2.3/tests/__init__.py
--rw-r--r--   0        0        0     5850 2020-02-02 00:00:00.000000 django_markov-0.2.3/tests/settings.py
--rw-r--r--   0        0        0     7838 2020-02-02 00:00:00.000000 django_markov-0.2.3/tests/test_models.py
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 django_markov-0.2.3/tests/urls.py
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 django_markov-0.2.3/.gitignore
--rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 django_markov-0.2.3/LICENSE
--rw-r--r--   0        0        0     6834 2020-02-02 00:00:00.000000 django_markov-0.2.3/README.md
--rw-r--r--   0        0        0     5873 2020-02-02 00:00:00.000000 django_markov-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     8290 2020-02-02 00:00:00.000000 django_markov-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 django_markov-0.2.4/src/django_markov/__init__.py
+-rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 django_markov-0.2.4/src/django_markov/admin.py
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 django_markov-0.2.4/src/django_markov/apps.py
+-rw-r--r--   0        0        0    13249 2020-02-02 00:00:00.000000 django_markov-0.2.4/src/django_markov/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_markov-0.2.4/src/django_markov/py.typed
+-rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 django_markov-0.2.4/src/django_markov/text_models.py
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 django_markov-0.2.4/src/django_markov/urls.py
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 django_markov-0.2.4/src/django_markov/views.py
+-rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 django_markov-0.2.4/src/django_markov/migrations/0001_initial.py
+-rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 django_markov-0.2.4/src/django_markov/migrations/0002_alter_markovtextmodel_created_and_more.py
+-rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 django_markov-0.2.4/src/django_markov/migrations/0003_markovtextmodel_compiled.py
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 django_markov-0.2.4/src/django_markov/migrations/0004_remove_markovtextmodel_compiled.py
+-rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 django_markov-0.2.4/src/django_markov/migrations/0005_alter_markovtextmodel_data.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_markov-0.2.4/src/django_markov/migrations/__init__.py
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 django_markov-0.2.4/tests/__init__.py
+-rw-r--r--   0        0        0     5919 2020-02-02 00:00:00.000000 django_markov-0.2.4/tests/settings.py
+-rw-r--r--   0        0        0     9099 2020-02-02 00:00:00.000000 django_markov-0.2.4/tests/test_models.py
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 django_markov-0.2.4/tests/urls.py
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 django_markov-0.2.4/.gitignore
+-rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 django_markov-0.2.4/LICENSE
+-rw-r--r--   0        0        0     7215 2020-02-02 00:00:00.000000 django_markov-0.2.4/README.md
+-rw-r--r--   0        0        0     5873 2020-02-02 00:00:00.000000 django_markov-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     8671 2020-02-02 00:00:00.000000 django_markov-0.2.4/PKG-INFO
```

### Comparing `django_markov-0.2.3/src/django_markov/models.py` & `django_markov-0.2.4/src/django_markov/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,14 +43,28 @@
     if not hasattr(settings, "MARKOV_CORPUS_MAX_CHAR_LIMIT") or not isinstance(
         settings.MARKOV_CORPUS_MAX_CHAR_LIMIT, int
     ):
         return 0
     return settings.MARKOV_CORPUS_MAX_CHAR_LIMIT
 
 
+def _get_default_state_size() -> int:
+    """Get the state size from settings or return a
+    default value. A state size of 2 is the default for markovify.
+    """
+    if not hasattr(settings, "MARKOV_STATE_SIZE") or not isinstance(
+        settings.MARKOV_STATE_SIZE, int
+    ):
+        return 2
+    return settings.MARKOV_STATE_SIZE
+
+
+STATE_SIZE = _get_default_state_size()
+
+
 class MarkovTextModel(models.Model):
     """Stores a compiled markov text model.
 
     Attributes:
         created (datetime.datetime): Date and time when the model was created.
         modified (datetime.datetime): Date and time when the model was last modified.
         data (JSON): The text model as JSON.
@@ -102,14 +116,17 @@
         text_model = POSifiedText.from_json(self.data)
         return text_model
 
     @cached_property
     def is_compiled_model(self) -> bool:
         """
         Checks if the stored data for the text mile is compiled.
+
+        Raises:
+            MarkovEmptyError: if the model data is null.
         """
         text_model = self._as_text_model()
         if text_model is None:
             msg = "There is not data in this model and it cannot be inspected."
             raise MarkovEmptyError(msg)
         return text_model.chain.compiled
 
@@ -159,15 +176,15 @@
             store_compiled = settings.MARKOV_STORE_COMPILED_MODELS
         else:
             store_compiled = False
         corpus = " ".join(corpus_entries)
         if char_limit != 0 and char_limit < len(corpus):
             msg = f"Supplied corpus is over the maximum character limit: {char_limit}"
             raise ValueError(msg)
-        updated_model = POSifiedText(corpus)
+        updated_model = POSifiedText(corpus, state_size=STATE_SIZE)
         if store_compiled:
             updated_model.compile(inplace=True)
         self.data = updated_model.to_json()
         await self.asave()
 
     def update_model_from_corpus(
         self,
@@ -258,38 +275,50 @@
                 persisted to the database or a POSifiedText object to manipulate at a
                 low level, and the total number of models combined.
         """
         # First we check to ensure that the models are combinable.
         empty_models = []
         compiled_models = []
         workable_models = []
+        invalid_state_sizes = []
         if mode not in ["strict", "permissive"]:
             msg = f"Invalid mode: {mode}. Must be one of 'strict' or 'permissive'!"
             raise ValueError(msg)
         if weights is not None and mode != "strict":
             msg = "Weights can only be provided if mode is set to strict!"
             raise ValueError(msg)
         if return_type not in ["model_instance", "text_model"]:
             msg = (
                 f"Invalid return_type of {return_type} requested. Must be one of "
                 "'model_instance' or 'text_model'"
             )
             raise ValueError(msg)
+        current_state_size = 0
         for model in models:
             if not model.is_ready:
                 empty_models.append(model)
             else:
                 tm = model._as_text_model()
-                if tm and tm.chain.compiled:
-                    compiled_models.append(model)
+                if tm is None:
+                    empty_models.append(
+                        model
+                    )  # no cov, catchall to make pyright happy.
                 else:
-                    workable_models.append(model)
+                    if current_state_size == 0:
+                        current_state_size = tm.state_size
+                    if tm.state_size != current_state_size:
+                        invalid_state_sizes.append(model)
+                    elif tm and tm.chain.compiled:
+                        compiled_models.append(model)
+                    else:
+                        workable_models.append(model)
         if mode == "strict":
-            if empty_models or compiled_models:
-                msg = f"There are {len(compiled_models)} compiled models "
+            if empty_models or compiled_models or invalid_state_sizes:
+                msg = f"There are {len(compiled_models)} compiled models, "
+                f"{len(invalid_state_sizes)} models with incompatible state sizes, "
                 f"and {len(empty_models)} empty models in set!"
                 raise MarkovCombineError(msg)
         if len(workable_models) <= 1:
             msg = f"There is only {len(workable_models)}. Cannot combine!"
             raise MarkovCombineError(msg)
         models_combined = len(workable_models)
         try:
```

### Comparing `django_markov-0.2.3/src/django_markov/text_models.py` & `django_markov-0.2.4/src/django_markov/text_models.py`

 * *Files identical despite different names*

### Comparing `django_markov-0.2.3/src/django_markov/migrations/0001_initial.py` & `django_markov-0.2.4/src/django_markov/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_markov-0.2.3/src/django_markov/migrations/0002_alter_markovtextmodel_created_and_more.py` & `django_markov-0.2.4/src/django_markov/migrations/0002_alter_markovtextmodel_created_and_more.py`

 * *Files identical despite different names*

### Comparing `django_markov-0.2.3/src/django_markov/migrations/0003_markovtextmodel_compiled.py` & `django_markov-0.2.4/src/django_markov/migrations/0003_markovtextmodel_compiled.py`

 * *Files identical despite different names*

### Comparing `django_markov-0.2.3/tests/settings.py` & `django_markov-0.2.4/tests/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -188,7 +188,8 @@
 # https://docs.djangoproject.com/en/dev/ref/settings/#email-backend
 EMAIL_BACKEND = "django.core.mail.backends.locmem.EmailBackend"
 
 MARKOV_CORPUS_MAX_CHAR_LIMIT = env("DJANGO_MARKOV_MAX_CHAR_LIMIT", cast=int, default=0)  # type: ignore
 MARKOV_STORE_COMPILED_MODELS = env.bool(
     "DJANGO_MARKOV_STORE_COMPILED_MODELS", default=True
 )
+MARKOV_STATE_SIZE = 2  # What state size to use for the text models.
```

### Comparing `django_markov-0.2.3/tests/test_models.py` & `django_markov-0.2.4/tests/test_models.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from faker import Faker
 
 from django_markov.models import (
     MarkovCombineError,
     MarkovEmptyError,
     MarkovTextModel,
     _get_corpus_char_limit,
+    _get_default_state_size,
 )
 from django_markov.text_models import POSifiedText
 
 pytestmark = pytest.mark.django_db(transaction=True)
 
 
 @pytest.mark.parametrize(
@@ -38,14 +39,34 @@
 
 
 def test_get_char_limit_missing_settings(settings):
     del settings.MARKOV_CORPUS_MAX_CHAR_LIMIT
     assert _get_corpus_char_limit() == 0  # Setting was not present
 
 
+@pytest.mark.parametrize(
+    "override_value,expected_result",
+    [
+        (None, 2),
+        ("I'm a string!", 2),
+        (3, 3),
+    ],
+)
+def test_get_setting_state_size(
+    settings, override_value: int | None, expected_result
+) -> None:
+    settings.MARKOV_STATE_SIZE = override_value
+    assert _get_default_state_size() == expected_result
+
+
+def test_get_state_size_missing_settings(settings):
+    del settings.MARKOV_STATE_SIZE
+    assert _get_default_state_size() == 2  # noqa: PLR2004
+
+
 def test_text_models_return_none_on_empty_directive():
     model = MarkovTextModel.objects.create()
     assert not model._as_text_model()
     assert not model._compiled_model
 
 
 def test_do_not_recompile_compiled_model(compiled_model):
@@ -195,14 +216,35 @@
             mode=mode,
             return_type=return_type,
             weights=weights,
         )
 
 
 @pytest.mark.asyncio
+async def test_combine_different_state_sizes(sample_corpus) -> None:
+    new_model = await MarkovTextModel.objects.acreate()
+    next_model = await MarkovTextModel.objects.acreate()
+    await new_model.aupdate_model_from_corpus(
+        corpus_entries=[
+            sample_corpus,
+            "I've got a state size of 2, which is the default.",
+        ],
+        store_compiled=False,
+        char_limit=0,
+    )
+    text_state_3 = POSifiedText(sample_corpus, state_size=3)
+    next_model.data = text_state_3.to_json()
+    await next_model.asave()
+    with pytest.raises(MarkovCombineError):
+        await MarkovTextModel.acombine_models(
+            models=[new_model, next_model], mode="strict"
+        )
+
+
+@pytest.mark.asyncio
 @pytest.mark.parametrize(
     "num_clean,num_empty,num_compiled,mode,result_type,weights,expected_result_type",
     [
         (3, 0, 0, "strict", "model_instance", [1.0, 1.0, 1.0], MarkovTextModel),
         (3, 0, 0, "strict", "text_model", [1.0, 1.0, 1.0], POSifiedText),
         (3, 0, 0, "strict", "model_instance", None, MarkovTextModel),
         (3, 0, 0, "strict", "text_model", None, POSifiedText),
```

### Comparing `django_markov-0.2.3/tests/urls.py` & `django_markov-0.2.4/tests/urls.py`

 * *Files identical despite different names*

### Comparing `django_markov-0.2.3/LICENSE` & `django_markov-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `django_markov-0.2.3/README.md` & `django_markov-0.2.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -61,14 +61,22 @@
 # Compile text models by default when writing to database.
 # Compiled models are significantly more performant when
 # generating sentences, but they cannot be chained with other
 # model without parsing the entire corpus again.
 # What's best will depend on your use case. If you don't intend
 # to combine multiple models, you'll want this set to True.
 MARKOV_STORE_COMPILED_MODELS = True
+
+# Specify a state size for generated models. State size is the
+# number of words the probability of a next word depends on.
+# The default for the markovify library is 2.
+# NOTE: models with different state sizes cannot be combined
+# with one another. If you change this setting after creating
+# models, you should regenerate them with their original corpus.
+MARKOV_STATE_SIZE = 2
 ```
 
 Then run migrations as usual.
 
 ```bash
 python manage.py migrate
 ```
```

### Comparing `django_markov-0.2.3/pyproject.toml` & `django_markov-0.2.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "django-markov"
-version = "0.2.3"
+version = "0.2.4"
 description = "django-markov is a reusable Django app that enables you to create Markov text models, and store them in the database. Those models can then be used to generate Markov chain sentences."
 authors = [
     { name = "Daniel Andrlik", email = "daniel@andrlik.org" }
 ]
 dependencies = [
     "django>=4.2",
     "markovify>=0.9.4",
@@ -224,15 +224,15 @@
   "--reuse-db"
 ]
 
 [tool.check-wheel-contents]
 ignore = ["W004"]
 
 [tool.bumpversion]
-current_version = "0.2.3"
+current_version = "0.2.4"
 parse = "(?P<major>\\d+)\\.(?P<minor>\\d+)\\.(?P<patch>\\d+)"
 serialize = ["{major}.{minor}.{patch}"]
 search = "{current_version}"
 replace = "{new_version}"
 regex = false
 ignore_missing_version = false
 tag = true
```

### Comparing `django_markov-0.2.3/PKG-INFO` & `django_markov-0.2.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: django-markov
-Version: 0.2.3
+Version: 0.2.4
 Summary: django-markov is a reusable Django app that enables you to create Markov text models, and store them in the database. Those models can then be used to generate Markov chain sentences.
 Project-URL: Repository, https://github.com/andrlik/django-markov
 Project-URL: Documentation, https://andrlik.github.io/django-markov
 Project-URL: Homepage, https://andrlik.github.io/django-markov
 Author-email: Daniel Andrlik <daniel@andrlik.org>
 License-Expression: BSD-3-Clause
 License-File: LICENSE
@@ -94,14 +94,22 @@
 # Compile text models by default when writing to database.
 # Compiled models are significantly more performant when
 # generating sentences, but they cannot be chained with other
 # model without parsing the entire corpus again.
 # What's best will depend on your use case. If you don't intend
 # to combine multiple models, you'll want this set to True.
 MARKOV_STORE_COMPILED_MODELS = True
+
+# Specify a state size for generated models. State size is the
+# number of words the probability of a next word depends on.
+# The default for the markovify library is 2.
+# NOTE: models with different state sizes cannot be combined
+# with one another. If you change this setting after creating
+# models, you should regenerate them with their original corpus.
+MARKOV_STATE_SIZE = 2
 ```
 
 Then run migrations as usual.
 
 ```bash
 python manage.py migrate
 ```
```


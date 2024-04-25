# Comparing `tmp/kinya_tn-0.0.1.tar.gz` & `tmp/kinya_tn-0.0.1.1.tar.gz`

## Comparing `kinya_tn-0.0.1.tar` & `kinya_tn-0.0.1.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 kinya_tn-0.0.1/src/kinya_tn/__init__.py
--rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 kinya_tn-0.0.1/src/kinya_tn/text_normalization.py
--rw-r--r--   0        0        0  3205359 2020-02-02 00:00:00.000000 kinya_tn-0.0.1/src/kinya_tn/tokenize_and_classify.far
--rw-r--r--   0        0        0  1134472 2020-02-02 00:00:00.000000 kinya_tn-0.0.1/src/kinya_tn/verbalize.far
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 kinya_tn-0.0.1/LICENSE
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 kinya_tn-0.0.1/README.md
--rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 kinya_tn-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 kinya_tn-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 kinya_tn-0.0.1.1/src/kinya_tn/__init__.py
+-rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 kinya_tn-0.0.1.1/src/kinya_tn/text_normalization.py
+-rw-r--r--   0        0        0  3205359 2020-02-02 00:00:00.000000 kinya_tn-0.0.1.1/src/kinya_tn/tokenize_and_classify.far
+-rw-r--r--   0        0        0  1134472 2020-02-02 00:00:00.000000 kinya_tn-0.0.1.1/src/kinya_tn/verbalize.far
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 kinya_tn-0.0.1.1/LICENSE
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 kinya_tn-0.0.1.1/README.md
+-rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 kinya_tn-0.0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 kinya_tn-0.0.1.1/PKG-INFO
```

### Comparing `kinya_tn-0.0.1/src/kinya_tn/text_normalization.py` & `kinya_tn-0.0.1.1/src/kinya_tn/text_normalization.py`

 * *Files identical despite different names*

### Comparing `kinya_tn-0.0.1/src/kinya_tn/tokenize_and_classify.far` & `kinya_tn-0.0.1.1/src/kinya_tn/tokenize_and_classify.far`

 * *Files identical despite different names*

### Comparing `kinya_tn-0.0.1/src/kinya_tn/verbalize.far` & `kinya_tn-0.0.1.1/src/kinya_tn/verbalize.far`

 * *Files identical despite different names*

### Comparing `kinya_tn-0.0.1/LICENSE` & `kinya_tn-0.0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `kinya_tn-0.0.1/pyproject.toml` & `kinya_tn-0.0.1.1/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 [build-system]
 requires = ["hatchling","pynini"]
 build-backend = "hatchling.build"
 
 
 [project]
 name="kinya_tn"
-version = "0.0.1"
+version = "0.0.1.1"
+dependencies = ['pynini']
 authors = [
   { name="DigitalUmuganda", email="samuel@digitalumuganda.com" },
 ]
 description = "A small package that convert time, cardinal numbers, some acronyms and transliterations cases from their written form to their verbalized form. It can be used to normalize text before feeding it into a text-to-speech model."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `kinya_tn-0.0.1/PKG-INFO` & `kinya_tn-0.0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.3
 Name: kinya_tn
-Version: 0.0.1
+Version: 0.0.1.1
 Summary: A small package that convert time, cardinal numbers, some acronyms and transliterations cases from their written form to their verbalized form. It can be used to normalize text before feeding it into a text-to-speech model.
 Project-URL: Homepage, https://github.com/Digital-Umuganda/text_normalization_tts_rw/
 Project-URL: Issues, https://github.com/Digital-Umuganda/text_normalization_tts_rw/issues
 Author-email: DigitalUmuganda <samuel@digitalumuganda.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
+Requires-Dist: pynini
 Description-Content-Type: text/markdown
 
 # Kinya_TN
 
 Kinyarwanda_TextNormalization(Kinya_TN) is a small package that convert time, cardinal numbers, some acronyms and transliterations cases from their written form to their verbalized form. It can be used to preprocess text to an adequate form for text-to-speech models.
 
 ## Installation
```


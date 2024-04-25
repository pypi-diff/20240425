# Comparing `tmp/gliner-spacy-0.0.5.tar.gz` & `tmp/gliner-spacy-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gliner-spacy-0.0.5.tar", last modified: Sun Apr 21 00:51:06 2024, max compression
+gzip compressed data, was "gliner-spacy-0.0.6.tar", last modified: Thu Apr 25 03:57:02 2024, max compression
```

## Comparing `gliner-spacy-0.0.5.tar` & `gliner-spacy-0.0.6.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 wjbmattingly   (501) staff       (20)        0 2024-04-21 00:51:06.369721 gliner-spacy-0.0.5/
--rw-r--r--   0 wjbmattingly   (501) staff       (20)     1073 2024-04-08 09:18:42.000000 gliner-spacy-0.0.5/LICENSE
--rw-r--r--   0 wjbmattingly   (501) staff       (20)     3360 2024-04-21 00:51:06.369611 gliner-spacy-0.0.5/PKG-INFO
--rw-r--r--   0 wjbmattingly   (501) staff       (20)     2651 2024-04-08 09:20:31.000000 gliner-spacy-0.0.5/README.md
-drwxr-xr-x   0 wjbmattingly   (501) staff       (20)        0 2024-04-21 00:51:06.368986 gliner-spacy-0.0.5/gliner_spacy/
--rw-r--r--   0 wjbmattingly   (501) staff       (20)       27 2024-03-09 11:26:23.000000 gliner-spacy-0.0.5/gliner_spacy/__init__.py
--rw-r--r--   0 wjbmattingly   (501) staff       (20)     2934 2024-04-21 00:49:34.000000 gliner-spacy-0.0.5/gliner_spacy/pipeline.py
-drwxr-xr-x   0 wjbmattingly   (501) staff       (20)        0 2024-04-21 00:51:06.369471 gliner-spacy-0.0.5/gliner_spacy.egg-info/
--rw-r--r--   0 wjbmattingly   (501) staff       (20)     3360 2024-04-21 00:51:06.000000 gliner-spacy-0.0.5/gliner_spacy.egg-info/PKG-INFO
--rw-r--r--   0 wjbmattingly   (501) staff       (20)      255 2024-04-21 00:51:06.000000 gliner-spacy-0.0.5/gliner_spacy.egg-info/SOURCES.txt
--rw-r--r--   0 wjbmattingly   (501) staff       (20)        1 2024-04-21 00:51:06.000000 gliner-spacy-0.0.5/gliner_spacy.egg-info/dependency_links.txt
--rw-r--r--   0 wjbmattingly   (501) staff       (20)       13 2024-04-21 00:51:06.000000 gliner-spacy-0.0.5/gliner_spacy.egg-info/requires.txt
--rw-r--r--   0 wjbmattingly   (501) staff       (20)       13 2024-04-21 00:51:06.000000 gliner-spacy-0.0.5/gliner_spacy.egg-info/top_level.txt
--rw-r--r--   0 wjbmattingly   (501) staff       (20)       38 2024-04-21 00:51:06.369757 gliner-spacy-0.0.5/setup.cfg
--rw-r--r--   0 wjbmattingly   (501) staff       (20)     1088 2024-04-21 00:50:18.000000 gliner-spacy-0.0.5/setup.py
+drwxr-xr-x   0 wjbmattingly   (501) staff       (20)        0 2024-04-25 03:57:02.970188 gliner-spacy-0.0.6/
+-rw-r--r--   0 wjbmattingly   (501) staff       (20)     1073 2024-04-08 09:18:42.000000 gliner-spacy-0.0.6/LICENSE
+-rw-r--r--   0 wjbmattingly   (501) staff       (20)     3435 2024-04-25 03:57:02.970073 gliner-spacy-0.0.6/PKG-INFO
+-rw-r--r--   0 wjbmattingly   (501) staff       (20)     2727 2024-04-25 03:43:07.000000 gliner-spacy-0.0.6/README.md
+drwxr-xr-x   0 wjbmattingly   (501) staff       (20)        0 2024-04-25 03:57:02.969331 gliner-spacy-0.0.6/gliner_spacy/
+-rw-r--r--   0 wjbmattingly   (501) staff       (20)       60 2024-04-25 03:46:10.000000 gliner-spacy-0.0.6/gliner_spacy/__init__.py
+-rw-r--r--   0 wjbmattingly   (501) staff       (20)     2895 2024-04-25 03:41:51.000000 gliner-spacy-0.0.6/gliner_spacy/pipeline.py
+-rw-r--r--   0 wjbmattingly   (501) staff       (20)       22 2024-04-25 03:37:21.000000 gliner-spacy-0.0.6/gliner_spacy/version.py
+drwxr-xr-x   0 wjbmattingly   (501) staff       (20)        0 2024-04-25 03:57:02.969913 gliner-spacy-0.0.6/gliner_spacy.egg-info/
+-rw-r--r--   0 wjbmattingly   (501) staff       (20)     3435 2024-04-25 03:57:02.000000 gliner-spacy-0.0.6/gliner_spacy.egg-info/PKG-INFO
+-rw-r--r--   0 wjbmattingly   (501) staff       (20)      279 2024-04-25 03:57:02.000000 gliner-spacy-0.0.6/gliner_spacy.egg-info/SOURCES.txt
+-rw-r--r--   0 wjbmattingly   (501) staff       (20)        1 2024-04-25 03:57:02.000000 gliner-spacy-0.0.6/gliner_spacy.egg-info/dependency_links.txt
+-rw-r--r--   0 wjbmattingly   (501) staff       (20)       13 2024-04-25 03:57:02.000000 gliner-spacy-0.0.6/gliner_spacy.egg-info/requires.txt
+-rw-r--r--   0 wjbmattingly   (501) staff       (20)       13 2024-04-25 03:57:02.000000 gliner-spacy-0.0.6/gliner_spacy.egg-info/top_level.txt
+-rw-r--r--   0 wjbmattingly   (501) staff       (20)       38 2024-04-25 03:57:02.970231 gliner-spacy-0.0.6/setup.cfg
+-rw-r--r--   0 wjbmattingly   (501) staff       (20)     1295 2024-04-25 03:43:39.000000 gliner-spacy-0.0.6/setup.py
```

### Comparing `gliner-spacy-0.0.5/LICENSE` & `gliner-spacy-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `gliner-spacy-0.0.5/PKG-INFO` & `gliner-spacy-0.0.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 Metadata-Version: 2.1
 Name: gliner-spacy
-Version: 0.0.5
+Version: 0.0.6
 Summary: A SpaCy wrapper for the GLiNER model for enhanced Named Entity Recognition capabilities
 Home-page: https://github.com/theirstory/gliner-spacy
 Author: William J. B. Mattingly
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7,<=3.10
+Requires-Python: >=3.7,<3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # GLiNER SpaCy Wrapper
 
 ## Introduction
 This project is a wrapper for integrating [GLiNER](https://github.com/urchade/GLiNER), a Named Entity Recognition (NER) model, with the SpaCy Natural Language Processing (NLP) library. GLiNER, which stands for Generalized Language INdependent Entity Recognition, is an advanced model for recognizing entities in text. The SpaCy wrapper enables easy integration and use of GLiNER within the SpaCy environment, enhancing NER capabilities with GLiNER's advanced features.
 
+**For GliNER to work properly, you need to use a Python version 3.7-3.10**
+
 ## Features
 - Integrates GLiNER with SpaCy for advanced NER tasks.
 - Customizable chunk size for processing large texts.
 - Support for specific entity labels like 'person' and 'organization'.
 - Configurable output style for entity recognition results.
 
 ## Installation
```

### Comparing `gliner-spacy-0.0.5/README.md` & `gliner-spacy-0.0.6/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # GLiNER SpaCy Wrapper
 
 ## Introduction
 This project is a wrapper for integrating [GLiNER](https://github.com/urchade/GLiNER), a Named Entity Recognition (NER) model, with the SpaCy Natural Language Processing (NLP) library. GLiNER, which stands for Generalized Language INdependent Entity Recognition, is an advanced model for recognizing entities in text. The SpaCy wrapper enables easy integration and use of GLiNER within the SpaCy environment, enhancing NER capabilities with GLiNER's advanced features.
 
+**For GliNER to work properly, you need to use a Python version 3.7-3.10**
+
 ## Features
 - Integrates GLiNER with SpaCy for advanced NER tasks.
 - Customizable chunk size for processing large texts.
 - Support for specific entity labels like 'person' and 'organization'.
 - Configurable output style for entity recognition results.
 
 ## Installation
```

### Comparing `gliner-spacy-0.0.5/gliner_spacy/pipeline.py` & `gliner-spacy-0.0.6/gliner_spacy/pipeline.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,15 +26,15 @@
                  threshold: float
                  ):
         
         self.nlp = nlp
         self.model = GLiNER.from_pretrained(gliner_model)
         self.labels = labels
         self.chunk_size = chunk_size
-        self.style = style  # Store style as an instance variable
+        self.style = style
         self.threshold = threshold
 
     def __call__(self, doc):
         # Tokenize the text
         chunks = []
         start = 0
         text = doc.text
```

### Comparing `gliner-spacy-0.0.5/gliner_spacy.egg-info/PKG-INFO` & `gliner-spacy-0.0.6/gliner_spacy.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 Metadata-Version: 2.1
 Name: gliner-spacy
-Version: 0.0.5
+Version: 0.0.6
 Summary: A SpaCy wrapper for the GLiNER model for enhanced Named Entity Recognition capabilities
 Home-page: https://github.com/theirstory/gliner-spacy
 Author: William J. B. Mattingly
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7,<=3.10
+Requires-Python: >=3.7,<3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # GLiNER SpaCy Wrapper
 
 ## Introduction
 This project is a wrapper for integrating [GLiNER](https://github.com/urchade/GLiNER), a Named Entity Recognition (NER) model, with the SpaCy Natural Language Processing (NLP) library. GLiNER, which stands for Generalized Language INdependent Entity Recognition, is an advanced model for recognizing entities in text. The SpaCy wrapper enables easy integration and use of GLiNER within the SpaCy environment, enhancing NER capabilities with GLiNER's advanced features.
 
+**For GliNER to work properly, you need to use a Python version 3.7-3.10**
+
 ## Features
 - Integrates GLiNER with SpaCy for advanced NER tasks.
 - Customizable chunk size for processing large texts.
 - Support for specific entity labels like 'person' and 'organization'.
 - Configurable output style for entity recognition results.
 
 ## Installation
```


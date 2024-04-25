# Comparing `tmp/sigmund-0.16.1.tar.gz` & `tmp/sigmund-0.16.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sigmund-0.16.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "sigmund-0.16.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `sigmund-0.16.1.tar` & `sigmund-0.16.2.tar`

### file list

```diff
@@ -1,58 +1,58 @@
--rw-r--r--   0        0        0    35147 2024-04-25 09:20:53.712593 sigmund-0.16.1/COPYING
--rw-r--r--   0        0        0     1017 2024-04-25 09:20:53.712593 sigmund-0.16.1/pyproject.toml
--rw-r--r--   0        0        0     3037 2024-04-25 09:20:53.712593 sigmund-0.16.1/readme.md
--rw-r--r--   0        0        0      101 2024-04-25 09:20:53.712593 sigmund-0.16.1/sigmund/__init__.py
--rw-r--r--   0        0        0     2746 2024-04-25 09:20:53.712593 sigmund-0.16.1/sigmund/attachments.py
--rw-r--r--   0        0        0     9696 2024-04-25 09:20:53.712593 sigmund-0.16.1/sigmund/config.py
--rw-r--r--   0        0        0        0 2024-04-25 09:20:53.712593 sigmund-0.16.1/sigmund/database/__init__.py
--rw-r--r--   0        0        0     1030 2024-04-25 09:20:53.712593 sigmund-0.16.1/sigmund/database/encryption.py
--rw-r--r--   0        0        0    14378 2024-04-25 09:20:53.712593 sigmund-0.16.1/sigmund/database/manager.py
--rw-r--r--   0        0        0     3213 2024-04-25 09:20:53.712593 sigmund-0.16.1/sigmund/database/models.py
--rw-r--r--   0        0        0     4630 2024-04-25 09:20:53.712593 sigmund-0.16.1/sigmund/documentation.py
--rw-r--r--   0        0        0      389 2024-04-25 09:20:53.712593 sigmund-0.16.1/sigmund/forms.py
--rw-r--r--   0        0        0     2547 2024-04-25 09:20:53.712593 sigmund-0.16.1/sigmund/library.py
--rw-r--r--   0        0        0    10115 2024-04-25 09:20:53.712593 sigmund-0.16.1/sigmund/messages.py
--rw-r--r--   0        0        0     1263 2024-04-25 09:20:53.712593 sigmund-0.16.1/sigmund/model/__init__.py
--rw-r--r--   0        0        0     5297 2024-04-25 09:20:53.712593 sigmund-0.16.1/sigmund/model/_anthropic_model.py
--rw-r--r--   0        0        0     4573 2024-04-25 09:20:53.712593 sigmund-0.16.1/sigmund/model/_base_model.py
--rw-r--r--   0        0        0      379 2024-04-25 09:20:53.712593 sigmund-0.16.1/sigmund/model/_dummy_model.py
--rw-r--r--   0        0        0     2608 2024-04-25 09:20:53.712593 sigmund-0.16.1/sigmund/model/_mistral_model.py
--rw-r--r--   0        0        0     3273 2024-04-25 09:20:53.712593 sigmund-0.16.1/sigmund/model/_openai_model.py
--rw-r--r--   0        0        0     1980 2024-04-25 09:20:53.712593 sigmund-0.16.1/sigmund/prompt.py
--rw-r--r--   0        0        0      160 2024-04-25 09:20:53.712593 sigmund-0.16.1/sigmund/routes/__init__.py
--rw-r--r--   0        0        0     7298 2024-04-25 09:20:53.712593 sigmund-0.16.1/sigmund/routes/api.py
--rw-r--r--   0        0        0     5775 2024-04-25 09:20:53.712593 sigmund-0.16.1/sigmund/routes/app.py
--rw-r--r--   0        0        0     3606 2024-04-25 09:20:53.712593 sigmund-0.16.1/sigmund/routes/google_login.py
--rw-r--r--   0        0        0     7732 2024-04-25 09:20:53.712593 sigmund-0.16.1/sigmund/routes/subscribe.py
--rw-r--r--   0        0        0     1494 2024-04-25 09:20:53.712593 sigmund-0.16.1/sigmund/server.py
--rw-r--r--   0        0        0     9354 2024-04-25 09:20:53.712593 sigmund-0.16.1/sigmund/sigmund.py
--rw-r--r--   0        0        0     4270 2024-04-25 09:20:53.712593 sigmund-0.16.1/sigmund/static/about.md
--rw-r--r--   0        0        0  4708018 2024-04-25 09:20:53.720594 sigmund-0.16.1/sigmund/static/background.png
--rw-r--r--   0        0        0      386 2024-04-25 09:20:53.720594 sigmund-0.16.1/sigmund/static/favicon.svg
--rw-r--r--   0        0        0     1433 2024-04-25 09:20:53.720594 sigmund-0.16.1/sigmund/static/login.md
--rw-r--r--   0        0        0     4976 2024-04-25 09:20:53.720594 sigmund-0.16.1/sigmund/static/pygments.css
--rw-r--r--   0        0        0   708136 2024-04-25 09:20:53.724593 sigmund-0.16.1/sigmund/static/sofa-with-sigmund.png
--rw-r--r--   0        0        0   684883 2024-04-25 09:20:53.724593 sigmund-0.16.1/sigmund/static/sofa.png
--rw-r--r--   0        0        0     3428 2024-04-25 09:20:53.724593 sigmund-0.16.1/sigmund/static/terms.md
--rw-r--r--   0        0        0     1359 2024-04-25 09:20:53.724593 sigmund-0.16.1/sigmund/templates/chat.html
--rw-r--r--   0        0        0      242 2024-04-25 09:20:53.724593 sigmund-0.16.1/sigmund/templates/footer.html
--rw-r--r--   0        0        0      574 2024-04-25 09:20:53.724593 sigmund-0.16.1/sigmund/templates/head.html
--rw-r--r--   0        0        0      244 2024-04-25 09:20:53.724593 sigmund-0.16.1/sigmund/templates/header.html
--rw-r--r--   0        0        0      329 2024-04-25 09:20:53.724593 sigmund-0.16.1/sigmund/templates/info-page.html
--rw-r--r--   0        0        0     3739 2024-04-25 09:20:53.724593 sigmund-0.16.1/sigmund/templates/login.html
--rw-r--r--   0        0        0    10786 2024-04-25 09:20:53.724593 sigmund-0.16.1/sigmund/templates/main.js
--rw-r--r--   0        0        0    12359 2024-04-25 09:20:53.724593 sigmund-0.16.1/sigmund/templates/menu.html
--rw-r--r--   0        0        0       80 2024-04-25 09:20:53.724593 sigmund-0.16.1/sigmund/templates/sign-out.html
--rw-r--r--   0        0        0     6353 2024-04-25 09:20:53.724593 sigmund-0.16.1/sigmund/templates/stylesheet.css.jinja
--rw-r--r--   0        0        0      531 2024-04-25 09:20:53.724593 sigmund-0.16.1/sigmund/templates/subscribe-error.html
--rw-r--r--   0        0        0     1206 2024-04-25 09:20:53.724593 sigmund-0.16.1/sigmund/templates/subscribe-now.html
--rw-r--r--   0        0        0      515 2024-04-25 09:20:53.724593 sigmund-0.16.1/sigmund/templates/subscribe-success.html
--rw-r--r--   0        0        0      265 2024-04-25 09:20:53.724593 sigmund-0.16.1/sigmund/tools/__init__.py
--rw-r--r--   0        0        0     2231 2024-04-25 09:20:53.724593 sigmund-0.16.1/sigmund/tools/_base_tool.py
--rw-r--r--   0        0        0     2920 2024-04-25 09:20:53.724593 sigmund-0.16.1/sigmund/tools/_download.py
--rw-r--r--   0        0        0     2011 2024-04-25 09:20:53.724593 sigmund-0.16.1/sigmund/tools/_execute_code.py
--rw-r--r--   0        0        0     1846 2024-04-25 09:20:53.724593 sigmund-0.16.1/sigmund/tools/_read_attachment.py
--rw-r--r--   0        0        0     2211 2024-04-25 09:20:53.724593 sigmund-0.16.1/sigmund/tools/_search_documentation.py
--rw-r--r--   0        0        0     1275 2024-04-25 09:20:53.724593 sigmund-0.16.1/sigmund/tools/_search_google_scholar.py
--rw-r--r--   0        0        0     4358 2024-04-25 09:20:53.724593 sigmund-0.16.1/sigmund/utils.py
--rw-r--r--   0        0        0     4228 1970-01-01 00:00:00.000000 sigmund-0.16.1/PKG-INFO
+-rw-r--r--   0        0        0    35147 2024-04-25 16:09:18.866095 sigmund-0.16.2/COPYING
+-rw-r--r--   0        0        0     1017 2024-04-25 16:09:18.866095 sigmund-0.16.2/pyproject.toml
+-rw-r--r--   0        0        0     3037 2024-04-25 16:09:18.866095 sigmund-0.16.2/readme.md
+-rw-r--r--   0        0        0      101 2024-04-25 16:09:18.866095 sigmund-0.16.2/sigmund/__init__.py
+-rw-r--r--   0        0        0     2746 2024-04-25 16:09:18.866095 sigmund-0.16.2/sigmund/attachments.py
+-rw-r--r--   0        0        0     9770 2024-04-25 16:09:18.866095 sigmund-0.16.2/sigmund/config.py
+-rw-r--r--   0        0        0        0 2024-04-25 16:09:18.866095 sigmund-0.16.2/sigmund/database/__init__.py
+-rw-r--r--   0        0        0     1030 2024-04-25 16:09:18.866095 sigmund-0.16.2/sigmund/database/encryption.py
+-rw-r--r--   0        0        0    14378 2024-04-25 16:09:18.866095 sigmund-0.16.2/sigmund/database/manager.py
+-rw-r--r--   0        0        0     3213 2024-04-25 16:09:18.866095 sigmund-0.16.2/sigmund/database/models.py
+-rw-r--r--   0        0        0     5559 2024-04-25 16:09:18.866095 sigmund-0.16.2/sigmund/documentation.py
+-rw-r--r--   0        0        0      389 2024-04-25 16:09:18.866095 sigmund-0.16.2/sigmund/forms.py
+-rw-r--r--   0        0        0     2547 2024-04-25 16:09:18.866095 sigmund-0.16.2/sigmund/library.py
+-rw-r--r--   0        0        0    10115 2024-04-25 16:09:18.866095 sigmund-0.16.2/sigmund/messages.py
+-rw-r--r--   0        0        0     1263 2024-04-25 16:09:18.866095 sigmund-0.16.2/sigmund/model/__init__.py
+-rw-r--r--   0        0        0     5297 2024-04-25 16:09:18.866095 sigmund-0.16.2/sigmund/model/_anthropic_model.py
+-rw-r--r--   0        0        0     4573 2024-04-25 16:09:18.866095 sigmund-0.16.2/sigmund/model/_base_model.py
+-rw-r--r--   0        0        0      379 2024-04-25 16:09:18.866095 sigmund-0.16.2/sigmund/model/_dummy_model.py
+-rw-r--r--   0        0        0     2608 2024-04-25 16:09:18.866095 sigmund-0.16.2/sigmund/model/_mistral_model.py
+-rw-r--r--   0        0        0     3273 2024-04-25 16:09:18.866095 sigmund-0.16.2/sigmund/model/_openai_model.py
+-rw-r--r--   0        0        0     1980 2024-04-25 16:09:18.866095 sigmund-0.16.2/sigmund/prompt.py
+-rw-r--r--   0        0        0      160 2024-04-25 16:09:18.866095 sigmund-0.16.2/sigmund/routes/__init__.py
+-rw-r--r--   0        0        0     7298 2024-04-25 16:09:18.866095 sigmund-0.16.2/sigmund/routes/api.py
+-rw-r--r--   0        0        0     5775 2024-04-25 16:09:18.866095 sigmund-0.16.2/sigmund/routes/app.py
+-rw-r--r--   0        0        0     3606 2024-04-25 16:09:18.866095 sigmund-0.16.2/sigmund/routes/google_login.py
+-rw-r--r--   0        0        0     7732 2024-04-25 16:09:18.866095 sigmund-0.16.2/sigmund/routes/subscribe.py
+-rw-r--r--   0        0        0     1494 2024-04-25 16:09:18.866095 sigmund-0.16.2/sigmund/server.py
+-rw-r--r--   0        0        0     9354 2024-04-25 16:09:18.866095 sigmund-0.16.2/sigmund/sigmund.py
+-rw-r--r--   0        0        0     4270 2024-04-25 16:09:18.866095 sigmund-0.16.2/sigmund/static/about.md
+-rw-r--r--   0        0        0  4708018 2024-04-25 16:09:18.874095 sigmund-0.16.2/sigmund/static/background.png
+-rw-r--r--   0        0        0      386 2024-04-25 16:09:18.874095 sigmund-0.16.2/sigmund/static/favicon.svg
+-rw-r--r--   0        0        0     1433 2024-04-25 16:09:18.874095 sigmund-0.16.2/sigmund/static/login.md
+-rw-r--r--   0        0        0     4976 2024-04-25 16:09:18.874095 sigmund-0.16.2/sigmund/static/pygments.css
+-rw-r--r--   0        0        0   708136 2024-04-25 16:09:18.878095 sigmund-0.16.2/sigmund/static/sofa-with-sigmund.png
+-rw-r--r--   0        0        0   684883 2024-04-25 16:09:18.878095 sigmund-0.16.2/sigmund/static/sofa.png
+-rw-r--r--   0        0        0     3428 2024-04-25 16:09:18.878095 sigmund-0.16.2/sigmund/static/terms.md
+-rw-r--r--   0        0        0     1359 2024-04-25 16:09:18.878095 sigmund-0.16.2/sigmund/templates/chat.html
+-rw-r--r--   0        0        0      242 2024-04-25 16:09:18.878095 sigmund-0.16.2/sigmund/templates/footer.html
+-rw-r--r--   0        0        0      574 2024-04-25 16:09:18.878095 sigmund-0.16.2/sigmund/templates/head.html
+-rw-r--r--   0        0        0      244 2024-04-25 16:09:18.878095 sigmund-0.16.2/sigmund/templates/header.html
+-rw-r--r--   0        0        0      329 2024-04-25 16:09:18.878095 sigmund-0.16.2/sigmund/templates/info-page.html
+-rw-r--r--   0        0        0     3739 2024-04-25 16:09:18.878095 sigmund-0.16.2/sigmund/templates/login.html
+-rw-r--r--   0        0        0    10786 2024-04-25 16:09:18.878095 sigmund-0.16.2/sigmund/templates/main.js
+-rw-r--r--   0        0        0    12359 2024-04-25 16:09:18.878095 sigmund-0.16.2/sigmund/templates/menu.html
+-rw-r--r--   0        0        0       80 2024-04-25 16:09:18.878095 sigmund-0.16.2/sigmund/templates/sign-out.html
+-rw-r--r--   0        0        0     6353 2024-04-25 16:09:18.878095 sigmund-0.16.2/sigmund/templates/stylesheet.css.jinja
+-rw-r--r--   0        0        0      531 2024-04-25 16:09:18.878095 sigmund-0.16.2/sigmund/templates/subscribe-error.html
+-rw-r--r--   0        0        0     1555 2024-04-25 16:09:18.878095 sigmund-0.16.2/sigmund/templates/subscribe-now.html
+-rw-r--r--   0        0        0      515 2024-04-25 16:09:18.878095 sigmund-0.16.2/sigmund/templates/subscribe-success.html
+-rw-r--r--   0        0        0      265 2024-04-25 16:09:18.878095 sigmund-0.16.2/sigmund/tools/__init__.py
+-rw-r--r--   0        0        0     2231 2024-04-25 16:09:18.878095 sigmund-0.16.2/sigmund/tools/_base_tool.py
+-rw-r--r--   0        0        0     2920 2024-04-25 16:09:18.878095 sigmund-0.16.2/sigmund/tools/_download.py
+-rw-r--r--   0        0        0     2085 2024-04-25 16:09:18.878095 sigmund-0.16.2/sigmund/tools/_execute_code.py
+-rw-r--r--   0        0        0     1846 2024-04-25 16:09:18.878095 sigmund-0.16.2/sigmund/tools/_read_attachment.py
+-rw-r--r--   0        0        0     2211 2024-04-25 16:09:18.878095 sigmund-0.16.2/sigmund/tools/_search_documentation.py
+-rw-r--r--   0        0        0     1275 2024-04-25 16:09:18.878095 sigmund-0.16.2/sigmund/tools/_search_google_scholar.py
+-rw-r--r--   0        0        0     4358 2024-04-25 16:09:18.878095 sigmund-0.16.2/sigmund/utils.py
+-rw-r--r--   0        0        0     4228 1970-01-01 00:00:00.000000 sigmund-0.16.2/PKG-INFO
```

### Comparing `sigmund-0.16.1/COPYING` & `sigmund-0.16.2/COPYING`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.1/pyproject.toml` & `sigmund-0.16.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.1/readme.md` & `sigmund-0.16.2/readme.md`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.1/sigmund/attachments.py` & `sigmund-0.16.2/sigmund/attachments.py`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.1/sigmund/config.py` & `sigmund-0.16.2/sigmund/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -167,17 +167,18 @@
     'osweb': 'sources/topics/inline_javascript.js',
     'javascript': 'sources/topics/inline_javascript.js',
     'inline_javascript': 'sources/topics/inline_javascript.js',
     'datamatrix': 'sources/topics/datamatrix.py',
     'data_analysis': 'sources/topics/datamatrix.py',
     'questions_howto': 'sources/topics/questions-how-to.md',
 }
-# The number of documents that is added to the documentation for each search
-# query
-search_docs_per_query = 2
+# The number of documents that is considered for each search query
+search_docs_per_query = 20
+# The number of documents that is kept for all search queries combined
+search_docs_max = 4
 # The distance metric used for search. The cosine metric is useful because it
 # is somewhat invariant to changes in document length
 search_metric = 'cosine'
 # The cache folder for the library that is used to chat
 db_cache = '.db.cache'
 # The cache folder for the library that is used for public search
 public_search_cache = '.ps.cache'
```

### Comparing `sigmund-0.16.1/sigmund/database/encryption.py` & `sigmund-0.16.2/sigmund/database/encryption.py`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.1/sigmund/database/manager.py` & `sigmund-0.16.2/sigmund/database/manager.py`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.1/sigmund/database/models.py` & `sigmund-0.16.2/sigmund/database/models.py`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.1/sigmund/documentation.py` & `sigmund-0.16.2/sigmund/documentation.py`

 * *Files 12% similar despite different names*

```diff
@@ -102,29 +102,42 @@
                 'No OpenAI API key provided, no documentation available')
             return
         self._embeddings_model = OpenAIEmbeddings(
             openai_api_key=config.openai_api_key)
         logger.info('reading FAISS documentation cache')
         self._db = FAISS.load_local(Path('.db.cache'), self._embeddings_model,
                                     allow_dangerous_deserialization=True)
-        self._retriever = self._db.as_retriever(
-            search_kwargs={'k': config.search_docs_per_query,
-                           'metric': config.search_metric})
     
     def search(self, queries):
         if config.openai_api_key is None:
             return []
         docs = []
         for query in queries:
-            logger.info(f'searching FAISS')
-            for doc in self._retriever.invoke(query):
+            for doc, score in self._db.similarity_search_with_score(
+                    query, k=config.search_docs_per_query):
                 doc_desc = f'{doc.metadata["url"]} ({doc.metadata["seq_num"]})'
-                if any(doc.page_content == ref.page_content for ref in docs):
-                    logger.info(f'duplicate {doc_desc}')
+                if any(doc.page_content == ref.page_content for ref, _ in docs):
                     continue
                 if doc.page_content not in self._sigmund.documentation and \
                         doc.page_content not in docs:
-                    logger.info(f'adding {doc_desc}')
-                    docs.append(doc)
-                else:
-                    logger.info(f'skipping {doc_desc}')
-        return docs
+                    docs.append((doc, score))
+        # The documents that are retrieved need a little re-ordering to be
+        # optimal. First we rank them by score across all search queries. Then
+        # we reorder them so that documents without URL, which tend to be short
+        # how-to's alternate with documents with URL, which tend to be longer
+        # pieces of documentation. This is to make sure that documentation
+        # stands a chance against the how-to's, which tend to be preferred by
+        # the algorithm. Finally we keep only the top few documents.
+        docs = sorted(docs, key=lambda doc: -doc[1])
+        with_url = [d for d in docs if d[0].metadata['url'] is not None]
+        without_url = [d for d in docs if d[0].metadata['url'] is None]
+        reordered_docs = []
+        while with_url or without_url:
+            if with_url:
+                reordered_docs.append(with_url.pop(0))
+            if without_url:
+                reordered_docs.append(without_url.pop(0))
+        reordered_docs = reordered_docs[:config.search_docs_max]
+        for doc, score in reordered_docs:
+            doc_desc = f'{doc.metadata["url"]} ({doc.metadata["seq_num"]})'
+            logger.info(f'considering {doc_desc}, score: {score}')
+        return [doc for doc, _ in reordered_docs]
```

### Comparing `sigmund-0.16.1/sigmund/library.py` & `sigmund-0.16.2/sigmund/library.py`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.1/sigmund/messages.py` & `sigmund-0.16.2/sigmund/messages.py`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.1/sigmund/model/__init__.py` & `sigmund-0.16.2/sigmund/model/__init__.py`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.1/sigmund/model/_anthropic_model.py` & `sigmund-0.16.2/sigmund/model/_anthropic_model.py`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.1/sigmund/model/_base_model.py` & `sigmund-0.16.2/sigmund/model/_base_model.py`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.1/sigmund/model/_mistral_model.py` & `sigmund-0.16.2/sigmund/model/_mistral_model.py`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.1/sigmund/model/_openai_model.py` & `sigmund-0.16.2/sigmund/model/_openai_model.py`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.1/sigmund/prompt.py` & `sigmund-0.16.2/sigmund/prompt.py`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.1/sigmund/routes/api.py` & `sigmund-0.16.2/sigmund/routes/api.py`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.1/sigmund/routes/app.py` & `sigmund-0.16.2/sigmund/routes/app.py`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.1/sigmund/routes/google_login.py` & `sigmund-0.16.2/sigmund/routes/google_login.py`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.1/sigmund/routes/subscribe.py` & `sigmund-0.16.2/sigmund/routes/subscribe.py`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.1/sigmund/server.py` & `sigmund-0.16.2/sigmund/server.py`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.1/sigmund/sigmund.py` & `sigmund-0.16.2/sigmund/sigmund.py`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.1/sigmund/static/about.md` & `sigmund-0.16.2/sigmund/static/about.md`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.1/sigmund/static/background.png` & `sigmund-0.16.2/sigmund/static/background.png`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.1/sigmund/static/login.md` & `sigmund-0.16.2/sigmund/static/login.md`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.1/sigmund/static/pygments.css` & `sigmund-0.16.2/sigmund/static/pygments.css`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.1/sigmund/static/sofa-with-sigmund.png` & `sigmund-0.16.2/sigmund/static/sofa-with-sigmund.png`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.1/sigmund/static/sofa.png` & `sigmund-0.16.2/sigmund/static/sofa.png`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.1/sigmund/static/terms.md` & `sigmund-0.16.2/sigmund/static/terms.md`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.1/sigmund/templates/chat.html` & `sigmund-0.16.2/sigmund/templates/chat.html`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.1/sigmund/templates/head.html` & `sigmund-0.16.2/sigmund/templates/head.html`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.1/sigmund/templates/login.html` & `sigmund-0.16.2/sigmund/templates/login.html`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.1/sigmund/templates/main.js` & `sigmund-0.16.2/sigmund/templates/main.js`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.1/sigmund/templates/menu.html` & `sigmund-0.16.2/sigmund/templates/menu.html`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.1/sigmund/templates/stylesheet.css.jinja` & `sigmund-0.16.2/sigmund/templates/stylesheet.css.jinja`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.1/sigmund/templates/subscribe-error.html` & `sigmund-0.16.2/sigmund/templates/subscribe-error.html`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.1/sigmund/templates/subscribe-success.html` & `sigmund-0.16.2/sigmund/templates/subscribe-success.html`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.1/sigmund/tools/_base_tool.py` & `sigmund-0.16.2/sigmund/tools/_base_tool.py`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.1/sigmund/tools/_download.py` & `sigmund-0.16.2/sigmund/tools/_download.py`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.1/sigmund/tools/_execute_code.py` & `sigmund-0.16.2/sigmund/tools/_execute_code.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from . import BaseTool
 import logging
 import requests
 logger = logging.getLogger('sigmund')
 
 
 class execute_code(BaseTool):
-    """Execute Python and R code. Only use for code that should be executed. Don't use for example code."""
+    """Execute Python and R code. Do not use this tool unless code should actually be executed. When executing Python, you can only use modules from the Python standard library."""
     
     arguments = {
         'language': {
             'type': 'string',
             'description': 'The programming language to use',
             'enum': ['r', 'python']
         },
@@ -54,8 +54,8 @@
 
 ```
 {result}
 ```
 '''
             return 'Executing code ...', result, True
         logger.error(f"Error: {response.status_code} with message: {response.content}")
-        return 'Failed to execute code', '', True
+        return 'Failed to execute code', '', True
```

### Comparing `sigmund-0.16.1/sigmund/tools/_read_attachment.py` & `sigmund-0.16.2/sigmund/tools/_read_attachment.py`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.1/sigmund/tools/_search_documentation.py` & `sigmund-0.16.2/sigmund/tools/_search_documentation.py`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.1/sigmund/tools/_search_google_scholar.py` & `sigmund-0.16.2/sigmund/tools/_search_google_scholar.py`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.1/sigmund/utils.py` & `sigmund-0.16.2/sigmund/utils.py`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.1/PKG-INFO` & `sigmund-0.16.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sigmund
-Version: 0.16.1
+Version: 0.16.2
 Summary: AI-based chatbot that provides sensible answers based on documentation
 Keywords: ai,chatbot,llm
 Author-email: Sebastiaan Mathôt <s.mathot@cogsci.nl>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: anthropic
 Requires-Dist: cryptography
```


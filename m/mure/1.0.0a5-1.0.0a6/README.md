# Comparing `tmp/mure-1.0.0a5.tar.gz` & `tmp/mure-1.0.0a6.tar.gz`

## Comparing `mure-1.0.0a5.tar` & `mure-1.0.0a6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 mure-1.0.0a5/.pre-commit-config.yaml
--rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 mure-1.0.0a5/requirements-dev.lock
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 mure-1.0.0a5/requirements.lock
--rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 mure-1.0.0a5/.github/workflows/main.yml
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 mure-1.0.0a5/.vscode/settings.json
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 mure-1.0.0a5/examples/example.py
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 mure-1.0.0a5/mure/__init__.py
--rw-r--r--   0        0        0     3705 2020-02-02 00:00:00.000000 mure-1.0.0a5/mure/cache.py
--rw-r--r--   0        0        0     5829 2020-02-02 00:00:00.000000 mure-1.0.0a5/mure/core.py
--rw-r--r--   0        0        0     3881 2020-02-02 00:00:00.000000 mure-1.0.0a5/mure/dtos.py
--rw-r--r--   0        0        0     9208 2020-02-02 00:00:00.000000 mure-1.0.0a5/mure/iterator.py
--rw-r--r--   0        0        0     4272 2020-02-02 00:00:00.000000 mure-1.0.0a5/mure/logging.py
--rw-r--r--   0        0        0     2313 2020-02-02 00:00:00.000000 mure-1.0.0a5/tests/test_mure.py
--rw-r--r--   0        0        0     1809 2020-02-02 00:00:00.000000 mure-1.0.0a5/.gitignore
--rw-r--r--   0        0        0    11345 2020-02-02 00:00:00.000000 mure-1.0.0a5/LICENSE
--rw-r--r--   0        0        0     6540 2020-02-02 00:00:00.000000 mure-1.0.0a5/README.md
--rw-r--r--   0        0        0     2876 2020-02-02 00:00:00.000000 mure-1.0.0a5/pyproject.toml
--rw-r--r--   0        0        0     6892 2020-02-02 00:00:00.000000 mure-1.0.0a5/PKG-INFO
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 mure-1.0.0a6/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 mure-1.0.0a6/requirements-dev.lock
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 mure-1.0.0a6/requirements.lock
+-rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 mure-1.0.0a6/.github/workflows/main.yml
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 mure-1.0.0a6/.vscode/settings.json
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 mure-1.0.0a6/examples/example.py
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 mure-1.0.0a6/mure/__init__.py
+-rw-r--r--   0        0        0     4198 2020-02-02 00:00:00.000000 mure-1.0.0a6/mure/cache.py
+-rw-r--r--   0        0        0     5829 2020-02-02 00:00:00.000000 mure-1.0.0a6/mure/core.py
+-rw-r--r--   0        0        0     3881 2020-02-02 00:00:00.000000 mure-1.0.0a6/mure/dtos.py
+-rw-r--r--   0        0        0     9315 2020-02-02 00:00:00.000000 mure-1.0.0a6/mure/iterator.py
+-rw-r--r--   0        0        0     4272 2020-02-02 00:00:00.000000 mure-1.0.0a6/mure/logging.py
+-rw-r--r--   0        0        0     2313 2020-02-02 00:00:00.000000 mure-1.0.0a6/tests/test_mure.py
+-rw-r--r--   0        0        0     1809 2020-02-02 00:00:00.000000 mure-1.0.0a6/.gitignore
+-rw-r--r--   0        0        0    11345 2020-02-02 00:00:00.000000 mure-1.0.0a6/LICENSE
+-rw-r--r--   0        0        0     6540 2020-02-02 00:00:00.000000 mure-1.0.0a6/README.md
+-rw-r--r--   0        0        0     2876 2020-02-02 00:00:00.000000 mure-1.0.0a6/pyproject.toml
+-rw-r--r--   0        0        0     6892 2020-02-02 00:00:00.000000 mure-1.0.0a6/PKG-INFO
```

### Comparing `mure-1.0.0a5/requirements-dev.lock` & `mure-1.0.0a6/requirements-dev.lock`

 * *Files identical despite different names*

### Comparing `mure-1.0.0a5/.vscode/settings.json` & `mure-1.0.0a6/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `mure-1.0.0a5/examples/example.py` & `mure-1.0.0a6/examples/example.py`

 * *Files identical despite different names*

### Comparing `mure-1.0.0a5/mure/core.py` & `mure-1.0.0a6/mure/core.py`

 * *Files identical despite different names*

### Comparing `mure-1.0.0a5/mure/dtos.py` & `mure-1.0.0a6/mure/dtos.py`

 * *Files identical despite different names*

### Comparing `mure-1.0.0a5/mure/iterator.py` & `mure-1.0.0a6/mure/iterator.py`

 * *Files 3% similar despite different names*

```diff
@@ -173,21 +173,23 @@
         event : Event
             Event to set when the response is ready.
         """
         LOGGER.debug(f"Started {priority}")
 
         # if cache is given and has the resource, use it
         if self.cache and self.cache.has(resource):
+            LOGGER.debug("Found response in cache")
             response = self.cache.get(resource)
         else:
             response = await self._afetch(session, resource)
 
             # save response to cache
             if self.cache:
-                self.cache.save(resource, response)
+                self.cache.set(resource, response)
+                LOGGER.debug("Saved response to cache")
 
         # put response in the queue
         await self._queue.put((priority, response))
 
         # set event to notify that the response is ready
         event.set()
```

### Comparing `mure-1.0.0a5/mure/logging.py` & `mure-1.0.0a6/mure/logging.py`

 * *Files identical despite different names*

### Comparing `mure-1.0.0a5/tests/test_mure.py` & `mure-1.0.0a6/tests/test_mure.py`

 * *Files identical despite different names*

### Comparing `mure-1.0.0a5/.gitignore` & `mure-1.0.0a6/.gitignore`

 * *Files identical despite different names*

### Comparing `mure-1.0.0a5/LICENSE` & `mure-1.0.0a6/LICENSE`

 * *Files identical despite different names*

### Comparing `mure-1.0.0a5/README.md` & `mure-1.0.0a6/README.md`

 * *Files identical despite different names*

### Comparing `mure-1.0.0a5/pyproject.toml` & `mure-1.0.0a6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "mure"
-version = "1.0.0a5"
+version = "1.0.0a6"
 description = "Perform multiple HTTP requests concurrently – without worrying about async functions."
 authors = [{ name = "Severin Simmler", email = "s.simmler@snapaddy.com" }]
 dependencies = ["aiohttp>=3.9.3", "chardet>=5.2.0"]
 readme = "README.md"
 requires-python = ">= 3.11, < 4"
 
 [build-system]
```

### Comparing `mure-1.0.0a5/PKG-INFO` & `mure-1.0.0a6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: mure
-Version: 1.0.0a5
+Version: 1.0.0a6
 Summary: Perform multiple HTTP requests concurrently – without worrying about async functions.
 Author-email: Severin Simmler <s.simmler@snapaddy.com>
 License-File: LICENSE
 Requires-Python: <4,>=3.11
 Requires-Dist: aiohttp>=3.9.3
 Requires-Dist: chardet>=5.2.0
 Description-Content-Type: text/markdown
```


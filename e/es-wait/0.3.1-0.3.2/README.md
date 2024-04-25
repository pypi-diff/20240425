# Comparing `tmp/es_wait-0.3.1.tar.gz` & `tmp/es_wait-0.3.2.tar.gz`

## Comparing `es_wait-0.3.1.tar` & `es_wait-0.3.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 es_wait-0.3.1/pytest.ini
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 es_wait-0.3.1/src/es_wait/__init__.py
--rw-r--r--   0        0        0     2036 2020-02-02 00:00:00.000000 es_wait-0.3.1/src/es_wait/args.py
--rw-r--r--   0        0        0     3309 2020-02-02 00:00:00.000000 es_wait-0.3.1/src/es_wait/base.py
--rw-r--r--   0        0        0     2080 2020-02-02 00:00:00.000000 es_wait-0.3.1/src/es_wait/exists.py
--rw-r--r--   0        0        0     3022 2020-02-02 00:00:00.000000 es_wait-0.3.1/src/es_wait/health.py
--rw-r--r--   0        0        0     2134 2020-02-02 00:00:00.000000 es_wait-0.3.1/src/es_wait/relocate.py
--rw-r--r--   0        0        0     3155 2020-02-02 00:00:00.000000 es_wait-0.3.1/src/es_wait/restore.py
--rw-r--r--   0        0        0     2807 2020-02-02 00:00:00.000000 es_wait-0.3.1/src/es_wait/snapshot.py
--rw-r--r--   0        0        0     3232 2020-02-02 00:00:00.000000 es_wait-0.3.1/src/es_wait/task.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 es_wait-0.3.1/.gitignore
--rw-r--r--   0        0        0    11347 2020-02-02 00:00:00.000000 es_wait-0.3.1/LICENSE
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 es_wait-0.3.1/README.md
--rw-r--r--   0        0        0     3922 2020-02-02 00:00:00.000000 es_wait-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 es_wait-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 es_wait-0.3.2/pytest.ini
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 es_wait-0.3.2/src/es_wait/__init__.py
+-rw-r--r--   0        0        0     2036 2020-02-02 00:00:00.000000 es_wait-0.3.2/src/es_wait/args.py
+-rw-r--r--   0        0        0     3309 2020-02-02 00:00:00.000000 es_wait-0.3.2/src/es_wait/base.py
+-rw-r--r--   0        0        0     2080 2020-02-02 00:00:00.000000 es_wait-0.3.2/src/es_wait/exists.py
+-rw-r--r--   0        0        0     3022 2020-02-02 00:00:00.000000 es_wait-0.3.2/src/es_wait/health.py
+-rw-r--r--   0        0        0     2134 2020-02-02 00:00:00.000000 es_wait-0.3.2/src/es_wait/relocate.py
+-rw-r--r--   0        0        0     3155 2020-02-02 00:00:00.000000 es_wait-0.3.2/src/es_wait/restore.py
+-rw-r--r--   0        0        0     2699 2020-02-02 00:00:00.000000 es_wait-0.3.2/src/es_wait/snapshot.py
+-rw-r--r--   0        0        0     3232 2020-02-02 00:00:00.000000 es_wait-0.3.2/src/es_wait/task.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 es_wait-0.3.2/.gitignore
+-rw-r--r--   0        0        0    11347 2020-02-02 00:00:00.000000 es_wait-0.3.2/LICENSE
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 es_wait-0.3.2/README.md
+-rw-r--r--   0        0        0     3922 2020-02-02 00:00:00.000000 es_wait-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 es_wait-0.3.2/PKG-INFO
```

### Comparing `es_wait-0.3.1/src/es_wait/args.py` & `es_wait-0.3.2/src/es_wait/args.py`

 * *Files identical despite different names*

### Comparing `es_wait-0.3.1/src/es_wait/base.py` & `es_wait-0.3.2/src/es_wait/base.py`

 * *Files identical despite different names*

### Comparing `es_wait-0.3.1/src/es_wait/exists.py` & `es_wait-0.3.2/src/es_wait/exists.py`

 * *Files identical despite different names*

### Comparing `es_wait-0.3.1/src/es_wait/health.py` & `es_wait-0.3.2/src/es_wait/health.py`

 * *Files identical despite different names*

### Comparing `es_wait-0.3.1/src/es_wait/relocate.py` & `es_wait-0.3.2/src/es_wait/relocate.py`

 * *Files identical despite different names*

### Comparing `es_wait-0.3.1/src/es_wait/restore.py` & `es_wait-0.3.2/src/es_wait/restore.py`

 * *Files identical despite different names*

### Comparing `es_wait-0.3.1/src/es_wait/snapshot.py` & `es_wait-0.3.2/src/es_wait/snapshot.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,29 +32,27 @@
         and tests to see whether the snapshot is complete, and if so, with what status.  It will log
         errors according to the result. If the snapshot is still ``IN_PROGRESS``, it will return
         ``False``. ``SUCCESS`` will be an ``INFO`` level message, ``PARTIAL`` nets a ``WARNING``
         message, ``FAILED`` is an ``ERROR``, message, and all others will be a ``WARNING`` level
         message.
         """
         state = self.snapstate['snapshots'][0]['state']
-        self.logger.debug('Snapshot state = %s', state)
         retval = True
         if state == 'IN_PROGRESS':
             self.logger.debug('Snapshot %s still in progress.', self.snapshot)
             retval = False
         if retval:
             self.log_completion(state)
         return retval
 
     @property
     def snapstate(self) -> t.Dict:
         result = {}
         try:
             result = self.client.snapshot.get(repository=self.repository, snapshot=self.snapshot)
-            self.logger.debug('RESULT: %s', result)
         except Exception as err:
             raise ValueError(
                 f'Unable to obtain information for snapshot "{self.snapshot}" in repository '
                 f'"{self.repository}". Error: {err}'
             ) from err
         return result
```

### Comparing `es_wait-0.3.1/src/es_wait/task.py` & `es_wait-0.3.2/src/es_wait/task.py`

 * *Files identical despite different names*

### Comparing `es_wait-0.3.1/.gitignore` & `es_wait-0.3.2/.gitignore`

 * *Files identical despite different names*

### Comparing `es_wait-0.3.1/LICENSE` & `es_wait-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `es_wait-0.3.1/pyproject.toml` & `es_wait-0.3.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `es_wait-0.3.1/PKG-INFO` & `es_wait-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: es-wait
-Version: 0.3.1
+Version: 0.3.2
 Summary: Helping you wait for certain Elasticsearch tasks and API calls to finish
 Project-URL: Documentation, https://github.com/untergeek/es-wait#readme
 Project-URL: Issues, https://github.com/untergeek/es-wait/issues
 Project-URL: Source, https://github.com/untergeek/es-wait
 Author-email: Aaron Mildenstein <untergeek@elastic.co>
 License: Apache-2.0
 License-File: LICENSE
```


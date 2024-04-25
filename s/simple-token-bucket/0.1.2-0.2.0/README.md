# Comparing `tmp/simple_token_bucket-0.1.2.tar.gz` & `tmp/simple_token_bucket-0.2.0.tar.gz`

## Comparing `simple_token_bucket-0.1.2.tar` & `simple_token_bucket-0.2.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 simple_token_bucket-0.1.2/.readthedocs.yaml
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 simple_token_bucket-0.1.2/.github/workflows/publish.yml
--rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 simple_token_bucket-0.1.2/.github/workflows/test.yml
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 simple_token_bucket-0.1.2/docs/api.rst
--rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 simple_token_bucket-0.1.2/docs/conf.py
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 simple_token_bucket-0.1.2/docs/contributing.rst
--rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 simple_token_bucket-0.1.2/docs/index.rst
--rw-r--r--   0        0        0     1411 2020-02-02 00:00:00.000000 simple_token_bucket-0.1.2/simple_token_bucket/__init__.py
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 simple_token_bucket-0.1.2/simple_token_bucket/backends/__init__.py
--rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 simple_token_bucket-0.1.2/simple_token_bucket/backends/redis.py
--rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 simple_token_bucket-0.1.2/tests/test_redis_backend.py
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 simple_token_bucket-0.1.2/.gitignore
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 simple_token_bucket-0.1.2/LICENSE
--rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 simple_token_bucket-0.1.2/README.md
--rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 simple_token_bucket-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2196 2020-02-02 00:00:00.000000 simple_token_bucket-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 simple_token_bucket-0.2.0/.readthedocs.yaml
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 simple_token_bucket-0.2.0/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 simple_token_bucket-0.2.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 simple_token_bucket-0.2.0/docs/api.rst
+-rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 simple_token_bucket-0.2.0/docs/conf.py
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 simple_token_bucket-0.2.0/docs/contributing.rst
+-rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 simple_token_bucket-0.2.0/docs/index.rst
+-rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 simple_token_bucket-0.2.0/simple_token_bucket/__init__.py
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 simple_token_bucket-0.2.0/simple_token_bucket/backends/__init__.py
+-rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 simple_token_bucket-0.2.0/simple_token_bucket/backends/redis.py
+-rw-r--r--   0        0        0     1421 2020-02-02 00:00:00.000000 simple_token_bucket-0.2.0/tests/test_redis_backend.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 simple_token_bucket-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 simple_token_bucket-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 simple_token_bucket-0.2.0/README.md
+-rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 simple_token_bucket-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2196 2020-02-02 00:00:00.000000 simple_token_bucket-0.2.0/PKG-INFO
```

### Comparing `simple_token_bucket-0.1.2/.github/workflows/test.yml` & `simple_token_bucket-0.2.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `simple_token_bucket-0.1.2/docs/conf.py` & `simple_token_bucket-0.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `simple_token_bucket-0.1.2/docs/contributing.rst` & `simple_token_bucket-0.2.0/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `simple_token_bucket-0.1.2/docs/index.rst` & `simple_token_bucket-0.2.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `simple_token_bucket-0.1.2/simple_token_bucket/__init__.py` & `simple_token_bucket-0.2.0/simple_token_bucket/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,24 @@
-__version__ = "0.1.2"
+__version__ = "0.2.0"
 
 
+from typing import Callable, Optional
+
 from .backends import Backend
 
 
 class SimpleTokenBucket:
-    def __init__(self, name: str, bucket_size: int, refresh_interval: int, backend: Backend):
+    def __init__(
+        self,
+        name: str,
+        bucket_size: int,
+        refresh_interval: int,
+        backend: Backend,
+        listener: Optional[Callable[[int], None]] = None,
+    ):
         """Create a new SimpleTokenBucket.
 
         Every `refresh_interval` the token bucket is refresh and `bucket_size`
         tokens are available again.
 
         Args:
             name: Bucket name.
@@ -17,22 +26,26 @@
             refresh_interval: Bucket reset time interval (in seconds).
             backend: a :class:`.backends.Backend` implementation.
         """
         self.name = name
         self.bucket_size = bucket_size
         self.refresh_interval = refresh_interval
         self._backend = backend
+        self._listener_callback = listener
 
     def try_get_token(self, raises=True) -> bool:
         available_tokens, ttl = self._backend.get_token(
             bucket_name=self.name,
             bucket_size=self.bucket_size,
             refresh_interval=self.refresh_interval,
         )
 
+        if self._listener_callback is not None:
+            self._listener_callback(available_tokens)
+
         if available_tokens <= 0:
             if raises:
                 raise NotEnoughTokens(remaining_seconds=ttl)
             else:
                 return False
 
         return True
```

### Comparing `simple_token_bucket-0.1.2/simple_token_bucket/backends/__init__.py` & `simple_token_bucket-0.2.0/simple_token_bucket/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `simple_token_bucket-0.1.2/simple_token_bucket/backends/redis.py` & `simple_token_bucket-0.2.0/simple_token_bucket/backends/redis.py`

 * *Files identical despite different names*

### Comparing `simple_token_bucket-0.1.2/tests/test_redis_backend.py` & `simple_token_bucket-0.2.0/tests/test_redis_backend.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,32 @@
-import pytest
+from unittest import mock
+
 import fakeredis
+import pytest
 
-from simple_token_bucket import SimpleTokenBucket, NotEnoughTokens
+from simple_token_bucket import NotEnoughTokens, SimpleTokenBucket
 from simple_token_bucket.backends.redis import RedisBackend
 
 
 @pytest.fixture
 def redis_client():
     return fakeredis.FakeStrictRedis(version=6)
 
 
 def test_redis_backend_ok(redis_client):
+    listener = mock.MagicMock()
     token_bucket = SimpleTokenBucket(
         name="test_ok",
         bucket_size=3,
         refresh_interval=60,
         backend=RedisBackend(redis_client),
+        listener=listener,
     )
     assert token_bucket.try_get_token() is True
+    listener.assert_called_once_with(3)
 
 
 def test_redis_backend_not_enough_tokens_raises(redis_client):
     token_bucket = SimpleTokenBucket(
         name="test_not_enough_tokens",
         bucket_size=1,
         refresh_interval=60,
```

### Comparing `simple_token_bucket-0.1.2/LICENSE` & `simple_token_bucket-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `simple_token_bucket-0.1.2/README.md` & `simple_token_bucket-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `simple_token_bucket-0.1.2/pyproject.toml` & `simple_token_bucket-0.2.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 [tool.hatch.version]
 path = "simple_token_bucket/__init__.py"
 
 [tool.hatch.envs.test]
 dependencies = [
   "pytest",
   "pytest-cov",
-  "fakeredis",
+  "fakeredis<=2.21.3",
 ]
 
 [[tool.hatch.envs.test.matrix]]
 python = ["3.11", "3.10", "3.9", "3.8"]
 
 [tool.hatch.envs.test.scripts]
 cov = "pytest --cov=simple_token_bucket {args:tests}"
```

### Comparing `simple_token_bucket-0.1.2/PKG-INFO` & `simple_token_bucket-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: simple-token-bucket
-Version: 0.1.2
+Version: 0.2.0
 Project-URL: Source, https://github.com/buserbrasil/simple-token-bucket
 Project-URL: Issues, https://github.com/buserbrasil/simple-token-bucket/issues
 Author-email: Erle Carrara <carrara.erle@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```


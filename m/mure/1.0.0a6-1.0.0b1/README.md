# Comparing `tmp/mure-1.0.0a6.tar.gz` & `tmp/mure-1.0.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "mure-1.0.0b1.tar", max compression
```

## Comparing `mure-1.0.0a6.tar` & `mure-1.0.0b1.tar`

### file list

```diff
@@ -1,18 +1,10 @@
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 mure-1.0.0a6/.pre-commit-config.yaml
--rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 mure-1.0.0a6/requirements-dev.lock
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 mure-1.0.0a6/requirements.lock
--rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 mure-1.0.0a6/.github/workflows/main.yml
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 mure-1.0.0a6/.vscode/settings.json
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 mure-1.0.0a6/examples/example.py
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 mure-1.0.0a6/mure/__init__.py
--rw-r--r--   0        0        0     4198 2020-02-02 00:00:00.000000 mure-1.0.0a6/mure/cache.py
--rw-r--r--   0        0        0     5829 2020-02-02 00:00:00.000000 mure-1.0.0a6/mure/core.py
--rw-r--r--   0        0        0     3881 2020-02-02 00:00:00.000000 mure-1.0.0a6/mure/dtos.py
--rw-r--r--   0        0        0     9315 2020-02-02 00:00:00.000000 mure-1.0.0a6/mure/iterator.py
--rw-r--r--   0        0        0     4272 2020-02-02 00:00:00.000000 mure-1.0.0a6/mure/logging.py
--rw-r--r--   0        0        0     2313 2020-02-02 00:00:00.000000 mure-1.0.0a6/tests/test_mure.py
--rw-r--r--   0        0        0     1809 2020-02-02 00:00:00.000000 mure-1.0.0a6/.gitignore
--rw-r--r--   0        0        0    11345 2020-02-02 00:00:00.000000 mure-1.0.0a6/LICENSE
--rw-r--r--   0        0        0     6540 2020-02-02 00:00:00.000000 mure-1.0.0a6/README.md
--rw-r--r--   0        0        0     2876 2020-02-02 00:00:00.000000 mure-1.0.0a6/pyproject.toml
--rw-r--r--   0        0        0     6892 2020-02-02 00:00:00.000000 mure-1.0.0a6/PKG-INFO
+-rw-r--r--   0        0        0    11345 2024-04-25 12:32:55.563618 mure-1.0.0b1/LICENSE
+-rw-r--r--   0        0        0     5557 2024-04-25 12:32:55.563618 mure-1.0.0b1/README.md
+-rw-r--r--   0        0        0      212 2024-04-25 12:32:55.563618 mure-1.0.0b1/mure/__init__.py
+-rw-r--r--   0        0        0     3097 2024-04-25 12:32:55.563618 mure-1.0.0b1/mure/cache.py
+-rw-r--r--   0        0        0     4419 2024-04-25 12:32:55.563618 mure-1.0.0b1/mure/core.py
+-rw-r--r--   0        0        0     9076 2024-04-25 12:32:55.563618 mure-1.0.0b1/mure/iterator.py
+-rw-r--r--   0        0        0     4272 2024-04-25 12:32:55.563618 mure-1.0.0b1/mure/logging.py
+-rw-r--r--   0        0        0     3874 2024-04-25 12:32:55.563618 mure-1.0.0b1/mure/models.py
+-rw-r--r--   0        0        0     2794 2024-04-25 12:32:55.563618 mure-1.0.0b1/pyproject.toml
+-rw-r--r--   0        0        0     6072 1970-01-01 00:00:00.000000 mure-1.0.0b1/PKG-INFO
```

### Comparing `mure-1.0.0a6/mure/cache.py` & `mure-1.0.0b1/mure/core.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,157 +1,177 @@
-import json
-import shelve
-from abc import ABC, abstractmethod
-from hashlib import blake2b
-from pathlib import Path
-
-from mure.dtos import HTTPResource, Response
-
-
-class Cache(ABC):
-    """Abstract class for a cache."""
-
-    @abstractmethod
-    def has(self, resource: HTTPResource) -> bool:
-        """Check if a resource is in the cache.
-
-        Parameters
-        ----------
-        resource : HTTPResource
-            Resource to check if it's in the cache.
-
-        Returns
-        -------
-        bool
-            True if the resource is in the cache; otherwise, False.
-        """
-
-    @abstractmethod
-    def get(self, resource: HTTPResource) -> Response | None:
-        """Get the response for the specified resource from the cache.
-
-        Parameters
-        ----------
-        resource : HTTPResource
-            Resource to get response from the cache.
-
-        Returns
-        -------
-        Response | None
-            Response from the cache or None if the resource is not in the cache.
-        """
-
-    @abstractmethod
-    def set(self, resource: HTTPResource, response: Response):
-        """Save a resource and its response to the cache.
-
-        Parameters
-        ----------
-        resource : HTTPResource
-            Resource to save to the cache.
-        response : Response
-            Response to save to the cache.
-        """
-
-    def identify_resource(self, resource: HTTPResource) -> str:
-        """Identify a resource.
-
-        Parameters
-        ----------
-        resource : HTTPResource
-            Resource to get an identifier for.
-
-        Returns
-        -------
-        str
-            JSON representation of the resource.
-        """
-        # generate a hash based on the components
-        key = blake2b(digest_size=8)
-        for part in [
-            resource["method"],
-            resource["url"],
-            json.dumps(resource.get("params"), sort_keys=True, ensure_ascii=False),
-            json.dumps(resource.get("data"), sort_keys=True, ensure_ascii=False),
-            json.dumps(resource.get("json"), sort_keys=True, ensure_ascii=False),
-        ]:
-            key.update(self._encode(part))
-
-        return key.hexdigest()
-
-    @staticmethod
-    def _encode(value: str) -> bytes:
-        """Encode a string to bytes.
-
-        Parameters
-        ----------
-        value : str
-            String to encode.
-
-        Returns
-        -------
-        bytes
-            Encoded string.
-        """
-        if not value:
-            return b""
-
-        return value if isinstance(value, bytes) else str(value).encode("utf-8")
-
-
-class InMemoryCache(Cache):
-    """Simple in-memory cache."""
-
-    def __init__(self):
-        self._cache = {}
-
-    def has(self, resource: HTTPResource) -> bool:
-        """Check if a resource is in the cache.
-
-        Parameters
-        ----------
-        resource : HTTPResource
-            Resource to check if it's in the cache.
-
-        Returns
-        -------
-        bool
-            True if the resource is in the cache; otherwise, False.
-        """
-        return self.identify_resource(resource) in self._cache
-
-    def get(self, resource: HTTPResource) -> Response | None:
-        """Get the response for the specified resource from the cache.
-
-        Parameters
-        ----------
-        resource : HTTPResource
-            Resource to get response from the cache.
-
-        Returns
-        -------
-        Response | None
-            Response from the cache or None if the resource is not in the cache.
-        """
-        return self._cache.get(self.identify_resource(resource))
-
-    def set(self, resource: HTTPResource, response: Response):
-        """Save a resource and its response to the cache.
-
-        Parameters
-        ----------
-        resource : HTTPResource
-            Resource to save to the cache.
-        response : Response
-            Response to save to the cache.
-        """
-        self._cache[self.identify_resource(resource)] = response
-
-
-class ShelveCache(InMemoryCache):
-    """Shelve cache."""
-
-    def __init__(self, path: Path = Path("mure-cache.shelve")):
-        super().__init__()
-
-        self.path = path
-        self._cache = shelve.open(str(self.path.resolve()))
+from mure.cache import Cache
+from mure.iterator import ResponseIterator
+from mure.models import Request, Resource
+
+
+def delete(
+    resources: list[Resource],
+    *,
+    batch_size: int = 5,
+    cache: Cache | None = None,
+) -> ResponseIterator:
+    """Perform a DELETE request for each resource.
+
+    Parameters
+    ----------
+    resources : list[Resource]
+        Resources to request.
+    batch_size : int
+        Number of items to request per batch concurrently, by default 5.
+    cache : Cache | None, optional
+        Cache to use for storing responses, by default None.
+
+    Returns
+    -------
+    ResponseIterator
+        The server's responses for each resource.
+    """
+    return ResponseIterator(
+        [Request("DELETE", **resource) for resource in resources],
+        batch_size=batch_size,
+        cache=cache,
+    )
+
+
+def get(
+    resources: list[Resource],
+    *,
+    batch_size: int = 5,
+    cache: Cache | None = None,
+) -> ResponseIterator:
+    """Perform a GET request for each resource.
+
+    Parameters
+    ----------
+    resources : list[Resource]
+        Resources to request.
+    batch_size : int
+        Number of items to request per batch concurrently, by default 5.
+    cache : Cache | None, optional
+        Cache to use for storing responses, by default None.
+
+    Returns
+    -------
+    ResponseIterator
+        The server's responses for each resource.
+    """
+    return ResponseIterator(
+        [Request("GET", **resource) for resource in resources],
+        batch_size=batch_size,
+        cache=cache,
+    )
+
+
+def head(
+    resources: list[Resource],
+    *,
+    batch_size: int = 5,
+    cache: Cache | None = None,
+) -> ResponseIterator:
+    """Perform a HEAD request for each resource.
+
+    Parameters
+    ----------
+    resources : list[Resource]
+        Resources to request.
+    batch_size : int
+        Number of items to request per batch concurrently, by default 5.
+    cache : Cache | None, optional
+        Cache to use for storing responses, by default None.
+
+    Returns
+    -------
+    ResponseIterator
+        The server's responses for each resource.
+    """
+    return ResponseIterator(
+        [Request("HEAD", **resource) for resource in resources],
+        batch_size=batch_size,
+        cache=cache,
+    )
+
+
+def patch(
+    resources: list[Resource],
+    *,
+    batch_size: int = 5,
+    cache: Cache | None = None,
+) -> ResponseIterator:
+    """Perform a PATCH request for each resource.
+
+    Parameters
+    ----------
+    resources : list[Resource]
+        Resources to request.
+    batch_size : int
+        Number of items to request per batch concurrently, by default 5.
+    cache : Cache | None, optional
+        Cache to use for storing responses, by default None.
+
+    Returns
+    -------
+    ResponseIterator
+        The server's responses for each resource.
+    """
+    return ResponseIterator(
+        [Request("PATCH", **resource) for resource in resources],
+        batch_size=batch_size,
+        cache=cache,
+    )
+
+
+def post(
+    resources: list[Resource],
+    *,
+    batch_size: int = 5,
+    cache: Cache | None = None,
+) -> ResponseIterator:
+    """Perform a POST request for each resource.
+
+    Parameters
+    ----------
+    resources : list[Resource]
+        Resources to request.
+    batch_size : int
+        Number of items to request per batch concurrently, by default 5.
+    cache : Cache | None, optional
+        Cache to use for storing responses, by default None.
+
+    Returns
+    -------
+    ResponseIterator
+        The server's responses for each resource.
+    """
+    return ResponseIterator(
+        [Request("POST", **resource) for resource in resources],
+        batch_size=batch_size,
+        cache=cache,
+    )
+
+
+def put(
+    resources: list[Resource],
+    *,
+    batch_size: int = 5,
+    cache: Cache | None = None,
+) -> ResponseIterator:
+    """Perform a PUT request for each resource.
+
+    Parameters
+    ----------
+    resources : list[Resource]
+        Resources to request.
+    batch_size : int
+        Number of items to request per batch concurrently, by default 5.
+    cache : Cache | None, optional
+        Cache to use for storing responses, by default None.
+
+    Returns
+    -------
+    ResponseIterator
+        The server's responses for each resource.
+    """
+    return ResponseIterator(
+        [Request("PUT", **resource) for resource in resources],
+        batch_size=batch_size,
+        cache=cache,
+    )
```

### Comparing `mure-1.0.0a6/mure/iterator.py` & `mure-1.0.0b1/mure/iterator.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,64 +4,64 @@
 from collections.abc import AsyncGenerator, Iterator
 from typing import Self
 
 import chardet
 from aiohttp import ClientSession
 
 from mure.cache import Cache
-from mure.dtos import HistoricResponse, HTTPResource, Response
 from mure.logging import Logger
+from mure.models import Request, Response
 
 LOGGER = Logger(__name__)
 
 
 class ResponseIterator(Iterator[Response]):
     """Response iterator that fetches responses concurrently."""
 
     def __init__(
         self,
-        resources: list[HTTPResource],
+        requests: list[Request],
         *,
         batch_size: int = 5,
         cache: Cache | None = None,
     ):
         """Initialize a response iterator.
 
         Parameters
         ----------
-        resources : list[HTTPResource]
+        requests : list[Request]
             Resources to request.
         batch_size : int, optional
             Number of resources to request concurrently, by default 5.
         cache : Cache | None, optional
             Cache to use for storing responses, by default None.
         """
-        self.resources = resources
-        self.num_resources = len(resources)
-        self.pending = len(resources)
+        self.requests = requests
+        self.num_requests = len(requests)
+        self.pending = len(requests)
         self.batch_size = batch_size
         self.cache = cache
 
         self._log_errors = bool(os.environ.get("MURE_LOG_ERRORS"))
         self._loop = asyncio.new_event_loop()
         self._queue = PriorityQueue()
-        self._events = [Event() for _ in resources]
+        self._events = [Event() for _ in requests]
         self._tasks: set[Task] = set()
         self._responses = self._fetch_responses()
         self._generator = None
 
     def __repr__(self) -> str:
         """Response iterator representation.
 
         Returns
         -------
         str
-            Representation with number of pending resources.
+            Representation with number of pending requests.
         """
-        return f"<ResponseIterator: {self.pending}/{self.num_resources} pending>"
+        return f"<ResponseIterator: {self.pending}/{self.num_requests} pending>"
 
     def __len__(self) -> int | float:
         """Return the number of pending responses.
 
         Returns
         -------
         int
@@ -145,50 +145,50 @@
             Client session to use.
 
         Yields
         ------
         Iterator[Task]
             Tasks to fetch resources.
         """
-        for i, (resource, event) in enumerate(zip(self.resources, self._events, strict=False)):
+        for i, (request, event) in enumerate(zip(self.requests, self._events, strict=False)):
             # create task in the background
-            yield self._loop.create_task(self._aprocess_resource(i, session, resource, event))
+            yield self._loop.create_task(self._aprocess_request(i, session, request, event))
 
-    async def _aprocess_resource(
+    async def _aprocess_request(
         self,
         priority: int,
         session: ClientSession,
-        resource: HTTPResource,
+        request: Request,
         event: Event,
     ):
-        """Process a resource by fetching and putting it in the queue.
+        """Process a request by fetching and putting it in the queue.
 
         Parameters
         ----------
         priority : int
-            Priority of the resource.
+            Priority of the request.
         session : ClientSession
             Client session to use.
-        resource : HTTPResource
+        request. : Request
             Resource to request.
         event : Event
             Event to set when the response is ready.
         """
         LOGGER.debug(f"Started {priority}")
 
-        # if cache is given and has the resource, use it
-        if self.cache and self.cache.has(resource):
+        # if cache is given and has the request., use it
+        if self.cache and self.cache.has(request):
             LOGGER.debug("Found response in cache")
-            response = self.cache.get(resource)
+            response = self.cache.get(request)
         else:
-            response = await self._afetch(session, resource)
+            response = await self._afetch(session, request)
 
             # save response to cache
             if self.cache:
-                self.cache.set(resource, response)
+                self.cache.set(request, response)
                 LOGGER.debug("Saved response to cache")
 
         # put response in the queue
         await self._queue.put((priority, response))
 
         # set event to notify that the response is ready
         event.set()
@@ -218,25 +218,26 @@
         """Fetch responses concurrently.
 
         Yields
         ------
         Response
             The server's response.
         """
-        session = ClientSession()
-
         try:
+            # one session for all requests
+            session = ClientSession(loop=self._loop)
+
             # create tasks (lazy)
             tasks = self._create_tasks(session)
 
             # process first batch of tasks
             self._process_batch(tasks)
 
             for event in self._events:
-                # wait for the specific event to be set to preserve order of the resources
+                # wait for the specific event to be set to preserve order of the requests
                 await event.wait()
 
                 # process next batch of tasks
                 self._process_batch(tasks)
 
                 # get response from the queue
                 _, response = await self._queue.get()
@@ -248,33 +249,39 @@
                 self._queue.task_done()
                 self.pending -= 1
         except GeneratorExit:
             return
         finally:
             await session.close()
 
-    async def _afetch(self, session: ClientSession, resource: HTTPResource) -> Response:
+    async def _afetch(self, session: ClientSession, request: Request) -> Response:
         """Perform a HTTP request.
 
         Parameters
         ----------
         session : ClientSession
             Client session to use.
-        resource : Resource
+        request : Resource
             Resource to request.
 
         Returns
         -------
         Response
             The server's response.
         """
         try:
-            kwargs = {k: v for k, v in resource.items() if k not in {"method", "url"}}
-
-            async with session.request(resource["method"], resource["url"], **kwargs) as response:
+            async with session.request(
+                request.method,
+                request.url,
+                headers=request.headers,
+                params=request.params,
+                data=request.data,
+                json=request.json,
+                timeout=request.timeout,
+            ) as response:
                 content = await response.read()
                 encoding = response.get_encoding()
 
                 try:
                     text = content.decode(encoding, errors="replace")
                 except (LookupError, TypeError):
                     # LookupError is raised if the encoding was not found which could
@@ -286,22 +293,13 @@
 
                 return Response(
                     status=response.status,
                     reason=response.reason,
                     ok=response.ok,
                     text=text,
                     url=response.url.human_repr(),
-                    history=[
-                        HistoricResponse(
-                            status=h.status,
-                            reason=h.reason,
-                            ok=h.ok,
-                            url=h.url.human_repr(),
-                        )
-                        for h in response.history
-                    ],
                 )
         except Exception as error:
             if self._log_errors:
                 LOGGER.error(error)
 
-            return Response(status=0, reason=repr(error), ok=False, text="", url="", history=[])
+            return Response(status=0, reason=repr(error), ok=False, text="", url="")
```

### Comparing `mure-1.0.0a6/mure/logging.py` & `mure-1.0.0b1/mure/logging.py`

 * *Files identical despite different names*

### Comparing `mure-1.0.0a6/LICENSE` & `mure-1.0.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `mure-1.0.0a6/README.md` & `mure-1.0.0b1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,28 @@
+Metadata-Version: 2.1
+Name: mure
+Version: 1.0.0b1
+Summary: Perform multiple HTTP requests concurrently – without worrying about async/await.
+Author: Severin Simmler
+Author-email: s.simmler@snapaddy.com
+Requires-Python: >=3.11,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: aiohttp[speedups] (>=3.8.5,<4.0.0)
+Requires-Dist: chardet (>=5.2.0,<6.0.0)
+Description-Content-Type: text/markdown
+
 # mure
 
 [![downloads](https://static.pepy.tech/personalized-badge/mure?period=total&units=international_system&left_color=black&right_color=black&left_text=downloads)](https://pepy.tech/project/mure)
 [![downloads/month](https://static.pepy.tech/personalized-badge/mure?period=month&units=abbreviation&left_color=black&right_color=black&left_text=downloads/month)](https://pepy.tech/project/mure)
 [![downloads/week](https://static.pepy.tech/personalized-badge/mure?period=week&units=abbreviation&left_color=black&right_color=black&left_text=downloads/week)](https://pepy.tech/project/mure)
 
-This is a thin layer on top of [`aiohttp`](https://docs.aiohttp.org/en/stable/) to perform multiple HTTP requests concurrently – without worrying about `async` functions.
+This is a thin layer on top of [`aiohttp`](https://docs.aiohttp.org/en/stable/) to perform multiple HTTP requests concurrently – without worrying about async/await.
 
 `mure` means **mu**ltiple **re**quests, but is also the German term for a form of mass wasting involving fast-moving flow of debris and dirt that has become liquified by the addition of water.
 
 ![Göscheneralp. Kolorierung des Dias durch Margrit Wehrli-Frey](https://upload.wikimedia.org/wikipedia/commons/thumb/6/6b/ETH-BIB-Muhrgang_zur_Kehlen-Reuss_vom_Rotfirn-Dia_247-13368.tif/lossy-page1-1280px-ETH-BIB-Muhrgang_zur_Kehlen-Reuss_vom_Rotfirn-Dia_247-13368.tif.jpg)
 
 (The photo was taken by [Leo Wehrli](https://de.wikipedia.org/wiki/Leo_Wehrli) and is licensed under CC BY-SA 4.0)
 
@@ -22,15 +36,15 @@
 
 ## Usage
 
 Pass a list of dictionaries with at least a value for `url` and get a `ResponseIterator` with the corresponding responses. The first request is fired as soon as you access the first response:
 
 ```python
 >>> import mure
->>> from mure.dtos import Resource
+>>> from mure.models import Resource
 >>> resources: list[Resource] = [
 ...     {"url": "https://httpbin.org/get"},
 ...     {"url": "https://httpbin.org/get", "params": {"foo": "bar"}},
 ...     {"url": "invalid"},
 ... ]
 >>> responses = mure.get(resources, batch_size=2)
 >>> responses
@@ -41,64 +55,45 @@
 {'url': 'https://httpbin.org/get'} status code: 200
 {'url': 'https://httpbin.org/get', 'params': {'foo': 'bar'}} status code: 200
 {'url': 'invalid'} status code: 0
 >>> responses
 <ResponseIterator: 0/3 pending>
 ```
 
-The keyword argument `batch_size` defines the number of requests to perform concurrently (don't be too greedy). The resources are requested batch-wise, i. e. only one batch of responses is kept in memory (depends of course also on how you use the `ResponseIterator`). Once you start accessing the first response of a batch, the next batch of resources is requested already in the background. So while you are doing something with a batch of responses (e.g. some CPU-heavy operation like parsing HTML), the next batch is already requested in the background.
+The keyword argument `batch_size` defines the number of requests to perform concurrently. The resources are requested lazy and in batches, i.e. only one batch of responses is kept in memory. Once you start accessing the first response of a batch, the next resource is requested already in the background.
 
 For example, if you have four resources, set `batch_size` to `2` and execute:
 
 ```python
 >>> next(responses)
 ```
 
-the first two resources are requested concurrently and blocks until both of the responses are available (i.e. if resource 1 takes 1 second and resource 2 takes 10 seconds, it blocks 10 seconds although resource 1 is already available after 1 second). Before the response of resource 1 is yielded, the next batch of resources (i.e. 3 and 4) is already requested in the background.
+the first two resources are requested concurrently and block until both of the responses are available (i.e. if resource 1 takes 1 second and resource 2 takes 10 seconds, it blocks 10 seconds although resource 1 is already available after 1 second). Before the response of resource 1 is yielded, the next batch of resources (i.e. 3 and 4) is already requested in the background.
 
 Executing `next()` a second time:
 
 ```python
 >>> next(responses)
 ```
 
-will be super fast, because the response of resource 2 is already available (1 and 2 were in the same batch). If you are lucky, executing `next()` a third time will be fast as well, because the next batch of resources was already requested when you executed `next(responses)` the first time.
+will be super fast, because the response of resource 2 is already available (1 and 2 were in the same batch).
 
 ### HTTP Methods
 
 There are convenience functions for GET, POST, HEAD, PUT, PATCH and DELETE requests, for example:
 
 ```python
 >>> resources = [
 ...     {"url": "https://httpbin.org/post"},
 ...     {"url": "https://httpbin.org/post", "json": {"foo": "bar"}},
 ...     {"url": "invalid"},
 ... ]
 >>> responses = mure.post(resources)
 ```
 
-You can even mix HTTP methods in the list of resources (but have to specify the method for each resource):
-
-```python
->>> resources = [
-...     {"method": "GET", "url": "https://httpbin.org/get"},
-...     {"method": "GET", "url": "https://httpbin.org/get", "params": {"foo": "bar"}},
-...     {"method": "POST", "url": "https://httpbin.org/post"},
-...     {"method": "POST", "url": "https://httpbin.org/post", "json": {"foo": "bar"}},
-...     {"method": "GET", "url": "invalid"},
-... ]
->>> responses = mure.request(resources)
-```
-
-## Tips
-
-- Set timeouts (e.g. 10 seconds) to avoid waiting for too long.
-- It might be a good idea to order the URLs to be requested by domain names so that DNS resolution is done once per domain. Once a domain's IP has been resolved, subsequent requests to the same domain can benefit from cached DNS resolutions. Also when using protocols like HTTP/1.1, connections to the same domain can be reused. Batching requests by domain can allow for connection reuse.
-- Shuffling URLs randomly might be an alternative if you do not request the same domain multiple times. This helps in distributing potential slow URLs across different batches.
-
 ### Verbosity
 
 Control verbosity with the `MURE_LOG_ERRORS` environment variable:
 
 ```python
 >>> import os
 >>> import mure
@@ -119,7 +114,25 @@
   File "/home/severin/git/mure/.env/lib/python3.11/site-packages/aiohttp/client_reqrep.py", line 305, in __init__
     self.update_host(url)
   File "/home/severin/git/mure/.env/lib/python3.11/site-packages/aiohttp/client_reqrep.py", line 364, in update_host
     raise InvalidURL(url)
 aiohttp.client_exceptions.InvalidURL: invalid
 Response(status=0, reason='<InvalidURL invalid>', ok=False, text='')
 ```
+
+### Caching
+
+You can cache responses either in-memory (`MemoryCache`) or on your disk (`DiskCache`) to avoid requesting the same resources over and over again:
+
+```python
+>>> import mure
+>>> from mure.cache import DiskCache
+>>> cache = DiskCache()
+>>> resources = [
+...     {"url": "https://httpbin.org/post"},
+...     {"url": "https://httpbin.org/post", "json": {"foo": "bar"}},
+... ]
+>>> responses = mure.post(resources, cache=cache)
+```
+
+`MemoryCache` holds requests and corresponding responses in a simple dictionary in memory, `DiskCache` is serializing to disk using Python's `shelve` module from the standard library.
+
```

### Comparing `mure-1.0.0a6/pyproject.toml` & `mure-1.0.0b1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,23 @@
-[project]
+[tool.poetry]
 name = "mure"
-version = "1.0.0a6"
-description = "Perform multiple HTTP requests concurrently – without worrying about async functions."
-authors = [{ name = "Severin Simmler", email = "s.simmler@snapaddy.com" }]
-dependencies = ["aiohttp>=3.9.3", "chardet>=5.2.0"]
+version = "1.0.0b1"
+description = "Perform multiple HTTP requests concurrently – without worrying about async/await."
+authors = ["Severin Simmler <s.simmler@snapaddy.com>"]
 readme = "README.md"
-requires-python = ">= 3.11, < 4"
 
-[build-system]
-requires = ["hatchling"]
-build-backend = "hatchling.build"
-
-[tool.rye]
-managed = true
-dev-dependencies = ["pytest>=8.1.1", "pre-commit>=3.7.0"]
-
-[tool.hatch.metadata]
-allow-direct-references = true
-
-[tool.hatch.build.targets.wheel]
-packages = ["mure"]
+[tool.poetry.dependencies]
+python = "^3.11"
+aiohttp = { extras = ["speedups"], version = "^3.8.5" }
+chardet = "^5.2.0"
+
+[tool.poetry.group.dev.dependencies]
+pytest = "^8.0.1"
+pre-commit = "^3.4.0"
+ruff = "^0.4.1"
 
 [tool.ruff]
 line-length = 99
 extend-include = ["*.ipynb"]
 
 [tool.ruff.lint.per-file-ignores]
 "__init__.py" = [
@@ -83,12 +77,16 @@
     "RUF001", # String contains ambiguous character
     "S608",   # Possible SQL injection vector through string-based query construction
     "S110",   # Consider logging the exception before pass
     "S112",   # Consider logging the exception before continue
     "S105",   # Possible hardcoded password
     "S320",   # Using lxml to parse untrusted data
     "S311",   # Standard pseudo-random generators are not suitable for cryptographic purposes
-    "S301",   # Use of `pickle` and modules that wrap it
+    "S301",   # Pickle is used to serialize data
 ]
 
 [tool.ruff.lint.pydocstyle]
 convention = "numpy"
+
+[build-system]
+requires = ["poetry-core"]
+build-backend = "poetry.core.masonry.api"
```

### Comparing `mure-1.0.0a6/PKG-INFO` & `mure-1.0.0b1/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,25 +1,14 @@
-Metadata-Version: 2.3
-Name: mure
-Version: 1.0.0a6
-Summary: Perform multiple HTTP requests concurrently – without worrying about async functions.
-Author-email: Severin Simmler <s.simmler@snapaddy.com>
-License-File: LICENSE
-Requires-Python: <4,>=3.11
-Requires-Dist: aiohttp>=3.9.3
-Requires-Dist: chardet>=5.2.0
-Description-Content-Type: text/markdown
-
 # mure
 
 [![downloads](https://static.pepy.tech/personalized-badge/mure?period=total&units=international_system&left_color=black&right_color=black&left_text=downloads)](https://pepy.tech/project/mure)
 [![downloads/month](https://static.pepy.tech/personalized-badge/mure?period=month&units=abbreviation&left_color=black&right_color=black&left_text=downloads/month)](https://pepy.tech/project/mure)
 [![downloads/week](https://static.pepy.tech/personalized-badge/mure?period=week&units=abbreviation&left_color=black&right_color=black&left_text=downloads/week)](https://pepy.tech/project/mure)
 
-This is a thin layer on top of [`aiohttp`](https://docs.aiohttp.org/en/stable/) to perform multiple HTTP requests concurrently – without worrying about `async` functions.
+This is a thin layer on top of [`aiohttp`](https://docs.aiohttp.org/en/stable/) to perform multiple HTTP requests concurrently – without worrying about async/await.
 
 `mure` means **mu**ltiple **re**quests, but is also the German term for a form of mass wasting involving fast-moving flow of debris and dirt that has become liquified by the addition of water.
 
 ![Göscheneralp. Kolorierung des Dias durch Margrit Wehrli-Frey](https://upload.wikimedia.org/wikipedia/commons/thumb/6/6b/ETH-BIB-Muhrgang_zur_Kehlen-Reuss_vom_Rotfirn-Dia_247-13368.tif/lossy-page1-1280px-ETH-BIB-Muhrgang_zur_Kehlen-Reuss_vom_Rotfirn-Dia_247-13368.tif.jpg)
 
 (The photo was taken by [Leo Wehrli](https://de.wikipedia.org/wiki/Leo_Wehrli) and is licensed under CC BY-SA 4.0)
 
@@ -33,15 +22,15 @@
 
 ## Usage
 
 Pass a list of dictionaries with at least a value for `url` and get a `ResponseIterator` with the corresponding responses. The first request is fired as soon as you access the first response:
 
 ```python
 >>> import mure
->>> from mure.dtos import Resource
+>>> from mure.models import Resource
 >>> resources: list[Resource] = [
 ...     {"url": "https://httpbin.org/get"},
 ...     {"url": "https://httpbin.org/get", "params": {"foo": "bar"}},
 ...     {"url": "invalid"},
 ... ]
 >>> responses = mure.get(resources, batch_size=2)
 >>> responses
@@ -52,64 +41,45 @@
 {'url': 'https://httpbin.org/get'} status code: 200
 {'url': 'https://httpbin.org/get', 'params': {'foo': 'bar'}} status code: 200
 {'url': 'invalid'} status code: 0
 >>> responses
 <ResponseIterator: 0/3 pending>
 ```
 
-The keyword argument `batch_size` defines the number of requests to perform concurrently (don't be too greedy). The resources are requested batch-wise, i. e. only one batch of responses is kept in memory (depends of course also on how you use the `ResponseIterator`). Once you start accessing the first response of a batch, the next batch of resources is requested already in the background. So while you are doing something with a batch of responses (e.g. some CPU-heavy operation like parsing HTML), the next batch is already requested in the background.
+The keyword argument `batch_size` defines the number of requests to perform concurrently. The resources are requested lazy and in batches, i.e. only one batch of responses is kept in memory. Once you start accessing the first response of a batch, the next resource is requested already in the background.
 
 For example, if you have four resources, set `batch_size` to `2` and execute:
 
 ```python
 >>> next(responses)
 ```
 
-the first two resources are requested concurrently and blocks until both of the responses are available (i.e. if resource 1 takes 1 second and resource 2 takes 10 seconds, it blocks 10 seconds although resource 1 is already available after 1 second). Before the response of resource 1 is yielded, the next batch of resources (i.e. 3 and 4) is already requested in the background.
+the first two resources are requested concurrently and block until both of the responses are available (i.e. if resource 1 takes 1 second and resource 2 takes 10 seconds, it blocks 10 seconds although resource 1 is already available after 1 second). Before the response of resource 1 is yielded, the next batch of resources (i.e. 3 and 4) is already requested in the background.
 
 Executing `next()` a second time:
 
 ```python
 >>> next(responses)
 ```
 
-will be super fast, because the response of resource 2 is already available (1 and 2 were in the same batch). If you are lucky, executing `next()` a third time will be fast as well, because the next batch of resources was already requested when you executed `next(responses)` the first time.
+will be super fast, because the response of resource 2 is already available (1 and 2 were in the same batch).
 
 ### HTTP Methods
 
 There are convenience functions for GET, POST, HEAD, PUT, PATCH and DELETE requests, for example:
 
 ```python
 >>> resources = [
 ...     {"url": "https://httpbin.org/post"},
 ...     {"url": "https://httpbin.org/post", "json": {"foo": "bar"}},
 ...     {"url": "invalid"},
 ... ]
 >>> responses = mure.post(resources)
 ```
 
-You can even mix HTTP methods in the list of resources (but have to specify the method for each resource):
-
-```python
->>> resources = [
-...     {"method": "GET", "url": "https://httpbin.org/get"},
-...     {"method": "GET", "url": "https://httpbin.org/get", "params": {"foo": "bar"}},
-...     {"method": "POST", "url": "https://httpbin.org/post"},
-...     {"method": "POST", "url": "https://httpbin.org/post", "json": {"foo": "bar"}},
-...     {"method": "GET", "url": "invalid"},
-... ]
->>> responses = mure.request(resources)
-```
-
-## Tips
-
-- Set timeouts (e.g. 10 seconds) to avoid waiting for too long.
-- It might be a good idea to order the URLs to be requested by domain names so that DNS resolution is done once per domain. Once a domain's IP has been resolved, subsequent requests to the same domain can benefit from cached DNS resolutions. Also when using protocols like HTTP/1.1, connections to the same domain can be reused. Batching requests by domain can allow for connection reuse.
-- Shuffling URLs randomly might be an alternative if you do not request the same domain multiple times. This helps in distributing potential slow URLs across different batches.
-
 ### Verbosity
 
 Control verbosity with the `MURE_LOG_ERRORS` environment variable:
 
 ```python
 >>> import os
 >>> import mure
@@ -130,7 +100,24 @@
   File "/home/severin/git/mure/.env/lib/python3.11/site-packages/aiohttp/client_reqrep.py", line 305, in __init__
     self.update_host(url)
   File "/home/severin/git/mure/.env/lib/python3.11/site-packages/aiohttp/client_reqrep.py", line 364, in update_host
     raise InvalidURL(url)
 aiohttp.client_exceptions.InvalidURL: invalid
 Response(status=0, reason='<InvalidURL invalid>', ok=False, text='')
 ```
+
+### Caching
+
+You can cache responses either in-memory (`MemoryCache`) or on your disk (`DiskCache`) to avoid requesting the same resources over and over again:
+
+```python
+>>> import mure
+>>> from mure.cache import DiskCache
+>>> cache = DiskCache()
+>>> resources = [
+...     {"url": "https://httpbin.org/post"},
+...     {"url": "https://httpbin.org/post", "json": {"foo": "bar"}},
+... ]
+>>> responses = mure.post(resources, cache=cache)
+```
+
+`MemoryCache` holds requests and corresponding responses in a simple dictionary in memory, `DiskCache` is serializing to disk using Python's `shelve` module from the standard library.
```


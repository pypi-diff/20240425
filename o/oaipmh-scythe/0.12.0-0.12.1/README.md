# Comparing `tmp/oaipmh_scythe-0.12.0.tar.gz` & `tmp/oaipmh_scythe-0.12.1.tar.gz`

## Comparing `oaipmh_scythe-0.12.0.tar` & `oaipmh_scythe-0.12.1.tar`

### file list

```diff
@@ -1,16 +1,29 @@
--rw-r--r--   0        0        0    10927 2020-02-02 00:00:00.000000 oaipmh_scythe-0.12.0/CHANGELOG.md
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 oaipmh_scythe-0.12.0/src/oaipmh_scythe/__about__.py
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 oaipmh_scythe-0.12.0/src/oaipmh_scythe/__init__.py
--rw-r--r--   0        0        0    18213 2020-02-02 00:00:00.000000 oaipmh_scythe-0.12.0/src/oaipmh_scythe/client.py
--rw-r--r--   0        0        0     4335 2020-02-02 00:00:00.000000 oaipmh_scythe-0.12.0/src/oaipmh_scythe/exceptions.py
--rw-r--r--   0        0        0     8885 2020-02-02 00:00:00.000000 oaipmh_scythe-0.12.0/src/oaipmh_scythe/iterator.py
--rw-r--r--   0        0        0    11670 2020-02-02 00:00:00.000000 oaipmh_scythe-0.12.0/src/oaipmh_scythe/models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 oaipmh_scythe-0.12.0/src/oaipmh_scythe/py.typed
--rw-r--r--   0        0        0     1969 2020-02-02 00:00:00.000000 oaipmh_scythe-0.12.0/src/oaipmh_scythe/response.py
--rw-r--r--   0        0        0     5591 2020-02-02 00:00:00.000000 oaipmh_scythe-0.12.0/src/oaipmh_scythe/utils.py
--rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 oaipmh_scythe-0.12.0/.gitignore
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 oaipmh_scythe-0.12.0/AUTHORS.md
--rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 oaipmh_scythe-0.12.0/LICENSE
--rw-r--r--   0        0        0     7256 2020-02-02 00:00:00.000000 oaipmh_scythe-0.12.0/README.md
--rw-r--r--   0        0        0     7318 2020-02-02 00:00:00.000000 oaipmh_scythe-0.12.0/pyproject.toml
--rw-r--r--   0        0        0     9251 2020-02-02 00:00:00.000000 oaipmh_scythe-0.12.0/PKG-INFO
+-rw-r--r--   0        0        0    12092 2020-02-02 00:00:00.000000 oaipmh_scythe-0.12.1/CHANGELOG.md
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 oaipmh_scythe-0.12.1/docs/src/changelog.md
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 oaipmh_scythe-0.12.1/docs/src/contributing.md
+-rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 oaipmh_scythe-0.12.1/docs/src/customizing.md
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 oaipmh_scythe-0.12.1/docs/src/index.md
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 oaipmh_scythe-0.12.1/docs/src/license.md
+-rw-r--r--   0        0        0     3013 2020-02-02 00:00:00.000000 oaipmh_scythe-0.12.1/docs/src/oaipmh.md
+-rw-r--r--   0        0        0    11441 2020-02-02 00:00:00.000000 oaipmh_scythe-0.12.1/docs/src/tutorial.md
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 oaipmh_scythe-0.12.1/docs/src/api/client.md
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 oaipmh_scythe-0.12.1/docs/src/api/exceptions.md
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 oaipmh_scythe-0.12.1/docs/src/api/iterator.md
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 oaipmh_scythe-0.12.1/docs/src/api/models.md
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 oaipmh_scythe-0.12.1/docs/src/api/response.md
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 oaipmh_scythe-0.12.1/docs/src/api/utils.md
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 oaipmh_scythe-0.12.1/src/oaipmh_scythe/__about__.py
+-rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 oaipmh_scythe-0.12.1/src/oaipmh_scythe/__init__.py
+-rw-r--r--   0        0        0    18229 2020-02-02 00:00:00.000000 oaipmh_scythe-0.12.1/src/oaipmh_scythe/client.py
+-rw-r--r--   0        0        0     4336 2020-02-02 00:00:00.000000 oaipmh_scythe-0.12.1/src/oaipmh_scythe/exceptions.py
+-rw-r--r--   0        0        0     8881 2020-02-02 00:00:00.000000 oaipmh_scythe-0.12.1/src/oaipmh_scythe/iterator.py
+-rw-r--r--   0        0        0    11670 2020-02-02 00:00:00.000000 oaipmh_scythe-0.12.1/src/oaipmh_scythe/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 oaipmh_scythe-0.12.1/src/oaipmh_scythe/py.typed
+-rw-r--r--   0        0        0     1969 2020-02-02 00:00:00.000000 oaipmh_scythe-0.12.1/src/oaipmh_scythe/response.py
+-rw-r--r--   0        0        0     5591 2020-02-02 00:00:00.000000 oaipmh_scythe-0.12.1/src/oaipmh_scythe/utils.py
+-rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 oaipmh_scythe-0.12.1/.gitignore
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 oaipmh_scythe-0.12.1/AUTHORS.md
+-rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 oaipmh_scythe-0.12.1/LICENSE
+-rw-r--r--   0        0        0     7280 2020-02-02 00:00:00.000000 oaipmh_scythe-0.12.1/README.md
+-rw-r--r--   0        0        0     7408 2020-02-02 00:00:00.000000 oaipmh_scythe-0.12.1/pyproject.toml
+-rw-r--r--   0        0        0     9275 2020-02-02 00:00:00.000000 oaipmh_scythe-0.12.1/PKG-INFO
```

### Comparing `oaipmh_scythe-0.12.0/CHANGELOG.md` & `oaipmh_scythe-0.12.1/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,18 +2,36 @@
 
 All notable changes to this project will be documented in this file.
 
 This project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html). See
 [conventional commits](https://www.conventionalcommits.org/en/v1.0.0/) for commit guidelines.
 
 
-## [Unreleased](https://github.com/afuetterer/oaipmh-scythe/compare/0.12.0...main)
+## [Unreleased](https://github.com/afuetterer/oaipmh-scythe/compare/0.12.1...main)
 
 
 
+## [0.12.1](https://github.com/afuetterer/oaipmh-scythe/compare/0.12.0...0.12.1) (2024-04-25)
+
+### Bug Fixes
+
+- **exceptions:** rename nometadataformat to nometadataformats (#349) ([`255acb2`](https://github.com/afuetterer/oaipmh-scythe/commit/255acb257a35533e78b0eb1aed85704c386e4e0a))
+
+### Code Refactoring
+
+- make all exceptions available in the main init file (#348) ([`bad60ff`](https://github.com/afuetterer/oaipmh-scythe/commit/bad60ff61f6a8ceb96134e97e321eca93cbc6eab))
+- **client:** set up explicit default encoding in httpx.Client (#330) ([`25ef4cb`](https://github.com/afuetterer/oaipmh-scythe/commit/25ef4cbde2488426b7736e1240b5de798bd6fe34))
+- **iterator:** rename params argument to query in itemiterator (#329) ([`1de6cd5`](https://github.com/afuetterer/oaipmh-scythe/commit/1de6cd57efbf64dc44762243024b1b81bdcaac32))
+
+### Documentation
+
+- add api reference pages for all modules (#344) ([`8578031`](https://github.com/afuetterer/oaipmh-scythe/commit/8578031a21fd35ae7f8e0cd66fc955b8cc84bea0))
+- add python standard library inventory (#338) ([`20d176c`](https://github.com/afuetterer/oaipmh-scythe/commit/20d176cc1bbf00e40f19c836681d3bb6b46f5390))
+
+
 ## [0.12.0](https://github.com/afuetterer/oaipmh-scythe/compare/0.11.0...0.12.0) (2024-04-04)
 
 ### Features
 
 - **client:** add authentication parameter (#316) ([`035c0fe`](https://github.com/afuetterer/oaipmh-scythe/commit/035c0fe4af20c1a749ce3dc02d1f5174aa13c57c))
 
 ### Documentation
```

### Comparing `oaipmh_scythe-0.12.0/src/oaipmh_scythe/client.py` & `oaipmh_scythe-0.12.1/src/oaipmh_scythe/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,15 +79,15 @@
         endpoint: str,
         http_method: str = "GET",
         iterator: type[BaseOAIIterator] = OAIItemIterator,
         max_retries: int = 0,
         retry_status_codes: Iterable[int] | None = None,
         default_retry_after: int = 60,
         class_mapping: dict[str, type[OAIItem]] | None = None,
-        encoding: str | None = None,
+        encoding: str = "utf-8",
         auth: AuthTypes | None = None,
         timeout: int = 60,
     ):
         self.endpoint = endpoint
         if http_method not in ("GET", "POST"):
             raise ValueError("Invalid HTTP method: %s! Must be GET or POST.")
         self.http_method = http_method
@@ -115,15 +115,19 @@
 
         Returns:
             A reusable HTTP client instance for making HTTP requests.
         """
         if self._client is None or self._client.is_closed:
             headers = {"Accept": "text/xml; charset=utf-8", "user-agent": USER_AGENT}
             self._client = httpx.Client(
-                headers=headers, timeout=self.timeout, auth=self.auth, event_hooks={"response": [log_response]}
+                headers=headers,
+                timeout=self.timeout,
+                auth=self.auth,
+                default_encoding=self.encoding,
+                event_hooks={"response": [log_response]},
             )
         return self._client
 
     def close(self) -> None:
         """Close the internal HTTP client if it exists and is open.
 
         This method is responsible for explicitly closing the `httpx.Client` instance used
@@ -164,16 +168,14 @@
         for _ in range(self.max_retries):
             if httpx.codes.is_error(http_response.status_code) and http_response.status_code in self.retry_status_codes:
                 retry_after = self.get_retry_after(http_response)
                 logger.warning("HTTP %d! Retrying after %d seconds...", http_response.status_code, retry_after)
                 time.sleep(retry_after)
                 http_response = self._request(query)
         http_response.raise_for_status()
-        if self.encoding:
-            http_response.encoding = self.encoding
         return OAIResponse(http_response, params=query)
 
     def _request(self, query: dict[str, str]) -> httpx.Response:
         """Send an HTTP request to the OAI server using the configured HTTP method and given query parameters.
 
         Args:
             query: A dictionary containing the request parameters.
```

### Comparing `oaipmh_scythe-0.12.0/src/oaipmh_scythe/exceptions.py` & `oaipmh_scythe-0.12.1/src/oaipmh_scythe/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,15 +74,15 @@
 class NoSetHierarchy(OAIPMHException):
     """Exception raised when sets are not supported by the repository.
 
     This error indicates that the repository does not support the concept of set hierarchies.
     """
 
 
-class NoMetadataFormat(OAIPMHException):
+class NoMetadataFormats(OAIPMHException):
     """Exception raised when there are no available metadata formats for the specified item.
 
     Indicates a lack of metadata formats that can be disseminated for the requested item.
     """
 
 
 class NoRecordsMatch(OAIPMHException):
```

### Comparing `oaipmh_scythe-0.12.0/src/oaipmh_scythe/iterator.py` & `oaipmh_scythe-0.12.1/src/oaipmh_scythe/iterator.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,23 +154,23 @@
     """An iterator class for iterating over various types of OAI items aggregated via OAI-PMH.
 
     This iterator is designed to handle the iteration of specific OAI items, such as records or sets, from a repository.
     It extends the functionality of the BaseOAIIterator to parse and yield individual items from the OAI-PMH responses.
 
     Args:
         scythe: The Scythe instance used for making OAI-PMH requests.
-        params: A dictionary of OAI-PMH request parameters.
+        query: A dictionary of OAI-PMH request parameters.
         ignore_deleted: A boolean indicating whether to ignore deleted records in the response.
     """
 
-    def __init__(self, scythe: Scythe, params: dict[str, str], ignore_deleted: bool = False) -> None:
-        self.verb = params["verb"]
+    def __init__(self, scythe: Scythe, query: dict[str, str], ignore_deleted: bool = False) -> None:
+        self.verb = query["verb"]
         self.mapper = scythe.class_mapping[self.verb]
         self.element = VERBS_ELEMENTS[self.verb]
-        super().__init__(scythe, params, ignore_deleted)
+        super().__init__(scythe, query, ignore_deleted)
 
     def _next_response(self) -> None:
         """Fetch and process the next response from the OAI server.
 
         Override the BaseOAIIterator's _next_response method to parse and set up the iterator
         for the specific elements (e.g. records, headers) based on the current resumption token.
         """
```

### Comparing `oaipmh_scythe-0.12.0/src/oaipmh_scythe/models.py` & `oaipmh_scythe-0.12.1/src/oaipmh_scythe/models.py`

 * *Files identical despite different names*

### Comparing `oaipmh_scythe-0.12.0/src/oaipmh_scythe/response.py` & `oaipmh_scythe-0.12.1/src/oaipmh_scythe/response.py`

 * *Files identical despite different names*

### Comparing `oaipmh_scythe-0.12.0/src/oaipmh_scythe/utils.py` & `oaipmh_scythe-0.12.1/src/oaipmh_scythe/utils.py`

 * *Files identical despite different names*

### Comparing `oaipmh_scythe-0.12.0/.gitignore` & `oaipmh_scythe-0.12.1/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,15 @@
 env/
 venv/
 ENV/
 env.bak/
 venv.bak/
 
 # mkdocs documentation
-/site
+docs/site
 
 # mypy
 .mypy_cache/
 .dmypy.json
 dmypy.json
 
 # Cython debug symbols
```

### Comparing `oaipmh_scythe-0.12.0/LICENSE` & `oaipmh_scythe-0.12.1/LICENSE`

 * *Files identical despite different names*

### Comparing `oaipmh_scythe-0.12.0/README.md` & `oaipmh_scythe-0.12.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -53,22 +53,22 @@
 
 ## Similar Projects
 
 There are a couple of similar projects available on [PyPI](https://pypi.org/search/?q=oai-pmh) and GitHub, e.g. via the
 topics [oai-pmh](https://github.com/topics/oai-pmh) and [oai-pmh-client](https://github.com/topics/oai-pmh-client).
 Among them are these implementations in Python:
 
-| Project                                                                          | Description                        | Last commit                                                                                           |
-| -------------------------------------------------------------------------------- | ---------------------------------- | ----------------------------------------------------------------------------------------------------- |
-| [sickle](https://github.com/mloesch/sickle)                                      | oaipmh-scythe is a fork of sickle  | ![last-commit](https://img.shields.io/github/last-commit/mloesch/sickle)                              |
-| [pyoai](https://github.com/infrae/pyoai)                                         | sickle was inspired by pyoai       | ![last-commit](https://img.shields.io/github/last-commit/infrae/pyoai)                                |
-| [pyoaiharvester](https://github.com/vphill/pyoaiharvester)                       | oai-pmh harvester CLI              | ![last-commit](https://img.shields.io/github/last-commit/vphill/pyoaiharvester)                       |
-| [ddblabs-ometha](https://github.com/Deutsche-Digitale-Bibliothek/ddblabs-ometha) | oai-pmh harvester with CLI and TUI | ![last-commit](https://img.shields.io/github/last-commit/Deutsche-Digitale-Bibliothek/ddblabs-ometha) |
-| [oai-harvest](https://github.com/bloomonkey/oai-harvest)                         | uses pyoai internally              | ![last-commit](https://img.shields.io/github/last-commit/bloomonkey/oai-harvest)                      |
-| [oai-pmh-harvester](https://github.com/MITLibraries/oai-pmh-harvester)           | uses sickle internally             | ![last-commit](https://img.shields.io/github/last-commit/MITLibraries/oai-pmh-harvester)              |
+| Project                                                                          | Description                           | Last commit                                                                                           |
+| -------------------------------------------------------------------------------- | ------------------------------------- | ----------------------------------------------------------------------------------------------------- |
+| [sickle](https://github.com/mloesch/sickle)                                      | `oaipmh-scythe` is a fork of `sickle` | ![last-commit](https://img.shields.io/github/last-commit/mloesch/sickle)                              |
+| [pyoai](https://github.com/infrae/pyoai)                                         | `sickle` was inspired by `pyoai`      | ![last-commit](https://img.shields.io/github/last-commit/infrae/pyoai)                                |
+| [pyoaiharvester](https://github.com/vphill/pyoaiharvester)                       | oai-pmh harvester CLI                 | ![last-commit](https://img.shields.io/github/last-commit/vphill/pyoaiharvester)                       |
+| [ddblabs-ometha](https://github.com/Deutsche-Digitale-Bibliothek/ddblabs-ometha) | oai-pmh harvester with CLI and TUI    | ![last-commit](https://img.shields.io/github/last-commit/Deutsche-Digitale-Bibliothek/ddblabs-ometha) |
+| [oai-harvest](https://github.com/bloomonkey/oai-harvest)                         | uses `pyoai` internally               | ![last-commit](https://img.shields.io/github/last-commit/bloomonkey/oai-harvest)                      |
+| [oai-pmh-harvester](https://github.com/MITLibraries/oai-pmh-harvester)           | uses `sickle` internally              | ![last-commit](https://img.shields.io/github/last-commit/MITLibraries/oai-pmh-harvester)              |
 
 There are also similar projects available in [Java](https://github.com/topics/oai-pmh-client?l=java) and
 [PHP](https://github.com/topics/oai-pmh-client?l=php).
 
 ## Acknowledgments
 
 This is a fork of [sickle](https://github.com/mloesch/sickle) which was originally written by Mathias Loesch.
```

### Comparing `oaipmh_scythe-0.12.0/pyproject.toml` & `oaipmh_scythe-0.12.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -97,16 +97,16 @@
   python -c "import json;print(json.load(open('coverage.json'))['totals']['percent_covered_display'])"
 """
 
 [tool.hatch.envs.docs]
 features = ["docs"]
 template = "docs"
 [tool.hatch.envs.docs.scripts]
-build = "mkdocs build --strict --config-file=docs/mkdocs.yml"
-serve = "mkdocs serve --strict --config-file=docs/mkdocs.yml"
+build = "mkdocs build --config-file=docs/mkdocs.yml"
+serve = "mkdocs serve --verbose --config-file=docs/mkdocs.yml"
 deploy = "mkdocs gh-deploy --force --config-file=docs/mkdocs.yml"
 
 [tool.hatch.envs.release]
 features = ["release"]
 template = "release"
 [tool.hatch.envs.release.scripts]
 next-version = "semantic-release version --print"
@@ -138,15 +138,18 @@
   "I",    # isort
   "G",    # flake8-logging-format
   "PERF", # perflint-perf
   "PGH",  # pygrep-hooks
   "PIE",  # flake8-pie
   "PL",   # pylint
   "PT",   # flake8-pytest-style
+  "RET",  # flake8-return
+  "RSE",  # flake8-raise
   "RUF",  # ruff
+  "SIM",  # flake8-simplify
   "TCH",  # flake8-type-checking
   "T20",  # flake8-print
   "UP",   # pyupgrade
   "W",    # pycodestyle
   "YTT",  # flake8-2020
 ]
 ignore = [
@@ -250,16 +253,16 @@
 logging_use_named_masks = true
 major_on_zero = false
 tag_format = "{version}"
 version_variables = [
   "src/oaipmh_scythe/__about__.py:__version__",
 ]
 build_command = """
-python -m pip install build
-python -m build
+python -m pip install build[uv]
+python -m build --installer=uv
 """
 changelog.template_dir = ".github/templates"
 changelog.environment.keep_trailing_newline = true
 
 # typos
 # Ref: https://github.com/crate-ci/typos/blob/master/docs/reference.md
 # ------------------------------------------------------------------------------
```

### Comparing `oaipmh_scythe-0.12.0/PKG-INFO` & `oaipmh_scythe-0.12.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: oaipmh-scythe
-Version: 0.12.0
+Version: 0.12.1
 Summary: A Scythe for harvesting OAI-PMH repositories.
 Project-URL: Changelog, https://github.com/afuetterer/oaipmh-scythe/blob/main/CHANGELOG.md
 Project-URL: Documentation, https://afuetterer.github.io/oaipmh-scythe
 Project-URL: Issues, https://github.com/afuetterer/oaipmh-scythe/issues
 Project-URL: Repository, https://github.com/afuetterer/oaipmh-scythe.git
 Author: Heinz-Alexander Fütterer
 License: BSD-3-Clause
@@ -99,22 +99,22 @@
 
 ## Similar Projects
 
 There are a couple of similar projects available on [PyPI](https://pypi.org/search/?q=oai-pmh) and GitHub, e.g. via the
 topics [oai-pmh](https://github.com/topics/oai-pmh) and [oai-pmh-client](https://github.com/topics/oai-pmh-client).
 Among them are these implementations in Python:
 
-| Project                                                                          | Description                        | Last commit                                                                                           |
-| -------------------------------------------------------------------------------- | ---------------------------------- | ----------------------------------------------------------------------------------------------------- |
-| [sickle](https://github.com/mloesch/sickle)                                      | oaipmh-scythe is a fork of sickle  | ![last-commit](https://img.shields.io/github/last-commit/mloesch/sickle)                              |
-| [pyoai](https://github.com/infrae/pyoai)                                         | sickle was inspired by pyoai       | ![last-commit](https://img.shields.io/github/last-commit/infrae/pyoai)                                |
-| [pyoaiharvester](https://github.com/vphill/pyoaiharvester)                       | oai-pmh harvester CLI              | ![last-commit](https://img.shields.io/github/last-commit/vphill/pyoaiharvester)                       |
-| [ddblabs-ometha](https://github.com/Deutsche-Digitale-Bibliothek/ddblabs-ometha) | oai-pmh harvester with CLI and TUI | ![last-commit](https://img.shields.io/github/last-commit/Deutsche-Digitale-Bibliothek/ddblabs-ometha) |
-| [oai-harvest](https://github.com/bloomonkey/oai-harvest)                         | uses pyoai internally              | ![last-commit](https://img.shields.io/github/last-commit/bloomonkey/oai-harvest)                      |
-| [oai-pmh-harvester](https://github.com/MITLibraries/oai-pmh-harvester)           | uses sickle internally             | ![last-commit](https://img.shields.io/github/last-commit/MITLibraries/oai-pmh-harvester)              |
+| Project                                                                          | Description                           | Last commit                                                                                           |
+| -------------------------------------------------------------------------------- | ------------------------------------- | ----------------------------------------------------------------------------------------------------- |
+| [sickle](https://github.com/mloesch/sickle)                                      | `oaipmh-scythe` is a fork of `sickle` | ![last-commit](https://img.shields.io/github/last-commit/mloesch/sickle)                              |
+| [pyoai](https://github.com/infrae/pyoai)                                         | `sickle` was inspired by `pyoai`      | ![last-commit](https://img.shields.io/github/last-commit/infrae/pyoai)                                |
+| [pyoaiharvester](https://github.com/vphill/pyoaiharvester)                       | oai-pmh harvester CLI                 | ![last-commit](https://img.shields.io/github/last-commit/vphill/pyoaiharvester)                       |
+| [ddblabs-ometha](https://github.com/Deutsche-Digitale-Bibliothek/ddblabs-ometha) | oai-pmh harvester with CLI and TUI    | ![last-commit](https://img.shields.io/github/last-commit/Deutsche-Digitale-Bibliothek/ddblabs-ometha) |
+| [oai-harvest](https://github.com/bloomonkey/oai-harvest)                         | uses `pyoai` internally               | ![last-commit](https://img.shields.io/github/last-commit/bloomonkey/oai-harvest)                      |
+| [oai-pmh-harvester](https://github.com/MITLibraries/oai-pmh-harvester)           | uses `sickle` internally              | ![last-commit](https://img.shields.io/github/last-commit/MITLibraries/oai-pmh-harvester)              |
 
 There are also similar projects available in [Java](https://github.com/topics/oai-pmh-client?l=java) and
 [PHP](https://github.com/topics/oai-pmh-client?l=php).
 
 ## Acknowledgments
 
 This is a fork of [sickle](https://github.com/mloesch/sickle) which was originally written by Mathias Loesch.
```


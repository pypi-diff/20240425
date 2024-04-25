# Comparing `tmp/docker_tidy-2.1.7.tar.gz` & `tmp/docker_tidy-2.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docker_tidy-2.1.7.tar", max compression
+gzip compressed data, was "docker_tidy-2.1.8.tar", max compression
```

## Comparing `docker_tidy-2.1.7.tar` & `docker_tidy-2.1.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0    11366 2024-04-14 09:48:03.261774 docker_tidy-2.1.7/LICENSE
--rw-r--r--   0        0        0     1748 2024-04-14 09:48:03.261774 docker_tidy-2.1.7/README.md
--rw-r--r--   0        0        0       46 2024-04-14 09:48:17.037833 docker_tidy-2.1.7/dockertidy/__init__.py
--rw-r--r--   0        0        0     3046 2024-04-14 09:48:03.265774 docker_tidy-2.1.7/dockertidy/autostop.py
--rw-r--r--   0        0        0     4807 2024-04-14 09:48:03.265774 docker_tidy-2.1.7/dockertidy/cli.py
--rw-r--r--   0        0        0     8462 2024-04-14 09:48:03.265774 docker_tidy-2.1.7/dockertidy/config.py
--rw-r--r--   0        0        0      384 2024-04-14 09:48:03.265774 docker_tidy-2.1.7/dockertidy/exception.py
--rw-r--r--   0        0        0    11649 2024-04-14 09:48:03.265774 docker_tidy-2.1.7/dockertidy/garbage_collector.py
--rw-r--r--   0        0        0     5866 2024-04-14 09:48:03.265774 docker_tidy-2.1.7/dockertidy/logger.py
--rw-r--r--   0        0        0     1206 2024-04-14 09:48:03.265774 docker_tidy-2.1.7/dockertidy/parser.py
--rw-r--r--   0        0        0        0 2024-04-14 09:48:03.713777 docker_tidy-2.1.7/dockertidy/test/__init__.py
--rw-r--r--   0        0        0        0 2024-04-14 09:48:03.713777 docker_tidy-2.1.7/dockertidy/test/fixtures/__init__.py
--rw-r--r--   0        0        0     1942 2024-04-14 09:48:03.265774 docker_tidy-2.1.7/dockertidy/test/fixtures/fixtures.py
--rw-r--r--   0        0        0     1244 2024-04-14 09:48:03.265774 docker_tidy-2.1.7/dockertidy/test/unit/test_autostop.py
--rw-r--r--   0        0        0    12327 2024-04-14 09:48:03.265774 docker_tidy-2.1.7/dockertidy/test/unit/test_garbagecollector.py
--rw-r--r--   0        0        0     1065 2024-04-14 09:48:03.265774 docker_tidy-2.1.7/dockertidy/utils.py
--rw-r--r--   0        0        0     3235 2024-04-14 09:48:17.033833 docker_tidy-2.1.7/pyproject.toml
--rw-r--r--   0        0        0     3703 1970-01-01 00:00:00.000000 docker_tidy-2.1.7/PKG-INFO
+-rw-r--r--   0        0        0    11366 2024-04-25 08:27:17.019060 docker_tidy-2.1.8/LICENSE
+-rw-r--r--   0        0        0     1748 2024-04-25 08:27:17.019060 docker_tidy-2.1.8/README.md
+-rw-r--r--   0        0        0       46 2024-04-25 08:27:30.798954 docker_tidy-2.1.8/dockertidy/__init__.py
+-rw-r--r--   0        0        0     3046 2024-04-25 08:27:17.019060 docker_tidy-2.1.8/dockertidy/autostop.py
+-rw-r--r--   0        0        0     4807 2024-04-25 08:27:17.019060 docker_tidy-2.1.8/dockertidy/cli.py
+-rw-r--r--   0        0        0     8462 2024-04-25 08:27:17.019060 docker_tidy-2.1.8/dockertidy/config.py
+-rw-r--r--   0        0        0      384 2024-04-25 08:27:17.019060 docker_tidy-2.1.8/dockertidy/exception.py
+-rw-r--r--   0        0        0    11649 2024-04-25 08:27:17.019060 docker_tidy-2.1.8/dockertidy/garbage_collector.py
+-rw-r--r--   0        0        0     5866 2024-04-25 08:27:17.019060 docker_tidy-2.1.8/dockertidy/logger.py
+-rw-r--r--   0        0        0     1206 2024-04-25 08:27:17.023060 docker_tidy-2.1.8/dockertidy/parser.py
+-rw-r--r--   0        0        0        0 2024-04-25 08:27:17.823053 docker_tidy-2.1.8/dockertidy/test/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 08:27:17.823053 docker_tidy-2.1.8/dockertidy/test/fixtures/__init__.py
+-rw-r--r--   0        0        0     1942 2024-04-25 08:27:17.023060 docker_tidy-2.1.8/dockertidy/test/fixtures/fixtures.py
+-rw-r--r--   0        0        0     1244 2024-04-25 08:27:17.023060 docker_tidy-2.1.8/dockertidy/test/unit/test_autostop.py
+-rw-r--r--   0        0        0    12327 2024-04-25 08:27:17.023060 docker_tidy-2.1.8/dockertidy/test/unit/test_garbagecollector.py
+-rw-r--r--   0        0        0     1065 2024-04-25 08:27:17.023060 docker_tidy-2.1.8/dockertidy/utils.py
+-rw-r--r--   0        0        0     3235 2024-04-25 08:27:30.798954 docker_tidy-2.1.8/pyproject.toml
+-rw-r--r--   0        0        0     3703 1970-01-01 00:00:00.000000 docker_tidy-2.1.8/PKG-INFO
```

### Comparing `docker_tidy-2.1.7/LICENSE` & `docker_tidy-2.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `docker_tidy-2.1.7/README.md` & `docker_tidy-2.1.8/README.md`

 * *Files identical despite different names*

### Comparing `docker_tidy-2.1.7/dockertidy/autostop.py` & `docker_tidy-2.1.8/dockertidy/autostop.py`

 * *Files identical despite different names*

### Comparing `docker_tidy-2.1.7/dockertidy/cli.py` & `docker_tidy-2.1.8/dockertidy/cli.py`

 * *Files identical despite different names*

### Comparing `docker_tidy-2.1.7/dockertidy/config.py` & `docker_tidy-2.1.8/dockertidy/config.py`

 * *Files identical despite different names*

### Comparing `docker_tidy-2.1.7/dockertidy/garbage_collector.py` & `docker_tidy-2.1.8/dockertidy/garbage_collector.py`

 * *Files identical despite different names*

### Comparing `docker_tidy-2.1.7/dockertidy/logger.py` & `docker_tidy-2.1.8/dockertidy/logger.py`

 * *Files identical despite different names*

### Comparing `docker_tidy-2.1.7/dockertidy/parser.py` & `docker_tidy-2.1.8/dockertidy/parser.py`

 * *Files identical despite different names*

### Comparing `docker_tidy-2.1.7/dockertidy/test/fixtures/fixtures.py` & `docker_tidy-2.1.8/dockertidy/test/fixtures/fixtures.py`

 * *Files identical despite different names*

### Comparing `docker_tidy-2.1.7/dockertidy/test/unit/test_autostop.py` & `docker_tidy-2.1.8/dockertidy/test/unit/test_autostop.py`

 * *Files identical despite different names*

### Comparing `docker_tidy-2.1.7/dockertidy/test/unit/test_garbagecollector.py` & `docker_tidy-2.1.8/dockertidy/test/unit/test_garbagecollector.py`

 * *Files identical despite different names*

### Comparing `docker_tidy-2.1.7/dockertidy/utils.py` & `docker_tidy-2.1.8/dockertidy/utils.py`

 * *Files identical despite different names*

### Comparing `docker_tidy-2.1.7/pyproject.toml` & `docker_tidy-2.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 include = ["LICENSE"]
 keywords = ["docker", "gc", "prune", "garbage"]
 license = "Apache-2.0"
 name = "docker-tidy"
 packages = [{ include = "dockertidy" }]
 readme = "README.md"
 repository = "https://github.com/thegeeklab/docker-tidy/"
-version = "2.1.7"
+version = "2.1.8"
 
 [tool.poetry.dependencies]
 anyconfig = "0.14.0"
 appdirs = "1.4.4"
 certifi = "2024.2.2"
 colorama = "0.4.6"
 dateparser = "1.2.0"
@@ -46,22 +46,22 @@
 nested-lookup = "0.2.25"
 pathspec = "0.12.1"
 python = "^3.8.0"
 python-dateutil = "2.9.0.post0"
 python-json-logger = "2.0.7"
 requests = "2.31.0"
 "ruamel.yaml" = "0.18.6"
-websocket_client = "1.7.0"
+websocket_client = "1.8.0"
 zipp = "3.18.1"
 
 [tool.poetry.scripts]
 docker-tidy = "dockertidy.cli:main"
 
 [tool.poetry.group.dev.dependencies]
-ruff = "0.3.5"
+ruff = "0.4.1"
 pytest = "8.1.1"
 pytest-mock = "3.14.0"
 pytest-cov = "5.0.0"
 toml = "0.10.2"
 
 [tool.poetry-dynamic-versioning]
 enable = false
```

### Comparing `docker_tidy-2.1.7/PKG-INFO` & `docker_tidy-2.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docker-tidy
-Version: 2.1.7
+Version: 2.1.8
 Summary: Keep docker hosts tidy.
 Home-page: https://docker-tidy.geekdocs.de/
 License: Apache-2.0
 Keywords: docker,gc,prune,garbage
 Author: Robert Kaussow
 Author-email: mail@thegeeklab.de
 Requires-Python: >=3.8.0,<4.0.0
@@ -38,15 +38,15 @@
 Requires-Dist: jsonschema (==4.21.1)
 Requires-Dist: nested-lookup (==0.2.25)
 Requires-Dist: pathspec (==0.12.1)
 Requires-Dist: python-dateutil (==2.9.0.post0)
 Requires-Dist: python-json-logger (==2.0.7)
 Requires-Dist: requests (==2.31.0)
 Requires-Dist: ruamel.yaml (==0.18.6)
-Requires-Dist: websocket_client (==1.7.0)
+Requires-Dist: websocket_client (==1.8.0)
 Requires-Dist: zipp (==3.18.1)
 Project-URL: Documentation, https://docker-tidy.geekdocs.de/
 Project-URL: Repository, https://github.com/thegeeklab/docker-tidy/
 Description-Content-Type: text/markdown
 
 # docker-tidy
```


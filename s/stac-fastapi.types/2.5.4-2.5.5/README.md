# Comparing `tmp/stac_fastapi_types-2.5.4.tar.gz` & `tmp/stac_fastapi_types-2.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stac_fastapi_types-2.5.4.tar", last modified: Wed Apr 24 16:03:51 2024, max compression
+gzip compressed data, was "stac_fastapi_types-2.5.5.tar", last modified: Thu Apr 25 06:06:26 2024, max compression
```

## Comparing `stac_fastapi_types-2.5.4.tar` & `stac_fastapi_types-2.5.5.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:03:51.424560 stac_fastapi_types-2.5.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-04-24 16:03:51.424560 stac_fastapi_types-2.5.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 16:03:38.000000 stac_fastapi_types-2.5.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-24 16:03:51.424560 stac_fastapi_types-2.5.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-04-24 16:03:38.000000 stac_fastapi_types-2.5.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:03:51.420560 stac_fastapi_types-2.5.4/stac_fastapi/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:03:51.424560 stac_fastapi_types-2.5.4/stac_fastapi/types/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-24 16:03:38.000000 stac_fastapi_types-2.5.4/stac_fastapi/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-04-24 16:03:38.000000 stac_fastapi_types-2.5.4/stac_fastapi/types/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-04-24 16:03:38.000000 stac_fastapi_types-2.5.4/stac_fastapi/types/conformance.py
--rw-r--r--   0 runner    (1001) docker     (127)    25419 2024-04-24 16:03:38.000000 stac_fastapi_types-2.5.4/stac_fastapi/types/core.py
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-24 16:03:38.000000 stac_fastapi_types-2.5.4/stac_fastapi/types/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-04-24 16:03:38.000000 stac_fastapi_types-2.5.4/stac_fastapi/types/extension.py
--rw-r--r--   0 runner    (1001) docker     (127)     3369 2024-04-24 16:03:38.000000 stac_fastapi_types-2.5.4/stac_fastapi/types/links.py
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-24 16:03:38.000000 stac_fastapi_types-2.5.4/stac_fastapi/types/requests.py
--rw-r--r--   0 runner    (1001) docker     (127)     3728 2024-04-24 16:03:38.000000 stac_fastapi_types-2.5.4/stac_fastapi/types/rfc3339.py
--rw-r--r--   0 runner    (1001) docker     (127)     6640 2024-04-24 16:03:38.000000 stac_fastapi_types-2.5.4/stac_fastapi/types/search.py
--rw-r--r--   0 runner    (1001) docker     (127)     2085 2024-04-24 16:03:38.000000 stac_fastapi_types-2.5.4/stac_fastapi/types/stac.py
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-24 16:03:38.000000 stac_fastapi_types-2.5.4/stac_fastapi/types/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:03:51.424560 stac_fastapi_types-2.5.4/stac_fastapi.types.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-04-24 16:03:51.000000 stac_fastapi_types-2.5.4/stac_fastapi.types.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      677 2024-04-24 16:03:51.000000 stac_fastapi_types-2.5.4/stac_fastapi.types.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 16:03:51.000000 stac_fastapi_types-2.5.4/stac_fastapi.types.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 16:03:51.000000 stac_fastapi_types-2.5.4/stac_fastapi.types.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-24 16:03:51.000000 stac_fastapi_types-2.5.4/stac_fastapi.types.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-24 16:03:51.000000 stac_fastapi_types-2.5.4/stac_fastapi.types.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:03:51.424560 stac_fastapi_types-2.5.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-24 16:03:38.000000 stac_fastapi_types-2.5.4/tests/test_limit.py
--rw-r--r--   0 runner    (1001) docker     (127)     3665 2024-04-24 16:03:38.000000 stac_fastapi_types-2.5.4/tests/test_rfc3339.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:06:26.383743 stac_fastapi_types-2.5.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-04-25 06:06:26.383743 stac_fastapi_types-2.5.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 06:06:15.000000 stac_fastapi_types-2.5.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-25 06:06:26.383743 stac_fastapi_types-2.5.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-04-25 06:06:15.000000 stac_fastapi_types-2.5.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:06:26.375743 stac_fastapi_types-2.5.5/stac_fastapi/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:06:26.379743 stac_fastapi_types-2.5.5/stac_fastapi/types/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-25 06:06:15.000000 stac_fastapi_types-2.5.5/stac_fastapi/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-04-25 06:06:15.000000 stac_fastapi_types-2.5.5/stac_fastapi/types/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-04-25 06:06:15.000000 stac_fastapi_types-2.5.5/stac_fastapi/types/conformance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25282 2024-04-25 06:06:15.000000 stac_fastapi_types-2.5.5/stac_fastapi/types/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-25 06:06:15.000000 stac_fastapi_types-2.5.5/stac_fastapi/types/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-04-25 06:06:15.000000 stac_fastapi_types-2.5.5/stac_fastapi/types/extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3369 2024-04-25 06:06:15.000000 stac_fastapi_types-2.5.5/stac_fastapi/types/links.py
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-25 06:06:15.000000 stac_fastapi_types-2.5.5/stac_fastapi/types/requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3728 2024-04-25 06:06:15.000000 stac_fastapi_types-2.5.5/stac_fastapi/types/rfc3339.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6640 2024-04-25 06:06:15.000000 stac_fastapi_types-2.5.5/stac_fastapi/types/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2085 2024-04-25 06:06:15.000000 stac_fastapi_types-2.5.5/stac_fastapi/types/stac.py
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-25 06:06:15.000000 stac_fastapi_types-2.5.5/stac_fastapi/types/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:06:26.379743 stac_fastapi_types-2.5.5/stac_fastapi.types.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-04-25 06:06:26.000000 stac_fastapi_types-2.5.5/stac_fastapi.types.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-04-25 06:06:26.000000 stac_fastapi_types-2.5.5/stac_fastapi.types.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 06:06:26.000000 stac_fastapi_types-2.5.5/stac_fastapi.types.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 06:06:26.000000 stac_fastapi_types-2.5.5/stac_fastapi.types.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-25 06:06:26.000000 stac_fastapi_types-2.5.5/stac_fastapi.types.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-25 06:06:26.000000 stac_fastapi_types-2.5.5/stac_fastapi.types.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:06:26.379743 stac_fastapi_types-2.5.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-25 06:06:15.000000 stac_fastapi_types-2.5.5/tests/test_limit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3665 2024-04-25 06:06:15.000000 stac_fastapi_types-2.5.5/tests/test_rfc3339.py
```

### Comparing `stac_fastapi_types-2.5.4/PKG-INFO` & `stac_fastapi_types-2.5.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stac-fastapi.types
-Version: 2.5.4
+Version: 2.5.5
 Summary: An implementation of STAC API based on the FastAPI framework.
 Home-page: https://github.com/stac-utils/stac-fastapi
 Author: Arturo Engineering
 Author-email: engineering@arturo.ai
 License: MIT
 Keywords: STAC FastAPI COG
 Classifier: Intended Audience :: Developers
```

### Comparing `stac_fastapi_types-2.5.4/setup.py` & `stac_fastapi_types-2.5.5/setup.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_types-2.5.4/stac_fastapi/types/config.py` & `stac_fastapi_types-2.5.5/stac_fastapi/types/config.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_types-2.5.4/stac_fastapi/types/conformance.py` & `stac_fastapi_types-2.5.5/stac_fastapi/types/conformance.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_types-2.5.4/stac_fastapi/types/core.py` & `stac_fastapi_types-2.5.5/stac_fastapi/types/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -400,29 +400,25 @@
 
         # Add OpenAPI URL
         landing_page["links"].append(
             {
                 "rel": "service-desc",
                 "type": "application/vnd.oai.openapi+json;version=3.0",
                 "title": "OpenAPI service description",
-                "href": urljoin(
-                    str(request.base_url), request.app.openapi_url.lstrip("/")
-                ),
+                "href": str(request.url_for("openapi")),
             }
         )
 
         # Add human readable service-doc
         landing_page["links"].append(
             {
                 "rel": "service-doc",
                 "type": "text/html",
                 "title": "OpenAPI service documentation",
-                "href": urljoin(
-                    str(request.base_url), request.app.docs_url.lstrip("/")
-                ),
+                "href": str(request.url_for("swagger_ui_html")),
             }
         )
 
         return landing_page
 
     def conformance(self, **kwargs) -> stac_types.Conformance:
         """Conformance classes.
```

### Comparing `stac_fastapi_types-2.5.4/stac_fastapi/types/errors.py` & `stac_fastapi_types-2.5.5/stac_fastapi/types/errors.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_types-2.5.4/stac_fastapi/types/extension.py` & `stac_fastapi_types-2.5.5/stac_fastapi/types/extension.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_types-2.5.4/stac_fastapi/types/links.py` & `stac_fastapi_types-2.5.5/stac_fastapi/types/links.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_types-2.5.4/stac_fastapi/types/rfc3339.py` & `stac_fastapi_types-2.5.5/stac_fastapi/types/rfc3339.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_types-2.5.4/stac_fastapi/types/search.py` & `stac_fastapi_types-2.5.5/stac_fastapi/types/search.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_types-2.5.4/stac_fastapi/types/stac.py` & `stac_fastapi_types-2.5.5/stac_fastapi/types/stac.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_types-2.5.4/stac_fastapi.types.egg-info/PKG-INFO` & `stac_fastapi_types-2.5.5/stac_fastapi.types.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stac-fastapi.types
-Version: 2.5.4
+Version: 2.5.5
 Summary: An implementation of STAC API based on the FastAPI framework.
 Home-page: https://github.com/stac-utils/stac-fastapi
 Author: Arturo Engineering
 Author-email: engineering@arturo.ai
 License: MIT
 Keywords: STAC FastAPI COG
 Classifier: Intended Audience :: Developers
```

### Comparing `stac_fastapi_types-2.5.4/stac_fastapi.types.egg-info/SOURCES.txt` & `stac_fastapi_types-2.5.5/stac_fastapi.types.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `stac_fastapi_types-2.5.4/tests/test_limit.py` & `stac_fastapi_types-2.5.5/tests/test_limit.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_types-2.5.4/tests/test_rfc3339.py` & `stac_fastapi_types-2.5.5/tests/test_rfc3339.py`

 * *Files identical despite different names*


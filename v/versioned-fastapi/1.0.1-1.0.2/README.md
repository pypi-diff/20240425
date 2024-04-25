# Comparing `tmp/versioned_fastapi-1.0.1.tar.gz` & `tmp/versioned_fastapi-1.0.2.tar.gz`

## Comparing `versioned_fastapi-1.0.1.tar` & `versioned_fastapi-1.0.2.tar`

### file list

```diff
@@ -1,19 +1,22 @@
--rw-r--r--   0        0        0    27221 2020-02-02 00:00:00.000000 versioned_fastapi-1.0.1/docs/swagger_ui_example_1.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 versioned_fastapi-1.0.1/examples/__init__.py
--rw-r--r--   0        0        0     4067 2020-02-02 00:00:00.000000 versioned_fastapi-1.0.1/examples/customization.py
--rw-r--r--   0        0        0     2319 2020-02-02 00:00:00.000000 versioned_fastapi-1.0.1/examples/simple.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 versioned_fastapi-1.0.1/tests/__init__.py
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 versioned_fastapi-1.0.1/tests/conftest.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 versioned_fastapi-1.0.1/tests/test_customization_example/__init__.py
--rw-r--r--   0        0        0    11862 2020-02-02 00:00:00.000000 versioned_fastapi-1.0.1/tests/test_customization_example/openapi_definitions.json
--rw-r--r--   0        0        0     2335 2020-02-02 00:00:00.000000 versioned_fastapi-1.0.1/tests/test_customization_example/test_customization.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 versioned_fastapi-1.0.1/tests/test_simple_example/__init__.py
--rw-r--r--   0        0        0    31702 2020-02-02 00:00:00.000000 versioned_fastapi-1.0.1/tests/test_simple_example/openapi_definitions.json
--rw-r--r--   0        0        0     2639 2020-02-02 00:00:00.000000 versioned_fastapi-1.0.1/tests/test_simple_example/test_simple.py
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 versioned_fastapi-1.0.1/versioned_fastapi/__init__.py
--rw-r--r--   0        0        0    10943 2020-02-02 00:00:00.000000 versioned_fastapi-1.0.1/versioned_fastapi/version_fastapi.py
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 versioned_fastapi-1.0.1/.gitignore
--rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 versioned_fastapi-1.0.1/LICENSE
--rw-r--r--   0        0        0     5227 2020-02-02 00:00:00.000000 versioned_fastapi-1.0.1/README.md
--rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 versioned_fastapi-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     6035 2020-02-02 00:00:00.000000 versioned_fastapi-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0    27221 2020-02-02 00:00:00.000000 versioned_fastapi-1.0.2/docs/swagger_ui_example_1.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 versioned_fastapi-1.0.2/examples/__init__.py
+-rw-r--r--   0        0        0     4268 2020-02-02 00:00:00.000000 versioned_fastapi-1.0.2/examples/customization.py
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 versioned_fastapi-1.0.2/examples/mounts.py
+-rw-r--r--   0        0        0     2319 2020-02-02 00:00:00.000000 versioned_fastapi-1.0.2/examples/simple.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 versioned_fastapi-1.0.2/tests/__init__.py
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 versioned_fastapi-1.0.2/tests/conftest.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 versioned_fastapi-1.0.2/tests/test_customization_example/__init__.py
+-rw-r--r--   0        0        0    11862 2020-02-02 00:00:00.000000 versioned_fastapi-1.0.2/tests/test_customization_example/openapi_definitions.json
+-rw-r--r--   0        0        0     2335 2020-02-02 00:00:00.000000 versioned_fastapi-1.0.2/tests/test_customization_example/test_customization.py
+-rw-r--r--   0        0        0     8548 2020-02-02 00:00:00.000000 versioned_fastapi-1.0.2/tests/test_mounts_example.py/openapi_definitions.json
+-rw-r--r--   0        0        0     2733 2020-02-02 00:00:00.000000 versioned_fastapi-1.0.2/tests/test_mounts_example.py/test_mounts.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 versioned_fastapi-1.0.2/tests/test_simple_example/__init__.py
+-rw-r--r--   0        0        0    31702 2020-02-02 00:00:00.000000 versioned_fastapi-1.0.2/tests/test_simple_example/openapi_definitions.json
+-rw-r--r--   0        0        0     2639 2020-02-02 00:00:00.000000 versioned_fastapi-1.0.2/tests/test_simple_example/test_simple.py
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 versioned_fastapi-1.0.2/versioned_fastapi/__init__.py
+-rw-r--r--   0        0        0    10781 2020-02-02 00:00:00.000000 versioned_fastapi-1.0.2/versioned_fastapi/version_fastapi.py
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 versioned_fastapi-1.0.2/.gitignore
+-rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 versioned_fastapi-1.0.2/LICENSE
+-rw-r--r--   0        0        0     5227 2020-02-02 00:00:00.000000 versioned_fastapi-1.0.2/README.md
+-rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 versioned_fastapi-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     6035 2020-02-02 00:00:00.000000 versioned_fastapi-1.0.2/PKG-INFO
```

### Comparing `versioned_fastapi-1.0.1/docs/swagger_ui_example_1.png` & `versioned_fastapi-1.0.2/docs/swagger_ui_example_1.png`

 * *Files identical despite different names*

### Comparing `versioned_fastapi-1.0.1/examples/customization.py` & `versioned_fastapi-1.0.2/examples/customization.py`

 * *Files 9% similar despite different names*

```diff
@@ -109,14 +109,18 @@
 versioner.title_format = "{title} - Version {version}"
 versioner.description_format = "{description}"
 versioner.summary_format = "{summary} - Version {version}"
 versioner.swagger_favicon_url = "https://www.google.com/favicon.ico"
 versioner.swagger_css_urls = (
     "https://cdn.jsdelivr.net/npm/swagger-ui-dist@5.9.0/swagger-ui.css",
 )
+versioner.swagger_js_urls = (
+    "https://cdn.jsdelivr.net/npm/swagger-ui-dist@5.9.0/swagger-ui-bundle.js",
+    "https://cdn.jsdelivr.net/npm/swagger-ui-dist@5.9.0/swagger-ui-standalone-preset.js",
+)
 
 versions = versioner.version_fastapi()
 
 if __name__ == "__main__":
     uvicorn.run(
         f"{Path(__file__).stem}:app",
         reload=True,
```

### Comparing `versioned_fastapi-1.0.1/examples/simple.py` & `versioned_fastapi-1.0.2/examples/simple.py`

 * *Files identical despite different names*

### Comparing `versioned_fastapi-1.0.1/tests/conftest.py` & `versioned_fastapi-1.0.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `versioned_fastapi-1.0.1/tests/test_customization_example/openapi_definitions.json` & `versioned_fastapi-1.0.2/tests/test_customization_example/openapi_definitions.json`

 * *Files identical despite different names*

### Comparing `versioned_fastapi-1.0.1/tests/test_customization_example/test_customization.py` & `versioned_fastapi-1.0.2/tests/test_customization_example/test_customization.py`

 * *Files identical despite different names*

### Comparing `versioned_fastapi-1.0.1/tests/test_simple_example/openapi_definitions.json` & `versioned_fastapi-1.0.2/tests/test_simple_example/openapi_definitions.json`

 * *Files identical despite different names*

### Comparing `versioned_fastapi-1.0.1/tests/test_simple_example/test_simple.py` & `versioned_fastapi-1.0.2/tests/test_simple_example/test_simple.py`

 * *Files identical despite different names*

### Comparing `versioned_fastapi-1.0.1/versioned_fastapi/version_fastapi.py` & `versioned_fastapi-1.0.2/versioned_fastapi/version_fastapi.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     summary_format: str = "{summary}"
     """Defines the format of the swagger summary, can contain "{summary}" and "{version}". Available since OpenAPI 3.1.0, FastAPI 0.99.0."""
     swagger_js_urls: Iterable[str] = (
         "https://cdn.jsdelivr.net/npm/swagger-ui-dist@5/swagger-ui-bundle.js",
         "https://cdn.jsdelivr.net/npm/swagger-ui-dist@5/swagger-ui-standalone-preset.js",
     )
     """The URLs to use to load the Swagger UI JavaScript."""
-    swagger_css_urls: Union[Iterable[str], None] = [
+    swagger_css_urls: Iterable[str] = [
         "https://cdn.jsdelivr.net/npm/swagger-ui-dist@5/swagger-ui.css"
     ]
     """The URLs to use to load Swagger UI CSS. Leave None to use FastAPIs default."""
     swagger_favicon_url: Union[str, None] = None
     """The URL of the favicon to use. Leave None to use FastAPIs default."""
 
     def __init__(
@@ -178,73 +178,70 @@
             router.prefix + self.app.openapi_url,  # type: ignore
             get_versioned_openapi,
             include_in_schema=False,
         )
 
     def _override_swagger_docs(self, versions: List[str]):
         """Overwrites the swagger docs to enable a dropdown menu for version selection."""
-        # Swagger api definition urls, see https://swagger.io/docs/open-source-tools/swagger-ui/usage/configuration/
-        openapi_urls = []
-        if self.include_main_openapi:
-            openapi_urls.append({"name": "All Routes", "url": self.app.openapi_url})
-        openapi_urls.extend(
-            [
-                {
-                    "name": f"Version {v}",
-                    "url": f"{self.prefix_format.format(version=v)}{self.app.openapi_url}",
-                }
-                for v in versions
-            ]
-        )
-        swagger_html_kwargs = {
-            "swagger_js_url": '"></script><script src="'.join(self.swagger_js_urls),
-            "swagger_ui_parameters": {
-                "layout": "StandaloneLayout",
-                "urls": openapi_urls,
-            },
-            "title": self.app.title + " - Swagger UI",
-        }
-        if self.primary_swagger_version:
-            swagger_html_kwargs["swagger_ui_parameters"][
-                "urls.primaryName"
-            ] = f"Version {self.primary_swagger_version}"
-        if self.swagger_css_urls:
-            swagger_html_kwargs[
-                "swagger_css_url"
-            ] = '"><link type="text/css" rel="stylesheet" href="'.join(
-                self.swagger_css_urls
-            )
-        if self.swagger_favicon_url:
-            swagger_html_kwargs["swagger_favicon_url"] = self.swagger_favicon_url
 
         async def get_versioned_swagger_ui_html(request: Request) -> HTMLResponse:
             root_path = request.scope.get("root_path", "").rstrip("/")
-            openapi_url = root_path + self.app.openapi_url  # type: ignore
+            openapi_url = f"{root_path}{self.app.openapi_url}"
             oauth2_redirect_url = (
                 self.app.swagger_ui_oauth2_redirect_url
                 and root_path + self.app.swagger_ui_oauth2_redirect_url
             )
-            if root_path:
-                for openapi_url in swagger_html_kwargs["swagger_ui_parameters"]["urls"]:
-                    openapi_url["url"] = root_path + openapi_url["url"]
-
-            swagger_html_kwargs.update(
-                {
-                    "openapi_url": openapi_url,  # Will be overridden by 'urls' anyway
-                    "oauth2_redirect_url": oauth2_redirect_url,
-                }
+
+            title = self.app.title + " - Swagger UI"
+            swagger_js_url = '"></script><script src="'.join(self.swagger_js_urls)
+            swagger_css_urls = '"><link type="text/css" rel="stylesheet" href="'.join(
+                self.swagger_css_urls
             )
-            if self.app.swagger_ui_parameters:
-                swagger_html_kwargs["swagger_ui_parameters"].update(
-                    self.app.swagger_ui_parameters
+
+            # Swagger api definition urls, see https://swagger.io/docs/open-source-tools/swagger-ui/usage/configuration/
+            versioned_openapi_urls = []
+            if self.include_main_openapi:
+                versioned_openapi_urls.append(
+                    {"name": "All Routes", "url": openapi_url}
                 )
+            versioned_openapi_urls.extend(
+                [
+                    {
+                        "name": f"Version {v}",
+                        "url": f"{root_path}{self.prefix_format.format(version=v)}{self.app.openapi_url}",
+                    }
+                    for v in versions
+                ]
+            )
+            swagger_ui_parameters = {
+                "layout": "StandaloneLayout",
+                "urls": versioned_openapi_urls,
+            }
+            if self.primary_swagger_version:
+                swagger_ui_parameters["urls.primaryName"] = (
+                    f"Version {self.primary_swagger_version}"
+                )
+            if self.app.swagger_ui_parameters:
+                swagger_ui_parameters.update(self.app.swagger_ui_parameters)
+
+            optional_kwargs = {}
+            if self.swagger_favicon_url:
+                optional_kwargs["swagger_favicon_url"] = self.swagger_favicon_url
 
             # It might be better to override get_swagger_ui_html completely instead of modifying its response...
-            html_body = get_swagger_ui_html(**swagger_html_kwargs).body
-            html_body = html_body.replace(
+            html_response = get_swagger_ui_html(
+                openapi_url=openapi_url,
+                title=title,
+                swagger_js_url=swagger_js_url,
+                swagger_css_url=swagger_css_urls,
+                oauth2_redirect_url=oauth2_redirect_url,
+                swagger_ui_parameters=swagger_ui_parameters,
+                **optional_kwargs,
+            )
+            html_body = html_response.body.replace(
                 b"SwaggerUIBundle.SwaggerUIStandalonePreset",
                 b"SwaggerUIStandalonePreset",
             )
             html_body = html_body.replace(
                 b"<body>", b"<body style='margin:0;padding:0'>"
             )
             return HTMLResponse(html_body)
```

### Comparing `versioned_fastapi-1.0.1/LICENSE` & `versioned_fastapi-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `versioned_fastapi-1.0.1/README.md` & `versioned_fastapi-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `versioned_fastapi-1.0.1/pyproject.toml` & `versioned_fastapi-1.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `versioned_fastapi-1.0.1/PKG-INFO` & `versioned_fastapi-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: versioned-fastapi
-Version: 1.0.1
+Version: 1.0.2
 Summary: Simple versioning of FastAPI web applications
 Project-URL: Documentation, https://github.com/mivoelcker/versioned-fastapi#readme
 Project-URL: Source, https://github.com/mivoelcker/versioned-fastapi
 License-Expression: MIT
 License-File: LICENSE
 Keywords: fastapi,version,versioned-fastapi,versioning
 Classifier: Programming Language :: Python
```


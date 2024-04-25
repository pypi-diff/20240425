# Comparing `tmp/firestoned-0.3.5.tar.gz` & `tmp/firestoned-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "firestoned-0.3.5.tar", max compression
+gzip compressed data, was "firestoned-0.3.6.tar", max compression
```

## Comparing `firestoned-0.3.5.tar` & `firestoned-0.3.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0    11357 2024-03-25 16:52:14.878006 firestoned-0.3.5/LICENSE
--rw-r--r--   0        0        0     9347 2024-03-25 16:52:14.878006 firestoned-0.3.5/README.md
--rw-r--r--   0        0        0        0 2024-03-25 16:52:14.882006 firestoned-0.3.5/firestone/__init__.py
--rw-r--r--   0        0        0     5085 2024-03-25 16:52:14.882006 firestoned-0.3.5/firestone/__main__.py
--rw-r--r--   0        0        0        0 2024-03-25 16:52:14.882006 firestoned-0.3.5/firestone/schema/__init__.py
--rw-r--r--   0        0        0      322 2024-03-25 16:52:14.882006 firestoned-0.3.5/firestone/schema/asyncapi.jinja2
--rw-r--r--   0        0        0     8205 2024-03-25 16:52:14.882006 firestoned-0.3.5/firestone/schema/main.py.jinja2
--rw-r--r--   0        0        0      437 2024-03-25 16:52:14.882006 firestoned-0.3.5/firestone/schema/openapi.jinja2
--rw-r--r--   0        0        0     2263 2024-03-25 16:52:14.882006 firestoned-0.3.5/firestone/schema/resource.yaml
--rw-r--r--   0        0        0      176 2024-03-25 16:52:14.882006 firestoned-0.3.5/firestone/spec/__init__.py
--rw-r--r--   0        0        0      867 2024-03-25 16:52:14.882006 firestoned-0.3.5/firestone/spec/_base.py
--rw-r--r--   0        0        0    13391 2024-03-25 16:52:14.882006 firestoned-0.3.5/firestone/spec/asyncapi.py
--rw-r--r--   0        0        0     9827 2024-03-25 16:52:14.882006 firestoned-0.3.5/firestone/spec/cli.py
--rw-r--r--   0        0        0    19242 2024-03-25 16:52:14.882006 firestoned-0.3.5/firestone/spec/openapi.py
--rw-r--r--   0        0        0     1689 2024-03-25 16:52:14.886006 firestoned-0.3.5/pyproject.toml
--rw-r--r--   0        0        0    10496 1970-01-01 00:00:00.000000 firestoned-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-25 03:53:52.045334 firestoned-0.3.6/LICENSE
+-rw-r--r--   0        0        0     9347 2024-04-25 03:53:52.045334 firestoned-0.3.6/README.md
+-rw-r--r--   0        0        0        0 2024-04-25 03:53:52.053334 firestoned-0.3.6/firestone/__init__.py
+-rw-r--r--   0        0        0     5085 2024-04-25 03:53:52.053334 firestoned-0.3.6/firestone/__main__.py
+-rw-r--r--   0        0        0        0 2024-04-25 03:53:52.053334 firestoned-0.3.6/firestone/schema/__init__.py
+-rw-r--r--   0        0        0      322 2024-04-25 03:53:52.053334 firestoned-0.3.6/firestone/schema/asyncapi.jinja2
+-rw-r--r--   0        0        0     8125 2024-04-25 03:53:52.053334 firestoned-0.3.6/firestone/schema/main.py.jinja2
+-rw-r--r--   0        0        0      437 2024-04-25 03:53:52.053334 firestoned-0.3.6/firestone/schema/openapi.jinja2
+-rw-r--r--   0        0        0     2263 2024-04-25 03:53:52.053334 firestoned-0.3.6/firestone/schema/resource.yaml
+-rw-r--r--   0        0        0      176 2024-04-25 03:53:52.053334 firestoned-0.3.6/firestone/spec/__init__.py
+-rw-r--r--   0        0        0      867 2024-04-25 03:53:52.053334 firestoned-0.3.6/firestone/spec/_base.py
+-rw-r--r--   0        0        0    13391 2024-04-25 03:53:52.053334 firestoned-0.3.6/firestone/spec/asyncapi.py
+-rw-r--r--   0        0        0     9827 2024-04-25 03:53:52.053334 firestoned-0.3.6/firestone/spec/cli.py
+-rw-r--r--   0        0        0    19242 2024-04-25 03:53:52.053334 firestoned-0.3.6/firestone/spec/openapi.py
+-rw-r--r--   0        0        0     1689 2024-04-25 03:53:52.053334 firestoned-0.3.6/pyproject.toml
+-rw-r--r--   0        0        0    10496 1970-01-01 00:00:00.000000 firestoned-0.3.6/PKG-INFO
```

### Comparing `firestoned-0.3.5/LICENSE` & `firestoned-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `firestoned-0.3.5/README.md` & `firestoned-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `firestoned-0.3.5/firestone/__main__.py` & `firestoned-0.3.6/firestone/__main__.py`

 * *Files identical despite different names*

### Comparing `firestoned-0.3.5/firestone/schema/main.py.jinja2` & `firestoned-0.3.6/firestone/schema/main.py.jinja2`

 * *Files 9% similar despite different names*

```diff
@@ -25,24 +25,26 @@
 
 _LOGGER = logging.getLogger(__name__)
 
 
 def api_exc(func):
     """Handle ApiExceptions in all functions."""
     async def wrapper(*args, **kwargs):
-        api_obj = args[0]["api_obj"]
         resp = None
         try:
             return await func(*args, **kwargs)
         except exceptions.ApiException as apie:
             if apie.body:
                 click.echo(apie.body)
             else:
                 click.echo(apie.reason)
-            await api_obj.api_client.close()
+
+            api_obj = args[0].get("api_obj")
+            if api_obj:
+                await api_obj.api_client.close()
         sys.exit(-1)
 
     return functools.update_wrapper(wrapper, func)
 
 
 @click.group()
 @click.option("--debug", help="Turn on debugging", is_flag=True)
@@ -70,31 +72,20 @@
 @click.pass_context
 def main(ctx, debug, api_key, api_url, client_cert, client_key, trust_proxy):
     """{{ title }}
 
     {{ description }}
     """
     if not trust_proxy:
-        # Convert to loop
-        if "http_proxy" in os.environ:
-            del os.environ["http_proxy"]
-        if "https_proxy" in os.environ:
-            del os.environ["https_proxy"]
-        if "all_http_proxy" in os.environ:
-            del os.environ["all_http_proxy"]
-        if "all_https_proxy" in os.environ:
-            del os.environ["https_proxy"]
-        if "HTTP_PROXY" in os.environ:
-            del os.environ["HTTP_PROXY"]
-        if "HTTPS_PROXY" in os.environ:
-            del os.environ["HTTPS_PROXY"]
-        if "ALL_HTTP_PROXY" in os.environ:
-            del os.environ["ALL_HTTP_PROXY"]
-        if "ALL_HTTPS_PROXY" in os.environ:
-            del os.environ["ALL_HTTPS_PROXY"]
+        for prefix in ["http", "https", "all_http", "all_https"]:
+            env_var = f"{prefix}_proxy"
+            if env_var in os.environ:
+                del os.environ[env_var]
+            if env_var.upper() in os.environ:
+                del os.environ[env_var.upper()]
 
     try:
         cli.init_logging("{{ pkg }}.resources.logging", "cli.conf")
     # pylint: disable=broad-except
     except Exception:
         logging.basicConfig(
             level=logging.INFO,
@@ -157,17 +148,27 @@
     """{{ op["description"] }}"""
     api_obj = ctx_obj["api_obj"]
     params = {
         {% for attr in op["attrs"]|sort(attribute='name') -%}
         "{{ attr["name"] }}":  {{ attr["name"].replace("-", "_") }},
         {% endfor %}
     }
-    {% set comp_name = rsrc["name"] if not rsrc["name"].endswith("s") else rsrc["name"][:-1] %}
-    {% if op["name"] == "create" %}
-    req_body = create_{{ comp_name }}_model.Create{{ comp_name.capitalize() }}(**params)
+    {% set comp_name = rsrc["name"] if not rsrc["name"].endswith("s") else rsrc["name"][:-1] -%}
+    {% if op["name"] == "create" -%}
+
+    {% set clazz_name = comp_name.capitalize() -%}
+    {% if "_" in clazz_name -%}
+    {% set new_clazz_name = [] -%}
+    {% for part in  clazz_name.split("_") -%}
+        {% set _ = new_clazz_name.append(part.capitalize()) -%}
+    {% endfor -%}
+    {% set clazz_name = "".join(new_clazz_name) -%}
+    {% endif -%}
+
+    req_body = create_{{ comp_name }}_model.Create{{ clazz_name }}(**params)
     resp = await api_obj.{{ op["id"] }}(req_body)
     {% else %}
     resp = await api_obj.{{ op["id"] }}(**params)
     {% endif -%}
     _LOGGER.debug(f"resp: {resp}")
 
     if isinstance(resp, list):
```

### Comparing `firestoned-0.3.5/firestone/schema/resource.yaml` & `firestoned-0.3.6/firestone/schema/resource.yaml`

 * *Files identical despite different names*

### Comparing `firestoned-0.3.5/firestone/spec/_base.py` & `firestoned-0.3.6/firestone/spec/_base.py`

 * *Files identical despite different names*

### Comparing `firestoned-0.3.5/firestone/spec/asyncapi.py` & `firestoned-0.3.6/firestone/spec/asyncapi.py`

 * *Files identical despite different names*

### Comparing `firestoned-0.3.5/firestone/spec/cli.py` & `firestoned-0.3.6/firestone/spec/cli.py`

 * *Files identical despite different names*

### Comparing `firestoned-0.3.5/firestone/spec/openapi.py` & `firestoned-0.3.6/firestone/spec/openapi.py`

 * *Files identical despite different names*

### Comparing `firestoned-0.3.5/pyproject.toml` & `firestoned-0.3.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "firestoned"
-version = "0.3.5"
+version = "0.3.6"
 description = "Build OpenAPI and AsyncAPI specs based off one or more resource json schema files"
 authors = ["Erick Bourgeois <erick@jeb.ca>"]
 license = "Apache 2.0"
 readme = "README.md"
 repository = "https://github.com/firestoned/firestone"
 packages = [
     { include = "firestone" }
```

### Comparing `firestoned-0.3.5/PKG-INFO` & `firestoned-0.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: firestoned
-Version: 0.3.5
+Version: 0.3.6
 Summary: Build OpenAPI and AsyncAPI specs based off one or more resource json schema files
 Home-page: https://github.com/firestoned/firestone
 License: Apache 2.0
 Author: Erick Bourgeois
 Author-email: erick@jeb.ca
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: firestoned Version: 0.3.5 Summary: Build OpenAPI
+Metadata-Version: 2.1 Name: firestoned Version: 0.3.6 Summary: Build OpenAPI
 and AsyncAPI specs based off one or more resource json schema files Home-page:
 https://github.com/firestoned/firestone License: Apache 2.0 Author: Erick
 Bourgeois Author-email: erick@jeb.ca Requires-Python: >=3.9,<4.0 Classifier:
 License :: Other/Proprietary License Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12 Provides-Extra: caching
```


# Comparing `tmp/nestipy_metadata-0.1.0.tar.gz` & `tmp/nestipy_metadata-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nestipy_metadata-0.1.0.tar", max compression
+gzip compressed data, was "nestipy_metadata-0.1.1.tar", max compression
```

## Comparing `nestipy_metadata-0.1.0.tar` & `nestipy_metadata-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0        0 2024-04-22 12:21:33.698414 nestipy_metadata-0.1.0/README.md
--rw-r--r--   0        0        0      335 2024-04-22 12:31:44.711385 nestipy_metadata-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      458 2024-04-22 12:25:19.348610 nestipy_metadata-0.1.0/src/nestipy_metadata/__init__.py
--rw-r--r--   0        0        0     1514 2024-04-22 09:57:49.101103 nestipy_metadata-0.1.0/src/nestipy_metadata/class_.py
--rw-r--r--   0        0        0      478 2024-04-22 12:11:47.812303 nestipy_metadata-0.1.0/src/nestipy_metadata/container.py
--rw-r--r--   0        0        0      710 2024-03-29 11:21:44.572810 nestipy_metadata-0.1.0/src/nestipy_metadata/decorator.py
--rw-r--r--   0        0        0      662 2024-03-29 11:21:44.572810 nestipy_metadata-0.1.0/src/nestipy_metadata/dependency.py
--rw-r--r--   0        0        0      236 2024-04-17 10:37:35.138306 nestipy_metadata-0.1.0/src/nestipy_metadata/module.py
--rw-r--r--   0        0        0       88 2024-03-29 11:21:44.572810 nestipy_metadata-0.1.0/src/nestipy_metadata/provider_token.py
--rw-r--r--   0        0        0      688 2024-03-29 11:21:44.572810 nestipy_metadata-0.1.0/src/nestipy_metadata/reflect.py
--rw-r--r--   0        0        0      107 2024-03-29 11:21:44.572810 nestipy_metadata-0.1.0/src/nestipy_metadata/route.py
--rw-r--r--   0        0        0      398 1970-01-01 00:00:00.000000 nestipy_metadata-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-22 12:21:33.698414 nestipy_metadata-0.1.1/README.md
+-rw-r--r--   0        0        0      335 2024-04-25 12:32:30.569118 nestipy_metadata-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      458 2024-04-22 12:25:19.348610 nestipy_metadata-0.1.1/src/nestipy_metadata/__init__.py
+-rw-r--r--   0        0        0     1673 2024-04-25 13:24:55.667717 nestipy_metadata-0.1.1/src/nestipy_metadata/class_.py
+-rw-r--r--   0        0        0      478 2024-04-22 12:11:47.812303 nestipy_metadata-0.1.1/src/nestipy_metadata/container.py
+-rw-r--r--   0        0        0      710 2024-03-29 11:21:44.572810 nestipy_metadata-0.1.1/src/nestipy_metadata/decorator.py
+-rw-r--r--   0        0        0      662 2024-03-29 11:21:44.572810 nestipy_metadata-0.1.1/src/nestipy_metadata/dependency.py
+-rw-r--r--   0        0        0      236 2024-04-17 10:37:35.138306 nestipy_metadata-0.1.1/src/nestipy_metadata/module.py
+-rw-r--r--   0        0        0       88 2024-03-29 11:21:44.572810 nestipy_metadata-0.1.1/src/nestipy_metadata/provider_token.py
+-rw-r--r--   0        0        0      688 2024-03-29 11:21:44.572810 nestipy_metadata-0.1.1/src/nestipy_metadata/reflect.py
+-rw-r--r--   0        0        0      107 2024-03-29 11:21:44.572810 nestipy_metadata-0.1.1/src/nestipy_metadata/route.py
+-rw-r--r--   0        0        0      398 1970-01-01 00:00:00.000000 nestipy_metadata-0.1.1/PKG-INFO
```

### Comparing `nestipy_metadata-0.1.0/src/nestipy_metadata/class_.py` & `nestipy_metadata-0.1.1/src/nestipy_metadata/class_.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,24 +13,28 @@
         self._module = module
         self._global_providers = global_providers or []
 
     def get_module(self):
         return self._module
 
     def get_service_providers(self):
-        providers = self._global_providers + Reflect.get_metadata(self._module, ModuleMetadata.Providers, [])
+        providers = Reflect.get_metadata(self._module, ModuleMetadata.Providers, [])
         import_providers_form_exports = []
         # Only not a root module need to get import_providers to share
-        if not Reflect.get_metadata(self._module, ModuleMetadata.Root, False):
-            for im in Reflect.get_metadata(self._module, ModuleMetadata.Imports, []):
-                for export in Reflect.get_metadata(im, ModuleMetadata.Exports, []):
-                    # For module re-exporting
-                    is_module: bool = Reflect.get_metadata(export, ModuleMetadata.Module, False)
-                    if is_module:
-                        import_providers_form_exports = import_providers_form_exports + Reflect.get_metadata(
-                            export,
-                            ModuleMetadata.Providers,
-                            []
-                        )
-                    else:
-                        import_providers_form_exports.append(export)
+        # if not Reflect.get_metadata(self._module, ModuleMetadata.Root, False):
+        for im in Reflect.get_metadata(self._module, ModuleMetadata.Imports, []):
+            exports = Reflect.get_metadata(im.module if hasattr(im, 'module') else im, ModuleMetadata.Exports, [])
+            # check if dynamic module
+            # if hasattr(im, 'module') and hasattr(im, 'exports'):
+            #     exports = getattr(im, 'exports', [])
+            for export in exports:
+                # For module re-exporting
+                is_module: bool = Reflect.get_metadata(export, ModuleMetadata.Module, False)
+                if is_module:
+                    import_providers_form_exports = import_providers_form_exports + Reflect.get_metadata(
+                        export,
+                        ModuleMetadata.Providers,
+                        []
+                    )
+                else:
+                    import_providers_form_exports.append(export)
         return providers, import_providers_form_exports
```

### Comparing `nestipy_metadata-0.1.0/src/nestipy_metadata/decorator.py` & `nestipy_metadata-0.1.1/src/nestipy_metadata/decorator.py`

 * *Files identical despite different names*

### Comparing `nestipy_metadata-0.1.0/src/nestipy_metadata/dependency.py` & `nestipy_metadata-0.1.1/src/nestipy_metadata/dependency.py`

 * *Files identical despite different names*

### Comparing `nestipy_metadata-0.1.0/src/nestipy_metadata/reflect.py` & `nestipy_metadata-0.1.1/src/nestipy_metadata/reflect.py`

 * *Files identical despite different names*


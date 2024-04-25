# Comparing `tmp/eodc-2024.4.3.tar.gz` & `tmp/eodc-2024.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eodc-2024.4.3.tar", max compression
+gzip compressed data, was "eodc-2024.4.4.tar", max compression
```

## Comparing `eodc-2024.4.3.tar` & `eodc-2024.4.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      676 2024-04-22 13:37:21.078859 eodc-2024.4.3/README.md
--rw-r--r--   0        0        0      195 2024-04-22 13:37:21.078859 eodc-2024.4.3/eodc/__init__.py
--rw-r--r--   0        0        0     1794 2024-04-22 13:37:21.078859 eodc-2024.4.3/eodc/auth.py
--rw-r--r--   0        0        0     1311 2024-04-22 13:37:21.078859 eodc-2024.4.3/eodc/dask.py
--rw-r--r--   0        0        0    13711 2024-04-22 13:37:21.078859 eodc-2024.4.3/eodc/faas.py
--rw-r--r--   0        0        0     1183 2024-04-22 13:37:21.078859 eodc-2024.4.3/eodc/settings.py
--rw-r--r--   0        0        0     2240 2024-04-22 13:37:21.078859 eodc-2024.4.3/eodc/storage.py
--rw-r--r--   0        0        0        0 2024-04-22 13:37:21.078859 eodc-2024.4.3/eodc/visualisation/__init__.py
--rw-r--r--   0        0        0        0 2024-04-22 13:37:21.078859 eodc-2024.4.3/eodc/visualisation/vessel_detection/__init__.py
--rwxr-xr-x   0        0        0    15080 2024-04-22 13:37:21.078859 eodc-2024.4.3/eodc/visualisation/vessel_detection/app.py
--rw-r--r--   0        0        0      261 2024-04-22 13:37:21.078859 eodc-2024.4.3/eodc/visualisation/vessel_detection/assets/app.css
--rw-r--r--   0        0        0     2539 2024-04-22 13:37:21.078859 eodc-2024.4.3/eodc/visualisation/vessel_detection/cards.py
--rw-r--r--   0        0        0     8522 2024-04-22 13:37:21.078859 eodc-2024.4.3/eodc/visualisation/vessel_detection/navbar.py
--rw-r--r--   0        0        0     2867 2024-04-22 13:37:21.078859 eodc-2024.4.3/eodc/visualisation/vessel_detection/utils.py
--rw-r--r--   0        0        0    32022 2024-04-22 13:37:21.078859 eodc-2024.4.3/eodc/workspace.py
--rw-r--r--   0        0        0     1890 2024-04-22 13:37:21.082859 eodc-2024.4.3/pyproject.toml
--rw-r--r--   0        0        0     2802 1970-01-01 00:00:00.000000 eodc-2024.4.3/PKG-INFO
+-rw-r--r--   0        0        0      676 2024-04-25 09:22:21.505405 eodc-2024.4.4/README.md
+-rw-r--r--   0        0        0      195 2024-04-25 09:22:21.505405 eodc-2024.4.4/eodc/__init__.py
+-rw-r--r--   0        0        0     1794 2024-04-25 09:22:21.505405 eodc-2024.4.4/eodc/auth.py
+-rw-r--r--   0        0        0     1311 2024-04-25 09:22:21.505405 eodc-2024.4.4/eodc/dask.py
+-rw-r--r--   0        0        0    13711 2024-04-25 09:22:21.505405 eodc-2024.4.4/eodc/faas.py
+-rw-r--r--   0        0        0     1183 2024-04-25 09:22:21.505405 eodc-2024.4.4/eodc/settings.py
+-rw-r--r--   0        0        0     2240 2024-04-25 09:22:21.505405 eodc-2024.4.4/eodc/storage.py
+-rw-r--r--   0        0        0        0 2024-04-25 09:22:21.505405 eodc-2024.4.4/eodc/visualisation/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 09:22:21.505405 eodc-2024.4.4/eodc/visualisation/vessel_detection/__init__.py
+-rwxr-xr-x   0        0        0    15080 2024-04-25 09:22:21.505405 eodc-2024.4.4/eodc/visualisation/vessel_detection/app.py
+-rw-r--r--   0        0        0      261 2024-04-25 09:22:21.505405 eodc-2024.4.4/eodc/visualisation/vessel_detection/assets/app.css
+-rw-r--r--   0        0        0     2539 2024-04-25 09:22:21.505405 eodc-2024.4.4/eodc/visualisation/vessel_detection/cards.py
+-rw-r--r--   0        0        0     8522 2024-04-25 09:22:21.505405 eodc-2024.4.4/eodc/visualisation/vessel_detection/navbar.py
+-rw-r--r--   0        0        0     2867 2024-04-25 09:22:21.505405 eodc-2024.4.4/eodc/visualisation/vessel_detection/utils.py
+-rw-r--r--   0        0        0    32028 2024-04-25 09:22:21.505405 eodc-2024.4.4/eodc/workspace.py
+-rw-r--r--   0        0        0     1890 2024-04-25 09:22:21.509405 eodc-2024.4.4/pyproject.toml
+-rw-r--r--   0        0        0     2802 1970-01-01 00:00:00.000000 eodc-2024.4.4/PKG-INFO
```

### Comparing `eodc-2024.4.3/README.md` & `eodc-2024.4.4/README.md`

 * *Files identical despite different names*

### Comparing `eodc-2024.4.3/eodc/auth.py` & `eodc-2024.4.4/eodc/auth.py`

 * *Files identical despite different names*

### Comparing `eodc-2024.4.3/eodc/dask.py` & `eodc-2024.4.4/eodc/dask.py`

 * *Files identical despite different names*

### Comparing `eodc-2024.4.3/eodc/faas.py` & `eodc-2024.4.4/eodc/faas.py`

 * *Files identical despite different names*

### Comparing `eodc-2024.4.3/eodc/settings.py` & `eodc-2024.4.4/eodc/settings.py`

 * *Files identical despite different names*

### Comparing `eodc-2024.4.3/eodc/storage.py` & `eodc-2024.4.4/eodc/storage.py`

 * *Files identical despite different names*

### Comparing `eodc-2024.4.3/eodc/visualisation/vessel_detection/app.py` & `eodc-2024.4.4/eodc/visualisation/vessel_detection/app.py`

 * *Files identical despite different names*

### Comparing `eodc-2024.4.3/eodc/visualisation/vessel_detection/cards.py` & `eodc-2024.4.4/eodc/visualisation/vessel_detection/cards.py`

 * *Files identical despite different names*

### Comparing `eodc-2024.4.3/eodc/visualisation/vessel_detection/navbar.py` & `eodc-2024.4.4/eodc/visualisation/vessel_detection/navbar.py`

 * *Files identical despite different names*

### Comparing `eodc-2024.4.3/eodc/visualisation/vessel_detection/utils.py` & `eodc-2024.4.4/eodc/visualisation/vessel_detection/utils.py`

 * *Files identical despite different names*

### Comparing `eodc-2024.4.3/eodc/workspace.py` & `eodc-2024.4.4/eodc/workspace.py`

 * *Files 0% similar despite different names*

```diff
@@ -556,15 +556,15 @@
         )
 
     def describe_workspace_policy(self, workspace_name: str):
         return self.s3_client.get_bucket_policy(Bucket=workspace_name)
 
     # Implement the abstract methods from DefaultStacIO
 
-    def parse_workspace_STAC_source(source: Union[str, Link]) -> tuple[str, str]:
+    def parse_workspace_STAC_source(self, source: Union[str, Link]) -> tuple[str, str]:
         """ """
         split_source = source.split("/")
 
         bucket_name = split_source[1]
         object_key = "/".join(split_source[2:])
 
         return bucket_name, object_key
```

### Comparing `eodc-2024.4.3/pyproject.toml` & `eodc-2024.4.4/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "eodc"
 
-version = "2024.4.3"
+version = "2024.4.4"
 description = "Python SDK for interacting with EODC services."
 authors = ["Lukas Weidenholzer <lukas.weidenholzer@eodc.eu>", "Gerald Irsiegler <gerald.irsiegler@eodc.eu>", "Christoph Reimer <christoph.reimer@eodc.eu>"]
 maintainers = ["EODC Staff <support@eodc.eu>"]
 readme = "README.md"
 repository = "https://github.com/eodcgmbh/eodc-sdk"
 classifiers = [
     "Development Status :: 1 - Planning",
```

### Comparing `eodc-2024.4.3/PKG-INFO` & `eodc-2024.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eodc
-Version: 2024.4.3
+Version: 2024.4.4
 Summary: Python SDK for interacting with EODC services.
 Home-page: https://github.com/eodcgmbh/eodc-sdk
 Author: Lukas Weidenholzer
 Author-email: lukas.weidenholzer@eodc.eu
 Maintainer: EODC Staff
 Maintainer-email: support@eodc.eu
 Requires-Python: >=3.9,<3.12
```


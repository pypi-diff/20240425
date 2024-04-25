# Comparing `tmp/dagster-fivetran-0.23.2rc4.tar.gz` & `tmp/dagster-fivetran-0.23.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-fivetran-0.23.2rc4.tar", last modified: Fri Apr 19 18:15:13 2024, max compression
+gzip compressed data, was "dagster-fivetran-0.23.3.tar", last modified: Thu Apr 25 20:15:32 2024, max compression
```

## Comparing `dagster-fivetran-0.23.2rc4.tar` & `dagster-fivetran-0.23.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 18:15:13.210904 dagster-fivetran-0.23.2rc4/
--rw-r--r--   0 root         (0) root         (0)    11349 2024-04-19 18:01:50.000000 dagster-fivetran-0.23.2rc4/LICENSE
--rw-r--r--   0 root         (0) root         (0)       68 2024-04-19 18:01:50.000000 dagster-fivetran-0.23.2rc4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      738 2024-04-19 18:15:13.210904 dagster-fivetran-0.23.2rc4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      134 2024-04-19 18:01:50.000000 dagster-fivetran-0.23.2rc4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 18:15:13.194904 dagster-fivetran-0.23.2rc4/dagster_fivetran/
--rw-r--r--   0 root         (0) root         (0)      854 2024-04-19 18:01:50.000000 dagster-fivetran-0.23.2rc4/dagster_fivetran/__init__.py
--rw-r--r--   0 root         (0) root         (0)    22343 2024-04-19 18:01:50.000000 dagster-fivetran-0.23.2rc4/dagster_fivetran/asset_defs.py
--rw-r--r--   0 root         (0) root         (0)      426 2024-04-19 18:01:50.000000 dagster-fivetran-0.23.2rc4/dagster_fivetran/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 18:15:13.206904 dagster-fivetran-0.23.2rc4/dagster_fivetran/managed/
--rw-r--r--   0 root         (0) root         (0)      212 2024-04-19 18:01:50.000000 dagster-fivetran-0.23.2rc4/dagster_fivetran/managed/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14615 2024-04-19 18:01:50.000000 dagster-fivetran-0.23.2rc4/dagster_fivetran/managed/reconciliation.py
--rw-r--r--   0 root         (0) root         (0)     3628 2024-04-19 18:01:50.000000 dagster-fivetran-0.23.2rc4/dagster_fivetran/managed/types.py
--rw-r--r--   0 root         (0) root         (0)     7139 2024-04-19 18:01:50.000000 dagster-fivetran-0.23.2rc4/dagster_fivetran/ops.py
--rw-r--r--   0 root         (0) root         (0)        8 2024-04-19 18:01:50.000000 dagster-fivetran-0.23.2rc4/dagster_fivetran/py.typed
--rw-r--r--   0 root         (0) root         (0)    18339 2024-04-19 18:01:50.000000 dagster-fivetran-0.23.2rc4/dagster_fivetran/resources.py
--rw-r--r--   0 root         (0) root         (0)      936 2024-04-19 18:01:50.000000 dagster-fivetran-0.23.2rc4/dagster_fivetran/types.py
--rw-r--r--   0 root         (0) root         (0)     2996 2024-04-19 18:01:50.000000 dagster-fivetran-0.23.2rc4/dagster_fivetran/utils.py
--rw-r--r--   0 root         (0) root         (0)       26 2024-04-19 18:01:50.000000 dagster-fivetran-0.23.2rc4/dagster_fivetran/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 18:15:13.194904 dagster-fivetran-0.23.2rc4/dagster_fivetran.egg-info/
--rw-r--r--   0 root         (0) root         (0)      738 2024-04-19 18:15:12.000000 dagster-fivetran-0.23.2rc4/dagster_fivetran.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      687 2024-04-19 18:15:12.000000 dagster-fivetran-0.23.2rc4/dagster_fivetran.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-19 18:15:12.000000 dagster-fivetran-0.23.2rc4/dagster_fivetran.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       63 2024-04-19 18:15:12.000000 dagster-fivetran-0.23.2rc4/dagster_fivetran.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-19 18:15:12.000000 dagster-fivetran-0.23.2rc4/dagster_fivetran.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       65 2024-04-19 18:15:12.000000 dagster-fivetran-0.23.2rc4/dagster_fivetran.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2024-04-19 18:15:12.000000 dagster-fivetran-0.23.2rc4/dagster_fivetran.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      163 2024-04-19 18:15:13.210904 dagster-fivetran-0.23.2rc4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1540 2024-04-19 18:01:50.000000 dagster-fivetran-0.23.2rc4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:15:32.524715 dagster-fivetran-0.23.3/
+-rw-r--r--   0 root         (0) root         (0)    11349 2024-04-25 20:08:31.000000 dagster-fivetran-0.23.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       68 2024-04-25 20:08:31.000000 dagster-fivetran-0.23.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      735 2024-04-25 20:15:32.524715 dagster-fivetran-0.23.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      134 2024-04-25 20:08:31.000000 dagster-fivetran-0.23.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:15:32.520715 dagster-fivetran-0.23.3/dagster_fivetran/
+-rw-r--r--   0 root         (0) root         (0)      854 2024-04-25 20:08:31.000000 dagster-fivetran-0.23.3/dagster_fivetran/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    22841 2024-04-25 20:08:31.000000 dagster-fivetran-0.23.3/dagster_fivetran/asset_defs.py
+-rw-r--r--   0 root         (0) root         (0)      426 2024-04-25 20:08:31.000000 dagster-fivetran-0.23.3/dagster_fivetran/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:15:32.524715 dagster-fivetran-0.23.3/dagster_fivetran/managed/
+-rw-r--r--   0 root         (0) root         (0)      212 2024-04-25 20:08:31.000000 dagster-fivetran-0.23.3/dagster_fivetran/managed/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14615 2024-04-25 20:08:31.000000 dagster-fivetran-0.23.3/dagster_fivetran/managed/reconciliation.py
+-rw-r--r--   0 root         (0) root         (0)     3628 2024-04-25 20:08:31.000000 dagster-fivetran-0.23.3/dagster_fivetran/managed/types.py
+-rw-r--r--   0 root         (0) root         (0)     7139 2024-04-25 20:08:31.000000 dagster-fivetran-0.23.3/dagster_fivetran/ops.py
+-rw-r--r--   0 root         (0) root         (0)        8 2024-04-25 20:08:31.000000 dagster-fivetran-0.23.3/dagster_fivetran/py.typed
+-rw-r--r--   0 root         (0) root         (0)    18339 2024-04-25 20:08:31.000000 dagster-fivetran-0.23.3/dagster_fivetran/resources.py
+-rw-r--r--   0 root         (0) root         (0)      936 2024-04-25 20:08:31.000000 dagster-fivetran-0.23.3/dagster_fivetran/types.py
+-rw-r--r--   0 root         (0) root         (0)     2996 2024-04-25 20:08:31.000000 dagster-fivetran-0.23.3/dagster_fivetran/utils.py
+-rw-r--r--   0 root         (0) root         (0)       23 2024-04-25 20:08:31.000000 dagster-fivetran-0.23.3/dagster_fivetran/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:15:32.524715 dagster-fivetran-0.23.3/dagster_fivetran.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      735 2024-04-25 20:15:32.000000 dagster-fivetran-0.23.3/dagster_fivetran.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      687 2024-04-25 20:15:32.000000 dagster-fivetran-0.23.3/dagster_fivetran.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-25 20:15:32.000000 dagster-fivetran-0.23.3/dagster_fivetran.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       63 2024-04-25 20:15:32.000000 dagster-fivetran-0.23.3/dagster_fivetran.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-25 20:15:32.000000 dagster-fivetran-0.23.3/dagster_fivetran.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       59 2024-04-25 20:15:32.000000 dagster-fivetran-0.23.3/dagster_fivetran.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2024-04-25 20:15:32.000000 dagster-fivetran-0.23.3/dagster_fivetran.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      163 2024-04-25 20:15:32.524715 dagster-fivetran-0.23.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1534 2024-04-25 20:08:31.000000 dagster-fivetran-0.23.3/setup.py
```

### Comparing `dagster-fivetran-0.23.2rc4/LICENSE` & `dagster-fivetran-0.23.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-fivetran-0.23.2rc4/PKG-INFO` & `dagster-fivetran-0.23.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-fivetran
-Version: 0.23.2rc4
+Version: 0.23.3
 Summary: Package for integrating Fivetran with Dagster.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-fivetran
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-fivetran-0.23.2rc4/dagster_fivetran/__init__.py` & `dagster-fivetran-0.23.3/dagster_fivetran/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-fivetran-0.23.2rc4/dagster_fivetran/asset_defs.py` & `dagster-fivetran-0.23.3/dagster_fivetran/asset_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -315,14 +315,15 @@
         self,
         fivetran_resource_def: Union[FivetranResource, ResourceDefinition],
         key_prefix: Sequence[str],
         connector_to_group_fn: Optional[Callable[[str], Optional[str]]],
         connector_filter: Optional[Callable[[FivetranConnectionMetadata], bool]],
         connector_to_io_manager_key_fn: Optional[Callable[[str], Optional[str]]],
         connector_to_asset_key_fn: Optional[Callable[[FivetranConnectionMetadata, str], AssetKey]],
+        destination_ids: Optional[List[str]],
         poll_interval: float,
         poll_timeout: Optional[float],
     ):
         self._fivetran_resource_def = fivetran_resource_def
         if isinstance(fivetran_resource_def, FivetranResource):
             # We hold a copy which is not fully processed, this retains e.g. EnvVars for
             # display in the UI
@@ -342,28 +343,32 @@
         self._key_prefix = key_prefix
         self._connector_to_group_fn = connector_to_group_fn
         self._connection_filter = connector_filter
         self._connector_to_io_manager_key_fn = connector_to_io_manager_key_fn
         self._connector_to_asset_key_fn: Callable[[FivetranConnectionMetadata, str], AssetKey] = (
             connector_to_asset_key_fn or (lambda _, table: AssetKey(path=table.split(".")))
         )
+        self._destination_ids = destination_ids
         self._poll_interval = poll_interval
         self._poll_timeout = poll_timeout
 
         contents = hashlib.sha1()
         contents.update(",".join(key_prefix).encode("utf-8"))
         if connector_filter:
             contents.update(inspect.getsource(connector_filter).encode("utf-8"))
 
         super().__init__(unique_id=f"fivetran-{contents.hexdigest()}")
 
     def _get_connectors(self) -> Sequence[FivetranConnectionMetadata]:
         output_connectors: List[FivetranConnectionMetadata] = []
 
-        groups = self._fivetran_instance.make_request("GET", "groups")["items"]
+        if not self._destination_ids:
+            groups = self._fivetran_instance.make_request("GET", "groups")["items"]
+        else:
+            groups = [{"id": destination_id} for destination_id in self._destination_ids]
 
         for group in groups:
             group_id = group["id"]
 
             connectors = self._fivetran_instance.make_request(
                 "GET", f"groups/{group_id}/connectors"
             )["items"]
@@ -444,14 +449,15 @@
     connector_to_group_fn: Optional[Callable[[str], Optional[str]]] = _clean_name,
     io_manager_key: Optional[str] = None,
     connector_to_io_manager_key_fn: Optional[Callable[[str], Optional[str]]] = None,
     connector_filter: Optional[Callable[[FivetranConnectionMetadata], bool]] = None,
     connector_to_asset_key_fn: Optional[
         Callable[[FivetranConnectionMetadata, str], AssetKey]
     ] = None,
+    destination_ids: Optional[List[str]] = None,
     poll_interval: float = DEFAULT_POLL_INTERVAL,
     poll_timeout: Optional[float] = None,
 ) -> CacheableAssetsDefinition:
     """Loads Fivetran connector assets from a configured FivetranResource instance. This fetches information
     about defined connectors at initialization time, and will error on workspace load if the Fivetran
     instance is not reachable.
 
@@ -468,14 +474,16 @@
             IO manager key for a given Fivetran connector name. When other ops are downstream of the loaded assets,
             the IOManager specified determines how the inputs to those ops are loaded. Defaults to "io_manager".
         connector_filter (Optional[Callable[[FivetranConnectorMetadata], bool]]): Optional function which takes
             in connector metadata and returns False if the connector should be excluded from the output assets.
         connector_to_asset_key_fn (Optional[Callable[[FivetranConnectorMetadata, str], AssetKey]]): Optional function
             which takes in connector metadata and a table name and returns an AssetKey for that table. Defaults to
             a function that generates an AssetKey matching the table name, split by ".".
+        destination_ids (Optional[List[str]]): A list of destination IDs to fetch connectors from. If None, all destinations
+            will be polled for connectors.
         poll_interval (float): The time (in seconds) that will be waited between successive polls.
         poll_timeout (Optional[float]): The maximum time that will waited before this operation is
             timed out. By default, this will never time out.
 
     **Examples:**
 
     Loading all Fivetran connectors as assets:
@@ -523,10 +531,11 @@
     return FivetranInstanceCacheableAssetsDefinition(
         fivetran_resource_def=fivetran,
         key_prefix=key_prefix,
         connector_to_group_fn=connector_to_group_fn,
         connector_to_io_manager_key_fn=connector_to_io_manager_key_fn,
         connector_filter=connector_filter,
         connector_to_asset_key_fn=connector_to_asset_key_fn,
+        destination_ids=destination_ids,
         poll_interval=poll_interval,
         poll_timeout=poll_timeout,
     )
```

### Comparing `dagster-fivetran-0.23.2rc4/dagster_fivetran/managed/reconciliation.py` & `dagster-fivetran-0.23.3/dagster_fivetran/managed/reconciliation.py`

 * *Files identical despite different names*

### Comparing `dagster-fivetran-0.23.2rc4/dagster_fivetran/managed/types.py` & `dagster-fivetran-0.23.3/dagster_fivetran/managed/types.py`

 * *Files identical despite different names*

### Comparing `dagster-fivetran-0.23.2rc4/dagster_fivetran/ops.py` & `dagster-fivetran-0.23.3/dagster_fivetran/ops.py`

 * *Files identical despite different names*

### Comparing `dagster-fivetran-0.23.2rc4/dagster_fivetran/resources.py` & `dagster-fivetran-0.23.3/dagster_fivetran/resources.py`

 * *Files identical despite different names*

### Comparing `dagster-fivetran-0.23.2rc4/dagster_fivetran/types.py` & `dagster-fivetran-0.23.3/dagster_fivetran/types.py`

 * *Files identical despite different names*

### Comparing `dagster-fivetran-0.23.2rc4/dagster_fivetran/utils.py` & `dagster-fivetran-0.23.3/dagster_fivetran/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-fivetran-0.23.2rc4/dagster_fivetran.egg-info/PKG-INFO` & `dagster-fivetran-0.23.3/dagster_fivetran.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-fivetran
-Version: 0.23.2rc4
+Version: 0.23.3
 Summary: Package for integrating Fivetran with Dagster.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-fivetran
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-fivetran-0.23.2rc4/dagster_fivetran.egg-info/SOURCES.txt` & `dagster-fivetran-0.23.3/dagster_fivetran.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dagster-fivetran-0.23.2rc4/setup.py` & `dagster-fivetran-0.23.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,20 +30,20 @@
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_fivetran_tests*"]),
     python_requires=">=3.8,<3.13",
-    install_requires=["dagster==1.7.2rc4"],
+    install_requires=["dagster==1.7.3"],
     zip_safe=False,
     entry_points={
         "console_scripts": [
             "dagster-fivetran = dagster_fivetran.cli:main",
         ]
     },
     extras_require={
         "managed": [
-            "dagster-managed-elements==0.23.2rc4",
+            "dagster-managed-elements==0.23.3",
         ],
     },
 )
```


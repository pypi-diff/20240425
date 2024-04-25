# Comparing `tmp/dagster-embedded-elt-0.23.2rc4.tar.gz` & `tmp/dagster-embedded-elt-0.23.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-embedded-elt-0.23.2rc4.tar", last modified: Fri Apr 19 18:10:27 2024, max compression
+gzip compressed data, was "dagster-embedded-elt-0.23.3.tar", last modified: Thu Apr 25 20:20:52 2024, max compression
```

## Comparing `dagster-embedded-elt-0.23.2rc4.tar` & `dagster-embedded-elt-0.23.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 18:10:27.301017 dagster-embedded-elt-0.23.2rc4/
--rw-r--r--   0 root         (0) root         (0)    11349 2024-04-19 18:01:50.000000 dagster-embedded-elt-0.23.2rc4/LICENSE
--rw-r--r--   0 root         (0) root         (0)       97 2024-04-19 18:01:50.000000 dagster-embedded-elt-0.23.2rc4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      747 2024-04-19 18:10:27.301017 dagster-embedded-elt-0.23.2rc4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      146 2024-04-19 18:01:50.000000 dagster-embedded-elt-0.23.2rc4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 18:10:27.293017 dagster-embedded-elt-0.23.2rc4/dagster_embedded_elt/
--rw-r--r--   0 root         (0) root         (0)      163 2024-04-19 18:01:50.000000 dagster-embedded-elt-0.23.2rc4/dagster_embedded_elt/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 18:10:27.297017 dagster-embedded-elt-0.23.2rc4/dagster_embedded_elt/dlt/
--rw-r--r--   0 root         (0) root         (0)      270 2024-04-19 18:01:50.000000 dagster-embedded-elt-0.23.2rc4/dagster_embedded_elt/dlt/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3681 2024-04-19 18:01:50.000000 dagster-embedded-elt-0.23.2rc4/dagster_embedded_elt/dlt/asset_decorator.py
--rw-r--r--   0 root         (0) root         (0)      129 2024-04-19 18:01:50.000000 dagster-embedded-elt-0.23.2rc4/dagster_embedded_elt/dlt/constants.py
--rw-r--r--   0 root         (0) root         (0)     7024 2024-04-19 18:01:50.000000 dagster-embedded-elt-0.23.2rc4/dagster_embedded_elt/dlt/resource.py
--rw-r--r--   0 root         (0) root         (0)     1563 2024-04-19 18:01:50.000000 dagster-embedded-elt-0.23.2rc4/dagster_embedded_elt/dlt/translator.py
--rw-r--r--   0 root         (0) root         (0)        8 2024-04-19 18:01:50.000000 dagster-embedded-elt-0.23.2rc4/dagster_embedded_elt/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 18:10:27.301017 dagster-embedded-elt-0.23.2rc4/dagster_embedded_elt/sling/
--rw-r--r--   0 root         (0) root         (0)      718 2024-04-19 18:01:50.000000 dagster-embedded-elt-0.23.2rc4/dagster_embedded_elt/sling/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4738 2024-04-19 18:01:50.000000 dagster-embedded-elt-0.23.2rc4/dagster_embedded_elt/sling/asset_decorator.py
--rw-r--r--   0 root         (0) root         (0)     4162 2024-04-19 18:01:50.000000 dagster-embedded-elt-0.23.2rc4/dagster_embedded_elt/sling/asset_defs.py
--rw-r--r--   0 root         (0) root         (0)     8087 2024-04-19 18:01:50.000000 dagster-embedded-elt-0.23.2rc4/dagster_embedded_elt/sling/dagster_sling_translator.py
--rw-r--r--   0 root         (0) root         (0)    17560 2024-04-19 18:01:50.000000 dagster-embedded-elt-0.23.2rc4/dagster_embedded_elt/sling/resources.py
--rw-r--r--   0 root         (0) root         (0)     1106 2024-04-19 18:01:50.000000 dagster-embedded-elt-0.23.2rc4/dagster_embedded_elt/sling/sling_replication.py
--rw-r--r--   0 root         (0) root         (0)       26 2024-04-19 18:01:50.000000 dagster-embedded-elt-0.23.2rc4/dagster_embedded_elt/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 18:10:27.293017 dagster-embedded-elt-0.23.2rc4/dagster_embedded_elt.egg-info/
--rw-r--r--   0 root         (0) root         (0)      747 2024-04-19 18:10:27.000000 dagster-embedded-elt-0.23.2rc4/dagster_embedded_elt.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      886 2024-04-19 18:10:27.000000 dagster-embedded-elt-0.23.2rc4/dagster_embedded_elt.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-19 18:10:27.000000 dagster-embedded-elt-0.23.2rc4/dagster_embedded_elt.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-19 18:10:27.000000 dagster-embedded-elt-0.23.2rc4/dagster_embedded_elt.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       55 2024-04-19 18:10:27.000000 dagster-embedded-elt-0.23.2rc4/dagster_embedded_elt.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       21 2024-04-19 18:10:27.000000 dagster-embedded-elt-0.23.2rc4/dagster_embedded_elt.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      124 2024-04-19 18:01:50.000000 dagster-embedded-elt-0.23.2rc4/integration.yaml
--rw-r--r--   0 root         (0) root         (0)      167 2024-04-19 18:10:27.301017 dagster-embedded-elt-0.23.2rc4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1430 2024-04-19 18:01:50.000000 dagster-embedded-elt-0.23.2rc4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:20:52.501854 dagster-embedded-elt-0.23.3/
+-rw-r--r--   0 root         (0) root         (0)    11349 2024-04-25 20:08:31.000000 dagster-embedded-elt-0.23.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       97 2024-04-25 20:08:31.000000 dagster-embedded-elt-0.23.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      744 2024-04-25 20:20:52.501854 dagster-embedded-elt-0.23.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      146 2024-04-25 20:08:31.000000 dagster-embedded-elt-0.23.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:20:52.497854 dagster-embedded-elt-0.23.3/dagster_embedded_elt/
+-rw-r--r--   0 root         (0) root         (0)      163 2024-04-25 20:08:31.000000 dagster-embedded-elt-0.23.3/dagster_embedded_elt/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:20:52.501854 dagster-embedded-elt-0.23.3/dagster_embedded_elt/dlt/
+-rw-r--r--   0 root         (0) root         (0)      270 2024-04-25 20:08:31.000000 dagster-embedded-elt-0.23.3/dagster_embedded_elt/dlt/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3875 2024-04-25 20:08:31.000000 dagster-embedded-elt-0.23.3/dagster_embedded_elt/dlt/asset_decorator.py
+-rw-r--r--   0 root         (0) root         (0)      129 2024-04-25 20:08:31.000000 dagster-embedded-elt-0.23.3/dagster_embedded_elt/dlt/constants.py
+-rw-r--r--   0 root         (0) root         (0)     7033 2024-04-25 20:08:31.000000 dagster-embedded-elt-0.23.3/dagster_embedded_elt/dlt/resource.py
+-rw-r--r--   0 root         (0) root         (0)     1563 2024-04-25 20:08:31.000000 dagster-embedded-elt-0.23.3/dagster_embedded_elt/dlt/translator.py
+-rw-r--r--   0 root         (0) root         (0)        8 2024-04-25 20:08:31.000000 dagster-embedded-elt-0.23.3/dagster_embedded_elt/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:20:52.501854 dagster-embedded-elt-0.23.3/dagster_embedded_elt/sling/
+-rw-r--r--   0 root         (0) root         (0)      718 2024-04-25 20:08:31.000000 dagster-embedded-elt-0.23.3/dagster_embedded_elt/sling/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4954 2024-04-25 20:08:31.000000 dagster-embedded-elt-0.23.3/dagster_embedded_elt/sling/asset_decorator.py
+-rw-r--r--   0 root         (0) root         (0)     4162 2024-04-25 20:08:31.000000 dagster-embedded-elt-0.23.3/dagster_embedded_elt/sling/asset_defs.py
+-rw-r--r--   0 root         (0) root         (0)     8087 2024-04-25 20:08:31.000000 dagster-embedded-elt-0.23.3/dagster_embedded_elt/sling/dagster_sling_translator.py
+-rw-r--r--   0 root         (0) root         (0)    17560 2024-04-25 20:08:31.000000 dagster-embedded-elt-0.23.3/dagster_embedded_elt/sling/resources.py
+-rw-r--r--   0 root         (0) root         (0)     1106 2024-04-25 20:08:31.000000 dagster-embedded-elt-0.23.3/dagster_embedded_elt/sling/sling_replication.py
+-rw-r--r--   0 root         (0) root         (0)       23 2024-04-25 20:08:31.000000 dagster-embedded-elt-0.23.3/dagster_embedded_elt/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:20:52.497854 dagster-embedded-elt-0.23.3/dagster_embedded_elt.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      744 2024-04-25 20:20:52.000000 dagster-embedded-elt-0.23.3/dagster_embedded_elt.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      886 2024-04-25 20:20:52.000000 dagster-embedded-elt-0.23.3/dagster_embedded_elt.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-25 20:20:52.000000 dagster-embedded-elt-0.23.3/dagster_embedded_elt.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-25 20:20:52.000000 dagster-embedded-elt-0.23.3/dagster_embedded_elt.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       52 2024-04-25 20:20:52.000000 dagster-embedded-elt-0.23.3/dagster_embedded_elt.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-25 20:20:52.000000 dagster-embedded-elt-0.23.3/dagster_embedded_elt.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      124 2024-04-25 20:08:31.000000 dagster-embedded-elt-0.23.3/integration.yaml
+-rw-r--r--   0 root         (0) root         (0)      167 2024-04-25 20:20:52.505854 dagster-embedded-elt-0.23.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1427 2024-04-25 20:08:31.000000 dagster-embedded-elt-0.23.3/setup.py
```

### Comparing `dagster-embedded-elt-0.23.2rc4/LICENSE` & `dagster-embedded-elt-0.23.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-embedded-elt-0.23.2rc4/dagster_embedded_elt/dlt/asset_decorator.py` & `dagster-embedded-elt-0.23.3/dagster_embedded_elt/dlt/asset_decorator.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from typing import Any, Callable, Optional
 
 from dagster import (
     AssetsDefinition,
     AssetSpec,
+    _check as check,
     multi_asset,
 )
 from dlt.extract.source import DltSource
 from dlt.pipeline.pipeline import Pipeline
 
 from .constants import META_KEY_PIPELINE, META_KEY_SOURCE, META_KEY_TRANSLATOR
 from .translator import DagsterDltTranslator
@@ -14,15 +15,15 @@
 
 def dlt_assets(
     *,
     dlt_source: DltSource,
     dlt_pipeline: Pipeline,
     name: Optional[str] = None,
     group_name: Optional[str] = None,
-    dlt_dagster_translator: DagsterDltTranslator = DagsterDltTranslator(),
+    dlt_dagster_translator: Optional[DagsterDltTranslator] = None,
 ) -> Callable[[Callable[..., Any]], AssetsDefinition]:
     """Asset Factory for using data load tool (dlt).
 
     Args:
         dlt_source (DltSource): The DltSource to be ingested.
         dlt_pipeline (Pipeline): The dlt Pipeline defining the destination parameters.
         name (Optional[str], optional): The name of the op.
@@ -72,14 +73,18 @@
                 name="github",
                 group_name="github",
             )
             def github_reactions_dagster_assets(context: AssetExecutionContext, dlt: DltDagsterResource):
                 yield from dlt.run(context=context)
 
     """
+    dlt_dagster_translator = (
+        check.opt_inst_param(dlt_dagster_translator, "dlt_dagster_translator", DagsterDltTranslator)
+        or DagsterDltTranslator()
+    )
     return multi_asset(
         name=name,
         group_name=group_name,
         compute_kind="dlt",
         can_subset=True,
         specs=[
             AssetSpec(
@@ -90,10 +95,10 @@
                 ),
                 metadata={
                     META_KEY_SOURCE: dlt_source,
                     META_KEY_PIPELINE: dlt_pipeline,
                     META_KEY_TRANSLATOR: dlt_dagster_translator,
                 },
             )
-            for dlt_source_resource in dlt_source.resources.values()
+            for dlt_source_resource in dlt_source.selected_resources.values()
         ],
     )
```

### Comparing `dagster-embedded-elt-0.23.2rc4/dagster_embedded_elt/dlt/resource.py` & `dagster-embedded-elt-0.23.3/dagster_embedded_elt/dlt/resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -138,15 +138,15 @@
         )
 
         # Default to base translator if undefined
         dagster_dlt_translator = dagster_dlt_translator or DagsterDltTranslator()
 
         asset_key_dlt_source_resource_mapping = {
             dagster_dlt_translator.get_asset_key(dlt_source_resource): dlt_source_resource
-            for dlt_source_resource in dlt_source.resources.values()
+            for dlt_source_resource in dlt_source.selected_resources.values()
         }
 
         # Filter sources by asset key sub-selection
         if context.is_subset:
             asset_key_dlt_source_resource_mapping = {
                 asset_key: asset_dlt_source_resource
                 for (
```

### Comparing `dagster-embedded-elt-0.23.2rc4/dagster_embedded_elt/dlt/translator.py` & `dagster-embedded-elt-0.23.3/dagster_embedded_elt/dlt/translator.py`

 * *Files identical despite different names*

### Comparing `dagster-embedded-elt-0.23.2rc4/dagster_embedded_elt/sling/__init__.py` & `dagster-embedded-elt-0.23.3/dagster_embedded_elt/sling/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-embedded-elt-0.23.2rc4/dagster_embedded_elt/sling/asset_decorator.py` & `dagster-embedded-elt-0.23.3/dagster_embedded_elt/sling/asset_decorator.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from typing import Any, Callable, Iterable, Mapping, Optional
 
 from dagster import (
     AssetsDefinition,
     AssetSpec,
     BackfillPolicy,
     PartitionsDefinition,
+    _check as check,
     multi_asset,
 )
 from dagster._utils.security import non_secure_md5_hash_str
 
 from dagster_embedded_elt.sling.dagster_sling_translator import DagsterSlingTranslator
 from dagster_embedded_elt.sling.sling_replication import SlingReplicationParam, validate_replication
 
@@ -25,15 +26,15 @@
             continue
         yield {"name": stream, "config": config}
 
 
 def sling_assets(
     *,
     replication_config: SlingReplicationParam,
-    dagster_sling_translator: DagsterSlingTranslator = DagsterSlingTranslator(),
+    dagster_sling_translator: Optional[DagsterSlingTranslator] = None,
     name: Optional[str] = None,
     partitions_def: Optional[PartitionsDefinition] = None,
     backfill_policy: Optional[BackfillPolicy] = None,
     op_tags: Optional[Mapping[str, Any]] = None,
 ) -> Callable[[Callable[..., Any]], AssetsDefinition]:
     """Create a definition for how to materialize a set of Sling replication streams as Dagster assets, as
     described by a Sling replication config. This will create on Asset for every Sling target stream.
@@ -76,14 +77,21 @@
             def my_assets(context, sling: SlingResource):
                 yield from sling.replicate(context=context)
     """
     replication_config = validate_replication(replication_config)
     streams = get_streams_from_replication(replication_config)
     code_version = non_secure_md5_hash_str(str(replication_config).encode())
 
+    dagster_sling_translator = (
+        check.opt_inst_param(
+            dagster_sling_translator, "dagster_sling_translator", DagsterSlingTranslator
+        )
+        or DagsterSlingTranslator()
+    )
+
     return multi_asset(
         name=name,
         compute_kind="sling",
         partitions_def=partitions_def,
         can_subset=False,
         op_tags=op_tags,
         backfill_policy=backfill_policy,
```

### Comparing `dagster-embedded-elt-0.23.2rc4/dagster_embedded_elt/sling/asset_defs.py` & `dagster-embedded-elt-0.23.3/dagster_embedded_elt/sling/asset_defs.py`

 * *Files identical despite different names*

### Comparing `dagster-embedded-elt-0.23.2rc4/dagster_embedded_elt/sling/dagster_sling_translator.py` & `dagster-embedded-elt-0.23.3/dagster_embedded_elt/sling/dagster_sling_translator.py`

 * *Files identical despite different names*

### Comparing `dagster-embedded-elt-0.23.2rc4/dagster_embedded_elt/sling/resources.py` & `dagster-embedded-elt-0.23.3/dagster_embedded_elt/sling/resources.py`

 * *Files identical despite different names*

### Comparing `dagster-embedded-elt-0.23.2rc4/dagster_embedded_elt/sling/sling_replication.py` & `dagster-embedded-elt-0.23.3/dagster_embedded_elt/sling/sling_replication.py`

 * *Files identical despite different names*

### Comparing `dagster-embedded-elt-0.23.2rc4/dagster_embedded_elt.egg-info/SOURCES.txt` & `dagster-embedded-elt-0.23.3/dagster_embedded_elt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dagster-embedded-elt-0.23.2rc4/setup.py` & `dagster-embedded-elt-0.23.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_embedded_elt_tests*"]),
     python_requires=">=3.8,<3.13",
-    install_requires=["dagster==1.7.2rc4", "sling>=1.1.5", "dlt>=0.4"],
+    install_requires=["dagster==1.7.3", "sling>=1.1.5", "dlt>=0.4"],
     zip_safe=False,
     extras_require={
         "test": [
             "duckdb",
         ]
     },
 )
```


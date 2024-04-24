# Comparing `tmp/geneweaver_core-0.9.0a9.tar.gz` & `tmp/geneweaver_core-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geneweaver_core-0.9.0a9.tar", max compression
+gzip compressed data, was "geneweaver_core-0.9.1.tar", max compression
```

## Comparing `geneweaver_core-0.9.0a9.tar` & `geneweaver_core-0.9.1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0    11356 2024-04-19 19:16:27.514305 geneweaver_core-0.9.0a9/LICENSE
--rw-r--r--   0        0        0     3413 2024-04-19 19:16:27.514305 geneweaver_core-0.9.0a9/README.md
--rw-r--r--   0        0        0     1036 2024-04-19 19:16:27.514305 geneweaver_core-0.9.0a9/pyproject.toml
--rw-r--r--   0        0        0      109 2024-04-19 19:16:27.514305 geneweaver_core-0.9.0a9/src/geneweaver/core/__init__.py
--rw-r--r--   0        0        0      171 2024-04-19 19:16:27.514305 geneweaver_core-0.9.0a9/src/geneweaver/core/config.py
--rw-r--r--   0        0        0      739 2024-04-19 19:16:27.514305 geneweaver_core-0.9.0a9/src/geneweaver/core/config_class.py
--rw-r--r--   0        0        0    12499 2024-04-19 19:16:27.514305 geneweaver_core-0.9.0a9/src/geneweaver/core/enum.py
--rw-r--r--   0        0        0      257 2024-04-19 19:16:27.514305 geneweaver_core-0.9.0a9/src/geneweaver/core/exc.py
--rw-r--r--   0        0        0      638 2024-04-19 19:16:27.514305 geneweaver_core-0.9.0a9/src/geneweaver/core/mapping.py
--rw-r--r--   0        0        0       53 2024-04-19 19:16:27.514305 geneweaver_core-0.9.0a9/src/geneweaver/core/parse/__init__.py
--rw-r--r--   0        0        0    18345 2024-04-19 19:16:27.514305 geneweaver_core-0.9.0a9/src/geneweaver/core/parse/batch.py
--rw-r--r--   0        0        0     5841 2024-04-19 19:16:27.518305 geneweaver_core-0.9.0a9/src/geneweaver/core/parse/csv.py
--rw-r--r--   0        0        0      322 2024-04-19 19:16:27.518305 geneweaver_core-0.9.0a9/src/geneweaver/core/parse/enum.py
--rw-r--r--   0        0        0     1456 2024-04-19 19:16:27.518305 geneweaver_core-0.9.0a9/src/geneweaver/core/parse/exceptions.py
--rw-r--r--   0        0        0     5053 2024-04-19 19:16:27.518305 geneweaver_core-0.9.0a9/src/geneweaver/core/parse/numpy.py
--rw-r--r--   0        0        0     9436 2024-04-19 19:16:27.518305 geneweaver_core-0.9.0a9/src/geneweaver/core/parse/score.py
--rw-r--r--   0        0        0     3435 2024-04-19 19:16:27.518305 geneweaver_core-0.9.0a9/src/geneweaver/core/parse/threshold.py
--rw-r--r--   0        0        0     1936 2024-04-19 19:16:27.518305 geneweaver_core-0.9.0a9/src/geneweaver/core/parse/utils.py
--rw-r--r--   0        0        0    10903 2024-04-19 19:16:27.518305 geneweaver_core-0.9.0a9/src/geneweaver/core/parse/xlsx.py
--rw-r--r--   0        0        0       81 2024-04-19 19:16:27.518305 geneweaver_core-0.9.0a9/src/geneweaver/core/publication/__init__.py
--rw-r--r--   0        0        0     6079 2024-04-19 19:16:27.518305 geneweaver_core-0.9.0a9/src/geneweaver/core/publication/pubmed.py
--rw-r--r--   0        0        0       79 2024-04-19 19:16:27.518305 geneweaver_core-0.9.0a9/src/geneweaver/core/render/__init__.py
--rw-r--r--   0        0        0     1913 2024-04-19 19:16:27.518305 geneweaver_core-0.9.0a9/src/geneweaver/core/render/batch.py
--rw-r--r--   0        0        0     1281 2024-04-19 19:16:27.518305 geneweaver_core-0.9.0a9/src/geneweaver/core/render/csv.py
--rw-r--r--   0        0        0      679 2024-04-19 19:16:27.518305 geneweaver_core-0.9.0a9/src/geneweaver/core/render/gene_list.py
--rw-r--r--   0        0        0      417 2024-04-19 19:16:27.518305 geneweaver_core-0.9.0a9/src/geneweaver/core/schema/__init__.py
--rw-r--r--   0        0        0      717 2024-04-19 19:16:27.518305 geneweaver_core-0.9.0a9/src/geneweaver/core/schema/api_response.py
--rw-r--r--   0        0        0     4263 2024-04-19 19:16:27.518305 geneweaver_core-0.9.0a9/src/geneweaver/core/schema/batch.py
--rw-r--r--   0        0        0     1696 2024-04-19 19:16:27.518305 geneweaver_core-0.9.0a9/src/geneweaver/core/schema/gene.py
--rw-r--r--   0        0        0     2360 2024-04-19 19:16:27.518305 geneweaver_core-0.9.0a9/src/geneweaver/core/schema/geneset.py
--rw-r--r--   0        0        0      462 2024-04-19 19:16:27.518305 geneweaver_core-0.9.0a9/src/geneweaver/core/schema/group.py
--rw-r--r--   0        0        0     1204 2024-04-19 19:16:27.518305 geneweaver_core-0.9.0a9/src/geneweaver/core/schema/legacy_api.py
--rw-r--r--   0        0        0      814 2024-04-19 19:16:27.518305 geneweaver_core-0.9.0a9/src/geneweaver/core/schema/messages.py
--rw-r--r--   0        0        0      505 2024-04-19 19:16:27.518305 geneweaver_core-0.9.0a9/src/geneweaver/core/schema/ontology.py
--rw-r--r--   0        0        0      330 2024-04-19 19:16:27.518305 geneweaver_core-0.9.0a9/src/geneweaver/core/schema/project.py
--rw-r--r--   0        0        0      511 2024-04-19 19:16:27.518305 geneweaver_core-0.9.0a9/src/geneweaver/core/schema/publication.py
--rw-r--r--   0        0        0      944 2024-04-19 19:16:27.518305 geneweaver_core-0.9.0a9/src/geneweaver/core/schema/score.py
--rw-r--r--   0        0        0      594 2024-04-19 19:16:27.518305 geneweaver_core-0.9.0a9/src/geneweaver/core/schema/species.py
--rw-r--r--   0        0        0      212 2024-04-19 19:16:27.518305 geneweaver_core-0.9.0a9/src/geneweaver/core/schema/stubgenerator.py
--rw-r--r--   0        0        0      942 2024-04-19 19:16:27.518305 geneweaver_core-0.9.0a9/src/geneweaver/core/schema/user.py
--rw-r--r--   0        0        0     1453 2024-04-19 19:16:27.518305 geneweaver_core-0.9.0a9/src/geneweaver/core/threshold.py
--rw-r--r--   0        0        0      321 2024-04-19 19:16:27.518305 geneweaver_core-0.9.0a9/src/geneweaver/core/types.py
--rw-r--r--   0        0        0      528 2024-04-19 19:16:27.518305 geneweaver_core-0.9.0a9/src/geneweaver/core/utils.py
--rw-r--r--   0        0        0     4340 1970-01-01 00:00:00.000000 geneweaver_core-0.9.0a9/PKG-INFO
+-rw-r--r--   0        0        0    11356 2024-04-22 12:56:13.352972 geneweaver_core-0.9.1/LICENSE
+-rw-r--r--   0        0        0     3413 2024-04-22 12:56:13.352972 geneweaver_core-0.9.1/README.md
+-rw-r--r--   0        0        0     1034 2024-04-22 12:56:13.352972 geneweaver_core-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0      109 2024-04-22 12:56:13.352972 geneweaver_core-0.9.1/src/geneweaver/core/__init__.py
+-rw-r--r--   0        0        0      171 2024-04-22 12:56:13.352972 geneweaver_core-0.9.1/src/geneweaver/core/config.py
+-rw-r--r--   0        0        0      739 2024-04-22 12:56:13.352972 geneweaver_core-0.9.1/src/geneweaver/core/config_class.py
+-rw-r--r--   0        0        0    12499 2024-04-22 12:56:13.352972 geneweaver_core-0.9.1/src/geneweaver/core/enum.py
+-rw-r--r--   0        0        0      257 2024-04-22 12:56:13.352972 geneweaver_core-0.9.1/src/geneweaver/core/exc.py
+-rw-r--r--   0        0        0      638 2024-04-22 12:56:13.352972 geneweaver_core-0.9.1/src/geneweaver/core/mapping.py
+-rw-r--r--   0        0        0       53 2024-04-22 12:56:13.352972 geneweaver_core-0.9.1/src/geneweaver/core/parse/__init__.py
+-rw-r--r--   0        0        0    18345 2024-04-22 12:56:13.352972 geneweaver_core-0.9.1/src/geneweaver/core/parse/batch.py
+-rw-r--r--   0        0        0     5841 2024-04-22 12:56:13.352972 geneweaver_core-0.9.1/src/geneweaver/core/parse/csv.py
+-rw-r--r--   0        0        0      322 2024-04-22 12:56:13.352972 geneweaver_core-0.9.1/src/geneweaver/core/parse/enum.py
+-rw-r--r--   0        0        0     1456 2024-04-22 12:56:13.352972 geneweaver_core-0.9.1/src/geneweaver/core/parse/exceptions.py
+-rw-r--r--   0        0        0     5053 2024-04-22 12:56:13.356972 geneweaver_core-0.9.1/src/geneweaver/core/parse/numpy.py
+-rw-r--r--   0        0        0     9436 2024-04-22 12:56:13.356972 geneweaver_core-0.9.1/src/geneweaver/core/parse/score.py
+-rw-r--r--   0        0        0     3435 2024-04-22 12:56:13.356972 geneweaver_core-0.9.1/src/geneweaver/core/parse/threshold.py
+-rw-r--r--   0        0        0     1936 2024-04-22 12:56:13.356972 geneweaver_core-0.9.1/src/geneweaver/core/parse/utils.py
+-rw-r--r--   0        0        0    10903 2024-04-22 12:56:13.356972 geneweaver_core-0.9.1/src/geneweaver/core/parse/xlsx.py
+-rw-r--r--   0        0        0       81 2024-04-22 12:56:13.356972 geneweaver_core-0.9.1/src/geneweaver/core/publication/__init__.py
+-rw-r--r--   0        0        0     6079 2024-04-22 12:56:13.356972 geneweaver_core-0.9.1/src/geneweaver/core/publication/pubmed.py
+-rw-r--r--   0        0        0       79 2024-04-22 12:56:13.356972 geneweaver_core-0.9.1/src/geneweaver/core/render/__init__.py
+-rw-r--r--   0        0        0     1913 2024-04-22 12:56:13.356972 geneweaver_core-0.9.1/src/geneweaver/core/render/batch.py
+-rw-r--r--   0        0        0     1281 2024-04-22 12:56:13.356972 geneweaver_core-0.9.1/src/geneweaver/core/render/csv.py
+-rw-r--r--   0        0        0      679 2024-04-22 12:56:13.356972 geneweaver_core-0.9.1/src/geneweaver/core/render/gene_list.py
+-rw-r--r--   0        0        0      417 2024-04-22 12:56:13.356972 geneweaver_core-0.9.1/src/geneweaver/core/schema/__init__.py
+-rw-r--r--   0        0        0      717 2024-04-22 12:56:13.356972 geneweaver_core-0.9.1/src/geneweaver/core/schema/api_response.py
+-rw-r--r--   0        0        0     4263 2024-04-22 12:56:13.356972 geneweaver_core-0.9.1/src/geneweaver/core/schema/batch.py
+-rw-r--r--   0        0        0     1696 2024-04-22 12:56:13.356972 geneweaver_core-0.9.1/src/geneweaver/core/schema/gene.py
+-rw-r--r--   0        0        0     2360 2024-04-22 12:56:13.356972 geneweaver_core-0.9.1/src/geneweaver/core/schema/geneset.py
+-rw-r--r--   0        0        0      462 2024-04-22 12:56:13.356972 geneweaver_core-0.9.1/src/geneweaver/core/schema/group.py
+-rw-r--r--   0        0        0     1204 2024-04-22 12:56:13.356972 geneweaver_core-0.9.1/src/geneweaver/core/schema/legacy_api.py
+-rw-r--r--   0        0        0      814 2024-04-22 12:56:13.356972 geneweaver_core-0.9.1/src/geneweaver/core/schema/messages.py
+-rw-r--r--   0        0        0      505 2024-04-22 12:56:13.356972 geneweaver_core-0.9.1/src/geneweaver/core/schema/ontology.py
+-rw-r--r--   0        0        0      330 2024-04-22 12:56:13.356972 geneweaver_core-0.9.1/src/geneweaver/core/schema/project.py
+-rw-r--r--   0        0        0      511 2024-04-22 12:56:13.356972 geneweaver_core-0.9.1/src/geneweaver/core/schema/publication.py
+-rw-r--r--   0        0        0      944 2024-04-22 12:56:13.356972 geneweaver_core-0.9.1/src/geneweaver/core/schema/score.py
+-rw-r--r--   0        0        0      594 2024-04-22 12:56:13.356972 geneweaver_core-0.9.1/src/geneweaver/core/schema/species.py
+-rw-r--r--   0        0        0      212 2024-04-22 12:56:13.356972 geneweaver_core-0.9.1/src/geneweaver/core/schema/stubgenerator.py
+-rw-r--r--   0        0        0      942 2024-04-22 12:56:13.356972 geneweaver_core-0.9.1/src/geneweaver/core/schema/user.py
+-rw-r--r--   0        0        0     1453 2024-04-22 12:56:13.356972 geneweaver_core-0.9.1/src/geneweaver/core/threshold.py
+-rw-r--r--   0        0        0      321 2024-04-22 12:56:13.356972 geneweaver_core-0.9.1/src/geneweaver/core/types.py
+-rw-r--r--   0        0        0      528 2024-04-22 12:56:13.356972 geneweaver_core-0.9.1/src/geneweaver/core/utils.py
+-rw-r--r--   0        0        0     4338 1970-01-01 00:00:00.000000 geneweaver_core-0.9.1/PKG-INFO
```

### Comparing `geneweaver_core-0.9.0a9/LICENSE` & `geneweaver_core-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `geneweaver_core-0.9.0a9/README.md` & `geneweaver_core-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `geneweaver_core-0.9.0a9/pyproject.toml` & `geneweaver_core-0.9.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "geneweaver-core"
-version = "0.9.0a9"
+version = "0.9.1"
 description = "The core of the Jax-Geneweaver Python library"
 authors = ["Jax Computational Sciences <cssc@jax.org>"]
 readme = "README.md"
 license = "Apache-2.0"
 repository = "https://github.com/TheJacksonLaboratory/geneweaver-client"
 homepage = "https://thejacksonlaboratory.github.io/geneweaver-docs/"
 packages = [
```

### Comparing `geneweaver_core-0.9.0a9/src/geneweaver/core/config_class.py` & `geneweaver_core-0.9.1/src/geneweaver/core/config_class.py`

 * *Files identical despite different names*

### Comparing `geneweaver_core-0.9.0a9/src/geneweaver/core/enum.py` & `geneweaver_core-0.9.1/src/geneweaver/core/enum.py`

 * *Files identical despite different names*

### Comparing `geneweaver_core-0.9.0a9/src/geneweaver/core/mapping.py` & `geneweaver_core-0.9.1/src/geneweaver/core/mapping.py`

 * *Files identical despite different names*

### Comparing `geneweaver_core-0.9.0a9/src/geneweaver/core/parse/batch.py` & `geneweaver_core-0.9.1/src/geneweaver/core/parse/batch.py`

 * *Files identical despite different names*

### Comparing `geneweaver_core-0.9.0a9/src/geneweaver/core/parse/csv.py` & `geneweaver_core-0.9.1/src/geneweaver/core/parse/csv.py`

 * *Files identical despite different names*

### Comparing `geneweaver_core-0.9.0a9/src/geneweaver/core/parse/exceptions.py` & `geneweaver_core-0.9.1/src/geneweaver/core/parse/exceptions.py`

 * *Files identical despite different names*

### Comparing `geneweaver_core-0.9.0a9/src/geneweaver/core/parse/numpy.py` & `geneweaver_core-0.9.1/src/geneweaver/core/parse/numpy.py`

 * *Files identical despite different names*

### Comparing `geneweaver_core-0.9.0a9/src/geneweaver/core/parse/score.py` & `geneweaver_core-0.9.1/src/geneweaver/core/parse/score.py`

 * *Files identical despite different names*

### Comparing `geneweaver_core-0.9.0a9/src/geneweaver/core/parse/threshold.py` & `geneweaver_core-0.9.1/src/geneweaver/core/parse/threshold.py`

 * *Files identical despite different names*

### Comparing `geneweaver_core-0.9.0a9/src/geneweaver/core/parse/utils.py` & `geneweaver_core-0.9.1/src/geneweaver/core/parse/utils.py`

 * *Files identical despite different names*

### Comparing `geneweaver_core-0.9.0a9/src/geneweaver/core/parse/xlsx.py` & `geneweaver_core-0.9.1/src/geneweaver/core/parse/xlsx.py`

 * *Files identical despite different names*

### Comparing `geneweaver_core-0.9.0a9/src/geneweaver/core/publication/pubmed.py` & `geneweaver_core-0.9.1/src/geneweaver/core/publication/pubmed.py`

 * *Files identical despite different names*

### Comparing `geneweaver_core-0.9.0a9/src/geneweaver/core/render/batch.py` & `geneweaver_core-0.9.1/src/geneweaver/core/render/batch.py`

 * *Files identical despite different names*

### Comparing `geneweaver_core-0.9.0a9/src/geneweaver/core/render/csv.py` & `geneweaver_core-0.9.1/src/geneweaver/core/render/csv.py`

 * *Files identical despite different names*

### Comparing `geneweaver_core-0.9.0a9/src/geneweaver/core/render/gene_list.py` & `geneweaver_core-0.9.1/src/geneweaver/core/render/gene_list.py`

 * *Files identical despite different names*

### Comparing `geneweaver_core-0.9.0a9/src/geneweaver/core/schema/api_response.py` & `geneweaver_core-0.9.1/src/geneweaver/core/schema/api_response.py`

 * *Files identical despite different names*

### Comparing `geneweaver_core-0.9.0a9/src/geneweaver/core/schema/batch.py` & `geneweaver_core-0.9.1/src/geneweaver/core/schema/batch.py`

 * *Files identical despite different names*

### Comparing `geneweaver_core-0.9.0a9/src/geneweaver/core/schema/gene.py` & `geneweaver_core-0.9.1/src/geneweaver/core/schema/gene.py`

 * *Files identical despite different names*

### Comparing `geneweaver_core-0.9.0a9/src/geneweaver/core/schema/geneset.py` & `geneweaver_core-0.9.1/src/geneweaver/core/schema/geneset.py`

 * *Files identical despite different names*

### Comparing `geneweaver_core-0.9.0a9/src/geneweaver/core/schema/legacy_api.py` & `geneweaver_core-0.9.1/src/geneweaver/core/schema/legacy_api.py`

 * *Files identical despite different names*

### Comparing `geneweaver_core-0.9.0a9/src/geneweaver/core/schema/messages.py` & `geneweaver_core-0.9.1/src/geneweaver/core/schema/messages.py`

 * *Files identical despite different names*

### Comparing `geneweaver_core-0.9.0a9/src/geneweaver/core/schema/score.py` & `geneweaver_core-0.9.1/src/geneweaver/core/schema/score.py`

 * *Files identical despite different names*

### Comparing `geneweaver_core-0.9.0a9/src/geneweaver/core/schema/species.py` & `geneweaver_core-0.9.1/src/geneweaver/core/schema/species.py`

 * *Files identical despite different names*

### Comparing `geneweaver_core-0.9.0a9/src/geneweaver/core/schema/user.py` & `geneweaver_core-0.9.1/src/geneweaver/core/schema/user.py`

 * *Files identical despite different names*

### Comparing `geneweaver_core-0.9.0a9/src/geneweaver/core/threshold.py` & `geneweaver_core-0.9.1/src/geneweaver/core/threshold.py`

 * *Files identical despite different names*

### Comparing `geneweaver_core-0.9.0a9/src/geneweaver/core/utils.py` & `geneweaver_core-0.9.1/src/geneweaver/core/utils.py`

 * *Files identical despite different names*

### Comparing `geneweaver_core-0.9.0a9/PKG-INFO` & `geneweaver_core-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geneweaver-core
-Version: 0.9.0a9
+Version: 0.9.1
 Summary: The core of the Jax-Geneweaver Python library
 Home-page: https://thejacksonlaboratory.github.io/geneweaver-docs/
 License: Apache-2.0
 Author: Jax Computational Sciences
 Author-email: cssc@jax.org
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```


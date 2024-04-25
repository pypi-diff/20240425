# Comparing `tmp/moveread_datasets-0.1.2.tar.gz` & `tmp/moveread_datasets-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moveread_datasets-0.1.2.tar", last modified: Thu Apr 25 07:24:14 2024, max compression
+gzip compressed data, was "moveread_datasets-0.1.3.tar", last modified: Thu Apr 25 14:56:56 2024, max compression
```

## Comparing `moveread_datasets-0.1.2.tar` & `moveread_datasets-0.1.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 07:24:14.054243 moveread_datasets-0.1.2/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      504 2024-04-25 07:24:14.054243 moveread_datasets-0.1.2/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       33 2024-04-24 09:15:05.000000 moveread_datasets-0.1.2/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      549 2024-04-25 07:24:10.000000 moveread_datasets-0.1.2/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-25 07:24:14.054243 moveread_datasets-0.1.2/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 07:24:14.044243 moveread_datasets-0.1.2/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 07:24:14.044243 moveread_datasets-0.1.2/src/moveread/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 07:24:14.054243 moveread_datasets-0.1.2/src/moveread/datasets/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      112 2024-04-25 05:56:30.000000 moveread_datasets-0.1.2/src/moveread/datasets/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1145 2024-04-25 07:23:48.000000 moveread_datasets-0.1.2/src/moveread/datasets/main.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 07:24:14.054243 moveread_datasets-0.1.2/src/moveread_datasets.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      504 2024-04-25 07:24:14.000000 moveread_datasets-0.1.2/src/moveread_datasets.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      312 2024-04-25 07:24:14.000000 moveread_datasets-0.1.2/src/moveread_datasets.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-25 07:24:14.000000 moveread_datasets-0.1.2/src/moveread_datasets.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       61 2024-04-25 07:24:14.000000 moveread_datasets-0.1.2/src/moveread_datasets.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        9 2024-04-25 07:24:14.000000 moveread_datasets-0.1.2/src/moveread_datasets.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 14:56:56.741749 moveread_datasets-0.1.3/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      504 2024-04-25 14:56:56.741749 moveread_datasets-0.1.3/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       33 2024-04-24 09:15:05.000000 moveread_datasets-0.1.3/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      549 2024-04-25 14:56:52.000000 moveread_datasets-0.1.3/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-25 14:56:56.741749 moveread_datasets-0.1.3/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 14:56:56.731749 moveread_datasets-0.1.3/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 14:56:56.731749 moveread_datasets-0.1.3/src/moveread/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 14:56:56.731749 moveread_datasets-0.1.3/src/moveread/datasets/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      112 2024-04-25 05:56:30.000000 moveread_datasets-0.1.3/src/moveread/datasets/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1228 2024-04-25 14:51:26.000000 moveread_datasets-0.1.3/src/moveread/datasets/main.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 14:56:56.731749 moveread_datasets-0.1.3/src/moveread_datasets.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      504 2024-04-25 14:56:56.000000 moveread_datasets-0.1.3/src/moveread_datasets.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      312 2024-04-25 14:56:56.000000 moveread_datasets-0.1.3/src/moveread_datasets.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-25 14:56:56.000000 moveread_datasets-0.1.3/src/moveread_datasets.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       61 2024-04-25 14:56:56.000000 moveread_datasets-0.1.3/src/moveread_datasets.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        9 2024-04-25 14:56:56.000000 moveread_datasets-0.1.3/src/moveread_datasets.egg-info/top_level.txt
```

### Comparing `moveread_datasets-0.1.2/pyproject.toml` & `moveread_datasets-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "moveread-datasets"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
   {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "Datasets storage API for Moveread"
 dependencies = [
   "kv-api", "kv-fs", "typing-extensions"
 ]
```

### Comparing `moveread_datasets-0.1.2/src/moveread/datasets/main.py` & `moveread_datasets-0.1.3/src/moveread/datasets/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from dataclasses import dataclass
 from pydantic import BaseModel
 from haskellian import either as E, promise as P
 from kv.api import KV
 from kv.fs import FilesystemKV
 import tf_ocr as ocr
 
-Source = Literal['llobregat23', 'original-train', 'original-test', 'original-val']
+Source = Literal['llobregat23', 'original-train', 'original-test', 'original-val'] | str
 
 class Dataset(BaseModel):
   file: str
   source: Source
 
 @dataclass
 class DatasetsAPI:
@@ -27,12 +27,13 @@
       data=FilesystemKV[bytes](os.path.join(path, 'data'))
     )
   
   @P.lift
   async def readall(self) -> Sequence[tuple[str, Dataset]]:
     return await self.meta.items().map(E.unsafe).sync()
   
-  def load(self, datasetIds: Iterable[str], **params: Unpack[ocr.ReadParams]) -> ocr.Dataset:
+  async def load(self, datasetIds: Iterable[str], **params: Unpack[ocr.ReadParams]):
+    datasets = await P.all([self.meta.read(id).then(E.unsafe) for id in datasetIds])
     params['compression'] = 'GZIP'
-    files = [self.data.url(id) for id in datasetIds]
+    files = [self.data.url(d.file) for d in datasets]
     return ocr.read_dataset(files, **params)
```


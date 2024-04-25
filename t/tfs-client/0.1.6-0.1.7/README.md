# Comparing `tmp/tfs_client-0.1.6.tar.gz` & `tmp/tfs_client-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tfs_client-0.1.6.tar", last modified: Mon Apr 15 18:37:43 2024, max compression
+gzip compressed data, was "tfs_client-0.1.7.tar", last modified: Thu Apr 18 13:00:20 2024, max compression
```

## Comparing `tfs_client-0.1.6.tar` & `tfs_client-0.1.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-15 18:37:43.502496 tfs_client-0.1.6/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      439 2024-04-15 18:37:43.502496 tfs_client-0.1.6/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      101 2024-03-15 10:11:13.000000 tfs_client-0.1.6/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      499 2024-04-15 18:37:40.000000 tfs_client-0.1.6/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-15 18:37:43.502496 tfs_client-0.1.6/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-15 18:37:43.502496 tfs_client-0.1.6/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-15 18:37:43.502496 tfs_client-0.1.6/src/tfs_client/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       78 2024-03-17 18:31:13.000000 tfs_client-0.1.6/src/tfs_client/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      761 2024-03-16 14:16:09.000000 tfs_client-0.1.6/src/tfs_client/http.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-15 18:37:43.502496 tfs_client-0.1.6/src/tfs_client/util/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       52 2024-03-16 14:17:28.000000 tfs_client-0.1.6/src/tfs_client/util/__init__.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-15 18:37:43.502496 tfs_client-0.1.6/src/tfs_client/util/cit_images/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       80 2024-03-16 14:18:51.000000 tfs_client-0.1.6/src/tfs_client/util/cit_images/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1498 2024-03-19 10:06:52.000000 tfs_client-0.1.6/src/tfs_client/util/cit_images/cit_images.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      734 2024-04-15 18:35:38.000000 tfs_client-0.1.6/src/tfs_client/util/postprocessing.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-15 18:37:43.502496 tfs_client-0.1.6/src/tfs_client.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      439 2024-04-15 18:37:43.000000 tfs_client-0.1.6/src/tfs_client.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      421 2024-04-15 18:37:43.000000 tfs_client-0.1.6/src/tfs_client.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-15 18:37:43.000000 tfs_client-0.1.6/src/tfs_client.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       40 2024-04-15 18:37:43.000000 tfs_client-0.1.6/src/tfs_client.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       11 2024-04-15 18:37:43.000000 tfs_client-0.1.6/src/tfs_client.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-18 13:00:20.432648 tfs_client-0.1.7/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      439 2024-04-18 13:00:20.432648 tfs_client-0.1.7/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      101 2024-03-15 10:11:13.000000 tfs_client-0.1.7/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      499 2024-04-18 13:00:17.000000 tfs_client-0.1.7/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-18 13:00:20.432648 tfs_client-0.1.7/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-18 13:00:20.422648 tfs_client-0.1.7/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-18 13:00:20.432648 tfs_client-0.1.7/src/tfs_client/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       78 2024-03-17 18:31:13.000000 tfs_client-0.1.7/src/tfs_client/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      813 2024-04-16 05:22:03.000000 tfs_client-0.1.7/src/tfs_client/http.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-18 13:00:20.432648 tfs_client-0.1.7/src/tfs_client/util/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       52 2024-03-16 14:17:28.000000 tfs_client-0.1.7/src/tfs_client/util/__init__.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-18 13:00:20.432648 tfs_client-0.1.7/src/tfs_client/util/cit_images/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       80 2024-03-16 14:18:51.000000 tfs_client-0.1.7/src/tfs_client/util/cit_images/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1496 2024-04-17 09:23:48.000000 tfs_client-0.1.7/src/tfs_client/util/cit_images/cit_images.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      731 2024-04-16 08:50:27.000000 tfs_client-0.1.7/src/tfs_client/util/postprocessing.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-18 13:00:20.432648 tfs_client-0.1.7/src/tfs_client.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      439 2024-04-18 13:00:20.000000 tfs_client-0.1.7/src/tfs_client.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      421 2024-04-18 13:00:20.000000 tfs_client-0.1.7/src/tfs_client.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-18 13:00:20.000000 tfs_client-0.1.7/src/tfs_client.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       40 2024-04-18 13:00:20.000000 tfs_client-0.1.7/src/tfs_client.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       11 2024-04-18 13:00:20.000000 tfs_client-0.1.7/src/tfs_client.egg-info/top_level.txt
```

### Comparing `tfs_client-0.1.6/src/tfs_client/http.py` & `tfs_client-0.1.7/src/tfs_client/http.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-from typing import TypedDict
+from typing import TypedDict, NotRequired
 from pydantic import BaseModel
 import aiohttp
 
 class SamplePreds(BaseModel):
   preds: list[str]
   logprobs: list[float]
 
 class TFSResponse(BaseModel):
   predictions: list[SamplePreds]
   
 class Params(TypedDict):
-  host: str
-  port: int
-  endpoint: str
+  host: NotRequired[str]
+  port: NotRequired[int]
+  endpoint: NotRequired[str]
   
 async def predict(b64imgs: list[str], host: str = 'http://localhost', port: int = 8501, endpoint: str = '/v1/models/ocr:predict') -> list[SamplePreds]:
   base = f'{host.strip("/")}:{port}'
   async with aiohttp.ClientSession(base) as session:
     req = session.post(endpoint, json={
       "signature_name": "serving_default",
       "instances": b64imgs
```

### Comparing `tfs_client-0.1.6/src/tfs_client/util/cit_images/cit_images.py` & `tfs_client-0.1.7/src/tfs_client/util/cit_images/cit_images.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 def read64(path: str) -> str:
   """Read an image as URL-safe base64"""
   with open(path, 'rb') as f:
     bytes = f.read()
     return base64.urlsafe_b64encode(bytes).decode()
   
-def box_path(player: int = 0, ply: int = 0, images_path: str = './images'):
+def box_path(player: int = 0, ply: int = 0, images_path: str = 'images'):
   """Box path (use with `cit images`)"""
   return os.path.join(images_path, 'boxes', f'boxes-{player}-{ply}.jpg')
 
 def read_boxes(players = range(2), plys = range(8), images_path: str = './images') -> list[tuple[str, ...]]:
   plys = list(plys)
   return [
     tuple(read64(box_path(player, ply, images_path)) for player in players)
```

### Comparing `tfs_client-0.1.6/src/tfs_client/util/postprocessing.py` & `tfs_client-0.1.7/src/tfs_client/util/postprocessing.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,11 +9,11 @@
     """Returns an array of shape `BATCH x PLAYERS x TOP_PREDS` of `(pred, logprob)`"""
     if len(b64_multibatch) == 0:
         return []
     num_players = len(b64_multibatch[0])
     flatbatch = list(hk.flatten(b64_multibatch))
     flatpreds = await predict(flatbatch, **params)
     return pipe(
-        hk.map(transpose, flatpreds),
+        map(transpose, flatpreds),
         hk.batch(num_players),
         list
     )
```


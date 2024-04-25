# Comparing `tmp/moveread-core-0.1.2.tar.gz` & `tmp/moveread_core-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moveread-core-0.1.2.tar", last modified: Sat Apr  6 17:03:14 2024, max compression
+gzip compressed data, was "moveread_core-0.1.3.tar", last modified: Thu Apr 25 05:46:36 2024, max compression
```

## Comparing `moveread-core-0.1.2.tar` & `moveread_core-0.1.3.tar`

### file list

```diff
@@ -1,26 +1,22 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-06 17:03:14.620519 moveread-core-0.1.2/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      460 2024-04-06 17:03:14.610520 moveread-core-0.1.2/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-05 13:38:22.000000 moveread-core-0.1.2/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      664 2024-04-06 17:03:12.000000 moveread-core-0.1.2/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-06 17:03:14.620519 moveread-core-0.1.2/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-06 17:03:14.610520 moveread-core-0.1.2/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-06 17:03:14.610520 moveread-core-0.1.2/src/moveread/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-06 17:03:14.610520 moveread-core-0.1.2/src/moveread/core/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      178 2024-04-05 13:38:22.000000 moveread-core-0.1.2/src/moveread/core/__init__.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-06 17:03:14.610520 moveread-core-0.1.2/src/moveread/core/api/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       24 2024-04-05 13:38:22.000000 moveread-core-0.1.2/src/moveread/core/api/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      750 2024-04-05 13:39:47.000000 moveread-core-0.1.2/src/moveread/core/api/api.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-06 17:03:14.610520 moveread-core-0.1.2/src/moveread/core/models/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      114 2024-04-05 13:38:22.000000 moveread-core-0.1.2/src/moveread/core/models/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      721 2024-04-05 13:42:16.000000 moveread-core-0.1.2/src/moveread/core/models/ids.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      656 2024-04-06 14:12:05.000000 moveread-core-0.1.2/src/moveread/core/models/models.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-06 17:03:14.610520 moveread-core-0.1.2/src/moveread/core/scripts/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        0 2024-04-06 16:57:02.000000 moveread-core-0.1.2/src/moveread/core/scripts/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      673 2024-04-06 17:00:06.000000 moveread-core-0.1.2/src/moveread/core/scripts/tsgen.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-06 17:03:14.610520 moveread-core-0.1.2/src/moveread_core.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      460 2024-04-06 17:03:14.000000 moveread-core-0.1.2/src/moveread_core.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      542 2024-04-06 17:03:14.000000 moveread-core-0.1.2/src/moveread_core.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-06 17:03:14.000000 moveread-core-0.1.2/src/moveread_core.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       73 2024-04-06 17:03:14.000000 moveread-core-0.1.2/src/moveread_core.egg-info/entry_points.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       57 2024-04-06 17:03:14.000000 moveread-core-0.1.2/src/moveread_core.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        9 2024-04-06 17:03:14.000000 moveread-core-0.1.2/src/moveread_core.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 05:46:36.344239 moveread_core-0.1.3/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      728 2024-04-25 05:46:36.344239 moveread_core-0.1.3/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      141 2024-04-25 05:39:05.000000 moveread_core-0.1.3/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      666 2024-04-25 05:46:34.000000 moveread_core-0.1.3/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-25 05:46:36.344239 moveread_core-0.1.3/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 05:46:36.344239 moveread_core-0.1.3/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 05:46:36.344239 moveread_core-0.1.3/src/moveread/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 05:46:36.344239 moveread_core-0.1.3/src/moveread/core/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      154 2024-04-21 17:19:59.000000 moveread_core-0.1.3/src/moveread/core/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      393 2024-04-21 18:22:43.000000 moveread_core-0.1.3/src/moveread/core/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      548 2024-04-25 05:23:56.000000 moveread_core-0.1.3/src/moveread/core/core.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1082 2024-04-10 15:22:00.000000 moveread_core-0.1.3/src/moveread/core/ids.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      721 2024-04-22 10:50:59.000000 moveread_core-0.1.3/src/moveread/core/local.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1226 2024-04-25 05:24:15.000000 moveread_core-0.1.3/src/moveread/core/models.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      746 2024-04-21 17:22:52.000000 moveread_core-0.1.3/src/moveread/core/tsgen.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 05:46:36.344239 moveread_core-0.1.3/src/moveread_core.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      728 2024-04-25 05:46:36.000000 moveread_core-0.1.3/src/moveread_core.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      466 2024-04-25 05:46:36.000000 moveread_core-0.1.3/src/moveread_core.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-25 05:46:36.000000 moveread_core-0.1.3/src/moveread_core.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       65 2024-04-25 05:46:36.000000 moveread_core-0.1.3/src/moveread_core.egg-info/entry_points.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      113 2024-04-25 05:46:36.000000 moveread_core-0.1.3/src/moveread_core.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        9 2024-04-25 05:46:36.000000 moveread_core-0.1.3/src/moveread_core.egg-info/top_level.txt
```

### Comparing `moveread-core-0.1.2/pyproject.toml` & `moveread_core-0.1.3/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,26 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "moveread-core"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
   {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "Moveread core models and API"
 dependencies = [
-  "pydantic", "kv-api", "haskellian-either"
+  "pydantic", "kv-api", "haskellian", "lazy-loader", "moveread-annotations"
 ]
 requires-python = ">=3.10"
 readme = {file="README.md", content-type="text/markdown"}
 
 [project.urls]
 repo = "https://github.com/moveread/python-core"
 
 [project.scripts]
-moveread-core-tsgen = "moveread.core.scripts.tsgen:main"
+moveread-core-tsgen = "moveread.core.tsgen:main"
 
 [project.optional-dependencies]
 ts-gen = ["quicktype-ts"]
-# test = [
-#   "pytest < 5.0.0",
-#   "pytest-cov[all]"
-# ]
+local = ["kv-fs", "kv-sqlite-sync"]
```

### Comparing `moveread-core-0.1.2/src/moveread/core/models/ids.py` & `moveread_core-0.1.3/src/moveread/core/ids.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,35 +1,44 @@
-from dataclasses import dataclass, asdict
+from dataclasses import dataclass
 
 @dataclass
 class GameID:
   gameId: str
 
   def playerId(self, player: int = 0) -> 'PlayerID':
-    return PlayerID(**asdict(self), player=player)
+    return PlayerID(gameId=self.gameId, player=player)
 
 @dataclass
 class PlayerID(GameID):
   player: int
 
   def sheetId(self, page: int = 0) -> 'SheetID':
-    return SheetID(**asdict(self), page=page)
+    return SheetID(gameId=self.gameId, player=self.player, page=page)
+  
+  def __str__(self):
+    return f'{self.gameId}-{self.player}'
 
 @dataclass
 class SheetID(PlayerID):
   page: int
 
   def imageId(self, version: int = 0) -> 'ImageID':
-    return ImageID(**asdict(self), version=version)
+    return ImageID(gameId=self.gameId, player=self.player, page=self.page, version=version)
+
+  def __str__(self):
+    return f'{self.gameId}-{self.player}-{self.page}'
 
 @dataclass
 class ImageID(SheetID):
   version: int = 0
 
   def boxId(self, idx: int) -> 'BoxID':
-    return BoxID(**asdict(self), idx=idx)
+    return BoxID(gameId=self.gameId, player=self.player, page=self.page, version=self.version, idx=idx)
+  
+  def __str__(self):
+    return f'{self.gameId}/{self.player}-{self.page}-{self.version}'
 
 @dataclass
-class BoxID(SheetID):
-  idx: int
+class BoxID(ImageID):
+  idx: int = 0
 
 ID = GameID | PlayerID | SheetID | ImageID | BoxID
```

### Comparing `moveread-core-0.1.2/src/moveread/core/scripts/tsgen.py` & `moveread_core-0.1.3/src/moveread/core/tsgen.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 import os
 from argparse import ArgumentParser
-from quicktype_ts import pydantic2typescript
-from moveread.core import Game
 
-def main():
-
-  parser = ArgumentParser()
-  parser.add_argument('--src-path', required=True)
-  args = parser.parse_args()
-  base = os.path.join(args.src_path, 'src')
+def run(base: str):
+  from quicktype_ts import pydantic2typescript
+  from moveread.core import Game
 
   os.makedirs(base, exist_ok=True)
   code = pydantic2typescript(Game)
 
   models = os.path.join(base, 'models.ts')
   print(f'Writing {models}...')
   with open(models, 'wb') as f:
     f.write(code)
 
   index = os.path.join(base, 'index.ts')
   print(f'Writing {index}...')
   with open(index, 'w') as f:
     f.write("export * from './models.js'\n")
 
-  print('Generated code successfully!')
+  print('Generated code successfully!')
+
+def main():
+  parser = ArgumentParser()
+  parser.add_argument('--src-path', required=True)
+  args = parser.parse_args()
+  base = os.path.join(args.src_path, 'src')
+  run(base)
+
+if __name__ == '__main__':
+  main()
```


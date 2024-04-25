# Comparing `tmp/moveread-annotations-0.1.3.tar.gz` & `tmp/moveread_annotations-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moveread-annotations-0.1.3.tar", last modified: Sat Apr  6 17:11:26 2024, max compression
+gzip compressed data, was "moveread_annotations-0.1.4.tar", last modified: Thu Apr 25 05:46:02 2024, max compression
```

## Comparing `moveread-annotations-0.1.3.tar` & `moveread_annotations-0.1.4.tar`

### file list

```diff
@@ -1,31 +1,22 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-06 17:11:26.840513 moveread-annotations-0.1.3/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      866 2024-04-06 17:11:26.840513 moveread-annotations-0.1.3/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      355 2024-04-05 16:24:36.000000 moveread-annotations-0.1.3/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      686 2024-04-06 17:11:24.000000 moveread-annotations-0.1.3/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-06 17:11:26.840513 moveread-annotations-0.1.3/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-06 17:11:26.830513 moveread-annotations-0.1.3/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-06 17:11:26.830513 moveread-annotations-0.1.3/src/moveread/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-06 17:11:26.830513 moveread-annotations-0.1.3/src/moveread/annotations/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       86 2024-04-05 15:49:41.000000 moveread-annotations-0.1.3/src/moveread/annotations/__init__.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-06 17:11:26.830513 moveread-annotations-0.1.3/src/moveread/annotations/games/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       82 2024-04-05 18:52:46.000000 moveread-annotations-0.1.3/src/moveread/annotations/games/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1676 2024-04-06 14:11:45.000000 moveread-annotations-0.1.3/src/moveread/annotations/games/games.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-06 17:11:26.830513 moveread-annotations-0.1.3/src/moveread/annotations/images/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       77 2024-04-05 16:22:04.000000 moveread-annotations-0.1.3/src/moveread/annotations/images/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      938 2024-04-06 14:26:54.000000 moveread-annotations-0.1.3/src/moveread/annotations/images/images.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-06 17:11:26.830513 moveread-annotations-0.1.3/src/moveread/annotations/players/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      142 2024-04-05 19:04:45.000000 moveread-annotations-0.1.3/src/moveread/annotations/players/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      769 2024-04-06 14:26:36.000000 moveread-annotations-0.1.3/src/moveread/annotations/players/players.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-06 17:11:26.830513 moveread-annotations-0.1.3/src/moveread/annotations/scripts/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        0 2024-04-06 17:03:55.000000 moveread-annotations-0.1.3/src/moveread/annotations/scripts/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1212 2024-04-06 17:09:13.000000 moveread-annotations-0.1.3/src/moveread/annotations/scripts/tsgen.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-06 17:11:26.840513 moveread-annotations-0.1.3/src/moveread/annotations/sheets/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       62 2024-04-05 16:22:22.000000 moveread-annotations-0.1.3/src/moveread/annotations/sheets/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      839 2024-04-06 14:26:45.000000 moveread-annotations-0.1.3/src/moveread/annotations/sheets/sheets.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-06 17:11:26.840513 moveread-annotations-0.1.3/src/moveread_annotations.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      866 2024-04-06 17:11:26.000000 moveread-annotations-0.1.3/src/moveread_annotations.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      782 2024-04-06 17:11:26.000000 moveread-annotations-0.1.3/src/moveread_annotations.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-06 17:11:26.000000 moveread-annotations-0.1.3/src/moveread_annotations.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       87 2024-04-06 17:11:26.000000 moveread-annotations-0.1.3/src/moveread_annotations.egg-info/entry_points.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       97 2024-04-06 17:11:26.000000 moveread-annotations-0.1.3/src/moveread_annotations.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        9 2024-04-06 17:11:26.000000 moveread-annotations-0.1.3/src/moveread_annotations.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 05:46:02.714239 moveread_annotations-0.1.4/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      606 2024-04-25 05:46:02.714239 moveread_annotations-0.1.4/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       67 2024-04-09 05:54:21.000000 moveread_annotations-0.1.4/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      695 2024-04-25 05:46:00.000000 moveread_annotations-0.1.4/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-25 05:46:02.714239 moveread_annotations-0.1.4/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 05:46:02.704239 moveread_annotations-0.1.4/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 05:46:02.704239 moveread_annotations-0.1.4/src/moveread/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 05:46:02.704239 moveread_annotations-0.1.4/src/moveread/annotations/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      171 2024-04-21 17:02:02.000000 moveread_annotations-0.1.4/src/moveread/annotations/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      470 2024-04-22 10:28:54.000000 moveread_annotations-0.1.4/src/moveread/annotations/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      784 2024-04-23 18:14:46.000000 moveread_annotations-0.1.4/src/moveread/annotations/games.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      431 2024-04-25 05:37:35.000000 moveread_annotations-0.1.4/src/moveread/annotations/images.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      202 2024-04-22 10:28:26.000000 moveread_annotations-0.1.4/src/moveread/annotations/players.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      184 2024-04-21 16:57:10.000000 moveread_annotations-0.1.4/src/moveread/annotations/sheets.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1177 2024-04-21 17:04:06.000000 moveread_annotations-0.1.4/src/moveread/annotations/tsgen.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 05:46:02.714239 moveread_annotations-0.1.4/src/moveread_annotations.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      606 2024-04-25 05:46:02.000000 moveread_annotations-0.1.4/src/moveread_annotations.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      563 2024-04-25 05:46:02.000000 moveread_annotations-0.1.4/src/moveread_annotations.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-25 05:46:02.000000 moveread_annotations-0.1.4/src/moveread_annotations.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       79 2024-04-25 05:46:02.000000 moveread_annotations-0.1.4/src/moveread_annotations.egg-info/entry_points.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      111 2024-04-25 05:46:02.000000 moveread_annotations-0.1.4/src/moveread_annotations.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        9 2024-04-25 05:46:02.000000 moveread_annotations-0.1.4/src/moveread_annotations.egg-info/top_level.txt
```

### Comparing `moveread-annotations-0.1.3/pyproject.toml` & `moveread_annotations-0.1.4/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "moveread-annotations"
-version = "0.1.3"
+version = "0.1.4"
 authors = [
   {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "Annotation schemas for the Moveread Core"
 dependencies = [
-  "pydantic", "haskellian-either",
-  "moveread-labels", "moveread-boxes", "moveread-errors"
+  "pydantic", "robust-extraction", "lazy-loader",
+  "moveread-labels", "moveread-boxes", "scoresheet-models"
 ]
 requires-python = ">=3.10"
 readme = {file="README.md", content-type="text/markdown"}
 
 [project.urls]
 repo = "https://github.com/moveread/python-core"
 
 [project.scripts]
-moveread-annotations-tsgen = "moveread.annotations.scripts.tsgen:main"
+moveread-annotations-tsgen = "moveread.annotations.tsgen:main"
 
 [project.optional-dependencies]
 ts-gen = ["quicktype-ts"]
```

### Comparing `moveread-annotations-0.1.3/src/moveread/annotations/scripts/tsgen.py` & `moveread_annotations-0.1.4/src/moveread/annotations/tsgen.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,13 @@
-import os
 from argparse import ArgumentParser
-from quicktype_ts import pydantic2typescript
-from moveread.annotations.games import GameMeta
-from moveread.annotations.players import PlayerMeta
-from moveread.annotations.sheets import SheetMeta
-from moveread.annotations.images import ImageMeta
 
-
-def main():
-
-  parser = ArgumentParser()
-  parser.add_argument('--src-path', required=True)
-  args = parser.parse_args()
-  base = os.path.join(args.src_path, 'src')
+def run(base: str):
+  import os
+  from quicktype_ts import pydantic2typescript
+  from moveread.annotations import GameMeta, PlayerMeta, SheetMeta, ImageMeta
 
   models = [('games', GameMeta), ('players', PlayerMeta), ('sheets', SheetMeta), ('images', ImageMeta)]
 
   os.makedirs(base, exist_ok=True)
   for filename, model in models:
     path = os.path.join(base, f'{filename}.ts')
     print(f'Generating {path}...')
@@ -24,17 +15,28 @@
     with open(path, 'wb') as f:
       f.write(code)
 
   # fix Rectangle
   images = os.path.join(base, 'images.ts')
   os.system("sed -i '/^export type Rectangle/,/}/d' " + images) # delete Rectangle
   rect = """
-  // hand-generated as quicktype treats `[number, number]` as `any[]`
+  // hand-generated since quicktype treats `[number, number]` as `any[]`
   export type Rectangle = {
     size: [number, number]
     tl: [number, number]
   }
   """
   with open(images, 'a') as f:
     f.write(rect)
 
-  print('Successfully generated code!')
+  print('Successfully generated code!')
+
+def main():
+  parser = ArgumentParser()
+  parser.add_argument('--src-path', required=True)
+  args = parser.parse_args()
+  import os
+  base = os.path.join(args.src_path, 'src')
+  run(base)
+
+if __name__ == '__main__':
+  main()
```

### Comparing `moveread-annotations-0.1.3/src/moveread_annotations.egg-info/SOURCES.txt` & `moveread_annotations-0.1.4/src/moveread_annotations.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,15 @@
 README.md
 pyproject.toml
 src/moveread/annotations/__init__.py
-src/moveread/annotations/games/__init__.py
-src/moveread/annotations/games/games.py
-src/moveread/annotations/images/__init__.py
-src/moveread/annotations/images/images.py
-src/moveread/annotations/players/__init__.py
-src/moveread/annotations/players/players.py
-src/moveread/annotations/scripts/__init__.py
-src/moveread/annotations/scripts/tsgen.py
-src/moveread/annotations/sheets/__init__.py
-src/moveread/annotations/sheets/sheets.py
+src/moveread/annotations/__init__.pyi
+src/moveread/annotations/games.py
+src/moveread/annotations/images.py
+src/moveread/annotations/players.py
+src/moveread/annotations/sheets.py
+src/moveread/annotations/tsgen.py
 src/moveread_annotations.egg-info/PKG-INFO
 src/moveread_annotations.egg-info/SOURCES.txt
 src/moveread_annotations.egg-info/dependency_links.txt
 src/moveread_annotations.egg-info/entry_points.txt
 src/moveread_annotations.egg-info/requires.txt
 src/moveread_annotations.egg-info/top_level.txt
```


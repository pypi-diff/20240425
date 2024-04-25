# Comparing `tmp/tmdbapis-1.2.7.tar.gz` & `tmp/tmdbapis-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tmdbapis-1.2.7.tar", last modified: Fri Feb 23 19:20:47 2024, max compression
+gzip compressed data, was "tmdbapis-1.2.9.tar", last modified: Thu Mar 28 15:29:22 2024, max compression
```

## Comparing `tmdbapis-1.2.7.tar` & `tmdbapis-1.2.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 19:20:47.156390 tmdbapis-1.2.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-02-23 19:20:38.000000 tmdbapis-1.2.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     9643 2024-02-23 19:20:47.156390 tmdbapis-1.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8580 2024-02-23 19:20:38.000000 tmdbapis-1.2.7/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-23 19:20:47.156390 tmdbapis-1.2.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-02-23 19:20:38.000000 tmdbapis-1.2.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 19:20:47.152390 tmdbapis-1.2.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    21719 2024-02-23 19:20:38.000000 tmdbapis-1.2.7/tests/test_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 19:20:47.152390 tmdbapis-1.2.7/tmdbapis/
--rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-02-23 19:20:38.000000 tmdbapis-1.2.7/tmdbapis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   145200 2024-02-23 19:20:38.000000 tmdbapis-1.2.7/tmdbapis/api3.py
--rw-r--r--   0 runner    (1001) docker     (127)    23774 2024-02-23 19:20:38.000000 tmdbapis-1.2.7/tmdbapis/api4.py
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-02-23 19:20:38.000000 tmdbapis-1.2.7/tmdbapis/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 19:20:47.156390 tmdbapis-1.2.7/tmdbapis/objs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 19:20:38.000000 tmdbapis-1.2.7/tmdbapis/objs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3362 2024-02-23 19:20:38.000000 tmdbapis-1.2.7/tmdbapis/objs/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3243 2024-02-23 19:20:38.000000 tmdbapis-1.2.7/tmdbapis/objs/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-02-23 19:20:38.000000 tmdbapis-1.2.7/tmdbapis/objs/mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)    39050 2024-02-23 19:20:38.000000 tmdbapis-1.2.7/tmdbapis/objs/pagination.py
--rw-r--r--   0 runner    (1001) docker     (127)    58341 2024-02-23 19:20:38.000000 tmdbapis-1.2.7/tmdbapis/objs/reload.py
--rw-r--r--   0 runner    (1001) docker     (127)    15589 2024-02-23 19:20:38.000000 tmdbapis-1.2.7/tmdbapis/objs/simple.py
--rw-r--r--   0 runner    (1001) docker     (127)    79861 2024-02-23 19:20:38.000000 tmdbapis-1.2.7/tmdbapis/tmdb.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 19:20:47.156390 tmdbapis-1.2.7/tmdbapis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9643 2024-02-23 19:20:47.000000 tmdbapis-1.2.7/tmdbapis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-02-23 19:20:47.000000 tmdbapis-1.2.7/tmdbapis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-23 19:20:47.000000 tmdbapis-1.2.7/tmdbapis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-02-23 19:20:47.000000 tmdbapis-1.2.7/tmdbapis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-02-23 19:20:47.000000 tmdbapis-1.2.7/tmdbapis.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:29:22.934346 tmdbapis-1.2.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-03-28 15:28:57.000000 tmdbapis-1.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9643 2024-03-28 15:29:22.934346 tmdbapis-1.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8580 2024-03-28 15:28:57.000000 tmdbapis-1.2.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-28 15:29:22.934346 tmdbapis-1.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-03-28 15:28:57.000000 tmdbapis-1.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:29:22.930346 tmdbapis-1.2.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    21719 2024-03-28 15:28:57.000000 tmdbapis-1.2.9/tests/test_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:29:22.930346 tmdbapis-1.2.9/tmdbapis/
+-rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-03-28 15:28:57.000000 tmdbapis-1.2.9/tmdbapis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   145200 2024-03-28 15:28:57.000000 tmdbapis-1.2.9/tmdbapis/api3.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23774 2024-03-28 15:28:57.000000 tmdbapis-1.2.9/tmdbapis/api4.py
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-03-28 15:28:57.000000 tmdbapis-1.2.9/tmdbapis/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:29:22.930346 tmdbapis-1.2.9/tmdbapis/objs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 15:28:57.000000 tmdbapis-1.2.9/tmdbapis/objs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3362 2024-03-28 15:28:57.000000 tmdbapis-1.2.9/tmdbapis/objs/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3243 2024-03-28 15:28:57.000000 tmdbapis-1.2.9/tmdbapis/objs/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-03-28 15:28:57.000000 tmdbapis-1.2.9/tmdbapis/objs/mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39050 2024-03-28 15:28:57.000000 tmdbapis-1.2.9/tmdbapis/objs/pagination.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58528 2024-03-28 15:28:57.000000 tmdbapis-1.2.9/tmdbapis/objs/reload.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15589 2024-03-28 15:28:57.000000 tmdbapis-1.2.9/tmdbapis/objs/simple.py
+-rw-r--r--   0 runner    (1001) docker     (127)    79861 2024-03-28 15:28:57.000000 tmdbapis-1.2.9/tmdbapis/tmdb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:29:22.934346 tmdbapis-1.2.9/tmdbapis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9643 2024-03-28 15:29:22.000000 tmdbapis-1.2.9/tmdbapis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-03-28 15:29:22.000000 tmdbapis-1.2.9/tmdbapis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 15:29:22.000000 tmdbapis-1.2.9/tmdbapis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-28 15:29:22.000000 tmdbapis-1.2.9/tmdbapis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-28 15:29:22.000000 tmdbapis-1.2.9/tmdbapis.egg-info/top_level.txt
```

### Comparing `tmdbapis-1.2.7/LICENSE` & `tmdbapis-1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `tmdbapis-1.2.7/PKG-INFO` & `tmdbapis-1.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tmdbapis
-Version: 1.2.7
+Version: 1.2.9
 Summary: A lightweight Python library for The V3 and V4 TMDb APIs.
 Home-page: https://github.com/meisnate12/TMDbAPIs
 Author: Nathan Taggart
 Author-email: meisnate12@gmail.com
 License: MIT License
 Project-URL: Documentation, https://tmdbapis.metamanager.wiki
 Project-URL: Funding, https://github.com/sponsors/meisnate12
```

### Comparing `tmdbapis-1.2.7/README.rst` & `tmdbapis-1.2.9/README.rst`

 * *Files identical despite different names*

### Comparing `tmdbapis-1.2.7/setup.py` & `tmdbapis-1.2.9/setup.py`

 * *Files identical despite different names*

### Comparing `tmdbapis-1.2.7/tests/test_api.py` & `tmdbapis-1.2.9/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `tmdbapis-1.2.7/tmdbapis/__init__.py` & `tmdbapis-1.2.9/tmdbapis/__init__.py`

 * *Files identical despite different names*

### Comparing `tmdbapis-1.2.7/tmdbapis/api3.py` & `tmdbapis-1.2.9/tmdbapis/api3.py`

 * *Files identical despite different names*

### Comparing `tmdbapis-1.2.7/tmdbapis/api4.py` & `tmdbapis-1.2.9/tmdbapis/api4.py`

 * *Files identical despite different names*

### Comparing `tmdbapis-1.2.7/tmdbapis/exceptions.py` & `tmdbapis-1.2.9/tmdbapis/exceptions.py`

 * *Files identical despite different names*

### Comparing `tmdbapis-1.2.7/tmdbapis/objs/base.py` & `tmdbapis-1.2.9/tmdbapis/objs/base.py`

 * *Files identical despite different names*

### Comparing `tmdbapis-1.2.7/tmdbapis/objs/image.py` & `tmdbapis-1.2.9/tmdbapis/objs/image.py`

 * *Files identical despite different names*

### Comparing `tmdbapis-1.2.7/tmdbapis/objs/mixin.py` & `tmdbapis-1.2.9/tmdbapis/objs/mixin.py`

 * *Files identical despite different names*

### Comparing `tmdbapis-1.2.7/tmdbapis/objs/pagination.py` & `tmdbapis-1.2.9/tmdbapis/objs/pagination.py`

 * *Files identical despite different names*

### Comparing `tmdbapis-1.2.7/tmdbapis/objs/reload.py` & `tmdbapis-1.2.9/tmdbapis/objs/reload.py`

 * *Files 0% similar despite different names*

```diff
@@ -810,14 +810,15 @@
             season_number (int): Season Number.
             title (str): alias of name.
             translations (List[:class:`~tmdbapis.objs.simple.Translation`]): List of Translations for the Season.
             tv_id (int): TMDb TV Show ID the contains the Season.
             tvdb_id (int): TVDB ID of the Season.
             tvrage_id (int): TV Rage ID of the Season.
             videos (List[:class:`~tmdbapis.objs.simple.Video`]): List of Videos associated with the Season.
+            vote_average (float): Vote Average for the TV Season.
     """
 
     def __init__(self, tmdb, data, tv_id, load=False, partial=False):
         self._tv_id = tv_id
         super().__init__(tmdb, data=data, load=load, partial=partial)
 
     def _load(self, data, partial=False):
@@ -839,18 +840,19 @@
         self.posters = self._parse(attrs=["images", "posters"], value_type="poster", is_list=True)
         self.season_number = self._parse(attrs="season_number", value_type="int")
         self.title = self.name
         self.translations = self._parse(attrs=["translations", "translations"], value_type="translation", is_list=True)
         self.tvdb_id = self._parse(attrs=["external_ids", "tvdb_id"], value_type="int")
         self.tvrage_id = self._parse(attrs=["external_ids", "tvrage_id"], value_type="int")
         self.videos = self._parse(attrs=["videos", "results"], value_type="video", is_list=True)
+        self.vote_average = self._parse(attrs="vote_average", value_type="float")
         self._finish(self.name)
 
     def _append_str(self):
-        return "images,translations"
+        return "images,external_ids,translations,aggregate_credits,credits"
 
     def _full_load(self, partial=None):
         return self._api.tv_seasons_get_details(
             self.tv_id, self.season_number,
             language=self._tmdb.language,
             include_image_language=self._tmdb._include_language,
             include_video_language=self._tmdb._include_language,
```

### Comparing `tmdbapis-1.2.7/tmdbapis/objs/simple.py` & `tmdbapis-1.2.9/tmdbapis/objs/simple.py`

 * *Files identical despite different names*

### Comparing `tmdbapis-1.2.7/tmdbapis/tmdb.py` & `tmdbapis-1.2.9/tmdbapis/tmdb.py`

 * *Files identical despite different names*

### Comparing `tmdbapis-1.2.7/tmdbapis.egg-info/PKG-INFO` & `tmdbapis-1.2.9/tmdbapis.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tmdbapis
-Version: 1.2.7
+Version: 1.2.9
 Summary: A lightweight Python library for The V3 and V4 TMDb APIs.
 Home-page: https://github.com/meisnate12/TMDbAPIs
 Author: Nathan Taggart
 Author-email: meisnate12@gmail.com
 License: MIT License
 Project-URL: Documentation, https://tmdbapis.metamanager.wiki
 Project-URL: Funding, https://github.com/sponsors/meisnate12
```


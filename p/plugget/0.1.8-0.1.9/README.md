# Comparing `tmp/plugget-0.1.8.tar.gz` & `tmp/plugget-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plugget-0.1.8.tar", last modified: Mon Jan 15 10:38:47 2024, max compression
+gzip compressed data, was "plugget-0.1.9.tar", last modified: Tue Jan 16 10:29:15 2024, max compression
```

## Comparing `plugget-0.1.8.tar` & `plugget-0.1.9.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 10:38:47.219313 plugget-0.1.8/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 10:38:47.207313 plugget-0.1.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 10:38:47.211313 plugget-0.1.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-01-15 10:38:38.000000 plugget-0.1.8/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3077 2024-01-15 10:38:38.000000 plugget-0.1.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     4036 2024-01-15 10:38:47.219313 plugget-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3426 2024-01-15 10:38:38.000000 plugget-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 10:38:47.211313 plugget-0.1.8/plugget/
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-01-15 10:38:38.000000 plugget-0.1.8/plugget/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-01-15 10:38:38.000000 plugget-0.1.8/plugget/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 10:38:47.215313 plugget-0.1.8/plugget/actions/
--rw-r--r--   0 runner    (1001) docker     (127)     2703 2024-01-15 10:38:38.000000 plugget-0.1.8/plugget/actions/_copy_files.py
--rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-01-15 10:38:38.000000 plugget-0.1.8/plugget/actions/_max3ds_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-01-15 10:38:38.000000 plugget-0.1.8/plugget/actions/_maya_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4526 2024-01-15 10:38:38.000000 plugget-0.1.8/plugget/actions/_requirements.py
--rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-01-15 10:38:38.000000 plugget-0.1.8/plugget/actions/_template.py
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-01-15 10:38:38.000000 plugget-0.1.8/plugget/actions/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4658 2024-01-15 10:38:38.000000 plugget-0.1.8/plugget/actions/blender_addon.py
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-01-15 10:38:38.000000 plugget-0.1.8/plugget/actions/blender_requirements.py
--rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-01-15 10:38:38.000000 plugget-0.1.8/plugget/actions/krita_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-01-15 10:38:38.000000 plugget-0.1.8/plugget/actions/krita_requirements.py
--rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-01-15 10:38:38.000000 plugget-0.1.8/plugget/actions/max3ds_macroscript.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-01-15 10:38:38.000000 plugget-0.1.8/plugget/actions/max3ds_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-01-15 10:38:38.000000 plugget-0.1.8/plugget/actions/max3ds_requirements.py
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-01-15 10:38:38.000000 plugget-0.1.8/plugget/actions/maya_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-01-15 10:38:38.000000 plugget-0.1.8/plugget/actions/maya_requirements.py
--rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-01-15 10:38:38.000000 plugget-0.1.8/plugget/actions/substance_painter_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-01-15 10:38:38.000000 plugget-0.1.8/plugget/actions/substance_painter_requirements.py
--rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-01-15 10:38:38.000000 plugget-0.1.8/plugget/actions/unreal_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2868 2024-01-15 10:38:38.000000 plugget-0.1.8/plugget/actions/unreal_requirements.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 10:38:47.215313 plugget-0.1.8/plugget/commands/
--rw-r--r--   0 runner    (1001) docker     (127)    17009 2024-01-15 10:38:38.000000 plugget-0.1.8/plugget/commands/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 10:38:47.215313 plugget-0.1.8/plugget/data/
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-01-15 10:38:38.000000 plugget-0.1.8/plugget/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20398 2024-01-15 10:38:38.000000 plugget-0.1.8/plugget/data/package.py
--rw-r--r--   0 runner    (1001) docker     (127)     4231 2024-01-15 10:38:38.000000 plugget-0.1.8/plugget/data/packages_meta.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 10:38:47.219313 plugget-0.1.8/plugget/github/
--rw-r--r--   0 runner    (1001) docker     (127)     2773 2024-01-15 10:38:38.000000 plugget-0.1.8/plugget/github/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-01-15 10:38:38.000000 plugget-0.1.8/plugget/github/async.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 10:38:47.219313 plugget-0.1.8/plugget/gumroad/
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-01-15 10:38:38.000000 plugget-0.1.8/plugget/gumroad/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 10:38:47.219313 plugget-0.1.8/plugget/resources/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-01-15 10:38:38.000000 plugget-0.1.8/plugget/resources/config.json
--rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-01-15 10:38:38.000000 plugget-0.1.8/plugget/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 10:38:47.219313 plugget-0.1.8/plugget.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4036 2024-01-15 10:38:47.000000 plugget-0.1.8/plugget.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-01-15 10:38:47.000000 plugget-0.1.8/plugget.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-15 10:38:47.000000 plugget-0.1.8/plugget.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-01-15 10:38:47.000000 plugget-0.1.8/plugget.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-01-15 10:38:47.000000 plugget-0.1.8/plugget.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      981 2024-01-15 10:38:38.000000 plugget-0.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-01-15 10:38:38.000000 plugget-0.1.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-15 10:38:47.219313 plugget-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-01-15 10:38:38.000000 plugget-0.1.8/testcode.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 10:29:15.970225 plugget-0.1.9/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 10:29:15.962225 plugget-0.1.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 10:29:15.962225 plugget-0.1.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-01-16 10:29:06.000000 plugget-0.1.9/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3077 2024-01-16 10:29:06.000000 plugget-0.1.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     4036 2024-01-16 10:29:15.970225 plugget-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3426 2024-01-16 10:29:06.000000 plugget-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 10:29:15.966225 plugget-0.1.9/plugget/
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-01-16 10:29:06.000000 plugget-0.1.9/plugget/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-01-16 10:29:06.000000 plugget-0.1.9/plugget/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 10:29:15.970225 plugget-0.1.9/plugget/actions/
+-rw-r--r--   0 runner    (1001) docker     (127)     2703 2024-01-16 10:29:06.000000 plugget-0.1.9/plugget/actions/_copy_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-01-16 10:29:06.000000 plugget-0.1.9/plugget/actions/_max3ds_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-01-16 10:29:06.000000 plugget-0.1.9/plugget/actions/_maya_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4526 2024-01-16 10:29:06.000000 plugget-0.1.9/plugget/actions/_requirements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-01-16 10:29:06.000000 plugget-0.1.9/plugget/actions/_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-01-16 10:29:06.000000 plugget-0.1.9/plugget/actions/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4658 2024-01-16 10:29:06.000000 plugget-0.1.9/plugget/actions/blender_addon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-01-16 10:29:06.000000 plugget-0.1.9/plugget/actions/blender_requirements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-01-16 10:29:06.000000 plugget-0.1.9/plugget/actions/krita_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-01-16 10:29:06.000000 plugget-0.1.9/plugget/actions/krita_requirements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-01-16 10:29:06.000000 plugget-0.1.9/plugget/actions/max3ds_macroscript.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-01-16 10:29:06.000000 plugget-0.1.9/plugget/actions/max3ds_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-01-16 10:29:06.000000 plugget-0.1.9/plugget/actions/max3ds_requirements.py
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-01-16 10:29:06.000000 plugget-0.1.9/plugget/actions/maya_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-01-16 10:29:06.000000 plugget-0.1.9/plugget/actions/maya_requirements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-01-16 10:29:06.000000 plugget-0.1.9/plugget/actions/substance_painter_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-01-16 10:29:06.000000 plugget-0.1.9/plugget/actions/substance_painter_requirements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-01-16 10:29:06.000000 plugget-0.1.9/plugget/actions/unreal_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2868 2024-01-16 10:29:06.000000 plugget-0.1.9/plugget/actions/unreal_requirements.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 10:29:15.970225 plugget-0.1.9/plugget/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)    17009 2024-01-16 10:29:06.000000 plugget-0.1.9/plugget/commands/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 10:29:15.970225 plugget-0.1.9/plugget/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-01-16 10:29:06.000000 plugget-0.1.9/plugget/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20398 2024-01-16 10:29:06.000000 plugget-0.1.9/plugget/data/package.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4231 2024-01-16 10:29:06.000000 plugget-0.1.9/plugget/data/packages_meta.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 10:29:15.970225 plugget-0.1.9/plugget/github/
+-rw-r--r--   0 runner    (1001) docker     (127)     2773 2024-01-16 10:29:06.000000 plugget-0.1.9/plugget/github/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-01-16 10:29:06.000000 plugget-0.1.9/plugget/github/async.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 10:29:15.970225 plugget-0.1.9/plugget/gumroad/
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-01-16 10:29:06.000000 plugget-0.1.9/plugget/gumroad/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 10:29:15.970225 plugget-0.1.9/plugget/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-01-16 10:29:06.000000 plugget-0.1.9/plugget/resources/config.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-01-16 10:29:06.000000 plugget-0.1.9/plugget/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 10:29:15.970225 plugget-0.1.9/plugget.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4036 2024-01-16 10:29:15.000000 plugget-0.1.9/plugget.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-01-16 10:29:15.000000 plugget-0.1.9/plugget.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-16 10:29:15.000000 plugget-0.1.9/plugget.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-01-16 10:29:15.000000 plugget-0.1.9/plugget.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-01-16 10:29:15.000000 plugget-0.1.9/plugget.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      981 2024-01-16 10:29:06.000000 plugget-0.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-01-16 10:29:06.000000 plugget-0.1.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-16 10:29:15.970225 plugget-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-01-16 10:29:06.000000 plugget-0.1.9/testcode.py
```

### Comparing `plugget-0.1.8/.github/workflows/python-publish.yml` & `plugget-0.1.9/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `plugget-0.1.8/.gitignore` & `plugget-0.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `plugget-0.1.8/PKG-INFO` & `plugget-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plugget
-Version: 0.1.8
+Version: 0.1.9
 Summary: a package manager to install packages in your app
 Author: Hannes Delbeke
 Project-URL: Homepage, https://github.com/plugget/plugget
 Project-URL: Source, https://github.com/plugget/plugget
 Keywords: plugin,addon,add-on,extension,package,manager,resource,studio,dcc,app,application,pipeline,blender,krita,max
 Classifier: Programming Language :: Python :: 3.7
 Requires-Python: >=3.4
```

### Comparing `plugget-0.1.8/README.md` & `plugget-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `plugget-0.1.8/plugget/actions/_copy_files.py` & `plugget-0.1.9/plugget/actions/_copy_files.py`

 * *Files identical despite different names*

### Comparing `plugget-0.1.8/plugget/actions/_max3ds_utils.py` & `plugget-0.1.9/plugget/actions/_max3ds_utils.py`

 * *Files identical despite different names*

### Comparing `plugget-0.1.8/plugget/actions/_maya_utils.py` & `plugget-0.1.9/plugget/actions/_maya_utils.py`

 * *Files identical despite different names*

### Comparing `plugget-0.1.8/plugget/actions/_requirements.py` & `plugget-0.1.9/plugget/actions/_requirements.py`

 * *Files identical despite different names*

### Comparing `plugget-0.1.8/plugget/actions/_template.py` & `plugget-0.1.9/plugget/actions/_template.py`

 * *Files identical despite different names*

### Comparing `plugget-0.1.8/plugget/actions/_utils.py` & `plugget-0.1.9/plugget/actions/_utils.py`

 * *Files identical despite different names*

### Comparing `plugget-0.1.8/plugget/actions/blender_addon.py` & `plugget-0.1.9/plugget/actions/blender_addon.py`

 * *Files identical despite different names*

### Comparing `plugget-0.1.8/plugget/actions/blender_requirements.py` & `plugget-0.1.9/plugget/actions/blender_requirements.py`

 * *Files identical despite different names*

### Comparing `plugget-0.1.8/plugget/actions/krita_plugin.py` & `plugget-0.1.9/plugget/actions/krita_plugin.py`

 * *Files identical despite different names*

### Comparing `plugget-0.1.8/plugget/actions/krita_requirements.py` & `plugget-0.1.9/plugget/actions/krita_requirements.py`

 * *Files identical despite different names*

### Comparing `plugget-0.1.8/plugget/actions/max3ds_macroscript.py` & `plugget-0.1.9/plugget/actions/max3ds_macroscript.py`

 * *Files identical despite different names*

### Comparing `plugget-0.1.8/plugget/actions/maya_plugin.py` & `plugget-0.1.9/plugget/actions/maya_plugin.py`

 * *Files identical despite different names*

### Comparing `plugget-0.1.8/plugget/actions/substance_painter_plugin.py` & `plugget-0.1.9/plugget/actions/substance_painter_plugin.py`

 * *Files identical despite different names*

### Comparing `plugget-0.1.8/plugget/actions/substance_painter_requirements.py` & `plugget-0.1.9/plugget/actions/substance_painter_requirements.py`

 * *Files identical despite different names*

### Comparing `plugget-0.1.8/plugget/actions/unreal_plugin.py` & `plugget-0.1.9/plugget/actions/unreal_plugin.py`

 * *Files identical despite different names*

### Comparing `plugget-0.1.8/plugget/actions/unreal_requirements.py` & `plugget-0.1.9/plugget/actions/unreal_requirements.py`

 * *Files identical despite different names*

### Comparing `plugget-0.1.8/plugget/commands/__init__.py` & `plugget-0.1.9/plugget/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `plugget-0.1.8/plugget/data/package.py` & `plugget-0.1.9/plugget/data/package.py`

 * *Files identical despite different names*

### Comparing `plugget-0.1.8/plugget/data/packages_meta.py` & `plugget-0.1.9/plugget/data/packages_meta.py`

 * *Files identical despite different names*

### Comparing `plugget-0.1.8/plugget/github/__init__.py` & `plugget-0.1.9/plugget/github/__init__.py`

 * *Files identical despite different names*

### Comparing `plugget-0.1.8/plugget/github/async.py` & `plugget-0.1.9/plugget/github/async.py`

 * *Files identical despite different names*

### Comparing `plugget-0.1.8/plugget/gumroad/__init__.py` & `plugget-0.1.9/plugget/gumroad/__init__.py`

 * *Files identical despite different names*

### Comparing `plugget-0.1.8/plugget/settings.py` & `plugget-0.1.9/plugget/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 try:
     with importlib.resources.path('plugget.resources', 'config.json') as p:
         DEFAULT_PLUGGET_SETTINGS_PATH = Path(p).resolve()
 except Exception as e:
     logging.error("failed to get default settings path", e)
     DEFAULT_PLUGGET_SETTINGS_PATH = Path()
 
+
 # get settings for the actions etc, requires unique name for each action
 # todo support duplicates of the same settings for each app (blender, blender2, maya, etc)
 # actions request plugget for their settings
 # plugget manages & saves the settings and returns them
 
 
 registered_settings_paths = set([DEFAULT_PLUGGET_SETTINGS_PATH, USER_SETTINGS_PATH])
@@ -52,15 +53,15 @@
     """Load the registered settings configs"""
     settings = {}
     for path in registered_settings_paths:
         path = Path(path)
         if not path.exists():
             logging.warning(f"settings file not found: '{path}'")
             continue
-        data = _load_json_settings(USER_SETTINGS_PATH)
+        data = _load_json_settings(path)
         settings.update(data)
     return settings
 
 
 def load_plugget_settings():
     """load all plugget settings (default, user)"""
     global sources
```

### Comparing `plugget-0.1.8/plugget.egg-info/PKG-INFO` & `plugget-0.1.9/plugget.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plugget
-Version: 0.1.8
+Version: 0.1.9
 Summary: a package manager to install packages in your app
 Author: Hannes Delbeke
 Project-URL: Homepage, https://github.com/plugget/plugget
 Project-URL: Source, https://github.com/plugget/plugget
 Keywords: plugin,addon,add-on,extension,package,manager,resource,studio,dcc,app,application,pipeline,blender,krita,max
 Classifier: Programming Language :: Python :: 3.7
 Requires-Python: >=3.4
```

### Comparing `plugget-0.1.8/plugget.egg-info/SOURCES.txt` & `plugget-0.1.9/plugget.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `plugget-0.1.8/pyproject.toml` & `plugget-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 #license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python :: 3.7",
 ]
 #dynamic = ["dependencies"]
 dependencies = ['importlib-metadata; python_version<"3.7"', "detect-app", "py-pip", "requests"]
 #dynamic = ["version"]
-version = "0.1.8"
+version = "0.1.9"
 
 #[project.optional-dependencies]
 #yaml = ["pyyaml"]
 
 #[project.scripts]
 #my-script = "my_package.module:function"
```

### Comparing `plugget-0.1.8/testcode.py` & `plugget-0.1.9/testcode.py`

 * *Files identical despite different names*


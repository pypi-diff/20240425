# Comparing `tmp/glpic-99.0.202404251850.tar.gz` & `tmp/glpic-99.0.202404251853.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glpic-99.0.202404251850.tar", last modified: Thu Apr 25 18:50:19 2024, max compression
+gzip compressed data, was "glpic-99.0.202404251853.tar", last modified: Thu Apr 25 18:53:49 2024, max compression
```

## Comparing `glpic-99.0.202404251850.tar` & `glpic-99.0.202404251853.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:50:19.012611 glpic-99.0.202404251850/
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-25 18:50:19.012611 glpic-99.0.202404251850/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-25 18:50:06.000000 glpic-99.0.202404251850/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:50:19.012611 glpic-99.0.202404251850/glpic/
--rw-r--r--   0 runner    (1001) docker     (127)    10545 2024-04-25 18:50:06.000000 glpic-99.0.202404251850/glpic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10237 2024-04-25 18:50:06.000000 glpic-99.0.202404251850/glpic/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:50:19.012611 glpic-99.0.202404251850/glpic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-25 18:50:18.000000 glpic-99.0.202404251850/glpic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-25 18:50:18.000000 glpic-99.0.202404251850/glpic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 18:50:18.000000 glpic-99.0.202404251850/glpic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-25 18:50:18.000000 glpic-99.0.202404251850/glpic.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 18:50:18.000000 glpic-99.0.202404251850/glpic.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-25 18:50:18.000000 glpic-99.0.202404251850/glpic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-25 18:50:18.000000 glpic-99.0.202404251850/glpic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 18:50:19.012611 glpic-99.0.202404251850/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-04-25 18:50:18.000000 glpic-99.0.202404251850/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:53:49.084484 glpic-99.0.202404251853/
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-25 18:53:49.084484 glpic-99.0.202404251853/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-25 18:53:33.000000 glpic-99.0.202404251853/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:53:49.084484 glpic-99.0.202404251853/glpic/
+-rw-r--r--   0 runner    (1001) docker     (127)    10545 2024-04-25 18:53:33.000000 glpic-99.0.202404251853/glpic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10237 2024-04-25 18:53:33.000000 glpic-99.0.202404251853/glpic/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:53:49.084484 glpic-99.0.202404251853/glpic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-25 18:53:49.000000 glpic-99.0.202404251853/glpic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-25 18:53:49.000000 glpic-99.0.202404251853/glpic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 18:53:49.000000 glpic-99.0.202404251853/glpic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-25 18:53:49.000000 glpic-99.0.202404251853/glpic.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 18:53:49.000000 glpic-99.0.202404251853/glpic.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-25 18:53:49.000000 glpic-99.0.202404251853/glpic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-25 18:53:49.000000 glpic-99.0.202404251853/glpic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 18:53:49.088484 glpic-99.0.202404251853/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-04-25 18:53:48.000000 glpic-99.0.202404251853/setup.py
```

### Comparing `glpic-99.0.202404251850/README.md` & `glpic-99.0.202404251853/README.md`

 * *Files identical despite different names*

### Comparing `glpic-99.0.202404251850/glpic/__init__.py` & `glpic-99.0.202404251853/glpic/__init__.py`

 * *Files identical despite different names*

### Comparing `glpic-99.0.202404251850/glpic/cli.py` & `glpic-99.0.202404251853/glpic/cli.py`

 * *Files identical despite different names*

### Comparing `glpic-99.0.202404251850/setup.py` & `glpic-99.0.202404251853/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 description = 'Glpic wrapper'
 long_description = description
 if os.path.exists('README.rst'):
     long_description = open('README.rst').read()
 
 setup(
     name='glpic',
-    version='99.0.202404251850',
+    version='99.0.202404251853',
     include_package_data=True,
     packages=find_packages(),
     zip_safe=False,
     description=description,
     long_description=long_description,
     url='http://github.com/karmab/glpic',
     author='Karim Boumedhel',
```


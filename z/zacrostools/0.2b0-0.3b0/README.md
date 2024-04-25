# Comparing `tmp/zacrostools-0.2b0.tar.gz` & `tmp/zacrostools-0.3b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zacrostools-0.2b0.tar", last modified: Tue Apr 23 23:24:21 2024, max compression
+gzip compressed data, was "zacrostools-0.3b0.tar", last modified: Thu Apr 25 16:05:38 2024, max compression
```

## Comparing `zacrostools-0.2b0.tar` & `zacrostools-0.3b0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 install    (505) staff       (20)        0 2024-04-23 23:24:21.093886 zacrostools-0.2b0/
--rw-r--r--   0 install    (505) staff       (20)     1069 2024-04-23 22:06:48.000000 zacrostools-0.2b0/LICENSE.txt
--rw-r--r--   0 install    (505) staff       (20)    12056 2024-04-23 23:24:21.093387 zacrostools-0.2b0/PKG-INFO
--rw-r--r--   0 install    (505) staff       (20)    11581 2024-04-23 23:21:51.000000 zacrostools-0.2b0/README.md
--rw-r--r--   0 install    (505) staff       (20)       79 2024-04-23 23:24:21.095848 zacrostools-0.2b0/setup.cfg
--rw-r--r--   0 install    (505) staff       (20)      684 2024-04-23 23:24:03.000000 zacrostools-0.2b0/setup.py
-drwxr-xr-x   0 install    (505) staff       (20)        0 2024-04-23 23:24:21.072403 zacrostools-0.2b0/zacrostools/
--rw-r--r--   0 install    (505) staff       (20)        0 2024-04-23 21:56:46.000000 zacrostools-0.2b0/zacrostools/__init__.py
--rw-r--r--   0 install    (505) staff       (20)      374 2024-04-23 21:56:46.000000 zacrostools-0.2b0/zacrostools/analysis_functions.py
--rw-r--r--   0 install    (505) staff       (20)     3185 2024-04-23 21:59:51.000000 zacrostools-0.2b0/zacrostools/energetics_input.py
--rw-r--r--   0 install    (505) staff       (20)     6339 2024-04-23 21:58:56.000000 zacrostools-0.2b0/zacrostools/input_functions.py
--rw-r--r--   0 install    (505) staff       (20)     6216 2024-04-23 22:15:09.000000 zacrostools-0.2b0/zacrostools/kmc_model.py
--rw-r--r--   0 install    (505) staff       (20)     1824 2024-04-23 22:03:22.000000 zacrostools-0.2b0/zacrostools/lattice_input.py
--rw-r--r--   0 install    (505) staff       (20)     6958 2024-04-23 22:16:16.000000 zacrostools-0.2b0/zacrostools/mechanism_input.py
--rw-r--r--   0 install    (505) staff       (20)     1526 2024-04-23 21:56:46.000000 zacrostools-0.2b0/zacrostools/read_functions.py
-drwxr-xr-x   0 install    (505) staff       (20)        0 2024-04-23 23:24:21.092473 zacrostools-0.2b0/zacrostools.egg-info/
--rw-r--r--   0 install    (505) staff       (20)    12056 2024-04-23 23:24:21.000000 zacrostools-0.2b0/zacrostools.egg-info/PKG-INFO
--rw-r--r--   0 install    (505) staff       (20)      450 2024-04-23 23:24:21.000000 zacrostools-0.2b0/zacrostools.egg-info/SOURCES.txt
--rw-r--r--   0 install    (505) staff       (20)        1 2024-04-23 23:24:21.000000 zacrostools-0.2b0/zacrostools.egg-info/dependency_links.txt
--rw-r--r--   0 install    (505) staff       (20)       13 2024-04-23 23:24:21.000000 zacrostools-0.2b0/zacrostools.egg-info/requires.txt
--rw-r--r--   0 install    (505) staff       (20)       12 2024-04-23 23:24:21.000000 zacrostools-0.2b0/zacrostools.egg-info/top_level.txt
+drwxr-xr-x   0 install    (505) staff       (20)        0 2024-04-25 16:05:38.548390 zacrostools-0.3b0/
+-rw-r--r--   0 install    (505) staff       (20)     1069 2024-04-23 22:06:48.000000 zacrostools-0.3b0/LICENSE.txt
+-rw-r--r--   0 install    (505) staff       (20)     1347 2024-04-25 16:05:38.547321 zacrostools-0.3b0/PKG-INFO
+-rw-r--r--   0 install    (505) staff       (20)      872 2024-04-25 15:59:34.000000 zacrostools-0.3b0/README.md
+-rw-r--r--   0 install    (505) staff       (20)       79 2024-04-25 16:05:38.550446 zacrostools-0.3b0/setup.cfg
+-rw-r--r--   0 install    (505) staff       (20)      684 2024-04-25 16:03:03.000000 zacrostools-0.3b0/setup.py
+drwxr-xr-x   0 install    (505) staff       (20)        0 2024-04-25 16:05:38.524490 zacrostools-0.3b0/zacrostools/
+-rw-r--r--   0 install    (505) staff       (20)        0 2024-04-23 21:56:46.000000 zacrostools-0.3b0/zacrostools/__init__.py
+-rw-r--r--   0 install    (505) staff       (20)      374 2024-04-23 21:56:46.000000 zacrostools-0.3b0/zacrostools/analysis_functions.py
+-rw-r--r--   0 install    (505) staff       (20)     3185 2024-04-23 21:59:51.000000 zacrostools-0.3b0/zacrostools/energetics_input.py
+-rw-r--r--   0 install    (505) staff       (20)     6339 2024-04-23 21:58:56.000000 zacrostools-0.3b0/zacrostools/input_functions.py
+-rw-r--r--   0 install    (505) staff       (20)     6216 2024-04-23 22:15:09.000000 zacrostools-0.3b0/zacrostools/kmc_model.py
+-rw-r--r--   0 install    (505) staff       (20)     1824 2024-04-23 22:03:22.000000 zacrostools-0.3b0/zacrostools/lattice_input.py
+-rw-r--r--   0 install    (505) staff       (20)     6958 2024-04-23 22:16:16.000000 zacrostools-0.3b0/zacrostools/mechanism_input.py
+-rw-r--r--   0 install    (505) staff       (20)     1526 2024-04-23 21:56:46.000000 zacrostools-0.3b0/zacrostools/read_functions.py
+drwxr-xr-x   0 install    (505) staff       (20)        0 2024-04-25 16:05:38.544883 zacrostools-0.3b0/zacrostools.egg-info/
+-rw-r--r--   0 install    (505) staff       (20)     1347 2024-04-25 16:05:38.000000 zacrostools-0.3b0/zacrostools.egg-info/PKG-INFO
+-rw-r--r--   0 install    (505) staff       (20)      450 2024-04-25 16:05:38.000000 zacrostools-0.3b0/zacrostools.egg-info/SOURCES.txt
+-rw-r--r--   0 install    (505) staff       (20)        1 2024-04-25 16:05:38.000000 zacrostools-0.3b0/zacrostools.egg-info/dependency_links.txt
+-rw-r--r--   0 install    (505) staff       (20)       13 2024-04-25 16:05:38.000000 zacrostools-0.3b0/zacrostools.egg-info/requires.txt
+-rw-r--r--   0 install    (505) staff       (20)       12 2024-04-25 16:05:38.000000 zacrostools-0.3b0/zacrostools.egg-info/top_level.txt
```

### Comparing `zacrostools-0.2b0/LICENSE.txt` & `zacrostools-0.3b0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zacrostools-0.2b0/setup.py` & `zacrostools-0.3b0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name='zacrostools',
-    version='0.2-beta',
+    version='0.3-beta',
     description='A collective of tools for the preparation of input files for ZACROS',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(),
     url='https://github.com/hprats/ZacrosTools',
-    download_url='https://github.com/hprats/ZacrosTools/archive/refs/tags/v0.2-beta.tar.gz',
+    download_url='https://github.com/hprats/ZacrosTools/archive/refs/tags/v0.3-beta.tar.gz',
     author='Hector Prats',
     author_email='hpratsgarcia@gmail.com',
     keywords=['python', 'chemistry', 'KMC', 'ZACROS'],
     install_requires=['pandas', 'scipy']
 )
```

### Comparing `zacrostools-0.2b0/zacrostools/energetics_input.py` & `zacrostools-0.3b0/zacrostools/energetics_input.py`

 * *Files identical despite different names*

### Comparing `zacrostools-0.2b0/zacrostools/input_functions.py` & `zacrostools-0.3b0/zacrostools/input_functions.py`

 * *Files identical despite different names*

### Comparing `zacrostools-0.2b0/zacrostools/kmc_model.py` & `zacrostools-0.3b0/zacrostools/kmc_model.py`

 * *Files identical despite different names*

### Comparing `zacrostools-0.2b0/zacrostools/lattice_input.py` & `zacrostools-0.3b0/zacrostools/lattice_input.py`

 * *Files identical despite different names*

### Comparing `zacrostools-0.2b0/zacrostools/mechanism_input.py` & `zacrostools-0.3b0/zacrostools/mechanism_input.py`

 * *Files identical despite different names*

### Comparing `zacrostools-0.2b0/zacrostools/read_functions.py` & `zacrostools-0.3b0/zacrostools/read_functions.py`

 * *Files identical despite different names*


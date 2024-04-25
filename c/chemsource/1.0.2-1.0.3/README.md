# Comparing `tmp/chemsource-1.0.2.tar.gz` & `tmp/chemsource-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chemsource-1.0.2.tar", last modified: Tue Apr 23 20:48:50 2024, max compression
+gzip compressed data, was "chemsource-1.0.3.tar", last modified: Thu Apr 25 08:18:41 2024, max compression
```

## Comparing `chemsource-1.0.2.tar` & `chemsource-1.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 prajitrajkumar   (501) staff       (20)        0 2024-04-23 20:48:50.759873 chemsource-1.0.2/
--rw-r--r--   0 prajitrajkumar   (501) staff       (20)     1072 2024-04-23 08:23:13.000000 chemsource-1.0.2/LICENSE
--rw-r--r--   0 prajitrajkumar   (501) staff       (20)      508 2024-04-23 20:48:50.759719 chemsource-1.0.2/PKG-INFO
--rw-r--r--   0 prajitrajkumar   (501) staff       (20)     1474 2024-04-23 07:25:30.000000 chemsource-1.0.2/README.md
--rw-r--r--   0 prajitrajkumar   (501) staff       (20)      113 2024-04-23 20:48:50.760499 chemsource-1.0.2/setup.cfg
--rw-r--r--   0 prajitrajkumar   (501) staff       (20)      664 2024-04-23 20:22:21.000000 chemsource-1.0.2/setup.py
-drwxr-xr-x   0 prajitrajkumar   (501) staff       (20)        0 2024-04-23 20:48:50.753691 chemsource-1.0.2/src/
-drwxr-xr-x   0 prajitrajkumar   (501) staff       (20)        0 2024-04-23 20:48:50.757460 chemsource-1.0.2/src/chemsource/
--rw-r--r--   0 prajitrajkumar   (501) staff       (20)       57 2024-04-23 20:48:41.000000 chemsource-1.0.2/src/chemsource/__init__.py
--rw-r--r--   0 prajitrajkumar   (501) staff       (20)     1864 2024-04-23 20:37:25.000000 chemsource-1.0.2/src/chemsource/chemsource.py
--rw-r--r--   0 prajitrajkumar   (501) staff       (20)      653 2024-04-23 20:48:21.000000 chemsource-1.0.2/src/chemsource/classifier.py
--rw-r--r--   0 prajitrajkumar   (501) staff       (20)     2918 2024-04-23 20:35:54.000000 chemsource-1.0.2/src/chemsource/config.py
--rw-r--r--   0 prajitrajkumar   (501) staff       (20)      823 2024-04-10 21:23:32.000000 chemsource-1.0.2/src/chemsource/exceptions.py
--rw-r--r--   0 prajitrajkumar   (501) staff       (20)     4019 2024-04-23 19:48:05.000000 chemsource-1.0.2/src/chemsource/retriever.py
-drwxr-xr-x   0 prajitrajkumar   (501) staff       (20)        0 2024-04-23 20:48:50.759159 chemsource-1.0.2/src/chemsource.egg-info/
--rw-r--r--   0 prajitrajkumar   (501) staff       (20)      508 2024-04-23 20:48:50.000000 chemsource-1.0.2/src/chemsource.egg-info/PKG-INFO
--rw-r--r--   0 prajitrajkumar   (501) staff       (20)      392 2024-04-23 20:48:50.000000 chemsource-1.0.2/src/chemsource.egg-info/SOURCES.txt
--rw-r--r--   0 prajitrajkumar   (501) staff       (20)        1 2024-04-23 20:48:50.000000 chemsource-1.0.2/src/chemsource.egg-info/dependency_links.txt
--rw-r--r--   0 prajitrajkumar   (501) staff       (20)       63 2024-04-23 20:48:50.000000 chemsource-1.0.2/src/chemsource.egg-info/requires.txt
--rw-r--r--   0 prajitrajkumar   (501) staff       (20)       11 2024-04-23 20:48:50.000000 chemsource-1.0.2/src/chemsource.egg-info/top_level.txt
+drwxr-xr-x   0 prajitrajkumar   (501) staff       (20)        0 2024-04-25 08:18:41.142543 chemsource-1.0.3/
+-rw-r--r--   0 prajitrajkumar   (501) staff       (20)     1072 2024-04-23 08:23:13.000000 chemsource-1.0.3/LICENSE
+-rw-r--r--   0 prajitrajkumar   (501) staff       (20)     9597 2024-04-25 08:18:41.142392 chemsource-1.0.3/PKG-INFO
+-rw-r--r--   0 prajitrajkumar   (501) staff       (20)     9047 2024-04-25 08:17:22.000000 chemsource-1.0.3/README.md
+-rw-r--r--   0 prajitrajkumar   (501) staff       (20)      113 2024-04-25 08:18:41.142960 chemsource-1.0.3/setup.cfg
+-rw-r--r--   0 prajitrajkumar   (501) staff       (20)      880 2024-04-25 08:12:55.000000 chemsource-1.0.3/setup.py
+drwxr-xr-x   0 prajitrajkumar   (501) staff       (20)        0 2024-04-25 08:18:41.136414 chemsource-1.0.3/src/
+drwxr-xr-x   0 prajitrajkumar   (501) staff       (20)        0 2024-04-25 08:18:41.139723 chemsource-1.0.3/src/chemsource/
+-rw-r--r--   0 prajitrajkumar   (501) staff       (20)       57 2024-04-25 08:18:25.000000 chemsource-1.0.3/src/chemsource/__init__.py
+-rw-r--r--   0 prajitrajkumar   (501) staff       (20)     1864 2024-04-23 20:37:25.000000 chemsource-1.0.3/src/chemsource/chemsource.py
+-rw-r--r--   0 prajitrajkumar   (501) staff       (20)      653 2024-04-23 20:48:21.000000 chemsource-1.0.3/src/chemsource/classifier.py
+-rw-r--r--   0 prajitrajkumar   (501) staff       (20)     2918 2024-04-23 20:35:54.000000 chemsource-1.0.3/src/chemsource/config.py
+-rw-r--r--   0 prajitrajkumar   (501) staff       (20)      823 2024-04-10 21:23:32.000000 chemsource-1.0.3/src/chemsource/exceptions.py
+-rw-r--r--   0 prajitrajkumar   (501) staff       (20)     4219 2024-04-25 07:37:13.000000 chemsource-1.0.3/src/chemsource/retriever.py
+drwxr-xr-x   0 prajitrajkumar   (501) staff       (20)        0 2024-04-25 08:18:41.141833 chemsource-1.0.3/src/chemsource.egg-info/
+-rw-r--r--   0 prajitrajkumar   (501) staff       (20)     9597 2024-04-25 08:18:41.000000 chemsource-1.0.3/src/chemsource.egg-info/PKG-INFO
+-rw-r--r--   0 prajitrajkumar   (501) staff       (20)      392 2024-04-25 08:18:41.000000 chemsource-1.0.3/src/chemsource.egg-info/SOURCES.txt
+-rw-r--r--   0 prajitrajkumar   (501) staff       (20)        1 2024-04-25 08:18:41.000000 chemsource-1.0.3/src/chemsource.egg-info/dependency_links.txt
+-rw-r--r--   0 prajitrajkumar   (501) staff       (20)       63 2024-04-25 08:18:41.000000 chemsource-1.0.3/src/chemsource.egg-info/requires.txt
+-rw-r--r--   0 prajitrajkumar   (501) staff       (20)       11 2024-04-25 08:18:41.000000 chemsource-1.0.3/src/chemsource.egg-info/top_level.txt
```

### Comparing `chemsource-1.0.2/LICENSE` & `chemsource-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `chemsource-1.0.2/setup.py` & `chemsource-1.0.3/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,12 @@
 from setuptools import setup, find_packages
+from pathlib import Path
+
+this_directory = Path(__file__).parent
+long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="chemsource",
     author="Prajit Rajkumar",
     author_email="prajkumar@ucsd.edu",
     description="Tool to classify novel drugs and other health-related" 
                 + " chemicals by origin",
@@ -16,8 +20,10 @@
     python_requires='>=3.6',
     install_requires=[
         "lxml>=4.9.4",
         "openai>=1.23.2",
         "requests>=2.0.0,<3",
         "wikipedia>=1.4.0",
     ],
+    long_description=long_description,
+    long_description_content_type='text/markdown'
 )
```

### Comparing `chemsource-1.0.2/src/chemsource/chemsource.py` & `chemsource-1.0.3/src/chemsource/chemsource.py`

 * *Files identical despite different names*

### Comparing `chemsource-1.0.2/src/chemsource/classifier.py` & `chemsource-1.0.3/src/chemsource/classifier.py`

 * *Files identical despite different names*

### Comparing `chemsource-1.0.2/src/chemsource/config.py` & `chemsource-1.0.3/src/chemsource/config.py`

 * *Files identical despite different names*

### Comparing `chemsource-1.0.2/src/chemsource/exceptions.py` & `chemsource-1.0.3/src/chemsource/exceptions.py`

 * *Files identical despite different names*

### Comparing `chemsource-1.0.2/src/chemsource/retriever.py` & `chemsource-1.0.3/src/chemsource/retriever.py`

 * *Files 8% similar despite different names*

```diff
@@ -54,21 +54,25 @@
         try:
             description = wikipedia_retrieve(name)
             info_source = "WIKIPEDIA"
         except:
             description = None
             info_source = None
     
-    else:
+    elif (priority == "PUBMED" and single_source):
         try:
             description = pubmed_retrieve(name, ncbikey)
             info_source = "PUBMED"
         except:
             description = None
             info_source = None
+    
+    else:
+        raise ValueError("priority must be either WIKIPEDIA or PUBMED" 
+                         + "and single_source must be a boolean value")
 
     return info_source, description
     
 def pubmed_retrieve(drug, ncbikey=None):
     temp_search_params = SEARCH_PARAMS
     temp_search_params['api_key'] = ncbikey
```


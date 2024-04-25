# Comparing `tmp/g2p-mix-0.4.0.tar.gz` & `tmp/g2p-mix-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "g2p-mix-0.4.0.tar", last modified: Thu Apr 25 15:25:05 2024, max compression
+gzip compressed data, was "g2p-mix-0.4.1.tar", last modified: Thu Apr 25 15:28:30 2024, max compression
```

## Comparing `g2p-mix-0.4.0.tar` & `g2p-mix-0.4.1.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:25:05.446702 g2p-mix-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-25 15:25:04.000000 g2p-mix-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-25 15:25:04.000000 g2p-mix-0.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-04-25 15:25:05.446702 g2p-mix-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-25 15:25:04.000000 g2p-mix-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:25:05.438702 g2p-mix-0.4.0/g2p_mix/
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-25 15:25:04.000000 g2p-mix-0.4.0/g2p_mix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-25 15:25:04.000000 g2p-mix-0.4.0/g2p_mix/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-04-25 15:25:04.000000 g2p-mix-0.4.0/g2p_mix/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-04-25 15:25:04.000000 g2p-mix-0.4.0/g2p_mix/g2p_eng.py
--rw-r--r--   0 runner    (1001) docker     (127)     5007 2024-04-25 15:25:04.000000 g2p-mix-0.4.0/g2p_mix/g2p_mix.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:25:05.438702 g2p-mix-0.4.0/g2p_mix/nltk_data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:25:05.442702 g2p-mix-0.4.0/g2p_mix/nltk_data/corpora/
--rw-r--r--   0 runner    (1001) docker     (127)   896069 2024-04-25 15:25:04.000000 g2p-mix-0.4.0/g2p_mix/nltk_data/corpora/cmudict.zip
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:25:05.442702 g2p-mix-0.4.0/g2p_mix/nltk_data/taggers/
--rw-r--r--   0 runner    (1001) docker     (127)  2526731 2024-04-25 15:25:04.000000 g2p-mix-0.4.0/g2p_mix/nltk_data/taggers/averaged_perceptron_tagger.zip
--rw-r--r--   0 runner    (1001) docker     (127)     2047 2024-04-25 15:25:04.000000 g2p-mix-0.4.0/g2p_mix/token.py
--rw-r--r--   0 runner    (1001) docker     (127)    11066 2024-04-25 15:25:04.000000 g2p-mix-0.4.0/g2p_mix/tone_sandhi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:25:05.438702 g2p-mix-0.4.0/g2p_mix.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-04-25 15:25:05.000000 g2p-mix-0.4.0/g2p_mix.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-25 15:25:05.000000 g2p-mix-0.4.0/g2p_mix.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 15:25:05.000000 g2p-mix-0.4.0/g2p_mix.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-25 15:25:05.000000 g2p-mix-0.4.0/g2p_mix.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-25 15:25:05.000000 g2p-mix-0.4.0/g2p_mix.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-25 15:25:05.000000 g2p-mix-0.4.0/g2p_mix.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-25 15:25:04.000000 g2p-mix-0.4.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 15:25:05.446702 g2p-mix-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-04-25 15:25:04.000000 g2p-mix-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:28:30.910365 g2p-mix-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-25 15:28:30.000000 g2p-mix-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-25 15:28:30.000000 g2p-mix-0.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-04-25 15:28:30.910365 g2p-mix-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-25 15:28:30.000000 g2p-mix-0.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-25 15:28:30.000000 g2p-mix-0.4.1/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:28:30.902364 g2p-mix-0.4.1/g2p_mix/
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-25 15:28:30.000000 g2p-mix-0.4.1/g2p_mix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-25 15:28:30.000000 g2p-mix-0.4.1/g2p_mix/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-04-25 15:28:30.000000 g2p-mix-0.4.1/g2p_mix/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-04-25 15:28:30.000000 g2p-mix-0.4.1/g2p_mix/g2p_eng.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5007 2024-04-25 15:28:30.000000 g2p-mix-0.4.1/g2p_mix/g2p_mix.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:28:30.902364 g2p-mix-0.4.1/g2p_mix/nltk_data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:28:30.906365 g2p-mix-0.4.1/g2p_mix/nltk_data/corpora/
+-rw-r--r--   0 runner    (1001) docker     (127)   896069 2024-04-25 15:28:30.000000 g2p-mix-0.4.1/g2p_mix/nltk_data/corpora/cmudict.zip
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:28:30.906365 g2p-mix-0.4.1/g2p_mix/nltk_data/taggers/
+-rw-r--r--   0 runner    (1001) docker     (127)  2526731 2024-04-25 15:28:30.000000 g2p-mix-0.4.1/g2p_mix/nltk_data/taggers/averaged_perceptron_tagger.zip
+-rw-r--r--   0 runner    (1001) docker     (127)     2047 2024-04-25 15:28:30.000000 g2p-mix-0.4.1/g2p_mix/token.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11066 2024-04-25 15:28:30.000000 g2p-mix-0.4.1/g2p_mix/tone_sandhi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:28:30.906365 g2p-mix-0.4.1/g2p_mix.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-04-25 15:28:30.000000 g2p-mix-0.4.1/g2p_mix.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-25 15:28:30.000000 g2p-mix-0.4.1/g2p_mix.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 15:28:30.000000 g2p-mix-0.4.1/g2p_mix.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-25 15:28:30.000000 g2p-mix-0.4.1/g2p_mix.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-25 15:28:30.000000 g2p-mix-0.4.1/g2p_mix.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-25 15:28:30.000000 g2p-mix-0.4.1/g2p_mix.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-25 15:28:30.000000 g2p-mix-0.4.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 15:28:30.910365 g2p-mix-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-04-25 15:28:30.000000 g2p-mix-0.4.1/setup.py
```

### Comparing `g2p-mix-0.4.0/LICENSE` & `g2p-mix-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `g2p-mix-0.4.0/PKG-INFO` & `g2p-mix-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: g2p-mix
-Version: 0.4.0
+Version: 0.4.1
 Summary: G2P mix
 Home-page: https://github.com/pengzhendong/g2p-mix
 Author: Zhendong Peng
 Author-email: pzd17@tsinghua.org.cn
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `g2p-mix-0.4.0/README.md` & `g2p-mix-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `g2p-mix-0.4.0/g2p_mix/__init__.py` & `g2p-mix-0.4.1/g2p_mix/__init__.py`

 * *Files identical despite different names*

### Comparing `g2p-mix-0.4.0/g2p_mix/cli.py` & `g2p-mix-0.4.1/g2p_mix/cli.py`

 * *Files identical despite different names*

### Comparing `g2p-mix-0.4.0/g2p_mix/constants.py` & `g2p-mix-0.4.1/g2p_mix/constants.py`

 * *Files identical despite different names*

### Comparing `g2p-mix-0.4.0/g2p_mix/g2p_eng.py` & `g2p-mix-0.4.1/g2p_mix/g2p_eng.py`

 * *Files identical despite different names*

### Comparing `g2p-mix-0.4.0/g2p_mix/g2p_mix.py` & `g2p-mix-0.4.1/g2p_mix/g2p_mix.py`

 * *Files identical despite different names*

### Comparing `g2p-mix-0.4.0/g2p_mix/nltk_data/corpora/cmudict.zip` & `g2p-mix-0.4.1/g2p_mix/nltk_data/corpora/cmudict.zip`

 * *Files identical despite different names*

### Comparing `g2p-mix-0.4.0/g2p_mix/nltk_data/taggers/averaged_perceptron_tagger.zip` & `g2p-mix-0.4.1/g2p_mix/nltk_data/taggers/averaged_perceptron_tagger.zip`

 * *Files identical despite different names*

### Comparing `g2p-mix-0.4.0/g2p_mix/token.py` & `g2p-mix-0.4.1/g2p_mix/token.py`

 * *Files identical despite different names*

### Comparing `g2p-mix-0.4.0/g2p_mix/tone_sandhi.py` & `g2p-mix-0.4.1/g2p_mix/tone_sandhi.py`

 * *Files identical despite different names*

### Comparing `g2p-mix-0.4.0/g2p_mix.egg-info/PKG-INFO` & `g2p-mix-0.4.1/g2p_mix.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: g2p-mix
-Version: 0.4.0
+Version: 0.4.1
 Summary: G2P mix
 Home-page: https://github.com/pengzhendong/g2p-mix
 Author: Zhendong Peng
 Author-email: pzd17@tsinghua.org.cn
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `g2p-mix-0.4.0/setup.py` & `g2p-mix-0.4.1/setup.py`

 * *Files identical despite different names*


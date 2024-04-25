# Comparing `tmp/cryptonita-0.6.2.tar.gz` & `tmp/cryptonita-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cryptonita-0.6.2.tar", last modified: Thu Mar 28 19:09:10 2024, max compression
+gzip compressed data, was "cryptonita-0.6.3.tar", last modified: Thu Apr 25 14:54:50 2024, max compression
```

## Comparing `cryptonita-0.6.2.tar` & `cryptonita-0.6.3.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-03-28 19:09:10.949078 cryptonita-0.6.2/
--rw-r--r--   0 user      (1000) user      (1000)    20469 2024-03-28 19:09:10.949078 cryptonita-0.6.2/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)    15620 2024-03-28 19:09:10.000000 cryptonita-0.6.2/README.rst
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-03-28 19:09:10.945077 cryptonita-0.6.2/cryptonita/
--rw-r--r--   0 user      (1000) user      (1000)      916 2024-03-28 19:08:40.000000 cryptonita-0.6.2/cryptonita/__init__.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-03-28 19:09:10.945077 cryptonita-0.6.2/cryptonita/attacks/
--rw-r--r--   0 user      (1000) user      (1000)    10105 2023-04-03 00:16:55.000000 cryptonita-0.6.2/cryptonita/attacks/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)     3689 2022-06-20 19:51:05.000000 cryptonita-0.6.2/cryptonita/attacks/block_ciphers.py
--rw-r--r--   0 user      (1000) user      (1000)     2597 2024-03-28 18:39:16.000000 cryptonita-0.6.2/cryptonita/attacks/mapping.py
--rw-r--r--   0 user      (1000) user      (1000)     4304 2024-03-26 03:51:03.000000 cryptonita-0.6.2/cryptonita/attacks/prng.py
--rw-r--r--   0 user      (1000) user      (1000)     7892 2024-03-28 18:39:16.000000 cryptonita-0.6.2/cryptonita/bytestrings.py
--rw-r--r--   0 user      (1000) user      (1000)    12508 2024-03-28 18:59:03.000000 cryptonita-0.6.2/cryptonita/conv.py
--rw-r--r--   0 user      (1000) user      (1000)      461 2024-03-28 19:08:17.000000 cryptonita-0.6.2/cryptonita/deps.py
--rw-r--r--   0 user      (1000) user      (1000)    14291 2023-01-14 13:34:40.000000 cryptonita-0.6.2/cryptonita/fuzzy_set.py
--rw-r--r--   0 user      (1000) user      (1000)     3502 2022-06-20 20:45:28.000000 cryptonita-0.6.2/cryptonita/helpers.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-03-28 19:09:10.945077 cryptonita-0.6.2/cryptonita/metrics/
--rw-r-----   0 user      (1000) user      (1000)     7963 2022-06-23 23:13:08.000000 cryptonita-0.6.2/cryptonita/metrics/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)    19979 2023-04-06 22:33:46.000000 cryptonita-0.6.2/cryptonita/mixins.py
--rw-r--r--   0 user      (1000) user      (1000)      936 2024-03-28 18:39:16.000000 cryptonita-0.6.2/cryptonita/mod.py
--rw-r--r--   0 user      (1000) user      (1000)     3989 2022-06-20 19:51:05.000000 cryptonita-0.6.2/cryptonita/plots.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-03-28 19:09:10.945077 cryptonita-0.6.2/cryptonita/scoring/
--rw-r--r--   0 user      (1000) user      (1000)     1070 2023-01-14 01:18:26.000000 cryptonita-0.6.2/cryptonita/scoring/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)     4031 2024-03-28 18:37:21.000000 cryptonita-0.6.2/cryptonita/scoring/freq.py
--rw-r--r--   0 user      (1000) user      (1000)    10884 2024-03-28 18:39:16.000000 cryptonita-0.6.2/cryptonita/scoring/score_funcs.py
--rw-r--r--   0 user      (1000) user      (1000)     6925 2024-03-20 14:47:10.000000 cryptonita-0.6.2/cryptonita/space.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-03-28 19:09:10.945077 cryptonita-0.6.2/cryptonita/stats/
--rw-r--r--   0 user      (1000) user      (1000)     1444 2022-06-20 19:51:05.000000 cryptonita-0.6.2/cryptonita/stats/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)    12129 2022-06-20 19:51:05.000000 cryptonita-0.6.2/cryptonita/stats/kasiski.py
--rw-r--r--   0 user      (1000) user      (1000)     1670 2022-06-20 19:51:05.000000 cryptonita-0.6.2/cryptonita/suggesters.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-03-28 19:09:10.945077 cryptonita-0.6.2/cryptonita/toys/
--rw-r--r--   0 user      (1000) user      (1000)       76 2022-06-20 19:51:05.000000 cryptonita-0.6.2/cryptonita/toys/__init__.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-03-28 19:09:10.945077 cryptonita-0.6.2/cryptonita/toys/hashes/
--rw-r--r--   0 user      (1000) user      (1000)        0 2023-03-17 18:19:17.000000 cryptonita-0.6.2/cryptonita/toys/hashes/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)      288 2024-03-20 13:14:32.000000 cryptonita-0.6.2/cryptonita/toys/hashes/keyed.py
--rw-r--r--   0 user      (1000) user      (1000)     3571 2024-03-20 13:13:37.000000 cryptonita-0.6.2/cryptonita/toys/hashes/md4.py
--rw-r--r--   0 user      (1000) user      (1000)     3108 2024-03-20 13:12:45.000000 cryptonita-0.6.2/cryptonita/toys/hashes/sha1.py
--rw-r--r--   0 user      (1000) user      (1000)     6166 2024-03-20 13:14:32.000000 cryptonita-0.6.2/cryptonita/toys/hashes/sha256.py
--rw-r--r--   0 user      (1000) user      (1000)     4924 2024-03-28 18:39:16.000000 cryptonita-0.6.2/cryptonita/toys/substitution_ciphers.py
--rw-r--r--   0 user      (1000) user      (1000)     3559 2024-03-28 18:38:08.000000 cryptonita-0.6.2/cryptonita/toys/transposition_ciphers.py
--rw-r--r--   0 user      (1000) user      (1000)     8953 2023-01-19 23:25:36.000000 cryptonita-0.6.2/cryptonita/views.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-03-28 19:09:10.945077 cryptonita-0.6.2/cryptonita.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)    20469 2024-03-28 19:09:10.000000 cryptonita-0.6.2/cryptonita.egg-info/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)     1034 2024-03-28 19:09:10.000000 cryptonita-0.6.2/cryptonita.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1000) user      (1000)        1 2024-03-28 19:09:10.000000 cryptonita-0.6.2/cryptonita.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1000) user      (1000)      104 2024-03-28 19:09:10.000000 cryptonita-0.6.2/cryptonita.egg-info/requires.txt
--rw-r--r--   0 user      (1000) user      (1000)       11 2024-03-28 19:09:10.000000 cryptonita-0.6.2/cryptonita.egg-info/top_level.txt
--rw-r--r--   0 user      (1000) user      (1000)       60 2023-03-17 21:20:42.000000 cryptonita-0.6.2/pyproject.toml
--rw-r--r--   0 user      (1000) user      (1000)       38 2024-03-28 19:09:10.949078 cryptonita-0.6.2/setup.cfg
--rw-r--r--   0 user      (1000) user      (1000)     2841 2024-03-28 18:43:39.000000 cryptonita-0.6.2/setup.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-04-25 14:54:50.567540 cryptonita-0.6.3/
+-rw-r--r--   0 user      (1000) user      (1000)    20469 2024-04-25 14:54:50.567540 cryptonita-0.6.3/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)    15620 2024-04-25 14:54:50.000000 cryptonita-0.6.3/README.rst
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-04-25 14:54:50.551533 cryptonita-0.6.3/cryptonita/
+-rw-r--r--   0 user      (1000) user      (1000)      916 2024-04-25 14:54:03.000000 cryptonita-0.6.3/cryptonita/__init__.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-04-25 14:54:50.555534 cryptonita-0.6.3/cryptonita/attacks/
+-rw-r--r--   0 user      (1000) user      (1000)    10105 2023-04-03 00:16:55.000000 cryptonita-0.6.3/cryptonita/attacks/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)     3689 2022-06-20 19:51:05.000000 cryptonita-0.6.3/cryptonita/attacks/block_ciphers.py
+-rw-r--r--   0 user      (1000) user      (1000)     2597 2024-03-28 18:39:16.000000 cryptonita-0.6.3/cryptonita/attacks/mapping.py
+-rw-r--r--   0 user      (1000) user      (1000)     4274 2024-04-25 14:51:54.000000 cryptonita-0.6.3/cryptonita/attacks/prng.py
+-rw-r--r--   0 user      (1000) user      (1000)     7892 2024-03-28 18:39:16.000000 cryptonita-0.6.3/cryptonita/bytestrings.py
+-rw-r--r--   0 user      (1000) user      (1000)    12508 2024-03-28 18:59:03.000000 cryptonita-0.6.3/cryptonita/conv.py
+-rw-r--r--   0 user      (1000) user      (1000)      461 2024-03-28 19:08:17.000000 cryptonita-0.6.3/cryptonita/deps.py
+-rw-r--r--   0 user      (1000) user      (1000)    14291 2023-01-14 13:34:40.000000 cryptonita-0.6.3/cryptonita/fuzzy_set.py
+-rw-r--r--   0 user      (1000) user      (1000)     3502 2022-06-20 20:45:28.000000 cryptonita-0.6.3/cryptonita/helpers.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-04-25 14:54:50.555534 cryptonita-0.6.3/cryptonita/metrics/
+-rw-r-----   0 user      (1000) user      (1000)     7963 2022-06-23 23:13:08.000000 cryptonita-0.6.3/cryptonita/metrics/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)    19979 2023-04-06 22:33:46.000000 cryptonita-0.6.3/cryptonita/mixins.py
+-rw-r--r--   0 user      (1000) user      (1000)      936 2024-03-28 18:39:16.000000 cryptonita-0.6.3/cryptonita/mod.py
+-rw-r--r--   0 user      (1000) user      (1000)     3989 2022-06-20 19:51:05.000000 cryptonita-0.6.3/cryptonita/plots.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-04-25 14:54:50.559536 cryptonita-0.6.3/cryptonita/scoring/
+-rw-r--r--   0 user      (1000) user      (1000)     1070 2023-01-14 01:18:26.000000 cryptonita-0.6.3/cryptonita/scoring/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)     4031 2024-03-28 18:37:21.000000 cryptonita-0.6.3/cryptonita/scoring/freq.py
+-rw-r--r--   0 user      (1000) user      (1000)    10884 2024-03-28 18:39:16.000000 cryptonita-0.6.3/cryptonita/scoring/score_funcs.py
+-rw-r--r--   0 user      (1000) user      (1000)     6925 2024-03-20 14:47:10.000000 cryptonita-0.6.3/cryptonita/space.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-04-25 14:54:50.559536 cryptonita-0.6.3/cryptonita/stats/
+-rw-r--r--   0 user      (1000) user      (1000)     1444 2022-06-20 19:51:05.000000 cryptonita-0.6.3/cryptonita/stats/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)    12129 2022-06-20 19:51:05.000000 cryptonita-0.6.3/cryptonita/stats/kasiski.py
+-rw-r--r--   0 user      (1000) user      (1000)     1670 2022-06-20 19:51:05.000000 cryptonita-0.6.3/cryptonita/suggesters.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-04-25 14:54:50.563538 cryptonita-0.6.3/cryptonita/toys/
+-rw-r--r--   0 user      (1000) user      (1000)       76 2022-06-20 19:51:05.000000 cryptonita-0.6.3/cryptonita/toys/__init__.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-04-25 14:54:50.567540 cryptonita-0.6.3/cryptonita/toys/hashes/
+-rw-r--r--   0 user      (1000) user      (1000)        0 2023-03-17 18:19:17.000000 cryptonita-0.6.3/cryptonita/toys/hashes/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)      288 2024-03-20 13:14:32.000000 cryptonita-0.6.3/cryptonita/toys/hashes/keyed.py
+-rw-r--r--   0 user      (1000) user      (1000)     3571 2024-03-20 13:13:37.000000 cryptonita-0.6.3/cryptonita/toys/hashes/md4.py
+-rw-r--r--   0 user      (1000) user      (1000)     3108 2024-03-20 13:12:45.000000 cryptonita-0.6.3/cryptonita/toys/hashes/sha1.py
+-rw-r--r--   0 user      (1000) user      (1000)     6166 2024-03-20 13:14:32.000000 cryptonita-0.6.3/cryptonita/toys/hashes/sha256.py
+-rw-r--r--   0 user      (1000) user      (1000)     4924 2024-03-28 18:39:16.000000 cryptonita-0.6.3/cryptonita/toys/substitution_ciphers.py
+-rw-r--r--   0 user      (1000) user      (1000)     3559 2024-03-28 18:38:08.000000 cryptonita-0.6.3/cryptonita/toys/transposition_ciphers.py
+-rw-r--r--   0 user      (1000) user      (1000)     8953 2023-01-19 23:25:36.000000 cryptonita-0.6.3/cryptonita/views.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-04-25 14:54:50.551533 cryptonita-0.6.3/cryptonita.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)    20469 2024-04-25 14:54:50.000000 cryptonita-0.6.3/cryptonita.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)     1034 2024-04-25 14:54:50.000000 cryptonita-0.6.3/cryptonita.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1000) user      (1000)        1 2024-04-25 14:54:50.000000 cryptonita-0.6.3/cryptonita.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1000) user      (1000)      104 2024-04-25 14:54:50.000000 cryptonita-0.6.3/cryptonita.egg-info/requires.txt
+-rw-r--r--   0 user      (1000) user      (1000)       11 2024-04-25 14:54:50.000000 cryptonita-0.6.3/cryptonita.egg-info/top_level.txt
+-rw-r--r--   0 user      (1000) user      (1000)       60 2023-03-17 21:20:42.000000 cryptonita-0.6.3/pyproject.toml
+-rw-r--r--   0 user      (1000) user      (1000)       38 2024-04-25 14:54:50.567540 cryptonita-0.6.3/setup.cfg
+-rw-r--r--   0 user      (1000) user      (1000)     2841 2024-03-28 18:43:39.000000 cryptonita-0.6.3/setup.py
```

### Comparing `cryptonita-0.6.2/PKG-INFO` & `cryptonita-0.6.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cryptonita
-Version: 0.6.2
+Version: 0.6.3
 Summary: Cryptanalysis swiss army knife
 Home-page: UNKNOWN
 Author: Di Paola Martin
 Author-email: use-github-issues@example.com
 License: GNU GPLv3
 Description: ``cryptonita`` - Cryptanalysis Swiss Army Knife
         ===============================================
```

### Comparing `cryptonita-0.6.2/README.rst` & `cryptonita-0.6.3/README.rst`

 * *Files identical despite different names*

### Comparing `cryptonita-0.6.2/cryptonita/__init__.py` & `cryptonita-0.6.3/cryptonita/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 '''Cryptanalysis swiss army knife'''
 
-__version__ = "0.6.2"
+__version__ = "0.6.3"
 
 _author = 'Di Paola Martin'
 _license = 'GNU GPLv3'
 _url = ' - '
 
 _license_disclaimer = r'''Copyright (C) {author} - {url}
```

### Comparing `cryptonita-0.6.2/cryptonita/attacks/__init__.py` & `cryptonita-0.6.3/cryptonita/attacks/__init__.py`

 * *Files identical despite different names*

### Comparing `cryptonita-0.6.2/cryptonita/attacks/block_ciphers.py` & `cryptonita-0.6.3/cryptonita/attacks/block_ciphers.py`

 * *Files identical despite different names*

### Comparing `cryptonita-0.6.2/cryptonita/attacks/mapping.py` & `cryptonita-0.6.3/cryptonita/attacks/mapping.py`

 * *Files identical despite different names*

### Comparing `cryptonita-0.6.2/cryptonita/attacks/prng.py` & `cryptonita-0.6.3/cryptonita/attacks/prng.py`

 * *Files 9% similar despite different names*

```diff
@@ -58,28 +58,28 @@
     return g
 
 
 def clone_mt19937(out):
     ''' Clone the internal state of a Mersenne Twister 19937 (MT19937)
         from its output <out>.
 
-        For MT19937 we need 624 sequential numbers at minimum to clone
+        For MT19937 we need 624 sequential numbers to clone
         the state.
 
             >>> from cryptonita.attacks.prng import clone_mt19937
             >>> clone_mt19937([1, 2, 3])           # byexample: +norm-ws
             Traceback <...>
-            ValueError: You need at least 624 numbers to clone the MT19937 PRNG
-                        but you have only 3.
+            ValueError: You need 624 numbers to clone the MT19937 PRNG
+                        but you provided 3.
         '''
 
     n = 624
-    if len(out) < n:
-        raise ValueError(("You need at least %i numbers to clone the MT19937 PRNG" +\
-                          " but you have only %i.") % (n, len(out)))
+    if len(out) != n:
+        raise ValueError(("You need %i numbers to clone the MT19937 PRNG" +\
+                          " but you provided %i.") % (n, len(out)))
 
     u, d = 11, 0xffffffff
     s, b = 7, 0x9d2c5680
     t, c = 15, 0xefc60000
     l = 18
 
     state = []
```

### Comparing `cryptonita-0.6.2/cryptonita/bytestrings.py` & `cryptonita-0.6.3/cryptonita/bytestrings.py`

 * *Files identical despite different names*

### Comparing `cryptonita-0.6.2/cryptonita/conv.py` & `cryptonita-0.6.3/cryptonita/conv.py`

 * *Files identical despite different names*

### Comparing `cryptonita-0.6.2/cryptonita/fuzzy_set.py` & `cryptonita-0.6.3/cryptonita/fuzzy_set.py`

 * *Files identical despite different names*

### Comparing `cryptonita-0.6.2/cryptonita/helpers.py` & `cryptonita-0.6.3/cryptonita/helpers.py`

 * *Files identical despite different names*

### Comparing `cryptonita-0.6.2/cryptonita/metrics/__init__.py` & `cryptonita-0.6.3/cryptonita/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `cryptonita-0.6.2/cryptonita/mixins.py` & `cryptonita-0.6.3/cryptonita/mixins.py`

 * *Files identical despite different names*

### Comparing `cryptonita-0.6.2/cryptonita/mod.py` & `cryptonita-0.6.3/cryptonita/mod.py`

 * *Files identical despite different names*

### Comparing `cryptonita-0.6.2/cryptonita/plots.py` & `cryptonita-0.6.3/cryptonita/plots.py`

 * *Files identical despite different names*

### Comparing `cryptonita-0.6.2/cryptonita/scoring/__init__.py` & `cryptonita-0.6.3/cryptonita/scoring/__init__.py`

 * *Files identical despite different names*

### Comparing `cryptonita-0.6.2/cryptonita/scoring/freq.py` & `cryptonita-0.6.3/cryptonita/scoring/freq.py`

 * *Files identical despite different names*

### Comparing `cryptonita-0.6.2/cryptonita/scoring/score_funcs.py` & `cryptonita-0.6.3/cryptonita/scoring/score_funcs.py`

 * *Files identical despite different names*

### Comparing `cryptonita-0.6.2/cryptonita/space.py` & `cryptonita-0.6.3/cryptonita/space.py`

 * *Files identical despite different names*

### Comparing `cryptonita-0.6.2/cryptonita/stats/__init__.py` & `cryptonita-0.6.3/cryptonita/stats/__init__.py`

 * *Files identical despite different names*

### Comparing `cryptonita-0.6.2/cryptonita/stats/kasiski.py` & `cryptonita-0.6.3/cryptonita/stats/kasiski.py`

 * *Files identical despite different names*

### Comparing `cryptonita-0.6.2/cryptonita/suggesters.py` & `cryptonita-0.6.3/cryptonita/suggesters.py`

 * *Files identical despite different names*

### Comparing `cryptonita-0.6.2/cryptonita/toys/hashes/md4.py` & `cryptonita-0.6.3/cryptonita/toys/hashes/md4.py`

 * *Files identical despite different names*

### Comparing `cryptonita-0.6.2/cryptonita/toys/hashes/sha1.py` & `cryptonita-0.6.3/cryptonita/toys/hashes/sha1.py`

 * *Files identical despite different names*

### Comparing `cryptonita-0.6.2/cryptonita/toys/hashes/sha256.py` & `cryptonita-0.6.3/cryptonita/toys/hashes/sha256.py`

 * *Files identical despite different names*

### Comparing `cryptonita-0.6.2/cryptonita/toys/substitution_ciphers.py` & `cryptonita-0.6.3/cryptonita/toys/substitution_ciphers.py`

 * *Files identical despite different names*

### Comparing `cryptonita-0.6.2/cryptonita/toys/transposition_ciphers.py` & `cryptonita-0.6.3/cryptonita/toys/transposition_ciphers.py`

 * *Files identical despite different names*

### Comparing `cryptonita-0.6.2/cryptonita/views.py` & `cryptonita-0.6.3/cryptonita/views.py`

 * *Files identical despite different names*

### Comparing `cryptonita-0.6.2/cryptonita.egg-info/PKG-INFO` & `cryptonita-0.6.3/cryptonita.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cryptonita
-Version: 0.6.2
+Version: 0.6.3
 Summary: Cryptanalysis swiss army knife
 Home-page: UNKNOWN
 Author: Di Paola Martin
 Author-email: use-github-issues@example.com
 License: GNU GPLv3
 Description: ``cryptonita`` - Cryptanalysis Swiss Army Knife
         ===============================================
```

### Comparing `cryptonita-0.6.2/cryptonita.egg-info/SOURCES.txt` & `cryptonita-0.6.3/cryptonita.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cryptonita-0.6.2/setup.py` & `cryptonita-0.6.3/setup.py`

 * *Files identical despite different names*


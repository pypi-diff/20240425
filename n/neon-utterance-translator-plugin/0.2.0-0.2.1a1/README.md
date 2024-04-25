# Comparing `tmp/neon_utterance_translator_plugin-0.2.0.tar.gz` & `tmp/neon_utterance_translator_plugin-0.2.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon_utterance_translator_plugin-0.2.0.tar", last modified: Sat Dec 16 01:06:35 2023, max compression
+gzip compressed data, was "neon_utterance_translator_plugin-0.2.1a1.tar", last modified: Thu Apr 25 18:31:40 2024, max compression
```

## Comparing `neon_utterance_translator_plugin-0.2.0.tar` & `neon_utterance_translator_plugin-0.2.1a1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 01:06:35.901316 neon_utterance_translator_plugin-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)      533 2023-12-16 01:06:35.901316 neon_utterance_translator_plugin-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      129 2023-12-16 01:06:32.000000 neon_utterance_translator_plugin-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 01:06:35.901316 neon_utterance_translator_plugin-0.2.0/neon_utterance_translator_plugin/
--rw-r--r--   0 runner    (1001) docker     (127)     5952 2023-12-16 01:06:32.000000 neon_utterance_translator_plugin-0.2.0/neon_utterance_translator_plugin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 01:06:35.901316 neon_utterance_translator_plugin-0.2.0/neon_utterance_translator_plugin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      533 2023-12-16 01:06:35.000000 neon_utterance_translator_plugin-0.2.0/neon_utterance_translator_plugin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      452 2023-12-16 01:06:35.000000 neon_utterance_translator_plugin-0.2.0/neon_utterance_translator_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-16 01:06:35.000000 neon_utterance_translator_plugin-0.2.0/neon_utterance_translator_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      107 2023-12-16 01:06:35.000000 neon_utterance_translator_plugin-0.2.0/neon_utterance_translator_plugin.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2023-12-16 01:06:35.000000 neon_utterance_translator_plugin-0.2.0/neon_utterance_translator_plugin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2023-12-16 01:06:35.000000 neon_utterance_translator_plugin-0.2.0/neon_utterance_translator_plugin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-16 01:06:35.000000 neon_utterance_translator_plugin-0.2.0/neon_utterance_translator_plugin.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-16 01:06:35.901316 neon_utterance_translator_plugin-0.2.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     3972 2023-12-16 01:06:32.000000 neon_utterance_translator_plugin-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:31:40.865698 neon_utterance_translator_plugin-0.2.1a1/
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-25 18:31:40.865698 neon_utterance_translator_plugin-0.2.1a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-25 18:31:34.000000 neon_utterance_translator_plugin-0.2.1a1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:31:40.865698 neon_utterance_translator_plugin-0.2.1a1/neon_utterance_translator_plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)     5956 2024-04-25 18:31:34.000000 neon_utterance_translator_plugin-0.2.1a1/neon_utterance_translator_plugin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:31:40.865698 neon_utterance_translator_plugin-0.2.1a1/neon_utterance_translator_plugin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-25 18:31:40.000000 neon_utterance_translator_plugin-0.2.1a1/neon_utterance_translator_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-25 18:31:40.000000 neon_utterance_translator_plugin-0.2.1a1/neon_utterance_translator_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 18:31:40.000000 neon_utterance_translator_plugin-0.2.1a1/neon_utterance_translator_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-25 18:31:40.000000 neon_utterance_translator_plugin-0.2.1a1/neon_utterance_translator_plugin.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-25 18:31:40.000000 neon_utterance_translator_plugin-0.2.1a1/neon_utterance_translator_plugin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-25 18:31:40.000000 neon_utterance_translator_plugin-0.2.1a1/neon_utterance_translator_plugin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 18:31:40.000000 neon_utterance_translator_plugin-0.2.1a1/neon_utterance_translator_plugin.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 18:31:40.865698 neon_utterance_translator_plugin-0.2.1a1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3972 2024-04-25 18:31:34.000000 neon_utterance_translator_plugin-0.2.1a1/setup.py
```

### Comparing `neon_utterance_translator_plugin-0.2.0/PKG-INFO` & `neon_utterance_translator_plugin-0.2.1a1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon_utterance_translator_plugin
-Version: 0.2.0
+Version: 0.2.1a1
 Summary: A utterance parser/classifier/transformer plugin for ovos/neon/mycroft
 Home-page: https://github.com/NeonGeckoCom/neon_utterance_translator_plugin
 Author: Neongecko
 Author-email: developers@neon.ai
 License: bsd3
 Keywords: mycroft plugin utterance parser/classifier/transformer
 Description-Content-Type: text/markdown
```

### Comparing `neon_utterance_translator_plugin-0.2.0/neon_utterance_translator_plugin/__init__.py` & `neon_utterance_translator_plugin-0.2.1a1/neon_utterance_translator_plugin/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,10 +106,10 @@
                     "internal": self.internal_lang,
                     "was_translated": was_translated,
                     "raw_utterance": original,
                     "translated_utterance": utterances[idx]
 
                 }]
             except Exception as e:
-                LOG.error(e)
+                LOG.exception(e)
         # return translated utterances + data
         return utterances, {"translation_data": metadata}
```

### Comparing `neon_utterance_translator_plugin-0.2.0/neon_utterance_translator_plugin.egg-info/PKG-INFO` & `neon_utterance_translator_plugin-0.2.1a1/neon_utterance_translator_plugin.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-utterance-translator-plugin
-Version: 0.2.0
+Version: 0.2.1a1
 Summary: A utterance parser/classifier/transformer plugin for ovos/neon/mycroft
 Home-page: https://github.com/NeonGeckoCom/neon_utterance_translator_plugin
 Author: Neongecko
 Author-email: developers@neon.ai
 License: bsd3
 Keywords: mycroft plugin utterance parser/classifier/transformer
 Description-Content-Type: text/markdown
```

### Comparing `neon_utterance_translator_plugin-0.2.0/setup.py` & `neon_utterance_translator_plugin-0.2.1a1/setup.py`

 * *Files identical despite different names*


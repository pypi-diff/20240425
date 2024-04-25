# Comparing `tmp/suricata-language-server-0.9.2.tar.gz` & `tmp/suricata_language_server-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "suricata-language-server-0.9.2.tar", last modified: Tue Feb 20 10:22:04 2024, max compression
+gzip compressed data, was "suricata_language_server-0.9.3.tar", last modified: Thu Apr 25 06:21:31 2024, max compression
```

## Comparing `suricata-language-server-0.9.2.tar` & `suricata_language_server-0.9.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 eric      (1000) eric      (1000)        0 2024-02-20 10:22:04.992640 suricata-language-server-0.9.2/
--rw-r--r--   0 eric      (1000) eric      (1000)    35147 2022-01-10 22:02:29.000000 suricata-language-server-0.9.2/LICENSE
--rw-r--r--   0 eric      (1000) eric      (1000)     8786 2024-02-20 10:22:04.992640 suricata-language-server-0.9.2/PKG-INFO
--rw-r--r--   0 eric      (1000) eric      (1000)     8097 2023-09-12 06:54:59.000000 suricata-language-server-0.9.2/README.rst
--rw-r--r--   0 eric      (1000) eric      (1000)      109 2022-01-10 22:02:29.000000 suricata-language-server-0.9.2/pyproject.toml
--rw-r--r--   0 eric      (1000) eric      (1000)      875 2024-02-20 10:22:04.996640 suricata-language-server-0.9.2/setup.cfg
-drwxr-xr-x   0 eric      (1000) eric      (1000)        0 2024-02-20 10:22:04.992640 suricata-language-server-0.9.2/suricata_language_server.egg-info/
--rw-r--r--   0 eric      (1000) eric      (1000)     8786 2024-02-20 10:22:04.000000 suricata-language-server-0.9.2/suricata_language_server.egg-info/PKG-INFO
--rw-r--r--   0 eric      (1000) eric      (1000)      507 2024-02-20 10:22:04.000000 suricata-language-server-0.9.2/suricata_language_server.egg-info/SOURCES.txt
--rw-r--r--   0 eric      (1000) eric      (1000)        1 2024-02-20 10:22:04.000000 suricata-language-server-0.9.2/suricata_language_server.egg-info/dependency_links.txt
--rw-r--r--   0 eric      (1000) eric      (1000)       70 2024-02-20 10:22:04.000000 suricata-language-server-0.9.2/suricata_language_server.egg-info/entry_points.txt
--rw-r--r--   0 eric      (1000) eric      (1000)       11 2024-02-20 10:22:04.000000 suricata-language-server-0.9.2/suricata_language_server.egg-info/top_level.txt
--rw-r--r--   0 eric      (1000) eric      (1000)        1 2022-01-10 22:38:25.000000 suricata-language-server-0.9.2/suricata_language_server.egg-info/zip-safe
-drwxr-xr-x   0 eric      (1000) eric      (1000)        0 2024-02-20 10:22:04.992640 suricata-language-server-0.9.2/suricatals/
--rw-r--r--   0 eric      (1000) eric      (1000)     3634 2024-02-20 10:18:42.000000 suricata-language-server-0.9.2/suricatals/__init__.py
--rw-r--r--   0 eric      (1000) eric      (1000)     8996 2023-03-20 20:54:57.000000 suricata-language-server-0.9.2/suricatals/jsonrpc.py
--rw-r--r--   0 eric      (1000) eric      (1000)    18287 2024-02-20 10:19:09.000000 suricata-language-server-0.9.2/suricatals/langserver.py
--rw-r--r--   0 eric      (1000) eric      (1000)     2812 2023-10-20 09:12:26.000000 suricata-language-server-0.9.2/suricatals/lsp_helpers.py
--rw-r--r--   0 eric      (1000) eric      (1000)    16235 2024-02-20 10:19:09.000000 suricata-language-server-0.9.2/suricatals/parse_signatures.py
--rw-r--r--   0 eric      (1000) eric      (1000)    35772 2024-02-20 10:18:42.000000 suricata-language-server-0.9.2/suricatals/tests_rules.py
--rw-r--r--   0 eric      (1000) eric      (1000)     2522 2024-02-20 10:18:42.000000 suricata-language-server-0.9.2/suricatals/unit_tests.py
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2024-04-25 06:21:31.239220 suricata_language_server-0.9.3/
+-rw-r--r--   0 eric      (1000) eric      (1000)    35147 2021-12-31 12:35:43.000000 suricata_language_server-0.9.3/LICENSE
+-rw-r--r--   0 eric      (1000) eric      (1000)     8786 2024-04-25 06:21:31.239220 suricata_language_server-0.9.3/PKG-INFO
+-rw-r--r--   0 eric      (1000) eric      (1000)     8097 2023-07-12 07:06:35.000000 suricata_language_server-0.9.3/README.rst
+-rw-r--r--   0 eric      (1000) eric      (1000)      109 2022-01-02 10:25:28.000000 suricata_language_server-0.9.3/pyproject.toml
+-rw-rw-r--   0 eric      (1000) eric      (1000)      875 2024-04-25 06:21:31.239220 suricata_language_server-0.9.3/setup.cfg
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2024-04-25 06:21:31.239220 suricata_language_server-0.9.3/suricata_language_server.egg-info/
+-rw-r--r--   0 eric      (1000) eric      (1000)     8786 2024-04-25 06:21:31.000000 suricata_language_server-0.9.3/suricata_language_server.egg-info/PKG-INFO
+-rw-r--r--   0 eric      (1000) eric      (1000)      507 2024-04-25 06:21:31.000000 suricata_language_server-0.9.3/suricata_language_server.egg-info/SOURCES.txt
+-rw-r--r--   0 eric      (1000) eric      (1000)        1 2024-04-25 06:21:31.000000 suricata_language_server-0.9.3/suricata_language_server.egg-info/dependency_links.txt
+-rw-r--r--   0 eric      (1000) eric      (1000)       70 2024-04-25 06:21:31.000000 suricata_language_server-0.9.3/suricata_language_server.egg-info/entry_points.txt
+-rw-r--r--   0 eric      (1000) eric      (1000)       11 2024-04-25 06:21:31.000000 suricata_language_server-0.9.3/suricata_language_server.egg-info/top_level.txt
+-rw-r--r--   0 eric      (1000) eric      (1000)        1 2022-01-02 10:45:30.000000 suricata_language_server-0.9.3/suricata_language_server.egg-info/zip-safe
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2024-04-25 06:21:31.239220 suricata_language_server-0.9.3/suricatals/
+-rw-rw-r--   0 eric      (1000) eric      (1000)     3634 2024-04-25 06:17:51.000000 suricata_language_server-0.9.3/suricatals/__init__.py
+-rw-r--r--   0 eric      (1000) eric      (1000)     8996 2023-03-19 21:57:26.000000 suricata_language_server-0.9.3/suricatals/jsonrpc.py
+-rw-rw-r--   0 eric      (1000) eric      (1000)    18287 2024-04-23 16:19:31.000000 suricata_language_server-0.9.3/suricatals/langserver.py
+-rw-rw-r--   0 eric      (1000) eric      (1000)     2812 2024-04-23 16:19:31.000000 suricata_language_server-0.9.3/suricatals/lsp_helpers.py
+-rw-rw-r--   0 eric      (1000) eric      (1000)    16235 2024-04-23 16:19:31.000000 suricata_language_server-0.9.3/suricatals/parse_signatures.py
+-rw-rw-r--   0 eric      (1000) eric      (1000)    35918 2024-04-25 06:17:14.000000 suricata_language_server-0.9.3/suricatals/tests_rules.py
+-rw-rw-r--   0 eric      (1000) eric      (1000)     2522 2024-04-23 16:19:31.000000 suricata_language_server-0.9.3/suricatals/unit_tests.py
```

### Comparing `suricata-language-server-0.9.2/LICENSE` & `suricata_language_server-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `suricata-language-server-0.9.2/PKG-INFO` & `suricata_language_server-0.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: suricata-language-server
-Version: 0.9.2
+Version: 0.9.3
 Summary: Suricata Signatures Language Server for the Language Server Protocol
 Home-page: https://github.com/StamusNetworks/suricata-language-server
 Author: Eric Leblond
 Author-email: el@stamus-networks.com
 License: GNU General Public License v3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```

### Comparing `suricata-language-server-0.9.2/README.rst` & `suricata_language_server-0.9.3/README.rst`

 * *Files identical despite different names*

### Comparing `suricata-language-server-0.9.2/setup.cfg` & `suricata_language_server-0.9.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = suricata-language-server
-version = 0.9.2
+version = 0.9.3
 description = Suricata Signatures Language Server for the Language Server Protocol
 long_description = file: README.rst
 license = GNU General Public License v3
 classifiers = 
 	License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 	Programming Language :: Python :: 3
 	Development Status :: 4 - Beta
```

### Comparing `suricata-language-server-0.9.2/suricata_language_server.egg-info/PKG-INFO` & `suricata_language_server-0.9.3/suricata_language_server.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: suricata-language-server
-Version: 0.9.2
+Version: 0.9.3
 Summary: Suricata Signatures Language Server for the Language Server Protocol
 Home-page: https://github.com/StamusNetworks/suricata-language-server
 Author: Eric Leblond
 Author-email: el@stamus-networks.com
 License: GNU General Public License v3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```

### Comparing `suricata-language-server-0.9.2/suricatals/__init__.py` & `suricata_language_server-0.9.3/suricatals/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 """
 
 import sys
 import argparse
 from suricatals.langserver import LangServer
 from suricatals.jsonrpc import JSONRPC2Connection, ReadWriter
 import json
-__version__ = '0.9.2'
+__version__ = '0.9.3'
 
 
 def error_exit(error_str):
     print("ERROR: {0}".format(error_str))
     sys.exit(-1)
```

### Comparing `suricata-language-server-0.9.2/suricatals/jsonrpc.py` & `suricata_language_server-0.9.3/suricatals/jsonrpc.py`

 * *Files identical despite different names*

### Comparing `suricata-language-server-0.9.2/suricatals/langserver.py` & `suricata_language_server-0.9.3/suricatals/langserver.py`

 * *Files identical despite different names*

### Comparing `suricata-language-server-0.9.2/suricatals/lsp_helpers.py` & `suricata_language_server-0.9.3/suricatals/lsp_helpers.py`

 * *Files identical despite different names*

### Comparing `suricata-language-server-0.9.2/suricatals/parse_signatures.py` & `suricata_language_server-0.9.3/suricatals/parse_signatures.py`

 * *Files identical despite different names*

### Comparing `suricata-language-server-0.9.2/suricatals/tests_rules.py` & `suricata_language_server-0.9.3/suricatals/tests_rules.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,21 +47,26 @@
   - console:
       enabled: yes
       type: json
 app-layer:
   protocols:
     tls:
       ja3-fingerprints: yes
+security:
+  lua:
+    allow-rules: yes
 engine-analysis:
   rules-fast-pattern: yes
   rules: yes
 vars:
   address-groups:
     HOME_NET: "[192.168.0.0/16,10.0.0.0/8,172.16.0.0/12]"
     EXTERNAL_NET: "!$HOME_NET"
+    SCANNERS: "127.0.0.1"
+    DC_SERVERS: "127.0.0.1"
     HTTP_SERVERS: "$HOME_NET"
     SMTP_SERVERS: "$HOME_NET"
     SQL_SERVERS: "$HOME_NET"
     DNS_SERVERS: "$HOME_NET"
     TELNET_SERVERS: "$HOME_NET"
     AIM_SERVERS: "$EXTERNAL_NET"
     DNP3_SERVER: "$HOME_NET"
@@ -449,18 +454,19 @@
 
         suri_cmd = [self.suricata_binary, '--engine-analysis', '-l', tmpdir, '-S', rule_file, '-c', config_file]
         suriprocess = subprocess.Popen(suri_cmd, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
         suriprocess.communicate()
 
         res = {}
         json_path = os.path.join(tmpdir, 'rules.json')
-        with open(json_path, 'r', encoding='utf-8') as f:
-            for line in f.readlines():
-                content = json.loads(line)
-                res[content['id']] = content
+        if os.path.exists(json_path):
+            with open(json_path, 'r', encoding='utf-8') as f:
+                for line in f.readlines():
+                    content = json.loads(line)
+                    res[content['id']] = content
 
         return res
 
     def rule_buffer(self, rule_buffer, engine_analysis=True, config_buffer=None, related_files=None,
                     reference_config=None, classification_config=None, extra_buffers=None):
         tmpdir = tempfile.mkdtemp()
         config_file = self._prepare_conf(
```

### Comparing `suricata-language-server-0.9.2/suricatals/unit_tests.py` & `suricata_language_server-0.9.3/suricatals/unit_tests.py`

 * *Files identical despite different names*


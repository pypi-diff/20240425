# Comparing `tmp/colabexts-0.11800000000000002.tar.gz` & `tmp/colabexts-0.12100000000000002.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/colabexts-0.11800000000000002.tar", last modified: Sun Sep  5 18:43:32 2021, max compression
+gzip compressed data, was "colabexts-0.12100000000000002.tar", last modified: Thu Apr 25 19:23:31 2024, max compression
```

## Comparing `colabexts-0.11800000000000002.tar` & `colabexts-0.12100000000000002.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 snarayan   (501) wheel        (0)        0 2021-09-05 18:43:32.710025 colabexts-0.11800000000000002/
--rw-r--r--   0 snarayan   (501) wheel        (0)      769 2021-09-05 18:43:32.709711 colabexts-0.11800000000000002/PKG-INFO
--rw-r--r--   0 snarayan   (501) wheel        (0)     1081 2021-09-05 18:40:14.000000 colabexts-0.11800000000000002/README.md
-drwxr-xr-x   0 snarayan   (501) wheel        (0)        0 2021-09-05 18:43:32.707646 colabexts-0.11800000000000002/colabexts/
--rw-r--r--   0 snarayan   (501) wheel        (0)        0 2021-09-05 18:40:14.000000 colabexts-0.11800000000000002/colabexts/__init__.py
--rw-r--r--   0 snarayan   (501) wheel        (0)    11411 2021-09-05 18:40:14.000000 colabexts-0.11800000000000002/colabexts/jcommon.ipynb
--rw-r--r--   0 snarayan   (501) wheel        (0)     3707 2021-09-05 18:40:14.000000 colabexts-0.11800000000000002/colabexts/jcommon.py
--rw-r--r--   0 snarayan   (501) wheel        (0)      454 2021-09-05 18:42:16.000000 colabexts-0.11800000000000002/colabexts/log.py
--rw-r--r--   0 snarayan   (501) wheel        (0)       27 2021-09-05 18:43:31.000000 colabexts-0.11800000000000002/colabexts/version.txt
-drwxr-xr-x   0 snarayan   (501) wheel        (0)        0 2021-09-05 18:43:32.709298 colabexts-0.11800000000000002/colabexts.egg-info/
--rw-r--r--   0 snarayan   (501) wheel        (0)      769 2021-09-05 18:43:32.000000 colabexts-0.11800000000000002/colabexts.egg-info/PKG-INFO
--rw-r--r--   0 snarayan   (501) wheel        (0)      320 2021-09-05 18:43:32.000000 colabexts-0.11800000000000002/colabexts.egg-info/SOURCES.txt
--rw-r--r--   0 snarayan   (501) wheel        (0)        1 2021-09-05 18:43:32.000000 colabexts-0.11800000000000002/colabexts.egg-info/dependency_links.txt
--rw-r--r--   0 snarayan   (501) wheel        (0)        1 2021-09-05 18:43:32.000000 colabexts-0.11800000000000002/colabexts.egg-info/not-zip-safe
--rw-r--r--   0 snarayan   (501) wheel        (0)       20 2021-09-05 18:43:32.000000 colabexts-0.11800000000000002/colabexts.egg-info/requires.txt
--rw-r--r--   0 snarayan   (501) wheel        (0)       10 2021-09-05 18:43:32.000000 colabexts-0.11800000000000002/colabexts.egg-info/top_level.txt
--rw-r--r--   0 snarayan   (501) wheel        (0)       38 2021-09-05 18:43:32.710101 colabexts-0.11800000000000002/setup.cfg
--rw-r--r--   0 snarayan   (501) wheel        (0)     1678 2021-09-05 18:43:31.000000 colabexts-0.11800000000000002/setup.py
+drwxr-xr-x   0 snarayan   (501) wheel        (0)        0 2024-04-25 19:23:31.301974 colabexts-0.12100000000000002/
+-rw-r--r--   0 snarayan   (501) wheel        (0)      780 2024-04-25 19:23:31.301129 colabexts-0.12100000000000002/PKG-INFO
+-rw-r--r--   0 snarayan   (501) wheel        (0)     1081 2022-11-26 05:52:19.000000 colabexts-0.12100000000000002/README.md
+drwxr-xr-x   0 snarayan   (501) wheel        (0)        0 2024-04-25 19:23:31.298113 colabexts-0.12100000000000002/colabexts/
+-rw-r--r--   0 snarayan   (501) wheel        (0)        0 2022-11-26 05:52:19.000000 colabexts-0.12100000000000002/colabexts/__init__.py
+-rw-r--r--   0 snarayan   (501) wheel        (0)    11567 2024-04-23 12:55:18.000000 colabexts-0.12100000000000002/colabexts/jcommon.ipynb
+-rw-r--r--   0 snarayan   (501) wheel        (0)     4669 2024-04-23 12:57:14.000000 colabexts-0.12100000000000002/colabexts/jcommon.py
+-rw-r--r--   0 snarayan   (501) wheel        (0)      454 2022-11-26 05:52:19.000000 colabexts-0.12100000000000002/colabexts/log.py
+-rw-r--r--   0 snarayan   (501) wheel        (0)     3846 2024-04-23 21:58:20.000000 colabexts-0.12100000000000002/colabexts/utils.py
+-rw-r--r--   0 snarayan   (501) wheel        (0)       27 2024-04-25 19:23:31.000000 colabexts-0.12100000000000002/colabexts/version.txt
+drwxr-xr-x   0 snarayan   (501) wheel        (0)        0 2024-04-25 19:23:31.300711 colabexts-0.12100000000000002/colabexts.egg-info/
+-rw-r--r--   0 snarayan   (501) wheel        (0)      780 2024-04-25 19:23:31.000000 colabexts-0.12100000000000002/colabexts.egg-info/PKG-INFO
+-rw-r--r--   0 snarayan   (501) wheel        (0)      339 2024-04-25 19:23:31.000000 colabexts-0.12100000000000002/colabexts.egg-info/SOURCES.txt
+-rw-r--r--   0 snarayan   (501) wheel        (0)        1 2024-04-25 19:23:31.000000 colabexts-0.12100000000000002/colabexts.egg-info/dependency_links.txt
+-rw-r--r--   0 snarayan   (501) wheel        (0)        1 2024-04-23 15:26:14.000000 colabexts-0.12100000000000002/colabexts.egg-info/not-zip-safe
+-rw-r--r--   0 snarayan   (501) wheel        (0)       20 2024-04-25 19:23:31.000000 colabexts-0.12100000000000002/colabexts.egg-info/requires.txt
+-rw-r--r--   0 snarayan   (501) wheel        (0)       10 2024-04-25 19:23:31.000000 colabexts-0.12100000000000002/colabexts.egg-info/top_level.txt
+-rw-r--r--   0 snarayan   (501) wheel        (0)       38 2024-04-25 19:23:31.302126 colabexts-0.12100000000000002/setup.cfg
+-rw-r--r--   0 snarayan   (501) wheel        (0)     1678 2024-04-25 19:23:31.000000 colabexts-0.12100000000000002/setup.py
```

### Comparing `colabexts-0.11800000000000002/PKG-INFO` & `colabexts-0.12100000000000002/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: colabexts
-Version: 0.11800000000000002
+Version: 0.12100000000000002
 Summary: Some simple Utilities
 Home-page: https://github.com/meyers007/colabext.git
 Author: Code Red
 Author-email: meyers@geospaces.org
 License: Apache License 2.0
-Description: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.2
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Requires-Dist: matplotlib
+Requires-Dist: openpyxl
```

### Comparing `colabexts-0.11800000000000002/README.md` & `colabexts-0.12100000000000002/README.md`

 * *Files identical despite different names*

### Comparing `colabexts-0.11800000000000002/colabexts/jcommon.ipynb` & `colabexts-0.12100000000000002/colabexts/jcommon.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8669351336236644%*

 * *Differences: {"'cells'": "{0: {'execution_count': 4}, 1: {'execution_count': 5, 'outputs': {0: {'data': "*

 * *            "{'text/html': {insert: [(10, '<!--\\n'), (27, '-->\\n'), (28, '<style>\\n'), (29, "*

 * *            "'\\n'), (30, '</style>\\n'), (32, '\\n')]}}}}, 'source': {insert: [(10, '<!--\\n'), "*

 * *            "(27, '-->\\n'), (28, '<style>\\n'), (29, '\\n'), (30, '</style>\\n'), (32, '\\n')]}}, "*

 * *            "2: {'source': {insert: [(5, '<link "*

 * *            'href="https://fonts.googleapis.com/css2?family=Roboto&displ […]*

```diff
@@ -1,24 +1,24 @@
 {
     "cells": [
         {
             "cell_type": "code",
-            "execution_count": 1,
+            "execution_count": 4,
             "metadata": {},
             "outputs": [],
             "source": [
                 "%reload_ext autoreload\n",
                 "%autoreload 2\n",
                 "%matplotlib inline\n",
                 "from colabexts.jcommon import *"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 20,
+            "execution_count": 5,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "\n",
                             "<textarea rows=5 id=nav_head_content style=\"width:100%;display:none;\">\n",
@@ -26,14 +26,15 @@
                             "a.bh,  a.bh:visited, a.bh:link, a.bh:active {\n",
                             "  ttext-decoration: none; \n",
                             "  color: black;\n",
                             "  font-family: 'Roboto','Heebo',Arial,sans-serif;\n",
                             "  font-size: 3em\n",
                             "}\n",
                             "</style>\n",
+                            "<!--\n",
                             "<div id='HTMLTopBar' style=\"    \n",
                             "    z-index: 50;\n",
                             "    align-items: stretch;\n",
                             "    width:100%\">\n",
                             "    <div  style=\"\n",
                             "        text-color: black;\n",
                             "        background-color: #fefefe;\n",
@@ -42,16 +43,21 @@
                             "        box-shadow: 5px 1px #ccc;\n",
                             "        height: 40px; left: 0; \n",
                             "        padding: 14px;\n",
                             "        \"\n",
                             "    >\n",
                             "    <a class=bh1 href=\"#\" onclick=\"$('#maintoolbar').toggle();\">X</a>\n",
                             "</div>\n",
+                            "-->\n",
+                            "<style>\n",
+                            "\n",
+                            "</style>\n",
                             "</textarea>\n",
                             "\n",
+                            "\n",
                             "<script>\n",
                             "if ($('#nav_head').length < 1) {\n",
                             "    $('#notebook-container').prepend('<div id=\"nav_head\" style=\"width:100%;\">.</div>')\n",
                             "    console.log(\"Added a div\")\n",
                             "} else{\n",
                             "    console.log(\"Already Added\")    \n",
                             "}\n",
@@ -76,14 +82,15 @@
                 "a.bh,  a.bh:visited, a.bh:link, a.bh:active {\n",
                 "  ttext-decoration: none; \n",
                 "  color: black;\n",
                 "  font-family: 'Roboto','Heebo',Arial,sans-serif;\n",
                 "  font-size: 3em\n",
                 "}\n",
                 "</style>\n",
+                "<!--\n",
                 "<div id='HTMLTopBar' style=\"    \n",
                 "    z-index: 50;\n",
                 "    align-items: stretch;\n",
                 "    width:100%\">\n",
                 "    <div  style=\"\n",
                 "        text-color: black;\n",
                 "        background-color: #fefefe;\n",
@@ -92,16 +99,21 @@
                 "        box-shadow: 5px 1px #ccc;\n",
                 "        height: 40px; left: 0; \n",
                 "        padding: 14px;\n",
                 "        \"\n",
                 "    >\n",
                 "    <a class=bh1 href=\"#\" onclick=\"$('#maintoolbar').toggle();\">X</a>\n",
                 "</div>\n",
+                "-->\n",
+                "<style>\n",
+                "\n",
+                "</style>\n",
                 "</textarea>\n",
                 "\n",
+                "\n",
                 "<script>\n",
                 "if ($('#nav_head').length < 1) {\n",
                 "    $('#notebook-container').prepend('<div id=\"nav_head\" style=\"width:100%;\">.</div>')\n",
                 "    console.log(\"Added a div\")\n",
                 "} else{\n",
                 "    console.log(\"Already Added\")    \n",
                 "}\n",
@@ -160,16 +172,15 @@
             ],
             "source": [
                 "%%HTML\n",
                 "<style>\n",
                 "@import url('https://fonts.googleapis.com/css2?family=Roboto&display=swap');\n",
                 "</style>\n",
                 "<style>\n",
-                "<link href=\"https://fonts.googleapis.com/css2?family=Roboto&display=swap\" \n",
-                "                            rel=\"stylesheet\">\n",
+                "<link href=\"https://fonts.googleapis.com/css2?family=Roboto&display=swap\" rel=\"stylesheet\">\n",
                 "\n",
                 "body  p ol li {\n",
                 "    font-family: \"Roboto\",  \"Lucida Grande\", \"Lucida Sans Unicode\";\n",
                 "    font-size: 14px;\n",
                 "    background: #fff\n",
                 "}\n",
                 "\n",
@@ -358,29 +369,29 @@
             "source": []
         }
     ],
     "metadata": {
         "anaconda-cloud": {},
         "hide_input": false,
         "kernelspec": {
-            "display_name": "Python 3",
+            "display_name": "Python 3 (ipykernel)",
             "language": "python",
             "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.7.3"
+            "version": "3.11.8"
         },
         "latex_envs": {
             "LaTeX_envs_menu_present": true,
             "autoclose": false,
             "autocomplete": true,
             "bibliofile": "biblio.bib",
             "cite_by": "number",
@@ -412,9 +423,9 @@
                 "width": "248.026px"
             },
             "toc_section_display": "block",
             "toc_window_display": true
         }
     },
     "nbformat": 4,
-    "nbformat_minor": 1
+    "nbformat_minor": 4
 }
```

### Comparing `colabexts-0.11800000000000002/colabexts/jcommon.py` & `colabexts-0.12100000000000002/colabexts/jcommon.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 import pandas as pd
 from datetime import timedelta;
 from collections import defaultdict
 from pylab import rcParams
 import matplotlib.pyplot as plt
 import urllib.request;
 from random import randint
-from collections import defaultdict
 from pylab import rcParams
 import warnings
 warnings.filterwarnings('ignore')
 
 matplotlib.rcParams['figure.figsize'] = (16, 5)
 matplotlib.rcParams['axes.grid'] = True
 
@@ -112,8 +111,33 @@
 #--------------------------------------------------------------------------------
 def is_number(s):
     try:
         float(s)
         return True
     except ValueError:
         return False
+#--------------------------------------------------------------------------------
+def encrypt(msg_text = b'message', secret_key='password'):
+    if (type(msg_text) == str):
+        msg_text = bytes(msg_text, encoding='utf-8').rjust(32)
+    if (type(secret_key) == str):
+        secret_key = bytes(secret_key, encoding='utf-8') .rjust(32)
+
+    cipher = AES.new(secret_key,AES.MODE_ECB) 
+    encoded = base64.b64encode(cipher.encrypt(msg_text))
+    ret = encoded.decode("utf-8")
+    print(ret)
+    return ret
 
+#--------------------------------------------------------------------------------
+def decrypt(encoded, secret_key='password'):
+    if (type(secret_key) == str):
+        secret_key = bytes(secret_key, encoding='utf-8') .rjust(32)
+
+    cipher = AES.new(secret_key,AES.MODE_ECB) 
+    if (type(encoded) == str):
+        encoded = bytes(encoded, encoding='utf-8')
+    decoded = cipher.decrypt(base64.b64decode(encoded))
+    ret =decoded.decode("utf-8").strip()
+    print(ret)
+    return ret
+
```

### Comparing `colabexts-0.11800000000000002/colabexts.egg-info/PKG-INFO` & `colabexts-0.12100000000000002/colabexts.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: colabexts
-Version: 0.11800000000000002
+Version: 0.12100000000000002
 Summary: Some simple Utilities
 Home-page: https://github.com/meyers007/colabext.git
 Author: Code Red
 Author-email: meyers@geospaces.org
 License: Apache License 2.0
-Description: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.2
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Requires-Dist: matplotlib
+Requires-Dist: openpyxl
```

### Comparing `colabexts-0.11800000000000002/setup.py` & `colabexts-0.12100000000000002/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-version=0.11800000000000002
+version=0.12100000000000002
 
 setup(name='colabexts', 
       version=str(version), 
       description='Some simple Utilities',
       url='https://github.com/meyers007/colabext.git',
       author='Code Red',
       author_email='meyers@geospaces.org',
```


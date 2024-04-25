# Comparing `tmp/fonttoolsWB-0.2.4.tar.gz` & `tmp/fonttoolswb-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fonttoolsWB-0.2.4.tar", last modified: Tue Mar 26 15:10:06 2024, max compression
+gzip compressed data, was "fonttoolswb-0.2.5.tar", last modified: Thu Apr 25 16:23:52 2024, max compression
```

## Comparing `fonttoolsWB-0.2.4.tar` & `fonttoolswb-0.2.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 15:10:06.175152 fonttoolsWB-0.2.4/
--rw-rw-rw-   0 root         (0) root         (0)     1079 2024-03-26 15:10:04.000000 fonttoolsWB-0.2.4/LICENSE
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 15:10:06.170152 fonttoolsWB-0.2.4/Lib/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 15:10:06.172152 fonttoolsWB-0.2.4/Lib/fonttoolsWB/
--rw-rw-rw-   0 root         (0) root         (0)      335 2024-03-26 15:10:04.000000 fonttoolsWB-0.2.4/Lib/fonttoolsWB/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 15:10:06.174152 fonttoolsWB-0.2.4/Lib/fonttoolsWB/data/
--rw-rw-rw-   0 root         (0) root         (0)       98 2024-03-26 15:10:04.000000 fonttoolsWB-0.2.4/Lib/fonttoolsWB/data/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      631 2024-03-26 15:10:04.000000 fonttoolsWB-0.2.4/Lib/fonttoolsWB/data/application.yml
--rw-rw-rw-   0 root         (0) root         (0)     2379 2024-03-26 15:10:04.000000 fonttoolsWB-0.2.4/Lib/fonttoolsWB/data/firstRun.py
--rw-rw-rw-   0 root         (0) root         (0)     9767 2024-03-26 15:10:04.000000 fonttoolsWB-0.2.4/Lib/fonttoolsWB/data/splashscreen.png
--rw-rw-rw-   0 root         (0) root         (0)      319 2024-03-26 15:10:04.000000 fonttoolsWB-0.2.4/Lib/fonttoolsWB/gui.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 15:10:06.174152 fonttoolsWB-0.2.4/Lib/fonttoolsWB.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3076 2024-03-26 15:10:06.000000 fonttoolsWB-0.2.4/Lib/fonttoolsWB.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      485 2024-03-26 15:10:06.000000 fonttoolsWB-0.2.4/Lib/fonttoolsWB.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-26 15:10:06.000000 fonttoolsWB-0.2.4/Lib/fonttoolsWB.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       96 2024-03-26 15:10:06.000000 fonttoolsWB-0.2.4/Lib/fonttoolsWB.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      185 2024-03-26 15:10:06.000000 fonttoolsWB-0.2.4/Lib/fonttoolsWB.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2024-03-26 15:10:06.000000 fonttoolsWB-0.2.4/Lib/fonttoolsWB.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     3076 2024-03-26 15:10:06.175152 fonttoolsWB-0.2.4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1154 2024-03-26 15:10:04.000000 fonttoolsWB-0.2.4/README.md
--rw-rw-rw-   0 root         (0) root         (0)     2467 2024-03-26 15:10:06.176152 fonttoolsWB-0.2.4/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       39 2024-03-26 15:10:04.000000 fonttoolsWB-0.2.4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 15:10:06.174152 fonttoolsWB-0.2.4/tests/
--rw-rw-rw-   0 root         (0) root         (0)      342 2024-03-26 15:10:04.000000 fonttoolsWB-0.2.4/tests/test_plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 16:23:52.429727 fonttoolswb-0.2.5/
+-rw-rw-rw-   0 root         (0) root         (0)     1079 2024-04-25 16:23:51.000000 fonttoolswb-0.2.5/LICENSE
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 16:23:52.423727 fonttoolswb-0.2.5/Lib/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 16:23:52.425727 fonttoolswb-0.2.5/Lib/fonttoolsWB/
+-rw-rw-rw-   0 root         (0) root         (0)      335 2024-04-25 16:23:51.000000 fonttoolswb-0.2.5/Lib/fonttoolsWB/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 16:23:52.428727 fonttoolswb-0.2.5/Lib/fonttoolsWB/data/
+-rw-rw-rw-   0 root         (0) root         (0)       98 2024-04-25 16:23:51.000000 fonttoolswb-0.2.5/Lib/fonttoolsWB/data/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      631 2024-04-25 16:23:51.000000 fonttoolswb-0.2.5/Lib/fonttoolsWB/data/application.yml
+-rw-rw-rw-   0 root         (0) root         (0)     2379 2024-04-25 16:23:51.000000 fonttoolswb-0.2.5/Lib/fonttoolsWB/data/firstRun.py
+-rw-rw-rw-   0 root         (0) root         (0)     9767 2024-04-25 16:23:51.000000 fonttoolswb-0.2.5/Lib/fonttoolsWB/data/splashscreen.png
+-rw-rw-rw-   0 root         (0) root         (0)      319 2024-04-25 16:23:51.000000 fonttoolswb-0.2.5/Lib/fonttoolsWB/gui.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 16:23:52.428727 fonttoolswb-0.2.5/Lib/fonttoolsWB.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3078 2024-04-25 16:23:52.000000 fonttoolswb-0.2.5/Lib/fonttoolsWB.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      485 2024-04-25 16:23:52.000000 fonttoolswb-0.2.5/Lib/fonttoolsWB.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-25 16:23:52.000000 fonttoolswb-0.2.5/Lib/fonttoolsWB.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       96 2024-04-25 16:23:52.000000 fonttoolswb-0.2.5/Lib/fonttoolsWB.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      187 2024-04-25 16:23:52.000000 fonttoolswb-0.2.5/Lib/fonttoolsWB.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2024-04-25 16:23:52.000000 fonttoolswb-0.2.5/Lib/fonttoolsWB.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     3078 2024-04-25 16:23:52.429727 fonttoolswb-0.2.5/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1154 2024-04-25 16:23:51.000000 fonttoolswb-0.2.5/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     2469 2024-04-25 16:23:52.430727 fonttoolswb-0.2.5/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       39 2024-04-25 16:23:51.000000 fonttoolswb-0.2.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 16:23:52.428727 fonttoolswb-0.2.5/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      342 2024-04-25 16:23:51.000000 fonttoolswb-0.2.5/tests/test_plugin.py
```

### Comparing `fonttoolsWB-0.2.4/LICENSE` & `fonttoolswb-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `fonttoolsWB-0.2.4/Lib/fonttoolsWB/data/application.yml` & `fonttoolswb-0.2.5/Lib/fonttoolsWB/data/application.yml`

 * *Files identical despite different names*

### Comparing `fonttoolsWB-0.2.4/Lib/fonttoolsWB/data/firstRun.py` & `fonttoolswb-0.2.5/Lib/fonttoolsWB/data/firstRun.py`

 * *Files identical despite different names*

### Comparing `fonttoolsWB-0.2.4/Lib/fonttoolsWB/data/splashscreen.png` & `fonttoolswb-0.2.5/Lib/fonttoolsWB/data/splashscreen.png`

 * *Files identical despite different names*

### Comparing `fonttoolsWB-0.2.4/Lib/fonttoolsWB.egg-info/PKG-INFO` & `fonttoolswb-0.2.5/Lib/fonttoolsWB.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fonttoolsWB
-Version: 0.2.4
+Version: 0.2.5
 Summary: FontTools WorkBench - Edit OpenType fonts as XML.
 Home-page: https://gitlab.com/workbench2/fonttoolsWB
 Author: Andreas Eigendorf
 License: MIT
 Project-URL: Source, https://gitlab.com/workbench2/fonttoolsWB
 Project-URL: Documentation, https://workbench2.gitlab.io/fonttoolsWB
 Project-URL: Tracker, https://gitlab.com/workbench2/fonttoolsWB/-/issues
@@ -31,20 +31,20 @@
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Topic :: Text Processing :: Fonts
 Classifier: Topic :: Multimedia :: Graphics
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: wbBase>=0.2.8
-Requires-Dist: wbpFonttools>=0.2.5
+Requires-Dist: wbBase>=0.2.9
+Requires-Dist: wbpFonttools>=0.2.6
 Requires-Dist: wbpLoglist>=0.2
 Requires-Dist: wbpOutput>=0.2
 Requires-Dist: wbpShell>=0.2
-Requires-Dist: wbpTextedit>=0.2
+Requires-Dist: wbpTextedit>=0.2.2
 Requires-Dist: wbpUItools>=0.2
 Provides-Extra: develop
 Requires-Dist: wbpNamespace>=0.2; extra == "develop"
 Requires-Dist: wbpWidgetinspector>=0.2; extra == "develop"
 Requires-Dist: wbpHTMLpanel>=0.2.4; extra == "develop"
 
 # fonttoolsWB
```

### Comparing `fonttoolsWB-0.2.4/PKG-INFO` & `fonttoolswb-0.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fonttoolsWB
-Version: 0.2.4
+Version: 0.2.5
 Summary: FontTools WorkBench - Edit OpenType fonts as XML.
 Home-page: https://gitlab.com/workbench2/fonttoolsWB
 Author: Andreas Eigendorf
 License: MIT
 Project-URL: Source, https://gitlab.com/workbench2/fonttoolsWB
 Project-URL: Documentation, https://workbench2.gitlab.io/fonttoolsWB
 Project-URL: Tracker, https://gitlab.com/workbench2/fonttoolsWB/-/issues
@@ -31,20 +31,20 @@
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Topic :: Text Processing :: Fonts
 Classifier: Topic :: Multimedia :: Graphics
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: wbBase>=0.2.8
-Requires-Dist: wbpFonttools>=0.2.5
+Requires-Dist: wbBase>=0.2.9
+Requires-Dist: wbpFonttools>=0.2.6
 Requires-Dist: wbpLoglist>=0.2
 Requires-Dist: wbpOutput>=0.2
 Requires-Dist: wbpShell>=0.2
-Requires-Dist: wbpTextedit>=0.2
+Requires-Dist: wbpTextedit>=0.2.2
 Requires-Dist: wbpUItools>=0.2
 Provides-Extra: develop
 Requires-Dist: wbpNamespace>=0.2; extra == "develop"
 Requires-Dist: wbpWidgetinspector>=0.2; extra == "develop"
 Requires-Dist: wbpHTMLpanel>=0.2.4; extra == "develop"
 
 # fonttoolsWB
```

### Comparing `fonttoolsWB-0.2.4/README.md` & `fonttoolswb-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `fonttoolsWB-0.2.4/setup.cfg` & `fonttoolswb-0.2.5/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.2.4
+current_version = 0.2.5
 commit = True
 tag = True
 tag_name = {new_version}
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)?
 serialize = 
 	{major}.{minor}.{patch}
 
@@ -57,20 +57,20 @@
 
 [options]
 packages = find:
 package_dir = 
 	=Lib
 python_requires = >=3.8
 install_requires = 
-	wbBase>=0.2.8
-	wbpFonttools>=0.2.5
+	wbBase>=0.2.9
+	wbpFonttools>=0.2.6
 	wbpLoglist>=0.2
 	wbpOutput>=0.2
 	wbpShell>=0.2
-	wbpTextedit>=0.2
+	wbpTextedit>=0.2.2
 	wbpUItools>=0.2
 
 [options.extras_require]
 develop = 
 	wbpNamespace>=0.2
 	wbpWidgetinspector>=0.2
 	wbpHTMLpanel>=0.2.4
```


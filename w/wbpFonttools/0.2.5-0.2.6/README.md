# Comparing `tmp/wbpFonttools-0.2.5.tar.gz` & `tmp/wbpfonttools-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wbpFonttools-0.2.5.tar", last modified: Wed Feb 14 15:57:08 2024, max compression
+gzip compressed data, was "wbpfonttools-0.2.6.tar", last modified: Thu Apr 25 12:23:47 2024, max compression
```

## Comparing `wbpFonttools-0.2.5.tar` & `wbpfonttools-0.2.6.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-14 15:57:08.655215 wbpFonttools-0.2.5/
--rw-rw-rw-   0 root         (0) root         (0)     1080 2024-02-14 15:57:07.000000 wbpFonttools-0.2.5/LICENSE
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-14 15:57:08.650215 wbpFonttools-0.2.5/Lib/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-14 15:57:08.653215 wbpFonttools-0.2.5/Lib/wbpFonttools/
--rw-rw-rw-   0 root         (0) root         (0)      663 2024-02-14 15:57:07.000000 wbpFonttools-0.2.5/Lib/wbpFonttools/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4895 2024-02-14 15:57:07.000000 wbpFonttools-0.2.5/Lib/wbpFonttools/config.py
--rw-rw-rw-   0 root         (0) root         (0)     6778 2024-02-14 15:57:07.000000 wbpFonttools-0.2.5/Lib/wbpFonttools/control.py
--rw-rw-rw-   0 root         (0) root         (0)     2000 2024-02-14 15:57:07.000000 wbpFonttools-0.2.5/Lib/wbpFonttools/dialog.py
--rw-rw-rw-   0 root         (0) root         (0)     3730 2024-02-14 15:57:07.000000 wbpFonttools-0.2.5/Lib/wbpFonttools/document.py
--rw-rw-rw-   0 root         (0) root         (0)     1991 2024-02-14 15:57:07.000000 wbpFonttools-0.2.5/Lib/wbpFonttools/selectFontsDialogUI.py
--rw-rw-rw-   0 root         (0) root         (0)     3281 2024-02-14 15:57:07.000000 wbpFonttools-0.2.5/Lib/wbpFonttools/template.py
--rw-rw-rw-   0 root         (0) root         (0)     3144 2024-02-14 15:57:07.000000 wbpFonttools-0.2.5/Lib/wbpFonttools/tools.py
--rw-rw-rw-   0 root         (0) root         (0)     2370 2024-02-14 15:57:07.000000 wbpFonttools-0.2.5/Lib/wbpFonttools/view.py
--rw-rw-rw-   0 root         (0) root         (0)    17751 2024-02-14 15:57:07.000000 wbpFonttools-0.2.5/Lib/wbpFonttools/window.py
--rw-rw-rw-   0 root         (0) root         (0)     4362 2024-02-14 15:57:07.000000 wbpFonttools-0.2.5/Lib/wbpFonttools/windowUI.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-14 15:57:08.655215 wbpFonttools-0.2.5/Lib/wbpFonttools.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2531 2024-02-14 15:57:08.000000 wbpFonttools-0.2.5/Lib/wbpFonttools.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      640 2024-02-14 15:57:08.000000 wbpFonttools-0.2.5/Lib/wbpFonttools.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-14 15:57:08.000000 wbpFonttools-0.2.5/Lib/wbpFonttools.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       41 2024-02-14 15:57:08.000000 wbpFonttools-0.2.5/Lib/wbpFonttools.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       83 2024-02-14 15:57:08.000000 wbpFonttools-0.2.5/Lib/wbpFonttools.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2024-02-14 15:57:08.000000 wbpFonttools-0.2.5/Lib/wbpFonttools.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     2531 2024-02-14 15:57:08.655215 wbpFonttools-0.2.5/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      761 2024-02-14 15:57:07.000000 wbpFonttools-0.2.5/README.md
--rw-rw-rw-   0 root         (0) root         (0)     2339 2024-02-14 15:57:08.656215 wbpFonttools-0.2.5/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       39 2024-02-14 15:57:07.000000 wbpFonttools-0.2.5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-14 15:57:08.655215 wbpFonttools-0.2.5/tests/
--rw-rw-rw-   0 root         (0) root         (0)      825 2024-02-14 15:57:07.000000 wbpFonttools-0.2.5/tests/test_imports.py
--rw-rw-rw-   0 root         (0) root         (0)     2610 2024-02-14 15:57:07.000000 wbpFonttools-0.2.5/tests/test_templates.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 12:23:47.853100 wbpfonttools-0.2.6/
+-rw-rw-rw-   0 root         (0) root         (0)     1080 2024-04-25 12:23:46.000000 wbpfonttools-0.2.6/LICENSE
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 12:23:47.846100 wbpfonttools-0.2.6/Lib/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 12:23:47.850100 wbpfonttools-0.2.6/Lib/wbpFonttools/
+-rw-rw-rw-   0 root         (0) root         (0)      663 2024-04-25 12:23:46.000000 wbpfonttools-0.2.6/Lib/wbpFonttools/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4895 2024-04-25 12:23:46.000000 wbpfonttools-0.2.6/Lib/wbpFonttools/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     6778 2024-04-25 12:23:46.000000 wbpfonttools-0.2.6/Lib/wbpFonttools/control.py
+-rw-rw-rw-   0 root         (0) root         (0)     2000 2024-04-25 12:23:46.000000 wbpfonttools-0.2.6/Lib/wbpFonttools/dialog.py
+-rw-rw-rw-   0 root         (0) root         (0)     3730 2024-04-25 12:23:46.000000 wbpfonttools-0.2.6/Lib/wbpFonttools/document.py
+-rw-rw-rw-   0 root         (0) root         (0)     1991 2024-04-25 12:23:46.000000 wbpfonttools-0.2.6/Lib/wbpFonttools/selectFontsDialogUI.py
+-rw-rw-rw-   0 root         (0) root         (0)     3281 2024-04-25 12:23:46.000000 wbpfonttools-0.2.6/Lib/wbpFonttools/template.py
+-rw-rw-rw-   0 root         (0) root         (0)     3144 2024-04-25 12:23:46.000000 wbpfonttools-0.2.6/Lib/wbpFonttools/tools.py
+-rw-rw-rw-   0 root         (0) root         (0)     2370 2024-04-25 12:23:46.000000 wbpfonttools-0.2.6/Lib/wbpFonttools/view.py
+-rw-rw-rw-   0 root         (0) root         (0)    17751 2024-04-25 12:23:46.000000 wbpfonttools-0.2.6/Lib/wbpFonttools/window.py
+-rw-rw-rw-   0 root         (0) root         (0)     4362 2024-04-25 12:23:46.000000 wbpfonttools-0.2.6/Lib/wbpFonttools/windowUI.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 12:23:47.852100 wbpfonttools-0.2.6/Lib/wbpFonttools.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2516 2024-04-25 12:23:47.000000 wbpfonttools-0.2.6/Lib/wbpFonttools.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      640 2024-04-25 12:23:47.000000 wbpfonttools-0.2.6/Lib/wbpFonttools.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-25 12:23:47.000000 wbpfonttools-0.2.6/Lib/wbpFonttools.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       41 2024-04-25 12:23:47.000000 wbpfonttools-0.2.6/Lib/wbpFonttools.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       68 2024-04-25 12:23:47.000000 wbpfonttools-0.2.6/Lib/wbpFonttools.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2024-04-25 12:23:47.000000 wbpfonttools-0.2.6/Lib/wbpFonttools.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     2516 2024-04-25 12:23:47.853100 wbpfonttools-0.2.6/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      761 2024-04-25 12:23:46.000000 wbpfonttools-0.2.6/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     2324 2024-04-25 12:23:47.853100 wbpfonttools-0.2.6/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       39 2024-04-25 12:23:46.000000 wbpfonttools-0.2.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 12:23:47.852100 wbpfonttools-0.2.6/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      825 2024-04-25 12:23:46.000000 wbpfonttools-0.2.6/tests/test_imports.py
+-rw-rw-rw-   0 root         (0) root         (0)     2610 2024-04-25 12:23:46.000000 wbpfonttools-0.2.6/tests/test_templates.py
```

### Comparing `wbpFonttools-0.2.5/LICENSE` & `wbpfonttools-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `wbpFonttools-0.2.5/Lib/wbpFonttools/__init__.py` & `wbpfonttools-0.2.6/Lib/wbpFonttools/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     OpenType_TTC_Template,
     OpenType_TTF_Template,
     WebFont_WOFF_2_Template,
     WebFont_WOFF_Template,
 )
 from .tools import AllFonts, CurrentFont, SelectFonts
 
-__version__ = "0.2.5"
+__version__ = "0.2.6"
 
 
 doctemplates = (
     OpenType_OTF_Template,
     OpenType_TTC_Template,
     OpenType_TTF_Template,
     WebFont_WOFF_2_Template,
```

### Comparing `wbpFonttools-0.2.5/Lib/wbpFonttools/config.py` & `wbpfonttools-0.2.6/Lib/wbpFonttools/config.py`

 * *Files identical despite different names*

### Comparing `wbpFonttools-0.2.5/Lib/wbpFonttools/control.py` & `wbpfonttools-0.2.6/Lib/wbpFonttools/control.py`

 * *Files identical despite different names*

### Comparing `wbpFonttools-0.2.5/Lib/wbpFonttools/dialog.py` & `wbpfonttools-0.2.6/Lib/wbpFonttools/dialog.py`

 * *Files identical despite different names*

### Comparing `wbpFonttools-0.2.5/Lib/wbpFonttools/document.py` & `wbpfonttools-0.2.6/Lib/wbpFonttools/document.py`

 * *Files identical despite different names*

### Comparing `wbpFonttools-0.2.5/Lib/wbpFonttools/selectFontsDialogUI.py` & `wbpfonttools-0.2.6/Lib/wbpFonttools/selectFontsDialogUI.py`

 * *Files identical despite different names*

### Comparing `wbpFonttools-0.2.5/Lib/wbpFonttools/template.py` & `wbpfonttools-0.2.6/Lib/wbpFonttools/template.py`

 * *Files identical despite different names*

### Comparing `wbpFonttools-0.2.5/Lib/wbpFonttools/tools.py` & `wbpfonttools-0.2.6/Lib/wbpFonttools/tools.py`

 * *Files identical despite different names*

### Comparing `wbpFonttools-0.2.5/Lib/wbpFonttools/view.py` & `wbpfonttools-0.2.6/Lib/wbpFonttools/view.py`

 * *Files identical despite different names*

### Comparing `wbpFonttools-0.2.5/Lib/wbpFonttools/window.py` & `wbpfonttools-0.2.6/Lib/wbpFonttools/window.py`

 * *Files identical despite different names*

### Comparing `wbpFonttools-0.2.5/Lib/wbpFonttools/windowUI.py` & `wbpfonttools-0.2.6/Lib/wbpFonttools/windowUI.py`

 * *Files identical despite different names*

### Comparing `wbpFonttools-0.2.5/Lib/wbpFonttools.egg-info/PKG-INFO` & `wbpfonttools-0.2.6/Lib/wbpFonttools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wbpFonttools
-Version: 0.2.5
+Version: 0.2.6
 Summary: FontTools font editor for Workbench applications.
 Home-page: https://gitlab.com/workbench2/workbench-plugins/wbpfonttools
 Author: Andreas Eigendorf
 License: MIT
 Project-URL: Source, https://gitlab.com/workbench2/workbench-plugins/wbpfonttools
 Project-URL: Documentation, https://workbench2.gitlab.io/workbench-plugins/wbpfonttools
 Project-URL: Tracker, https://gitlab.com/workbench2/workbench-plugins/wbpfonttools/-/issues
@@ -33,15 +33,15 @@
 Classifier: Topic :: Software Development :: User Interfaces
 Classifier: Topic :: Text Processing :: Fonts
 Classifier: Topic :: Multimedia :: Graphics
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: wbBase>=0.2.8
-Requires-Dist: fonttools[interpolatable,lxml,plot,symfont,ufo,unicode,woff]>=4.48.1
+Requires-Dist: fonttools[lxml,plot,symfont,ufo,unicode,woff]>=4.48.1
 
 # wbpFonttools
 
 FontTools plugin for [Workbench](https://pypi.org/project/wbBase/) applications.
 
 This plugin provides Workbench document templates for the following font formats:
 - OpenType-TTF Font
```

### Comparing `wbpFonttools-0.2.5/Lib/wbpFonttools.egg-info/SOURCES.txt` & `wbpfonttools-0.2.6/Lib/wbpFonttools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `wbpFonttools-0.2.5/PKG-INFO` & `wbpfonttools-0.2.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wbpFonttools
-Version: 0.2.5
+Version: 0.2.6
 Summary: FontTools font editor for Workbench applications.
 Home-page: https://gitlab.com/workbench2/workbench-plugins/wbpfonttools
 Author: Andreas Eigendorf
 License: MIT
 Project-URL: Source, https://gitlab.com/workbench2/workbench-plugins/wbpfonttools
 Project-URL: Documentation, https://workbench2.gitlab.io/workbench-plugins/wbpfonttools
 Project-URL: Tracker, https://gitlab.com/workbench2/workbench-plugins/wbpfonttools/-/issues
@@ -33,15 +33,15 @@
 Classifier: Topic :: Software Development :: User Interfaces
 Classifier: Topic :: Text Processing :: Fonts
 Classifier: Topic :: Multimedia :: Graphics
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: wbBase>=0.2.8
-Requires-Dist: fonttools[interpolatable,lxml,plot,symfont,ufo,unicode,woff]>=4.48.1
+Requires-Dist: fonttools[lxml,plot,symfont,ufo,unicode,woff]>=4.48.1
 
 # wbpFonttools
 
 FontTools plugin for [Workbench](https://pypi.org/project/wbBase/) applications.
 
 This plugin provides Workbench document templates for the following font formats:
 - OpenType-TTF Font
```

### Comparing `wbpFonttools-0.2.5/README.md` & `wbpfonttools-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `wbpFonttools-0.2.5/setup.cfg` & `wbpfonttools-0.2.6/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.2.5
+current_version = 0.2.6
 commit = True
 tag = True
 tag_name = {new_version}
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)?
 serialize = 
 	{major}.{minor}.{patch}
 
@@ -55,15 +55,15 @@
 [options]
 package_dir = 
 	=Lib
 packages = find:
 python_requires = >=3.8
 install_requires = 
 	wbBase>=0.2.8
-	fonttools[ufo,lxml,woff,unicode,interpolatable,plot,symfont]>=4.48.1
+	fonttools[ufo,lxml,woff,unicode,plot,symfont]>=4.48.1
 
 [options.packages.find]
 where = Lib
 
 [options.entry_points]
 wbbase.plugin = fonttools = wbpFonttools
```

### Comparing `wbpFonttools-0.2.5/tests/test_imports.py` & `wbpfonttools-0.2.6/tests/test_imports.py`

 * *Files identical despite different names*

### Comparing `wbpFonttools-0.2.5/tests/test_templates.py` & `wbpfonttools-0.2.6/tests/test_templates.py`

 * *Files identical despite different names*


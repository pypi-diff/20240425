# Comparing `tmp/flet_easy-0.2.1.dev10.tar.gz` & `tmp/flet_easy-0.2.1.dev20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flet_easy-0.2.1.dev10.tar", last modified: Mon Apr 22 03:26:28 2024, max compression
+gzip compressed data, was "flet_easy-0.2.1.dev20.tar", last modified: Thu Apr 25 01:39:26 2024, max compression
```

## Comparing `flet_easy-0.2.1.dev10.tar` & `flet_easy-0.2.1.dev20.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0    11541 2024-04-22 02:46:04.968016 flet_easy-0.2.1.dev10/LICENSE
--rw-r--r--   0        0        0    11541 2024-04-22 02:46:04.968016 flet_easy-0.2.1.dev10/LICENSE
--rw-r--r--   0        0        0     5794 2024-04-22 02:46:04.968016 flet_easy-0.2.1.dev10/README.md
--rw-r--r--   0        0        0     5794 2024-04-22 02:46:04.968016 flet_easy-0.2.1.dev10/README.md
--rw-r--r--   0        0        0     1889 2024-04-22 03:26:28.417297 flet_easy-0.2.1.dev10/pyproject.toml
--rw-r--r--   0        0        0      432 2024-04-22 02:46:05.087392 flet_easy-0.2.1.dev10/src/flet_easy/__init__.py
--rw-r--r--   0        0        0     1282 2024-04-22 02:46:05.088420 flet_easy-0.2.1.dev10/src/flet_easy/auto_route.py
--rw-r--r--   0        0        0     2356 2024-04-22 02:46:05.088943 flet_easy-0.2.1.dev10/src/flet_easy/cli/copy.py
--rw-r--r--   0        0        0     2099 2024-04-22 02:46:05.089968 flet_easy-0.2.1.dev10/src/flet_easy/cli/main.py
--rw-r--r--   0        0        0     3266 2024-04-22 02:46:05.090972 flet_easy-0.2.1.dev10/src/flet_easy/cli/templates/.gitignore
--rw-r--r--   0        0        0      213 2024-04-22 02:46:05.090972 flet_easy-0.2.1.dev10/src/flet_easy/cli/templates/README.md
--rw-r--r--   0        0        0     1020 2024-04-22 02:46:05.091969 flet_easy-0.2.1.dev10/src/flet_easy/cli/templates/assets/favicon.png
--rw-r--r--   0        0        0    30189 2024-04-22 02:46:05.092969 flet_easy-0.2.1.dev10/src/flet_easy/cli/templates/assets/icon.png
--rw-r--r--   0        0        0     7610 2024-04-22 02:46:05.093972 flet_easy-0.2.1.dev10/src/flet_easy/cli/templates/assets/icons/icon-192.png
--rw-r--r--   0        0        0    33055 2024-04-22 02:46:05.093972 flet_easy-0.2.1.dev10/src/flet_easy/cli/templates/assets/icons/icon-512.png
--rw-r--r--   0        0        0     7610 2024-04-22 02:46:05.094968 flet_easy-0.2.1.dev10/src/flet_easy/cli/templates/assets/icons/icon-maskable-192.png
--rw-r--r--   0        0        0    33055 2024-04-22 02:46:05.096024 flet_easy-0.2.1.dev10/src/flet_easy/cli/templates/assets/icons/icon-maskable-512.png
--rw-r--r--   0        0        0    56474 2024-04-22 02:46:05.097486 flet_easy-0.2.1.dev10/src/flet_easy/cli/templates/assets/icons/loading-animation.png
--rw-r--r--   0        0        0     3626 2024-04-22 02:46:05.097486 flet_easy-0.2.1.dev10/src/flet_easy/cli/templates/assets/index.html
--rw-r--r--   0        0        0      932 2024-04-22 02:46:05.098514 flet_easy-0.2.1.dev10/src/flet_easy/cli/templates/assets/manifest.json
--rw-r--r--   0        0        0       84 2024-04-22 02:46:05.099510 flet_easy-0.2.1.dev10/src/flet_easy/cli/templates/components/__init__.py
--rw-r--r--   0        0        0     2422 2024-04-22 02:46:05.100031 flet_easy-0.2.1.dev10/src/flet_easy/cli/templates/components/counter.py
--rw-r--r--   0        0        0      543 2024-04-22 02:46:05.100031 flet_easy-0.2.1.dev10/src/flet_easy/cli/templates/components/swoDrawer.py
--rw-r--r--   0        0        0       45 2024-04-22 02:46:05.101050 flet_easy-0.2.1.dev10/src/flet_easy/cli/templates/controllers/__init__.py
--rw-r--r--   0        0        0     1258 2024-04-22 02:46:05.102079 flet_easy-0.2.1.dev10/src/flet_easy/cli/templates/controllers/counter.py
--rw-r--r--   0        0        0        0 2024-04-22 02:46:05.102079 flet_easy-0.2.1.dev10/src/flet_easy/cli/templates/core/__init__.py
--rw-r--r--   0        0        0     1662 2024-04-22 02:46:05.103083 flet_easy-0.2.1.dev10/src/flet_easy/cli/templates/core/config.py
--rw-r--r--   0        0        0      246 2024-04-22 02:46:05.103083 flet_easy-0.2.1.dev10/src/flet_easy/cli/templates/main.py
--rw-r--r--   0        0        0        0 2024-04-22 02:46:05.104076 flet_easy-0.2.1.dev10/src/flet_easy/cli/templates/models/__init__.py
--rw-r--r--   0        0        0      588 2024-04-22 02:46:05.105080 flet_easy-0.2.1.dev10/src/flet_easy/cli/templates/views/counter.py
--rw-r--r--   0        0        0      615 2024-04-22 02:46:05.105080 flet_easy-0.2.1.dev10/src/flet_easy/cli/templates/views/index.py
--rw-r--r--   0        0        0    12208 2024-04-22 02:46:05.106146 flet_easy-0.2.1.dev10/src/flet_easy/datasy.py
--rw-r--r--   0        0        0      187 2024-04-22 02:46:05.107076 flet_easy-0.2.1.dev10/src/flet_easy/extra.py
--rw-r--r--   0        0        0     2483 2024-04-22 02:46:05.107593 flet_easy-0.2.1.dev10/src/flet_easy/extrasJwt.py
--rw-r--r--   0        0        0    18351 2024-04-22 02:46:05.107593 flet_easy-0.2.1.dev10/src/flet_easy/fletEasy.py
--rw-r--r--   0        0        0     9856 2024-04-22 02:46:05.108619 flet_easy-0.2.1.dev10/src/flet_easy/inheritance.py
--rw-r--r--   0        0        0     1191 2024-04-22 02:46:05.110135 flet_easy-0.2.1.dev10/src/flet_easy/job.py
--rw-r--r--   0        0        0     4024 2024-04-22 02:46:05.110135 flet_easy-0.2.1.dev10/src/flet_easy/jwt.py
--rw-r--r--   0        0        0     7512 2024-04-22 02:46:05.111160 flet_easy-0.2.1.dev10/src/flet_easy/pagesy.py
--rw-r--r--   0        0        0    11143 2024-04-22 02:59:13.549820 flet_easy-0.2.1.dev10/src/flet_easy/route.py
--rw-r--r--   0        0        0     1540 2024-04-22 02:46:05.112163 flet_easy-0.2.1.dev10/src/flet_easy/view_404.py
--rw-r--r--   0        0        0     6937 1970-01-01 00:00:00.000000 flet_easy-0.2.1.dev10/PKG-INFO
+-rw-r--r--   0        0        0    11541 2024-04-25 01:11:21.131137 flet_easy-0.2.1.dev20/LICENSE
+-rw-r--r--   0        0        0    11541 2024-04-25 01:11:21.131137 flet_easy-0.2.1.dev20/LICENSE
+-rw-r--r--   0        0        0     5794 2024-04-25 01:11:21.131137 flet_easy-0.2.1.dev20/README.md
+-rw-r--r--   0        0        0     5794 2024-04-25 01:11:21.131137 flet_easy-0.2.1.dev20/README.md
+-rw-r--r--   0        0        0     1909 2024-04-25 01:39:26.416424 flet_easy-0.2.1.dev20/pyproject.toml
+-rw-r--r--   0        0        0      432 2024-04-25 01:11:21.244553 flet_easy-0.2.1.dev20/src/flet_easy/__init__.py
+-rw-r--r--   0        0        0     1282 2024-04-25 01:11:21.244553 flet_easy-0.2.1.dev20/src/flet_easy/auto_route.py
+-rw-r--r--   0        0        0     2356 2024-04-25 01:11:21.245552 flet_easy-0.2.1.dev20/src/flet_easy/cli/copy.py
+-rw-r--r--   0        0        0     2099 2024-04-25 01:32:13.586652 flet_easy-0.2.1.dev20/src/flet_easy/cli/main.py
+-rw-r--r--   0        0        0     3266 2024-04-25 01:11:21.247574 flet_easy-0.2.1.dev20/src/flet_easy/cli/templates/.gitignore
+-rw-r--r--   0        0        0      213 2024-04-25 01:11:21.247574 flet_easy-0.2.1.dev20/src/flet_easy/cli/templates/README.md
+-rw-r--r--   0        0        0     1020 2024-04-25 01:11:21.248581 flet_easy-0.2.1.dev20/src/flet_easy/cli/templates/assets/favicon.png
+-rw-r--r--   0        0        0    30189 2024-04-25 01:11:21.249571 flet_easy-0.2.1.dev20/src/flet_easy/cli/templates/assets/icon.png
+-rw-r--r--   0        0        0     7610 2024-04-25 01:11:21.250567 flet_easy-0.2.1.dev20/src/flet_easy/cli/templates/assets/icons/icon-192.png
+-rw-r--r--   0        0        0    33055 2024-04-25 01:11:21.250567 flet_easy-0.2.1.dev20/src/flet_easy/cli/templates/assets/icons/icon-512.png
+-rw-r--r--   0        0        0     7610 2024-04-25 01:11:21.251570 flet_easy-0.2.1.dev20/src/flet_easy/cli/templates/assets/icons/icon-maskable-192.png
+-rw-r--r--   0        0        0    33055 2024-04-25 01:11:21.252569 flet_easy-0.2.1.dev20/src/flet_easy/cli/templates/assets/icons/icon-maskable-512.png
+-rw-r--r--   0        0        0    56474 2024-04-25 01:11:21.253573 flet_easy-0.2.1.dev20/src/flet_easy/cli/templates/assets/icons/loading-animation.png
+-rw-r--r--   0        0        0     3626 2024-04-25 01:11:21.254090 flet_easy-0.2.1.dev20/src/flet_easy/cli/templates/assets/index.html
+-rw-r--r--   0        0        0      932 2024-04-25 01:11:21.255114 flet_easy-0.2.1.dev20/src/flet_easy/cli/templates/assets/manifest.json
+-rw-r--r--   0        0        0       84 2024-04-25 01:11:21.255114 flet_easy-0.2.1.dev20/src/flet_easy/cli/templates/components/__init__.py
+-rw-r--r--   0        0        0     2422 2024-04-25 01:11:21.256137 flet_easy-0.2.1.dev20/src/flet_easy/cli/templates/components/counter.py
+-rw-r--r--   0        0        0      543 2024-04-25 01:11:21.257134 flet_easy-0.2.1.dev20/src/flet_easy/cli/templates/components/swoDrawer.py
+-rw-r--r--   0        0        0       45 2024-04-25 01:11:21.257134 flet_easy-0.2.1.dev20/src/flet_easy/cli/templates/controllers/__init__.py
+-rw-r--r--   0        0        0     1258 2024-04-25 01:11:21.258140 flet_easy-0.2.1.dev20/src/flet_easy/cli/templates/controllers/counter.py
+-rw-r--r--   0        0        0        0 2024-04-25 01:11:21.258140 flet_easy-0.2.1.dev20/src/flet_easy/cli/templates/core/__init__.py
+-rw-r--r--   0        0        0     1662 2024-04-25 01:11:21.259136 flet_easy-0.2.1.dev20/src/flet_easy/cli/templates/core/config.py
+-rw-r--r--   0        0        0      246 2024-04-25 01:11:21.259136 flet_easy-0.2.1.dev20/src/flet_easy/cli/templates/main.py
+-rw-r--r--   0        0        0        0 2024-04-25 01:11:21.260137 flet_easy-0.2.1.dev20/src/flet_easy/cli/templates/models/__init__.py
+-rw-r--r--   0        0        0      588 2024-04-25 01:11:21.261140 flet_easy-0.2.1.dev20/src/flet_easy/cli/templates/views/counter.py
+-rw-r--r--   0        0        0      615 2024-04-25 01:11:21.261140 flet_easy-0.2.1.dev20/src/flet_easy/cli/templates/views/index.py
+-rw-r--r--   0        0        0    12208 2024-04-25 01:11:21.262139 flet_easy-0.2.1.dev20/src/flet_easy/datasy.py
+-rw-r--r--   0        0        0      187 2024-04-25 01:11:21.262139 flet_easy-0.2.1.dev20/src/flet_easy/extra.py
+-rw-r--r--   0        0        0     2483 2024-04-25 01:11:21.262139 flet_easy-0.2.1.dev20/src/flet_easy/extrasJwt.py
+-rw-r--r--   0        0        0    18351 2024-04-25 01:11:21.263715 flet_easy-0.2.1.dev20/src/flet_easy/fletEasy.py
+-rw-r--r--   0        0        0     9856 2024-04-25 01:11:21.264681 flet_easy-0.2.1.dev20/src/flet_easy/inheritance.py
+-rw-r--r--   0        0        0     1191 2024-04-25 01:11:21.264681 flet_easy-0.2.1.dev20/src/flet_easy/job.py
+-rw-r--r--   0        0        0     4024 2024-04-25 01:11:21.265679 flet_easy-0.2.1.dev20/src/flet_easy/jwt.py
+-rw-r--r--   0        0        0     7512 2024-04-25 01:11:21.265679 flet_easy-0.2.1.dev20/src/flet_easy/pagesy.py
+-rw-r--r--   0        0        0    11143 2024-04-25 01:11:21.266698 flet_easy-0.2.1.dev20/src/flet_easy/route.py
+-rw-r--r--   0        0        0     1540 2024-04-25 01:11:21.266698 flet_easy-0.2.1.dev20/src/flet_easy/view_404.py
+-rw-r--r--   0        0        0     6950 1970-01-01 00:00:00.000000 flet_easy-0.2.1.dev20/PKG-INFO
```

### Comparing `flet_easy-0.2.1.dev10/LICENSE` & `flet_easy-0.2.1.dev20/LICENSE`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.1.dev10/README.md` & `flet_easy-0.2.1.dev20/README.md`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.1.dev10/pyproject.toml` & `flet_easy-0.2.1.dev20/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "flet-easy"
-version = "0.2.1.dev10"
-description = "Flet-Easy is a package created as a Flet add-on, designed to be easy to use with a cleaner order in the code, having many customizable features."
+version = "0.2.1.dev20"
+description = "⚡Flet-Easy is a package created as a Flet add-on, designed to be easy to use with a cleaner order in the code, having many customizable features."
 authors = [
     { name = "Daxexs", email = "Daxexsdev@gmail.com" },
 ]
 dependencies = [
     "parse>=1.20.1",
     "pyJWT>=2.8.0",
     "rsa>=4.9",
@@ -22,14 +22,15 @@
     "python web template",
     "app python",
     "flet mvc",
     "flet easy mvc",
     "flet easy fastapi",
     "flutter python",
     "web application",
+    "fast flet",
 ]
 classifiers = [
     "Topic :: Software Development :: Build Tools",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `flet_easy-0.2.1.dev10/src/flet_easy/auto_route.py` & `flet_easy-0.2.1.dev20/src/flet_easy/auto_route.py`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.1.dev10/src/flet_easy/cli/copy.py` & `flet_easy-0.2.1.dev20/src/flet_easy/cli/copy.py`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.1.dev10/src/flet_easy/cli/main.py` & `flet_easy-0.2.1.dev20/src/flet_easy/cli/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from rich.prompt import Prompt
 from rich_argparse import RichHelpFormatter
 from tomlkit import dump
 
 from .copy import _copy_template
 
-VERSION = "0.2.0"
+VERSION = "0.2.1"
 
 RichHelpFormatter.styles["argparse.text"] = "italic"
 RichHelpFormatter.styles["argparse.help"] = "light_sky_blue3"
 RichHelpFormatter.styles["argparse.prog"] = "blue"
 
 
 def init_app():
```

### Comparing `flet_easy-0.2.1.dev10/src/flet_easy/cli/templates/.gitignore` & `flet_easy-0.2.1.dev20/src/flet_easy/cli/templates/.gitignore`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.1.dev10/src/flet_easy/cli/templates/assets/favicon.png` & `flet_easy-0.2.1.dev20/src/flet_easy/cli/templates/assets/favicon.png`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.1.dev10/src/flet_easy/cli/templates/assets/icon.png` & `flet_easy-0.2.1.dev20/src/flet_easy/cli/templates/assets/icon.png`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.1.dev10/src/flet_easy/cli/templates/assets/icons/icon-192.png` & `flet_easy-0.2.1.dev20/src/flet_easy/cli/templates/assets/icons/icon-192.png`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.1.dev10/src/flet_easy/cli/templates/assets/icons/icon-512.png` & `flet_easy-0.2.1.dev20/src/flet_easy/cli/templates/assets/icons/icon-512.png`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.1.dev10/src/flet_easy/cli/templates/assets/icons/icon-maskable-192.png` & `flet_easy-0.2.1.dev20/src/flet_easy/cli/templates/assets/icons/icon-maskable-192.png`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.1.dev10/src/flet_easy/cli/templates/assets/icons/icon-maskable-512.png` & `flet_easy-0.2.1.dev20/src/flet_easy/cli/templates/assets/icons/icon-maskable-512.png`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.1.dev10/src/flet_easy/cli/templates/assets/icons/loading-animation.png` & `flet_easy-0.2.1.dev20/src/flet_easy/cli/templates/assets/icons/loading-animation.png`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.1.dev10/src/flet_easy/cli/templates/assets/index.html` & `flet_easy-0.2.1.dev20/src/flet_easy/cli/templates/assets/index.html`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.1.dev10/src/flet_easy/cli/templates/assets/manifest.json` & `flet_easy-0.2.1.dev20/src/flet_easy/cli/templates/assets/manifest.json`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.1.dev10/src/flet_easy/cli/templates/components/counter.py` & `flet_easy-0.2.1.dev20/src/flet_easy/cli/templates/components/counter.py`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.1.dev10/src/flet_easy/cli/templates/components/swoDrawer.py` & `flet_easy-0.2.1.dev20/src/flet_easy/cli/templates/components/swoDrawer.py`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.1.dev10/src/flet_easy/cli/templates/controllers/counter.py` & `flet_easy-0.2.1.dev20/src/flet_easy/cli/templates/controllers/counter.py`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.1.dev10/src/flet_easy/cli/templates/core/config.py` & `flet_easy-0.2.1.dev20/src/flet_easy/cli/templates/core/config.py`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.1.dev10/src/flet_easy/cli/templates/views/counter.py` & `flet_easy-0.2.1.dev20/src/flet_easy/cli/templates/views/counter.py`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.1.dev10/src/flet_easy/cli/templates/views/index.py` & `flet_easy-0.2.1.dev20/src/flet_easy/cli/templates/views/index.py`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.1.dev10/src/flet_easy/datasy.py` & `flet_easy-0.2.1.dev20/src/flet_easy/datasy.py`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.1.dev10/src/flet_easy/extrasJwt.py` & `flet_easy-0.2.1.dev20/src/flet_easy/extrasJwt.py`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.1.dev10/src/flet_easy/fletEasy.py` & `flet_easy-0.2.1.dev20/src/flet_easy/fletEasy.py`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.1.dev10/src/flet_easy/inheritance.py` & `flet_easy-0.2.1.dev20/src/flet_easy/inheritance.py`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.1.dev10/src/flet_easy/job.py` & `flet_easy-0.2.1.dev20/src/flet_easy/job.py`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.1.dev10/src/flet_easy/jwt.py` & `flet_easy-0.2.1.dev20/src/flet_easy/jwt.py`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.1.dev10/src/flet_easy/pagesy.py` & `flet_easy-0.2.1.dev20/src/flet_easy/pagesy.py`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.1.dev10/src/flet_easy/route.py` & `flet_easy-0.2.1.dev20/src/flet_easy/route.py`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.1.dev10/src/flet_easy/view_404.py` & `flet_easy-0.2.1.dev20/src/flet_easy/view_404.py`

 * *Files identical despite different names*

### Comparing `flet_easy-0.2.1.dev10/PKG-INFO` & `flet_easy-0.2.1.dev20/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: flet-easy
-Version: 0.2.1.dev10
-Summary: Flet-Easy is a package created as a Flet add-on, designed to be easy to use with a cleaner order in the code, having many customizable features.
-Keywords: flet easy,flet,python,flet easy route,python web template,app python,flet mvc,flet easy mvc,flet easy fastapi,flutter python,web application
+Version: 0.2.1.dev20
+Summary: ⚡Flet-Easy is a package created as a Flet add-on, designed to be easy to use with a cleaner order in the code, having many customizable features.
+Keywords: flet easy,flet,python,flet easy route,python web template,app python,flet mvc,flet easy mvc,flet easy fastapi,flutter python,web application,fast flet
 Author-Email: Daxexs <Daxexsdev@gmail.com>
 License: apache-2.0
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```


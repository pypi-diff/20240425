# Comparing `tmp/pick-2.3.0.tar.gz` & `tmp/pick-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pick-2.3.0.tar", max compression
+gzip compressed data, was "pick-2.3.1.tar", max compression
```

## Comparing `pick-2.3.0.tar` & `pick-2.3.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1080 2024-04-19 12:28:44.312843 pick-2.3.0/LICENSE
--rw-r--r--   0        0        0     2463 2024-04-22 10:46:10.505924 pick-2.3.0/README.md
--rw-r--r--   0        0        0      622 2024-04-22 10:46:10.506294 pick-2.3.0/pyproject.toml
--rw-r--r--   0        0        0     7795 2024-04-22 10:45:57.237655 pick-2.3.0/src/pick/__init__.py
--rw-r--r--   0        0        0        0 2024-04-19 12:28:44.315867 pick-2.3.0/src/pick/py.typed
--rw-r--r--   0        0        0     3288 1970-01-01 00:00:00.000000 pick-2.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1080 2024-04-19 12:28:44.312843 pick-2.3.1/LICENSE
+-rw-r--r--   0        0        0     2463 2024-04-24 11:05:12.122434 pick-2.3.1/README.md
+-rw-r--r--   0        0        0      622 2024-04-24 11:37:38.497417 pick-2.3.1/pyproject.toml
+-rw-r--r--   0        0        0     7802 2024-04-24 11:31:11.184104 pick-2.3.1/src/pick/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-19 12:28:44.315867 pick-2.3.1/src/pick/py.typed
+-rw-r--r--   0        0        0     3288 1970-01-01 00:00:00.000000 pick-2.3.1/PKG-INFO
```

### Comparing `pick-2.3.0/LICENSE` & `pick-2.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pick-2.3.0/README.md` & `pick-2.3.1/README.md`

 * *Files identical despite different names*

### Comparing `pick-2.3.0/pyproject.toml` & `pick-2.3.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pick"
-version = "2.3.0"
+version = "2.3.1"
 description = "Pick an option in the terminal with a simple GUI"
 authors = ["wong2 <wonderfuly@gmail.com>", "AN Long <aisk1988@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/aisk/pick"
 homepage = "https://github.com/aisk/pick"
 keywords = ["terminal", "gui"]
```

### Comparing `pick-2.3.0/src/pick/__init__.py` & `pick-2.3.1/src/pick/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -148,15 +148,15 @@
         if current_line > max_rows:
             scroll_top = current_line - max_rows
 
         lines_to_draw = lines[scroll_top : scroll_top + max_rows]
 
         description_present = False
         for option in self.options:
-            if isinstance(option, str) or option.description is not None:
+            if not isinstance(option, Option) or option.description is not None:
                 description_present = True
                 break
 
         for line in lines_to_draw:
             if description_present:
                 screen.addnstr(y, x, line, max_x // 2 - 2)
             else:
```

### Comparing `pick-2.3.0/PKG-INFO` & `pick-2.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pick
-Version: 2.3.0
+Version: 2.3.1
 Summary: Pick an option in the terminal with a simple GUI
 Home-page: https://github.com/aisk/pick
 License: MIT
 Keywords: terminal,gui
 Author: wong2
 Author-email: wonderfuly@gmail.com
 Requires-Python: >=3.7
```


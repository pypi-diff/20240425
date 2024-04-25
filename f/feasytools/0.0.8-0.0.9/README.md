# Comparing `tmp/feasytools-0.0.8.tar.gz` & `tmp/feasytools-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\feasytools-0.0.8.tar", last modified: Thu Apr 25 07:23:23 2024, max compression
+gzip compressed data, was "dist\feasytools-0.0.9.tar", last modified: Thu Apr 25 07:29:46 2024, max compression
```

## Comparing `feasytools-0.0.8.tar` & `feasytools-0.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-25 07:23:23.000000 feasytools-0.0.8/
-drwxrwxrwx   0        0        0        0 2024-04-25 07:23:23.000000 feasytools-0.0.8/feasytools/
--rw-rw-rw-   0        0        0     5414 2024-04-25 06:52:49.000000 feasytools-0.0.8/feasytools/argchk.py
--rw-rw-rw-   0        0        0     5348 2024-04-25 07:22:13.000000 feasytools-0.0.8/feasytools/pq.py
--rw-rw-rw-   0        0        0     1897 2024-03-23 07:36:53.000000 feasytools-0.0.8/feasytools/rangelist.py
--rw-rw-rw-   0        0        0    17755 2024-03-23 07:46:48.000000 feasytools-0.0.8/feasytools/table.py
--rw-rw-rw-   0        0        0     8469 2024-03-28 11:21:46.000000 feasytools-0.0.8/feasytools/tfunc.py
--rw-rw-rw-   0        0        0      963 2024-04-25 07:22:31.000000 feasytools-0.0.8/feasytools/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-25 07:23:23.000000 feasytools-0.0.8/feasytools.egg-info/
--rw-rw-rw-   0        0        0        1 2024-04-25 07:23:23.000000 feasytools-0.0.8/feasytools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      835 2024-04-25 07:23:23.000000 feasytools-0.0.8/feasytools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       14 2024-04-25 07:23:23.000000 feasytools-0.0.8/feasytools.egg-info/requires.txt
--rw-rw-rw-   0        0        0      312 2024-04-25 07:23:23.000000 feasytools-0.0.8/feasytools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       11 2024-04-25 07:23:23.000000 feasytools-0.0.8/feasytools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      835 2024-04-25 07:23:23.000000 feasytools-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      316 2024-03-23 07:58:23.000000 feasytools-0.0.8/README.md
--rw-rw-rw-   0        0        0       42 2024-04-25 07:23:23.000000 feasytools-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      683 2024-04-25 07:22:52.000000 feasytools-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-25 07:29:46.000000 feasytools-0.0.9/
+drwxrwxrwx   0        0        0        0 2024-04-25 07:29:46.000000 feasytools-0.0.9/feasytools/
+-rw-rw-rw-   0        0        0     5478 2024-04-25 07:29:09.000000 feasytools-0.0.9/feasytools/argchk.py
+-rw-rw-rw-   0        0        0     5348 2024-04-25 07:22:13.000000 feasytools-0.0.9/feasytools/pq.py
+-rw-rw-rw-   0        0        0     1897 2024-03-23 07:36:53.000000 feasytools-0.0.9/feasytools/rangelist.py
+-rw-rw-rw-   0        0        0    17755 2024-03-23 07:46:48.000000 feasytools-0.0.9/feasytools/table.py
+-rw-rw-rw-   0        0        0     8469 2024-03-28 11:21:46.000000 feasytools-0.0.9/feasytools/tfunc.py
+-rw-rw-rw-   0        0        0      963 2024-04-25 07:22:31.000000 feasytools-0.0.9/feasytools/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-25 07:29:46.000000 feasytools-0.0.9/feasytools.egg-info/
+-rw-rw-rw-   0        0        0        1 2024-04-25 07:29:46.000000 feasytools-0.0.9/feasytools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      835 2024-04-25 07:29:46.000000 feasytools-0.0.9/feasytools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       14 2024-04-25 07:29:46.000000 feasytools-0.0.9/feasytools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      312 2024-04-25 07:29:46.000000 feasytools-0.0.9/feasytools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       11 2024-04-25 07:29:46.000000 feasytools-0.0.9/feasytools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      835 2024-04-25 07:29:46.000000 feasytools-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      316 2024-03-23 07:58:23.000000 feasytools-0.0.9/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-25 07:29:46.000000 feasytools-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      683 2024-04-25 07:28:35.000000 feasytools-0.0.9/setup.py
```

### Comparing `feasytools-0.0.8/feasytools/argchk.py` & `feasytools-0.0.9/feasytools/argchk.py`

 * *Files 5% similar despite different names*

```diff
@@ -41,21 +41,21 @@
             return float(v)
         except:
             return v.strip('"')
 
     @staticmethod
     def get_dict(
         params: "Union[str,Iterable[str]]" = sys.argv[1:],
-        force_parametric:"list[str]" = []
+        force_parametric: "list[str]" = [],
     ) -> "dict[str,Union[str,Any]]":
-        """ Return the input parameters as a dict """
+        """Return the input parameters as a dict"""
         if isinstance(params, str):
             cur_item = ""
             inquote = 0
-            new_params:list[str] = []
+            new_params: list[str] = []
             for c in params:
                 if c == " " and inquote == 0:
                     if cur_item != "":
                         new_params.append(cur_item)
                         cur_item = ""
                 else:
                     if c == '"' and inquote == 0:
@@ -93,23 +93,29 @@
                 # Argument without key
                 ArgChecker.__err(KeyError, v)
         if cur_key != None:
             ret[cur_key] = True
         return ret
 
     @overload
-    def __init__(self, *, force_parametric: "list[str]") -> None: ...
+    def __init__(self, *, force_parametric: "list[str]" = []) -> None: ...
 
     @overload
-    def __init__(self, pars: str, force_parametric: "list[str]") -> None: ...
+    def __init__(self, pars: str, force_parametric: "list[str]" = []) -> None: ...
 
     @overload
-    def __init__(self, pars: "dict[str, Any]", force_parametric: "list[str]") -> None: ...
-    
-    def __init__(self, pars: "Union[None,str,dict[str,Any]]" = None, force_parametric:"list[str]" = []):
+    def __init__(
+        self, pars: "dict[str, Any]", force_parametric: "list[str]" = []
+    ) -> None: ...
+
+    def __init__(
+        self,
+        pars: "Union[None,str,dict[str,Any]]" = None,
+        force_parametric: "list[str]" = [],
+    ):
         if pars is None:
             self.__args = ArgChecker.get_dict(force_parametric=force_parametric)
         elif isinstance(pars, str):
             self.__args = ArgChecker.get_dict(pars, force_parametric=force_parametric)
         elif isinstance(pars, dict):
             self.__args = pars
         else:
```

### Comparing `feasytools-0.0.8/feasytools/pq.py` & `feasytools-0.0.9/feasytools/pq.py`

 * *Files identical despite different names*

### Comparing `feasytools-0.0.8/feasytools/rangelist.py` & `feasytools-0.0.9/feasytools/rangelist.py`

 * *Files identical despite different names*

### Comparing `feasytools-0.0.8/feasytools/table.py` & `feasytools-0.0.9/feasytools/table.py`

 * *Files identical despite different names*

### Comparing `feasytools-0.0.8/feasytools/tfunc.py` & `feasytools-0.0.9/feasytools/tfunc.py`

 * *Files identical despite different names*

### Comparing `feasytools-0.0.8/feasytools/__init__.py` & `feasytools-0.0.9/feasytools/__init__.py`

 * *Files identical despite different names*

### Comparing `feasytools-0.0.8/feasytools.egg-info/PKG-INFO` & `feasytools-0.0.9/feasytools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feasytools
-Version: 0.0.8
+Version: 0.0.9
 Summary: A set of tools for data processing, including Time Function, Table, Priority Queue, Range List, etc.
 Home-page: UNKNOWN
 Author: fmy_xfk
 License: UNKNOWN
 Description: # FEasyTools: Some useful components
         - dprov: Data provider as time functions
         - argchk: Argument parser with type checking
```

### Comparing `feasytools-0.0.8/PKG-INFO` & `feasytools-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feasytools
-Version: 0.0.8
+Version: 0.0.9
 Summary: A set of tools for data processing, including Time Function, Table, Priority Queue, Range List, etc.
 Home-page: UNKNOWN
 Author: fmy_xfk
 License: UNKNOWN
 Description: # FEasyTools: Some useful components
         - dprov: Data provider as time functions
         - argchk: Argument parser with type checking
```

### Comparing `feasytools-0.0.8/setup.py` & `feasytools-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="feasytools",
-    version="0.0.8",
+    version="0.0.9",
     author="fmy_xfk",
     packages=find_packages(),
     description="A set of tools for data processing, including Time Function, Table, Priority Queue, Range List, etc.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
         "Programming Language :: Python :: 3",
```


# Comparing `tmp/streamlit-js-1.0.5.tar.gz` & `tmp/streamlit-js-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit-js-1.0.5.tar", last modified: Thu Apr 25 04:53:49 2024, max compression
+gzip compressed data, was "streamlit-js-1.0.6.tar", last modified: Thu Apr 25 04:56:34 2024, max compression
```

## Comparing `streamlit-js-1.0.5.tar` & `streamlit-js-1.0.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 sne        (501) staff       (20)        0 2024-04-25 04:53:49.587913 streamlit-js-1.0.5/
--rw-r--r--   0 sne        (501) staff       (20)     1063 2024-03-21 10:14:00.000000 streamlit-js-1.0.5/LICENSE
--rw-r--r--   0 sne        (501) staff       (20)       48 2024-03-21 12:56:30.000000 streamlit-js-1.0.5/MANIFEST.in
--rw-r--r--   0 sne        (501) staff       (20)     2010 2024-04-25 04:53:49.587679 streamlit-js-1.0.5/PKG-INFO
--rw-r--r--   0 sne        (501) staff       (20)     1274 2024-03-28 04:57:59.000000 streamlit-js-1.0.5/README.md
--rw-r--r--   0 sne        (501) staff       (20)       38 2024-04-25 04:53:49.587955 streamlit-js-1.0.5/setup.cfg
--rw-r--r--   0 sne        (501) staff       (20)     1145 2024-04-25 04:51:45.000000 streamlit-js-1.0.5/setup.py
-drwxr-xr-x   0 sne        (501) staff       (20)        0 2024-04-25 04:53:49.580956 streamlit-js-1.0.5/streamlit_js/
--rw-r--r--   0 sne        (501) staff       (20)     5122 2024-03-28 05:54:37.000000 streamlit-js-1.0.5/streamlit_js/__init__.py
-drwxr-xr-x   0 sne        (501) staff       (20)        0 2024-04-25 04:53:49.580111 streamlit-js-1.0.5/streamlit_js/frontend/
-drwxr-xr-x   0 sne        (501) staff       (20)        0 2024-04-25 04:53:49.582731 streamlit-js-1.0.5/streamlit_js/frontend/build/
--rw-r--r--   0 sne        (501) staff       (20)      221 2024-04-25 04:52:19.000000 streamlit-js-1.0.5/streamlit_js/frontend/build/asset-manifest.json
--rw-r--r--   0 sne        (501) staff       (20)   197459 2024-04-25 04:52:14.000000 streamlit-js-1.0.5/streamlit_js/frontend/build/bootstrap.min.css
--rw-r--r--   0 sne        (501) staff       (20)      492 2024-04-25 04:52:19.000000 streamlit-js-1.0.5/streamlit_js/frontend/build/index.html
-drwxr-xr-x   0 sne        (501) staff       (20)        0 2024-04-25 04:53:49.580228 streamlit-js-1.0.5/streamlit_js/frontend/build/static/
-drwxr-xr-x   0 sne        (501) staff       (20)        0 2024-04-25 04:53:49.584666 streamlit-js-1.0.5/streamlit_js/frontend/build/static/js/
--rw-r--r--   0 sne        (501) staff       (20)   317454 2024-04-25 04:52:19.000000 streamlit-js-1.0.5/streamlit_js/frontend/build/static/js/main.53d6ba46.js
--rw-r--r--   0 sne        (501) staff       (20)     1293 2024-04-25 04:52:19.000000 streamlit-js-1.0.5/streamlit_js/frontend/build/static/js/main.53d6ba46.js.LICENSE.txt
--rw-r--r--   0 sne        (501) staff       (20)  1247238 2024-04-25 04:52:19.000000 streamlit-js-1.0.5/streamlit_js/frontend/build/static/js/main.53d6ba46.js.map
-drwxr-xr-x   0 sne        (501) staff       (20)        0 2024-04-25 04:53:49.586893 streamlit-js-1.0.5/streamlit_js.egg-info/
--rw-r--r--   0 sne        (501) staff       (20)     2010 2024-04-25 04:53:49.000000 streamlit-js-1.0.5/streamlit_js.egg-info/PKG-INFO
--rw-r--r--   0 sne        (501) staff       (20)      556 2024-04-25 04:53:49.000000 streamlit-js-1.0.5/streamlit_js.egg-info/SOURCES.txt
--rw-r--r--   0 sne        (501) staff       (20)        1 2024-04-25 04:53:49.000000 streamlit-js-1.0.5/streamlit_js.egg-info/dependency_links.txt
--rw-r--r--   0 sne        (501) staff       (20)      140 2024-04-25 04:53:49.000000 streamlit-js-1.0.5/streamlit_js.egg-info/requires.txt
--rw-r--r--   0 sne        (501) staff       (20)       13 2024-04-25 04:53:49.000000 streamlit-js-1.0.5/streamlit_js.egg-info/top_level.txt
+drwxr-xr-x   0 sne        (501) staff       (20)        0 2024-04-25 04:56:34.151987 streamlit-js-1.0.6/
+-rw-r--r--   0 sne        (501) staff       (20)     1063 2024-03-21 10:14:00.000000 streamlit-js-1.0.6/LICENSE
+-rw-r--r--   0 sne        (501) staff       (20)       48 2024-03-21 12:56:30.000000 streamlit-js-1.0.6/MANIFEST.in
+-rw-r--r--   0 sne        (501) staff       (20)     2010 2024-04-25 04:56:34.151622 streamlit-js-1.0.6/PKG-INFO
+-rw-r--r--   0 sne        (501) staff       (20)     1274 2024-03-28 04:57:59.000000 streamlit-js-1.0.6/README.md
+-rw-r--r--   0 sne        (501) staff       (20)       38 2024-04-25 04:56:34.152042 streamlit-js-1.0.6/setup.cfg
+-rw-r--r--   0 sne        (501) staff       (20)     1145 2024-04-25 04:56:14.000000 streamlit-js-1.0.6/setup.py
+drwxr-xr-x   0 sne        (501) staff       (20)        0 2024-04-25 04:56:34.142313 streamlit-js-1.0.6/streamlit_js/
+-rw-r--r--   0 sne        (501) staff       (20)     5185 2024-04-25 04:55:59.000000 streamlit-js-1.0.6/streamlit_js/__init__.py
+drwxr-xr-x   0 sne        (501) staff       (20)        0 2024-04-25 04:56:34.141437 streamlit-js-1.0.6/streamlit_js/frontend/
+drwxr-xr-x   0 sne        (501) staff       (20)        0 2024-04-25 04:56:34.145981 streamlit-js-1.0.6/streamlit_js/frontend/build/
+-rw-r--r--   0 sne        (501) staff       (20)      221 2024-04-25 04:52:19.000000 streamlit-js-1.0.6/streamlit_js/frontend/build/asset-manifest.json
+-rw-r--r--   0 sne        (501) staff       (20)   197459 2024-04-25 04:52:14.000000 streamlit-js-1.0.6/streamlit_js/frontend/build/bootstrap.min.css
+-rw-r--r--   0 sne        (501) staff       (20)      492 2024-04-25 04:52:19.000000 streamlit-js-1.0.6/streamlit_js/frontend/build/index.html
+drwxr-xr-x   0 sne        (501) staff       (20)        0 2024-04-25 04:56:34.141547 streamlit-js-1.0.6/streamlit_js/frontend/build/static/
+drwxr-xr-x   0 sne        (501) staff       (20)        0 2024-04-25 04:56:34.148207 streamlit-js-1.0.6/streamlit_js/frontend/build/static/js/
+-rw-r--r--   0 sne        (501) staff       (20)   317454 2024-04-25 04:52:19.000000 streamlit-js-1.0.6/streamlit_js/frontend/build/static/js/main.53d6ba46.js
+-rw-r--r--   0 sne        (501) staff       (20)     1293 2024-04-25 04:52:19.000000 streamlit-js-1.0.6/streamlit_js/frontend/build/static/js/main.53d6ba46.js.LICENSE.txt
+-rw-r--r--   0 sne        (501) staff       (20)  1247238 2024-04-25 04:52:19.000000 streamlit-js-1.0.6/streamlit_js/frontend/build/static/js/main.53d6ba46.js.map
+drwxr-xr-x   0 sne        (501) staff       (20)        0 2024-04-25 04:56:34.150648 streamlit-js-1.0.6/streamlit_js.egg-info/
+-rw-r--r--   0 sne        (501) staff       (20)     2010 2024-04-25 04:56:34.000000 streamlit-js-1.0.6/streamlit_js.egg-info/PKG-INFO
+-rw-r--r--   0 sne        (501) staff       (20)      556 2024-04-25 04:56:34.000000 streamlit-js-1.0.6/streamlit_js.egg-info/SOURCES.txt
+-rw-r--r--   0 sne        (501) staff       (20)        1 2024-04-25 04:56:34.000000 streamlit-js-1.0.6/streamlit_js.egg-info/dependency_links.txt
+-rw-r--r--   0 sne        (501) staff       (20)      140 2024-04-25 04:56:34.000000 streamlit-js-1.0.6/streamlit_js.egg-info/requires.txt
+-rw-r--r--   0 sne        (501) staff       (20)       13 2024-04-25 04:56:34.000000 streamlit-js-1.0.6/streamlit_js.egg-info/top_level.txt
```

### Comparing `streamlit-js-1.0.5/LICENSE` & `streamlit-js-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit-js-1.0.5/PKG-INFO` & `streamlit-js-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-js
-Version: 1.0.5
+Version: 1.0.6
 Summary: Streamlit component that allows you to run js code with both blocking and non-blocking modes.
 Home-page: https://github.com/toolittlecakes/streamlit_js
 Author: Nikolay Sheyko
 Author-email: nickolay.sheyko@gmail.com.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `streamlit-js-1.0.5/README.md` & `streamlit-js-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `streamlit-js-1.0.5/setup.py` & `streamlit-js-1.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name="streamlit-js",
-    version="1.0.5",
+    version="1.0.6",
     author="Nikolay Sheyko",
     author_email="nickolay.sheyko@gmail.com.com",
     description="Streamlit component that allows you to run js code with both blocking and non-blocking modes.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/toolittlecakes/streamlit_js",
     packages=setuptools.find_packages(),
```

### Comparing `streamlit-js-1.0.5/streamlit_js/__init__.py` & `streamlit-js-1.0.6/streamlit_js/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     # replace the `url` param with `path`, and point it to the component's
     # build directory:
     parent_dir = os.path.dirname(os.path.abspath(__file__))
     build_dir = os.path.join(parent_dir, "frontend/build")
     _component_func = components.declare_component("streamlit_js", path=build_dir)
 
 
-def st_js(code: str, key=None):
+def st_js(code: str, expect_result=True, key=None):
     """
     This is a non-blocking streamlit component that executes JavaScript code.
 
     Parameters
     ----------
     code: str
         The code to be executed by the component.
@@ -55,15 +55,17 @@
     list
         [] if the code is still running.
         [<result>] if the code is finished.
         {"error": <error>} if the code throws an error.
         Where <result> is the value of executed code. It has to be serializable.
         It's already deserialized by Streamlit into Python object.
     """
-    return _component_func(code=code, key=key, default=[], height=0)
+    return _component_func(
+        code=code, expect_result=expect_result, key=key, default=[], height=0
+    )
 
 
 def st_js_blocking(code, key=None):
     """
     This is a blocking version of streamlit_js.
     It will block the script until the component is finished and result is returned.
     In case of an error, it will raise an exception.
```

### Comparing `streamlit-js-1.0.5/streamlit_js/frontend/build/bootstrap.min.css` & `streamlit-js-1.0.6/streamlit_js/frontend/build/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `streamlit-js-1.0.5/streamlit_js/frontend/build/static/js/main.53d6ba46.js` & `streamlit-js-1.0.6/streamlit_js/frontend/build/static/js/main.53d6ba46.js`

 * *Files identical despite different names*

### Comparing `streamlit-js-1.0.5/streamlit_js/frontend/build/static/js/main.53d6ba46.js.LICENSE.txt` & `streamlit-js-1.0.6/streamlit_js/frontend/build/static/js/main.53d6ba46.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlit-js-1.0.5/streamlit_js/frontend/build/static/js/main.53d6ba46.js.map` & `streamlit-js-1.0.6/streamlit_js/frontend/build/static/js/main.53d6ba46.js.map`

 * *Files identical despite different names*

### Comparing `streamlit-js-1.0.5/streamlit_js.egg-info/PKG-INFO` & `streamlit-js-1.0.6/streamlit_js.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-js
-Version: 1.0.5
+Version: 1.0.6
 Summary: Streamlit component that allows you to run js code with both blocking and non-blocking modes.
 Home-page: https://github.com/toolittlecakes/streamlit_js
 Author: Nikolay Sheyko
 Author-email: nickolay.sheyko@gmail.com.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `streamlit-js-1.0.5/streamlit_js.egg-info/SOURCES.txt` & `streamlit-js-1.0.6/streamlit_js.egg-info/SOURCES.txt`

 * *Files identical despite different names*


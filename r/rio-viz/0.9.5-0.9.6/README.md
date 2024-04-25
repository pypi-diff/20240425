# Comparing `tmp/rio-viz-0.9.5.tar.gz` & `tmp/rio-viz-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rio-viz-0.9.5.tar", last modified: Tue May 17 19:52:52 2022, max compression
+gzip compressed data, was "rio-viz-0.9.6.tar", last modified: Tue Jun 14 08:50:26 2022, max compression
```

## Comparing `rio-viz-0.9.5.tar` & `rio-viz-0.9.6.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0      211 2022-05-17 19:52:26.375932 rio-viz-0.9.5/.bumpversion.cfg
--rw-r--r--   0        0        0      136 2022-05-17 19:52:26.375932 rio-viz-0.9.5/.flake8
--rw-r--r--   0        0        0     1215 2022-05-17 19:52:26.375932 rio-viz-0.9.5/.gitignore
--rw-r--r--   0        0        0      674 2022-05-17 19:52:26.375932 rio-viz-0.9.5/.pre-commit-config.yaml
--rw-r--r--   0        0        0      531 2022-05-17 19:52:26.375932 rio-viz-0.9.5/Dockerfile
--rw-r--r--   0        0        0     1073 2022-05-17 19:52:26.375932 rio-viz-0.9.5/LICENSE
--rw-r--r--   0        0        0     5510 2022-05-17 19:52:26.375932 rio-viz-0.9.5/README.md
--rw-r--r--   0        0        0     1617 2022-05-17 19:52:26.375932 rio-viz-0.9.5/pyproject.toml
--rw-r--r--   0        0        0      122 2022-05-17 19:52:26.375932 rio-viz-0.9.5/rio_viz/__init__.py
--rw-r--r--   0        0        0    26299 2022-05-17 19:52:26.375932 rio-viz-0.9.5/rio_viz/app.py
--rw-r--r--   0        0        0     3297 2022-05-17 19:52:26.375932 rio-viz-0.9.5/rio_viz/compat.py
--rw-r--r--   0        0        0      154 2022-05-17 19:52:26.375932 rio-viz-0.9.5/rio_viz/io/__init__.py
--rw-r--r--   0        0        0     5297 2022-05-17 19:52:26.375932 rio-viz-0.9.5/rio_viz/io/mosaic.py
--rw-r--r--   0        0        0     2438 2022-05-17 19:52:26.375932 rio-viz-0.9.5/rio_viz/io/reader.py
--rw-r--r--   0        0        0       25 2022-05-17 19:52:26.375932 rio-viz-0.9.5/rio_viz/resources/__init__.py
--rw-r--r--   0        0        0     1895 2022-05-17 19:52:26.375932 rio-viz-0.9.5/rio_viz/resources/enums.py
--rw-r--r--   0        0        0       19 2022-05-17 19:52:26.375932 rio-viz-0.9.5/rio_viz/scripts/__init__.py
--rw-r--r--   0        0        0     4814 2022-05-17 19:52:26.375932 rio-viz-0.9.5/rio_viz/scripts/cli.py
--rw-r--r--   0        0        0   179483 2022-05-17 19:52:26.379932 rio-viz-0.9.5/rio_viz/src/css/assembly.min.css
--rw-r--r--   0        0        0    34683 2022-05-17 19:52:26.379932 rio-viz-0.9.5/rio_viz/src/css/mapbox-gl.css
--rw-r--r--   0        0        0    48874 2022-05-17 19:52:26.379932 rio-viz-0.9.5/rio_viz/src/js/assembly.js
--rw-r--r--   0        0        0   472081 2022-05-17 19:52:26.379932 rio-viz-0.9.5/rio_viz/src/js/d3.v4.js
--rw-r--r--   0        0        0   744707 2022-05-17 19:52:26.387932 rio-viz-0.9.5/rio_viz/src/js/mapbox-gl.js
--rw-r--r--   0        0        0  3028436 2022-05-17 19:52:26.403932 rio-viz-0.9.5/rio_viz/src/js/mapbox-gl.js.map
--rw-r--r--   0        0        0    36425 2022-05-17 19:52:26.403932 rio-viz-0.9.5/rio_viz/templates/assets.html
--rw-r--r--   0        0        0    36738 2022-05-17 19:52:26.403932 rio-viz-0.9.5/rio_viz/templates/bands.html
--rw-r--r--   0        0        0    36926 2022-05-17 19:52:26.403932 rio-viz-0.9.5/rio_viz/templates/index.html
--rw-r--r--   0        0        0     2955 2022-05-17 19:52:26.403932 rio-viz-0.9.5/rio_viz/templates/wmts.xml
--rw-r--r--   0        0        0     6660 1970-01-01 00:00:00.000000 rio-viz-0.9.5/PKG-INFO
+-rw-r--r--   0        0        0      211 2022-06-14 08:49:55.186339 rio-viz-0.9.6/.bumpversion.cfg
+-rw-r--r--   0        0        0      136 2022-06-14 08:49:55.186339 rio-viz-0.9.6/.flake8
+-rw-r--r--   0        0        0     1215 2022-06-14 08:49:55.190339 rio-viz-0.9.6/.gitignore
+-rw-r--r--   0        0        0      674 2022-06-14 08:49:55.190339 rio-viz-0.9.6/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      531 2022-06-14 08:49:55.190339 rio-viz-0.9.6/Dockerfile
+-rw-r--r--   0        0        0     1073 2022-06-14 08:49:55.190339 rio-viz-0.9.6/LICENSE
+-rw-r--r--   0        0        0     5510 2022-06-14 08:49:55.190339 rio-viz-0.9.6/README.md
+-rw-r--r--   0        0        0     1615 2022-06-14 08:49:55.190339 rio-viz-0.9.6/pyproject.toml
+-rw-r--r--   0        0        0      122 2022-06-14 08:49:55.190339 rio-viz-0.9.6/rio_viz/__init__.py
+-rw-r--r--   0        0        0    26299 2022-06-14 08:49:55.190339 rio-viz-0.9.6/rio_viz/app.py
+-rw-r--r--   0        0        0     3297 2022-06-14 08:49:55.190339 rio-viz-0.9.6/rio_viz/compat.py
+-rw-r--r--   0        0        0      154 2022-06-14 08:49:55.190339 rio-viz-0.9.6/rio_viz/io/__init__.py
+-rw-r--r--   0        0        0     5297 2022-06-14 08:49:55.190339 rio-viz-0.9.6/rio_viz/io/mosaic.py
+-rw-r--r--   0        0        0     2438 2022-06-14 08:49:55.190339 rio-viz-0.9.6/rio_viz/io/reader.py
+-rw-r--r--   0        0        0       25 2022-06-14 08:49:55.190339 rio-viz-0.9.6/rio_viz/resources/__init__.py
+-rw-r--r--   0        0        0     1895 2022-06-14 08:49:55.190339 rio-viz-0.9.6/rio_viz/resources/enums.py
+-rw-r--r--   0        0        0       19 2022-06-14 08:49:55.190339 rio-viz-0.9.6/rio_viz/scripts/__init__.py
+-rw-r--r--   0        0        0     4814 2022-06-14 08:49:55.190339 rio-viz-0.9.6/rio_viz/scripts/cli.py
+-rw-r--r--   0        0        0   179483 2022-06-14 08:49:55.190339 rio-viz-0.9.6/rio_viz/src/css/assembly.min.css
+-rw-r--r--   0        0        0    34683 2022-06-14 08:49:55.190339 rio-viz-0.9.6/rio_viz/src/css/mapbox-gl.css
+-rw-r--r--   0        0        0    48874 2022-06-14 08:49:55.190339 rio-viz-0.9.6/rio_viz/src/js/assembly.js
+-rw-r--r--   0        0        0   472081 2022-06-14 08:49:55.194339 rio-viz-0.9.6/rio_viz/src/js/d3.v4.js
+-rw-r--r--   0        0        0   744707 2022-06-14 08:49:55.198339 rio-viz-0.9.6/rio_viz/src/js/mapbox-gl.js
+-rw-r--r--   0        0        0  3028436 2022-06-14 08:49:55.218339 rio-viz-0.9.6/rio_viz/src/js/mapbox-gl.js.map
+-rw-r--r--   0        0        0    36425 2022-06-14 08:49:55.218339 rio-viz-0.9.6/rio_viz/templates/assets.html
+-rw-r--r--   0        0        0    36738 2022-06-14 08:49:55.218339 rio-viz-0.9.6/rio_viz/templates/bands.html
+-rw-r--r--   0        0        0    36926 2022-06-14 08:49:55.218339 rio-viz-0.9.6/rio_viz/templates/index.html
+-rw-r--r--   0        0        0     2955 2022-06-14 08:49:55.218339 rio-viz-0.9.6/rio_viz/templates/wmts.xml
+-rw-r--r--   0        0        0     6658 1970-01-01 00:00:00.000000 rio-viz-0.9.6/PKG-INFO
```

### Comparing `rio-viz-0.9.5/.gitignore` & `rio-viz-0.9.6/.gitignore`

 * *Files identical despite different names*

### Comparing `rio-viz-0.9.5/.pre-commit-config.yaml` & `rio-viz-0.9.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `rio-viz-0.9.5/Dockerfile` & `rio-viz-0.9.6/Dockerfile`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 RUN apt-get update
 
 COPY rio_viz rio_viz
 COPY pyproject.toml pyproject.toml
 COPY README.md README.md
 
-RUN pip install . rasterio>=1.3a3 --no-cache-dir --upgrade
+RUN pip install . rasterio>=1.3b1 --no-cache-dir --upgrade
 
 # We add additional readers provided by rio-tiler-pds
 RUN pip install rio-tiler-pds
 
 ENV GDAL_INGESTED_BYTES_AT_OPEN 32768
 ENV GDAL_DISABLE_READDIR_ON_OPEN EMPTY_DIR
 ENV GDAL_HTTP_MERGE_CONSECUTIVE_RANGES YES
```

### Comparing `rio-viz-0.9.5/LICENSE` & `rio-viz-0.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `rio-viz-0.9.5/README.md` & `rio-viz-0.9.6/README.md`

 * *Files identical despite different names*

### Comparing `rio-viz-0.9.5/pyproject.toml` & `rio-viz-0.9.6/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -16,16 +16,16 @@
     "Programming Language :: Python :: 3.9",
     "Topic :: Scientific/Engineering :: GIS",
 ]
 dynamic = ["version"]
 dependencies = [
     "braceexpand",
     "rio-cogeo>=3.1",
-    "titiler.core>=0.5,<0.7",
-    "starlette-cramjam>=0.1.0,<0.2",
+    "titiler.core>=0.5,<0.8",
+    "starlette-cramjam>=0.3,<0.4",
     "uvicorn",
 ]
 
 [project.optional-dependencies]
 mvt = [
     "rio-tiler-mvt==0.0.1.dev2",
 ]
```

### Comparing `rio-viz-0.9.5/rio_viz/app.py` & `rio-viz-0.9.6/rio_viz/app.py`

 * *Files identical despite different names*

### Comparing `rio-viz-0.9.5/rio_viz/compat.py` & `rio-viz-0.9.6/rio_viz/compat.py`

 * *Files identical despite different names*

### Comparing `rio-viz-0.9.5/rio_viz/io/mosaic.py` & `rio-viz-0.9.6/rio_viz/io/mosaic.py`

 * *Files identical despite different names*

### Comparing `rio-viz-0.9.5/rio_viz/io/reader.py` & `rio-viz-0.9.6/rio_viz/io/reader.py`

 * *Files identical despite different names*

### Comparing `rio-viz-0.9.5/rio_viz/resources/enums.py` & `rio-viz-0.9.6/rio_viz/resources/enums.py`

 * *Files identical despite different names*

### Comparing `rio-viz-0.9.5/rio_viz/scripts/cli.py` & `rio-viz-0.9.6/rio_viz/scripts/cli.py`

 * *Files identical despite different names*

### Comparing `rio-viz-0.9.5/rio_viz/src/css/assembly.min.css` & `rio-viz-0.9.6/rio_viz/src/css/assembly.min.css`

 * *Files identical despite different names*

### Comparing `rio-viz-0.9.5/rio_viz/src/css/mapbox-gl.css` & `rio-viz-0.9.6/rio_viz/src/css/mapbox-gl.css`

 * *Files identical despite different names*

### Comparing `rio-viz-0.9.5/rio_viz/src/js/assembly.js` & `rio-viz-0.9.6/rio_viz/src/js/assembly.js`

 * *Files identical despite different names*

### Comparing `rio-viz-0.9.5/rio_viz/src/js/d3.v4.js` & `rio-viz-0.9.6/rio_viz/src/js/d3.v4.js`

 * *Files identical despite different names*

### Comparing `rio-viz-0.9.5/rio_viz/src/js/mapbox-gl.js` & `rio-viz-0.9.6/rio_viz/src/js/mapbox-gl.js`

 * *Files identical despite different names*

### Comparing `rio-viz-0.9.5/rio_viz/src/js/mapbox-gl.js.map` & `rio-viz-0.9.6/rio_viz/src/js/mapbox-gl.js.map`

 * *Files identical despite different names*

### Comparing `rio-viz-0.9.5/rio_viz/templates/assets.html` & `rio-viz-0.9.6/rio_viz/templates/assets.html`

 * *Files identical despite different names*

### Comparing `rio-viz-0.9.5/rio_viz/templates/bands.html` & `rio-viz-0.9.6/rio_viz/templates/bands.html`

 * *Files identical despite different names*

### Comparing `rio-viz-0.9.5/rio_viz/templates/index.html` & `rio-viz-0.9.6/rio_viz/templates/index.html`

 * *Files identical despite different names*

### Comparing `rio-viz-0.9.5/rio_viz/templates/wmts.xml` & `rio-viz-0.9.6/rio_viz/templates/wmts.xml`

 * *Files identical despite different names*

### Comparing `rio-viz-0.9.5/PKG-INFO` & `rio-viz-0.9.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: rio-viz
-Version: 0.9.5
+Version: 0.9.6
 Summary: Visualize Cloud Optimized GeoTIFF in browser
 Author-email: Vincent Sarago <vincent@developmentseed.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering :: GIS
 Requires-Dist: braceexpand
 Requires-Dist: rio-cogeo>=3.1
-Requires-Dist: titiler.core>=0.5,<0.7
-Requires-Dist: starlette-cramjam>=0.1.0,<0.2
+Requires-Dist: titiler.core>=0.5,<0.8
+Requires-Dist: starlette-cramjam>=0.3,<0.4
 Requires-Dist: uvicorn
 Requires-Dist: pre-commit ; extra == "dev"
 Requires-Dist: rio-tiler-mvt==0.0.1.dev2 ; extra == "mvt"
 Requires-Dist: pytest ; extra == "test"
 Requires-Dist: pytest-cov ; extra == "test"
 Requires-Dist: pytest-asyncio ; extra == "test"
 Requires-Dist: requests ; extra == "test"
```

#### html2text {}

```diff
@@ -1,17 +1,17 @@
-Metadata-Version: 2.1 Name: rio-viz Version: 0.9.5 Summary: Visualize Cloud
+Metadata-Version: 2.1 Name: rio-viz Version: 0.9.6 Summary: Visualize Cloud
 Optimized GeoTIFF in browser Author-email: Vincent Sarago
 developmentseed.com> Requires-Python: >=3.7 Description-Content-Type: text/
 markdown Classifier: Intended Audience :: Information Technology Classifier:
 Intended Audience :: Science/Research Classifier: License :: OSI Approved ::
 BSD License Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Topic :: Scientific/Engineering :: GIS Requires-Dist:
-braceexpand Requires-Dist: rio-cogeo>=3.1 Requires-Dist: titiler.core>=0.5,<0.7
-Requires-Dist: starlette-cramjam>=0.1.0,<0.2 Requires-Dist: uvicorn Requires-
+braceexpand Requires-Dist: rio-cogeo>=3.1 Requires-Dist: titiler.core>=0.5,<0.8
+Requires-Dist: starlette-cramjam>=0.3,<0.4 Requires-Dist: uvicorn Requires-
 Dist: pre-commit ; extra == "dev" Requires-Dist: rio-tiler-mvt==0.0.1.dev2 ;
 extra == "mvt" Requires-Dist: pytest ; extra == "test" Requires-Dist: pytest-
 cov ; extra == "test" Requires-Dist: pytest-asyncio ; extra == "test" Requires-
 Dist: requests ; extra == "test" Project-URL: Source, https://github.com/
 developmentseed/rio-viz Provides-Extra: dev Provides-Extra: mvt Provides-Extra:
 test # rio-viz
   [https://user-images.githubusercontent.com/10407788/60689165-78be7780-9e88-
```


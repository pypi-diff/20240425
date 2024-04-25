# Comparing `tmp/datasette-leaflet-geojson-0.8.1.tar.gz` & `tmp/datasette_leaflet_geojson-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datasette-leaflet-geojson-0.8.1.tar", last modified: Thu Dec  7 20:55:25 2023, max compression
+gzip compressed data, was "datasette_leaflet_geojson-0.8.2.tar", last modified: Thu Apr 25 05:05:27 2024, max compression
```

## Comparing `datasette-leaflet-geojson-0.8.1.tar` & `datasette_leaflet_geojson-0.8.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 20:55:25.048192 datasette-leaflet-geojson-0.8.1/
--rw-r--r--   0 runner    (1001) docker     (127)     2197 2023-12-07 20:55:25.048192 datasette-leaflet-geojson-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1716 2023-12-07 20:55:09.000000 datasette-leaflet-geojson-0.8.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 20:55:25.044192 datasette-leaflet-geojson-0.8.1/datasette_leaflet_geojson/
--rw-r--r--   0 runner    (1001) docker     (127)     1739 2023-12-07 20:55:09.000000 datasette-leaflet-geojson-0.8.1/datasette_leaflet_geojson/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 20:55:25.048192 datasette-leaflet-geojson-0.8.1/datasette_leaflet_geojson/static/
--rw-r--r--   0 runner    (1001) docker     (127)     3666 2023-12-07 20:55:09.000000 datasette-leaflet-geojson-0.8.1/datasette_leaflet_geojson/static/datasette-leaflet-geojson.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 20:55:25.048192 datasette-leaflet-geojson-0.8.1/datasette_leaflet_geojson.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2197 2023-12-07 20:55:25.000000 datasette-leaflet-geojson-0.8.1/datasette_leaflet_geojson.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      461 2023-12-07 20:55:25.000000 datasette-leaflet-geojson-0.8.1/datasette_leaflet_geojson.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-07 20:55:25.000000 datasette-leaflet-geojson-0.8.1/datasette_leaflet_geojson.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2023-12-07 20:55:25.000000 datasette-leaflet-geojson-0.8.1/datasette_leaflet_geojson.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2023-12-07 20:55:25.000000 datasette-leaflet-geojson-0.8.1/datasette_leaflet_geojson.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2023-12-07 20:55:25.000000 datasette-leaflet-geojson-0.8.1/datasette_leaflet_geojson.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-07 20:55:25.048192 datasette-leaflet-geojson-0.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2023-12-07 20:55:09.000000 datasette-leaflet-geojson-0.8.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 20:55:25.048192 datasette-leaflet-geojson-0.8.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      613 2023-12-07 20:55:09.000000 datasette-leaflet-geojson-0.8.1/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2023-12-07 20:55:09.000000 datasette-leaflet-geojson-0.8.1/tests/test_render_cell.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 05:05:27.474771 datasette_leaflet_geojson-0.8.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-04-25 05:05:27.474771 datasette_leaflet_geojson-0.8.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1716 2024-04-25 05:05:22.000000 datasette_leaflet_geojson-0.8.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 05:05:27.470771 datasette_leaflet_geojson-0.8.2/datasette_leaflet_geojson/
+-rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-04-25 05:05:22.000000 datasette_leaflet_geojson-0.8.2/datasette_leaflet_geojson/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 05:05:27.474771 datasette_leaflet_geojson-0.8.2/datasette_leaflet_geojson/static/
+-rw-r--r--   0 runner    (1001) docker     (127)     4314 2024-04-25 05:05:22.000000 datasette_leaflet_geojson-0.8.2/datasette_leaflet_geojson/static/datasette-leaflet-geojson.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 05:05:27.474771 datasette_leaflet_geojson-0.8.2/datasette_leaflet_geojson.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-04-25 05:05:27.000000 datasette_leaflet_geojson-0.8.2/datasette_leaflet_geojson.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-25 05:05:27.000000 datasette_leaflet_geojson-0.8.2/datasette_leaflet_geojson.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 05:05:27.000000 datasette_leaflet_geojson-0.8.2/datasette_leaflet_geojson.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-25 05:05:27.000000 datasette_leaflet_geojson-0.8.2/datasette_leaflet_geojson.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-25 05:05:27.000000 datasette_leaflet_geojson-0.8.2/datasette_leaflet_geojson.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-25 05:05:27.000000 datasette_leaflet_geojson-0.8.2/datasette_leaflet_geojson.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 05:05:27.474771 datasette_leaflet_geojson-0.8.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-04-25 05:05:22.000000 datasette_leaflet_geojson-0.8.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 05:05:27.474771 datasette_leaflet_geojson-0.8.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-25 05:05:22.000000 datasette_leaflet_geojson-0.8.2/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-04-25 05:05:22.000000 datasette_leaflet_geojson-0.8.2/tests/test_render_cell.py
```

### Comparing `datasette-leaflet-geojson-0.8.1/PKG-INFO` & `datasette_leaflet_geojson-0.8.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datasette-leaflet-geojson
-Version: 0.8.1
+Version: 0.8.2
 Summary:  A Datasette plugin that renders GeoJSON columns using Leaflet
 Home-page: https://github.com/simonw/datasette-leaflet-geojson
 Author: Simon Willison
 License: Apache License, Version 2.0
 Description-Content-Type: text/markdown
 Requires-Dist: datasette>=0.54
 Requires-Dist: datasette-leaflet>=0.2
```

### Comparing `datasette-leaflet-geojson-0.8.1/README.md` & `datasette_leaflet_geojson-0.8.2/README.md`

 * *Files identical despite different names*

### Comparing `datasette-leaflet-geojson-0.8.1/datasette_leaflet_geojson/__init__.py` & `datasette_leaflet_geojson-0.8.2/datasette_leaflet_geojson/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,16 @@
         data = json.loads(value)
     except (ValueError, TypeError):
         return None
     if not isinstance(data, dict):
         return None
     if "type" not in data:
         return None
+    if not isinstance(data["type"], str):
+        return None
     if data["type"] in GEOJSON_TYPES:
         # Reduce floating point accuracy to something sensible
         return json.dumps(round_floats(data))
     return None
 
 
 def round_floats(o):
```

### Comparing `datasette-leaflet-geojson-0.8.1/datasette_leaflet_geojson/static/datasette-leaflet-geojson.js` & `datasette_leaflet_geojson-0.8.2/datasette_leaflet_geojson/static/datasette-leaflet-geojson.js`

 * *Files 16% similar despite different names*

#### js-beautify {}

```diff
@@ -53,28 +53,45 @@
         el.style.backgroundColor = "#eee";
         while (td.firstChild) {
             td.removeChild(td.firstChild);
         }
         td.appendChild(el);
 
         function addMap() {
-            let map = L.map(el, {
-                layers: [
-                    L.tileLayer(tilesUrl, {
-                        maxZoom: 19,
-                        detectRetina: true,
-                        attribution: attribution,
-                    }),
-                ],
-            });
-            let layer = L.geoJSON(data);
-            layer.addTo(map);
-            map.fitBounds(layer.getBounds(), {
-                maxZoom: 14,
-            });
+            var map = null;
+            try {
+                map = L.map(el, {
+                    layers: [
+                        L.tileLayer(tilesUrl, {
+                            maxZoom: 19,
+                            detectRetina: true,
+                            attribution: attribution,
+                        }),
+                    ],
+                });
+                let layer = L.geoJSON(data);
+                layer.addTo(map);
+                map.fitBounds(layer.getBounds(), {
+                    maxZoom: 14,
+                });
+            } catch (error) {
+                console.warn("Map creation failed", data, error);
+                let div = document.createElement("div");
+                div.innerHTML = "Error while displaying map: " + error;
+                div.style.color = "#666";
+                div.style.display = "flex";
+                div.style.justifyContent = "center";
+                div.style.alignItems = "center";
+                div.style.height = "400px";
+
+                if (map) {
+                    map.remove();
+                }
+                el.appendChild(div);
+            }
         }
         if (activate) {
             addMap();
         } else {
             let a = document.createElement("a");
             a.innerHTML = "Click to show map";
             a.href = "#";
@@ -117,19 +134,23 @@
                     data: data,
                 });
             });
         if (tdsToUpgrade.length) {
             loadDependencies(() => {
                 let numDone = 0;
                 tdsToUpgrade.forEach((item) => {
-                    upgradeTd(
-                        item,
-                        numDone < window.DATASETTE_LEAFLET_GEOJSON_DEFAULT_MAPS_TO_LOAD
-                    );
-                    numDone += 1;
+                    try {
+                        upgradeTd(
+                            item,
+                            numDone < window.DATASETTE_LEAFLET_GEOJSON_DEFAULT_MAPS_TO_LOAD
+                        );
+                        numDone += 1;
+                    } catch (error) {
+                        console.warn("Failed to add map for", item, error);
+                    }
                 });
             });
         }
         // don't throw an error if another JS library expect Events to be attached to the DOM.
         // Happens with Plot/D3
         try {
             window.dispatchEvent(new Event("resize"));
```

### Comparing `datasette-leaflet-geojson-0.8.1/datasette_leaflet_geojson.egg-info/PKG-INFO` & `datasette_leaflet_geojson-0.8.2/datasette_leaflet_geojson.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datasette-leaflet-geojson
-Version: 0.8.1
+Version: 0.8.2
 Summary:  A Datasette plugin that renders GeoJSON columns using Leaflet
 Home-page: https://github.com/simonw/datasette-leaflet-geojson
 Author: Simon Willison
 License: Apache License, Version 2.0
 Description-Content-Type: text/markdown
 Requires-Dist: datasette>=0.54
 Requires-Dist: datasette-leaflet>=0.2
```

### Comparing `datasette-leaflet-geojson-0.8.1/setup.py` & `datasette_leaflet_geojson-0.8.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 import os
 
-VERSION = "0.8.1"
+VERSION = "0.8.2"
 
 
 def get_long_description():
     with open(
         os.path.join(os.path.dirname(os.path.abspath(__file__)), "README.md"),
         encoding="utf8",
     ) as fp:
```

### Comparing `datasette-leaflet-geojson-0.8.1/tests/test_config.py` & `datasette_leaflet_geojson-0.8.2/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `datasette-leaflet-geojson-0.8.1/tests/test_render_cell.py` & `datasette_leaflet_geojson-0.8.2/tests/test_render_cell.py`

 * *Files 12% similar despite different names*

```diff
@@ -37,7 +37,18 @@
         }
     )
     actual = render_cell(value)
     assert {
         "type": "MultiPolygon",
         "coordinates": [[[[-122.33006, 37.44676], [-122.32875, 37.44794]]]],
     } == json.loads(actual)
+
+
+def test_render_cell_not_confused_by_other_properties():
+    # https://github.com/simonw/datasette-leaflet-geojson/issues/24
+    value = json.dumps(
+        {
+            "type": {"type": "string"},
+        }
+    )
+    actual = render_cell(value)
+    assert actual is None
```


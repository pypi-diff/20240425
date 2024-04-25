# Comparing `tmp/d3vis_ipynb-0.1.2.tar.gz` & `tmp/d3vis_ipynb-0.1.3.tar.gz`

## Comparing `d3vis_ipynb-0.1.2.tar` & `d3vis_ipynb-0.1.3.tar`

### file list

```diff
@@ -1,41 +1,45 @@
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.2/D3vis_ipynb.json
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.2/MANIFEST.in
--rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.2/RELEASE.md
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.2/install.json
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.2/setup.cfg
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.2/setup.py
--rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.2/d3vis_ipynb/__init__.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.2/d3vis_ipynb/_version.py
--rw-r--r--   0        0        0     5686 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.2/d3vis_ipynb/embedding.py
--rw-r--r--   0        0        0     2054 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.2/d3vis_ipynb/web.py
--rw-r--r--   0        0        0     4552 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.2/d3vis_ipynb/widgets.py
--rw-r--r--   0        0        0     1966 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.2/d3vis_ipynb/labextension/package.json
--rw-r--r--   0        0        0    23018 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.2/d3vis_ipynb/labextension/static/380.5f71b19ff5261cd2e5de.js
--rw-r--r--   0        0        0    23626 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.2/d3vis_ipynb/labextension/static/493.6062c0a7b585f6ae1d22.js
--rw-r--r--   0        0        0   282230 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.2/d3vis_ipynb/labextension/static/693.c8409ce8329f6703470f.js
--rw-r--r--   0        0        0     6875 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.2/d3vis_ipynb/labextension/static/remoteEntry.bf58726a1c33e2ff91a1.js
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.2/d3vis_ipynb/labextension/static/style.js
--rw-r--r--   0        0        0    35163 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.2/d3vis_ipynb/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0    88816 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.2/d3vis_ipynb/nbextension/index.js
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.2/js/README.md
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.2/js/amd-public-path.js
--rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.2/js/package.json
--rw-r--r--   0        0        0     2828 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.2/js/webpack.config.js
--rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.2/js/webpack.exports.config.js
--rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.2/js/css/widget.css
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.2/js/lib/extension.js
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.2/js/lib/index.js
--rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.2/js/lib/labplugin.js
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.2/js/lib/web-dev.js
--rw-r--r--   0        0        0     9759 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.2/js/lib/widgets.js
--rw-r--r--   0        0        0     9087 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.2/js/lib/graphs/barplot.js
--rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.2/js/lib/graphs/histogramplot.js
--rw-r--r--   0        0        0     3680 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.2/js/lib/graphs/linearhistplot.js
--rw-r--r--   0        0        0     4355 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.2/js/lib/graphs/scatterplot.js
--rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.2/js/lib/tools/lasso.js
--rw-r--r--   0        0        0     5894 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.2/js/lib/wrappers/embedding.wrapper.js
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.2/.gitignore
--rw-r--r--   0        0        0     1503 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.2/LICENSE.txt
--rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.2/README.md
--rw-r--r--   0        0        0     2583 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     4165 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.3/D3vis_ipynb.json
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.3/MANIFEST.in
+-rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.3/RELEASE.md
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.3/install.json
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.3/setup.cfg
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.3/setup.py
+-rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.3/d3vis_ipynb/__init__.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.3/d3vis_ipynb/_version.py
+-rw-r--r--   0        0        0     5686 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.3/d3vis_ipynb/embedding.py
+-rw-r--r--   0        0        0     2309 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.3/d3vis_ipynb/web.py
+-rw-r--r--   0        0        0     5804 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.3/d3vis_ipynb/widgets.py
+-rw-r--r--   0        0        0     1966 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.3/d3vis_ipynb/labextension/package.json
+-rw-r--r--   0        0        0    27776 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.3/d3vis_ipynb/labextension/static/363.e98e5e3babbb9b69956a.js
+-rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.3/d3vis_ipynb/labextension/static/493.053b071a46f0bcccaab9.js
+-rw-r--r--   0        0        0   282230 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.3/d3vis_ipynb/labextension/static/693.c8409ce8329f6703470f.js
+-rw-r--r--   0        0        0     6790 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.3/d3vis_ipynb/labextension/static/remoteEntry.8f26db161f1984f5ad68.js
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.3/d3vis_ipynb/labextension/static/style.js
+-rw-r--r--   0        0        0    35163 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.3/d3vis_ipynb/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0    93598 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.3/d3vis_ipynb/nbextension/index.js
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.3/js/README.md
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.3/js/amd-public-path.js
+-rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.3/js/package.json
+-rw-r--r--   0        0        0     2828 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.3/js/webpack.config.js
+-rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.3/js/webpack.exports.config.js
+-rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.3/js/css/widget.css
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.3/js/lib/extension.js
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.3/js/lib/index.js
+-rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.3/js/lib/labplugin.js
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.3/js/lib/web-dev.js
+-rw-r--r--   0        0        0    12733 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.3/js/lib/widgets.js
+-rw-r--r--   0        0        0     9087 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.3/js/lib/graphs/barplot.js
+-rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.3/js/lib/graphs/histogramplot.js
+-rw-r--r--   0        0        0     3987 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.3/js/lib/graphs/linearhistplot.js
+-rw-r--r--   0        0        0     3071 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.3/js/lib/graphs/rangeslider.js
+-rw-r--r--   0        0        0     4355 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.3/js/lib/graphs/scatterplot.js
+-rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.3/js/lib/tools/lasso.js
+-rw-r--r--   0        0        0     5894 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.3/js/lib/wrappers/embedding.wrapper.js
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.3/testes/index.html
+-rw-r--r--   0        0        0     1481 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.3/testes/index.js
+-rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.3/testes/style.css
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.3/.gitignore
+-rw-r--r--   0        0        0     1503 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.3/LICENSE.txt
+-rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.3/README.md
+-rw-r--r--   0        0        0     2599 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     4165 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.3/PKG-INFO
```

### Comparing `d3vis_ipynb-0.1.2/RELEASE.md` & `d3vis_ipynb-0.1.3/RELEASE.md`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.1.2/setup.cfg` & `d3vis_ipynb-0.1.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.1.2/d3vis_ipynb/__init__.py` & `d3vis_ipynb-0.1.3/d3vis_ipynb/__init__.py`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.1.2/d3vis_ipynb/embedding.py` & `d3vis_ipynb-0.1.3/d3vis_ipynb/embedding.py`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.1.2/d3vis_ipynb/web.py` & `d3vis_ipynb-0.1.3/d3vis_ipynb/web.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,19 +5,26 @@
 class WebWidget(anywidget.AnyWidget):
     def readFromWeb(url):
         http = urllib3.PoolManager(cert_reqs="CERT_NONE")
         response = http.request("GET", url)
         text = response.data.decode("utf-8")
         return text
 
-    def createWidgetFromUrl(widgetCall: str, varList: list, jsUrl: str):
+    def createWidgetFromUrl(
+        widgetCall: str, varList: list, updatableVars: list, jsUrl: str
+    ):
         modelVars = ""
+        modelChanges = ""
         for var in varList:
-            newLine = "let " + var + ' = model.get("' + var + '");\n'
-            modelVars += newLine
+            newModelVar = "let " + var + ' = model.get("' + var + '");\n'
+            modelVars += newModelVar
+
+        for var in updatableVars:
+            newModelChange = 'model.on("change:' + var + '", plotAfterInterval);\n'
+            modelChanges += newModelChange
 
         jsUrlStr = WebWidget.readFromWeb(jsUrl)
         jsStr = """
         import * as d3 from "https://esm.sh/d3@7";
 
         function render({{ model, el }} ) {{
             {jsUrlStr}
@@ -46,23 +53,26 @@
                 const margin = {{ top: 20, right: 20, bottom: 30, left: 40 }};
                 
                 {widgetCall};
             }}
 
             plotAfterInterval();
             
-            model.on("change:data", plotAfterInterval);
-            window.addEventListener("resize", () => plotAfterInterval(this).bind(this));
+            {modelChanges}
+            window.addEventListener("resize", () => plotAfterInterval(this));
         }}
         
         
 
         export default {{ render }};
         """.format(
-            jsUrlStr=jsUrlStr, modelVars=modelVars, widgetCall=widgetCall
+            jsUrlStr=jsUrlStr,
+            modelVars=modelVars,
+            widgetCall=widgetCall,
+            modelChanges=modelChanges,
         )
 
         return jsStr
 
     def linkData(self, widget, widgetAttr):
         def callback(change):
             self.data = getattr(widget, widgetAttr)
```

### Comparing `d3vis_ipynb-0.1.2/d3vis_ipynb/widgets.py` & `d3vis_ipynb-0.1.3/d3vis_ipynb/widgets.py`

 * *Files 12% similar despite different names*

```diff
@@ -33,14 +33,17 @@
             "histogramData": self.histogramData,
             "elementId": self.elementId,
             "observing": self._observing,
         }
 
         return {self._name: data}
 
+    def on_click_value(self, callback):
+        self.observe(callback, names=["clickedValue"])
+
 
 @widgets.register
 class ScatterPlot(widgets.DOMWidget):
     _view_name = Unicode("ScatterPlotView").tag(sync=True)
     _model_name = Unicode("ScatterPlotModel").tag(sync=True)
     _view_module = Unicode("d3vis_ipynb").tag(sync=True)
     _model_module = Unicode("d3vis_ipynb").tag(sync=True)
@@ -69,14 +72,20 @@
             "hue": self.hue,
             "elementId": self.elementId,
             "observing": self._observing,
         }
 
         return {self._name: data}
 
+    def on_select_values(self, callback):
+        self.observe(callback, names=["selectedValues"])
+
+    def on_click_value(self, callback):
+        self.observe(callback, names=["clickedValue"])
+
 
 @widgets.register
 class BarPlot(widgets.DOMWidget):
     _view_name = Unicode("BarPlotView").tag(sync=True)
     _model_name = Unicode("BarPlotModel").tag(sync=True)
     _view_module = Unicode("d3vis_ipynb").tag(sync=True)
     _model_module = Unicode("d3vis_ipynb").tag(sync=True)
@@ -103,22 +112,14 @@
             "hue": self.hue,
             "elementId": self.elementId,
             "observing": self._observing,
         }
 
         return {self._name: data}
 
-    def linkData(self, widget, widgetAttr):
-        self._observing.append({"data": {widget.name(): widgetAttr}})
-
-        def callback(change):
-            self.data = getattr(widget, widgetAttr)
-
-        widget.observe(callback, names=[widgetAttr])
-
 
 @widgets.register
 class HistogramPlot(widgets.DOMWidget):
     _view_name = Unicode("HistogramPlotView").tag(sync=True)
     _model_name = Unicode("HistogramPlotModel").tag(sync=True)
     _view_module = Unicode("d3vis_ipynb").tag(sync=True)
     _model_module = Unicode("d3vis_ipynb").tag(sync=True)
@@ -144,7 +145,46 @@
             "start": self.start,
             "end": self.end,
             "elementId": self.elementId,
             "observing": self._observing,
         }
 
         return {self._name: data}
+
+
+@widgets.register
+class RangeSlider(widgets.DOMWidget):
+    _view_name = Unicode("RangeSliderView").tag(sync=True)
+    _model_name = Unicode("RangeSliderModel").tag(sync=True)
+    _view_module = Unicode("d3vis_ipynb").tag(sync=True)
+    _model_module = Unicode("d3vis_ipynb").tag(sync=True)
+    _view_module_version = Unicode(NPM_PACKAGE_RANGE).tag(sync=True)
+    _model_module_version = Unicode(NPM_PACKAGE_RANGE).tag(sync=True)
+
+    _name = "rangeslider"
+    _observing = []
+
+    data = List([]).tag(sync=True)
+    variable = Unicode().tag(sync=True)
+    step = Float().tag(sync=True)
+    description = Unicode().tag(sync=True)
+    minValue = Float().tag(sync=True)
+    maxValue = Float().tag(sync=True)
+    elementId = Unicode().tag(sync=True)
+
+    def name(self):
+        return self._name
+
+    def export_data(self):
+        data = {
+            "data": self.data,
+            "variable": self.variable,
+            "step": self.step,
+            "description": self.description,
+            "elementId": self.elementId,
+            "observing": self._observing,
+        }
+
+        return {self._name: data}
+
+    def on_drag(self, callback):
+        self.observe(callback, names=["minValue", "maxValue"])
```

### Comparing `d3vis_ipynb-0.1.2/d3vis_ipynb/labextension/package.json` & `d3vis_ipynb-0.1.3/d3vis_ipynb/labextension/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9603365384615384%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.8f26db161f1984f5ad68.js'}}",*

 * * "'version'": "'0.1.3'"}*

```diff
@@ -16,15 +16,15 @@
         "lib/**/*.js",
         "dist/*.js",
         "css/*.css"
     ],
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.bf58726a1c33e2ff91a1.js"
+            "load": "static/remoteEntry.8f26db161f1984f5ad68.js"
         },
         "extension": "lib/labplugin",
         "outputDir": "../d3vis_ipynb/labextension",
         "sharedPackages": {
             "@jupyter-widgets/base": {
                 "bundled": false,
                 "singleton": true
@@ -54,9 +54,9 @@
         "export": "webpack --env export --config webpack.exports.config.js",
         "prepublish": "yarn run clean && yarn run build:prod",
         "start": "webpack serve --open --config webpack.exports.config.js",
         "start:export": "webpack serve --open --config webpack.exports.config.js --env export",
         "test": "echo \"Error: no test specified\" && exit 1",
         "watch": "webpack --watch --mode=development"
     },
-    "version": "0.1.2"
+    "version": "0.1.3"
 }
```

### Comparing `d3vis_ipynb-0.1.2/d3vis_ipynb/labextension/static/380.5f71b19ff5261cd2e5de.js` & `d3vis_ipynb-0.1.3/d3vis_ipynb/labextension/static/363.e98e5e3babbb9b69956a.js`

 * *Files 15% similar despite different names*

#### js-beautify {}

```diff
@@ -1,64 +1,66 @@
 "use strict";
 (self.webpackChunkd3vis_ipynb = self.webpackChunkd3vis_ipynb || []).push([
-    [380, 56], {
-        380: (e, t, n) => {
+    [363], {
+        363: (e, t, n) => {
             n.r(t), n.d(t, {
-                BarPlotModel: () => L,
-                BarPlotView: () => j,
-                EmbeddingModel: () => O,
-                EmbeddingView: () => I,
+                BarPlotModel: () => S,
+                BarPlotView: () => V,
+                EmbeddingModel: () => C,
+                EmbeddingView: () => O,
                 HistogramPlotModel: () => D,
-                HistogramPlotView: () => V,
+                HistogramPlotView: () => j,
                 LinearHistPlotModel: () => M,
-                LinearHistPlotView: () => S,
-                ScatterPlotModel: () => A,
-                ScatterPlotView: () => E,
-                author: () => C.author,
-                dependencies: () => C.dependencies,
-                description: () => C.description,
-                devDependencies: () => C.devDependencies,
-                files: () => C.files,
-                jupyterlab: () => C.jupyterlab,
-                keywords: () => C.keywords,
-                license: () => C.license,
-                main: () => C.main,
-                name: () => C.name,
-                repository: () => C.repository,
-                scripts: () => C.scripts,
-                version: () => C.version
+                LinearHistPlotView: () => E,
+                RangeSliderModel: () => I,
+                RangeSliderView: () => B,
+                ScatterPlotModel: () => L,
+                ScatterPlotView: () => A,
+                author: () => W.author,
+                dependencies: () => W.dependencies,
+                description: () => W.description,
+                devDependencies: () => W.devDependencies,
+                files: () => W.files,
+                jupyterlab: () => W.jupyterlab,
+                keywords: () => W.keywords,
+                license: () => W.license,
+                main: () => W.main,
+                name: () => W.name,
+                repository: () => W.repository,
+                scripts: () => W.scripts,
+                version: () => W.version
             });
             var a = n(801),
-                r = n(840);
+                i = n(72),
+                o = n.n(i),
+                s = n(825),
+                r = n.n(s),
+                l = n(659),
+                d = n.n(l),
+                c = n(56),
+                m = n.n(c),
+                u = n(540),
+                p = n.n(u),
+                h = n(113),
+                g = n.n(h),
+                v = n(930),
+                f = {};
+            f.styleTagTransform = g(), f.setAttributes = m(), f.insert = d().bind(null, "head"), f.domAPI = r(), f.insertStyleElement = p(), o()(v.A, f), v.A && v.A.locals && v.A.locals;
+            var _ = n(840);
 
-            function i(e) {
+            function x(e) {
                 const t = e.reduce(((e, t) => e + t), 0) / e.length,
                     n = 1.96 * function(e, t) {
                         let n = 0;
                         return e.forEach((e => n += (e - t) ** 2)), n = Math.sqrt(n) / e.length, n
                     }(e, t);
                 return [t - n, t + n]
             }
-            var o = n(72),
-                s = n.n(o),
-                l = n(825),
-                d = n.n(l),
-                c = n(659),
-                m = n.n(c),
-                u = n(56),
-                p = n.n(u),
-                h = n(540),
-                f = n.n(h),
-                g = n(113),
-                v = n.n(g),
-                _ = n(930),
-                x = {};
-            x.styleTagTransform = v(), x.setAttributes = p(), x.insert = m().bind(null, "head"), x.domAPI = d(), x.insertStyleElement = f(), s()(_.A, x), _.A && _.A.locals && _.A.locals;
-            const y = n(330),
-                b = 400,
+            const b = n(330),
+                y = 400,
                 w = {
                     top: 20,
                     right: 20,
                     bottom: 30,
                     left: 40
                 };
 
@@ -81,394 +83,398 @@
                         linearData_y: [],
                         histogramData: [],
                         elementId: String,
                         clickedValue: String
                     }
                 }
                 static model_name = "LinearHistPlotModel";
-                static model_module = y.name;
-                static model_module_version = y.version;
+                static model_module = b.name;
+                static model_module_version = b.version;
                 static view_name = "LinearHistPlotView";
-                static view_module = y.name;
-                static view_module_version = y.version
+                static view_module = b.name;
+                static view_module_version = b.version
             }
-            class S extends a.DOMWidgetView {
+            class E extends a.DOMWidgetView {
                 timeout;
                 render() {
-                    k(this), this.model.on("change:linearData_x", (() => k(this)), this), window.addEventListener("resize", (() => k(this).bind(this)))
+                    k(this), this.model.on("change:linearData_x", (() => k(this)), this), this.model.on("change:linearData_y", (() => k(this)), this), this.model.on("change:histogramData", (() => k(this)), this), window.addEventListener("resize", (() => k(this)))
                 }
                 plot() {
                     const e = this.model.get("linearData_x"),
                         t = this.model.get("linearData_y"),
                         n = this.model.get("histogramData"),
                         a = this.model.get("elementId");
-                    let i = b,
+                    let i = y,
                         o = this.el;
                     a && (o = document.getElementById(a), i = o.clientHeight);
                     let s = o.clientWidth;
-                    const l = w;
-                    ! function(e, t, n, a, i, o, s, l) {
-                        const d = o - l.left - l.right,
-                            c = s - l.top - l.bottom,
-                            m = c / 4;
-                        r.select(a).selectAll("*").remove();
-                        const u = Math.min(r.min(e), r.min(n)),
-                            p = Math.max(r.max(e), r.max(n)),
-                            h = r.scaleLinear().range([0, d]),
-                            f = r.scaleLinear().range([c, 0]),
-                            g = r.scaleLinear().range([m, 0]),
-                            v = r.axisBottom(h),
-                            _ = r.axisLeft(f),
-                            x = r.bin().thresholds(20).value((e => Math.round(10 * e) / 10))(n),
-                            y = r.select(a).append("svg").attr("width", o).attr("height", s).append("g").attr("transform", "translate(" + l.left + "," + l.top + ")");
-                        h.domain([u, p]), f.domain(r.extent(t)), g.domain([0, r.max(x, (e => e.length))]);
-                        const b = y.append("g").append("rect").style("fill", "none").attr("width", 160).attr("height", 40).attr("stroke", "#69b3a2").attr("stroke-width", 4).style("opacity", 0),
-                            w = y.append("g").append("text").style("opacity", 0).attr("text-anchor", "left").attr("alignment-baseline", "middle");
-                        y.append("g").attr("transform", "translate(0," + c + ")").call(v).append("text").attr("x", d).attr("y", -6).style("text-anchor", "end"), y.append("g").call(_).append("text").attr("transform", "rotate(-90)").attr("y", 6).attr("dy", ".71em").style("text-anchor", "end"), y.append("path").datum(x).attr("fill", "paleturquoise").attr("stroke", "steelblue").attr("stroke-width", 1).attr("d", r.line().x((e => h((e.x1 + e.x0) / 2))).y((e => g(e.length) + c - m)).curve(r.curveCatmullRom));
-                        const k = e.map(((e, n) => [e, t[n]])).map((([e, t]) => ({
+                    const r = w;
+                    ! function(e, t, n, a, i, o, s, r) {
+                        const l = o - r.left - r.right,
+                            d = s - r.top - r.bottom,
+                            c = d / 4;
+                        _.select(a).selectAll("*").remove();
+                        const m = Math.min(_.min(e), _.min(n)),
+                            u = Math.max(_.max(e), _.max(n)),
+                            p = _.scaleLinear().range([0, l]),
+                            h = _.scaleLinear().range([d, 0]),
+                            g = _.scaleLinear().range([c, 0]),
+                            v = _.axisBottom(p),
+                            f = _.axisLeft(h),
+                            x = _.bin().thresholds(20).value((e => Math.round(10 * e) / 10))(n),
+                            b = _.select(a).append("svg").attr("width", o).attr("height", s).append("g").attr("transform", "translate(" + r.left + "," + r.top + ")");
+                        p.domain([m, u]), h.domain(_.extent(t)), g.domain([0, _.max(x, (e => e.length))]);
+                        const y = b.append("g").append("rect").style("fill", "none").attr("width", 160).attr("height", 40).attr("stroke", "#69b3a2").attr("stroke-width", 4).style("opacity", 0),
+                            w = b.append("g").append("text").style("opacity", 0).attr("text-anchor", "left").attr("alignment-baseline", "middle");
+                        b.append("g").attr("transform", "translate(0," + d + ")").call(v).append("text").attr("x", l).attr("y", -6).style("text-anchor", "end"), b.append("g").call(f).append("text").attr("transform", "rotate(-90)").attr("y", 6).attr("dy", ".71em").style("text-anchor", "end");
+                        const k = [];
+                        k.x0 = x[0].x0 - 2.5, k.x1 = x[0].x1 - 2.5, x.unshift(k);
+                        const M = [];
+                        M.x0 = x[x.length - 1].x0 + 2.5, M.x1 = x[x.length - 1].x1 + 2.5, b.append("path").datum(x).attr("fill", "paleturquoise").attr("stroke", "steelblue").attr("stroke-width", 1).attr("d", _.line().x((e => p((e.x1 + e.x0) / 2))).y((e => g(e.length) + d - c)).curve(_.curveCatmullRom));
+                        const E = e.map(((e, n) => [e, t[n]])).map((([e, t]) => ({
                             x: e,
                             y: t
                         })));
-                        y.append("path").datum(k).attr("fill", "none").attr("stroke", "steelblue").attr("stroke-width", 1.5).attr("d", r.line().x((e => h(e.x))).y((e => f(e.y)))), y.selectAll("myCircles").data(k).enter().append("circle").attr("fill", "red").attr("stroke", "none").attr("cx", (e => h(e.x))).attr("cy", (e => f(e.y))).attr("r", 3).on("mouseover", (function(e, t) {
-                            b.style("opacity", 1), w.style("opacity", 1), b.attr("x", e.offsetX - 30).attr("y", e.offsetY - 40), w.html("x:" + Math.round(10 * t.x) / 10 + "  -  y:" + Math.round(10 * t.y) / 10).attr("x", e.offsetX - 15).attr("y", e.offsetY - 20)
+                        b.append("path").datum(E).attr("fill", "none").attr("stroke", "steelblue").attr("stroke-width", 1.5).attr("d", _.line().x((e => p(e.x))).y((e => h(e.y)))), b.selectAll("myCircles").data(E).enter().append("circle").attr("fill", "red").attr("stroke", "none").attr("cx", (e => p(e.x))).attr("cy", (e => h(e.y))).attr("r", 3).on("mouseover", (function(e, t) {
+                            y.style("opacity", 1), w.style("opacity", 1), y.attr("x", e.offsetX - 30).attr("y", e.offsetY - 40), w.html("x:" + Math.round(10 * t.x) / 10 + "  -  y:" + Math.round(10 * t.y) / 10).attr("x", e.offsetX - 15).attr("y", e.offsetY - 20)
                         })).on("mouseout", (function() {
-                            b.style("opacity", 0), w.style("opacity", 0)
+                            y.style("opacity", 0), w.style("opacity", 0)
                         })).on("click", (function(e, t) {
                             const n = "x:" + Math.round(10 * t.x) / 10 + "  -  y:" + Math.round(10 * t.y) / 10;
                             void 0 !== i && i(n)
                         }))
-                    }(e, t, n, o, this.setValue.bind(this), s, i, l)
+                    }(e, t, n, o, this.setValue.bind(this), s, i, r)
                 }
                 setValue(e) {
                     this.model.set({
                         clickedValue: e
                     }), this.model.save_changes()
                 }
             }
-            class A extends a.DOMWidgetModel {
+            class L extends a.DOMWidgetModel {
                 defaults() {
                     return {
                         ...super.defaults(),
-                        _model_name: A.model_name,
-                        _view_name: A.view_name,
-                        _model_module: A.model_module,
-                        _view_module: A.view_module,
-                        _model_module_version: A.model_module_version,
-                        _view_module_version: A.view_module_version,
+                        _model_name: L.model_name,
+                        _view_name: L.view_name,
+                        _model_module: L.model_module,
+                        _view_module: L.view_module,
+                        _model_module_version: L.model_module_version,
+                        _view_module_version: L.view_module_version,
                         data: [],
                         x: String,
                         y: String,
                         hue: String,
                         elementId: String,
                         clickedValue: String,
                         selectedValues: []
                     }
                 }
                 static model_name = "ScatterplotModel";
-                static model_module = y.name;
-                static model_module_version = y.version;
+                static model_module = b.name;
+                static model_module_version = b.version;
                 static view_name = "ScatterplotView";
-                static view_module = y.name;
-                static view_module_version = y.version
+                static view_module = b.name;
+                static view_module_version = b.version
             }
-            class E extends a.DOMWidgetView {
+            class A extends a.DOMWidgetView {
                 timeout;
                 render() {
-                    k(this), this.model.on("change:data", (() => k(this)), this), window.addEventListener("resize", (() => k(this).bind(this)))
+                    k(this), this.model.on("change:data", (() => k(this)), this), this.model.on("change:x", (() => k(this)), this), this.model.on("change:y", (() => k(this)), this), this.model.on("change:hue", (() => k(this)), this), window.addEventListener("resize", (() => k(this)))
                 }
                 plot() {
                     const e = this.model.get("data"),
                         t = this.model.get("x"),
                         n = this.model.get("y"),
                         a = this.model.get("hue"),
                         i = this.model.get("elementId");
-                    let o = b,
+                    let o = y,
                         s = this.el;
                     i && (s = document.getElementById(i), o = s.clientHeight);
-                    let l = s.clientWidth;
-                    const d = w;
-                    ! function(e, t, n, a, i, o, s, l, d, c) {
-                        const m = l - c.left - c.right,
-                            u = d - c.top - c.bottom;
+                    let r = s.clientWidth;
+                    const l = w;
+                    ! function(e, t, n, a, i, o, s, r, l, d) {
+                        const c = r - d.left - d.right,
+                            m = l - d.top - d.bottom;
                         for (let t = 0; t < e.length; t++) e[t].id = t;
-                        const p = Math.floor(Math.random() * Date.now() * 1e4).toString(36);
-                        r.select(i).selectAll("*").remove();
-                        const h = r.scaleLinear().range([0, m]),
-                            f = r.scaleLinear().range([u, 0]),
-                            g = r.scaleOrdinal(r.schemeCategory10),
-                            v = r.axisBottom(h),
-                            _ = r.axisLeft(f),
-                            x = r.select(i).append("svg").attr("width", l).attr("height", d).append("g").attr("transform", "translate(" + c.left + "," + c.top + ")");
-                        h.domain(r.extent(e, (function(e) {
+                        const u = Math.floor(Math.random() * Date.now() * 1e4).toString(36);
+                        _.select(i).selectAll("*").remove();
+                        const p = _.scaleLinear().range([0, c]),
+                            h = _.scaleLinear().range([m, 0]),
+                            g = _.scaleOrdinal(_.schemeCategory10),
+                            v = _.axisBottom(p),
+                            f = _.axisLeft(h),
+                            x = _.select(i).append("svg").attr("width", r).attr("height", l).append("g").attr("transform", "translate(" + d.left + "," + d.top + ")");
+                        p.domain(_.extent(e, (function(e) {
                                 return e[t]
-                            }))).nice(), f.domain(r.extent(e, (function(e) {
+                            }))).nice(), h.domain(_.extent(e, (function(e) {
                                 return e[n]
-                            }))).nice(), x.append("g").attr("class", "x axis").attr("transform", "translate(0," + u + ")").call(v).append("text").attr("class", "label").attr("x", m).attr("y", -6).style("text-anchor", "end"), x.append("g").attr("class", "y axis").call(_).append("text").attr("class", "label").attr("transform", "rotate(-90)").attr("y", 6).attr("dy", ".71em").style("text-anchor", "end"), x.selectAll(".dot").data(e).enter().append("circle").attr("id", (function(e, t) {
-                                return "dot-" + p + e.id
+                            }))).nice(), x.append("g").attr("class", "x axis").attr("transform", "translate(0," + m + ")").call(v).append("text").attr("class", "label").attr("x", c).attr("y", -6).style("text-anchor", "end"), x.append("g").attr("class", "y axis").call(f).append("text").attr("class", "label").attr("transform", "rotate(-90)").attr("y", 6).attr("dy", ".71em").style("text-anchor", "end"), x.selectAll(".dot").data(e).enter().append("circle").attr("id", (function(e, t) {
+                                return "dot-" + u + e.id
                             })).attr("class", "dot").attr("r", 3.5).attr("cx", (function(e) {
-                                return h(e[t])
+                                return p(e[t])
                             })).attr("cy", (function(e) {
-                                return f(e[n])
+                                return h(e[n])
                             })).style("fill", (function(e) {
                                 return g(e[a])
                             })).on("mouseover", (function(e, a) {
-                                b.style("opacity", 1), w.style("opacity", 1), b.attr("x", e.offsetX - 30).attr("y", e.offsetY - 40), w.html("x: " + Math.round(10 * a[t]) / 10 + "&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;y: " + Math.round(10 * a[n]) / 10).attr("x", e.offsetX - 15).attr("y", e.offsetY - 20)
+                                y.style("opacity", 1), w.style("opacity", 1), y.attr("x", e.offsetX - 30).attr("y", e.offsetY - 40), w.html("x: " + Math.round(10 * a[t]) / 10 + "&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;y: " + Math.round(10 * a[n]) / 10).attr("x", e.offsetX - 15).attr("y", e.offsetY - 20)
                             })).on("mouseout", (function() {
-                                b.style("opacity", 0), w.style("opacity", 0)
+                                y.style("opacity", 0), w.style("opacity", 0)
                             })).on("click", (function(e, a) {
-                                const r = "x:" + Math.round(10 * a[t]) / 10 + "    y:" + Math.round(10 * a[n]) / 10;
-                                void 0 !== o && o(r)
+                                const i = "x:" + Math.round(10 * a[t]) / 10 + "    y:" + Math.round(10 * a[n]) / 10;
+                                void 0 !== o && o(i)
                             })),
-                            function(e, t, n, a, i, o, s, l, d, c) {
-                                let m = [];
-                                const u = r.line(),
-                                    p = r.select(e).selectAll(".dot"),
-                                    h = r.drag().on("start", (function() {
-                                        m = [], l(), r.select(e).select("svg").append("path").attr("id", "lasso" + c)
+                            function(e, t, n, a, i, o, s, r, l, d) {
+                                let c = [];
+                                const m = _.line(),
+                                    u = _.select(e).selectAll(".dot"),
+                                    p = _.drag().on("start", (function() {
+                                        c = [], r(), _.select(e).select("svg").append("path").attr("id", "lasso" + d)
                                     })).on("drag", (function(e) {
                                         let t = e.sourceEvent.offsetX,
                                             n = e.sourceEvent.offsetY;
-                                        m.push([t, n]), r.select("#lasso" + c).style("stroke", "blue").style("stroke-width", 2).style("fill", "#00008854").attr("d", u(m))
+                                        c.push([t, n]), _.select("#lasso" + d).style("stroke", "blue").style("stroke-width", 2).style("fill", "#00008854").attr("d", m(c))
                                     })).on("end", (function() {
                                         let e = [];
-                                        p.each(((l, d) => {
+                                        u.each(((r, l) => {
                                             (function(e, t) {
-                                                for (var n = e[0], a = e[1], r = !1, i = 0, o = t.length - 1; i < t.length; o = i++) {
-                                                    var s = t[i][0],
-                                                        l = t[i][1],
-                                                        d = t[o][0],
-                                                        c = t[o][1];
-                                                    l > a != c > a && n < (d - s) * (a - l) / (c - l) + s && (r = !r)
+                                                for (var n = e[0], a = e[1], i = !1, o = 0, s = t.length - 1; o < t.length; s = o++) {
+                                                    var r = t[o][0],
+                                                        l = t[o][1],
+                                                        d = t[s][0],
+                                                        c = t[s][1];
+                                                    l > a != c > a && n < (d - r) * (a - l) / (c - l) + r && (i = !i)
                                                 }
-                                                return r
-                                            })([t(l[a]) + o, n(l[i]) + s], m) && (r.select("#dot-" + c + l.id).style("fill", "red").attr("r", 6), e.push(l))
-                                        })), r.select("#lasso" + c).remove(), d(e)
+                                                return i
+                                            })([t(r[a]) + o, n(r[i]) + s], c) && (_.select("#dot-" + d + r.id).style("fill", "red").attr("r", 6), e.push(r))
+                                        })), _.select("#lasso" + d).remove(), l(e)
                                     }));
-                                r.select(e).call(h)
-                            }(i, h, f, t, n, c.left, c.top, (function() {
+                                _.select(e).call(p)
+                            }(i, p, h, t, n, d.left, d.top, (function() {
                                 x.selectAll(".dot").data(e).attr("r", 3.5).style("fill", (function(e) {
                                     return g(e[a])
                                 }))
                             }), (function(e) {
                                 void 0 !== s && s(e)
-                            }), p);
-                        const y = x.selectAll(".legend").data(g.domain()).enter().append("g").attr("class", "legend").attr("transform", (function(e, t) {
+                            }), u);
+                        const b = x.selectAll(".legend").data(g.domain()).enter().append("g").attr("class", "legend").attr("transform", (function(e, t) {
                             return "translate(0," + 20 * t + ")"
                         }));
-                        y.append("rect").attr("x", m - 18).attr("width", 18).attr("height", 18).style("fill", g), y.append("text").attr("x", m - 24).attr("y", 9).attr("dy", ".35em").style("text-anchor", "end").text((function(e) {
+                        b.append("rect").attr("x", c - 18).attr("width", 18).attr("height", 18).style("fill", g), b.append("text").attr("x", c - 24).attr("y", 9).attr("dy", ".35em").style("text-anchor", "end").text((function(e) {
                             return e
                         }));
-                        const b = x.append("g").append("rect").style("fill", "none").attr("width", 160).attr("height", 40).attr("stroke", "#69b3a2").attr("stroke-width", 4).style("opacity", 0),
+                        const y = x.append("g").append("rect").style("fill", "none").attr("width", 160).attr("height", 40).attr("stroke", "#69b3a2").attr("stroke-width", 4).style("opacity", 0),
                             w = x.append("g").append("text").style("opacity", 0).attr("text-anchor", "left").attr("alignment-baseline", "middle")
-                    }(e, t, n, a, s, this.setValue.bind(this), this.setSelectedValues.bind(this), l, o, d)
+                    }(e, t, n, a, s, this.setValue.bind(this), this.setSelectedValues.bind(this), r, o, l)
                 }
                 setValue(e) {
                     this.model.set({
                         clickedValue: e
                     }), this.model.save_changes()
                 }
                 setSelectedValues(e) {
                     this.model.set({
                         selectedValues: e
                     }), this.model.save_changes()
                 }
             }
-            class L extends a.DOMWidgetModel {
+            class S extends a.DOMWidgetModel {
                 defaults() {
                     return {
                         ...super.defaults(),
-                        _model_name: L.model_name,
-                        _view_name: L.view_name,
-                        _model_module: L.model_module,
-                        _view_module: L.view_module,
-                        _model_module_version: L.model_module_version,
-                        _view_module_version: L.view_module_version,
+                        _model_name: S.model_name,
+                        _view_name: S.view_name,
+                        _model_module: S.model_module,
+                        _view_module: S.view_module,
+                        _model_module_version: S.model_module_version,
+                        _view_module_version: S.view_module_version,
                         data: [],
                         x: String,
                         y: String,
                         hue: String,
                         elementId: String
                     }
                 }
                 static model_name = "BarplotModel";
-                static model_module = y.name;
-                static model_module_version = y.version;
+                static model_module = b.name;
+                static model_module_version = b.version;
                 static view_name = "BarplotView";
-                static view_module = y.name;
-                static view_module_version = y.version
+                static view_module = b.name;
+                static view_module_version = b.version
             }
-            class j extends a.DOMWidgetView {
+            class V extends a.DOMWidgetView {
                 timeout;
                 render() {
-                    k(this), this.model.on("change:data", (() => k(this)), this), window.addEventListener("resize", (() => k(this).bind(this)))
+                    k(this), this.model.on("change:data", (() => k(this)), this), this.model.on("change:x", (() => k(this)), this), this.model.on("change:y", (() => k(this)), this), this.model.on("change:hue", (() => k(this)), this), window.addEventListener("resize", (() => k(this)))
                 }
                 plot() {
                     const e = this.model.get("data"),
                         t = this.model.get("x"),
                         n = this.model.get("y"),
                         a = this.model.get("hue"),
-                        o = this.model.get("elementId");
-                    let s = b,
-                        l = this.el;
-                    o && (l = document.getElementById(o), s = l.clientHeight),
-                        function(e, t, n, a, o, s, l, d) {
-                            const c = s - d.left - d.right,
-                                m = l - d.top - d.bottom;
-                            r.select(o).selectAll("*").remove();
-                            const u = r.select(o).append("svg").attr("width", s).attr("height", l).append("g").attr("transform", "translate(" + d.left + "," + d.top + ")");
+                        i = this.model.get("elementId");
+                    let o = y,
+                        s = this.el;
+                    i && (s = document.getElementById(i), o = s.clientHeight),
+                        function(e, t, n, a, i, o, s, r) {
+                            const l = o - r.left - r.right,
+                                d = s - r.top - r.bottom;
+                            _.select(i).selectAll("*").remove();
+                            const c = _.select(i).append("svg").attr("width", o).attr("height", s).append("g").attr("transform", "translate(" + r.left + "," + r.top + ")");
                             a || (a = t);
-                            const p = e.reduce(((e, t) => (e && -1 === e.indexOf(t[a]) && e.push(t[a]), e)), []),
-                                h = {},
-                                f = r.scaleOrdinal(r.schemeCategory10);
+                            const m = e.reduce(((e, t) => (e && -1 === e.indexOf(t[a]) && e.push(t[a]), e)), []),
+                                u = {},
+                                p = _.scaleOrdinal(_.schemeCategory10);
                             a == t ? function() {
                                 let a = e.reduce(((e, a) => {
-                                    const r = a[t],
-                                        i = a[n];
-                                    if (r in e) e[r] += i, h[r].qt += 1, h[r][n].push(i);
+                                    const i = a[t],
+                                        o = a[n];
+                                    if (i in e) e[i] += o, u[i].qt += 1, u[i][n].push(o);
                                     else {
                                         const t = {
                                             qt: 1
                                         };
-                                        t[n] = [], t[n].push(i), h[r] = t, e[r] = i
+                                        t[n] = [], t[n].push(o), u[i] = t, e[i] = o
                                     }
                                     return e
                                 }), {});
                                 a = Object.keys(a).map((e => {
-                                    const r = {};
-                                    return r[t] = e, r[n] = a[e], 0 != h[e].qt && (r[n] = r[n] / h[e].qt), r
-                                })), Object.keys(h).forEach((e => {
-                                    const t = h[e][n],
-                                        [a, r] = i(t);
-                                    h[e].min = a, h[e].max = r
+                                    const i = {};
+                                    return i[t] = e, i[n] = a[e], 0 != u[e].qt && (i[n] = i[n] / u[e].qt), i
+                                })), Object.keys(u).forEach((e => {
+                                    const t = u[e][n],
+                                        [a, i] = x(t);
+                                    u[e].min = a, u[e].max = i
                                 }));
-                                const o = a.map((e => e[t])),
-                                    s = [],
-                                    l = Object.keys(h).map((e => h[e]));
-                                s.push(r.min(l, (e => e.min))), s.push(r.max(l, (e => e.max))), s[0] > 0 && s[1] > 0 ? s[0] = 0 : s[0] < 0 && s[1] < 0 && (s[1] = 0);
-                                const d = r.scaleLinear().domain(s).range([m, 0]);
-                                u.append("g").call(r.axisLeft(d));
-                                const g = r.scaleBand().domain(o).range([0, c]).padding([.2]);
-                                u.append("g").selectAll("g").data(a).enter().append("rect").attr("x", (function(e) {
-                                    return g(e[t])
+                                const i = a.map((e => e[t])),
+                                    o = [],
+                                    s = Object.keys(u).map((e => u[e]));
+                                o.push(_.min(s, (e => e.min))), o.push(_.max(s, (e => e.max))), o[0] > 0 && o[1] > 0 ? o[0] = 0 : o[0] < 0 && o[1] < 0 && (o[1] = 0);
+                                const r = _.scaleLinear().domain(o).range([d, 0]);
+                                c.append("g").call(_.axisLeft(r));
+                                const h = _.scaleBand().domain(i).range([0, l]).padding([.2]);
+                                c.append("g").selectAll("g").data(a).enter().append("rect").attr("x", (function(e) {
+                                    return h(e[t])
                                 })).attr("y", (function(e) {
-                                    return d(e[n]) < d(0) ? d(e[n]) : d(0)
-                                })).attr("width", g.bandwidth()).attr("height", (function(e) {
-                                    return Math.abs(d(0) - d(e[n]))
-                                })).data(p).attr("fill", (function(e) {
-                                    return f(e)
+                                    return r(e[n]) < r(0) ? r(e[n]) : r(0)
+                                })).attr("width", h.bandwidth()).attr("height", (function(e) {
+                                    return Math.abs(r(0) - r(e[n]))
+                                })).data(m).attr("fill", (function(e) {
+                                    return p(e)
                                 }));
-                                const v = Object.keys(h).map((e => {
+                                const g = Object.keys(u).map((e => {
                                     const n = {};
-                                    return n[t] = e, n.min = h[e].min, n.max = h[e].max, n
+                                    return n[t] = e, n.min = u[e].min, n.max = u[e].max, n
                                 }));
-                                u.append("g").selectAll("g").data(v).enter().append("rect").attr("x", (function(e) {
-                                    return g(e[t]) + g.bandwidth() / 2 - 1
+                                c.append("g").selectAll("g").data(g).enter().append("rect").attr("x", (function(e) {
+                                    return h(e[t]) + h.bandwidth() / 2 - 1
                                 })).attr("y", (function(e) {
-                                    return d(e.max)
+                                    return r(e.max)
                                 })).attr("width", 2).attr("height", (function(e) {
-                                    return d(e.min) - d(e.max)
-                                })), u.append("g").style("font", "18px times").attr("transform", "translate(0," + d(0) + ")").call(r.axisBottom(g).tickSize(0))
+                                    return r(e.min) - r(e.max)
+                                })), c.append("g").style("font", "18px times").attr("transform", "translate(0," + r(0) + ")").call(_.axisBottom(h).tickSize(0))
                             }() : function() {
-                                let o = e.reduce(((e, r) => {
-                                    const i = r[t],
-                                        o = r[n],
-                                        s = r[a];
-                                    if (i in e) {
-                                        h[i].qt[n + "-" + s] += 1, h[i][s][n].push(o);
-                                        for (const t of p) s == t && (e[i][n + "-" + t] += o)
+                                let i = e.reduce(((e, i) => {
+                                    const o = i[t],
+                                        s = i[n],
+                                        r = i[a];
+                                    if (o in e) {
+                                        u[o].qt[n + "-" + r] += 1, u[o][r][n].push(s);
+                                        for (const t of m) r == t && (e[o][n + "-" + t] += s)
                                     } else {
                                         const t = {};
-                                        p.forEach((e => {
+                                        m.forEach((e => {
                                             t[e] = {}, t[e][n] = []
                                         }));
                                         const a = {};
-                                        for (const e of p) a[n + "-" + e] = 0;
-                                        a[n + "-" + s] = 1, t.qt = a, t[s][n].push(o), h[i] = t;
-                                        const r = {};
-                                        for (const e of p) r[n + "-" + e] = s == e ? o : 0;
-                                        e[i] = r
+                                        for (const e of m) a[n + "-" + e] = 0;
+                                        a[n + "-" + r] = 1, t.qt = a, t[r][n].push(s), u[o] = t;
+                                        const i = {};
+                                        for (const e of m) i[n + "-" + e] = r == e ? s : 0;
+                                        e[o] = i
                                     }
                                     return e
                                 }), {});
-                                o = Object.keys(o).map((e => {
+                                i = Object.keys(i).map((e => {
                                     let n = {};
                                     n[t] = e;
-                                    for (const t of Object.keys(o[e])) 0 != h[e].qt[t] && (o[e][t] = o[e][t] / h[e].qt[t]);
+                                    for (const t of Object.keys(i[e])) 0 != u[e].qt[t] && (i[e][t] = i[e][t] / u[e].qt[t]);
                                     return n = {
                                         ...n,
-                                        ...o[e]
+                                        ...i[e]
                                     }, n
-                                })), Object.keys(h).forEach((e => {
-                                    p.forEach((t => {
-                                        const a = h[e][t][n],
-                                            [r, o] = i(a);
-                                        h[e][t].min = r, h[e][t].max = o
+                                })), Object.keys(u).forEach((e => {
+                                    m.forEach((t => {
+                                        const a = u[e][t][n],
+                                            [i, o] = x(a);
+                                        u[e][t].min = i, u[e][t].max = o
                                     }))
                                 }));
-                                const s = p.map((e => n + "-" + e)),
-                                    l = o.map((e => e[t])),
-                                    d = [];
-                                Object.keys(h).map((e => {
-                                    p.forEach((t => d.push(h[e][t])))
+                                const o = m.map((e => n + "-" + e)),
+                                    s = i.map((e => e[t])),
+                                    r = [];
+                                Object.keys(u).map((e => {
+                                    m.forEach((t => r.push(u[e][t])))
                                 }));
-                                const g = [];
-                                g.push(r.min(d, (e => e.min))), g.push(r.max(d, (e => e.max))), g[0] > 0 && g[1] > 0 ? g[0] = 0 : g[0] < 0 && g[1] < 0 && (g[1] = 0);
-                                const v = r.scaleLinear().domain(g).range([m, 0]);
-                                u.append("g").call(r.axisLeft(v));
-                                const _ = r.scaleBand().domain(l).range([0, c]).padding([.2]),
-                                    x = r.scaleBand().domain(s).range([0, _.bandwidth()]).padding([.05]);
-                                u.append("g").selectAll("g").data(o).enter().append("g").attr("transform", (function(e) {
-                                    return "translate(" + _(e[t]) + ",0)"
+                                const h = [];
+                                h.push(_.min(r, (e => e.min))), h.push(_.max(r, (e => e.max))), h[0] > 0 && h[1] > 0 ? h[0] = 0 : h[0] < 0 && h[1] < 0 && (h[1] = 0);
+                                const g = _.scaleLinear().domain(h).range([d, 0]);
+                                c.append("g").call(_.axisLeft(g));
+                                const v = _.scaleBand().domain(s).range([0, l]).padding([.2]),
+                                    f = _.scaleBand().domain(o).range([0, v.bandwidth()]).padding([.05]);
+                                c.append("g").selectAll("g").data(i).enter().append("g").attr("transform", (function(e) {
+                                    return "translate(" + v(e[t]) + ",0)"
                                 })).selectAll("rect").data((function(e) {
-                                    return s.map((function(t) {
+                                    return o.map((function(t) {
                                         return {
                                             key: t,
                                             value: e[t]
                                         }
                                     }))
                                 })).enter().append("rect").attr("x", (function(e) {
-                                    return x(e.key)
+                                    return f(e.key)
                                 })).attr("y", (function(e) {
-                                    return v(e.value) < v(0) ? v(e.value) : v(0)
-                                })).attr("width", x.bandwidth()).attr("height", (function(e) {
-                                    return Math.abs(v(0) - v(e.value))
-                                })).data(p).attr("fill", (function(e) {
-                                    return f(e)
+                                    return g(e.value) < g(0) ? g(e.value) : g(0)
+                                })).attr("width", f.bandwidth()).attr("height", (function(e) {
+                                    return Math.abs(g(0) - g(e.value))
+                                })).data(m).attr("fill", (function(e) {
+                                    return p(e)
                                 }));
-                                const y = Object.keys(h).map((e => {
+                                const b = Object.keys(u).map((e => {
                                     let n = {};
                                     return n[t] = e, n = {
                                         ...n,
-                                        ...h[e]
+                                        ...u[e]
                                     }, n
                                 }));
-                                u.append("g").selectAll("g").data(y).enter().append("g").attr("transform", (function(e) {
-                                    return "translate(" + _(e[t]) + ",0)"
+                                c.append("g").selectAll("g").data(b).enter().append("g").attr("transform", (function(e) {
+                                    return "translate(" + v(e[t]) + ",0)"
                                 })).selectAll("rect").data((function(e) {
-                                    return p.map((function(t) {
+                                    return m.map((function(t) {
                                         return {
                                             key: n + "-" + t,
                                             value: e[t]
                                         }
                                     }))
                                 })).enter().append("rect").attr("x", (function(e) {
-                                    return x(e.key) + x.bandwidth() / 2 - 1
+                                    return f(e.key) + f.bandwidth() / 2 - 1
                                 })).attr("y", (function(e) {
-                                    return e.value.max ? v(e.value.max) : 0
+                                    return e.value.max ? g(e.value.max) : 0
                                 })).attr("width", 2).attr("height", (function(e) {
-                                    return e.value.min && e.value.max ? v(e.value.min) - v(e.value.max) : 0
+                                    return e.value.min && e.value.max ? g(e.value.min) - g(e.value.max) : 0
                                 }));
-                                const b = u.selectAll(".legend").data(f.domain()).enter().append("g").attr("class", "legend").attr("transform", (function(e, t) {
+                                const y = c.selectAll(".legend").data(p.domain()).enter().append("g").attr("class", "legend").attr("transform", (function(e, t) {
                                     return "translate(0," + 20 * t + ")"
                                 }));
-                                b.append("rect").attr("x", c - 18).attr("width", 18).attr("height", 18).style("fill", f), b.append("text").attr("x", c - 24).attr("y", 9).attr("dy", ".35em").style("text-anchor", "end").text((function(e) {
+                                y.append("rect").attr("x", l - 18).attr("width", 18).attr("height", 18).style("fill", p), y.append("text").attr("x", l - 24).attr("y", 9).attr("dy", ".35em").style("text-anchor", "end").text((function(e) {
                                     return e
-                                })), u.append("g").style("font", "18px times").attr("transform", "translate(0," + v(0) + ")").call(r.axisBottom(_).tickSize(0))
+                                })), c.append("g").style("font", "18px times").attr("transform", "translate(0," + g(0) + ")").call(_.axisBottom(v).tickSize(0))
                             }()
-                        }(e, t, n, a, l, l.clientWidth, s, w)
+                        }(e, t, n, a, s, s.clientWidth, o, w)
                 }
             }
             class D extends a.DOMWidgetModel {
                 defaults() {
                     return {
                         ...super.defaults(),
                         _model_name: D.model_name,
@@ -481,127 +487,212 @@
                         x: String,
                         start: Number,
                         end: Number,
                         elementId: String
                     }
                 }
                 static model_name = "HistogramplotModel";
-                static model_module = y.name;
-                static model_module_version = y.version;
+                static model_module = b.name;
+                static model_module_version = b.version;
                 static view_name = "HistogramplotView";
-                static view_module = y.name;
-                static view_module_version = y.version
+                static view_module = b.name;
+                static view_module_version = b.version
             }
-            class V extends a.DOMWidgetView {
+            class j extends a.DOMWidgetView {
                 timeout;
                 render() {
-                    k(this), this.model.on("change:data", (() => k(this)), this), window.addEventListener("resize", (() => k(this).bind(this)))
+                    k(this), this.model.on("change:data", (() => k(this)), this), this.model.on("change:x", (() => k(this)), this), this.model.on("change:start", (() => k(this)), this), this.model.on("change:end", (() => k(this)), this), window.addEventListener("resize", (() => k(this)))
                 }
                 plot() {
                     const e = this.model.get("data"),
                         t = this.model.get("x"),
                         n = this.model.get("start"),
                         a = this.model.get("end"),
                         i = this.model.get("elementId");
-                    let o = b,
+                    let o = y,
                         s = this.el;
                     i && (s = document.getElementById(i), o = s.clientHeight),
-                        function(e, t, n, a, i, o, s, l) {
-                            const d = o - l.left - l.right,
-                                c = s - l.top - l.bottom;
-                            r.select(i).selectAll("*").remove();
-                            let m = n;
-                            n || (m = r.min(e, (e => e[t])));
-                            let u = a;
-                            a || (u = r.max(e, (e => e[t])));
-                            const p = r.scaleLinear().range([0, d]),
-                                h = r.scaleLinear().range([c, 0]),
-                                f = r.axisBottom(p),
-                                g = r.axisLeft(h),
-                                v = r.bin().thresholds(40).value((e => Math.round(10 * e[t]) / 10))(e),
-                                _ = r.select(i).append("svg").attr("width", o).attr("height", s).append("g").attr("transform", "translate(" + l.left + "," + l.top + ")");
-                            p.domain([m, u]), h.domain([0, r.max(v, (e => e.length))]), _.append("g").attr("transform", "translate(0," + c + ")").call(f).append("text").attr("x", d).attr("y", -6).style("text-anchor", "end"), _.append("g").call(g).append("text").attr("transform", "rotate(-90)").attr("y", 6).attr("dy", ".71em").style("text-anchor", "end"), _.append("g").attr("fill", "steelblue").selectAll().data(v).join("rect").attr("x", (e => p(e.x0) + 1)).attr("width", (e => p(e.x1) - p(e.x0) - 1)).attr("y", (e => h(e.length))).attr("height", (e => h(0) - h(e.length)))
+                        function(e, t, n, a, i, o, s, r) {
+                            const l = o - r.left - r.right,
+                                d = s - r.top - r.bottom;
+                            _.select(i).selectAll("*").remove();
+                            let c = n;
+                            n || (c = _.min(e, (e => e[t])));
+                            let m = a;
+                            a || (m = _.max(e, (e => e[t])));
+                            const u = _.scaleLinear().range([0, l]),
+                                p = _.scaleLinear().range([d, 0]),
+                                h = _.axisBottom(u),
+                                g = _.axisLeft(p),
+                                v = _.bin().thresholds(40).value((e => Math.round(10 * e[t]) / 10))(e),
+                                f = _.select(i).append("svg").attr("width", o).attr("height", s).append("g").attr("transform", "translate(" + r.left + "," + r.top + ")");
+                            u.domain([c, m]), p.domain([0, _.max(v, (e => e.length))]), f.append("g").attr("transform", "translate(0," + d + ")").call(h).append("text").attr("x", l).attr("y", -6).style("text-anchor", "end"), f.append("g").call(g).append("text").attr("transform", "rotate(-90)").attr("y", 6).attr("dy", ".71em").style("text-anchor", "end"), f.append("g").attr("fill", "steelblue").selectAll().data(v).join("rect").attr("x", (e => u(e.x0) + 1)).attr("width", (e => u(e.x1) - u(e.x0) - 1)).attr("y", (e => p(e.length))).attr("height", (e => p(0) - p(e.length)))
                         }(e, t, n, a, s, s.clientWidth, o, w)
                 }
             }
-            class O extends a.DOMWidgetModel {
+            class C extends a.DOMWidgetModel {
                 defaults() {
                     return {
                         ...super.defaults(),
-                        _model_name: O.model_name,
-                        _view_name: O.view_name,
-                        _model_module: O.model_module,
-                        _view_module: O.view_module,
-                        _model_module_version: O.model_module_version,
-                        _view_module_version: O.view_module_version,
+                        _model_name: C.model_name,
+                        _view_name: C.view_name,
+                        _model_module: C.model_module,
+                        _view_module: C.view_module,
+                        _model_module_version: C.model_module_version,
+                        _view_module_version: C.view_module_version,
                         matrix: [],
                         grid_areas: [],
                         grid_template_areas: String,
                         style: String
                     }
                 }
                 static model_name = "EmbeddingModel";
-                static model_module = y.name;
-                static model_module_version = y.version;
+                static model_module = b.name;
+                static model_module_version = b.version;
                 static view_name = "EmbeddingView";
-                static view_module = y.name;
-                static view_module_version = y.version
+                static view_module = b.name;
+                static view_module_version = b.version
             }
-            class I extends a.DOMWidgetView {
+            class O extends a.DOMWidgetView {
                 render() {
                     this.value_changed()
                 }
                 value_changed() {
                     const e = this.model.get("matrix"),
                         t = this.model.get("grid_areas"),
                         n = this.model.get("grid_template_areas");
                     let a = this.model.get("style");
                     a || (a = "basic");
-                    const r = document.createElement("div");
-                    r.classList.add(a), r.style.display = "grid", r.style.gridTemplateAreas = n, r.style.gridTemplateRows = "repeat(" + e.length + ", 20vh)", r.style.gridTemplateColumns = "repeat(" + e[0].length + ", 1fr)", r.style.width = "100%", t.forEach((e => {
+                    const i = document.createElement("div");
+                    i.classList.add(a), i.style.display = "grid", i.style.gridTemplateAreas = n, i.style.gridTemplateRows = "repeat(" + e.length + ", 20vh)", i.style.gridTemplateColumns = "repeat(" + e[0].length + ", 1fr)", i.style.width = "100%", t.forEach((e => {
                         const t = document.createElement("div");
-                        t.setAttribute("id", e), t.style.gridArea = e, t.classList.add("dashboard-div"), r.appendChild(t)
-                    })), this.el.appendChild(r)
+                        t.setAttribute("id", e), t.style.gridArea = e, t.classList.add("dashboard-div"), i.appendChild(t)
+                    })), this.el.appendChild(i)
+                }
+            }
+            class I extends a.DOMWidgetModel {
+                defaults() {
+                    return {
+                        ...super.defaults(),
+                        _model_name: I.model_name,
+                        _view_name: I.view_name,
+                        _model_module: I.model_module,
+                        _view_module: I.view_module,
+                        _model_module_version: I.model_module_version,
+                        _view_module_version: I.view_module_version,
+                        data: [],
+                        variable: String,
+                        step: Number,
+                        description: String,
+                        minValue: Number,
+                        maxValue: Number,
+                        elementId: String
+                    }
+                }
+                static model_name = "RangeSliderModel";
+                static model_module = b.name;
+                static model_module_version = b.version;
+                static view_name = "RangeSliderView";
+                static view_module = b.name;
+                static view_module_version = b.version
+            }
+            class B extends a.DOMWidgetView {
+                render() {
+                    k(this), this.model.on("change:data", (() => k(this)), this), this.model.on("change:variable", (() => k(this)), this), this.model.on("change:step", (() => k(this)), this), this.model.on("change:description", (() => k(this)), this), window.addEventListener("resize", (() => k(this)))
+                }
+                plot() {
+                    const e = this.model.get("data"),
+                        t = this.model.get("variable"),
+                        n = this.model.get("step"),
+                        a = this.model.get("description"),
+                        i = this.model.get("elementId"),
+                        o = this.model.get("minValue"),
+                        s = this.model.get("maxValue");
+                    let r = this.el;
+                    i && (r = document.getElementById(i));
+                    const l = w;
+                    ! function(e, t, n, a, i, o, s, r, l) {
+                        const d = document.createElement("div");
+                        d.classList.add("range_outside_container"), d.style.margin = l.top + "px " + l.right + "px " + l.bottom + "px " + l.left + "px";
+                        const c = document.createElement("span");
+                        c.classList.add("range_description"), c.textContent = a, d.appendChild(c);
+                        const m = document.createElement("div");
+                        m.classList.add("range_inside_container"), d.appendChild(m);
+                        const u = document.createElement("span");
+                        u.classList.add("range_value"), d.appendChild(u);
+                        const p = document.createElement("div");
+                        p.classList.add("sliders_control"), m.appendChild(p);
+                        const h = document.createElement("input");
+                        h.classList.add("top_slider"), h.setAttribute("step", n), h.setAttribute("type", "range"), p.appendChild(h);
+                        const g = document.createElement("input");
+
+                        function v(e, t) {
+                            u.textContent = e + " - " + t, s(e, t)
+                        }
+                        g.setAttribute("step", n), g.setAttribute("type", "range"), p.appendChild(g);
+                        const f = _.min(e, (e => e[t])),
+                            x = _.max(e, (e => e[t]));
+                        h.setAttribute("min", f), h.setAttribute("max", x), g.setAttribute("min", f), g.setAttribute("max", x), i && o ? (h.value = i, g.value = o) : (h.value = f, g.value = x), v(parseFloat(h.value), parseFloat(g.value)), h.addEventListener("input", (() => {
+                            const e = parseFloat(h.value),
+                                t = parseFloat(g.value);
+                            e > t && (h.value = g.value), v(e, t)
+                        })), g.addEventListener("input", (() => {
+                            const e = parseFloat(h.value),
+                                t = parseFloat(g.value);
+                            t < e && (g.value = h.value), v(e, t)
+                        })), h.addEventListener("click", (() => {
+                            h.classList.add("top_slider"), g.classList.remove("top_slider")
+                        })), g.addEventListener("click", (() => {
+                            g.classList.add("top_slider"), h.classList.remove("top_slider")
+                        })), r.innerHTML = "", r.appendChild(d)
+                    }(e, t, n, a, o, s, this.setValues.bind(this), r, l)
+                }
+                setValues(e, t) {
+                    this.model.set({
+                        minValue: e
+                    }), this.model.set({
+                        maxValue: t
+                    }), this.model.save_changes()
                 }
             }
-            var C = n(330)
+            var W = n(330)
         },
         930: (e, t, n) => {
             n.d(t, {
-                A: () => s
+                A: () => r
             });
             var a = n(601),
-                r = n.n(a),
-                i = n(314),
-                o = n.n(i)()(r());
-            o.push([e.id, "/***** BASIC *****/\n.basic .dashboard-div {\n  border: 1px solid black;\n  text-align: center;\n}\n\n/***** DARK *****/\n.dark .dashboard-div {\n  margin: 2px;\n  border-radius: 10px;\n  background-color: #262626;\n  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.5);\n}\n\n/***** GLASSMORPHISM *****/\n.glassmorphism .dashboard-div {\n  margin: 5px;\n  border-radius: 10px;\n  background: rgb(255, 254, 254);\n  border: 1px solid rgb(255, 255, 255);\n  backdrop-filter: blur(10px);\n  box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);\n}\n\n/***** NEUMORPHISM *****/\n.neumorphism .dashboard-div {\n  margin: 10px;\n  border-radius: 15px;\n  background-color: #e0e0e0;\n  box-shadow: 5px 5px 10px #bebebe, -5px -5px 10px #ffffff;\n}\n\n/***** MINIMALISM *****/\n.minimalism .dashboard-div {\n  margin-bottom: 5px;\n}\n", ""]);
-            const s = o
+                i = n.n(a),
+                o = n(314),
+                s = n.n(o)()(i());
+            s.push([e.id, '/***** EMBEDDING *****/\n.basic .dashboard-div {\n  border: 1px solid black;\n  text-align: center;\n}\n\n.dark .dashboard-div {\n  margin: 2px;\n  border-radius: 10px;\n  background-color: #262626;\n  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.5);\n}\n\n.glassmorphism .dashboard-div {\n  margin: 5px;\n  border-radius: 10px;\n  background: rgb(255, 254, 254);\n  border: 1px solid rgb(255, 255, 255);\n  backdrop-filter: blur(10px);\n  box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);\n}\n\n.neumorphism .dashboard-div {\n  margin: 10px;\n  border-radius: 15px;\n  background-color: #e0e0e0;\n  box-shadow: 5px 5px 10px #bebebe, -5px -5px 10px #ffffff;\n}\n\n.minimalism .dashboard-div {\n  margin-bottom: 5px;\n}\n\n/***** RANGE SLIDER *****/\n.range_outside_container {\n  display: flex;\n  max-width: 500px;\n}\n\n.range_inside_container {\n  display: flex;\n  flex-direction: column;\n  width: 80%;\n}\n\n.range_description {\n  padding-right: 20px;\n}\n\n.range_value {\n  padding-left: 20px;\n  width: 80px;\n}\n\n.sliders_control {\n  position: relative;\n  min-height: 50px;\n}\n\ninput[type="range"]::-webkit-slider-thumb {\n  -webkit-appearance: none;\n  pointer-events: all;\n  width: 24px;\n  height: 24px;\n  background-color: #fff;\n  border-radius: 50%;\n  box-shadow: 0 0 0 1px #c6c6c6;\n  cursor: pointer;\n}\n\ninput[type="range"]::-moz-range-thumb {\n  -webkit-appearance: none;\n  pointer-events: all;\n  width: 24px;\n  height: 24px;\n  background-color: #fff;\n  border-radius: 50%;\n  box-shadow: 0 0 0 1px #c6c6c6;\n  cursor: pointer;\n}\n\ninput[type="range"]::-webkit-slider-thumb:hover {\n  background: #f7f7f7;\n}\n\ninput[type="range"]::-webkit-slider-thumb:active {\n  box-shadow: inset 0 0 3px #387bbe, 0 0 9px #387bbe;\n  -webkit-box-shadow: inset 0 0 3px #387bbe, 0 0 9px #387bbe;\n}\n\ninput[type="range"] {\n  -webkit-appearance: none;\n  appearance: none;\n  height: 10px;\n  width: 100%;\n  position: absolute;\n  background-color: #f79847;\n  pointer-events: none;\n}\n\n.top_slider {\n  height: 0 !important;\n  z-index: 1;\n  top: 5px;\n}\n', ""]);
+            const r = s
         },
         314: e => {
             e.exports = function(e) {
                 var t = [];
                 return t.toString = function() {
                     return this.map((function(t) {
                         var n = "",
                             a = void 0 !== t[5];
                         return t[4] && (n += "@supports (".concat(t[4], ") {")), t[2] && (n += "@media ".concat(t[2], " {")), a && (n += "@layer".concat(t[5].length > 0 ? " ".concat(t[5]) : "", " {")), n += e(t), a && (n += "}"), t[2] && (n += "}"), t[4] && (n += "}"), n
                     })).join("")
-                }, t.i = function(e, n, a, r, i) {
+                }, t.i = function(e, n, a, i, o) {
                     "string" == typeof e && (e = [
                         [null, e, void 0]
                     ]);
-                    var o = {};
+                    var s = {};
                     if (a)
-                        for (var s = 0; s < this.length; s++) {
-                            var l = this[s][0];
-                            null != l && (o[l] = !0)
+                        for (var r = 0; r < this.length; r++) {
+                            var l = this[r][0];
+                            null != l && (s[l] = !0)
                         }
                     for (var d = 0; d < e.length; d++) {
                         var c = [].concat(e[d]);
-                        a && o[c[0]] || (void 0 !== i && (void 0 === c[5] || (c[1] = "@layer".concat(c[5].length > 0 ? " ".concat(c[5]) : "", " {").concat(c[1], "}")), c[5] = i), n && (c[2] ? (c[1] = "@media ".concat(c[2], " {").concat(c[1], "}"), c[2] = n) : c[2] = n), r && (c[4] ? (c[1] = "@supports (".concat(c[4], ") {").concat(c[1], "}"), c[4] = r) : c[4] = "".concat(r)), t.push(c))
+                        a && s[c[0]] || (void 0 !== o && (void 0 === c[5] || (c[1] = "@layer".concat(c[5].length > 0 ? " ".concat(c[5]) : "", " {").concat(c[1], "}")), c[5] = o), n && (c[2] ? (c[1] = "@media ".concat(c[2], " {").concat(c[1], "}"), c[2] = n) : c[2] = n), i && (c[4] ? (c[1] = "@supports (".concat(c[4], ") {").concat(c[1], "}"), c[4] = i) : c[4] = "".concat(i)), t.push(c))
                     }
                 }, t
             }
         },
         601: e => {
             e.exports = function(e) {
                 return e[1]
@@ -615,65 +706,65 @@
                     if (t[a].identifier === e) {
                         n = a;
                         break
                     } return n
             }
 
             function a(e, a) {
-                for (var i = {}, o = [], s = 0; s < e.length; s++) {
-                    var l = e[s],
+                for (var o = {}, s = [], r = 0; r < e.length; r++) {
+                    var l = e[r],
                         d = a.base ? l[0] + a.base : l[0],
-                        c = i[d] || 0,
+                        c = o[d] || 0,
                         m = "".concat(d, " ").concat(c);
-                    i[d] = c + 1;
+                    o[d] = c + 1;
                     var u = n(m),
                         p = {
                             css: l[1],
                             media: l[2],
                             sourceMap: l[3],
                             supports: l[4],
                             layer: l[5]
                         };
                     if (-1 !== u) t[u].references++, t[u].updater(p);
                     else {
-                        var h = r(p, a);
-                        a.byIndex = s, t.splice(s, 0, {
+                        var h = i(p, a);
+                        a.byIndex = r, t.splice(r, 0, {
                             identifier: m,
                             updater: h,
                             references: 1
                         })
                     }
-                    o.push(m)
+                    s.push(m)
                 }
-                return o
+                return s
             }
 
-            function r(e, t) {
+            function i(e, t) {
                 var n = t.domAPI(t);
                 return n.update(e),
                     function(t) {
                         if (t) {
                             if (t.css === e.css && t.media === e.media && t.sourceMap === e.sourceMap && t.supports === e.supports && t.layer === e.layer) return;
                             n.update(e = t)
                         } else n.remove()
                     }
             }
-            e.exports = function(e, r) {
-                var i = a(e = e || [], r = r || {});
+            e.exports = function(e, i) {
+                var o = a(e = e || [], i = i || {});
                 return function(e) {
                     e = e || [];
-                    for (var o = 0; o < i.length; o++) {
-                        var s = n(i[o]);
-                        t[s].references--
+                    for (var s = 0; s < o.length; s++) {
+                        var r = n(o[s]);
+                        t[r].references--
                     }
-                    for (var l = a(e, r), d = 0; d < i.length; d++) {
-                        var c = n(i[d]);
+                    for (var l = a(e, i), d = 0; d < o.length; d++) {
+                        var c = n(o[d]);
                         0 === t[c].references && (t[c].updater(), t.splice(c, 1))
                     }
-                    i = l
+                    o = l
                 }
             }
         },
         659: e => {
             var t = {};
             e.exports = function(e, n) {
                 var a = function(e) {
@@ -712,18 +803,18 @@
                 };
                 var t = e.insertStyleElement(e);
                 return {
                     update: function(n) {
                         ! function(e, t, n) {
                             var a = "";
                             n.supports && (a += "@supports (".concat(n.supports, ") {")), n.media && (a += "@media ".concat(n.media, " {"));
-                            var r = void 0 !== n.layer;
-                            r && (a += "@layer".concat(n.layer.length > 0 ? " ".concat(n.layer) : "", " {")), a += n.css, r && (a += "}"), n.media && (a += "}"), n.supports && (a += "}");
-                            var i = n.sourceMap;
-                            i && "undefined" != typeof btoa && (a += "\n/*# sourceMappingURL=data:application/json;base64,".concat(btoa(unescape(encodeURIComponent(JSON.stringify(i)))), " */")), t.styleTagTransform(a, e, t.options)
+                            var i = void 0 !== n.layer;
+                            i && (a += "@layer".concat(n.layer.length > 0 ? " ".concat(n.layer) : "", " {")), a += n.css, i && (a += "}"), n.media && (a += "}"), n.supports && (a += "}");
+                            var o = n.sourceMap;
+                            o && "undefined" != typeof btoa && (a += "\n/*# sourceMappingURL=data:application/json;base64,".concat(btoa(unescape(encodeURIComponent(JSON.stringify(o)))), " */")), t.styleTagTransform(a, e, t.options)
                         }(t, e, n)
                     },
                     remove: function() {
                         ! function(e) {
                             if (null === e.parentNode) return !1;
                             e.parentNode.removeChild(e)
                         }(t)
@@ -737,11 +828,11 @@
                 else {
                     for (; t.firstChild;) t.removeChild(t.firstChild);
                     t.appendChild(document.createTextNode(e))
                 }
             }
         },
         330: e => {
-            e.exports = JSON.parse('{"name":"d3vis_ipynb","version":"0.1.2","description":"A Custom Jupyter Widget Library with visualizations created with D3.js.","author":"Daniel Adam Miranda","license":"BSD-3-Clause","main":"lib/index.js","repository":{"type":"git","url":"https://github.com/H-IAAC/d3vis_ipynb.git"},"keywords":["jupyter","widgets","ipython","ipywidgets","jupyterlab-extension"],"files":["lib/**/*.js","dist/*.js","css/*.css"],"scripts":{"clean":"rimraf dist/ && rimraf ../d3vis_ipynb/labextension/ && rimraf ../d3vis_ipynb/nbextension","prepublish":"yarn run clean && yarn run build:prod","build":"webpack --mode=development && yarn run build:labextension:dev","build:prod":"webpack --mode=production && yarn run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","watch":"webpack --watch --mode=development","start":"webpack serve --open --config webpack.exports.config.js","start:export":"webpack serve --open --config webpack.exports.config.js --env export","export":"webpack --env export --config webpack.exports.config.js","test":"echo \\"Error: no test specified\\" && exit 1"},"devDependencies":{"@jupyterlab/builder":"^4.0.6","html-webpack-plugin":"^5.6.0","rimraf":"^2.6.1","webpack":"^5","webpack-dev-server":"^5.0.2"},"dependencies":{"@jupyter-widgets/base":"^1.1 || ^2 || ^3 || ^4 || ^6","d3":"^7.9.0"},"jupyterlab":{"extension":"lib/labplugin","outputDir":"../d3vis_ipynb/labextension","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}}}')
+            e.exports = JSON.parse('{"name":"d3vis_ipynb","version":"0.1.3","description":"A Custom Jupyter Widget Library with visualizations created with D3.js.","author":"Daniel Adam Miranda","license":"BSD-3-Clause","main":"lib/index.js","repository":{"type":"git","url":"https://github.com/H-IAAC/d3vis_ipynb.git"},"keywords":["jupyter","widgets","ipython","ipywidgets","jupyterlab-extension"],"files":["lib/**/*.js","dist/*.js","css/*.css"],"scripts":{"clean":"rimraf dist/ && rimraf ../d3vis_ipynb/labextension/ && rimraf ../d3vis_ipynb/nbextension","prepublish":"yarn run clean && yarn run build:prod","build":"webpack --mode=development && yarn run build:labextension:dev","build:prod":"webpack --mode=production && yarn run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","watch":"webpack --watch --mode=development","start":"webpack serve --open --config webpack.exports.config.js","start:export":"webpack serve --open --config webpack.exports.config.js --env export","export":"webpack --env export --config webpack.exports.config.js","test":"echo \\"Error: no test specified\\" && exit 1"},"devDependencies":{"@jupyterlab/builder":"^4.0.6","html-webpack-plugin":"^5.6.0","rimraf":"^2.6.1","webpack":"^5","webpack-dev-server":"^5.0.2"},"dependencies":{"@jupyter-widgets/base":"^1.1 || ^2 || ^3 || ^4 || ^6","d3":"^7.9.0"},"jupyterlab":{"extension":"lib/labplugin","outputDir":"../d3vis_ipynb/labextension","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}}}')
         }
     }
 ]);
```

### Comparing `d3vis_ipynb-0.1.2/d3vis_ipynb/labextension/static/693.c8409ce8329f6703470f.js` & `d3vis_ipynb-0.1.3/d3vis_ipynb/labextension/static/693.c8409ce8329f6703470f.js`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.1.2/d3vis_ipynb/labextension/static/remoteEntry.bf58726a1c33e2ff91a1.js` & `d3vis_ipynb-0.1.3/d3vis_ipynb/labextension/static/remoteEntry.8f26db161f1984f5ad68.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -1,15 +1,15 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, o, i, a, d, u, f, s, l, p, c, h, v, b, g, m, y, w = {
+    var e, r, t, n, o, i, a, d, u, s, l, f, c, p, h, v, b, g, m, y, w = {
             772: (e, r, t) => {
                 var n = {
-                        "./index": () => t.e(380).then((() => () => t(380))),
-                        "./extension": () => Promise.all([t.e(56), t.e(493)]).then((() => () => t(493)))
+                        "./index": () => t.e(363).then((() => () => t(363))),
+                        "./extension": () => Promise.all([t.e(363), t.e(493)]).then((() => () => t(493)))
                     },
                     o = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
                     })), t.R = void 0, r),
                     i = (e, r) => {
                         if (t.S) {
                             var n = "default",
@@ -42,53 +42,51 @@
         }), r
     }, E.d = (e, r) => {
         for (var t in r) E.o(r, t) && !E.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, E.f = {}, E.e = e => Promise.all(Object.keys(E.f).reduce(((r, t) => (E.f[t](e, r), r)), [])), E.u = e => e + "." + {
-        56: "2d1dea0ba8f2782da6dd",
-        380: "5f71b19ff5261cd2e5de",
-        493: "6062c0a7b585f6ae1d22",
+        363: "e98e5e3babbb9b69956a",
+        493: "053b071a46f0bcccaab9",
         693: "c8409ce8329f6703470f"
     } [e] + ".js?v=" + {
-        56: "2d1dea0ba8f2782da6dd",
-        380: "5f71b19ff5261cd2e5de",
-        493: "6062c0a7b585f6ae1d22",
+        363: "e98e5e3babbb9b69956a",
+        493: "053b071a46f0bcccaab9",
         693: "c8409ce8329f6703470f"
     } [e], E.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
     }(), E.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "d3vis_ipynb:", E.l = (t, n, o, i) => {
         if (e[t]) e[t].push(n);
         else {
             var a, d;
             if (void 0 !== o)
-                for (var u = document.getElementsByTagName("script"), f = 0; f < u.length; f++) {
-                    var s = u[f];
-                    if (s.getAttribute("src") == t || s.getAttribute("data-webpack") == r + o) {
-                        a = s;
+                for (var u = document.getElementsByTagName("script"), s = 0; s < u.length; s++) {
+                    var l = u[s];
+                    if (l.getAttribute("src") == t || l.getAttribute("data-webpack") == r + o) {
+                        a = l;
                         break
                     }
                 }
             a || (d = !0, (a = document.createElement("script")).charset = "utf-8", a.timeout = 120, E.nc && a.setAttribute("nonce", E.nc), a.setAttribute("data-webpack", r + o), a.src = t), e[t] = [n];
-            var l = (r, n) => {
-                    a.onerror = a.onload = null, clearTimeout(p);
+            var f = (r, n) => {
+                    a.onerror = a.onload = null, clearTimeout(c);
                     var o = e[t];
                     if (delete e[t], a.parentNode && a.parentNode.removeChild(a), o && o.forEach((e => e(n))), r) return r(n)
                 },
-                p = setTimeout(l.bind(null, void 0, {
+                c = setTimeout(f.bind(null, void 0, {
                     type: "timeout",
                     target: a
                 }), 12e4);
-            a.onerror = l.bind(null, a.onerror), a.onload = l.bind(null, a.onload), d && document.head.appendChild(a)
+            a.onerror = f.bind(null, a.onerror), a.onload = f.bind(null, a.onload), d && document.head.appendChild(a)
         }
     }, E.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
@@ -110,15 +108,15 @@
                         (!d || !d.loaded && (!n != !d.eager ? n : a > d.from)) && (o[r] = {
                             get: t,
                             from: a,
                             eager: !!n
                         })
                     },
                     u = [];
-                return "default" === t && (d("d3", "7.9.0", (() => E.e(693).then((() => () => E(693))))), d("d3vis_ipynb", "0.1.2", (() => E.e(380).then((() => () => E(380)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                return "default" === t && (d("d3", "7.9.0", (() => E.e(693).then((() => () => E(693))))), d("d3vis_ipynb", "0.1.3", (() => E.e(363).then((() => () => E(363)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         E.g.importScripts && (e = E.g.location + "");
         var r = E.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -168,74 +166,73 @@
     }, i = (e, r) => {
         if (0 in e) {
             r = t(r);
             var n = e[0],
                 o = n < 0;
             o && (n = -n - 1);
             for (var a = 0, d = 1, u = !0;; d++, a++) {
-                var f, s, l = d < e.length ? (typeof e[d])[0] : "";
-                if (a >= r.length || "o" == (s = (typeof(f = r[a]))[0])) return !u || ("u" == l ? d > n && !o : "" == l != o);
-                if ("u" == s) {
-                    if (!u || "u" != l) return !1
+                var s, l, f = d < e.length ? (typeof e[d])[0] : "";
+                if (a >= r.length || "o" == (l = (typeof(s = r[a]))[0])) return !u || ("u" == f ? d > n && !o : "" == f != o);
+                if ("u" == l) {
+                    if (!u || "u" != f) return !1
                 } else if (u)
-                    if (l == s)
+                    if (f == l)
                         if (d <= n) {
-                            if (f != e[d]) return !1
+                            if (s != e[d]) return !1
                         } else {
-                            if (o ? f > e[d] : f < e[d]) return !1;
-                            f != e[d] && (u = !1)
+                            if (o ? s > e[d] : s < e[d]) return !1;
+                            s != e[d] && (u = !1)
                         }
-                else if ("s" != l && "n" != l) {
+                else if ("s" != f && "n" != f) {
                     if (o || d <= n) return !1;
                     u = !1, d--
                 } else {
-                    if (d <= n || s < l != o) return !1;
+                    if (d <= n || l < f != o) return !1;
                     u = !1
-                } else "s" != l && "n" != l && (u = !1, d--)
+                } else "s" != f && "n" != f && (u = !1, d--)
             }
         }
-        var p = [],
-            c = p.pop.bind(p);
+        var c = [],
+            p = c.pop.bind(c);
         for (a = 1; a < e.length; a++) {
             var h = e[a];
-            p.push(1 == h ? c() | c() : 2 == h ? c() & c() : h ? i(h, r) : !c())
+            c.push(1 == h ? p() | p() : 2 == h ? p() & p() : h ? i(h, r) : !p())
         }
-        return !!c()
+        return !!p()
     }, a = (e, r) => {
         var t = E.S[e];
         if (!t || !E.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, d = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
-    }, u = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(n) + ")", f = (e, r, t, n) => {
+    }, u = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(n) + ")", s = (e, r, t, n) => {
         var o = d(e, t);
-        return i(n, o) || l(u(e, t, o, n)), p(e[t][o])
-    }, s = (e, r, t) => {
+        return i(n, o) || f(u(e, t, o, n)), c(e[t][o])
+    }, l = (e, r, t) => {
         var o = e[r];
         return (r = Object.keys(o).reduce(((e, r) => !i(t, r) || e && !n(e, r) ? e : r), 0)) && o[r]
-    }, l = e => {
+    }, f = e => {
         "undefined" != typeof console && console.warn && console.warn(e)
-    }, p = e => (e.loaded = 1, e.get()), h = (c = e => function(r, t, n, o) {
+    }, c = e => (e.loaded = 1, e.get()), h = (p = e => function(r, t, n, o) {
         var i = E.I(r);
         return i && i.then ? i.then(e.bind(e, r, E.S[r], t, n, o)) : e(r, E.S[r], t, n, o)
-    })(((e, r, t, n) => (a(e, t), f(r, 0, t, n)))), v = c(((e, r, t, n, o) => {
-        var i = r && E.o(r, t) && s(r, t, n);
-        return i ? p(i) : o()
+    })(((e, r, t, n) => (a(e, t), s(r, 0, t, n)))), v = p(((e, r, t, n, o) => {
+        var i = r && E.o(r, t) && l(r, t, n);
+        return i ? c(i) : o()
     })), b = {}, g = {
         801: () => h("default", "@jupyter-widgets/base", [, [1, 6],
             [1, 4],
             [1, 3],
             [1, 2],
             [1, 1, 1], 1, 1, 1, 1
         ]),
         840: () => v("default", "d3", [1, 7, 9, 0], (() => E.e(693).then((() => () => E(693)))))
     }, m = {
-        56: [801, 840],
-        380: [801, 840]
+        363: [801, 840]
     }, y = {}, E.f.consumes = (e, r) => {
         E.o(m, e) && m[e].forEach((e => {
             if (E.o(b, e)) return r.push(b[e]);
             if (!y[e]) {
                 var t = r => {
                     b[e] = 0, E.m[e] = t => {
                         delete E.c[e], t.exports = r()
@@ -259,27 +256,27 @@
         var e = {
             71: 0
         };
         E.f.j = (r, t) => {
             var n = E.o(e, r) ? e[r] : void 0;
             if (0 !== n)
                 if (n) t.push(n[2]);
-                else if (56 != r) {
-                var o = new Promise(((t, o) => n = e[r] = [t, o]));
-                t.push(n[2] = o);
-                var i = E.p + E.u(r),
-                    a = new Error;
-                E.l(i, (t => {
-                    if (E.o(e, r) && (0 !== (n = e[r]) && (e[r] = void 0), n)) {
-                        var o = t && ("load" === t.type ? "missing" : t.type),
-                            i = t && t.target && t.target.src;
-                        a.message = "Loading chunk " + r + " failed.\n(" + o + ": " + i + ")", a.name = "ChunkLoadError", a.type = o, a.request = i, n[1](a)
-                    }
-                }), "chunk-" + r, r)
-            } else e[r] = 0
+                else {
+                    var o = new Promise(((t, o) => n = e[r] = [t, o]));
+                    t.push(n[2] = o);
+                    var i = E.p + E.u(r),
+                        a = new Error;
+                    E.l(i, (t => {
+                        if (E.o(e, r) && (0 !== (n = e[r]) && (e[r] = void 0), n)) {
+                            var o = t && ("load" === t.type ? "missing" : t.type),
+                                i = t && t.target && t.target.src;
+                            a.message = "Loading chunk " + r + " failed.\n(" + o + ": " + i + ")", a.name = "ChunkLoadError", a.type = o, a.request = i, n[1](a)
+                        }
+                    }), "chunk-" + r, r)
+                }
         };
         var r = (r, t) => {
                 var n, o, [i, a, d] = t,
                     u = 0;
                 if (i.some((r => 0 !== e[r]))) {
                     for (n in a) E.o(a, n) && (E.m[n] = a[n]);
                     d && d(E)
```

### Comparing `d3vis_ipynb-0.1.2/d3vis_ipynb/labextension/static/third-party-licenses.json` & `d3vis_ipynb-0.1.3/d3vis_ipynb/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.1.2/d3vis_ipynb/nbextension/index.js` & `d3vis_ipynb-0.1.3/d3vis_ipynb/nbextension/index.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -5,15 +5,15 @@
                 n.d(e, {
                     A: () => s
                 });
                 var r = n(601),
                     i = n.n(r),
                     o = n(314),
                     a = n.n(o)()(i());
-                a.push([t.id, "/***** BASIC *****/\n.basic .dashboard-div {\n  border: 1px solid black;\n  text-align: center;\n}\n\n/***** DARK *****/\n.dark .dashboard-div {\n  margin: 2px;\n  border-radius: 10px;\n  background-color: #262626;\n  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.5);\n}\n\n/***** GLASSMORPHISM *****/\n.glassmorphism .dashboard-div {\n  margin: 5px;\n  border-radius: 10px;\n  background: rgb(255, 254, 254);\n  border: 1px solid rgb(255, 255, 255);\n  backdrop-filter: blur(10px);\n  box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);\n}\n\n/***** NEUMORPHISM *****/\n.neumorphism .dashboard-div {\n  margin: 10px;\n  border-radius: 15px;\n  background-color: #e0e0e0;\n  box-shadow: 5px 5px 10px #bebebe, -5px -5px 10px #ffffff;\n}\n\n/***** MINIMALISM *****/\n.minimalism .dashboard-div {\n  margin-bottom: 5px;\n}\n", ""]);
+                a.push([t.id, '/***** EMBEDDING *****/\n.basic .dashboard-div {\n  border: 1px solid black;\n  text-align: center;\n}\n\n.dark .dashboard-div {\n  margin: 2px;\n  border-radius: 10px;\n  background-color: #262626;\n  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.5);\n}\n\n.glassmorphism .dashboard-div {\n  margin: 5px;\n  border-radius: 10px;\n  background: rgb(255, 254, 254);\n  border: 1px solid rgb(255, 255, 255);\n  backdrop-filter: blur(10px);\n  box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);\n}\n\n.neumorphism .dashboard-div {\n  margin: 10px;\n  border-radius: 15px;\n  background-color: #e0e0e0;\n  box-shadow: 5px 5px 10px #bebebe, -5px -5px 10px #ffffff;\n}\n\n.minimalism .dashboard-div {\n  margin-bottom: 5px;\n}\n\n/***** RANGE SLIDER *****/\n.range_outside_container {\n  display: flex;\n  max-width: 500px;\n}\n\n.range_inside_container {\n  display: flex;\n  flex-direction: column;\n  width: 80%;\n}\n\n.range_description {\n  padding-right: 20px;\n}\n\n.range_value {\n  padding-left: 20px;\n  width: 80px;\n}\n\n.sliders_control {\n  position: relative;\n  min-height: 50px;\n}\n\ninput[type="range"]::-webkit-slider-thumb {\n  -webkit-appearance: none;\n  pointer-events: all;\n  width: 24px;\n  height: 24px;\n  background-color: #fff;\n  border-radius: 50%;\n  box-shadow: 0 0 0 1px #c6c6c6;\n  cursor: pointer;\n}\n\ninput[type="range"]::-moz-range-thumb {\n  -webkit-appearance: none;\n  pointer-events: all;\n  width: 24px;\n  height: 24px;\n  background-color: #fff;\n  border-radius: 50%;\n  box-shadow: 0 0 0 1px #c6c6c6;\n  cursor: pointer;\n}\n\ninput[type="range"]::-webkit-slider-thumb:hover {\n  background: #f7f7f7;\n}\n\ninput[type="range"]::-webkit-slider-thumb:active {\n  box-shadow: inset 0 0 3px #387bbe, 0 0 9px #387bbe;\n  -webkit-box-shadow: inset 0 0 3px #387bbe, 0 0 9px #387bbe;\n}\n\ninput[type="range"] {\n  -webkit-appearance: none;\n  appearance: none;\n  height: 10px;\n  width: 100%;\n  position: absolute;\n  background-color: #f79847;\n  pointer-events: none;\n}\n\n.top_slider {\n  height: 0 !important;\n  z-index: 1;\n  top: 5px;\n}\n', ""]);
                 const s = a
             },
             314: t => {
                 t.exports = function(t) {
                     var e = [];
                     return e.toString = function() {
                         return this.map((function(e) {
@@ -24,19 +24,19 @@
                     }, e.i = function(t, n, r, i, o) {
                         "string" == typeof t && (t = [
                             [null, t, void 0]
                         ]);
                         var a = {};
                         if (r)
                             for (var s = 0; s < this.length; s++) {
-                                var u = this[s][0];
-                                null != u && (a[u] = !0)
+                                var l = this[s][0];
+                                null != l && (a[l] = !0)
                             }
-                        for (var l = 0; l < t.length; l++) {
-                            var c = [].concat(t[l]);
+                        for (var u = 0; u < t.length; u++) {
+                            var c = [].concat(t[u]);
                             r && a[c[0]] || (void 0 !== o && (void 0 === c[5] || (c[1] = "@layer".concat(c[5].length > 0 ? " ".concat(c[5]) : "", " {").concat(c[1], "}")), c[5] = o), n && (c[2] ? (c[1] = "@media ".concat(c[2], " {").concat(c[1], "}"), c[2] = n) : c[2] = n), i && (c[4] ? (c[1] = "@supports (".concat(c[4], ") {").concat(c[1], "}"), c[4] = i) : c[4] = "".concat(i)), e.push(c))
                         }
                     }, e
                 }
             },
             601: t => {
                 t.exports = function(t) {
@@ -52,26 +52,26 @@
                             n = r;
                             break
                         } return n
                 }
 
                 function r(t, r) {
                     for (var o = {}, a = [], s = 0; s < t.length; s++) {
-                        var u = t[s],
-                            l = r.base ? u[0] + r.base : u[0],
-                            c = o[l] || 0,
-                            h = "".concat(l, " ").concat(c);
-                        o[l] = c + 1;
+                        var l = t[s],
+                            u = r.base ? l[0] + r.base : l[0],
+                            c = o[u] || 0,
+                            h = "".concat(u, " ").concat(c);
+                        o[u] = c + 1;
                         var f = n(h),
                             d = {
-                                css: u[1],
-                                media: u[2],
-                                sourceMap: u[3],
-                                supports: u[4],
-                                layer: u[5]
+                                css: l[1],
+                                media: l[2],
+                                sourceMap: l[3],
+                                supports: l[4],
+                                layer: l[5]
                             };
                         if (-1 !== f) e[f].references++, e[f].updater(d);
                         else {
                             var p = i(d, r);
                             r.byIndex = s, e.splice(s, 0, {
                                 identifier: h,
                                 updater: p,
@@ -97,19 +97,19 @@
                     var o = r(t = t || [], i = i || {});
                     return function(t) {
                         t = t || [];
                         for (var a = 0; a < o.length; a++) {
                             var s = n(o[a]);
                             e[s].references--
                         }
-                        for (var u = r(t, i), l = 0; l < o.length; l++) {
-                            var c = n(o[l]);
+                        for (var l = r(t, i), u = 0; u < o.length; u++) {
+                            var c = n(o[u]);
                             0 === e[c].references && (e[c].updater(), e.splice(c, 1))
                         }
-                        o = u
+                        o = l
                     }
                 }
             },
             659: t => {
                 var e = {};
                 t.exports = function(t, n) {
                     var r = function(t) {
@@ -179,15 +179,15 @@
             55: t => {
                 t.exports = e
             },
             308: e => {
                 e.exports = t
             },
             330: t => {
-                t.exports = JSON.parse('{"name":"d3vis_ipynb","version":"0.1.2","description":"A Custom Jupyter Widget Library with visualizations created with D3.js.","author":"Daniel Adam Miranda","license":"BSD-3-Clause","main":"lib/index.js","repository":{"type":"git","url":"https://github.com/H-IAAC/d3vis_ipynb.git"},"keywords":["jupyter","widgets","ipython","ipywidgets","jupyterlab-extension"],"files":["lib/**/*.js","dist/*.js","css/*.css"],"scripts":{"clean":"rimraf dist/ && rimraf ../d3vis_ipynb/labextension/ && rimraf ../d3vis_ipynb/nbextension","prepublish":"yarn run clean && yarn run build:prod","build":"webpack --mode=development && yarn run build:labextension:dev","build:prod":"webpack --mode=production && yarn run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","watch":"webpack --watch --mode=development","start":"webpack serve --open --config webpack.exports.config.js","start:export":"webpack serve --open --config webpack.exports.config.js --env export","export":"webpack --env export --config webpack.exports.config.js","test":"echo \\"Error: no test specified\\" && exit 1"},"devDependencies":{"@jupyterlab/builder":"^4.0.6","html-webpack-plugin":"^5.6.0","rimraf":"^2.6.1","webpack":"^5","webpack-dev-server":"^5.0.2"},"dependencies":{"@jupyter-widgets/base":"^1.1 || ^2 || ^3 || ^4 || ^6","d3":"^7.9.0"},"jupyterlab":{"extension":"lib/labplugin","outputDir":"../d3vis_ipynb/labextension","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}}}')
+                t.exports = JSON.parse('{"name":"d3vis_ipynb","version":"0.1.3","description":"A Custom Jupyter Widget Library with visualizations created with D3.js.","author":"Daniel Adam Miranda","license":"BSD-3-Clause","main":"lib/index.js","repository":{"type":"git","url":"https://github.com/H-IAAC/d3vis_ipynb.git"},"keywords":["jupyter","widgets","ipython","ipywidgets","jupyterlab-extension"],"files":["lib/**/*.js","dist/*.js","css/*.css"],"scripts":{"clean":"rimraf dist/ && rimraf ../d3vis_ipynb/labextension/ && rimraf ../d3vis_ipynb/nbextension","prepublish":"yarn run clean && yarn run build:prod","build":"webpack --mode=development && yarn run build:labextension:dev","build:prod":"webpack --mode=production && yarn run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","watch":"webpack --watch --mode=development","start":"webpack serve --open --config webpack.exports.config.js","start:export":"webpack serve --open --config webpack.exports.config.js --env export","export":"webpack --env export --config webpack.exports.config.js","test":"echo \\"Error: no test specified\\" && exit 1"},"devDependencies":{"@jupyterlab/builder":"^4.0.6","html-webpack-plugin":"^5.6.0","rimraf":"^2.6.1","webpack":"^5","webpack-dev-server":"^5.0.2"},"dependencies":{"@jupyter-widgets/base":"^1.1 || ^2 || ^3 || ^4 || ^6","d3":"^7.9.0"},"jupyterlab":{"extension":"lib/labplugin","outputDir":"../d3vis_ipynb/labextension","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}}}')
             }
         },
         r = {};
 
     function i(t) {
         var e = r[t];
         if (void 0 !== e) return e.exports;
@@ -217,75 +217,92 @@
     var o = {};
     return (() => {
         var t = i(308);
         const e = new URL(t.uri, document.location);
         e.pathname = e.pathname.slice(0, e.pathname.lastIndexOf("/") + 1), i.p = `${e.origin}${e.pathname}`
     })(), (() => {
         i.r(o), i.d(o, {
-            BarPlotModel: () => Ii,
-            BarPlotView: () => Vi,
-            EmbeddingModel: () => Li,
+            BarPlotModel: () => Vi,
+            BarPlotView: () => Li,
+            EmbeddingModel: () => qi,
             EmbeddingView: () => Hi,
             HistogramPlotModel: () => Di,
-            HistogramPlotView: () => qi,
+            HistogramPlotView: () => Ii,
             LinearHistPlotModel: () => Ti,
-            LinearHistPlotView: () => Pi,
-            ScatterPlotModel: () => Ci,
-            ScatterPlotView: () => Oi,
-            author: () => Xi.author,
-            dependencies: () => Xi.dependencies,
-            description: () => Xi.description,
-            devDependencies: () => Xi.devDependencies,
-            files: () => Xi.files,
-            jupyterlab: () => Xi.jupyterlab,
-            keywords: () => Xi.keywords,
-            license: () => Xi.license,
-            main: () => Xi.main,
-            name: () => Xi.name,
-            repository: () => Xi.repository,
-            scripts: () => Xi.scripts,
-            version: () => Xi.version
+            LinearHistPlotView: () => ji,
+            RangeSliderModel: () => zi,
+            RangeSliderView: () => Xi,
+            ScatterPlotModel: () => Oi,
+            ScatterPlotView: () => Pi,
+            author: () => Ri.author,
+            dependencies: () => Ri.dependencies,
+            description: () => Ri.description,
+            devDependencies: () => Ri.devDependencies,
+            files: () => Ri.files,
+            jupyterlab: () => Ri.jupyterlab,
+            keywords: () => Ri.keywords,
+            license: () => Ri.license,
+            main: () => Ri.main,
+            name: () => Ri.name,
+            repository: () => Ri.repository,
+            scripts: () => Ri.scripts,
+            version: () => Ri.version
         });
-        var t = i(55);
+        var t = i(55),
+            e = i(72),
+            n = i.n(e),
+            r = i(825),
+            a = i.n(r),
+            s = i(659),
+            l = i.n(s),
+            u = i(56),
+            c = i.n(u),
+            h = i(540),
+            f = i.n(h),
+            d = i(113),
+            p = i.n(d),
+            m = i(930),
+            _ = {};
 
-        function e(t, e) {
+        function g(t, e) {
             let n, r;
             if (void 0 === e)
                 for (const e of t) null != e && (void 0 === n ? e >= e && (n = r = e) : (n > e && (n = e), r < e && (r = e)));
             else {
                 let i = -1;
                 for (let o of t) null != (o = e(o, ++i, t)) && (void 0 === n ? o >= o && (n = r = o) : (n > o && (n = o), r < o && (r = o)))
             }
             return [n, r]
         }
-        var n = Array.prototype,
-            r = n.slice;
+        _.styleTagTransform = p(), _.setAttributes = c(), _.insert = l().bind(null, "head"), _.domAPI = a(), _.insertStyleElement = f(), n()(m.A, _), m.A && m.A.locals && m.A.locals;
+        var v = Array.prototype,
+            y = v.slice;
 
-        function a(t, e) {
+        function w(t, e) {
             return null == t || null == e ? NaN : t < e ? -1 : t > e ? 1 : t >= e ? 0 : NaN
         }
 
-        function s(t, e) {
+        function x(t, e) {
             return null == t || null == e ? NaN : e < t ? -1 : e > t ? 1 : e >= t ? 0 : NaN
         }
 
-        function u(t) {
+        function b(t) {
             let e, n, r;
 
             function i(t, r, i = 0, o = t.length) {
                 if (i < o) {
                     if (0 !== e(r, r)) return o;
                     do {
                         const e = i + o >>> 1;
                         n(t[e], r) < 0 ? i = e + 1 : o = e
                     } while (i < o)
                 }
                 return i
             }
-            return 2 !== t.length ? (e = a, n = (e, n) => a(t(e), n), r = (e, n) => t(e) - n) : (e = t === a || t === s ? t : l, n = t, r = t), {
+            return 2 !== t.length ? (e = w, n = (e, n) => w(t(e), n), r = (e, n) => t(e) - n) : (e = t === w || t === x ? t : M, n = t, r = t), {
                 left: i,
                 center: function(t, e, n = 0, o = t.length) {
                     const a = i(t, e, n, o - 1);
                     return a > n && r(t[a - 1], e) > -r(t[a], e) ? a - 1 : a
                 },
                 right: function(t, r, i = 0, o = t.length) {
                     if (i < o) {
@@ -296,219 +313,219 @@
                         } while (i < o)
                     }
                     return i
                 }
             }
         }
 
-        function l() {
+        function M() {
             return 0
         }
-        n.map;
-        const c = u(a),
-            h = c.right,
-            f = (c.left, u((function(t) {
+        v.map;
+        const k = b(w),
+            A = k.right,
+            E = (k.left, b((function(t) {
                 return null === t ? NaN : +t
-            })).center, h);
+            })).center, A);
 
-        function d(t) {
+        function N(t) {
             return () => t
         }
 
-        function p(t) {
+        function S(t) {
             return t
         }
-        const m = Math.sqrt(50),
-            _ = Math.sqrt(10),
-            g = Math.sqrt(2);
+        const $ = Math.sqrt(50),
+            C = Math.sqrt(10),
+            T = Math.sqrt(2);
 
-        function v(t, e, n) {
+        function j(t, e, n) {
             const r = (e - t) / Math.max(0, n),
                 i = Math.floor(Math.log10(r)),
                 o = r / Math.pow(10, i),
-                a = o >= m ? 10 : o >= _ ? 5 : o >= g ? 2 : 1;
-            let s, u, l;
-            return i < 0 ? (l = Math.pow(10, -i) / a, s = Math.round(t * l), u = Math.round(e * l), s / l < t && ++s, u / l > e && --u, l = -l) : (l = Math.pow(10, i) * a, s = Math.round(t / l), u = Math.round(e / l), s * l < t && ++s, u * l > e && --u), u < s && .5 <= n && n < 2 ? v(t, e, 2 * n) : [s, u, l]
+                a = o >= $ ? 10 : o >= C ? 5 : o >= T ? 2 : 1;
+            let s, l, u;
+            return i < 0 ? (u = Math.pow(10, -i) / a, s = Math.round(t * u), l = Math.round(e * u), s / u < t && ++s, l / u > e && --l, u = -u) : (u = Math.pow(10, i) * a, s = Math.round(t / u), l = Math.round(e / u), s * u < t && ++s, l * u > e && --l), l < s && .5 <= n && n < 2 ? j(t, e, 2 * n) : [s, l, u]
         }
 
-        function y(t, e, n) {
+        function O(t, e, n) {
             if (!((n = +n) > 0)) return [];
             if ((t = +t) == (e = +e)) return [t];
             const r = e < t,
-                [i, o, a] = r ? v(e, t, n) : v(t, e, n);
+                [i, o, a] = r ? j(e, t, n) : j(t, e, n);
             if (!(o >= i)) return [];
             const s = o - i + 1,
-                u = new Array(s);
+                l = new Array(s);
             if (r)
                 if (a < 0)
-                    for (let t = 0; t < s; ++t) u[t] = (o - t) / -a;
+                    for (let t = 0; t < s; ++t) l[t] = (o - t) / -a;
                 else
-                    for (let t = 0; t < s; ++t) u[t] = (o - t) * a;
+                    for (let t = 0; t < s; ++t) l[t] = (o - t) * a;
             else if (a < 0)
-                for (let t = 0; t < s; ++t) u[t] = (i + t) / -a;
+                for (let t = 0; t < s; ++t) l[t] = (i + t) / -a;
             else
-                for (let t = 0; t < s; ++t) u[t] = (i + t) * a;
-            return u
+                for (let t = 0; t < s; ++t) l[t] = (i + t) * a;
+            return l
         }
 
-        function w(t, e, n) {
-            return v(t = +t, e = +e, n = +n)[2]
+        function P(t, e, n) {
+            return j(t = +t, e = +e, n = +n)[2]
         }
 
-        function x(t) {
+        function V(t) {
             return Math.max(1, Math.ceil(Math.log(function(t, e) {
                 let n = 0;
                 for (let e of t) null != e && (e = +e) >= e && ++n;
                 return n
             }(t)) / Math.LN2) + 1)
         }
 
-        function b() {
-            var t = p,
-                n = e,
-                i = x;
+        function L() {
+            var t = S,
+                e = g,
+                n = V;
 
-            function o(r) {
+            function r(r) {
                 Array.isArray(r) || (r = Array.from(r));
-                var o, a, s, u = r.length,
-                    l = new Array(u);
-                for (o = 0; o < u; ++o) l[o] = t(r[o], o, r);
-                var c = n(l),
-                    h = c[0],
-                    d = c[1],
-                    p = i(l, h, d);
-                if (!Array.isArray(p)) {
-                    const t = d,
-                        r = +p;
-                    if (n === e && ([h, d] = function(t, e, n) {
+                var i, o, a, s = r.length,
+                    l = new Array(s);
+                for (i = 0; i < s; ++i) l[i] = t(r[i], i, r);
+                var u = e(l),
+                    c = u[0],
+                    h = u[1],
+                    f = n(l, c, h);
+                if (!Array.isArray(f)) {
+                    const t = h,
+                        n = +f;
+                    if (e === g && ([c, h] = function(t, e, n) {
                             let r;
                             for (;;) {
-                                const i = w(t, e, n);
+                                const i = P(t, e, n);
                                 if (i === r || 0 === i || !isFinite(i)) return [t, e];
                                 i > 0 ? (t = Math.floor(t / i) * i, e = Math.ceil(e / i) * i) : i < 0 && (t = Math.ceil(t * i) / i, e = Math.floor(e * i) / i), r = i
                             }
-                        }(h, d, r)), (p = y(h, d, r))[0] <= h && (s = w(h, d, r)), p[p.length - 1] >= d)
-                        if (t >= d && n === e) {
-                            const t = w(h, d, r);
-                            isFinite(t) && (t > 0 ? d = (Math.floor(d / t) + 1) * t : t < 0 && (d = (Math.ceil(d * -t) + 1) / -t))
-                        } else p.pop()
-                }
-                for (var m = p.length, _ = 0, g = m; p[_] <= h;) ++_;
-                for (; p[g - 1] > d;) --g;
-                (_ || g < m) && (p = p.slice(_, g), m = g - _);
-                var v, x = new Array(m + 1);
-                for (o = 0; o <= m; ++o)(v = x[o] = []).x0 = o > 0 ? p[o - 1] : h, v.x1 = o < m ? p[o] : d;
-                if (isFinite(s)) {
-                    if (s > 0)
-                        for (o = 0; o < u; ++o) null != (a = l[o]) && h <= a && a <= d && x[Math.min(m, Math.floor((a - h) / s))].push(r[o]);
-                    else if (s < 0)
-                        for (o = 0; o < u; ++o)
-                            if (null != (a = l[o]) && h <= a && a <= d) {
-                                const t = Math.floor((h - a) * s);
-                                x[Math.min(m, t + (p[t] <= a))].push(r[o])
+                        }(c, h, n)), (f = O(c, h, n))[0] <= c && (a = P(c, h, n)), f[f.length - 1] >= h)
+                        if (t >= h && e === g) {
+                            const t = P(c, h, n);
+                            isFinite(t) && (t > 0 ? h = (Math.floor(h / t) + 1) * t : t < 0 && (h = (Math.ceil(h * -t) + 1) / -t))
+                        } else f.pop()
+                }
+                for (var d = f.length, p = 0, m = d; f[p] <= c;) ++p;
+                for (; f[m - 1] > h;) --m;
+                (p || m < d) && (f = f.slice(p, m), d = m - p);
+                var _, v = new Array(d + 1);
+                for (i = 0; i <= d; ++i)(_ = v[i] = []).x0 = i > 0 ? f[i - 1] : c, _.x1 = i < d ? f[i] : h;
+                if (isFinite(a)) {
+                    if (a > 0)
+                        for (i = 0; i < s; ++i) null != (o = l[i]) && c <= o && o <= h && v[Math.min(d, Math.floor((o - c) / a))].push(r[i]);
+                    else if (a < 0)
+                        for (i = 0; i < s; ++i)
+                            if (null != (o = l[i]) && c <= o && o <= h) {
+                                const t = Math.floor((c - o) * a);
+                                v[Math.min(d, t + (f[t] <= o))].push(r[i])
                             }
                 } else
-                    for (o = 0; o < u; ++o) null != (a = l[o]) && h <= a && a <= d && x[f(p, a, 0, m)].push(r[o]);
-                return x
+                    for (i = 0; i < s; ++i) null != (o = l[i]) && c <= o && o <= h && v[E(f, o, 0, d)].push(r[i]);
+                return v
             }
-            return o.value = function(e) {
-                return arguments.length ? (t = "function" == typeof e ? e : d(e), o) : t
-            }, o.domain = function(t) {
-                return arguments.length ? (n = "function" == typeof t ? t : d([t[0], t[1]]), o) : n
-            }, o.thresholds = function(t) {
-                return arguments.length ? (i = "function" == typeof t ? t : d(Array.isArray(t) ? r.call(t) : t), o) : i
-            }, o
+            return r.value = function(e) {
+                return arguments.length ? (t = "function" == typeof e ? e : N(e), r) : t
+            }, r.domain = function(t) {
+                return arguments.length ? (e = "function" == typeof t ? t : N([t[0], t[1]]), r) : e
+            }, r.thresholds = function(t) {
+                return arguments.length ? (n = "function" == typeof t ? t : N(Array.isArray(t) ? y.call(t) : t), r) : n
+            }, r
         }
 
-        function M(t, e) {
+        function D(t, e) {
             let n;
             if (void 0 === e)
                 for (const e of t) null != e && (n < e || void 0 === n && e >= e) && (n = e);
             else {
                 let r = -1;
                 for (let i of t) null != (i = e(i, ++r, t)) && (n < i || void 0 === n && i >= i) && (n = i)
             }
             return n
         }
 
-        function k(t, e) {
+        function I(t, e) {
             let n;
             if (void 0 === e)
                 for (const e of t) null != e && (n > e || void 0 === n && e >= e) && (n = e);
             else {
                 let r = -1;
                 for (let i of t) null != (i = e(i, ++r, t)) && (n > i || void 0 === n && i >= i) && (n = i)
             }
             return n
         }
 
-        function A(t) {
+        function q(t) {
             return t
         }
-        var N = 1,
-            $ = 2,
-            S = 3,
-            E = 4,
-            j = 1e-6;
+        var H = 1,
+            z = 2,
+            X = 3,
+            R = 4,
+            Y = 1e-6;
 
-        function T(t) {
+        function B(t) {
             return "translate(" + t + ",0)"
         }
 
-        function P(t) {
+        function F(t) {
             return "translate(0," + t + ")"
         }
 
-        function C(t) {
+        function W(t) {
             return e => +t(e)
         }
 
-        function O(t, e) {
+        function U(t, e) {
             return e = Math.max(0, t.bandwidth() - 2 * e) / 2, t.round() && (e = Math.round(e)), n => +t(n) + e
         }
 
-        function I() {
+        function G() {
             return !this.__axis
         }
 
-        function V(t, e) {
+        function J(t, e) {
             var n = [],
                 r = null,
                 i = null,
                 o = 6,
                 a = 6,
                 s = 3,
-                u = "undefined" != typeof window && window.devicePixelRatio > 1 ? 0 : .5,
-                l = t === N || t === E ? -1 : 1,
-                c = t === E || t === $ ? "x" : "y",
-                h = t === N || t === S ? T : P;
+                l = "undefined" != typeof window && window.devicePixelRatio > 1 ? 0 : .5,
+                u = t === H || t === R ? -1 : 1,
+                c = t === R || t === z ? "x" : "y",
+                h = t === H || t === X ? B : F;
 
             function f(f) {
                 var d = null == r ? e.ticks ? e.ticks.apply(e, n) : e.domain() : r,
-                    p = null == i ? e.tickFormat ? e.tickFormat.apply(e, n) : A : i,
+                    p = null == i ? e.tickFormat ? e.tickFormat.apply(e, n) : q : i,
                     m = Math.max(o, 0) + s,
                     _ = e.range(),
-                    g = +_[0] + u,
-                    v = +_[_.length - 1] + u,
-                    y = (e.bandwidth ? O : C)(e.copy(), u),
+                    g = +_[0] + l,
+                    v = +_[_.length - 1] + l,
+                    y = (e.bandwidth ? U : W)(e.copy(), l),
                     w = f.selection ? f.selection() : f,
                     x = w.selectAll(".domain").data([null]),
                     b = w.selectAll(".tick").data(d, e).order(),
                     M = b.exit(),
                     k = b.enter().append("g").attr("class", "tick"),
-                    T = b.select("line"),
-                    P = b.select("text");
-                x = x.merge(x.enter().insert("path", ".tick").attr("class", "domain").attr("stroke", "currentColor")), b = b.merge(k), T = T.merge(k.append("line").attr("stroke", "currentColor").attr(c + "2", l * o)), P = P.merge(k.append("text").attr("fill", "currentColor").attr(c, l * m).attr("dy", t === N ? "0em" : t === S ? "0.71em" : "0.32em")), f !== w && (x = x.transition(f), b = b.transition(f), T = T.transition(f), P = P.transition(f), M = M.transition(f).attr("opacity", j).attr("transform", (function(t) {
-                    return isFinite(t = y(t)) ? h(t + u) : this.getAttribute("transform")
-                })), k.attr("opacity", j).attr("transform", (function(t) {
+                    A = b.select("line"),
+                    E = b.select("text");
+                x = x.merge(x.enter().insert("path", ".tick").attr("class", "domain").attr("stroke", "currentColor")), b = b.merge(k), A = A.merge(k.append("line").attr("stroke", "currentColor").attr(c + "2", u * o)), E = E.merge(k.append("text").attr("fill", "currentColor").attr(c, u * m).attr("dy", t === H ? "0em" : t === X ? "0.71em" : "0.32em")), f !== w && (x = x.transition(f), b = b.transition(f), A = A.transition(f), E = E.transition(f), M = M.transition(f).attr("opacity", Y).attr("transform", (function(t) {
+                    return isFinite(t = y(t)) ? h(t + l) : this.getAttribute("transform")
+                })), k.attr("opacity", Y).attr("transform", (function(t) {
                     var e = this.parentNode.__axis;
-                    return h((e && isFinite(e = e(t)) ? e : y(t)) + u)
-                }))), M.remove(), x.attr("d", t === E || t === $ ? a ? "M" + l * a + "," + g + "H" + u + "V" + v + "H" + l * a : "M" + u + "," + g + "V" + v : a ? "M" + g + "," + l * a + "V" + u + "H" + v + "V" + l * a : "M" + g + "," + u + "H" + v), b.attr("opacity", 1).attr("transform", (function(t) {
-                    return h(y(t) + u)
-                })), T.attr(c + "2", l * o), P.attr(c, l * m).text(p), w.filter(I).attr("fill", "none").attr("font-size", 10).attr("font-family", "sans-serif").attr("text-anchor", t === $ ? "start" : t === E ? "end" : "middle"), w.each((function() {
+                    return h((e && isFinite(e = e(t)) ? e : y(t)) + l)
+                }))), M.remove(), x.attr("d", t === R || t === z ? a ? "M" + u * a + "," + g + "H" + l + "V" + v + "H" + u * a : "M" + l + "," + g + "V" + v : a ? "M" + g + "," + u * a + "V" + l + "H" + v + "V" + u * a : "M" + g + "," + l + "H" + v), b.attr("opacity", 1).attr("transform", (function(t) {
+                    return h(y(t) + l)
+                })), A.attr(c + "2", u * o), E.attr(c, u * m).text(p), w.filter(G).attr("fill", "none").attr("font-size", 10).attr("font-family", "sans-serif").attr("text-anchor", t === z ? "start" : t === R ? "end" : "middle"), w.each((function() {
                     this.__axis = y
                 }))
             }
             return f.scale = function(t) {
                 return arguments.length ? (e = t, f) : e
             }, f.ticks = function() {
                 return n = Array.from(arguments), f
@@ -523,348 +540,348 @@
             }, f.tickSizeInner = function(t) {
                 return arguments.length ? (o = +t, f) : o
             }, f.tickSizeOuter = function(t) {
                 return arguments.length ? (a = +t, f) : a
             }, f.tickPadding = function(t) {
                 return arguments.length ? (s = +t, f) : s
             }, f.offset = function(t) {
-                return arguments.length ? (u = +t, f) : u
+                return arguments.length ? (l = +t, f) : l
             }, f
         }
 
-        function D(t) {
-            return V(S, t)
+        function Z(t) {
+            return J(X, t)
         }
 
-        function q(t) {
-            return V(E, t)
+        function K(t) {
+            return J(R, t)
         }
 
-        function L() {}
+        function Q() {}
 
-        function H(t) {
-            return null == t ? L : function() {
+        function tt(t) {
+            return null == t ? Q : function() {
                 return this.querySelector(t)
             }
         }
 
-        function X() {
+        function et() {
             return []
         }
 
-        function z(t) {
-            return null == t ? X : function() {
+        function nt(t) {
+            return null == t ? et : function() {
                 return this.querySelectorAll(t)
             }
         }
 
-        function R(t) {
+        function rt(t) {
             return function() {
                 return this.matches(t)
             }
         }
 
-        function Y(t) {
+        function it(t) {
             return function(e) {
                 return e.matches(t)
             }
         }
-        var B = Array.prototype.find;
+        var ot = Array.prototype.find;
 
-        function W() {
+        function at() {
             return this.firstElementChild
         }
-        var F = Array.prototype.filter;
+        var st = Array.prototype.filter;
 
-        function U() {
+        function lt() {
             return Array.from(this.children)
         }
 
-        function G(t) {
+        function ut(t) {
             return new Array(t.length)
         }
 
-        function J(t, e) {
+        function ct(t, e) {
             this.ownerDocument = t.ownerDocument, this.namespaceURI = t.namespaceURI, this._next = null, this._parent = t, this.__data__ = e
         }
 
-        function K(t, e, n, r, i, o) {
-            for (var a, s = 0, u = e.length, l = o.length; s < l; ++s)(a = e[s]) ? (a.__data__ = o[s], r[s] = a) : n[s] = new J(t, o[s]);
-            for (; s < u; ++s)(a = e[s]) && (i[s] = a)
+        function ht(t, e, n, r, i, o) {
+            for (var a, s = 0, l = e.length, u = o.length; s < u; ++s)(a = e[s]) ? (a.__data__ = o[s], r[s] = a) : n[s] = new ct(t, o[s]);
+            for (; s < l; ++s)(a = e[s]) && (i[s] = a)
         }
 
-        function Z(t, e, n, r, i, o, a) {
-            var s, u, l, c = new Map,
+        function ft(t, e, n, r, i, o, a) {
+            var s, l, u, c = new Map,
                 h = e.length,
                 f = o.length,
                 d = new Array(h);
-            for (s = 0; s < h; ++s)(u = e[s]) && (d[s] = l = a.call(u, u.__data__, s, e) + "", c.has(l) ? i[s] = u : c.set(l, u));
-            for (s = 0; s < f; ++s) l = a.call(t, o[s], s, o) + "", (u = c.get(l)) ? (r[s] = u, u.__data__ = o[s], c.delete(l)) : n[s] = new J(t, o[s]);
-            for (s = 0; s < h; ++s)(u = e[s]) && c.get(d[s]) === u && (i[s] = u)
+            for (s = 0; s < h; ++s)(l = e[s]) && (d[s] = u = a.call(l, l.__data__, s, e) + "", c.has(u) ? i[s] = l : c.set(u, l));
+            for (s = 0; s < f; ++s) u = a.call(t, o[s], s, o) + "", (l = c.get(u)) ? (r[s] = l, l.__data__ = o[s], c.delete(u)) : n[s] = new ct(t, o[s]);
+            for (s = 0; s < h; ++s)(l = e[s]) && c.get(d[s]) === l && (i[s] = l)
         }
 
-        function Q(t) {
+        function dt(t) {
             return t.__data__
         }
 
-        function tt(t) {
+        function pt(t) {
             return "object" == typeof t && "length" in t ? t : Array.from(t)
         }
 
-        function et(t, e) {
+        function mt(t, e) {
             return t < e ? -1 : t > e ? 1 : t >= e ? 0 : NaN
         }
-        J.prototype = {
-            constructor: J,
+        ct.prototype = {
+            constructor: ct,
             appendChild: function(t) {
                 return this._parent.insertBefore(t, this._next)
             },
             insertBefore: function(t, e) {
                 return this._parent.insertBefore(t, e)
             },
             querySelector: function(t) {
                 return this._parent.querySelector(t)
             },
             querySelectorAll: function(t) {
                 return this._parent.querySelectorAll(t)
             }
         };
-        var nt = "http://www.w3.org/1999/xhtml";
-        const rt = {
+        var _t = "http://www.w3.org/1999/xhtml";
+        const gt = {
             svg: "http://www.w3.org/2000/svg",
-            xhtml: nt,
+            xhtml: _t,
             xlink: "http://www.w3.org/1999/xlink",
             xml: "http://www.w3.org/XML/1998/namespace",
             xmlns: "http://www.w3.org/2000/xmlns/"
         };
 
-        function it(t) {
+        function vt(t) {
             var e = t += "",
                 n = e.indexOf(":");
-            return n >= 0 && "xmlns" !== (e = t.slice(0, n)) && (t = t.slice(n + 1)), rt.hasOwnProperty(e) ? {
-                space: rt[e],
+            return n >= 0 && "xmlns" !== (e = t.slice(0, n)) && (t = t.slice(n + 1)), gt.hasOwnProperty(e) ? {
+                space: gt[e],
                 local: t
             } : t
         }
 
-        function ot(t) {
+        function yt(t) {
             return function() {
                 this.removeAttribute(t)
             }
         }
 
-        function at(t) {
+        function wt(t) {
             return function() {
                 this.removeAttributeNS(t.space, t.local)
             }
         }
 
-        function st(t, e) {
+        function xt(t, e) {
             return function() {
                 this.setAttribute(t, e)
             }
         }
 
-        function ut(t, e) {
+        function bt(t, e) {
             return function() {
                 this.setAttributeNS(t.space, t.local, e)
             }
         }
 
-        function lt(t, e) {
+        function Mt(t, e) {
             return function() {
                 var n = e.apply(this, arguments);
                 null == n ? this.removeAttribute(t) : this.setAttribute(t, n)
             }
         }
 
-        function ct(t, e) {
+        function kt(t, e) {
             return function() {
                 var n = e.apply(this, arguments);
                 null == n ? this.removeAttributeNS(t.space, t.local) : this.setAttributeNS(t.space, t.local, n)
             }
         }
 
-        function ht(t) {
+        function At(t) {
             return t.ownerDocument && t.ownerDocument.defaultView || t.document && t || t.defaultView
         }
 
-        function ft(t) {
+        function Et(t) {
             return function() {
                 this.style.removeProperty(t)
             }
         }
 
-        function dt(t, e, n) {
+        function Nt(t, e, n) {
             return function() {
                 this.style.setProperty(t, e, n)
             }
         }
 
-        function pt(t, e, n) {
+        function St(t, e, n) {
             return function() {
                 var r = e.apply(this, arguments);
                 null == r ? this.style.removeProperty(t) : this.style.setProperty(t, r, n)
             }
         }
 
-        function mt(t, e) {
-            return t.style.getPropertyValue(e) || ht(t).getComputedStyle(t, null).getPropertyValue(e)
+        function $t(t, e) {
+            return t.style.getPropertyValue(e) || At(t).getComputedStyle(t, null).getPropertyValue(e)
         }
 
-        function _t(t) {
+        function Ct(t) {
             return function() {
                 delete this[t]
             }
         }
 
-        function gt(t, e) {
+        function Tt(t, e) {
             return function() {
                 this[t] = e
             }
         }
 
-        function vt(t, e) {
+        function jt(t, e) {
             return function() {
                 var n = e.apply(this, arguments);
                 null == n ? delete this[t] : this[t] = n
             }
         }
 
-        function yt(t) {
+        function Ot(t) {
             return t.trim().split(/^|\s+/)
         }
 
-        function wt(t) {
-            return t.classList || new xt(t)
+        function Pt(t) {
+            return t.classList || new Vt(t)
         }
 
-        function xt(t) {
-            this._node = t, this._names = yt(t.getAttribute("class") || "")
+        function Vt(t) {
+            this._node = t, this._names = Ot(t.getAttribute("class") || "")
         }
 
-        function bt(t, e) {
-            for (var n = wt(t), r = -1, i = e.length; ++r < i;) n.add(e[r])
+        function Lt(t, e) {
+            for (var n = Pt(t), r = -1, i = e.length; ++r < i;) n.add(e[r])
         }
 
-        function Mt(t, e) {
-            for (var n = wt(t), r = -1, i = e.length; ++r < i;) n.remove(e[r])
+        function Dt(t, e) {
+            for (var n = Pt(t), r = -1, i = e.length; ++r < i;) n.remove(e[r])
         }
 
-        function kt(t) {
+        function It(t) {
             return function() {
-                bt(this, t)
+                Lt(this, t)
             }
         }
 
-        function At(t) {
+        function qt(t) {
             return function() {
-                Mt(this, t)
+                Dt(this, t)
             }
         }
 
-        function Nt(t, e) {
+        function Ht(t, e) {
             return function() {
-                (e.apply(this, arguments) ? bt : Mt)(this, t)
+                (e.apply(this, arguments) ? Lt : Dt)(this, t)
             }
         }
 
-        function $t() {
+        function zt() {
             this.textContent = ""
         }
 
-        function St(t) {
+        function Xt(t) {
             return function() {
                 this.textContent = t
             }
         }
 
-        function Et(t) {
+        function Rt(t) {
             return function() {
                 var e = t.apply(this, arguments);
                 this.textContent = null == e ? "" : e
             }
         }
 
-        function jt() {
+        function Yt() {
             this.innerHTML = ""
         }
 
-        function Tt(t) {
+        function Bt(t) {
             return function() {
                 this.innerHTML = t
             }
         }
 
-        function Pt(t) {
+        function Ft(t) {
             return function() {
                 var e = t.apply(this, arguments);
                 this.innerHTML = null == e ? "" : e
             }
         }
 
-        function Ct() {
+        function Wt() {
             this.nextSibling && this.parentNode.appendChild(this)
         }
 
-        function Ot() {
+        function Ut() {
             this.previousSibling && this.parentNode.insertBefore(this, this.parentNode.firstChild)
         }
 
-        function It(t) {
+        function Gt(t) {
             return function() {
                 var e = this.ownerDocument,
                     n = this.namespaceURI;
-                return n === nt && e.documentElement.namespaceURI === nt ? e.createElement(t) : e.createElementNS(n, t)
+                return n === _t && e.documentElement.namespaceURI === _t ? e.createElement(t) : e.createElementNS(n, t)
             }
         }
 
-        function Vt(t) {
+        function Jt(t) {
             return function() {
                 return this.ownerDocument.createElementNS(t.space, t.local)
             }
         }
 
-        function Dt(t) {
-            var e = it(t);
-            return (e.local ? Vt : It)(e)
+        function Zt(t) {
+            var e = vt(t);
+            return (e.local ? Jt : Gt)(e)
         }
 
-        function qt() {
+        function Kt() {
             return null
         }
 
-        function Lt() {
+        function Qt() {
             var t = this.parentNode;
             t && t.removeChild(this)
         }
 
-        function Ht() {
+        function te() {
             var t = this.cloneNode(!1),
                 e = this.parentNode;
             return e ? e.insertBefore(t, this.nextSibling) : t
         }
 
-        function Xt() {
+        function ee() {
             var t = this.cloneNode(!0),
                 e = this.parentNode;
             return e ? e.insertBefore(t, this.nextSibling) : t
         }
 
-        function zt(t) {
+        function ne(t) {
             return function() {
                 var e = this.__on;
                 if (e) {
                     for (var n, r = 0, i = -1, o = e.length; r < o; ++r) n = e[r], t.type && n.type !== t.type || n.name !== t.name ? e[++i] = n : this.removeEventListener(n.type, n.listener, n.options);
                     ++i ? e.length = i : delete this.__on
                 }
             }
         }
 
-        function Rt(t, e, n) {
+        function re(t, e, n) {
             return function() {
                 var r, i = this.__on,
                     o = function(t) {
                         return function(e) {
                             t.call(this, e, this.__data__)
                         }
                     }(e);
@@ -877,154 +894,154 @@
                     value: e,
                     listener: o,
                     options: n
                 }, i ? i.push(r) : this.__on = [r]
             }
         }
 
-        function Yt(t, e, n) {
-            var r = ht(t),
+        function ie(t, e, n) {
+            var r = At(t),
                 i = r.CustomEvent;
             "function" == typeof i ? i = new i(e, n) : (i = r.document.createEvent("Event"), n ? (i.initEvent(e, n.bubbles, n.cancelable), i.detail = n.detail) : i.initEvent(e, !1, !1)), t.dispatchEvent(i)
         }
 
-        function Bt(t, e) {
+        function oe(t, e) {
             return function() {
-                return Yt(this, t, e)
+                return ie(this, t, e)
             }
         }
 
-        function Wt(t, e) {
+        function ae(t, e) {
             return function() {
-                return Yt(this, t, e.apply(this, arguments))
+                return ie(this, t, e.apply(this, arguments))
             }
         }
-        xt.prototype = {
+        Vt.prototype = {
             add: function(t) {
                 this._names.indexOf(t) < 0 && (this._names.push(t), this._node.setAttribute("class", this._names.join(" ")))
             },
             remove: function(t) {
                 var e = this._names.indexOf(t);
                 e >= 0 && (this._names.splice(e, 1), this._node.setAttribute("class", this._names.join(" ")))
             },
             contains: function(t) {
                 return this._names.indexOf(t) >= 0
             }
         };
-        var Ft = [null];
+        var se = [null];
 
-        function Ut(t, e) {
+        function le(t, e) {
             this._groups = t, this._parents = e
         }
 
-        function Gt() {
-            return new Ut([
+        function ue() {
+            return new le([
                 [document.documentElement]
-            ], Ft)
+            ], se)
         }
-        Ut.prototype = Gt.prototype = {
-            constructor: Ut,
+        le.prototype = ue.prototype = {
+            constructor: le,
             select: function(t) {
-                "function" != typeof t && (t = H(t));
+                "function" != typeof t && (t = tt(t));
                 for (var e = this._groups, n = e.length, r = new Array(n), i = 0; i < n; ++i)
-                    for (var o, a, s = e[i], u = s.length, l = r[i] = new Array(u), c = 0; c < u; ++c)(o = s[c]) && (a = t.call(o, o.__data__, c, s)) && ("__data__" in o && (a.__data__ = o.__data__), l[c] = a);
-                return new Ut(r, this._parents)
+                    for (var o, a, s = e[i], l = s.length, u = r[i] = new Array(l), c = 0; c < l; ++c)(o = s[c]) && (a = t.call(o, o.__data__, c, s)) && ("__data__" in o && (a.__data__ = o.__data__), u[c] = a);
+                return new le(r, this._parents)
             },
             selectAll: function(t) {
                 t = "function" == typeof t ? function(t) {
                     return function() {
                         return null == (e = t.apply(this, arguments)) ? [] : Array.isArray(e) ? e : Array.from(e);
                         var e
                     }
-                }(t) : z(t);
+                }(t) : nt(t);
                 for (var e = this._groups, n = e.length, r = [], i = [], o = 0; o < n; ++o)
-                    for (var a, s = e[o], u = s.length, l = 0; l < u; ++l)(a = s[l]) && (r.push(t.call(a, a.__data__, l, s)), i.push(a));
-                return new Ut(r, i)
+                    for (var a, s = e[o], l = s.length, u = 0; u < l; ++u)(a = s[u]) && (r.push(t.call(a, a.__data__, u, s)), i.push(a));
+                return new le(r, i)
             },
             selectChild: function(t) {
-                return this.select(null == t ? W : function(t) {
+                return this.select(null == t ? at : function(t) {
                     return function() {
-                        return B.call(this.children, t)
+                        return ot.call(this.children, t)
                     }
-                }("function" == typeof t ? t : Y(t)))
+                }("function" == typeof t ? t : it(t)))
             },
             selectChildren: function(t) {
-                return this.selectAll(null == t ? U : function(t) {
+                return this.selectAll(null == t ? lt : function(t) {
                     return function() {
-                        return F.call(this.children, t)
+                        return st.call(this.children, t)
                     }
-                }("function" == typeof t ? t : Y(t)))
+                }("function" == typeof t ? t : it(t)))
             },
             filter: function(t) {
-                "function" != typeof t && (t = R(t));
+                "function" != typeof t && (t = rt(t));
                 for (var e = this._groups, n = e.length, r = new Array(n), i = 0; i < n; ++i)
-                    for (var o, a = e[i], s = a.length, u = r[i] = [], l = 0; l < s; ++l)(o = a[l]) && t.call(o, o.__data__, l, a) && u.push(o);
-                return new Ut(r, this._parents)
+                    for (var o, a = e[i], s = a.length, l = r[i] = [], u = 0; u < s; ++u)(o = a[u]) && t.call(o, o.__data__, u, a) && l.push(o);
+                return new le(r, this._parents)
             },
             data: function(t, e) {
-                if (!arguments.length) return Array.from(this, Q);
-                var n, r = e ? Z : K,
+                if (!arguments.length) return Array.from(this, dt);
+                var n, r = e ? ft : ht,
                     i = this._parents,
                     o = this._groups;
                 "function" != typeof t && (n = t, t = function() {
                     return n
                 });
-                for (var a = o.length, s = new Array(a), u = new Array(a), l = new Array(a), c = 0; c < a; ++c) {
+                for (var a = o.length, s = new Array(a), l = new Array(a), u = new Array(a), c = 0; c < a; ++c) {
                     var h = i[c],
                         f = o[c],
                         d = f.length,
-                        p = tt(t.call(h, h && h.__data__, c, i)),
+                        p = pt(t.call(h, h && h.__data__, c, i)),
                         m = p.length,
-                        _ = u[c] = new Array(m),
+                        _ = l[c] = new Array(m),
                         g = s[c] = new Array(m);
-                    r(h, f, _, g, l[c] = new Array(d), p, e);
+                    r(h, f, _, g, u[c] = new Array(d), p, e);
                     for (var v, y, w = 0, x = 0; w < m; ++w)
                         if (v = _[w]) {
                             for (w >= x && (x = w + 1); !(y = g[x]) && ++x < m;);
                             v._next = y || null
                         }
                 }
-                return (s = new Ut(s, i))._enter = u, s._exit = l, s
+                return (s = new le(s, i))._enter = l, s._exit = u, s
             },
             enter: function() {
-                return new Ut(this._enter || this._groups.map(G), this._parents)
+                return new le(this._enter || this._groups.map(ut), this._parents)
             },
             exit: function() {
-                return new Ut(this._exit || this._groups.map(G), this._parents)
+                return new le(this._exit || this._groups.map(ut), this._parents)
             },
             join: function(t, e, n) {
                 var r = this.enter(),
                     i = this,
                     o = this.exit();
                 return "function" == typeof t ? (r = t(r)) && (r = r.selection()) : r = r.append(t + ""), null != e && (i = e(i)) && (i = i.selection()), null == n ? o.remove() : n(o), r && i ? r.merge(i).order() : i
             },
             merge: function(t) {
-                for (var e = t.selection ? t.selection() : t, n = this._groups, r = e._groups, i = n.length, o = r.length, a = Math.min(i, o), s = new Array(i), u = 0; u < a; ++u)
-                    for (var l, c = n[u], h = r[u], f = c.length, d = s[u] = new Array(f), p = 0; p < f; ++p)(l = c[p] || h[p]) && (d[p] = l);
-                for (; u < i; ++u) s[u] = n[u];
-                return new Ut(s, this._parents)
+                for (var e = t.selection ? t.selection() : t, n = this._groups, r = e._groups, i = n.length, o = r.length, a = Math.min(i, o), s = new Array(i), l = 0; l < a; ++l)
+                    for (var u, c = n[l], h = r[l], f = c.length, d = s[l] = new Array(f), p = 0; p < f; ++p)(u = c[p] || h[p]) && (d[p] = u);
+                for (; l < i; ++l) s[l] = n[l];
+                return new le(s, this._parents)
             },
             selection: function() {
                 return this
             },
             order: function() {
                 for (var t = this._groups, e = -1, n = t.length; ++e < n;)
                     for (var r, i = t[e], o = i.length - 1, a = i[o]; --o >= 0;)(r = i[o]) && (a && 4 ^ r.compareDocumentPosition(a) && a.parentNode.insertBefore(r, a), a = r);
                 return this
             },
             sort: function(t) {
                 function e(e, n) {
                     return e && n ? t(e.__data__, n.__data__) : !e - !n
                 }
-                t || (t = et);
+                t || (t = mt);
                 for (var n = this._groups, r = n.length, i = new Array(r), o = 0; o < r; ++o) {
-                    for (var a, s = n[o], u = s.length, l = i[o] = new Array(u), c = 0; c < u; ++c)(a = s[c]) && (l[c] = a);
-                    l.sort(e)
+                    for (var a, s = n[o], l = s.length, u = i[o] = new Array(l), c = 0; c < l; ++c)(a = s[c]) && (u[c] = a);
+                    u.sort(e)
                 }
-                return new Ut(i, this._parents).order()
+                return new le(i, this._parents).order()
             },
             call: function() {
                 var t = arguments[0];
                 return arguments[0] = this, t.apply(null, arguments), this
             },
             nodes: function() {
                 return Array.from(this)
@@ -1047,66 +1064,66 @@
             },
             each: function(t) {
                 for (var e = this._groups, n = 0, r = e.length; n < r; ++n)
                     for (var i, o = e[n], a = 0, s = o.length; a < s; ++a)(i = o[a]) && t.call(i, i.__data__, a, o);
                 return this
             },
             attr: function(t, e) {
-                var n = it(t);
+                var n = vt(t);
                 if (arguments.length < 2) {
                     var r = this.node();
                     return n.local ? r.getAttributeNS(n.space, n.local) : r.getAttribute(n)
                 }
-                return this.each((null == e ? n.local ? at : ot : "function" == typeof e ? n.local ? ct : lt : n.local ? ut : st)(n, e))
+                return this.each((null == e ? n.local ? wt : yt : "function" == typeof e ? n.local ? kt : Mt : n.local ? bt : xt)(n, e))
             },
             style: function(t, e, n) {
-                return arguments.length > 1 ? this.each((null == e ? ft : "function" == typeof e ? pt : dt)(t, e, null == n ? "" : n)) : mt(this.node(), t)
+                return arguments.length > 1 ? this.each((null == e ? Et : "function" == typeof e ? St : Nt)(t, e, null == n ? "" : n)) : $t(this.node(), t)
             },
             property: function(t, e) {
-                return arguments.length > 1 ? this.each((null == e ? _t : "function" == typeof e ? vt : gt)(t, e)) : this.node()[t]
+                return arguments.length > 1 ? this.each((null == e ? Ct : "function" == typeof e ? jt : Tt)(t, e)) : this.node()[t]
             },
             classed: function(t, e) {
-                var n = yt(t + "");
+                var n = Ot(t + "");
                 if (arguments.length < 2) {
-                    for (var r = wt(this.node()), i = -1, o = n.length; ++i < o;)
+                    for (var r = Pt(this.node()), i = -1, o = n.length; ++i < o;)
                         if (!r.contains(n[i])) return !1;
                     return !0
                 }
-                return this.each(("function" == typeof e ? Nt : e ? kt : At)(n, e))
+                return this.each(("function" == typeof e ? Ht : e ? It : qt)(n, e))
             },
             text: function(t) {
-                return arguments.length ? this.each(null == t ? $t : ("function" == typeof t ? Et : St)(t)) : this.node().textContent
+                return arguments.length ? this.each(null == t ? zt : ("function" == typeof t ? Rt : Xt)(t)) : this.node().textContent
             },
             html: function(t) {
-                return arguments.length ? this.each(null == t ? jt : ("function" == typeof t ? Pt : Tt)(t)) : this.node().innerHTML
+                return arguments.length ? this.each(null == t ? Yt : ("function" == typeof t ? Ft : Bt)(t)) : this.node().innerHTML
             },
             raise: function() {
-                return this.each(Ct)
+                return this.each(Wt)
             },
             lower: function() {
-                return this.each(Ot)
+                return this.each(Ut)
             },
             append: function(t) {
-                var e = "function" == typeof t ? t : Dt(t);
+                var e = "function" == typeof t ? t : Zt(t);
                 return this.select((function() {
                     return this.appendChild(e.apply(this, arguments))
                 }))
             },
             insert: function(t, e) {
-                var n = "function" == typeof t ? t : Dt(t),
-                    r = null == e ? qt : "function" == typeof e ? e : H(e);
+                var n = "function" == typeof t ? t : Zt(t),
+                    r = null == e ? Kt : "function" == typeof e ? e : tt(e);
                 return this.select((function() {
                     return this.insertBefore(n.apply(this, arguments), r.apply(this, arguments) || null)
                 }))
             },
             remove: function() {
-                return this.each(Lt)
+                return this.each(Qt)
             },
             clone: function(t) {
-                return this.select(t ? Xt : Ht)
+                return this.select(t ? ee : te)
             },
             datum: function(t) {
                 return arguments.length ? this.property("__data__", t) : this.node().__data__
             },
             on: function(t, e, n) {
                 var r, i, o = function(t) {
                         return t.trim().split(/^|\s+/).map((function(t) {
@@ -1116,65 +1133,65 @@
                                 type: t,
                                 name: e
                             }
                         }))
                     }(t + ""),
                     a = o.length;
                 if (!(arguments.length < 2)) {
-                    for (s = e ? Rt : zt, r = 0; r < a; ++r) this.each(s(o[r], e, n));
+                    for (s = e ? re : ne, r = 0; r < a; ++r) this.each(s(o[r], e, n));
                     return this
                 }
                 var s = this.node().__on;
                 if (s)
-                    for (var u, l = 0, c = s.length; l < c; ++l)
-                        for (r = 0, u = s[l]; r < a; ++r)
-                            if ((i = o[r]).type === u.type && i.name === u.name) return u.value
+                    for (var l, u = 0, c = s.length; u < c; ++u)
+                        for (r = 0, l = s[u]; r < a; ++r)
+                            if ((i = o[r]).type === l.type && i.name === l.name) return l.value
             },
             dispatch: function(t, e) {
-                return this.each(("function" == typeof e ? Wt : Bt)(t, e))
+                return this.each(("function" == typeof e ? ae : oe)(t, e))
             },
             [Symbol.iterator]: function*() {
                 for (var t = this._groups, e = 0, n = t.length; e < n; ++e)
                     for (var r, i = t[e], o = 0, a = i.length; o < a; ++o)(r = i[o]) && (yield r)
             }
         };
-        const Jt = Gt;
-        var Kt = {
+        const ce = ue;
+        var he = {
             value: () => {}
         };
 
-        function Zt() {
+        function fe() {
             for (var t, e = 0, n = arguments.length, r = {}; e < n; ++e) {
                 if (!(t = arguments[e] + "") || t in r || /[\s.]/.test(t)) throw new Error("illegal type: " + t);
                 r[t] = []
             }
-            return new Qt(r)
+            return new de(r)
         }
 
-        function Qt(t) {
+        function de(t) {
             this._ = t
         }
 
-        function te(t, e) {
+        function pe(t, e) {
             for (var n, r = 0, i = t.length; r < i; ++r)
                 if ((n = t[r]).name === e) return n.value
         }
 
-        function ee(t, e, n) {
+        function me(t, e, n) {
             for (var r = 0, i = t.length; r < i; ++r)
                 if (t[r].name === e) {
-                    t[r] = Kt, t = t.slice(0, r).concat(t.slice(r + 1));
+                    t[r] = he, t = t.slice(0, r).concat(t.slice(r + 1));
                     break
                 } return null != n && t.push({
                 name: e,
                 value: n
             }), t
         }
-        Qt.prototype = Zt.prototype = {
-            constructor: Qt,
+        de.prototype = fe.prototype = {
+            constructor: de,
             on: function(t, e) {
                 var n, r, i = this._,
                     o = (r = i, (t + "").trim().split(/^|\s+/).map((function(t) {
                         var e = "",
                             n = t.indexOf(".");
                         if (n >= 0 && (e = t.slice(n + 1), t = t.slice(0, n)), t && !r.hasOwnProperty(t)) throw new Error("unknown type: " + t);
                         return {
@@ -1183,341 +1200,341 @@
                         }
                     }))),
                     a = -1,
                     s = o.length;
                 if (!(arguments.length < 2)) {
                     if (null != e && "function" != typeof e) throw new Error("invalid callback: " + e);
                     for (; ++a < s;)
-                        if (n = (t = o[a]).type) i[n] = ee(i[n], t.name, e);
+                        if (n = (t = o[a]).type) i[n] = me(i[n], t.name, e);
                         else if (null == e)
-                        for (n in i) i[n] = ee(i[n], t.name, null);
+                        for (n in i) i[n] = me(i[n], t.name, null);
                     return this
                 }
                 for (; ++a < s;)
-                    if ((n = (t = o[a]).type) && (n = te(i[n], t.name))) return n
+                    if ((n = (t = o[a]).type) && (n = pe(i[n], t.name))) return n
             },
             copy: function() {
                 var t = {},
                     e = this._;
                 for (var n in e) t[n] = e[n].slice();
-                return new Qt(t)
+                return new de(t)
             },
             call: function(t, e) {
                 if ((n = arguments.length - 2) > 0)
                     for (var n, r, i = new Array(n), o = 0; o < n; ++o) i[o] = arguments[o + 2];
                 if (!this._.hasOwnProperty(t)) throw new Error("unknown type: " + t);
                 for (o = 0, n = (r = this._[t]).length; o < n; ++o) r[o].value.apply(e, i)
             },
             apply: function(t, e, n) {
                 if (!this._.hasOwnProperty(t)) throw new Error("unknown type: " + t);
                 for (var r = this._[t], i = 0, o = r.length; i < o; ++i) r[i].value.apply(e, n)
             }
         };
-        const ne = Zt;
-        var re, ie, oe = 0,
-            ae = 0,
-            se = 0,
-            ue = 1e3,
-            le = 0,
-            ce = 0,
-            he = 0,
-            fe = "object" == typeof performance && performance.now ? performance : Date,
-            de = "object" == typeof window && window.requestAnimationFrame ? window.requestAnimationFrame.bind(window) : function(t) {
+        const _e = fe;
+        var ge, ve, ye = 0,
+            we = 0,
+            xe = 0,
+            be = 1e3,
+            Me = 0,
+            ke = 0,
+            Ae = 0,
+            Ee = "object" == typeof performance && performance.now ? performance : Date,
+            Ne = "object" == typeof window && window.requestAnimationFrame ? window.requestAnimationFrame.bind(window) : function(t) {
                 setTimeout(t, 17)
             };
 
-        function pe() {
-            return ce || (de(me), ce = fe.now() + he)
+        function Se() {
+            return ke || (Ne($e), ke = Ee.now() + Ae)
         }
 
-        function me() {
-            ce = 0
+        function $e() {
+            ke = 0
         }
 
-        function _e() {
+        function Ce() {
             this._call = this._time = this._next = null
         }
 
-        function ge(t, e, n) {
-            var r = new _e;
+        function Te(t, e, n) {
+            var r = new Ce;
             return r.restart(t, e, n), r
         }
 
-        function ve() {
-            ce = (le = fe.now()) + he, oe = ae = 0;
+        function je() {
+            ke = (Me = Ee.now()) + Ae, ye = we = 0;
             try {
                 ! function() {
-                    pe(), ++oe;
-                    for (var t, e = re; e;)(t = ce - e._time) >= 0 && e._call.call(void 0, t), e = e._next;
-                    --oe
+                    Se(), ++ye;
+                    for (var t, e = ge; e;)(t = ke - e._time) >= 0 && e._call.call(void 0, t), e = e._next;
+                    --ye
                 }()
             } finally {
-                oe = 0,
+                ye = 0,
                     function() {
-                        for (var t, e, n = re, r = 1 / 0; n;) n._call ? (r > n._time && (r = n._time), t = n, n = n._next) : (e = n._next, n._next = null, n = t ? t._next = e : re = e);
-                        ie = t, we(r)
-                    }(), ce = 0
+                        for (var t, e, n = ge, r = 1 / 0; n;) n._call ? (r > n._time && (r = n._time), t = n, n = n._next) : (e = n._next, n._next = null, n = t ? t._next = e : ge = e);
+                        ve = t, Pe(r)
+                    }(), ke = 0
             }
         }
 
-        function ye() {
-            var t = fe.now(),
-                e = t - le;
-            e > ue && (he -= e, le = t)
+        function Oe() {
+            var t = Ee.now(),
+                e = t - Me;
+            e > be && (Ae -= e, Me = t)
         }
 
-        function we(t) {
-            oe || (ae && (ae = clearTimeout(ae)), t - ce > 24 ? (t < 1 / 0 && (ae = setTimeout(ve, t - fe.now() - he)), se && (se = clearInterval(se))) : (se || (le = fe.now(), se = setInterval(ye, ue)), oe = 1, de(ve)))
+        function Pe(t) {
+            ye || (we && (we = clearTimeout(we)), t - ke > 24 ? (t < 1 / 0 && (we = setTimeout(je, t - Ee.now() - Ae)), xe && (xe = clearInterval(xe))) : (xe || (Me = Ee.now(), xe = setInterval(Oe, be)), ye = 1, Ne(je)))
         }
 
-        function xe(t, e, n) {
-            var r = new _e;
+        function Ve(t, e, n) {
+            var r = new Ce;
             return e = null == e ? 0 : +e, r.restart((n => {
                 r.stop(), t(n + e)
             }), e, n), r
         }
-        _e.prototype = ge.prototype = {
-            constructor: _e,
+        Ce.prototype = Te.prototype = {
+            constructor: Ce,
             restart: function(t, e, n) {
                 if ("function" != typeof t) throw new TypeError("callback is not a function");
-                n = (null == n ? pe() : +n) + (null == e ? 0 : +e), this._next || ie === this || (ie ? ie._next = this : re = this, ie = this), this._call = t, this._time = n, we()
+                n = (null == n ? Se() : +n) + (null == e ? 0 : +e), this._next || ve === this || (ve ? ve._next = this : ge = this, ve = this), this._call = t, this._time = n, Pe()
             },
             stop: function() {
-                this._call && (this._call = null, this._time = 1 / 0, we())
+                this._call && (this._call = null, this._time = 1 / 0, Pe())
             }
         };
-        var be = ne("start", "end", "cancel", "interrupt"),
-            Me = [],
-            ke = 0,
-            Ae = 3;
+        var Le = _e("start", "end", "cancel", "interrupt"),
+            De = [],
+            Ie = 0,
+            qe = 3;
 
-        function Ne(t, e, n, r, i, o) {
+        function He(t, e, n, r, i, o) {
             var a = t.__transition;
             if (a) {
                 if (n in a) return
             } else t.__transition = {};
             ! function(t, e, n) {
                 var r, i = t.__transition;
 
-                function o(u) {
-                    var l, c, h, f;
+                function o(l) {
+                    var u, c, h, f;
                     if (1 !== n.state) return s();
-                    for (l in i)
-                        if ((f = i[l]).name === n.name) {
-                            if (f.state === Ae) return xe(o);
-                            4 === f.state ? (f.state = 6, f.timer.stop(), f.on.call("interrupt", t, t.__data__, f.index, f.group), delete i[l]) : +l < e && (f.state = 6, f.timer.stop(), f.on.call("cancel", t, t.__data__, f.index, f.group), delete i[l])
-                        } if (xe((function() {
-                            n.state === Ae && (n.state = 4, n.timer.restart(a, n.delay, n.time), a(u))
+                    for (u in i)
+                        if ((f = i[u]).name === n.name) {
+                            if (f.state === qe) return Ve(o);
+                            4 === f.state ? (f.state = 6, f.timer.stop(), f.on.call("interrupt", t, t.__data__, f.index, f.group), delete i[u]) : +u < e && (f.state = 6, f.timer.stop(), f.on.call("cancel", t, t.__data__, f.index, f.group), delete i[u])
+                        } if (Ve((function() {
+                            n.state === qe && (n.state = 4, n.timer.restart(a, n.delay, n.time), a(l))
                         })), n.state = 2, n.on.call("start", t, t.__data__, n.index, n.group), 2 === n.state) {
-                        for (n.state = Ae, r = new Array(h = n.tween.length), l = 0, c = -1; l < h; ++l)(f = n.tween[l].value.call(t, t.__data__, n.index, n.group)) && (r[++c] = f);
+                        for (n.state = qe, r = new Array(h = n.tween.length), u = 0, c = -1; u < h; ++u)(f = n.tween[u].value.call(t, t.__data__, n.index, n.group)) && (r[++c] = f);
                         r.length = c + 1
                     }
                 }
 
                 function a(e) {
                     for (var i = e < n.duration ? n.ease.call(null, e / n.duration) : (n.timer.restart(s), n.state = 5, 1), o = -1, a = r.length; ++o < a;) r[o].call(t, i);
                     5 === n.state && (n.on.call("end", t, t.__data__, n.index, n.group), s())
                 }
 
                 function s() {
                     for (var r in n.state = 6, n.timer.stop(), delete i[e], i) return;
                     delete t.__transition
                 }
-                i[e] = n, n.timer = ge((function(t) {
+                i[e] = n, n.timer = Te((function(t) {
                     n.state = 1, n.timer.restart(o, n.delay, n.time), n.delay <= t && o(t - n.delay)
                 }), 0, n.time)
             }(t, n, {
                 name: e,
                 index: r,
                 group: i,
-                on: be,
-                tween: Me,
+                on: Le,
+                tween: De,
                 time: o.time,
                 delay: o.delay,
                 duration: o.duration,
                 ease: o.ease,
                 timer: null,
-                state: ke
+                state: Ie
             })
         }
 
-        function $e(t, e) {
-            var n = Ee(t, e);
-            if (n.state > ke) throw new Error("too late; already scheduled");
+        function ze(t, e) {
+            var n = Re(t, e);
+            if (n.state > Ie) throw new Error("too late; already scheduled");
             return n
         }
 
-        function Se(t, e) {
-            var n = Ee(t, e);
-            if (n.state > Ae) throw new Error("too late; already running");
+        function Xe(t, e) {
+            var n = Re(t, e);
+            if (n.state > qe) throw new Error("too late; already running");
             return n
         }
 
-        function Ee(t, e) {
+        function Re(t, e) {
             var n = t.__transition;
             if (!n || !(n = n[e])) throw new Error("transition not found");
             return n
         }
 
-        function je(t, e) {
+        function Ye(t, e) {
             return t = +t, e = +e,
                 function(n) {
                     return t * (1 - n) + e * n
                 }
         }
-        var Te, Pe = 180 / Math.PI,
-            Ce = {
+        var Be, Fe = 180 / Math.PI,
+            We = {
                 translateX: 0,
                 translateY: 0,
                 rotate: 0,
                 skewX: 0,
                 scaleX: 1,
                 scaleY: 1
             };
 
-        function Oe(t, e, n, r, i, o) {
-            var a, s, u;
-            return (a = Math.sqrt(t * t + e * e)) && (t /= a, e /= a), (u = t * n + e * r) && (n -= t * u, r -= e * u), (s = Math.sqrt(n * n + r * r)) && (n /= s, r /= s, u /= s), t * r < e * n && (t = -t, e = -e, u = -u, a = -a), {
+        function Ue(t, e, n, r, i, o) {
+            var a, s, l;
+            return (a = Math.sqrt(t * t + e * e)) && (t /= a, e /= a), (l = t * n + e * r) && (n -= t * l, r -= e * l), (s = Math.sqrt(n * n + r * r)) && (n /= s, r /= s, l /= s), t * r < e * n && (t = -t, e = -e, l = -l, a = -a), {
                 translateX: i,
                 translateY: o,
-                rotate: Math.atan2(e, t) * Pe,
-                skewX: Math.atan(u) * Pe,
+                rotate: Math.atan2(e, t) * Fe,
+                skewX: Math.atan(l) * Fe,
                 scaleX: a,
                 scaleY: s
             }
         }
 
-        function Ie(t, e, n, r) {
+        function Ge(t, e, n, r) {
             function i(t) {
                 return t.length ? t.pop() + " " : ""
             }
             return function(o, a) {
                 var s = [],
-                    u = [];
+                    l = [];
                 return o = t(o), a = t(a),
                     function(t, r, i, o, a, s) {
                         if (t !== i || r !== o) {
-                            var u = a.push("translate(", null, e, null, n);
+                            var l = a.push("translate(", null, e, null, n);
                             s.push({
-                                i: u - 4,
-                                x: je(t, i)
+                                i: l - 4,
+                                x: Ye(t, i)
                             }, {
-                                i: u - 2,
-                                x: je(r, o)
+                                i: l - 2,
+                                x: Ye(r, o)
                             })
                         } else(i || o) && a.push("translate(" + i + e + o + n)
-                    }(o.translateX, o.translateY, a.translateX, a.translateY, s, u),
+                    }(o.translateX, o.translateY, a.translateX, a.translateY, s, l),
                     function(t, e, n, o) {
                         t !== e ? (t - e > 180 ? e += 360 : e - t > 180 && (t += 360), o.push({
                             i: n.push(i(n) + "rotate(", null, r) - 2,
-                            x: je(t, e)
+                            x: Ye(t, e)
                         })) : e && n.push(i(n) + "rotate(" + e + r)
-                    }(o.rotate, a.rotate, s, u),
+                    }(o.rotate, a.rotate, s, l),
                     function(t, e, n, o) {
                         t !== e ? o.push({
                             i: n.push(i(n) + "skewX(", null, r) - 2,
-                            x: je(t, e)
+                            x: Ye(t, e)
                         }) : e && n.push(i(n) + "skewX(" + e + r)
-                    }(o.skewX, a.skewX, s, u),
+                    }(o.skewX, a.skewX, s, l),
                     function(t, e, n, r, o, a) {
                         if (t !== n || e !== r) {
                             var s = o.push(i(o) + "scale(", null, ",", null, ")");
                             a.push({
                                 i: s - 4,
-                                x: je(t, n)
+                                x: Ye(t, n)
                             }, {
                                 i: s - 2,
-                                x: je(e, r)
+                                x: Ye(e, r)
                             })
                         } else 1 === n && 1 === r || o.push(i(o) + "scale(" + n + "," + r + ")")
-                    }(o.scaleX, o.scaleY, a.scaleX, a.scaleY, s, u), o = a = null,
+                    }(o.scaleX, o.scaleY, a.scaleX, a.scaleY, s, l), o = a = null,
                     function(t) {
-                        for (var e, n = -1, r = u.length; ++n < r;) s[(e = u[n]).i] = e.x(t);
+                        for (var e, n = -1, r = l.length; ++n < r;) s[(e = l[n]).i] = e.x(t);
                         return s.join("")
                     }
             }
         }
-        var Ve = Ie((function(t) {
+        var Je = Ge((function(t) {
                 const e = new("function" == typeof DOMMatrix ? DOMMatrix : WebKitCSSMatrix)(t + "");
-                return e.isIdentity ? Ce : Oe(e.a, e.b, e.c, e.d, e.e, e.f)
+                return e.isIdentity ? We : Ue(e.a, e.b, e.c, e.d, e.e, e.f)
             }), "px, ", "px)", "deg)"),
-            De = Ie((function(t) {
-                return null == t ? Ce : (Te || (Te = document.createElementNS("http://www.w3.org/2000/svg", "g")), Te.setAttribute("transform", t), (t = Te.transform.baseVal.consolidate()) ? Oe((t = t.matrix).a, t.b, t.c, t.d, t.e, t.f) : Ce)
+            Ze = Ge((function(t) {
+                return null == t ? We : (Be || (Be = document.createElementNS("http://www.w3.org/2000/svg", "g")), Be.setAttribute("transform", t), (t = Be.transform.baseVal.consolidate()) ? Ue((t = t.matrix).a, t.b, t.c, t.d, t.e, t.f) : We)
             }), ", ", ")", ")");
 
-        function qe(t, e) {
+        function Ke(t, e) {
             var n, r;
             return function() {
-                var i = Se(this, t),
+                var i = Xe(this, t),
                     o = i.tween;
                 if (o !== n)
                     for (var a = 0, s = (r = n = o).length; a < s; ++a)
                         if (r[a].name === e) {
                             (r = r.slice()).splice(a, 1);
                             break
                         } i.tween = r
             }
         }
 
-        function Le(t, e, n) {
+        function Qe(t, e, n) {
             var r, i;
             if ("function" != typeof n) throw new Error;
             return function() {
-                var o = Se(this, t),
+                var o = Xe(this, t),
                     a = o.tween;
                 if (a !== r) {
                     i = (r = a).slice();
                     for (var s = {
                             name: e,
                             value: n
-                        }, u = 0, l = i.length; u < l; ++u)
-                        if (i[u].name === e) {
-                            i[u] = s;
+                        }, l = 0, u = i.length; l < u; ++l)
+                        if (i[l].name === e) {
+                            i[l] = s;
                             break
-                        } u === l && i.push(s)
+                        } l === u && i.push(s)
                 }
                 o.tween = i
             }
         }
 
-        function He(t, e, n) {
+        function tn(t, e, n) {
             var r = t._id;
             return t.each((function() {
-                    var t = Se(this, r);
+                    var t = Xe(this, r);
                     (t.value || (t.value = {}))[e] = n.apply(this, arguments)
                 })),
                 function(t) {
-                    return Ee(t, r).value[e]
+                    return Re(t, r).value[e]
                 }
         }
 
-        function Xe(t, e, n) {
+        function en(t, e, n) {
             t.prototype = e.prototype = n, n.constructor = t
         }
 
-        function ze(t, e) {
+        function nn(t, e) {
             var n = Object.create(t.prototype);
             for (var r in e) n[r] = e[r];
             return n
         }
 
-        function Re() {}
-        var Ye = .7,
-            Be = 1 / Ye,
-            We = "\\s*([+-]?\\d+)\\s*",
-            Fe = "\\s*([+-]?(?:\\d*\\.)?\\d+(?:[eE][+-]?\\d+)?)\\s*",
-            Ue = "\\s*([+-]?(?:\\d*\\.)?\\d+(?:[eE][+-]?\\d+)?)%\\s*",
-            Ge = /^#([0-9a-f]{3,8})$/,
-            Je = new RegExp(`^rgb\\(${We},${We},${We}\\)$`),
-            Ke = new RegExp(`^rgb\\(${Ue},${Ue},${Ue}\\)$`),
-            Ze = new RegExp(`^rgba\\(${We},${We},${We},${Fe}\\)$`),
-            Qe = new RegExp(`^rgba\\(${Ue},${Ue},${Ue},${Fe}\\)$`),
-            tn = new RegExp(`^hsl\\(${Fe},${Ue},${Ue}\\)$`),
-            en = new RegExp(`^hsla\\(${Fe},${Ue},${Ue},${Fe}\\)$`),
-            nn = {
+        function rn() {}
+        var on = .7,
+            an = 1 / on,
+            sn = "\\s*([+-]?\\d+)\\s*",
+            ln = "\\s*([+-]?(?:\\d*\\.)?\\d+(?:[eE][+-]?\\d+)?)\\s*",
+            un = "\\s*([+-]?(?:\\d*\\.)?\\d+(?:[eE][+-]?\\d+)?)%\\s*",
+            cn = /^#([0-9a-f]{3,8})$/,
+            hn = new RegExp(`^rgb\\(${sn},${sn},${sn}\\)$`),
+            fn = new RegExp(`^rgb\\(${un},${un},${un}\\)$`),
+            dn = new RegExp(`^rgba\\(${sn},${sn},${sn},${ln}\\)$`),
+            pn = new RegExp(`^rgba\\(${un},${un},${un},${ln}\\)$`),
+            mn = new RegExp(`^hsl\\(${ln},${un},${un}\\)$`),
+            _n = new RegExp(`^hsla\\(${ln},${un},${un},${ln}\\)$`),
+            gn = {
                 aliceblue: 15792383,
                 antiquewhite: 16444375,
                 aqua: 65535,
                 aquamarine: 8388564,
                 azure: 15794175,
                 beige: 16119260,
                 bisque: 16770244,
@@ -1660,508 +1677,508 @@
                 wheat: 16113331,
                 white: 16777215,
                 whitesmoke: 16119285,
                 yellow: 16776960,
                 yellowgreen: 10145074
             };
 
-        function rn() {
+        function vn() {
             return this.rgb().formatHex()
         }
 
-        function on() {
+        function yn() {
             return this.rgb().formatRgb()
         }
 
-        function an(t) {
+        function wn(t) {
             var e, n;
-            return t = (t + "").trim().toLowerCase(), (e = Ge.exec(t)) ? (n = e[1].length, e = parseInt(e[1], 16), 6 === n ? sn(e) : 3 === n ? new cn(e >> 8 & 15 | e >> 4 & 240, e >> 4 & 15 | 240 & e, (15 & e) << 4 | 15 & e, 1) : 8 === n ? un(e >> 24 & 255, e >> 16 & 255, e >> 8 & 255, (255 & e) / 255) : 4 === n ? un(e >> 12 & 15 | e >> 8 & 240, e >> 8 & 15 | e >> 4 & 240, e >> 4 & 15 | 240 & e, ((15 & e) << 4 | 15 & e) / 255) : null) : (e = Je.exec(t)) ? new cn(e[1], e[2], e[3], 1) : (e = Ke.exec(t)) ? new cn(255 * e[1] / 100, 255 * e[2] / 100, 255 * e[3] / 100, 1) : (e = Ze.exec(t)) ? un(e[1], e[2], e[3], e[4]) : (e = Qe.exec(t)) ? un(255 * e[1] / 100, 255 * e[2] / 100, 255 * e[3] / 100, e[4]) : (e = tn.exec(t)) ? _n(e[1], e[2] / 100, e[3] / 100, 1) : (e = en.exec(t)) ? _n(e[1], e[2] / 100, e[3] / 100, e[4]) : nn.hasOwnProperty(t) ? sn(nn[t]) : "transparent" === t ? new cn(NaN, NaN, NaN, 0) : null
+            return t = (t + "").trim().toLowerCase(), (e = cn.exec(t)) ? (n = e[1].length, e = parseInt(e[1], 16), 6 === n ? xn(e) : 3 === n ? new kn(e >> 8 & 15 | e >> 4 & 240, e >> 4 & 15 | 240 & e, (15 & e) << 4 | 15 & e, 1) : 8 === n ? bn(e >> 24 & 255, e >> 16 & 255, e >> 8 & 255, (255 & e) / 255) : 4 === n ? bn(e >> 12 & 15 | e >> 8 & 240, e >> 8 & 15 | e >> 4 & 240, e >> 4 & 15 | 240 & e, ((15 & e) << 4 | 15 & e) / 255) : null) : (e = hn.exec(t)) ? new kn(e[1], e[2], e[3], 1) : (e = fn.exec(t)) ? new kn(255 * e[1] / 100, 255 * e[2] / 100, 255 * e[3] / 100, 1) : (e = dn.exec(t)) ? bn(e[1], e[2], e[3], e[4]) : (e = pn.exec(t)) ? bn(255 * e[1] / 100, 255 * e[2] / 100, 255 * e[3] / 100, e[4]) : (e = mn.exec(t)) ? Cn(e[1], e[2] / 100, e[3] / 100, 1) : (e = _n.exec(t)) ? Cn(e[1], e[2] / 100, e[3] / 100, e[4]) : gn.hasOwnProperty(t) ? xn(gn[t]) : "transparent" === t ? new kn(NaN, NaN, NaN, 0) : null
         }
 
-        function sn(t) {
-            return new cn(t >> 16 & 255, t >> 8 & 255, 255 & t, 1)
+        function xn(t) {
+            return new kn(t >> 16 & 255, t >> 8 & 255, 255 & t, 1)
         }
 
-        function un(t, e, n, r) {
-            return r <= 0 && (t = e = n = NaN), new cn(t, e, n, r)
+        function bn(t, e, n, r) {
+            return r <= 0 && (t = e = n = NaN), new kn(t, e, n, r)
         }
 
-        function ln(t, e, n, r) {
-            return 1 === arguments.length ? ((i = t) instanceof Re || (i = an(i)), i ? new cn((i = i.rgb()).r, i.g, i.b, i.opacity) : new cn) : new cn(t, e, n, null == r ? 1 : r);
+        function Mn(t, e, n, r) {
+            return 1 === arguments.length ? ((i = t) instanceof rn || (i = wn(i)), i ? new kn((i = i.rgb()).r, i.g, i.b, i.opacity) : new kn) : new kn(t, e, n, null == r ? 1 : r);
             var i
         }
 
-        function cn(t, e, n, r) {
+        function kn(t, e, n, r) {
             this.r = +t, this.g = +e, this.b = +n, this.opacity = +r
         }
 
-        function hn() {
-            return `#${mn(this.r)}${mn(this.g)}${mn(this.b)}`
+        function An() {
+            return `#${$n(this.r)}${$n(this.g)}${$n(this.b)}`
         }
 
-        function fn() {
-            const t = dn(this.opacity);
-            return `${1===t?"rgb(":"rgba("}${pn(this.r)}, ${pn(this.g)}, ${pn(this.b)}${1===t?")":`, ${t})`}`
+        function En() {
+            const t = Nn(this.opacity);
+            return `${1===t?"rgb(":"rgba("}${Sn(this.r)}, ${Sn(this.g)}, ${Sn(this.b)}${1===t?")":`, ${t})`}`
         }
 
-        function dn(t) {
+        function Nn(t) {
             return isNaN(t) ? 1 : Math.max(0, Math.min(1, t))
         }
 
-        function pn(t) {
+        function Sn(t) {
             return Math.max(0, Math.min(255, Math.round(t) || 0))
         }
 
-        function mn(t) {
-            return ((t = pn(t)) < 16 ? "0" : "") + t.toString(16)
+        function $n(t) {
+            return ((t = Sn(t)) < 16 ? "0" : "") + t.toString(16)
         }
 
-        function _n(t, e, n, r) {
-            return r <= 0 ? t = e = n = NaN : n <= 0 || n >= 1 ? t = e = NaN : e <= 0 && (t = NaN), new vn(t, e, n, r)
+        function Cn(t, e, n, r) {
+            return r <= 0 ? t = e = n = NaN : n <= 0 || n >= 1 ? t = e = NaN : e <= 0 && (t = NaN), new jn(t, e, n, r)
         }
 
-        function gn(t) {
-            if (t instanceof vn) return new vn(t.h, t.s, t.l, t.opacity);
-            if (t instanceof Re || (t = an(t)), !t) return new vn;
-            if (t instanceof vn) return t;
+        function Tn(t) {
+            if (t instanceof jn) return new jn(t.h, t.s, t.l, t.opacity);
+            if (t instanceof rn || (t = wn(t)), !t) return new jn;
+            if (t instanceof jn) return t;
             var e = (t = t.rgb()).r / 255,
                 n = t.g / 255,
                 r = t.b / 255,
                 i = Math.min(e, n, r),
                 o = Math.max(e, n, r),
                 a = NaN,
                 s = o - i,
-                u = (o + i) / 2;
-            return s ? (a = e === o ? (n - r) / s + 6 * (n < r) : n === o ? (r - e) / s + 2 : (e - n) / s + 4, s /= u < .5 ? o + i : 2 - o - i, a *= 60) : s = u > 0 && u < 1 ? 0 : a, new vn(a, s, u, t.opacity)
+                l = (o + i) / 2;
+            return s ? (a = e === o ? (n - r) / s + 6 * (n < r) : n === o ? (r - e) / s + 2 : (e - n) / s + 4, s /= l < .5 ? o + i : 2 - o - i, a *= 60) : s = l > 0 && l < 1 ? 0 : a, new jn(a, s, l, t.opacity)
         }
 
-        function vn(t, e, n, r) {
+        function jn(t, e, n, r) {
             this.h = +t, this.s = +e, this.l = +n, this.opacity = +r
         }
 
-        function yn(t) {
+        function On(t) {
             return (t = (t || 0) % 360) < 0 ? t + 360 : t
         }
 
-        function wn(t) {
+        function Pn(t) {
             return Math.max(0, Math.min(1, t || 0))
         }
 
-        function xn(t, e, n) {
+        function Vn(t, e, n) {
             return 255 * (t < 60 ? e + (n - e) * t / 60 : t < 180 ? n : t < 240 ? e + (n - e) * (240 - t) / 60 : e)
         }
 
-        function bn(t, e, n, r, i) {
+        function Ln(t, e, n, r, i) {
             var o = t * t,
                 a = o * t;
             return ((1 - 3 * t + 3 * o - a) * e + (4 - 6 * o + 3 * a) * n + (1 + 3 * t + 3 * o - 3 * a) * r + a * i) / 6
         }
-        Xe(Re, an, {
+        en(rn, wn, {
             copy(t) {
                 return Object.assign(new this.constructor, this, t)
             },
             displayable() {
                 return this.rgb().displayable()
             },
-            hex: rn,
-            formatHex: rn,
+            hex: vn,
+            formatHex: vn,
             formatHex8: function() {
                 return this.rgb().formatHex8()
             },
             formatHsl: function() {
-                return gn(this).formatHsl()
+                return Tn(this).formatHsl()
             },
-            formatRgb: on,
-            toString: on
-        }), Xe(cn, ln, ze(Re, {
+            formatRgb: yn,
+            toString: yn
+        }), en(kn, Mn, nn(rn, {
             brighter(t) {
-                return t = null == t ? Be : Math.pow(Be, t), new cn(this.r * t, this.g * t, this.b * t, this.opacity)
+                return t = null == t ? an : Math.pow(an, t), new kn(this.r * t, this.g * t, this.b * t, this.opacity)
             },
             darker(t) {
-                return t = null == t ? Ye : Math.pow(Ye, t), new cn(this.r * t, this.g * t, this.b * t, this.opacity)
+                return t = null == t ? on : Math.pow(on, t), new kn(this.r * t, this.g * t, this.b * t, this.opacity)
             },
             rgb() {
                 return this
             },
             clamp() {
-                return new cn(pn(this.r), pn(this.g), pn(this.b), dn(this.opacity))
+                return new kn(Sn(this.r), Sn(this.g), Sn(this.b), Nn(this.opacity))
             },
             displayable() {
                 return -.5 <= this.r && this.r < 255.5 && -.5 <= this.g && this.g < 255.5 && -.5 <= this.b && this.b < 255.5 && 0 <= this.opacity && this.opacity <= 1
             },
-            hex: hn,
-            formatHex: hn,
+            hex: An,
+            formatHex: An,
             formatHex8: function() {
-                return `#${mn(this.r)}${mn(this.g)}${mn(this.b)}${mn(255*(isNaN(this.opacity)?1:this.opacity))}`
+                return `#${$n(this.r)}${$n(this.g)}${$n(this.b)}${$n(255*(isNaN(this.opacity)?1:this.opacity))}`
             },
-            formatRgb: fn,
-            toString: fn
-        })), Xe(vn, (function(t, e, n, r) {
-            return 1 === arguments.length ? gn(t) : new vn(t, e, n, null == r ? 1 : r)
-        }), ze(Re, {
+            formatRgb: En,
+            toString: En
+        })), en(jn, (function(t, e, n, r) {
+            return 1 === arguments.length ? Tn(t) : new jn(t, e, n, null == r ? 1 : r)
+        }), nn(rn, {
             brighter(t) {
-                return t = null == t ? Be : Math.pow(Be, t), new vn(this.h, this.s, this.l * t, this.opacity)
+                return t = null == t ? an : Math.pow(an, t), new jn(this.h, this.s, this.l * t, this.opacity)
             },
             darker(t) {
-                return t = null == t ? Ye : Math.pow(Ye, t), new vn(this.h, this.s, this.l * t, this.opacity)
+                return t = null == t ? on : Math.pow(on, t), new jn(this.h, this.s, this.l * t, this.opacity)
             },
             rgb() {
                 var t = this.h % 360 + 360 * (this.h < 0),
                     e = isNaN(t) || isNaN(this.s) ? 0 : this.s,
                     n = this.l,
                     r = n + (n < .5 ? n : 1 - n) * e,
                     i = 2 * n - r;
-                return new cn(xn(t >= 240 ? t - 240 : t + 120, i, r), xn(t, i, r), xn(t < 120 ? t + 240 : t - 120, i, r), this.opacity)
+                return new kn(Vn(t >= 240 ? t - 240 : t + 120, i, r), Vn(t, i, r), Vn(t < 120 ? t + 240 : t - 120, i, r), this.opacity)
             },
             clamp() {
-                return new vn(yn(this.h), wn(this.s), wn(this.l), dn(this.opacity))
+                return new jn(On(this.h), Pn(this.s), Pn(this.l), Nn(this.opacity))
             },
             displayable() {
                 return (0 <= this.s && this.s <= 1 || isNaN(this.s)) && 0 <= this.l && this.l <= 1 && 0 <= this.opacity && this.opacity <= 1
             },
             formatHsl() {
-                const t = dn(this.opacity);
-                return `${1===t?"hsl(":"hsla("}${yn(this.h)}, ${100*wn(this.s)}%, ${100*wn(this.l)}%${1===t?")":`, ${t})`}`
+                const t = Nn(this.opacity);
+                return `${1===t?"hsl(":"hsla("}${On(this.h)}, ${100*Pn(this.s)}%, ${100*Pn(this.l)}%${1===t?")":`, ${t})`}`
             }
         }));
-        const Mn = t => () => t;
+        const Dn = t => () => t;
 
-        function kn(t, e) {
+        function In(t, e) {
             var n = e - t;
             return n ? function(t, e) {
                 return function(n) {
                     return t + n * e
                 }
-            }(t, n) : Mn(isNaN(t) ? e : t)
+            }(t, n) : Dn(isNaN(t) ? e : t)
         }
-        const An = function t(e) {
+        const qn = function t(e) {
             var n = function(t) {
-                return 1 == (t = +t) ? kn : function(e, n) {
+                return 1 == (t = +t) ? In : function(e, n) {
                     return n - e ? function(t, e, n) {
                         return t = Math.pow(t, n), e = Math.pow(e, n) - t, n = 1 / n,
                             function(r) {
                                 return Math.pow(t + r * e, n)
                             }
-                    }(e, n, t) : Mn(isNaN(e) ? n : e)
+                    }(e, n, t) : Dn(isNaN(e) ? n : e)
                 }
             }(e);
 
             function r(t, e) {
-                var r = n((t = ln(t)).r, (e = ln(e)).r),
+                var r = n((t = Mn(t)).r, (e = Mn(e)).r),
                     i = n(t.g, e.g),
                     o = n(t.b, e.b),
-                    a = kn(t.opacity, e.opacity);
+                    a = In(t.opacity, e.opacity);
                 return function(e) {
                     return t.r = r(e), t.g = i(e), t.b = o(e), t.opacity = a(e), t + ""
                 }
             }
             return r.gamma = t, r
         }(1);
 
-        function Nn(t) {
+        function Hn(t) {
             return function(e) {
                 var n, r, i = e.length,
                     o = new Array(i),
                     a = new Array(i),
                     s = new Array(i);
-                for (n = 0; n < i; ++n) r = ln(e[n]), o[n] = r.r || 0, a[n] = r.g || 0, s[n] = r.b || 0;
+                for (n = 0; n < i; ++n) r = Mn(e[n]), o[n] = r.r || 0, a[n] = r.g || 0, s[n] = r.b || 0;
                 return o = t(o), a = t(a), s = t(s), r.opacity = 1,
                     function(t) {
                         return r.r = o(t), r.g = a(t), r.b = s(t), r + ""
                     }
             }
         }
-        Nn((function(t) {
+        Hn((function(t) {
             var e = t.length - 1;
             return function(n) {
                 var r = n <= 0 ? n = 0 : n >= 1 ? (n = 1, e - 1) : Math.floor(n * e),
                     i = t[r],
                     o = t[r + 1],
                     a = r > 0 ? t[r - 1] : 2 * i - o,
                     s = r < e - 1 ? t[r + 2] : 2 * o - i;
-                return bn((n - r / e) * e, a, i, o, s)
+                return Ln((n - r / e) * e, a, i, o, s)
             }
-        })), Nn((function(t) {
+        })), Hn((function(t) {
             var e = t.length;
             return function(n) {
                 var r = Math.floor(((n %= 1) < 0 ? ++n : n) * e),
                     i = t[(r + e - 1) % e],
                     o = t[r % e],
                     a = t[(r + 1) % e],
                     s = t[(r + 2) % e];
-                return bn((n - r / e) * e, i, o, a, s)
+                return Ln((n - r / e) * e, i, o, a, s)
             }
         }));
-        var $n = /[-+]?(?:\d+\.?\d*|\.?\d+)(?:[eE][-+]?\d+)?/g,
-            Sn = new RegExp($n.source, "g");
+        var zn = /[-+]?(?:\d+\.?\d*|\.?\d+)(?:[eE][-+]?\d+)?/g,
+            Xn = new RegExp(zn.source, "g");
 
-        function En(t, e) {
-            var n, r, i, o = $n.lastIndex = Sn.lastIndex = 0,
+        function Rn(t, e) {
+            var n, r, i, o = zn.lastIndex = Xn.lastIndex = 0,
                 a = -1,
                 s = [],
-                u = [];
+                l = [];
             for (t += "", e += "";
-                (n = $n.exec(t)) && (r = Sn.exec(e));)(i = r.index) > o && (i = e.slice(o, i), s[a] ? s[a] += i : s[++a] = i), (n = n[0]) === (r = r[0]) ? s[a] ? s[a] += r : s[++a] = r : (s[++a] = null, u.push({
+                (n = zn.exec(t)) && (r = Xn.exec(e));)(i = r.index) > o && (i = e.slice(o, i), s[a] ? s[a] += i : s[++a] = i), (n = n[0]) === (r = r[0]) ? s[a] ? s[a] += r : s[++a] = r : (s[++a] = null, l.push({
                 i: a,
-                x: je(n, r)
-            })), o = Sn.lastIndex;
-            return o < e.length && (i = e.slice(o), s[a] ? s[a] += i : s[++a] = i), s.length < 2 ? u[0] ? function(t) {
+                x: Ye(n, r)
+            })), o = Xn.lastIndex;
+            return o < e.length && (i = e.slice(o), s[a] ? s[a] += i : s[++a] = i), s.length < 2 ? l[0] ? function(t) {
                 return function(e) {
                     return t(e) + ""
                 }
-            }(u[0].x) : function(t) {
+            }(l[0].x) : function(t) {
                 return function() {
                     return t
                 }
-            }(e) : (e = u.length, function(t) {
-                for (var n, r = 0; r < e; ++r) s[(n = u[r]).i] = n.x(t);
+            }(e) : (e = l.length, function(t) {
+                for (var n, r = 0; r < e; ++r) s[(n = l[r]).i] = n.x(t);
                 return s.join("")
             })
         }
 
-        function jn(t, e) {
+        function Yn(t, e) {
             var n;
-            return ("number" == typeof e ? je : e instanceof an ? An : (n = an(e)) ? (e = n, An) : En)(t, e)
+            return ("number" == typeof e ? Ye : e instanceof wn ? qn : (n = wn(e)) ? (e = n, qn) : Rn)(t, e)
         }
 
-        function Tn(t) {
+        function Bn(t) {
             return function() {
                 this.removeAttribute(t)
             }
         }
 
-        function Pn(t) {
+        function Fn(t) {
             return function() {
                 this.removeAttributeNS(t.space, t.local)
             }
         }
 
-        function Cn(t, e, n) {
+        function Wn(t, e, n) {
             var r, i, o = n + "";
             return function() {
                 var a = this.getAttribute(t);
                 return a === o ? null : a === r ? i : i = e(r = a, n)
             }
         }
 
-        function On(t, e, n) {
+        function Un(t, e, n) {
             var r, i, o = n + "";
             return function() {
                 var a = this.getAttributeNS(t.space, t.local);
                 return a === o ? null : a === r ? i : i = e(r = a, n)
             }
         }
 
-        function In(t, e, n) {
+        function Gn(t, e, n) {
             var r, i, o;
             return function() {
-                var a, s, u = n(this);
-                if (null != u) return (a = this.getAttribute(t)) === (s = u + "") ? null : a === r && s === i ? o : (i = s, o = e(r = a, u));
+                var a, s, l = n(this);
+                if (null != l) return (a = this.getAttribute(t)) === (s = l + "") ? null : a === r && s === i ? o : (i = s, o = e(r = a, l));
                 this.removeAttribute(t)
             }
         }
 
-        function Vn(t, e, n) {
+        function Jn(t, e, n) {
             var r, i, o;
             return function() {
-                var a, s, u = n(this);
-                if (null != u) return (a = this.getAttributeNS(t.space, t.local)) === (s = u + "") ? null : a === r && s === i ? o : (i = s, o = e(r = a, u));
+                var a, s, l = n(this);
+                if (null != l) return (a = this.getAttributeNS(t.space, t.local)) === (s = l + "") ? null : a === r && s === i ? o : (i = s, o = e(r = a, l));
                 this.removeAttributeNS(t.space, t.local)
             }
         }
 
-        function Dn(t, e) {
+        function Zn(t, e) {
             var n, r;
 
             function i() {
                 var i = e.apply(this, arguments);
                 return i !== r && (n = (r = i) && function(t, e) {
                     return function(n) {
                         this.setAttributeNS(t.space, t.local, e.call(this, n))
                     }
                 }(t, i)), n
             }
             return i._value = e, i
         }
 
-        function qn(t, e) {
+        function Kn(t, e) {
             var n, r;
 
             function i() {
                 var i = e.apply(this, arguments);
                 return i !== r && (n = (r = i) && function(t, e) {
                     return function(n) {
                         this.setAttribute(t, e.call(this, n))
                     }
                 }(t, i)), n
             }
             return i._value = e, i
         }
 
-        function Ln(t, e) {
+        function Qn(t, e) {
             return function() {
-                $e(this, t).delay = +e.apply(this, arguments)
+                ze(this, t).delay = +e.apply(this, arguments)
             }
         }
 
-        function Hn(t, e) {
+        function tr(t, e) {
             return e = +e,
                 function() {
-                    $e(this, t).delay = e
+                    ze(this, t).delay = e
                 }
         }
 
-        function Xn(t, e) {
+        function er(t, e) {
             return function() {
-                Se(this, t).duration = +e.apply(this, arguments)
+                Xe(this, t).duration = +e.apply(this, arguments)
             }
         }
 
-        function zn(t, e) {
+        function nr(t, e) {
             return e = +e,
                 function() {
-                    Se(this, t).duration = e
+                    Xe(this, t).duration = e
                 }
         }
-        var Rn = Jt.prototype.constructor;
+        var rr = ce.prototype.constructor;
 
-        function Yn(t) {
+        function ir(t) {
             return function() {
                 this.style.removeProperty(t)
             }
         }
-        var Bn = 0;
+        var or = 0;
 
-        function Wn(t, e, n, r) {
+        function ar(t, e, n, r) {
             this._groups = t, this._parents = e, this._name = n, this._id = r
         }
 
-        function Fn() {
-            return ++Bn
+        function sr() {
+            return ++or
         }
-        var Un = Jt.prototype;
-        Wn.prototype = function(t) {
-            return Jt().transition(t)
+        var lr = ce.prototype;
+        ar.prototype = function(t) {
+            return ce().transition(t)
         }.prototype = {
-            constructor: Wn,
+            constructor: ar,
             select: function(t) {
                 var e = this._name,
                     n = this._id;
-                "function" != typeof t && (t = H(t));
+                "function" != typeof t && (t = tt(t));
                 for (var r = this._groups, i = r.length, o = new Array(i), a = 0; a < i; ++a)
-                    for (var s, u, l = r[a], c = l.length, h = o[a] = new Array(c), f = 0; f < c; ++f)(s = l[f]) && (u = t.call(s, s.__data__, f, l)) && ("__data__" in s && (u.__data__ = s.__data__), h[f] = u, Ne(h[f], e, n, f, h, Ee(s, n)));
-                return new Wn(o, this._parents, e, n)
+                    for (var s, l, u = r[a], c = u.length, h = o[a] = new Array(c), f = 0; f < c; ++f)(s = u[f]) && (l = t.call(s, s.__data__, f, u)) && ("__data__" in s && (l.__data__ = s.__data__), h[f] = l, He(h[f], e, n, f, h, Re(s, n)));
+                return new ar(o, this._parents, e, n)
             },
             selectAll: function(t) {
                 var e = this._name,
                     n = this._id;
-                "function" != typeof t && (t = z(t));
+                "function" != typeof t && (t = nt(t));
                 for (var r = this._groups, i = r.length, o = [], a = [], s = 0; s < i; ++s)
-                    for (var u, l = r[s], c = l.length, h = 0; h < c; ++h)
-                        if (u = l[h]) {
-                            for (var f, d = t.call(u, u.__data__, h, l), p = Ee(u, n), m = 0, _ = d.length; m < _; ++m)(f = d[m]) && Ne(f, e, n, m, d, p);
-                            o.push(d), a.push(u)
-                        } return new Wn(o, a, e, n)
+                    for (var l, u = r[s], c = u.length, h = 0; h < c; ++h)
+                        if (l = u[h]) {
+                            for (var f, d = t.call(l, l.__data__, h, u), p = Re(l, n), m = 0, _ = d.length; m < _; ++m)(f = d[m]) && He(f, e, n, m, d, p);
+                            o.push(d), a.push(l)
+                        } return new ar(o, a, e, n)
             },
-            selectChild: Un.selectChild,
-            selectChildren: Un.selectChildren,
+            selectChild: lr.selectChild,
+            selectChildren: lr.selectChildren,
             filter: function(t) {
-                "function" != typeof t && (t = R(t));
+                "function" != typeof t && (t = rt(t));
                 for (var e = this._groups, n = e.length, r = new Array(n), i = 0; i < n; ++i)
-                    for (var o, a = e[i], s = a.length, u = r[i] = [], l = 0; l < s; ++l)(o = a[l]) && t.call(o, o.__data__, l, a) && u.push(o);
-                return new Wn(r, this._parents, this._name, this._id)
+                    for (var o, a = e[i], s = a.length, l = r[i] = [], u = 0; u < s; ++u)(o = a[u]) && t.call(o, o.__data__, u, a) && l.push(o);
+                return new ar(r, this._parents, this._name, this._id)
             },
             merge: function(t) {
                 if (t._id !== this._id) throw new Error;
                 for (var e = this._groups, n = t._groups, r = e.length, i = n.length, o = Math.min(r, i), a = new Array(r), s = 0; s < o; ++s)
-                    for (var u, l = e[s], c = n[s], h = l.length, f = a[s] = new Array(h), d = 0; d < h; ++d)(u = l[d] || c[d]) && (f[d] = u);
+                    for (var l, u = e[s], c = n[s], h = u.length, f = a[s] = new Array(h), d = 0; d < h; ++d)(l = u[d] || c[d]) && (f[d] = l);
                 for (; s < r; ++s) a[s] = e[s];
-                return new Wn(a, this._parents, this._name, this._id)
+                return new ar(a, this._parents, this._name, this._id)
             },
             selection: function() {
-                return new Rn(this._groups, this._parents)
+                return new rr(this._groups, this._parents)
             },
             transition: function() {
-                for (var t = this._name, e = this._id, n = Fn(), r = this._groups, i = r.length, o = 0; o < i; ++o)
-                    for (var a, s = r[o], u = s.length, l = 0; l < u; ++l)
-                        if (a = s[l]) {
-                            var c = Ee(a, e);
-                            Ne(a, t, n, l, s, {
+                for (var t = this._name, e = this._id, n = sr(), r = this._groups, i = r.length, o = 0; o < i; ++o)
+                    for (var a, s = r[o], l = s.length, u = 0; u < l; ++u)
+                        if (a = s[u]) {
+                            var c = Re(a, e);
+                            He(a, t, n, u, s, {
                                 time: c.time + c.delay + c.duration,
                                 delay: 0,
                                 duration: c.duration,
                                 ease: c.ease
                             })
-                        } return new Wn(r, this._parents, t, n)
+                        } return new ar(r, this._parents, t, n)
             },
-            call: Un.call,
-            nodes: Un.nodes,
-            node: Un.node,
-            size: Un.size,
-            empty: Un.empty,
-            each: Un.each,
+            call: lr.call,
+            nodes: lr.nodes,
+            node: lr.node,
+            size: lr.size,
+            empty: lr.empty,
+            each: lr.each,
             on: function(t, e) {
                 var n = this._id;
-                return arguments.length < 2 ? Ee(this.node(), n).on.on(t) : this.each(function(t, e, n) {
+                return arguments.length < 2 ? Re(this.node(), n).on.on(t) : this.each(function(t, e, n) {
                     var r, i, o = function(t) {
                         return (t + "").trim().split(/^|\s+/).every((function(t) {
                             var e = t.indexOf(".");
                             return e >= 0 && (t = t.slice(0, e)), !t || "start" === t
                         }))
-                    }(e) ? $e : Se;
+                    }(e) ? ze : Xe;
                     return function() {
                         var a = o(this, t),
                             s = a.on;
                         s !== r && (i = (r = s).copy()).on(e, n), a.on = i
                     }
                 }(n, t, e))
             },
             attr: function(t, e) {
-                var n = it(t),
-                    r = "transform" === n ? De : jn;
-                return this.attrTween(t, "function" == typeof e ? (n.local ? Vn : In)(n, r, He(this, "attr." + t, e)) : null == e ? (n.local ? Pn : Tn)(n) : (n.local ? On : Cn)(n, r, e))
+                var n = vt(t),
+                    r = "transform" === n ? Ze : Yn;
+                return this.attrTween(t, "function" == typeof e ? (n.local ? Jn : Gn)(n, r, tn(this, "attr." + t, e)) : null == e ? (n.local ? Fn : Bn)(n) : (n.local ? Un : Wn)(n, r, e))
             },
             attrTween: function(t, e) {
                 var n = "attr." + t;
                 if (arguments.length < 2) return (n = this.tween(n)) && n._value;
                 if (null == e) return this.tween(n, null);
                 if ("function" != typeof e) throw new Error;
-                var r = it(t);
-                return this.tween(n, (r.local ? Dn : qn)(r, e))
+                var r = vt(t);
+                return this.tween(n, (r.local ? Zn : Kn)(r, e))
             },
             style: function(t, e, n) {
-                var r = "transform" == (t += "") ? Ve : jn;
+                var r = "transform" == (t += "") ? Je : Yn;
                 return null == e ? this.styleTween(t, function(t, e) {
                     var n, r, i;
                     return function() {
-                        var o = mt(this, t),
-                            a = (this.style.removeProperty(t), mt(this, t));
+                        var o = $t(this, t),
+                            a = (this.style.removeProperty(t), $t(this, t));
                         return o === a ? null : o === n && a === r ? i : i = e(n = o, r = a)
                     }
-                }(t, r)).on("end.style." + t, Yn(t)) : "function" == typeof e ? this.styleTween(t, function(t, e, n) {
+                }(t, r)).on("end.style." + t, ir(t)) : "function" == typeof e ? this.styleTween(t, function(t, e, n) {
                     var r, i, o;
                     return function() {
-                        var a = mt(this, t),
+                        var a = $t(this, t),
                             s = n(this),
-                            u = s + "";
-                        return null == s && (this.style.removeProperty(t), u = s = mt(this, t)), a === u ? null : a === r && u === i ? o : (i = u, o = e(r = a, s))
+                            l = s + "";
+                        return null == s && (this.style.removeProperty(t), l = s = $t(this, t)), a === l ? null : a === r && l === i ? o : (i = l, o = e(r = a, s))
                     }
-                }(t, r, He(this, "style." + t, e))).each(function(t, e) {
+                }(t, r, tn(this, "style." + t, e))).each(function(t, e) {
                     var n, r, i, o, a = "style." + e,
                         s = "end." + a;
                     return function() {
-                        var u = Se(this, t),
-                            l = u.on,
-                            c = null == u.value[a] ? o || (o = Yn(e)) : void 0;
-                        l === n && i === c || (r = (n = l).copy()).on(s, i = c), u.on = r
+                        var l = Xe(this, t),
+                            u = l.on,
+                            c = null == l.value[a] ? o || (o = ir(e)) : void 0;
+                        u === n && i === c || (r = (n = u).copy()).on(s, i = c), l.on = r
                     }
                 }(this._id, t)) : this.styleTween(t, function(t, e, n) {
                     var r, i, o = n + "";
                     return function() {
-                        var a = mt(this, t);
+                        var a = $t(this, t);
                         return a === o ? null : a === r ? i : i = e(r = a, n)
                     }
                 }(t, r, e), n).on("end.style." + t, null)
             },
             styleTween: function(t, e, n) {
                 var r = "style." + (t += "");
                 if (arguments.length < 2) return (r = this.tween(r)) && r._value;
@@ -2183,15 +2200,15 @@
             },
             text: function(t) {
                 return this.tween("text", "function" == typeof t ? function(t) {
                     return function() {
                         var e = t(this);
                         this.textContent = null == e ? "" : e
                     }
-                }(He(this, "text", t)) : function(t) {
+                }(tn(this, "text", t)) : function(t) {
                     return function() {
                         this.textContent = t
                     }
                 }(null == t ? "" : t + ""))
             },
             textTween: function(t) {
                 var e = "text";
@@ -2221,122 +2238,122 @@
                         e && e.removeChild(this)
                     }
                 }(this._id))
             },
             tween: function(t, e) {
                 var n = this._id;
                 if (t += "", arguments.length < 2) {
-                    for (var r, i = Ee(this.node(), n).tween, o = 0, a = i.length; o < a; ++o)
+                    for (var r, i = Re(this.node(), n).tween, o = 0, a = i.length; o < a; ++o)
                         if ((r = i[o]).name === t) return r.value;
                     return null
                 }
-                return this.each((null == e ? qe : Le)(n, t, e))
+                return this.each((null == e ? Ke : Qe)(n, t, e))
             },
             delay: function(t) {
                 var e = this._id;
-                return arguments.length ? this.each(("function" == typeof t ? Ln : Hn)(e, t)) : Ee(this.node(), e).delay
+                return arguments.length ? this.each(("function" == typeof t ? Qn : tr)(e, t)) : Re(this.node(), e).delay
             },
             duration: function(t) {
                 var e = this._id;
-                return arguments.length ? this.each(("function" == typeof t ? Xn : zn)(e, t)) : Ee(this.node(), e).duration
+                return arguments.length ? this.each(("function" == typeof t ? er : nr)(e, t)) : Re(this.node(), e).duration
             },
             ease: function(t) {
                 var e = this._id;
                 return arguments.length ? this.each(function(t, e) {
                     if ("function" != typeof e) throw new Error;
                     return function() {
-                        Se(this, t).ease = e
+                        Xe(this, t).ease = e
                     }
-                }(e, t)) : Ee(this.node(), e).ease
+                }(e, t)) : Re(this.node(), e).ease
             },
             easeVarying: function(t) {
                 if ("function" != typeof t) throw new Error;
                 return this.each(function(t, e) {
                     return function() {
                         var n = e.apply(this, arguments);
                         if ("function" != typeof n) throw new Error;
-                        Se(this, t).ease = n
+                        Xe(this, t).ease = n
                     }
                 }(this._id, t))
             },
             end: function() {
                 var t, e, n = this,
                     r = n._id,
                     i = n.size();
                 return new Promise((function(o, a) {
                     var s = {
                             value: a
                         },
-                        u = {
+                        l = {
                             value: function() {
                                 0 == --i && o()
                             }
                         };
                     n.each((function() {
-                        var n = Se(this, r),
+                        var n = Xe(this, r),
                             i = n.on;
-                        i !== t && ((e = (t = i).copy())._.cancel.push(s), e._.interrupt.push(s), e._.end.push(u)), n.on = e
+                        i !== t && ((e = (t = i).copy())._.cancel.push(s), e._.interrupt.push(s), e._.end.push(l)), n.on = e
                     })), 0 === i && o()
                 }))
             },
-            [Symbol.iterator]: Un[Symbol.iterator]
+            [Symbol.iterator]: lr[Symbol.iterator]
         };
-        var Gn = {
+        var ur = {
             time: null,
             delay: 0,
             duration: 250,
             ease: function(t) {
                 return ((t *= 2) <= 1 ? t * t * t : (t -= 2) * t * t + 2) / 2
             }
         };
 
-        function Jn(t, e) {
+        function cr(t, e) {
             for (var n; !(n = t.__transition) || !(n = n[e]);)
                 if (!(t = t.parentNode)) throw new Error(`transition ${e} not found`);
             return n
         }
-        Jt.prototype.interrupt = function(t) {
+        ce.prototype.interrupt = function(t) {
             return this.each((function() {
                 ! function(t, e) {
                     var n, r, i, o = t.__transition,
                         a = !0;
                     if (o) {
                         for (i in e = null == e ? null : e + "", o)(n = o[i]).name === e ? (r = n.state > 2 && n.state < 5, n.state = 6, n.timer.stop(), n.on.call(r ? "interrupt" : "cancel", t, t.__data__, n.index, n.group), delete o[i]) : a = !1;
                         a && delete t.__transition
                     }
                 }(this, t)
             }))
-        }, Jt.prototype.transition = function(t) {
+        }, ce.prototype.transition = function(t) {
             var e, n;
-            t instanceof Wn ? (e = t._id, t = t._name) : (e = Fn(), (n = Gn).time = pe(), t = null == t ? null : t + "");
+            t instanceof ar ? (e = t._id, t = t._name) : (e = sr(), (n = ur).time = Se(), t = null == t ? null : t + "");
             for (var r = this._groups, i = r.length, o = 0; o < i; ++o)
-                for (var a, s = r[o], u = s.length, l = 0; l < u; ++l)(a = s[l]) && Ne(a, t, e, l, s, n || Jn(a, e));
-            return new Wn(r, this._parents, t, e)
+                for (var a, s = r[o], l = s.length, u = 0; u < l; ++u)(a = s[u]) && He(a, t, e, u, s, n || cr(a, e));
+            return new ar(r, this._parents, t, e)
         };
         const {
-            abs: Kn,
-            max: Zn,
-            min: Qn
+            abs: hr,
+            max: fr,
+            min: dr
         } = Math;
 
-        function tr(t) {
+        function pr(t) {
             return {
                 type: t
             }
         }
 
-        function er(t) {
-            return "string" == typeof t ? new Ut([
+        function mr(t) {
+            return "string" == typeof t ? new le([
                 [document.querySelector(t)]
-            ], [document.documentElement]) : new Ut([
+            ], [document.documentElement]) : new le([
                 [t]
-            ], Ft)
+            ], se)
         }
 
-        function nr(t, e) {
+        function _r(t, e) {
             if (t = function(t) {
                     let e;
                     for (; e = t.sourceEvent;) t = e;
                     return t
                 }(t), void 0 === e && (e = t.currentTarget), e) {
                 var n = e.ownerSVGElement || e;
                 if (n.createSVGPoint) {
@@ -2345,42 +2362,42 @@
                 }
                 if (e.getBoundingClientRect) {
                     var i = e.getBoundingClientRect();
                     return [t.clientX - i.left - e.clientLeft, t.clientY - i.top - e.clientTop]
                 }
             }
             return [t.pageX, t.pageY]
-        } ["w", "e"].map(tr), ["n", "s"].map(tr), ["n", "w", "e", "s", "nw", "ne", "sw", "se"].map(tr);
-        const rr = {
+        } ["w", "e"].map(pr), ["n", "s"].map(pr), ["n", "w", "e", "s", "nw", "ne", "sw", "se"].map(pr);
+        const gr = {
                 passive: !1
             },
-            ir = {
+            vr = {
                 capture: !0,
                 passive: !1
             };
 
-        function or(t) {
+        function yr(t) {
             t.stopImmediatePropagation()
         }
 
-        function ar(t) {
+        function wr(t) {
             t.preventDefault(), t.stopImmediatePropagation()
         }
-        const sr = t => () => t;
+        const xr = t => () => t;
 
-        function ur(t, {
+        function br(t, {
             sourceEvent: e,
             subject: n,
             target: r,
             identifier: i,
             active: o,
             x: a,
             y: s,
-            dx: u,
-            dy: l,
+            dx: l,
+            dy: u,
             dispatch: c
         }) {
             Object.defineProperties(this, {
                 type: {
                     value: t,
                     enumerable: !0,
                     configurable: !0
@@ -2417,81 +2434,81 @@
                 },
                 y: {
                     value: s,
                     enumerable: !0,
                     configurable: !0
                 },
                 dx: {
-                    value: u,
+                    value: l,
                     enumerable: !0,
                     configurable: !0
                 },
                 dy: {
-                    value: l,
+                    value: u,
                     enumerable: !0,
                     configurable: !0
                 },
                 _: {
                     value: c
                 }
             })
         }
 
-        function lr(t) {
+        function Mr(t) {
             return !t.ctrlKey && !t.button
         }
 
-        function cr() {
+        function kr() {
             return this.parentNode
         }
 
-        function hr(t, e) {
+        function Ar(t, e) {
             return null == e ? {
                 x: t.x,
                 y: t.y
             } : e
         }
 
-        function fr() {
+        function Er() {
             return navigator.maxTouchPoints || "ontouchstart" in this
         }
 
-        function dr(t, e) {
+        function Nr(t, e) {
             switch (arguments.length) {
                 case 0:
                     break;
                 case 1:
                     this.range(t);
                     break;
                 default:
                     this.range(e).domain(t)
             }
             return this
         }
-        ur.prototype.on = function() {
+        br.prototype.on = function() {
             var t = this._.on.apply(this._, arguments);
             return t === this._ ? this : t
         };
-        class pr extends Map {
-            constructor(t, e = _r) {
+        class Sr extends Map {
+            constructor(t, e = Cr) {
                 if (super(), Object.defineProperties(this, {
                         _intern: {
                             value: new Map
                         },
                         _key: {
                             value: e
                         }
                     }), null != t)
                     for (const [e, n] of t) this.set(e, n)
             }
             get(t) {
-                return super.get(mr(this, t))
+                return super.get($r(this, t))
             }
             has(t) {
-                return super.has(mr(this, t))
+                return super.has($r(this, t))
             }
             set(t, e) {
                 return super.set(function({
                     _intern: t,
                     _key: e
                 }, n) {
                     const r = e(n);
@@ -2505,73 +2522,73 @@
                 }, n) {
                     const r = e(n);
                     return t.has(r) && (n = t.get(r), t.delete(r)), n
                 }(this, t))
             }
         }
 
-        function mr({
+        function $r({
             _intern: t,
             _key: e
         }, n) {
             const r = e(n);
             return t.has(r) ? t.get(r) : n
         }
 
-        function _r(t) {
+        function Cr(t) {
             return null !== t && "object" == typeof t ? t.valueOf() : t
         }
         Set;
-        const gr = Symbol("implicit");
+        const Tr = Symbol("implicit");
 
-        function vr() {
-            var t = new pr,
+        function jr() {
+            var t = new Sr,
                 e = [],
                 n = [],
-                r = gr;
+                r = Tr;
 
             function i(i) {
                 let o = t.get(i);
                 if (void 0 === o) {
-                    if (r !== gr) return r;
+                    if (r !== Tr) return r;
                     t.set(i, o = e.push(i) - 1)
                 }
                 return n[o % n.length]
             }
             return i.domain = function(n) {
                 if (!arguments.length) return e.slice();
-                e = [], t = new pr;
+                e = [], t = new Sr;
                 for (const r of n) t.has(r) || t.set(r, e.push(r) - 1);
                 return i
             }, i.range = function(t) {
                 return arguments.length ? (n = Array.from(t), i) : n.slice()
             }, i.unknown = function(t) {
                 return arguments.length ? (r = t, i) : r
             }, i.copy = function() {
-                return vr(e, n).unknown(r)
-            }, dr.apply(i, arguments), i
+                return jr(e, n).unknown(r)
+            }, Nr.apply(i, arguments), i
         }
 
-        function yr() {
-            var t, e, n = vr().unknown(void 0),
+        function Or() {
+            var t, e, n = jr().unknown(void 0),
                 r = n.domain,
                 i = n.range,
                 o = 0,
                 a = 1,
                 s = !1,
-                u = 0,
                 l = 0,
+                u = 0,
                 c = .5;
 
             function h() {
                 var n = r().length,
                     h = a < o,
                     f = h ? a : o,
                     d = h ? o : a;
-                t = (d - f) / Math.max(1, n - u + 2 * l), s && (t = Math.floor(t)), f += (d - f - t * (n - u)) * c, e = t * (1 - u), s && (f = Math.round(f), e = Math.round(e));
+                t = (d - f) / Math.max(1, n - l + 2 * u), s && (t = Math.floor(t)), f += (d - f - t * (n - l)) * c, e = t * (1 - l), s && (f = Math.round(f), e = Math.round(e));
                 var p = function(t, e, n) {
                     t = +t, e = +e, n = (i = arguments.length) < 2 ? (e = t, t = 0, 1) : i < 3 ? 1 : +n;
                     for (var r = -1, i = 0 | Math.max(0, Math.ceil((e - t) / n)), o = new Array(i); ++r < i;) o[r] = t + r * n;
                     return o
                 }(n).map((function(e) {
                     return f + t * e
                 }));
@@ -2586,330 +2603,330 @@
             }, n.bandwidth = function() {
                 return e
             }, n.step = function() {
                 return t
             }, n.round = function(t) {
                 return arguments.length ? (s = !!t, h()) : s
             }, n.padding = function(t) {
-                return arguments.length ? (u = Math.min(1, l = +t), h()) : u
+                return arguments.length ? (l = Math.min(1, u = +t), h()) : l
             }, n.paddingInner = function(t) {
-                return arguments.length ? (u = Math.min(1, t), h()) : u
+                return arguments.length ? (l = Math.min(1, t), h()) : l
             }, n.paddingOuter = function(t) {
-                return arguments.length ? (l = +t, h()) : l
+                return arguments.length ? (u = +t, h()) : u
             }, n.align = function(t) {
                 return arguments.length ? (c = Math.max(0, Math.min(1, t)), h()) : c
             }, n.copy = function() {
-                return yr(r(), [o, a]).round(s).paddingInner(u).paddingOuter(l).align(c)
-            }, dr.apply(h(), arguments)
+                return Or(r(), [o, a]).round(s).paddingInner(l).paddingOuter(u).align(c)
+            }, Nr.apply(h(), arguments)
         }
 
-        function wr(t, e) {
+        function Pr(t, e) {
             var n, r = e ? e.length : 0,
                 i = t ? Math.min(r, t.length) : 0,
                 o = new Array(i),
                 a = new Array(r);
-            for (n = 0; n < i; ++n) o[n] = kr(t[n], e[n]);
+            for (n = 0; n < i; ++n) o[n] = Ir(t[n], e[n]);
             for (; n < r; ++n) a[n] = e[n];
             return function(t) {
                 for (n = 0; n < i; ++n) a[n] = o[n](t);
                 return a
             }
         }
 
-        function xr(t, e) {
+        function Vr(t, e) {
             var n = new Date;
             return t = +t, e = +e,
                 function(r) {
                     return n.setTime(t * (1 - r) + e * r), n
                 }
         }
 
-        function br(t, e) {
+        function Lr(t, e) {
             var n, r = {},
                 i = {};
-            for (n in null !== t && "object" == typeof t || (t = {}), null !== e && "object" == typeof e || (e = {}), e) n in t ? r[n] = kr(t[n], e[n]) : i[n] = e[n];
+            for (n in null !== t && "object" == typeof t || (t = {}), null !== e && "object" == typeof e || (e = {}), e) n in t ? r[n] = Ir(t[n], e[n]) : i[n] = e[n];
             return function(t) {
                 for (n in r) i[n] = r[n](t);
                 return i
             }
         }
 
-        function Mr(t, e) {
+        function Dr(t, e) {
             e || (e = []);
             var n, r = t ? Math.min(e.length, t.length) : 0,
                 i = e.slice();
             return function(o) {
                 for (n = 0; n < r; ++n) i[n] = t[n] * (1 - o) + e[n] * o;
                 return i
             }
         }
 
-        function kr(t, e) {
+        function Ir(t, e) {
             var n, r, i = typeof e;
-            return null == e || "boolean" === i ? Mn(e) : ("number" === i ? je : "string" === i ? (n = an(e)) ? (e = n, An) : En : e instanceof an ? An : e instanceof Date ? xr : (r = e, !ArrayBuffer.isView(r) || r instanceof DataView ? Array.isArray(e) ? wr : "function" != typeof e.valueOf && "function" != typeof e.toString || isNaN(e) ? br : je : Mr))(t, e)
+            return null == e || "boolean" === i ? Dn(e) : ("number" === i ? Ye : "string" === i ? (n = wn(e)) ? (e = n, qn) : Rn : e instanceof wn ? qn : e instanceof Date ? Vr : (r = e, !ArrayBuffer.isView(r) || r instanceof DataView ? Array.isArray(e) ? Pr : "function" != typeof e.valueOf && "function" != typeof e.toString || isNaN(e) ? Lr : Ye : Dr))(t, e)
         }
 
-        function Ar(t, e) {
+        function qr(t, e) {
             return t = +t, e = +e,
                 function(n) {
                     return Math.round(t * (1 - n) + e * n)
                 }
         }
 
-        function Nr(t) {
+        function Hr(t) {
             return +t
         }
-        var $r = [0, 1];
+        var zr = [0, 1];
 
-        function Sr(t) {
+        function Xr(t) {
             return t
         }
 
-        function Er(t, e) {
+        function Rr(t, e) {
             return (e -= t = +t) ? function(n) {
                 return (n - t) / e
             } : (n = isNaN(e) ? NaN : .5, function() {
                 return n
             });
             var n
         }
 
-        function jr(t, e, n) {
+        function Yr(t, e, n) {
             var r = t[0],
                 i = t[1],
                 o = e[0],
                 a = e[1];
-            return i < r ? (r = Er(i, r), o = n(a, o)) : (r = Er(r, i), o = n(o, a)),
+            return i < r ? (r = Rr(i, r), o = n(a, o)) : (r = Rr(r, i), o = n(o, a)),
                 function(t) {
                     return o(r(t))
                 }
         }
 
-        function Tr(t, e, n) {
+        function Br(t, e, n) {
             var r = Math.min(t.length, e.length) - 1,
                 i = new Array(r),
                 o = new Array(r),
                 a = -1;
-            for (t[r] < t[0] && (t = t.slice().reverse(), e = e.slice().reverse()); ++a < r;) i[a] = Er(t[a], t[a + 1]), o[a] = n(e[a], e[a + 1]);
+            for (t[r] < t[0] && (t = t.slice().reverse(), e = e.slice().reverse()); ++a < r;) i[a] = Rr(t[a], t[a + 1]), o[a] = n(e[a], e[a + 1]);
             return function(e) {
-                var n = f(t, e, 1, r) - 1;
+                var n = E(t, e, 1, r) - 1;
                 return o[n](i[n](e))
             }
         }
-        var Pr, Cr = /^(?:(.)?([<>=^]))?([+\-( ])?([$#])?(0)?(\d+)?(,)?(\.\d+)?(~)?([a-z%])?$/i;
+        var Fr, Wr = /^(?:(.)?([<>=^]))?([+\-( ])?([$#])?(0)?(\d+)?(,)?(\.\d+)?(~)?([a-z%])?$/i;
 
-        function Or(t) {
-            if (!(e = Cr.exec(t))) throw new Error("invalid format: " + t);
+        function Ur(t) {
+            if (!(e = Wr.exec(t))) throw new Error("invalid format: " + t);
             var e;
-            return new Ir({
+            return new Gr({
                 fill: e[1],
                 align: e[2],
                 sign: e[3],
                 symbol: e[4],
                 zero: e[5],
                 width: e[6],
                 comma: e[7],
                 precision: e[8] && e[8].slice(1),
                 trim: e[9],
                 type: e[10]
             })
         }
 
-        function Ir(t) {
+        function Gr(t) {
             this.fill = void 0 === t.fill ? " " : t.fill + "", this.align = void 0 === t.align ? ">" : t.align + "", this.sign = void 0 === t.sign ? "-" : t.sign + "", this.symbol = void 0 === t.symbol ? "" : t.symbol + "", this.zero = !!t.zero, this.width = void 0 === t.width ? void 0 : +t.width, this.comma = !!t.comma, this.precision = void 0 === t.precision ? void 0 : +t.precision, this.trim = !!t.trim, this.type = void 0 === t.type ? "" : t.type + ""
         }
 
-        function Vr(t, e) {
+        function Jr(t, e) {
             if ((n = (t = e ? t.toExponential(e - 1) : t.toExponential()).indexOf("e")) < 0) return null;
             var n, r = t.slice(0, n);
             return [r.length > 1 ? r[0] + r.slice(2) : r, +t.slice(n + 1)]
         }
 
-        function Dr(t) {
-            return (t = Vr(Math.abs(t))) ? t[1] : NaN
+        function Zr(t) {
+            return (t = Jr(Math.abs(t))) ? t[1] : NaN
         }
 
-        function qr(t, e) {
-            var n = Vr(t, e);
+        function Kr(t, e) {
+            var n = Jr(t, e);
             if (!n) return t + "";
             var r = n[0],
                 i = n[1];
             return i < 0 ? "0." + new Array(-i).join("0") + r : r.length > i + 1 ? r.slice(0, i + 1) + "." + r.slice(i + 1) : r + new Array(i - r.length + 2).join("0")
         }
-        Or.prototype = Ir.prototype, Ir.prototype.toString = function() {
+        Ur.prototype = Gr.prototype, Gr.prototype.toString = function() {
             return this.fill + this.align + this.sign + this.symbol + (this.zero ? "0" : "") + (void 0 === this.width ? "" : Math.max(1, 0 | this.width)) + (this.comma ? "," : "") + (void 0 === this.precision ? "" : "." + Math.max(0, 0 | this.precision)) + (this.trim ? "~" : "") + this.type
         };
-        const Lr = {
+        const Qr = {
             "%": (t, e) => (100 * t).toFixed(e),
             b: t => Math.round(t).toString(2),
             c: t => t + "",
             d: function(t) {
                 return Math.abs(t = Math.round(t)) >= 1e21 ? t.toLocaleString("en").replace(/,/g, "") : t.toString(10)
             },
             e: (t, e) => t.toExponential(e),
             f: (t, e) => t.toFixed(e),
             g: (t, e) => t.toPrecision(e),
             o: t => Math.round(t).toString(8),
-            p: (t, e) => qr(100 * t, e),
-            r: qr,
+            p: (t, e) => Kr(100 * t, e),
+            r: Kr,
             s: function(t, e) {
-                var n = Vr(t, e);
+                var n = Jr(t, e);
                 if (!n) return t + "";
                 var r = n[0],
                     i = n[1],
-                    o = i - (Pr = 3 * Math.max(-8, Math.min(8, Math.floor(i / 3)))) + 1,
+                    o = i - (Fr = 3 * Math.max(-8, Math.min(8, Math.floor(i / 3)))) + 1,
                     a = r.length;
-                return o === a ? r : o > a ? r + new Array(o - a + 1).join("0") : o > 0 ? r.slice(0, o) + "." + r.slice(o) : "0." + new Array(1 - o).join("0") + Vr(t, Math.max(0, e + o - 1))[0]
+                return o === a ? r : o > a ? r + new Array(o - a + 1).join("0") : o > 0 ? r.slice(0, o) + "." + r.slice(o) : "0." + new Array(1 - o).join("0") + Jr(t, Math.max(0, e + o - 1))[0]
             },
             X: t => Math.round(t).toString(16).toUpperCase(),
             x: t => Math.round(t).toString(16)
         };
 
-        function Hr(t) {
+        function ti(t) {
             return t
         }
-        var Xr, zr, Rr, Yr = Array.prototype.map,
-            Br = ["y", "z", "a", "f", "p", "n", "µ", "m", "", "k", "M", "G", "T", "P", "E", "Z", "Y"];
+        var ei, ni, ri, ii = Array.prototype.map,
+            oi = ["y", "z", "a", "f", "p", "n", "µ", "m", "", "k", "M", "G", "T", "P", "E", "Z", "Y"];
 
-        function Wr() {
+        function ai() {
             var t = function() {
-                var t, e, n, r, i, o, a = $r,
-                    s = $r,
-                    u = kr,
-                    l = Sr;
+                var t, e, n, r, i, o, a = zr,
+                    s = zr,
+                    l = Ir,
+                    u = Xr;
 
                 function c() {
-                    var t, e, n, u = Math.min(a.length, s.length);
-                    return l !== Sr && (t = a[0], e = a[u - 1], t > e && (n = t, t = e, e = n), l = function(n) {
+                    var t, e, n, l = Math.min(a.length, s.length);
+                    return u !== Xr && (t = a[0], e = a[l - 1], t > e && (n = t, t = e, e = n), u = function(n) {
                         return Math.max(t, Math.min(e, n))
-                    }), r = u > 2 ? Tr : jr, i = o = null, h
+                    }), r = l > 2 ? Br : Yr, i = o = null, h
                 }
 
                 function h(e) {
-                    return null == e || isNaN(e = +e) ? n : (i || (i = r(a.map(t), s, u)))(t(l(e)))
+                    return null == e || isNaN(e = +e) ? n : (i || (i = r(a.map(t), s, l)))(t(u(e)))
                 }
                 return h.invert = function(n) {
-                        return l(e((o || (o = r(s, a.map(t), je)))(n)))
+                        return u(e((o || (o = r(s, a.map(t), Ye)))(n)))
                     }, h.domain = function(t) {
-                        return arguments.length ? (a = Array.from(t, Nr), c()) : a.slice()
+                        return arguments.length ? (a = Array.from(t, Hr), c()) : a.slice()
                     }, h.range = function(t) {
                         return arguments.length ? (s = Array.from(t), c()) : s.slice()
                     }, h.rangeRound = function(t) {
-                        return s = Array.from(t), u = Ar, c()
+                        return s = Array.from(t), l = qr, c()
                     }, h.clamp = function(t) {
-                        return arguments.length ? (l = !!t || Sr, c()) : l !== Sr
+                        return arguments.length ? (u = !!t || Xr, c()) : u !== Xr
                     }, h.interpolate = function(t) {
-                        return arguments.length ? (u = t, c()) : u
+                        return arguments.length ? (l = t, c()) : l
                     }, h.unknown = function(t) {
                         return arguments.length ? (n = t, h) : n
                     },
                     function(n, r) {
                         return t = n, e = r, c()
                     }
-            }()(Sr, Sr);
+            }()(Xr, Xr);
             return t.copy = function() {
-                    return e = t, Wr().domain(e.domain()).range(e.range()).interpolate(e.interpolate()).clamp(e.clamp()).unknown(e.unknown());
+                    return e = t, ai().domain(e.domain()).range(e.range()).interpolate(e.interpolate()).clamp(e.clamp()).unknown(e.unknown());
                     var e
-                }, dr.apply(t, arguments),
+                }, Nr.apply(t, arguments),
                 function(t) {
                     var e = t.domain;
                     return t.ticks = function(t) {
                         var n = e();
-                        return y(n[0], n[n.length - 1], null == t ? 10 : t)
+                        return O(n[0], n[n.length - 1], null == t ? 10 : t)
                     }, t.tickFormat = function(t, n) {
                         var r = e();
                         return function(t, e, n, r) {
                             var i, o = function(t, e, n) {
                                 n = +n;
                                 const r = (e = +e) < (t = +t),
-                                    i = r ? w(e, t, n) : w(t, e, n);
+                                    i = r ? P(e, t, n) : P(t, e, n);
                                 return (r ? -1 : 1) * (i < 0 ? 1 / -i : i)
                             }(t, e, n);
-                            switch ((r = Or(null == r ? ",f" : r)).type) {
+                            switch ((r = Ur(null == r ? ",f" : r)).type) {
                                 case "s":
                                     var a = Math.max(Math.abs(t), Math.abs(e));
                                     return null != r.precision || isNaN(i = function(t, e) {
-                                        return Math.max(0, 3 * Math.max(-8, Math.min(8, Math.floor(Dr(e) / 3))) - Dr(Math.abs(t)))
-                                    }(o, a)) || (r.precision = i), Rr(r, a);
+                                        return Math.max(0, 3 * Math.max(-8, Math.min(8, Math.floor(Zr(e) / 3))) - Zr(Math.abs(t)))
+                                    }(o, a)) || (r.precision = i), ri(r, a);
                                 case "":
                                 case "e":
                                 case "g":
                                 case "p":
                                 case "r":
                                     null != r.precision || isNaN(i = function(t, e) {
-                                        return t = Math.abs(t), e = Math.abs(e) - t, Math.max(0, Dr(e) - Dr(t)) + 1
+                                        return t = Math.abs(t), e = Math.abs(e) - t, Math.max(0, Zr(e) - Zr(t)) + 1
                                     }(o, Math.max(Math.abs(t), Math.abs(e)))) || (r.precision = i - ("e" === r.type));
                                     break;
                                 case "f":
                                 case "%":
                                     null != r.precision || isNaN(i = function(t) {
-                                        return Math.max(0, -Dr(Math.abs(t)))
+                                        return Math.max(0, -Zr(Math.abs(t)))
                                     }(o)) || (r.precision = i - 2 * ("%" === r.type))
                             }
-                            return zr(r)
+                            return ni(r)
                         }(r[0], r[r.length - 1], null == t ? 10 : t, n)
                     }, t.nice = function(n) {
                         null == n && (n = 10);
                         var r, i, o = e(),
                             a = 0,
                             s = o.length - 1,
-                            u = o[a],
-                            l = o[s],
+                            l = o[a],
+                            u = o[s],
                             c = 10;
-                        for (l < u && (i = u, u = l, l = i, i = a, a = s, s = i); c-- > 0;) {
-                            if ((i = w(u, l, n)) === r) return o[a] = u, o[s] = l, e(o);
-                            if (i > 0) u = Math.floor(u / i) * i, l = Math.ceil(l / i) * i;
+                        for (u < l && (i = l, l = u, u = i, i = a, a = s, s = i); c-- > 0;) {
+                            if ((i = P(l, u, n)) === r) return o[a] = l, o[s] = u, e(o);
+                            if (i > 0) l = Math.floor(l / i) * i, u = Math.ceil(u / i) * i;
                             else {
                                 if (!(i < 0)) break;
-                                u = Math.ceil(u * i) / i, l = Math.floor(l * i) / i
+                                l = Math.ceil(l * i) / i, u = Math.floor(u * i) / i
                             }
                             r = i
                         }
                         return t
                     }, t
                 }(t)
         }
-        Xr = function(t) {
-            var e, n, r = void 0 === t.grouping || void 0 === t.thousands ? Hr : (e = Yr.call(t.grouping, Number), n = t.thousands + "", function(t, r) {
-                    for (var i = t.length, o = [], a = 0, s = e[0], u = 0; i > 0 && s > 0 && (u + s + 1 > r && (s = Math.max(1, r - u)), o.push(t.substring(i -= s, i + s)), !((u += s + 1) > r));) s = e[a = (a + 1) % e.length];
+        ei = function(t) {
+            var e, n, r = void 0 === t.grouping || void 0 === t.thousands ? ti : (e = ii.call(t.grouping, Number), n = t.thousands + "", function(t, r) {
+                    for (var i = t.length, o = [], a = 0, s = e[0], l = 0; i > 0 && s > 0 && (l + s + 1 > r && (s = Math.max(1, r - l)), o.push(t.substring(i -= s, i + s)), !((l += s + 1) > r));) s = e[a = (a + 1) % e.length];
                     return o.reverse().join(n)
                 }),
                 i = void 0 === t.currency ? "" : t.currency[0] + "",
                 o = void 0 === t.currency ? "" : t.currency[1] + "",
                 a = void 0 === t.decimal ? "." : t.decimal + "",
-                s = void 0 === t.numerals ? Hr : function(t) {
+                s = void 0 === t.numerals ? ti : function(t) {
                     return function(e) {
                         return e.replace(/[0-9]/g, (function(e) {
                             return t[+e]
                         }))
                     }
-                }(Yr.call(t.numerals, String)),
-                u = void 0 === t.percent ? "%" : t.percent + "",
-                l = void 0 === t.minus ? "−" : t.minus + "",
+                }(ii.call(t.numerals, String)),
+                l = void 0 === t.percent ? "%" : t.percent + "",
+                u = void 0 === t.minus ? "−" : t.minus + "",
                 c = void 0 === t.nan ? "NaN" : t.nan + "";
 
             function h(t) {
-                var e = (t = Or(t)).fill,
+                var e = (t = Ur(t)).fill,
                     n = t.align,
                     h = t.sign,
                     f = t.symbol,
                     d = t.zero,
                     p = t.width,
                     m = t.comma,
                     _ = t.precision,
                     g = t.trim,
                     v = t.type;
-                "n" === v ? (m = !0, v = "g") : Lr[v] || (void 0 === _ && (_ = 12), g = !0, v = "g"), (d || "0" === e && "=" === n) && (d = !0, e = "0", n = "=");
+                "n" === v ? (m = !0, v = "g") : Qr[v] || (void 0 === _ && (_ = 12), g = !0, v = "g"), (d || "0" === e && "=" === n) && (d = !0, e = "0", n = "=");
                 var y = "$" === f ? i : "#" === f && /[boxX]/.test(v) ? "0" + v.toLowerCase() : "",
-                    w = "$" === f ? o : /[%p]/.test(v) ? u : "",
-                    x = Lr[v],
+                    w = "$" === f ? o : /[%p]/.test(v) ? l : "",
+                    x = Qr[v],
                     b = /[defgprs%]/.test(v);
 
                 function M(t) {
-                    var i, o, u, f = y,
+                    var i, o, l, f = y,
                         M = w;
                     if ("c" === v) M = x(t) + M, t = "";
                     else {
                         var k = (t = +t) < 0 || 1 / t < 0;
                         if (t = isNaN(t) ? c : x(Math.abs(t), _), g && (t = function(t) {
                                 t: for (var e, n = t.length, r = 1, i = -1; r < n; ++r) switch (t[r]) {
                                     case ".":
@@ -2919,79 +2936,79 @@
                                         0 === i && (i = r), e = r;
                                         break;
                                     default:
                                         if (!+t[r]) break t;
                                         i > 0 && (i = 0)
                                 }
                                 return i > 0 ? t.slice(0, i) + t.slice(e + 1) : t
-                            }(t)), k && 0 == +t && "+" !== h && (k = !1), f = (k ? "(" === h ? h : l : "-" === h || "(" === h ? "" : h) + f, M = ("s" === v ? Br[8 + Pr / 3] : "") + M + (k && "(" === h ? ")" : ""), b)
+                            }(t)), k && 0 == +t && "+" !== h && (k = !1), f = (k ? "(" === h ? h : u : "-" === h || "(" === h ? "" : h) + f, M = ("s" === v ? oi[8 + Fr / 3] : "") + M + (k && "(" === h ? ")" : ""), b)
                             for (i = -1, o = t.length; ++i < o;)
-                                if (48 > (u = t.charCodeAt(i)) || u > 57) {
-                                    M = (46 === u ? a + t.slice(i + 1) : t.slice(i)) + M, t = t.slice(0, i);
+                                if (48 > (l = t.charCodeAt(i)) || l > 57) {
+                                    M = (46 === l ? a + t.slice(i + 1) : t.slice(i)) + M, t = t.slice(0, i);
                                     break
                                 }
                     }
                     m && !d && (t = r(t, 1 / 0));
                     var A = f.length + t.length + M.length,
-                        N = A < p ? new Array(p - A + 1).join(e) : "";
-                    switch (m && d && (t = r(N + t, N.length ? p - M.length : 1 / 0), N = ""), n) {
+                        E = A < p ? new Array(p - A + 1).join(e) : "";
+                    switch (m && d && (t = r(E + t, E.length ? p - M.length : 1 / 0), E = ""), n) {
                         case "<":
-                            t = f + t + M + N;
+                            t = f + t + M + E;
                             break;
                         case "=":
-                            t = f + N + t + M;
+                            t = f + E + t + M;
                             break;
                         case "^":
-                            t = N.slice(0, A = N.length >> 1) + f + t + M + N.slice(A);
+                            t = E.slice(0, A = E.length >> 1) + f + t + M + E.slice(A);
                             break;
                         default:
-                            t = N + f + t + M
+                            t = E + f + t + M
                     }
                     return s(t)
                 }
                 return _ = void 0 === _ ? 6 : /[gprs]/.test(v) ? Math.max(1, Math.min(21, _)) : Math.max(0, Math.min(20, _)), M.toString = function() {
                     return t + ""
                 }, M
             }
             return {
                 format: h,
                 formatPrefix: function(t, e) {
-                    var n = h(((t = Or(t)).type = "f", t)),
-                        r = 3 * Math.max(-8, Math.min(8, Math.floor(Dr(e) / 3))),
+                    var n = h(((t = Ur(t)).type = "f", t)),
+                        r = 3 * Math.max(-8, Math.min(8, Math.floor(Zr(e) / 3))),
                         i = Math.pow(10, -r),
-                        o = Br[8 + r / 3];
+                        o = oi[8 + r / 3];
                     return function(t) {
                         return n(i * t) + o
                     }
                 }
             }
         }({
             thousands: ",",
             grouping: [3],
             currency: ["$", ""]
-        }), zr = Xr.format, Rr = Xr.formatPrefix;
-        const Fr = function(t) {
+        }), ni = ei.format, ri = ei.formatPrefix;
+        const si = function(t) {
             for (var e = new Array(10), n = 0; n < 10;) e[n] = "#" + t.slice(6 * n, 6 * ++n);
             return e
         }("1f77b4ff7f0e2ca02cd627289467bd8c564be377c27f7f7fbcbd2217becf");
 
-        function Ur(t) {
+        function li(t) {
             return function() {
                 return t
             }
         }
 
-        function Gr(t) {
+        function ui(t) {
             this._context = t
         }
 
-        function Jr(t) {
-            return new Gr(t)
+        function ci(t) {
+            return new ui(t)
         }
-        Array.prototype.slice, Gr.prototype = {
+        Array.prototype.slice, ui.prototype = {
             areaStart: function() {
                 this._line = 0
             },
             areaEnd: function() {
                 this._line = NaN
             },
             lineStart: function() {
@@ -3008,29 +3025,29 @@
                     case 1:
                         this._point = 2;
                     default:
                         this._context.lineTo(t, e)
                 }
             }
         };
-        const Kr = Math.PI,
-            Zr = 2 * Kr,
-            Qr = 1e-6,
-            ti = Zr - Qr;
+        const hi = Math.PI,
+            fi = 2 * hi,
+            di = 1e-6,
+            pi = fi - di;
 
-        function ei(t) {
+        function mi(t) {
             this._ += t[0];
             for (let e = 1, n = t.length; e < n; ++e) this._ += arguments[e] + t[e]
         }
-        class ni {
+        class _i {
             constructor(t) {
-                this._x0 = this._y0 = this._x1 = this._y1 = null, this._ = "", this._append = null == t ? ei : function(t) {
+                this._x0 = this._y0 = this._x1 = this._y1 = null, this._ = "", this._append = null == t ? mi : function(t) {
                     let e = Math.floor(t);
                     if (!(e >= 0)) throw new Error(`invalid digits: ${t}`);
-                    if (e > 15) return ei;
+                    if (e > 15) return mi;
                     const n = 10 ** e;
                     return function(t) {
                         this._ += t[0];
                         for (let e = 1, r = t.length; e < r; ++e) this._ += Math.round(arguments[e] * n) / n + t[e]
                     }
                 }(t)
             }
@@ -3050,111 +3067,111 @@
                 this._append`C${+t},${+e},${+n},${+r},${this._x1=+i},${this._y1=+o}`
             }
             arcTo(t, e, n, r, i) {
                 if (t = +t, e = +e, n = +n, r = +r, (i = +i) < 0) throw new Error(`negative radius: ${i}`);
                 let o = this._x1,
                     a = this._y1,
                     s = n - t,
-                    u = r - e,
-                    l = o - t,
+                    l = r - e,
+                    u = o - t,
                     c = a - e,
-                    h = l * l + c * c;
+                    h = u * u + c * c;
                 if (null === this._x1) this._append`M${this._x1=t},${this._y1=e}`;
-                else if (h > Qr)
-                    if (Math.abs(c * s - u * l) > Qr && i) {
+                else if (h > di)
+                    if (Math.abs(c * s - l * u) > di && i) {
                         let f = n - o,
                             d = r - a,
-                            p = s * s + u * u,
+                            p = s * s + l * l,
                             m = f * f + d * d,
                             _ = Math.sqrt(p),
                             g = Math.sqrt(h),
-                            v = i * Math.tan((Kr - Math.acos((p + h - m) / (2 * _ * g))) / 2),
+                            v = i * Math.tan((hi - Math.acos((p + h - m) / (2 * _ * g))) / 2),
                             y = v / g,
                             w = v / _;
-                        Math.abs(y - 1) > Qr && this._append`L${t+y*l},${e+y*c}`, this._append`A${i},${i},0,0,${+(c*f>l*d)},${this._x1=t+w*s},${this._y1=e+w*u}`
+                        Math.abs(y - 1) > di && this._append`L${t+y*u},${e+y*c}`, this._append`A${i},${i},0,0,${+(c*f>u*d)},${this._x1=t+w*s},${this._y1=e+w*l}`
                     } else this._append`L${this._x1=t},${this._y1=e}`
             }
             arc(t, e, n, r, i, o) {
                 if (t = +t, e = +e, o = !!o, (n = +n) < 0) throw new Error(`negative radius: ${n}`);
                 let a = n * Math.cos(r),
                     s = n * Math.sin(r),
-                    u = t + a,
-                    l = e + s,
+                    l = t + a,
+                    u = e + s,
                     c = 1 ^ o,
                     h = o ? r - i : i - r;
-                null === this._x1 ? this._append`M${u},${l}` : (Math.abs(this._x1 - u) > Qr || Math.abs(this._y1 - l) > Qr) && this._append`L${u},${l}`, n && (h < 0 && (h = h % Zr + Zr), h > ti ? this._append`A${n},${n},0,1,${c},${t-a},${e-s}A${n},${n},0,1,${c},${this._x1=u},${this._y1=l}` : h > Qr && this._append`A${n},${n},0,${+(h>=Kr)},${c},${this._x1=t+n*Math.cos(i)},${this._y1=e+n*Math.sin(i)}`)
+                null === this._x1 ? this._append`M${l},${u}` : (Math.abs(this._x1 - l) > di || Math.abs(this._y1 - u) > di) && this._append`L${l},${u}`, n && (h < 0 && (h = h % fi + fi), h > pi ? this._append`A${n},${n},0,1,${c},${t-a},${e-s}A${n},${n},0,1,${c},${this._x1=l},${this._y1=u}` : h > di && this._append`A${n},${n},0,${+(h>=hi)},${c},${this._x1=t+n*Math.cos(i)},${this._y1=e+n*Math.sin(i)}`)
             }
             rect(t, e, n, r) {
                 this._append`M${this._x0=this._x1=+t},${this._y0=this._y1=+e}h${n=+n}v${+r}h${-n}Z`
             }
             toString() {
                 return this._
             }
         }
 
-        function ri(t) {
+        function gi(t) {
             return t[0]
         }
 
-        function ii(t) {
+        function vi(t) {
             return t[1]
         }
 
-        function oi(t, e) {
-            var n = Ur(!0),
+        function yi(t, e) {
+            var n = li(!0),
                 r = null,
-                i = Jr,
+                i = ci,
                 o = null,
                 a = function(t) {
                     let e = 3;
                     return t.digits = function(n) {
                         if (!arguments.length) return e;
                         if (null == n) e = null;
                         else {
                             const t = Math.floor(n);
                             if (!(t >= 0)) throw new RangeError(`invalid digits: ${n}`);
                             e = t
                         }
                         return t
-                    }, () => new ni(e)
+                    }, () => new _i(e)
                 }(s);
 
             function s(s) {
-                var u, l, c, h = (s = function(t) {
+                var l, u, c, h = (s = function(t) {
                         return "object" == typeof t && "length" in t ? t : Array.from(t)
                     }(s)).length,
                     f = !1;
-                for (null == r && (o = i(c = a())), u = 0; u <= h; ++u) !(u < h && n(l = s[u], u, s)) === f && ((f = !f) ? o.lineStart() : o.lineEnd()), f && o.point(+t(l, u, s), +e(l, u, s));
+                for (null == r && (o = i(c = a())), l = 0; l <= h; ++l) !(l < h && n(u = s[l], l, s)) === f && ((f = !f) ? o.lineStart() : o.lineEnd()), f && o.point(+t(u, l, s), +e(u, l, s));
                 if (c) return o = null, c + "" || null
             }
-            return t = "function" == typeof t ? t : void 0 === t ? ri : Ur(t), e = "function" == typeof e ? e : void 0 === e ? ii : Ur(e), s.x = function(e) {
-                return arguments.length ? (t = "function" == typeof e ? e : Ur(+e), s) : t
+            return t = "function" == typeof t ? t : void 0 === t ? gi : li(t), e = "function" == typeof e ? e : void 0 === e ? vi : li(e), s.x = function(e) {
+                return arguments.length ? (t = "function" == typeof e ? e : li(+e), s) : t
             }, s.y = function(t) {
-                return arguments.length ? (e = "function" == typeof t ? t : Ur(+t), s) : e
+                return arguments.length ? (e = "function" == typeof t ? t : li(+t), s) : e
             }, s.defined = function(t) {
-                return arguments.length ? (n = "function" == typeof t ? t : Ur(!!t), s) : n
+                return arguments.length ? (n = "function" == typeof t ? t : li(!!t), s) : n
             }, s.curve = function(t) {
                 return arguments.length ? (i = t, null != r && (o = i(r)), s) : i
             }, s.context = function(t) {
                 return arguments.length ? (null == t ? r = o = null : o = i(r = t), s) : r
             }, s
         }
 
-        function ai(t, e, n) {
+        function wi(t, e, n) {
             t._context.bezierCurveTo(t._x1 + t._k * (t._x2 - t._x0), t._y1 + t._k * (t._y2 - t._y0), t._x2 + t._k * (t._x1 - e), t._y2 + t._k * (t._y1 - n), t._x2, t._y2)
         }
 
-        function si(t, e) {
+        function xi(t, e) {
             this._context = t, this._k = (1 - e) / 6
         }
 
-        function ui(t, e) {
+        function bi(t, e) {
             this._context = t, this._alpha = e
         }
-        ni.prototype, Math.abs, Math.atan2, Math.cos, Math.max, Math.min, Math.sin, Math.sqrt, Math.PI, si.prototype = {
+        _i.prototype, Math.abs, Math.atan2, Math.cos, Math.max, Math.min, Math.sin, Math.sqrt, Math.PI, xi.prototype = {
                 areaStart: function() {
                     this._line = 0
                 },
                 areaEnd: function() {
                     this._line = NaN
                 },
                 lineStart: function() {
@@ -3162,41 +3179,41 @@
                 },
                 lineEnd: function() {
                     switch (this._point) {
                         case 2:
                             this._context.lineTo(this._x2, this._y2);
                             break;
                         case 3:
-                            ai(this, this._x1, this._y1)
+                            wi(this, this._x1, this._y1)
                     }(this._line || 0 !== this._line && 1 === this._point) && this._context.closePath(), this._line = 1 - this._line
                 },
                 point: function(t, e) {
                     switch (t = +t, e = +e, this._point) {
                         case 0:
                             this._point = 1, this._line ? this._context.lineTo(t, e) : this._context.moveTo(t, e);
                             break;
                         case 1:
                             this._point = 2, this._x1 = t, this._y1 = e;
                             break;
                         case 2:
                             this._point = 3;
                         default:
-                            ai(this, t, e)
+                            wi(this, t, e)
                     }
                     this._x0 = this._x1, this._x1 = this._x2, this._x2 = t, this._y0 = this._y1, this._y1 = this._y2, this._y2 = e
                 }
             },
             function t(e) {
                 function n(t) {
-                    return new si(t, e)
+                    return new xi(t, e)
                 }
                 return n.tension = function(e) {
                     return t(+e)
                 }, n
-            }(0), ui.prototype = {
+            }(0), bi.prototype = {
                 areaStart: function() {
                     this._line = 0
                 },
                 areaEnd: function() {
                     this._line = NaN
                 },
                 lineStart: function() {
@@ -3230,205 +3247,205 @@
                             ! function(t, e, n) {
                                 var r = t._x1,
                                     i = t._y1,
                                     o = t._x2,
                                     a = t._y2;
                                 if (t._l01_a > 1e-12) {
                                     var s = 2 * t._l01_2a + 3 * t._l01_a * t._l12_a + t._l12_2a,
-                                        u = 3 * t._l01_a * (t._l01_a + t._l12_a);
-                                    r = (r * s - t._x0 * t._l12_2a + t._x2 * t._l01_2a) / u, i = (i * s - t._y0 * t._l12_2a + t._y2 * t._l01_2a) / u
+                                        l = 3 * t._l01_a * (t._l01_a + t._l12_a);
+                                    r = (r * s - t._x0 * t._l12_2a + t._x2 * t._l01_2a) / l, i = (i * s - t._y0 * t._l12_2a + t._y2 * t._l01_2a) / l
                                 }
                                 if (t._l23_a > 1e-12) {
-                                    var l = 2 * t._l23_2a + 3 * t._l23_a * t._l12_a + t._l12_2a,
+                                    var u = 2 * t._l23_2a + 3 * t._l23_a * t._l12_a + t._l12_2a,
                                         c = 3 * t._l23_a * (t._l23_a + t._l12_a);
-                                    o = (o * l + t._x1 * t._l23_2a - e * t._l12_2a) / c, a = (a * l + t._y1 * t._l23_2a - n * t._l12_2a) / c
+                                    o = (o * u + t._x1 * t._l23_2a - e * t._l12_2a) / c, a = (a * u + t._y1 * t._l23_2a - n * t._l12_2a) / c
                                 }
                                 t._context.bezierCurveTo(r, i, o, a, t._x2, t._y2)
                             }(this, t, e)
                     }
                     this._l01_a = this._l12_a, this._l12_a = this._l23_a, this._l01_2a = this._l12_2a, this._l12_2a = this._l23_2a, this._x0 = this._x1, this._x1 = this._x2, this._x2 = t, this._y0 = this._y1, this._y1 = this._y2, this._y2 = e
                 }
             };
-        const li = function t(e) {
+        const Mi = function t(e) {
             function n(t) {
-                return e ? new ui(t, e) : new si(t, 0)
+                return e ? new bi(t, e) : new xi(t, 0)
             }
             return n.alpha = function(e) {
                 return t(+e)
             }, n
         }(.5);
 
-        function ci(t, e, n) {
+        function ki(t, e, n) {
             this.k = t, this.x = e, this.y = n
         }
 
-        function hi(t, e, n, r, i, o, a, s, u, l) {
+        function Ai(t) {
+            const e = t.reduce(((t, e) => t + e), 0) / t.length,
+                n = 1.96 * function(t, e) {
+                    let n = 0;
+                    return t.forEach((t => n += (t - e) ** 2)), n = Math.sqrt(n) / t.length, n
+                }(t, e);
+            return [e - n, e + n]
+        }
+
+        function Ei(t, e, n, r, i, o, a, s, l, u) {
             let c = [];
-            const h = oi(),
-                f = er(t).selectAll(".dot"),
+            const h = yi(),
+                f = mr(t).selectAll(".dot"),
                 d = function() {
-                    var t, e, n, r, i = lr,
-                        o = cr,
-                        a = hr,
-                        s = fr,
-                        u = {},
-                        l = ne("start", "drag", "end"),
+                    var t, e, n, r, i = Mr,
+                        o = kr,
+                        a = Ar,
+                        s = Er,
+                        l = {},
+                        u = _e("start", "drag", "end"),
                         c = 0,
                         h = 0;
 
                     function f(t) {
-                        t.on("mousedown.drag", d).filter(s).on("touchstart.drag", _).on("touchmove.drag", g, rr).on("touchend.drag touchcancel.drag", v).style("touch-action", "none").style("-webkit-tap-highlight-color", "rgba(0,0,0,0)")
+                        t.on("mousedown.drag", d).filter(s).on("touchstart.drag", _).on("touchmove.drag", g, gr).on("touchend.drag touchcancel.drag", v).style("touch-action", "none").style("-webkit-tap-highlight-color", "rgba(0,0,0,0)")
                     }
 
                     function d(a, s) {
                         if (!r && i.call(this, a, s)) {
-                            var u = y(this, o.call(this, a, s), a, s, "mouse");
-                            u && (er(a.view).on("mousemove.drag", p, ir).on("mouseup.drag", m, ir), function(t) {
+                            var l = y(this, o.call(this, a, s), a, s, "mouse");
+                            l && (mr(a.view).on("mousemove.drag", p, vr).on("mouseup.drag", m, vr), function(t) {
                                 var e = t.document.documentElement,
-                                    n = er(t).on("dragstart.drag", ar, ir);
-                                "onselectstart" in e ? n.on("selectstart.drag", ar, ir) : (e.__noselect = e.style.MozUserSelect, e.style.MozUserSelect = "none")
-                            }(a.view), or(a), n = !1, t = a.clientX, e = a.clientY, u("start", a))
+                                    n = mr(t).on("dragstart.drag", wr, vr);
+                                "onselectstart" in e ? n.on("selectstart.drag", wr, vr) : (e.__noselect = e.style.MozUserSelect, e.style.MozUserSelect = "none")
+                            }(a.view), yr(a), n = !1, t = a.clientX, e = a.clientY, l("start", a))
                         }
                     }
 
                     function p(r) {
-                        if (ar(r), !n) {
+                        if (wr(r), !n) {
                             var i = r.clientX - t,
                                 o = r.clientY - e;
                             n = i * i + o * o > h
                         }
-                        u.mouse("drag", r)
+                        l.mouse("drag", r)
                     }
 
                     function m(t) {
-                        er(t.view).on("mousemove.drag mouseup.drag", null),
+                        mr(t.view).on("mousemove.drag mouseup.drag", null),
                             function(t, e) {
                                 var n = t.document.documentElement,
-                                    r = er(t).on("dragstart.drag", null);
-                                e && (r.on("click.drag", ar, ir), setTimeout((function() {
+                                    r = mr(t).on("dragstart.drag", null);
+                                e && (r.on("click.drag", wr, vr), setTimeout((function() {
                                     r.on("click.drag", null)
                                 }), 0)), "onselectstart" in n ? r.on("selectstart.drag", null) : (n.style.MozUserSelect = n.__noselect, delete n.__noselect)
-                            }(t.view, n), ar(t), u.mouse("end", t)
+                            }(t.view, n), wr(t), l.mouse("end", t)
                     }
 
                     function _(t, e) {
                         if (i.call(this, t, e)) {
                             var n, r, a = t.changedTouches,
                                 s = o.call(this, t, e),
-                                u = a.length;
-                            for (n = 0; n < u; ++n)(r = y(this, s, t, e, a[n].identifier, a[n])) && (or(t), r("start", t, a[n]))
+                                l = a.length;
+                            for (n = 0; n < l; ++n)(r = y(this, s, t, e, a[n].identifier, a[n])) && (yr(t), r("start", t, a[n]))
                         }
                     }
 
                     function g(t) {
                         var e, n, r = t.changedTouches,
                             i = r.length;
-                        for (e = 0; e < i; ++e)(n = u[r[e].identifier]) && (ar(t), n("drag", t, r[e]))
+                        for (e = 0; e < i; ++e)(n = l[r[e].identifier]) && (wr(t), n("drag", t, r[e]))
                     }
 
                     function v(t) {
                         var e, n, i = t.changedTouches,
                             o = i.length;
                         for (r && clearTimeout(r), r = setTimeout((function() {
                                 r = null
-                            }), 500), e = 0; e < o; ++e)(n = u[i[e].identifier]) && (or(t), n("end", t, i[e]))
+                            }), 500), e = 0; e < o; ++e)(n = l[i[e].identifier]) && (yr(t), n("end", t, i[e]))
                     }
 
                     function y(t, e, n, r, i, o) {
-                        var s, h, d, p = l.copy(),
-                            m = nr(o || n, e);
-                        if (null != (d = a.call(t, new ur("beforestart", {
+                        var s, h, d, p = u.copy(),
+                            m = _r(o || n, e);
+                        if (null != (d = a.call(t, new br("beforestart", {
                                 sourceEvent: n,
                                 target: f,
                                 identifier: i,
                                 active: c,
                                 x: m[0],
                                 y: m[1],
                                 dx: 0,
                                 dy: 0,
                                 dispatch: p
                             }), r))) return s = d.x - m[0] || 0, h = d.y - m[1] || 0,
-                            function n(o, a, l) {
+                            function n(o, a, u) {
                                 var _, g = m;
                                 switch (o) {
                                     case "start":
-                                        u[i] = n, _ = c++;
+                                        l[i] = n, _ = c++;
                                         break;
                                     case "end":
-                                        delete u[i], --c;
+                                        delete l[i], --c;
                                     case "drag":
-                                        m = nr(l || a, e), _ = c
+                                        m = _r(u || a, e), _ = c
                                 }
-                                p.call(o, t, new ur(o, {
+                                p.call(o, t, new br(o, {
                                     sourceEvent: a,
                                     subject: d,
                                     target: f,
                                     identifier: i,
                                     active: _,
                                     x: m[0] + s,
                                     y: m[1] + h,
                                     dx: m[0] - g[0],
                                     dy: m[1] - g[1],
                                     dispatch: p
                                 }), r)
                             }
                     }
                     return f.filter = function(t) {
-                        return arguments.length ? (i = "function" == typeof t ? t : sr(!!t), f) : i
+                        return arguments.length ? (i = "function" == typeof t ? t : xr(!!t), f) : i
                     }, f.container = function(t) {
-                        return arguments.length ? (o = "function" == typeof t ? t : sr(t), f) : o
+                        return arguments.length ? (o = "function" == typeof t ? t : xr(t), f) : o
                     }, f.subject = function(t) {
-                        return arguments.length ? (a = "function" == typeof t ? t : sr(t), f) : a
+                        return arguments.length ? (a = "function" == typeof t ? t : xr(t), f) : a
                     }, f.touchable = function(t) {
-                        return arguments.length ? (s = "function" == typeof t ? t : sr(!!t), f) : s
+                        return arguments.length ? (s = "function" == typeof t ? t : xr(!!t), f) : s
                     }, f.on = function() {
-                        var t = l.on.apply(l, arguments);
-                        return t === l ? f : t
+                        var t = u.on.apply(u, arguments);
+                        return t === u ? f : t
                     }, f.clickDistance = function(t) {
                         return arguments.length ? (h = (t = +t) * t, f) : Math.sqrt(h)
                     }, f
                 }().on("start", (function() {
-                    c = [], s(), er(t).select("svg").append("path").attr("id", "lasso" + l)
+                    c = [], s(), mr(t).select("svg").append("path").attr("id", "lasso" + u)
                 })).on("drag", (function(t) {
                     let e = t.sourceEvent.offsetX,
                         n = t.sourceEvent.offsetY;
-                    c.push([e, n]), er("#lasso" + l).style("stroke", "blue").style("stroke-width", 2).style("fill", "#00008854").attr("d", h(c))
+                    c.push([e, n]), mr("#lasso" + u).style("stroke", "blue").style("stroke-width", 2).style("fill", "#00008854").attr("d", h(c))
                 })).on("end", (function() {
                     let t = [];
-                    f.each(((s, u) => {
+                    f.each(((s, l) => {
                         (function(t, e) {
                             for (var n = t[0], r = t[1], i = !1, o = 0, a = e.length - 1; o < e.length; a = o++) {
                                 var s = e[o][0],
-                                    u = e[o][1],
-                                    l = e[a][0],
+                                    l = e[o][1],
+                                    u = e[a][0],
                                     c = e[a][1];
-                                u > r != c > r && n < (l - s) * (r - u) / (c - u) + s && (i = !i)
+                                l > r != c > r && n < (u - s) * (r - l) / (c - l) + s && (i = !i)
                             }
                             return i
-                        })([e(s[r]) + o, n(s[i]) + a], c) && (er("#dot-" + l + s.id).style("fill", "red").attr("r", 6), t.push(s))
-                    })), er("#lasso" + l).remove(), u(t)
+                        })([e(s[r]) + o, n(s[i]) + a], c) && (mr("#dot-" + u + s.id).style("fill", "red").attr("r", 6), t.push(s))
+                    })), mr("#lasso" + u).remove(), l(t)
                 }));
-            er(t).call(d)
-        }
-
-        function fi(t) {
-            const e = t.reduce(((t, e) => t + e), 0) / t.length,
-                n = 1.96 * function(t, e) {
-                    let n = 0;
-                    return t.forEach((t => n += (t - e) ** 2)), n = Math.sqrt(n) / t.length, n
-                }(t, e);
-            return [e - n, e + n]
+            mr(t).call(d)
         }
-        ci.prototype = {
-            constructor: ci,
+        ki.prototype = {
+            constructor: ki,
             scale: function(t) {
-                return 1 === t ? this : new ci(this.k * t, this.x, this.y)
+                return 1 === t ? this : new ki(this.k * t, this.x, this.y)
             },
             translate: function(t, e) {
-                return 0 === t & 0 === e ? this : new ci(this.k, this.x + this.k * t, this.y + this.k * e)
+                return 0 === t & 0 === e ? this : new ki(this.k, this.x + this.k * t, this.y + this.k * e)
             },
             apply: function(t) {
                 return [t[0] * this.k + this.x, t[1] * this.k + this.y]
             },
             applyX: function(t) {
                 return t * this.k + this.x
             },
@@ -3449,40 +3466,25 @@
             },
             rescaleY: function(t) {
                 return t.copy().domain(t.range().map(this.invertY, this).map(t.invert, t))
             },
             toString: function() {
                 return "translate(" + this.x + "," + this.y + ") scale(" + this.k + ")"
             }
-        }, new ci(1, 0, 0), ci.prototype;
-        var di = i(72),
-            pi = i.n(di),
-            mi = i(825),
-            _i = i.n(mi),
-            gi = i(659),
-            vi = i.n(gi),
-            yi = i(56),
-            wi = i.n(yi),
-            xi = i(540),
-            bi = i.n(xi),
-            Mi = i(113),
-            ki = i.n(Mi),
-            Ai = i(930),
-            Ni = {};
-        Ni.styleTagTransform = ki(), Ni.setAttributes = wi(), Ni.insert = vi().bind(null, "head"), Ni.domAPI = _i(), Ni.insertStyleElement = bi(), pi()(Ai.A, Ni), Ai.A && Ai.A.locals && Ai.A.locals;
-        const $i = i(330),
+        }, new ki(1, 0, 0), ki.prototype;
+        const Ni = i(330),
             Si = 400,
-            Ei = {
+            $i = {
                 top: 20,
                 right: 20,
                 bottom: 30,
                 left: 40
             };
 
-        function ji(t) {
+        function Ci(t) {
             t.timeout && clearTimeout(t.timeout), t.timeout = setTimeout((() => {
                 t.plot()
             }), 100)
         }
         class Ti extends t.DOMWidgetModel {
             defaults() {
                 return {
@@ -3497,221 +3499,225 @@
                     linearData_y: [],
                     histogramData: [],
                     elementId: String,
                     clickedValue: String
                 }
             }
             static model_name = "LinearHistPlotModel";
-            static model_module = $i.name;
-            static model_module_version = $i.version;
+            static model_module = Ni.name;
+            static model_module_version = Ni.version;
             static view_name = "LinearHistPlotView";
-            static view_module = $i.name;
-            static view_module_version = $i.version
+            static view_module = Ni.name;
+            static view_module_version = Ni.version
         }
-        class Pi extends t.DOMWidgetView {
+        class ji extends t.DOMWidgetView {
             timeout;
             render() {
-                ji(this), this.model.on("change:linearData_x", (() => ji(this)), this), window.addEventListener("resize", (() => ji(this).bind(this)))
+                Ci(this), this.model.on("change:linearData_x", (() => Ci(this)), this), this.model.on("change:linearData_y", (() => Ci(this)), this), this.model.on("change:histogramData", (() => Ci(this)), this), window.addEventListener("resize", (() => Ci(this)))
             }
             plot() {
                 const t = this.model.get("linearData_x"),
-                    n = this.model.get("linearData_y"),
-                    r = this.model.get("histogramData"),
-                    i = this.model.get("elementId");
-                let o = Si,
-                    a = this.el;
-                i && (a = document.getElementById(i), o = a.clientHeight);
-                let s = a.clientWidth;
-                const u = Ei;
-                ! function(t, n, r, i, o, a, s, u) {
-                    const l = a - u.left - u.right,
-                        c = s - u.top - u.bottom,
-                        h = c / 4;
-                    er(i).selectAll("*").remove();
-                    const f = Math.min(k(t), k(r)),
-                        d = Math.max(M(t), M(r)),
-                        p = Wr().range([0, l]),
-                        m = Wr().range([c, 0]),
-                        _ = Wr().range([h, 0]),
-                        g = D(p),
-                        v = q(m),
-                        y = b().thresholds(20).value((t => Math.round(10 * t) / 10))(r),
-                        w = er(i).append("svg").attr("width", a).attr("height", s).append("g").attr("transform", "translate(" + u.left + "," + u.top + ")");
-                    p.domain([f, d]), m.domain(e(n)), _.domain([0, M(y, (t => t.length))]);
+                    e = this.model.get("linearData_y"),
+                    n = this.model.get("histogramData"),
+                    r = this.model.get("elementId");
+                let i = Si,
+                    o = this.el;
+                r && (o = document.getElementById(r), i = o.clientHeight);
+                let a = o.clientWidth;
+                const s = $i;
+                ! function(t, e, n, r, i, o, a, s) {
+                    const l = o - s.left - s.right,
+                        u = a - s.top - s.bottom,
+                        c = u / 4;
+                    mr(r).selectAll("*").remove();
+                    const h = Math.min(I(t), I(n)),
+                        f = Math.max(D(t), D(n)),
+                        d = ai().range([0, l]),
+                        p = ai().range([u, 0]),
+                        m = ai().range([c, 0]),
+                        _ = Z(d),
+                        v = K(p),
+                        y = L().thresholds(20).value((t => Math.round(10 * t) / 10))(n),
+                        w = mr(r).append("svg").attr("width", o).attr("height", a).append("g").attr("transform", "translate(" + s.left + "," + s.top + ")");
+                    d.domain([h, f]), p.domain(g(e)), m.domain([0, D(y, (t => t.length))]);
                     const x = w.append("g").append("rect").style("fill", "none").attr("width", 160).attr("height", 40).attr("stroke", "#69b3a2").attr("stroke-width", 4).style("opacity", 0),
-                        A = w.append("g").append("text").style("opacity", 0).attr("text-anchor", "left").attr("alignment-baseline", "middle");
-                    w.append("g").attr("transform", "translate(0," + c + ")").call(g).append("text").attr("x", l).attr("y", -6).style("text-anchor", "end"), w.append("g").call(v).append("text").attr("transform", "rotate(-90)").attr("y", 6).attr("dy", ".71em").style("text-anchor", "end"), w.append("path").datum(y).attr("fill", "paleturquoise").attr("stroke", "steelblue").attr("stroke-width", 1).attr("d", oi().x((t => p((t.x1 + t.x0) / 2))).y((t => _(t.length) + c - h)).curve(li));
-                    const N = t.map(((t, e) => [t, n[e]])).map((([t, e]) => ({
+                        b = w.append("g").append("text").style("opacity", 0).attr("text-anchor", "left").attr("alignment-baseline", "middle");
+                    w.append("g").attr("transform", "translate(0," + u + ")").call(_).append("text").attr("x", l).attr("y", -6).style("text-anchor", "end"), w.append("g").call(v).append("text").attr("transform", "rotate(-90)").attr("y", 6).attr("dy", ".71em").style("text-anchor", "end");
+                    const M = [];
+                    M.x0 = y[0].x0 - 2.5, M.x1 = y[0].x1 - 2.5, y.unshift(M);
+                    const k = [];
+                    k.x0 = y[y.length - 1].x0 + 2.5, k.x1 = y[y.length - 1].x1 + 2.5, w.append("path").datum(y).attr("fill", "paleturquoise").attr("stroke", "steelblue").attr("stroke-width", 1).attr("d", yi().x((t => d((t.x1 + t.x0) / 2))).y((t => m(t.length) + u - c)).curve(Mi));
+                    const A = t.map(((t, n) => [t, e[n]])).map((([t, e]) => ({
                         x: t,
                         y: e
                     })));
-                    w.append("path").datum(N).attr("fill", "none").attr("stroke", "steelblue").attr("stroke-width", 1.5).attr("d", oi().x((t => p(t.x))).y((t => m(t.y)))), w.selectAll("myCircles").data(N).enter().append("circle").attr("fill", "red").attr("stroke", "none").attr("cx", (t => p(t.x))).attr("cy", (t => m(t.y))).attr("r", 3).on("mouseover", (function(t, e) {
-                        x.style("opacity", 1), A.style("opacity", 1), x.attr("x", t.offsetX - 30).attr("y", t.offsetY - 40), A.html("x:" + Math.round(10 * e.x) / 10 + "  -  y:" + Math.round(10 * e.y) / 10).attr("x", t.offsetX - 15).attr("y", t.offsetY - 20)
+                    w.append("path").datum(A).attr("fill", "none").attr("stroke", "steelblue").attr("stroke-width", 1.5).attr("d", yi().x((t => d(t.x))).y((t => p(t.y)))), w.selectAll("myCircles").data(A).enter().append("circle").attr("fill", "red").attr("stroke", "none").attr("cx", (t => d(t.x))).attr("cy", (t => p(t.y))).attr("r", 3).on("mouseover", (function(t, e) {
+                        x.style("opacity", 1), b.style("opacity", 1), x.attr("x", t.offsetX - 30).attr("y", t.offsetY - 40), b.html("x:" + Math.round(10 * e.x) / 10 + "  -  y:" + Math.round(10 * e.y) / 10).attr("x", t.offsetX - 15).attr("y", t.offsetY - 20)
                     })).on("mouseout", (function() {
-                        x.style("opacity", 0), A.style("opacity", 0)
+                        x.style("opacity", 0), b.style("opacity", 0)
                     })).on("click", (function(t, e) {
                         const n = "x:" + Math.round(10 * e.x) / 10 + "  -  y:" + Math.round(10 * e.y) / 10;
-                        void 0 !== o && o(n)
+                        void 0 !== i && i(n)
                     }))
-                }(t, n, r, a, this.setValue.bind(this), s, o, u)
+                }(t, e, n, o, this.setValue.bind(this), a, i, s)
             }
             setValue(t) {
                 this.model.set({
                     clickedValue: t
                 }), this.model.save_changes()
             }
         }
-        class Ci extends t.DOMWidgetModel {
+        class Oi extends t.DOMWidgetModel {
             defaults() {
                 return {
                     ...super.defaults(),
-                    _model_name: Ci.model_name,
-                    _view_name: Ci.view_name,
-                    _model_module: Ci.model_module,
-                    _view_module: Ci.view_module,
-                    _model_module_version: Ci.model_module_version,
-                    _view_module_version: Ci.view_module_version,
+                    _model_name: Oi.model_name,
+                    _view_name: Oi.view_name,
+                    _model_module: Oi.model_module,
+                    _view_module: Oi.view_module,
+                    _model_module_version: Oi.model_module_version,
+                    _view_module_version: Oi.view_module_version,
                     data: [],
                     x: String,
                     y: String,
                     hue: String,
                     elementId: String,
                     clickedValue: String,
                     selectedValues: []
                 }
             }
             static model_name = "ScatterplotModel";
-            static model_module = $i.name;
-            static model_module_version = $i.version;
+            static model_module = Ni.name;
+            static model_module_version = Ni.version;
             static view_name = "ScatterplotView";
-            static view_module = $i.name;
-            static view_module_version = $i.version
+            static view_module = Ni.name;
+            static view_module_version = Ni.version
         }
-        class Oi extends t.DOMWidgetView {
+        class Pi extends t.DOMWidgetView {
             timeout;
             render() {
-                ji(this), this.model.on("change:data", (() => ji(this)), this), window.addEventListener("resize", (() => ji(this).bind(this)))
+                Ci(this), this.model.on("change:data", (() => Ci(this)), this), this.model.on("change:x", (() => Ci(this)), this), this.model.on("change:y", (() => Ci(this)), this), this.model.on("change:hue", (() => Ci(this)), this), window.addEventListener("resize", (() => Ci(this)))
             }
             plot() {
                 const t = this.model.get("data"),
-                    n = this.model.get("x"),
-                    r = this.model.get("y"),
-                    i = this.model.get("hue"),
-                    o = this.model.get("elementId");
-                let a = Si,
-                    s = this.el;
-                o && (s = document.getElementById(o), a = s.clientHeight);
-                let u = s.clientWidth;
-                const l = Ei;
-                ! function(t, n, r, i, o, a, s, u, l, c) {
-                    const h = u - c.left - c.right,
-                        f = l - c.top - c.bottom;
+                    e = this.model.get("x"),
+                    n = this.model.get("y"),
+                    r = this.model.get("hue"),
+                    i = this.model.get("elementId");
+                let o = Si,
+                    a = this.el;
+                i && (a = document.getElementById(i), o = a.clientHeight);
+                let s = a.clientWidth;
+                const l = $i;
+                ! function(t, e, n, r, i, o, a, s, l, u) {
+                    const c = s - u.left - u.right,
+                        h = l - u.top - u.bottom;
                     for (let e = 0; e < t.length; e++) t[e].id = e;
-                    const d = Math.floor(Math.random() * Date.now() * 1e4).toString(36);
-                    er(o).selectAll("*").remove();
-                    const p = Wr().range([0, h]),
-                        m = Wr().range([f, 0]),
-                        _ = vr(Fr),
-                        g = D(p),
-                        v = q(m),
-                        y = er(o).append("svg").attr("width", u).attr("height", l).append("g").attr("transform", "translate(" + c.left + "," + c.top + ")");
-                    p.domain(e(t, (function(t) {
+                    const f = Math.floor(Math.random() * Date.now() * 1e4).toString(36);
+                    mr(i).selectAll("*").remove();
+                    const d = ai().range([0, c]),
+                        p = ai().range([h, 0]),
+                        m = jr(si),
+                        _ = Z(d),
+                        v = K(p),
+                        y = mr(i).append("svg").attr("width", s).attr("height", l).append("g").attr("transform", "translate(" + u.left + "," + u.top + ")");
+                    d.domain(g(t, (function(t) {
+                        return t[e]
+                    }))).nice(), p.domain(g(t, (function(t) {
                         return t[n]
-                    }))).nice(), m.domain(e(t, (function(t) {
-                        return t[r]
-                    }))).nice(), y.append("g").attr("class", "x axis").attr("transform", "translate(0," + f + ")").call(g).append("text").attr("class", "label").attr("x", h).attr("y", -6).style("text-anchor", "end"), y.append("g").attr("class", "y axis").call(v).append("text").attr("class", "label").attr("transform", "rotate(-90)").attr("y", 6).attr("dy", ".71em").style("text-anchor", "end"), y.selectAll(".dot").data(t).enter().append("circle").attr("id", (function(t, e) {
-                        return "dot-" + d + t.id
+                    }))).nice(), y.append("g").attr("class", "x axis").attr("transform", "translate(0," + h + ")").call(_).append("text").attr("class", "label").attr("x", c).attr("y", -6).style("text-anchor", "end"), y.append("g").attr("class", "y axis").call(v).append("text").attr("class", "label").attr("transform", "rotate(-90)").attr("y", 6).attr("dy", ".71em").style("text-anchor", "end"), y.selectAll(".dot").data(t).enter().append("circle").attr("id", (function(t, e) {
+                        return "dot-" + f + t.id
                     })).attr("class", "dot").attr("r", 3.5).attr("cx", (function(t) {
-                        return p(t[n])
+                        return d(t[e])
                     })).attr("cy", (function(t) {
-                        return m(t[r])
+                        return p(t[n])
                     })).style("fill", (function(t) {
-                        return _(t[i])
-                    })).on("mouseover", (function(t, e) {
-                        x.style("opacity", 1), b.style("opacity", 1), x.attr("x", t.offsetX - 30).attr("y", t.offsetY - 40), b.html("x: " + Math.round(10 * e[n]) / 10 + "&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;y: " + Math.round(10 * e[r]) / 10).attr("x", t.offsetX - 15).attr("y", t.offsetY - 20)
+                        return m(t[r])
+                    })).on("mouseover", (function(t, r) {
+                        x.style("opacity", 1), b.style("opacity", 1), x.attr("x", t.offsetX - 30).attr("y", t.offsetY - 40), b.html("x: " + Math.round(10 * r[e]) / 10 + "&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;y: " + Math.round(10 * r[n]) / 10).attr("x", t.offsetX - 15).attr("y", t.offsetY - 20)
                     })).on("mouseout", (function() {
                         x.style("opacity", 0), b.style("opacity", 0)
-                    })).on("click", (function(t, e) {
-                        const i = "x:" + Math.round(10 * e[n]) / 10 + "    y:" + Math.round(10 * e[r]) / 10;
-                        void 0 !== a && a(i)
-                    })), hi(o, p, m, n, r, c.left, c.top, (function() {
+                    })).on("click", (function(t, r) {
+                        const i = "x:" + Math.round(10 * r[e]) / 10 + "    y:" + Math.round(10 * r[n]) / 10;
+                        void 0 !== o && o(i)
+                    })), Ei(i, d, p, e, n, u.left, u.top, (function() {
                         y.selectAll(".dot").data(t).attr("r", 3.5).style("fill", (function(t) {
-                            return _(t[i])
+                            return m(t[r])
                         }))
                     }), (function(t) {
-                        void 0 !== s && s(t)
-                    }), d);
-                    const w = y.selectAll(".legend").data(_.domain()).enter().append("g").attr("class", "legend").attr("transform", (function(t, e) {
+                        void 0 !== a && a(t)
+                    }), f);
+                    const w = y.selectAll(".legend").data(m.domain()).enter().append("g").attr("class", "legend").attr("transform", (function(t, e) {
                         return "translate(0," + 20 * e + ")"
                     }));
-                    w.append("rect").attr("x", h - 18).attr("width", 18).attr("height", 18).style("fill", _), w.append("text").attr("x", h - 24).attr("y", 9).attr("dy", ".35em").style("text-anchor", "end").text((function(t) {
+                    w.append("rect").attr("x", c - 18).attr("width", 18).attr("height", 18).style("fill", m), w.append("text").attr("x", c - 24).attr("y", 9).attr("dy", ".35em").style("text-anchor", "end").text((function(t) {
                         return t
                     }));
                     const x = y.append("g").append("rect").style("fill", "none").attr("width", 160).attr("height", 40).attr("stroke", "#69b3a2").attr("stroke-width", 4).style("opacity", 0),
                         b = y.append("g").append("text").style("opacity", 0).attr("text-anchor", "left").attr("alignment-baseline", "middle")
-                }(t, n, r, i, s, this.setValue.bind(this), this.setSelectedValues.bind(this), u, a, l)
+                }(t, e, n, r, a, this.setValue.bind(this), this.setSelectedValues.bind(this), s, o, l)
             }
             setValue(t) {
                 this.model.set({
                     clickedValue: t
                 }), this.model.save_changes()
             }
             setSelectedValues(t) {
                 this.model.set({
                     selectedValues: t
                 }), this.model.save_changes()
             }
         }
-        class Ii extends t.DOMWidgetModel {
+        class Vi extends t.DOMWidgetModel {
             defaults() {
                 return {
                     ...super.defaults(),
-                    _model_name: Ii.model_name,
-                    _view_name: Ii.view_name,
-                    _model_module: Ii.model_module,
-                    _view_module: Ii.view_module,
-                    _model_module_version: Ii.model_module_version,
-                    _view_module_version: Ii.view_module_version,
+                    _model_name: Vi.model_name,
+                    _view_name: Vi.view_name,
+                    _model_module: Vi.model_module,
+                    _view_module: Vi.view_module,
+                    _model_module_version: Vi.model_module_version,
+                    _view_module_version: Vi.view_module_version,
                     data: [],
                     x: String,
                     y: String,
                     hue: String,
                     elementId: String
                 }
             }
             static model_name = "BarplotModel";
-            static model_module = $i.name;
-            static model_module_version = $i.version;
+            static model_module = Ni.name;
+            static model_module_version = Ni.version;
             static view_name = "BarplotView";
-            static view_module = $i.name;
-            static view_module_version = $i.version
+            static view_module = Ni.name;
+            static view_module_version = Ni.version
         }
-        class Vi extends t.DOMWidgetView {
+        class Li extends t.DOMWidgetView {
             timeout;
             render() {
-                ji(this), this.model.on("change:data", (() => ji(this)), this), window.addEventListener("resize", (() => ji(this).bind(this)))
+                Ci(this), this.model.on("change:data", (() => Ci(this)), this), this.model.on("change:x", (() => Ci(this)), this), this.model.on("change:y", (() => Ci(this)), this), this.model.on("change:hue", (() => Ci(this)), this), window.addEventListener("resize", (() => Ci(this)))
             }
             plot() {
                 const t = this.model.get("data"),
                     e = this.model.get("x"),
                     n = this.model.get("y"),
                     r = this.model.get("hue"),
                     i = this.model.get("elementId");
                 let o = Si,
                     a = this.el;
                 i && (a = document.getElementById(i), o = a.clientHeight),
                     function(t, e, n, r, i, o, a, s) {
-                        const u = o - s.left - s.right,
-                            l = a - s.top - s.bottom;
-                        er(i).selectAll("*").remove();
-                        const c = er(i).append("svg").attr("width", o).attr("height", a).append("g").attr("transform", "translate(" + s.left + "," + s.top + ")");
+                        const l = o - s.left - s.right,
+                            u = a - s.top - s.bottom;
+                        mr(i).selectAll("*").remove();
+                        const c = mr(i).append("svg").attr("width", o).attr("height", a).append("g").attr("transform", "translate(" + s.left + "," + s.top + ")");
                         r || (r = e);
                         const h = t.reduce(((t, e) => (t && -1 === t.indexOf(e[r]) && t.push(e[r]), t)), []),
                             f = {},
-                            d = vr(Fr);
+                            d = jr(si);
                         r == e ? function() {
                             let r = t.reduce(((t, r) => {
                                 const i = r[e],
                                     o = r[n];
                                 if (i in t) t[i] += o, f[i].qt += 1, f[i][n].push(o);
                                 else {
                                     const e = {
@@ -3722,24 +3728,24 @@
                                 return t
                             }), {});
                             r = Object.keys(r).map((t => {
                                 const i = {};
                                 return i[e] = t, i[n] = r[t], 0 != f[t].qt && (i[n] = i[n] / f[t].qt), i
                             })), Object.keys(f).forEach((t => {
                                 const e = f[t][n],
-                                    [r, i] = fi(e);
+                                    [r, i] = Ai(e);
                                 f[t].min = r, f[t].max = i
                             }));
                             const i = r.map((t => t[e])),
                                 o = [],
                                 a = Object.keys(f).map((t => f[t]));
-                            o.push(k(a, (t => t.min))), o.push(M(a, (t => t.max))), o[0] > 0 && o[1] > 0 ? o[0] = 0 : o[0] < 0 && o[1] < 0 && (o[1] = 0);
-                            const s = Wr().domain(o).range([l, 0]);
-                            c.append("g").call(q(s));
-                            const p = yr().domain(i).range([0, u]).padding([.2]);
+                            o.push(I(a, (t => t.min))), o.push(D(a, (t => t.max))), o[0] > 0 && o[1] > 0 ? o[0] = 0 : o[0] < 0 && o[1] < 0 && (o[1] = 0);
+                            const s = ai().domain(o).range([u, 0]);
+                            c.append("g").call(K(s));
+                            const p = Or().domain(i).range([0, l]).padding([.2]);
                             c.append("g").selectAll("g").data(r).enter().append("rect").attr("x", (function(t) {
                                 return p(t[e])
                             })).attr("y", (function(t) {
                                 return s(t[n]) < s(0) ? s(t[n]) : s(0)
                             })).attr("width", p.bandwidth()).attr("height", (function(t) {
                                 return Math.abs(s(0) - s(t[n]))
                             })).data(h).attr("fill", (function(t) {
@@ -3751,15 +3757,15 @@
                             }));
                             c.append("g").selectAll("g").data(m).enter().append("rect").attr("x", (function(t) {
                                 return p(t[e]) + p.bandwidth() / 2 - 1
                             })).attr("y", (function(t) {
                                 return s(t.max)
                             })).attr("width", 2).attr("height", (function(t) {
                                 return s(t.min) - s(t.max)
-                            })), c.append("g").style("font", "18px times").attr("transform", "translate(0," + s(0) + ")").call(D(p).tickSize(0))
+                            })), c.append("g").style("font", "18px times").attr("transform", "translate(0," + s(0) + ")").call(Z(p).tickSize(0))
                         }() : function() {
                             let i = t.reduce(((t, i) => {
                                 const o = i[e],
                                     a = i[n],
                                     s = i[r];
                                 if (o in t) {
                                     f[o].qt[n + "-" + s] += 1, f[o][s][n].push(a);
@@ -3785,30 +3791,30 @@
                                 return n = {
                                     ...n,
                                     ...i[t]
                                 }, n
                             })), Object.keys(f).forEach((t => {
                                 h.forEach((e => {
                                     const r = f[t][e][n],
-                                        [i, o] = fi(r);
+                                        [i, o] = Ai(r);
                                     f[t][e].min = i, f[t][e].max = o
                                 }))
                             }));
                             const o = h.map((t => n + "-" + t)),
                                 a = i.map((t => t[e])),
                                 s = [];
                             Object.keys(f).map((t => {
                                 h.forEach((e => s.push(f[t][e])))
                             }));
                             const p = [];
-                            p.push(k(s, (t => t.min))), p.push(M(s, (t => t.max))), p[0] > 0 && p[1] > 0 ? p[0] = 0 : p[0] < 0 && p[1] < 0 && (p[1] = 0);
-                            const m = Wr().domain(p).range([l, 0]);
-                            c.append("g").call(q(m));
-                            const _ = yr().domain(a).range([0, u]).padding([.2]),
-                                g = yr().domain(o).range([0, _.bandwidth()]).padding([.05]);
+                            p.push(I(s, (t => t.min))), p.push(D(s, (t => t.max))), p[0] > 0 && p[1] > 0 ? p[0] = 0 : p[0] < 0 && p[1] < 0 && (p[1] = 0);
+                            const m = ai().domain(p).range([u, 0]);
+                            c.append("g").call(K(m));
+                            const _ = Or().domain(a).range([0, l]).padding([.2]),
+                                g = Or().domain(o).range([0, _.bandwidth()]).padding([.05]);
                             c.append("g").selectAll("g").data(i).enter().append("g").attr("transform", (function(t) {
                                 return "translate(" + _(t[e]) + ",0)"
                             })).selectAll("rect").data((function(t) {
                                 return o.map((function(e) {
                                     return {
                                         key: e,
                                         value: t[e]
@@ -3845,19 +3851,19 @@
                                 return t.value.max ? m(t.value.max) : 0
                             })).attr("width", 2).attr("height", (function(t) {
                                 return t.value.min && t.value.max ? m(t.value.min) - m(t.value.max) : 0
                             }));
                             const y = c.selectAll(".legend").data(d.domain()).enter().append("g").attr("class", "legend").attr("transform", (function(t, e) {
                                 return "translate(0," + 20 * e + ")"
                             }));
-                            y.append("rect").attr("x", u - 18).attr("width", 18).attr("height", 18).style("fill", d), y.append("text").attr("x", u - 24).attr("y", 9).attr("dy", ".35em").style("text-anchor", "end").text((function(t) {
+                            y.append("rect").attr("x", l - 18).attr("width", 18).attr("height", 18).style("fill", d), y.append("text").attr("x", l - 24).attr("y", 9).attr("dy", ".35em").style("text-anchor", "end").text((function(t) {
                                 return t
-                            })), c.append("g").style("font", "18px times").attr("transform", "translate(0," + m(0) + ")").call(D(_).tickSize(0))
+                            })), c.append("g").style("font", "18px times").attr("transform", "translate(0," + m(0) + ")").call(Z(_).tickSize(0))
                         }()
-                    }(t, e, n, r, a, a.clientWidth, o, Ei)
+                    }(t, e, n, r, a, a.clientWidth, o, $i)
             }
         }
         class Di extends t.DOMWidgetModel {
             defaults() {
                 return {
                     ...super.defaults(),
                     _model_name: Di.model_name,
@@ -3870,74 +3876,74 @@
                     x: String,
                     start: Number,
                     end: Number,
                     elementId: String
                 }
             }
             static model_name = "HistogramplotModel";
-            static model_module = $i.name;
-            static model_module_version = $i.version;
+            static model_module = Ni.name;
+            static model_module_version = Ni.version;
             static view_name = "HistogramplotView";
-            static view_module = $i.name;
-            static view_module_version = $i.version
+            static view_module = Ni.name;
+            static view_module_version = Ni.version
         }
-        class qi extends t.DOMWidgetView {
+        class Ii extends t.DOMWidgetView {
             timeout;
             render() {
-                ji(this), this.model.on("change:data", (() => ji(this)), this), window.addEventListener("resize", (() => ji(this).bind(this)))
+                Ci(this), this.model.on("change:data", (() => Ci(this)), this), this.model.on("change:x", (() => Ci(this)), this), this.model.on("change:start", (() => Ci(this)), this), this.model.on("change:end", (() => Ci(this)), this), window.addEventListener("resize", (() => Ci(this)))
             }
             plot() {
                 const t = this.model.get("data"),
                     e = this.model.get("x"),
                     n = this.model.get("start"),
                     r = this.model.get("end"),
                     i = this.model.get("elementId");
                 let o = Si,
                     a = this.el;
                 i && (a = document.getElementById(i), o = a.clientHeight),
                     function(t, e, n, r, i, o, a, s) {
-                        const u = o - s.left - s.right,
-                            l = a - s.top - s.bottom;
-                        er(i).selectAll("*").remove();
+                        const l = o - s.left - s.right,
+                            u = a - s.top - s.bottom;
+                        mr(i).selectAll("*").remove();
                         let c = n;
-                        n || (c = k(t, (t => t[e])));
+                        n || (c = I(t, (t => t[e])));
                         let h = r;
-                        r || (h = M(t, (t => t[e])));
-                        const f = Wr().range([0, u]),
-                            d = Wr().range([l, 0]),
-                            p = D(f),
-                            m = q(d),
-                            _ = b().thresholds(40).value((t => Math.round(10 * t[e]) / 10))(t),
-                            g = er(i).append("svg").attr("width", o).attr("height", a).append("g").attr("transform", "translate(" + s.left + "," + s.top + ")");
-                        f.domain([c, h]), d.domain([0, M(_, (t => t.length))]), g.append("g").attr("transform", "translate(0," + l + ")").call(p).append("text").attr("x", u).attr("y", -6).style("text-anchor", "end"), g.append("g").call(m).append("text").attr("transform", "rotate(-90)").attr("y", 6).attr("dy", ".71em").style("text-anchor", "end"), g.append("g").attr("fill", "steelblue").selectAll().data(_).join("rect").attr("x", (t => f(t.x0) + 1)).attr("width", (t => f(t.x1) - f(t.x0) - 1)).attr("y", (t => d(t.length))).attr("height", (t => d(0) - d(t.length)))
-                    }(t, e, n, r, a, a.clientWidth, o, Ei)
+                        r || (h = D(t, (t => t[e])));
+                        const f = ai().range([0, l]),
+                            d = ai().range([u, 0]),
+                            p = Z(f),
+                            m = K(d),
+                            _ = L().thresholds(40).value((t => Math.round(10 * t[e]) / 10))(t),
+                            g = mr(i).append("svg").attr("width", o).attr("height", a).append("g").attr("transform", "translate(" + s.left + "," + s.top + ")");
+                        f.domain([c, h]), d.domain([0, D(_, (t => t.length))]), g.append("g").attr("transform", "translate(0," + u + ")").call(p).append("text").attr("x", l).attr("y", -6).style("text-anchor", "end"), g.append("g").call(m).append("text").attr("transform", "rotate(-90)").attr("y", 6).attr("dy", ".71em").style("text-anchor", "end"), g.append("g").attr("fill", "steelblue").selectAll().data(_).join("rect").attr("x", (t => f(t.x0) + 1)).attr("width", (t => f(t.x1) - f(t.x0) - 1)).attr("y", (t => d(t.length))).attr("height", (t => d(0) - d(t.length)))
+                    }(t, e, n, r, a, a.clientWidth, o, $i)
             }
         }
-        class Li extends t.DOMWidgetModel {
+        class qi extends t.DOMWidgetModel {
             defaults() {
                 return {
                     ...super.defaults(),
-                    _model_name: Li.model_name,
-                    _view_name: Li.view_name,
-                    _model_module: Li.model_module,
-                    _view_module: Li.view_module,
-                    _model_module_version: Li.model_module_version,
-                    _view_module_version: Li.view_module_version,
+                    _model_name: qi.model_name,
+                    _view_name: qi.view_name,
+                    _model_module: qi.model_module,
+                    _view_module: qi.view_module,
+                    _model_module_version: qi.model_module_version,
+                    _view_module_version: qi.view_module_version,
                     matrix: [],
                     grid_areas: [],
                     grid_template_areas: String,
                     style: String
                 }
             }
             static model_name = "EmbeddingModel";
-            static model_module = $i.name;
-            static model_module_version = $i.version;
+            static model_module = Ni.name;
+            static model_module_version = Ni.version;
             static view_name = "EmbeddingView";
-            static view_module = $i.name;
-            static view_module_version = $i.version
+            static view_module = Ni.name;
+            static view_module_version = Ni.version
         }
         class Hi extends t.DOMWidgetView {
             render() {
                 this.value_changed()
             }
             value_changed() {
                 const t = this.model.get("matrix"),
@@ -3948,10 +3954,95 @@
                 const i = document.createElement("div");
                 i.classList.add(r), i.style.display = "grid", i.style.gridTemplateAreas = n, i.style.gridTemplateRows = "repeat(" + t.length + ", 20vh)", i.style.gridTemplateColumns = "repeat(" + t[0].length + ", 1fr)", i.style.width = "100%", e.forEach((t => {
                     const e = document.createElement("div");
                     e.setAttribute("id", t), e.style.gridArea = t, e.classList.add("dashboard-div"), i.appendChild(e)
                 })), this.el.appendChild(i)
             }
         }
-        var Xi = i(330)
+        class zi extends t.DOMWidgetModel {
+            defaults() {
+                return {
+                    ...super.defaults(),
+                    _model_name: zi.model_name,
+                    _view_name: zi.view_name,
+                    _model_module: zi.model_module,
+                    _view_module: zi.view_module,
+                    _model_module_version: zi.model_module_version,
+                    _view_module_version: zi.view_module_version,
+                    data: [],
+                    variable: String,
+                    step: Number,
+                    description: String,
+                    minValue: Number,
+                    maxValue: Number,
+                    elementId: String
+                }
+            }
+            static model_name = "RangeSliderModel";
+            static model_module = Ni.name;
+            static model_module_version = Ni.version;
+            static view_name = "RangeSliderView";
+            static view_module = Ni.name;
+            static view_module_version = Ni.version
+        }
+        class Xi extends t.DOMWidgetView {
+            render() {
+                Ci(this), this.model.on("change:data", (() => Ci(this)), this), this.model.on("change:variable", (() => Ci(this)), this), this.model.on("change:step", (() => Ci(this)), this), this.model.on("change:description", (() => Ci(this)), this), window.addEventListener("resize", (() => Ci(this)))
+            }
+            plot() {
+                const t = this.model.get("data"),
+                    e = this.model.get("variable"),
+                    n = this.model.get("step"),
+                    r = this.model.get("description"),
+                    i = this.model.get("elementId"),
+                    o = this.model.get("minValue"),
+                    a = this.model.get("maxValue");
+                let s = this.el;
+                i && (s = document.getElementById(i));
+                const l = $i;
+                ! function(t, e, n, r, i, o, a, s, l) {
+                    const u = document.createElement("div");
+                    u.classList.add("range_outside_container"), u.style.margin = l.top + "px " + l.right + "px " + l.bottom + "px " + l.left + "px";
+                    const c = document.createElement("span");
+                    c.classList.add("range_description"), c.textContent = r, u.appendChild(c);
+                    const h = document.createElement("div");
+                    h.classList.add("range_inside_container"), u.appendChild(h);
+                    const f = document.createElement("span");
+                    f.classList.add("range_value"), u.appendChild(f);
+                    const d = document.createElement("div");
+                    d.classList.add("sliders_control"), h.appendChild(d);
+                    const p = document.createElement("input");
+                    p.classList.add("top_slider"), p.setAttribute("step", n), p.setAttribute("type", "range"), d.appendChild(p);
+                    const m = document.createElement("input");
+
+                    function _(t, e) {
+                        f.textContent = t + " - " + e, a(t, e)
+                    }
+                    m.setAttribute("step", n), m.setAttribute("type", "range"), d.appendChild(m);
+                    const g = I(t, (t => t[e])),
+                        v = D(t, (t => t[e]));
+                    p.setAttribute("min", g), p.setAttribute("max", v), m.setAttribute("min", g), m.setAttribute("max", v), i && o ? (p.value = i, m.value = o) : (p.value = g, m.value = v), _(parseFloat(p.value), parseFloat(m.value)), p.addEventListener("input", (() => {
+                        const t = parseFloat(p.value),
+                            e = parseFloat(m.value);
+                        t > e && (p.value = m.value), _(t, e)
+                    })), m.addEventListener("input", (() => {
+                        const t = parseFloat(p.value),
+                            e = parseFloat(m.value);
+                        e < t && (m.value = p.value), _(t, e)
+                    })), p.addEventListener("click", (() => {
+                        p.classList.add("top_slider"), m.classList.remove("top_slider")
+                    })), m.addEventListener("click", (() => {
+                        m.classList.add("top_slider"), p.classList.remove("top_slider")
+                    })), s.innerHTML = "", s.appendChild(u)
+                }(t, e, n, r, o, a, this.setValues.bind(this), s, l)
+            }
+            setValues(t, e) {
+                this.model.set({
+                    minValue: t
+                }), this.model.set({
+                    maxValue: e
+                }), this.model.save_changes()
+            }
+        }
+        var Ri = i(330)
     })(), o
 })()));
```

### Comparing `d3vis_ipynb-0.1.2/js/amd-public-path.js` & `d3vis_ipynb-0.1.3/js/amd-public-path.js`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.1.2/js/package.json` & `d3vis_ipynb-0.1.3/js/package.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9615384615384616%*

 * *Differences: {"'version'": "'0.1.3'"}*

```diff
@@ -50,9 +50,9 @@
         "export": "webpack --env export --config webpack.exports.config.js",
         "prepublish": "yarn run clean && yarn run build:prod",
         "start": "webpack serve --open --config webpack.exports.config.js",
         "start:export": "webpack serve --open --config webpack.exports.config.js --env export",
         "test": "echo \"Error: no test specified\" && exit 1",
         "watch": "webpack --watch --mode=development"
     },
-    "version": "0.1.2"
+    "version": "0.1.3"
 }
```

### Comparing `d3vis_ipynb-0.1.2/js/webpack.config.js` & `d3vis_ipynb-0.1.3/js/webpack.config.js`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.1.2/js/webpack.exports.config.js` & `d3vis_ipynb-0.1.3/js/webpack.exports.config.js`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.1.2/js/lib/labplugin.js` & `d3vis_ipynb-0.1.3/js/lib/labplugin.js`

 * *Files 20% similar despite different names*

#### js-beautify {}

```diff
@@ -1,23 +1,25 @@
 import {
-    LinearHistPlotModel,
-    LinearHistPlotView,
-    ScatterPlotModel,
-    ScatterPlotView,
+    IJupyterWidgetRegistry
+} from "@jupyter-widgets/base";
+import {
     BarPlotModel,
     BarPlotView,
-    HistogramPlotModel,
-    HistogramPlotView,
     EmbeddingModel,
     EmbeddingView,
+    HistogramPlotModel,
+    HistogramPlotView,
+    LinearHistPlotModel,
+    LinearHistPlotView,
+    RangeSliderModel,
+    RangeSliderView,
+    ScatterPlotModel,
+    ScatterPlotView,
     version,
 } from "./index";
-import {
-    IJupyterWidgetRegistry
-} from "@jupyter-widgets/base";
 
 export const helloWidgetPlugin = {
     id: "d3vis_ipynb:plugin",
     requires: [IJupyterWidgetRegistry],
     activate: function(app, widgets) {
         widgets.registerWidget({
             name: "d3vis_ipynb",
@@ -29,14 +31,16 @@
                 ScatterPlotView,
                 BarPlotModel,
                 BarPlotView,
                 HistogramPlotModel,
                 HistogramPlotView,
                 EmbeddingModel,
                 EmbeddingView,
+                RangeSliderModel,
+                RangeSliderView,
             },
         });
     },
     autoStart: true,
 };
 
 export default helloWidgetPlugin;
```

### Comparing `d3vis_ipynb-0.1.2/js/lib/web-dev.js` & `d3vis_ipynb-0.1.3/js/lib/web-dev.js`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.1.2/js/lib/widgets.js` & `d3vis_ipynb-0.1.3/js/lib/widgets.js`

 * *Files 22% similar despite different names*

#### js-beautify {}

```diff
@@ -1,24 +1,27 @@
 import {
     DOMWidgetModel,
     DOMWidgetView
 } from "@jupyter-widgets/base";
-import {
-    linearhistplot
-} from "./graphs/linearhistplot";
-import {
-    scatterplot
-} from "./graphs/scatterplot";
+import "../css/widget.css";
 import {
     barplot
 } from "./graphs/barplot";
 import {
     histogramplot
 } from "./graphs/histogramplot";
-import "../css/widget.css";
+import {
+    linearhistplot
+} from "./graphs/linearhistplot";
+import {
+    rangeslider
+} from "./graphs/rangeslider";
+import {
+    scatterplot
+} from "./graphs/scatterplot";
 const data = require("../package.json");
 
 const WIDGET_HEIGHT = 400;
 const WIDGET_MARGIN = {
     top: 20,
     right: 20,
     bottom: 30,
@@ -65,15 +68,17 @@
 export class LinearHistPlotView extends DOMWidgetView {
     timeout;
 
     render() {
         plotAfterInterval(this);
 
         this.model.on("change:linearData_x", () => plotAfterInterval(this), this);
-        window.addEventListener("resize", () => plotAfterInterval(this).bind(this));
+        this.model.on("change:linearData_y", () => plotAfterInterval(this), this);
+        this.model.on("change:histogramData", () => plotAfterInterval(this), this);
+        window.addEventListener("resize", () => plotAfterInterval(this));
     }
 
     plot() {
         const linearData_x = this.model.get("linearData_x");
         const linearData_y = this.model.get("linearData_y");
         const histogramData = this.model.get("histogramData");
         const elementId = this.model.get("elementId");
@@ -139,15 +144,18 @@
 export class ScatterPlotView extends DOMWidgetView {
     timeout;
 
     render() {
         plotAfterInterval(this);
 
         this.model.on("change:data", () => plotAfterInterval(this), this);
-        window.addEventListener("resize", () => plotAfterInterval(this).bind(this));
+        this.model.on("change:x", () => plotAfterInterval(this), this);
+        this.model.on("change:y", () => plotAfterInterval(this), this);
+        this.model.on("change:hue", () => plotAfterInterval(this), this);
+        window.addEventListener("resize", () => plotAfterInterval(this));
     }
 
     plot() {
         const data = this.model.get("data");
         const x = this.model.get("x");
         const y = this.model.get("y");
         const hue = this.model.get("hue");
@@ -221,15 +229,18 @@
 export class BarPlotView extends DOMWidgetView {
     timeout;
 
     render() {
         plotAfterInterval(this);
 
         this.model.on("change:data", () => plotAfterInterval(this), this);
-        window.addEventListener("resize", () => plotAfterInterval(this).bind(this));
+        this.model.on("change:x", () => plotAfterInterval(this), this);
+        this.model.on("change:y", () => plotAfterInterval(this), this);
+        this.model.on("change:hue", () => plotAfterInterval(this), this);
+        window.addEventListener("resize", () => plotAfterInterval(this));
     }
 
     plot() {
         const data = this.model.get("data");
         const x = this.model.get("x");
         const y = this.model.get("y");
         const hue = this.model.get("hue");
@@ -278,15 +289,18 @@
 export class HistogramPlotView extends DOMWidgetView {
     timeout;
 
     render() {
         plotAfterInterval(this);
 
         this.model.on("change:data", () => plotAfterInterval(this), this);
-        window.addEventListener("resize", () => plotAfterInterval(this).bind(this));
+        this.model.on("change:x", () => plotAfterInterval(this), this);
+        this.model.on("change:start", () => plotAfterInterval(this), this);
+        this.model.on("change:end", () => plotAfterInterval(this), this);
+        window.addEventListener("resize", () => plotAfterInterval(this));
     }
 
     plot() {
         const data = this.model.get("data");
         const x = this.model.get("x");
         const start = this.model.get("start");
         const end = this.model.get("end");
@@ -361,8 +375,87 @@
             grid_area.style.gridArea = area;
             grid_area.classList.add("dashboard-div");
             node.appendChild(grid_area);
         });
 
         this.el.appendChild(node);
     }
+}
+
+export class RangeSliderModel extends DOMWidgetModel {
+    defaults() {
+        return {
+            ...super.defaults(),
+            _model_name: RangeSliderModel.model_name,
+            _view_name: RangeSliderModel.view_name,
+            _model_module: RangeSliderModel.model_module,
+            _view_module: RangeSliderModel.view_module,
+            _model_module_version: RangeSliderModel.model_module_version,
+            _view_module_version: RangeSliderModel.view_module_version,
+
+            data: [],
+            variable: String,
+            step: Number,
+            description: String,
+            minValue: Number,
+            maxValue: Number,
+            elementId: String,
+        };
+    }
+
+    static model_name = "RangeSliderModel";
+    static model_module = data.name;
+    static model_module_version = data.version;
+    static view_name = "RangeSliderView"; // Set to null if no view
+    static view_module = data.name; // Set to null if no view
+    static view_module_version = data.version;
+}
+
+export class RangeSliderView extends DOMWidgetView {
+    render() {
+        plotAfterInterval(this);
+
+        this.model.on("change:data", () => plotAfterInterval(this), this);
+        this.model.on("change:variable", () => plotAfterInterval(this), this);
+        this.model.on("change:step", () => plotAfterInterval(this), this);
+        this.model.on("change:description", () => plotAfterInterval(this), this);
+        window.addEventListener("resize", () => plotAfterInterval(this));
+    }
+
+    plot() {
+        const data = this.model.get("data");
+        const variable = this.model.get("variable");
+        const step = this.model.get("step");
+        const description = this.model.get("description");
+        const elementId = this.model.get("elementId");
+        const minValue = this.model.get("minValue");
+        const maxValue = this.model.get("maxValue");
+
+        let element = this.el;
+        if (elementId) {
+            element = document.getElementById(elementId);
+        }
+        const margin = WIDGET_MARGIN;
+
+        rangeslider(
+            data,
+            variable,
+            step,
+            description,
+            minValue,
+            maxValue,
+            this.setValues.bind(this),
+            element,
+            margin
+        );
+    }
+
+    setValues(min, max) {
+        this.model.set({
+            minValue: min
+        });
+        this.model.set({
+            maxValue: max
+        });
+        this.model.save_changes();
+    }
 }
```

### Comparing `d3vis_ipynb-0.1.2/js/lib/graphs/barplot.js` & `d3vis_ipynb-0.1.3/js/lib/graphs/barplot.js`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.1.2/js/lib/graphs/histogramplot.js` & `d3vis_ipynb-0.1.3/js/lib/graphs/histogramplot.js`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.1.2/js/lib/graphs/linearhistplot.js` & `d3vis_ipynb-0.1.3/js/lib/graphs/linearhistplot.js`

 * *Files 10% similar despite different names*

#### js-beautify {}

```diff
@@ -109,14 +109,22 @@
         .call(yAxis)
         .append("text")
         .attr("transform", "rotate(-90)")
         .attr("y", 6)
         .attr("dy", ".71em")
         .style("text-anchor", "end");
 
+    const firstPathPoint = []
+    firstPathPoint['x0'] = bins[0]['x0'] - 2.5
+    firstPathPoint['x1'] = bins[0]['x1'] - 2.5
+    bins.unshift(firstPathPoint)
+    const lastPathPoint = []
+    lastPathPoint['x0'] = bins[bins.length - 1]['x0'] + 2.5
+    lastPathPoint['x1'] = bins[bins.length - 1]['x1'] + 2.5
+
     svg
         .append("path")
         .datum(bins)
         .attr("fill", "paleturquoise")
         .attr("stroke", "steelblue")
         .attr("stroke-width", 1)
         .attr(
```

### Comparing `d3vis_ipynb-0.1.2/js/lib/graphs/scatterplot.js` & `d3vis_ipynb-0.1.3/js/lib/graphs/scatterplot.js`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.1.2/js/lib/tools/lasso.js` & `d3vis_ipynb-0.1.3/js/lib/tools/lasso.js`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.1.2/js/lib/wrappers/embedding.wrapper.js` & `d3vis_ipynb-0.1.3/js/lib/wrappers/embedding.wrapper.js`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.1.2/LICENSE.txt` & `d3vis_ipynb-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.1.2/README.md` & `d3vis_ipynb-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.1.2/pyproject.toml` & `d3vis_ipynb-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     "Programming Language :: Python :: 3.12",
 ]
 dependencies = [
     "ipywidgets>=7.7.1",
     "simplejson >=3.19.0",
     "anywidget >= 0.9.6"
 ]
-version = "0.1.2"
+version = "0.1.3"
 
 [project.optional-dependencies]
 docs = [
     "jupyter_sphinx",
     "nbsphinx",
     "nbsphinx-link",
     "pypandoc",
@@ -78,14 +78,15 @@
 "./install.json" = "share/jupyter/labextensions/d3vis_ipynb/install.json"
 "./d3vis_ipynb.json" = "etc/jupyter/nbconfig/notebook.d/d3vis_ipynb.json"
 
 [tool.hatch.build.targets.sdist]
 exclude = [
     ".github",
     "samples",
+    "examples",
 ]
 
 [tool.hatch.build.hooks.jupyter-builder]
 build-function = "hatch_jupyter_builder.npm_builder"
 ensured-targets = [
     "d3vis_ipynb/nbextension/index.js",
     "d3vis_ipynb/labextension/package.json",
```

### Comparing `d3vis_ipynb-0.1.2/PKG-INFO` & `d3vis_ipynb-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: d3vis_ipynb
-Version: 0.1.2
+Version: 0.1.3
 Summary: A Custom Jupyter Widget Library with visualizations created with D3.js.
 Project-URL: Homepage, https://github.com/H-IAAC/d3vis_ipynb
 Author-email: Daniel Adam Miranda <daniel.miranda@eldorado.org.br>
 License: Copyright (c) 2024 Daniel Adam Miranda
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
```


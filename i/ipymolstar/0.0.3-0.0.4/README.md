# Comparing `tmp/ipymolstar-0.0.3.tar.gz` & `tmp/ipymolstar-0.0.4.tar.gz`

## Comparing `ipymolstar-0.0.3.tar` & `ipymolstar-0.0.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 ipymolstar-0.0.3/src/ipymolstar/__init__.py
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 ipymolstar-0.0.3/src/ipymolstar/pdbe-dark.css
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 ipymolstar-0.0.3/src/ipymolstar/pdbe-light.css
--rw-r--r--   0        0        0     8633 2020-02-02 00:00:00.000000 ipymolstar-0.0.3/src/ipymolstar/widget.js
--rw-r--r--   0        0        0     6048 2020-02-02 00:00:00.000000 ipymolstar-0.0.3/src/ipymolstar/widget.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 ipymolstar-0.0.3/.gitignore
--rw-r--r--   0        0        0     1485 2020-02-02 00:00:00.000000 ipymolstar-0.0.3/README.md
--rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 ipymolstar-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 ipymolstar-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 ipymolstar-0.0.4/src/ipymolstar/__init__.py
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 ipymolstar-0.0.4/src/ipymolstar/pdbe-dark.css
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 ipymolstar-0.0.4/src/ipymolstar/pdbe-light.css
+-rw-r--r--   0        0        0     7959 2020-02-02 00:00:00.000000 ipymolstar-0.0.4/src/ipymolstar/widget.js
+-rw-r--r--   0        0        0     6103 2020-02-02 00:00:00.000000 ipymolstar-0.0.4/src/ipymolstar/widget.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 ipymolstar-0.0.4/.gitignore
+-rw-r--r--   0        0        0     4816 2020-02-02 00:00:00.000000 ipymolstar-0.0.4/README.md
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 ipymolstar-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     5040 2020-02-02 00:00:00.000000 ipymolstar-0.0.4/PKG-INFO
```

### Comparing `ipymolstar-0.0.3/src/ipymolstar/widget.js` & `ipymolstar-0.0.4/src/ipymolstar/widget.js`

 * *Files 16% similar despite different names*

#### js-beautify {}

```diff
@@ -73,18 +73,30 @@
     if (model.get("hide_animation_icon")) {
         hideCanvasControls.push("animation");
     }
 
     return hideCanvasControls;
 }
 
+function getCustomData(model) {
+    var customData = model.get("custom_data");
+
+    if (customData && 'data' in customData) {
+        var url = URL.createObjectURL(new Blob([customData.data]));
+        customData.url = url;
+        delete customData.data;
+    }
+
+    return customData;
+}
+
 function getOptions(model) {
     var options = {
         moleculeId: model.get("molecule_id"),
-        customData: model.get("custom_data"),
+        customData: getCustomData(model),
         assemblyId: model.get("assembly_id"),
         defaultPreset: model.get("default_preset"),
         ligandView: model.get("ligand_view"),
         alphafoldView: model.get("alphafold_view"),
         superposition: model.get("superposition"),
         superpositionParams: model.get("superposition_params"),
         visualStyle: model.get("visual_style"),
@@ -178,50 +190,55 @@
         },
         "change:custom_data": () => {
             viewerInstance.visual.update(getOptions(model), true);
         },
         "change:bg_color": () => {
             viewerInstance.canvas.setBgColor(toRgb(model.get("bg_color")));
         },
+        "change:_reset": () => {
+            const resetValue = model.get("_reset");
+            if (resetValue !== null) {
+                viewerInstance.visual.reset(resetValue);
+            }
+        },
     };
 
     let combinedCallbacks = Object.assign({},
         callbacksLoadComplete,
         otherCallbacks
     );
 
     viewerInstance.events.loadComplete.subscribe(() => {
-        // trigger callabacks which need to
+        // trigger callabacks which need to be called after loading
         Object.values(callbacksLoadComplete).forEach((callback) => callback());
     });
 
     // subscribe to events and collect unsubscribe funcs
     let unsubscribes = Object.entries(combinedCallbacks).map(([name, callback]) =>
         subscribe(model, name, callback)
     );
 
+    document.addEventListener("PDB.molstar.mouseover", (e) => {
+        const eventData = e.eventData;
+        model.set("mouseover_event", eventData);
+        model.save_changes();
+    });
+
     // TODO return unsubscribe
 
     // these require re-render
     // model.on("change:visual_style", () => {
     //     viewerInstance.visual.update({visualStyle: model.get('visual_style')});
     //     console.log(model.get('visual_style'));
     // });
 
     // model.on("change:lighting", () => {
     //     viewerInstance.visual.update({lighting: model.get('lighting')});
     // });
 
-    // model.on("change:color_data", () => {
-    //     const selectValue = model.get("color_data");
-    //     if (selectValue !== null) {
-    //         viewerInstance.visual.select(selectValue);
-    //     }
-    // });
-
     // model.on("change:_focus", () => {
     //   const focusValue = model.get("_focus");
     //   if (focusValue !== null) {
     //     viewerInstance.visual.focus(focusValue);
     //   }
     // });
     // model.on("change:_highlight", () => {
@@ -233,48 +250,21 @@
     // model.on("change:_clear_highlight", () => {
     //   1;
     //   viewerInstance.visual.clearHighlight();
     // });
     // model.on("change:_clear_selection", () => {
     //   viewerInstance.visual.clearSelection(model.get("_args")["number"]);
     // });
-    // model.on("change:_reset", () => {
-    //   const resetValue = model.get("_reset");
-    //   if (resetValue !== null) {
-    //     viewerInstance.visual.reset(resetValue);
-    //   }
     // });
     // model.on("change:_update", () => {
     //   const updateValue = model.get("_update");
     //   if (updateValue !== null) {
     //     viewerInstance.visual.update(updateValue);
     //   }
-    // });
-    //   model.on("change:molecule_id", () => {
-    //     viewerInstance.visual.update(getOptions(model), true);
-    //   });
-    // model.on("change:spin", () => {
-    //   viewerInstance.visual.toggleSpin(model.get("spin"));
-    // });
-    // model.on("change:hide_polymer", () => {
-    //   viewerInstance.visual.visibility({ water: !model.get("hide_polymer") });
-    // });
-    // model.on("change:hide_water", () => {
-    //     viewerInstance.visual.visibility({water:!model.get('hide_water')});
-    // });
-    // model.on("change:hide_heteroatoms", () => {
-    //   viewerInstance.visual.visibility({ water: !model.get("hide_heteroatoms") });
-    // });
-    // model.on("change:hide_carbs", () => {
-    //   viewerInstance.visual.visibility({ water: !model.get("hide_carbs") });
-    // });
-    // model.on("change:hide_non_standard", () => {
-    //   viewerInstance.visual.visibility({
-    //     water: !model.get("hide_non_standard"),
-    //   });
+
     // });
     // model.on("change:hide_coarse", () => {
     //   viewerInstance.visual.visibility({ water: !model.get("hide_coarse") });
     // });
 
     // this could be a loop?
     return () => {
```

### Comparing `ipymolstar-0.0.3/src/ipymolstar/widget.py` & `ipymolstar-0.0.4/src/ipymolstar/widget.py`

 * *Files 0% similar despite different names*

```diff
@@ -111,14 +111,16 @@
     _clear_selection = traitlets.Bool(default_value=False).tag(sync=True)
     _set_color = traitlets.Dict(default_value=None, allow_none=True).tag(sync=True)
     _reset = traitlets.Dict(allow_none=True, default_value=None).tag(sync=True)
     _update = traitlets.Dict(allow_none=True, default_value=None).tag(sync=True)
 
     _args = traitlets.Dict().tag(sync=True)
 
+    mouseover_event = traitlets.Dict().tag(sync=True)
+
     def __init__(self, theme="light", **kwargs):
         _css = THEMES[theme]["css"]
         bg_color = kwargs.pop("bg_color", THEMES[theme]["bg_color"])
         super().__init__(_css=_css, bg_color=bg_color, **kwargs)
 
     def color(self, data, non_selected_color=None):
         """
```


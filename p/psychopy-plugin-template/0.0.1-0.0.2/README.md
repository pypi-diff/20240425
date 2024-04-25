# Comparing `tmp/psychopy_plugin_template-0.0.1.tar.gz` & `tmp/psychopy_plugin_template-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psychopy_plugin_template-0.0.1.tar", last modified: Thu Apr 25 12:58:56 2024, max compression
+gzip compressed data, was "psychopy_plugin_template-0.0.2.tar", last modified: Thu Apr 25 13:43:47 2024, max compression
```

## Comparing `psychopy_plugin_template-0.0.1.tar` & `psychopy_plugin_template-0.0.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2024-04-25 12:58:56.469754 psychopy_plugin_template-0.0.1/
--rw-rw-rw-   0        0        0      661 2024-04-25 12:58:56.468754 psychopy_plugin_template-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-04-04 13:49:56.000000 psychopy_plugin_template-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-25 12:58:56.433875 psychopy_plugin_template-0.0.1/psychopy-plugin-template/
--rw-rw-rw-   0        0        0        0 2024-04-04 13:53:25.000000 psychopy_plugin_template-0.0.1/psychopy-plugin-template/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-25 12:58:56.434875 psychopy_plugin_template-0.0.1/psychopy-plugin-template/components/
--rw-rw-rw-   0        0        0        0 2024-04-04 13:52:44.000000 psychopy_plugin_template-0.0.1/psychopy-plugin-template/components/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-25 12:58:56.435876 psychopy_plugin_template-0.0.1/psychopy-plugin-template/components/exampleComponent/
--rw-rw-rw-   0        0        0     6696 2024-04-25 12:39:02.000000 psychopy_plugin_template-0.0.1/psychopy-plugin-template/components/exampleComponent/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-25 12:58:56.438112 psychopy_plugin_template-0.0.1/psychopy-plugin-template/components/exampleComponent/classic/
--rw-rw-rw-   0        0        0     3612 2024-04-25 12:39:02.000000 psychopy_plugin_template-0.0.1/psychopy-plugin-template/components/exampleComponent/classic/example.png
--rw-rw-rw-   0        0        0     9490 2024-04-25 12:39:02.000000 psychopy_plugin_template-0.0.1/psychopy-plugin-template/components/exampleComponent/classic/example@2x.png
-drwxrwxrwx   0        0        0        0 2024-04-25 12:58:56.440050 psychopy_plugin_template-0.0.1/psychopy-plugin-template/components/exampleComponent/dark/
--rw-rw-rw-   0        0        0     1706 2024-04-25 12:39:02.000000 psychopy_plugin_template-0.0.1/psychopy-plugin-template/components/exampleComponent/dark/example.png
--rw-rw-rw-   0        0        0     2926 2024-04-25 12:39:02.000000 psychopy_plugin_template-0.0.1/psychopy-plugin-template/components/exampleComponent/dark/example@2x.png
-drwxrwxrwx   0        0        0        0 2024-04-25 12:58:56.442061 psychopy_plugin_template-0.0.1/psychopy-plugin-template/components/exampleComponent/light/
--rw-rw-rw-   0        0        0     1706 2024-04-25 12:39:02.000000 psychopy_plugin_template-0.0.1/psychopy-plugin-template/components/exampleComponent/light/example.png
--rw-rw-rw-   0        0        0     2926 2024-04-25 12:39:02.000000 psychopy_plugin_template-0.0.1/psychopy-plugin-template/components/exampleComponent/light/example@2x.png
-drwxrwxrwx   0        0        0        0 2024-04-25 12:58:56.445207 psychopy_plugin_template-0.0.1/psychopy-plugin-template/hardware/
--rw-rw-rw-   0        0        0       70 2024-04-05 14:36:07.000000 psychopy_plugin_template-0.0.1/psychopy-plugin-template/hardware/__init__.py
--rw-rw-rw-   0        0        0      480 2024-04-11 09:28:38.000000 psychopy_plugin_template-0.0.1/psychopy-plugin-template/hardware/exampleDevice.py
--rw-rw-rw-   0        0        0     1040 2024-04-11 09:28:38.000000 psychopy_plugin_template-0.0.1/psychopy-plugin-template/hardware/exampleResponseDevice.py
-drwxrwxrwx   0        0        0        0 2024-04-25 12:58:56.446207 psychopy_plugin_template-0.0.1/psychopy-plugin-template/routines/
--rw-rw-rw-   0        0        0        0 2024-04-04 13:52:44.000000 psychopy_plugin_template-0.0.1/psychopy-plugin-template/routines/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-25 12:58:56.446207 psychopy_plugin_template-0.0.1/psychopy-plugin-template/routines/exampleStandaloneRoutine/
--rw-rw-rw-   0        0        0      409 2024-04-05 11:25:28.000000 psychopy_plugin_template-0.0.1/psychopy-plugin-template/routines/exampleStandaloneRoutine/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-25 12:58:56.448208 psychopy_plugin_template-0.0.1/psychopy-plugin-template/visual/
--rw-rw-rw-   0        0        0        0 2024-04-04 14:20:58.000000 psychopy_plugin_template-0.0.1/psychopy-plugin-template/visual/__init__.py
--rw-rw-rw-   0        0        0     2147 2024-04-25 12:39:02.000000 psychopy_plugin_template-0.0.1/psychopy-plugin-template/visual/exampleVisualStim.py
-drwxrwxrwx   0        0        0        0 2024-04-25 12:58:56.467753 psychopy_plugin_template-0.0.1/psychopy_plugin_template.egg-info/
--rw-rw-rw-   0        0        0      661 2024-04-25 12:58:56.000000 psychopy_plugin_template-0.0.1/psychopy_plugin_template.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1271 2024-04-25 12:58:56.000000 psychopy_plugin_template-0.0.1/psychopy_plugin_template.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-25 12:58:56.000000 psychopy_plugin_template-0.0.1/psychopy_plugin_template.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      568 2024-04-25 12:58:56.000000 psychopy_plugin_template-0.0.1/psychopy_plugin_template.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       54 2024-04-25 12:58:56.000000 psychopy_plugin_template-0.0.1/psychopy_plugin_template.egg-info/requires.txt
--rw-rw-rw-   0        0        0       30 2024-04-25 12:58:56.000000 psychopy_plugin_template-0.0.1/psychopy_plugin_template.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2444 2024-04-25 12:58:44.000000 psychopy_plugin_template-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-25 12:58:56.469754 psychopy_plugin_template-0.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:43:47.744127 psychopy_plugin_template-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-25 13:43:47.744127 psychopy_plugin_template-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 13:43:36.000000 psychopy_plugin_template-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:43:47.740127 psychopy_plugin_template-0.0.2/psychopy_plugin_template/
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-25 13:43:36.000000 psychopy_plugin_template-0.0.2/psychopy_plugin_template/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:43:47.744127 psychopy_plugin_template-0.0.2/psychopy_plugin_template/components/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 13:43:36.000000 psychopy_plugin_template-0.0.2/psychopy_plugin_template/components/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:43:47.744127 psychopy_plugin_template-0.0.2/psychopy_plugin_template/components/exampleComponent/
+-rw-r--r--   0 runner    (1001) docker     (127)     6537 2024-04-25 13:43:36.000000 psychopy_plugin_template-0.0.2/psychopy_plugin_template/components/exampleComponent/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:43:47.744127 psychopy_plugin_template-0.0.2/psychopy_plugin_template/components/exampleComponent/classic/
+-rw-r--r--   0 runner    (1001) docker     (127)     3612 2024-04-25 13:43:36.000000 psychopy_plugin_template-0.0.2/psychopy_plugin_template/components/exampleComponent/classic/example.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9490 2024-04-25 13:43:36.000000 psychopy_plugin_template-0.0.2/psychopy_plugin_template/components/exampleComponent/classic/example@2x.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:43:47.744127 psychopy_plugin_template-0.0.2/psychopy_plugin_template/components/exampleComponent/dark/
+-rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-04-25 13:43:36.000000 psychopy_plugin_template-0.0.2/psychopy_plugin_template/components/exampleComponent/dark/example.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-04-25 13:43:36.000000 psychopy_plugin_template-0.0.2/psychopy_plugin_template/components/exampleComponent/dark/example@2x.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:43:47.744127 psychopy_plugin_template-0.0.2/psychopy_plugin_template/components/exampleComponent/light/
+-rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-04-25 13:43:36.000000 psychopy_plugin_template-0.0.2/psychopy_plugin_template/components/exampleComponent/light/example.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-04-25 13:43:36.000000 psychopy_plugin_template-0.0.2/psychopy_plugin_template/components/exampleComponent/light/example@2x.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:43:47.744127 psychopy_plugin_template-0.0.2/psychopy_plugin_template/hardware/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-25 13:43:36.000000 psychopy_plugin_template-0.0.2/psychopy_plugin_template/hardware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-25 13:43:36.000000 psychopy_plugin_template-0.0.2/psychopy_plugin_template/hardware/exampleDevice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-04-25 13:43:36.000000 psychopy_plugin_template-0.0.2/psychopy_plugin_template/hardware/exampleResponseDevice.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:43:47.744127 psychopy_plugin_template-0.0.2/psychopy_plugin_template/routines/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 13:43:36.000000 psychopy_plugin_template-0.0.2/psychopy_plugin_template/routines/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:43:47.744127 psychopy_plugin_template-0.0.2/psychopy_plugin_template/routines/exampleStandaloneRoutine/
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-25 13:43:36.000000 psychopy_plugin_template-0.0.2/psychopy_plugin_template/routines/exampleStandaloneRoutine/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:43:47.744127 psychopy_plugin_template-0.0.2/psychopy_plugin_template/visual/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 13:43:36.000000 psychopy_plugin_template-0.0.2/psychopy_plugin_template/visual/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2094 2024-04-25 13:43:36.000000 psychopy_plugin_template-0.0.2/psychopy_plugin_template/visual/exampleVisualStim.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:43:47.744127 psychopy_plugin_template-0.0.2/psychopy_plugin_template.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-25 13:43:47.000000 psychopy_plugin_template-0.0.2/psychopy_plugin_template.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-04-25 13:43:47.000000 psychopy_plugin_template-0.0.2/psychopy_plugin_template.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 13:43:47.000000 psychopy_plugin_template-0.0.2/psychopy_plugin_template.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-25 13:43:47.000000 psychopy_plugin_template-0.0.2/psychopy_plugin_template.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-25 13:43:47.000000 psychopy_plugin_template-0.0.2/psychopy_plugin_template.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-25 13:43:47.000000 psychopy_plugin_template-0.0.2/psychopy_plugin_template.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2387 2024-04-25 13:43:36.000000 psychopy_plugin_template-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 13:43:47.744127 psychopy_plugin_template-0.0.2/setup.cfg
```

### Comparing `psychopy_plugin_template-0.0.1/PKG-INFO` & `psychopy_plugin_template-0.0.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-Metadata-Version: 2.1
-Name: psychopy-plugin-template
-Version: 0.0.1
-Summary: Tutorial on how to create a plugin component for both PsychoPy and PsychoJS
-Author-email: OST Science Team <science@opensceincetools.org>
-License: MIT
-Project-URL: homepage, https://github.com/psychopy/psychopy-plugin-template
-Project-URL: changelog, https://github.com/psychopy/psychopy-plugin-template/blob/main/CHANGELOG.md
-Provides-Extra: docs
-Requires-Dist: psychopy; extra == "docs"
-Requires-Dist: sphinx; extra == "docs"
-Requires-Dist: furo; extra == "docs"
-Provides-Extra: tests
-Requires-Dist: psychopy; extra == "tests"
-Requires-Dist: pytest; extra == "tests"
+Metadata-Version: 2.1
+Name: psychopy-plugin-template
+Version: 0.0.2
+Summary: Tutorial on how to create a plugin component for both PsychoPy and PsychoJS
+Author-email: OST Science Team <science@opensceincetools.org>
+License: MIT
+Project-URL: homepage, https://github.com/psychopy/psychopy-plugin-template
+Project-URL: changelog, https://github.com/psychopy/psychopy-plugin-template/blob/main/CHANGELOG.md
+Provides-Extra: docs
+Requires-Dist: psychopy; extra == "docs"
+Requires-Dist: sphinx; extra == "docs"
+Requires-Dist: furo; extra == "docs"
+Provides-Extra: tests
+Requires-Dist: psychopy; extra == "tests"
+Requires-Dist: pytest; extra == "tests"
```

### Comparing `psychopy_plugin_template-0.0.1/psychopy-plugin-template/components/exampleComponent/__init__.py` & `psychopy_plugin_template-0.0.2/psychopy_plugin_template/components/exampleComponent/__init__.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,159 +1,159 @@
-from psychopy.experiment.components import BaseComponent, Param, getInitVals
-from pathlib import Path
-
-class ExampleComponent(BaseComponent):
-    """
-    Example Component to show you how to make and document one.
-    """
-    # mark it as coming from this plugin
-    plugin = "psychopy-example-plugin"
-    # specify what libraries it has code for - PsychoPy and/or PsychoJS
-    targets = ["PsychoPy"]
-    # specify what category (or categories) to list this Component under in Builder
-    categories = ['Custom']
-    # path to this Component's icon file - ignoring the light/dark/classic folder and any @2x in the filename (PsychoPy will add these accordingly)
-    iconFile = Path(__file__).parent / "example.png"
-    # Text to display when this Component is hovered over
-    tooltip = "Example Component to show you how to use PsychoPy"
-    # what is the earliest version of PsychoPy this Component works with?
-    version = "0.0.0"
-    # is this Component still in beta?
-    beta = True
-
-    def __init__(
-        self, exp, parentName, 
-        # basic
-        name="",
-        # appearance
-        exampleAttribute="red",
-    ):
-        # initialise the base component class
-        BaseComponent.__init__(self, exp, parentName, name=name)
-        # base params like start and stop time are already added by BaseComponent, so add any other params in here...
-
-        # --- Params ---
-
-        # appearance
-        self.order += [
-            "exampleAttribute"
-        ]
-        self.params['exampleAttribute'] = Param(
-            exampleAttribute, valType="code", inputType="single", categ="Appearance",
-            label="Example attribute", hint="An example attribute to show you how to add one"
-        )
-    
-    def writeInitCode(self, buff):
-        """
-        Write the Python code which initialises the object for this Component.
-
-        Parameters
-        ----------
-        buff : 
-            String buffer to write to, i.e. the .py file
-        """
-        # any params using set each frame / repeat will need a safe value to start off with, this functon automatically substitutes those
-        inits = getInitVals(self.params)
-        # construct the actual code, using Python string formatting
-        # remember that params with valType="str" will already have quotes so you don't need to add them
-        code = (
-            "%(name)s = visual.ExampleVisualStim(\n"
-            "    win=win,\n"
-            "    name='%(name)s',\n"
-            ")\n"
-            "%(name)s.setExampleAttribute(%(exampleAttribute)s, log=False)\n"
-        )
-        # write the code to the string buffer (with params inserted)
-        buff.writeIndentedLines(code % inits)
-    
-    def writeInitCodeJS(self, buff):
-        """
-        This example only writes Python code, but if you want your Component to write JS you can use this function!
-
-        Parameters
-        ----------
-        buff : 
-            String buffer to write to, i.e. the .js file
-        """
-        pass
-
-    def writeRoutineStartCode(self, buff):
-        """
-        Write the Python code which is called at the start of this Component's Routine
-
-        Parameters
-        ----------
-        buff : 
-            String buffer to write to, i.e. the .py file
-        """
-        # update any parameters which need updating
-        self.writeParamUpdates(buff, updateType="set every repeat")
-        # aaaaand that's all you need! unless you want anything else to happen here - it's essentially the equivalent of the Begin Routine tab in a Code Component
-    
-    def writeFrameCode(self, buff):
-        """
-        Write the Python code which is called each frame for this Component.
-
-        Parameters
-        ----------
-        buff : 
-            String buffer to write to, i.e. the .py file
-        """
-        # update any parameters which need updating
-        self.writeParamUpdates(buff, updateType="set every frame")
-        # some code we want to run just once on the first frame of the Component - so we'll use the writeStartTestCode function to open an if statement and then dedent after
-        dedent = self.writeStartTestCode(buff)
-        # we only want the following code written if an if loop actually was opened, not if the start time is None! so make sure to use dedent as a boolean to avoid writing broken code
-        if dedent:
-            # status setting is already written by writeStartTestCode, so here we can just worry about extra stuff
-            code = (
-                "%(name)s.autoDraw = True\n"
-                "print('%(name)s has started! Yay!')\n"
-            )
-            buff.writeIndentedLines(code % self.params)
-            # dedent after!
-            buff.setIndentLevel(-dedent, relative=True)
-        
-        # use the same principle as we used for first-frame-of-Component code to add code which only runs while the Component is active
-        dedent = self.writeActiveTestCode(buff)
-        if dedent:
-            # here we can just add anything we want to happen each frame - let's update some arbitrary variable for fun
-            code = (
-                "%(name)s.someAttribute = randchoice(['a', 'b', 'c']))\n"
-            )
-            buff.writeIndentedLines(code % self.params)
-            # dedent after!
-            buff.setIndentLevel(-dedent, relative=True)
-        
-        # use the same principles again for last-frame-of-Component code
-        dedent = self.writeStopTestCode(buff)
-        if dedent:
-            # aaaaaaand some extra code for when the Component stops
-            code = (
-                "%(name)s.autoDraw = False\n"
-                "print('%(name)s has finished! Yay!')\n"
-            )
-            buff.writeIndentedLines(code % self.params)
-            # dedent after!
-            buff.setIndentLevel(-dedent, relative=True)
-    
-    def writeRoutineEndCode(self, buff):
-        """
-        Write the Python code which is called at the end of this Component's Routine
-
-        Parameters
-        ----------
-        buff : 
-            String buffer to write to, i.e. the .py file
-        """
-        # create a copy of params so that we can safely edit stuff
-        params = self.params.copy()
-        # add reference to the current loop (handy for data writing)
-        params['currentLoop'] = self.currentLoop
-        # store any data we'd like to store (start/stop are already handled)
-        code = (
-            "%(currentLoop)s.addData('%(name)s.someAttribute', %(name)s.someAttribute)"
-        )
-        buff.writeIndentedLines(code % params)
-
-        
-
+from psychopy.experiment.components import BaseComponent, Param, getInitVals
+from pathlib import Path
+
+class ExampleComponent(BaseComponent):
+    """
+    Example Component to show you how to make and document one.
+    """
+    # mark it as coming from this plugin
+    plugin = "psychopy-example-plugin"
+    # specify what libraries it has code for - PsychoPy and/or PsychoJS
+    targets = ["PsychoPy"]
+    # specify what category (or categories) to list this Component under in Builder
+    categories = ['Custom']
+    # path to this Component's icon file - ignoring the light/dark/classic folder and any @2x in the filename (PsychoPy will add these accordingly)
+    iconFile = Path(__file__).parent / "example.png"
+    # Text to display when this Component is hovered over
+    tooltip = "Example Component to show you how to use PsychoPy"
+    # what is the earliest version of PsychoPy this Component works with?
+    version = "0.0.0"
+    # is this Component still in beta?
+    beta = True
+
+    def __init__(
+        self, exp, parentName, 
+        # basic
+        name="",
+        # appearance
+        exampleAttribute="red",
+    ):
+        # initialise the base component class
+        BaseComponent.__init__(self, exp, parentName, name=name)
+        # base params like start and stop time are already added by BaseComponent, so add any other params in here...
+
+        # --- Params ---
+
+        # appearance
+        self.order += [
+            "exampleAttribute"
+        ]
+        self.params['exampleAttribute'] = Param(
+            exampleAttribute, valType="code", inputType="single", categ="Appearance",
+            label="Example attribute", hint="An example attribute to show you how to add one"
+        )
+    
+    def writeInitCode(self, buff):
+        """
+        Write the Python code which initialises the object for this Component.
+
+        Parameters
+        ----------
+        buff : 
+            String buffer to write to, i.e. the .py file
+        """
+        # any params using set each frame / repeat will need a safe value to start off with, this functon automatically substitutes those
+        inits = getInitVals(self.params)
+        # construct the actual code, using Python string formatting
+        # remember that params with valType="str" will already have quotes so you don't need to add them
+        code = (
+            "%(name)s = visual.ExampleVisualStim(\n"
+            "    win=win,\n"
+            "    name='%(name)s',\n"
+            ")\n"
+            "%(name)s.setExampleAttribute(%(exampleAttribute)s, log=False)\n"
+        )
+        # write the code to the string buffer (with params inserted)
+        buff.writeIndentedLines(code % inits)
+    
+    def writeInitCodeJS(self, buff):
+        """
+        This example only writes Python code, but if you want your Component to write JS you can use this function!
+
+        Parameters
+        ----------
+        buff : 
+            String buffer to write to, i.e. the .js file
+        """
+        pass
+
+    def writeRoutineStartCode(self, buff):
+        """
+        Write the Python code which is called at the start of this Component's Routine
+
+        Parameters
+        ----------
+        buff : 
+            String buffer to write to, i.e. the .py file
+        """
+        # update any parameters which need updating
+        self.writeParamUpdates(buff, updateType="set every repeat")
+        # aaaaand that's all you need! unless you want anything else to happen here - it's essentially the equivalent of the Begin Routine tab in a Code Component
+    
+    def writeFrameCode(self, buff):
+        """
+        Write the Python code which is called each frame for this Component.
+
+        Parameters
+        ----------
+        buff : 
+            String buffer to write to, i.e. the .py file
+        """
+        # update any parameters which need updating
+        self.writeParamUpdates(buff, updateType="set every frame")
+        # some code we want to run just once on the first frame of the Component - so we'll use the writeStartTestCode function to open an if statement and then dedent after
+        dedent = self.writeStartTestCode(buff)
+        # we only want the following code written if an if loop actually was opened, not if the start time is None! so make sure to use dedent as a boolean to avoid writing broken code
+        if dedent:
+            # status setting is already written by writeStartTestCode, so here we can just worry about extra stuff
+            code = (
+                "%(name)s.autoDraw = True\n"
+                "print('%(name)s has started! Yay!')\n"
+            )
+            buff.writeIndentedLines(code % self.params)
+            # dedent after!
+            buff.setIndentLevel(-dedent, relative=True)
+        
+        # use the same principle as we used for first-frame-of-Component code to add code which only runs while the Component is active
+        dedent = self.writeActiveTestCode(buff)
+        if dedent:
+            # here we can just add anything we want to happen each frame - let's update some arbitrary variable for fun
+            code = (
+                "%(name)s.someAttribute = randchoice(['a', 'b', 'c']))\n"
+            )
+            buff.writeIndentedLines(code % self.params)
+            # dedent after!
+            buff.setIndentLevel(-dedent, relative=True)
+        
+        # use the same principles again for last-frame-of-Component code
+        dedent = self.writeStopTestCode(buff)
+        if dedent:
+            # aaaaaaand some extra code for when the Component stops
+            code = (
+                "%(name)s.autoDraw = False\n"
+                "print('%(name)s has finished! Yay!')\n"
+            )
+            buff.writeIndentedLines(code % self.params)
+            # dedent after!
+            buff.setIndentLevel(-dedent, relative=True)
+    
+    def writeRoutineEndCode(self, buff):
+        """
+        Write the Python code which is called at the end of this Component's Routine
+
+        Parameters
+        ----------
+        buff : 
+            String buffer to write to, i.e. the .py file
+        """
+        # create a copy of params so that we can safely edit stuff
+        params = self.params.copy()
+        # add reference to the current loop (handy for data writing)
+        params['currentLoop'] = self.currentLoop
+        # store any data we'd like to store (start/stop are already handled)
+        code = (
+            "%(currentLoop)s.addData('%(name)s.someAttribute', %(name)s.someAttribute)"
+        )
+        buff.writeIndentedLines(code % params)
+
+        
+
```

### Comparing `psychopy_plugin_template-0.0.1/psychopy-plugin-template/components/exampleComponent/classic/example.png` & `psychopy_plugin_template-0.0.2/psychopy_plugin_template/components/exampleComponent/classic/example.png`

 * *Files identical despite different names*

### Comparing `psychopy_plugin_template-0.0.1/psychopy-plugin-template/components/exampleComponent/classic/example@2x.png` & `psychopy_plugin_template-0.0.2/psychopy_plugin_template/components/exampleComponent/classic/example@2x.png`

 * *Files identical despite different names*

### Comparing `psychopy_plugin_template-0.0.1/psychopy-plugin-template/components/exampleComponent/dark/example.png` & `psychopy_plugin_template-0.0.2/psychopy_plugin_template/components/exampleComponent/dark/example.png`

 * *Files identical despite different names*

### Comparing `psychopy_plugin_template-0.0.1/psychopy-plugin-template/components/exampleComponent/dark/example@2x.png` & `psychopy_plugin_template-0.0.2/psychopy_plugin_template/components/exampleComponent/dark/example@2x.png`

 * *Files identical despite different names*

### Comparing `psychopy_plugin_template-0.0.1/psychopy-plugin-template/components/exampleComponent/light/example.png` & `psychopy_plugin_template-0.0.2/psychopy_plugin_template/components/exampleComponent/light/example.png`

 * *Files identical despite different names*

### Comparing `psychopy_plugin_template-0.0.1/psychopy-plugin-template/components/exampleComponent/light/example@2x.png` & `psychopy_plugin_template-0.0.2/psychopy_plugin_template/components/exampleComponent/light/example@2x.png`

 * *Files identical despite different names*

### Comparing `psychopy_plugin_template-0.0.1/psychopy-plugin-template/hardware/exampleResponseDevice.py` & `psychopy_plugin_template-0.0.2/psychopy_plugin_template/hardware/exampleResponseDevice.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-from psychopy.hardware.base import BaseResponseDevice, BaseResponse
-
-
-class ExampleResponse(BaseResponse):
-    """ 
-    Blank hardware response object to showcase how to make a new type of hardware response for a ResponseDevice.
-
-    Parameters
-    ----------
-    t : float
-        Time at which the response happened
-    value
-        Value received (e.g. the key on a keyboard)
-    """
-
-class ExampleResponseDevice(BaseResponseDevice):
-    """
-    Blank hardware object to showcase how to make a new type of hardware object for a response device.
-    
-    Should be deleted before publishing your plugin.
-
-    Attributes
-    ----------
-    listeners : list[psychopy.hardware.listeners.BaseListener]
-        List of listeners to send responses to
-    responses : list[ExampleResponse]
-        List of responses received by this device object
-    muteOutsidePsychopy : bool
-        If True, then mute any responses gathered when the PsychoPy window is not in focus
-    """
-    responseClass = ExampleResponse
+from psychopy.hardware.base import BaseResponseDevice, BaseResponse
+
+
+class ExampleResponse(BaseResponse):
+    """ 
+    Blank hardware response object to showcase how to make a new type of hardware response for a ResponseDevice.
+
+    Parameters
+    ----------
+    t : float
+        Time at which the response happened
+    value
+        Value received (e.g. the key on a keyboard)
+    """
+
+class ExampleResponseDevice(BaseResponseDevice):
+    """
+    Blank hardware object to showcase how to make a new type of hardware object for a response device.
+    
+    Should be deleted before publishing your plugin.
+
+    Attributes
+    ----------
+    listeners : list[psychopy.hardware.listeners.BaseListener]
+        List of listeners to send responses to
+    responses : list[ExampleResponse]
+        List of responses received by this device object
+    muteOutsidePsychopy : bool
+        If True, then mute any responses gathered when the PsychoPy window is not in focus
+    """
+    responseClass = ExampleResponse
```

### Comparing `psychopy_plugin_template-0.0.1/psychopy-plugin-template/visual/exampleVisualStim.py` & `psychopy_plugin_template-0.0.2/psychopy_plugin_template/visual/exampleVisualStim.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,53 +1,53 @@
-from psychopy.visual.basevisual import BaseVisualStim
-from psychopy.tools.attributetools import attributeSetter, setAttribute
-
-class ExampleVisualStim(BaseVisualStim):
-    """
-    Blank visual stim to showcase how to make a new visual stim. Should be deleted before publishing your plugin.
-
-    Parameters
-    ----------
-    win : psychopy.visual.Window
-        Window to draw stimulus to
-    units : str
-        Spatial unit space in which to specify size, pos, etc. for stimulus.
-    name : str
-        Arbitrary name by which to refer to stimulus
-    autoLog : bool
-        Whether to automatically log any changes to stimulus' attributes
-    """
-    def draw(self):
-        """
-        Your stimulus class needs to define a `draw` function - otherwise you'll hit a NotImplementedError at the first win flip!
-        """
-        return
-    
-    @attributeSetter
-    def exampleAttribute(self, value):
-        """
-        Example attribute to show how to use the attributeSetter decorator.
-
-        Parameters
-        ----------
-        value : any
-            Whatever value you want to set
-        """
-        # attributeSetter handles all of the necessary logging stuff - so all you need to do is set the base value in this object's __dict__
-        self.__dict__['exampleAttribute'] = value
-        # you may want setting this attribute to do something else - let's say changing color if given one of three color names
-        if value in ("red", "green", "blue"):
-            self.fillColor = value
-    
-    def setExampleAttribute(self, value, log=True):
-        """
-        If an attribute can be set each frame/repeat from Builder, there needs to be a function called set<attribute name in PascalCase> as this will be called from the generated code.
-
-        Parameters
-        ----------
-        value : any
-            Whatever value you want to set
-        log : bool, optional
-            Whether or not to log setting this attribute - will be True for set each repeat and False for set each frame
-        """
-        setAttribute(self, "exampleAttribute", value=value, log=log)
-
+from psychopy.visual.basevisual import BaseVisualStim
+from psychopy.tools.attributetools import attributeSetter, setAttribute
+
+class ExampleVisualStim(BaseVisualStim):
+    """
+    Blank visual stim to showcase how to make a new visual stim. Should be deleted before publishing your plugin.
+
+    Parameters
+    ----------
+    win : psychopy.visual.Window
+        Window to draw stimulus to
+    units : str
+        Spatial unit space in which to specify size, pos, etc. for stimulus.
+    name : str
+        Arbitrary name by which to refer to stimulus
+    autoLog : bool
+        Whether to automatically log any changes to stimulus' attributes
+    """
+    def draw(self):
+        """
+        Your stimulus class needs to define a `draw` function - otherwise you'll hit a NotImplementedError at the first win flip!
+        """
+        return
+    
+    @attributeSetter
+    def exampleAttribute(self, value):
+        """
+        Example attribute to show how to use the attributeSetter decorator.
+
+        Parameters
+        ----------
+        value : any
+            Whatever value you want to set
+        """
+        # attributeSetter handles all of the necessary logging stuff - so all you need to do is set the base value in this object's __dict__
+        self.__dict__['exampleAttribute'] = value
+        # you may want setting this attribute to do something else - let's say changing color if given one of three color names
+        if value in ("red", "green", "blue"):
+            self.fillColor = value
+    
+    def setExampleAttribute(self, value, log=True):
+        """
+        If an attribute can be set each frame/repeat from Builder, there needs to be a function called set<attribute name in PascalCase> as this will be called from the generated code.
+
+        Parameters
+        ----------
+        value : any
+            Whatever value you want to set
+        log : bool, optional
+            Whether or not to log setting this attribute - will be True for set each repeat and False for set each frame
+        """
+        setAttribute(self, "exampleAttribute", value=value, log=log)
+
```

### Comparing `psychopy_plugin_template-0.0.1/psychopy_plugin_template.egg-info/PKG-INFO` & `psychopy_plugin_template-0.0.2/psychopy_plugin_template.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-Metadata-Version: 2.1
-Name: psychopy-plugin-template
-Version: 0.0.1
-Summary: Tutorial on how to create a plugin component for both PsychoPy and PsychoJS
-Author-email: OST Science Team <science@opensceincetools.org>
-License: MIT
-Project-URL: homepage, https://github.com/psychopy/psychopy-plugin-template
-Project-URL: changelog, https://github.com/psychopy/psychopy-plugin-template/blob/main/CHANGELOG.md
-Provides-Extra: docs
-Requires-Dist: psychopy; extra == "docs"
-Requires-Dist: sphinx; extra == "docs"
-Requires-Dist: furo; extra == "docs"
-Provides-Extra: tests
-Requires-Dist: psychopy; extra == "tests"
-Requires-Dist: pytest; extra == "tests"
+Metadata-Version: 2.1
+Name: psychopy-plugin-template
+Version: 0.0.2
+Summary: Tutorial on how to create a plugin component for both PsychoPy and PsychoJS
+Author-email: OST Science Team <science@opensceincetools.org>
+License: MIT
+Project-URL: homepage, https://github.com/psychopy/psychopy-plugin-template
+Project-URL: changelog, https://github.com/psychopy/psychopy-plugin-template/blob/main/CHANGELOG.md
+Provides-Extra: docs
+Requires-Dist: psychopy; extra == "docs"
+Requires-Dist: sphinx; extra == "docs"
+Requires-Dist: furo; extra == "docs"
+Provides-Extra: tests
+Requires-Dist: psychopy; extra == "tests"
+Requires-Dist: pytest; extra == "tests"
```

### Comparing `psychopy_plugin_template-0.0.1/psychopy_plugin_template.egg-info/SOURCES.txt` & `psychopy_plugin_template-0.0.2/psychopy_plugin_template.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 README.md
 pyproject.toml
-psychopy-plugin-template/__init__.py
-psychopy-plugin-template/components/__init__.py
-psychopy-plugin-template/components/exampleComponent/__init__.py
-psychopy-plugin-template/components/exampleComponent/classic/example.png
-psychopy-plugin-template/components/exampleComponent/classic/example@2x.png
-psychopy-plugin-template/components/exampleComponent/dark/example.png
-psychopy-plugin-template/components/exampleComponent/dark/example@2x.png
-psychopy-plugin-template/components/exampleComponent/light/example.png
-psychopy-plugin-template/components/exampleComponent/light/example@2x.png
-psychopy-plugin-template/hardware/__init__.py
-psychopy-plugin-template/hardware/exampleDevice.py
-psychopy-plugin-template/hardware/exampleResponseDevice.py
-psychopy-plugin-template/routines/__init__.py
-psychopy-plugin-template/routines/exampleStandaloneRoutine/__init__.py
-psychopy-plugin-template/visual/__init__.py
-psychopy-plugin-template/visual/exampleVisualStim.py
+psychopy_plugin_template/__init__.py
 psychopy_plugin_template.egg-info/PKG-INFO
 psychopy_plugin_template.egg-info/SOURCES.txt
 psychopy_plugin_template.egg-info/dependency_links.txt
 psychopy_plugin_template.egg-info/entry_points.txt
 psychopy_plugin_template.egg-info/requires.txt
-psychopy_plugin_template.egg-info/top_level.txt
+psychopy_plugin_template.egg-info/top_level.txt
+psychopy_plugin_template/components/__init__.py
+psychopy_plugin_template/components/exampleComponent/__init__.py
+psychopy_plugin_template/components/exampleComponent/classic/example.png
+psychopy_plugin_template/components/exampleComponent/classic/example@2x.png
+psychopy_plugin_template/components/exampleComponent/dark/example.png
+psychopy_plugin_template/components/exampleComponent/dark/example@2x.png
+psychopy_plugin_template/components/exampleComponent/light/example.png
+psychopy_plugin_template/components/exampleComponent/light/example@2x.png
+psychopy_plugin_template/hardware/__init__.py
+psychopy_plugin_template/hardware/exampleDevice.py
+psychopy_plugin_template/hardware/exampleResponseDevice.py
+psychopy_plugin_template/routines/__init__.py
+psychopy_plugin_template/routines/exampleStandaloneRoutine/__init__.py
+psychopy_plugin_template/visual/__init__.py
+psychopy_plugin_template/visual/exampleVisualStim.py
```

### Comparing `psychopy_plugin_template-0.0.1/psychopy_plugin_template.egg-info/entry_points.txt` & `psychopy_plugin_template-0.0.2/psychopy_plugin_template.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `psychopy_plugin_template-0.0.1/pyproject.toml` & `psychopy_plugin_template-0.0.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,58 +1,58 @@
-[project]
-# the name of your plugin (required)
-name = "psychopy-plugin-template"
-# the current version of the plugin (required)
-version = "0.0.1" 
-# a brief description of what your plugin does
-description = "Tutorial on how to create a plugin component for both PsychoPy and PsychoJS"
-# contact information for yourself and anyone else who worked on the plugin 
-authors = [
-  { name = "OST Science Team", email = "science@opensceincetools.org" },
-]
-# a license tells other people how to use your code and protects you from stealing
-license = { text = "MIT" }
-# add any packages which your plugin needs in order to run
-dependencies = []
-
-[project.urls]
-# some handy links to help people find your plugin's documentation
-homepage = "https://github.com/psychopy/psychopy-plugin-template"
-changelog = "https://github.com/psychopy/psychopy-plugin-template/blob/main/CHANGELOG.md"
-
-[project.optional-dependencies]
-# dependencies for building the docs
-docs = [
-  "psychopy",
-  "sphinx",
-  "furo",
-]
-# dependencies for running the test suite
-tests = [
-  "psychopy",
-  "pytest",
-]
-
-[project.entry-points."psychopy.experiment.components"]
-# if you want a Component to appear in the "Components" panel, add its class here
-ExampleComponent = "psychopy_example_plugin.components.exampleComponent:ExampleComponent"
-
-[project.entry-points."psychopy.experiment.routines"]
-# if you want a Standalone Routine to appear in the "Components" panel, add its class here
-ExampleStandaloneRoutine = "psychopy_example_plugin.routines.exampleStandaloneRoutine:ExampleStandaloneRoutine"
-
-[project.entry-points."psychopy.visual"]
-# if you want something to be importable from psychopy.visual, add it here
-ExampleVisualStim = "psychopy_example_plugin.visual.exampleVisualStim:ExampleVisualStim"
-
-[project.entry-points."psychopy.hardware"]
-# if you want something to be importable from psychopy.hardware, add it here
-ExampleDevice = "psychopy_example_plugin.hardware.exampleDevice:ExampleDevice"
-ExampleResponseDevice = "psychopy_example_plugin.hardware.exampleResponseDevice:ExampleResponseDevice"
-
-[tool.setuptools.package-data]
-# any resources you want including in the package, add their file extensions here (e.g. "*.wav" if you want audio files)
-"*" = ["*.png"] 
-
-[tool.setuptools.packages.find]
-# any folders to ignore when building the Python package for this plugin
+[project]
+# the name of your plugin (required)
+name = "psychopy-plugin-template"
+# the current version of the plugin (required)
+version = "0.0.2" 
+# a brief description of what your plugin does
+description = "Tutorial on how to create a plugin component for both PsychoPy and PsychoJS"
+# contact information for yourself and anyone else who worked on the plugin 
+authors = [
+  { name = "OST Science Team", email = "science@opensceincetools.org" },
+]
+# a license tells other people how to use your code and protects you from stealing
+license = { text = "MIT" }
+# add any packages which your plugin needs in order to run
+dependencies = []
+
+[project.urls]
+# some handy links to help people find your plugin's documentation
+homepage = "https://github.com/psychopy/psychopy-plugin-template"
+changelog = "https://github.com/psychopy/psychopy-plugin-template/blob/main/CHANGELOG.md"
+
+[project.optional-dependencies]
+# dependencies for building the docs
+docs = [
+  "psychopy",
+  "sphinx",
+  "furo",
+]
+# dependencies for running the test suite
+tests = [
+  "psychopy",
+  "pytest",
+]
+
+[project.entry-points."psychopy.experiment.components"]
+# if you want a Component to appear in the "Components" panel, add its class here
+ExampleComponent = "psychopy_example_plugin.components.exampleComponent:ExampleComponent"
+
+[project.entry-points."psychopy.experiment.routines"]
+# if you want a Standalone Routine to appear in the "Components" panel, add its class here
+ExampleStandaloneRoutine = "psychopy_example_plugin.routines.exampleStandaloneRoutine:ExampleStandaloneRoutine"
+
+[project.entry-points."psychopy.visual"]
+# if you want something to be importable from psychopy.visual, add it here
+ExampleVisualStim = "psychopy_example_plugin.visual.exampleVisualStim:ExampleVisualStim"
+
+[project.entry-points."psychopy.hardware"]
+# if you want something to be importable from psychopy.hardware, add it here
+ExampleDevice = "psychopy_example_plugin.hardware.exampleDevice:ExampleDevice"
+ExampleResponseDevice = "psychopy_example_plugin.hardware.exampleResponseDevice:ExampleResponseDevice"
+
+[tool.setuptools.package-data]
+# any resources you want including in the package, add their file extensions here (e.g. "*.wav" if you want audio files)
+"*" = ["*.png"] 
+
+[tool.setuptools.packages.find]
+# any folders to ignore when building the Python package for this plugin
 exclude = ["docs*", "docs_src*", "tests*"]
```


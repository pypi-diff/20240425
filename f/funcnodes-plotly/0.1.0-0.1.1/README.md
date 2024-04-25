# Comparing `tmp/funcnodes_plotly-0.1.0.tar.gz` & `tmp/funcnodes_plotly-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funcnodes_plotly-0.1.0.tar", max compression
+gzip compressed data, was "funcnodes_plotly-0.1.1.tar", max compression
```

## Comparing `funcnodes_plotly-0.1.0.tar` & `funcnodes_plotly-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      874 2024-04-25 07:29:53.059506 funcnodes_plotly-0.1.0/funcnodes_plotly/__init__.py
--rw-r--r--   0        0        0     1576 2024-04-25 07:30:29.875384 funcnodes_plotly-0.1.0/funcnodes_plotly/figure.py
--rw-r--r--   0        0        0      476 2024-04-25 07:34:34.883959 funcnodes_plotly-0.1.0/funcnodes_plotly/layout.py
--rw-r--r--   0        0        0     1628 2024-04-25 07:30:46.097146 funcnodes_plotly-0.1.0/funcnodes_plotly/plots.py
--rw-r--r--   0        0        0      712 2024-04-25 07:30:37.354304 funcnodes_plotly-0.1.0/funcnodes_plotly/utils.py
--rw-r--r--   0        0        0      392 2024-04-24 15:13:13.612668 funcnodes_plotly-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-25 09:59:08.711878 funcnodes_plotly-0.1.0/README.md
--rw-r--r--   0        0        0      532 1970-01-01 00:00:00.000000 funcnodes_plotly-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1008 2024-04-25 10:10:00.331002 funcnodes_plotly-0.1.1/funcnodes_plotly/__init__.py
+-rw-r--r--   0        0        0     1512 2024-04-25 10:07:50.895177 funcnodes_plotly-0.1.1/funcnodes_plotly/figure.py
+-rw-r--r--   0        0        0      476 2024-04-25 07:34:34.883959 funcnodes_plotly-0.1.1/funcnodes_plotly/layout.py
+-rw-r--r--   0        0        0     1628 2024-04-25 10:07:33.248130 funcnodes_plotly-0.1.1/funcnodes_plotly/plots.py
+-rw-r--r--   0        0        0      712 2024-04-25 07:30:37.354304 funcnodes_plotly-0.1.1/funcnodes_plotly/utils.py
+-rw-r--r--   0        0        0      472 2024-04-25 10:12:13.570972 funcnodes_plotly-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-25 09:59:08.711878 funcnodes_plotly-0.1.1/README.md
+-rw-r--r--   0        0        0      730 1970-01-01 00:00:00.000000 funcnodes_plotly-0.1.1/PKG-INFO
```

### Comparing `funcnodes_plotly-0.1.0/funcnodes_plotly/__init__.py` & `funcnodes_plotly-0.1.1/funcnodes_plotly/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,26 +1,32 @@
 from typing import Tuple, Any
 import plotly.graph_objects as go
 from plotly.basedatatypes import BaseTraceType
 import funcnodes as fn
 from exposedfunctionality.function_parser.types import add_type
 
-from .plots import make_scatter, make_bar
-from .figure import make_figue, add_trace, plot
-
-
 add_type(
     go.Figure,
     "plotly.Figure",
 )
 add_type(
     BaseTraceType,
     "plotly.Trace",
 )
 
+from .plots import make_scatter, make_bar
+from .figure import make_figue, add_trace, plot
+
+
+FUNCNODES_RENDER_OPTIONS: fn.RenderOptions = {
+    "typemap": {
+        go.Figure: "plotly.Figure",
+    },
+}
+
 
 def figureencoder(figure: go.Figure, preview: bool = False) -> Tuple[Any, bool]:
     if isinstance(figure, go.Figure):
         return figure.to_plotly_json(), True
     return figure, False
 
 
@@ -35,7 +41,10 @@
         add_trace,
         plot,
     ],
     name="Plotly",
     description="A collection of functions for creating plotly plots.",
     subshelves=[],
 )
+
+
+__version__ = "0.1.1"
```

### Comparing `funcnodes_plotly-0.1.0/funcnodes_plotly/figure.py` & `funcnodes_plotly-0.1.1/funcnodes_plotly/figure.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from copy import deepcopy
 from typing import List, Dict, Tuple, Any, Literal, Optional
 import plotly.graph_objects as go
 from plotly.basedatatypes import BaseTraceType
 import funcnodes as fn
-from exposedfunctionality.function_parser.types import add_type
 
 from .utils import clone_trace, clone_figure
 
 
 @fn.NodeDecorator("plotly.make_figure", name="Make Figure")
 def make_figue() -> go.Figure:
     """
```

### Comparing `funcnodes_plotly-0.1.0/funcnodes_plotly/plots.py` & `funcnodes_plotly-0.1.1/funcnodes_plotly/plots.py`

 * *Files identical despite different names*

### Comparing `funcnodes_plotly-0.1.0/funcnodes_plotly/utils.py` & `funcnodes_plotly-0.1.1/funcnodes_plotly/utils.py`

 * *Files identical despite different names*


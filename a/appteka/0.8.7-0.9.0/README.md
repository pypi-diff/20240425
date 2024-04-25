# Comparing `tmp/appteka-0.8.7.tar.gz` & `tmp/appteka-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/appteka-0.8.7.tar", last modified: Fri Apr  3 13:29:04 2020, max compression
+gzip compressed data, was "dist/appteka-0.9.0.tar", last modified: Fri Jul 31 14:29:40 2020, max compression
```

## Comparing `appteka-0.8.7.tar` & `appteka-0.9.0.tar`

### file list

```diff
@@ -1,37 +1,38 @@
-drwxrwxr-x   0 apopov    (1000) apopov    (1000)        0 2020-04-03 13:29:04.000000 appteka-0.8.7/
--rw-rw-r--   0 apopov    (1000) apopov    (1000)       19 2019-09-03 13:55:44.000000 appteka-0.8.7/README
-drwxrwxr-x   0 apopov    (1000) apopov    (1000)        0 2020-04-03 13:29:04.000000 appteka-0.8.7/appteka.egg-info/
--rw-rw-r--   0 apopov    (1000) apopov    (1000)       16 2020-04-03 13:29:04.000000 appteka-0.8.7/appteka.egg-info/requires.txt
--rw-rw-r--   0 apopov    (1000) apopov    (1000)        8 2020-04-03 13:29:04.000000 appteka-0.8.7/appteka.egg-info/top_level.txt
--rw-rw-r--   0 apopov    (1000) apopov    (1000)      690 2020-04-03 13:29:04.000000 appteka-0.8.7/appteka.egg-info/SOURCES.txt
--rw-rw-r--   0 apopov    (1000) apopov    (1000)      726 2020-04-03 13:29:04.000000 appteka-0.8.7/appteka.egg-info/PKG-INFO
--rw-rw-r--   0 apopov    (1000) apopov    (1000)        1 2020-04-03 13:29:04.000000 appteka-0.8.7/appteka.egg-info/dependency_links.txt
--rw-rw-r--   0 apopov    (1000) apopov    (1000)     1776 2019-09-03 13:55:44.000000 appteka-0.8.7/setup.py
-drwxrwxr-x   0 apopov    (1000) apopov    (1000)        0 2020-04-03 13:29:04.000000 appteka-0.8.7/test/
--rw-rw-r--   0 apopov    (1000) apopov    (1000)     1358 2020-01-16 09:56:40.000000 appteka-0.8.7/test/test_waveform.py
--rw-rw-r--   0 apopov    (1000) apopov    (1000)     1918 2020-03-27 13:57:11.000000 appteka-0.8.7/test/test_multiwaveform.py
--rw-rw-r--   0 apopov    (1000) apopov    (1000)      767 2020-01-16 09:56:40.000000 appteka-0.8.7/test/test_editor.py
--rw-rw-r--   0 apopov    (1000) apopov    (1000)     5184 2020-01-16 09:56:40.000000 appteka-0.8.7/test/test_phasor.py
--rw-rw-r--   0 apopov    (1000) apopov    (1000)       38 2020-04-03 13:29:04.000000 appteka-0.8.7/setup.cfg
-drwxrwxr-x   0 apopov    (1000) apopov    (1000)        0 2020-04-03 13:29:04.000000 appteka-0.8.7/appteka/
--rw-rw-r--   0 apopov    (1000) apopov    (1000)     2079 2020-04-03 13:28:23.000000 appteka-0.8.7/appteka/test_sqlite_schema.py
--rw-rw-r--   0 apopov    (1000) apopov    (1000)     4581 2020-01-14 11:38:09.000000 appteka-0.8.7/appteka/io.py
--rw-rw-r--   0 apopov    (1000) apopov    (1000)     1874 2020-01-13 14:23:16.000000 appteka-0.8.7/appteka/simple_signal.py
--rw-rw-r--   0 apopov    (1000) apopov    (1000)     4513 2020-01-13 14:23:16.000000 appteka-0.8.7/appteka/reporter.py
-drwxrwxr-x   0 apopov    (1000) apopov    (1000)        0 2020-04-03 13:29:04.000000 appteka-0.8.7/appteka/pyqtgraph/
--rw-rw-r--   0 apopov    (1000) apopov    (1000)     4386 2020-01-13 14:23:16.000000 appteka-0.8.7/appteka/pyqtgraph/phasor.py
--rw-rw-r--   0 apopov    (1000) apopov    (1000)     8927 2020-03-27 13:57:11.000000 appteka-0.8.7/appteka/pyqtgraph/waveform.py
--rw-rw-r--   0 apopov    (1000) apopov    (1000)      728 2020-01-13 14:23:16.000000 appteka-0.8.7/appteka/pyqtgraph/__init__.py
--rw-rw-r--   0 apopov    (1000) apopov    (1000)     1790 2020-01-13 14:23:16.000000 appteka-0.8.7/appteka/distrib.py
--rw-rw-r--   0 apopov    (1000) apopov    (1000)     4744 2020-01-13 14:23:16.000000 appteka-0.8.7/appteka/config.py
--rw-rw-r--   0 apopov    (1000) apopov    (1000)     1214 2020-01-13 14:23:16.000000 appteka-0.8.7/appteka/routine.py
-drwxrwxr-x   0 apopov    (1000) apopov    (1000)        0 2020-04-03 13:29:04.000000 appteka-0.8.7/appteka/pyqt/
--rw-rw-r--   0 apopov    (1000) apopov    (1000)     5220 2020-01-16 09:56:40.000000 appteka-0.8.7/appteka/pyqt/testing.py
--rw-rw-r--   0 apopov    (1000) apopov    (1000)     2064 2020-01-13 14:23:16.000000 appteka-0.8.7/appteka/pyqt/control_states.py
--rw-rw-r--   0 apopov    (1000) apopov    (1000)     4587 2020-01-13 14:23:16.000000 appteka-0.8.7/appteka/pyqt/codetextedit.py
--rw-rw-r--   0 apopov    (1000) apopov    (1000)     2516 2020-01-13 14:23:16.000000 appteka-0.8.7/appteka/pyqt/gui.py
--rw-rw-r--   0 apopov    (1000) apopov    (1000)      728 2020-01-13 14:23:16.000000 appteka-0.8.7/appteka/pyqt/__init__.py
--rw-rw-r--   0 apopov    (1000) apopov    (1000)     2740 2020-01-13 14:23:16.000000 appteka-0.8.7/appteka/pyqt/select_item_dialog.py
--rw-rw-r--   0 apopov    (1000) apopov    (1000)      751 2020-04-03 13:28:23.000000 appteka-0.8.7/appteka/__init__.py
--rw-rw-r--   0 apopov    (1000) apopov    (1000)     1407 2020-01-13 14:23:16.000000 appteka-0.8.7/appteka/cli.py
--rw-rw-r--   0 apopov    (1000) apopov    (1000)      726 2020-04-03 13:29:04.000000 appteka-0.8.7/PKG-INFO
+drwxrwxr-x   0 apopov    (1000) apopov    (1000)        0 2020-07-31 14:29:40.000000 appteka-0.9.0/
+-rw-rw-r--   0 apopov    (1000) apopov    (1000)       19 2019-09-03 13:55:44.000000 appteka-0.9.0/README
+drwxrwxr-x   0 apopov    (1000) apopov    (1000)        0 2020-07-31 14:29:40.000000 appteka-0.9.0/appteka.egg-info/
+-rw-rw-r--   0 apopov    (1000) apopov    (1000)       16 2020-07-31 14:29:39.000000 appteka-0.9.0/appteka.egg-info/requires.txt
+-rw-rw-r--   0 apopov    (1000) apopov    (1000)        8 2020-07-31 14:29:39.000000 appteka-0.9.0/appteka.egg-info/top_level.txt
+-rw-rw-r--   0 apopov    (1000) apopov    (1000)      721 2020-07-31 14:29:40.000000 appteka-0.9.0/appteka.egg-info/SOURCES.txt
+-rw-rw-r--   0 apopov    (1000) apopov    (1000)      726 2020-07-31 14:29:39.000000 appteka-0.9.0/appteka.egg-info/PKG-INFO
+-rw-rw-r--   0 apopov    (1000) apopov    (1000)        1 2020-07-31 14:29:39.000000 appteka-0.9.0/appteka.egg-info/dependency_links.txt
+-rw-rw-r--   0 apopov    (1000) apopov    (1000)     1776 2019-09-03 13:55:44.000000 appteka-0.9.0/setup.py
+drwxrwxr-x   0 apopov    (1000) apopov    (1000)        0 2020-07-31 14:29:40.000000 appteka-0.9.0/test/
+-rw-rw-r--   0 apopov    (1000) apopov    (1000)     1358 2020-07-31 13:50:55.000000 appteka-0.9.0/test/test_waveform.py
+-rw-rw-r--   0 apopov    (1000) apopov    (1000)     1576 2020-07-31 14:28:40.000000 appteka-0.9.0/test/test_multiwaveform.py
+-rw-rw-r--   0 apopov    (1000) apopov    (1000)      769 2020-07-31 14:28:40.000000 appteka-0.9.0/test/test_editor.py
+-rw-rw-r--   0 apopov    (1000) apopov    (1000)     5184 2020-01-16 09:56:40.000000 appteka-0.9.0/test/test_phasor.py
+-rw-rw-r--   0 apopov    (1000) apopov    (1000)       38 2020-07-31 14:29:40.000000 appteka-0.9.0/setup.cfg
+drwxrwxr-x   0 apopov    (1000) apopov    (1000)        0 2020-07-31 14:29:40.000000 appteka-0.9.0/appteka/
+-rw-rw-r--   0 apopov    (1000) apopov    (1000)     2079 2020-04-03 13:28:23.000000 appteka-0.9.0/appteka/test_sqlite_schema.py
+-rw-rw-r--   0 apopov    (1000) apopov    (1000)     4581 2020-07-31 12:29:27.000000 appteka-0.9.0/appteka/io.py
+-rw-rw-r--   0 apopov    (1000) apopov    (1000)     1874 2020-01-13 14:23:16.000000 appteka-0.9.0/appteka/simple_signal.py
+-rw-rw-r--   0 apopov    (1000) apopov    (1000)     4513 2020-01-13 14:23:16.000000 appteka-0.9.0/appteka/reporter.py
+drwxrwxr-x   0 apopov    (1000) apopov    (1000)        0 2020-07-31 14:29:40.000000 appteka-0.9.0/appteka/pyqtgraph/
+-rw-rw-r--   0 apopov    (1000) apopov    (1000)     4386 2020-07-31 14:28:40.000000 appteka-0.9.0/appteka/pyqtgraph/phasor.py
+-rw-rw-r--   0 apopov    (1000) apopov    (1000)     8990 2020-07-31 14:28:40.000000 appteka-0.9.0/appteka/pyqtgraph/waveform.py
+-rw-rw-r--   0 apopov    (1000) apopov    (1000)      728 2020-01-13 14:23:16.000000 appteka-0.9.0/appteka/pyqtgraph/__init__.py
+-rw-rw-r--   0 apopov    (1000) apopov    (1000)     1790 2020-01-13 14:23:16.000000 appteka-0.9.0/appteka/distrib.py
+-rw-rw-r--   0 apopov    (1000) apopov    (1000)     4722 2020-07-31 14:28:40.000000 appteka-0.9.0/appteka/config.py
+-rw-rw-r--   0 apopov    (1000) apopov    (1000)     1214 2020-01-13 14:23:16.000000 appteka-0.9.0/appteka/routine.py
+drwxrwxr-x   0 apopov    (1000) apopov    (1000)        0 2020-07-31 14:29:40.000000 appteka-0.9.0/appteka/pyqt/
+-rw-rw-r--   0 apopov    (1000) apopov    (1000)     5220 2020-07-31 14:14:09.000000 appteka-0.9.0/appteka/pyqt/testing.py
+-rw-rw-r--   0 apopov    (1000) apopov    (1000)     2031 2020-07-31 14:28:40.000000 appteka-0.9.0/appteka/pyqt/control_states.py
+-rw-rw-r--   0 apopov    (1000) apopov    (1000)      949 2020-07-31 14:28:40.000000 appteka-0.9.0/appteka/pyqt/codetextedit.py
+-rw-rw-r--   0 apopov    (1000) apopov    (1000)     2516 2020-01-13 14:23:16.000000 appteka-0.9.0/appteka/pyqt/gui.py
+-rw-rw-r--   0 apopov    (1000) apopov    (1000)     4481 2020-07-31 14:28:40.000000 appteka-0.9.0/appteka/pyqt/code_text_edit.py
+-rw-rw-r--   0 apopov    (1000) apopov    (1000)      728 2020-01-13 14:23:16.000000 appteka-0.9.0/appteka/pyqt/__init__.py
+-rw-rw-r--   0 apopov    (1000) apopov    (1000)     2740 2020-01-13 14:23:16.000000 appteka-0.9.0/appteka/pyqt/select_item_dialog.py
+-rw-rw-r--   0 apopov    (1000) apopov    (1000)      774 2020-07-31 14:28:40.000000 appteka-0.9.0/appteka/__init__.py
+-rw-rw-r--   0 apopov    (1000) apopov    (1000)     1407 2020-01-13 14:23:16.000000 appteka-0.9.0/appteka/cli.py
+-rw-rw-r--   0 apopov    (1000) apopov    (1000)      726 2020-07-31 14:29:40.000000 appteka-0.9.0/PKG-INFO
```

### Comparing `appteka-0.8.7/appteka.egg-info/SOURCES.txt` & `appteka-0.9.0/appteka.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 appteka/test_sqlite_schema.py
 appteka.egg-info/PKG-INFO
 appteka.egg-info/SOURCES.txt
 appteka.egg-info/dependency_links.txt
 appteka.egg-info/requires.txt
 appteka.egg-info/top_level.txt
 appteka/pyqt/__init__.py
+appteka/pyqt/code_text_edit.py
 appteka/pyqt/codetextedit.py
 appteka/pyqt/control_states.py
 appteka/pyqt/gui.py
 appteka/pyqt/select_item_dialog.py
 appteka/pyqt/testing.py
 appteka/pyqtgraph/__init__.py
 appteka/pyqtgraph/phasor.py
```

### Comparing `appteka-0.8.7/appteka.egg-info/PKG-INFO` & `appteka-0.9.0/appteka.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: appteka
-Version: 0.8.7
+Version: 0.9.0
 Summary: All goods
 Home-page: https://bitbucket.org/aleneus/appteka
 Author: Aleksandr Popov
 Author-email: aleneus@gmail.com
 License: LGPLv3
 Description: Helpers collection
```

### Comparing `appteka-0.8.7/setup.py` & `appteka-0.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `appteka-0.8.7/test/test_waveform.py` & `appteka-0.9.0/test/test_waveform.py`

 * *Files identical despite different names*

### Comparing `appteka-0.8.7/test/test_editor.py` & `appteka-0.9.0/test/test_editor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import sys
 import os
 
 sys.path.insert(0, os.path.abspath("."))
 from appteka.pyqt import testing
-from appteka.pyqt.codetextedit import CodeTextEdit
+from appteka.pyqt.code_text_edit import CodeTextEdit
 
 
 class TestCodeTextEdit(testing.TestDialog):
     """Tests for CodeTextEdit"""
     def __init__(self):
         super().__init__()
         self.resize(600, 600)
```

### Comparing `appteka-0.8.7/test/test_phasor.py` & `appteka-0.9.0/test/test_phasor.py`

 * *Files identical despite different names*

### Comparing `appteka-0.8.7/appteka/test_sqlite_schema.py` & `appteka-0.9.0/appteka/test_sqlite_schema.py`

 * *Files identical despite different names*

### Comparing `appteka-0.8.7/appteka/io.py` & `appteka-0.9.0/appteka/io.py`

 * *Files identical despite different names*

### Comparing `appteka-0.8.7/appteka/simple_signal.py` & `appteka-0.9.0/appteka/simple_signal.py`

 * *Files identical despite different names*

### Comparing `appteka-0.8.7/appteka/reporter.py` & `appteka-0.9.0/appteka/reporter.py`

 * *Files identical despite different names*

### Comparing `appteka-0.8.7/appteka/pyqtgraph/phasor.py` & `appteka-0.9.0/appteka/pyqtgraph/phasor.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,23 +53,23 @@
     def set_range(self, value):
         """Set range of diagram."""
         self.__update_grid(value)
         self.__update_labels(value)
 
     def __build_grid(self):
         self.circles = []
-        for i in range(DEFAULT_CIRCLES_NUM):
+        for _ in range(DEFAULT_CIRCLES_NUM):
             circle = pg.QtGui.QGraphicsEllipseItem()
             circle.setPen(pg.mkPen(0.2))
             self.circles.append(circle)
             self.addItem(circle)
 
     def __build_labels(self):
         self.labels = []
-        for i in range(2):
+        for _ in range(2):
             label = pg.TextItem()
             self.labels.append(label)
             self.addItem(label)
 
     def __update_grid(self, value):
         for i in range(DEFAULT_CIRCLES_NUM):
             r = (i + 1) * value / DEFAULT_CIRCLES_NUM
```

### Comparing `appteka-0.8.7/appteka/pyqtgraph/waveform.py` & `appteka-0.9.0/appteka/pyqtgraph/waveform.py`

 * *Files 3% similar despite different names*

```diff
@@ -60,18 +60,18 @@
     return res
 
 
 class Waveform(pg.PlotWidget):
     """Customized PyQtGraph.PlotWidget."""
     def __init__(self, parent=None, xlabel=None, time_axis=True):
         if time_axis:
-            axisItems = get_time_stamp_axis_item()
+            axis_items = get_time_stamp_axis_item()
         else:
-            axisItems = None
-        super().__init__(parent, axisItems=axisItems)
+            axis_items = None
+        super().__init__(parent, axisItems=axis_items)
 
         self.showAxis('top')
         self.showAxis('right')
 
         self.state = {
             'online': False,
             'plot_color': (255, 255, 255),
@@ -181,15 +181,15 @@
         for axis in ['left', 'right']:
             plot.getAxis(axis).setStyle(
                 tickTextWidth=40,
                 autoExpandTextSpace=False
             )
         plot.enableAutoRange(True)
 
-    def add_plot(self, key, title=None, main=False, time_axes=False):
+    def add_plot(self, key, title=None, main=None, time_axes=False):
         """Add plot."""
         if time_axes:
             axes = get_time_stamp_axis_item()
         else:
             axes = None
 
         self.plots[key] = self.addPlot(len(self.plots), 0, axisItems=axes)
@@ -197,16 +197,16 @@
 
         if title is not None:
             self.plots[key].setTitle(title, justify='left')
 
         self.curves[key] = self.plots[key].plot()
         self.curves[key].setPen(self.state['plot_color'])
 
-        if main:
-            self._main = key
+        if main is not None:
+            warn("MultiWaveform.add_plot(): deprecated main arg was ignored")
 
     def set_title(self, plot_key, value):
         """Changes title of the given plot."""
         self.plots[plot_key].setTitle(value, justify='left')
 
     def remove_plots(self):
         """Remove all plots."""
```

### Comparing `appteka-0.8.7/appteka/pyqtgraph/__init__.py` & `appteka-0.9.0/appteka/pyqtgraph/__init__.py`

 * *Files identical despite different names*

### Comparing `appteka-0.8.7/appteka/distrib.py` & `appteka-0.9.0/appteka/distrib.py`

 * *Files identical despite different names*

### Comparing `appteka-0.8.7/appteka/config.py` & `appteka-0.9.0/appteka/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,16 +17,16 @@
 
 """ Class for work with JSON config files. """
 
 from collections import OrderedDict
 import os
 import shutil
 import json
-import pkg_resources
 import logging
+import pkg_resources
 
 LOG = logging.getLogger(__name__)
 
 
 class Config:
     """ Work with config files: create desired file if it not exists,
     read and save settings. """
@@ -113,16 +113,15 @@
         if 'version' not in settings.keys() and self.version is None:
             return True
         if 'version' not in settings.keys() and self.version is not None:
             return False
         if 'version' in settings.keys() and self.version is not None:
             if settings['version'] != self.version:
                 return False
-            else:
-                return True
+            return True
         return True
 
     def upgrade(self):
         """ Replace config file which have unsupported version newer
         file. """
         self._backup()
         self._copy_resource_file()
```

### Comparing `appteka-0.8.7/appteka/routine.py` & `appteka-0.9.0/appteka/routine.py`

 * *Files identical despite different names*

### Comparing `appteka-0.8.7/appteka/pyqt/testing.py` & `appteka-0.9.0/appteka/pyqt/testing.py`

 * *Files identical despite different names*

### Comparing `appteka-0.8.7/appteka/pyqt/control_states.py` & `appteka-0.9.0/appteka/pyqt/control_states.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,13 +43,12 @@
     def set_state(self, state_name):
         """ Set currect state. """
         for c in self.__controls:
             c.setVisible(c not in self.__states[state_name]['invisible'])
             c.setEnabled(c not in self.__states[state_name]['disabled'])
 
     def _setup_controls_state(self, controls, state_name, key):
-        """ Helper function. """
         self.__states[state_name][key] = []
         for c in controls:
             if c not in self.__controls:
                 self.__controls.append(c)
             self.__states[state_name][key].append(c)
```

### Comparing `appteka-0.8.7/appteka/pyqt/codetextedit.py` & `appteka-0.9.0/appteka/pyqt/code_text_edit.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,116 +11,110 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # Lesser GNU General Public License for more details.
 
 # You should have received a copy of the Lesser GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-"""This module implements text edit with line numbers and highlighting
-of current line."""
+"""Here the text edit with line numbers and highlighting of current
+line is implemented."""
 
 from PyQt5 import QtWidgets, QtGui
 from PyQt5.QtCore import QSize, QRect, Qt
 
+LINE_COLOR = QtGui.QColor(Qt.yellow).lighter(160)
+FONT = "monospace"
+
 
 class CodeTextEdit(QtWidgets.QPlainTextEdit):
     """Text field for editing the source code."""
     def __init__(self, parent=None):
         super().__init__(parent)
         self.lineNumberArea = LineNumberArea(self)
 
         self.blockCountChanged.connect(self.updateLineNumberAreaWidth)
         self.updateRequest.connect(self.updateLineNumberArea)
         self.cursorPositionChanged.connect(self.highlightCurrentLine)
 
         self.updateLineNumberAreaWidth(0)
         self.highlightCurrentLine()
 
-        f = QtGui.QFont("monospace")
-        f.setStyleHint(QtGui.QFont.Monospace)
-        self.setFont(f)
+        font = QtGui.QFont(FONT)
+        font.setStyleHint(QtGui.QFont.Monospace)
+        self.setFont(font)
 
     def set_text(self, text):
         """Set text."""
         self.document().setPlainText(text)
 
     def lineNumberAreaPaintEvent(self, event):
         painter = QtGui.QPainter(self.lineNumberArea)
         painter.fillRect(event.rect(), Qt.lightGray)
 
         block = self.firstVisibleBlock()
-        blockNumber = block.blockNumber()
+        block_number = block.blockNumber()
         top = self.blockBoundingGeometry(block).translated(
             self.contentOffset()).top()
         bottom = top + self.blockBoundingRect(block).height()
 
         while block.isValid() and top <= event.rect().bottom():
             if block.isVisible() and bottom >= event.rect().top():
-                number = "{}".format(blockNumber + 1)
+                number = "{}".format(block_number + 1)
                 painter.setPen(Qt.black)
                 painter.drawText(
                     0, top, self.lineNumberArea.width(),
                     self.fontMetrics().height(), Qt.AlignRight,
-                    number
-                )
+                    number)
 
             block = block.next()
             top = bottom
             bottom = top + self.blockBoundingRect(block).height()
-            blockNumber = blockNumber + 1
+            block_number = block_number + 1
 
     def lineNumberAreaWidth(self):
+        count = max(1, self.blockCount())
         digits = 1
-        mx = max(1, self.blockCount())
-        while mx >= 10:
-            mx = mx / 10
+        while count >= 10:
+            count = count / 10
             digits = digits + 1
 
-        # ch = QLatin1Char('9')
-        ch = '9'
-        space = 3 + self.fontMetrics().horizontalAdvance(ch) * digits
-        return space
+        return 3 + self.fontMetrics().horizontalAdvance('9') * digits
 
     def resizeEvent(self, e):
         super().resizeEvent(e)
-        cr = self.contentsRect()
-        r = QRect(
-            cr.left(),
-            cr.top(),
-            self.lineNumberAreaWidth(),
-            cr.height()
-        )
-        self.lineNumberArea.setGeometry(r)
+
+        rect = self.contentsRect()
+        self.lineNumberArea.setGeometry(QRect(
+            rect.left(), rect.top(),
+            self.lineNumberAreaWidth(), rect.height()))
 
     def updateLineNumberAreaWidth(self, newBlockCount):
         self.setViewportMargins(self.lineNumberAreaWidth(), 0, 0, 0)
 
     def highlightCurrentLine(self):
-        extraSelections = []
+        extra_selections = []
         if not self.isReadOnly():
             selection = QtWidgets.QTextEdit.ExtraSelection()
-            lineColor = QtGui.QColor(Qt.yellow).lighter(160)
-            selection.format.setBackground(lineColor)
+            selection.format.setBackground(LINE_COLOR)
             selection.format.setProperty(
                 QtGui.QTextFormat.FullWidthSelection, True)
             selection.cursor = self.textCursor()
             selection.cursor.clearSelection()
-            extraSelections.append(selection)
+            extra_selections.append(selection)
 
-        self.setExtraSelections(extraSelections)
+        self.setExtraSelections(extra_selections)
 
     def updateLineNumberArea(self, rect, dy):
         if dy:
             self.lineNumberArea.scroll(0, dy)
         else:
             self.lineNumberArea.update(
                 0, rect.y(),
                 self.lineNumberArea.width(),
-                rect.height()
-            )
+                rect.height())
 
         if rect.contains(self.viewport().rect()):
             self.updateLineNumberAreaWidth(0)
 
 
 class LineNumberArea(QtWidgets.QWidget):
     def __init__(self, editor):
```

### Comparing `appteka-0.8.7/appteka/pyqt/gui.py` & `appteka-0.9.0/appteka/pyqt/gui.py`

 * *Files identical despite different names*

### Comparing `appteka-0.8.7/appteka/pyqt/__init__.py` & `appteka-0.9.0/appteka/pyqt/__init__.py`

 * *Files identical despite different names*

### Comparing `appteka-0.8.7/appteka/pyqt/select_item_dialog.py` & `appteka-0.9.0/appteka/pyqt/select_item_dialog.py`

 * *Files identical despite different names*

### Comparing `appteka-0.8.7/appteka/__init__.py` & `appteka-0.9.0/appteka/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,8 +11,10 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # Lesser GNU General Public License for more details.
 
 # You should have received a copy of the Lesser GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-__version__ = '0.8.7'
+"""Initial script."""
+
+__version__ = '0.9.0'
```

### Comparing `appteka-0.8.7/appteka/cli.py` & `appteka-0.9.0/appteka/cli.py`

 * *Files identical despite different names*

### Comparing `appteka-0.8.7/PKG-INFO` & `appteka-0.9.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: appteka
-Version: 0.8.7
+Version: 0.9.0
 Summary: All goods
 Home-page: https://bitbucket.org/aleneus/appteka
 Author: Aleksandr Popov
 Author-email: aleneus@gmail.com
 License: LGPLv3
 Description: Helpers collection
```


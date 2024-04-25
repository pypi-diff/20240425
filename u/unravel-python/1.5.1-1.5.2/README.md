# Comparing `tmp/unravel_python-1.5.1.tar.gz` & `tmp/unravel_python-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unravel_python-1.5.1.tar", last modified: Fri Apr 19 09:40:29 2024, max compression
+gzip compressed data, was "unravel_python-1.5.2.tar", last modified: Thu Apr 25 16:28:40 2024, max compression
```

## Comparing `unravel_python-1.5.1.tar` & `unravel_python-1.5.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-04-19 09:40:29.740000 unravel_python-1.5.1/
--rw-rw-rw-   0        0        0    35823 2024-02-01 10:17:26.000000 unravel_python-1.5.1/LICENSE
--rw-rw-rw-   0        0        0     4515 2024-04-19 09:40:30.000000 unravel_python-1.5.1/PKG-INFO
--rw-rw-rw-   0        0        0     3801 2024-02-01 10:17:26.000000 unravel_python-1.5.1/README.md
--rw-rw-rw-   0        0        0      970 2024-02-01 10:17:26.000000 unravel_python-1.5.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-19 09:40:30.000000 unravel_python-1.5.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-19 09:40:29.750000 unravel_python-1.5.1/src/
-drwxrwxrwx   0        0        0        0 2024-04-19 09:40:29.750000 unravel_python-1.5.1/src/unravel/
--rw-rw-rw-   0        0        0      358 2024-04-19 09:39:30.000000 unravel_python-1.5.1/src/unravel/__init__.py
--rw-rw-rw-   0        0        0     3038 2024-02-21 12:39:26.000000 unravel_python-1.5.1/src/unravel/analysis.py
--rw-rw-rw-   0        0        0    44450 2024-02-01 10:17:26.000000 unravel_python-1.5.1/src/unravel/core.py
--rw-rw-rw-   0        0        0     4547 2024-02-21 12:33:42.000000 unravel_python-1.5.1/src/unravel/example.py
--rw-rw-rw-   0        0        0    20810 2024-04-19 09:36:20.000000 unravel_python-1.5.1/src/unravel/stream.py
--rw-rw-rw-   0        0        0    15988 2024-04-15 14:45:40.000000 unravel_python-1.5.1/src/unravel/utils.py
--rw-rw-rw-   0        0        0    20577 2024-04-15 15:01:06.000000 unravel_python-1.5.1/src/unravel/viz.py
-drwxrwxrwx   0        0        0        0 2024-04-19 09:40:29.760000 unravel_python-1.5.1/src/unravel_python.egg-info/
--rw-rw-rw-   0        0        0     4515 2024-04-19 09:40:30.000000 unravel_python-1.5.1/src/unravel_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      394 2024-04-19 09:40:30.000000 unravel_python-1.5.1/src/unravel_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 09:40:30.000000 unravel_python-1.5.1/src/unravel_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2024-04-19 09:40:30.000000 unravel_python-1.5.1/src/unravel_python.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-19 09:40:30.000000 unravel_python-1.5.1/src/unravel_python.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-25 16:28:40.630000 unravel_python-1.5.2/
+-rw-rw-rw-   0        0        0    35823 2024-02-01 10:17:26.000000 unravel_python-1.5.2/LICENSE
+-rw-rw-rw-   0        0        0     4515 2024-04-25 16:28:42.000000 unravel_python-1.5.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3801 2024-02-01 10:17:26.000000 unravel_python-1.5.2/README.md
+-rw-rw-rw-   0        0        0      970 2024-02-01 10:17:26.000000 unravel_python-1.5.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-25 16:28:42.000000 unravel_python-1.5.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-25 16:28:40.640000 unravel_python-1.5.2/src/
+drwxrwxrwx   0        0        0        0 2024-04-25 16:28:40.650000 unravel_python-1.5.2/src/unravel/
+-rw-rw-rw-   0        0        0      358 2024-04-25 16:27:56.000000 unravel_python-1.5.2/src/unravel/__init__.py
+-rw-rw-rw-   0        0        0     3038 2024-02-21 12:39:26.000000 unravel_python-1.5.2/src/unravel/analysis.py
+-rw-rw-rw-   0        0        0    44450 2024-02-01 10:17:26.000000 unravel_python-1.5.2/src/unravel/core.py
+-rw-rw-rw-   0        0        0     4547 2024-02-21 12:33:42.000000 unravel_python-1.5.2/src/unravel/example.py
+-rw-rw-rw-   0        0        0    20810 2024-04-19 09:36:20.000000 unravel_python-1.5.2/src/unravel/stream.py
+-rw-rw-rw-   0        0        0    15988 2024-04-15 14:45:40.000000 unravel_python-1.5.2/src/unravel/utils.py
+-rw-rw-rw-   0        0        0    20874 2024-04-25 16:26:12.000000 unravel_python-1.5.2/src/unravel/viz.py
+drwxrwxrwx   0        0        0        0 2024-04-25 16:28:40.660000 unravel_python-1.5.2/src/unravel_python.egg-info/
+-rw-rw-rw-   0        0        0     4515 2024-04-25 16:28:42.000000 unravel_python-1.5.2/src/unravel_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      394 2024-04-25 16:28:42.000000 unravel_python-1.5.2/src/unravel_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 16:28:42.000000 unravel_python-1.5.2/src/unravel_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2024-04-25 16:28:42.000000 unravel_python-1.5.2/src/unravel_python.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-25 16:28:42.000000 unravel_python-1.5.2/src/unravel_python.egg-info/top_level.txt
```

### Comparing `unravel_python-1.5.1/LICENSE` & `unravel_python-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `unravel_python-1.5.1/PKG-INFO` & `unravel_python-1.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unravel-python
-Version: 1.5.1
+Version: 1.5.2
 Summary: Implementation of UNRAVEL
 Author-email: Nicolas Delinte <nicolas.delinte@uclouvain.be>
 License: GNU General Public License v3.0
 Project-URL: GitHub, https://github.com/DelinteNicolas/UNRAVEL
 Project-URL: Documentation, https://unravel.readthedocs.io/en/latest/
 Keywords: tractography,multi-fixel
 Classifier: Intended Audience :: Science/Research
```

### Comparing `unravel_python-1.5.1/README.md` & `unravel_python-1.5.2/README.md`

 * *Files identical despite different names*

### Comparing `unravel_python-1.5.1/pyproject.toml` & `unravel_python-1.5.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `unravel_python-1.5.1/src/unravel/analysis.py` & `unravel_python-1.5.2/src/unravel/analysis.py`

 * *Files identical despite different names*

### Comparing `unravel_python-1.5.1/src/unravel/core.py` & `unravel_python-1.5.2/src/unravel/core.py`

 * *Files identical despite different names*

### Comparing `unravel_python-1.5.1/src/unravel/example.py` & `unravel_python-1.5.2/src/unravel/example.py`

 * *Files identical despite different names*

### Comparing `unravel_python-1.5.1/src/unravel/stream.py` & `unravel_python-1.5.2/src/unravel/stream.py`

 * *Files identical despite different names*

### Comparing `unravel_python-1.5.1/src/unravel/utils.py` & `unravel_python-1.5.2/src/unravel/utils.py`

 * *Files identical despite different names*

### Comparing `unravel_python-1.5.1/src/unravel/viz.py` & `unravel_python-1.5.2/src/unravel/viz.py`

 * *Files 2% similar despite different names*

```diff
@@ -537,15 +537,16 @@
     scalar : TYPE, optional
         DESCRIPTION. The default is None.
     opacity : float, optional
         DESCRIPTION. The default is 1.
     show_points : bool, optional
         Enable to show points instead of lines. The default is False.
     color_map : str, optional
-        Color map for the labels The default is None.
+        Color map for the labels. 'Set3' or 'tab20' recommend for
+        segmented color maps. The default is None.
     resolution_increase : int, optional
         DESCRIPTION. The default is 2.
     background : str, optional
         DESCRIPTION. The default is 'black'.
     plotter : TYPE, optional
         If not specifed, creates a new figure. The default is None.
 
@@ -626,29 +627,31 @@
                    scalars=scalars, rgb=rgb)
     p.background_color = background
     if plotter is None:
         p.show()
 
 
 def plot_metric_along_trajectory(mean, dev, new_fig: bool = True,
-                                 label: str = ''):
+                                 label: str = '', color: str = None):
     '''
     Plots the output of unravel.analysis.get_metric_along_trajectory.
 
     Parameters
     ----------
     mean : 1D array of size (n)
-        DESCRIPTION.
+        List of means for each subsection.
     dev : 1D array of size (n)
-        DESCRIPTION.
+        List of deviations for each subsection.
     new_fig : bool, optional
         If false, print the plot on the previous 'plt' figure. Useful when
         plotting multiple lines in a single plot. The default is True.
     label : str, optional
         Line label. The default is ''.
+    color : str, optional
+        Line color. The default is None.
 
     Returns
     -------
     None.
 
     '''
 
@@ -656,10 +659,12 @@
     std_spline = Akima1DInterpolator(range(len(mean)), dev)
     xs = np.arange(1, len(mean)-1, 0.1)
     ys = spline(xs)
     stds = std_spline(xs)
 
     if new_fig:
         plt.figure()
-    plt.plot(xs, ys, label=label)
+    p = plt.plot(xs, ys, label=label, color=color)
     plt.fill_between(xs, np.array(ys)-np.array(stds),
-                     np.array(ys) + np.array(stds), alpha=.15)
+                     np.array(ys) + np.array(stds),
+                     color=p[-1].get_color(), alpha=.15)
+    plt.xlim([1, len(mean)-1])
```

### Comparing `unravel_python-1.5.1/src/unravel_python.egg-info/PKG-INFO` & `unravel_python-1.5.2/src/unravel_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unravel-python
-Version: 1.5.1
+Version: 1.5.2
 Summary: Implementation of UNRAVEL
 Author-email: Nicolas Delinte <nicolas.delinte@uclouvain.be>
 License: GNU General Public License v3.0
 Project-URL: GitHub, https://github.com/DelinteNicolas/UNRAVEL
 Project-URL: Documentation, https://unravel.readthedocs.io/en/latest/
 Keywords: tractography,multi-fixel
 Classifier: Intended Audience :: Science/Research
```


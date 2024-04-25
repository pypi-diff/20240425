# Comparing `tmp/autoviz-0.1.808.tar.gz` & `tmp/autoviz-0.1.901.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autoviz-0.1.808.tar", last modified: Tue Apr  2 12:19:15 2024, max compression
+gzip compressed data, was "autoviz-0.1.901.tar", last modified: Thu Apr 25 11:03:02 2024, max compression
```

## Comparing `autoviz-0.1.808.tar` & `autoviz-0.1.901.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0 ram       (1000) ram       (1000)        0 2024-04-02 12:19:15.250666 autoviz-0.1.808/
--rwxrwxrwx   0 ram       (1000) ram       (1000)    17919 2024-04-02 12:19:15.250666 autoviz-0.1.808/PKG-INFO
--rwxrwxrwx   0 ram       (1000) ram       (1000)    15585 2024-03-30 12:37:03.000000 autoviz-0.1.808/README.md
-drwxrwxrwx   0 ram       (1000) ram       (1000)        0 2024-04-02 12:19:15.087843 autoviz-0.1.808/autoviz/
--rwxrwxrwx   0 ram       (1000) ram       (1000)    34934 2024-04-01 12:36:55.000000 autoviz-0.1.808/autoviz/AutoViz_Class.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)    64549 2024-04-02 11:28:31.000000 autoviz-0.1.808/autoviz/AutoViz_Holo.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)    24022 2024-04-01 11:59:10.000000 autoviz-0.1.808/autoviz/AutoViz_NLP.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)   117365 2024-04-02 11:29:27.000000 autoviz-0.1.808/autoviz/AutoViz_Utils.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)      875 2024-04-01 11:59:10.000000 autoviz-0.1.808/autoviz/__init__.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)      404 2024-04-02 11:12:43.000000 autoviz-0.1.808/autoviz/__version__.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)    18388 2024-04-01 11:59:10.000000 autoviz-0.1.808/autoviz/classify_method.py
-drwxrwxrwx   0 ram       (1000) ram       (1000)        0 2024-04-02 12:19:15.219415 autoviz-0.1.808/autoviz.egg-info/
--rwxrwxrwx   0 ram       (1000) ram       (1000)    17919 2024-04-02 12:19:14.000000 autoviz-0.1.808/autoviz.egg-info/PKG-INFO
--rwxrwxrwx   0 ram       (1000) ram       (1000)      339 2024-04-02 12:19:14.000000 autoviz-0.1.808/autoviz.egg-info/SOURCES.txt
--rwxrwxrwx   0 ram       (1000) ram       (1000)        1 2024-04-02 12:19:14.000000 autoviz-0.1.808/autoviz.egg-info/dependency_links.txt
--rwxrwxrwx   0 ram       (1000) ram       (1000)      258 2024-04-02 12:19:14.000000 autoviz-0.1.808/autoviz.egg-info/requires.txt
--rwxrwxrwx   0 ram       (1000) ram       (1000)        8 2024-04-02 12:19:14.000000 autoviz-0.1.808/autoviz.egg-info/top_level.txt
--rwxrwxrwx   0 ram       (1000) ram       (1000)       38 2024-04-02 12:19:15.250666 autoviz-0.1.808/setup.cfg
--rwxrwxrwx   0 ram       (1000) ram       (1000)     2963 2024-04-02 11:12:26.000000 autoviz-0.1.808/setup.py
+drwxrwxrwx   0 ram       (1000) ram       (1000)        0 2024-04-25 11:03:02.464404 autoviz-0.1.901/
+-rwxrwxrwx   0 ram       (1000) ram       (1000)    17919 2024-04-25 11:03:02.460260 autoviz-0.1.901/PKG-INFO
+-rwxrwxrwx   0 ram       (1000) ram       (1000)    15585 2024-03-30 12:37:03.000000 autoviz-0.1.901/README.md
+drwxrwxrwx   0 ram       (1000) ram       (1000)        0 2024-04-25 11:03:02.332745 autoviz-0.1.901/autoviz/
+-rwxrwxrwx   0 ram       (1000) ram       (1000)    34934 2024-04-01 12:36:55.000000 autoviz-0.1.901/autoviz/AutoViz_Class.py
+-rwxrwxrwx   0 ram       (1000) ram       (1000)    64881 2024-04-15 14:08:34.000000 autoviz-0.1.901/autoviz/AutoViz_Holo.py
+-rwxrwxrwx   0 ram       (1000) ram       (1000)    24022 2024-04-01 11:59:10.000000 autoviz-0.1.901/autoviz/AutoViz_NLP.py
+-rwxrwxrwx   0 ram       (1000) ram       (1000)   117365 2024-04-02 11:29:27.000000 autoviz-0.1.901/autoviz/AutoViz_Utils.py
+-rwxrwxrwx   0 ram       (1000) ram       (1000)      875 2024-04-01 11:59:10.000000 autoviz-0.1.901/autoviz/__init__.py
+-rwxrwxrwx   0 ram       (1000) ram       (1000)      404 2024-04-25 10:29:14.000000 autoviz-0.1.901/autoviz/__version__.py
+-rwxrwxrwx   0 ram       (1000) ram       (1000)    18388 2024-04-01 11:59:10.000000 autoviz-0.1.901/autoviz/classify_method.py
+drwxrwxrwx   0 ram       (1000) ram       (1000)        0 2024-04-25 11:03:02.440736 autoviz-0.1.901/autoviz.egg-info/
+-rwxrwxrwx   0 ram       (1000) ram       (1000)    17919 2024-04-25 11:03:01.000000 autoviz-0.1.901/autoviz.egg-info/PKG-INFO
+-rwxrwxrwx   0 ram       (1000) ram       (1000)      339 2024-04-25 11:03:01.000000 autoviz-0.1.901/autoviz.egg-info/SOURCES.txt
+-rwxrwxrwx   0 ram       (1000) ram       (1000)        1 2024-04-25 11:03:01.000000 autoviz-0.1.901/autoviz.egg-info/dependency_links.txt
+-rwxrwxrwx   0 ram       (1000) ram       (1000)      256 2024-04-25 11:03:01.000000 autoviz-0.1.901/autoviz.egg-info/requires.txt
+-rwxrwxrwx   0 ram       (1000) ram       (1000)        8 2024-04-25 11:03:01.000000 autoviz-0.1.901/autoviz.egg-info/top_level.txt
+-rwxrwxrwx   0 ram       (1000) ram       (1000)       38 2024-04-25 11:03:02.464404 autoviz-0.1.901/setup.cfg
+-rwxrwxrwx   0 ram       (1000) ram       (1000)     3013 2024-04-25 10:55:30.000000 autoviz-0.1.901/setup.py
```

### Comparing `autoviz-0.1.808/PKG-INFO` & `autoviz-0.1.901/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoviz
-Version: 0.1.808
+Version: 0.1.901
 Summary: Automatically Visualize any dataset, any size with a single line of code
 Home-page: https://github.com/AutoViML/AutoViz.git
 Author: Ram Seshadri
 License: Apache License 2.0
 Description: # AutoViz: The One-Line Automatic Data Visualization Library
         
         ![logo](images/logo.png)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: autoviz Version: 0.1.808 Summary: Automatically
+Metadata-Version: 2.1 Name: autoviz Version: 0.1.901 Summary: Automatically
 Visualize any dataset, any size with a single line of code Home-page: https://
 github.com/AutoViML/AutoViz.git Author: Ram Seshadri License: Apache License
 2.0 Description: # AutoViz: The One-Line Automatic Data Visualization Library !
 [logo](images/logo.png) Unlock the power of **AutoViz** to visualize any
 dataset, any size, with just a single line of code! Plus, now you can get a
 quick assessment of your dataset's quality and fix DQ issues through the FixDQ
 () function. [![Pepy Downloads](https://pepy.tech/badge/autoviz)](https://
```

### Comparing `autoviz-0.1.808/README.md` & `autoviz-0.1.901/README.md`

 * *Files identical despite different names*

### Comparing `autoviz-0.1.808/autoviz/AutoViz_Class.py` & `autoviz-0.1.901/autoviz/AutoViz_Class.py`

 * *Files identical despite different names*

### Comparing `autoviz-0.1.808/autoviz/AutoViz_Holo.py` & `autoviz-0.1.901/autoviz/AutoViz_Holo.py`

 * *Files 1% similar despite different names*

```diff
@@ -221,15 +221,20 @@
     except:
         ### This KDE plot errors a lot due to DynamicMaps of holoviews being buggy, so better to skip it!
         print('KDE plot is erroring due to problems with DynamicMaps. Hence it is skipped')
     if len(nums) > 0:
         drawobj5 = draw_violinplot_hv(dfin, dep, nums, chart_format, problem_type, mk_dir, verbose)
         ls_objects.append(drawobj5)
     if len(nums) > 0:
-        drawobj6 = draw_heatmap_hv(dfin, nums, chart_format, date_vars, dep, problem_type, classes, 
+        #### Adding int vars to nums since pandas has changed the df.corr() to error when cats are included ###
+        if len(cats) > 0:
+            nums_in = nums + dfin[cats].select_dtypes(include="number").columns.tolist()
+        else:
+            nums_in = nums[:]
+        drawobj6 = draw_heatmap_hv(dfin, nums_in, chart_format, date_vars, dep, problem_type, classes, 
                             mk_dir, verbose)
         ls_objects.append(drawobj6)
     if len(date_vars) > 0:
         drawobj7 = draw_date_vars_hv(dfin,dep,date_vars, nums, chart_format, problem_type, mk_dir, verbose)
         ls_objects.append(drawobj7)
     if len(nums) > 0 and len(cats) > 0:
         drawobj8 = draw_cat_vars_hv(dfin, dep, nums, cats, chart_format, problem_type, mk_dir, verbose)
@@ -1031,15 +1036,15 @@
         opts = dict(width=width_size, height=height_size, 
             line_color='black',
             line_width=1, line_dash='dotted', line_alpha=0.5)
         #opts['size'] = bubble_size
         opts['alpha'] = alpha
         opts['tools'] = ['hover']
         opts['toolbar'] = 'above'
-        opts['colorbar'] = True
+        #opts['colorbar'] = True
         #opts['color'] = next(colors)
         opts['title'] = title='Time Series plots of Numeric vars'
         dft = df.set_index(df[x])
         conti_df = df[[x,y]].set_index(df[x]).drop(x, axis=1)
         return hv.Curve(conti_df).opts(**opts)
 
     widgets = pn.WidgetBox(x, y)
@@ -1111,23 +1116,24 @@
         cols = 1
         if timeseries_flag:
             dft_target = dft[[dep]+conti].diff()
         else:
             dft_target = dft[conti]
             dft_target[dep] = dft[dep].values
         corre = dft_target.corr()
+        corre = corre.round(2)
         if timeseries_flag:
             heatmap = corre.hvplot.heatmap(height=height_size, width=width_size, colorbar=True, 
                     cmap=cmap_list, rot=70,
-            title='Time Series: Heatmap of all Differenced Continuous vars for target = %s' %dep)
+            title='Time Series: Heatmap of all Differenced Numeric vars for target = %s' %dep)
         else:
             heatmap = corre.hvplot.heatmap(height=height_size, width=width_size,  colorbar=True,
                     cmap=cmap_list,
                     rot=70,
-            title='Heatmap of all Continuous Variables including target');
+            title='Heatmap of all Numeric Variables including target');
         hv_plot = heatmap * hv.Labels(heatmap).opts(opts.Labels(text_font_size='7pt'))
         hv_panel = pn.panel(hv_plot)
         if verbose == 2:
             imgdata_list = append_panels(hv_panel, imgdata_list, chart_format)
             image_count += 1
     else:
         ### This is for Regression and None Dep variable problems only ##
@@ -1139,25 +1145,26 @@
         dft_target = dft[conti]
         if timeseries_flag:
             dft_target = dft_target.diff().dropna()
         else:
             dft_target = dft_target[:]
         N = len(conti)
         corre = dft_target.corr()
+        corre = corre.round(2)
         if timeseries_flag:
             heatmap = corre.hvplot.heatmap(height=height_size, width=width_size, colorbar=True, 
                     cmap=cmap_list,
                                            rot=70,
-                title='Time Series Data: Heatmap of Differenced Continuous vars including target').opts(
+                title='Time Series Data: Heatmap of Differenced Numeric vars including target').opts(
                         opts.HeatMap(tools=['hover'], toolbar='above'))
         else:
             heatmap = corre.hvplot.heatmap(height=height_size, width=width_size, colorbar=True, 
                     cmap=cmap_list,
                                            rot=70,
-            title='Heatmap of all Continuous Variables including target').opts(
+            title='Heatmap of all Numeric Variables including target').opts(
                                     opts.HeatMap(tools=['hover'],  toolbar='above'))
         hv_plot = heatmap * hv.Labels(heatmap).opts(opts.Labels(text_font_size='7pt'))
         hv_panel = pn.panel(hv_plot)
         if verbose == 2:
             imgdata_list = append_panels(hv_panel, imgdata_list, chart_format)
             image_count += 1
     ############# End of Heat Maps ##############
```

### Comparing `autoviz-0.1.808/autoviz/AutoViz_NLP.py` & `autoviz-0.1.901/autoviz/AutoViz_NLP.py`

 * *Files identical despite different names*

### Comparing `autoviz-0.1.808/autoviz/AutoViz_Utils.py` & `autoviz-0.1.901/autoviz/AutoViz_Utils.py`

 * *Files identical despite different names*

### Comparing `autoviz-0.1.808/autoviz/__init__.py` & `autoviz-0.1.901/autoviz/__init__.py`

 * *Files identical despite different names*

### Comparing `autoviz-0.1.808/autoviz/classify_method.py` & `autoviz-0.1.901/autoviz/classify_method.py`

 * *Files identical despite different names*

### Comparing `autoviz-0.1.808/autoviz.egg-info/PKG-INFO` & `autoviz-0.1.901/autoviz.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoviz
-Version: 0.1.808
+Version: 0.1.901
 Summary: Automatically Visualize any dataset, any size with a single line of code
 Home-page: https://github.com/AutoViML/AutoViz.git
 Author: Ram Seshadri
 License: Apache License 2.0
 Description: # AutoViz: The One-Line Automatic Data Visualization Library
         
         ![logo](images/logo.png)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: autoviz Version: 0.1.808 Summary: Automatically
+Metadata-Version: 2.1 Name: autoviz Version: 0.1.901 Summary: Automatically
 Visualize any dataset, any size with a single line of code Home-page: https://
 github.com/AutoViML/AutoViz.git Author: Ram Seshadri License: Apache License
 2.0 Description: # AutoViz: The One-Line Automatic Data Visualization Library !
 [logo](images/logo.png) Unlock the power of **AutoViz** to visualize any
 dataset, any size, with just a single line of code! Plus, now you can get a
 quick assessment of your dataset's quality and fix DQ issues through the FixDQ
 () function. [![Pepy Downloads](https://pepy.tech/badge/autoviz)](https://
```

### Comparing `autoviz-0.1.808/setup.py` & `autoviz-0.1.901/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,33 +25,33 @@
     "pandas-dq>=1.29"
 ]
 # Define default dependencies (compatible with older Python versions)
 install_requires = list_req
 
 if python_version <= (3, 10):
     install_requires = list_req + [
-    "numpy<1.25.0",  
+    "numpy<1.24",  # older version. otherwise you get numpy bool error
     "hvplot~=0.7.3",      # Older compatible version
     "holoviews<=1.14.9",  # Older compatible version
     "panel~=0.14.4", ## this is an old versjon of panel
     "param==1.13.0", ### something broke in panel without this
     "pandas<2.0", ## pandas must be below 2.0 version
     ]
 
 # For Python versions >= 3.10 and < 3.11, update the dependency list
 if (3, 10) < python_version <= (3, 11):
     install_requires = list_req + [
         # Keep most dependencies as is, adjust only where necessary
-        "numpy>=1.25.0",  # Update as needed for compatibility with newer HoloViews
+        "numpy>=1.24.0",  # Update as needed for compatibility with newer HoloViews
         # Update other dependencies as needed
         "hvplot>=0.9.2", ###newer hvplot
-        "holoviews>=1.15.3",  # Update based on the bug fix relevant to Python 3.10
+        "holoviews>=1.16.0",  # Update based on the bug fix relevant to Python 3.10
         # Ensure other dependencies are compatible
         "panel>=1.4.0", ## this is a new version of panel
-        "pandas<2.0", ## pandas must be below 2.0 version
+        "pandas>=2.0", ## pandas must be below 2.0 version
     ]
 
 # For Python versions >= 3.11, ensure HoloViews is at least 1.15.3 for the bug fix
 if python_version > (3, 11):
     install_requires = list_req + [
         # Adjust dependencies as needed for Python 3.11
         "numpy>=1.25.0",  # Update as needed for compatibility with newer HoloViews
@@ -60,15 +60,15 @@
         # Update or keep other dependencies as needed
         "panel>=1.4.0", ## this is a new version of panel
         "pandas<2.0", ## pandas must be below 2.0 version
     ]
 
 setuptools.setup(
     name="autoviz",
-    version="0.1.808",
+    version="0.1.901",
     author="Ram Seshadri",
     description="Automatically Visualize any dataset, any size with a single line of code",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='Apache License 2.0',
     url="https://github.com/AutoViML/AutoViz.git",
     packages=setuptools.find_packages(exclude=("tests",)),
```


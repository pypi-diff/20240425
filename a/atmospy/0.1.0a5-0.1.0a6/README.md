# Comparing `tmp/atmospy-0.1.0a5.tar.gz` & `tmp/atmospy-0.1.0a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atmospy-0.1.0a5.tar", max compression
+gzip compressed data, was "atmospy-0.1.0a6.tar", max compression
```

## Comparing `atmospy-0.1.0a5.tar` & `atmospy-0.1.0a6.tar`

### file list

```diff
@@ -1,13 +1,12 @@
--rw-r--r--   0        0        0    11323 2024-04-24 02:23:44.919094 atmospy-0.1.0a5/LICENSE
--rw-r--r--   0        0        0     1431 2024-04-24 02:23:44.919094 atmospy-0.1.0a5/README.md
--rw-r--r--   0        0        0      435 2024-04-24 02:23:44.919094 atmospy-0.1.0a5/atmospy/__init__.py
--rw-r--r--   0        0        0        0 2024-04-24 02:23:44.919094 atmospy-0.1.0a5/atmospy/_base.py
--rw-r--r--   0        0        0     8954 2024-04-24 02:23:44.919094 atmospy-0.1.0a5/atmospy/calendar.py
--rw-r--r--   0        0        0      640 2024-04-24 02:23:44.919094 atmospy-0.1.0a5/atmospy/distributions.py
--rw-r--r--   0        0        0     1190 2024-04-24 02:23:44.919094 atmospy-0.1.0a5/atmospy/rcmod.py
--rw-r--r--   0        0        0     2876 2024-04-24 02:23:44.919094 atmospy-0.1.0a5/atmospy/relational.py
--rw-r--r--   0        0        0     5466 2024-04-24 02:23:44.919094 atmospy-0.1.0a5/atmospy/rose.py
--rw-r--r--   0        0        0     2648 2024-04-24 02:23:44.919094 atmospy-0.1.0a5/atmospy/trends.py
--rw-r--r--   0        0        0     4038 2024-04-24 02:23:44.919094 atmospy-0.1.0a5/atmospy/utils.py
--rw-r--r--   0        0        0     1121 2024-04-24 02:23:44.919094 atmospy-0.1.0a5/pyproject.toml
--rw-r--r--   0        0        0     2469 1970-01-01 00:00:00.000000 atmospy-0.1.0a5/PKG-INFO
+-rw-r--r--   0        0        0    11323 2024-04-25 14:04:27.380619 atmospy-0.1.0a6/LICENSE
+-rw-r--r--   0        0        0     1603 2024-04-25 14:04:27.380619 atmospy-0.1.0a6/README.md
+-rw-r--r--   0        0        0      411 2024-04-25 14:04:27.380619 atmospy-0.1.0a6/atmospy/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 14:04:27.380619 atmospy-0.1.0a6/atmospy/_base.py
+-rw-r--r--   0        0        0      640 2024-04-25 14:04:27.380619 atmospy-0.1.0a6/atmospy/distributions.py
+-rw-r--r--   0        0        0     1936 2024-04-25 14:04:27.380619 atmospy-0.1.0a6/atmospy/rcmod.py
+-rw-r--r--   0        0        0     4519 2024-04-25 14:04:27.380619 atmospy-0.1.0a6/atmospy/relational.py
+-rw-r--r--   0        0        0     6828 2024-04-25 14:04:27.380619 atmospy-0.1.0a6/atmospy/rose.py
+-rw-r--r--   0        0        0    13082 2024-04-25 14:04:27.380619 atmospy-0.1.0a6/atmospy/trends.py
+-rw-r--r--   0        0        0     5208 2024-04-25 14:04:27.380619 atmospy-0.1.0a6/atmospy/utils.py
+-rw-r--r--   0        0        0     1292 2024-04-25 14:04:27.384619 atmospy-0.1.0a6/pyproject.toml
+-rw-r--r--   0        0        0     2641 1970-01-01 00:00:00.000000 atmospy-0.1.0a6/PKG-INFO
```

### Comparing `atmospy-0.1.0a5/LICENSE` & `atmospy-0.1.0a6/LICENSE`

 * *Files identical despite different names*

### Comparing `atmospy-0.1.0a5/README.md` & `atmospy-0.1.0a6/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,46 +1,58 @@
 # atmospy: air quality data visualization
 
 
-<!-- [![PyPI version](https://badge.fury.io/py/quantaq-cli.svg)](https://badge.fury.io/py/atmospy) -->
-<!-- ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/atmospy)
-[![license](https://img.shields.io/github/license/mashape/apistatus.svg)](https://github.com/quant-aq/atmospy/blob/master/LICENSE) -->
+[![PyPI version](https://badge.fury.io/py/atmospy.svg)](https://badge.fury.io/py/atmospy)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/atmospy)
 [![Tests](https://github.com/dhhagan/atmospy/actions/workflows/tests.yml/badge.svg)](https://github.com/dhhagan/atmospy/actions/workflows/tests.yml)
 [![codecov](https://codecov.io/gh/dhhagan/atmospy/branch/main/graph/badge.svg)](https://codecov.io/gh/dhhagan/atmospy)
 ![Apache 2.0 licensed](https://img.shields.io/github/license/dhhagan/atmospy)
 
 
-`atmospy` is a Python visualization library based on matplotlib and seaborn. 
+**atmospy** is a Python visualization library based on matplotlib and seaborn. 
 
 ## Documentation
 
-Coming soon.
+Documentation for **atmospy** can be found [here](https://dhhagan.github.io/atmospy/index.html).
 
 ## Dependencies
 
 ### Supported Python versions
 
-`atmospy` supports Python 3.8+.
+**atmospy** supports Python 3.8 through Python 3.11.
 
 ### Mandatory dependencies
 
   * numpy
   * pandas
   * seaborn
   * matplotlib
   * scipy
 
 ## Installation
 
-The latest stable release can by installed by installing directly from Github:
+The latest release can be installed directly from PyPi:
 
 ```sh
-$ pip install git+https://github.com/dhhagan/atmospy.git
+$ pip install atmospy
+```
+
+You can also install pre-releases from GitHub:
+
+```sh
+$ pip install atmospy --pre
+```
+
+If you would like to install from a specific branch or release, you can do so directly from GitHub:
+
+
+```sh
+$ pip install git+https://github.com/dhhagan/atmospy.git@<tag-or-version>
 ```
 
 ## Testing
 
 ## Development
 
-`atmospy` development takes place on GitHub: https://github.com/dhhagan/atmospy
+**atmospy** development takes place on GitHub: https://github.com/dhhagan/atmospy
 
 Please submit bugs that you encounter to the [issue tracker](https://github.com/dhhagan/atmospy/issues) with a reproducible example that clearly demonstrates the problem.
```

### Comparing `atmospy-0.1.0a5/atmospy/calendar.py` & `atmospy-0.1.0a6/atmospy/trends.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,34 +1,27 @@
-"""This file will contain figures for:
-
-  1. Calendar
-  2. straight line calendar thing like Sentry?
-"""
+import matplotlib as mpl
+import matplotlib.pyplot as plt
+import seaborn as sns
+import pandas as pd
+import numpy as np
+import math
 from .utils import (
-    remove_na,
-)
-from seaborn import (
-    FacetGrid,
-)
-from atmospy.utils import (
     check_for_numeric_cols,
     check_for_timestamp_col
 )
-import numpy as np
-import math
-import matplotlib as mpl
-import matplotlib.pyplot as plt
 
-__all__ = ["calendarplot", ]
+# Turn off chained assignment warnings
+pd.options.mode.chained_assignment = None
+
+__all__ = ["dielplot", "calendarplot"]
 
 @mpl.ticker.FuncFormatter
 def custom_month_formatter(x, pos):
     return str(math.ceil(x))
 
-
 def _yearplot(data, x, y, ax=None, agg="mean", cmap="crest", 
               height=2, aspect=5, vmin=None, vmax=None,
               linecolor="white", linewidths=0, cbar=True, cbar_kws=None, units=""):
     """Plot a full year of time series data on a heatmap by month.
     """
     if ax is None:
         ax = plt.gca()
@@ -36,16 +29,16 @@
         
     # if more than 1Y of data was provided, limit to 1Y
     years = np.unique(data.index.year)
     if years.size > 1:
         # warn
         data = data[data.index.year == years[0]]
         
-    data["Day of Week"] = data.index.weekday
-    data["Week of Year"] = data.index.isocalendar().week
+    data.loc[:, "Day of Week"] = data.index.weekday
+    data.loc[:, "Week of Year"] = data.index.isocalendar().week
     
     # compute pivoted data
     pivot = data.pivot_table(
         index="Day of Week", 
         columns="Week of Year", 
         values=y, 
         aggfunc=agg
@@ -128,16 +121,16 @@
     # if more than 1mo of data was provided, limit to 1mo
     months = np.unique(data.index.month)
     if months.size > 1:
         # TODO: log warning
         data = data[data.index.month == months[0]]
         
     # add pivot columns
-    data["Day of Month"] = data.index.day
-    data["Hour of Day"] = data.index.hour
+    data.loc[:, "Day of Month"] = data.index.day
+    data.loc[:, "Hour of Day"] = data.index.hour
     
     # compute the pivot data
     pivot = data.pivot_table(
         index="Hour of Day",
         columns="Day of Month",
         values=y,
         aggfunc=agg
@@ -190,24 +183,37 @@
     
     return ax
 
 
 def calendarplot(data, x, y, freq="day", agg="mean", vmin=None, vmax=None, cmap="crest", 
                  ax=None, linecolor="white", linewidths=0, cbar=True, cbar_kws=None,
                  xlabel=None, ylabel=None, title=None, units="", height=2, aspect=5.0):
-    """Create a heatmap from time series data.
+    """Visualize data as a heatmap on a monthly or annual basis.
+    
+    Calendar plots can be a useful way to visualize trends in data over longer periods 
+    of time. This function is quite generic and allows you to visualize data either by 
+    month (where the x-axis is day of month and y-axis is hour of day) or year (where 
+    x-axis is the week of the year and y-axis is the day of the week). Configure the plot
+    to aggregrate the data any way you choose (e.g., sum, mean, max).
+    
+    Currently, you can only plot a single month or single year at a time depending on 
+    configuration. To facet these, please set up a Seaborn FacetGrid and call the 
+    calendarplot separately.
+    
+    This function is heavily influenced by the `calplot <https://calplot.readthedocs.io/en/latest/>`_ 
+    python library.
     
     Parameters
     ----------
-    data : pd.DataFrame
-        Dataframe containing the data of interest.
-    x : str
-        The name of the datetime column.
-    y : str
-        The name of the data column.
+    data : :class:`pandas.DataFrame`
+        Tabular data as a pandas DataFrame.
+    x : key in `data`
+        Variable that corresponds to the timestamp column in `data`.
+    y : key in `data`
+        Variable that corresponds to the variable you would like to group and plot.
     freq : str, optional
         The frequency by which to average (one of [`hour`, `day`]), by default "day"
     agg : str, optional
         The function to aggregate by, by default "mean"
     vmin : float, optional
         The minimum value to color by, by default None
     vmax : float, optional
@@ -232,22 +238,26 @@
         The figure title, by default None
     units : str, optional
         The units of the plotted item for labeling purposes only, by default ""
     height : int, optional
         The figure height in inches, by default 2
     aspect : float, optional
         The aspect ratio of the figure, by default 5.0
-        
-    Examples
-    --------
     
     Returns
     -------
-    ax : axes object
-        TODO: Fill this out.
+    :class:`matplotlib.axes._axes.Axes`
+
+    Examples
+    --------
+    
+    Plot a simple heatmap for the entire year.
+
+    >>> df = atmospy.load_dataset("us-bc")
+    >>> atmospy.calendarplot(df, x="Timestamp GMT", y="Sample Measurement")
     
     """
     check_for_timestamp_col(data, x)
     check_for_numeric_cols(data, [y])
     
     if freq not in ("hour", "day"):
         raise ValueError("Invalid argument for `freq`")
@@ -292,8 +302,115 @@
     
     if xlabel:
         ax.set_xlabel(xlabel)
         
     if ylabel:
         ax.set_ylabel(ylabel)
     
+    return ax
+
+
+def dielplot(data, x, y, ax=None, ylim=None, xlabel=None, 
+             ylabel=None, title=None, plot_kws=None, **kwargs):
+    """Plot the diel (e.g., diurnal) trend for a pollutant.
+    
+    Diel plots can be incredibly useful for understanding daily 
+    patterns of air pollutants.
+
+    Parameters
+    ----------
+    data : :class:`pandas.DataFrame`
+        Tabular data as a pandas DataFrame.
+    x : key in `data`
+        Variable that corresponds to the timestamp in `data`.
+    y : key in `data`
+        Variable that corresponds to the pollutant of interest.
+    ax : :class:`matplotlib.axes._axes.Axes`, optional
+        An axis to plot on; if not defined, one will be created, by default None
+    ylim : tuple of floats, optional
+        A tuple describing (ymin, ymax), by default None
+    xlabel : str, optional
+        The label for the x-axis, by default None
+    ylabel : str, optional
+        The label for the y-axis, by default None
+    title : str, optional
+        The title for the plot, by default None
+    plot_kws : dict or None, optional
+        Additional keyword arguments are passed directly to the underlying plot call
+        , by default None
+        
+    Returns
+    -------
+    :class:`matplotlib.axes._axes.Axes`
+
+        
+    Examples
+    --------
+    
+    Plot a simple heatmap for the entire year.
+
+    >>> df = atmospy.load_dataset("us-bc")
+    >>> atmospy.dielplot(df, x="Timestamp GMT", y="Sample Measurement")
+    
+    """
+    default_plot_kws = {
+        "lw": 3,
+    }
+    
+    # complete some initial data quality checks
+    check_for_timestamp_col(data, x)
+    check_for_numeric_cols(data, [y])
+    
+    # 
+    plot_kws = {} if plot_kws is None else dict(default_plot_kws, **plot_kws)
+    
+    # copy over only the needed data
+    _data = data[[x, y]].copy(deep=True)
+    _data = _data.set_index(x)
+    
+    # 
+    # figure setup
+    if ax is None:
+        ax = plt.gca()
+        
+    # compute the diel statistics
+    stats = _data.groupby([_data.index.hour, _data.index.minute], as_index=False).describe()
+    
+    # build an index we can use to make the figure
+    index = stats.index.values
+    freq = int(60 / (index.size / 24))
+    figure_index = pd.date_range(start='2020-01-01', periods=index.size, freq=f"{freq}min")
+    
+    # plot the diel average
+    ax.plot(figure_index, stats[y]['mean'], **plot_kws)
+    
+    # add the IQR as a shaded region
+    ax.fill_between(
+        figure_index,
+        y1=stats[y]['25%'],
+        y2=stats[y]['75%'],
+        alpha=0.25,
+        lw=2,
+        color=plt.gca().lines[-1].get_color()
+    )
+    
+    # adjust plot parameters
+    xticks = ax.get_xticks()
+    ax.set_xticks(np.linspace(xticks[0], xticks[-1], 5))
+    ax.set(xlim=(xticks[0], xticks[-1]))
+    ax.xaxis.set_major_formatter(mpl.dates.DateFormatter("%I:%M\n%p"))
+    ax.xaxis.set_minor_locator(mpl.dates.HourLocator(interval=1))
+
+    # add optional labels
+    if xlabel:
+        ax.set_xlabel(xlabel)
+    
+    if ylabel:
+        ax.set_ylabel(ylabel)
+    
+    if title:
+        ax.set_title(title)
+        
+    if ylim:
+        ax.set_ylim(ylim)
+    
     return ax
```

### Comparing `atmospy-0.1.0a5/atmospy/distributions.py` & `atmospy-0.1.0a6/atmospy/distributions.py`

 * *Files identical despite different names*

### Comparing `atmospy-0.1.0a5/pyproject.toml` & `atmospy-0.1.0a6/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "atmospy"
-version = "0.1.0a5"
+version = "0.1.0a6"
 description = "Data analysis and visualization for air quality data."
 authors = ["David H Hagan <david.hagan@quant-aq.com>"]
 license = "Apache-2.0"
 maintainers = []
 readme = "README.md"
 homepage = "https://github.com/dhhagan/atmospy/"
 repository = "https://github.com/dhhagan/atmospy/"
@@ -32,14 +32,21 @@
 # sphinx-issues = "^1.2.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.1.1"
 pytest-cov = "^5.0.0"
 ipykernel = "^6.29.4"
 jupyter = "^1.0.0"
+sphinx = "<6.0.0"
+sphinx-copybutton = "^0.5.2"
+pydata-sphinx-theme = "0.10.0rc2"
+nbconvert = "^7.16.3"
+numpydoc = "^1.5"
+sphinx-issues = "^4.1.0"
+sphinx-design = "^0.5.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/quant-aq/atmospy/issues"
```

### Comparing `atmospy-0.1.0a5/PKG-INFO` & `atmospy-0.1.0a6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atmospy
-Version: 0.1.0a5
+Version: 0.1.0a6
 Summary: Data analysis and visualization for air quality data.
 Home-page: https://github.com/dhhagan/atmospy/
 License: Apache-2.0
 Author: David H Hagan
 Author-email: david.hagan@quant-aq.com
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: Apache Software License
@@ -23,50 +23,62 @@
 Project-URL: Documentation, https://dhhagan.github.io/atmospy/
 Project-URL: Repository, https://github.com/dhhagan/atmospy/
 Description-Content-Type: text/markdown
 
 # atmospy: air quality data visualization
 
 
-<!-- [![PyPI version](https://badge.fury.io/py/quantaq-cli.svg)](https://badge.fury.io/py/atmospy) -->
-<!-- ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/atmospy)
-[![license](https://img.shields.io/github/license/mashape/apistatus.svg)](https://github.com/quant-aq/atmospy/blob/master/LICENSE) -->
+[![PyPI version](https://badge.fury.io/py/atmospy.svg)](https://badge.fury.io/py/atmospy)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/atmospy)
 [![Tests](https://github.com/dhhagan/atmospy/actions/workflows/tests.yml/badge.svg)](https://github.com/dhhagan/atmospy/actions/workflows/tests.yml)
 [![codecov](https://codecov.io/gh/dhhagan/atmospy/branch/main/graph/badge.svg)](https://codecov.io/gh/dhhagan/atmospy)
 ![Apache 2.0 licensed](https://img.shields.io/github/license/dhhagan/atmospy)
 
 
-`atmospy` is a Python visualization library based on matplotlib and seaborn. 
+**atmospy** is a Python visualization library based on matplotlib and seaborn. 
 
 ## Documentation
 
-Coming soon.
+Documentation for **atmospy** can be found [here](https://dhhagan.github.io/atmospy/index.html).
 
 ## Dependencies
 
 ### Supported Python versions
 
-`atmospy` supports Python 3.8+.
+**atmospy** supports Python 3.8 through Python 3.11.
 
 ### Mandatory dependencies
 
   * numpy
   * pandas
   * seaborn
   * matplotlib
   * scipy
 
 ## Installation
 
-The latest stable release can by installed by installing directly from Github:
+The latest release can be installed directly from PyPi:
 
 ```sh
-$ pip install git+https://github.com/dhhagan/atmospy.git
+$ pip install atmospy
+```
+
+You can also install pre-releases from GitHub:
+
+```sh
+$ pip install atmospy --pre
+```
+
+If you would like to install from a specific branch or release, you can do so directly from GitHub:
+
+
+```sh
+$ pip install git+https://github.com/dhhagan/atmospy.git@<tag-or-version>
 ```
 
 ## Testing
 
 ## Development
 
-`atmospy` development takes place on GitHub: https://github.com/dhhagan/atmospy
+**atmospy** development takes place on GitHub: https://github.com/dhhagan/atmospy
 
 Please submit bugs that you encounter to the [issue tracker](https://github.com/dhhagan/atmospy/issues) with a reproducible example that clearly demonstrates the problem.
```


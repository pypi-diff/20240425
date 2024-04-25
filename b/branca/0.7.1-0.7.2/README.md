# Comparing `tmp/branca-0.7.1.tar.gz` & `tmp/branca-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "branca-0.7.1.tar", last modified: Tue Jan 30 18:32:40 2024, max compression
+gzip compressed data, was "branca-0.7.2.tar", last modified: Thu Apr 25 14:32:30 2024, max compression
```

## Comparing `branca-0.7.1.tar` & `branca-0.7.2.tar`

### file list

```diff
@@ -1,33 +1,31 @@
-drwxrwxr-x   0 filipe    (1000) filipe    (1000)        0 2024-01-30 18:32:40.162833 branca-0.7.1/
-drwxrwxr-x   0 filipe    (1000) filipe    (1000)        0 2024-01-30 18:32:40.154833 branca-0.7.1/.github/
-drwxrwxr-x   0 filipe    (1000) filipe    (1000)        0 2024-01-30 18:32:40.158833 branca-0.7.1/.github/workflows/
--rw-rw-r--   0 filipe    (1000) filipe    (1000)     1027 2023-11-06 17:10:54.000000 branca-0.7.1/.github/workflows/deploy-docs.yml
--rw-rw-r--   0 filipe    (1000) filipe    (1000)     1094 2022-11-09 17:37:13.000000 branca-0.7.1/.github/workflows/pypi.yml
--rw-rw-r--   0 filipe    (1000) filipe    (1000)     1151 2023-11-06 17:10:54.000000 branca-0.7.1/.github/workflows/test_code.yml
--rw-rw-r--   0 filipe    (1000) filipe    (1000)      667 2023-11-06 17:10:54.000000 branca-0.7.1/.github/workflows/test_code_notebooks.yml
--rw-rw-r--   0 filipe    (1000) filipe    (1000)      656 2023-11-06 17:10:54.000000 branca-0.7.1/.github/workflows/test_selenium.yml
--rw-rw-r--   0 filipe    (1000) filipe    (1000)     2210 2023-11-06 17:10:54.000000 branca-0.7.1/CHANGES.txt
--rw-rw-r--   0 filipe    (1000) filipe    (1000)     1079 2022-11-07 18:20:12.000000 branca-0.7.1/LICENSE.txt
--rw-rw-r--   0 filipe    (1000) filipe    (1000)      380 2022-11-07 19:04:46.000000 branca-0.7.1/MANIFEST.in
--rw-r--r--   0 filipe    (1000) filipe    (1000)     1476 2024-01-30 18:32:40.162833 branca-0.7.1/PKG-INFO
--rw-rw-r--   0 filipe    (1000) filipe    (1000)      728 2022-11-08 19:07:21.000000 branca-0.7.1/README.md
-drwxrwxr-x   0 filipe    (1000) filipe    (1000)        0 2024-01-30 18:32:40.162833 branca-0.7.1/branca/
--rw-rw-r--   0 filipe    (1000) filipe    (1000)      207 2022-11-08 19:07:21.000000 branca-0.7.1/branca/__init__.py
--rw-rw-r--   0 filipe    (1000) filipe    (1000)     3540 2022-11-08 19:07:21.000000 branca-0.7.1/branca/_cnames.json
--rw-rw-r--   0 filipe    (1000) filipe    (1000)    21192 2023-11-06 17:10:52.000000 branca-0.7.1/branca/_schemes.json
--rw-rw-r--   0 filipe    (1000) filipe    (1000)    20252 2024-01-30 18:29:21.000000 branca-0.7.1/branca/colormap.py
--rw-rw-r--   0 filipe    (1000) filipe    (1000)    22061 2023-11-23 14:28:41.000000 branca-0.7.1/branca/element.py
-drwxrwxr-x   0 filipe    (1000) filipe    (1000)        0 2024-01-30 18:32:40.162833 branca-0.7.1/branca/plugins/
--rw-rw-r--   0 filipe    (1000) filipe    (1000)      104 2022-11-08 19:07:21.000000 branca-0.7.1/branca/plugins/__init__.py
--rw-rw-r--   0 filipe    (1000) filipe    (1000)      370 2023-11-06 17:10:52.000000 branca-0.7.1/branca/scheme_base_codes.json
--rw-rw-r--   0 filipe    (1000) filipe    (1000)      904 2023-11-06 17:10:52.000000 branca-0.7.1/branca/scheme_info.json
-drwxrwxr-x   0 filipe    (1000) filipe    (1000)        0 2024-01-30 18:32:40.162833 branca-0.7.1/branca/templates/
--rw-rw-r--   0 filipe    (1000) filipe    (1000)     2300 2022-11-08 19:07:21.000000 branca-0.7.1/branca/templates/color_scale.js
--rw-rw-r--   0 filipe    (1000) filipe    (1000)    15499 2024-01-30 18:29:21.000000 branca-0.7.1/branca/utilities.py
-drwxrwxr-x   0 filipe    (1000) filipe    (1000)        0 2024-01-30 18:32:40.162833 branca-0.7.1/branca.egg-info/
--rw-rw-r--   0 filipe    (1000) filipe    (1000)      518 2024-01-30 18:32:40.000000 branca-0.7.1/branca.egg-info/SOURCES.txt
--rw-rw-r--   0 filipe    (1000) filipe    (1000)      105 2022-11-07 19:04:46.000000 branca-0.7.1/pyproject.toml
--rw-rw-r--   0 filipe    (1000) filipe    (1000)      224 2023-11-06 17:10:52.000000 branca-0.7.1/requirements-dev.txt
--rw-rw-r--   0 filipe    (1000) filipe    (1000)       10 2024-01-30 18:29:21.000000 branca-0.7.1/requirements.txt
--rw-rw-r--   0 filipe    (1000) filipe    (1000)      402 2024-01-30 18:32:40.162833 branca-0.7.1/setup.cfg
--rw-rw-r--   0 filipe    (1000) filipe    (1000)     2124 2022-11-08 19:07:21.000000 branca-0.7.1/setup.py
+drwxrwxr-x   0 filipe    (1000) filipe    (1000)        0 2024-04-25 14:32:30.939676 branca-0.7.2/
+drwxrwxr-x   0 filipe    (1000) filipe    (1000)        0 2024-04-25 14:32:30.931676 branca-0.7.2/.github/
+drwxrwxr-x   0 filipe    (1000) filipe    (1000)        0 2024-04-25 14:32:30.935676 branca-0.7.2/.github/workflows/
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)     1027 2023-11-06 17:10:54.000000 branca-0.7.2/.github/workflows/deploy-docs.yml
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)     1094 2022-11-09 17:37:13.000000 branca-0.7.2/.github/workflows/pypi.yml
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)      858 2024-04-16 18:42:17.000000 branca-0.7.2/.github/workflows/test_code.yml
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)      667 2023-11-06 17:10:54.000000 branca-0.7.2/.github/workflows/test_code_notebooks.yml
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)      656 2023-11-06 17:10:54.000000 branca-0.7.2/.github/workflows/test_selenium.yml
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)     2210 2023-11-06 17:10:54.000000 branca-0.7.2/CHANGES.txt
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)     1079 2022-11-07 18:20:12.000000 branca-0.7.2/LICENSE.txt
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)      380 2022-11-07 19:04:46.000000 branca-0.7.2/MANIFEST.in
+-rw-r--r--   0 filipe    (1000) filipe    (1000)     1477 2024-04-25 14:32:30.939676 branca-0.7.2/PKG-INFO
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)      728 2022-11-08 19:07:21.000000 branca-0.7.2/README.md
+drwxrwxr-x   0 filipe    (1000) filipe    (1000)        0 2024-04-25 14:32:30.939676 branca-0.7.2/branca/
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)      207 2022-11-08 19:07:21.000000 branca-0.7.2/branca/__init__.py
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)     3540 2022-11-08 19:07:21.000000 branca-0.7.2/branca/_cnames.json
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)    21192 2023-11-06 17:10:52.000000 branca-0.7.2/branca/_schemes.json
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)    20378 2024-04-16 18:42:17.000000 branca-0.7.2/branca/colormap.py
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)    22061 2023-11-23 14:28:41.000000 branca-0.7.2/branca/element.py
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)      370 2023-11-06 17:10:52.000000 branca-0.7.2/branca/scheme_base_codes.json
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)      904 2023-11-06 17:10:52.000000 branca-0.7.2/branca/scheme_info.json
+drwxrwxr-x   0 filipe    (1000) filipe    (1000)        0 2024-04-25 14:32:30.939676 branca-0.7.2/branca/templates/
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)     2300 2022-11-08 19:07:21.000000 branca-0.7.2/branca/templates/color_scale.js
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)    14549 2024-04-16 18:42:17.000000 branca-0.7.2/branca/utilities.py
+drwxrwxr-x   0 filipe    (1000) filipe    (1000)        0 2024-04-25 14:32:30.939676 branca-0.7.2/branca.egg-info/
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)      491 2024-04-25 14:32:30.000000 branca-0.7.2/branca.egg-info/SOURCES.txt
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)      105 2022-11-07 19:04:46.000000 branca-0.7.2/pyproject.toml
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)      224 2023-11-06 17:10:52.000000 branca-0.7.2/requirements-dev.txt
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)       10 2024-01-30 18:29:21.000000 branca-0.7.2/requirements.txt
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)      402 2024-04-25 14:32:30.939676 branca-0.7.2/setup.cfg
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)     2125 2024-04-16 18:42:17.000000 branca-0.7.2/setup.py
```

### Comparing `branca-0.7.1/.github/workflows/deploy-docs.yml` & `branca-0.7.2/.github/workflows/deploy-docs.yml`

 * *Files identical despite different names*

### Comparing `branca-0.7.1/.github/workflows/pypi.yml` & `branca-0.7.2/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `branca-0.7.1/.github/workflows/test_code_notebooks.yml` & `branca-0.7.2/.github/workflows/test_code_notebooks.yml`

 * *Files identical despite different names*

### Comparing `branca-0.7.1/.github/workflows/test_selenium.yml` & `branca-0.7.2/.github/workflows/test_selenium.yml`

 * *Files identical despite different names*

### Comparing `branca-0.7.1/CHANGES.txt` & `branca-0.7.2/CHANGES.txt`

 * *Files identical despite different names*

### Comparing `branca-0.7.1/LICENSE.txt` & `branca-0.7.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `branca-0.7.1/PKG-INFO` & `branca-0.7.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: branca
-Version: 0.7.1
+Version: 0.7.2
 Summary: Generate complex HTML+JS pages with Python
 Home-page: https://github.com/python-visualization/branca
 Author: Martin Journois
 License: MIT
 Keywords: data visualization
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 5 - Production/Stable
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: jinja2>=3
```

### Comparing `branca-0.7.1/README.md` & `branca-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `branca-0.7.1/branca/_cnames.json` & `branca-0.7.2/branca/_cnames.json`

 * *Files identical despite different names*

### Comparing `branca-0.7.1/branca/_schemes.json` & `branca-0.7.2/branca/_schemes.json`

 * *Files identical despite different names*

### Comparing `branca-0.7.1/branca/colormap.py` & `branca-0.7.2/branca/colormap.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,17 +91,21 @@
 
         self.width = 450
         self.height = 40
 
     def render(self, **kwargs):
         """Renders the HTML representation of the element."""
         self.color_domain = [
-            self.vmin + (self.vmax - self.vmin) * k / 499.0 for k in range(500)
+            float(self.vmin + (self.vmax - self.vmin) * k / 499.0) for k in range(500)
         ]
         self.color_range = [self.__call__(x) for x in self.color_domain]
+
+        # sanitize possible numpy floats to native python floats
+        self.index = [float(i) for i in self.index]
+
         if self.tick_labels is None:
             self.tick_labels = legend_scaler(self.index, self.max_labels)
 
         super().render(**kwargs)
 
         figure = self.get_root()
         assert isinstance(figure, Figure), (
```

### Comparing `branca-0.7.1/branca/element.py` & `branca-0.7.2/branca/element.py`

 * *Files identical despite different names*

### Comparing `branca-0.7.1/branca/scheme_info.json` & `branca-0.7.2/branca/scheme_info.json`

 * *Files identical despite different names*

### Comparing `branca-0.7.1/branca/templates/color_scale.js` & `branca-0.7.2/branca/templates/color_scale.js`

 * *Files identical despite different names*

### Comparing `branca-0.7.1/branca/utilities.py` & `branca-0.7.2/branca/utilities.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,19 +15,14 @@
 import typing
 import zlib
 from typing import Any, Callable, Union
 
 from jinja2 import Environment, PackageLoader
 
 try:
-    import pandas as pd
-except ImportError:
-    pd = None
-
-try:
     import numpy as np
 except ImportError:
     np = None
 
 if typing.TYPE_CHECKING:
     from branca.colormap import ColorMap
 
@@ -199,47 +194,14 @@
         if not color_reverse:
             color_scheme = schemes.get(core_color_code, None)
         else:
             color_scheme = schemes.get(core_color_code, None)[::-1]
     return color_scheme
 
 
-def split_six(series=None):
-    """
-    Given a Pandas Series, get a domain of values from zero to the 90% quantile
-    rounded to the nearest order-of-magnitude integer. For example, 2100 is
-    rounded to 2000, 2790 to 3000.
-
-    Parameters
-    ----------
-    series: Pandas series, default None
-
-    Returns
-    -------
-    list
-
-    """
-    if pd is None:
-        raise ImportError("The Pandas package is required" " for this functionality")
-    if np is None:
-        raise ImportError("The NumPy package is required" " for this functionality")
-
-    def base(x):
-        if x > 0:
-            base = pow(10, math.floor(math.log10(x)))
-            return round(x / base) * base
-        else:
-            return 0
-
-    quants = [0, 50, 75, 85, 90]
-    # Some weirdness in series quantiles a la 0.13.
-    arr = series.values
-    return [base(np.percentile(arr, x)) for x in quants]
-
-
 def image_to_url(image, colormap=None, origin="upper"):
     """Infers the type of an image argument and transforms it into a URL.
 
     Parameters
     ----------
     image: string, file or array-like object
         * If string, it will be written directly in the output file.
```

### Comparing `branca-0.7.1/setup.py` & `branca-0.7.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,19 +49,19 @@
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Martin Journois",
     url="https://github.com/python-visualization/branca",
     keywords="data visualization",
     classifiers=[
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "License :: OSI Approved :: MIT License",
         "Development Status :: 5 - Production/Stable",
     ],
     packages=pkgs,
     package_data=pkg_data,
     include_package_data=True,
     use_scm_version={
```


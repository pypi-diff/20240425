# Comparing `tmp/fknni-1.0.0.tar.gz` & `tmp/fknni-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fknni-1.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "fknni-1.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `fknni-1.0.0.tar` & `fknni-1.1.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0      289 2024-04-23 19:36:04.020086 fknni-1.0.0/.codecov.yaml
--rw-r--r--   0        0        0      937 2024-04-23 20:01:11.452795 fknni-1.0.0/.cruft.json
--rw-r--r--   0        0        0      241 2024-04-23 19:36:04.020086 fknni-1.0.0/.editorconfig
--rw-r--r--   0        0        0     3080 2024-04-23 19:36:04.050086 fknni-1.0.0/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0        0        0      197 2024-04-23 19:36:04.053419 fknni-1.0.0/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      389 2024-04-23 20:02:59.097036 fknni-1.0.0/.github/ISSUE_TEMPLATE/feature_request.yml
--rw-r--r--   0        0        0      702 2024-04-24 11:23:22.038420 fknni-1.0.0/.github/workflows/build.yaml
--rw-r--r--   0        0        0      763 2024-04-24 11:23:22.011753 fknni-1.0.0/.github/workflows/release.yaml
--rw-r--r--   0        0        0     1546 2024-04-24 11:23:22.055087 fknni-1.0.0/.github/workflows/test.yaml
--rw-r--r--   0        0        0      289 2024-04-23 19:39:14.425024 fknni-1.0.0/.gitignore
--rw-r--r--   0        0        0     1352 2024-04-23 19:41:51.476348 fknni-1.0.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      325 2024-04-23 21:45:01.535357 fknni-1.0.0/.readthedocs.yaml
--rw-r--r--   0        0        0      405 2024-04-24 11:32:08.916359 fknni-1.0.0/CHANGELOG.md
--rw-r--r--   0        0        0    10798 2024-04-23 19:38:26.364619 fknni-1.0.0/LICENSE
--rw-r--r--   0        0        0     1613 2024-04-24 11:32:28.956168 fknni-1.0.0/README.md
--rw-r--r--   0        0        0      634 2024-04-23 19:36:04.060086 fknni-1.0.0/docs/Makefile
--rw-r--r--   0        0        0        0 2024-04-23 19:36:04.090086 fknni-1.0.0/docs/_static/.gitkeep
--rw-r--r--   0        0        0      165 2024-04-23 19:36:04.090086 fknni-1.0.0/docs/_static/css/custom.css
--rw-r--r--   0        0        0        0 2024-04-23 19:36:04.093420 fknni-1.0.0/docs/_templates/.gitkeep
--rw-r--r--   0        0        0     1026 2024-04-23 19:36:04.093420 fknni-1.0.0/docs/_templates/autosummary/class.rst
--rw-r--r--   0        0        0      150 2024-04-23 21:45:01.538690 fknni-1.0.0/docs/api.md
--rw-r--r--   0        0        0       34 2024-04-23 19:36:04.060086 fknni-1.0.0/docs/changelog.md
--rw-r--r--   0        0        0     3734 2024-04-23 21:45:01.538690 fknni-1.0.0/docs/conf.py
--rw-r--r--   0        0        0     7199 2024-04-23 20:03:19.820544 fknni-1.0.0/docs/contributing.md
--rw-r--r--   0        0        0     1028 2024-04-23 19:36:04.096753 fknni-1.0.0/docs/extensions/typed_returns.py
--rw-r--r--   0        0        0      144 2024-04-24 11:07:56.997960 fknni-1.0.0/docs/index.md
--rw-r--r--   0        0        0    34226 2024-04-24 11:25:57.149097 fknni-1.0.0/docs/notebooks/faiss.ipynb
--rw-r--r--   0        0        0     1046 2024-04-23 19:36:04.083420 fknni-1.0.0/docs/references.bib
--rw-r--r--   0        0        0       44 2024-04-23 19:36:04.083420 fknni-1.0.0/docs/references.md
--rw-r--r--   0        0        0     3198 2024-04-24 11:23:22.028420 fknni-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      125 2024-04-24 07:30:01.767795 fknni-1.0.0/src/fknni/__init__.py
--rw-r--r--   0        0        0       32 2024-04-23 20:40:28.600844 fknni-1.0.0/src/fknni/faiss/__init__.py
--rw-r--r--   0        0        0     5094 2024-04-24 11:02:50.400263 fknni-1.0.0/src/fknni/faiss/faiss.py
--rw-r--r--   0        0        0     1169 2024-04-23 20:54:35.393725 fknni-1.0.0/tests/test_faiss_imputation.py
--rw-r--r--   0        0        0     2877 1970-01-01 00:00:00.000000 fknni-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      289 2024-04-23 19:36:04.020086 fknni-1.1.0/.codecov.yaml
+-rw-r--r--   0        0        0      937 2024-04-23 20:01:11.452795 fknni-1.1.0/.cruft.json
+-rw-r--r--   0        0        0      241 2024-04-23 19:36:04.020086 fknni-1.1.0/.editorconfig
+-rw-r--r--   0        0        0     3080 2024-04-23 19:36:04.050086 fknni-1.1.0/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0        0        0       27 2024-04-24 13:16:19.127409 fknni-1.1.0/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      389 2024-04-23 20:02:59.097036 fknni-1.1.0/.github/ISSUE_TEMPLATE/feature_request.yml
+-rw-r--r--   0        0        0      702 2024-04-24 11:23:22.038420 fknni-1.1.0/.github/workflows/build.yaml
+-rw-r--r--   0        0        0      763 2024-04-24 11:23:22.011753 fknni-1.1.0/.github/workflows/release.yaml
+-rw-r--r--   0        0        0     1546 2024-04-24 11:23:22.055087 fknni-1.1.0/.github/workflows/test.yaml
+-rw-r--r--   0        0        0      289 2024-04-23 19:39:14.425024 fknni-1.1.0/.gitignore
+-rw-r--r--   0        0        0     1352 2024-04-23 19:41:51.476348 fknni-1.1.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      325 2024-04-23 21:45:01.535357 fknni-1.1.0/.readthedocs.yaml
+-rw-r--r--   0        0        0      405 2024-04-24 11:32:08.916359 fknni-1.1.0/CHANGELOG.md
+-rw-r--r--   0        0        0    10798 2024-04-23 19:38:26.364619 fknni-1.1.0/LICENSE
+-rw-r--r--   0        0        0     1609 2024-04-24 15:07:20.818527 fknni-1.1.0/README.md
+-rw-r--r--   0        0        0      634 2024-04-23 19:36:04.060086 fknni-1.1.0/docs/Makefile
+-rw-r--r--   0        0        0        0 2024-04-23 19:36:04.090086 fknni-1.1.0/docs/_static/.gitkeep
+-rw-r--r--   0        0        0      165 2024-04-23 19:36:04.090086 fknni-1.1.0/docs/_static/css/custom.css
+-rw-r--r--   0        0        0        0 2024-04-23 19:36:04.093420 fknni-1.1.0/docs/_templates/.gitkeep
+-rw-r--r--   0        0        0     1026 2024-04-23 19:36:04.093420 fknni-1.1.0/docs/_templates/autosummary/class.rst
+-rw-r--r--   0        0        0      150 2024-04-23 21:45:01.538690 fknni-1.1.0/docs/api.md
+-rw-r--r--   0        0        0       34 2024-04-23 19:36:04.060086 fknni-1.1.0/docs/changelog.md
+-rw-r--r--   0        0        0     3734 2024-04-23 21:45:01.538690 fknni-1.1.0/docs/conf.py
+-rw-r--r--   0        0        0     7199 2024-04-23 20:03:19.820544 fknni-1.1.0/docs/contributing.md
+-rw-r--r--   0        0        0     1028 2024-04-23 19:36:04.096753 fknni-1.1.0/docs/extensions/typed_returns.py
+-rw-r--r--   0        0        0      144 2024-04-24 11:07:56.997960 fknni-1.1.0/docs/index.md
+-rw-r--r--   0        0        0    34788 2024-04-25 16:10:00.897320 fknni-1.1.0/docs/notebooks/faiss.ipynb
+-rw-r--r--   0        0        0     1046 2024-04-23 19:36:04.083420 fknni-1.1.0/docs/references.bib
+-rw-r--r--   0        0        0       44 2024-04-23 19:36:04.083420 fknni-1.1.0/docs/references.md
+-rw-r--r--   0        0        0     3197 2024-04-25 16:10:00.897320 fknni-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0      125 2024-04-24 07:30:01.767795 fknni-1.1.0/src/fknni/__init__.py
+-rw-r--r--   0        0        0       32 2024-04-23 20:40:28.600844 fknni-1.1.0/src/fknni/faiss/__init__.py
+-rw-r--r--   0        0        0     4950 2024-04-25 16:10:00.897320 fknni-1.1.0/src/fknni/faiss/faiss.py
+-rw-r--r--   0        0        0     1169 2024-04-23 20:54:35.393725 fknni-1.1.0/tests/test_faiss_imputation.py
+-rw-r--r--   0        0        0     2872 1970-01-01 00:00:00.000000 fknni-1.1.0/PKG-INFO
```

### Comparing `fknni-1.0.0/.cruft.json` & `fknni-1.1.0/.cruft.json`

 * *Files identical despite different names*

### Comparing `fknni-1.0.0/.github/ISSUE_TEMPLATE/bug_report.yml` & `fknni-1.1.0/.github/ISSUE_TEMPLATE/bug_report.yml`

 * *Files identical despite different names*

### Comparing `fknni-1.0.0/.github/workflows/build.yaml` & `fknni-1.1.0/.github/workflows/build.yaml`

 * *Files identical despite different names*

### Comparing `fknni-1.0.0/.github/workflows/release.yaml` & `fknni-1.1.0/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `fknni-1.0.0/.github/workflows/test.yaml` & `fknni-1.1.0/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `fknni-1.0.0/.pre-commit-config.yaml` & `fknni-1.1.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `fknni-1.0.0/LICENSE` & `fknni-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fknni-1.0.0/README.md` & `fknni-1.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 -   [Faiss example notebook][link-faiss-example].
 
 ## Installation
 
 You need to have Python 3.10 or newer installed on your system.
 If you don't have Python installed, we recommend installing [Mambaforge](https://github.com/conda-forge/miniforge#mambaforge).
 
-Install the latest release of `fknni` from `PyPI <https://pypi.org/project/fknni/>`\_:
+Install the latest release of `fknni` from [PyPI](https://pypi.org/project/fknni):
 
 ```bash
 pip install fknni
 ```
 
 Install the latest development version:
```

### Comparing `fknni-1.0.0/docs/Makefile` & `fknni-1.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `fknni-1.0.0/docs/_templates/autosummary/class.rst` & `fknni-1.1.0/docs/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `fknni-1.0.0/docs/conf.py` & `fknni-1.1.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `fknni-1.0.0/docs/contributing.md` & `fknni-1.1.0/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `fknni-1.0.0/docs/extensions/typed_returns.py` & `fknni-1.1.0/docs/extensions/typed_returns.py`

 * *Files identical despite different names*

### Comparing `fknni-1.0.0/docs/notebooks/faiss.ipynb` & `fknni-1.1.0/docs/notebooks/faiss.ipynb`

 * *Files 15% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.975517113095238%*

 * *Differences: {"'cells'": "{3: {'metadata': {'ExecuteTime': {'end_time': '2024-04-25T13:28:24.303873023Z', "*

 * *            "'start_time': '2024-04-25T13:28:23.142744575Z'}}}, 4: {'metadata': {'ExecuteTime': "*

 * *            "{'end_time': '2024-04-25T13:28:24.305268342Z', 'start_time': "*

 * *            "'2024-04-25T13:28:24.303696739Z'}}}, 5: {'metadata': {'ExecuteTime': {'end_time': "*

 * *            "'2024-04-25T13:28:24.306365966Z', 'start_time': '2024-04-25T13:28:24.303915508Z'}}}, "*

 * *            "6: {'execution_count': 4, 'metada […]*

```diff
@@ -27,16 +27,16 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 1,
             "metadata": {
                 "ExecuteTime": {
-                    "end_time": "2024-04-24T10:54:54.274792998Z",
-                    "start_time": "2024-04-24T10:54:51.910270112Z"
+                    "end_time": "2024-04-25T13:28:24.303873023Z",
+                    "start_time": "2024-04-25T13:28:23.142744575Z"
                 },
                 "collapsed": false
             },
             "outputs": [],
             "source": [
                 "import numpy as np\n",
                 "import pandas as pd\n",
@@ -45,16 +45,16 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 2,
             "metadata": {
                 "ExecuteTime": {
-                    "end_time": "2024-04-24T10:54:54.404276414Z",
-                    "start_time": "2024-04-24T10:54:54.315428592Z"
+                    "end_time": "2024-04-25T13:28:24.305268342Z",
+                    "start_time": "2024-04-25T13:28:24.303696739Z"
                 },
                 "collapsed": false
             },
             "outputs": [
                 {
                     "data": {
                         "text/html": "<div>\n<style scoped>\n    .dataframe tbody tr th:only-of-type {\n        vertical-align: middle;\n    }\n\n    .dataframe tbody tr th {\n        vertical-align: top;\n    }\n\n    .dataframe thead th {\n        text-align: right;\n    }\n</style>\n<table border=\"1\" class=\"dataframe\">\n  <thead>\n    <tr style=\"text-align: right;\">\n      <th></th>\n      <th>A</th>\n      <th>B</th>\n      <th>C</th>\n      <th>D</th>\n      <th>E</th>\n    </tr>\n  </thead>\n  <tbody>\n    <tr>\n      <th>0</th>\n      <td>85</td>\n      <td>63</td>\n      <td>51</td>\n      <td>26</td>\n      <td>30</td>\n    </tr>\n    <tr>\n      <th>1</th>\n      <td>4</td>\n      <td>7</td>\n      <td>1</td>\n      <td>17</td>\n      <td>81</td>\n    </tr>\n    <tr>\n      <th>2</th>\n      <td>64</td>\n      <td>91</td>\n      <td>50</td>\n      <td>60</td>\n      <td>97</td>\n    </tr>\n    <tr>\n      <th>3</th>\n      <td>72</td>\n      <td>63</td>\n      <td>54</td>\n      <td>55</td>\n      <td>93</td>\n    </tr>\n    <tr>\n      <th>4</th>\n      <td>27</td>\n      <td>81</td>\n      <td>67</td>\n      <td>0</td>\n      <td>39</td>\n    </tr>\n    <tr>\n      <th>5</th>\n      <td>85</td>\n      <td>55</td>\n      <td>3</td>\n      <td>76</td>\n      <td>72</td>\n    </tr>\n    <tr>\n      <th>6</th>\n      <td>84</td>\n      <td>17</td>\n      <td>8</td>\n      <td>86</td>\n      <td>2</td>\n    </tr>\n    <tr>\n      <th>7</th>\n      <td>54</td>\n      <td>8</td>\n      <td>29</td>\n      <td>48</td>\n      <td>42</td>\n    </tr>\n    <tr>\n      <th>8</th>\n      <td>40</td>\n      <td>2</td>\n      <td>0</td>\n      <td>12</td>\n      <td>0</td>\n    </tr>\n    <tr>\n      <th>9</th>\n      <td>67</td>\n      <td>52</td>\n      <td>64</td>\n      <td>25</td>\n      <td>61</td>\n    </tr>\n  </tbody>\n</table>\n</div>",
@@ -74,16 +74,16 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 3,
             "metadata": {
                 "ExecuteTime": {
-                    "end_time": "2024-04-24T10:54:54.405925984Z",
-                    "start_time": "2024-04-24T10:54:54.324637066Z"
+                    "end_time": "2024-04-25T13:28:24.306365966Z",
+                    "start_time": "2024-04-25T13:28:24.303915508Z"
                 },
                 "collapsed": false
             },
             "outputs": [
                 {
                     "data": {
                         "text/html": "<div>\n<style scoped>\n    .dataframe tbody tr th:only-of-type {\n        vertical-align: middle;\n    }\n\n    .dataframe tbody tr th {\n        vertical-align: top;\n    }\n\n    .dataframe thead th {\n        text-align: right;\n    }\n</style>\n<table border=\"1\" class=\"dataframe\">\n  <thead>\n    <tr style=\"text-align: right;\">\n      <th></th>\n      <th>A</th>\n      <th>B</th>\n      <th>C</th>\n      <th>D</th>\n      <th>E</th>\n    </tr>\n  </thead>\n  <tbody>\n    <tr>\n      <th>0</th>\n      <td>85.0</td>\n      <td>63.0</td>\n      <td>51.0</td>\n      <td>26.0</td>\n      <td>30.0</td>\n    </tr>\n    <tr>\n      <th>1</th>\n      <td>NaN</td>\n      <td>7.0</td>\n      <td>NaN</td>\n      <td>17.0</td>\n      <td>NaN</td>\n    </tr>\n    <tr>\n      <th>2</th>\n      <td>64.0</td>\n      <td>NaN</td>\n      <td>50.0</td>\n      <td>60.0</td>\n      <td>NaN</td>\n    </tr>\n    <tr>\n      <th>3</th>\n      <td>72.0</td>\n      <td>63.0</td>\n      <td>54.0</td>\n      <td>55.0</td>\n      <td>NaN</td>\n    </tr>\n    <tr>\n      <th>4</th>\n      <td>NaN</td>\n      <td>81.0</td>\n      <td>67.0</td>\n      <td>0.0</td>\n      <td>39.0</td>\n    </tr>\n    <tr>\n      <th>5</th>\n      <td>85.0</td>\n      <td>55.0</td>\n      <td>3.0</td>\n      <td>76.0</td>\n      <td>72.0</td>\n    </tr>\n    <tr>\n      <th>6</th>\n      <td>84.0</td>\n      <td>17.0</td>\n      <td>8.0</td>\n      <td>86.0</td>\n      <td>2.0</td>\n    </tr>\n    <tr>\n      <th>7</th>\n      <td>54.0</td>\n      <td>NaN</td>\n      <td>29.0</td>\n      <td>48.0</td>\n      <td>42.0</td>\n    </tr>\n    <tr>\n      <th>8</th>\n      <td>NaN</td>\n      <td>2.0</td>\n      <td>0.0</td>\n      <td>12.0</td>\n      <td>0.0</td>\n    </tr>\n    <tr>\n      <th>9</th>\n      <td>67.0</td>\n      <td>52.0</td>\n      <td>64.0</td>\n      <td>NaN</td>\n      <td>61.0</td>\n    </tr>\n  </tbody>\n</table>\n</div>",
@@ -101,130 +101,180 @@
                 "for i, j in indices[:10]:\n",
                 "    df_missing.iat[i, j] = np.nan\n",
                 "df_missing"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 8,
+            "execution_count": 4,
             "metadata": {
                 "ExecuteTime": {
-                    "end_time": "2024-04-24T10:58:11.360790550Z",
-                    "start_time": "2024-04-24T10:58:11.315812849Z"
+                    "end_time": "2024-04-25T13:28:24.316976982Z",
+                    "start_time": "2024-04-25T13:28:24.304031716Z"
                 },
                 "collapsed": false
             },
             "outputs": [
                 {
                     "data": {
-                        "text/plain": "array([[85.        , 63.        , 51.        , 26.        , 30.        ],\n       [69.80000305,  7.        , 33.2444458 , 17.        , 28.45714378],\n       [64.        , 52.59999847, 50.        , 60.        , 40.65714264],\n       [72.        , 63.        , 54.        , 55.        , 40.65714264],\n       [72.19999695, 81.        , 67.        ,  0.        , 39.        ],\n       [85.        , 55.        ,  3.        , 76.        , 72.        ],\n       [84.        , 17.        ,  8.        , 86.        ,  2.        ],\n       [54.        , 52.59999847, 29.        , 48.        , 42.        ],\n       [73.80000305,  2.        ,  0.        , 12.        ,  0.        ],\n       [67.        , 52.        , 64.        , 46.2444458 , 61.        ]])"
+                        "text/plain": "array([[85.      , 63.      , 51.      , 26.      , 30.      ],\n       [76.72608 ,  7.      , 47.481873, 17.      , 23.080992],\n       [64.      , 44.638355, 50.      , 60.      , 29.523823],\n       [72.      , 63.      , 54.      , 55.      , 28.8196  ],\n       [82.59041 , 81.      , 67.      ,  0.      , 39.      ],\n       [85.      , 55.      ,  3.      , 76.      , 72.      ],\n       [84.      , 17.      ,  8.      , 86.      ,  2.      ],\n       [54.      , 40.739155, 29.      , 48.      , 42.      ],\n       [73.946655,  2.      ,  0.      , 12.      ,  0.      ],\n       [67.      , 52.      , 64.      , 28.033165, 61.      ]],\n      dtype=float32)"
                     },
-                    "execution_count": 8,
+                    "execution_count": 4,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "faiss_imputer = FaissImputer(n_neighbors=5, strategy=\"mean\")\n",
+                "faiss_imputer = FaissImputer(n_neighbors=5, strategy=\"weighted\")\n",
                 "\n",
                 "df_imputed_faiss = faiss_imputer.fit_transform(df_missing)\n",
                 "df_imputed_faiss"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 9,
+            "execution_count": 5,
             "metadata": {
                 "ExecuteTime": {
-                    "end_time": "2024-04-24T10:58:12.017341110Z",
-                    "start_time": "2024-04-24T10:58:11.979862921Z"
+                    "end_time": "2024-04-25T13:28:24.318561902Z",
+                    "start_time": "2024-04-25T13:28:24.313935463Z"
                 },
                 "collapsed": false
             },
             "outputs": [],
             "source": [
                 "imputer = KNNImputer(n_neighbors=5)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 10,
+            "execution_count": 6,
             "metadata": {
                 "ExecuteTime": {
-                    "end_time": "2024-04-24T10:58:14.814817872Z",
-                    "start_time": "2024-04-24T10:58:14.802774507Z"
+                    "end_time": "2024-04-25T13:28:24.407326999Z",
+                    "start_time": "2024-04-25T13:28:24.319140339Z"
                 },
                 "collapsed": false
             },
             "outputs": [
                 {
                     "data": {
                         "text/plain": "array([[85. , 63. , 51. , 26. , 30. ],\n       [68.4,  7. , 38.8, 17. , 27. ],\n       [64. , 50. , 50. , 60. , 41.4],\n       [72. , 63. , 54. , 55. , 48.8],\n       [68.4, 81. , 67. ,  0. , 39. ],\n       [85. , 55. ,  3. , 76. , 72. ],\n       [84. , 17. ,  8. , 86. ,  2. ],\n       [54. , 48. , 29. , 48. , 42. ],\n       [71.8,  2. ,  0. , 12. ,  0. ],\n       [67. , 52. , 64. , 37.8, 61. ]])"
                     },
-                    "execution_count": 10,
+                    "execution_count": 6,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "df_imputed_scikit = imputer.fit_transform(df_missing)\n",
                 "df_imputed_scikit"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 12,
+            "execution_count": 7,
             "metadata": {
                 "ExecuteTime": {
-                    "end_time": "2024-04-24T10:59:49.312441609Z",
-                    "start_time": "2024-04-24T10:59:49.264281741Z"
+                    "end_time": "2024-04-25T13:28:24.511852649Z",
+                    "start_time": "2024-04-25T13:28:24.342122845Z"
                 },
                 "collapsed": false
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Mean Squared Error: 4.38948107984583\n",
-                        "Mean Absolute Error: 0.7748571701049802\n"
+                        "Mean Absolute Error between scikit-learn and faiss: 1.8301985855102538\n"
                     ]
                 }
             ],
             "source": [
                 "mse = np.mean((df_imputed_scikit - df_imputed_faiss) ** 2)\n",
                 "mae = np.mean(np.abs(df_imputed_scikit - df_imputed_faiss))\n",
                 "\n",
-                "print(f\"Mean Squared Error: {mse}\")\n",
-                "print(f\"Mean Absolute Error: {mae}\")"
+                "print(f\"Mean Absolute Error between scikit-learn and faiss: {mae}\")"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 8,
+            "metadata": {
+                "ExecuteTime": {
+                    "end_time": "2024-04-25T13:28:24.512921328Z",
+                    "start_time": "2024-04-25T13:28:24.383682270Z"
+                },
+                "collapsed": false
+            },
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "Mean Absolute Error between original DataFrame and faiss: 9.6090913772583\n"
+                    ]
+                }
+            ],
+            "source": [
+                "mse = np.mean((df - df_imputed_faiss) ** 2)\n",
+                "mae = np.mean(np.abs(df - df_imputed_faiss))\n",
+                "\n",
+                "print(f\"Mean Absolute Error between original DataFrame and faiss: {mae}\")"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 9,
+            "metadata": {
+                "ExecuteTime": {
+                    "end_time": "2024-04-25T13:28:24.513834024Z",
+                    "start_time": "2024-04-25T13:28:24.383846470Z"
+                },
+                "collapsed": false
+            },
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "Mean Absolute Error between original DataFrame and scikit-learn: 8.46\n"
+                    ]
+                }
+            ],
+            "source": [
+                "mse = np.mean((df - df_imputed_scikit) ** 2)\n",
+                "mae = np.mean(np.abs(df - df_imputed_scikit))\n",
+                "\n",
+                "print(f\"Mean Absolute Error between original DataFrame and scikit-learn: {mae}\")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "collapsed": false
             },
             "source": [
                 "## Speed comparison"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 7,
+            "execution_count": 10,
             "metadata": {
                 "ExecuteTime": {
-                    "end_time": "2024-04-24T10:56:18.352006752Z",
-                    "start_time": "2024-04-24T10:54:54.490986452Z"
+                    "end_time": "2024-04-25T13:29:06.633118482Z",
+                    "start_time": "2024-04-25T13:28:24.388024377Z"
                 },
                 "collapsed": false
             },
             "outputs": [
                 {
                     "data": {
-                        "image/png": "iVBORw0KGgoAAAANSUhEUgAAAjMAAAGxCAYAAACXwjeMAAAAOXRFWHRTb2Z0d2FyZQBNYXRwbG90bGliIHZlcnNpb24zLjguNCwgaHR0cHM6Ly9tYXRwbG90bGliLm9yZy8fJSN1AAAACXBIWXMAAA9hAAAPYQGoP6dpAAA/c0lEQVR4nO3deVyU5f7/8feIOiwCrmzGUVQw17QoEyuwgnIrsyyX3C08WkpkKsdMLIXUI5FaelpEWqxOWZ5OHU3ccK1Qs8U86ikXTAkzBBcEhfv3Rz/n2wgog9Bw0+v5eNyPh3Pd19z3Z2aYmbfXfd33WAzDMAQAAGBStZxdAAAAwNUgzAAAAFMjzAAAAFMjzAAAAFMjzAAAAFMjzAAAAFMjzAAAAFMjzAAAAFMjzAAAAFMjzKDGW7p0qSwWi7Zv3+7sUi7r6NGjio+P165duyq8je+//17x8fE6ePBgiXXDhw9X8+bNK7ztihg+fLgsFssVl+HDh2vDhg2yWCzasGHDH1rjlRQXF+vNN9/UnXfeqcaNG6tOnTry8fFR79699e9//1vFxcXOLrHKWSwWxcfHO7sMoEy1nV0AgN8cPXpUM2bMUPPmzdWpU6cKbeP777/XjBkzFBERUSK4TJs2TRMmTLj6Qh0wbdo0jRkzxnZ7586dGjdunBISEtS9e3dbe5MmTdSkSRNt27ZNbdu2/UNrvJxz586pb9++Wr16tQYMGKBFixbJz89Px48f16pVq9S/f3+99957uvfee51dapXatm2brrnmGmeXAZSJMAP8SbRs2dIp+/z9fs+dOydJCg4O1s0331yif2ltzhQbG6vPPvtMqampGjp0qN26fv366amnnlJ+fr6TqqtahmHo3LlzcnNzq3avC3ApDjPhT2n48OGqV6+e/vvf/+quu+6Sh4eH/P399fzzz0uSPv/8c91yyy3y8PBQSEiIUlNT7e5/8dBVWlqaRowYoYYNG8rDw0N9+vTRjz/+aNe3efPmGj58eIkaIiIiFBERIUnasGGDbrzxRknSiBEjbIdfLg7tb9++XQMGDFDz5s3l5uam5s2ba+DAgTp06JBdTf3795ckde/e3baNpUuX2h7zpaM1586dU1xcnIKCglS3bl01bdpU48aN08mTJ0s8ht69e2vVqlW6/vrr5ebmpmuvvVZLliwp71N+RaUdZrra10mSsrKyFB0drWuuuUZ169ZVUFCQZsyYoQsXLly2nqysLL322mu66667SgSZi4KDg9WxY0fb7cOHD+vhhx+Wj4+PrFar2rRpo3nz5tkdijp48KAsFovmzp2r2bNn217TiIgI7du3T+fPn9eUKVMUEBAgb29v3XfffcrOzrbb78XX46OPPlLHjh3l6uqqFi1aaP78+Xb9zp07pyeffFKdOnWSt7e3GjZsqK5du+pf//pXicdisVj02GOPafHixWrTpo2sVqvt+bz0MNPZs2c1ceJEBQUFydXVVQ0bNlRoaKjeeecdu21+/PHH6tq1q9zd3eXp6anIyEht27bNrk98fLwsFot2796tgQMHytvbW76+vho5cqRyc3Mv8woB/4eRGfxpnT9/Xv369dOYMWP01FNPadmyZYqLi1NeXp6WL1+uyZMn65prrtGCBQs0fPhwtW/fXjfccIPdNkaNGqXIyEgtW7ZMmZmZevrppxUREaFvvvlG9evXL3ct119/vVJSUjRixAg9/fTT6tWrlyTZhvYPHjyo1q1ba8CAAWrYsKGOHTumRYsW6cYbb9T333+vxo0bq1evXkpISNDf/vY3vfTSS7r++usllT0iYxiG+vbtq7Vr1youLk633nqrvvnmG02fPl3btm3Ttm3bZLVabf2//vprPfnkk5oyZYp8fX312muvadSoUWrVqpVuu+02R556h1zN65SVlaWbbrpJtWrV0jPPPKOWLVtq27Ztmjlzpg4ePKiUlJQy97t+/XqdP39effv2LVedx48fV1hYmAoLC/Xcc8+pefPm+uSTTzRx4kT98MMPevnll+36v/TSS+rYsaNeeuklnTx5Uk8++aT69OmjLl26qE6dOlqyZIkOHTqkiRMnavTo0fr444/t7r9r1y7FxMQoPj5efn5+evvttzVhwgQVFhZq4sSJkqSCggL9+uuvmjhxopo2barCwkKtWbNG/fr1U0pKSomQtmLFCm3atEnPPPOM/Pz85OPjU+pjjY2N1ZtvvqmZM2eqc+fOOnPmjL777judOHHC1mfZsmUaPHiwoqKi9M4776igoEBz5sxRRESE1q5dq1tuucVum/fff78eeughjRo1St9++63i4uIkqVIDM2owA6jhUlJSDElGRkaGrW3YsGGGJGP58uW2tvPnzxtNmjQxJBk7d+60tZ84ccJwcXExYmNjS2zzvvvus9vXli1b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NEn5+fkaO3ascnJy1KVLF61evVqenp5OrBwAAFQXTr3OzB+B68wAzlOzP10AVCXTXGcGAADgahFmAACAqRFmAACAqRFmAACAqRFmAACAqRFmAACAqRFmAACAqRFmAACAqRFmAACAqRFmAACAqRFmAACAqRFmAACAqRFmAACAqRFmAACAqRFmAACAqRFmAACAqRFmAACAqRFmAACAqRFmAACAqRFmAACAqRFmAACAqRFmAACAqRFmAACAqRFmAACAqRFmAACAqRFmAACAqRFmAACAqRFmAACAqRFmAACAqV11mMnLy9OKFSu0Z8+eyqgHAADAIQ6HmQcffFALFy6UJOXn5ys0NFQPPvigOnbsqOXLl1d6gQAAAJfjcJjZuHGjbr31VknSRx99JMMwdPLkSc2fP18zZ86s9AIBAAAux+Ewk5ubq4YNG0qSVq1apfvvv1/u7u7q1auX9u/fX+kFAgAAXI7DYSYwMFDbtm3TmTNntGrVKkVFRUmScnJy5OrqWukFAgAAXE5tR+8QExOjwYMHq169emrWrJkiIiIk/Xb4qUOHDpVdHwAAwGU5PDIzduxYbdu2TUuWLNHmzZtVq9Zvm2jRooXDc2bi4+NlsVjsFj8/P9t6wzAUHx+vgIAAubm5KSIiQrt373a0ZAAAUIM5PDIjSaGhoQoNDbVr69WrV4UKaNeundasWWO77eLiYvv3nDlzlJSUpKVLlyokJEQzZ85UZGSk9u7dK09PzwrtDwAA1CzlCjOxsbHl3mBSUpJjBdSubTcac5FhGEpOTtbUqVPVr18/SVJqaqp8fX21bNkyRUdHO7QfAABQM5UrzHz11Vd2t3fs2KGioiK1bt1akrRv3z65uLjohhtucLiA/fv3KyAgQFarVV26dFFCQoJatGihAwcOKCsryzbBWJKsVqvCw8O1devWMsNMQUGBCgoKbLfz8vIcrgkAAJhHucLM+vXrbf9OSkqSp6enUlNT1aBBA0m/nck0YsQI2/VnyqtLly564403FBISop9//lkzZ85UWFiYdu/eraysLEmSr6+v3X18fX116NChMreZmJioGTNmOFQHAAAwL4thGIYjd2jatKlWr16tdu3a2bV/9913ioqK0tGjRytczJkzZ9SyZUtNmjRJN998s7p166ajR4/K39/f1ueRRx5RZmamVq1aVeo2ShuZCQwMVG5urry8vCpcW1kslkrfJFBjOPbpAgD/Jy8vT97e3uX6/nb4bKa8vDz9/PPPJdqzs7N16tQpRzdnx8PDQx06dND+/ftt82gujtD8fj+Xjtb8ntVqlZeXl90CAABqLofDzH333acRI0bogw8+0JEjR3TkyBF98MEHGjVqlG2ibkUVFBRoz5498vf3V1BQkPz8/JSWlmZbX1hYqPT0dIWFhV3VfgAAQM3h8KnZixcv1sSJE/Xwww/r/Pnzv22kdm2NGjVKc+fOdWhbEydOVJ8+ffSXv/xF2dnZmjlzpvLy8jRs2DBZLBbFxMQoISFBwcHBCg4OVkJCgtzd3TVo0CBHywYAADWUw2HG3d1dL7/8subOnasffvhBhmGoVatW8vDwcHjnR44c0cCBA/XLL7+oSZMmuvnmm/X555+rWbNmkqRJkyYpPz9fY8eOVU5Ojrp06aLVq1dzjRkAAGDj8ARgs3FkAlFFMAEYKFvN/nQBUJUc+f52eGTmzJkzev7557V27VplZ2eruLjYbv2PP/7o6CYBAAAqzOEwM3r0aKWnp2vIkCHy9/eXhaEJAADgRA6HmZUrV+rTTz9Vt27dqqIeAAAAhzh8anaDBg3UsGHDqqgFAADAYQ6Hmeeee07PPPOMzp49WxX1AAAAOMThw0zz5s3TDz/8IF9fXzVv3lx16tSxW79z585KKw4AAOBKHA4zffv2rYIyAAAAKobrzFwlTuYCylazP10AVKUqvc7MRTt27NCePXtksVjUtm1bde7cuaKbAgAAqDCHw0x2drYGDBigDRs2qH79+jIMQ7m5uerevbveffddNWnSpCrqBAAAKJXDZzM9/vjjysvL0+7du/Xrr78qJydH3333nfLy8jR+/PiqqBEAAKBMDs+Z8fb21po1a3TjjTfatX/55ZeKiorSyZMnK7O+q8acGcB5mDMDoKIc+f52eGSmuLi4xOnYklSnTp0Sv9MEAABQ1RwOM7fffrsmTJigo0eP2tp++uknPfHEE7rjjjsqtTgAAIArcTjMLFy4UKdOnVLz5s3VsmVLtWrVSkFBQTp16pQWLFhQFTUCAACUyeGzmQIDA7Vz506lpaXpv//9rwzDUNu2bXXnnXdWRX0AAACXxUXzrhITgIGy1exPFwBVqUonAI8fP17z588v0b5w4ULFxMQ4ujkAAICr4nCYWb58ubp161aiPSwsTB988EGlFAUAAFBeDoeZEydOyNvbu0S7l5eXfvnll0opCgAAoLwcDjOtWrXSqlWrSrSvXLlSLVq0qJSiAAAAysvhs5liY2P12GOP6fjx47r99tslSWvXrtW8efOUnJxc2fUBAABclsNhZuTIkSooKNCsWbP03HPPSZKaN2+uRYsWaejQoZVeIAAAwOVc1anZx48fl5ubm+rVq1eZNVUqTs0GnIdTswFUVJWemi1JFy5c0Jo1a/Thhx/qYhY6evSoTp8+XZHNAQAAVJjDh5kOHTqku+++W4cPH1ZBQYEiIyPl6empOXPm6Ny5c1q8eHFV1AkAAFAqh0dmJkyYoNDQUOXk5MjNzc3Wft9992nt2rWVWhwAAMCVODwys3nzZm3ZskV169a1a2/WrJl++umnSisMAACgPBwemSkuLlZRUVGJ9iNHjsjT07NSigIAACgvh8NMZGSk3fVkLBaLTp8+renTp6tnz56VWRsAAMAVOXxq9tGjR9W9e3e5uLho//79Cg0N1f79+9W4cWNt3LhRPj4+VVVrhXBqNuA8nJoNoKIc+f52eM5MQECAdu3apXfffVc7duxQcXGxRo0apcGDB9tNCAYAAPgjXNVF88yAkRnAeWr2pwuAqlSlF81LTU3Vp59+ars9adIk1a9fX2FhYTp06JDj1QIAAFwFh8NMQkKC7XDStm3btHDhQs2ZM0eNGzfWE088UekFAgAAXI7DYSYzM1OtWrWSJK1YsUIPPPCAHn30USUmJmrTpk0VLiQxMVEWi0UxMTG2NsMwFB8fr4CAALm5uSkiIkK7d++u8D4AAEDN43CYqVevnk6cOCFJWr16te68805Jkqurq/Lz8ytUREZGhl555RV17NjRrn3OnDlKSkrSwoULlZGRIT8/P0VGRurUqVMV2g8AAKh5KnSdmdGjR2v06NHat2+fevXqJUnavXu3mjdv7nABp0+f1uDBg/Xqq6+qQYMGtnbDMJScnKypU6eqX79+at++vVJTU3X27FktW7bM4f0AAICayeEw89JLL6lr1646fvy4li9frkaNGkmSduzYoYEDBzpcwLhx49SrVy/bCM9FBw4cUFZWlqKiomxtVqtV4eHh2rp1a5nbKygoUF5ent0CAABqLoevM1O/fn0tXLiwRPuMGTMc3vm7776rnTt3KiMjo8S6rKwsSZKvr69du6+v72XPmkpMTKxQLQAAwJwcHpmpLJmZmZowYYLeeustubq6ltnPcsmFXAzDKNH2e3FxccrNzbUtmZmZlVYzAACofhwemaksO3bsUHZ2tm644QZbW1FRkTZu3KiFCxdq7969kn4bofH397f1yc7OLjFa83tWq1VWq7XqCgcAANWK00Zm7rjjDn377bfatWuXbQkNDdXgwYO1a9cutWjRQn5+fkpLS7Pdp7CwUOnp6QoLC3NW2QAAoJpx2siMp6en2rdvb9fm4eGhRo0a2dpjYmKUkJCg4OBgBQcHKyEhQe7u7ho0aJAzSgYAANWQ08JMeUyaNEn5+fkaO3ascnJy1KVLF61evVqenp7OLg0AAFQTDv/Q5M8//6yJEydq7dq1ys7O1qV3LyoqqtQCrxY/NAk4Dz80CaCiHPn+dnhkZvjw4Tp8+LCmTZsmf3//y55ZBAAAUNUcDjObN2/Wpk2b1KlTpyooBwAAwDEOn80UGBhY4tASAACAszgcZpKTkzVlyhQdPHiwCsoBAABwjMOHmR566CGdPXtWLVu2lLu7u+rUqWO3/tdff6204gAAAK7E4TCTnJxcBWUAAABUjMNhZtiwYVVRBwAAQIWUK8zk5eXZzvHOy8u7bN+quJYLAABAWcoVZho0aKBjx47Jx8dH9evXL/XaMhd/zbq6XTQPAADUbOUKM+vWrVPDhg0lSevXr6/SggAAABzh8M8ZmA0/ZwA4T83+dAFQlRz5/nb4OjMAAADVCWEGAACYGmEGAACYGmEGAACYWoXCzIULF7RmzRr94x//0KlTpyRJR48e1enTpyu1OAAAgCtx+ArAhw4d0t13363Dhw+roKBAkZGR8vT01Jw5c3Tu3DktXry4KuoEAAAolcMjMxMmTFBoaKhycnLk5uZma7/vvvu0du3aSi0OAADgShwemdm8ebO2bNmiunXr2rU3a9ZMP/30U6UVBgAAUB4Oj8wUFxeX+pMFR44ckaenZ6UUBQAAUF4Oh5nIyEglJyfbblssFp0+fVrTp09Xz549K7M2AACAK3L45wyOHj2q7t27y8XFRfv371doaKj279+vxo0ba+PGjfLx8amqWiuEnzMAnIefMwBQUY58fzs8ZyYgIEC7du3SO++8o507d6q4uFijRo3S4MGD7SYEAwAA/BH4ocmrxMgMULaa/ekCoCpV6ciMJP3000/asmWLsrOzVVxcbLdu/PjxFdkkAABAhTgcZlJSUjRmzBjVrVtXjRo1kuV3QxMWi4UwAwAA/lAOH2YKDAzUmDFjFBcXp1q1qv9PO3GYCXAeDjMBqChHvr8dTiNnz57VgAEDTBFkAABAzedwIhk1apTef//9qqgFAADAYQ4fZioqKlLv3r2Vn5+vDh06qE6dOnbrk5KSKrXAq8VhJsB5OMwEoKKq9GymhIQEffbZZ2rdurUklZgADAAA8EdyOMwkJSVpyZIlGj58eBWUAwAA4BiH58xYrVZ169atKmoBAABwmMNhZsKECVqwYEFV1AIAAOAwhw8zffnll1q3bp0++eQTtWvXrsQE4A8//LDSigMAALgSh0dm6tevr379+ik8PFyNGzeWt7e33eKIRYsWqWPHjvLy8pKXl5e6du2qlStX2tYbhqH4+HgFBATIzc1NERER2r17t6MlAwCAGsypPzT573//Wy4uLmrVqpUkKTU1VXPnztVXX32ldu3aafbs2Zo1a5aWLl2qkJAQzZw5Uxs3btTevXvl6elZrn1wajbgPJyaDaCiHPn+rna/mt2wYUPNnTtXI0eOVEBAgGJiYjR58mRJUkFBgXx9fTV79mxFR0eXa3uEGcB5qtenCwAzqfTrzFx//fVau3atGjRooM6dO1/2ejI7d+50rNr/r6ioSO+//77OnDmjrl276sCBA8rKylJUVJStj9VqVXh4uLZu3VpmmCkoKFBBQYHtdl5eXoXqAQAA5lCuMHPvvffKarVKkvr27VupBXz77bfq2rWrzp07p3r16umjjz5S27ZttXXrVkmSr6+vXX9fX18dOnSozO0lJiZqxowZlVojAACovsp9mGnkyJF68cUXyz1XpbwKCwt1+PBhnTx5UsuXL9drr72m9PR0nTx5Ut26ddPRo0fl7+9v6//II48oMzNTq1atKnV7pY3MBAYGcpgJcAIOMwGoqCr51ezU1FTl5+dfdXGXqlu3rlq1aqXQ0FAlJibquuuu04svvig/Pz9JUlZWll3/7OzsEqM1v2e1Wm1nR11cAABAzVXuMPNHzRM2DEMFBQUKCgqSn5+f0tLSbOsKCwuVnp6usLCwP6QWAABQ/Tl00bzK/iHJv/3tb+rRo4cCAwN16tQpvfvuu9qwYYNWrVoli8WimJgYJSQkKDg4WMHBwUpISJC7u7sGDRpUqXUAAADzcijMhISEXDHQ/Prrr+Xe3s8//6whQ4bo2LFj8vb2VseOHbVq1SpFRkZKkiZNmqT8/HyNHTtWOTk56tKli1avXl3p83YAAIB5lXsCcK1atZScnHzFq/wOGzasUgqrLFxnBnAeJgADqKhKv87MRQMGDJCPj89VFQcAAFCZyj0BuLLnywAAAFSGanc2EwAAgCPKfZipuLi4KusAAACokHKPzAAAAFRHhBkAAGBqhBkAAGBqhBkAAGBqhBkAAGBqhBkAAGBqhBkAAGBqhBkAAGBqhBkAAGBqhBkAAGBqhBkAAGBqhBkAAGBqhBkAAGBqhBkAAGBqhBkAAGBqhBkAAGBqhBkAAGBqhBkAAGBqhBkAAGBqhBkAAGBqhBkAAGBqhBkAAGBqhBkAAGBqhBkAAGBqhBkAAGBqhBkAAGBqhBkAAGBqhBkAAGBqhBkAAGBqhBkAAGBqhBkAAGBqTg0ziYmJuvHGG+Xp6SkfHx/17dtXe/futetjGIbi4+MVEBAgNzc3RUREaPfu3U6qGAAAVDdODTPp6ekaN26cPv/8c6WlpenChQuKiorSmTNnbH3mzJmjpKQkLVy4UBkZGfLz81NkZKROnTrlxMoBAEB1YTEMw3B2ERcdP35cPj4+Sk9P12233SbDMBQQEKCYmBhNnjxZklRQUCBfX1/Nnj1b0dHRJbZRUFCggoIC2+28vDwFBgYqNzdXXl5elV6zxVLpmwRqjOrz6QLAbPLy8uTt7V2u7+9qNWcmNzdXktSwYUNJ0oEDB5SVlaWoqChbH6vVqvDwcG3durXUbSQmJsrb29u2BAYGVn3hAADAaapNmDEMQ7GxsbrlllvUvn17SVJWVpYkydfX166vr6+vbd2l4uLilJuba1syMzOrtnAAAOBUtZ1dwEWPPfaYvvnmG23evLnEOsslx3IMwyjRdpHVapXVaq2SGgEAQPVTLUZmHn/8cX388cdav369rrnmGlu7n5+fJJUYhcnOzi4xWgMAAP6cnBpmDMPQY489pg8//FDr1q1TUFCQ3fqgoCD5+fkpLS3N1lZYWKj09HSFhYX90eUCAIBqyKmHmcaNG6dly5bpX//6lzw9PW0jMN7e3nJzc5PFYlFMTIwSEhIUHBys4OBgJSQkyN3dXYMGDXJm6QAAoJpwaphZtGiRJCkiIsKuPSUlRcOHD5ckTZo0Sfn5+Ro7dqxycnLUpUsXrV69Wp6enn9wtQAAoDqqVteZqQqOnKdeEVxnBihbzf50AVCVTHudGQAAAEcRZgAAgKkRZgAAgKkRZgAAgKkRZgAAgKkRZgAAgKkRZgAAgKkRZgAAgKkRZgAAgKkRZgAAgKkRZgAAgKkRZgAAgKkRZgAAgKkRZgAAgKkRZgAAgKkRZgAAgKkRZgAAgKkRZgAAgKkRZgAAgKkRZgAAgKkRZgAAgKkRZgAAgKkRZgAAgKkRZgAAgKkRZgAAgKkRZgAAgKkRZgAAgKkRZgAAgKkRZgAAgKkRZgAAgKkRZgAAgKkRZgAAgKkRZgAAgKkRZgAAgKkRZgAAgKk5Ncxs3LhRffr0UUBAgCwWi1asWGG33jAMxcfHKyAgQG5uboqIiNDu3budUywAAKiWnBpmzpw5o+uuu04LFy4sdf2cOXOUlJSkhQsXKiMjQ35+foqMjNSpU6f+4EoBAEB1VduZO+/Ro4d69OhR6jrDMJScnKypU6eqX79+kqTU1FT5+vpq2bJlio6OLvV+BQUFKigosN3Oy8ur/MIBAEC1UW3nzBw4cEBZWVmKioqytVmtVoWHh2vr1q1l3i8xMVHe3t62JTAw8I8oFwAAOEm1DTNZWVmSJF9fX7t2X19f27rSxMXFKTc317ZkZmZWaZ0AAMC5nHqYqTwsFovdbcMwSrT9ntVqldVqreqyAABANVFtR2b8/PwkqcQoTHZ2donRGgAA8OdVbcNMUFCQ/Pz8lJaWZmsrLCxUenq6wsLCnFgZAACoTpx6mOn06dP63//+Z7t94MAB7dq1Sw0bNtRf/vIXxcTEKCEhQcHBwQoODlZCQoLc3d01aNAgJ1YNAACqE6eGme3bt6t79+6227GxsZKkYcOGaenSpZo0aZLy8/M1duxY5eTkqEuXLlq9erU8PT2dVTIAAKhmLIZhGM4uoirl5eXJ29tbubm58vLyqvTtX2YuMvCnV7M/XQBUJUe+v6vtnBkAAIDyIMwAAABTI8wAAABTI8wAAABTI8wAAABTI8wAAABTI8wAAABTI8wAAABTI8wAAABTI8wAAABTI8wAAABTI8wAAABTI8wAAABTI8wAAABTq+3sAgCgurPMsDi7BKDaMqYbzi6BkRkAAGBuhBkAAGBqhBkAAGBqhBkAAGBqhBkAAGBqhBkAAGBqhBkAAGBqhBkAAGBqhBkAAGBqhBkAAGBqhBkAAGBqhBkAAGBqhBkAAGBqhBkAAGBqhBkAAGBqhBkAAGBqhBkAAGBqhBkAAGBqhBkAAGBqpggzL7/8soKCguTq6qobbrhBmzZtcnZJAACgmqj2Yea9995TTEyMpk6dqq+++kq33nqrevToocOHDzu7NAAAUA1U+zCTlJSkUaNGafTo0WrTpo2Sk5MVGBioRYsWObs0AABQDdR2dgGXU1hYqB07dmjKlCl27VFRUdq6dWup9ykoKFBBQYHtdm5uriQpLy+v6goFUKoa87Y75+wCgOqrqr5fL27XMIwr9q3WYeaXX35RUVGRfH197dp9fX2VlZVV6n0SExM1Y8aMEu2BgYFVUiOAsnl7O7sCAFXN+/mqfaOfOnVK3lf4MKnWYeYii8Vid9swjBJtF8XFxSk2NtZ2u7i4WL/++qsaNWpU5n1QM+Tl5SkwMFCZmZny8vJydjkAqgDv8z8PwzB06tQpBQQEXLFvtQ4zjRs3louLS4lRmOzs7BKjNRdZrVZZrVa7tvr161dViaiGvLy8+JADajje538OVxqRuahaTwCuW7eubrjhBqWlpdm1p6WlKSwszElVAQCA6qRaj8xIUmxsrIYMGaLQ0FB17dpVr7zyig4fPqwxY8Y4uzQAAFANVPsw89BDD+nEiRN69tlndezYMbVv317/+c9/1KxZM2eXhmrGarVq+vTpJQ4zAqg5eJ+jNBajPOc8AQAAVFPVes4MAADAlRBmAACAqRFmAACAqRFmAACAqRFmagCLxaIVK1ZIkg4ePCiLxaJdu3aVq78jIiIiFBMTU6EaAdRMS5cu5cKkcDrCTA1w7Ngx9ejRo0L9yxN+zOLSkHb+/HkNGDBA/v7++uabbyRJzZs3l8Vi0eeff25335iYGEVERNhux8fHy2KxlLie0a5du2SxWHTw4EFJ1ev5q061wHyGDx8ui8VSYvnf//532fs99NBD2rdv31Xvvzr9/VanWlA+hJkawM/Pz6FrLjja/49UWFhYKds5e/as7rnnHmVkZGjz5s3q2LGjbZ2rq6smT558xW24urrq9ddfr5QParM5f/68s0uAE9x99906duyY3RIUFHTZ+7i5ucnHx+cPqtB8eC/9MQgz1cQHH3ygDh06yM3NTY0aNdKdd96pM2fO2NYvWbJE7dq1k9Vqlb+/vx577DHbussdNiouLtYjjzyikJAQHTp0qET/ix9UnTt3lsVisRuduJLCwkJNmjRJTZs2lYeHh7p06aINGzbY1p84cUIDBw7UNddcI3d3d3Xo0EHvvPOO3TYiIiL02GOPKTY2Vo0bN1ZkZKQ2bNggi8WitWvXKjQ0VO7u7goLC9PevXvLVdfJkycVFRWln376SZs3b1bLli3t1kdHR+vzzz/Xf/7zn8tup3Xr1urevbuefvrp8j0hkq32zz77TJ07d5abm5tuv/12ZWdna+XKlWrTpo28vLw0cOBAnT17tsTz8Nhjj6l+/fpq1KiRnn76af3+MlClvc7169fX0qVLJV3+tUxJSVGbNm3k6uqqa6+9Vi+//LJt3cX/hf7zn/9URESEXF1d9dZbb5X7MaPmsFqt8vPzs1tefPFFdejQQR4eHgoMDNTYsWN1+vRp230uPcz09ddfq3v37vL09JSXl5duuOEGbd++XZJ06NAh9enTRw0aNJCHh4fatWtX5vuQ9xIcQZipBo4dO6aBAwdq5MiR2rNnjzZs2KB+/frZ3nyLFi3SuHHj9Oijj+rbb7/Vxx9/rFatWl1xu4WFhXrwwQe1fft2bd68udSrJn/55ZeSpDVr1ujYsWP68MMPy133iBEjtGXLFr377rv65ptv1L9/f919993av3+/JOncuXO64YYb9Mknn+i7777To48+qiFDhuiLL76w205qaqpq166tLVu26B//+IetferUqZo3b562b9+u2rVra+TIkVesKSsrS+Hh4SouLlZ6err8/f1L9GnevLnGjBmjuLg4FRcXX3Z7zz//vJYvX66MjIzyPCU28fHxWrhwobZu3arMzEw9+OCDSk5O1rJly/Tpp58qLS1NCxYssLvPxefhiy++0Pz58/XCCy/otddeK/c+y3otX331VU2dOlWzZs3Snj17lJCQoGnTpik1NdXu/pMnT9b48eO1Z88e3XXXXQ49XtRctWrV0vz58/Xdd98pNTVV69at06RJk8rsP3jwYF1zzTXKyMjQjh07NGXKFNWpU0eSNG7cOBUUFGjjxo369ttvNXv2bNWrV++y++e9hHIx4HQ7duwwJBkHDx4sdX1AQIAxderUMu8vyfjoo48MwzCMAwcOGJKMTZs2GXfeeafRrVs34+TJk1fs/9VXX12xzvDwcGPChAmGYRjG//73P8NisRg//fSTXZ877rjDiIuLK3MbPXv2NJ588km7bXbq1Mmuz/r16w1Jxpo1a2xtn376qSHJyM/PL3Pbkoy6desa1157rXHmzJlS+zRr1sx44YUXjOzsbMPT09N44403DMMwjAkTJhjh4eG2ftOnTzeuu+46wzAMY8CAAcbtt99uGIZhfPXVV4Yk48CBA4ZhlHz+Sqs9MTHRkGT88MMPtrbo6Gjjrrvusnse2rRpYxQXF9vaJk+ebLRp08bu8V183S7y9vY2UlJSSq3losDAQGPZsmV2bc8995zRtWtXu/slJyeX+pzhz2HYsGGGi4uL4eHhYVseeOCBEv3++c9/Go0aNbLdTklJMby9vW23PT09jaVLl5a6jw4dOhjx8fGlruO9hKvByEw1cN111+mOO+5Qhw4d1L9/f7366qvKycmRJGVnZ+vo0aO64447HNrmwIEDdfr0aa1evbrcP6F+0aZNm1SvXj3b8vbbb5fos3PnThmGoZCQELu+6enp+uGHHyRJRUVFmjVrljp27KhGjRqpXr16Wr16tQ4fPmy3rdDQ0FLr+P08l4sjLNnZ2ZetvU+fPtq3b5/dCE9pmjRpookTJ+qZZ5654jydmTNnatOmTVq9evVl+/3e72v39fWVu7u7WrRoYdd26WO5+eabZbFYbLe7du2q/fv3q6ioqNz7vdTx48eVmZmpUaNG2b1OM2fOtL1OF5X1OuDPo3v37tq1a5dtmT9/vtavX6/IyEg1bdpUnp6eGjp0qE6cOGF3GPz3YmNjNXr0aN155516/vnn7f7Oxo8fr5kzZ6pbt26aPn26bWL+5fBeQnkQZqoBFxcXpaWlaeXKlWrbtq0WLFig1q1b68CBA3Jzc6vQNnv27KlvvvmmxFk75REaGmr3gXbPPfeU6FNcXCwXFxft2LHDru+ePXv04osvSpLmzZunF154QZMmTdK6deu0a9cu3XXXXSXCg4eHR6l1XByalmT7YLrSYaGHH35YKSkpeuqpp/T3v//9sn1jY2OVn59vd8y7NC1bttQjjzyiKVOm2B13v5xLa//97YttV3osl7JYLCX2f6XJhRf38eqrr9q9Tt99912Jv42yXgf8eXh4eKhVq1a2pbCwUD179lT79u21fPly7dixQy+99JKksv/24uPjtXv3bvXq1Uvr1q1T27Zt9dFHH0mSRo8erR9//FFDhgzRt99+q9DQ0BKHiC7FewnlUe1/NfvPwmKxqFu3burWrZueeeYZNWvWTB999JFiY2PVvHlzrV27Vt27dy/39v7617+qffv2uueee/Tpp58qPDy81H5169aVJLv/sbi5uV1xTk7nzp1VVFSk7Oxs3XrrraX22bRpk+699149/PDDkn77MNi/f7/atGlT7sdREUOHDpWLi4uGDRum4uLiMo/v16tXT9OmTVN8fLz69Olz2W0+88wzatmypd59992qKFmSSnwgfv755woODpaLi4uk30aTjh07Zlu/f/9+u4mPpb2Wvr6+atq0qX788UcNHjy4ympHzbR9+3ZduHBB8+bNU61av/3f95///OcV7xcSEqKQkBA98cQTGjhwoFJSUnTfffdJkgIDAzVmzBjbvLVXX31Vjz/+eKXWzXvpz4cwUw188cUXWrt2raKiouTj46MvvvhCx48ft33px8fHa8yYMfLx8VGPHj106tQpbdmy5YofAI8//riKiorUu3dvrVy5UrfcckuJPj4+PnJzc9OqVat0zTXXyNXVtVyHpUJCQjR48GANHTpU8+bNU+fOnfXLL79o3bp16tChg3r27KlWrVpp+fLl2rp1qxo0aKCkpCRlZWVVeZiRfpuEWKtWLQ0ZMkTFxcWaMmVKqf0effRRvfDCC3rnnXfUpUuXMrfn6+ur2NhYzZ07t6pKVmZmpmJjYxUdHa2dO3dqwYIFmjdvnm397bffroULF+rmm29WcXGxJk+ebPe/1LJey/j4eI0fP15eXl7q0aOHCgoKtH37duXk5Cg2NrbKHg/Mr2XLlrpw4YIWLFigPn36aMuWLVq8eHGZ/fPz8/XUU0/pgQceUFBQkI4cOaKMjAzdf//9kn67nlOPHj0UEhKinJwcrVu3rko+D3gv/flwmKka8PLy0saNG9WzZ0+FhITo6aef1rx582wXths2bJiSk5P18ssvq127durdu7ftjKEriYmJ0YwZM9SzZ09t3bq1xPratWtr/vz5+sc//qGAgADde++95a47JSVFQ4cO1ZNPPqnWrVvrnnvu0RdffKHAwEBJ0rRp03T99dfrrrvuUkREhPz8/NS3b99yb/9qDRw4UMuWLdO0adOUkJBQap86deroueee07lz5664vaeeeuqKZ15cjaFDhyo/P1833XSTxo0bp8cff1yPPvqobf28efMUGBio2267TYMGDdLEiRPl7u5uW1/Wazl69Gi99tprWrp0qTp06KDw8HAtXbr0itcPATp16qSkpCTNnj1b7du319tvv63ExMQy+7u4uOjEiRMaOnSoQkJC9OCDD6pHjx6aMWOGpN9GOsaNG6c2bdro7rvvVuvWra94mLcieC/9+ViM8k4CAFBlIiIi1KlTJyUnJzu7FMDUeC/9OTEyAwAATI0wAwAATI3DTAAAwNQYmQEAAKZGmAEAAKZGmAEAAKZGmAEAAKZGmAEAAKZGmAEAAKZGmAEAAKZGmAEAAKb2/wBmhP6Dj+hBEwAAAABJRU5ErkJggg==",
+                        "image/png": "iVBORw0KGgoAAAANSUhEUgAAAjMAAAGxCAYAAACXwjeMAAAAOXRFWHRTb2Z0d2FyZQBNYXRwbG90bGliIHZlcnNpb24zLjguNCwgaHR0cHM6Ly9tYXRwbG90bGliLm9yZy8fJSN1AAAACXBIWXMAAA9hAAAPYQGoP6dpAAA9nklEQVR4nO3deXiM9/7/8dfYJhFJrNnIN0kRx1ratLaeSrRRlNq6WIooLaVKU7VUVZy2KIeiWrqGtpTTKqenSqWIXRvUqaqjaWuJkkaVDMEguX9/9DI/I+tE0pk7fT6u674u87k/c9/vmcnMvHzuz32PxTAMQwAAACZVzt0FAAAA3AjCDAAAMDXCDAAAMDXCDAAAMDXCDAAAMDXCDAAAMDXCDAAAMDXCDAAAMDXCDAAAMDXCDMq8RYsWyWKxaNeuXe4upUDHjx9XQkKC9u7dW+xtfP/990pISNDhw4dzrYuLi1N4eHixt10ccXFxslgshS5xcXFKTk6WxWJRcnLyn1pjYXJycvT+++/r7rvvVs2aNVWxYkUFBASoS5cu+s9//qOcnBx3l1jqLBaLEhIS3F0GkK8K7i4AwB+OHz+uKVOmKDw8XM2bNy/WNr7//ntNmTJF0dHRuYLLpEmTNGrUqBsv1AWTJk3SsGHDHLf37NmjESNGaOrUqYqJiXG016pVS7Vq1dKOHTvUqFGjP7XGgly8eFHdu3fXunXr1Lt3by1YsEBBQUE6efKk1q5dqwceeEDLly9Xt27d3F1qqdqxY4fq1Knj7jKAfBFmgL+IunXrumWf1+734sWLkqT69eurVatWufrn1eZO8fHx+uKLL7R48WINGDDAaV3Pnj31zDPP6MKFC26qrnQZhqGLFy/K29vb414X4HocZsJfUlxcnKpUqaL//e9/uueee+Tj46Pg4GBNnz5dkrRz507dcccd8vHxUWRkpBYvXux0/6uHrpKSkjRo0CBVr15dPj4+6tq1q37++WenvuHh4YqLi8tVQ3R0tKKjoyVJycnJuu222yRJgwYNchx+uTq0v2vXLvXu3Vvh4eHy9vZWeHi4+vTpoyNHjjjV9MADD0iSYmJiHNtYtGiR4zFfP1pz8eJFTZgwQREREapUqZJq166tESNG6MyZM7keQ5cuXbR27Vrdcsst8vb21t/+9je9++67RX3KC5XXYaYbfZ0kKT09XUOHDlWdOnVUqVIlRUREaMqUKbpy5UqB9aSnp+vtt9/WPffckyvIXFW/fn01a9bMcfvo0aN6+OGHFRAQIKvVqoYNG2rWrFlOh6IOHz4si8WimTNn6uWXX3a8ptHR0frhhx90+fJljR8/XiEhIfL391ePHj2UkZHhtN+rr8fKlSvVrFkzeXl56aabbtK8efOc+l28eFFPP/20mjdvLn9/f1WvXl2tW7fWv//971yPxWKx6IknntDChQvVsGFDWa1Wx/N5/WGm8+fPa8yYMYqIiJCXl5eqV6+uqKgoffjhh07b/PTTT9W6dWtVrlxZvr6+io2N1Y4dO5z6JCQkyGKxaP/+/erTp4/8/f0VGBioRx55RJmZmQW8QsD/x8gM/rIuX76snj17atiwYXrmmWe0dOlSTZgwQTabTStWrNC4ceNUp04dvfrqq4qLi1OTJk106623Om1j8ODBio2N1dKlS5WWlqbnnntO0dHR+vbbb1W1atUi13LLLbcoMTFRgwYN0nPPPad7771XkhxD+4cPH1aDBg3Uu3dvVa9eXSdOnNCCBQt022236fvvv1fNmjV17733aurUqXr22Wf12muv6ZZbbpGU/4iMYRjq3r271q9frwkTJujvf/+7vv32W02ePFk7duzQjh07ZLVaHf3/+9//6umnn9b48eMVGBiot99+W4MHD1a9evV05513uvLUu+RGXqf09HTdfvvtKleunJ5//nnVrVtXO3bs0IsvvqjDhw8rMTEx3/1u3LhRly9fVvfu3YtU58mTJ9WmTRtdunRJL7zwgsLDw/XZZ59pzJgx+umnn/T666879X/ttdfUrFkzvfbaazpz5oyefvppde3aVS1btlTFihX17rvv6siRIxozZoyGDBmiTz/91On+e/fu1ejRo5WQkKCgoCAtWbJEo0aN0qVLlzRmzBhJkt1u1++//64xY8aodu3aunTpkr788kv17NlTiYmJuULaqlWrtGXLFj3//PMKCgpSQEBAno81Pj5e77//vl588UW1aNFCWVlZ+u6773Tq1ClHn6VLl6pfv37q0KGDPvzwQ9ntds2YMUPR0dFav3697rjjDqdt9urVSw899JAGDx6sffv2acKECZJUooEZZZgBlHGJiYmGJCMlJcXRNnDgQEOSsWLFCkfb5cuXjVq1ahmSjD179jjaT506ZZQvX96Ij4/Ptc0ePXo47Wvbtm2GJOPFF190tIWFhRkDBw7MVVe7du2Mdu3aOW6npKQYkozExMRCH9OVK1eMc+fOGT4+PsbcuXMd7R999JEhydi4cWOu+wwcONAICwtz3F67dq0hyZgxY4ZTv+XLlxuSjDfffNPpMXh5eRlHjhxxtF24cMGoXr26MXTo0ELrvWrjxo2GJOOjjz7Kd921td/o6zR06FCjSpUqTnUbhmH885//NCQZ+/fvz7fW6dOnG5KMtWvXFumxjR8/3pBkfPXVV07tjz/+uGGxWIyDBw8ahmEYhw4dMiQZN998s5Gdne3oN2fOHEOScd999zndf/To0YYkIzMz09EWFhZmWCwWY+/evU59Y2NjDT8/PyMrKyvPGq9cuWJcvnzZGDx4sNGiRQundZIMf39/4/fff891P0nG5MmTHbebNGlidO/ePd/nIjs72wgJCTGaNm3q9BjPnj1rBAQEGG3atHG0TZ48Oc+/w+HDhxteXl5GTk5OvvsBruIwE/6yLBaLOnfu7LhdoUIF1atXT8HBwWrRooWjvXr16goICHA6pHNVv379nG63adNGYWFh2rhxY4nWeu7cOY0bN0716tVThQoVVKFCBVWpUkVZWVk6cOBAsba5YcMGScp1COyBBx6Qj4+P1q9f79TevHlz/d///Z/jtpeXlyIjI/N8XkrSjbxOn332mWJiYhQSEqIrV644lk6dOkmSNm3aVGJ1btiwQY0aNdLtt9/u1B4XFyfDMBzP91WdO3dWuXL//yO4YcOGkuQYlbu+/ejRo07tjRs31s033+zU1rdvX9lsNu3Zs8fR9tFHH6lt27aqUqWKKlSooIoVK+qdd97J8++mffv2qlatWqGP9fbbb9eaNWs0fvx4JScn55o3dPDgQR0/flz9+/d3eoxVqlRRr169tHPnTp0/f97pPvfdd5/T7WbNmunixYu5DrEBeSHM4C+rcuXK8vLycmqrVKmSqlevnqtvpUqVHJNXrxUUFJRn27XD7SWhb9++mj9/voYMGaIvvvhCX3/9tVJSUlSrVq1iT0A9deqUKlSooFq1ajm1WyyWPB9DjRo1cm3DarWW+gTYG3mdfv31V/3nP/9RxYoVnZbGjRtLkn777bd893s1uB06dKhIdZ46dUrBwcG52kNCQhzrr3V9/ZUqVSqw/fq/v/z+9q7d1yeffKIHH3xQtWvX1gcffKAdO3YoJSVFjzzySJ5/z3nVn5d58+Zp3LhxWrVqlWJiYlS9enV1795dqampTvvP7/nIycnR6dOnndqv//u6eoizrE6wRslizgxwA9LT0/Nsq1evnuO2l5eX7HZ7rn6//fabatasWeg+MjMz9dlnn2ny5MkaP368o/3qfIjiqlGjhq5cuaKTJ086BRrDMJSenu6YkGxmNWvWVLNmzfTSSy/luf5q0MhLTEyMKlasqFWrVjmdXp6fGjVq6MSJE7najx8/7qilJOX3t3e1Fkn64IMPFBERoeXLl8tisTj65fX3KMmpT0F8fHw0ZcoUTZkyRb/++qtjlKZr16763//+59h/fs9HuXLlijQCBBQVIzPADViyZInT7e3bt+vIkSOOs5SkP848+fbbb536/fDDDzp48KBTW37/E7VYLDIMw2kyriS9/fbbys7OLtI28nLXXXdJ+uML71orVqxQVlaWY72ZdenSRd99953q1q2rqKioXEtBYSYoKMgxEvbee+/l2eenn35yvLZ33XWXvv/+e6dDPJL03nvvyWKxOF1XpyTs379f//3vf53ali5dKl9fX8fkb4vFokqVKjmFlPT09DzPZiquwMBAxcXFqU+fPjp48KDOnz+vBg0aqHbt2lq6dKkMw3D0zcrK0ooVKxxnOAElhZEZ4Abs2rVLQ4YM0QMPPKC0tDRNnDhRtWvX1vDhwx19+vfvr4cffljDhw9Xr169dOTIEc2YMSPX4Z26devK29tbS5YsUcOGDVWlShWFhIQoJCREd955p2bOnKmaNWsqPDxcmzZt0jvvvJPrjKkmTZpIkt588035+vrKy8tLEREReR4iio2N1T333KNx48bJZrOpbdu2jrOZWrRoof79+5f8E/Yn+8c//qGkpCS1adNGTz75pBo0aKCLFy/q8OHD+vzzz7Vw4cICLwY3e/Zs/fzzz4qLi9MXX3yhHj16KDAwUL/99puSkpKUmJioZcuWqVmzZnrqqaf03nvv6d5779U//vEPhYWFafXq1Xr99df1+OOPKzIyskQfW0hIiO677z4lJCQoODhYH3zwgZKSkvTyyy87gkKXLl30ySefaPjw4br//vuVlpamF154QcHBwY5DQsXRsmVLdenSRc2aNVO1atV04MABvf/++04hZcaMGerXr5+6dOmioUOHym63a+bMmTpz5ozj1HqgpBBmgBvwzjvv6P3331fv3r1l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rZOvr687ywYAAB7E464zU9K4zgzgPmX70wVAaTLldWYAAACKgzADAABMjTADAABMjTADAABMjTADAABMjTADAABMjTADAABMjTADAABMjTADAABMjTADAABMjTADAABMjTADAABMjTADAABMjTADAABMjTADAABMjTADAABMjTADAABMjTADAABMjTADAABMjTADAABMjTADAABMjTADAABM7YbDjM1m06pVq3TgwIGSqAcAAMAlLoeZBx98UPPnz5ckXbhwQVFRUXrwwQfVrFkzrVixosQLBAAAKIjLYWbz5s36+9//LklauXKlDMPQmTNnNG/ePL344oslXiAAAEBBXA4zmZmZql69uiRp7dq16tWrlypXrqx7771XqampJV4gAABAQVwOM6GhodqxY4eysrK0du1adejQQZJ0+vRpeXl5lXiBAAAABang6h1Gjx6tfv36qUqVKgoLC1N0dLSkPw4/NW3atKTrAwAAKJDLYWb48OG6/fbblZaWptjYWJUr98fgzk033cScGQAA8KezGIZhuLuI0mSz2eTv76/MzEz5+fmV+PYtlhLfJFBmlO1PFwClyZXv7yKNzMTHxxd557Nnzy5yXwAAgBtVpDDzzTffON3evXu3srOz1aBBA0nSDz/8oPLly+vWW28t+QoBAAAKUKQws3HjRse/Z8+eLV9fXy1evFjVqlWT9MeZTIMGDXJcfwYAAODP4vKcmdq1a2vdunVq3LixU/t3332nDh066Pjx4yVa4I1izgzgPsyZAVBcrnx/u3ydGZvNpl9//TVXe0ZGhs6ePevStqZNm6bbbrtNvr6+CggIUPfu3XXw4EGnPnFxcbJYLE5Lq1atXC0bAACUUS6HmR49emjQoEH6+OOPdezYMR07dkwff/yxBg8erJ49e7q0rU2bNmnEiBHauXOnkpKSdOXKFXXo0EFZWVlO/Tp27KgTJ044ls8//9zVsgEAQBnl8nVmFi5cqDFjxujhhx/W5cuX/9hIhQoaPHiwZs6c6dK21q5d63Q7MTFRAQEB2r17t+68805Hu9VqVVBQkKulAgCAvwCXw0zlypX1+uuva+bMmfrpp59kGIbq1asnHx+fGy4mMzNTkhy//XRVcnKyAgICVLVqVbVr104vvfSSAgIC8tyG3W6X3W533LbZbDdcFwAA8Fwec9E8wzDUrVs3nT59Wlu2bHG0L1++3PHTCYcOHdKkSZN05coV7d69W1arNdd2EhISNGXKlFztTAAG/nye8ekCwIxcmQDscpjJysrS9OnTtX79emVkZCgnJ8dp/c8//+x6xZJGjBih1atXa+vWrapTp06+/U6cOKGwsDAtW7Yszzk6eY3MhIaGEmYANyDMACiuEr8C8LWGDBmiTZs2qX///goODpalBL7NR44cqU8//VSbN28uMMhIUnBwsMLCwpSamprneqvVmueIDQAAKJtcDjNr1qzR6tWr1bZt2xveuWEYGjlypFauXKnk5GRFREQUep9Tp04pLS1NwcHBN7x/AABgfi6fml2tWrVcE3SLa8SIEfrggw+0dOlS+fr6Kj09Xenp6bpw4YIk6dy5cxozZox27Nihw4cPKzk5WV27dlXNmjXVo0ePEqkBAACYm8th5oUXXtDzzz+v8+fP3/DOFyxYoMzMTEVHRys4ONixLF++XJJUvnx57du3T926dVNkZKQGDhyoyMhI7dixQ76+vje8fwAAYH4uTwBu0aKF45Ts8PBwVaxY0Wn9nj17SrTAG8XPGQDuwwRgAMVVqhOAu3fvXty6AAAASpzHXGemtDAyA7hP2f50AVCaSnVk5qrdu3frwIEDslgsatSokVq0aFHcTQEAABSby2EmIyNDvXv3VnJysqpWrSrDMJSZmamYmBgtW7ZMtWrVKo06AQAA8uTy2UwjR46UzWbT/v379fvvv+v06dP67rvvZLPZ9OSTT5ZGjQAAAPlyec6Mv7+/vvzyS912221O7V9//bU6dOigM2fOlGR9N4w5M4D7MGcGQHG58v3t8shMTk5OrtOxJalixYq5fqcJAACgtLkcZtq3b69Ro0bp+PHjjrZffvlFTz31lO66664SLQ4AAKAwLoeZ+fPn6+zZswoPD1fdunVVr149RURE6OzZs3r11VdLo0YAAIB8uXw2U2hoqPbs2aOkpCT973//k2EYatSoke6+++7SqA8AAKBAXDTvBjEBGMhf2f50AVCaSnUC8JNPPql58+blap8/f75Gjx7t6uYAAABuiMthZsWKFWrbtm2u9jZt2ujjjz8ukaIAAACKyuUwc+rUKfn7++dq9/Pz02+//VYiRQEAABSVy2GmXr16Wrt2ba72NWvW6KabbiqRogAAAIrK5bOZ4uPj9cQTT+jkyZNq3769JGn9+vWaNWuW5syZU9L1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rbfqs88+03fffafHHntM/fv311dffeW0ncWLF6tChQratm2b3njjDUf7xIkTNWvWLO3atUsVKlTQI488UmhN6enpateunXJycrRp0yYFBwfn6hMeHq5hw4ZpwoQJysnJKXB706dP14oVK5SSklKUp8QhISFB8+fP1/bt25WWlqYHH3xQc+bM0dKlS7V69WolJSXp1VdfdbrP1efhq6++0rx58/TKK6/o7bffLvI+83st33rrLU2cOFEvvfSSDhw4oKlTp2rSpElavHix0/3HjRunJ598UgcOHNA999zj0uNF2VWuXDnNmzdP3333nRYvXqwNGzZo7Nix+fbv16+f6tSpo5SUFO3evVvjx49XxYoVJUkjRoyQ3W7X5s2btW/fPr388suqUqVKgfvnvYQiMeB2u3fvNiQZhw8fznN9SEiIMXHixHzvL8lYuXKlYRiGcejQIUOSsWXLFuPuu+822rZta5w5c6bQ/t98802hdbZr184YNWqUYRiG8eOPPxoWi8X45ZdfnPrcddddxoQJE/LdRufOnY2nn37aaZvNmzd36rNx40ZDkvHll1862lavXm1IMi5cuJDvtiUZlSpVMv72t78ZWVlZefYJCwszXnnlFSMjI8Pw9fU13nvvPcMwDGPUqFFGu3btHP0mT55s3HzzzYZhGEbv3r2N9u3bG4ZhGN98840hyTh06JBhGLmfv7xqnzZtmiHJ+OmnnxxtQ4cONe655x6n56Fhw4ZGTk6Oo23cuHFGw4YNnR7f1dftKn9/fyMxMTHPWq4KDQ01li5d6tT2wgsvGK1bt3a635w5c/J8zvDXMHDgQKN8+fKGj4+PY7n//vtz9fvXv/5l1KhRw3E7MTHR8Pf3d9z29fU1Fi1alOc+mjZtaiQkJOS5jvcSbgQjMx7g5ptv1l133aWmTZvqgQce0FtvvaXTp09LkjIyMnT8+HHdddddLm2zT58+OnfunNatW1fkn1C/asuWLapSpYpjWbJkSa4+e/bskWEYioyMdOq7adMm/fTTT5Kk7OxsvfTSS2rWrJlq1KihKlWqaN26dTp69KjTtqKiovKs49p5LldHWDIyMgqsvWvXrvrhhx+cRnjyUqtWLY0ZM0bPP/98ofN0XnzxRW3ZskXr1q0rsN+1rq09MDBQlStX1k033eTUdv1jadWqlSwWi+N269atlZqaquzs7CLv93onT55UWlqaBg8e7PQ6vfjii47X6ar8Xgf8dcTExGjv3r2OZd68edq4caNiY2NVu3Zt+fr6asCAATp16pTTYfBrxcfHa8iQIbr77rs1ffp0p7+zJ598Ui+++KLatm2ryZMnOybmF4T3EoqCMOMBypcvr6SkJK1Zs0aNGjXSq6++qgYNGujQoUPy9vYu1jY7d+6sb7/9NtdZO0URFRXl9IF233335eqTk5Oj8uXLa/fu3U59Dxw4oLlz50qSZs2apVdeeUVjx47Vhg0btHfvXt1zzz25woOPj0+edVwdmpbk+GAq7LDQww8/rMTERD3zzDP65z//WWDf+Ph4XbhwwemYd17q1q2rRx99VOPHj3c67l6Q62u/9vbVtsIey/UsFkuu/Rc2ufDqPt566y2n1+m7777L9beR3+uAvw4fHx/Vq1fPsVy6dEmdO3dWkyZNtGLFCu3evVuvvfaapPz/9hISErR//37de++92rBhgxo1aqSVK1dKkoYMGaKff/5Z/fv31759+xQVFZXrENH1eC+hKDz+V7P/KiwWi9q2bau2bdvq+eefV1hYmFauXKn4+HiFh4dr/fr1iomJKfL2Hn/8cTVp0kT33XefVq9erXbt2uXZr1KlSpLk9D8Wb2/vQufktGjRQtnZ2crIyNDf//73PPts2bJF3bp108MPPyzpjw+D1NRUNWzYsMiPozgGDBig8uXLa+DAgcrJycn3+H6VKlU0adIkJSQkqGvXrgVu8/nnn1fdunW1bNmy0ihZknJ9IO7cuVP169dX+fLlJf0xmnTixAnH+tTUVKeJj3m9loGBgapdu7Z+/vln9evXr9RqR9m0a9cuXblyRbNmzVK5cn/83/df//pXofeLjIxUZGSknnrqKfXp00eJiYnq0aOHJCk0NFTDhg1zzFt76623NHLkyBKtm/fSXw9hxgN89dVXWr9+vTp06KCAgAB99dVXOnnypONLPyEhQcOGDVNAQIA6deqks2fPatu2bYV+AIwcOVLZ2dnq0qWL1qxZozvuuCNXn4CAAHl7e2vt2rWqU6eOvLy8inRYKjIyUv369dOAAQM0a9YstWjRQr/99ps2bNigpk2bqnPnzqpXr55WrFih7du3q1q1apo9e7bS09NLPcxIf0xCLFeunPr376+cnByNHz8+z36PPfaYXnnlFX344Ydq2bJlvtsLDAxUfHy8Zs6cWVolKy0tTfHx8Ro6dKj27NmjV199VbNmzXKsb9++vebPn69WrVopJydH48aNc/pfan6vZUJCgp588kn5+fmpU6dOstvt2rVrl06fPq34+PhSezwwv7p16+rKlSt69dVX1bVrV23btk0LFy7Mt/+FCxf0zDPP6P7771dERISOHTumlJQU9erVS9If13Pq1KmTIiMjdfr0aW3YsKFUPg94L/31cJjJA/j5+Wnz5s3q3LmzIiMj9dxzz2nWrFmOC9sNHDhQc+bM0euvv67GjRurS5cujjOGCjN69GhNmTJFnTt31vbt23Otr1ChgubNm6c33nhDISEh6tatW5HrTkxM1IABA/T000+rQYMGuu+++/TVV18pNDRUkjRp0iTdcsstuueeexQdHa2goCB17969yNu/UX369NHSpUs1adIkTZ06Nc8+FStW1AsvvKCLFy8Wur1nnnmm0DMvbsSAAQN04cIF3X777RoxYoRGjhypxx57zLF+1qxZCg0N1Z133qm+fftqzJgxqly5smN9fq/lkCFD9Pbbb2vRokVq2rSp2rVrp0WLFhV6/RCgefPmmj17tl5++WU1adJES5Ys0bRp0/LtX758eZ06dUoDBgxQZGSkHnzwQXXq1ElTpkyR9MdIx4gRI9SwYUN17NhRDRo0KPQwb3HwXvrrsRhFnQQAoNRER0erefPmmjNnjrtLAUyN99JfEyMzAADA1AgzAADA1DjMBAAATI2RGQAAYGqEGQAAYGqEGQAAYGqEGQAAYGqEGQAAYGqEGQAAYGqEGQAAYGqEGQAAYGr/Dxv7sMhQIkjdAAAAAElFTkSuQmCC",
                         "text/plain": "<Figure size 640x480 with 1 Axes>"
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 }
             ],
             "source": [
```

### Comparing `fknni-1.0.0/docs/references.bib` & `fknni-1.1.0/docs/references.bib`

 * *Files identical despite different names*

### Comparing `fknni-1.0.0/pyproject.toml` & `fknni-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [build-system]
 build-backend = "hatchling.build"
 requires = ["hatchling"]
 
 [project]
 name = "fknni"
-version = "1.0.0"
+version = "1.1.0"
 description = "Fast implementations of KNN imputation."
 readme = "README.md"
-requires-python = ">=3.10"
+requires-python = ">=3.9"
 license = {file = "LICENSE"}
 authors = [
     {name = "Lukas Heumos"},
 ]
 maintainers = [
     {name = "Lukas Heumos", email = "lukas.heumos@posteo.net"},
 ]
```

### Comparing `fknni-1.0.0/src/fknni/faiss/faiss.py` & `fknni-1.1.0/src/fknni/faiss/faiss.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,37 +1,41 @@
-from typing import Literal
+from typing import Literal, Union
 
 import faiss
 import numpy as np
 import pandas as pd
 from sklearn.base import BaseEstimator, TransformerMixin
 from sklearn.utils.validation import check_array, check_is_fitted
 
 
 class FaissImputer(BaseEstimator, TransformerMixin):
     """Imputer for completing missing values using Faiss, incorporating weighted averages based on distance."""
 
     def __init__(
         self,
+        missing_values: Union[int, float, str, None] = np.nan,
         n_neighbors: int = 5,
+        *,
         metric: Literal["l2", "ip"] = "l2",
-        strategy: Literal["mean", "median", "weighted"] = "weighted",
+        strategy: Literal["mean", "median", "weighted"] = "mean",
         index_factory: str = "Flat",
     ):
         """Initializes FaissImputer with specified parameters that are used for the imputation.
 
         Args:
+            missing_values: The missing value to impute. Defaults to np.nan.
             n_neighbors: Number of neighbors to use for imputation. Defaults to 5.
             metric: Distance metric to use for neighbor search. Defaults to 'l2'.
             strategy: Method to compute imputed values among neighbors.
                       The weighted strategy is similar to scikt-learn's implementation,
                       where closer neighbors have a higher influence on the imputation.
             index_factory: Description of the Faiss index type to build. Defaults to 'Flat'.
         """
         super().__init__()
+        self.missing_values = missing_values
         self.n_neighbors = n_neighbors
         self.metric = metric
         self.strategy = strategy
         self.index_factory = index_factory
 
     def fit(self, X: np.ndarray | pd.DataFrame, *, y: np.ndarray | None = None) -> "FaissImputer":
         """Fits the FaissImputer to the provided data.
@@ -39,78 +43,74 @@
         Args:
             X: Input data with potential missing values.
             y: Ignored, present for compatibility with sklearn's TransformerMixin.
 
         Raises:
           ValueError: If any parameters are set to an invalid value.
         """
-        X = check_array(X, force_all_finite="allow-nan")
-        self.input_dtype_ = X.dtype
+        X = np.asarray(X, dtype=np.float32)
+        if isinstance(X, pd.DataFrame):
+            X = X.replace(self.missing_values, np.nan).values
+        else:
+            X = np.where(X == self.missing_values, np.nan, X)
 
-        # Handle missing values for indexing
-        self.means_ = np.nanmean(X, axis=0)  # Store means for missing value handling
-        X_non_missing = np.where(np.isnan(X), self.means_, X).astype(np.float32)
-
-        index = faiss.index_factory(
-            X_non_missing.shape[1],
-            self.index_factory,
-            faiss.METRIC_L2 if self.metric == "l2" else faiss.METRIC_INNER_PRODUCT,
-        )
+        if np.isnan(X).all(axis=0).any():
+            raise ValueError("Features with all values missing cannot be handled.")
+
+        mask = ~np.isnan(X).any(axis=1)
+        X_non_missing = X[mask]
+
+        index = faiss.index_factory(X_non_missing.shape[1], self.index_factory)
+        index.metric_type = faiss.METRIC_L2 if self.metric == "l2" else faiss.METRIC_INNER_PRODUCT
         index.train(X_non_missing)
         index.add(X_non_missing)
+
         self.index_ = index
+        self.global_fallbacks_ = (
+            np.nanmean(X, axis=0) if self.strategy in ["mean", "weighted"] else np.nanmedian(X, axis=0)
+        )
 
         return self
 
     def transform(self, X: np.ndarray | pd.DataFrame) -> np.ndarray:
         """Imputes missing values in the data using the fitted Faiss index.
 
         Args:
             X: Data with missing values to impute. Expected to be either a NumPy array or a pandas DataFrame.
 
         Returns:
             Data with imputed values as a NumPy array of the original data type.
         """
-        X = check_array(X, force_all_finite="allow-nan")
-        check_is_fitted(self, "index_")
-        X_imputed = np.array(X, dtype=np.float32)  # Use float32 for processing
-        missing_mask = np.isnan(X_imputed)
-
-        X_filled = np.where(missing_mask, self.means_, X_imputed)
-
-        for sample_idx in np.where(missing_mask.any(axis=1))[0]:
-            sample_row_filled = X_filled[sample_idx]
-            sample_missing_cols = np.where(missing_mask[sample_idx])[0]
-
-            distances, neighbor_indices = self.index_.search(sample_row_filled.reshape(1, -1), self.n_neighbors)
-            neighbors = X_filled[neighbor_indices[0]]
-
-            for col in sample_missing_cols:
-                valid_neighbors = neighbors[:, col][~np.isnan(neighbors[:, col])]
-                valid_distances = distances[0, : len(valid_neighbors)]
-
-                if len(valid_neighbors) < self.n_neighbors:
-                    if len(valid_neighbors) == 0:
-                        imputed_value = self.means_[col]
-                    else:
-                        if self.strategy in {"mean", "weighted"}:
-                            weights = (
-                                1 / (1 + valid_distances)
-                                if self.strategy == "weighted"
-                                else np.ones_like(valid_distances)
-                            )
-                            imputed_value = np.average(valid_neighbors, weights=weights)
-                        elif self.strategy == "median":
-                            imputed_value = np.median(valid_neighbors)
-                else:
-                    if self.strategy == "mean":
-                        imputed_value = np.mean(valid_neighbors)
-                    elif self.strategy == "median":
-                        imputed_value = np.median(valid_neighbors)
-                    elif self.strategy == "weighted":
-                        small_constant = 1e-10  # Small constant to prevent division by zero
-                        weights = 1 / (valid_distances + small_constant)
-                        imputed_value = np.average(valid_neighbors, weights=weights)
+        X = check_array(X, dtype=np.float32, force_all_finite="allow-nan")
+        check_is_fitted(self)
+        is_value_missing = np.isnan(X)
+
+        for sample_index in np.where(is_value_missing.any(axis=1))[0]:
+            sample_data = X[sample_index]
+            missing_value_mask = is_value_missing[sample_index]
+            missing_columns = np.where(missing_value_mask)[0]
+            sample_data[missing_value_mask] = self.global_fallbacks_[missing_value_mask]
+
+            distances, neighbor_indices = self.index_.search(sample_data.reshape(1, -1), self.n_neighbors)
+            neighbors_data = X[neighbor_indices[0]]
+            neighbor_values = neighbors_data[:, missing_columns]
+
+            if self.strategy == "mean":
+                imputed_values = np.nanmean(neighbor_values, axis=0)
+            elif self.strategy == "median":
+                imputed_values = np.nanmedian(neighbor_values, axis=0)
+            elif self.strategy == "weighted":
+                weights = 1 / (distances[0] + 1e-10)
+                adjusted_weights = weights[:, np.newaxis]
+                weighted_totals = np.nansum(neighbor_values * adjusted_weights, axis=0)
+                total_weights = np.nansum(adjusted_weights, axis=0)
+                imputed_values = weighted_totals / total_weights
+
+                no_weight_conditions = total_weights == 0
+                if no_weight_conditions.any():
+                    fallback_values = self.global_fallbacks_[missing_columns][no_weight_conditions]
+                    imputed_values[no_weight_conditions] = fallback_values
 
-                X_imputed[sample_idx, col] = imputed_value
+            sample_data[missing_columns] = imputed_values
+            X[sample_index] = sample_data
 
-        return X_imputed.astype(self.input_dtype_)  # Cast back to the original input dtype
+        return X
```

### Comparing `fknni-1.0.0/tests/test_faiss_imputation.py` & `fknni-1.1.0/tests/test_faiss_imputation.py`

 * *Files identical despite different names*

### Comparing `fknni-1.0.0/PKG-INFO` & `fknni-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: fknni
-Version: 1.0.0
+Version: 1.1.0
 Summary: Fast implementations of KNN imputation.
 Author: Lukas Heumos
 Maintainer-email: Lukas Heumos <lukas.heumos@posteo.net>
-Requires-Python: >=3.10
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: scikit-learn
 Requires-Dist: faiss-cpu
 Requires-Dist: pandas
 Requires-Dist: pre-commit ; extra == "dev"
 Requires-Dist: twine>=4.0.2 ; extra == "dev"
 Requires-Dist: docutils>=0.8,!=0.18.*,!=0.19.* ; extra == "doc"
@@ -54,15 +54,15 @@
 -   [Faiss example notebook][link-faiss-example].
 
 ## Installation
 
 You need to have Python 3.10 or newer installed on your system.
 If you don't have Python installed, we recommend installing [Mambaforge](https://github.com/conda-forge/miniforge#mambaforge).
 
-Install the latest release of `fknni` from `PyPI <https://pypi.org/project/fknni/>`\_:
+Install the latest release of `fknni` from [PyPI](https://pypi.org/project/fknni):
 
 ```bash
 pip install fknni
 ```
 
 Install the latest development version:
```


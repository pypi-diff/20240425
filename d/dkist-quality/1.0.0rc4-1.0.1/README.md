# Comparing `tmp/dkist-quality-1.0.0rc4.tar.gz` & `tmp/dkist_quality-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dkist-quality-1.0.0rc4.tar", last modified: Fri Feb 23 00:02:53 2024, max compression
+gzip compressed data, was "dkist_quality-1.0.1.tar", last modified: Thu Apr 25 19:41:27 2024, max compression
```

## Comparing `dkist-quality-1.0.0rc4.tar` & `dkist_quality-1.0.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-23 00:02:53.834111 dkist-quality-1.0.0rc4/
--rw-rw-rw-   0 root         (0) root         (0)     3104 2024-02-23 00:02:26.000000 dkist-quality-1.0.0rc4/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      580 2024-02-23 00:02:26.000000 dkist-quality-1.0.0rc4/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)      468 2024-02-23 00:02:26.000000 dkist-quality-1.0.0rc4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2156 2024-02-23 00:02:53.834111 dkist-quality-1.0.0rc4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1229 2024-02-23 00:02:26.000000 dkist-quality-1.0.0rc4/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     2513 2024-02-23 00:02:26.000000 dkist-quality-1.0.0rc4/bitbucket-pipelines.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-23 00:02:53.818111 dkist-quality-1.0.0rc4/dkist_quality/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-23 00:02:26.000000 dkist-quality-1.0.0rc4/dkist_quality/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      414 2024-02-23 00:02:53.000000 dkist-quality-1.0.0rc4/dkist_quality/_version.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-23 00:02:53.834111 dkist-quality-1.0.0rc4/dkist_quality/fonts/
--rw-rw-rw-   0 root         (0) root         (0)    91676 2024-02-23 00:02:26.000000 dkist-quality-1.0.0rc4/dkist_quality/fonts/Oswald-Bold.ttf
--rw-rw-rw-   0 root         (0) root         (0)    91400 2024-02-23 00:02:26.000000 dkist-quality-1.0.0rc4/dkist_quality/fonts/Oswald-Regular.ttf
--rw-rw-rw-   0 root         (0) root         (0)      871 2024-02-23 00:02:26.000000 dkist-quality-1.0.0rc4/dkist_quality/json_encoder.py
--rw-rw-rw-   0 root         (0) root         (0)    34162 2024-02-23 00:02:26.000000 dkist-quality-1.0.0rc4/dkist_quality/report.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-23 00:02:53.834111 dkist-quality-1.0.0rc4/dkist_quality/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-23 00:02:26.000000 dkist-quality-1.0.0rc4/dkist_quality/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11169 2024-02-23 00:02:26.000000 dkist-quality-1.0.0rc4/dkist_quality/tests/test_report.py
--rw-rw-rw-   0 root         (0) root         (0)      346 2024-02-23 00:02:26.000000 dkist-quality-1.0.0rc4/dkist_quality/version.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-23 00:02:53.834111 dkist-quality-1.0.0rc4/dkist_quality.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2156 2024-02-23 00:02:53.000000 dkist-quality-1.0.0rc4/dkist_quality.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      668 2024-02-23 00:02:53.000000 dkist-quality-1.0.0rc4/dkist_quality.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2024-02-23 00:02:53.000000 dkist-quality-1.0.0rc4/dkist_quality.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2024-02-23 00:02:53.000000 dkist-quality-1.0.0rc4/dkist_quality.egg-info/not-zip-safe
--rw-rw-rw-   0 root         (0) root         (0)      150 2024-02-23 00:02:53.000000 dkist-quality-1.0.0rc4/dkist_quality.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       34 2024-02-23 00:02:53.000000 dkist-quality-1.0.0rc4/dkist_quality.egg-info/top_level.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-23 00:02:53.834111 dkist-quality-1.0.0rc4/licenses/
--rw-rw-rw-   0 root         (0) root         (0)     1482 2024-02-23 00:02:26.000000 dkist-quality-1.0.0rc4/licenses/LICENSE.rst
--rw-rw-rw-   0 root         (0) root         (0)      372 2024-02-23 00:02:26.000000 dkist-quality-1.0.0rc4/licenses/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     1659 2024-02-23 00:02:26.000000 dkist-quality-1.0.0rc4/licenses/TEMPLATE_LICENSE.rst
--rw-rw-rw-   0 root         (0) root         (0)     2035 2024-02-23 00:02:26.000000 dkist-quality-1.0.0rc4/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       38 2024-02-23 00:02:53.834111 dkist-quality-1.0.0rc4/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1214 2024-02-23 00:02:26.000000 dkist-quality-1.0.0rc4/tox.ini
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-25 19:41:27.820276 dkist_quality-1.0.1/
+-rw-rw-rw-   0 root         (0) root         (0)     3104 2024-04-25 19:41:15.000000 dkist_quality-1.0.1/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      580 2024-04-25 19:41:15.000000 dkist_quality-1.0.1/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      468 2024-04-25 19:41:15.000000 dkist_quality-1.0.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2155 2024-04-25 19:41:27.820276 dkist_quality-1.0.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1229 2024-04-25 19:41:15.000000 dkist_quality-1.0.1/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2513 2024-04-25 19:41:15.000000 dkist_quality-1.0.1/bitbucket-pipelines.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-25 19:41:27.820276 dkist_quality-1.0.1/dkist_quality/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-25 19:41:15.000000 dkist_quality-1.0.1/dkist_quality/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      411 2024-04-25 19:41:27.000000 dkist_quality-1.0.1/dkist_quality/_version.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-25 19:41:27.820276 dkist_quality-1.0.1/dkist_quality/fonts/
+-rw-rw-rw-   0 root         (0) root         (0)    91676 2024-04-25 19:41:15.000000 dkist_quality-1.0.1/dkist_quality/fonts/Oswald-Bold.ttf
+-rw-rw-rw-   0 root         (0) root         (0)    91400 2024-04-25 19:41:15.000000 dkist_quality-1.0.1/dkist_quality/fonts/Oswald-Regular.ttf
+-rw-rw-rw-   0 root         (0) root         (0)      871 2024-04-25 19:41:15.000000 dkist_quality-1.0.1/dkist_quality/json_encoder.py
+-rw-rw-rw-   0 root         (0) root         (0)    34162 2024-04-25 19:41:15.000000 dkist_quality-1.0.1/dkist_quality/report.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-25 19:41:27.820276 dkist_quality-1.0.1/dkist_quality/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-25 19:41:15.000000 dkist_quality-1.0.1/dkist_quality/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11169 2024-04-25 19:41:15.000000 dkist_quality-1.0.1/dkist_quality/tests/test_report.py
+-rw-rw-rw-   0 root         (0) root         (0)      346 2024-04-25 19:41:15.000000 dkist_quality-1.0.1/dkist_quality/version.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-25 19:41:27.820276 dkist_quality-1.0.1/dkist_quality.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2155 2024-04-25 19:41:27.000000 dkist_quality-1.0.1/dkist_quality.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      668 2024-04-25 19:41:27.000000 dkist_quality-1.0.1/dkist_quality.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-04-25 19:41:27.000000 dkist_quality-1.0.1/dkist_quality.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-04-25 19:41:27.000000 dkist_quality-1.0.1/dkist_quality.egg-info/not-zip-safe
+-rw-rw-rw-   0 root         (0) root         (0)      152 2024-04-25 19:41:27.000000 dkist_quality-1.0.1/dkist_quality.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       34 2024-04-25 19:41:27.000000 dkist_quality-1.0.1/dkist_quality.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-25 19:41:27.820276 dkist_quality-1.0.1/licenses/
+-rw-rw-rw-   0 root         (0) root         (0)     1482 2024-04-25 19:41:15.000000 dkist_quality-1.0.1/licenses/LICENSE.rst
+-rw-rw-rw-   0 root         (0) root         (0)      372 2024-04-25 19:41:15.000000 dkist_quality-1.0.1/licenses/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1659 2024-04-25 19:41:15.000000 dkist_quality-1.0.1/licenses/TEMPLATE_LICENSE.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2037 2024-04-25 19:41:15.000000 dkist_quality-1.0.1/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       38 2024-04-25 19:41:27.820276 dkist_quality-1.0.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1214 2024-04-25 19:41:15.000000 dkist_quality-1.0.1/tox.ini
```

### Comparing `dkist-quality-1.0.0rc4/.gitignore` & `dkist_quality-1.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `dkist-quality-1.0.0rc4/.pre-commit-config.yaml` & `dkist_quality-1.0.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dkist-quality-1.0.0rc4/PKG-INFO` & `dkist_quality-1.0.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: dkist-quality
-Version: 1.0.0rc4
+Version: 1.0.1
 Summary: DKIST library for generating quality report pdf
 Author-email: NSO / AURA <dkistdc@nso.edu>
 License: BSD 3-Clause
 Project-URL: repository, https://bitbucket.org/dkistdc/dkist-quality
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.10
 Description-Content-Type: text/x-rst
-Requires-Dist: reportlab==4.1.0
-Requires-Dist: matplotlib==3.7.4
-Requires-Dist: seaborn==0.13.2
-Requires-Dist: dacite==1.8.1
-Requires-Dist: natsort==8.4.0
-Requires-Dist: pydantic<2,>=1.10.14
+Requires-Dist: reportlab>=4.0.4
+Requires-Dist: matplotlib<3.8,>=3.6
+Requires-Dist: seaborn>=0.13.0
+Requires-Dist: dacite>=1.8.0
+Requires-Dist: natsort>=8.0.0
+Requires-Dist: pydantic<2,>=1.10.4
 Provides-Extra: test
 Requires-Dist: tox>=4; extra == "test"
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Requires-Dist: Pygments; extra == "test"
 Requires-Dist: PyPDF4; extra == "test"
```

### Comparing `dkist-quality-1.0.0rc4/README.rst` & `dkist_quality-1.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `dkist-quality-1.0.0rc4/bitbucket-pipelines.yml` & `dkist_quality-1.0.1/bitbucket-pipelines.yml`

 * *Files identical despite different names*

### Comparing `dkist-quality-1.0.0rc4/dkist_quality/fonts/Oswald-Bold.ttf` & `dkist_quality-1.0.1/dkist_quality/fonts/Oswald-Bold.ttf`

 * *Files identical despite different names*

### Comparing `dkist-quality-1.0.0rc4/dkist_quality/fonts/Oswald-Regular.ttf` & `dkist_quality-1.0.1/dkist_quality/fonts/Oswald-Regular.ttf`

 * *Files identical despite different names*

### Comparing `dkist-quality-1.0.0rc4/dkist_quality/json_encoder.py` & `dkist_quality-1.0.1/dkist_quality/json_encoder.py`

 * *Files identical despite different names*

### Comparing `dkist-quality-1.0.0rc4/dkist_quality/report.py` & `dkist_quality-1.0.1/dkist_quality/report.py`

 * *Files identical despite different names*

### Comparing `dkist-quality-1.0.0rc4/dkist_quality/tests/test_report.py` & `dkist_quality-1.0.1/dkist_quality/tests/test_report.py`

 * *Files identical despite different names*

### Comparing `dkist-quality-1.0.0rc4/dkist_quality.egg-info/PKG-INFO` & `dkist_quality-1.0.1/dkist_quality.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: dkist-quality
-Version: 1.0.0rc4
+Version: 1.0.1
 Summary: DKIST library for generating quality report pdf
 Author-email: NSO / AURA <dkistdc@nso.edu>
 License: BSD 3-Clause
 Project-URL: repository, https://bitbucket.org/dkistdc/dkist-quality
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.10
 Description-Content-Type: text/x-rst
-Requires-Dist: reportlab==4.1.0
-Requires-Dist: matplotlib==3.7.4
-Requires-Dist: seaborn==0.13.2
-Requires-Dist: dacite==1.8.1
-Requires-Dist: natsort==8.4.0
-Requires-Dist: pydantic<2,>=1.10.14
+Requires-Dist: reportlab>=4.0.4
+Requires-Dist: matplotlib<3.8,>=3.6
+Requires-Dist: seaborn>=0.13.0
+Requires-Dist: dacite>=1.8.0
+Requires-Dist: natsort>=8.0.0
+Requires-Dist: pydantic<2,>=1.10.4
 Provides-Extra: test
 Requires-Dist: tox>=4; extra == "test"
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Requires-Dist: Pygments; extra == "test"
 Requires-Dist: PyPDF4; extra == "test"
```

### Comparing `dkist-quality-1.0.0rc4/dkist_quality.egg-info/SOURCES.txt` & `dkist_quality-1.0.1/dkist_quality.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dkist-quality-1.0.0rc4/licenses/LICENSE.rst` & `dkist_quality-1.0.1/licenses/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `dkist-quality-1.0.0rc4/licenses/TEMPLATE_LICENSE.rst` & `dkist_quality-1.0.1/licenses/TEMPLATE_LICENSE.rst`

 * *Files identical despite different names*

### Comparing `dkist-quality-1.0.0rc4/pyproject.toml` & `dkist_quality-1.0.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -20,20 +20,20 @@
 ]
 license = { text = "BSD 3-Clause" }
 authors = [
   { name = "NSO / AURA", email = "dkistdc@nso.edu" },
 ]
 # the current version of Airflow does not support pydantic v2
 dependencies = [
-    "reportlab==4.1.0",
-    "matplotlib==3.7.4",
-    "seaborn==0.13.2",
-    "dacite==1.8.1",
-    "natsort==8.4.0",
-    "pydantic>=1.10.14,<2",
+    "reportlab>=4.0.4",
+    "matplotlib>=3.6,<3.8",
+    "seaborn>=0.13.0",
+    "dacite>=1.8.0",
+    "natsort>=8.0.0",
+    "pydantic>=1.10.4,<2",
 ]
 dynamic = ["version"]
 
 # tox is not required to run the tests, but simplifies IDE integration
 # Pygments is solely to support README.rst rendering
 [project.optional-dependencies]
 test = [
```

### Comparing `dkist-quality-1.0.0rc4/tox.ini` & `dkist_quality-1.0.1/tox.ini`

 * *Files identical despite different names*


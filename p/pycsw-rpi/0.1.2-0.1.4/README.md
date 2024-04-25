# Comparing `tmp/pycsw-rpi-0.1.2.tar.gz` & `tmp/pycsw_rpi-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycsw-rpi-0.1.2.tar", max compression
+gzip compressed data, was "pycsw_rpi-0.1.4.tar", max compression
```

## Comparing `pycsw-rpi-0.1.2.tar` & `pycsw_rpi-0.1.4.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0     1728 2023-06-05 11:29:05.611314 pycsw-rpi-0.1.2/Readme.md
--rw-r--r--   0        0        0     1400 2023-06-05 11:29:05.611314 pycsw-rpi-0.1.2/pycsw_rpi/admin.py
--rw-r--r--   0        0        0     1164 2023-06-05 11:29:05.611314 pycsw-rpi-0.1.2/pycsw_rpi/apiso.py
--rw-r--r--   0        0        0      796 2023-06-05 11:29:05.611314 pycsw-rpi-0.1.2/pycsw_rpi/config.py
--rw-r--r--   0        0        0     3064 2023-06-05 11:29:05.611314 pycsw-rpi-0.1.2/pycsw_rpi/metadata.py
--rw-r--r--   0        0        0      601 2023-06-05 11:29:05.611314 pycsw-rpi-0.1.2/pycsw_rpi/wsgi.py
--rw-r--r--   0        0        0      957 2023-06-05 11:37:10.633764 pycsw-rpi-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2646 2023-06-05 11:37:17.166885 pycsw-rpi-0.1.2/setup.py
--rw-r--r--   0        0        0     2483 2023-06-05 11:37:17.167250 pycsw-rpi-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1962 2024-04-25 06:51:03.766849 pycsw_rpi-0.1.4/Readme.md
+-rw-r--r--   0        0        0     1400 2023-06-05 11:29:05.611314 pycsw_rpi-0.1.4/pycsw_rpi/admin.py
+-rw-r--r--   0        0        0     1164 2023-06-05 11:29:05.611314 pycsw_rpi-0.1.4/pycsw_rpi/apiso.py
+-rw-r--r--   0        0        0      796 2023-06-05 11:29:05.611314 pycsw_rpi-0.1.4/pycsw_rpi/config.py
+-rw-r--r--   0        0        0     4627 2024-04-25 06:51:03.766849 pycsw_rpi-0.1.4/pycsw_rpi/metadata.py
+-rw-r--r--   0        0        0      601 2023-06-05 11:29:05.611314 pycsw_rpi-0.1.4/pycsw_rpi/wsgi.py
+-rw-r--r--   0        0        0      957 2024-04-25 07:07:23.200010 pycsw_rpi-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     2819 1970-01-01 00:00:00.000000 pycsw_rpi-0.1.4/PKG-INFO
```

### Comparing `pycsw-rpi-0.1.2/pycsw_rpi/admin.py` & `pycsw_rpi-0.1.4/pycsw_rpi/admin.py`

 * *Files identical despite different names*

### Comparing `pycsw-rpi-0.1.2/pycsw_rpi/apiso.py` & `pycsw_rpi-0.1.4/pycsw_rpi/apiso.py`

 * *Files identical despite different names*

### Comparing `pycsw-rpi-0.1.2/pycsw_rpi/config.py` & `pycsw_rpi-0.1.4/pycsw_rpi/config.py`

 * *Files identical despite different names*

### Comparing `pycsw-rpi-0.1.2/pycsw_rpi/wsgi.py` & `pycsw_rpi-0.1.4/pycsw_rpi/wsgi.py`

 * *Files identical despite different names*

### Comparing `pycsw-rpi-0.1.2/pyproject.toml` & `pycsw_rpi-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pycsw-rpi"
-version = "0.1.2"
+version = "0.1.4"
 description = "PyCSW monkey patched for Slovak national catalogue service"
 authors = ["Peter Mozolík <petermozolik@gmail.com>"]
 license = "MIT"
 readme = "Readme.md"
 repository = "https://gitlab.com/mzpsr/minzp/geocloud.sk/applications/pycsw-rpi"
 
 [tool.poetry.dependencies]
```

### Comparing `pycsw-rpi-0.1.2/PKG-INFO` & `pycsw_rpi-0.1.4/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 Metadata-Version: 2.1
 Name: pycsw-rpi
-Version: 0.1.2
+Version: 0.1.4
 Summary: PyCSW monkey patched for Slovak national catalogue service
 Home-page: https://gitlab.com/mzpsr/minzp/geocloud.sk/applications/pycsw-rpi
 License: MIT
 Author: Peter Mozolík
 Author-email: petermozolik@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: SQLAlchemy (>=1.4,<2.0)
 Requires-Dist: pycsw (>=2.6,<3.0)
 Project-URL: Repository, https://gitlab.com/mzpsr/minzp/geocloud.sk/applications/pycsw-rpi
 Description-Content-Type: text/markdown
 
 # PyCSW RPI `pycsw-rpi`
 
-[Monkey patched](https://en.wikipedia.org/wiki/Monkey_patch) `pycsw` for Slovak national catalogue service. 
+[Monkey patched](https://en.wikipedia.org/wiki/Monkey_patch) `pycsw` for Slovak national catalogue service.
 
 Check [original `pycsw` documentation ](https://docs.pycsw.org/en/2.6.1/index.html) for more details.
 
 ---
 
 ## Setup
 
@@ -33,15 +35,15 @@
 
 ```bash
 pip install --user pycsw-rpi
 ```
 
 ### Create configuration file
 
-Configuration file is not distributed with package. 
+Configuration file is not distributed with package.
 
 Sample configuration can be downloaded from `<<url>>`
 
 ### Administrative command (CLI)
 
 `pycsw_rpi-admin` script is installed with package in `$PATH`, this script is replacement for original `pycsw-admin.py` script supporting modified beahaviour and can be used exactly like original one.
 
@@ -63,31 +65,37 @@
 
 ```bash
 python -m pycsw_rpi.wsgi
 ```
 
 ### Deploy as WSGI application
 
-`pycsw_rpi.wsgi` module contains WSGI `application` object (function) ready to be deployed with WSGI server (e.g. `gunicorn`, `uwsgi`). No WSGI server is installed with this package as dependecy. 
+`pycsw_rpi.wsgi` module contains WSGI `application` object (function) ready to be deployed with WSGI server (e.g. `gunicorn`, `uwsgi`). No WSGI server is installed with this package as dependecy.
 
 To deploy with `gunicorn`:
 
 ```bash
 # `gunicorn` package need to installed separately
 pip install --user gunicorn
 gunicorn pycsw_rpi.wsgi:application
 ```
 
 ---
 
 ## Modifications implemented (via monkey patches) to original `pycsw`
 
 Added queryables to APISO plugin:
+
 - `rpi:OrganizationUUID`
 - `rpi:IsViewable`
 - `rpi:IsSearchable`
 
+Modified APISO queryables:
+
+- `apiso:ParentIdentifier` support for gmx:Anchor encoding added
+- `apiso:SpecificationTitle` support for gmx:Anchor encoding added
+- `apiso:Subject` support for gmx:Anchor encoding added in keywords parsing
+
 ---
 
 ## Contributions
 
-
```


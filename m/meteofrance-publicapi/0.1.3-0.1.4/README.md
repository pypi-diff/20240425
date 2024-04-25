# Comparing `tmp/meteofrance-publicapi-0.1.3.tar.gz` & `tmp/meteofrance_publicapi-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meteofrance-publicapi-0.1.3.tar", last modified: Fri Apr  5 18:54:03 2024, max compression
+gzip compressed data, was "meteofrance_publicapi-0.1.4.tar", last modified: Thu Apr 25 13:09:53 2024, max compression
```

## Comparing `meteofrance-publicapi-0.1.3.tar` & `meteofrance_publicapi-0.1.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:54:03.107198 meteofrance-publicapi-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-05 18:53:56.000000 meteofrance-publicapi-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    46449 2024-04-05 18:54:03.107198 meteofrance-publicapi-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4329 2024-04-05 18:53:56.000000 meteofrance-publicapi-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:54:03.103198 meteofrance-publicapi-0.1.3/meteofrance_publicapi/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-05 18:53:56.000000 meteofrance-publicapi-0.1.3/meteofrance_publicapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10886 2024-04-05 18:53:56.000000 meteofrance-publicapi-0.1.3/meteofrance_publicapi/arome.py
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-05 18:53:56.000000 meteofrance-publicapi-0.1.3/meteofrance_publicapi/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     5353 2024-04-05 18:53:56.000000 meteofrance-publicapi-0.1.3/meteofrance_publicapi/core.py
--rw-r--r--   0 runner    (1001) docker     (127)      971 2024-04-05 18:53:56.000000 meteofrance-publicapi-0.1.3/meteofrance_publicapi/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     5653 2024-04-05 18:53:56.000000 meteofrance-publicapi-0.1.3/meteofrance_publicapi/observations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-04-05 18:53:56.000000 meteofrance-publicapi-0.1.3/meteofrance_publicapi/raster.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:54:03.103198 meteofrance-publicapi-0.1.3/meteofrance_publicapi/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 18:53:56.000000 meteofrance-publicapi-0.1.3/meteofrance_publicapi/tests/__inti__.py
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-05 18:53:56.000000 meteofrance-publicapi-0.1.3/meteofrance_publicapi/tests/test_import.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:54:03.107198 meteofrance-publicapi-0.1.3/meteofrance_publicapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    46449 2024-04-05 18:54:03.000000 meteofrance-publicapi-0.1.3/meteofrance_publicapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-05 18:54:03.000000 meteofrance-publicapi-0.1.3/meteofrance_publicapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 18:54:03.000000 meteofrance-publicapi-0.1.3/meteofrance_publicapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 18:54:02.000000 meteofrance-publicapi-0.1.3/meteofrance_publicapi.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-05 18:54:03.000000 meteofrance-publicapi-0.1.3/meteofrance_publicapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-05 18:54:03.000000 meteofrance-publicapi-0.1.3/meteofrance_publicapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4273 2024-04-05 18:53:56.000000 meteofrance-publicapi-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 18:54:03.107198 meteofrance-publicapi-0.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:09:53.566203 meteofrance_publicapi-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-25 13:09:49.000000 meteofrance_publicapi-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    46453 2024-04-25 13:09:53.566203 meteofrance_publicapi-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4333 2024-04-25 13:09:49.000000 meteofrance_publicapi-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:09:53.562203 meteofrance_publicapi-0.1.4/meteofrance_publicapi/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-25 13:09:49.000000 meteofrance_publicapi-0.1.4/meteofrance_publicapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-25 13:09:49.000000 meteofrance_publicapi-0.1.4/meteofrance_publicapi/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5353 2024-04-25 13:09:49.000000 meteofrance_publicapi-0.1.4/meteofrance_publicapi/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-25 13:09:49.000000 meteofrance_publicapi-0.1.4/meteofrance_publicapi/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14023 2024-04-25 13:09:49.000000 meteofrance_publicapi-0.1.4/meteofrance_publicapi/forecast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5653 2024-04-25 13:09:49.000000 meteofrance_publicapi-0.1.4/meteofrance_publicapi/observations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-04-25 13:09:49.000000 meteofrance_publicapi-0.1.4/meteofrance_publicapi/raster.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:09:53.562203 meteofrance_publicapi-0.1.4/meteofrance_publicapi/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 13:09:49.000000 meteofrance_publicapi-0.1.4/meteofrance_publicapi/tests/__inti__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-25 13:09:49.000000 meteofrance_publicapi-0.1.4/meteofrance_publicapi/tests/test_import.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:09:53.566203 meteofrance_publicapi-0.1.4/meteofrance_publicapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    46453 2024-04-25 13:09:53.000000 meteofrance_publicapi-0.1.4/meteofrance_publicapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-25 13:09:53.000000 meteofrance_publicapi-0.1.4/meteofrance_publicapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 13:09:53.000000 meteofrance_publicapi-0.1.4/meteofrance_publicapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 13:09:53.000000 meteofrance_publicapi-0.1.4/meteofrance_publicapi.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-25 13:09:53.000000 meteofrance_publicapi-0.1.4/meteofrance_publicapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-25 13:09:53.000000 meteofrance_publicapi-0.1.4/meteofrance_publicapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4273 2024-04-25 13:09:49.000000 meteofrance_publicapi-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 13:09:53.566203 meteofrance_publicapi-0.1.4/setup.cfg
```

### Comparing `meteofrance-publicapi-0.1.3/LICENSE` & `meteofrance_publicapi-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `meteofrance-publicapi-0.1.3/PKG-INFO` & `meteofrance_publicapi-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meteofrance-publicapi
-Version: 0.1.3
+Version: 0.1.4
 Summary: A wrapper of the portail-api.meteofrance.fr datasets
 Author: Antoine Tavant
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -792,13 +792,13 @@
 | 2099       | 98832005 | NaN       | OUINNE                  | -21.984000 | 166.680500 | 54             | 1974-01-01 | ETENDU |
 | 2100       | 98832006 | NaN       | RIVIERE BLANCHE         | -22.132667 | 166.726333 | 171            | 2000-11-01 | ETENDU |
 | 2101       | 98832101 | NaN       | GORO_ANCIENNE_PEPINIERE | -22.269167 | 166.967500 | 298            | 1995-01-01 | ETENDU |
 | 2102       | 98833002 | NaN       | MEA                     | -21.455500 | 165.767333 | 571            | 1988-01-01 | ETENDU |
 
 ### Accessing Arome Forecasts
 
-See the notebook [Arome Forecast](./examples/arome.ipynb) for examples of accessing the forecast of the Arome model.
+See the notebook [Arome Forecast](./doc/examples/arome.ipynb) for examples of accessing the forecast of the AROME model.
 
 # TODO
 
 - [ ] Add local cache capabilities, for instance with [joblib](https://joblib.readthedocs.io/en/stable/memory.html)
 - [ ] Add persistent storage, locally or with a could provider
```

### Comparing `meteofrance-publicapi-0.1.3/README.md` & `meteofrance_publicapi-0.1.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -76,13 +76,13 @@
 | 2099       | 98832005 | NaN       | OUINNE                  | -21.984000 | 166.680500 | 54             | 1974-01-01 | ETENDU |
 | 2100       | 98832006 | NaN       | RIVIERE BLANCHE         | -22.132667 | 166.726333 | 171            | 2000-11-01 | ETENDU |
 | 2101       | 98832101 | NaN       | GORO_ANCIENNE_PEPINIERE | -22.269167 | 166.967500 | 298            | 1995-01-01 | ETENDU |
 | 2102       | 98833002 | NaN       | MEA                     | -21.455500 | 165.767333 | 571            | 1988-01-01 | ETENDU |
 
 ### Accessing Arome Forecasts
 
-See the notebook [Arome Forecast](./examples/arome.ipynb) for examples of accessing the forecast of the Arome model.
+See the notebook [Arome Forecast](./doc/examples/arome.ipynb) for examples of accessing the forecast of the AROME model.
 
 # TODO
 
 - [ ] Add local cache capabilities, for instance with [joblib](https://joblib.readthedocs.io/en/stable/memory.html)
 - [ ] Add persistent storage, locally or with a could provider
```

### Comparing `meteofrance-publicapi-0.1.3/meteofrance_publicapi/arome.py` & `meteofrance_publicapi-0.1.4/meteofrance_publicapi/forecast.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,33 @@
 from pathlib import Path
 import xmltodict
+from .errors import MissingDataError
 import logging
 from .core import MeteoFranceAPI
 
 logger = logging.getLogger(__name__)
 
 #: The available territories for the AROME model.
-AVAILABLE_TERRITORY = [
+AVAILABLE_AROME_TERRITORY = [
     "FRANCE",
     "NCALED",
     "INDIEN",
     "POLYN",
     "GUYANE",
     "ANTIL",
 ]
 
-precision_float_to_str = {0.01: "001", 0.025: "0025"}
+AVAILABLE_ARPEGE_TERRITORY = [ "EUROPE", "GLOBE", "ATOURX", "EURAT"]
+RELATION_TERRITORY_TO_PREC_ARPEGE = {"EUROPE": 0.1,
+                                     "GLOBE": 0.25,
+                                     "ATOURX": 0.1,
+                                     "EURAT": 0.05}
+
+precision_float_to_str = {0.25: "025", 0.1: "01", 0.05: "005", 0.01: "001", 0.025: "0025"}
+
 
 
 class AromeForecast(MeteoFranceAPI):
     """Access the AROME numerical Forcast.
 
     Parameters
     ----------
@@ -108,17 +116,17 @@
         self.all_coverageid = None # the list of all coverage ID
         self._validate_parameters()
 
     def _validate_parameters(self):
         """Assert the parameters are valid."""
         if self.precision not in [0.01, 0.025]:
             raise ValueError("The parameter precision must be 0.01 or 0.025")
-        if self.territory not in AVAILABLE_TERRITORY:
+        if self.territory not in AVAILABLE_AROME_TERRITORY:
             raise ValueError(
-                f"The parameter precision must be in {AVAILABLE_TERRITORY}"
+                f"The parameter precision must be in {AVAILABLE_AROME_TERRITORY}"
             )
 
     @property
     def entry_point(self):
         """The entry point to the AROME service."""
         return f"wcs/MF-NWP-HIGHRES-AROME-{precision_float_to_str[self.precision]}-{self.territory}-WCS"
 
@@ -143,17 +151,28 @@
         if self.data_capabilities is None:
             url = f"{self.base_url}/{self.entry_point_capabilities}"
             params = {
                 "service": "WCS",
                 "version": "2.0.1",
                 "language": "eng",
             }
-            response = self.session.get(url, params=params)
+            try :
+                response = self._get_request(url, params=params)
+            except MissingDataError as e:
+                logger.error(f"Error fetching the capabilities: {e}")
+                logging.error(f"URL: {url}")
+                logging.error(f"Params: {params}")
+                raise e
             xml = response.text
-            self.data_capabilities = xmltodict.parse(xml)
+            try:
+                self.data_capabilities = xmltodict.parse(xml)
+            except MissingDataError as e:
+                logger.error(f"Error parsing the XML response: {e}")
+                logger.error(f"Response: {xml}")
+                raise e
         return self.data_capabilities
 
     def get_capabilities(self):
         """Get the capabilities of the service.
         In particular, lists the available coverages IDs,
         that is a mandatory parameter for the get_coverage request."""
         list_capabilities = self.capabilities["wcs:Capabilities"]["wcs:Contents"]["wcs:CoverageSummary"]
@@ -283,7 +302,65 @@
             }
             response = self._get_request(url, params=params)
             # save res.text to tiff file
             filepath.parent.mkdir(parents=True, exist_ok=True)
             with open(filepath, "wb") as f:
                 f.write(response.content)
         return filepath
+
+
+class ArpegeForecast(AromeForecast):
+    api_version = "1.0"
+    base_url = "https://public-api.meteofrance.fr/public/arpege/" + api_version
+
+    def __init__(
+        self,
+        territory: str = "EUROPE",
+        api_key: str | None = None,
+        token: str | None = None,
+        application_id: str | None = None,
+        cache_dir: str | None = None,
+    ):
+        """Init the ArpegeForecast object.
+
+        Parameters
+        ----------
+        territory : str, optional
+            The ARPEGE territory to fetch, by default "FRANCE"
+        api_key : str | None, optional
+            The API Key, by default None
+        token : str | None, optional
+            The API Token, by default None
+        application_id : str | None, optional
+            The Application ID, by default None
+        cache_dir : str | None, optional
+            The path to the caching directory, by default None.
+            If None, the cache directory is set to "/tmp/cache".
+
+        Note
+        ----
+        See :class:`.MeteoFranceAPI` for the parameters `api_key`, `token` and `application_id`.
+
+        The available territories are listed in :data:`.AVAILABLE_TERRITORY`.
+
+        """
+        super(AromeForecast, self).__init__(api_key, token, application_id)
+        cache_dir = cache_dir or "/tmp/cache"
+        self.cache_dir = Path(cache_dir)
+        self.precision = RELATION_TERRITORY_TO_PREC_ARPEGE[territory]  # the precision of the ARPEGE model, in Degrees.
+        self.territory = territory  # the territory of the forecast.
+        self.data_capabilities = None
+        self.all_coverageid_prefix = None # the list of all coverage ID prefix
+        self.all_coverageid = None # the list of all coverage ID
+        self._validate_parameters()
+
+    def _validate_parameters(self):
+        """Assert the parameters are valid."""
+        if self.territory not in AVAILABLE_ARPEGE_TERRITORY:
+            raise ValueError(
+                f"The parameter precision must be in {AVAILABLE_ARPEGE_TERRITORY}"
+            )
+
+    @property
+    def entry_point(self):
+        """The entry point to the AROME service."""
+        return f"wcs/MF-NWP-GLOBAL-ARPEGE-{precision_float_to_str[self.precision]}-{self.territory}-WCS"
```

### Comparing `meteofrance-publicapi-0.1.3/meteofrance_publicapi/core.py` & `meteofrance_publicapi-0.1.4/meteofrance_publicapi/core.py`

 * *Files identical despite different names*

### Comparing `meteofrance-publicapi-0.1.3/meteofrance_publicapi/errors.py` & `meteofrance_publicapi-0.1.4/meteofrance_publicapi/errors.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,17 +8,20 @@
         description = data["am:fault"]["am:description"]
         self.message = f"{message}\n {description}"
         super().__init__(self.message)
 
 class MissingDataError(Exception):
     def __init__(self, text: str):
         #parse the error message with xmltodict
-        data = xmltodict.parse(text)
-        exception = data["mw:fault"]["mw:description"]["ns0:ExceptionReport"]["ns0:Exception"]
-        code = exception["@exceptionCode"]
-        locator = exception["@locator"]
-        text = exception["ns0:ExceptionText"]
-        message = (f"Error code: {code}\n"
-                   f"Locator: {locator}\n"
-                   f"Text: {text}")
+        try :
+            data = xmltodict.parse(text)
+            exception = data["mw:fault"]["mw:description"]["ns0:ExceptionReport"]["ns0:Exception"]
+            code = exception["@exceptionCode"]
+            locator = exception["@locator"]
+            text = exception["ns0:ExceptionText"]
+            message = (f"Error code: {code}\n"
+                    f"Locator: {locator}\n"
+                    f"Text: {text}")
+        except Exception as e:
+            message = text
         self.message = message
         super().__init__(self.message)
```

### Comparing `meteofrance-publicapi-0.1.3/meteofrance_publicapi/observations.py` & `meteofrance_publicapi-0.1.4/meteofrance_publicapi/observations.py`

 * *Files identical despite different names*

### Comparing `meteofrance-publicapi-0.1.3/meteofrance_publicapi/raster.py` & `meteofrance_publicapi-0.1.4/meteofrance_publicapi/raster.py`

 * *Files identical despite different names*

### Comparing `meteofrance-publicapi-0.1.3/meteofrance_publicapi.egg-info/PKG-INFO` & `meteofrance_publicapi-0.1.4/meteofrance_publicapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meteofrance-publicapi
-Version: 0.1.3
+Version: 0.1.4
 Summary: A wrapper of the portail-api.meteofrance.fr datasets
 Author: Antoine Tavant
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -792,13 +792,13 @@
 | 2099       | 98832005 | NaN       | OUINNE                  | -21.984000 | 166.680500 | 54             | 1974-01-01 | ETENDU |
 | 2100       | 98832006 | NaN       | RIVIERE BLANCHE         | -22.132667 | 166.726333 | 171            | 2000-11-01 | ETENDU |
 | 2101       | 98832101 | NaN       | GORO_ANCIENNE_PEPINIERE | -22.269167 | 166.967500 | 298            | 1995-01-01 | ETENDU |
 | 2102       | 98833002 | NaN       | MEA                     | -21.455500 | 165.767333 | 571            | 1988-01-01 | ETENDU |
 
 ### Accessing Arome Forecasts
 
-See the notebook [Arome Forecast](./examples/arome.ipynb) for examples of accessing the forecast of the Arome model.
+See the notebook [Arome Forecast](./doc/examples/arome.ipynb) for examples of accessing the forecast of the AROME model.
 
 # TODO
 
 - [ ] Add local cache capabilities, for instance with [joblib](https://joblib.readthedocs.io/en/stable/memory.html)
 - [ ] Add persistent storage, locally or with a could provider
```

### Comparing `meteofrance-publicapi-0.1.3/meteofrance_publicapi.egg-info/SOURCES.txt` & `meteofrance_publicapi-0.1.4/meteofrance_publicapi.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 LICENSE
 README.md
 pyproject.toml
 meteofrance_publicapi/__init__.py
-meteofrance_publicapi/arome.py
 meteofrance_publicapi/const.py
 meteofrance_publicapi/core.py
 meteofrance_publicapi/errors.py
+meteofrance_publicapi/forecast.py
 meteofrance_publicapi/observations.py
 meteofrance_publicapi/raster.py
 meteofrance_publicapi.egg-info/PKG-INFO
 meteofrance_publicapi.egg-info/SOURCES.txt
 meteofrance_publicapi.egg-info/dependency_links.txt
 meteofrance_publicapi.egg-info/not-zip-safe
 meteofrance_publicapi.egg-info/requires.txt
```

### Comparing `meteofrance-publicapi-0.1.3/pyproject.toml` & `meteofrance_publicapi-0.1.4/pyproject.toml`

 * *Files identical despite different names*


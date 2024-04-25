# Comparing `tmp/cwms-python-0.1.0.tar.gz` & `tmp/cwms_python-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cwms-python-0.1.0.tar", last modified: Mon Jan 22 22:01:02 2024, max compression
+gzip compressed data, was "cwms_python-0.3.0.tar", max compression
```

## Comparing `cwms-python-0.1.0.tar` & `cwms_python-0.3.0.tar`

### file list

```diff
@@ -1,36 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 22:01:02.958302 cwms-python-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 22:01:02.954302 cwms-python-0.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 22:01:02.954302 cwms-python-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3218 2024-01-22 22:00:53.000000 cwms-python-0.1.0/.github/workflows/publish-to-test-pypi.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 22:01:02.954302 cwms-python-0.1.0/CWMS/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 22:01:02.958302 cwms-python-0.1.0/CWMS/.ipynb_checkpoints/
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-01-22 22:00:53.000000 cwms-python-0.1.0/CWMS/.ipynb_checkpoints/__init__-checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-22 22:00:53.000000 cwms-python-0.1.0/CWMS/.ipynb_checkpoints/core-checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-01-22 22:00:53.000000 cwms-python-0.1.0/CWMS/.ipynb_checkpoints/cwms_loc-checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-01-22 22:00:53.000000 cwms-python-0.1.0/CWMS/.ipynb_checkpoints/cwms_ts-checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-01-22 22:00:53.000000 cwms-python-0.1.0/CWMS/.ipynb_checkpoints/utils-checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-01-22 22:00:53.000000 cwms-python-0.1.0/CWMS/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 22:01:02.958302 cwms-python-0.1.0/CWMS/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-01-22 22:00:53.000000 cwms-python-0.1.0/CWMS/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 runner    (1001) docker     (127)      952 2024-01-22 22:00:53.000000 cwms-python-0.1.0/CWMS/__pycache__/core.cpython-39.pyc
--rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-01-22 22:00:53.000000 cwms-python-0.1.0/CWMS/__pycache__/cwms_loc.cpython-39.pyc
--rw-r--r--   0 runner    (1001) docker     (127)     8012 2024-01-22 22:00:53.000000 cwms-python-0.1.0/CWMS/__pycache__/cwms_ts.cpython-39.pyc
--rw-r--r--   0 runner    (1001) docker     (127)     2487 2024-01-22 22:00:53.000000 cwms-python-0.1.0/CWMS/__pycache__/utils.cpython-39.pyc
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-01-22 22:00:53.000000 cwms-python-0.1.0/CWMS/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-01-22 22:00:53.000000 cwms-python-0.1.0/CWMS/cwms_loc.py
--rw-r--r--   0 runner    (1001) docker     (127)     9217 2024-01-22 22:00:53.000000 cwms-python-0.1.0/CWMS/cwms_ts.py
--rw-r--r--   0 runner    (1001) docker     (127)     2703 2024-01-22 22:00:53.000000 cwms-python-0.1.0/CWMS/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-01-22 22:00:53.000000 cwms-python-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1998 2024-01-22 22:01:02.958302 cwms-python-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-01-22 22:00:53.000000 cwms-python-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 22:01:02.958302 cwms-python-0.1.0/cwms_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1998 2024-01-22 22:01:02.000000 cwms-python-0.1.0/cwms_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-01-22 22:01:02.000000 cwms-python-0.1.0/cwms_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-22 22:01:02.000000 cwms-python-0.1.0/cwms_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-01-22 22:01:02.000000 cwms-python-0.1.0/cwms_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-01-22 22:01:02.000000 cwms-python-0.1.0/cwms_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-01-22 22:00:53.000000 cwms-python-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-22 22:01:02.958302 cwms-python-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-01-22 22:00:53.000000 cwms-python-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 22:01:02.958302 cwms-python-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-22 22:00:53.000000 cwms-python-0.1.0/tests/__init__.py
+-rw-r--r--   0        0        0     1086 2024-04-25 15:24:52.749728 cwms_python-0.3.0/LICENSE
+-rw-r--r--   0        0        0     1452 2024-04-25 15:24:52.749728 cwms_python-0.3.0/README.md
+-rw-r--r--   0        0        0      348 2024-04-25 15:24:52.749728 cwms_python-0.3.0/cwms/__init__.py
+-rw-r--r--   0        0        0      933 2024-04-25 15:24:52.749728 cwms_python-0.3.0/cwms/_constants.py
+-rw-r--r--   0        0        0     8875 2024-04-25 15:24:52.749728 cwms_python-0.3.0/cwms/api.py
+-rw-r--r--   0        0        0      926 2024-04-25 15:24:52.749728 cwms_python-0.3.0/cwms/core.py
+-rw-r--r--   0        0        0     3827 2024-04-25 15:24:52.749728 cwms_python-0.3.0/cwms/exceptions.py
+-rw-r--r--   0        0        0     8468 2024-04-25 15:24:52.749728 cwms_python-0.3.0/cwms/forecast/forecast_instance.py
+-rw-r--r--   0        0        0     7099 2024-04-25 15:24:52.749728 cwms_python-0.3.0/cwms/forecast/forecast_spec.py
+-rw-r--r--   0        0        0    17364 2024-04-25 15:24:52.749728 cwms_python-0.3.0/cwms/levels/location_levels.py
+-rw-r--r--   0        0        0     1453 2024-04-25 15:24:52.749728 cwms_python-0.3.0/cwms/locations/physical_locations.py
+-rw-r--r--   0        0        0     7978 2024-04-25 15:24:52.749728 cwms_python-0.3.0/cwms/timeseries/timeseries.py
+-rw-r--r--   0        0        0     6667 2024-04-25 15:24:52.749728 cwms_python-0.3.0/cwms/timeseries/timeseries_bin.py
+-rw-r--r--   0        0        0    11373 2024-04-25 15:24:52.749728 cwms_python-0.3.0/cwms/timeseries/timeseries_txt.py
+-rw-r--r--   0        0        0     1752 2024-04-25 15:24:52.749728 cwms_python-0.3.0/cwms/types.py
+-rw-r--r--   0        0        0     2258 2024-04-25 15:24:52.749728 cwms_python-0.3.0/cwms/utils.py
+-rw-r--r--   0        0        0      958 2024-04-25 15:24:52.753728 cwms_python-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2252 1970-01-01 00:00:00.000000 cwms_python-0.3.0/PKG-INFO
```

### Comparing `cwms-python-0.1.0/CWMS/cwms_ts.py` & `cwms_python-0.3.0/cwms/api.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,182 +1,294 @@
-from .utils import queryCDA
-import pandas as pd
+""" Session management and REST functions for CWMS Data API.
+
+This module provides functions for making REST calls to the CWMS Data API (CDA). These
+functions should be used internally to interact with the API. The user should not have to
+interact with these directly.
+
+The `init_session()` function can be used to specify an alternative root URL, and to
+provide an authentication key (if required). If `init_session()` is not called, the
+default root URL (see `API_ROOT` below) will be used, and no authentication keys will be
+included when making API calls.
+
+Example: Initializing a session
+
+    # Specify an alternate URL
+    init_session(api_root="https://example.com/cwms-data")
+
+    # Specify an alternate URL and an auth key
+    init_session(api_root="https://example.com/cwms-data", api_key="API_KEY")
+
+Functions which make API calls that _may_ return a JSON response will return a `dict`
+containing the deserialized data. If the API response does not include data, an empty
+`dict` will be returned.
+
+In the event the API returns an error response, the function will raise an `APIError`
+which includes the response object and provides some hints to the user on how to address
+the error.
+"""
+
 import json
+import logging
+from json import JSONDecodeError
+from typing import Optional, cast
+
+from requests import Response
+from requests_toolbelt import sessions  # type: ignore
+from requests_toolbelt.sessions import BaseUrlSession  # type: ignore
+
+from cwms.types import JSON, RequestParams
+
+# Specify the default API root URL and version.
+API_ROOT = "https://cwms-data.usace.army.mil/cwms-data/"
+API_VERSION = 2
+
+# Initialize a non-authenticated session with the default root URL.
+SESSION = sessions.BaseUrlSession(base_url=API_ROOT)
+
+
+class InvalidVersion(Exception):
+    pass
+
+
+class ApiError(Exception):
+    """CWMS Data Api Error.
+
+    This class is a light wrapper around a `requests.Response` object. Its primary purpose
+    is to generate an error message that includes the request URL and provide additional
+    information to the user to help them resolve the error.
+    """
+
+    def __init__(self, response: Response):
+        self.response = response
+
+    def __str__(self) -> str:
+        # Include the request URL in the error message.
+        message = f"CWMS API Error ({self.response.url})"
+
+        # If a reason is provided in the response, add it to the message.
+        if reason := self.response.reason:
+            message += f" {reason}"
+
+        message += "."
+
+        # Add additional context to help the user resolve the issue.
+        if hint := self.hint():
+            message += f" {hint}"
+
+        if content := self.response.content:
+            message += f" {content.decode('utf8')}"
+
+        return message
+
+    def hint(self) -> str:
+        """Return a message with additional information on how to resolve the error."""
+
+        if self.response.status_code == 400:
+            return "Check that your parameters are correct."
+        elif self.response.status_code == 404:
+            return "May be the result of an empty query."
+        else:
+            return ""
+
+
+def init_session(
+    *, api_root: Optional[str] = None, api_key: Optional[str] = None
+) -> BaseUrlSession:
+    """Specify a root URL and authentication key for the CWMS Data API.
+
+    This function can be used to change the root URL used when interacting with the CDA.
+    All API calls made after this function is called will use the specified URL. If an
+    authentication key is given it will be included in all future request headers.
+
+    Keyword Args:
+        api_root (optional): The root URL for the CWMS Data API.
+        api_key (optional): An authentication key.
+
+    Returns:
+        Returns the updated session object.
+    """
+
+    global SESSION
+
+    if api_root:
+        logging.debug(f"Initializing root URL: api_root={api_root}")
+        SESSION = sessions.BaseUrlSession(base_url=api_root)
+
+    if api_key:
+        logging.debug(f"Setting authorization key: api_key={api_key}")
+        SESSION.headers.update({"Authorization": api_key})
+
+    return SESSION
+
+
+def return_base_url() -> str:
+    """returns the base URL for the CDA instance that is connected to.
+
+    Returns:
+        str: base URL
+    """
+
+    return str(SESSION.base_url)
+
+
+def api_version_text(api_version: int) -> str:
+    """Initialize CDA request headers.
+
+    The CDA supports multiple versions. To request a specific version, the version number
+    must be included in the request headers.
+
+    Args:
+        api_version: The CDA version to use for the request.
+
+    Returns:
+        A dict containing the request headers.
+
+    Raises:
+        InvalidVersion: If an unsupported API version is specified.
+    """
+
+    if api_version == 1:
+        version = "application/json"
+    elif api_version == 2:
+        version = "application/json;version=2"
+    else:
+        raise InvalidVersion(f"API version {api_version} is not supported.")
+
+    return version
+
+
+def get(
+    endpoint: str,
+    params: Optional[RequestParams] = None,
+    *,
+    api_version: int = API_VERSION,
+) -> JSON:
+    """Make a GET request to the CWMS Data API.
+
+    Args:
+        endpoint: The CDA endpoint for the record(s).
+        params (optional): Query parameters for the request.
+
+    Keyword Args:
+        api_version (optional): The CDA version to use for the request. If not specified,
+            the default API_VERSION will be used.
+
+    Returns:
+        The deserialized JSON response data.
+
+    Raises:
+        ApiError: If an error response is return by the API.
+    """
+
+    headers = {"Accept": api_version_text(api_version)}
+    response = SESSION.get(endpoint, params=params, headers=headers)
+
+    if response.status_code != 200:
+        logging.error(f"CDA Error: response={response}")
+        raise ApiError(response)
+
+    try:
+        return cast(JSON, response.json())
+    except JSONDecodeError as error:
+        logging.error(f"Error decoding CDA response: {error}")
+        return {}
+
+
+def post(
+    endpoint: str,
+    data: JSON,
+    params: Optional[RequestParams] = None,
+    *,
+    api_version: int = API_VERSION,
+) -> None:
+    """Make a POST request to the CWMS Data API.
+
+    Args:
+        endpoint: The CDA endpoint for the record type.
+        data: A dict containing the new record data. Must be JSON-serializable.
+        params (optional): Query parameters for the request.
+
+    Keyword Args:
+        api_version (optional): The CDA version to use for the request. If not specified,
+            the default API_VERSION will be used.
+
+    Returns:
+        The deserialized JSON response data.
+
+    Raises:
+        ApiError: If an error response is return by the API.
+    """
+
+    # post requires different headers than get for
+    headers = {"accept": "*/*", "Content-Type": api_version_text(api_version)}
+
+    response = SESSION.post(
+        endpoint, params=params, headers=headers, data=json.dumps(data)
+    )
+
+    if response.status_code != 200:
+        logging.error(f"CDA Error: response={response}")
+        raise ApiError(response)
+
+
+def patch(
+    endpoint: str,
+    data: JSON,
+    params: Optional[RequestParams] = None,
+    *,
+    api_version: int = API_VERSION,
+) -> None:
+    """Make a PATCH request to the CWMS Data API.
+
+    Args:
+        endpoint: The CDA endpoint for the record.
+        data: A dict containing the updated record data. Must be JSON-serializable.
+        params (optional): Query parameters for the request.
+
+    Keyword Args:
+        api_version (optional): The CDA version to use for the request. If not specified,
+            the default API_VERSION will be used.
+
+    Returns:
+        The deserialized JSON response data.
+
+    Raises:
+        ApiError: If an error response is return by the API.
+    """
+
+    headers = {"accept": "*/*", "Content-Type": api_version_text(api_version)}
+
+    response = SESSION.patch(
+        endpoint, params=params, headers=headers, data=json.dumps(data)
+    )
+
+    if response.status_code != 200:
+        logging.error(f"CDA Error: response={response}")
+        raise ApiError(response)
+
+
+def delete(
+    endpoint: str,
+    params: Optional[RequestParams] = None,
+    *,
+    api_version: int = API_VERSION,
+) -> None:
+    """Make a DELETE request to the CWMS Data API.
+
+    Args:
+        endpoint: The CDA endpoint for the record.
+        params (optional): Query parameters for the request.
 
+    Keyword Args:
+        api_version (optional): The CDA version to use for the request. If not specified,
+            the default API_VERSION will be used.
 
-class CwmsTsMixin:
+    Raises:
+        ApiError: If an error response is return by the API.
+    """
 
-    def retreive_ts_group(self,p_group_id,p_category_id,p_office_id, return_type='df'):
-        """Retreives time series stored in the requested time series group
-        
-        Parameters
-        -------
-        p_group_id : str
-            Specifies the timeseries group whose data is to be included in the response (required)
-        p_category_id : str
-            Specifies the category containing the timeseries group whose data is to be included in the response. (required)
-        p_office_id : str
-            Specifies the owning office of the timeseries group whose data is to be included in the response. (required)
-        return_type : str
-            output type to return values as. 1. 'df' will return a pandas dataframe. 2. 'dict' will return a json decoded dictionay. 3. all other values will return Responce object from request package.
-        
-        Returns
-        -------
-        pandas df, json decoded dictionay, or Responce object from request package
-
-        Examples
-        -------
-        """
-        endPoint = f'timeseries/group/{p_group_id}'
-
-        params = {
-            "office": p_office_id,
-            "category-id": p_category_id
-        }
-
-        headerList={
-            "Accept": "application/json"
-        }
-
-        responce = queryCDA(self, endPoint, params, headerList, return_type, dict_key = ['assigned-time-series'])
-
-        #if dataframe:
-        #    responce = pd.DataFrame(responce['assigned-time-series'])
-
-        return responce
-
-    def retrieve_ts(self, p_tsId, p_office_id, p_unit='EN', p_datum=None, p_start_date=None, p_end_date=None, p_timezone=None, p_page_size=500000, return_type='df'):
-        """Retrieves time series data from a specified time series and time window.  Value date-times obtained are always in UTC.
-
-        Parameters
-        -----------
-        p_tsId : str (required)
-            Specifies the name(s) of the time series whose data is to be included in the response. A case insensitive comparison is used to match names.
-        p_office_id : str
-            Specifies the owning office of the time series(s) whose data is to be included in the response. If this field is not specified, matching location level information from all offices shall be returned.
-        p_unit : str
-            Specifies the unit or unit system of the response. Valid values for the unit field are: 1. EN. (default) Specifies English unit system. 2. SI.   Specifies the SI unit system. 3. Other. Any unit returned in the response to the units URI request that is appropriate for the requested parameters.
-        p_datum: str
-            Specifies the elevation datum of the response. This field affects only elevation location levels. Valid values for this field are:  1. NAVD88.  The elevation values will in the specified or default units above the NAVD-88 datum.  2. NGVD29.  The elevation values will be in the specified or default units above the NGVD-29 datum.
-        p_start_date : datetime
-            Specifies the start of the time window for data to be included in the response. If this field is not specified, any required time window begins 24 hours prior to the specified or default end time.
-        p_end_date : datetime
-            Specifies the end of the time window for data to be included in the response. If this field is not specified, any required time window ends at the current time.
-        p_timezone : string
-            Specifies the time zone of the values of the begin and end fields. UTC is the default.  This value does not impact the values in response.  response is always in UTC.  
-        return_type : str
-            output type to return values as. 1. 'df' will return a pandas dataframe. 2. 'dict' will return a json decoded dictionay. 3. all other values will return Responce object from request package.
-        Returns
-        --------
-        pandas df, json decoded dictionay, or Responce object from request package.  Dates in responce are in UTC.  
-
-        Examples
-        -------
-        """
-        #creates the dataframe from the timeseries data
-        endPoint = 'timeseries'
-        if p_start_date is not None: p_start_date = p_start_date.strftime('%Y-%m-%dT%H:%M:%S')
-
-        if p_end_date is not None: p_end_date = p_end_date.strftime('%Y-%m-%dT%H:%M:%S') 
-
-        params = {
-            "office": p_office_id,
-            "name": p_tsId,
-            "unit": p_unit,
-            "datum": p_datum,
-            "begin": p_start_date,
-            "end": p_end_date,
-            "timezone" : p_timezone,
-            "page-size" : p_page_size
-        }
-
-        headerList={
-            "Accept": "application/json;version=2"
-        }
-        responce = queryCDA(self,endPoint,params,headerList,return_type, dict_key = ['values'])
-
-        return responce
-
-    def write_ts(self, data, version_date = None, timezone = None, create_as_ltrs = False, store_rule = None, override_protection = None):
-        """Will Create new TimeSeries if not already present.  Will store any data provided.
-
-        Parameters
-        -------
-        data : pd.Dataframe, or Dictionay
-            Time Series data to be stored.  If dataframe data must be provided in the following format
-            df.tsId = timeseried id:specified name of the time series to be posted to
-            df.office = the owning office of the time series
-            df.units = units of values to be stored (ie. ft, in, m, cfs....)
-            dataframe should have three columns date-time, value, quality-code. date-time values can be a string in ISO8601 formate or a datetime field. 
-            if quality-code column is not present is will be set to 0.
-                                         date-time value  quality-code
-               0   2023-12-20T14:45:00.000-05:00  93.1           0
-               1   2023-12-20T15:00:00.000-05:00  99.8           0
-               2   2023-12-20T15:15:00.000-05:00  98.5           0
-               3   2023-12-20T15:30:00.000-05:00  98.5           0
-
-        version_date : str
-            Specifies the version date for the timeseries to create. If this field is not specified, a null version date will be used.  The format for this field is ISO 8601 extended, with optional timezone, i.e., 'format', e.g., '2021-06-10T13:00:00-0700[PST8PDT]'.
-        timezone : str
-            Specifies the time zone of the version-date field (unless otherwise specified). If this field is not specified, the default time zone of UTC shall be used.  Ignored if version-date was specified with offset and timezone.
-        create_as_lrts : bool
-            Flag indicating if timeseries should be created as Local Regular Time Series. 'True' or 'False', default is 'False'
-        store_rule : str
-            The business rule to use when merging the incoming with existing data. Available values : REPLACE_ALL, DO_NOT_REPLACE, REPLACE_MISSING_VALUES_ONLY, REPLACE_WITH_NON_MISSING, DELETE_INSERT
-        override_protection : bool
-            A flag to ignore the protected data quality when storing data. 'True' or 'False'
-
-        Returns
-        -------
-        Responce object from request package
-
-        Examples
-        -------
-        
-        """
-        endPoint = 'timeseries'
-        params = {
-                'version-date': version_date,
-                'timezone': timezone,
-                'create-as-lrts' : create_as_ltrs, 
-                'store-rule' : store_rule,
-                'override-protection' : override_protection
-            }
-        headerList={
-                'accept': '*/*',
-                'Content-Type': 'application/json;version=2',
-            }
-        if isinstance(data, pd.DataFrame):
-            #grab time series information
-            tsId = data.tsId
-            office = data.office
-            units = data.units
-
-            #check dataframe columns
-            if 'quality-code' not in data:
-                values['quality-code'] = 0
-            if 'date-time' not in data:
-                raise TypeError("date-time is a required column in data when posting as a dateframe")
-            if 'value' not in data:
-                raise TypeError("value is a required column when posting data when posting as a dataframe")
-                
-            #make sure that dataTime column is in iso8601 formate.      
-            data['date-time'] = pd.to_datetime(data['date-time']).apply(pd.Timestamp.isoformat)
-            data = data.reindex(columns=['date-time','value','quality-code'])
-            if data.isnull().values.any():
-                raise ValueError("Null/NaN data must be removed from the dataframe")
-                
-            ts_dict = {"name": tsId,
-                       "office-id": office,
-                       "units": units,
-                       "values": data.values.tolist()
-                       }  
-            
-        elif isinstance(data, dict): 
-            ts_dict = data
-
-        else: raise TypeError("data is not of type dataframe or dictionary")
-            
-        #print(ts_dict)
-        response = self.s.post(endPoint, headers = headerList, data = json.dumps(ts_dict))    
-        return response
+    headers = {"Accept": api_version_text(api_version)}
+    response = SESSION.delete(endpoint, params=params, headers=headers)
 
+    if response.status_code != 200:
+        logging.error(f"CDA Error: response={response}")
+        raise ApiError(response)
```


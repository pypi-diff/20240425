# Comparing `tmp/stac_fastapi_types-2.5.3.tar.gz` & `tmp/stac_fastapi_types-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stac_fastapi_types-2.5.3.tar", last modified: Mon Apr 22 17:12:19 2024, max compression
+gzip compressed data, was "stac_fastapi_types-2.5.4.tar", last modified: Wed Apr 24 16:03:51 2024, max compression
```

## Comparing `stac_fastapi_types-2.5.3.tar` & `stac_fastapi_types-2.5.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 17:12:19.691782 stac_fastapi_types-2.5.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-04-22 17:12:19.691782 stac_fastapi_types-2.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 17:12:04.000000 stac_fastapi_types-2.5.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-22 17:12:19.691782 stac_fastapi_types-2.5.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-04-22 17:12:04.000000 stac_fastapi_types-2.5.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 17:12:19.687782 stac_fastapi_types-2.5.3/stac_fastapi/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 17:12:19.691782 stac_fastapi_types-2.5.3/stac_fastapi/types/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-22 17:12:04.000000 stac_fastapi_types-2.5.3/stac_fastapi/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-04-22 17:12:04.000000 stac_fastapi_types-2.5.3/stac_fastapi/types/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-04-22 17:12:04.000000 stac_fastapi_types-2.5.3/stac_fastapi/types/conformance.py
--rw-r--r--   0 runner    (1001) docker     (127)    25413 2024-04-22 17:12:04.000000 stac_fastapi_types-2.5.3/stac_fastapi/types/core.py
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-22 17:12:04.000000 stac_fastapi_types-2.5.3/stac_fastapi/types/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-04-22 17:12:04.000000 stac_fastapi_types-2.5.3/stac_fastapi/types/extension.py
--rw-r--r--   0 runner    (1001) docker     (127)     3369 2024-04-22 17:12:04.000000 stac_fastapi_types-2.5.3/stac_fastapi/types/links.py
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-22 17:12:04.000000 stac_fastapi_types-2.5.3/stac_fastapi/types/requests.py
--rw-r--r--   0 runner    (1001) docker     (127)     3085 2024-04-22 17:12:04.000000 stac_fastapi_types-2.5.3/stac_fastapi/types/rfc3339.py
--rw-r--r--   0 runner    (1001) docker     (127)     6640 2024-04-22 17:12:04.000000 stac_fastapi_types-2.5.3/stac_fastapi/types/search.py
--rw-r--r--   0 runner    (1001) docker     (127)     2085 2024-04-22 17:12:04.000000 stac_fastapi_types-2.5.3/stac_fastapi/types/stac.py
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-22 17:12:04.000000 stac_fastapi_types-2.5.3/stac_fastapi/types/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 17:12:19.691782 stac_fastapi_types-2.5.3/stac_fastapi.types.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-04-22 17:12:19.000000 stac_fastapi_types-2.5.3/stac_fastapi.types.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      677 2024-04-22 17:12:19.000000 stac_fastapi_types-2.5.3/stac_fastapi.types.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 17:12:19.000000 stac_fastapi_types-2.5.3/stac_fastapi.types.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 17:12:19.000000 stac_fastapi_types-2.5.3/stac_fastapi.types.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-22 17:12:19.000000 stac_fastapi_types-2.5.3/stac_fastapi.types.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-22 17:12:19.000000 stac_fastapi_types-2.5.3/stac_fastapi.types.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 17:12:19.691782 stac_fastapi_types-2.5.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-22 17:12:04.000000 stac_fastapi_types-2.5.3/tests/test_limit.py
--rw-r--r--   0 runner    (1001) docker     (127)     3498 2024-04-22 17:12:04.000000 stac_fastapi_types-2.5.3/tests/test_rfc3339.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:03:51.424560 stac_fastapi_types-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-04-24 16:03:51.424560 stac_fastapi_types-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 16:03:38.000000 stac_fastapi_types-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-24 16:03:51.424560 stac_fastapi_types-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-04-24 16:03:38.000000 stac_fastapi_types-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:03:51.420560 stac_fastapi_types-2.5.4/stac_fastapi/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:03:51.424560 stac_fastapi_types-2.5.4/stac_fastapi/types/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-24 16:03:38.000000 stac_fastapi_types-2.5.4/stac_fastapi/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-04-24 16:03:38.000000 stac_fastapi_types-2.5.4/stac_fastapi/types/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-04-24 16:03:38.000000 stac_fastapi_types-2.5.4/stac_fastapi/types/conformance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25419 2024-04-24 16:03:38.000000 stac_fastapi_types-2.5.4/stac_fastapi/types/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-24 16:03:38.000000 stac_fastapi_types-2.5.4/stac_fastapi/types/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-04-24 16:03:38.000000 stac_fastapi_types-2.5.4/stac_fastapi/types/extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3369 2024-04-24 16:03:38.000000 stac_fastapi_types-2.5.4/stac_fastapi/types/links.py
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-24 16:03:38.000000 stac_fastapi_types-2.5.4/stac_fastapi/types/requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3728 2024-04-24 16:03:38.000000 stac_fastapi_types-2.5.4/stac_fastapi/types/rfc3339.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6640 2024-04-24 16:03:38.000000 stac_fastapi_types-2.5.4/stac_fastapi/types/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2085 2024-04-24 16:03:38.000000 stac_fastapi_types-2.5.4/stac_fastapi/types/stac.py
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-24 16:03:38.000000 stac_fastapi_types-2.5.4/stac_fastapi/types/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:03:51.424560 stac_fastapi_types-2.5.4/stac_fastapi.types.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-04-24 16:03:51.000000 stac_fastapi_types-2.5.4/stac_fastapi.types.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-04-24 16:03:51.000000 stac_fastapi_types-2.5.4/stac_fastapi.types.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 16:03:51.000000 stac_fastapi_types-2.5.4/stac_fastapi.types.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 16:03:51.000000 stac_fastapi_types-2.5.4/stac_fastapi.types.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-24 16:03:51.000000 stac_fastapi_types-2.5.4/stac_fastapi.types.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-24 16:03:51.000000 stac_fastapi_types-2.5.4/stac_fastapi.types.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:03:51.424560 stac_fastapi_types-2.5.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-24 16:03:38.000000 stac_fastapi_types-2.5.4/tests/test_limit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3665 2024-04-24 16:03:38.000000 stac_fastapi_types-2.5.4/tests/test_rfc3339.py
```

### Comparing `stac_fastapi_types-2.5.3/PKG-INFO` & `stac_fastapi_types-2.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stac-fastapi.types
-Version: 2.5.3
+Version: 2.5.4
 Summary: An implementation of STAC API based on the FastAPI framework.
 Home-page: https://github.com/stac-utils/stac-fastapi
 Author: Arturo Engineering
 Author-email: engineering@arturo.ai
 License: MIT
 Keywords: STAC FastAPI COG
 Classifier: Intended Audience :: Developers
```

### Comparing `stac_fastapi_types-2.5.3/setup.py` & `stac_fastapi_types-2.5.4/setup.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_types-2.5.3/stac_fastapi/types/config.py` & `stac_fastapi_types-2.5.4/stac_fastapi/types/config.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_types-2.5.3/stac_fastapi/types/conformance.py` & `stac_fastapi_types-2.5.4/stac_fastapi/types/conformance.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_types-2.5.3/stac_fastapi/types/core.py` & `stac_fastapi_types-2.5.4/stac_fastapi/types/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -105,18 +105,18 @@
 
     @abc.abstractmethod
     def update_collection(
         self, collection_id: str, collection: stac_types.Collection, **kwargs
     ) -> Optional[Union[stac_types.Collection, Response]]:
         """Perform a complete update on an existing collection.
 
-        Called with `PUT /collections/{collection_id}`. It is expected that this item
-        already exists.  The update should do a diff against the saved collection and
-        perform any necessary updates.  Partial updates are not supported by the
-        transactions extension.
+        Called with `PUT /collections/{collection_id}`. It is expected that this
+        collection already exists.  The update should do a diff against the saved
+        collection and perform any necessary updates.  Partial updates are not
+        supported by the transactions extension.
 
         Args:
             collection_id: id of the existing collection to be updated
             collection: the updated collection (must be complete)
 
         Returns:
             The updated collection.
```

### Comparing `stac_fastapi_types-2.5.3/stac_fastapi/types/errors.py` & `stac_fastapi_types-2.5.4/stac_fastapi/types/errors.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_types-2.5.3/stac_fastapi/types/extension.py` & `stac_fastapi_types-2.5.4/stac_fastapi/types/extension.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_types-2.5.3/stac_fastapi/types/links.py` & `stac_fastapi_types-2.5.4/stac_fastapi/types/links.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_types-2.5.3/stac_fastapi/types/rfc3339.py` & `stac_fastapi_types-2.5.4/stac_fastapi/types/rfc3339.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """rfc3339."""
 import re
 from datetime import datetime, timezone
 from typing import Optional, Tuple, Union
 
 import iso8601
+from fastapi import HTTPException
 from pystac.utils import datetime_to_str
 
 RFC33339_PATTERN = (
     r"^(\d\d\d\d)\-(\d\d)\-(\d\d)(T|t)(\d\d):(\d\d):(\d\d)([.]\d+)?"
     r"(Z|([-+])(\d\d):(\d\d))$"
 )
 
@@ -41,61 +42,82 @@
     if not result:
         raise ValueError("Invalid RFC3339 datetime.")
 
     # Parse with pyiso8601
     return iso8601.parse_date(s)
 
 
-def str_to_interval(interval: Optional[str]) -> Optional[DateTimeType]:
-    """Extract a tuple of datetimes from an interval string.
+def parse_single_date(date_str: str) -> datetime:
+    """
+    Parse a single RFC3339 date string into a datetime object.
+
+    Args:
+        date_str (str): A string representing the date in RFC3339 format.
+
+    Returns:
+        datetime: A datetime object parsed from the date_str.
+
+    Raises:
+        ValueError: If the date_str is empty or contains the placeholder '..'.
+    """
+    if ".." in date_str or not date_str:
+        raise ValueError("Invalid date format.")
+    return rfc3339_str_to_datetime(date_str)
+
 
-    Interval strings are defined by
-    OGC API - Features Part 1 for the datetime query parameter value. These follow the
-    form '1985-04-12T23:20:50.52Z/1986-04-12T23:20:50.52Z', and allow either the start
-    or end (but not both) to be open-ended with '..' or ''.
+def str_to_interval(interval: Optional[str]) -> Optional[DateTimeType]:
+    """
+    Extract a tuple of datetime objects from an interval string defined by the OGC API.
+    The interval can either be a single datetime or a range with start and end datetime.
 
     Args:
-        interval (str or None): The interval string to convert to a tuple of
-        datetime.datetime objects, or None if no datetime is specified.
+        interval (Optional[str]): The interval string to convert to datetime objects,
+        or None if no datetime is specified.
 
     Returns:
-        Optional[DateTimeType]: A tuple of datetime.datetime objects or None if
-        input is None.
+        Optional[DateTimeType]: A tuple of datetime.datetime objects or
+        None if input is None.
 
     Raises:
-        ValueError: If the string is not a valid interval string and not None.
+        HTTPException: If the string is not valid for various reasons such as being empty,
+        having more than one slash, or if date formats are invalid.
     """
     if interval is None:
         return None
 
     if not interval:
-        raise ValueError("Empty interval string is invalid.")
+        raise HTTPException(status_code=400, detail="Empty interval string is invalid.")
 
     values = interval.split("/")
-    if len(values) == 1:
-        # Single date for == date case
-        return rfc3339_str_to_datetime(values[0])
-    elif len(values) > 2:
-        raise ValueError(
-            f"Interval string '{interval}' contains more than one forward slash."
+    if len(values) > 2:
+        raise HTTPException(
+            status_code=400,
+            detail="Interval string contains more than one forward slash.",
         )
 
-    start = None
-    end = None
-    if values[0] not in ["..", ""]:
-        start = rfc3339_str_to_datetime(values[0])
-    if values[1] not in ["..", ""]:
-        end = rfc3339_str_to_datetime(values[1])
+    try:
+        start = parse_single_date(values[0]) if values[0] not in ["..", ""] else None
+        end = (
+            parse_single_date(values[1])
+            if len(values) > 1 and values[1] not in ["..", ""]
+            else None
+        )
+    except (ValueError, iso8601.ParseError) as e:
+        raise HTTPException(status_code=400, detail=str(e))
 
     if start is None and end is None:
-        raise ValueError("Double open-ended intervals are not allowed.")
+        raise HTTPException(
+            status_code=400, detail="Double open-ended intervals are not allowed."
+        )
     if start is not None and end is not None and start > end:
-        raise ValueError("Start datetime cannot be before end datetime.")
-    else:
-        return start, end
+        raise HTTPException(
+            status_code=400, detail="Start datetime cannot be before end datetime."
+        )
+
+    return start, end
 
 
 def now_in_utc() -> datetime:
     """Return a datetime value of now with the UTC timezone applied."""
     return datetime.now(timezone.utc)
```

### Comparing `stac_fastapi_types-2.5.3/stac_fastapi/types/search.py` & `stac_fastapi_types-2.5.4/stac_fastapi/types/search.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_types-2.5.3/stac_fastapi/types/stac.py` & `stac_fastapi_types-2.5.4/stac_fastapi/types/stac.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_types-2.5.3/stac_fastapi.types.egg-info/PKG-INFO` & `stac_fastapi_types-2.5.4/stac_fastapi.types.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stac-fastapi.types
-Version: 2.5.3
+Version: 2.5.4
 Summary: An implementation of STAC API based on the FastAPI framework.
 Home-page: https://github.com/stac-utils/stac-fastapi
 Author: Arturo Engineering
 Author-email: engineering@arturo.ai
 License: MIT
 Keywords: STAC FastAPI COG
 Classifier: Intended Audience :: Developers
```

### Comparing `stac_fastapi_types-2.5.3/stac_fastapi.types.egg-info/SOURCES.txt` & `stac_fastapi_types-2.5.4/stac_fastapi.types.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `stac_fastapi_types-2.5.3/tests/test_limit.py` & `stac_fastapi_types-2.5.4/tests/test_limit.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_types-2.5.3/tests/test_rfc3339.py` & `stac_fastapi_types-2.5.4/tests/test_rfc3339.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from datetime import timezone
 
 import pytest
+from fastapi import HTTPException
 
 from stac_fastapi.types.rfc3339 import (
     now_in_utc,
     now_to_rfc3339_str,
     rfc3339_str_to_datetime,
     str_to_interval,
 )
@@ -82,16 +83,19 @@
 @pytest.mark.parametrize("test_input", valid_datetimes)
 def test_parse_valid_str_to_datetime(test_input):
     assert rfc3339_str_to_datetime(test_input)
 
 
 @pytest.mark.parametrize("test_input", invalid_intervals)
 def test_parse_invalid_interval_to_datetime(test_input):
-    with pytest.raises(ValueError):
+    with pytest.raises(HTTPException) as exc_info:
         str_to_interval(test_input)
+    assert (
+        exc_info.value.status_code == 400
+    ), "Should return a 400 status code for invalid intervals"
 
 
 @pytest.mark.parametrize("test_input", valid_intervals)
 def test_parse_valid_interval_to_datetime(test_input):
     assert str_to_interval(test_input)
```


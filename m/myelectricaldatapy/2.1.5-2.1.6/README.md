# Comparing `tmp/myelectricaldatapy-2.1.5.tar.gz` & `tmp/myelectricaldatapy-2.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myelectricaldatapy-2.1.5.tar", last modified: Sat Apr 20 09:11:54 2024, max compression
+gzip compressed data, was "myelectricaldatapy-2.1.6.tar", last modified: Thu Apr 25 06:55:43 2024, max compression
```

## Comparing `myelectricaldatapy-2.1.5.tar` & `myelectricaldatapy-2.1.6.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 09:11:54.660608 myelectricaldatapy-2.1.5/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-20 09:11:42.000000 myelectricaldatapy-2.1.5/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 09:11:54.656608 myelectricaldatapy-2.1.5/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-20 09:11:42.000000 myelectricaldatapy-2.1.5/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 09:11:54.656608 myelectricaldatapy-2.1.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      909 2024-04-20 09:11:42.000000 myelectricaldatapy-2.1.5/.github/workflows/dependbot-auto-approve.yml
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-20 09:11:42.000000 myelectricaldatapy-2.1.5/.github/workflows/lint.yml
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-20 09:11:42.000000 myelectricaldatapy-2.1.5/.github/workflows/pythonpublish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-20 09:11:42.000000 myelectricaldatapy-2.1.5/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-04-20 09:11:42.000000 myelectricaldatapy-2.1.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-04-20 09:11:42.000000 myelectricaldatapy-2.1.5/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 09:11:54.656608 myelectricaldatapy-2.1.5/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-20 09:11:42.000000 myelectricaldatapy-2.1.5/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-20 09:11:42.000000 myelectricaldatapy-2.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-20 09:11:42.000000 myelectricaldatapy-2.1.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3857 2024-04-20 09:11:54.660608 myelectricaldatapy-2.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-04-20 09:11:42.000000 myelectricaldatapy-2.1.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-04-20 09:11:42.000000 myelectricaldatapy-2.1.5/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 09:11:54.656608 myelectricaldatapy-2.1.5/myelectricaldatapy/
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-20 09:11:42.000000 myelectricaldatapy-2.1.5/myelectricaldatapy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5767 2024-04-20 09:11:42.000000 myelectricaldatapy-2.1.5/myelectricaldatapy/analytics.py
--rw-r--r--   0 runner    (1001) docker     (127)     2690 2024-04-20 09:11:42.000000 myelectricaldatapy-2.1.5/myelectricaldatapy/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-20 09:11:42.000000 myelectricaldatapy-2.1.5/myelectricaldatapy/const.py
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-20 09:11:42.000000 myelectricaldatapy-2.1.5/myelectricaldatapy/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6972 2024-04-20 09:11:42.000000 myelectricaldatapy-2.1.5/myelectricaldatapy/myelectricaldata.py
--rw-r--r--   0 runner    (1001) docker     (127)    11526 2024-04-20 09:11:42.000000 myelectricaldatapy-2.1.5/myelectricaldatapy/mypdl.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 09:11:42.000000 myelectricaldatapy-2.1.5/myelectricaldatapy/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 09:11:54.660608 myelectricaldatapy-2.1.5/myelectricaldatapy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3857 2024-04-20 09:11:54.000000 myelectricaldatapy-2.1.5/myelectricaldatapy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-20 09:11:54.000000 myelectricaldatapy-2.1.5/myelectricaldatapy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 09:11:54.000000 myelectricaldatapy-2.1.5/myelectricaldatapy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-20 09:11:54.000000 myelectricaldatapy-2.1.5/myelectricaldatapy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-20 09:11:54.000000 myelectricaldatapy-2.1.5/myelectricaldatapy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-04-20 09:11:42.000000 myelectricaldatapy-2.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-20 09:11:42.000000 myelectricaldatapy-2.1.5/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-20 09:11:42.000000 myelectricaldatapy-2.1.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 09:11:54.660608 myelectricaldatapy-2.1.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 09:11:54.660608 myelectricaldatapy-2.1.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 09:11:42.000000 myelectricaldatapy-2.1.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-04-20 09:11:42.000000 myelectricaldatapy-2.1.5/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    52826 2024-04-20 09:11:42.000000 myelectricaldatapy-2.1.5/tests/consts.py
--rw-r--r--   0 runner    (1001) docker     (127)    10665 2024-04-20 09:11:42.000000 myelectricaldatapy-2.1.5/tests/test_analytics.py
--rw-r--r--   0 runner    (1001) docker     (127)     5142 2024-04-20 09:11:42.000000 myelectricaldatapy-2.1.5/tests/test_load_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:55:43.119400 myelectricaldatapy-2.1.6/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-25 06:55:29.000000 myelectricaldatapy-2.1.6/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:55:43.115400 myelectricaldatapy-2.1.6/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-25 06:55:29.000000 myelectricaldatapy-2.1.6/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:55:43.115400 myelectricaldatapy-2.1.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      909 2024-04-25 06:55:29.000000 myelectricaldatapy-2.1.6/.github/workflows/dependbot-auto-approve.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-25 06:55:29.000000 myelectricaldatapy-2.1.6/.github/workflows/lint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-25 06:55:29.000000 myelectricaldatapy-2.1.6/.github/workflows/pythonpublish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-25 06:55:29.000000 myelectricaldatapy-2.1.6/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-04-25 06:55:29.000000 myelectricaldatapy-2.1.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-04-25 06:55:29.000000 myelectricaldatapy-2.1.6/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:55:43.115400 myelectricaldatapy-2.1.6/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-25 06:55:29.000000 myelectricaldatapy-2.1.6/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-25 06:55:29.000000 myelectricaldatapy-2.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-25 06:55:29.000000 myelectricaldatapy-2.1.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3857 2024-04-25 06:55:43.119400 myelectricaldatapy-2.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-04-25 06:55:29.000000 myelectricaldatapy-2.1.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-04-25 06:55:29.000000 myelectricaldatapy-2.1.6/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:55:43.115400 myelectricaldatapy-2.1.6/myelectricaldatapy/
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-25 06:55:29.000000 myelectricaldatapy-2.1.6/myelectricaldatapy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5767 2024-04-25 06:55:29.000000 myelectricaldatapy-2.1.6/myelectricaldatapy/analytics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2690 2024-04-25 06:55:29.000000 myelectricaldatapy-2.1.6/myelectricaldatapy/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-25 06:55:29.000000 myelectricaldatapy-2.1.6/myelectricaldatapy/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-25 06:55:29.000000 myelectricaldatapy-2.1.6/myelectricaldatapy/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8727 2024-04-25 06:55:29.000000 myelectricaldatapy-2.1.6/myelectricaldatapy/myelectricaldata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11526 2024-04-25 06:55:29.000000 myelectricaldatapy-2.1.6/myelectricaldatapy/mypdl.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 06:55:29.000000 myelectricaldatapy-2.1.6/myelectricaldatapy/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:55:43.115400 myelectricaldatapy-2.1.6/myelectricaldatapy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3857 2024-04-25 06:55:43.000000 myelectricaldatapy-2.1.6/myelectricaldatapy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-25 06:55:43.000000 myelectricaldatapy-2.1.6/myelectricaldatapy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 06:55:43.000000 myelectricaldatapy-2.1.6/myelectricaldatapy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-25 06:55:43.000000 myelectricaldatapy-2.1.6/myelectricaldatapy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-25 06:55:43.000000 myelectricaldatapy-2.1.6/myelectricaldatapy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-04-25 06:55:29.000000 myelectricaldatapy-2.1.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-25 06:55:29.000000 myelectricaldatapy-2.1.6/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-25 06:55:29.000000 myelectricaldatapy-2.1.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 06:55:43.119400 myelectricaldatapy-2.1.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 06:55:43.115400 myelectricaldatapy-2.1.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 06:55:29.000000 myelectricaldatapy-2.1.6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-04-25 06:55:29.000000 myelectricaldatapy-2.1.6/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52826 2024-04-25 06:55:29.000000 myelectricaldatapy-2.1.6/tests/consts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10665 2024-04-25 06:55:29.000000 myelectricaldatapy-2.1.6/tests/test_analytics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5142 2024-04-25 06:55:29.000000 myelectricaldatapy-2.1.6/tests/test_load_data.py
```

### Comparing `myelectricaldatapy-2.1.5/.github/dependabot.yml` & `myelectricaldatapy-2.1.6/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-2.1.5/.github/workflows/dependbot-auto-approve.yml` & `myelectricaldatapy-2.1.6/.github/workflows/dependbot-auto-approve.yml`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-2.1.5/.github/workflows/lint.yml` & `myelectricaldatapy-2.1.6/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-2.1.5/.github/workflows/pythonpublish.yml` & `myelectricaldatapy-2.1.6/.github/workflows/pythonpublish.yml`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-2.1.5/.github/workflows/release.yml` & `myelectricaldatapy-2.1.6/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-2.1.5/.gitignore` & `myelectricaldatapy-2.1.6/.gitignore`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-2.1.5/.pre-commit-config.yaml` & `myelectricaldatapy-2.1.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-2.1.5/LICENSE` & `myelectricaldatapy-2.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-2.1.5/PKG-INFO` & `myelectricaldatapy-2.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myelectricaldatapy
-Version: 2.1.5
+Version: 2.1.6
 Summary: Fetch Linky data from myelectricaldata.fr
 Author-email: Cyr-ius <cyr-ius@ipocus.net>
 License: GPL-3
 Keywords: enedis,linky,async,myelectricaldata
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `myelectricaldatapy-2.1.5/README.md` & `myelectricaldatapy-2.1.6/README.md`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-2.1.5/example.py` & `myelectricaldatapy-2.1.6/example.py`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-2.1.5/myelectricaldatapy/analytics.py` & `myelectricaldatapy-2.1.6/myelectricaldatapy/analytics.py`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-2.1.5/myelectricaldatapy/auth.py` & `myelectricaldatapy-2.1.6/myelectricaldatapy/auth.py`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-2.1.5/myelectricaldatapy/myelectricaldata.py` & `myelectricaldatapy-2.1.6/myelectricaldatapy/myelectricaldata.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 """Class for Enedis Gateway (http://www.myelectricaldata.fr)."""
 
 from __future__ import annotations
 
+from datetime import date, datetime as dt, timedelta
 import logging
 import re
-from datetime import date
-from datetime import datetime as dt
-from datetime import timedelta
 from types import TracebackType
-from typing import Any
+from typing import Any, Generator, cast
 
 from .auth import EnedisAuth
 from .const import DAILY_CONSUM, DAILY_PROD, DETAIL_CONSUM, DETAIL_PROD, TIMEOUT
 
 _LOGGER = logging.getLogger(__name__)
 
 
@@ -148,19 +146,55 @@
 
     async def async_get_daily_production(self, pdl: str, start: dt, end: dt) -> Any:
         """Get daily production."""
         return await self.async_fetch_datas(DAILY_PROD, pdl, start, end)
 
     async def async_get_details_consumption(self, pdl: str, start: dt, end: dt) -> Any:
         """Get consumption details. (max: 7 days)."""
-        return await self.async_fetch_datas(DETAIL_CONSUM, pdl, start, end)
+        data = None
+        for interval in list(self.date_range(start, end, 7)):
+            start, end = interval
+            try:
+                rsp = await self.async_fetch_datas(DETAIL_CONSUM, pdl, start, end)
+            finally:
+                if (
+                    rsp is None
+                    or rsp.get("meter_reading", {}).get("interval_reading") is None
+                ):
+                    continue
+                elif data is None:
+                    data = cast(dict[str, Any], rsp)
+                else:
+                    data["meter_reading"]["interval_reading"].extend(
+                        rsp.get("meter_reading", {}).get("interval_reading")
+                    )
+
+        return data
 
     async def async_get_details_production(self, pdl: str, start: dt, end: dt) -> Any:
         """Get production details. (max: 7 days)."""
-        return await self.async_fetch_datas(DETAIL_PROD, pdl, start, end)
+        data = None
+        for interval in list(self.date_range(start, end, 7)):
+            start, end = interval
+            try:
+                rsp = await self.async_fetch_datas(DETAIL_PROD, pdl, start, end)
+            finally:
+                if (
+                    rsp is None
+                    or rsp.get("meter_reading", {}).get("interval_reading") is None
+                ):
+                    continue
+                elif data is None:
+                    data = cast(dict[str, Any], rsp)
+                else:
+                    data["meter_reading"]["interval_reading"].extend(
+                        rsp.get("meter_reading", {}).get("interval_reading")
+                    )
+
+        return data
 
     async def async_get_max_power(self, pdl: str, start: dt, end: dt) -> Any:
         """Get consumption max power."""
         return await self.async_fetch_datas(
             "daily_consumption_max_power", pdl, start, end
         )
 
@@ -176,7 +210,20 @@
     ) -> None:
         """Asynchronous exit."""
         await self.close()
 
     async def close(self) -> None:
         """Close the session."""
         await self.auth.async_close()
+
+    @staticmethod
+    def date_range(start: dt, end: dt, intv: int) -> Generator[tuple[dt, dt], dt, None]:
+        """Return range by interval date."""
+        diff = (
+            (end - start).days // intv
+            if (end - start).days % intv == 0
+            else ((end - start).days // intv) + 1
+        )
+        for i in range(1, diff):
+            yield (start, start + timedelta(days=intv))
+            start = start + timedelta(days=(intv + 1))
+        yield (start, end)
```

### Comparing `myelectricaldatapy-2.1.5/myelectricaldatapy/mypdl.py` & `myelectricaldatapy-2.1.6/myelectricaldatapy/mypdl.py`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-2.1.5/myelectricaldatapy.egg-info/PKG-INFO` & `myelectricaldatapy-2.1.6/myelectricaldatapy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myelectricaldatapy
-Version: 2.1.5
+Version: 2.1.6
 Summary: Fetch Linky data from myelectricaldata.fr
 Author-email: Cyr-ius <cyr-ius@ipocus.net>
 License: GPL-3
 Keywords: enedis,linky,async,myelectricaldata
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `myelectricaldatapy-2.1.5/myelectricaldatapy.egg-info/SOURCES.txt` & `myelectricaldatapy-2.1.6/myelectricaldatapy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-2.1.5/pyproject.toml` & `myelectricaldatapy-2.1.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-2.1.5/tests/conftest.py` & `myelectricaldatapy-2.1.6/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-2.1.5/tests/consts.py` & `myelectricaldatapy-2.1.6/tests/consts.py`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-2.1.5/tests/test_analytics.py` & `myelectricaldatapy-2.1.6/tests/test_analytics.py`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-2.1.5/tests/test_load_data.py` & `myelectricaldatapy-2.1.6/tests/test_load_data.py`

 * *Files identical despite different names*


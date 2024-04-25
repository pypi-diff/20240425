# Comparing `tmp/idos_scraper-0.2.3.tar.gz` & `tmp/idos_scraper-0.2.4.tar.gz`

## Comparing `idos_scraper-0.2.3.tar` & `idos_scraper-0.2.4.tar`

### file list

```diff
@@ -1,19 +1,20 @@
--rw-r--r--   0        0        0    16010 2020-02-02 00:00:00.000000 idos_scraper-0.2.3/resources/paging-response-jQuery.html
--rw-r--r--   0        0        0   150339 2020-02-02 00:00:00.000000 idos_scraper-0.2.3/resources/response.html
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 idos_scraper-0.2.3/src/idos_scraper/__init__.py
--rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 idos_scraper-0.2.3/src/idos_scraper/log.py
--rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 idos_scraper-0.2.3/src/idos_scraper/examples/async_search_and_page_connection.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 idos_scraper-0.2.3/src/idos_scraper/examples/search_and_page_connection.py
--rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 idos_scraper-0.2.3/src/idos_scraper/examples/ui_search_station.py
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 idos_scraper-0.2.3/src/idos_scraper/scrapers/__init__.py
--rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 idos_scraper-0.2.3/src/idos_scraper/scrapers/async_page_connections.py
--rw-r--r--   0        0        0     2499 2020-02-02 00:00:00.000000 idos_scraper-0.2.3/src/idos_scraper/scrapers/async_search_connections.py
--rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 idos_scraper-0.2.3/src/idos_scraper/scrapers/async_search_station.py
--rw-r--r--   0        0        0     2537 2020-02-02 00:00:00.000000 idos_scraper-0.2.3/src/idos_scraper/scrapers/page_connections.py
--rw-r--r--   0        0        0     9287 2020-02-02 00:00:00.000000 idos_scraper-0.2.3/src/idos_scraper/scrapers/search_connections.py
--rw-r--r--   0        0        0     4516 2020-02-02 00:00:00.000000 idos_scraper-0.2.3/src/idos_scraper/scrapers/search_station.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 idos_scraper-0.2.3/.gitignore
--rw-r--r--   0        0        0     1214 2020-02-02 00:00:00.000000 idos_scraper-0.2.3/LICENSE
--rw-r--r--   0        0        0     1957 2020-02-02 00:00:00.000000 idos_scraper-0.2.3/README.md
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 idos_scraper-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     2687 2020-02-02 00:00:00.000000 idos_scraper-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 idos_scraper-0.2.4/.vscode/launch.json
+-rw-r--r--   0        0        0    16010 2020-02-02 00:00:00.000000 idos_scraper-0.2.4/resources/paging-response-jQuery.html
+-rw-r--r--   0        0        0   150339 2020-02-02 00:00:00.000000 idos_scraper-0.2.4/resources/response.html
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 idos_scraper-0.2.4/src/idos_scraper/__init__.py
+-rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 idos_scraper-0.2.4/src/idos_scraper/log.py
+-rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 idos_scraper-0.2.4/src/idos_scraper/examples/async_search_and_page_connection.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 idos_scraper-0.2.4/src/idos_scraper/examples/search_and_page_connection.py
+-rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 idos_scraper-0.2.4/src/idos_scraper/examples/ui_search_station.py
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 idos_scraper-0.2.4/src/idos_scraper/scrapers/__init__.py
+-rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 idos_scraper-0.2.4/src/idos_scraper/scrapers/async_page_connections.py
+-rw-r--r--   0        0        0     2658 2020-02-02 00:00:00.000000 idos_scraper-0.2.4/src/idos_scraper/scrapers/async_search_connections.py
+-rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 idos_scraper-0.2.4/src/idos_scraper/scrapers/async_search_station.py
+-rw-r--r--   0        0        0     2537 2020-02-02 00:00:00.000000 idos_scraper-0.2.4/src/idos_scraper/scrapers/page_connections.py
+-rw-r--r--   0        0        0    10035 2020-02-02 00:00:00.000000 idos_scraper-0.2.4/src/idos_scraper/scrapers/search_connections.py
+-rw-r--r--   0        0        0     4516 2020-02-02 00:00:00.000000 idos_scraper-0.2.4/src/idos_scraper/scrapers/search_station.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 idos_scraper-0.2.4/.gitignore
+-rw-r--r--   0        0        0     1214 2020-02-02 00:00:00.000000 idos_scraper-0.2.4/LICENSE
+-rw-r--r--   0        0        0     1957 2020-02-02 00:00:00.000000 idos_scraper-0.2.4/README.md
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 idos_scraper-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     2687 2020-02-02 00:00:00.000000 idos_scraper-0.2.4/PKG-INFO
```

### Comparing `idos_scraper-0.2.3/resources/paging-response-jQuery.html` & `idos_scraper-0.2.4/resources/paging-response-jQuery.html`

 * *Files identical despite different names*

### Comparing `idos_scraper-0.2.3/resources/response.html` & `idos_scraper-0.2.4/resources/response.html`

 * *Files identical despite different names*

### Comparing `idos_scraper-0.2.3/src/idos_scraper/log.py` & `idos_scraper-0.2.4/src/idos_scraper/log.py`

 * *Files identical despite different names*

### Comparing `idos_scraper-0.2.3/src/idos_scraper/examples/async_search_and_page_connection.py` & `idos_scraper-0.2.4/src/idos_scraper/examples/async_search_and_page_connection.py`

 * *Files identical despite different names*

### Comparing `idos_scraper-0.2.3/src/idos_scraper/examples/search_and_page_connection.py` & `idos_scraper-0.2.4/src/idos_scraper/examples/search_and_page_connection.py`

 * *Files identical despite different names*

### Comparing `idos_scraper-0.2.3/src/idos_scraper/examples/ui_search_station.py` & `idos_scraper-0.2.4/src/idos_scraper/examples/ui_search_station.py`

 * *Files identical despite different names*

### Comparing `idos_scraper-0.2.3/src/idos_scraper/scrapers/async_page_connections.py` & `idos_scraper-0.2.4/src/idos_scraper/scrapers/async_page_connections.py`

 * *Files identical despite different names*

### Comparing `idos_scraper-0.2.3/src/idos_scraper/scrapers/async_search_connections.py` & `idos_scraper-0.2.4/src/idos_scraper/scrapers/async_search_connections.py`

 * *Files 10% similar despite different names*

```diff
@@ -45,12 +45,16 @@
         async with session.get(url) as resp:
             response_text = await resp.text()
         await session.close()
     else:
         async with session.get(url) as resp:
             response_text = await resp.text()
 
-    p = ParseConnections(response_text)
+    try:
+        p = ParseConnections(response_text)
+    except Exception as e:
+        logger.error("Unable to parse connections")
+        raise e # TODO: Create empty structure with dummy data
 
     logger.debug(p)
 
     return p
```

### Comparing `idos_scraper-0.2.3/src/idos_scraper/scrapers/async_search_station.py` & `idos_scraper-0.2.4/src/idos_scraper/scrapers/async_search_station.py`

 * *Files identical despite different names*

### Comparing `idos_scraper-0.2.3/src/idos_scraper/scrapers/page_connections.py` & `idos_scraper-0.2.4/src/idos_scraper/scrapers/page_connections.py`

 * *Files identical despite different names*

### Comparing `idos_scraper-0.2.3/src/idos_scraper/scrapers/search_connections.py` & `idos_scraper-0.2.4/src/idos_scraper/scrapers/search_connections.py`

 * *Files 3% similar despite different names*

```diff
@@ -150,34 +150,50 @@
 
         conn["id"] = re_id_match.group(1)
 
         for html_single in html_single_connections:
             conn_single = {}
 
             # Fill delay
-            conn_single["delay"] = ParseDelay(html_single)
+            try:
+                conn_single["delay"] = ParseDelay(html_single)
+            except Exception as e:
+                logger.error("Unable to parse time delay")
+                raise e
 
             # Fill icon
-            conn_single["icon"] = ParseIcon(html_single)
+            try:
+                conn_single["icon"] = ParseIcon(html_single)
+            except Exception as e:
+                logger.error("Unable to parse icon")
+                raise e
 
             # Fill connection type and number
             # conn_single["type"] = ""
             # conn_single["number"] = ""
-            conn_single.update(ParseTypeAndNumber(html_single))
-            logger.debug(f"\tA {conn_single['type']} {conn_single['number']}:")
+            try:
+                conn_single.update(ParseTypeAndNumber(html_single))
+                logger.debug(f"\tA {conn_single['type']} {conn_single['number']}:")
+            except Exception as e:
+                logger.error("Unable to parse type and number")
+                raise e
 
             # Fill stations and departure/arrival times
             # conn_single["times"] = list()
             # conn_single["stations"] = list()
             # conn_single["platforms"] = list()
-            conn_single.update(ParseSingleConnectionDetail(html_single))
-            logger.debug(
-                f"\t\tDeparture at {conn_single['times'][0]} from {conn_single['stations'][0]}."
-                f" Arrival at {conn_single['times'][1]} at {conn_single['stations'][1]}."
-                )
+            try:
+                conn_single.update(ParseSingleConnectionDetail(html_single))
+                logger.debug(
+                    f"\t\tDeparture at {conn_single['times'][0]} from {conn_single['stations'][0]}."
+                    f" Arrival at {conn_single['times'][1]} at {conn_single['stations'][1]}."
+                    )
+            except Exception as e:
+                logger.error("Unable to parse connection details")
+                raise e
 
             conn["single_connections"].append(conn_single)
 
         connection_query["connections"].append(conn)
 
     return connection_query
 
@@ -187,22 +203,25 @@
     if len(conn_delay.contents) != 3 or conn_delay.contents[1].text is None:
         return None
 
     return conn_delay.contents[1].text.replace("\\r\\n", "").rstrip()
 
 def ParseIcon(html_single) -> str | None:
     html_connection_string_container = html_single.find("div", class_="title-container")
+    html_connection_string = html_connection_string_container.find("span").next
 
-    connection_icon_path = html_connection_string_container.find("img")["src"]
-    re_match_icon = re.compile("/images/trtype/(2.svg|3.svg)").search(connection_icon_path)
+    # Legacy icon names before they changed <img> to <span> without img -_-
+    # (I actually do not know how they draw the image instead of a single char in span)
+    icon = None
+    if html_connection_string == "÷":
+        icon = "2.svg"
+    elif html_connection_string == "ü":
+        icon = "3.svg"
 
-    if re_match_icon is None:
-        return None
-
-    return re_match_icon.group(1)
+    return icon
 
 def ParseTypeAndNumber(html_single) -> dict:
     html_connection_string_container = html_single.find("div", class_="title-container")
     connection_num = html_single.find("h3").contents[0].contents[0]
 
     connection_string = html_connection_string_container.find("h3").contents[0].contents[0]
```

### Comparing `idos_scraper-0.2.3/src/idos_scraper/scrapers/search_station.py` & `idos_scraper-0.2.4/src/idos_scraper/scrapers/search_station.py`

 * *Files identical despite different names*

### Comparing `idos_scraper-0.2.3/LICENSE` & `idos_scraper-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `idos_scraper-0.2.3/README.md` & `idos_scraper-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `idos_scraper-0.2.3/pyproject.toml` & `idos_scraper-0.2.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "idos-scraper"
-version = "0.2.3"
+version = "0.2.4"
 authors = [
   { name="Tomas Deingruber", email="Deingruber.Tomas+idos-scraper@gmail.com" },
 ]
 description = "Scrapes Czech public transport data from IDOS"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `idos_scraper-0.2.3/PKG-INFO` & `idos_scraper-0.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: idos-scraper
-Version: 0.2.3
+Version: 0.2.4
 Summary: Scrapes Czech public transport data from IDOS
 Project-URL: Homepage, https://github.com/Tomdein/idos-scraper
 Project-URL: Repository, https://github.com/Tomdein/idos-scraper
 Project-URL: Documentation, https://github.com/Tomdein/idos-scraper
 Project-URL: Bug Tracker, https://github.com/Tomdein/idos-scraper/issues
 Author-email: Tomas Deingruber <Deingruber.Tomas+idos-scraper@gmail.com>
 License-File: LICENSE
```


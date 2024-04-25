# Comparing `tmp/pyriksdagen-1.1.0.tar.gz` & `tmp/pyriksdagen-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyriksdagen-1.1.0.tar", max compression
+gzip compressed data, was "pyriksdagen-1.2.0.tar", max compression
```

## Comparing `pyriksdagen-1.1.0.tar` & `pyriksdagen-1.2.0.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0     1107 2024-04-17 11:48:09.761917 pyriksdagen-1.1.0/LICENSE
--rw-r--r--   0        0        0      247 2024-04-17 11:48:09.761917 pyriksdagen-1.1.0/README.md
--rw-r--r--   0        0        0      847 2024-04-17 11:48:52.538331 pyriksdagen-1.1.0/pyproject.toml
--rw-r--r--   0        0        0       84 2024-04-17 11:48:09.761917 pyriksdagen-1.1.0/pyriksdagen/__init__.py
--rw-r--r--   0        0        0      286 2024-04-17 11:48:09.761917 pyriksdagen-1.1.0/pyriksdagen/data/queries/alias.rq
--rw-r--r--   0        0        0      432 2024-04-17 11:48:09.761917 pyriksdagen-1.1.0/pyriksdagen/data/queries/explicit_no_party.rq
--rw-r--r--   0        0        0      539 2024-04-17 11:48:09.761917 pyriksdagen-1.1.0/pyriksdagen/data/queries/external_identifiers.rq
--rw-r--r--   0        0        0      494 2024-04-17 11:48:09.761917 pyriksdagen-1.1.0/pyriksdagen/data/queries/government.rq
--rw-r--r--   0        0        0      777 2024-04-17 11:48:09.761917 pyriksdagen-1.1.0/pyriksdagen/data/queries/member_of_parliament.rq
--rw-r--r--   0        0        0      148 2024-04-17 11:48:09.761917 pyriksdagen-1.1.0/pyriksdagen/data/queries/member_of_parliament.txt
--rw-r--r--   0        0        0     1621 2024-04-17 11:48:09.761917 pyriksdagen-1.1.0/pyriksdagen/data/queries/minister.rq
--rw-r--r--   0        0        0      235 2024-04-17 11:48:09.761917 pyriksdagen-1.1.0/pyriksdagen/data/queries/minister.txt
--rw-r--r--   0        0        0      301 2024-04-17 11:48:09.761917 pyriksdagen-1.1.0/pyriksdagen/data/queries/name_location_specifier.rq
--rw-r--r--   0        0        0      527 2024-04-17 11:48:09.761917 pyriksdagen-1.1.0/pyriksdagen/data/queries/party_affiliation.rq
--rw-r--r--   0        0        0      588 2024-04-17 11:48:09.761917 pyriksdagen-1.1.0/pyriksdagen/data/queries/person.rq
--rw-r--r--   0        0        0      277 2024-04-17 11:48:09.761917 pyriksdagen-1.1.0/pyriksdagen/data/queries/place_of_birth.rq
--rw-r--r--   0        0        0      277 2024-04-17 11:48:09.761917 pyriksdagen-1.1.0/pyriksdagen/data/queries/place_of_death.rq
--rw-r--r--   0        0        0      251 2024-04-17 11:48:09.761917 pyriksdagen-1.1.0/pyriksdagen/data/queries/portraits.rq
--rw-r--r--   0        0        0      663 2024-04-17 11:48:09.761917 pyriksdagen-1.1.0/pyriksdagen/data/queries/speaker.rq
--rw-r--r--   0        0        0      253 2024-04-17 11:48:09.761917 pyriksdagen-1.1.0/pyriksdagen/data/queries/speaker.txt
--rw-r--r--   0        0        0      247 2024-04-17 11:48:09.761917 pyriksdagen-1.1.0/pyriksdagen/data/queries/twitter.rq
--rw-r--r--   0        0        0      959 2024-04-17 11:48:09.761917 pyriksdagen-1.1.0/pyriksdagen/data/queries/wiki_id.rq
--rw-r--r--   0        0        0      225 2024-04-17 11:48:09.761917 pyriksdagen-1.1.0/pyriksdagen/data/queries_backup/alias.rq
--rw-r--r--   0        0        0      482 2024-04-17 11:48:09.761917 pyriksdagen-1.1.0/pyriksdagen/data/queries_backup/government.rq
--rw-r--r--   0        0        0      722 2024-04-17 11:48:09.761917 pyriksdagen-1.1.0/pyriksdagen/data/queries_backup/member_of_parliament.rq
--rw-r--r--   0        0        0     1380 2024-04-17 11:48:09.761917 pyriksdagen-1.1.0/pyriksdagen/data/queries_backup/minister.rq
--rw-r--r--   0        0        0     1013 2024-04-17 11:48:09.761917 pyriksdagen-1.1.0/pyriksdagen/data/queries_backup/name_location_specifier.rq
--rw-r--r--   0        0        0     1230 2024-04-17 11:48:09.761917 pyriksdagen-1.1.0/pyriksdagen/data/queries_backup/party_affiliation.rq
--rw-r--r--   0        0        0     1412 2024-04-17 11:48:09.761917 pyriksdagen-1.1.0/pyriksdagen/data/queries_backup/person.rq
--rw-r--r--   0        0        0      616 2024-04-17 11:48:09.761917 pyriksdagen-1.1.0/pyriksdagen/data/queries_backup/speaker.rq
--rw-r--r--   0        0        0      959 2024-04-17 11:48:09.761917 pyriksdagen-1.1.0/pyriksdagen/data/queries_backup/twitter.rq
--rw-r--r--   0        0        0      798 2024-04-17 11:48:09.761917 pyriksdagen-1.1.0/pyriksdagen/data/segmentation/detection.csv
--rw-r--r--   0        0        0     3355 2024-04-17 11:48:09.761917 pyriksdagen-1.1.0/pyriksdagen/data/segmentation/patterns.json
--rw-r--r--   0        0        0     2195 2024-04-17 11:48:09.761917 pyriksdagen-1.1.0/pyriksdagen/dataset.py
--rw-r--r--   0        0        0    19798 2024-04-17 11:48:09.761917 pyriksdagen-1.1.0/pyriksdagen/date_handling.py
--rw-r--r--   0        0        0     7026 2024-04-17 11:48:09.761917 pyriksdagen-1.1.0/pyriksdagen/db.py
--rw-r--r--   0        0        0     8159 2024-04-17 11:48:09.761917 pyriksdagen-1.1.0/pyriksdagen/download.py
--rw-r--r--   0        0        0     5649 2024-04-17 11:48:09.761917 pyriksdagen-1.1.0/pyriksdagen/export.py
--rw-r--r--   0        0        0     5222 2024-04-17 11:48:09.761917 pyriksdagen-1.1.0/pyriksdagen/match_mp.py
--rw-r--r--   0        0        0    13611 2024-04-17 11:48:09.761917 pyriksdagen-1.1.0/pyriksdagen/metadata.py
--rw-r--r--   0        0        0    11120 2024-04-17 11:48:09.761917 pyriksdagen-1.1.0/pyriksdagen/mp.py
--rw-r--r--   0        0        0    17780 2024-04-17 11:48:09.761917 pyriksdagen-1.1.0/pyriksdagen/refine.py
--rwxr-xr-x   0        0        0      237 2024-04-17 11:48:09.765917 pyriksdagen-1.1.0/pyriksdagen/requirements.txt
--rw-r--r--   0        0        0     8441 2024-04-17 11:48:09.765917 pyriksdagen-1.1.0/pyriksdagen/segmentation.py
--rw-r--r--   0        0        0    10156 2024-04-17 11:48:09.765917 pyriksdagen-1.1.0/pyriksdagen/swerik_catalog.py
--rw-r--r--   0        0        0    10395 2024-04-17 11:48:09.765917 pyriksdagen-1.1.0/pyriksdagen/utils.py
--rw-r--r--   0        0        0     5682 2024-04-17 11:48:09.765917 pyriksdagen-1.1.0/pyriksdagen/wikidata.py
--rw-r--r--   0        0        0     1578 1970-01-01 00:00:00.000000 pyriksdagen-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1107 2024-04-25 14:05:04.212849 pyriksdagen-1.2.0/LICENSE
+-rw-r--r--   0        0        0      402 2024-04-25 14:05:04.212849 pyriksdagen-1.2.0/README.md
+-rw-r--r--   0        0        0      847 2024-04-25 14:05:43.301216 pyriksdagen-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0       84 2024-04-25 14:05:04.212849 pyriksdagen-1.2.0/pyriksdagen/__init__.py
+-rw-r--r--   0        0        0      286 2024-04-25 14:05:04.212849 pyriksdagen-1.2.0/pyriksdagen/data/queries/alias.rq
+-rw-r--r--   0        0        0      432 2024-04-25 14:05:04.212849 pyriksdagen-1.2.0/pyriksdagen/data/queries/explicit_no_party.rq
+-rw-r--r--   0        0        0      539 2024-04-25 14:05:04.212849 pyriksdagen-1.2.0/pyriksdagen/data/queries/external_identifiers.rq
+-rw-r--r--   0        0        0      494 2024-04-25 14:05:04.212849 pyriksdagen-1.2.0/pyriksdagen/data/queries/government.rq
+-rw-r--r--   0        0        0      777 2024-04-25 14:05:04.212849 pyriksdagen-1.2.0/pyriksdagen/data/queries/member_of_parliament.rq
+-rw-r--r--   0        0        0      148 2024-04-25 14:05:04.212849 pyriksdagen-1.2.0/pyriksdagen/data/queries/member_of_parliament.txt
+-rw-r--r--   0        0        0     1621 2024-04-25 14:05:04.212849 pyriksdagen-1.2.0/pyriksdagen/data/queries/minister.rq
+-rw-r--r--   0        0        0      235 2024-04-25 14:05:04.212849 pyriksdagen-1.2.0/pyriksdagen/data/queries/minister.txt
+-rw-r--r--   0        0        0      301 2024-04-25 14:05:04.212849 pyriksdagen-1.2.0/pyriksdagen/data/queries/name_location_specifier.rq
+-rw-r--r--   0        0        0      527 2024-04-25 14:05:04.212849 pyriksdagen-1.2.0/pyriksdagen/data/queries/party_affiliation.rq
+-rw-r--r--   0        0        0      588 2024-04-25 14:05:04.212849 pyriksdagen-1.2.0/pyriksdagen/data/queries/person.rq
+-rw-r--r--   0        0        0      277 2024-04-25 14:05:04.212849 pyriksdagen-1.2.0/pyriksdagen/data/queries/place_of_birth.rq
+-rw-r--r--   0        0        0      277 2024-04-25 14:05:04.212849 pyriksdagen-1.2.0/pyriksdagen/data/queries/place_of_death.rq
+-rw-r--r--   0        0        0      251 2024-04-25 14:05:04.212849 pyriksdagen-1.2.0/pyriksdagen/data/queries/portraits.rq
+-rw-r--r--   0        0        0      663 2024-04-25 14:05:04.212849 pyriksdagen-1.2.0/pyriksdagen/data/queries/speaker.rq
+-rw-r--r--   0        0        0      253 2024-04-25 14:05:04.212849 pyriksdagen-1.2.0/pyriksdagen/data/queries/speaker.txt
+-rw-r--r--   0        0        0      247 2024-04-25 14:05:04.212849 pyriksdagen-1.2.0/pyriksdagen/data/queries/twitter.rq
+-rw-r--r--   0        0        0      959 2024-04-25 14:05:04.212849 pyriksdagen-1.2.0/pyriksdagen/data/queries/wiki_id.rq
+-rw-r--r--   0        0        0      225 2024-04-25 14:05:04.212849 pyriksdagen-1.2.0/pyriksdagen/data/queries_backup/alias.rq
+-rw-r--r--   0        0        0      482 2024-04-25 14:05:04.212849 pyriksdagen-1.2.0/pyriksdagen/data/queries_backup/government.rq
+-rw-r--r--   0        0        0      722 2024-04-25 14:05:04.212849 pyriksdagen-1.2.0/pyriksdagen/data/queries_backup/member_of_parliament.rq
+-rw-r--r--   0        0        0     1380 2024-04-25 14:05:04.212849 pyriksdagen-1.2.0/pyriksdagen/data/queries_backup/minister.rq
+-rw-r--r--   0        0        0     1013 2024-04-25 14:05:04.212849 pyriksdagen-1.2.0/pyriksdagen/data/queries_backup/name_location_specifier.rq
+-rw-r--r--   0        0        0     1230 2024-04-25 14:05:04.212849 pyriksdagen-1.2.0/pyriksdagen/data/queries_backup/party_affiliation.rq
+-rw-r--r--   0        0        0     1412 2024-04-25 14:05:04.212849 pyriksdagen-1.2.0/pyriksdagen/data/queries_backup/person.rq
+-rw-r--r--   0        0        0      616 2024-04-25 14:05:04.212849 pyriksdagen-1.2.0/pyriksdagen/data/queries_backup/speaker.rq
+-rw-r--r--   0        0        0      959 2024-04-25 14:05:04.212849 pyriksdagen-1.2.0/pyriksdagen/data/queries_backup/twitter.rq
+-rw-r--r--   0        0        0      798 2024-04-25 14:05:04.212849 pyriksdagen-1.2.0/pyriksdagen/data/segmentation/detection.csv
+-rw-r--r--   0        0        0     3355 2024-04-25 14:05:04.212849 pyriksdagen-1.2.0/pyriksdagen/data/segmentation/patterns.json
+-rw-r--r--   0        0        0     2195 2024-04-25 14:05:04.212849 pyriksdagen-1.2.0/pyriksdagen/dataset.py
+-rw-r--r--   0        0        0    19798 2024-04-25 14:05:04.212849 pyriksdagen-1.2.0/pyriksdagen/date_handling.py
+-rw-r--r--   0        0        0     7026 2024-04-25 14:05:04.212849 pyriksdagen-1.2.0/pyriksdagen/db.py
+-rw-r--r--   0        0        0     8159 2024-04-25 14:05:04.212849 pyriksdagen-1.2.0/pyriksdagen/download.py
+-rw-r--r--   0        0        0     5649 2024-04-25 14:05:04.212849 pyriksdagen-1.2.0/pyriksdagen/export.py
+-rw-r--r--   0        0        0     5222 2024-04-25 14:05:04.212849 pyriksdagen-1.2.0/pyriksdagen/match_mp.py
+-rw-r--r--   0        0        0    13611 2024-04-25 14:05:04.216848 pyriksdagen-1.2.0/pyriksdagen/metadata.py
+-rw-r--r--   0        0        0    11120 2024-04-25 14:05:04.216848 pyriksdagen-1.2.0/pyriksdagen/mp.py
+-rw-r--r--   0        0        0    17780 2024-04-25 14:05:04.216848 pyriksdagen-1.2.0/pyriksdagen/refine.py
+-rwxr-xr-x   0        0        0      237 2024-04-25 14:05:04.216848 pyriksdagen-1.2.0/pyriksdagen/requirements.txt
+-rw-r--r--   0        0        0     8783 2024-04-25 14:05:04.216848 pyriksdagen-1.2.0/pyriksdagen/segmentation.py
+-rw-r--r--   0        0        0    10156 2024-04-25 14:05:04.216848 pyriksdagen-1.2.0/pyriksdagen/swerik_catalog.py
+-rw-r--r--   0        0        0    10395 2024-04-25 14:05:04.216848 pyriksdagen-1.2.0/pyriksdagen/utils.py
+-rw-r--r--   0        0        0     5682 2024-04-25 14:05:04.216848 pyriksdagen-1.2.0/pyriksdagen/wikidata.py
+-rw-r--r--   0        0        0     1733 1970-01-01 00:00:00.000000 pyriksdagen-1.2.0/PKG-INFO
```

### Comparing `pyriksdagen-1.1.0/LICENSE` & `pyriksdagen-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyriksdagen-1.1.0/pyproject.toml` & `pyriksdagen-1.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyriksdagen"
-version = "1.1.0"
+version = "1.2.0"
 description = "Access the Riksdagen corpus"
 authors = ["ninpnin <vainoyrjanainen@icloud.com>"]
 repository = "https://github.com/welfare-state-analytics/riksdagen-corpus"
 readme = "README.md"
 license = "MIT"
 packages = [
     { include = "pyriksdagen", from = "" }
```

### Comparing `pyriksdagen-1.1.0/pyriksdagen/data/queries/external_identifiers.rq` & `pyriksdagen-1.2.0/pyriksdagen/data/queries/external_identifiers.rq`

 * *Files identical despite different names*

### Comparing `pyriksdagen-1.1.0/pyriksdagen/data/queries/member_of_parliament.rq` & `pyriksdagen-1.2.0/pyriksdagen/data/queries/member_of_parliament.rq`

 * *Files identical despite different names*

### Comparing `pyriksdagen-1.1.0/pyriksdagen/data/queries/minister.rq` & `pyriksdagen-1.2.0/pyriksdagen/data/queries/minister.rq`

 * *Files identical despite different names*

### Comparing `pyriksdagen-1.1.0/pyriksdagen/data/queries/party_affiliation.rq` & `pyriksdagen-1.2.0/pyriksdagen/data/queries/party_affiliation.rq`

 * *Files identical despite different names*

### Comparing `pyriksdagen-1.1.0/pyriksdagen/data/queries/person.rq` & `pyriksdagen-1.2.0/pyriksdagen/data/queries/person.rq`

 * *Files identical despite different names*

### Comparing `pyriksdagen-1.1.0/pyriksdagen/data/queries/speaker.rq` & `pyriksdagen-1.2.0/pyriksdagen/data/queries/speaker.rq`

 * *Files identical despite different names*

### Comparing `pyriksdagen-1.1.0/pyriksdagen/data/queries/wiki_id.rq` & `pyriksdagen-1.2.0/pyriksdagen/data/queries/wiki_id.rq`

 * *Files identical despite different names*

### Comparing `pyriksdagen-1.1.0/pyriksdagen/data/queries_backup/member_of_parliament.rq` & `pyriksdagen-1.2.0/pyriksdagen/data/queries_backup/member_of_parliament.rq`

 * *Files identical despite different names*

### Comparing `pyriksdagen-1.1.0/pyriksdagen/data/queries_backup/minister.rq` & `pyriksdagen-1.2.0/pyriksdagen/data/queries_backup/minister.rq`

 * *Files identical despite different names*

### Comparing `pyriksdagen-1.1.0/pyriksdagen/data/queries_backup/name_location_specifier.rq` & `pyriksdagen-1.2.0/pyriksdagen/data/queries_backup/name_location_specifier.rq`

 * *Files identical despite different names*

### Comparing `pyriksdagen-1.1.0/pyriksdagen/data/queries_backup/party_affiliation.rq` & `pyriksdagen-1.2.0/pyriksdagen/data/queries_backup/party_affiliation.rq`

 * *Files identical despite different names*

### Comparing `pyriksdagen-1.1.0/pyriksdagen/data/queries_backup/person.rq` & `pyriksdagen-1.2.0/pyriksdagen/data/queries_backup/person.rq`

 * *Files identical despite different names*

### Comparing `pyriksdagen-1.1.0/pyriksdagen/data/queries_backup/speaker.rq` & `pyriksdagen-1.2.0/pyriksdagen/data/queries_backup/speaker.rq`

 * *Files identical despite different names*

### Comparing `pyriksdagen-1.1.0/pyriksdagen/data/queries_backup/twitter.rq` & `pyriksdagen-1.2.0/pyriksdagen/data/queries_backup/twitter.rq`

 * *Files identical despite different names*

### Comparing `pyriksdagen-1.1.0/pyriksdagen/data/segmentation/detection.csv` & `pyriksdagen-1.2.0/pyriksdagen/data/segmentation/detection.csv`

 * *Files identical despite different names*

### Comparing `pyriksdagen-1.1.0/pyriksdagen/data/segmentation/patterns.json` & `pyriksdagen-1.2.0/pyriksdagen/data/segmentation/patterns.json`

 * *Files identical despite different names*

### Comparing `pyriksdagen-1.1.0/pyriksdagen/dataset.py` & `pyriksdagen-1.2.0/pyriksdagen/dataset.py`

 * *Files identical despite different names*

### Comparing `pyriksdagen-1.1.0/pyriksdagen/date_handling.py` & `pyriksdagen-1.2.0/pyriksdagen/date_handling.py`

 * *Files identical despite different names*

### Comparing `pyriksdagen-1.1.0/pyriksdagen/db.py` & `pyriksdagen-1.2.0/pyriksdagen/db.py`

 * *Files identical despite different names*

### Comparing `pyriksdagen-1.1.0/pyriksdagen/download.py` & `pyriksdagen-1.2.0/pyriksdagen/download.py`

 * *Files identical despite different names*

### Comparing `pyriksdagen-1.1.0/pyriksdagen/export.py` & `pyriksdagen-1.2.0/pyriksdagen/export.py`

 * *Files identical despite different names*

### Comparing `pyriksdagen-1.1.0/pyriksdagen/match_mp.py` & `pyriksdagen-1.2.0/pyriksdagen/match_mp.py`

 * *Files identical despite different names*

### Comparing `pyriksdagen-1.1.0/pyriksdagen/metadata.py` & `pyriksdagen-1.2.0/pyriksdagen/metadata.py`

 * *Files identical despite different names*

### Comparing `pyriksdagen-1.1.0/pyriksdagen/mp.py` & `pyriksdagen-1.2.0/pyriksdagen/mp.py`

 * *Files identical despite different names*

### Comparing `pyriksdagen-1.1.0/pyriksdagen/refine.py` & `pyriksdagen-1.2.0/pyriksdagen/refine.py`

 * *Files identical despite different names*

### Comparing `pyriksdagen-1.1.0/pyriksdagen/segmentation.py` & `pyriksdagen-1.2.0/pyriksdagen/segmentation.py`

 * *Files 3% similar despite different names*

```diff
@@ -82,14 +82,24 @@
     lower_txt = matched_txt.lower()
 
     # Filter by gender
     if 'gender' in intro_dict:
         gender = intro_dict["gender"]
         minister_db = minister_db[minister_db["gender"] == gender]
 
+    # Filter by date
+    if 'date' in intro_dict:
+
+        minister_db = minister_db[
+                (minister_db["start"] <= intro_dict['date']) &
+                (minister_db["end"] >= intro_dict['date'])]
+        if not minister_db.empty:
+            if len(set(minister_db["id"])) == 1:
+                return minister_db["id"].iloc[0]
+
     # Match by name
     if 'name' in intro_dict:
         name = intro_dict["name"].lower()
         # thage petterson
         #print(minister_db)
         name_matches = names_in(name, minister_db)
         if not name_matches.empty:
```

### Comparing `pyriksdagen-1.1.0/pyriksdagen/swerik_catalog.py` & `pyriksdagen-1.2.0/pyriksdagen/swerik_catalog.py`

 * *Files identical despite different names*

### Comparing `pyriksdagen-1.1.0/pyriksdagen/utils.py` & `pyriksdagen-1.2.0/pyriksdagen/utils.py`

 * *Files identical despite different names*

### Comparing `pyriksdagen-1.1.0/pyriksdagen/wikidata.py` & `pyriksdagen-1.2.0/pyriksdagen/wikidata.py`

 * *Files identical despite different names*

### Comparing `pyriksdagen-1.1.0/PKG-INFO` & `pyriksdagen-1.2.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyriksdagen
-Version: 1.1.0
+Version: 1.2.0
 Summary: Access the Riksdagen corpus
 Home-page: https://github.com/welfare-state-analytics/riksdagen-corpus
 License: MIT
 Author: ninpnin
 Author-email: vainoyrjanainen@icloud.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -39,8 +39,9 @@
 Project-URL: Repository, https://github.com/welfare-state-analytics/riksdagen-corpus
 Description-Content-Type: text/markdown
 
 # pyriksdagen
 
 Python module for interacting with the Swedish Parliamentary Corpus
 
-The use of the module is demonstrated in the [Example Jupyter Notebook](https://github.com/swerik-project/pyriksdagen/blob/main/examples/corpus-walkthrough.ipynb).
+The use of the module is demonstrated in the [Example Jupyter Notebook](https://github.com/swerik-project/pyriksdagen/blob/main/examples/corpus-walkthrough.ipynb), which can also be run on [Google Colab](https://colab.research.google.com/github/swerik-project/pyriksdagen/blob/main/examples/corpus-walkthrough.ipynb).
+
```


# Comparing `tmp/krcg-3.8.tar.gz` & `tmp/krcg-3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "krcg-3.8.tar", last modified: Thu Feb  8 15:16:12 2024, max compression
+gzip compressed data, was "krcg-3.9.tar", last modified: Thu Feb  8 18:07:19 2024, max compression
```

## Comparing `krcg-3.8.tar` & `krcg-3.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 lpanhaleux   (501) staff       (20)        0 2024-02-08 15:16:12.890167 krcg-3.8/
--rw-r--r--   0 lpanhaleux   (501) staff       (20)    14485 2024-02-08 15:16:12.000000 krcg-3.8/CHANGELOG.rst
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     1073 2024-02-08 15:16:12.000000 krcg-3.8/LICENSE
--rw-r--r--   0 lpanhaleux   (501) staff       (20)      300 2024-02-08 15:16:12.000000 krcg-3.8/MANIFEST.in
--rw-r--r--   0 lpanhaleux   (501) staff       (20)    17505 2024-02-08 15:16:12.889910 krcg-3.8/PKG-INFO
--rw-r--r--   0 lpanhaleux   (501) staff       (20)    16147 2024-02-08 15:16:12.000000 krcg-3.8/README.md
-drwxr-xr-x   0 lpanhaleux   (501) staff       (20)        0 2024-02-08 15:16:12.888377 krcg-3.8/krcg/
--rw-r--r--   0 lpanhaleux   (501) staff       (20)        0 2024-02-08 15:16:12.000000 krcg-3.8/krcg/__init__.py
--rw-r--r--   0 lpanhaleux   (501) staff       (20)    10983 2024-02-08 15:16:12.000000 krcg-3.8/krcg/analyzer.py
--rw-r--r--   0 lpanhaleux   (501) staff       (20)    53464 2024-02-08 15:16:12.000000 krcg-3.8/krcg/cards.py
--rw-r--r--   0 lpanhaleux   (501) staff       (20)    11539 2024-02-08 15:16:12.000000 krcg-3.8/krcg/config.py
--rw-r--r--   0 lpanhaleux   (501) staff       (20)    19349 2024-02-08 15:16:12.000000 krcg-3.8/krcg/deck.py
--rw-r--r--   0 lpanhaleux   (501) staff       (20)    27610 2024-02-08 15:16:12.000000 krcg-3.8/krcg/parser.py
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     3449 2024-02-08 15:16:12.000000 krcg-3.8/krcg/rulings.py
--rw-r--r--   0 lpanhaleux   (501) staff       (20)    24346 2024-02-08 15:16:12.000000 krcg-3.8/krcg/seating.py
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     2782 2024-02-08 15:16:12.000000 krcg-3.8/krcg/sets.py
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     2955 2024-02-08 15:16:12.000000 krcg-3.8/krcg/twda.py
--rw-r--r--   0 lpanhaleux   (501) staff       (20)    10095 2024-02-08 15:16:12.000000 krcg-3.8/krcg/utils.py
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     3668 2024-02-08 15:16:12.000000 krcg-3.8/krcg/vtes.py
-drwxr-xr-x   0 lpanhaleux   (501) staff       (20)        0 2024-02-08 15:16:12.889343 krcg-3.8/krcg.egg-info/
--rw-r--r--   0 lpanhaleux   (501) staff       (20)      337 2024-02-08 15:16:12.000000 krcg-3.8/krcg.egg-info/SOURCES.txt
--rw-r--r--   0 lpanhaleux   (501) staff       (20)     1314 2024-02-08 15:16:12.000000 krcg-3.8/pyproject.toml
-drwxr-xr-x   0 lpanhaleux   (501) staff       (20)        0 2024-02-08 15:16:12.889133 krcg-3.8/rulings/
--rw-r--r--   0 lpanhaleux   (501) staff       (20)        0 2024-02-08 15:16:12.000000 krcg-3.8/rulings/__init__.py
--rw-r--r--   0 lpanhaleux   (501) staff       (20)   363939 2024-02-08 15:16:12.000000 krcg-3.8/rulings/cards-rulings.yaml
--rw-r--r--   0 lpanhaleux   (501) staff       (20)    34601 2024-02-08 15:16:12.000000 krcg-3.8/rulings/general-rulings.yaml
--rw-r--r--   0 lpanhaleux   (501) staff       (20)   139014 2024-02-08 15:16:12.000000 krcg-3.8/rulings/rulings-links.yaml
--rw-r--r--   0 lpanhaleux   (501) staff       (20)       38 2024-02-08 15:16:12.890211 krcg-3.8/setup.cfg
+drwxr-xr-x   0 lpanhaleux   (501) staff       (20)        0 2024-02-08 18:07:19.894683 krcg-3.9/
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)    14539 2024-02-08 18:07:19.000000 krcg-3.9/CHANGELOG.rst
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     1073 2024-02-08 18:07:19.000000 krcg-3.9/LICENSE
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)      285 2024-02-08 18:07:19.000000 krcg-3.9/MANIFEST.in
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)    17505 2024-02-08 18:07:19.894437 krcg-3.9/PKG-INFO
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)    16147 2024-02-08 18:07:19.000000 krcg-3.9/README.md
+drwxr-xr-x   0 lpanhaleux   (501) staff       (20)        0 2024-02-08 18:07:19.893040 krcg-3.9/krcg/
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)        0 2024-02-08 18:07:19.000000 krcg-3.9/krcg/__init__.py
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)    10983 2024-02-08 18:07:19.000000 krcg-3.9/krcg/analyzer.py
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)    53490 2024-02-08 18:07:19.000000 krcg-3.9/krcg/cards.py
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)    11539 2024-02-08 18:07:19.000000 krcg-3.9/krcg/config.py
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)    19349 2024-02-08 18:07:19.000000 krcg-3.9/krcg/deck.py
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)    27610 2024-02-08 18:07:19.000000 krcg-3.9/krcg/parser.py
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     3449 2024-02-08 18:07:19.000000 krcg-3.9/krcg/rulings.py
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)    24346 2024-02-08 18:07:19.000000 krcg-3.9/krcg/seating.py
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     2788 2024-02-08 18:07:19.000000 krcg-3.9/krcg/sets.py
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     2955 2024-02-08 18:07:19.000000 krcg-3.9/krcg/twda.py
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)    10095 2024-02-08 18:07:19.000000 krcg-3.9/krcg/utils.py
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     3668 2024-02-08 18:07:19.000000 krcg-3.9/krcg/vtes.py
+drwxr-xr-x   0 lpanhaleux   (501) staff       (20)        0 2024-02-08 18:07:19.893866 krcg-3.9/krcg.egg-info/
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)      337 2024-02-08 18:07:19.000000 krcg-3.9/krcg.egg-info/SOURCES.txt
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)     1314 2024-02-08 18:07:19.000000 krcg-3.9/pyproject.toml
+drwxr-xr-x   0 lpanhaleux   (501) staff       (20)        0 2024-02-08 18:07:19.893682 krcg-3.9/rulings/
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)        0 2024-02-08 18:07:19.000000 krcg-3.9/rulings/__init__.py
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)   363939 2024-02-08 18:07:19.000000 krcg-3.9/rulings/cards-rulings.yaml
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)    34601 2024-02-08 18:07:19.000000 krcg-3.9/rulings/general-rulings.yaml
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)   139014 2024-02-08 18:07:19.000000 krcg-3.9/rulings/rulings-links.yaml
+-rw-r--r--   0 lpanhaleux   (501) staff       (20)       38 2024-02-08 18:07:19.894719 krcg-3.9/setup.cfg
```

### Comparing `krcg-3.8/CHANGELOG.rst` & `krcg-3.9/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 Changelog
 =========
 
+3.9 (2024-02-08)
+----------------
+
+- Fix scans URLs
+
+
 3.8 (2024-02-08)
 ----------------
 
 - Fix rulings load
 - Fix TWD HTML load
```

### Comparing `krcg-3.8/LICENSE` & `krcg-3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `krcg-3.8/PKG-INFO` & `krcg-3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: krcg
-Version: 3.8
+Version: 3.9
 Summary: Library for VTES cards and TWDA.
 Author-email: Lionel Panhaleux <lionel.panhaleux+krcg@gmail.com>
 Project-URL: Repository, https://github.com/lionel-panhaleux/krcg
 Keywords: vtes,Vampire: The Eternal Struggle,CCG,TWD,TWDA
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `krcg-3.8/README.md` & `krcg-3.9/README.md`

 * *Files identical despite different names*

### Comparing `krcg-3.8/krcg/analyzer.py` & `krcg-3.9/krcg/analyzer.py`

 * *Files identical despite different names*

### Comparing `krcg-3.8/krcg/cards.py` & `krcg-3.9/krcg/cards.py`

 * *Files 1% similar despite different names*

```diff
@@ -265,14 +265,20 @@
         "Ron Spenser": "Ron Spencer",
         "Sam Araya": "Samuel Araya",
         "Sandra Chang": "Sandra Chang-Adair",
         "T. Bradstreet": "Tim Bradstreet",
         "Tom Baxa": "Thomas Baxa",
         "zelgaris": 'Tomáš "zelgaris" Zahradníček',
     }
+    _NAMED_PROMOS = {
+        "2019 Promo Pack 1": "promo-pack-1",
+        "2020 Promo Pack 2": "promo-pack-2",
+        "2021 Kickstarter Promo": "kickstarter-promo",
+        "2018 Humble Bundle": "humble-bundle",
+    }
 
     def __init__(self):
         super().__init__()
         self.id = 0
         #: use `vekn_name` or `name` properties instead
         self._name = ""
         self.url = ""
@@ -572,33 +578,25 @@
                 key=lambda x: set_dict[x].release_date,
             )
         else:
             warnings.warn(f"no set found for {self}")
         # some cards have one set, no date, eg. playtest cards
         if self.sets and not self.ordered_sets:
             self.ordered_sets = list(self.sets.keys())
-        self.scans = {
-            name: self._compute_url(
-                expansion=(
-                    {
-                        "2019 Promo Pack 1": "promo-pack-1",
-                        "2020 Promo Pack 2": "promo-pack-2",
-                        "2021 Kickstarter Promo": "kickstarter-promo",
-                        "2018 Humble Bundle": "humble-bundle",
-                    }.get(name, "promo")
-                    if set_dict[name].abbrev in set(sets.SetMap.PROMOS)
-                    else name.lower()
-                    .replace(":", "")
-                    .replace(" ", "-")
-                    .replace("(", "")
-                    .replace(")", "")
-                )
-            )
-            for name in self.sets.keys()
-        }
+        self.scans = {}
+        for name in self.sets.keys():
+            if name in self._NAMED_PROMOS:
+                folder_name = self._NAMED_PROMOS[name]
+            elif re.search(r"(^|\s)((P|p)romo|(R|r)ewards?)(\s|$)", name):
+                folder_name = "promo"
+            else:
+                folder_name = name.lower().replace(":", "")
+                folder_name = folder_name.replace("(", "").replace(")", "")
+                folder_name = folder_name.replace(" ", "-")
+            self.scans[name] = self._compute_url(expansion=folder_name)
         self.url = self._compute_url()
 
     def _compute_url(self, lang: str = None, expansion: str = None) -> str:
         """Compute image URL for given language."""
         return (
             config.KRCG_STATIC_SERVER
             + "/card/"
```

### Comparing `krcg-3.8/krcg/config.py` & `krcg-3.9/krcg/config.py`

 * *Files identical despite different names*

### Comparing `krcg-3.8/krcg/deck.py` & `krcg-3.9/krcg/deck.py`

 * *Files identical despite different names*

### Comparing `krcg-3.8/krcg/parser.py` & `krcg-3.9/krcg/parser.py`

 * *Files identical despite different names*

### Comparing `krcg-3.8/krcg/rulings.py` & `krcg-3.9/krcg/rulings.py`

 * *Files identical despite different names*

### Comparing `krcg-3.8/krcg/seating.py` & `krcg-3.9/krcg/seating.py`

 * *Files identical despite different names*

### Comparing `krcg-3.8/krcg/sets.py` & `krcg-3.9/krcg/sets.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         self.name = data["Full Name"]
         self.company = data["Company"]
 
 
 class SetMap(dict):
     """A dict of all sets, index by Abbreviation and English name."""
 
-    PROMOS = {
+    _UNLISTED = {
         "Promo-20231007": ["2023 Mineiro Promo", "2023-10-07"],
         "Promo-20230916": ["2023 Zaragosa Promo", "2023-09-16"],
         "Promo-20230729": ["2023 Ropecon Promo", "2023-07-29"],
         "Promo-20230603": ["2023 Andalusian Open Promo", "2023-06-03"],
         "Promo-20230501": ["2023 War of the Ages Promo", "2023-05-01"],
         "Promo-20230531": ["2023 Chapters Promo", "2023-05-31"],
         "Promo-20230507": ["2023 Belgian Championship Promo", "2023-05-07"],
@@ -49,15 +49,15 @@
         "HttBR": ["Heirs to the Blood Reprint", "2018-07-14"],
         "KoTR": ["Keepers of Tradition Reprint", "2018-05-05"],
     }
 
     def __init__(self):
         super().__init__()
         self.add(Set(abbrev="POD", name="Print on Demand"))
-        for abbrev, (name, release_date) in self.PROMOS.items():
+        for abbrev, (name, release_date) in self._UNLISTED.items():
             self.add(Set(abbrev=abbrev, name=name, release_date=release_date))
 
     def add(self, set_: Set) -> None:
         """Add a set to the map."""
         self[set_.abbrev] = set_
         self[set_.name] = set_
```

### Comparing `krcg-3.8/krcg/twda.py` & `krcg-3.9/krcg/twda.py`

 * *Files identical despite different names*

### Comparing `krcg-3.8/krcg/utils.py` & `krcg-3.9/krcg/utils.py`

 * *Files identical despite different names*

### Comparing `krcg-3.8/krcg/vtes.py` & `krcg-3.9/krcg/vtes.py`

 * *Files identical despite different names*

### Comparing `krcg-3.8/pyproject.toml` & `krcg-3.9/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=68"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "krcg"
-version = "3.8"
+version = "3.9"
 authors = [
     { name = "Lionel Panhaleux", email = "lionel.panhaleux+krcg@gmail.com" },
 ]
 description = "Library for VTES cards and TWDA."
 keywords = ["vtes", "Vampire: The Eternal Struggle", "CCG", "TWD", "TWDA"]
 readme = "README.md"
 requires-python = ">=3.10"
```

### Comparing `krcg-3.8/rulings/cards-rulings.yaml` & `krcg-3.9/rulings/cards-rulings.yaml`

 * *Files identical despite different names*

### Comparing `krcg-3.8/rulings/general-rulings.yaml` & `krcg-3.9/rulings/general-rulings.yaml`

 * *Files identical despite different names*

### Comparing `krcg-3.8/rulings/rulings-links.yaml` & `krcg-3.9/rulings/rulings-links.yaml`

 * *Files identical despite different names*


# Comparing `tmp/robocrys-0.2.8.tar.gz` & `tmp/robocrys-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robocrys-0.2.8.tar", last modified: Mon Jun  5 14:21:18 2023, max compression
+gzip compressed data, was "robocrys-0.2.9.tar", last modified: Thu Apr 25 09:51:48 2024, max compression
```

## Comparing `robocrys-0.2.8.tar` & `robocrys-0.2.9.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:21:18.693198 robocrys-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-06-05 14:16:31.000000 robocrys-0.2.8/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-06-05 14:16:31.000000 robocrys-0.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6829 2023-06-05 14:21:18.693198 robocrys-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5628 2023-06-05 14:16:31.000000 robocrys-0.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:21:18.677197 robocrys-0.2.8/robocrys/
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-05 14:16:31.000000 robocrys-0.2.8/robocrys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-05 14:16:31.000000 robocrys-0.2.8/robocrys/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5163 2023-06-05 14:16:31.000000 robocrys-0.2.8/robocrys/adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7469 2023-06-05 14:16:31.000000 robocrys-0.2.8/robocrys/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:21:18.685198 robocrys-0.2.8/robocrys/condense/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 14:16:31.000000 robocrys-0.2.8/robocrys/condense/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24397 2023-06-05 14:16:31.000000 robocrys-0.2.8/robocrys/condense/component.py
--rw-r--r--   0 runner    (1001) docker     (123)    13390 2023-06-05 14:16:31.000000 robocrys-0.2.8/robocrys/condense/condenser.py
--rw-r--r--   0 runner    (1001) docker     (123)     4480 2023-06-05 14:16:31.000000 robocrys-0.2.8/robocrys/condense/fingerprint.py
--rw-r--r--   0 runner    (1001) docker     (123)   565274 2023-06-05 14:16:31.000000 robocrys-0.2.8/robocrys/condense/formula_db.json.gz
--rw-r--r--   0 runner    (1001) docker     (123)    10619 2023-06-05 14:16:31.000000 robocrys-0.2.8/robocrys/condense/mineral.py
--rw-r--r--   0 runner    (1001) docker     (123)   155577 2023-06-05 14:16:31.000000 robocrys-0.2.8/robocrys/condense/mineral_db.json.gz
--rw-r--r--   0 runner    (1001) docker     (123)     4836 2023-06-05 14:16:31.000000 robocrys-0.2.8/robocrys/condense/molecule.py
--rw-r--r--   0 runner    (1001) docker     (123)  3041331 2023-06-05 14:16:31.000000 robocrys-0.2.8/robocrys/condense/molecule_db.json.gz
--rw-r--r--   0 runner    (1001) docker     (123)    33461 2023-06-05 14:16:31.000000 robocrys-0.2.8/robocrys/condense/site.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:21:18.689198 robocrys-0.2.8/robocrys/condense/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 14:16:31.000000 robocrys-0.2.8/robocrys/condense/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10848 2023-06-05 14:16:31.000000 robocrys-0.2.8/robocrys/condense/tests/test_component.py
--rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-06-05 14:16:31.000000 robocrys-0.2.8/robocrys/condense/tests/test_fingerprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-06-05 14:16:31.000000 robocrys-0.2.8/robocrys/condense/tests/test_mineral.py
--rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-06-05 14:16:31.000000 robocrys-0.2.8/robocrys/condense/tests/test_molecule.py
--rw-r--r--   0 runner    (1001) docker     (123)    10261 2023-06-05 14:16:31.000000 robocrys-0.2.8/robocrys/condense/tests/test_site.py
--rw-r--r--   0 runner    (1001) docker     (123)     4632 2023-06-05 14:16:31.000000 robocrys-0.2.8/robocrys/condense/tests/test_structure.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:21:18.689198 robocrys-0.2.8/robocrys/describe/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 14:16:31.000000 robocrys-0.2.8/robocrys/describe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13713 2023-06-05 14:16:31.000000 robocrys-0.2.8/robocrys/describe/adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)    29897 2023-06-05 14:16:31.000000 robocrys-0.2.8/robocrys/describe/describer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:21:18.689198 robocrys-0.2.8/robocrys/describe/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 14:16:31.000000 robocrys-0.2.8/robocrys/describe/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5337 2023-06-05 14:16:31.000000 robocrys-0.2.8/robocrys/describe/tests/test_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-06-05 14:16:31.000000 robocrys-0.2.8/robocrys/describe/tests/test_description.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:21:18.689198 robocrys-0.2.8/robocrys/featurize/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 14:16:31.000000 robocrys-0.2.8/robocrys/featurize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9833 2023-06-05 14:16:31.000000 robocrys-0.2.8/robocrys/featurize/adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5782 2023-06-05 14:16:31.000000 robocrys-0.2.8/robocrys/featurize/featurizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:21:18.693198 robocrys-0.2.8/robocrys/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-06-05 14:16:31.000000 robocrys-0.2.8/robocrys/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-06-05 14:16:31.000000 robocrys-0.2.8/robocrys/tests/adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-06-05 14:16:31.000000 robocrys-0.2.8/robocrys/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-06-05 14:16:31.000000 robocrys-0.2.8/robocrys/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     8525 2023-06-05 14:16:31.000000 robocrys-0.2.8/robocrys/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:21:18.681198 robocrys-0.2.8/robocrys.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6829 2023-06-05 14:21:18.000000 robocrys-0.2.8/robocrys.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-06-05 14:21:18.000000 robocrys-0.2.8/robocrys.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 14:21:18.000000 robocrys-0.2.8/robocrys.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-05 14:21:18.000000 robocrys-0.2.8/robocrys.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-05 14:21:18.000000 robocrys-0.2.8/robocrys.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-05 14:21:18.000000 robocrys-0.2.8/robocrys.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 14:21:18.693198 robocrys-0.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-06-05 14:16:31.000000 robocrys-0.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:51:48.673139 robocrys-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     3461 2024-04-25 09:47:38.000000 robocrys-0.2.9/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2431 2024-04-25 09:47:38.000000 robocrys-0.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6834 2024-04-25 09:51:48.673139 robocrys-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5633 2024-04-25 09:47:38.000000 robocrys-0.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:51:48.661139 robocrys-0.2.9/robocrys/
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-25 09:47:38.000000 robocrys-0.2.9/robocrys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-25 09:47:38.000000 robocrys-0.2.9/robocrys/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5163 2024-04-25 09:47:38.000000 robocrys-0.2.9/robocrys/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7388 2024-04-25 09:47:38.000000 robocrys-0.2.9/robocrys/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:51:48.669139 robocrys-0.2.9/robocrys/condense/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 09:47:38.000000 robocrys-0.2.9/robocrys/condense/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24397 2024-04-25 09:47:38.000000 robocrys-0.2.9/robocrys/condense/component.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13390 2024-04-25 09:47:38.000000 robocrys-0.2.9/robocrys/condense/condenser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4480 2024-04-25 09:47:38.000000 robocrys-0.2.9/robocrys/condense/fingerprint.py
+-rw-r--r--   0 runner    (1001) docker     (127)   565274 2024-04-25 09:47:38.000000 robocrys-0.2.9/robocrys/condense/formula_db.json.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    10641 2024-04-25 09:47:38.000000 robocrys-0.2.9/robocrys/condense/mineral.py
+-rw-r--r--   0 runner    (1001) docker     (127)   155577 2024-04-25 09:47:38.000000 robocrys-0.2.9/robocrys/condense/mineral_db.json.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     4858 2024-04-25 09:47:38.000000 robocrys-0.2.9/robocrys/condense/molecule.py
+-rw-r--r--   0 runner    (1001) docker     (127)  3041331 2024-04-25 09:47:38.000000 robocrys-0.2.9/robocrys/condense/molecule_db.json.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    33461 2024-04-25 09:47:38.000000 robocrys-0.2.9/robocrys/condense/site.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:51:48.669139 robocrys-0.2.9/robocrys/condense/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 09:47:38.000000 robocrys-0.2.9/robocrys/condense/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10848 2024-04-25 09:47:38.000000 robocrys-0.2.9/robocrys/condense/tests/test_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-04-25 09:47:38.000000 robocrys-0.2.9/robocrys/condense/tests/test_fingerprint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-04-25 09:47:38.000000 robocrys-0.2.9/robocrys/condense/tests/test_mineral.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2231 2024-04-25 09:47:38.000000 robocrys-0.2.9/robocrys/condense/tests/test_molecule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10261 2024-04-25 09:47:38.000000 robocrys-0.2.9/robocrys/condense/tests/test_site.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4632 2024-04-25 09:47:38.000000 robocrys-0.2.9/robocrys/condense/tests/test_structure.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:51:48.669139 robocrys-0.2.9/robocrys/describe/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 09:47:38.000000 robocrys-0.2.9/robocrys/describe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13713 2024-04-25 09:47:38.000000 robocrys-0.2.9/robocrys/describe/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29902 2024-04-25 09:47:38.000000 robocrys-0.2.9/robocrys/describe/describer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:51:48.669139 robocrys-0.2.9/robocrys/describe/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 09:47:38.000000 robocrys-0.2.9/robocrys/describe/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5337 2024-04-25 09:47:38.000000 robocrys-0.2.9/robocrys/describe/tests/test_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3354 2024-04-25 09:47:38.000000 robocrys-0.2.9/robocrys/describe/tests/test_description.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:51:48.669139 robocrys-0.2.9/robocrys/featurize/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 09:47:38.000000 robocrys-0.2.9/robocrys/featurize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9715 2024-04-25 09:47:38.000000 robocrys-0.2.9/robocrys/featurize/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5782 2024-04-25 09:47:38.000000 robocrys-0.2.9/robocrys/featurize/featurizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:51:48.673139 robocrys-0.2.9/robocrys/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-04-25 09:47:38.000000 robocrys-0.2.9/robocrys/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-04-25 09:47:38.000000 robocrys-0.2.9/robocrys/tests/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2075 2024-04-25 09:47:38.000000 robocrys-0.2.9/robocrys/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-04-25 09:47:38.000000 robocrys-0.2.9/robocrys/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8688 2024-04-25 09:47:38.000000 robocrys-0.2.9/robocrys/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:51:48.661139 robocrys-0.2.9/robocrys.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6834 2024-04-25 09:51:48.000000 robocrys-0.2.9/robocrys.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-04-25 09:51:48.000000 robocrys-0.2.9/robocrys.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 09:51:48.000000 robocrys-0.2.9/robocrys.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-25 09:51:48.000000 robocrys-0.2.9/robocrys.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-25 09:51:48.000000 robocrys-0.2.9/robocrys.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-25 09:51:48.000000 robocrys-0.2.9/robocrys.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 09:51:48.673139 robocrys-0.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2861 2024-04-25 09:47:38.000000 robocrys-0.2.9/setup.py
```

### Comparing `robocrys-0.2.8/CONTRIBUTING.rst` & `robocrys-0.2.9/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `robocrys-0.2.8/LICENSE` & `robocrys-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `robocrys-0.2.8/PKG-INFO` & `robocrys-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robocrys
-Version: 0.2.8
+Version: 0.2.9
 Summary: Automatic generation of crystal structure descriptions
 Home-page: https://github.com/hackingmaterials/robocrystallographer
 Author: Alex Ganose
 Author-email: aganose@lbl.gov
 License: modified BSD
 Keywords: crystal-structure crystallography materials-science
 Platform: UNKNOWN
@@ -83,16 +83,16 @@
 from pymatgen import Structure
 from robocrys import StructureCondenser, StructureDescriber
 
 structure = Structure.from_file("my_structure.cif") # other file formats also supported
 
 # alternatively, uncomment the lines below to use the MPRester object
 # to fetch structures from the Materials Project database
-# from pymatgen import MPRester
-# structure = MPRester(API_KEY=None).get_structure_by_material_id("mp-856")
+# from mp_api.client import MPRester
+# structure = MPRester(api_key=None).get_structure_by_material_id("mp-856")
 
 condenser = StructureCondenser()
 describer = StructureDescriber()
 
 condensed_structure = condenser.condense_structure(structure)
 description = describer.describe(condensed_structure)
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: robocrys Version: 0.2.8 Summary: Automatic
+Metadata-Version: 2.1 Name: robocrys Version: 0.2.9 Summary: Automatic
 generation of crystal structure descriptions Home-page: https://github.com/
 hackingmaterials/robocrystallographer Author: Alex Ganose Author-email:
 aganose@lbl.gov License: modified BSD Keywords: crystal-structure
 crystallography materials-science Platform: UNKNOWN Classifier: Development
 Status :: 3 - Alpha Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Information Technology Classifier: License ::
 OSI Approved :: MIT License Classifier: Natural Language :: English Classifier:
@@ -37,16 +37,16 @@
 condense the structure into an descriptive JSON representation. -
 `StructureDescriber`: to turn the condensed structure into a text description.
 A minimal working example for generating text descriptions is simply: ```python
 from pymatgen import Structure from robocrys import StructureCondenser,
 StructureDescriber structure = Structure.from_file("my_structure.cif") # other
 file formats also supported # alternatively, uncomment the lines below to use
 the MPRester object #Â to fetch structures from the Materials Project database
-# from pymatgen import MPRester # structure = MPRester
-(API_KEY=None).get_structure_by_material_id("mp-856") condenser =
+# from mp_api.client import MPRester # structure = MPRester
+(api_key=None).get_structure_by_material_id("mp-856") condenser =
 StructureCondenser() describer = StructureDescriber() condensed_structure =
 condenser.condense_structure(structure) description = describer.describe
 (condensed_structure) ``` Where `structure` is a pymatgen Structure object.
 Both classes have many options for customising the output of the structure
 descriptions. More information is provided in the [module documentation](https:
 //hackingmaterials.github.io/robocrystallographer/modules). ### Intermediate
 JSON format The format of the intermediate JSON representation is detailed on
```

### Comparing `robocrys-0.2.8/README.md` & `robocrys-0.2.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -51,16 +51,16 @@
 from pymatgen import Structure
 from robocrys import StructureCondenser, StructureDescriber
 
 structure = Structure.from_file("my_structure.cif") # other file formats also supported
 
 # alternatively, uncomment the lines below to use the MPRester object
 # to fetch structures from the Materials Project database
-# from pymatgen import MPRester
-# structure = MPRester(API_KEY=None).get_structure_by_material_id("mp-856")
+# from mp_api.client import MPRester
+# structure = MPRester(api_key=None).get_structure_by_material_id("mp-856")
 
 condenser = StructureCondenser()
 describer = StructureDescriber()
 
 condensed_structure = condenser.condense_structure(structure)
 description = describer.describe(condensed_structure)
 ```
```

#### html2text {}

```diff
@@ -21,16 +21,16 @@
 condense the structure into an descriptive JSON representation. -
 `StructureDescriber`: to turn the condensed structure into a text description.
 A minimal working example for generating text descriptions is simply: ```python
 from pymatgen import Structure from robocrys import StructureCondenser,
 StructureDescriber structure = Structure.from_file("my_structure.cif") # other
 file formats also supported # alternatively, uncomment the lines below to use
 the MPRester object #Â to fetch structures from the Materials Project database
-# from pymatgen import MPRester # structure = MPRester
-(API_KEY=None).get_structure_by_material_id("mp-856") condenser =
+# from mp_api.client import MPRester # structure = MPRester
+(api_key=None).get_structure_by_material_id("mp-856") condenser =
 StructureCondenser() describer = StructureDescriber() condensed_structure =
 condenser.condense_structure(structure) description = describer.describe
 (condensed_structure) ``` Where `structure` is a pymatgen Structure object.
 Both classes have many options for customising the output of the structure
 descriptions. More information is provided in the [module documentation](https:
 //hackingmaterials.github.io/robocrystallographer/modules). ### Intermediate
 JSON format The format of the intermediate JSON representation is detailed on
```

### Comparing `robocrys-0.2.8/robocrys/adapter.py` & `robocrys-0.2.9/robocrys/adapter.py`

 * *Files identical despite different names*

### Comparing `robocrys-0.2.8/robocrys/cli.py` & `robocrys-0.2.9/robocrys/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from __future__ import annotations
 
 import argparse
 import sys
 import warnings
 
 from pymatgen.core.structure import Structure
-from pymatgen.ext.matproj import MPRestError
+from mp_api.client import MPRestError
 
 from robocrys import StructureCondenser, StructureDescriber, __version__
 
 __author__ = "Alex Ganose"
 __maintainer__ = "Alex Ganose"
 __email__ = "aganose@lbl.gov"
 __date__ = "December 17, 2018"
@@ -206,22 +206,20 @@
     warnings.filterwarnings("ignore", category=DeprecationWarning)
 
     try:
         structure = Structure.from_file(args.filename)
 
     except FileNotFoundError:
         if args.filename[:3] in ["mp-", "mvc"]:
-            from pymatgen.ext.matproj import MPRester
+            from mp_api.client import MPRester
 
             mpr = MPRester(args.api_key)
 
             try:
-                structure = mpr.get_entry_by_material_id(
-                    args.filename, inc_structure="final"
-                ).structure
+                structure = mpr.get_structure_by_material_id(args.filename)
             except IndexError:
                 print("filename or mp-id not found.")
                 sys.exit()
             except MPRestError as e:
                 if "API_KEY is not supplied" in str(e):
                     print(
                         "Materials project API key not set. Use the the "
```

### Comparing `robocrys-0.2.8/robocrys/condense/component.py` & `robocrys-0.2.9/robocrys/condense/component.py`

 * *Files identical despite different names*

### Comparing `robocrys-0.2.8/robocrys/condense/condenser.py` & `robocrys-0.2.9/robocrys/condense/condenser.py`

 * *Files identical despite different names*

### Comparing `robocrys-0.2.8/robocrys/condense/fingerprint.py` & `robocrys-0.2.9/robocrys/condense/fingerprint.py`

 * *Files identical despite different names*

### Comparing `robocrys-0.2.8/robocrys/condense/formula_db.json.gz` & `robocrys-0.2.9/robocrys/condense/formula_db.json.gz`

 * *Files identical despite different names*

### Comparing `robocrys-0.2.8/robocrys/condense/mineral.py` & `robocrys-0.2.9/robocrys/condense/mineral.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from __future__ import annotations
 
 from itertools import islice
 from typing import Any
 
 import numpy as np
 from matminer.utils.io import load_dataframe_from_json
-from pkg_resources import resource_filename
+from importlib.resources import files as import_resource_file
 from pymatgen.analysis.prototypes import AflowPrototypeMatcher
 from pymatgen.core.structure import IStructure
 
 from robocrys.condense.fingerprint import (
     get_fingerprint_distance,
     get_structure_fingerprint,
 )
@@ -46,15 +46,15 @@
         self,
         initial_ltol: float = 0.2,
         initial_stol: float = 0.3,
         initial_angle_tol: float = 5.0,
         use_fingerprint_matching: bool = True,
         fingerprint_distance_cutoff: float = 0.4,
     ):
-        db_file = resource_filename("robocrys.condense", "mineral_db.json.gz")
+        db_file = import_resource_file("robocrys.condense") / "mineral_db.json.gz"
         self.mineral_db = load_dataframe_from_json(db_file)
         self.initial_ltol = initial_ltol
         self.initial_stol = initial_stol
         self.initial_angle_tol = initial_angle_tol
         self.fingerprint_distance_cutoff = fingerprint_distance_cutoff
         self.use_fingerprint_matching = use_fingerprint_matching
         self._structure = None
```

### Comparing `robocrys-0.2.8/robocrys/condense/mineral_db.json.gz` & `robocrys-0.2.9/robocrys/condense/mineral_db.json.gz`

 * *Files identical despite different names*

### Comparing `robocrys-0.2.8/robocrys/condense/molecule.py` & `robocrys-0.2.9/robocrys/condense/molecule.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 Some functionality relies on having a working internet connection.
 """
 from __future__ import annotations
 
 import warnings
 
 from monty.serialization import loadfn
-from pkg_resources import resource_filename
+from importlib.resources import files as import_resource_file
 from pubchempy import BadRequestError, get_compounds
 from pymatgen.analysis.graphs import MoleculeGraph
 from pymatgen.io.babel import BabelMolAdaptor
 
 
 class MoleculeNamer:
     name_sources = ("traditional", "iupac")
@@ -30,15 +30,15 @@
                 connection and for the ``pubchempy`` package to be installed.
             name_preference: The order of preference for determining compound
                 names. Options are "traditional", and "iupac". If the
                 first option is not available, the subsequent options will be
                 used. Should be provided as a tuple of options, from 1st choice
                 to last.
         """
-        db_file = resource_filename("robocrys.condense", "molecule_db.json.gz")
+        db_file = import_resource_file("robocrys.condense") / "molecule_db.json.gz"
         self.molecule_db = loadfn(db_file)
         self.matched_molecules = {}
         self.use_online_pubchem = use_online_pubchem
 
         # append the sources list to the end in case the user only supplies
         # a single preference
         self.name_preference = tuple(list(name_preference) + list(self.name_sources))
```

### Comparing `robocrys-0.2.8/robocrys/condense/molecule_db.json.gz` & `robocrys-0.2.9/robocrys/condense/molecule_db.json.gz`

 * *Files identical despite different names*

### Comparing `robocrys-0.2.8/robocrys/condense/site.py` & `robocrys-0.2.9/robocrys/condense/site.py`

 * *Files 1% similar despite different names*

```diff
@@ -143,16 +143,16 @@
             with the format::
 
                 {'element': el, 'dist': distance}
 
             If ``inc_inequivalent_site_index=True``, the data will have an
             additional key ``'inequiv_index'`` corresponding to the inequivalent
             site index. E.g. if two sites are structurally/symmetrically
-            equivalent (depending on the value of ``self.use_symmetry_equivalent_sites`` then
-            they will have the same ``inequiv_index``.
+            equivalent (depending on the value of ``self.use_symmetry_equivalent_sites``
+            then they will have the same ``inequiv_index``.
         """
         nn_sites = self.bonded_structure.get_connected_sites(site_index)
 
         if inc_inequivalent_site_index:
             return [
                 {
                     "element": str(site.site.specie),
@@ -191,16 +191,16 @@
             a :obj:`list` of :obj:`int`. Multiple bond angles are given when
             the two sites share more than nearest neighbor (e.g. if they are
             face-sharing or edge-sharing). The ``distance`` property gives the
             distance between the site and the next nearest neighbor.
             If ``inc_inequivalent_site_index=True``, the data will have an
             additional key ``'inequiv_index'`` corresponding to the inequivalent
             site index. E.g. if two sites are structurally/symmetrically
-            equivalent (depending on the value of ``self.use_symmetry_equivalent_sites`` then
-            they will have the same ``inequiv_index``.
+            equivalent (depending on the value of ``self.use_symmetry_equivalent_sites``
+            then they will have the same ``inequiv_index``.
         """
 
         def get_coords(a_site_index, a_site_image):
             return np.asarray(
                 self.bonded_structure.structure.lattice.get_cartesian_coords(
                     self.bonded_structure.structure.frac_coords[a_site_index]
                     + a_site_image
```

### Comparing `robocrys-0.2.8/robocrys/condense/tests/test_component.py` & `robocrys-0.2.9/robocrys/condense/tests/test_component.py`

 * *Files identical despite different names*

### Comparing `robocrys-0.2.8/robocrys/condense/tests/test_fingerprint.py` & `robocrys-0.2.9/robocrys/condense/tests/test_fingerprint.py`

 * *Files identical despite different names*

### Comparing `robocrys-0.2.8/robocrys/condense/tests/test_mineral.py` & `robocrys-0.2.9/robocrys/condense/tests/test_mineral.py`

 * *Files identical despite different names*

### Comparing `robocrys-0.2.8/robocrys/condense/tests/test_molecule.py` & `robocrys-0.2.9/robocrys/condense/tests/test_molecule.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,24 @@
 from __future__ import annotations
 
 import os
 
+import pytest
 from pymatgen.analysis.dimensionality import get_structure_components
 from pymatgen.analysis.local_env import CrystalNN
 
 from robocrys.condense.component import filter_molecular_components
 from robocrys.condense.molecule import MoleculeNamer
 from robocrys.tests import RobocrysTest
 
+try:
+    from openbabel import openbabel, pybel
+except Exception:
+    openbabel = None
+
 test_dir = os.path.join(os.path.dirname(__file__))
 
 
 class TestMoleculeMatcher(RobocrysTest):
     """Class to test component related functions."""
 
     def setUp(self):
@@ -27,25 +33,28 @@
         """Test initialising MoleculeNamer."""
         mn = MoleculeNamer()
         assert mn
 
         mn = MoleculeNamer(use_online_pubchem=False)
         assert mn
 
+    @pytest.mark.skipif(not openbabel, reason="Openbabel not installed.")
     def test_molecule_graph_to_smiles(self):
         """Test converting a molecule graph to SMILES string."""
         smiles = MoleculeNamer.molecule_graph_to_smiles(self.methylammonium)
         assert smiles == "C[NH3]"
 
+    @pytest.mark.skipif(not openbabel, reason="Openbabel not installed.")
     def test_get_name_from_pubchem(self):
         """Test downloading the molecule name from Pubchem."""
         mn = MoleculeNamer()
         name = mn.get_name_from_pubchem("C[NH3]")
         assert name == "methylammonium"
 
+    @pytest.mark.skipif(not openbabel, reason="Openbabel not installed.")
     def test_get_name_from_molecule_graph(self):
         """Test getting a molecule name from the molecule graph."""
         mn = MoleculeNamer()
         name = mn.get_name_from_molecule_graph(self.methylammonium)
         assert name == "methylammonium"
 
         # test iupac naming source
```

### Comparing `robocrys-0.2.8/robocrys/condense/tests/test_site.py` & `robocrys-0.2.9/robocrys/condense/tests/test_site.py`

 * *Files identical despite different names*

### Comparing `robocrys-0.2.8/robocrys/condense/tests/test_structure.py` & `robocrys-0.2.9/robocrys/condense/tests/test_structure.py`

 * *Files identical despite different names*

### Comparing `robocrys-0.2.8/robocrys/describe/adapter.py` & `robocrys-0.2.9/robocrys/describe/adapter.py`

 * *Files identical despite different names*

### Comparing `robocrys-0.2.8/robocrys/describe/describer.py` & `robocrys-0.2.9/robocrys/describe/describer.py`

 * *Files 0% similar despite different names*

```diff
@@ -236,15 +236,15 @@
                 elif self.fmt == "html":
                     formula = htmlify(formula)
 
                 comp_desc = f"{s_count} {formula} {shape}"
 
                 if component_group.dimensionality in [1, 2]:
                     orientations = list(
-                        {c.orientation for c in component_group.components}
+                        {str(c.orientation) for c in component_group.components}
                     )
                     s_direction = en.plural("direction", len(orientations))
                     comp_desc += " oriented in the {} {}".format(
                         en.join(orientations), s_direction
                     )
 
                 component_makeup_summaries.append(comp_desc)
```

### Comparing `robocrys-0.2.8/robocrys/describe/tests/test_adapter.py` & `robocrys-0.2.9/robocrys/describe/tests/test_adapter.py`

 * *Files identical despite different names*

### Comparing `robocrys-0.2.8/robocrys/describe/tests/test_description.py` & `robocrys-0.2.9/robocrys/describe/tests/test_description.py`

 * *Files identical despite different names*

### Comparing `robocrys-0.2.8/robocrys/featurize/adapter.py` & `robocrys-0.2.9/robocrys/featurize/adapter.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """This module implements a class to resolve the symbolic references in condensed
 structure data.
 """
 from __future__ import annotations
 
-import collections
+from collections.abc import Iterable
 from statistics import mean
 from typing import Any
 
 from robocrys.adapter import BaseAdapter
 
 
 class FeaturizerAdapter(BaseAdapter):
@@ -172,34 +172,27 @@
         Returns:
             Whether the structure contains the molecule.
         """
         return any(
             c["molecule_name"] == molecule_name for c in self.components.values()
         )
 
-    def is_dimensionality(
-        self, dimensionalities: int | list[int] | set[int]
-    ) -> bool:
+    def is_dimensionality(self, dimensionalities: int | list[int] | set[int]) -> bool:
         """Whether the structure only contains the specified dimensionalities.
 
         Args:
             dimensionalities: One or more dimensionalities.
 
         Returns:
             Whether the structure only contains the specified dimensionalities.
 
         """
-        try:
-            iterable = collections.Iterable
-        except:
-            iterable = collections.abc.Iterable
-
         if isinstance(dimensionalities, set):
             set_dimensionalities = dimensionalities
-        elif isinstance(dimensionalities, iterable):
+        elif isinstance(dimensionalities, Iterable):
             set_dimensionalities = set(dimensionalities)
         else:
             set_dimensionalities = {dimensionalities}
         return set(self.component_dimensionalities) == set_dimensionalities
 
     def contains_geometry_type(
         self, geometry: str, distorted: bool | None = None
```

### Comparing `robocrys-0.2.8/robocrys/featurize/featurizer.py` & `robocrys-0.2.9/robocrys/featurize/featurizer.py`

 * *Files identical despite different names*

### Comparing `robocrys-0.2.8/robocrys/tests/__init__.py` & `robocrys-0.2.9/robocrys/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `robocrys-0.2.8/robocrys/tests/adapter.py` & `robocrys-0.2.9/robocrys/tests/adapter.py`

 * *Files identical despite different names*

### Comparing `robocrys-0.2.8/robocrys/tests/test_util.py` & `robocrys-0.2.9/robocrys/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `robocrys-0.2.8/robocrys/util.py` & `robocrys-0.2.9/robocrys/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,20 +15,20 @@
 
 import re
 from collections import defaultdict
 from typing import Any
 
 from monty.json import MontyDecoder
 from monty.serialization import loadfn
-from pkg_resources import resource_filename
+from importlib.resources import files as import_resource_file
 from pymatgen.core.periodic_table import Element, Species, get_el_sp
 from pymatgen.util.string import latexify_spacegroup
 
 common_formulas: dict[str, str] = loadfn(
-    resource_filename("robocrys.condense", "formula_db.json.gz")
+    import_resource_file("robocrys.condense") / "formula_db.json.gz"
 )
 
 connected_geometries: list[str] = [
     "tetrahedral",
     "octahedral",
     "trigonal pyramidal",
     "square pyramidal",
@@ -281,13 +281,14 @@
 
     Returns:
         The condensed structure data.
     """
 
     # JSON does not support using integers a dictionary keys, therefore
     # manually convert dictionary keys from str to int if possible.
-    def json_keys_to_int(x):
-        if isinstance(x, dict):
-            return {int(k) if k.isdigit() else k: v for k, v in x.items()}
-        return None
-
-    return loadfn(filename, cls=MontyDecoder, object_hook=json_keys_to_int)
+    def json_keys_to_int(x : Any) -> Any:
+        if isinstance(x,dict):
+            return {int(k) if k.isdigit() else k: json_keys_to_int(v) for k, v in x.items()}
+        return x
+    # For some reason, specifying `object_hook = json_keys_to_int` in `loadfn`
+    # doesn't seem to work. This does reliably:
+    return json_keys_to_int(loadfn(filename, cls=MontyDecoder))
```

### Comparing `robocrys-0.2.8/robocrys.egg-info/PKG-INFO` & `robocrys-0.2.9/robocrys.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robocrys
-Version: 0.2.8
+Version: 0.2.9
 Summary: Automatic generation of crystal structure descriptions
 Home-page: https://github.com/hackingmaterials/robocrystallographer
 Author: Alex Ganose
 Author-email: aganose@lbl.gov
 License: modified BSD
 Keywords: crystal-structure crystallography materials-science
 Platform: UNKNOWN
@@ -83,16 +83,16 @@
 from pymatgen import Structure
 from robocrys import StructureCondenser, StructureDescriber
 
 structure = Structure.from_file("my_structure.cif") # other file formats also supported
 
 # alternatively, uncomment the lines below to use the MPRester object
 # to fetch structures from the Materials Project database
-# from pymatgen import MPRester
-# structure = MPRester(API_KEY=None).get_structure_by_material_id("mp-856")
+# from mp_api.client import MPRester
+# structure = MPRester(api_key=None).get_structure_by_material_id("mp-856")
 
 condenser = StructureCondenser()
 describer = StructureDescriber()
 
 condensed_structure = condenser.condense_structure(structure)
 description = describer.describe(condensed_structure)
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: robocrys Version: 0.2.8 Summary: Automatic
+Metadata-Version: 2.1 Name: robocrys Version: 0.2.9 Summary: Automatic
 generation of crystal structure descriptions Home-page: https://github.com/
 hackingmaterials/robocrystallographer Author: Alex Ganose Author-email:
 aganose@lbl.gov License: modified BSD Keywords: crystal-structure
 crystallography materials-science Platform: UNKNOWN Classifier: Development
 Status :: 3 - Alpha Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Information Technology Classifier: License ::
 OSI Approved :: MIT License Classifier: Natural Language :: English Classifier:
@@ -37,16 +37,16 @@
 condense the structure into an descriptive JSON representation. -
 `StructureDescriber`: to turn the condensed structure into a text description.
 A minimal working example for generating text descriptions is simply: ```python
 from pymatgen import Structure from robocrys import StructureCondenser,
 StructureDescriber structure = Structure.from_file("my_structure.cif") # other
 file formats also supported # alternatively, uncomment the lines below to use
 the MPRester object #Â to fetch structures from the Materials Project database
-# from pymatgen import MPRester # structure = MPRester
-(API_KEY=None).get_structure_by_material_id("mp-856") condenser =
+# from mp_api.client import MPRester # structure = MPRester
+(api_key=None).get_structure_by_material_id("mp-856") condenser =
 StructureCondenser() describer = StructureDescriber() condensed_structure =
 condenser.condense_structure(structure) description = describer.describe
 (condensed_structure) ``` Where `structure` is a pymatgen Structure object.
 Both classes have many options for customising the output of the structure
 descriptions. More information is provided in the [module documentation](https:
 //hackingmaterials.github.io/robocrystallographer/modules). ### Intermediate
 JSON format The format of the intermediate JSON representation is detailed on
```

### Comparing `robocrys-0.2.8/robocrys.egg-info/SOURCES.txt` & `robocrys-0.2.9/robocrys.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `robocrys-0.2.8/setup.py` & `robocrys-0.2.9/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 """"
 robocrystallographer: Automatic generation of crystal structure descriptions.
+
 """
 from __future__ import annotations
 
 from os.path import join as path_join
 
 from setuptools import find_packages, setup
 
 with open("README.md") as file:
     long_description = file.read()
 
-version = open("robocrys/_version.py").readlines()[-1].split()[-1].strip("\"'")
+with open("robocrys/_version.py") as file:
+    version = file.readlines()[-1].split()[-1].strip("\"'")
 
 setup(
     name="robocrys",
     version=version,
     description="Automatic generation of crystal structure descriptions",
     url="https://github.com/hackingmaterials/robocrystallographer",
     author="Alex Ganose",
@@ -41,22 +43,23 @@
     keywords="crystal-structure crystallography materials-science",
     test_suite="nose.collector",
     packages=find_packages(),
     install_requires=[
         "spglib",
         "numpy",
         "scipy",
-        "pymatgen>=2020.10.20",
+        "pymatgen",
         "inflect",
         "networkx",
-        "matminer",
+        "matminer>=0.9.2",
         "monty",
         "pubchempy",
         "pybtex",
         "ruamel.yaml",
+        "mp-api"
     ],
     extras_require={
         "docs": [
             "sphinx==5.3.0",
             "sphinx-argparse==0.4.0",
             "sphinx_rtd_theme==1.2.0",
             "sphinx-autodoc-typehints==1.23.0",
```


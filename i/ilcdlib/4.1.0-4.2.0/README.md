# Comparing `tmp/ilcdlib-4.1.0.tar.gz` & `tmp/ilcdlib-4.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ilcdlib-4.1.0.tar", max compression
+gzip compressed data, was "ilcdlib-4.2.0.tar", max compression
```

## Comparing `ilcdlib-4.1.0.tar` & `ilcdlib-4.2.0.tar`

### file list

```diff
@@ -1,61 +1,62 @@
--rw-r--r--   0        0        0    11357 2024-04-16 15:22:15.327666 ilcdlib-4.1.0/LICENSE
--rw-r--r--   0        0        0     4949 2024-04-16 15:22:15.327666 ilcdlib-4.1.0/README.md
--rw-r--r--   0        0        0     3525 2024-04-16 15:22:15.331667 ilcdlib-4.1.0/pyproject.toml
--rw-r--r--   0        0        0      837 2024-04-16 15:22:15.331667 ilcdlib-4.1.0/src/ilcdlib/__init__.py
--rw-r--r--   0        0        0      910 2024-04-16 15:22:15.331667 ilcdlib-4.1.0/src/ilcdlib/__main__.py
--rw-r--r--   0        0        0      855 2024-04-16 15:22:15.331667 ilcdlib-4.1.0/src/ilcdlib/__version__.py
--rw-r--r--   0        0        0     2959 2024-04-16 15:22:15.331667 ilcdlib-4.1.0/src/ilcdlib/cli.py
--rw-r--r--   0        0        0    17587 2024-04-16 15:22:15.331667 ilcdlib-4.1.0/src/ilcdlib/common.py
--rw-r--r--   0        0        0      837 2024-04-16 15:22:15.331667 ilcdlib-4.1.0/src/ilcdlib/compat/__init__.py
--rw-r--r--   0        0        0     1158 2024-04-16 15:22:15.331667 ilcdlib-4.1.0/src/ilcdlib/compat/pydantic.py
--rw-r--r--   0        0        0     1796 2024-04-16 15:22:15.331667 ilcdlib-4.1.0/src/ilcdlib/const.py
--rw-r--r--   0        0        0   172140 2024-04-16 15:22:15.331667 ilcdlib-4.1.0/src/ilcdlib/data/ilcd_epd_ref.zip
--rw-r--r--   0        0        0     4407 2024-04-16 15:22:15.331667 ilcdlib-4.1.0/src/ilcdlib/dto.py
--rw-r--r--   0        0        0      837 2024-04-16 15:22:15.331667 ilcdlib-4.1.0/src/ilcdlib/entity/__init__.py
--rw-r--r--   0        0        0     6946 2024-04-16 15:22:15.331667 ilcdlib-4.1.0/src/ilcdlib/entity/base_scope_set_reader.py
--rw-r--r--   0        0        0     3361 2024-04-16 15:22:15.331667 ilcdlib-4.1.0/src/ilcdlib/entity/category.py
--rw-r--r--   0        0        0     3052 2024-04-16 15:22:15.331667 ilcdlib-4.1.0/src/ilcdlib/entity/compliance.py
--rw-r--r--   0        0        0     6003 2024-04-16 15:22:15.331667 ilcdlib-4.1.0/src/ilcdlib/entity/contact.py
--rw-r--r--   0        0        0     4160 2024-04-16 15:22:15.331667 ilcdlib-4.1.0/src/ilcdlib/entity/exchage.py
--rw-r--r--   0        0        0     7981 2024-04-16 15:22:15.331667 ilcdlib-4.1.0/src/ilcdlib/entity/flow.py
--rw-r--r--   0        0        0     4230 2024-04-16 15:22:15.331667 ilcdlib-4.1.0/src/ilcdlib/entity/lcia.py
--rw-r--r--   0        0        0     5213 2024-04-16 15:22:15.331667 ilcdlib-4.1.0/src/ilcdlib/entity/material.py
--rw-r--r--   0        0        0     3930 2024-04-16 15:22:15.331667 ilcdlib-4.1.0/src/ilcdlib/entity/pcr.py
--rw-r--r--   0        0        0     3437 2024-04-16 15:22:15.331667 ilcdlib-4.1.0/src/ilcdlib/entity/source.py
--rw-r--r--   0        0        0     3797 2024-04-16 15:22:15.331667 ilcdlib-4.1.0/src/ilcdlib/entity/unit.py
--rw-r--r--   0        0        0     3331 2024-04-16 15:22:15.331667 ilcdlib-4.1.0/src/ilcdlib/entity/validation.py
--rw-r--r--   0        0        0      837 2024-04-16 15:22:15.331667 ilcdlib-4.1.0/src/ilcdlib/epd/__init__.py
--rw-r--r--   0        0        0    10064 2024-04-16 15:22:15.331667 ilcdlib-4.1.0/src/ilcdlib/epd/cli.py
--rw-r--r--   0        0        0      837 2024-04-16 15:22:15.331667 ilcdlib-4.1.0/src/ilcdlib/epd/dialect/__init__.py
--rw-r--r--   0        0        0     6864 2024-04-16 15:22:15.331667 ilcdlib-4.1.0/src/ilcdlib/epd/dialect/environdec.py
--rw-r--r--   0        0        0     2170 2024-04-16 15:22:15.331667 ilcdlib-4.1.0/src/ilcdlib/epd/dialect/epditaly.py
--rw-r--r--   0        0        0     1329 2024-04-16 15:22:15.331667 ilcdlib-4.1.0/src/ilcdlib/epd/dialect/indata.py
--rw-r--r--   0        0        0     2217 2024-04-16 15:22:15.331667 ilcdlib-4.1.0/src/ilcdlib/epd/dialect/oekobaudat.py
--rw-r--r--   0        0        0     3440 2024-04-16 15:22:15.331667 ilcdlib-4.1.0/src/ilcdlib/epd/factory.py
--rw-r--r--   0        0        0    32351 2024-04-16 15:22:15.331667 ilcdlib-4.1.0/src/ilcdlib/epd/reader.py
--rw-r--r--   0        0        0     2067 2024-04-16 15:22:15.331667 ilcdlib-4.1.0/src/ilcdlib/extension.py
--rw-r--r--   0        0        0     7667 2024-04-16 15:22:15.331667 ilcdlib-4.1.0/src/ilcdlib/http_common.py
--rw-r--r--   0        0        0      837 2024-04-16 15:22:15.331667 ilcdlib-4.1.0/src/ilcdlib/mapping/__init__.py
--rw-r--r--   0        0        0     1928 2024-04-16 15:22:15.331667 ilcdlib-4.1.0/src/ilcdlib/mapping/common.py
--rw-r--r--   0        0        0     1168 2024-04-16 15:22:15.331667 ilcdlib-4.1.0/src/ilcdlib/mapping/compliance.py
--rw-r--r--   0        0        0     1512 2024-04-16 15:22:15.331667 ilcdlib-4.1.0/src/ilcdlib/mapping/flows.py
--rw-r--r--   0        0        0     1892 2024-04-16 15:22:15.331667 ilcdlib-4.1.0/src/ilcdlib/mapping/impacts.py
--rw-r--r--   0        0        0     1651 2024-04-16 15:22:15.331667 ilcdlib-4.1.0/src/ilcdlib/mapping/indicators.py
--rw-r--r--   0        0        0     1212 2024-04-16 15:22:15.331667 ilcdlib-4.1.0/src/ilcdlib/mapping/properties.py
--rw-r--r--   0        0        0     2588 2024-04-16 15:22:15.331667 ilcdlib-4.1.0/src/ilcdlib/mapping/units.py
--rw-r--r--   0        0        0      837 2024-04-16 15:22:15.331667 ilcdlib-4.1.0/src/ilcdlib/medium/__init__.py
--rw-r--r--   0        0        0     7531 2024-04-16 15:22:15.331667 ilcdlib-4.1.0/src/ilcdlib/medium/archive.py
--rw-r--r--   0        0        0     6496 2024-04-16 15:22:15.331667 ilcdlib-4.1.0/src/ilcdlib/medium/soda4lca.py
--rw-r--r--   0        0        0        0 2024-04-16 15:22:15.335667 ilcdlib-4.1.0/src/ilcdlib/py.typed
--rw-r--r--   0        0        0     1435 2024-04-16 15:22:15.335667 ilcdlib-4.1.0/src/ilcdlib/reference_data.py
--rw-r--r--   0        0        0      837 2024-04-16 15:22:15.335667 ilcdlib-4.1.0/src/ilcdlib/sanitizing/__init__.py
--rw-r--r--   0        0        0     1735 2024-04-16 15:22:15.335667 ilcdlib-4.1.0/src/ilcdlib/sanitizing/domain.py
--rw-r--r--   0        0        0     1336 2024-04-16 15:22:15.335667 ilcdlib-4.1.0/src/ilcdlib/sanitizing/phone.py
--rw-r--r--   0        0        0     1122 2024-04-16 15:22:15.335667 ilcdlib-4.1.0/src/ilcdlib/sanitizing/text.py
--rw-r--r--   0        0        0      837 2024-04-16 15:22:15.335667 ilcdlib-4.1.0/src/ilcdlib/soda4lca/__init__.py
--rw-r--r--   0        0        0    10655 2024-04-16 15:22:15.335667 ilcdlib-4.1.0/src/ilcdlib/soda4lca/api_client.py
--rw-r--r--   0        0        0     2513 2024-04-16 15:22:15.335667 ilcdlib-4.1.0/src/ilcdlib/soda4lca/api_client_4x.py
--rw-r--r--   0        0        0     1206 2024-04-16 15:22:15.335667 ilcdlib-4.1.0/src/ilcdlib/type.py
--rw-r--r--   0        0        0     3682 2024-04-16 15:22:15.335667 ilcdlib-4.1.0/src/ilcdlib/utils.py
--rw-r--r--   0        0        0     2399 2024-04-16 15:22:15.335667 ilcdlib-4.1.0/src/ilcdlib/xml_parser.py
--rw-r--r--   0        0        0     6082 1970-01-01 00:00:00.000000 ilcdlib-4.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-25 13:24:54.049317 ilcdlib-4.2.0/LICENSE
+-rw-r--r--   0        0        0     4949 2024-04-25 13:24:54.049317 ilcdlib-4.2.0/README.md
+-rw-r--r--   0        0        0     3525 2024-04-25 13:24:54.049317 ilcdlib-4.2.0/pyproject.toml
+-rw-r--r--   0        0        0      837 2024-04-25 13:24:54.049317 ilcdlib-4.2.0/src/ilcdlib/__init__.py
+-rw-r--r--   0        0        0      910 2024-04-25 13:24:54.049317 ilcdlib-4.2.0/src/ilcdlib/__main__.py
+-rw-r--r--   0        0        0      855 2024-04-25 13:24:54.049317 ilcdlib-4.2.0/src/ilcdlib/__version__.py
+-rw-r--r--   0        0        0     2959 2024-04-25 13:24:54.049317 ilcdlib-4.2.0/src/ilcdlib/cli.py
+-rw-r--r--   0        0        0    17587 2024-04-25 13:24:54.049317 ilcdlib-4.2.0/src/ilcdlib/common.py
+-rw-r--r--   0        0        0      837 2024-04-25 13:24:54.049317 ilcdlib-4.2.0/src/ilcdlib/compat/__init__.py
+-rw-r--r--   0        0        0     1158 2024-04-25 13:24:54.049317 ilcdlib-4.2.0/src/ilcdlib/compat/pydantic.py
+-rw-r--r--   0        0        0     1796 2024-04-25 13:24:54.049317 ilcdlib-4.2.0/src/ilcdlib/const.py
+-rw-r--r--   0        0        0   172140 2024-04-25 13:24:54.049317 ilcdlib-4.2.0/src/ilcdlib/data/ilcd_epd_ref.zip
+-rw-r--r--   0        0        0     4407 2024-04-25 13:24:54.049317 ilcdlib-4.2.0/src/ilcdlib/dto.py
+-rw-r--r--   0        0        0      837 2024-04-25 13:24:54.049317 ilcdlib-4.2.0/src/ilcdlib/entity/__init__.py
+-rw-r--r--   0        0        0     7064 2024-04-25 13:24:54.049317 ilcdlib-4.2.0/src/ilcdlib/entity/base_scope_set_reader.py
+-rw-r--r--   0        0        0     3361 2024-04-25 13:24:54.049317 ilcdlib-4.2.0/src/ilcdlib/entity/category.py
+-rw-r--r--   0        0        0     3052 2024-04-25 13:24:54.049317 ilcdlib-4.2.0/src/ilcdlib/entity/compliance.py
+-rw-r--r--   0        0        0     6003 2024-04-25 13:24:54.049317 ilcdlib-4.2.0/src/ilcdlib/entity/contact.py
+-rw-r--r--   0        0        0     4173 2024-04-25 13:24:54.049317 ilcdlib-4.2.0/src/ilcdlib/entity/exchage.py
+-rw-r--r--   0        0        0     7981 2024-04-25 13:24:54.049317 ilcdlib-4.2.0/src/ilcdlib/entity/flow.py
+-rw-r--r--   0        0        0     4224 2024-04-25 13:24:54.049317 ilcdlib-4.2.0/src/ilcdlib/entity/lcia.py
+-rw-r--r--   0        0        0     5213 2024-04-25 13:24:54.049317 ilcdlib-4.2.0/src/ilcdlib/entity/material.py
+-rw-r--r--   0        0        0     3930 2024-04-25 13:24:54.049317 ilcdlib-4.2.0/src/ilcdlib/entity/pcr.py
+-rw-r--r--   0        0        0     3437 2024-04-25 13:24:54.049317 ilcdlib-4.2.0/src/ilcdlib/entity/source.py
+-rw-r--r--   0        0        0     3798 2024-04-25 13:24:54.049317 ilcdlib-4.2.0/src/ilcdlib/entity/unit.py
+-rw-r--r--   0        0        0     3331 2024-04-25 13:24:54.049317 ilcdlib-4.2.0/src/ilcdlib/entity/validation.py
+-rw-r--r--   0        0        0      837 2024-04-25 13:24:54.049317 ilcdlib-4.2.0/src/ilcdlib/epd/__init__.py
+-rw-r--r--   0        0        0    10064 2024-04-25 13:24:54.053317 ilcdlib-4.2.0/src/ilcdlib/epd/cli.py
+-rw-r--r--   0        0        0      837 2024-04-25 13:24:54.053317 ilcdlib-4.2.0/src/ilcdlib/epd/dialect/__init__.py
+-rw-r--r--   0        0        0     6864 2024-04-25 13:24:54.053317 ilcdlib-4.2.0/src/ilcdlib/epd/dialect/environdec.py
+-rw-r--r--   0        0        0     2170 2024-04-25 13:24:54.053317 ilcdlib-4.2.0/src/ilcdlib/epd/dialect/epditaly.py
+-rw-r--r--   0        0        0     1329 2024-04-25 13:24:54.053317 ilcdlib-4.2.0/src/ilcdlib/epd/dialect/indata.py
+-rw-r--r--   0        0        0     1156 2024-04-25 13:24:54.053317 ilcdlib-4.2.0/src/ilcdlib/epd/dialect/itb.py
+-rw-r--r--   0        0        0     2217 2024-04-25 13:24:54.053317 ilcdlib-4.2.0/src/ilcdlib/epd/dialect/oekobaudat.py
+-rw-r--r--   0        0        0     3532 2024-04-25 13:24:54.053317 ilcdlib-4.2.0/src/ilcdlib/epd/factory.py
+-rw-r--r--   0        0        0    32351 2024-04-25 13:24:54.053317 ilcdlib-4.2.0/src/ilcdlib/epd/reader.py
+-rw-r--r--   0        0        0     2067 2024-04-25 13:24:54.053317 ilcdlib-4.2.0/src/ilcdlib/extension.py
+-rw-r--r--   0        0        0     7667 2024-04-25 13:24:54.053317 ilcdlib-4.2.0/src/ilcdlib/http_common.py
+-rw-r--r--   0        0        0      837 2024-04-25 13:24:54.053317 ilcdlib-4.2.0/src/ilcdlib/mapping/__init__.py
+-rw-r--r--   0        0        0     2669 2024-04-25 13:24:54.053317 ilcdlib-4.2.0/src/ilcdlib/mapping/common.py
+-rw-r--r--   0        0        0     1168 2024-04-25 13:24:54.053317 ilcdlib-4.2.0/src/ilcdlib/mapping/compliance.py
+-rw-r--r--   0        0        0     1512 2024-04-25 13:24:54.053317 ilcdlib-4.2.0/src/ilcdlib/mapping/flows.py
+-rw-r--r--   0        0        0     3128 2024-04-25 13:24:54.053317 ilcdlib-4.2.0/src/ilcdlib/mapping/impacts.py
+-rw-r--r--   0        0        0     1651 2024-04-25 13:24:54.053317 ilcdlib-4.2.0/src/ilcdlib/mapping/indicators.py
+-rw-r--r--   0        0        0     1212 2024-04-25 13:24:54.053317 ilcdlib-4.2.0/src/ilcdlib/mapping/properties.py
+-rw-r--r--   0        0        0     2588 2024-04-25 13:24:54.053317 ilcdlib-4.2.0/src/ilcdlib/mapping/units.py
+-rw-r--r--   0        0        0      837 2024-04-25 13:24:54.053317 ilcdlib-4.2.0/src/ilcdlib/medium/__init__.py
+-rw-r--r--   0        0        0     7531 2024-04-25 13:24:54.053317 ilcdlib-4.2.0/src/ilcdlib/medium/archive.py
+-rw-r--r--   0        0        0     6496 2024-04-25 13:24:54.053317 ilcdlib-4.2.0/src/ilcdlib/medium/soda4lca.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:24:54.053317 ilcdlib-4.2.0/src/ilcdlib/py.typed
+-rw-r--r--   0        0        0     1435 2024-04-25 13:24:54.053317 ilcdlib-4.2.0/src/ilcdlib/reference_data.py
+-rw-r--r--   0        0        0      837 2024-04-25 13:24:54.053317 ilcdlib-4.2.0/src/ilcdlib/sanitizing/__init__.py
+-rw-r--r--   0        0        0     1735 2024-04-25 13:24:54.053317 ilcdlib-4.2.0/src/ilcdlib/sanitizing/domain.py
+-rw-r--r--   0        0        0     1336 2024-04-25 13:24:54.053317 ilcdlib-4.2.0/src/ilcdlib/sanitizing/phone.py
+-rw-r--r--   0        0        0     1122 2024-04-25 13:24:54.053317 ilcdlib-4.2.0/src/ilcdlib/sanitizing/text.py
+-rw-r--r--   0        0        0      837 2024-04-25 13:24:54.053317 ilcdlib-4.2.0/src/ilcdlib/soda4lca/__init__.py
+-rw-r--r--   0        0        0    10951 2024-04-25 13:24:54.053317 ilcdlib-4.2.0/src/ilcdlib/soda4lca/api_client.py
+-rw-r--r--   0        0        0     2770 2024-04-25 13:24:54.053317 ilcdlib-4.2.0/src/ilcdlib/soda4lca/api_client_4x.py
+-rw-r--r--   0        0        0     1206 2024-04-25 13:24:54.053317 ilcdlib-4.2.0/src/ilcdlib/type.py
+-rw-r--r--   0        0        0     3951 2024-04-25 13:24:54.053317 ilcdlib-4.2.0/src/ilcdlib/utils.py
+-rw-r--r--   0        0        0     2399 2024-04-25 13:24:54.053317 ilcdlib-4.2.0/src/ilcdlib/xml_parser.py
+-rw-r--r--   0        0        0     6082 1970-01-01 00:00:00.000000 ilcdlib-4.2.0/PKG-INFO
```

### Comparing `ilcdlib-4.1.0/LICENSE` & `ilcdlib-4.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.1.0/README.md` & `ilcdlib-4.2.0/README.md`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.1.0/pyproject.toml` & `ilcdlib-4.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ilcdlib"
-version = "4.1.0"
+version = "4.2.0"
 license = "Apache-2.0"
 description = "A toolkit for reading and writing ILCD format and it's derivatives"
 authors = ["C-Change Labs <support@c-change-labs.com>"]
 maintainers = ["C-Change Labs <open-source@c-change-labs.com>"]
 repository = "https://github.com/cchangelabs/ilcdlib"
 keywords = []
 classifiers = [
```

### Comparing `ilcdlib-4.1.0/src/ilcdlib/__init__.py` & `ilcdlib-4.2.0/src/ilcdlib/__init__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.1.0/src/ilcdlib/__main__.py` & `ilcdlib-4.2.0/src/ilcdlib/__main__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.1.0/src/ilcdlib/__version__.py` & `ilcdlib-4.2.0/src/ilcdlib/__version__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.1.0/src/ilcdlib/cli.py` & `ilcdlib-4.2.0/src/ilcdlib/cli.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.1.0/src/ilcdlib/common.py` & `ilcdlib-4.2.0/src/ilcdlib/common.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.1.0/src/ilcdlib/compat/__init__.py` & `ilcdlib-4.2.0/src/ilcdlib/compat/__init__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.1.0/src/ilcdlib/compat/pydantic.py` & `ilcdlib-4.2.0/src/ilcdlib/compat/pydantic.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.1.0/src/ilcdlib/const.py` & `ilcdlib-4.2.0/src/ilcdlib/const.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.1.0/src/ilcdlib/data/ilcd_epd_ref.zip` & `ilcdlib-4.2.0/src/ilcdlib/data/ilcd_epd_ref.zip`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.1.0/src/ilcdlib/dto.py` & `ilcdlib-4.2.0/src/ilcdlib/dto.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.1.0/src/ilcdlib/entity/__init__.py` & `ilcdlib-4.2.0/src/ilcdlib/entity/__init__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.1.0/src/ilcdlib/entity/base_scope_set_reader.py` & `ilcdlib-4.2.0/src/ilcdlib/entity/base_scope_set_reader.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 from openepd.model.base import BaseOpenEpdSchema
 from openepd.model.common import Measurement
 from openepd.model.lcia import EolScenario, ScopeSet
 
 from ilcdlib.common import BaseIlcdMediumSpecificReader, IlcdXmlReader, XmlPath
 from ilcdlib.entity.unit import IlcdUnitGroupReader
-from ilcdlib.mapping.common import SimpleDataMapper
+from ilcdlib.mapping.common import BaseDataMapper
 from ilcdlib.xml_parser import T_ET
 
 
 class BaseIlcdScopeSetsReader(IlcdXmlReader):
     """Read scope sets from XML file."""
 
     def __init__(
@@ -43,29 +43,32 @@
         self._entity = element
         self.unit_group_reader_cls = unit_group_reader_cls
 
     def _get_scope_set_for_el(
         self,
         el: T_ET.Element,
         reference_data_set: XmlPath,
-        mapper: SimpleDataMapper[str],
+        mapper: BaseDataMapper[str, str],
         scenario_names: dict[str, str],
-        scope_to_units_mapper: SimpleDataMapper[str],
+        scope_to_units_mapper: BaseDataMapper[str, str],
     ) -> tuple[ScopeSet, str] | None:
         """Extract all scope set information from element."""
         # Impact name
         type_el = self._get_el(el, reference_data_set)
         if type_el is None:
             return None
         type_uuid = type_el.attrib.get("refObjectId") if type_el is not None else None
         if type_uuid is None:
             return None
         impact_name: str | None = mapper.map(type_uuid, type_uuid)
         if impact_name == type_uuid:
-            impact_name = self._get_localized_text(type_el, ("common:shortDescription",), ("en", None))
+            description = self._get_localized_text(type_el, ("common:shortDescription",), ("en", None))
+            if description is not None:
+                impact_name = mapper.map(description, description)
+
         if impact_name is None:
             return None
         unit_el = self._get_external_tree(
             el,
             (
                 "common:other",
                 "epd2013:referenceToUnitGroupDataSet",
@@ -151,17 +154,17 @@
     def _extract_and_set_scope_set(
         self,
         el: T_ET.Element,
         reference_path: XmlPath,
         scope_set_type: Type[BaseOpenEpdSchema],
         scope_set_dict: dict[str, ScopeSet | dict],
         ext: dict[str, ScopeSet],
-        mapper: SimpleDataMapper[str],
+        mapper: BaseDataMapper[str, str],
         scenario_names: dict[str, str],
-        scope_to_units_mapper: SimpleDataMapper[str],
+        scope_to_units_mapper: BaseDataMapper[str, str],
     ) -> None:
         """Extract scope set from element and set to its dictionary."""
         scope_set_and_impact_name = self._get_scope_set_for_el(
             el, reference_path, mapper, scenario_names, scope_to_units_mapper
         )
         if scope_set_and_impact_name is None:
             return None
```

### Comparing `ilcdlib-4.1.0/src/ilcdlib/entity/category.py` & `ilcdlib-4.2.0/src/ilcdlib/entity/category.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.1.0/src/ilcdlib/entity/compliance.py` & `ilcdlib-4.2.0/src/ilcdlib/entity/compliance.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.1.0/src/ilcdlib/entity/contact.py` & `ilcdlib-4.2.0/src/ilcdlib/entity/contact.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.1.0/src/ilcdlib/entity/exchage.py` & `ilcdlib-4.2.0/src/ilcdlib/entity/exchage.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,32 +18,32 @@
 #  Find out more at www.BuildingTransparency.org
 #
 from typing import Type, TypeVar
 
 from openepd.model.lcia import OutputFlowSet, ResourceUseSet, ScopeSet
 
 from ilcdlib.entity.base_scope_set_reader import BaseIlcdScopeSetsReader
-from ilcdlib.mapping.common import SimpleDataMapper
+from ilcdlib.mapping.common import BaseDataMapper
 from ilcdlib.mapping.flows import default_flows_uuid_mapper
 from ilcdlib.mapping.indicators import default_indicators_uuid_mapper
 from ilcdlib.mapping.units import default_scope_to_units_mapper
 from ilcdlib.xml_parser import T_ET
 
 E = TypeVar("E", ResourceUseSet, OutputFlowSet)
 
 
 class IlcdExchangesReader(BaseIlcdScopeSetsReader):
     """Read exchanges from XML file."""
 
     def __init__(
         self,
         *args,
-        indicator_mapper: SimpleDataMapper[str] = default_indicators_uuid_mapper,
-        flow_mapper: SimpleDataMapper[str] = default_flows_uuid_mapper,
-        scope_to_units_mapper: SimpleDataMapper[str] = default_scope_to_units_mapper,
+        indicator_mapper: BaseDataMapper[str, str] = default_indicators_uuid_mapper,
+        flow_mapper: BaseDataMapper[str, str] = default_flows_uuid_mapper,
+        scope_to_units_mapper: BaseDataMapper[str, str] = default_scope_to_units_mapper,
         **kwargs,
     ):
         super().__init__(*args, **kwargs)
         self.indicator_mapper = indicator_mapper
         self.flow_mapper = flow_mapper
         self.scope_to_units_mapper = scope_to_units_mapper
 
@@ -73,17 +73,17 @@
             scope_to_units_mapper=self.scope_to_units_mapper,
         )
 
     def __get_exchanges(
         self,
         direction: str,
         scope_set_type: Type[E],
-        mapper: SimpleDataMapper[str],
+        mapper: BaseDataMapper[str, str],
         scenario_names: dict[str, str],
-        scope_to_units_mapper: SimpleDataMapper[str],
+        scope_to_units_mapper: BaseDataMapper[str, str],
     ) -> E:
         """Get indicators or flows from the ILCD EPD file."""
         ext: dict[str, ScopeSet] = {}
         exchanges = self._get_all_els(self._entity, ("process:exchange",))
         scope_sets: dict[str, ScopeSet | dict] = {"ext": ext}
 
         for exchange in exchanges:
```

### Comparing `ilcdlib-4.1.0/src/ilcdlib/entity/flow.py` & `ilcdlib-4.2.0/src/ilcdlib/entity/flow.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.1.0/src/ilcdlib/entity/lcia.py` & `ilcdlib-4.2.0/src/ilcdlib/entity/lcia.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,27 +20,27 @@
 import logging
 
 from openepd.model.common import Measurement
 from openepd.model.lcia import Impacts, ImpactSet, ScopeSet
 
 from ilcdlib.common import OpenEpdImpactSetSupportReader
 from ilcdlib.entity.base_scope_set_reader import BaseIlcdScopeSetsReader
-from ilcdlib.mapping.common import SimpleDataMapper
-from ilcdlib.mapping.impacts import default_impacts_uuid_mapper
+from ilcdlib.mapping.common import BaseDataMapper
+from ilcdlib.mapping.impacts import default_impacts_mapper
 from ilcdlib.mapping.units import default_scope_to_units_mapper
 
 
 class IlcdLciaResultsReader(OpenEpdImpactSetSupportReader, BaseIlcdScopeSetsReader):
     """Read an ILCD PCR XML file."""
 
     def __init__(
         self,
         *args,
-        impact_mapper: SimpleDataMapper[str] = default_impacts_uuid_mapper,
-        scope_to_units_mapper: SimpleDataMapper[str] = default_scope_to_units_mapper,
+        impact_mapper: BaseDataMapper[str, str] = default_impacts_mapper,
+        scope_to_units_mapper: BaseDataMapper[str, str] = default_scope_to_units_mapper,
         **kwargs,
     ):
         super().__init__(*args, **kwargs)
         self.impact_mapper = impact_mapper
         self.scope_to_units_mapper = scope_to_units_mapper
 
     def get_impact_set(self, scenario_names: dict[str, str]) -> ImpactSet:
```

### Comparing `ilcdlib-4.1.0/src/ilcdlib/entity/material.py` & `ilcdlib-4.2.0/src/ilcdlib/entity/material.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.1.0/src/ilcdlib/entity/pcr.py` & `ilcdlib-4.2.0/src/ilcdlib/entity/pcr.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.1.0/src/ilcdlib/entity/source.py` & `ilcdlib-4.2.0/src/ilcdlib/entity/source.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.1.0/src/ilcdlib/entity/unit.py` & `ilcdlib-4.2.0/src/ilcdlib/entity/unit.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 #  This software was developed with support from the Skanska USA,
 #  Charles Pankow Foundation, Microsoft Sustainability Fund, Interface, MKA Foundation, and others.
 #  Find out more at www.BuildingTransparency.org
 #
 from dataclasses import dataclass
 
 from ilcdlib.common import BaseIlcdMediumSpecificReader, IlcdXmlReader
-from ilcdlib.mapping.common import SimpleDataMapper
+from ilcdlib.mapping.common import BaseDataMapper
 from ilcdlib.mapping.units import default_units_uuid_mapper
 from ilcdlib.type import LangDef
 from ilcdlib.utils import none_throws
 from ilcdlib.xml_parser import T_ET
 
 
 @dataclass(kw_only=True)
@@ -39,15 +39,15 @@
     """Read an ILCD Unit Group XML file."""
 
     def __init__(
         self,
         element: T_ET.Element,
         data_provider: BaseIlcdMediumSpecificReader,
         *,
-        unit_mapper: SimpleDataMapper[str] = default_units_uuid_mapper,
+        unit_mapper: BaseDataMapper[str, str] = default_units_uuid_mapper,
     ):
         super().__init__(data_provider)
         self._entity = element
         self.unit_mapper = unit_mapper
 
     def get_uuid(self) -> str:
         """Get the UUID of the entity described by this data set."""
```

### Comparing `ilcdlib-4.1.0/src/ilcdlib/entity/validation.py` & `ilcdlib-4.2.0/src/ilcdlib/entity/validation.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.1.0/src/ilcdlib/epd/__init__.py` & `ilcdlib-4.2.0/src/ilcdlib/epd/__init__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.1.0/src/ilcdlib/epd/cli.py` & `ilcdlib-4.2.0/src/ilcdlib/epd/cli.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.1.0/src/ilcdlib/epd/dialect/__init__.py` & `ilcdlib-4.2.0/src/ilcdlib/epd/dialect/__init__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.1.0/src/ilcdlib/epd/dialect/environdec.py` & `ilcdlib-4.2.0/src/ilcdlib/epd/dialect/environdec.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.1.0/src/ilcdlib/epd/dialect/epditaly.py` & `ilcdlib-4.2.0/src/ilcdlib/epd/dialect/epditaly.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.1.0/src/ilcdlib/epd/dialect/indata.py` & `ilcdlib-4.2.0/src/ilcdlib/epd/dialect/indata.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.1.0/src/ilcdlib/epd/dialect/oekobaudat.py` & `ilcdlib-4.2.0/src/ilcdlib/epd/dialect/oekobaudat.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.1.0/src/ilcdlib/epd/factory.py` & `ilcdlib-4.2.0/src/ilcdlib/epd/factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,27 +18,29 @@
 #  Find out more at www.BuildingTransparency.org
 #
 from typing import Type
 
 from ilcdlib.epd.dialect.environdec import EnvirondecIlcdXmlEpdReader
 from ilcdlib.epd.dialect.epditaly import EpdItalyIlcdXmlEpdReader
 from ilcdlib.epd.dialect.indata import IndataIlcdXmlEpdReader
+from ilcdlib.epd.dialect.itb import ItbIlcdXmlEpdReader
 from ilcdlib.epd.dialect.oekobaudat import OekobauDatIlcdXmlEpdReader
 from ilcdlib.epd.reader import IlcdEpdReader
 
 
 class EpdReaderFactory:
     """Factory for creating EPD readers."""
 
     __DIALECTS: dict[str, Type[IlcdEpdReader]] = {
         "environdec": EnvirondecIlcdXmlEpdReader,
         "indata": IndataIlcdXmlEpdReader,
         "oekobau.dat": OekobauDatIlcdXmlEpdReader,
         "oekobaudat": OekobauDatIlcdXmlEpdReader,
         "epditaly": EpdItalyIlcdXmlEpdReader,
+        "itb": ItbIlcdXmlEpdReader,
     }
     DEFAULT_READER_CLASS = IlcdEpdReader
 
     def get_supported_dialects(self) -> list[str]:
         """Return a list of supported dialects."""
         return list(self.__DIALECTS.keys())
```

### Comparing `ilcdlib-4.1.0/src/ilcdlib/epd/reader.py` & `ilcdlib-4.2.0/src/ilcdlib/epd/reader.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.1.0/src/ilcdlib/extension.py` & `ilcdlib-4.2.0/src/ilcdlib/extension.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.1.0/src/ilcdlib/http_common.py` & `ilcdlib-4.2.0/src/ilcdlib/http_common.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.1.0/src/ilcdlib/mapping/__init__.py` & `ilcdlib-4.2.0/src/ilcdlib/mapping/__init__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.1.0/src/ilcdlib/mapping/compliance.py` & `ilcdlib-4.2.0/src/ilcdlib/mapping/compliance.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.1.0/src/ilcdlib/mapping/flows.py` & `ilcdlib-4.2.0/src/ilcdlib/mapping/flows.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.1.0/src/ilcdlib/mapping/indicators.py` & `ilcdlib-4.2.0/src/ilcdlib/mapping/indicators.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.1.0/src/ilcdlib/mapping/properties.py` & `ilcdlib-4.2.0/src/ilcdlib/mapping/properties.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.1.0/src/ilcdlib/mapping/units.py` & `ilcdlib-4.2.0/src/ilcdlib/mapping/units.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.1.0/src/ilcdlib/medium/__init__.py` & `ilcdlib-4.2.0/src/ilcdlib/medium/__init__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.1.0/src/ilcdlib/medium/archive.py` & `ilcdlib-4.2.0/src/ilcdlib/medium/archive.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.1.0/src/ilcdlib/medium/soda4lca.py` & `ilcdlib-4.2.0/src/ilcdlib/medium/soda4lca.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.1.0/src/ilcdlib/reference_data.py` & `ilcdlib-4.2.0/src/ilcdlib/reference_data.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.1.0/src/ilcdlib/sanitizing/__init__.py` & `ilcdlib-4.2.0/src/ilcdlib/sanitizing/__init__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.1.0/src/ilcdlib/sanitizing/domain.py` & `ilcdlib-4.2.0/src/ilcdlib/sanitizing/domain.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.1.0/src/ilcdlib/sanitizing/phone.py` & `ilcdlib-4.2.0/src/ilcdlib/sanitizing/phone.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.1.0/src/ilcdlib/sanitizing/text.py` & `ilcdlib-4.2.0/src/ilcdlib/sanitizing/text.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.1.0/src/ilcdlib/soda4lca/__init__.py` & `ilcdlib-4.2.0/src/ilcdlib/soda4lca/__init__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.1.0/src/ilcdlib/soda4lca/api_client.py` & `ilcdlib-4.2.0/src/ilcdlib/soda4lca/api_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -139,14 +139,20 @@
         except HTTPError as e:
             if e.response.status_code == 404:
                 raise FileNotFoundError(
                     f"Process {process_uuid} (ver={version}) doesn't have EPD document attached"
                 ) from e
             raise e
 
+    def get_total_size(self):
+        """Get total number of processes."""
+        response = self._do_request("get", "/processes", params={"pageSize": 1})
+        xml_response = T_ET.fromstring(response.content)
+        return int(xml_response.attrib.get(f"{{{self.ns['sapi']}}}totalSize", 0))
+
     def search_processes(
         self, offset: int = 0, page_size: int = 100, lang: str | None = None, **other_params
     ) -> ProcessSearchResponse:
         """
         Filter processes by various criteria.
 
         :param offset: offset from the beginning of the dataset
```

### Comparing `ilcdlib-4.1.0/src/ilcdlib/soda4lca/api_client_4x.py` & `ilcdlib-4.2.0/src/ilcdlib/soda4lca/api_client_4x.py`

 * *Files 17% similar despite different names*

```diff
@@ -13,28 +13,35 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 #  This software was developed with support from the Skanska USA,
 #  Charles Pankow Foundation, Microsoft Sustainability Fund, Interface, MKA Foundation, and others.
 #  Find out more at www.BuildingTransparency.org
 #
-from ilcdlib.dto import Category
+from ilcdlib.dto import Category, ProcessBasicInfo
 from ilcdlib.soda4lca.api_client import Soda4LcaXmlApiClient
 
 
 class Soda4LcaXmlApiClient4x(Soda4LcaXmlApiClient):
     """
     API client for Soda4LCA 4.x.
 
     Documentation for the API is available at https://bitbucket.org/okusche/soda4lca/src/842d85bb3b3b8f77415f20b431bb7b0789fee68f/Doc/src/Service_API/Service_API.md.
     """
 
     def __init__(self, *args, **kwargs):
         super(Soda4LcaXmlApiClient4x, self).__init__(*args, **kwargs)
 
+    def get_item_url(self, item: ProcessBasicInfo) -> str | None:
+        """Return the URL of the item."""
+        uuid = item.uuid
+        if uuid:
+            return f"{self.base_url}/showProcess.xhtml?uuid={uuid}"
+        return None
+
     def list_categories(self, category_system: str, data_type: str = "Process", lang: str = "en") -> list[Category]:
         """
         Return a flat list of all available categories for a given category system.
 
         :param str category_system: category system
         :param str data_type: type of dataset
         :param str lang: language
```

### Comparing `ilcdlib-4.1.0/src/ilcdlib/type.py` & `ilcdlib-4.2.0/src/ilcdlib/type.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.1.0/src/ilcdlib/utils.py` & `ilcdlib-4.2.0/src/ilcdlib/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 #  This software was developed with support from the Skanska USA,
 #  Charles Pankow Foundation, Microsoft Sustainability Fund, Interface, MKA Foundation, and others.
 #  Find out more at www.BuildingTransparency.org
 #
 from dataclasses import dataclass
 import datetime
 from typing import TYPE_CHECKING, Any, Optional, Self, TypeVar
+import uuid
 
 import pytz
 
 from ilcdlib import const
 from ilcdlib.sanitizing.domain import domain_from_url
 
 T = TypeVar("T")
@@ -100,7 +101,17 @@
     @staticmethod
     def _build_section(section: _MdSection) -> str:
         return f"{'#' * section.level} {section.title}\n\n{section.content or ''}"
 
     def build(self) -> str:
         """Build the Markdown string."""
         return "\n\n".join([self._build_section(x) for x in self._sections if x.content is not None])
+
+
+def is_valid_uuid(value: str, version: int = 4) -> bool:
+    """Check if the given string is a valid UUID."""
+
+    try:
+        uuid_obj = uuid.UUID(value, version=version)
+        return str(uuid_obj) == value
+    except ValueError:
+        return False
```

### Comparing `ilcdlib-4.1.0/src/ilcdlib/xml_parser.py` & `ilcdlib-4.2.0/src/ilcdlib/xml_parser.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.1.0/PKG-INFO` & `ilcdlib-4.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ilcdlib
-Version: 4.1.0
+Version: 4.2.0
 Summary: A toolkit for reading and writing ILCD format and it's derivatives
 Home-page: https://github.com/cchangelabs/ilcdlib
 License: Apache-2.0
 Author: C-Change Labs
 Author-email: support@c-change-labs.com
 Maintainer: C-Change Labs
 Maintainer-email: open-source@c-change-labs.com
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ilcdlib Version: 4.1.0 Summary: A toolkit for
+Metadata-Version: 2.1 Name: ilcdlib Version: 4.2.0 Summary: A toolkit for
 reading and writing ILCD format and it's derivatives Home-page: https://
 github.com/cchangelabs/ilcdlib License: Apache-2.0 Author: C-Change Labs
 Author-email: support@c-change-labs.com Maintainer: C-Change Labs Maintainer-
 email: open-source@c-change-labs.com Requires-Python: >=3.11,<4.0 Classifier:
 Development Status :: 3 - Alpha Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
```


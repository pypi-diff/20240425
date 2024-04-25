# Comparing `tmp/opset-4.0.7.tar.gz` & `tmp/opset-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opset-4.0.7.tar", max compression
+gzip compressed data, was "opset-4.1.0.tar", max compression
```

## Comparing `opset-4.0.7.tar` & `opset-4.1.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    11357 2023-07-17 16:21:49.415760 opset-4.0.7/LICENSE
--rw-r--r--   0        0        0    15699 2024-03-12 14:13:43.946162 opset-4.0.7/README.md
--rw-r--r--   0        0        0      558 2023-11-22 15:57:44.172155 opset-4.0.7/opset/__init__.py
--rw-r--r--   0        0        0    19086 2024-03-12 14:13:43.946162 opset-4.0.7/opset/configurator.py
--rw-r--r--   0        0        0     3809 2023-11-06 15:17:14.118550 opset-4.0.7/opset/gcp_secret_handler.py
--rw-r--r--   0        0        0        0 2023-07-17 16:21:49.415760 opset-4.0.7/opset/py.typed
--rw-r--r--   0        0        0     2496 2023-11-22 15:57:44.172155 opset-4.0.7/opset/utils.py
--rw-r--r--   0        0        0     1860 2024-03-12 14:13:43.946162 opset-4.0.7/pyproject.toml
--rw-r--r--   0        0        0    16876 1970-01-01 00:00:00.000000 opset-4.0.7/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-17 16:21:49.415760 opset-4.1.0/LICENSE
+-rw-r--r--   0        0        0    16365 2024-04-25 13:57:51.808604 opset-4.1.0/README.md
+-rw-r--r--   0        0        0      558 2023-11-22 15:57:44.172155 opset-4.1.0/opset/__init__.py
+-rw-r--r--   0        0        0    18601 2024-04-25 13:57:51.808604 opset-4.1.0/opset/configurator.py
+-rw-r--r--   0        0        0     6640 2024-04-25 13:57:51.808604 opset-4.1.0/opset/gcp_secret_handler.py
+-rw-r--r--   0        0        0        0 2023-07-17 16:21:49.415760 opset-4.1.0/opset/py.typed
+-rw-r--r--   0        0        0     2943 2024-04-25 13:57:51.808604 opset-4.1.0/opset/utils.py
+-rw-r--r--   0        0        0     1860 2024-04-25 13:57:51.808604 opset-4.1.0/pyproject.toml
+-rw-r--r--   0        0        0    17542 1970-01-01 00:00:00.000000 opset-4.1.0/PKG-INFO
```

### Comparing `opset-4.0.7/LICENSE` & `opset-4.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `opset-4.0.7/README.md` & `opset-4.1.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -148,14 +148,35 @@
 Example
 
 ```yaml
 database:
   host: opset+gcp://projects/dev-3423/secrets/db_host
 ```
 
+#### Combined secrets
+
+Combining multiple secrets into one single value is also supported for values of type `dict` or `list`. 
+Note that all values must also be of the same type. The way to do this is to split each secret with a 
+semicolon, like so:
+
+```yaml
+databases: >-
+  opset+gcp://
+  projects/canada/secrets/databases;
+  projects/usa/secrets/databases;
+  projects/europe/secrets/databases
+```
+
+**NOTE**: `>-` is used to allow for removing line breaks from multiline strings in YAML. The value 
+could also be provided in a single line.
+
+This will fetch the secrets from the three different projects and combine them into a single value.
+
+#### Project Mapping
+
 It is also possible to create a file `.opset.yml` in your project to create mapping for project name.
 For instance, with the following config.
 
 ```yaml
 gcp_project_mapping:
   dev: dev-3423
 ```
```

### Comparing `opset-4.0.7/opset/__init__.py` & `opset-4.1.0/opset/__init__.py`

 * *Files identical despite different names*

### Comparing `opset-4.0.7/opset/configurator.py` & `opset-4.1.0/opset/configurator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import inspect
-import json
 import logging
 import operator
 import os
 import socket
 import sys
 import typing
 import warnings
@@ -16,14 +15,15 @@
 import structlog
 import yaml
 from munch import munchify
 from pydantic import BaseModel, model_validator
 from pydantic.fields import FieldInfo
 from pydantic_core import PydanticUndefined
 
+from opset import utils
 from opset.gcp_secret_handler import (
     OPSET_GCP_PREFIX,
     MissingGcpSecretManagerLibrary,
     is_gcp_available,
     retrieve_gcp_secret_value,
 )
 
@@ -44,48 +44,32 @@
         unprocessed_gcp_secret_keys = []
         for k, field_info in cls.model_fields.items():
             if v := values.get(k):
                 if isinstance(v, str):
                     if v.startswith(OPSET_GCP_PREFIX):
                         unprocessed_gcp_secret_keys.append(k)
                     else:
-                        values[k] = cls._convert_type(v)
+                        values[k] = utils.convert_type(v)
 
             else:
                 field_type = typing.get_origin(field_info.annotation) or field_info.annotation
                 if inspect.isclass(field_type) and issubclass(field_type, OpsetSettingsBaseModel):
                     if (default := field_info.get_default()) and default != PydanticUndefined:
                         values[k] = default
                     else:
                         values[k] = field_type()
 
         if not is_gcp_available() and unprocessed_gcp_secret_keys:
             raise MissingGcpSecretManagerLibrary()
 
         for k in unprocessed_gcp_secret_keys:
-            values[k] = cls._convert_type(retrieve_gcp_secret_value(values[k], _opset_config))
+            values[k] = utils.convert_type(retrieve_gcp_secret_value(values[k], _opset_config))
 
         return values
 
-    @staticmethod
-    def _convert_type(value: str) -> str | bool | dict | list:
-        if value.lower() in ["y", "yes", "t", "true"]:
-            return True
-
-        if value.lower() in ["n", "no", "f", "false"]:
-            return False
-
-        if isinstance(value, str) and (value.startswith("{") or value.startswith("[")):
-            try:
-                return typing.cast(dict | list, json.loads(value))
-            except json.JSONDecodeError:
-                pass
-
-        return value
-
 
 class OpsetSettingsMainModel(OpsetSettingsBaseModel):
     _opset: "Config"
 
     def __init__(self, _opset: "Config", **data: dict[str, Any]) -> None:
         super().__init__(**data)
         self._opset = _opset
```

### Comparing `opset-4.0.7/opset/utils.py` & `opset-4.1.0/opset/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,36 @@
 # __init__.py
 # Emilio Assuncao, 2019-01-24
 # Copyright (c) Element AI Inc. All rights not expressly granted hereunder are reserved.
-
+import json
 from contextlib import contextmanager
 from tempfile import NamedTemporaryFile, _TemporaryFileWrapper  # noqa
-from typing import Any, Dict, Generator, Optional
+from typing import Any, Dict, Generator, Optional, cast
 from unittest.mock import patch
 
 import pkg_resources
 import yaml
 
 
+def convert_type(value: str) -> str | bool | dict | list:
+    if value.lower() in ["y", "yes", "t", "true"]:
+        return True
+
+    if value.lower() in ["n", "no", "f", "false"]:
+        return False
+
+    if isinstance(value, str) and (value.startswith("{") or value.startswith("[")):
+        try:
+            return cast(dict | list, json.loads(value))
+        except json.JSONDecodeError:
+            pass
+
+    return value
+
+
 @contextmanager
 def mock_config_file(
     local_values: Optional[Dict] = None,
     unit_test_values: Optional[Dict] = None,
 ) -> Generator[None, None, None]:
     """Spoof a config file by mocking out the return value of pkg_resources.resource_filename().
```

### Comparing `opset-4.0.7/pyproject.toml` & `opset-4.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "opset"
-version = "4.0.7"
+version = "4.1.0"
 description = "A library for simplifying the configuration of Python applications at all stages of deployment."
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/MarcDufresne/opset"
 repository = "https://github.com/MarcDufresne/opset"
 documentation = "https://github.com/MarcDufresne/opset"
 keywords = ["config", "management", "configuration", "logging", "setup"]
```

### Comparing `opset-4.0.7/PKG-INFO` & `opset-4.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opset
-Version: 4.0.7
+Version: 4.1.0
 Summary: A library for simplifying the configuration of Python applications at all stages of deployment.
 Home-page: https://github.com/MarcDufresne/opset
 License: Apache-2.0
 Keywords: config,management,configuration,logging,setup
 Author: Marc-André Dufresne
 Author-email: marc.andre.dufresne@gmail.com
 Requires-Python: >=3.10,<4.0
@@ -176,14 +176,35 @@
 Example
 
 ```yaml
 database:
   host: opset+gcp://projects/dev-3423/secrets/db_host
 ```
 
+#### Combined secrets
+
+Combining multiple secrets into one single value is also supported for values of type `dict` or `list`. 
+Note that all values must also be of the same type. The way to do this is to split each secret with a 
+semicolon, like so:
+
+```yaml
+databases: >-
+  opset+gcp://
+  projects/canada/secrets/databases;
+  projects/usa/secrets/databases;
+  projects/europe/secrets/databases
+```
+
+**NOTE**: `>-` is used to allow for removing line breaks from multiline strings in YAML. The value 
+could also be provided in a single line.
+
+This will fetch the secrets from the three different projects and combine them into a single value.
+
+#### Project Mapping
+
 It is also possible to create a file `.opset.yml` in your project to create mapping for project name.
 For instance, with the following config.
 
 ```yaml
 gcp_project_mapping:
   dev: dev-3423
 ```
```


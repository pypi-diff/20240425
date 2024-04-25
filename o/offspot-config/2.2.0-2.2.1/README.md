# Comparing `tmp/offspot_config-2.2.0.tar.gz` & `tmp/offspot_config-2.2.1.tar.gz`

## Comparing `offspot_config-2.2.0.tar` & `offspot_config-2.2.1.tar`

### file list

```diff
@@ -1,54 +1,54 @@
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 offspot_config-2.2.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0    11183 2020-02-02 00:00:00.000000 offspot_config-2.2.0/CHANGELOG.md
--rw-r--r--   0        0        0     3091 2020-02-02 00:00:00.000000 offspot_config-2.2.0/tasks.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 offspot_config-2.2.0/src/offspot_config/__init__.py
--rw-r--r--   0        0        0    33843 2020-02-02 00:00:00.000000 offspot_config-2.2.0/src/offspot_config/builder.py
--rw-r--r--   0        0        0    14110 2020-02-02 00:00:00.000000 offspot_config-2.2.0/src/offspot_config/catalog.json
--rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 offspot_config-2.2.0/src/offspot_config/catalog.py
--rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 offspot_config-2.2.0/src/offspot_config/constants.py
--rw-r--r--   0        0        0     5009 2020-02-02 00:00:00.000000 offspot_config-2.2.0/src/offspot_config/file.py
--rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 offspot_config-2.2.0/src/offspot_config/oci_images.py
--rw-r--r--   0        0        0     6652 2020-02-02 00:00:00.000000 offspot_config-2.2.0/src/offspot_config/packages.py
--rw-r--r--   0        0        0     3676 2020-02-02 00:00:00.000000 offspot_config-2.2.0/src/offspot_config/zim.py
--rw-r--r--   0        0        0     8233 2020-02-02 00:00:00.000000 offspot_config-2.2.0/src/offspot_config/branding/horizontal-logo-light.png
--rw-r--r--   0        0        0     7835 2020-02-02 00:00:00.000000 offspot_config-2.2.0/src/offspot_config/branding/square-logo-light.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 offspot_config-2.2.0/src/offspot_config/inputs/__init__.py
--rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 offspot_config-2.2.0/src/offspot_config/inputs/base.py
--rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 offspot_config-2.2.0/src/offspot_config/inputs/checksum.py
--rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 offspot_config-2.2.0/src/offspot_config/inputs/file.py
--rw-r--r--   0        0        0     3673 2020-02-02 00:00:00.000000 offspot_config-2.2.0/src/offspot_config/inputs/mainconfig.py
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 offspot_config-2.2.0/src/offspot_config/inputs/oci.py
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 offspot_config-2.2.0/src/offspot_config/inputs/output.py
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 offspot_config-2.2.0/src/offspot_config/inputs/str.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 offspot_config-2.2.0/src/offspot_config/inputs/ways.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 offspot_config-2.2.0/src/offspot_config/utils/__init__.py
--rw-r--r--   0        0        0     2337 2020-02-02 00:00:00.000000 offspot_config-2.2.0/src/offspot_config/utils/dashboard.py
--rw-r--r--   0        0        0     4458 2020-02-02 00:00:00.000000 offspot_config-2.2.0/src/offspot_config/utils/download.py
--rw-r--r--   0        0        0    12899 2020-02-02 00:00:00.000000 offspot_config-2.2.0/src/offspot_config/utils/misc.py
--rw-r--r--   0        0        0     1946 2020-02-02 00:00:00.000000 offspot_config-2.2.0/src/offspot_config/utils/sizes.py
--rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 offspot_config-2.2.0/src/offspot_config/utils/yaml.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 offspot_config-2.2.0/src/offspot_runtime/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 offspot_config-2.2.0/src/offspot_runtime/__init__.py
--rwxr-xr-x   0        0        0    18295 2020-02-02 00:00:00.000000 offspot_config-2.2.0/src/offspot_runtime/ap.py
--rw-r--r--   0        0        0    21248 2020-02-02 00:00:00.000000 offspot_config-2.2.0/src/offspot_runtime/checks.py
--rw-r--r--   0        0        0     4936 2020-02-02 00:00:00.000000 offspot_config-2.2.0/src/offspot_runtime/configlib.py
--rwxr-xr-x   0        0        0     2564 2020-02-02 00:00:00.000000 offspot_config-2.2.0/src/offspot_runtime/containers.py
--rwxr-xr-x   0        0        0     3341 2020-02-02 00:00:00.000000 offspot_config-2.2.0/src/offspot_runtime/dnsmasqspoof.py
--rwxr-xr-x   0        0        0     5142 2020-02-02 00:00:00.000000 offspot_config-2.2.0/src/offspot_runtime/ethernet.py
--rwxr-xr-x   0        0        0     5210 2020-02-02 00:00:00.000000 offspot_config-2.2.0/src/offspot_runtime/firmware.py
--rwxr-xr-x   0        0        0     8362 2020-02-02 00:00:00.000000 offspot_config-2.2.0/src/offspot_runtime/fromfile.py
--rwxr-xr-x   0        0        0     2122 2020-02-02 00:00:00.000000 offspot_config-2.2.0/src/offspot_runtime/hostname.py
--rwxr-xr-x   0        0        0     1678 2020-02-02 00:00:00.000000 offspot_config-2.2.0/src/offspot_runtime/timezone.py
--rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 offspot_config-2.2.0/tests/conftest.py
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 offspot_config-2.2.0/tests/test_catalog.py
--rw-r--r--   0        0        0    21249 2020-02-02 00:00:00.000000 offspot_config-2.2.0/tests/test_checks.py
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 offspot_config-2.2.0/tests/test_humanid.py
--rw-r--r--   0        0        0     1790 2020-02-02 00:00:00.000000 offspot_config-2.2.0/tests/test_inputs.py
--rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 offspot_config-2.2.0/tests/test_link.py
--rw-r--r--   0        0        0     7235 2020-02-02 00:00:00.000000 offspot_config-2.2.0/tests/test_reader.py
--rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 offspot_config-2.2.0/tests/test_zim.py
--rw-r--r--   0        0        0     4062 2020-02-02 00:00:00.000000 offspot_config-2.2.0/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 offspot_config-2.2.0/LICENSE
--rw-r--r--   0        0        0    11831 2020-02-02 00:00:00.000000 offspot_config-2.2.0/README.md
--rw-r--r--   0        0        0     6733 2020-02-02 00:00:00.000000 offspot_config-2.2.0/pyproject.toml
--rw-r--r--   0        0        0    13707 2020-02-02 00:00:00.000000 offspot_config-2.2.0/PKG-INFO
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 offspot_config-2.2.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    11315 2020-02-02 00:00:00.000000 offspot_config-2.2.1/CHANGELOG.md
+-rw-r--r--   0        0        0     3091 2020-02-02 00:00:00.000000 offspot_config-2.2.1/tasks.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 offspot_config-2.2.1/src/offspot_config/__init__.py
+-rw-r--r--   0        0        0    33843 2020-02-02 00:00:00.000000 offspot_config-2.2.1/src/offspot_config/builder.py
+-rw-r--r--   0        0        0    14110 2020-02-02 00:00:00.000000 offspot_config-2.2.1/src/offspot_config/catalog.json
+-rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 offspot_config-2.2.1/src/offspot_config/catalog.py
+-rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 offspot_config-2.2.1/src/offspot_config/constants.py
+-rw-r--r--   0        0        0     5009 2020-02-02 00:00:00.000000 offspot_config-2.2.1/src/offspot_config/file.py
+-rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 offspot_config-2.2.1/src/offspot_config/oci_images.py
+-rw-r--r--   0        0        0     6652 2020-02-02 00:00:00.000000 offspot_config-2.2.1/src/offspot_config/packages.py
+-rw-r--r--   0        0        0     3676 2020-02-02 00:00:00.000000 offspot_config-2.2.1/src/offspot_config/zim.py
+-rw-r--r--   0        0        0     8233 2020-02-02 00:00:00.000000 offspot_config-2.2.1/src/offspot_config/branding/horizontal-logo-light.png
+-rw-r--r--   0        0        0     7835 2020-02-02 00:00:00.000000 offspot_config-2.2.1/src/offspot_config/branding/square-logo-light.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 offspot_config-2.2.1/src/offspot_config/inputs/__init__.py
+-rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 offspot_config-2.2.1/src/offspot_config/inputs/base.py
+-rw-r--r--   0        0        0     1894 2020-02-02 00:00:00.000000 offspot_config-2.2.1/src/offspot_config/inputs/checksum.py
+-rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 offspot_config-2.2.1/src/offspot_config/inputs/file.py
+-rw-r--r--   0        0        0     3673 2020-02-02 00:00:00.000000 offspot_config-2.2.1/src/offspot_config/inputs/mainconfig.py
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 offspot_config-2.2.1/src/offspot_config/inputs/oci.py
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 offspot_config-2.2.1/src/offspot_config/inputs/output.py
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 offspot_config-2.2.1/src/offspot_config/inputs/str.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 offspot_config-2.2.1/src/offspot_config/inputs/ways.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 offspot_config-2.2.1/src/offspot_config/utils/__init__.py
+-rw-r--r--   0        0        0     2337 2020-02-02 00:00:00.000000 offspot_config-2.2.1/src/offspot_config/utils/dashboard.py
+-rw-r--r--   0        0        0     4458 2020-02-02 00:00:00.000000 offspot_config-2.2.1/src/offspot_config/utils/download.py
+-rw-r--r--   0        0        0    12899 2020-02-02 00:00:00.000000 offspot_config-2.2.1/src/offspot_config/utils/misc.py
+-rw-r--r--   0        0        0     1946 2020-02-02 00:00:00.000000 offspot_config-2.2.1/src/offspot_config/utils/sizes.py
+-rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 offspot_config-2.2.1/src/offspot_config/utils/yaml.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 offspot_config-2.2.1/src/offspot_runtime/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 offspot_config-2.2.1/src/offspot_runtime/__init__.py
+-rwxr-xr-x   0        0        0    18295 2020-02-02 00:00:00.000000 offspot_config-2.2.1/src/offspot_runtime/ap.py
+-rw-r--r--   0        0        0    21248 2020-02-02 00:00:00.000000 offspot_config-2.2.1/src/offspot_runtime/checks.py
+-rw-r--r--   0        0        0     4936 2020-02-02 00:00:00.000000 offspot_config-2.2.1/src/offspot_runtime/configlib.py
+-rwxr-xr-x   0        0        0     2564 2020-02-02 00:00:00.000000 offspot_config-2.2.1/src/offspot_runtime/containers.py
+-rwxr-xr-x   0        0        0     3341 2020-02-02 00:00:00.000000 offspot_config-2.2.1/src/offspot_runtime/dnsmasqspoof.py
+-rwxr-xr-x   0        0        0     5142 2020-02-02 00:00:00.000000 offspot_config-2.2.1/src/offspot_runtime/ethernet.py
+-rwxr-xr-x   0        0        0     5210 2020-02-02 00:00:00.000000 offspot_config-2.2.1/src/offspot_runtime/firmware.py
+-rwxr-xr-x   0        0        0     8362 2020-02-02 00:00:00.000000 offspot_config-2.2.1/src/offspot_runtime/fromfile.py
+-rwxr-xr-x   0        0        0     2122 2020-02-02 00:00:00.000000 offspot_config-2.2.1/src/offspot_runtime/hostname.py
+-rwxr-xr-x   0        0        0     1678 2020-02-02 00:00:00.000000 offspot_config-2.2.1/src/offspot_runtime/timezone.py
+-rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 offspot_config-2.2.1/tests/conftest.py
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 offspot_config-2.2.1/tests/test_catalog.py
+-rw-r--r--   0        0        0    21249 2020-02-02 00:00:00.000000 offspot_config-2.2.1/tests/test_checks.py
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 offspot_config-2.2.1/tests/test_humanid.py
+-rw-r--r--   0        0        0     1790 2020-02-02 00:00:00.000000 offspot_config-2.2.1/tests/test_inputs.py
+-rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 offspot_config-2.2.1/tests/test_link.py
+-rw-r--r--   0        0        0     7235 2020-02-02 00:00:00.000000 offspot_config-2.2.1/tests/test_reader.py
+-rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 offspot_config-2.2.1/tests/test_zim.py
+-rw-r--r--   0        0        0     4062 2020-02-02 00:00:00.000000 offspot_config-2.2.1/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 offspot_config-2.2.1/LICENSE
+-rw-r--r--   0        0        0    11831 2020-02-02 00:00:00.000000 offspot_config-2.2.1/README.md
+-rw-r--r--   0        0        0     6733 2020-02-02 00:00:00.000000 offspot_config-2.2.1/pyproject.toml
+-rw-r--r--   0        0        0    13707 2020-02-02 00:00:00.000000 offspot_config-2.2.1/PKG-INFO
```

### Comparing `offspot_config-2.2.0/.pre-commit-config.yaml` & `offspot_config-2.2.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `offspot_config-2.2.0/CHANGELOG.md` & `offspot_config-2.2.1/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,24 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [2.2.1] - 2024-04-25
+
+### Fixed
+
+- YAML repr of Checksum (#42)
+
+### Changed
+
+- Using captive-portal 1.4.2 with branding support
+
 ## [2.2.0] - 2024-04-24
 
 ### Added
 
 - [inputs.file] `File.is_base64_encoded` if `via` is `base64`
 - [utils.misc] `b64_encode()` and `b64_decode()` for reproducible base64 transport
 - [branding] `branding` folder in `offspot_config` containing official/original offspot branding files
```

### Comparing `offspot_config-2.2.0/tasks.py` & `offspot_config-2.2.1/tasks.py`

 * *Files identical despite different names*

### Comparing `offspot_config-2.2.0/src/offspot_config/builder.py` & `offspot_config-2.2.1/src/offspot_config/builder.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,17 +45,17 @@
 BRANDING_PATH = CONTENT_TARGET_PATH / "branding"
 
 KIWIX_ZIM_LOAD_BALANCER_URL = "https://download.kiwix.org/zim/"
 
 # data source for “internal images” (out of catalog)
 INTERNAL_IMAGES = {
     "captive-portal": {
-        "source": "ghcr.io/offspot/captive-portal:1.4.1",
-        "filesize": 189911040,
-        "fullsize": 189841976,
+        "source": "ghcr.io/offspot/captive-portal:1.4.2",
+        "filesize": 189900800,
+        "fullsize": 189833272,
     },
     "dashboard": {
         "source": "ghcr.io/offspot/dashboard:1.3.1",
         "filesize": 124354560,
         "fullsize": 124261524,
     },
     "file-browser": {
```

### Comparing `offspot_config-2.2.0/src/offspot_config/catalog.json` & `offspot_config-2.2.1/src/offspot_config/catalog.json`

 * *Files identical despite different names*

### Comparing `offspot_config-2.2.0/src/offspot_config/catalog.py` & `offspot_config-2.2.1/src/offspot_config/catalog.py`

 * *Files identical despite different names*

### Comparing `offspot_config-2.2.0/src/offspot_config/constants.py` & `offspot_config-2.2.1/src/offspot_config/constants.py`

 * *Files identical despite different names*

### Comparing `offspot_config-2.2.0/src/offspot_config/file.py` & `offspot_config-2.2.1/src/offspot_config/file.py`

 * *Files identical despite different names*

### Comparing `offspot_config-2.2.0/src/offspot_config/oci_images.py` & `offspot_config-2.2.1/src/offspot_config/oci_images.py`

 * *Files identical despite different names*

### Comparing `offspot_config-2.2.0/src/offspot_config/packages.py` & `offspot_config-2.2.1/src/offspot_config/packages.py`

 * *Files identical despite different names*

### Comparing `offspot_config-2.2.0/src/offspot_config/zim.py` & `offspot_config-2.2.1/src/offspot_config/zim.py`

 * *Files identical despite different names*

### Comparing `offspot_config-2.2.0/src/offspot_config/branding/horizontal-logo-light.png` & `offspot_config-2.2.1/src/offspot_config/branding/horizontal-logo-light.png`

 * *Files identical despite different names*

### Comparing `offspot_config-2.2.0/src/offspot_config/branding/square-logo-light.png` & `offspot_config-2.2.1/src/offspot_config/branding/square-logo-light.png`

 * *Files identical despite different names*

### Comparing `offspot_config-2.2.0/src/offspot_config/inputs/base.py` & `offspot_config-2.2.1/src/offspot_config/inputs/base.py`

 * *Files identical despite different names*

### Comparing `offspot_config-2.2.0/src/offspot_config/inputs/checksum.py` & `offspot_config-2.2.1/src/offspot_config/inputs/checksum.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from __future__ import annotations
 
 from attrs import asdict, define
 from typeguard import typechecked
 
 from offspot_config.constants import SUPPORTED_CHECKSUM_ALGORITHMS
 from offspot_config.utils.download import read_checksum_from
+from offspot_config.utils.yaml import custom_yaml_repr
 
 
+@custom_yaml_repr
 @typechecked
 @define(kw_only=True)
 class Checksum:
     """Checksum for download validation
 
     kind is either `digest` (default) or `url` to use the special async mode.
 
@@ -46,7 +48,13 @@
     @property
     def as_aria(self) -> str:
         """aria2-compatible checksum format: {algo}={digest}"""
         return f"{self.algo}={self.digest}"
 
     def to_dict(self) -> dict[str, str]:
         return asdict(self)
+
+    @staticmethod
+    def __yaml_repr__(dumper, data):
+        return dumper.represent_dict(
+            {key: value for key, value in asdict(data).items() if value is not None}
+        )
```

### Comparing `offspot_config-2.2.0/src/offspot_config/inputs/file.py` & `offspot_config-2.2.1/src/offspot_config/inputs/file.py`

 * *Files identical despite different names*

### Comparing `offspot_config-2.2.0/src/offspot_config/inputs/mainconfig.py` & `offspot_config-2.2.1/src/offspot_config/inputs/mainconfig.py`

 * *Files identical despite different names*

### Comparing `offspot_config-2.2.0/src/offspot_config/inputs/output.py` & `offspot_config-2.2.1/src/offspot_config/inputs/output.py`

 * *Files identical despite different names*

### Comparing `offspot_config-2.2.0/src/offspot_config/utils/dashboard.py` & `offspot_config-2.2.1/src/offspot_config/utils/dashboard.py`

 * *Files identical despite different names*

### Comparing `offspot_config-2.2.0/src/offspot_config/utils/download.py` & `offspot_config-2.2.1/src/offspot_config/utils/download.py`

 * *Files identical despite different names*

### Comparing `offspot_config-2.2.0/src/offspot_config/utils/misc.py` & `offspot_config-2.2.1/src/offspot_config/utils/misc.py`

 * *Files identical despite different names*

### Comparing `offspot_config-2.2.0/src/offspot_config/utils/sizes.py` & `offspot_config-2.2.1/src/offspot_config/utils/sizes.py`

 * *Files identical despite different names*

### Comparing `offspot_config-2.2.0/src/offspot_config/utils/yaml.py` & `offspot_config-2.2.1/src/offspot_config/utils/yaml.py`

 * *Files identical despite different names*

### Comparing `offspot_config-2.2.0/src/offspot_runtime/ap.py` & `offspot_config-2.2.1/src/offspot_runtime/ap.py`

 * *Files identical despite different names*

### Comparing `offspot_config-2.2.0/src/offspot_runtime/checks.py` & `offspot_config-2.2.1/src/offspot_runtime/checks.py`

 * *Files identical despite different names*

### Comparing `offspot_config-2.2.0/src/offspot_runtime/configlib.py` & `offspot_config-2.2.1/src/offspot_runtime/configlib.py`

 * *Files identical despite different names*

### Comparing `offspot_config-2.2.0/src/offspot_runtime/containers.py` & `offspot_config-2.2.1/src/offspot_runtime/containers.py`

 * *Files identical despite different names*

### Comparing `offspot_config-2.2.0/src/offspot_runtime/dnsmasqspoof.py` & `offspot_config-2.2.1/src/offspot_runtime/dnsmasqspoof.py`

 * *Files identical despite different names*

### Comparing `offspot_config-2.2.0/src/offspot_runtime/ethernet.py` & `offspot_config-2.2.1/src/offspot_runtime/ethernet.py`

 * *Files identical despite different names*

### Comparing `offspot_config-2.2.0/src/offspot_runtime/firmware.py` & `offspot_config-2.2.1/src/offspot_runtime/firmware.py`

 * *Files identical despite different names*

### Comparing `offspot_config-2.2.0/src/offspot_runtime/fromfile.py` & `offspot_config-2.2.1/src/offspot_runtime/fromfile.py`

 * *Files identical despite different names*

### Comparing `offspot_config-2.2.0/src/offspot_runtime/hostname.py` & `offspot_config-2.2.1/src/offspot_runtime/hostname.py`

 * *Files identical despite different names*

### Comparing `offspot_config-2.2.0/src/offspot_runtime/timezone.py` & `offspot_config-2.2.1/src/offspot_runtime/timezone.py`

 * *Files identical despite different names*

### Comparing `offspot_config-2.2.0/tests/conftest.py` & `offspot_config-2.2.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `offspot_config-2.2.0/tests/test_checks.py` & `offspot_config-2.2.1/tests/test_checks.py`

 * *Files identical despite different names*

### Comparing `offspot_config-2.2.0/tests/test_humanid.py` & `offspot_config-2.2.1/tests/test_humanid.py`

 * *Files identical despite different names*

### Comparing `offspot_config-2.2.0/tests/test_inputs.py` & `offspot_config-2.2.1/tests/test_inputs.py`

 * *Files identical despite different names*

### Comparing `offspot_config-2.2.0/tests/test_link.py` & `offspot_config-2.2.1/tests/test_link.py`

 * *Files identical despite different names*

### Comparing `offspot_config-2.2.0/tests/test_reader.py` & `offspot_config-2.2.1/tests/test_reader.py`

 * *Files identical despite different names*

### Comparing `offspot_config-2.2.0/tests/test_zim.py` & `offspot_config-2.2.1/tests/test_zim.py`

 * *Files identical despite different names*

### Comparing `offspot_config-2.2.0/.gitignore` & `offspot_config-2.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `offspot_config-2.2.0/LICENSE` & `offspot_config-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `offspot_config-2.2.0/README.md` & `offspot_config-2.2.1/README.md`

 * *Files identical despite different names*

### Comparing `offspot_config-2.2.0/pyproject.toml` & `offspot_config-2.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `offspot_config-2.2.0/PKG-INFO` & `offspot_config-2.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: offspot-config
-Version: 2.2.0
+Version: 2.2.1
 Summary: Offspot Config helpers
 Project-URL: Homepage, https://github.com/offspot/offspot-config
 Project-URL: Donate, https://www.kiwix.org/en/support-us/
 Author-email: Kiwix <dev@kiwix.org>
 License: GPL-3.0-or-later
 License-File: LICENSE
 Keywords: offspot
```


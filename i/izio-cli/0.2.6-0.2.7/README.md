# Comparing `tmp/izio_cli-0.2.6.tar.gz` & `tmp/izio_cli-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "izio_cli-0.2.6.tar", max compression
+gzip compressed data, was "izio_cli-0.2.7.tar", max compression
```

## Comparing `izio_cli-0.2.6.tar` & `izio_cli-0.2.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1257 2024-04-25 20:52:09.288775 izio_cli-0.2.6/LICENSE
--rw-r--r--   0        0        0     1889 2024-04-25 20:52:09.288775 izio_cli-0.2.6/README.md
--rw-r--r--   0        0        0       51 2024-04-25 20:52:21.088840 izio_cli-0.2.6/izio_cli/__init__.py
--rwxr-xr-x   0        0        0    19040 2024-04-25 20:52:09.292775 izio_cli-0.2.6/izio_cli/cli.py
--rw-r--r--   0        0        0        0 2024-04-25 20:52:09.292775 izio_cli-0.2.6/izio_cli/helper/__init__.py
--rw-r--r--   0        0        0     2416 2024-04-25 20:52:09.292775 izio_cli-0.2.6/izio_cli/helper/console_helper.py
--rw-r--r--   0        0        0      611 2024-04-25 20:52:09.292775 izio_cli-0.2.6/izio_cli/helper/console_validators.py
--rw-r--r--   0        0        0     1682 2024-04-25 20:52:09.292775 izio_cli-0.2.6/izio_cli/helper/fs_helper.py
--rw-r--r--   0        0        0     4991 2024-04-25 20:52:09.292775 izio_cli-0.2.6/izio_cli/helper/loyalty_helper.py
--rw-r--r--   0        0        0     2368 2024-04-25 20:52:09.292775 izio_cli-0.2.6/izio_cli/helper/pattern_helper.py
--rw-r--r--   0        0        0     3258 2024-04-25 20:52:09.292775 izio_cli-0.2.6/izio_cli/helper/project_helper.py
--rw-r--r--   0        0        0     1979 2024-04-25 20:52:09.292775 izio_cli-0.2.6/izio_cli/helper/strings_transformers.py
--rw-r--r--   0        0        0        0 2024-04-25 20:52:09.292775 izio_cli-0.2.6/izio_cli/pattern/__init__.py
--rw-r--r--   0        0        0    14409 2024-04-25 20:52:09.292775 izio_cli-0.2.6/izio_cli/pattern/dot_net_pattern.py
--rw-r--r--   0        0        0     8219 2024-04-25 20:52:09.292775 izio_cli-0.2.6/izio_cli/pattern/flutter_pattern.py
--rw-r--r--   0        0        0        0 2024-04-25 20:52:09.292775 izio_cli-0.2.6/izio_cli/values/__init__.py
--rw-r--r--   0        0        0     7440 2024-04-25 20:52:09.292775 izio_cli-0.2.6/izio_cli/values/dot_net_payload.py
--rw-r--r--   0        0        0     4915 2024-04-25 20:52:09.292775 izio_cli-0.2.6/izio_cli/values/flutter_payloads.py
--rw-r--r--   0        0        0     1532 2024-04-25 20:52:21.088840 izio_cli-0.2.6/pyproject.toml
--rw-r--r--   0        0        0     2696 1970-01-01 00:00:00.000000 izio_cli-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0     1257 2024-04-25 20:54:47.763758 izio_cli-0.2.7/LICENSE
+-rw-r--r--   0        0        0     1889 2024-04-25 20:54:47.763758 izio_cli-0.2.7/README.md
+-rw-r--r--   0        0        0       51 2024-04-25 20:54:58.087746 izio_cli-0.2.7/izio_cli/__init__.py
+-rwxr-xr-x   0        0        0    19040 2024-04-25 20:54:47.763758 izio_cli-0.2.7/izio_cli/cli.py
+-rw-r--r--   0        0        0        0 2024-04-25 20:54:47.763758 izio_cli-0.2.7/izio_cli/helper/__init__.py
+-rw-r--r--   0        0        0     2416 2024-04-25 20:54:47.763758 izio_cli-0.2.7/izio_cli/helper/console_helper.py
+-rw-r--r--   0        0        0      611 2024-04-25 20:54:47.763758 izio_cli-0.2.7/izio_cli/helper/console_validators.py
+-rw-r--r--   0        0        0     1682 2024-04-25 20:54:47.763758 izio_cli-0.2.7/izio_cli/helper/fs_helper.py
+-rw-r--r--   0        0        0     4991 2024-04-25 20:54:47.763758 izio_cli-0.2.7/izio_cli/helper/loyalty_helper.py
+-rw-r--r--   0        0        0     2368 2024-04-25 20:54:47.763758 izio_cli-0.2.7/izio_cli/helper/pattern_helper.py
+-rw-r--r--   0        0        0     3258 2024-04-25 20:54:47.763758 izio_cli-0.2.7/izio_cli/helper/project_helper.py
+-rw-r--r--   0        0        0     1979 2024-04-25 20:54:47.763758 izio_cli-0.2.7/izio_cli/helper/strings_transformers.py
+-rw-r--r--   0        0        0        0 2024-04-25 20:54:47.763758 izio_cli-0.2.7/izio_cli/pattern/__init__.py
+-rw-r--r--   0        0        0    14409 2024-04-25 20:54:47.763758 izio_cli-0.2.7/izio_cli/pattern/dot_net_pattern.py
+-rw-r--r--   0        0        0     8219 2024-04-25 20:54:47.763758 izio_cli-0.2.7/izio_cli/pattern/flutter_pattern.py
+-rw-r--r--   0        0        0        0 2024-04-25 20:54:47.763758 izio_cli-0.2.7/izio_cli/values/__init__.py
+-rw-r--r--   0        0        0     7440 2024-04-25 20:54:47.763758 izio_cli-0.2.7/izio_cli/values/dot_net_payload.py
+-rw-r--r--   0        0        0     4915 2024-04-25 20:54:47.763758 izio_cli-0.2.7/izio_cli/values/flutter_payloads.py
+-rw-r--r--   0        0        0     1532 2024-04-25 20:54:58.087746 izio_cli-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0     2696 1970-01-01 00:00:00.000000 izio_cli-0.2.7/PKG-INFO
```

### Comparing `izio_cli-0.2.6/LICENSE` & `izio_cli-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `izio_cli-0.2.6/README.md` & `izio_cli-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `izio_cli-0.2.6/izio_cli/cli.py` & `izio_cli-0.2.7/izio_cli/cli.py`

 * *Files identical despite different names*

### Comparing `izio_cli-0.2.6/izio_cli/helper/console_helper.py` & `izio_cli-0.2.7/izio_cli/helper/console_helper.py`

 * *Files identical despite different names*

### Comparing `izio_cli-0.2.6/izio_cli/helper/console_validators.py` & `izio_cli-0.2.7/izio_cli/helper/console_validators.py`

 * *Files identical despite different names*

### Comparing `izio_cli-0.2.6/izio_cli/helper/fs_helper.py` & `izio_cli-0.2.7/izio_cli/helper/fs_helper.py`

 * *Files identical despite different names*

### Comparing `izio_cli-0.2.6/izio_cli/helper/loyalty_helper.py` & `izio_cli-0.2.7/izio_cli/helper/loyalty_helper.py`

 * *Files identical despite different names*

### Comparing `izio_cli-0.2.6/izio_cli/helper/pattern_helper.py` & `izio_cli-0.2.7/izio_cli/helper/pattern_helper.py`

 * *Files identical despite different names*

### Comparing `izio_cli-0.2.6/izio_cli/helper/project_helper.py` & `izio_cli-0.2.7/izio_cli/helper/project_helper.py`

 * *Files identical despite different names*

### Comparing `izio_cli-0.2.6/izio_cli/helper/strings_transformers.py` & `izio_cli-0.2.7/izio_cli/helper/strings_transformers.py`

 * *Files identical despite different names*

### Comparing `izio_cli-0.2.6/izio_cli/pattern/dot_net_pattern.py` & `izio_cli-0.2.7/izio_cli/pattern/dot_net_pattern.py`

 * *Files identical despite different names*

### Comparing `izio_cli-0.2.6/izio_cli/pattern/flutter_pattern.py` & `izio_cli-0.2.7/izio_cli/pattern/flutter_pattern.py`

 * *Files identical despite different names*

### Comparing `izio_cli-0.2.6/izio_cli/values/dot_net_payload.py` & `izio_cli-0.2.7/izio_cli/values/dot_net_payload.py`

 * *Files identical despite different names*

### Comparing `izio_cli-0.2.6/izio_cli/values/flutter_payloads.py` & `izio_cli-0.2.7/izio_cli/values/flutter_payloads.py`

 * *Files identical despite different names*

### Comparing `izio_cli-0.2.6/pyproject.toml` & `izio_cli-0.2.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "izio-cli"
-version = "0.2.6"
+version = "0.2.7"
 description = "Izio CLI is a comprehensive command-line interface tool designed to facilitate the management and automation of various aspects of Izio&Co software development projects."
 authors = ["saulopef <saulopef@gmail.com>"]
 readme = "README.md"
 license = "BeerWare"
 packages = [
     { include = "izio_cli" },
     { include = "pattern", from = "izio_cli"},
```

### Comparing `izio_cli-0.2.6/PKG-INFO` & `izio_cli-0.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: izio-cli
-Version: 0.2.6
+Version: 0.2.7
 Summary: Izio CLI is a comprehensive command-line interface tool designed to facilitate the management and automation of various aspects of Izio&Co software development projects.
 License: Beerware
 Author: saulopef
 Author-email: saulopef@gmail.com
 Requires-Python: >=3.12,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```


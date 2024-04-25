# Comparing `tmp/totvs-dta-utils-0.1.3.tar.gz` & `tmp/totvs-dta-utils-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "totvs-dta-utils-0.1.3.tar", last modified: Tue Mar 26 19:46:17 2024, max compression
+gzip compressed data, was "totvs-dta-utils-0.1.4.tar", last modified: Thu Apr 25 17:29:44 2024, max compression
```

## Comparing `totvs-dta-utils-0.1.3.tar` & `totvs-dta-utils-0.1.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:17.928005 totvs-dta-utils-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)     5590 2024-03-26 19:46:17.928005 totvs-dta-utils-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5303 2024-03-26 19:46:17.000000 totvs-dta-utils-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:17.928005 totvs-dta-utils-0.1.3/dta_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-03-26 19:46:17.000000 totvs-dta-utils-0.1.3/dta_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:17.928005 totvs-dta-utils-0.1.3/dta_utils/services/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:17.000000 totvs-dta-utils-0.1.3/dta_utils/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-03-26 19:46:17.000000 totvs-dta-utils-0.1.3/dta_utils/services/dta_chat_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     7278 2024-03-26 19:46:17.000000 totvs-dta-utils-0.1.3/dta_utils/services/dta_observer_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-03-26 19:46:17.000000 totvs-dta-utils-0.1.3/dta_utils/services/dta_proxy_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    10726 2024-03-26 19:46:17.000000 totvs-dta-utils-0.1.3/dta_utils/services/dta_tracer_service.py
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-03-26 19:46:17.000000 totvs-dta-utils-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-26 19:46:17.928005 totvs-dta-utils-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-03-26 19:46:17.000000 totvs-dta-utils-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 19:46:17.928005 totvs-dta-utils-0.1.3/totvs_dta_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5590 2024-03-26 19:46:17.000000 totvs-dta-utils-0.1.3/totvs_dta_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-03-26 19:46:17.000000 totvs-dta-utils-0.1.3/totvs_dta_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 19:46:17.000000 totvs-dta-utils-0.1.3/totvs_dta_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-26 19:46:17.000000 totvs-dta-utils-0.1.3/totvs_dta_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-26 19:46:17.000000 totvs-dta-utils-0.1.3/totvs_dta_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:29:44.409181 totvs-dta-utils-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     5590 2024-04-25 17:29:44.409181 totvs-dta-utils-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5303 2024-04-25 17:29:42.000000 totvs-dta-utils-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:29:44.409181 totvs-dta-utils-0.1.4/dta_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-25 17:29:42.000000 totvs-dta-utils-0.1.4/dta_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:29:44.409181 totvs-dta-utils-0.1.4/dta_utils/services/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 17:29:42.000000 totvs-dta-utils-0.1.4/dta_utils/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-04-25 17:29:42.000000 totvs-dta-utils-0.1.4/dta_utils/services/dta_chat_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7278 2024-04-25 17:29:42.000000 totvs-dta-utils-0.1.4/dta_utils/services/dta_observer_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-04-25 17:29:42.000000 totvs-dta-utils-0.1.4/dta_utils/services/dta_proxy_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10813 2024-04-25 17:29:42.000000 totvs-dta-utils-0.1.4/dta_utils/services/dta_tracer_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-25 17:29:43.000000 totvs-dta-utils-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 17:29:44.409181 totvs-dta-utils-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-04-25 17:29:43.000000 totvs-dta-utils-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:29:44.409181 totvs-dta-utils-0.1.4/totvs_dta_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5590 2024-04-25 17:29:44.000000 totvs-dta-utils-0.1.4/totvs_dta_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-25 17:29:44.000000 totvs-dta-utils-0.1.4/totvs_dta_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 17:29:44.000000 totvs-dta-utils-0.1.4/totvs_dta_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-25 17:29:44.000000 totvs-dta-utils-0.1.4/totvs_dta_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-25 17:29:44.000000 totvs-dta-utils-0.1.4/totvs_dta_utils.egg-info/top_level.txt
```

### Comparing `totvs-dta-utils-0.1.3/PKG-INFO` & `totvs-dta-utils-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: totvs-dta-utils
-Version: 0.1.3
+Version: 0.1.4
 Summary: Lib for integration with DTA services
 Home-page: https://github.com/totvs-ai/dta-utils-python
 Author: TotvsLabs
 Author-email: info@totvs.ai
 Keywords: dta
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `totvs-dta-utils-0.1.3/README.md` & `totvs-dta-utils-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `totvs-dta-utils-0.1.3/dta_utils/services/dta_chat_service.py` & `totvs-dta-utils-0.1.4/dta_utils/services/dta_chat_service.py`

 * *Files identical despite different names*

### Comparing `totvs-dta-utils-0.1.3/dta_utils/services/dta_observer_service.py` & `totvs-dta-utils-0.1.4/dta_utils/services/dta_observer_service.py`

 * *Files identical despite different names*

### Comparing `totvs-dta-utils-0.1.3/dta_utils/services/dta_proxy_service.py` & `totvs-dta-utils-0.1.4/dta_utils/services/dta_proxy_service.py`

 * *Files identical despite different names*

### Comparing `totvs-dta-utils-0.1.3/dta_utils/services/dta_tracer_service.py` & `totvs-dta-utils-0.1.4/dta_utils/services/dta_tracer_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -182,14 +182,15 @@
 
         use_config = cls.get_keys(config=config)
 
         return CallbackHandler(
             host=use_config.url,
             public_key=use_config.public_key,
             secret_key=use_config.secret_key,
+            stateful_client=kwargs.get("stateful_client", cls._create(config=config)),
             **kwargs,
         )
 
     @classmethod
     def _props_not_none(
         cls, *, init_props: dict[str, Any] = {}, **kwargs
     ) -> dict[str, Any]:
```

### Comparing `totvs-dta-utils-0.1.3/setup.py` & `totvs-dta-utils-0.1.4/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     readme = rf.read()
 
 requirements = ["langfuse==2.*"]
 
 setup(
     name="totvs-dta-utils",
     author="TotvsLabs",
-    version="0.1.3",
+    version="0.1.4",
     author_email="info@totvs.ai",
     python_requires=">=3.10",
     description="Lib for integration with DTA services",
     long_description=readme,
     long_description_content_type="text/markdown",
     install_requires=requirements,
     include_package_data=True,
```

### Comparing `totvs-dta-utils-0.1.3/totvs_dta_utils.egg-info/PKG-INFO` & `totvs-dta-utils-0.1.4/totvs_dta_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: totvs-dta-utils
-Version: 0.1.3
+Version: 0.1.4
 Summary: Lib for integration with DTA services
 Home-page: https://github.com/totvs-ai/dta-utils-python
 Author: TotvsLabs
 Author-email: info@totvs.ai
 Keywords: dta
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```


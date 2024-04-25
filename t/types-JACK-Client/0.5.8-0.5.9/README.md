# Comparing `tmp/types-JACK-Client-0.5.8.tar.gz` & `tmp/types-JACK-Client-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-JACK-Client-0.5.8.tar", last modified: Thu Apr 28 06:27:55 2022, max compression
+gzip compressed data, was "types-JACK-Client-0.5.9.tar", last modified: Sun Jun 19 09:17:55 2022, max compression
```

## Comparing `types-JACK-Client-0.5.8.tar` & `types-JACK-Client-0.5.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-28 06:27:55.252911 types-JACK-Client-0.5.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1030 2022-04-28 06:27:53.000000 types-JACK-Client-0.5.8/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)       21 2022-04-28 06:27:53.000000 types-JACK-Client-0.5.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1174 2022-04-28 06:27:55.252911 types-JACK-Client-0.5.8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-28 06:27:55.248911 types-JACK-Client-0.5.8/jack-stubs/
--rw-r--r--   0 runner    (1001) docker     (121)       62 2022-04-28 06:27:53.000000 types-JACK-Client-0.5.8/jack-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (121)    10685 2022-04-28 06:27:41.000000 types-JACK-Client-0.5.8/jack-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-04-28 06:27:55.252911 types-JACK-Client-0.5.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1526 2022-04-28 06:27:53.000000 types-JACK-Client-0.5.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-28 06:27:55.252911 types-JACK-Client-0.5.8/types_JACK_Client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1174 2022-04-28 06:27:55.000000 types-JACK-Client-0.5.8/types_JACK_Client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      246 2022-04-28 06:27:55.000000 types-JACK-Client-0.5.8/types_JACK_Client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-28 06:27:55.000000 types-JACK-Client-0.5.8/types_JACK_Client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-04-28 06:27:55.000000 types-JACK-Client-0.5.8/types_JACK_Client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-19 09:17:55.350688 types-JACK-Client-0.5.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-06-19 09:17:54.000000 types-JACK-Client-0.5.9/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (121)       21 2022-06-19 09:17:54.000000 types-JACK-Client-0.5.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     1222 2022-06-19 09:17:55.350688 types-JACK-Client-0.5.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-19 09:17:55.350688 types-JACK-Client-0.5.9/jack-stubs/
+-rw-r--r--   0 runner    (1001) docker     (121)       70 2022-06-19 09:17:54.000000 types-JACK-Client-0.5.9/jack-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (121)    10685 2022-06-19 09:17:41.000000 types-JACK-Client-0.5.9/jack-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-19 09:17:55.350688 types-JACK-Client-0.5.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1575 2022-06-19 09:17:54.000000 types-JACK-Client-0.5.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-19 09:17:55.350688 types-JACK-Client-0.5.9/types_JACK_Client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1222 2022-06-19 09:17:55.000000 types-JACK-Client-0.5.9/types_JACK_Client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      246 2022-06-19 09:17:55.000000 types-JACK-Client-0.5.9/types_JACK_Client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-19 09:17:55.000000 types-JACK-Client-0.5.9/types_JACK_Client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       11 2022-06-19 09:17:55.000000 types-JACK-Client-0.5.9/types_JACK_Client.egg-info/top_level.txt
```

### Comparing `types-JACK-Client-0.5.8/CHANGELOG.md` & `types-JACK-Client-0.5.9/CHANGELOG.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+## 0.5.9 (2022-06-19)
+
+stubtest: use separate table in METADATA.toml (#8096)
+
 ## 0.5.8 (2022-04-28)
 
 jack: Fix MidiPort properties (#7730)
 
 Fixes #7729
 
 https://github.com/spatialaudio/jackclient-python/blob/26b648a36143b1e3db6e6fc827ca927b0c93cbec/src/jack.py#L1950
```

### Comparing `types-JACK-Client-0.5.8/PKG-INFO` & `types-JACK-Client-0.5.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 Metadata-Version: 2.1
 Name: types-JACK-Client
-Version: 0.5.8
+Version: 0.5.9
 Summary: Typing stubs for JACK-Client
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/JACK-Client.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
 Classifier: Typing :: Stubs Only
 Description-Content-Type: text/markdown
 
 ## Typing stubs for JACK-Client
 
 This is a PEP 561 type stub package for the `JACK-Client` package.
 It can be used by type-checking tools like mypy, PyCharm, pytype etc. to check code
 that uses `JACK-Client`. The source for this package can be found at
 https://github.com/python/typeshed/tree/master/stubs/JACK-Client. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/master/README.md for more details.
-This package was generated from typeshed commit `1deb9cb80698127b48df1c17b5418e792bbc2103`.
+This package was generated from typeshed commit `411d85feebc96e24a8d0c2c21fba405b1d650ce7`.
```

### Comparing `types-JACK-Client-0.5.8/jack-stubs/__init__.pyi` & `types-JACK-Client-0.5.9/jack-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-JACK-Client-0.5.8/setup.py` & `types-JACK-Client-0.5.9/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,19 +8,19 @@
 This is a PEP 561 type stub package for the `JACK-Client` package.
 It can be used by type-checking tools like mypy, PyCharm, pytype etc. to check code
 that uses `JACK-Client`. The source for this package can be found at
 https://github.com/python/typeshed/tree/master/stubs/JACK-Client. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/master/README.md for more details.
-This package was generated from typeshed commit `1deb9cb80698127b48df1c17b5418e792bbc2103`.
+This package was generated from typeshed commit `411d85feebc96e24a8d0c2c21fba405b1d650ce7`.
 '''.lstrip()
 
 setup(name=name,
-      version="0.5.8",
+      version="0.5.9",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/JACK-Client.md",
@@ -29,10 +29,11 @@
       },
       install_requires=[],
       packages=['jack-stubs'],
       package_data={'jack-stubs': ['__init__.pyi', 'METADATA.toml']},
       license="Apache-2.0 license",
       classifiers=[
           "License :: OSI Approved :: Apache Software License",
+          "Programming Language :: Python :: 3",
           "Typing :: Stubs Only",
       ]
 )
```

### Comparing `types-JACK-Client-0.5.8/types_JACK_Client.egg-info/PKG-INFO` & `types-JACK-Client-0.5.9/types_JACK_Client.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 Metadata-Version: 2.1
 Name: types-JACK-Client
-Version: 0.5.8
+Version: 0.5.9
 Summary: Typing stubs for JACK-Client
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/JACK-Client.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
 Classifier: Typing :: Stubs Only
 Description-Content-Type: text/markdown
 
 ## Typing stubs for JACK-Client
 
 This is a PEP 561 type stub package for the `JACK-Client` package.
 It can be used by type-checking tools like mypy, PyCharm, pytype etc. to check code
 that uses `JACK-Client`. The source for this package can be found at
 https://github.com/python/typeshed/tree/master/stubs/JACK-Client. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/master/README.md for more details.
-This package was generated from typeshed commit `1deb9cb80698127b48df1c17b5418e792bbc2103`.
+This package was generated from typeshed commit `411d85feebc96e24a8d0c2c21fba405b1d650ce7`.
```


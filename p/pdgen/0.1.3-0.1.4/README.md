# Comparing `tmp/pdgen-0.1.3.tar.gz` & `tmp/pdgen-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdgen-0.1.3.tar", last modified: Wed Apr 24 21:57:48 2024, max compression
+gzip compressed data, was "pdgen-0.1.4.tar", last modified: Wed Apr 24 22:16:31 2024, max compression
```

## Comparing `pdgen-0.1.3.tar` & `pdgen-0.1.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-04-24 21:57:48.713555 pdgen-0.1.3/
--rw-rw-rw-   0        0        0     1504 2024-04-24 21:57:48.712432 pdgen-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     1308 2024-04-24 21:57:41.000000 pdgen-0.1.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-24 21:57:48.713555 pdgen-0.1.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-24 21:57:48.685782 pdgen-0.1.3/src/
-drwxrwxrwx   0        0        0        0 2024-04-24 21:57:48.687946 pdgen-0.1.3/src/pdgen/
--rw-rw-rw-   0        0        0        0 2024-04-24 11:05:29.000000 pdgen-0.1.3/src/pdgen/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 21:57:48.709005 pdgen-0.1.3/src/pdgen/decorators/
--rw-rw-rw-   0        0        0        0 2024-04-24 18:00:32.000000 pdgen-0.1.3/src/pdgen/decorators/__init__.py
--rw-rw-rw-   0        0        0      687 2024-04-24 20:15:43.000000 pdgen-0.1.3/src/pdgen/decorators/decorators.py
--rw-rw-rw-   0        0        0     2185 2024-04-24 20:33:14.000000 pdgen-0.1.3/src/pdgen/decorators/generation.py
--rw-rw-rw-   0        0        0       82 2024-04-24 19:01:39.000000 pdgen-0.1.3/src/pdgen/decorators/store.py
--rw-rw-rw-   0        0        0     6590 2024-04-24 19:56:04.000000 pdgen-0.1.3/src/pdgen/decorators/uml_types.py
--rw-rw-rw-   0        0        0      730 2024-04-24 20:32:14.000000 pdgen-0.1.3/src/pdgen/diagram.py
-drwxrwxrwx   0        0        0        0 2024-04-24 21:57:48.711408 pdgen-0.1.3/src/pdgen.egg-info/
--rw-rw-rw-   0        0        0     1504 2024-04-24 21:57:48.000000 pdgen-0.1.3/src/pdgen.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      388 2024-04-24 21:57:48.000000 pdgen-0.1.3/src/pdgen.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-24 21:57:48.000000 pdgen-0.1.3/src/pdgen.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      348 2024-04-24 21:57:48.000000 pdgen-0.1.3/src/pdgen.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-04-24 21:57:48.000000 pdgen-0.1.3/src/pdgen.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-24 22:16:31.422407 pdgen-0.1.4/
+-rw-rw-rw-   0        0        0     1504 2024-04-24 22:16:31.421059 pdgen-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1308 2024-04-24 22:15:32.000000 pdgen-0.1.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-24 22:16:31.422407 pdgen-0.1.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-24 22:16:31.404502 pdgen-0.1.4/src/
+drwxrwxrwx   0        0        0        0 2024-04-24 22:16:31.407250 pdgen-0.1.4/src/pdgen/
+-rw-rw-rw-   0        0        0        0 2024-04-24 11:05:29.000000 pdgen-0.1.4/src/pdgen/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 22:16:31.418537 pdgen-0.1.4/src/pdgen/decorators/
+-rw-rw-rw-   0        0        0        0 2024-04-24 18:00:32.000000 pdgen-0.1.4/src/pdgen/decorators/__init__.py
+-rw-rw-rw-   0        0        0      687 2024-04-24 20:15:43.000000 pdgen-0.1.4/src/pdgen/decorators/decorators.py
+-rw-rw-rw-   0        0        0     2185 2024-04-24 20:33:14.000000 pdgen-0.1.4/src/pdgen/decorators/generation.py
+-rw-rw-rw-   0        0        0       82 2024-04-24 19:01:39.000000 pdgen-0.1.4/src/pdgen/decorators/store.py
+-rw-rw-rw-   0        0        0     6590 2024-04-24 19:56:04.000000 pdgen-0.1.4/src/pdgen/decorators/uml_types.py
+-rw-rw-rw-   0        0        0      730 2024-04-24 20:32:14.000000 pdgen-0.1.4/src/pdgen/diagram.py
+drwxrwxrwx   0        0        0        0 2024-04-24 22:16:31.420017 pdgen-0.1.4/src/pdgen.egg-info/
+-rw-rw-rw-   0        0        0     1504 2024-04-24 22:16:31.000000 pdgen-0.1.4/src/pdgen.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      388 2024-04-24 22:16:31.000000 pdgen-0.1.4/src/pdgen.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 22:16:31.000000 pdgen-0.1.4/src/pdgen.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      348 2024-04-24 22:16:31.000000 pdgen-0.1.4/src/pdgen.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-24 22:16:31.000000 pdgen-0.1.4/src/pdgen.egg-info/top_level.txt
```

### Comparing `pdgen-0.1.3/PKG-INFO` & `pdgen-0.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdgen
-Version: 0.1.3
+Version: 0.1.4
 Summary: A Python package for generating UML diagrams from Python code using PlantUML.
 Author-email: Tobias Bück <tab@softoft.de>
 Project-URL: Bug Reports, https://github.com/Softoft/pdgen/issues
 Project-URL: Source, https://github.com/Softoft/pdgen/
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pdgen-0.1.3/pyproject.toml` & `pdgen-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=42", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pdgen"
-version = "0.1.3"
+version = "0.1.4"
 authors = [{name="Tobias Bück", email="tab@softoft.de"}]
 description = "A Python package for generating UML diagrams from Python code using PlantUML."
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
```

### Comparing `pdgen-0.1.3/src/pdgen/decorators/decorators.py` & `pdgen-0.1.4/src/pdgen/decorators/decorators.py`

 * *Files identical despite different names*

### Comparing `pdgen-0.1.3/src/pdgen/decorators/generation.py` & `pdgen-0.1.4/src/pdgen/decorators/generation.py`

 * *Files identical despite different names*

### Comparing `pdgen-0.1.3/src/pdgen/decorators/uml_types.py` & `pdgen-0.1.4/src/pdgen/decorators/uml_types.py`

 * *Files identical despite different names*

### Comparing `pdgen-0.1.3/src/pdgen/diagram.py` & `pdgen-0.1.4/src/pdgen/diagram.py`

 * *Files identical despite different names*

### Comparing `pdgen-0.1.3/src/pdgen.egg-info/PKG-INFO` & `pdgen-0.1.4/src/pdgen.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdgen
-Version: 0.1.3
+Version: 0.1.4
 Summary: A Python package for generating UML diagrams from Python code using PlantUML.
 Author-email: Tobias Bück <tab@softoft.de>
 Project-URL: Bug Reports, https://github.com/Softoft/pdgen/issues
 Project-URL: Source, https://github.com/Softoft/pdgen/
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```


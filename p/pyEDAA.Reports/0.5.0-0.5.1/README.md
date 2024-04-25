# Comparing `tmp/pyedaa_reports-0.5.0.tar.gz` & `tmp/pyedaa_reports-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyedaa_reports-0.5.0.tar", last modified: Wed Apr 24 21:46:30 2024, max compression
+gzip compressed data, was "pyedaa_reports-0.5.1.tar", last modified: Thu Apr 25 19:28:10 2024, max compression
```

## Comparing `pyedaa_reports-0.5.0.tar` & `pyedaa_reports-0.5.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:46:30.908217 pyedaa_reports-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)    10571 2024-04-24 21:46:27.000000 pyedaa_reports-0.5.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     8957 2024-04-24 21:46:30.908217 pyedaa_reports-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5642 2024-04-24 21:46:27.000000 pyedaa_reports-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:46:30.896217 pyedaa_reports-0.5.0/pyEDAA/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:46:30.900217 pyedaa_reports-0.5.0/pyEDAA/Reports/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:46:30.900217 pyedaa_reports-0.5.0/pyEDAA/Reports/CLI/
--rw-r--r--   0 runner    (1001) docker     (127)     2313 2024-04-24 21:46:27.000000 pyedaa_reports-0.5.0/pyEDAA/Reports/CLI/Unittesting.py
--rw-r--r--   0 runner    (1001) docker     (127)     8403 2024-04-24 21:46:27.000000 pyedaa_reports-0.5.0/pyEDAA/Reports/CLI/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:46:30.900217 pyedaa_reports-0.5.0/pyEDAA/Reports/Dependency/
--rw-r--r--   0 runner    (1001) docker     (127)     3512 2024-04-24 21:46:27.000000 pyedaa_reports-0.5.0/pyEDAA/Reports/Dependency/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:46:30.900217 pyedaa_reports-0.5.0/pyEDAA/Reports/DocumentationCoverage/
--rw-r--r--   0 runner    (1001) docker     (127)    17852 2024-04-24 21:46:27.000000 pyedaa_reports-0.5.0/pyEDAA/Reports/DocumentationCoverage/Python.py
--rw-r--r--   0 runner    (1001) docker     (127)     4921 2024-04-24 21:46:27.000000 pyedaa_reports-0.5.0/pyEDAA/Reports/DocumentationCoverage/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:46:30.900217 pyedaa_reports-0.5.0/pyEDAA/Reports/Requirement/
--rw-r--r--   0 runner    (1001) docker     (127)     4372 2024-04-24 21:46:27.000000 pyedaa_reports-0.5.0/pyEDAA/Reports/Requirement/Python.py
--rw-r--r--   0 runner    (1001) docker     (127)     3512 2024-04-24 21:46:27.000000 pyedaa_reports-0.5.0/pyEDAA/Reports/Requirement/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:46:30.900217 pyedaa_reports-0.5.0/pyEDAA/Reports/Unittesting/
--rw-r--r--   0 runner    (1001) docker     (127)    13651 2024-04-24 21:46:27.000000 pyedaa_reports-0.5.0/pyEDAA/Reports/Unittesting/JUnit.py
--rw-r--r--   0 runner    (1001) docker     (127)     8761 2024-04-24 21:46:27.000000 pyedaa_reports-0.5.0/pyEDAA/Reports/Unittesting/OSVVM.py
--rw-r--r--   0 runner    (1001) docker     (127)    34747 2024-04-24 21:46:27.000000 pyedaa_reports-0.5.0/pyEDAA/Reports/Unittesting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4829 2024-04-24 21:46:27.000000 pyedaa_reports-0.5.0/pyEDAA/Reports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 21:46:27.000000 pyedaa_reports-0.5.0/pyEDAA/Reports/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:46:30.900217 pyedaa_reports-0.5.0/pyEDAA/Reports/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     6291 2024-04-24 21:46:27.000000 pyedaa_reports-0.5.0/pyEDAA/Reports/resources/Unittesting.xsd
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 21:46:27.000000 pyedaa_reports-0.5.0/pyEDAA/Reports/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:46:30.900217 pyedaa_reports-0.5.0/pyEDAA.Reports.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8957 2024-04-24 21:46:30.000000 pyedaa_reports-0.5.0/pyEDAA.Reports.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-24 21:46:30.000000 pyedaa_reports-0.5.0/pyEDAA.Reports.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 21:46:30.000000 pyedaa_reports-0.5.0/pyEDAA.Reports.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-24 21:46:30.000000 pyedaa_reports-0.5.0/pyEDAA.Reports.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-24 21:46:30.000000 pyedaa_reports-0.5.0/pyEDAA.Reports.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-24 21:46:30.000000 pyedaa_reports-0.5.0/pyEDAA.Reports.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-04-24 21:46:27.000000 pyedaa_reports-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 21:46:30.908217 pyedaa_reports-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-04-24 21:46:27.000000 pyedaa_reports-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:28:10.908492 pyedaa_reports-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    10571 2024-04-25 19:28:07.000000 pyedaa_reports-0.5.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8957 2024-04-25 19:28:10.908492 pyedaa_reports-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5642 2024-04-25 19:28:07.000000 pyedaa_reports-0.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:28:10.896492 pyedaa_reports-0.5.1/pyEDAA/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:28:10.900492 pyedaa_reports-0.5.1/pyEDAA/Reports/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:28:10.900492 pyedaa_reports-0.5.1/pyEDAA/Reports/CLI/
+-rw-r--r--   0 runner    (1001) docker     (127)     2313 2024-04-25 19:28:07.000000 pyedaa_reports-0.5.1/pyEDAA/Reports/CLI/Unittesting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8403 2024-04-25 19:28:07.000000 pyedaa_reports-0.5.1/pyEDAA/Reports/CLI/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:28:10.900492 pyedaa_reports-0.5.1/pyEDAA/Reports/Dependency/
+-rw-r--r--   0 runner    (1001) docker     (127)     3512 2024-04-25 19:28:07.000000 pyedaa_reports-0.5.1/pyEDAA/Reports/Dependency/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:28:10.900492 pyedaa_reports-0.5.1/pyEDAA/Reports/DocumentationCoverage/
+-rw-r--r--   0 runner    (1001) docker     (127)    17852 2024-04-25 19:28:07.000000 pyedaa_reports-0.5.1/pyEDAA/Reports/DocumentationCoverage/Python.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4921 2024-04-25 19:28:07.000000 pyedaa_reports-0.5.1/pyEDAA/Reports/DocumentationCoverage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:28:10.900492 pyedaa_reports-0.5.1/pyEDAA/Reports/Requirement/
+-rw-r--r--   0 runner    (1001) docker     (127)     4372 2024-04-25 19:28:07.000000 pyedaa_reports-0.5.1/pyEDAA/Reports/Requirement/Python.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3512 2024-04-25 19:28:07.000000 pyedaa_reports-0.5.1/pyEDAA/Reports/Requirement/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:28:10.904492 pyedaa_reports-0.5.1/pyEDAA/Reports/Unittesting/
+-rw-r--r--   0 runner    (1001) docker     (127)    14334 2024-04-25 19:28:07.000000 pyedaa_reports-0.5.1/pyEDAA/Reports/Unittesting/JUnit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8761 2024-04-25 19:28:07.000000 pyedaa_reports-0.5.1/pyEDAA/Reports/Unittesting/OSVVM.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35072 2024-04-25 19:28:07.000000 pyedaa_reports-0.5.1/pyEDAA/Reports/Unittesting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4829 2024-04-25 19:28:07.000000 pyedaa_reports-0.5.1/pyEDAA/Reports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 19:28:07.000000 pyedaa_reports-0.5.1/pyEDAA/Reports/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:28:10.904492 pyedaa_reports-0.5.1/pyEDAA/Reports/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     6291 2024-04-25 19:28:07.000000 pyedaa_reports-0.5.1/pyEDAA/Reports/resources/Unittesting.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 19:28:07.000000 pyedaa_reports-0.5.1/pyEDAA/Reports/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:28:10.904492 pyedaa_reports-0.5.1/pyEDAA.Reports.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8957 2024-04-25 19:28:10.000000 pyedaa_reports-0.5.1/pyEDAA.Reports.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-25 19:28:10.000000 pyedaa_reports-0.5.1/pyEDAA.Reports.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 19:28:10.000000 pyedaa_reports-0.5.1/pyEDAA.Reports.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-25 19:28:10.000000 pyedaa_reports-0.5.1/pyEDAA.Reports.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-25 19:28:10.000000 pyedaa_reports-0.5.1/pyEDAA.Reports.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-25 19:28:10.000000 pyedaa_reports-0.5.1/pyEDAA.Reports.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-04-25 19:28:07.000000 pyedaa_reports-0.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 19:28:10.908492 pyedaa_reports-0.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-04-25 19:28:07.000000 pyedaa_reports-0.5.1/setup.py
```

### Comparing `pyedaa_reports-0.5.0/LICENSE.md` & `pyedaa_reports-0.5.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyedaa_reports-0.5.0/PKG-INFO` & `pyedaa_reports-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyEDAA.Reports
-Version: 0.5.0
+Version: 0.5.1
 Summary: Various report abstract data models and report format converters.
 Home-page: https://GitHub.com/pyEDAA/pyEDAA.Reports
 Author: Patrick Lehmann
 Author-email: Paebbels@gmail.com
 License: Apache-2.0
 Project-URL: Documentation, https://pyEDAA.GitHub.io/pyEDAA.Reports
 Project-URL: Source Code, https://GitHub.com/pyEDAA/pyEDAA.Reports
@@ -18,61 +18,61 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Development Status :: 2 - Pre-Alpha
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
+Requires-Dist: ruamel.yaml~=0.18.6
 Requires-Dist: lxml~=5.1
 Requires-Dist: pyTooling~=6.1
-Requires-Dist: ruamel.yaml~=0.18.6
 Provides-Extra: doc
+Requires-Dist: sphinx_autodoc_typehints~=2.1; extra == "doc"
 Requires-Dist: ruamel.yaml~=0.18.6; extra == "doc"
-Requires-Dist: sphinx_reports~=0.6; extra == "doc"
-Requires-Dist: autoapi>=2.0.1; extra == "doc"
-Requires-Dist: sphinx_design>=0.5.0; extra == "doc"
-Requires-Dist: pyTooling~=6.1; extra == "doc"
+Requires-Dist: colorama>=0.4.6; extra == "doc"
+Requires-Dist: sphinx~=7.3; extra == "doc"
 Requires-Dist: docutils~=0.18.1; extra == "doc"
+Requires-Dist: setuptools~=69.5; extra == "doc"
 Requires-Dist: sphinx-copybutton>=0.5.2; extra == "doc"
+Requires-Dist: sphinxcontrib-mermaid>=0.9.2; extra == "doc"
+Requires-Dist: pyTooling~=6.1; extra == "doc"
+Requires-Dist: sphinx_design>=0.5.0; extra == "doc"
 Requires-Dist: lxml~=5.1; extra == "doc"
-Requires-Dist: setuptools~=69.5; extra == "doc"
-Requires-Dist: sphinx~=7.3; extra == "doc"
-Requires-Dist: colorama>=0.4.6; extra == "doc"
+Requires-Dist: sphinx_reports~=0.6; extra == "doc"
+Requires-Dist: autoapi>=2.0.1; extra == "doc"
 Requires-Dist: sphinx_rtd_theme~=2.0.0; extra == "doc"
-Requires-Dist: sphinxcontrib-mermaid>=0.9.2; extra == "doc"
-Requires-Dist: sphinx_autodoc_typehints~=2.1; extra == "doc"
 Provides-Extra: test
-Requires-Dist: pytest-cov~=5.0; extra == "test"
 Requires-Dist: ruamel.yaml~=0.18.6; extra == "test"
-Requires-Dist: mypy~=1.10; extra == "test"
 Requires-Dist: pytest~=8.1; extra == "test"
 Requires-Dist: Coverage~=7.5; extra == "test"
+Requires-Dist: mypy~=1.10; extra == "test"
 Requires-Dist: pyTooling~=6.1; extra == "test"
 Requires-Dist: lxml~=5.1; extra == "test"
+Requires-Dist: pytest-cov~=5.0; extra == "test"
 Requires-Dist: typing_extensions~=4.11; extra == "test"
 Provides-Extra: all
-Requires-Dist: autoapi>=2.0.1; extra == "all"
-Requires-Dist: sphinx-copybutton>=0.5.2; extra == "all"
-Requires-Dist: lxml~=5.1; extra == "all"
-Requires-Dist: typing_extensions~=4.11; extra == "all"
-Requires-Dist: sphinxcontrib-mermaid>=0.9.2; extra == "all"
-Requires-Dist: pyTooling~=6.1; extra == "all"
-Requires-Dist: setuptools~=69.5; extra == "all"
-Requires-Dist: sphinx_rtd_theme~=2.0.0; extra == "all"
 Requires-Dist: sphinx_autodoc_typehints~=2.1; extra == "all"
-Requires-Dist: pytest-cov~=5.0; extra == "all"
 Requires-Dist: ruamel.yaml~=0.18.6; extra == "all"
-Requires-Dist: pytest~=8.1; extra == "all"
+Requires-Dist: Coverage~=7.5; extra == "all"
+Requires-Dist: pytest-cov~=5.0; extra == "all"
+Requires-Dist: sphinx_reports~=0.6; extra == "all"
+Requires-Dist: sphinx_rtd_theme~=2.0.0; extra == "all"
+Requires-Dist: sphinx-copybutton>=0.5.2; extra == "all"
 Requires-Dist: sphinx_design>=0.5.0; extra == "all"
+Requires-Dist: pyTooling~=6.1; extra == "all"
+Requires-Dist: lxml~=5.1; extra == "all"
+Requires-Dist: typing_extensions~=4.11; extra == "all"
+Requires-Dist: colorama>=0.4.6; extra == "all"
+Requires-Dist: docutils~=0.18.1; extra == "all"
 Requires-Dist: sphinx~=7.3; extra == "all"
-Requires-Dist: sphinx_reports~=0.6; extra == "all"
 Requires-Dist: mypy~=1.10; extra == "all"
-Requires-Dist: docutils~=0.18.1; extra == "all"
-Requires-Dist: Coverage~=7.5; extra == "all"
-Requires-Dist: colorama>=0.4.6; extra == "all"
+Requires-Dist: pytest~=8.1; extra == "all"
+Requires-Dist: setuptools~=69.5; extra == "all"
+Requires-Dist: sphinxcontrib-mermaid>=0.9.2; extra == "all"
+Requires-Dist: autoapi>=2.0.1; extra == "all"
 
 <p align="center">
   <a title="edaa-org.github.io/pyEDAA.Reports" href="https://edaa-org.github.io/pyEDAA.Reports"><img height="80px" src="doc/_static/logo.svg"/></a>
 </p>
 
 [![Sourcecode on GitHub](https://img.shields.io/badge/pyEDAA-Reports-29b6f6.svg?longCache=true&style=flat-square&logo=GitHub&labelColor=0277bd)](https://GitHub.com/edaa-org/pyEDAA.Reports)
 [![Documentation](https://img.shields.io/website?longCache=true&style=flat-square&label=edaa-org.github.io%2FpyEDAA.Reports&logo=GitHub&logoColor=fff&up_color=blueviolet&up_message=Read%20now%20%E2%9E%9A&url=https%3A%2F%2Fedaa-org.github.io%2FpyEDAA.Reports%2Findex.html)](https://edaa-org.github.io/pyEDAA.Reports/)
```

### Comparing `pyedaa_reports-0.5.0/README.md` & `pyedaa_reports-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `pyedaa_reports-0.5.0/pyEDAA/Reports/CLI/Unittesting.py` & `pyedaa_reports-0.5.1/pyEDAA/Reports/CLI/Unittesting.py`

 * *Files identical despite different names*

### Comparing `pyedaa_reports-0.5.0/pyEDAA/Reports/CLI/__init__.py` & `pyedaa_reports-0.5.1/pyEDAA/Reports/CLI/__init__.py`

 * *Files identical despite different names*

### Comparing `pyedaa_reports-0.5.0/pyEDAA/Reports/Dependency/__init__.py` & `pyedaa_reports-0.5.1/pyEDAA/Reports/Dependency/__init__.py`

 * *Files identical despite different names*

### Comparing `pyedaa_reports-0.5.0/pyEDAA/Reports/DocumentationCoverage/Python.py` & `pyedaa_reports-0.5.1/pyEDAA/Reports/DocumentationCoverage/Python.py`

 * *Files identical despite different names*

### Comparing `pyedaa_reports-0.5.0/pyEDAA/Reports/DocumentationCoverage/__init__.py` & `pyedaa_reports-0.5.1/pyEDAA/Reports/DocumentationCoverage/__init__.py`

 * *Files identical despite different names*

### Comparing `pyedaa_reports-0.5.0/pyEDAA/Reports/Requirement/Python.py` & `pyedaa_reports-0.5.1/pyEDAA/Reports/Requirement/Python.py`

 * *Files identical despite different names*

### Comparing `pyedaa_reports-0.5.0/pyEDAA/Reports/Requirement/__init__.py` & `pyedaa_reports-0.5.1/pyEDAA/Reports/Requirement/__init__.py`

 * *Files identical despite different names*

### Comparing `pyedaa_reports-0.5.0/pyEDAA/Reports/Unittesting/JUnit.py` & `pyedaa_reports-0.5.1/pyEDAA/Reports/Unittesting/JUnit.py`

 * *Files 3% similar despite different names*

```diff
@@ -262,27 +262,39 @@
 
 		rootElement = Element("testsuites")
 		rootElement.attrib["name"] = self._name
 		if self._startTime is not None:
 			rootElement.attrib["timestamp"] = f"{self._startTime.isoformat()}"
 		if self._totalDuration is not None:
 			rootElement.attrib["time"] = f"{self._totalDuration.total_seconds():.6f}"
+		rootElement.attrib["tests"] = str(self._tests)
+		rootElement.attrib["failures"] = str(self._failed)
+		rootElement.attrib["errors"] = str(self._errored)
+		rootElement.attrib["skipped"] = str(self._skipped)
+		# if self._assertionCount is not None:
+		# 	rootElement.attrib["assertions"] = f"{self._assertionCount}"
 
 		self._xmlDocument = ElementTree(rootElement)
 
 		for testsuite in self._testsuites.values():
 			self._GenerateTestsuite(testsuite, rootElement)
 
 	def _GenerateTestsuite(self, testsuite: Testsuite, parentElement: _Element):
 		testsuiteElement = SubElement(parentElement, "testsuite")
 		testsuiteElement.attrib["name"] = testsuite._name
 		if testsuite._startTime is not None:
 			testsuiteElement.attrib["timestamp"] = f"{testsuite._startTime.isoformat()}"
 		if testsuite._totalDuration is not None:
 			testsuiteElement.attrib["time"] = f"{testsuite._totalDuration.total_seconds():.6f}"
+		testsuiteElement.attrib["tests"] = str(testsuite._tests)
+		testsuiteElement.attrib["failures"] = str(testsuite._failed)
+		testsuiteElement.attrib["errors"] = str(testsuite._errored)
+		testsuiteElement.attrib["skipped"] = str(testsuite._skipped)
+		# if testsuite._assertionCount is not None:
+		# 	testsuiteElement.attrib["assertions"] = f"{testsuite._assertionCount}"
 
 		for ts in testsuite._testsuites.values():
 			self._GenerateTestsuite(ts, testsuiteElement)
 
 		for tc in testsuite._testcases.values():
 			self._GenerateTestcase(tc, testsuiteElement)
```

### Comparing `pyedaa_reports-0.5.0/pyEDAA/Reports/Unittesting/OSVVM.py` & `pyedaa_reports-0.5.1/pyEDAA/Reports/Unittesting/OSVVM.py`

 * *Files identical despite different names*

### Comparing `pyedaa_reports-0.5.0/pyEDAA/Reports/Unittesting/__init__.py` & `pyedaa_reports-0.5.1/pyEDAA/Reports/Unittesting/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -441,19 +441,22 @@
 				if testsuite._name in self._testsuites:
 					raise DuplicateTestsuiteException(f"Testsuite already contains a testsuite with same name '{testsuite._name}'.")
 
 				testsuite._parent = self
 				self._testsuites[testsuite._name] = testsuite
 
 		self._status = TestsuiteStatus.Unknown
-		self._excluded = 0
-		self._skipped =  0
-		self._errored =  0
-		self._failed =   0
-		self._passed =   0
+		self._tests =        0
+		self._inconsistent = 0
+		self._excluded =     0
+		self._skipped =      0
+		self._errored =      0
+		self._weak =         0
+		self._failed =       0
+		self._passed =       0
 
 	@readonly
 	def Status(self) -> TestsuiteStatus:
 		return self._status
 
 	@readonly
 	def Testsuites(self) -> Dict[str, TestsuiteType]:
@@ -479,48 +482,60 @@
 
 	@readonly
 	def PassedAssertionCount(self) -> int:
 		raise NotImplementedError()
 		# return self._assertionCount - (self._warningCount + self._errorCount + self._fatalCount)
 
 	@readonly
-	def WarningCount(self) -> int:
-		raise NotImplementedError()
-		# return self._warningCount
-
-	@readonly
-	def ErrorCount(self) -> int:
-		raise NotImplementedError()
-		# return self._errorCount
+	def Tests(self) -> int:
+		return self._tests
 
 	@readonly
-	def FatalCount(self) -> int:
-		raise NotImplementedError()
-		# return self._fatalCount
+	def Inconsistent(self) -> int:
+		return self._inconsistent
 
 	@readonly
 	def Excluded(self) -> int:
 		return self._excluded
 
 	@readonly
 	def Skipped(self) -> int:
 		return self._skipped
 
 	@readonly
 	def Errored(self) -> int:
 		return self._errored
 
 	@readonly
+	def Weak(self) -> int:
+		return self._weak
+
+	@readonly
 	def Failed(self) -> int:
 		return self._failed
 
 	@readonly
 	def Passed(self) -> int:
 		return self._passed
 
+	@readonly
+	def WarningCount(self) -> int:
+		raise NotImplementedError()
+		# return self._warningCount
+
+	@readonly
+	def ErrorCount(self) -> int:
+		raise NotImplementedError()
+		# return self._errorCount
+
+	@readonly
+	def FatalCount(self) -> int:
+		raise NotImplementedError()
+		# return self._fatalCount
+
 	def Aggregate(self) -> TestsuiteAggregateReturnType:
 		tests = 0
 		inconsistent = 0
 		excluded = 0
 		skipped = 0
 		errored = 0
 		weak = 0
@@ -690,14 +705,15 @@
 			elif status is TestcaseStatus.Failed:
 				failed += 1
 			elif status & TestcaseStatus.Mask is not TestcaseStatus.Unknown:
 				raise UnittestException(f"Found testcase '{testcase._name}' with unsupported state '{status}'.")
 			else:
 				raise UnittestException(f"Internal error for testcase '{testcase._name}', field '_status' is '{status}'.")
 
+		self._tests = tests
 		self._inconsistent = inconsistent
 		self._excluded = excluded
 		self._skipped = skipped
 		self._errored = errored
 		self._weak = weak
 		self._failed = failed
 		self._passed = passed
@@ -767,14 +783,15 @@
 		parent: Nullable[TestsuiteType] = None
 	):
 		super().__init__(name, startTime, setupDuration, teardownDuration, totalDuration, status, warningCount, errorCount, fatalCount, testsuites, parent)
 
 	def Aggregate(self) -> TestsuiteAggregateReturnType:
 		tests, inconsistent, excluded, skipped, errored, weak, failed, passed, warningCount, errorCount, fatalCount = super().Aggregate()
 
+		self._tests = tests
 		self._inconsistent = inconsistent
 		self._excluded = excluded
 		self._skipped = skipped
 		self._errored = errored
 		self._weak = weak
 		self._failed = failed
 		self._passed = passed
```

### Comparing `pyedaa_reports-0.5.0/pyEDAA/Reports/__init__.py` & `pyedaa_reports-0.5.1/pyEDAA/Reports/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 """
 Various report abstract data models and report format converters.
 """
 __author__ =    "Patrick Lehmann"
 __email__ =     "Paebbels@gmail.com"
 __copyright__ = "2021-2024, Electronic Design Automation Abstraction (EDA²)"
 __license__ =   "Apache License, Version 2.0"
-__version__ =   "0.5.0"
+__version__ =   "0.5.1"
 __keywords__ =  ["Reports", "Abstract Model", "Data Model", "Test Case", "Test Suite", "OSVVM", "YAML", "XML"]
 
 from enum                 import Enum
 from importlib.resources  import files
 from pathlib              import Path
 from sys                  import version_info
 from types                import ModuleType
```

### Comparing `pyedaa_reports-0.5.0/pyEDAA/Reports/resources/Unittesting.xsd` & `pyedaa_reports-0.5.1/pyEDAA/Reports/resources/Unittesting.xsd`

 * *Files identical despite different names*

### Comparing `pyedaa_reports-0.5.0/pyEDAA.Reports.egg-info/PKG-INFO` & `pyedaa_reports-0.5.1/pyEDAA.Reports.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyEDAA.Reports
-Version: 0.5.0
+Version: 0.5.1
 Summary: Various report abstract data models and report format converters.
 Home-page: https://GitHub.com/pyEDAA/pyEDAA.Reports
 Author: Patrick Lehmann
 Author-email: Paebbels@gmail.com
 License: Apache-2.0
 Project-URL: Documentation, https://pyEDAA.GitHub.io/pyEDAA.Reports
 Project-URL: Source Code, https://GitHub.com/pyEDAA/pyEDAA.Reports
@@ -18,61 +18,61 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Development Status :: 2 - Pre-Alpha
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
+Requires-Dist: ruamel.yaml~=0.18.6
 Requires-Dist: lxml~=5.1
 Requires-Dist: pyTooling~=6.1
-Requires-Dist: ruamel.yaml~=0.18.6
 Provides-Extra: doc
+Requires-Dist: sphinx_autodoc_typehints~=2.1; extra == "doc"
 Requires-Dist: ruamel.yaml~=0.18.6; extra == "doc"
-Requires-Dist: sphinx_reports~=0.6; extra == "doc"
-Requires-Dist: autoapi>=2.0.1; extra == "doc"
-Requires-Dist: sphinx_design>=0.5.0; extra == "doc"
-Requires-Dist: pyTooling~=6.1; extra == "doc"
+Requires-Dist: colorama>=0.4.6; extra == "doc"
+Requires-Dist: sphinx~=7.3; extra == "doc"
 Requires-Dist: docutils~=0.18.1; extra == "doc"
+Requires-Dist: setuptools~=69.5; extra == "doc"
 Requires-Dist: sphinx-copybutton>=0.5.2; extra == "doc"
+Requires-Dist: sphinxcontrib-mermaid>=0.9.2; extra == "doc"
+Requires-Dist: pyTooling~=6.1; extra == "doc"
+Requires-Dist: sphinx_design>=0.5.0; extra == "doc"
 Requires-Dist: lxml~=5.1; extra == "doc"
-Requires-Dist: setuptools~=69.5; extra == "doc"
-Requires-Dist: sphinx~=7.3; extra == "doc"
-Requires-Dist: colorama>=0.4.6; extra == "doc"
+Requires-Dist: sphinx_reports~=0.6; extra == "doc"
+Requires-Dist: autoapi>=2.0.1; extra == "doc"
 Requires-Dist: sphinx_rtd_theme~=2.0.0; extra == "doc"
-Requires-Dist: sphinxcontrib-mermaid>=0.9.2; extra == "doc"
-Requires-Dist: sphinx_autodoc_typehints~=2.1; extra == "doc"
 Provides-Extra: test
-Requires-Dist: pytest-cov~=5.0; extra == "test"
 Requires-Dist: ruamel.yaml~=0.18.6; extra == "test"
-Requires-Dist: mypy~=1.10; extra == "test"
 Requires-Dist: pytest~=8.1; extra == "test"
 Requires-Dist: Coverage~=7.5; extra == "test"
+Requires-Dist: mypy~=1.10; extra == "test"
 Requires-Dist: pyTooling~=6.1; extra == "test"
 Requires-Dist: lxml~=5.1; extra == "test"
+Requires-Dist: pytest-cov~=5.0; extra == "test"
 Requires-Dist: typing_extensions~=4.11; extra == "test"
 Provides-Extra: all
-Requires-Dist: autoapi>=2.0.1; extra == "all"
-Requires-Dist: sphinx-copybutton>=0.5.2; extra == "all"
-Requires-Dist: lxml~=5.1; extra == "all"
-Requires-Dist: typing_extensions~=4.11; extra == "all"
-Requires-Dist: sphinxcontrib-mermaid>=0.9.2; extra == "all"
-Requires-Dist: pyTooling~=6.1; extra == "all"
-Requires-Dist: setuptools~=69.5; extra == "all"
-Requires-Dist: sphinx_rtd_theme~=2.0.0; extra == "all"
 Requires-Dist: sphinx_autodoc_typehints~=2.1; extra == "all"
-Requires-Dist: pytest-cov~=5.0; extra == "all"
 Requires-Dist: ruamel.yaml~=0.18.6; extra == "all"
-Requires-Dist: pytest~=8.1; extra == "all"
+Requires-Dist: Coverage~=7.5; extra == "all"
+Requires-Dist: pytest-cov~=5.0; extra == "all"
+Requires-Dist: sphinx_reports~=0.6; extra == "all"
+Requires-Dist: sphinx_rtd_theme~=2.0.0; extra == "all"
+Requires-Dist: sphinx-copybutton>=0.5.2; extra == "all"
 Requires-Dist: sphinx_design>=0.5.0; extra == "all"
+Requires-Dist: pyTooling~=6.1; extra == "all"
+Requires-Dist: lxml~=5.1; extra == "all"
+Requires-Dist: typing_extensions~=4.11; extra == "all"
+Requires-Dist: colorama>=0.4.6; extra == "all"
+Requires-Dist: docutils~=0.18.1; extra == "all"
 Requires-Dist: sphinx~=7.3; extra == "all"
-Requires-Dist: sphinx_reports~=0.6; extra == "all"
 Requires-Dist: mypy~=1.10; extra == "all"
-Requires-Dist: docutils~=0.18.1; extra == "all"
-Requires-Dist: Coverage~=7.5; extra == "all"
-Requires-Dist: colorama>=0.4.6; extra == "all"
+Requires-Dist: pytest~=8.1; extra == "all"
+Requires-Dist: setuptools~=69.5; extra == "all"
+Requires-Dist: sphinxcontrib-mermaid>=0.9.2; extra == "all"
+Requires-Dist: autoapi>=2.0.1; extra == "all"
 
 <p align="center">
   <a title="edaa-org.github.io/pyEDAA.Reports" href="https://edaa-org.github.io/pyEDAA.Reports"><img height="80px" src="doc/_static/logo.svg"/></a>
 </p>
 
 [![Sourcecode on GitHub](https://img.shields.io/badge/pyEDAA-Reports-29b6f6.svg?longCache=true&style=flat-square&logo=GitHub&labelColor=0277bd)](https://GitHub.com/edaa-org/pyEDAA.Reports)
 [![Documentation](https://img.shields.io/website?longCache=true&style=flat-square&label=edaa-org.github.io%2FpyEDAA.Reports&logo=GitHub&logoColor=fff&up_color=blueviolet&up_message=Read%20now%20%E2%9E%9A&url=https%3A%2F%2Fedaa-org.github.io%2FpyEDAA.Reports%2Findex.html)](https://edaa-org.github.io/pyEDAA.Reports/)
```

### Comparing `pyedaa_reports-0.5.0/pyEDAA.Reports.egg-info/SOURCES.txt` & `pyedaa_reports-0.5.1/pyEDAA.Reports.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyedaa_reports-0.5.0/pyEDAA.Reports.egg-info/requires.txt` & `pyedaa_reports-0.5.1/pyEDAA.Reports.egg-info/requires.txt`

 * *Ordering differences only*

 * *Files 5% similar despite different names*

```diff
@@ -1,50 +1,50 @@
+ruamel.yaml~=0.18.6
 lxml~=5.1
 pyTooling~=6.1
-ruamel.yaml~=0.18.6
 
 [all]
-autoapi>=2.0.1
-sphinx-copybutton>=0.5.2
-lxml~=5.1
-typing_extensions~=4.11
-sphinxcontrib-mermaid>=0.9.2
-pyTooling~=6.1
-setuptools~=69.5
-sphinx_rtd_theme~=2.0.0
 sphinx_autodoc_typehints~=2.1
-pytest-cov~=5.0
 ruamel.yaml~=0.18.6
-pytest~=8.1
+Coverage~=7.5
+pytest-cov~=5.0
+sphinx_reports~=0.6
+sphinx_rtd_theme~=2.0.0
+sphinx-copybutton>=0.5.2
 sphinx_design>=0.5.0
+pyTooling~=6.1
+lxml~=5.1
+typing_extensions~=4.11
+colorama>=0.4.6
+docutils~=0.18.1
 sphinx~=7.3
-sphinx_reports~=0.6
 mypy~=1.10
-docutils~=0.18.1
-Coverage~=7.5
-colorama>=0.4.6
+pytest~=8.1
+setuptools~=69.5
+sphinxcontrib-mermaid>=0.9.2
+autoapi>=2.0.1
 
 [doc]
+sphinx_autodoc_typehints~=2.1
 ruamel.yaml~=0.18.6
-sphinx_reports~=0.6
-autoapi>=2.0.1
-sphinx_design>=0.5.0
-pyTooling~=6.1
+colorama>=0.4.6
+sphinx~=7.3
 docutils~=0.18.1
+setuptools~=69.5
 sphinx-copybutton>=0.5.2
+sphinxcontrib-mermaid>=0.9.2
+pyTooling~=6.1
+sphinx_design>=0.5.0
 lxml~=5.1
-setuptools~=69.5
-sphinx~=7.3
-colorama>=0.4.6
+sphinx_reports~=0.6
+autoapi>=2.0.1
 sphinx_rtd_theme~=2.0.0
-sphinxcontrib-mermaid>=0.9.2
-sphinx_autodoc_typehints~=2.1
 
 [test]
-pytest-cov~=5.0
 ruamel.yaml~=0.18.6
-mypy~=1.10
 pytest~=8.1
 Coverage~=7.5
+mypy~=1.10
 pyTooling~=6.1
 lxml~=5.1
+pytest-cov~=5.0
 typing_extensions~=4.11
```

### Comparing `pyedaa_reports-0.5.0/pyproject.toml` & `pyedaa_reports-0.5.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyedaa_reports-0.5.0/setup.py` & `pyedaa_reports-0.5.1/setup.py`

 * *Files identical despite different names*


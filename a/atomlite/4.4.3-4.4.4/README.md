# Comparing `tmp/atomlite-4.4.3.tar.gz` & `tmp/atomlite-4.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atomlite-4.4.3.tar", last modified: Thu Apr 25 09:39:06 2024, max compression
+gzip compressed data, was "atomlite-4.4.4.tar", last modified: Thu Apr 25 10:24:39 2024, max compression
```

## Comparing `atomlite-4.4.3.tar` & `atomlite-4.4.4.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:39:06.526127 atomlite-4.4.3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:39:06.518127 atomlite-4.4.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:39:06.522127 atomlite-4.4.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-04-25 09:38:44.000000 atomlite-4.4.3/.github/workflows/publish_release.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-04-25 09:38:44.000000 atomlite-4.4.3/.github/workflows/tests.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-25 09:38:44.000000 atomlite-4.4.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-25 09:38:44.000000 atomlite-4.4.3/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-04-25 09:38:44.000000 atomlite-4.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-04-25 09:39:06.526127 atomlite-4.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-04-25 09:38:44.000000 atomlite-4.4.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:39:06.522127 atomlite-4.4.3/data/
--rw-r--r--   0 runner    (1001) docker     (127)    45056 2024-04-25 09:38:44.000000 atomlite-4.4.3/data/atomlite.db
--rw-r--r--   0 runner    (1001) docker     (127)    58447 2024-04-25 09:38:44.000000 atomlite-4.4.3/data/molecules.sdf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:39:06.522127 atomlite-4.4.3/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-25 09:38:44.000000 atomlite-4.4.3/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:39:06.522127 atomlite-4.4.3/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:39:06.522127 atomlite-4.4.3/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 09:38:44.000000 atomlite-4.4.3/docs/source/_static/empty
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:39:06.522127 atomlite-4.4.3/docs/source/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-25 09:38:44.000000 atomlite-4.4.3/docs/source/_templates/class.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-04-25 09:38:44.000000 atomlite-4.4.3/docs/source/_templates/module.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-04-25 09:38:44.000000 atomlite-4.4.3/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)    15307 2024-04-25 09:38:44.000000 atomlite-4.4.3/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-25 09:38:44.000000 atomlite-4.4.3/docs/source/modules.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:39:06.522127 atomlite-4.4.3/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-25 09:38:44.000000 atomlite-4.4.3/examples/from_sdf.py
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-25 09:38:44.000000 atomlite-4.4.3/examples/read_database.py
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-25 09:38:44.000000 atomlite-4.4.3/justfile
--rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-04-25 09:38:44.000000 atomlite-4.4.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 09:39:06.526127 atomlite-4.4.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:39:06.518127 atomlite-4.4.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:39:06.522127 atomlite-4.4.3/src/atomlite/
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-25 09:38:44.000000 atomlite-4.4.3/src/atomlite/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:39:06.522127 atomlite-4.4.3/src/atomlite/_internal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 09:38:44.000000 atomlite-4.4.3/src/atomlite/_internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31786 2024-04-25 09:38:44.000000 atomlite-4.4.3/src/atomlite/_internal/database.py
--rw-r--r--   0 runner    (1001) docker     (127)     5493 2024-04-25 09:38:44.000000 atomlite-4.4.3/src/atomlite/_internal/json.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 09:38:44.000000 atomlite-4.4.3/src/atomlite/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:39:06.526127 atomlite-4.4.3/src/atomlite.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-04-25 09:39:06.000000 atomlite-4.4.3/src/atomlite.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-25 09:39:06.000000 atomlite-4.4.3/src/atomlite.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 09:39:06.000000 atomlite-4.4.3/src/atomlite.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-25 09:39:06.000000 atomlite-4.4.3/src/atomlite.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-25 09:39:06.000000 atomlite-4.4.3/src/atomlite.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:39:06.522127 atomlite-4.4.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    25166 2024-04-25 09:38:44.000000 atomlite-4.4.3/tests/test_database.py
--rw-r--r--   0 runner    (1001) docker     (127)      939 2024-04-25 09:38:44.000000 atomlite-4.4.3/tests/test_json_serde.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:24:39.215079 atomlite-4.4.4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:24:39.207079 atomlite-4.4.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:24:39.207079 atomlite-4.4.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-04-25 10:24:13.000000 atomlite-4.4.4/.github/workflows/publish_release.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-04-25 10:24:13.000000 atomlite-4.4.4/.github/workflows/tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-25 10:24:13.000000 atomlite-4.4.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-25 10:24:13.000000 atomlite-4.4.4/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-04-25 10:24:13.000000 atomlite-4.4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-04-25 10:24:39.215079 atomlite-4.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-04-25 10:24:13.000000 atomlite-4.4.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:24:39.207079 atomlite-4.4.4/data/
+-rw-r--r--   0 runner    (1001) docker     (127)    45056 2024-04-25 10:24:13.000000 atomlite-4.4.4/data/atomlite.db
+-rw-r--r--   0 runner    (1001) docker     (127)    58447 2024-04-25 10:24:13.000000 atomlite-4.4.4/data/molecules.sdf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:24:39.207079 atomlite-4.4.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-25 10:24:13.000000 atomlite-4.4.4/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:24:39.211079 atomlite-4.4.4/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:24:39.211079 atomlite-4.4.4/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 10:24:13.000000 atomlite-4.4.4/docs/source/_static/empty
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:24:39.211079 atomlite-4.4.4/docs/source/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-25 10:24:13.000000 atomlite-4.4.4/docs/source/_templates/class.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-04-25 10:24:13.000000 atomlite-4.4.4/docs/source/_templates/module.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-04-25 10:24:13.000000 atomlite-4.4.4/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15307 2024-04-25 10:24:13.000000 atomlite-4.4.4/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-25 10:24:13.000000 atomlite-4.4.4/docs/source/modules.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:24:39.211079 atomlite-4.4.4/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-25 10:24:13.000000 atomlite-4.4.4/examples/from_sdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-25 10:24:13.000000 atomlite-4.4.4/examples/read_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-25 10:24:13.000000 atomlite-4.4.4/justfile
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-04-25 10:24:13.000000 atomlite-4.4.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 10:24:39.215079 atomlite-4.4.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:24:39.207079 atomlite-4.4.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:24:39.211079 atomlite-4.4.4/src/atomlite/
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-25 10:24:13.000000 atomlite-4.4.4/src/atomlite/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:24:39.211079 atomlite-4.4.4/src/atomlite/_internal/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 10:24:13.000000 atomlite-4.4.4/src/atomlite/_internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31786 2024-04-25 10:24:13.000000 atomlite-4.4.4/src/atomlite/_internal/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5493 2024-04-25 10:24:13.000000 atomlite-4.4.4/src/atomlite/_internal/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 10:24:13.000000 atomlite-4.4.4/src/atomlite/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:24:39.211079 atomlite-4.4.4/src/atomlite.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-04-25 10:24:39.000000 atomlite-4.4.4/src/atomlite.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-25 10:24:39.000000 atomlite-4.4.4/src/atomlite.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 10:24:39.000000 atomlite-4.4.4/src/atomlite.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-25 10:24:39.000000 atomlite-4.4.4/src/atomlite.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-25 10:24:39.000000 atomlite-4.4.4/src/atomlite.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:24:39.211079 atomlite-4.4.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    25166 2024-04-25 10:24:13.000000 atomlite-4.4.4/tests/test_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-04-25 10:24:13.000000 atomlite-4.4.4/tests/test_json_serde.py
```

### Comparing `atomlite-4.4.3/.github/workflows/publish_release.yaml` & `atomlite-4.4.4/.github/workflows/publish_release.yaml`

 * *Files identical despite different names*

### Comparing `atomlite-4.4.3/.github/workflows/tests.yaml` & `atomlite-4.4.4/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `atomlite-4.4.3/LICENSE` & `atomlite-4.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `atomlite-4.4.3/PKG-INFO` & `atomlite-4.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atomlite
-Version: 4.4.3
+Version: 4.4.4
 Summary: A SQLite chemical database.
 Maintainer-email: Lukas Turcani <lukasturcani93@gmail.com>
 Project-URL: github, https://github.com/lukasturcani/atomlite
 Project-URL: documentation, https://atomlite.readthedocs.io
 Requires-Python: >=3.11
 Description-Content-Type: text/x-rst
 License-File: LICENSE
```

### Comparing `atomlite-4.4.3/README.rst` & `atomlite-4.4.4/README.rst`

 * *Files identical despite different names*

### Comparing `atomlite-4.4.3/data/atomlite.db` & `atomlite-4.4.4/data/atomlite.db`

 * *Files identical despite different names*

### Comparing `atomlite-4.4.3/data/molecules.sdf` & `atomlite-4.4.4/data/molecules.sdf`

 * *Files identical despite different names*

### Comparing `atomlite-4.4.3/docs/Makefile` & `atomlite-4.4.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `atomlite-4.4.3/docs/source/_templates/class.rst` & `atomlite-4.4.4/docs/source/_templates/class.rst`

 * *Files 12% similar despite different names*

```diff
@@ -16,15 +16,15 @@
    {% endif %}
    {% endblock %}
 
    {% block methods %}
 
    {% set direct_methods = [] %}
    {% for item in methods %}
-      {%- if not item.startswith('_') and item not in inherited_members %}
+      {%- if item not in inherited_members %}
         {% set direct_methods = direct_methods.append(item) %}
       {%- endif -%}
    {% endfor %}
 
    {% if direct_methods %}
    .. rubric:: {{ _('Methods') }}
```

### Comparing `atomlite-4.4.3/docs/source/_templates/module.rst` & `atomlite-4.4.4/docs/source/_templates/module.rst`

 * *Files identical despite different names*

### Comparing `atomlite-4.4.3/docs/source/conf.py` & `atomlite-4.4.4/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `atomlite-4.4.3/docs/source/index.rst` & `atomlite-4.4.4/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `atomlite-4.4.3/examples/from_sdf.py` & `atomlite-4.4.4/examples/from_sdf.py`

 * *Files identical despite different names*

### Comparing `atomlite-4.4.3/examples/read_database.py` & `atomlite-4.4.4/examples/read_database.py`

 * *Files identical despite different names*

### Comparing `atomlite-4.4.3/justfile` & `atomlite-4.4.4/justfile`

 * *Files identical despite different names*

### Comparing `atomlite-4.4.3/pyproject.toml` & `atomlite-4.4.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `atomlite-4.4.3/src/atomlite/__init__.py` & `atomlite-4.4.4/src/atomlite/__init__.py`

 * *Files identical despite different names*

### Comparing `atomlite-4.4.3/src/atomlite/_internal/database.py` & `atomlite-4.4.4/src/atomlite/_internal/database.py`

 * *Files identical despite different names*

### Comparing `atomlite-4.4.3/src/atomlite/_internal/json.py` & `atomlite-4.4.4/src/atomlite/_internal/json.py`

 * *Files identical despite different names*

### Comparing `atomlite-4.4.3/src/atomlite.egg-info/PKG-INFO` & `atomlite-4.4.4/src/atomlite.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atomlite
-Version: 4.4.3
+Version: 4.4.4
 Summary: A SQLite chemical database.
 Maintainer-email: Lukas Turcani <lukasturcani93@gmail.com>
 Project-URL: github, https://github.com/lukasturcani/atomlite
 Project-URL: documentation, https://atomlite.readthedocs.io
 Requires-Python: >=3.11
 Description-Content-Type: text/x-rst
 License-File: LICENSE
```

### Comparing `atomlite-4.4.3/src/atomlite.egg-info/SOURCES.txt` & `atomlite-4.4.4/src/atomlite.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `atomlite-4.4.3/tests/test_database.py` & `atomlite-4.4.4/tests/test_database.py`

 * *Files identical despite different names*

### Comparing `atomlite-4.4.3/tests/test_json_serde.py` & `atomlite-4.4.4/tests/test_json_serde.py`

 * *Files identical despite different names*


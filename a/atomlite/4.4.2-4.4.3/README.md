# Comparing `tmp/atomlite-4.4.2.tar.gz` & `tmp/atomlite-4.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atomlite-4.4.2.tar", last modified: Thu Feb 29 11:47:15 2024, max compression
+gzip compressed data, was "atomlite-4.4.3.tar", last modified: Thu Apr 25 09:39:06 2024, max compression
```

## Comparing `atomlite-4.4.2.tar` & `atomlite-4.4.3.tar`

### file list

```diff
@@ -1,41 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 11:47:15.540858 atomlite-4.4.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 11:47:15.532858 atomlite-4.4.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 11:47:15.536858 atomlite-4.4.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-02-29 11:46:48.000000 atomlite-4.4.2/.github/workflows/publish_release.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-02-29 11:46:48.000000 atomlite-4.4.2/.github/workflows/tests.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-02-29 11:46:48.000000 atomlite-4.4.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-02-29 11:46:48.000000 atomlite-4.4.2/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-02-29 11:46:48.000000 atomlite-4.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-02-29 11:47:15.540858 atomlite-4.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-02-29 11:46:48.000000 atomlite-4.4.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 11:47:15.536858 atomlite-4.4.2/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-02-29 11:46:48.000000 atomlite-4.4.2/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 11:47:15.536858 atomlite-4.4.2/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 11:47:15.536858 atomlite-4.4.2/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 11:46:48.000000 atomlite-4.4.2/docs/source/_static/empty
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 11:47:15.536858 atomlite-4.4.2/docs/source/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-02-29 11:46:48.000000 atomlite-4.4.2/docs/source/_templates/class.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-02-29 11:46:48.000000 atomlite-4.4.2/docs/source/_templates/module.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-02-29 11:46:48.000000 atomlite-4.4.2/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)    15307 2024-02-29 11:46:48.000000 atomlite-4.4.2/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-02-29 11:46:48.000000 atomlite-4.4.2/docs/source/modules.rst
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-02-29 11:46:48.000000 atomlite-4.4.2/justfile
--rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-02-29 11:46:48.000000 atomlite-4.4.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-29 11:47:15.540858 atomlite-4.4.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 11:47:15.532858 atomlite-4.4.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 11:47:15.536858 atomlite-4.4.2/src/atomlite/
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-02-29 11:46:48.000000 atomlite-4.4.2/src/atomlite/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 11:47:15.536858 atomlite-4.4.2/src/atomlite/_internal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 11:46:48.000000 atomlite-4.4.2/src/atomlite/_internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31786 2024-02-29 11:46:48.000000 atomlite-4.4.2/src/atomlite/_internal/database.py
--rw-r--r--   0 runner    (1001) docker     (127)     5493 2024-02-29 11:46:48.000000 atomlite-4.4.2/src/atomlite/_internal/json.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 11:46:48.000000 atomlite-4.4.2/src/atomlite/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 11:47:15.536858 atomlite-4.4.2/src/atomlite.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-02-29 11:47:15.000000 atomlite-4.4.2/src/atomlite.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-02-29 11:47:15.000000 atomlite-4.4.2/src/atomlite.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-29 11:47:15.000000 atomlite-4.4.2/src/atomlite.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-02-29 11:47:15.000000 atomlite-4.4.2/src/atomlite.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-02-29 11:47:15.000000 atomlite-4.4.2/src/atomlite.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 11:47:15.536858 atomlite-4.4.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    25166 2024-02-29 11:46:48.000000 atomlite-4.4.2/tests/test_database.py
--rw-r--r--   0 runner    (1001) docker     (127)      939 2024-02-29 11:46:48.000000 atomlite-4.4.2/tests/test_json_serde.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:39:06.526127 atomlite-4.4.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:39:06.518127 atomlite-4.4.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:39:06.522127 atomlite-4.4.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-04-25 09:38:44.000000 atomlite-4.4.3/.github/workflows/publish_release.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-04-25 09:38:44.000000 atomlite-4.4.3/.github/workflows/tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-25 09:38:44.000000 atomlite-4.4.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-25 09:38:44.000000 atomlite-4.4.3/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-04-25 09:38:44.000000 atomlite-4.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-04-25 09:39:06.526127 atomlite-4.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-04-25 09:38:44.000000 atomlite-4.4.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:39:06.522127 atomlite-4.4.3/data/
+-rw-r--r--   0 runner    (1001) docker     (127)    45056 2024-04-25 09:38:44.000000 atomlite-4.4.3/data/atomlite.db
+-rw-r--r--   0 runner    (1001) docker     (127)    58447 2024-04-25 09:38:44.000000 atomlite-4.4.3/data/molecules.sdf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:39:06.522127 atomlite-4.4.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-25 09:38:44.000000 atomlite-4.4.3/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:39:06.522127 atomlite-4.4.3/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:39:06.522127 atomlite-4.4.3/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 09:38:44.000000 atomlite-4.4.3/docs/source/_static/empty
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:39:06.522127 atomlite-4.4.3/docs/source/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-25 09:38:44.000000 atomlite-4.4.3/docs/source/_templates/class.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-04-25 09:38:44.000000 atomlite-4.4.3/docs/source/_templates/module.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-04-25 09:38:44.000000 atomlite-4.4.3/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15307 2024-04-25 09:38:44.000000 atomlite-4.4.3/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-25 09:38:44.000000 atomlite-4.4.3/docs/source/modules.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:39:06.522127 atomlite-4.4.3/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-25 09:38:44.000000 atomlite-4.4.3/examples/from_sdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-25 09:38:44.000000 atomlite-4.4.3/examples/read_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-25 09:38:44.000000 atomlite-4.4.3/justfile
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-04-25 09:38:44.000000 atomlite-4.4.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 09:39:06.526127 atomlite-4.4.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:39:06.518127 atomlite-4.4.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:39:06.522127 atomlite-4.4.3/src/atomlite/
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-25 09:38:44.000000 atomlite-4.4.3/src/atomlite/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:39:06.522127 atomlite-4.4.3/src/atomlite/_internal/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 09:38:44.000000 atomlite-4.4.3/src/atomlite/_internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31786 2024-04-25 09:38:44.000000 atomlite-4.4.3/src/atomlite/_internal/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5493 2024-04-25 09:38:44.000000 atomlite-4.4.3/src/atomlite/_internal/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 09:38:44.000000 atomlite-4.4.3/src/atomlite/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:39:06.526127 atomlite-4.4.3/src/atomlite.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-04-25 09:39:06.000000 atomlite-4.4.3/src/atomlite.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-25 09:39:06.000000 atomlite-4.4.3/src/atomlite.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 09:39:06.000000 atomlite-4.4.3/src/atomlite.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-25 09:39:06.000000 atomlite-4.4.3/src/atomlite.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-25 09:39:06.000000 atomlite-4.4.3/src/atomlite.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:39:06.522127 atomlite-4.4.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    25166 2024-04-25 09:38:44.000000 atomlite-4.4.3/tests/test_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-04-25 09:38:44.000000 atomlite-4.4.3/tests/test_json_serde.py
```

### Comparing `atomlite-4.4.2/.github/workflows/publish_release.yaml` & `atomlite-4.4.3/.github/workflows/publish_release.yaml`

 * *Files identical despite different names*

### Comparing `atomlite-4.4.2/LICENSE` & `atomlite-4.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `atomlite-4.4.2/PKG-INFO` & `atomlite-4.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atomlite
-Version: 4.4.2
+Version: 4.4.3
 Summary: A SQLite chemical database.
 Maintainer-email: Lukas Turcani <lukasturcani93@gmail.com>
 Project-URL: github, https://github.com/lukasturcani/atomlite
 Project-URL: documentation, https://atomlite.readthedocs.io
 Requires-Python: >=3.11
 Description-Content-Type: text/x-rst
 License-File: LICENSE
```

### Comparing `atomlite-4.4.2/README.rst` & `atomlite-4.4.3/README.rst`

 * *Files identical despite different names*

### Comparing `atomlite-4.4.2/docs/Makefile` & `atomlite-4.4.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `atomlite-4.4.2/docs/source/_templates/class.rst` & `atomlite-4.4.3/docs/source/_templates/class.rst`

 * *Files 23% similar despite different names*

```diff
@@ -1,31 +1,37 @@
 {{ fullname | escape | underline}}
 
 .. currentmodule:: {{ module }}
 
 .. autoclass:: {{ objname }}
    :members:
 
-   {% block methods %}
-   {% if methods %}
-   .. rubric:: {{ _('Methods') }}
+   {% block attributes %}
+   {% if attributes %}
+   .. rubric:: {{ _('Attributes') }}
 
    .. autosummary::
-      :nosignatures:
-   {% for item in methods %}
-      {%- if not item.startswith('_') and item not in inherited_members %}
+   {% for item in attributes %}
       ~{{ name }}.{{ item }}
-      {%- endif -%}
    {%- endfor %}
    {% endif %}
    {% endblock %}
 
-   {% block attributes %}
-   {% if attributes %}
-   .. rubric:: {{ _('Attributes') }}
+   {% block methods %}
+
+   {% set direct_methods = [] %}
+   {% for item in methods %}
+      {%- if not item.startswith('_') and item not in inherited_members %}
+        {% set direct_methods = direct_methods.append(item) %}
+      {%- endif -%}
+   {% endfor %}
+
+   {% if direct_methods %}
+   .. rubric:: {{ _('Methods') }}
 
    .. autosummary::
-   {% for item in attributes %}
+      :nosignatures:
+   {% for item in direct_methods %}
       ~{{ name }}.{{ item }}
    {%- endfor %}
    {% endif %}
    {% endblock %}
```

### Comparing `atomlite-4.4.2/docs/source/_templates/module.rst` & `atomlite-4.4.3/docs/source/_templates/module.rst`

 * *Files identical despite different names*

### Comparing `atomlite-4.4.2/docs/source/conf.py` & `atomlite-4.4.3/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `atomlite-4.4.2/docs/source/index.rst` & `atomlite-4.4.3/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `atomlite-4.4.2/justfile` & `atomlite-4.4.3/justfile`

 * *Files 15% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 check:
   #!/usr/bin/env bash
 
   error=0
   trap error=1 ERR
 
   echo
-  (set -x; ruff . )
+  (set -x; ruff check . )
 
   echo
   ( set -x; ruff format --check . )
 
   echo
   ( set -x; mypy . )
 
@@ -35,12 +35,12 @@
   ( set -x; make -C docs doctest )
 
   test $error = 0
 
 # Auto-fix code issues.
 fix:
   ruff format .
-  ruff --fix .
+  ruff check --fix .
 
 # Build a release.
 build:
   python -m build
```

### Comparing `atomlite-4.4.2/pyproject.toml` & `atomlite-4.4.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `atomlite-4.4.2/src/atomlite/__init__.py` & `atomlite-4.4.3/src/atomlite/__init__.py`

 * *Files identical despite different names*

### Comparing `atomlite-4.4.2/src/atomlite/_internal/database.py` & `atomlite-4.4.3/src/atomlite/_internal/database.py`

 * *Files identical despite different names*

### Comparing `atomlite-4.4.2/src/atomlite/_internal/json.py` & `atomlite-4.4.3/src/atomlite/_internal/json.py`

 * *Files identical despite different names*

### Comparing `atomlite-4.4.2/src/atomlite.egg-info/PKG-INFO` & `atomlite-4.4.3/src/atomlite.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atomlite
-Version: 4.4.2
+Version: 4.4.3
 Summary: A SQLite chemical database.
 Maintainer-email: Lukas Turcani <lukasturcani93@gmail.com>
 Project-URL: github, https://github.com/lukasturcani/atomlite
 Project-URL: documentation, https://atomlite.readthedocs.io
 Requires-Python: >=3.11
 Description-Content-Type: text/x-rst
 License-File: LICENSE
```

### Comparing `atomlite-4.4.2/src/atomlite.egg-info/SOURCES.txt` & `atomlite-4.4.3/src/atomlite.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -2,21 +2,25 @@
 .readthedocs.yaml
 LICENSE
 README.rst
 justfile
 pyproject.toml
 .github/workflows/publish_release.yaml
 .github/workflows/tests.yaml
+data/atomlite.db
+data/molecules.sdf
 docs/Makefile
 docs/source/conf.py
 docs/source/index.rst
 docs/source/modules.rst
 docs/source/_static/empty
 docs/source/_templates/class.rst
 docs/source/_templates/module.rst
+examples/from_sdf.py
+examples/read_database.py
 src/atomlite/__init__.py
 src/atomlite/py.typed
 src/atomlite.egg-info/PKG-INFO
 src/atomlite.egg-info/SOURCES.txt
 src/atomlite.egg-info/dependency_links.txt
 src/atomlite.egg-info/requires.txt
 src/atomlite.egg-info/top_level.txt
```

### Comparing `atomlite-4.4.2/tests/test_database.py` & `atomlite-4.4.3/tests/test_database.py`

 * *Files identical despite different names*

### Comparing `atomlite-4.4.2/tests/test_json_serde.py` & `atomlite-4.4.3/tests/test_json_serde.py`

 * *Files identical despite different names*


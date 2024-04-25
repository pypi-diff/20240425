# Comparing `tmp/ansible_doctor-4.0.4.tar.gz` & `tmp/ansible_doctor-4.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansible_doctor-4.0.4.tar", max compression
+gzip compressed data, was "ansible_doctor-4.0.5.tar", max compression
```

## Comparing `ansible_doctor-4.0.4.tar` & `ansible_doctor-4.0.5.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0    32460 2024-04-14 09:47:16.028640 ansible_doctor-4.0.4/LICENSE
--rw-r--r--   0        0        0     2717 2024-04-14 09:47:16.028640 ansible_doctor-4.0.4/README.md
--rw-r--r--   0        0        0      205 2024-04-14 09:47:31.484658 ansible_doctor-4.0.4/ansibledoctor/__init__.py
--rw-r--r--   0        0        0     6210 2024-04-14 09:47:16.028640 ansible_doctor-4.0.4/ansibledoctor/annotation.py
--rw-r--r--   0        0        0     4042 2024-04-14 09:47:16.028640 ansible_doctor-4.0.4/ansibledoctor/cli.py
--rw-r--r--   0        0        0    11957 2024-04-14 09:47:16.028640 ansible_doctor-4.0.4/ansibledoctor/config.py
--rw-r--r--   0        0        0      120 2024-04-14 09:47:16.028640 ansible_doctor-4.0.4/ansibledoctor/contstants.py
--rw-r--r--   0        0        0     7261 2024-04-14 09:47:16.028640 ansible_doctor-4.0.4/ansibledoctor/doc_generator.py
--rw-r--r--   0        0        0     4072 2024-04-14 09:47:16.028640 ansible_doctor-4.0.4/ansibledoctor/doc_parser.py
--rw-r--r--   0        0        0      558 2024-04-14 09:47:16.028640 ansible_doctor-4.0.4/ansibledoctor/exception.py
--rw-r--r--   0        0        0     1670 2024-04-14 09:47:16.028640 ansible_doctor-4.0.4/ansibledoctor/file_registry.py
--rw-r--r--   0        0        0      377 2024-04-14 09:47:16.028640 ansible_doctor-4.0.4/ansibledoctor/templates/hugo-book/_meta.j2
--rw-r--r--   0        0        0      172 2024-04-14 09:47:16.028640 ansible_doctor-4.0.4/ansibledoctor/templates/hugo-book/_requirements.j2
--rw-r--r--   0        0        0      318 2024-04-14 09:47:16.028640 ansible_doctor-4.0.4/ansibledoctor/templates/hugo-book/_tag.j2
--rw-r--r--   0        0        0      371 2024-04-14 09:47:16.028640 ansible_doctor-4.0.4/ansibledoctor/templates/hugo-book/_toc.j2
--rw-r--r--   0        0        0      583 2024-04-14 09:47:16.028640 ansible_doctor-4.0.4/ansibledoctor/templates/hugo-book/_todo.j2
--rw-r--r--   0        0        0     1558 2024-04-14 09:47:16.028640 ansible_doctor-4.0.4/ansibledoctor/templates/hugo-book/_vars.j2
--rw-r--r--   0        0        0      848 2024-04-14 09:47:16.028640 ansible_doctor-4.0.4/ansibledoctor/templates/hugo-book/index.md.j2
--rw-r--r--   0        0        0      697 2024-04-14 09:47:16.028640 ansible_doctor-4.0.4/ansibledoctor/templates/readme/README.md.j2
--rw-r--r--   0        0        0      691 2024-04-14 09:47:16.028640 ansible_doctor-4.0.4/ansibledoctor/templates/readme/_meta.j2
--rw-r--r--   0        0        0      172 2024-04-14 09:47:16.028640 ansible_doctor-4.0.4/ansibledoctor/templates/readme/_requirements.j2
--rw-r--r--   0        0        0      365 2024-04-14 09:47:16.028640 ansible_doctor-4.0.4/ansibledoctor/templates/readme/_tag.j2
--rw-r--r--   0        0        0      434 2024-04-14 09:47:16.028640 ansible_doctor-4.0.4/ansibledoctor/templates/readme/_toc.j2
--rw-r--r--   0        0        0      583 2024-04-14 09:47:16.028640 ansible_doctor-4.0.4/ansibledoctor/templates/readme/_todo.j2
--rw-r--r--   0        0        0     1558 2024-04-14 09:47:16.028640 ansible_doctor-4.0.4/ansibledoctor/templates/readme/_vars.j2
--rw-r--r--   0        0        0     9463 2024-04-14 09:47:16.028640 ansible_doctor-4.0.4/ansibledoctor/utils/__init__.py
--rw-r--r--   0        0        0     2412 2024-04-14 09:47:16.028640 ansible_doctor-4.0.4/ansibledoctor/utils/yamlhelper.py
--rw-r--r--   0        0        0     3174 2024-04-14 09:47:31.484658 ansible_doctor-4.0.4/pyproject.toml
--rw-r--r--   0        0        0     4427 1970-01-01 00:00:00.000000 ansible_doctor-4.0.4/PKG-INFO
+-rw-r--r--   0        0        0    32460 2024-04-25 08:27:16.071068 ansible_doctor-4.0.5/LICENSE
+-rw-r--r--   0        0        0     2717 2024-04-25 08:27:16.071068 ansible_doctor-4.0.5/README.md
+-rw-r--r--   0        0        0      205 2024-04-25 08:27:29.510962 ansible_doctor-4.0.5/ansibledoctor/__init__.py
+-rw-r--r--   0        0        0     6210 2024-04-25 08:27:16.071068 ansible_doctor-4.0.5/ansibledoctor/annotation.py
+-rw-r--r--   0        0        0     4042 2024-04-25 08:27:16.071068 ansible_doctor-4.0.5/ansibledoctor/cli.py
+-rw-r--r--   0        0        0    11957 2024-04-25 08:27:16.075068 ansible_doctor-4.0.5/ansibledoctor/config.py
+-rw-r--r--   0        0        0      120 2024-04-25 08:27:16.075068 ansible_doctor-4.0.5/ansibledoctor/contstants.py
+-rw-r--r--   0        0        0     7261 2024-04-25 08:27:16.075068 ansible_doctor-4.0.5/ansibledoctor/doc_generator.py
+-rw-r--r--   0        0        0     4072 2024-04-25 08:27:16.075068 ansible_doctor-4.0.5/ansibledoctor/doc_parser.py
+-rw-r--r--   0        0        0      558 2024-04-25 08:27:16.075068 ansible_doctor-4.0.5/ansibledoctor/exception.py
+-rw-r--r--   0        0        0     1670 2024-04-25 08:27:16.075068 ansible_doctor-4.0.5/ansibledoctor/file_registry.py
+-rw-r--r--   0        0        0      377 2024-04-25 08:27:16.075068 ansible_doctor-4.0.5/ansibledoctor/templates/hugo-book/_meta.j2
+-rw-r--r--   0        0        0      172 2024-04-25 08:27:16.075068 ansible_doctor-4.0.5/ansibledoctor/templates/hugo-book/_requirements.j2
+-rw-r--r--   0        0        0      318 2024-04-25 08:27:16.075068 ansible_doctor-4.0.5/ansibledoctor/templates/hugo-book/_tag.j2
+-rw-r--r--   0        0        0      371 2024-04-25 08:27:16.075068 ansible_doctor-4.0.5/ansibledoctor/templates/hugo-book/_toc.j2
+-rw-r--r--   0        0        0      583 2024-04-25 08:27:16.075068 ansible_doctor-4.0.5/ansibledoctor/templates/hugo-book/_todo.j2
+-rw-r--r--   0        0        0     1558 2024-04-25 08:27:16.075068 ansible_doctor-4.0.5/ansibledoctor/templates/hugo-book/_vars.j2
+-rw-r--r--   0        0        0      848 2024-04-25 08:27:16.075068 ansible_doctor-4.0.5/ansibledoctor/templates/hugo-book/index.md.j2
+-rw-r--r--   0        0        0      697 2024-04-25 08:27:16.075068 ansible_doctor-4.0.5/ansibledoctor/templates/readme/README.md.j2
+-rw-r--r--   0        0        0      691 2024-04-25 08:27:16.075068 ansible_doctor-4.0.5/ansibledoctor/templates/readme/_meta.j2
+-rw-r--r--   0        0        0      172 2024-04-25 08:27:16.075068 ansible_doctor-4.0.5/ansibledoctor/templates/readme/_requirements.j2
+-rw-r--r--   0        0        0      365 2024-04-25 08:27:16.075068 ansible_doctor-4.0.5/ansibledoctor/templates/readme/_tag.j2
+-rw-r--r--   0        0        0      434 2024-04-25 08:27:16.075068 ansible_doctor-4.0.5/ansibledoctor/templates/readme/_toc.j2
+-rw-r--r--   0        0        0      583 2024-04-25 08:27:16.075068 ansible_doctor-4.0.5/ansibledoctor/templates/readme/_todo.j2
+-rw-r--r--   0        0        0     1558 2024-04-25 08:27:16.075068 ansible_doctor-4.0.5/ansibledoctor/templates/readme/_vars.j2
+-rw-r--r--   0        0        0     9463 2024-04-25 08:27:16.075068 ansible_doctor-4.0.5/ansibledoctor/utils/__init__.py
+-rw-r--r--   0        0        0     2412 2024-04-25 08:27:16.075068 ansible_doctor-4.0.5/ansibledoctor/utils/yamlhelper.py
+-rw-r--r--   0        0        0     3174 2024-04-25 08:27:29.506962 ansible_doctor-4.0.5/pyproject.toml
+-rw-r--r--   0        0        0     4427 1970-01-01 00:00:00.000000 ansible_doctor-4.0.5/PKG-INFO
```

### Comparing `ansible_doctor-4.0.4/LICENSE` & `ansible_doctor-4.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ansible_doctor-4.0.4/README.md` & `ansible_doctor-4.0.5/README.md`

 * *Files identical despite different names*

### Comparing `ansible_doctor-4.0.4/ansibledoctor/annotation.py` & `ansible_doctor-4.0.5/ansibledoctor/annotation.py`

 * *Files identical despite different names*

### Comparing `ansible_doctor-4.0.4/ansibledoctor/cli.py` & `ansible_doctor-4.0.5/ansibledoctor/cli.py`

 * *Files identical despite different names*

### Comparing `ansible_doctor-4.0.4/ansibledoctor/config.py` & `ansible_doctor-4.0.5/ansibledoctor/config.py`

 * *Files identical despite different names*

### Comparing `ansible_doctor-4.0.4/ansibledoctor/doc_generator.py` & `ansible_doctor-4.0.5/ansibledoctor/doc_generator.py`

 * *Files identical despite different names*

### Comparing `ansible_doctor-4.0.4/ansibledoctor/doc_parser.py` & `ansible_doctor-4.0.5/ansibledoctor/doc_parser.py`

 * *Files identical despite different names*

### Comparing `ansible_doctor-4.0.4/ansibledoctor/exception.py` & `ansible_doctor-4.0.5/ansibledoctor/exception.py`

 * *Files identical despite different names*

### Comparing `ansible_doctor-4.0.4/ansibledoctor/file_registry.py` & `ansible_doctor-4.0.5/ansibledoctor/file_registry.py`

 * *Files identical despite different names*

### Comparing `ansible_doctor-4.0.4/ansibledoctor/templates/hugo-book/_todo.j2` & `ansible_doctor-4.0.5/ansibledoctor/templates/hugo-book/_todo.j2`

 * *Files identical despite different names*

### Comparing `ansible_doctor-4.0.4/ansibledoctor/templates/hugo-book/_vars.j2` & `ansible_doctor-4.0.5/ansibledoctor/templates/hugo-book/_vars.j2`

 * *Files identical despite different names*

### Comparing `ansible_doctor-4.0.4/ansibledoctor/templates/hugo-book/index.md.j2` & `ansible_doctor-4.0.5/ansibledoctor/templates/hugo-book/index.md.j2`

 * *Files identical despite different names*

### Comparing `ansible_doctor-4.0.4/ansibledoctor/templates/readme/README.md.j2` & `ansible_doctor-4.0.5/ansibledoctor/templates/readme/README.md.j2`

 * *Files identical despite different names*

### Comparing `ansible_doctor-4.0.4/ansibledoctor/templates/readme/_meta.j2` & `ansible_doctor-4.0.5/ansibledoctor/templates/readme/_meta.j2`

 * *Files identical despite different names*

### Comparing `ansible_doctor-4.0.4/ansibledoctor/templates/readme/_todo.j2` & `ansible_doctor-4.0.5/ansibledoctor/templates/readme/_todo.j2`

 * *Files identical despite different names*

### Comparing `ansible_doctor-4.0.4/ansibledoctor/templates/readme/_vars.j2` & `ansible_doctor-4.0.5/ansibledoctor/templates/readme/_vars.j2`

 * *Files identical despite different names*

### Comparing `ansible_doctor-4.0.4/ansibledoctor/utils/__init__.py` & `ansible_doctor-4.0.5/ansibledoctor/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ansible_doctor-4.0.4/ansibledoctor/utils/yamlhelper.py` & `ansible_doctor-4.0.5/ansibledoctor/utils/yamlhelper.py`

 * *Files identical despite different names*

### Comparing `ansible_doctor-4.0.4/pyproject.toml` & `ansible_doctor-4.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -24,37 +24,37 @@
 include = ["LICENSE"]
 keywords = ["ansible", "role", "documentation"]
 license = "GPL-3.0-only"
 name = "ansible-doctor"
 packages = [{ include = "ansibledoctor" }]
 readme = "README.md"
 repository = "https://github.com/thegeeklab/ansible-doctor/"
-version = "4.0.4"
+version = "4.0.5"
 
 [tool.poetry.dependencies]
 Jinja2 = "3.1.3"
 anyconfig = "0.14.0"
 appdirs = "1.4.4"
 colorama = "0.4.6"
 environs = "11.0.0"
 jsonschema = "4.21.1"
 pathspec = "0.12.1"
 python = "^3.9.0"
 python-json-logger = "2.0.7"
 "ruamel.yaml" = "0.18.6"
-ansible-core = { version = "2.14.15", optional = true }
+ansible-core = { version = "2.14.16", optional = true }
 
 [tool.poetry.extras]
 ansible-core = ["ansible-core"]
 
 [tool.poetry.scripts]
 ansible-doctor = "ansibledoctor.cli:main"
 
 [tool.poetry.group.dev.dependencies]
-ruff = "0.3.5"
+ruff = "0.4.1"
 pytest = "8.1.1"
 pytest-mock = "3.14.0"
 pytest-cov = "5.0.0"
 toml = "0.10.2"
 
 [tool.poetry-dynamic-versioning]
 enable = false
```

### Comparing `ansible_doctor-4.0.4/PKG-INFO` & `ansible_doctor-4.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansible-doctor
-Version: 4.0.4
+Version: 4.0.5
 Summary: Generate documentation from annotated Ansible roles using templates.
 Home-page: https://ansible-doctor.geekdocs.de/
 License: GPL-3.0-only
 Keywords: ansible,role,documentation
 Author: Robert Kaussow
 Author-email: mail@thegeeklab.de
 Requires-Python: >=3.9.0,<4.0.0
@@ -22,15 +22,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Documentation
 Classifier: Topic :: Utilities
 Provides-Extra: ansible-core
 Requires-Dist: Jinja2 (==3.1.3)
-Requires-Dist: ansible-core (==2.14.15) ; extra == "ansible-core"
+Requires-Dist: ansible-core (==2.14.16) ; extra == "ansible-core"
 Requires-Dist: anyconfig (==0.14.0)
 Requires-Dist: appdirs (==1.4.4)
 Requires-Dist: colorama (==0.4.6)
 Requires-Dist: environs (==11.0.0)
 Requires-Dist: jsonschema (==4.21.1)
 Requires-Dist: pathspec (==0.12.1)
 Requires-Dist: python-json-logger (==2.0.7)
```


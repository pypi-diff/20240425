# Comparing `tmp/mdformat_mkdocs-2.0.8.tar.gz` & `tmp/mdformat_mkdocs-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mdformat_mkdocs-2.0.8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "mdformat_mkdocs-2.0.9.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `mdformat_mkdocs-2.0.8.tar` & `mdformat_mkdocs-2.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0      600 2024-04-13 20:01:44.698604 mdformat_mkdocs-2.0.8/.copier-answers.yml
--rw-r--r--   0        0        0     1819 2024-04-13 20:01:44.698604 mdformat_mkdocs-2.0.8/.gitignore
--rw-r--r--   0        0        0     1592 2024-04-13 20:01:44.698604 mdformat_mkdocs-2.0.8/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1085 2024-04-13 20:01:44.698604 mdformat_mkdocs-2.0.8/.pre-commit-test.yaml
--rw-r--r--   0        0        0     2882 2024-04-13 20:01:44.698604 mdformat_mkdocs-2.0.8/.ruff.toml
--rw-r--r--   0        0        0       21 2024-04-13 20:01:44.698604 mdformat_mkdocs-2.0.8/.tool-versions
--rw-r--r--   0        0        0      276 2024-04-13 20:01:44.698604 mdformat_mkdocs-2.0.8/.yamllint.yaml
--rw-r--r--   0        0        0     1366 2024-04-13 20:01:44.698604 mdformat_mkdocs-2.0.8/CONTRIBUTING.md
--rw-r--r--   0        0        0     1073 2024-04-13 20:01:44.698604 mdformat_mkdocs-2.0.8/LICENSE
--rw-r--r--   0        0        0     4366 2024-04-13 20:01:44.698604 mdformat_mkdocs-2.0.8/README.md
--rw-r--r--   0        0        0      303 2024-04-13 20:01:44.698604 mdformat_mkdocs-2.0.8/mdformat_mkdocs/__init__.py
--rw-r--r--   0        0        0      914 2024-04-13 20:01:44.698604 mdformat_mkdocs-2.0.8/mdformat_mkdocs/_helpers.py
--rw-r--r--   0        0        0    11592 2024-04-13 20:01:44.698604 mdformat_mkdocs-2.0.8/mdformat_mkdocs/_normalize_list.py
--rw-r--r--   0        0        0     2416 2024-04-13 20:01:44.698604 mdformat_mkdocs-2.0.8/mdformat_mkdocs/_postprocess_inline.py
--rw-r--r--   0        0        0      317 2024-04-13 20:01:44.698604 mdformat_mkdocs-2.0.8/mdformat_mkdocs/mdit_plugins/__init__.py
--rw-r--r--   0        0        0     2368 2024-04-13 20:01:44.698604 mdformat_mkdocs-2.0.8/mdformat_mkdocs/mdit_plugins/_content_tabs.py
--rw-r--r--   0        0        0     2843 2024-04-13 20:01:44.702604 mdformat_mkdocs-2.0.8/mdformat_mkdocs/mdit_plugins/_mkdocs_admon.py
--rw-r--r--   0        0        0      785 2024-04-13 20:01:44.702604 mdformat_mkdocs-2.0.8/mdformat_mkdocs/mdit_plugins/_mkdocstrings_crossreference.py
--rw-r--r--   0        0        0     3966 2024-04-13 20:01:44.702604 mdformat_mkdocs-2.0.8/mdformat_mkdocs/plugin.py
--rw-r--r--   0        0        0     1698 2024-04-13 20:01:44.702604 mdformat_mkdocs-2.0.8/pyproject.toml
--rw-r--r--   0        0        0      895 2024-04-13 20:01:44.702604 mdformat_mkdocs-2.0.8/tox.ini
--rw-r--r--   0        0        0     6023 1970-01-01 00:00:00.000000 mdformat_mkdocs-2.0.8/PKG-INFO
+-rw-r--r--   0        0        0      600 2024-04-15 01:53:06.194283 mdformat_mkdocs-2.0.9/.copier-answers.yml
+-rw-r--r--   0        0        0     1819 2024-04-15 01:53:06.194283 mdformat_mkdocs-2.0.9/.gitignore
+-rw-r--r--   0        0        0     1592 2024-04-15 01:53:06.194283 mdformat_mkdocs-2.0.9/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1085 2024-04-15 01:53:06.194283 mdformat_mkdocs-2.0.9/.pre-commit-test.yaml
+-rw-r--r--   0        0        0     2882 2024-04-15 01:53:06.194283 mdformat_mkdocs-2.0.9/.ruff.toml
+-rw-r--r--   0        0        0       21 2024-04-15 01:53:06.194283 mdformat_mkdocs-2.0.9/.tool-versions
+-rw-r--r--   0        0        0      276 2024-04-15 01:53:06.194283 mdformat_mkdocs-2.0.9/.yamllint.yaml
+-rw-r--r--   0        0        0     1366 2024-04-15 01:53:06.194283 mdformat_mkdocs-2.0.9/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1073 2024-04-15 01:53:06.194283 mdformat_mkdocs-2.0.9/LICENSE
+-rw-r--r--   0        0        0     4366 2024-04-15 01:53:06.194283 mdformat_mkdocs-2.0.9/README.md
+-rw-r--r--   0        0        0      303 2024-04-15 01:53:06.194283 mdformat_mkdocs-2.0.9/mdformat_mkdocs/__init__.py
+-rw-r--r--   0        0        0      914 2024-04-15 01:53:06.194283 mdformat_mkdocs-2.0.9/mdformat_mkdocs/_helpers.py
+-rw-r--r--   0        0        0    11592 2024-04-15 01:53:06.194283 mdformat_mkdocs-2.0.9/mdformat_mkdocs/_normalize_list.py
+-rw-r--r--   0        0        0     2416 2024-04-15 01:53:06.194283 mdformat_mkdocs-2.0.9/mdformat_mkdocs/_postprocess_inline.py
+-rw-r--r--   0        0        0      317 2024-04-15 01:53:06.194283 mdformat_mkdocs-2.0.9/mdformat_mkdocs/mdit_plugins/__init__.py
+-rw-r--r--   0        0        0     2368 2024-04-15 01:53:06.194283 mdformat_mkdocs-2.0.9/mdformat_mkdocs/mdit_plugins/_content_tabs.py
+-rw-r--r--   0        0        0     2843 2024-04-15 01:53:06.194283 mdformat_mkdocs-2.0.9/mdformat_mkdocs/mdit_plugins/_mkdocs_admon.py
+-rw-r--r--   0        0        0      785 2024-04-15 01:53:06.194283 mdformat_mkdocs-2.0.9/mdformat_mkdocs/mdit_plugins/_mkdocstrings_crossreference.py
+-rw-r--r--   0        0        0     3966 2024-04-15 01:53:06.194283 mdformat_mkdocs-2.0.9/mdformat_mkdocs/plugin.py
+-rw-r--r--   0        0        0     1698 2024-04-15 01:53:06.194283 mdformat_mkdocs-2.0.9/pyproject.toml
+-rw-r--r--   0        0        0      895 2024-04-15 01:53:06.198283 mdformat_mkdocs-2.0.9/tox.ini
+-rw-r--r--   0        0        0     6023 1970-01-01 00:00:00.000000 mdformat_mkdocs-2.0.9/PKG-INFO
```

### Comparing `mdformat_mkdocs-2.0.8/.copier-answers.yml` & `mdformat_mkdocs-2.0.9/.copier-answers.yml`

 * *Files identical despite different names*

### Comparing `mdformat_mkdocs-2.0.8/.gitignore` & `mdformat_mkdocs-2.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `mdformat_mkdocs-2.0.8/.pre-commit-config.yaml` & `mdformat_mkdocs-2.0.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `mdformat_mkdocs-2.0.8/.pre-commit-test.yaml` & `mdformat_mkdocs-2.0.9/.pre-commit-test.yaml`

 * *Files identical despite different names*

### Comparing `mdformat_mkdocs-2.0.8/.ruff.toml` & `mdformat_mkdocs-2.0.9/.ruff.toml`

 * *Files identical despite different names*

### Comparing `mdformat_mkdocs-2.0.8/CONTRIBUTING.md` & `mdformat_mkdocs-2.0.9/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `mdformat_mkdocs-2.0.8/LICENSE` & `mdformat_mkdocs-2.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mdformat_mkdocs-2.0.8/README.md` & `mdformat_mkdocs-2.0.9/README.md`

 * *Files identical despite different names*

### Comparing `mdformat_mkdocs-2.0.8/mdformat_mkdocs/_helpers.py` & `mdformat_mkdocs-2.0.9/mdformat_mkdocs/_helpers.py`

 * *Files identical despite different names*

### Comparing `mdformat_mkdocs-2.0.8/mdformat_mkdocs/_normalize_list.py` & `mdformat_mkdocs-2.0.9/mdformat_mkdocs/_normalize_list.py`

 * *Files identical despite different names*

### Comparing `mdformat_mkdocs-2.0.8/mdformat_mkdocs/_postprocess_inline.py` & `mdformat_mkdocs-2.0.9/mdformat_mkdocs/_postprocess_inline.py`

 * *Files identical despite different names*

### Comparing `mdformat_mkdocs-2.0.8/mdformat_mkdocs/mdit_plugins/_content_tabs.py` & `mdformat_mkdocs-2.0.9/mdformat_mkdocs/mdit_plugins/_content_tabs.py`

 * *Files identical despite different names*

### Comparing `mdformat_mkdocs-2.0.8/mdformat_mkdocs/mdit_plugins/_mkdocs_admon.py` & `mdformat_mkdocs-2.0.9/mdformat_mkdocs/mdit_plugins/_mkdocs_admon.py`

 * *Files identical despite different names*

### Comparing `mdformat_mkdocs-2.0.8/mdformat_mkdocs/mdit_plugins/_mkdocstrings_crossreference.py` & `mdformat_mkdocs-2.0.9/mdformat_mkdocs/mdit_plugins/_mkdocstrings_crossreference.py`

 * *Files identical despite different names*

### Comparing `mdformat_mkdocs-2.0.8/mdformat_mkdocs/plugin.py` & `mdformat_mkdocs-2.0.9/mdformat_mkdocs/plugin.py`

 * *Files identical despite different names*

### Comparing `mdformat_mkdocs-2.0.8/pyproject.toml` & `mdformat_mkdocs-2.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
   "Intended Audience :: Developers",
   "License :: OSI Approved :: MIT License",
   "Programming Language :: Python :: 3",
   "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 dependencies = [
   "mdformat >= 0.7.16",
-  "mdformat-admon >= 2.0.2",
+  "mdformat-admon >= 2.0.3",
   "mdformat-gfm >= 0.3.6",
   "more-itertools >= 10.2.0",
 ]
 dynamic = ["description", "version"]
 keywords = ["markdown", "markdown-it", "mdformat"]
 name = "mdformat_mkdocs"
 readme = "README.md"
```

### Comparing `mdformat_mkdocs-2.0.8/tox.ini` & `mdformat_mkdocs-2.0.9/tox.ini`

 * *Files identical despite different names*

### Comparing `mdformat_mkdocs-2.0.8/PKG-INFO` & `mdformat_mkdocs-2.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: mdformat_mkdocs
-Version: 2.0.8
+Version: 2.0.9
 Summary: An mdformat plugin for mkdocs.
 Keywords: markdown,markdown-it,mdformat
 Author-email: kyleking <dev.act.kyle@gmail.com>
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: mdformat >= 0.7.16
-Requires-Dist: mdformat-admon >= 2.0.2
+Requires-Dist: mdformat-admon >= 2.0.3
 Requires-Dist: mdformat-gfm >= 0.3.6
 Requires-Dist: more-itertools >= 10.2.0
 Requires-Dist: pre-commit ; extra == "dev"
 Requires-Dist: mdformat-beautysh >= 0.1.1 ; extra == "recommended"
 Requires-Dist: mdformat-config >= 0.1.3 ; extra == "recommended"
 Requires-Dist: mdformat-footnote >= 0.1.1 ; extra == "recommended"
 Requires-Dist: mdformat-frontmatter >= 2.0.8 ; extra == "recommended"
```


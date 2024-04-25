# Comparing `tmp/skope_rules_temp-0.2.2.tar.gz` & `tmp/skope_rules_temp-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skope_rules_temp-0.2.2.tar", max compression
+gzip compressed data, was "skope_rules_temp-0.2.3.tar", max compression
```

## Comparing `skope_rules_temp-0.2.2.tar` & `skope_rules_temp-0.2.3.tar`

### file list

```diff
@@ -1,12 +1,14 @@
--rw-r--r--   0        0        0     5465 2024-02-22 09:40:20.708654 skope_rules_temp-0.2.2/README.md
--rw-r--r--   0        0        0      484 2024-02-22 16:33:46.377386 skope_rules_temp-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      115 2024-02-22 09:09:51.504475 skope_rules_temp-0.2.2/src/skope_rules_temp/__init__.py
--rw-r--r--   0        0        0       74 2024-02-22 09:09:51.504642 skope_rules_temp-0.2.2/src/skope_rules_temp/datasets/__init__.py
--rw-r--r--   0        0        0     1435 2024-02-22 09:09:51.504781 skope_rules_temp-0.2.2/src/skope_rules_temp/datasets/credit_data.py
--rw-r--r--   0        0        0     2352 2024-02-22 09:09:51.504892 skope_rules_temp-0.2.2/src/skope_rules_temp/rule.py
--rw-r--r--   0        0        0    27240 2024-02-22 09:09:51.505048 skope_rules_temp-0.2.2/src/skope_rules_temp/skope_rules.py
--rw-r--r--   0        0        0        0 2024-02-22 09:09:51.505177 skope_rules_temp-0.2.2/src/skope_rules_temp/tests/__init__.py
--rw-r--r--   0        0        0      277 2024-02-22 09:09:51.505310 skope_rules_temp-0.2.2/src/skope_rules_temp/tests/test_common.py
--rw-r--r--   0        0        0     1872 2024-02-22 09:09:51.505421 skope_rules_temp-0.2.2/src/skope_rules_temp/tests/test_rule.py
--rw-r--r--   0        0        0     8074 2024-02-22 09:09:51.505535 skope_rules_temp-0.2.2/src/skope_rules_temp/tests/test_skope_rules.py
--rw-r--r--   0        0        0     6167 1970-01-01 00:00:00.000000 skope_rules_temp-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0      428 2024-03-05 21:27:15.152010 skope_rules_temp-0.2.3/AUTHORS.rst
+-rw-r--r--   0        0        0     1551 2024-03-05 21:27:15.152121 skope_rules_temp-0.2.3/COPYING
+-rw-r--r--   0        0        0     5465 2024-03-05 21:27:15.152351 skope_rules_temp-0.2.3/README.md
+-rw-r--r--   0        0        0      485 2024-04-25 10:00:31.690113 skope_rules_temp-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0      115 2024-03-05 21:27:15.158029 skope_rules_temp-0.2.3/src/skope_rules_temp/__init__.py
+-rw-r--r--   0        0        0       74 2024-03-05 21:27:15.158175 skope_rules_temp-0.2.3/src/skope_rules_temp/datasets/__init__.py
+-rw-r--r--   0        0        0     1435 2024-03-05 21:27:15.158300 skope_rules_temp-0.2.3/src/skope_rules_temp/datasets/credit_data.py
+-rw-r--r--   0        0        0     2352 2024-03-05 21:27:15.158409 skope_rules_temp-0.2.3/src/skope_rules_temp/rule.py
+-rw-r--r--   0        0        0    27240 2024-03-05 21:27:15.158638 skope_rules_temp-0.2.3/src/skope_rules_temp/skope_rules.py
+-rw-r--r--   0        0        0        0 2024-03-05 21:27:15.158776 skope_rules_temp-0.2.3/src/skope_rules_temp/tests/__init__.py
+-rw-r--r--   0        0        0      277 2024-03-05 21:27:15.158910 skope_rules_temp-0.2.3/src/skope_rules_temp/tests/test_common.py
+-rw-r--r--   0        0        0     1872 2024-03-05 21:27:15.159076 skope_rules_temp-0.2.3/src/skope_rules_temp/tests/test_rule.py
+-rw-r--r--   0        0        0     8074 2024-03-05 21:27:15.159227 skope_rules_temp-0.2.3/src/skope_rules_temp/tests/test_skope_rules.py
+-rw-r--r--   0        0        0     6213 1970-01-01 00:00:00.000000 skope_rules_temp-0.2.3/PKG-INFO
```

### Comparing `skope_rules_temp-0.2.2/README.md` & `skope_rules_temp-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `skope_rules_temp-0.2.2/src/skope_rules_temp/datasets/credit_data.py` & `skope_rules_temp-0.2.3/src/skope_rules_temp/datasets/credit_data.py`

 * *Files identical despite different names*

### Comparing `skope_rules_temp-0.2.2/src/skope_rules_temp/rule.py` & `skope_rules_temp-0.2.3/src/skope_rules_temp/rule.py`

 * *Files identical despite different names*

### Comparing `skope_rules_temp-0.2.2/src/skope_rules_temp/skope_rules.py` & `skope_rules_temp-0.2.3/src/skope_rules_temp/skope_rules.py`

 * *Files identical despite different names*

### Comparing `skope_rules_temp-0.2.2/src/skope_rules_temp/tests/test_rule.py` & `skope_rules_temp-0.2.3/src/skope_rules_temp/tests/test_rule.py`

 * *Files identical despite different names*

### Comparing `skope_rules_temp-0.2.2/src/skope_rules_temp/tests/test_skope_rules.py` & `skope_rules_temp-0.2.3/src/skope_rules_temp/tests/test_skope_rules.py`

 * *Files identical despite different names*

### Comparing `skope_rules_temp-0.2.2/PKG-INFO` & `skope_rules_temp-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: skope-rules-temp
-Version: 0.2.2
+Version: 0.2.3
 Summary: Fork of https://github.com/scikit-learn-contrib/skope-rules
 Author: Pierre Hulot
 Author-email: pierre@ai-vidence.com
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.10
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: numpy (>=1.26.4,<2.0.0)
 Requires-Dist: numpydoc (>=1.6.0,<2.0.0)
 Requires-Dist: pandas (>=2.2.0,<3.0.0)
 Requires-Dist: scikit-learn (>=1.4.1.post1,<2.0.0)
 Requires-Dist: scipy (>=1.12.0,<2.0.0)
```


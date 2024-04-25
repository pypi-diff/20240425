# Comparing `tmp/costyl-0.2.1.tar.gz` & `tmp/costyl-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "costyl-0.2.1.tar", max compression
+gzip compressed data, was "costyl-0.2.2.tar", max compression
```

## Comparing `costyl-0.2.1.tar` & `costyl-0.2.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      343 2024-03-27 04:11:24.898387 costyl-0.2.1/README.md
--rw-r--r--   0        0        0     2408 2024-03-27 19:42:10.196872 costyl-0.2.1/costyl/__init__.py
--rw-r--r--   0        0        0      470 2024-03-27 19:01:13.391799 costyl-0.2.1/costyl/analysers/__init__.py
--rw-r--r--   0        0        0     2244 2024-03-27 03:13:48.990248 costyl-0.2.1/costyl/analysers/layout.py
--rw-r--r--   0        0        0     4204 2024-03-27 18:50:27.672220 costyl-0.2.1/costyl/analysers/lexical.py
--rw-r--r--   0        0        0     1597 2024-03-27 18:59:11.454266 costyl-0.2.1/costyl/tools.py
--rw-r--r--   0        0        0      733 2024-03-27 03:22:31.868906 costyl-0.2.1/costyl/vectorizer/__init__.py
--rw-r--r--   0        0        0      420 2024-03-27 03:22:11.171965 costyl-0.2.1/costyl/vectorizer/__vectorizer.py
--rw-r--r--   0        0        0      421 2024-03-27 19:44:57.407723 costyl-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      950 1970-01-01 00:00:00.000000 costyl-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      343 2024-03-27 04:11:24.898387 costyl-0.2.2/README.md
+-rw-r--r--   0        0        0     2408 2024-03-27 19:42:10.196872 costyl-0.2.2/costyl/__init__.py
+-rw-r--r--   0        0        0      470 2024-03-27 19:01:13.391799 costyl-0.2.2/costyl/analysers/__init__.py
+-rw-r--r--   0        0        0     2244 2024-03-27 03:13:48.990248 costyl-0.2.2/costyl/analysers/layout.py
+-rw-r--r--   0        0        0     4324 2024-04-25 18:54:57.968152 costyl-0.2.2/costyl/analysers/lexical.py
+-rw-r--r--   0        0        0     1597 2024-03-27 18:59:11.454266 costyl-0.2.2/costyl/tools.py
+-rw-r--r--   0        0        0      733 2024-03-27 03:22:31.868906 costyl-0.2.2/costyl/vectorizer/__init__.py
+-rw-r--r--   0        0        0      420 2024-03-27 03:22:11.171965 costyl-0.2.2/costyl/vectorizer/__vectorizer.py
+-rw-r--r--   0        0        0      421 2024-04-25 19:33:25.735320 costyl-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      950 1970-01-01 00:00:00.000000 costyl-0.2.2/PKG-INFO
```

### Comparing `costyl-0.2.1/costyl/__init__.py` & `costyl-0.2.2/costyl/__init__.py`

 * *Files identical despite different names*

### Comparing `costyl-0.2.1/costyl/analysers/layout.py` & `costyl-0.2.2/costyl/analysers/layout.py`

 * *Files identical despite different names*

### Comparing `costyl-0.2.1/costyl/analysers/lexical.py` & `costyl-0.2.2/costyl/analysers/lexical.py`

 * *Files 4% similar despite different names*

```diff
@@ -191,12 +191,17 @@
         operatorLabelsCountDict = dict(zip(operatorLabels, operatorCount[i]))
         operatorLabelsCountDict = cleanLabelsCountDict(operatorLabelsCountDict)
         operatorCountSum = sum(list(operatorLabelsCountDict.values()))
 
         # Not at its most efficient state. Detects strings in commented lines
         stringLiteralCountSum = len(re.findall('(?:"(?:\\\\.|[^"\\\\])*"|\'(?:\\\\.|[^\'\\\\])*\')', files[i]))
 
-        feats[i, 0] = math.log(keywordCountSum/len(files[i]))
-        feats[i, 1] = math.log(operatorCountSum/len(files[i]))
-        feats[i, 2] = math.log(stringLiteralCountSum/len(files[i]))
+        if keywordCountSum != 0:
+            feats[i, 0] = math.log(keywordCountSum/len(files[i]))
+
+        if operatorCountSum != 0:
+            feats[i, 1] = math.log(operatorCountSum/len(files[i]))
+
+        if stringLiteralCountSum != 0:
+            feats[i, 2] = math.log(stringLiteralCountSum/len(files[i]))
 
     return feats
```

### Comparing `costyl-0.2.1/costyl/tools.py` & `costyl-0.2.2/costyl/tools.py`

 * *Files identical despite different names*

### Comparing `costyl-0.2.1/costyl/vectorizer/__init__.py` & `costyl-0.2.2/costyl/vectorizer/__init__.py`

 * *Files identical despite different names*

### Comparing `costyl-0.2.1/PKG-INFO` & `costyl-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: costyl
-Version: 0.2.1
+Version: 0.2.2
 Summary: Costyl is a python library to facilitate source code authorship attribution via stylometric analysis powered by machine learning.
 Author: Jbernardiss
 Author-email: joaobernardiss@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```


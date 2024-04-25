# Comparing `tmp/metamath-py-0.0.3.tar.gz` & `tmp/metamath_py-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metamath-py-0.0.3.tar", last modified: Tue Mar 26 01:06:36 2024, max compression
+gzip compressed data, was "metamath_py-0.0.4.tar", last modified: Thu Apr 25 03:12:17 2024, max compression
```

## Comparing `metamath-py-0.0.3.tar` & `metamath_py-0.0.4.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxrwxr-x   0 lightop   (1000) lightop   (1000)        0 2024-03-26 01:06:36.386936 metamath-py-0.0.3/
--rw-rw-r--   0 lightop   (1000) lightop   (1000)     1088 2023-09-27 00:57:53.000000 metamath-py-0.0.3/LICENSE
--rw-rw-r--   0 lightop   (1000) lightop   (1000)     3210 2024-03-26 01:06:36.386936 metamath-py-0.0.3/PKG-INFO
--rw-rw-r--   0 lightop   (1000) lightop   (1000)     2698 2024-01-31 23:13:41.000000 metamath-py-0.0.3/README.md
--rw-rw-r--   0 lightop   (1000) lightop   (1000)      585 2024-03-26 01:06:16.000000 metamath-py-0.0.3/pyproject.toml
--rw-rw-r--   0 lightop   (1000) lightop   (1000)       38 2024-03-26 01:06:36.386936 metamath-py-0.0.3/setup.cfg
-drwxrwxr-x   0 lightop   (1000) lightop   (1000)        0 2024-03-26 01:06:36.382936 metamath-py-0.0.3/src/
-drwxrwxr-x   0 lightop   (1000) lightop   (1000)        0 2024-03-26 01:06:36.382936 metamath-py-0.0.3/src/metamath_py.egg-info/
--rw-rw-r--   0 lightop   (1000) lightop   (1000)     3210 2024-03-26 01:06:36.000000 metamath-py-0.0.3/src/metamath_py.egg-info/PKG-INFO
--rw-rw-r--   0 lightop   (1000) lightop   (1000)      444 2024-03-26 01:06:36.000000 metamath-py-0.0.3/src/metamath_py.egg-info/SOURCES.txt
--rw-rw-r--   0 lightop   (1000) lightop   (1000)        1 2024-03-26 01:06:36.000000 metamath-py-0.0.3/src/metamath_py.egg-info/dependency_links.txt
--rw-rw-r--   0 lightop   (1000) lightop   (1000)       11 2024-03-26 01:06:36.000000 metamath-py-0.0.3/src/metamath_py.egg-info/top_level.txt
-drwxrwxr-x   0 lightop   (1000) lightop   (1000)        0 2024-03-26 01:06:36.386936 metamath-py-0.0.3/src/metamathpy/
--rw-rw-r--   0 lightop   (1000) lightop   (1000)        1 2024-01-31 23:13:41.000000 metamath-py-0.0.3/src/metamathpy/__init__.py
--rw-rw-r--   0 lightop   (1000) lightop   (1000)     6844 2024-03-24 20:58:34.000000 metamath-py-0.0.3/src/metamathpy/database.py
--rw-rw-r--   0 lightop   (1000) lightop   (1000)     2521 2024-01-31 23:13:41.000000 metamath-py-0.0.3/src/metamathpy/obvious.py
--rw-rw-r--   0 lightop   (1000) lightop   (1000)     7411 2024-01-31 23:13:41.000000 metamath-py-0.0.3/src/metamathpy/parse.py
--rw-rw-r--   0 lightop   (1000) lightop   (1000)    12437 2024-03-23 12:20:50.000000 metamath-py-0.0.3/src/metamathpy/proof.py
--rw-rw-r--   0 lightop   (1000) lightop   (1000)     1012 2024-01-31 23:13:41.000000 metamath-py-0.0.3/src/metamathpy/scratch.py
--rw-rw-r--   0 lightop   (1000) lightop   (1000)     6352 2024-01-31 23:13:41.000000 metamath-py-0.0.3/src/metamathpy/theory.py
--rw-rw-r--   0 lightop   (1000) lightop   (1000)      911 2024-01-31 23:24:22.000000 metamath-py-0.0.3/src/metamathpy/training_data.py
--rw-rw-r--   0 lightop   (1000) lightop   (1000)     1513 2024-03-23 12:20:50.000000 metamath-py-0.0.3/src/metamathpy/unification.py
-drwxrwxr-x   0 lightop   (1000) lightop   (1000)        0 2024-03-26 01:06:36.386936 metamath-py-0.0.3/tests/
--rw-rw-r--   0 lightop   (1000) lightop   (1000)     3097 2023-09-27 01:27:35.000000 metamath-py-0.0.3/tests/tests.py
+drwxrwxr-x   0 lightop   (1000) lightop   (1000)        0 2024-04-25 03:12:17.783798 metamath_py-0.0.4/
+-rw-rw-r--   0 lightop   (1000) lightop   (1000)     1088 2023-09-27 00:57:53.000000 metamath_py-0.0.4/LICENSE
+-rw-r--r--   0 lightop   (1000) lightop   (1000)     3309 2024-04-25 03:12:17.783798 metamath_py-0.0.4/PKG-INFO
+-rw-rw-r--   0 lightop   (1000) lightop   (1000)     2797 2024-03-26 01:28:31.000000 metamath_py-0.0.4/README.md
+-rw-rw-r--   0 lightop   (1000) lightop   (1000)      585 2024-04-25 03:09:33.000000 metamath_py-0.0.4/pyproject.toml
+-rw-rw-r--   0 lightop   (1000) lightop   (1000)       38 2024-04-25 03:12:17.783798 metamath_py-0.0.4/setup.cfg
+drwxrwxr-x   0 lightop   (1000) lightop   (1000)        0 2024-04-25 03:12:17.775798 metamath_py-0.0.4/src/
+drwxrwxr-x   0 lightop   (1000) lightop   (1000)        0 2024-04-25 03:12:17.783798 metamath_py-0.0.4/src/metamath_py.egg-info/
+-rw-r--r--   0 lightop   (1000) lightop   (1000)     3309 2024-04-25 03:12:17.000000 metamath_py-0.0.4/src/metamath_py.egg-info/PKG-INFO
+-rw-rw-r--   0 lightop   (1000) lightop   (1000)      474 2024-04-25 03:12:17.000000 metamath_py-0.0.4/src/metamath_py.egg-info/SOURCES.txt
+-rw-rw-r--   0 lightop   (1000) lightop   (1000)        1 2024-04-25 03:12:17.000000 metamath_py-0.0.4/src/metamath_py.egg-info/dependency_links.txt
+-rw-rw-r--   0 lightop   (1000) lightop   (1000)       11 2024-04-25 03:12:17.000000 metamath_py-0.0.4/src/metamath_py.egg-info/top_level.txt
+drwxrwxr-x   0 lightop   (1000) lightop   (1000)        0 2024-04-25 03:12:17.783798 metamath_py-0.0.4/src/metamathpy/
+-rw-rw-r--   0 lightop   (1000) lightop   (1000)        1 2024-01-31 23:13:41.000000 metamath_py-0.0.4/src/metamathpy/__init__.py
+-rw-rw-r--   0 lightop   (1000) lightop   (1000)     6844 2024-03-24 20:58:34.000000 metamath_py-0.0.4/src/metamathpy/database.py
+-rw-rw-r--   0 lightop   (1000) lightop   (1000)     2682 2024-04-25 03:07:24.000000 metamath_py-0.0.4/src/metamathpy/environment.py
+-rw-rw-r--   0 lightop   (1000) lightop   (1000)     2521 2024-01-31 23:13:41.000000 metamath_py-0.0.4/src/metamathpy/obvious.py
+-rw-rw-r--   0 lightop   (1000) lightop   (1000)     7411 2024-01-31 23:13:41.000000 metamath_py-0.0.4/src/metamathpy/parse.py
+-rw-rw-r--   0 lightop   (1000) lightop   (1000)    12437 2024-03-23 12:20:50.000000 metamath_py-0.0.4/src/metamathpy/proof.py
+-rw-rw-r--   0 lightop   (1000) lightop   (1000)     1012 2024-01-31 23:13:41.000000 metamath_py-0.0.4/src/metamathpy/scratch.py
+-rw-rw-r--   0 lightop   (1000) lightop   (1000)     6352 2024-01-31 23:13:41.000000 metamath_py-0.0.4/src/metamathpy/theory.py
+-rw-rw-r--   0 lightop   (1000) lightop   (1000)      911 2024-01-31 23:24:22.000000 metamath_py-0.0.4/src/metamathpy/training_data.py
+-rw-rw-r--   0 lightop   (1000) lightop   (1000)     1513 2024-03-23 12:20:50.000000 metamath_py-0.0.4/src/metamathpy/unification.py
+drwxrwxr-x   0 lightop   (1000) lightop   (1000)        0 2024-04-25 03:12:17.783798 metamath_py-0.0.4/tests/
+-rw-rw-r--   0 lightop   (1000) lightop   (1000)     3097 2023-09-27 01:27:35.000000 metamath_py-0.0.4/tests/tests.py
```

### Comparing `metamath-py-0.0.3/LICENSE` & `metamath_py-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `metamath-py-0.0.3/PKG-INFO` & `metamath_py-0.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metamath-py
-Version: 0.0.3
+Version: 0.0.4
 Summary: A Python interface to Metamath
 Author-email: "Garrett E. Katz" <garrett.katz@gmail.com>
 Project-URL: Homepage, https://github.com/garrettkatz/mmpy
 Project-URL: Bug Tracker, https://github.com/garrettkatz/mmpy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -21,17 +21,17 @@
 `$ pip install --user metamath-py`
 
 # basic usage
 
 Loading a .mm file (may take a minute for large databases):
 
 ```
->>> import metamathpy as mm
+>>> import metamathpy.database as md
 >>> import os
->>> db = mm.database.parse(os.path.join(os.environ["HOME"], "metamath", "set.mm"))
+>>> db = md.parse(os.path.join(os.environ["HOME"], "metamath", "set.mm"))
 ```
 
 Access any statement by its label, for example the major premise of the modus ponens axiom:
 
 ```
 >>> db.statements['maj'] # uses a named tuple data structure
 Statement(label='maj', tag='$e', tokens=['|-', '(', 'ph', '->', 'ps', ')'], proof=[])
@@ -40,15 +40,15 @@
 ```
 
 Access any inference rule by the label of its consequent:
 
 ```
 >>> db.rules['ax-mp']
 <metamathpy.database.Rule object at 0x7fe21f099370>
->>> db.rules['ax-mp'].print() # pretty-print it
+>>> print(db.rules['ax-mp']) # more human readable
 ax-mp $a |- ps $.
 disjoint variable sets: set()
   wph $f wff ph $.
   wps $f wff ps $.
   min $e |- ph $.
   maj $e |- ( ph -> ps ) $.
 ```
@@ -79,13 +79,13 @@
 >>> root.rule # the rule used to justify this step
 <metamathpy.database.Rule object at 0x7fe21f099370>
 >>> root.rule.consequent # in this case it is ax-mp
 Statement(label='ax-mp', tag='$a', tokens=['|-', 'ps'], proof=[])
 >>> root.substitution # the variable substitution that unified ax-mp with this step
 {'ph': ('ph',), 'ps': ('(', 'ps', '->', 'ph', ')')}
 >>> root.dependencies # the other steps on which this one was justified
-{'wph': wph wff ph, 'wps': wi wff ( ps -> ph ), 'min': a1i.1 |- ph, 'maj': ax-1 |- ( ph -> ( ps -> ph ) )}
+{'wph': ProofStep(conclusion=[wph] wff ph), 'wps': ProofStep(conclusion=[wi] wff ( ps -> ph )), 'min': ProofStep(conclusion=[a1i.1] |- ph), 'maj': ProofStep(conclusion=[ax-1] |- ( ph -> ( ps -> ph ) ))}
 ```
 
 The dependencies are a dictionary where keys are the labels of the rule's hypotheses, and values are the other proof steps that satisfied those hypotheses.  These can be thought of as the children of the root in the proof tree.
```

### Comparing `metamath-py-0.0.3/README.md` & `metamath_py-0.0.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 `$ pip install --user metamath-py`
 
 # basic usage
 
 Loading a .mm file (may take a minute for large databases):
 
 ```
->>> import metamathpy as mm
+>>> import metamathpy.database as md
 >>> import os
->>> db = mm.database.parse(os.path.join(os.environ["HOME"], "metamath", "set.mm"))
+>>> db = md.parse(os.path.join(os.environ["HOME"], "metamath", "set.mm"))
 ```
 
 Access any statement by its label, for example the major premise of the modus ponens axiom:
 
 ```
 >>> db.statements['maj'] # uses a named tuple data structure
 Statement(label='maj', tag='$e', tokens=['|-', '(', 'ph', '->', 'ps', ')'], proof=[])
@@ -26,15 +26,15 @@
 ```
 
 Access any inference rule by the label of its consequent:
 
 ```
 >>> db.rules['ax-mp']
 <metamathpy.database.Rule object at 0x7fe21f099370>
->>> db.rules['ax-mp'].print() # pretty-print it
+>>> print(db.rules['ax-mp']) # more human readable
 ax-mp $a |- ps $.
 disjoint variable sets: set()
   wph $f wff ph $.
   wps $f wff ps $.
   min $e |- ph $.
   maj $e |- ( ph -> ps ) $.
 ```
@@ -65,13 +65,13 @@
 >>> root.rule # the rule used to justify this step
 <metamathpy.database.Rule object at 0x7fe21f099370>
 >>> root.rule.consequent # in this case it is ax-mp
 Statement(label='ax-mp', tag='$a', tokens=['|-', 'ps'], proof=[])
 >>> root.substitution # the variable substitution that unified ax-mp with this step
 {'ph': ('ph',), 'ps': ('(', 'ps', '->', 'ph', ')')}
 >>> root.dependencies # the other steps on which this one was justified
-{'wph': wph wff ph, 'wps': wi wff ( ps -> ph ), 'min': a1i.1 |- ph, 'maj': ax-1 |- ( ph -> ( ps -> ph ) )}
+{'wph': ProofStep(conclusion=[wph] wff ph), 'wps': ProofStep(conclusion=[wi] wff ( ps -> ph )), 'min': ProofStep(conclusion=[a1i.1] |- ph), 'maj': ProofStep(conclusion=[ax-1] |- ( ph -> ( ps -> ph ) ))}
 ```
 
 The dependencies are a dictionary where keys are the labels of the rule's hypotheses, and values are the other proof steps that satisfied those hypotheses.  These can be thought of as the children of the root in the proof tree.
```

### Comparing `metamath-py-0.0.3/pyproject.toml` & `metamath_py-0.0.4/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "metamath-py"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Garrett E. Katz", email="garrett.katz@gmail.com" },
 ]
 description = "A Python interface to Metamath"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `metamath-py-0.0.3/src/metamath_py.egg-info/PKG-INFO` & `metamath_py-0.0.4/src/metamath_py.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metamath-py
-Version: 0.0.3
+Version: 0.0.4
 Summary: A Python interface to Metamath
 Author-email: "Garrett E. Katz" <garrett.katz@gmail.com>
 Project-URL: Homepage, https://github.com/garrettkatz/mmpy
 Project-URL: Bug Tracker, https://github.com/garrettkatz/mmpy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -21,17 +21,17 @@
 `$ pip install --user metamath-py`
 
 # basic usage
 
 Loading a .mm file (may take a minute for large databases):
 
 ```
->>> import metamathpy as mm
+>>> import metamathpy.database as md
 >>> import os
->>> db = mm.database.parse(os.path.join(os.environ["HOME"], "metamath", "set.mm"))
+>>> db = md.parse(os.path.join(os.environ["HOME"], "metamath", "set.mm"))
 ```
 
 Access any statement by its label, for example the major premise of the modus ponens axiom:
 
 ```
 >>> db.statements['maj'] # uses a named tuple data structure
 Statement(label='maj', tag='$e', tokens=['|-', '(', 'ph', '->', 'ps', ')'], proof=[])
@@ -40,15 +40,15 @@
 ```
 
 Access any inference rule by the label of its consequent:
 
 ```
 >>> db.rules['ax-mp']
 <metamathpy.database.Rule object at 0x7fe21f099370>
->>> db.rules['ax-mp'].print() # pretty-print it
+>>> print(db.rules['ax-mp']) # more human readable
 ax-mp $a |- ps $.
 disjoint variable sets: set()
   wph $f wff ph $.
   wps $f wff ps $.
   min $e |- ph $.
   maj $e |- ( ph -> ps ) $.
 ```
@@ -79,13 +79,13 @@
 >>> root.rule # the rule used to justify this step
 <metamathpy.database.Rule object at 0x7fe21f099370>
 >>> root.rule.consequent # in this case it is ax-mp
 Statement(label='ax-mp', tag='$a', tokens=['|-', 'ps'], proof=[])
 >>> root.substitution # the variable substitution that unified ax-mp with this step
 {'ph': ('ph',), 'ps': ('(', 'ps', '->', 'ph', ')')}
 >>> root.dependencies # the other steps on which this one was justified
-{'wph': wph wff ph, 'wps': wi wff ( ps -> ph ), 'min': a1i.1 |- ph, 'maj': ax-1 |- ( ph -> ( ps -> ph ) )}
+{'wph': ProofStep(conclusion=[wph] wff ph), 'wps': ProofStep(conclusion=[wi] wff ( ps -> ph )), 'min': ProofStep(conclusion=[a1i.1] |- ph), 'maj': ProofStep(conclusion=[ax-1] |- ( ph -> ( ps -> ph ) ))}
 ```
 
 The dependencies are a dictionary where keys are the labels of the rule's hypotheses, and values are the other proof steps that satisfied those hypotheses.  These can be thought of as the children of the root in the proof tree.
```

### Comparing `metamath-py-0.0.3/src/metamathpy/database.py` & `metamath_py-0.0.4/src/metamathpy/database.py`

 * *Files identical despite different names*

### Comparing `metamath-py-0.0.3/src/metamathpy/obvious.py` & `metamath_py-0.0.4/src/metamathpy/obvious.py`

 * *Files identical despite different names*

### Comparing `metamath-py-0.0.3/src/metamathpy/parse.py` & `metamath_py-0.0.4/src/metamathpy/parse.py`

 * *Files identical despite different names*

### Comparing `metamath-py-0.0.3/src/metamathpy/proof.py` & `metamath_py-0.0.4/src/metamathpy/proof.py`

 * *Files identical despite different names*

### Comparing `metamath-py-0.0.3/src/metamathpy/scratch.py` & `metamath_py-0.0.4/src/metamathpy/scratch.py`

 * *Files identical despite different names*

### Comparing `metamath-py-0.0.3/src/metamathpy/theory.py` & `metamath_py-0.0.4/src/metamathpy/theory.py`

 * *Files identical despite different names*

### Comparing `metamath-py-0.0.3/src/metamathpy/training_data.py` & `metamath_py-0.0.4/src/metamathpy/training_data.py`

 * *Files identical despite different names*

### Comparing `metamath-py-0.0.3/src/metamathpy/unification.py` & `metamath_py-0.0.4/src/metamathpy/unification.py`

 * *Files identical despite different names*

### Comparing `metamath-py-0.0.3/tests/tests.py` & `metamath_py-0.0.4/tests/tests.py`

 * *Files identical despite different names*


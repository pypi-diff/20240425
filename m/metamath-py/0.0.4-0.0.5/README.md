# Comparing `tmp/metamath_py-0.0.4.tar.gz` & `tmp/metamath_py-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metamath_py-0.0.4.tar", last modified: Thu Apr 25 03:12:17 2024, max compression
+gzip compressed data, was "metamath_py-0.0.5.tar", last modified: Thu Apr 25 03:47:16 2024, max compression
```

## Comparing `metamath_py-0.0.4.tar` & `metamath_py-0.0.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 lightop   (1000) lightop   (1000)        0 2024-04-25 03:12:17.783798 metamath_py-0.0.4/
--rw-rw-r--   0 lightop   (1000) lightop   (1000)     1088 2023-09-27 00:57:53.000000 metamath_py-0.0.4/LICENSE
--rw-r--r--   0 lightop   (1000) lightop   (1000)     3309 2024-04-25 03:12:17.783798 metamath_py-0.0.4/PKG-INFO
--rw-rw-r--   0 lightop   (1000) lightop   (1000)     2797 2024-03-26 01:28:31.000000 metamath_py-0.0.4/README.md
--rw-rw-r--   0 lightop   (1000) lightop   (1000)      585 2024-04-25 03:09:33.000000 metamath_py-0.0.4/pyproject.toml
--rw-rw-r--   0 lightop   (1000) lightop   (1000)       38 2024-04-25 03:12:17.783798 metamath_py-0.0.4/setup.cfg
-drwxrwxr-x   0 lightop   (1000) lightop   (1000)        0 2024-04-25 03:12:17.775798 metamath_py-0.0.4/src/
-drwxrwxr-x   0 lightop   (1000) lightop   (1000)        0 2024-04-25 03:12:17.783798 metamath_py-0.0.4/src/metamath_py.egg-info/
--rw-r--r--   0 lightop   (1000) lightop   (1000)     3309 2024-04-25 03:12:17.000000 metamath_py-0.0.4/src/metamath_py.egg-info/PKG-INFO
--rw-rw-r--   0 lightop   (1000) lightop   (1000)      474 2024-04-25 03:12:17.000000 metamath_py-0.0.4/src/metamath_py.egg-info/SOURCES.txt
--rw-rw-r--   0 lightop   (1000) lightop   (1000)        1 2024-04-25 03:12:17.000000 metamath_py-0.0.4/src/metamath_py.egg-info/dependency_links.txt
--rw-rw-r--   0 lightop   (1000) lightop   (1000)       11 2024-04-25 03:12:17.000000 metamath_py-0.0.4/src/metamath_py.egg-info/top_level.txt
-drwxrwxr-x   0 lightop   (1000) lightop   (1000)        0 2024-04-25 03:12:17.783798 metamath_py-0.0.4/src/metamathpy/
--rw-rw-r--   0 lightop   (1000) lightop   (1000)        1 2024-01-31 23:13:41.000000 metamath_py-0.0.4/src/metamathpy/__init__.py
--rw-rw-r--   0 lightop   (1000) lightop   (1000)     6844 2024-03-24 20:58:34.000000 metamath_py-0.0.4/src/metamathpy/database.py
--rw-rw-r--   0 lightop   (1000) lightop   (1000)     2682 2024-04-25 03:07:24.000000 metamath_py-0.0.4/src/metamathpy/environment.py
--rw-rw-r--   0 lightop   (1000) lightop   (1000)     2521 2024-01-31 23:13:41.000000 metamath_py-0.0.4/src/metamathpy/obvious.py
--rw-rw-r--   0 lightop   (1000) lightop   (1000)     7411 2024-01-31 23:13:41.000000 metamath_py-0.0.4/src/metamathpy/parse.py
--rw-rw-r--   0 lightop   (1000) lightop   (1000)    12437 2024-03-23 12:20:50.000000 metamath_py-0.0.4/src/metamathpy/proof.py
--rw-rw-r--   0 lightop   (1000) lightop   (1000)     1012 2024-01-31 23:13:41.000000 metamath_py-0.0.4/src/metamathpy/scratch.py
--rw-rw-r--   0 lightop   (1000) lightop   (1000)     6352 2024-01-31 23:13:41.000000 metamath_py-0.0.4/src/metamathpy/theory.py
--rw-rw-r--   0 lightop   (1000) lightop   (1000)      911 2024-01-31 23:24:22.000000 metamath_py-0.0.4/src/metamathpy/training_data.py
--rw-rw-r--   0 lightop   (1000) lightop   (1000)     1513 2024-03-23 12:20:50.000000 metamath_py-0.0.4/src/metamathpy/unification.py
-drwxrwxr-x   0 lightop   (1000) lightop   (1000)        0 2024-04-25 03:12:17.783798 metamath_py-0.0.4/tests/
--rw-rw-r--   0 lightop   (1000) lightop   (1000)     3097 2023-09-27 01:27:35.000000 metamath_py-0.0.4/tests/tests.py
+drwxrwxr-x   0 lightop   (1000) lightop   (1000)        0 2024-04-25 03:47:16.063389 metamath_py-0.0.5/
+-rw-rw-r--   0 lightop   (1000) lightop   (1000)     1088 2023-09-27 00:57:53.000000 metamath_py-0.0.5/LICENSE
+-rw-r--r--   0 lightop   (1000) lightop   (1000)     5145 2024-04-25 03:47:16.063389 metamath_py-0.0.5/PKG-INFO
+-rw-rw-r--   0 lightop   (1000) lightop   (1000)     4633 2024-04-25 03:46:23.000000 metamath_py-0.0.5/README.md
+-rw-rw-r--   0 lightop   (1000) lightop   (1000)      585 2024-04-25 03:47:03.000000 metamath_py-0.0.5/pyproject.toml
+-rw-rw-r--   0 lightop   (1000) lightop   (1000)       38 2024-04-25 03:47:16.063389 metamath_py-0.0.5/setup.cfg
+drwxrwxr-x   0 lightop   (1000) lightop   (1000)        0 2024-04-25 03:47:16.059389 metamath_py-0.0.5/src/
+drwxrwxr-x   0 lightop   (1000) lightop   (1000)        0 2024-04-25 03:47:16.063389 metamath_py-0.0.5/src/metamath_py.egg-info/
+-rw-r--r--   0 lightop   (1000) lightop   (1000)     5145 2024-04-25 03:47:16.000000 metamath_py-0.0.5/src/metamath_py.egg-info/PKG-INFO
+-rw-rw-r--   0 lightop   (1000) lightop   (1000)      474 2024-04-25 03:47:16.000000 metamath_py-0.0.5/src/metamath_py.egg-info/SOURCES.txt
+-rw-rw-r--   0 lightop   (1000) lightop   (1000)        1 2024-04-25 03:47:16.000000 metamath_py-0.0.5/src/metamath_py.egg-info/dependency_links.txt
+-rw-rw-r--   0 lightop   (1000) lightop   (1000)       11 2024-04-25 03:47:16.000000 metamath_py-0.0.5/src/metamath_py.egg-info/top_level.txt
+drwxrwxr-x   0 lightop   (1000) lightop   (1000)        0 2024-04-25 03:47:16.063389 metamath_py-0.0.5/src/metamathpy/
+-rw-rw-r--   0 lightop   (1000) lightop   (1000)        1 2024-01-31 23:13:41.000000 metamath_py-0.0.5/src/metamathpy/__init__.py
+-rw-rw-r--   0 lightop   (1000) lightop   (1000)     6844 2024-03-24 20:58:34.000000 metamath_py-0.0.5/src/metamathpy/database.py
+-rw-rw-r--   0 lightop   (1000) lightop   (1000)     2940 2024-04-25 03:45:07.000000 metamath_py-0.0.5/src/metamathpy/environment.py
+-rw-rw-r--   0 lightop   (1000) lightop   (1000)     2521 2024-01-31 23:13:41.000000 metamath_py-0.0.5/src/metamathpy/obvious.py
+-rw-rw-r--   0 lightop   (1000) lightop   (1000)     7411 2024-01-31 23:13:41.000000 metamath_py-0.0.5/src/metamathpy/parse.py
+-rw-rw-r--   0 lightop   (1000) lightop   (1000)    12437 2024-03-23 12:20:50.000000 metamath_py-0.0.5/src/metamathpy/proof.py
+-rw-rw-r--   0 lightop   (1000) lightop   (1000)     1012 2024-01-31 23:13:41.000000 metamath_py-0.0.5/src/metamathpy/scratch.py
+-rw-rw-r--   0 lightop   (1000) lightop   (1000)     6352 2024-01-31 23:13:41.000000 metamath_py-0.0.5/src/metamathpy/theory.py
+-rw-rw-r--   0 lightop   (1000) lightop   (1000)      911 2024-01-31 23:24:22.000000 metamath_py-0.0.5/src/metamathpy/training_data.py
+-rw-rw-r--   0 lightop   (1000) lightop   (1000)     1513 2024-03-23 12:20:50.000000 metamath_py-0.0.5/src/metamathpy/unification.py
+drwxrwxr-x   0 lightop   (1000) lightop   (1000)        0 2024-04-25 03:47:16.063389 metamath_py-0.0.5/tests/
+-rw-rw-r--   0 lightop   (1000) lightop   (1000)     3097 2023-09-27 01:27:35.000000 metamath_py-0.0.5/tests/tests.py
```

### Comparing `metamath_py-0.0.4/LICENSE` & `metamath_py-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `metamath_py-0.0.4/PKG-INFO` & `metamath_py-0.0.5/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: metamath-py
-Version: 0.0.4
-Summary: A Python interface to Metamath
-Author-email: "Garrett E. Katz" <garrett.katz@gmail.com>
-Project-URL: Homepage, https://github.com/garrettkatz/mmpy
-Project-URL: Bug Tracker, https://github.com/garrettkatz/mmpy/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 ## metamath-py
 
 A python interface to [Metamath](https://us.metamath.org/)
 
 # install
 
 `$ pip install --user metamath-py`
@@ -84,8 +70,46 @@
 {'ph': ('ph',), 'ps': ('(', 'ps', '->', 'ph', ')')}
 >>> root.dependencies # the other steps on which this one was justified
 {'wph': ProofStep(conclusion=[wph] wff ph), 'wps': ProofStep(conclusion=[wi] wff ( ps -> ph )), 'min': ProofStep(conclusion=[a1i.1] |- ph), 'maj': ProofStep(conclusion=[ax-1] |- ( ph -> ( ps -> ph ) ))}
 ```
 
 The dependencies are a dictionary where keys are the labels of the rule's hypotheses, and values are the other proof steps that satisfied those hypotheses.  These can be thought of as the children of the root in the proof tree.
 
+You can instantiate a gym-like environment that operates similarly to [metamath solitaire](https://catsarefluffy.github.io/mmsjs/unify.html).  Initialize it with a database and reset to a blank proof state, optionally with a claim you want to prove:
+
+```
+>>> from metamathpy.environment import Environment
+>>> env = Environment(db)
+>>> env.reset(claim=db.rules['mpd'])
+(<metamathpy.database.Rule object at 0x74ad291f37c0>, [], [])
+```
+
+It returns a state tuple (claim, proof, stack).  Rule applications are treated like actions and their labels are saved in the proof list.  The stack is updated according to the metamath proof verification algorithm.  To apply a rule, provide it as an action at the current step:
+
+```
+>>> env.step("wph")
+((<metamathpy.database.Rule object at 0x74ad291f37c0>, [], [ProofStep(conclusion=[wph] wff ph)]), '')
+>>> env.step("wps")
+((<metamathpy.database.Rule object at 0x74ad291f37c0>, [], [ProofStep(conclusion=[wph] wff ph), ProofStep(conclusion=[wps] wff ps)]), '')
+>>> env.step("wi")
+((<metamathpy.database.Rule object at 0x74ad291f37c0>, [], [ProofStep(conclusion=[wi] wff ( ph -> ps ))]), '')
+>>> env.step("wi")
+((<metamathpy.database.Rule object at 0x74ad291f37c0>, [], [None]), '2 hypotheses != 1 dependences')
+```
+
+The step returns a (state, msg) tuple.  msg is empty if the rule was valid, otherwise it contains an error message and the top of stack is None.
+
+Environments can be deep-copied if you want to use them in a branching tree search:
+
+```
+>>> env.reset()
+(None, [], [])
+>>> env.step("wph")
+((None, ['wph'], [ProofStep(conclusion=[wph] wff ph)]), '')
+>>> env2 = env.copy()
+>>> env.step("wi")
+((None, ['wph', 'wi'], [None]), '2 hypotheses != 1 dependences')
+>>> env2.step("wps")
+((None, ['wph', 'wps'], [ProofStep(conclusion=[wph] wff ph), ProofStep(conclusion=[wps] wff ps)]), '')
+
+```
```

### Comparing `metamath_py-0.0.4/pyproject.toml` & `metamath_py-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "metamath-py"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Garrett E. Katz", email="garrett.katz@gmail.com" },
 ]
 description = "A Python interface to Metamath"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `metamath_py-0.0.4/src/metamathpy/database.py` & `metamath_py-0.0.5/src/metamathpy/database.py`

 * *Files identical despite different names*

### Comparing `metamath_py-0.0.4/src/metamathpy/environment.py` & `metamath_py-0.0.5/src/metamathpy/environment.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,16 +23,16 @@
         self.claim = None
         self.proof = []
         self.stack = []
 
     def copy(self):
         env = Environment(self.db)
         env.claim = self.claim
-        env.proof = self.proof
-        env.stack = self.stack
+        env.proof = list(self.proof)
+        env.stack = list(self.stack)
         return env
 
     def reset(self, claim=None):
         self.claim = claim
         self.proof = []
         self.stack = []
         return (self.claim, list(self.proof), list(self.stack))
@@ -46,16 +46,19 @@
         # conduct next proof step
         rule = self.db.rules[action]
         proof_step, msg = conduct(rule, self.stack, disjoint)
 
         # push proof step onto stack
         self.stack.append(proof_step)
 
+        # save actions so far in proof
+        self.proof.append(action)
+
         # return state and message
-        state = (self.claim, self.proof, self.stack)
+        state = (self.claim, list(self.proof), list(self.stack))
         return state, msg
 
 if __name__ == "__main__":
 
     from .database import *
     import os
     fpath = os.path.join(os.environ["HOME"], "metamath", "set.mm")
@@ -89,9 +92,19 @@
     proof = ["wph", "wps", "ax-1", "wph"]
     env.reset()
     for a, action in enumerate(proof):
         (claim, _, stack), msg = env.step(action)
         print(f"{a}: action = {action}, stack:")
         print(stack)
 
+    env = Environment(db)
+    print(env.reset())
+    
+    print(env.step("wph"))
+    env2 = env.copy()
+
+    print(env.step("wi"))
+    print(env2.step("wps"))
+
+
```

### Comparing `metamath_py-0.0.4/src/metamathpy/obvious.py` & `metamath_py-0.0.5/src/metamathpy/obvious.py`

 * *Files identical despite different names*

### Comparing `metamath_py-0.0.4/src/metamathpy/parse.py` & `metamath_py-0.0.5/src/metamathpy/parse.py`

 * *Files identical despite different names*

### Comparing `metamath_py-0.0.4/src/metamathpy/proof.py` & `metamath_py-0.0.5/src/metamathpy/proof.py`

 * *Files identical despite different names*

### Comparing `metamath_py-0.0.4/src/metamathpy/scratch.py` & `metamath_py-0.0.5/src/metamathpy/scratch.py`

 * *Files identical despite different names*

### Comparing `metamath_py-0.0.4/src/metamathpy/theory.py` & `metamath_py-0.0.5/src/metamathpy/theory.py`

 * *Files identical despite different names*

### Comparing `metamath_py-0.0.4/src/metamathpy/training_data.py` & `metamath_py-0.0.5/src/metamathpy/training_data.py`

 * *Files identical despite different names*

### Comparing `metamath_py-0.0.4/src/metamathpy/unification.py` & `metamath_py-0.0.5/src/metamathpy/unification.py`

 * *Files identical despite different names*

### Comparing `metamath_py-0.0.4/tests/tests.py` & `metamath_py-0.0.5/tests/tests.py`

 * *Files identical despite different names*


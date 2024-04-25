# Comparing `tmp/g2p_mix-0.3.8.tar.gz` & `tmp/g2p-mix-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "g2p_mix-0.3.8.tar", last modified: Mon Apr 22 11:50:43 2024, max compression
+gzip compressed data, was "g2p-mix-0.3.9.tar", last modified: Thu Apr 25 14:51:04 2024, max compression
```

## Comparing `g2p_mix-0.3.8.tar` & `g2p-mix-0.3.9.tar`

### file list

```diff
@@ -1,26 +1,28 @@
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-22 11:50:43.761764 g2p_mix-0.3.8/
--rw-r--r--   0 admin      (501) staff       (20)     1066 2024-03-28 03:45:18.000000 g2p_mix-0.3.8/LICENSE
--rw-r--r--   0 admin      (501) staff       (20)       67 2024-03-29 02:45:49.000000 g2p_mix-0.3.8/MANIFEST.in
--rw-r--r--   0 admin      (501) staff       (20)     1378 2024-04-22 11:50:43.761530 g2p_mix-0.3.8/PKG-INFO
--rw-r--r--   0 admin      (501) staff       (20)      775 2024-03-28 03:45:18.000000 g2p_mix-0.3.8/README.md
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-22 11:50:43.755036 g2p_mix-0.3.8/g2p_mix/
--rw-r--r--   0 admin      (501) staff       (20)      630 2024-03-28 03:45:18.000000 g2p_mix-0.3.8/g2p_mix/__init__.py
--rw-r--r--   0 admin      (501) staff       (20)     3147 2024-03-28 03:45:18.000000 g2p_mix-0.3.8/g2p_mix/constants.py
--rw-r--r--   0 admin      (501) staff       (20)     2494 2024-04-22 11:48:52.000000 g2p_mix-0.3.8/g2p_mix/g2p_eng.py
--rw-r--r--   0 admin      (501) staff       (20)     5007 2024-04-16 06:49:15.000000 g2p_mix-0.3.8/g2p_mix/g2p_mix.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-22 11:50:43.752162 g2p_mix-0.3.8/g2p_mix/nltk_data/
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-22 11:50:43.756440 g2p_mix-0.3.8/g2p_mix/nltk_data/corpora/
--rw-r--r--   0 admin      (501) staff       (20)   896069 2024-03-28 03:45:18.000000 g2p_mix-0.3.8/g2p_mix/nltk_data/corpora/cmudict.zip
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-22 11:50:43.758347 g2p_mix-0.3.8/g2p_mix/nltk_data/taggers/
--rw-r--r--   0 admin      (501) staff       (20)  2526731 2024-03-28 03:45:18.000000 g2p_mix-0.3.8/g2p_mix/nltk_data/taggers/averaged_perceptron_tagger.zip
--rw-r--r--   0 admin      (501) staff       (20)     2047 2024-03-28 03:45:18.000000 g2p_mix-0.3.8/g2p_mix/token.py
--rw-r--r--   0 admin      (501) staff       (20)    11066 2024-03-28 03:45:18.000000 g2p_mix-0.3.8/g2p_mix/tone_sandhi.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-22 11:50:43.756291 g2p_mix-0.3.8/g2p_mix.egg-info/
--rw-r--r--   0 admin      (501) staff       (20)     1378 2024-04-22 11:50:43.000000 g2p_mix-0.3.8/g2p_mix.egg-info/PKG-INFO
--rw-r--r--   0 admin      (501) staff       (20)      423 2024-04-22 11:50:43.000000 g2p_mix-0.3.8/g2p_mix.egg-info/SOURCES.txt
--rw-r--r--   0 admin      (501) staff       (20)        1 2024-04-22 11:50:43.000000 g2p_mix-0.3.8/g2p_mix.egg-info/dependency_links.txt
--rw-r--r--   0 admin      (501) staff       (20)       87 2024-04-22 11:50:43.000000 g2p_mix-0.3.8/g2p_mix.egg-info/requires.txt
--rw-r--r--   0 admin      (501) staff       (20)        8 2024-04-22 11:50:43.000000 g2p_mix-0.3.8/g2p_mix.egg-info/top_level.txt
--rw-r--r--   0 admin      (501) staff       (20)       48 2024-03-29 02:28:25.000000 g2p_mix-0.3.8/requirements.txt
--rw-r--r--   0 admin      (501) staff       (20)       38 2024-04-22 11:50:43.761810 g2p_mix-0.3.8/setup.cfg
--rw-r--r--   0 admin      (501) staff       (20)     1465 2024-04-22 11:49:26.000000 g2p_mix-0.3.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:51:04.635049 g2p-mix-0.3.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-25 14:51:04.000000 g2p-mix-0.3.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-25 14:51:04.000000 g2p-mix-0.3.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-04-25 14:51:04.635049 g2p-mix-0.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-25 14:51:04.000000 g2p-mix-0.3.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:51:04.631049 g2p-mix-0.3.9/g2p_mix/
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-25 14:51:04.000000 g2p-mix-0.3.9/g2p_mix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-25 14:51:04.000000 g2p-mix-0.3.9/g2p_mix/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-04-25 14:51:04.000000 g2p-mix-0.3.9/g2p_mix/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-04-25 14:51:04.000000 g2p-mix-0.3.9/g2p_mix/g2p_eng.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5007 2024-04-25 14:51:04.000000 g2p-mix-0.3.9/g2p_mix/g2p_mix.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:51:04.627049 g2p-mix-0.3.9/g2p_mix/nltk_data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:51:04.631049 g2p-mix-0.3.9/g2p_mix/nltk_data/corpora/
+-rw-r--r--   0 runner    (1001) docker     (127)   896069 2024-04-25 14:51:04.000000 g2p-mix-0.3.9/g2p_mix/nltk_data/corpora/cmudict.zip
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:51:04.631049 g2p-mix-0.3.9/g2p_mix/nltk_data/taggers/
+-rw-r--r--   0 runner    (1001) docker     (127)  2526731 2024-04-25 14:51:04.000000 g2p-mix-0.3.9/g2p_mix/nltk_data/taggers/averaged_perceptron_tagger.zip
+-rw-r--r--   0 runner    (1001) docker     (127)     2047 2024-04-25 14:51:04.000000 g2p-mix-0.3.9/g2p_mix/token.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11066 2024-04-25 14:51:04.000000 g2p-mix-0.3.9/g2p_mix/tone_sandhi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:51:04.631049 g2p-mix-0.3.9/g2p_mix.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-04-25 14:51:04.000000 g2p-mix-0.3.9/g2p_mix.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-25 14:51:04.000000 g2p-mix-0.3.9/g2p_mix.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 14:51:04.000000 g2p-mix-0.3.9/g2p_mix.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-25 14:51:04.000000 g2p-mix-0.3.9/g2p_mix.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-25 14:51:04.000000 g2p-mix-0.3.9/g2p_mix.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-25 14:51:04.000000 g2p-mix-0.3.9/g2p_mix.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-25 14:51:04.000000 g2p-mix-0.3.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 14:51:04.635049 g2p-mix-0.3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-04-25 14:51:04.000000 g2p-mix-0.3.9/setup.py
```

### Comparing `g2p_mix-0.3.8/LICENSE` & `g2p-mix-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `g2p_mix-0.3.8/PKG-INFO` & `g2p-mix-0.3.9/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,32 +1,27 @@
 Metadata-Version: 2.1
-Name: g2p_mix
-Version: 0.3.8
+Name: g2p-mix
+Version: 0.3.9
 Summary: G2P mix
-Home-page: https://github.com/pengzhendong/g2p_mix
+Home-page: https://github.com/pengzhendong/g2p-mix
 Author: Zhendong Peng
 Author-email: pzd17@tsinghua.org.cn
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering
 Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: g2p_en
-Requires-Dist: jieba
-Requires-Dist: pypinyin
-Requires-Dist: pypinyin-dict
-Requires-Dist: wordsegment
 Provides-Extra: g2pw
-Requires-Dist: torch; extra == "g2pw"
-Requires-Dist: modelscope; extra == "g2pw"
-Requires-Dist: pypinyin-g2pw; extra == "g2pw"
+License-File: LICENSE
 
-# g2p_mix
+# g2p-mix
 
 ```bash
-$ pip install g2p_mix
+$ pip install g2p-mix
 $ python
 ```
 
 ```python
 >>> from g2p_mix import G2pMix
 >>> G2pMix().g2p("你这个idea, 不太make sense。")
 ```
@@ -41,7 +36,9 @@
   { "word": "不", "phones": ["b", "u4"], "lang": "ZH" },
   { "word": "太", "phones": ["t", "ai4"], "lang": "ZH" },
   { "word": "make", "phones": ["M", "EY1", "K"], "lang": "EN" },
   { "word": "sense", "phones": ["S", "EH1", "N", "S"], "lang": "EN" },
   { "word": "。", "phones": "。", "lang": "SYM" }
 ]
 ```
+
+
```

### Comparing `g2p_mix-0.3.8/README.md` & `g2p-mix-0.3.9/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-# g2p_mix
+# g2p-mix
 
 ```bash
-$ pip install g2p_mix
+$ pip install g2p-mix
 $ python
 ```
 
 ```python
 >>> from g2p_mix import G2pMix
 >>> G2pMix().g2p("你这个idea, 不太make sense。")
 ```
```

### Comparing `g2p_mix-0.3.8/g2p_mix/__init__.py` & `g2p-mix-0.3.9/g2p_mix/__init__.py`

 * *Files identical despite different names*

### Comparing `g2p_mix-0.3.8/g2p_mix/constants.py` & `g2p-mix-0.3.9/g2p_mix/constants.py`

 * *Files identical despite different names*

### Comparing `g2p_mix-0.3.8/g2p_mix/g2p_eng.py` & `g2p-mix-0.3.9/g2p_mix/g2p_eng.py`

 * *Files identical despite different names*

### Comparing `g2p_mix-0.3.8/g2p_mix/g2p_mix.py` & `g2p-mix-0.3.9/g2p_mix/g2p_mix.py`

 * *Files identical despite different names*

### Comparing `g2p_mix-0.3.8/g2p_mix/nltk_data/corpora/cmudict.zip` & `g2p-mix-0.3.9/g2p_mix/nltk_data/corpora/cmudict.zip`

 * *Files identical despite different names*

### Comparing `g2p_mix-0.3.8/g2p_mix/nltk_data/taggers/averaged_perceptron_tagger.zip` & `g2p-mix-0.3.9/g2p_mix/nltk_data/taggers/averaged_perceptron_tagger.zip`

 * *Files identical despite different names*

### Comparing `g2p_mix-0.3.8/g2p_mix/token.py` & `g2p-mix-0.3.9/g2p_mix/token.py`

 * *Files identical despite different names*

### Comparing `g2p_mix-0.3.8/g2p_mix/tone_sandhi.py` & `g2p-mix-0.3.9/g2p_mix/tone_sandhi.py`

 * *Files identical despite different names*

### Comparing `g2p_mix-0.3.8/g2p_mix.egg-info/PKG-INFO` & `g2p-mix-0.3.9/g2p_mix.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,32 +1,27 @@
 Metadata-Version: 2.1
 Name: g2p-mix
-Version: 0.3.8
+Version: 0.3.9
 Summary: G2P mix
-Home-page: https://github.com/pengzhendong/g2p_mix
+Home-page: https://github.com/pengzhendong/g2p-mix
 Author: Zhendong Peng
 Author-email: pzd17@tsinghua.org.cn
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering
 Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: g2p_en
-Requires-Dist: jieba
-Requires-Dist: pypinyin
-Requires-Dist: pypinyin-dict
-Requires-Dist: wordsegment
 Provides-Extra: g2pw
-Requires-Dist: torch; extra == "g2pw"
-Requires-Dist: modelscope; extra == "g2pw"
-Requires-Dist: pypinyin-g2pw; extra == "g2pw"
+License-File: LICENSE
 
-# g2p_mix
+# g2p-mix
 
 ```bash
-$ pip install g2p_mix
+$ pip install g2p-mix
 $ python
 ```
 
 ```python
 >>> from g2p_mix import G2pMix
 >>> G2pMix().g2p("你这个idea, 不太make sense。")
 ```
@@ -41,7 +36,9 @@
   { "word": "不", "phones": ["b", "u4"], "lang": "ZH" },
   { "word": "太", "phones": ["t", "ai4"], "lang": "ZH" },
   { "word": "make", "phones": ["M", "EY1", "K"], "lang": "EN" },
   { "word": "sense", "phones": ["S", "EH1", "N", "S"], "lang": "EN" },
   { "word": "。", "phones": "。", "lang": "SYM" }
 ]
 ```
+
+
```

### Comparing `g2p_mix-0.3.8/setup.py` & `g2p-mix-0.3.9/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -20,24 +20,30 @@
     long_description = fin.read()
 
 with open("requirements.txt", encoding="utf-8") as f:
     requirements = f.readlines()
 extras_require = {"g2pw": ["torch", "modelscope", "pypinyin-g2pw"]}
 
 setup(
-    name="g2p_mix",
-    version=os.getenv("BUILD_VERSION") or "0.3.8",
+    name="g2p-mix",
+    version=os.getenv("BUILD_VERSION") or "0.0.1",
     author="Zhendong Peng",
     author_email="pzd17@tsinghua.org.cn",
     long_description=long_description,
     long_description_content_type="text/markdown",
     description="G2P mix",
-    url="https://github.com/pengzhendong/g2p_mix",
+    url="https://github.com/pengzhendong/g2p-mix",
     packages=find_packages(),
     include_package_data=True,
     install_requires=requirements,
     extras_require=extras_require,
+    entry_points={
+        "console_scripts": [
+            "g2p_mix = g2p_mix.cli:main",
+        ]
+    },
     classifiers=[
         "Programming Language :: Python :: 3",
+        "Operating System :: OS Independent",
         "Topic :: Scientific/Engineering",
     ],
 )
```


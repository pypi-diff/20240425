# Comparing `tmp/g2p-mix-0.3.9.tar.gz` & `tmp/g2p-mix-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "g2p-mix-0.3.9.tar", last modified: Thu Apr 25 14:51:04 2024, max compression
+gzip compressed data, was "g2p-mix-0.4.0.tar", last modified: Thu Apr 25 15:25:05 2024, max compression
```

## Comparing `g2p-mix-0.3.9.tar` & `g2p-mix-0.4.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:51:04.635049 g2p-mix-0.3.9/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-25 14:51:04.000000 g2p-mix-0.3.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-25 14:51:04.000000 g2p-mix-0.3.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-04-25 14:51:04.635049 g2p-mix-0.3.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-25 14:51:04.000000 g2p-mix-0.3.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:51:04.631049 g2p-mix-0.3.9/g2p_mix/
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-25 14:51:04.000000 g2p-mix-0.3.9/g2p_mix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-25 14:51:04.000000 g2p-mix-0.3.9/g2p_mix/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-04-25 14:51:04.000000 g2p-mix-0.3.9/g2p_mix/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-04-25 14:51:04.000000 g2p-mix-0.3.9/g2p_mix/g2p_eng.py
--rw-r--r--   0 runner    (1001) docker     (127)     5007 2024-04-25 14:51:04.000000 g2p-mix-0.3.9/g2p_mix/g2p_mix.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:51:04.627049 g2p-mix-0.3.9/g2p_mix/nltk_data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:51:04.631049 g2p-mix-0.3.9/g2p_mix/nltk_data/corpora/
--rw-r--r--   0 runner    (1001) docker     (127)   896069 2024-04-25 14:51:04.000000 g2p-mix-0.3.9/g2p_mix/nltk_data/corpora/cmudict.zip
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:51:04.631049 g2p-mix-0.3.9/g2p_mix/nltk_data/taggers/
--rw-r--r--   0 runner    (1001) docker     (127)  2526731 2024-04-25 14:51:04.000000 g2p-mix-0.3.9/g2p_mix/nltk_data/taggers/averaged_perceptron_tagger.zip
--rw-r--r--   0 runner    (1001) docker     (127)     2047 2024-04-25 14:51:04.000000 g2p-mix-0.3.9/g2p_mix/token.py
--rw-r--r--   0 runner    (1001) docker     (127)    11066 2024-04-25 14:51:04.000000 g2p-mix-0.3.9/g2p_mix/tone_sandhi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:51:04.631049 g2p-mix-0.3.9/g2p_mix.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-04-25 14:51:04.000000 g2p-mix-0.3.9/g2p_mix.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-25 14:51:04.000000 g2p-mix-0.3.9/g2p_mix.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 14:51:04.000000 g2p-mix-0.3.9/g2p_mix.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-25 14:51:04.000000 g2p-mix-0.3.9/g2p_mix.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-25 14:51:04.000000 g2p-mix-0.3.9/g2p_mix.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-25 14:51:04.000000 g2p-mix-0.3.9/g2p_mix.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-25 14:51:04.000000 g2p-mix-0.3.9/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 14:51:04.635049 g2p-mix-0.3.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-04-25 14:51:04.000000 g2p-mix-0.3.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:25:05.446702 g2p-mix-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-25 15:25:04.000000 g2p-mix-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-25 15:25:04.000000 g2p-mix-0.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-04-25 15:25:05.446702 g2p-mix-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-25 15:25:04.000000 g2p-mix-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:25:05.438702 g2p-mix-0.4.0/g2p_mix/
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-25 15:25:04.000000 g2p-mix-0.4.0/g2p_mix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-25 15:25:04.000000 g2p-mix-0.4.0/g2p_mix/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-04-25 15:25:04.000000 g2p-mix-0.4.0/g2p_mix/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-04-25 15:25:04.000000 g2p-mix-0.4.0/g2p_mix/g2p_eng.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5007 2024-04-25 15:25:04.000000 g2p-mix-0.4.0/g2p_mix/g2p_mix.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:25:05.438702 g2p-mix-0.4.0/g2p_mix/nltk_data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:25:05.442702 g2p-mix-0.4.0/g2p_mix/nltk_data/corpora/
+-rw-r--r--   0 runner    (1001) docker     (127)   896069 2024-04-25 15:25:04.000000 g2p-mix-0.4.0/g2p_mix/nltk_data/corpora/cmudict.zip
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:25:05.442702 g2p-mix-0.4.0/g2p_mix/nltk_data/taggers/
+-rw-r--r--   0 runner    (1001) docker     (127)  2526731 2024-04-25 15:25:04.000000 g2p-mix-0.4.0/g2p_mix/nltk_data/taggers/averaged_perceptron_tagger.zip
+-rw-r--r--   0 runner    (1001) docker     (127)     2047 2024-04-25 15:25:04.000000 g2p-mix-0.4.0/g2p_mix/token.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11066 2024-04-25 15:25:04.000000 g2p-mix-0.4.0/g2p_mix/tone_sandhi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:25:05.438702 g2p-mix-0.4.0/g2p_mix.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-04-25 15:25:05.000000 g2p-mix-0.4.0/g2p_mix.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-25 15:25:05.000000 g2p-mix-0.4.0/g2p_mix.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 15:25:05.000000 g2p-mix-0.4.0/g2p_mix.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-25 15:25:05.000000 g2p-mix-0.4.0/g2p_mix.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-25 15:25:05.000000 g2p-mix-0.4.0/g2p_mix.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-25 15:25:05.000000 g2p-mix-0.4.0/g2p_mix.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-25 15:25:04.000000 g2p-mix-0.4.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 15:25:05.446702 g2p-mix-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-04-25 15:25:04.000000 g2p-mix-0.4.0/setup.py
```

### Comparing `g2p-mix-0.3.9/LICENSE` & `g2p-mix-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `g2p-mix-0.3.9/PKG-INFO` & `g2p-mix-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: g2p-mix
-Version: 0.3.9
+Version: 0.4.0
 Summary: G2P mix
 Home-page: https://github.com/pengzhendong/g2p-mix
 Author: Zhendong Peng
 Author-email: pzd17@tsinghua.org.cn
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `g2p-mix-0.3.9/README.md` & `g2p-mix-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `g2p-mix-0.3.9/g2p_mix/__init__.py` & `g2p-mix-0.4.0/g2p_mix/__init__.py`

 * *Files identical despite different names*

### Comparing `g2p-mix-0.3.9/g2p_mix/cli.py` & `g2p-mix-0.4.0/g2p_mix/cli.py`

 * *Files identical despite different names*

### Comparing `g2p-mix-0.3.9/g2p_mix/constants.py` & `g2p-mix-0.4.0/g2p_mix/constants.py`

 * *Files identical despite different names*

### Comparing `g2p-mix-0.3.9/g2p_mix/g2p_eng.py` & `g2p-mix-0.4.0/g2p_mix/g2p_eng.py`

 * *Files identical despite different names*

### Comparing `g2p-mix-0.3.9/g2p_mix/g2p_mix.py` & `g2p-mix-0.4.0/g2p_mix/g2p_mix.py`

 * *Files identical despite different names*

### Comparing `g2p-mix-0.3.9/g2p_mix/nltk_data/corpora/cmudict.zip` & `g2p-mix-0.4.0/g2p_mix/nltk_data/corpora/cmudict.zip`

 * *Files identical despite different names*

### Comparing `g2p-mix-0.3.9/g2p_mix/nltk_data/taggers/averaged_perceptron_tagger.zip` & `g2p-mix-0.4.0/g2p_mix/nltk_data/taggers/averaged_perceptron_tagger.zip`

 * *Files identical despite different names*

### Comparing `g2p-mix-0.3.9/g2p_mix/token.py` & `g2p-mix-0.4.0/g2p_mix/token.py`

 * *Files identical despite different names*

### Comparing `g2p-mix-0.3.9/g2p_mix/tone_sandhi.py` & `g2p-mix-0.4.0/g2p_mix/tone_sandhi.py`

 * *Files identical despite different names*

### Comparing `g2p-mix-0.3.9/g2p_mix.egg-info/PKG-INFO` & `g2p-mix-0.4.0/g2p_mix.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: g2p-mix
-Version: 0.3.9
+Version: 0.4.0
 Summary: G2P mix
 Home-page: https://github.com/pengzhendong/g2p-mix
 Author: Zhendong Peng
 Author-email: pzd17@tsinghua.org.cn
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `g2p-mix-0.3.9/setup.py` & `g2p-mix-0.4.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,28 +8,27 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import os
 from setuptools import setup, find_packages
 
 
 with open("README.md", encoding="utf8") as fin:
     long_description = fin.read()
 
-with open("requirements.txt", encoding="utf-8") as f:
+with open("requirements.txt", encoding="utf8") as f:
     requirements = f.readlines()
 extras_require = {"g2pw": ["torch", "modelscope", "pypinyin-g2pw"]}
 
 setup(
     name="g2p-mix",
-    version=os.getenv("BUILD_VERSION") or "0.0.1",
+    version=open("VERSION", encoding="utf8").read(),
     author="Zhendong Peng",
     author_email="pzd17@tsinghua.org.cn",
     long_description=long_description,
     long_description_content_type="text/markdown",
     description="G2P mix",
     url="https://github.com/pengzhendong/g2p-mix",
     packages=find_packages(),
```


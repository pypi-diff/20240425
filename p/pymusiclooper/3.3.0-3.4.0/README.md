# Comparing `tmp/pymusiclooper-3.3.0.tar.gz` & `tmp/pymusiclooper-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymusiclooper-3.3.0.tar", max compression
+gzip compressed data, was "pymusiclooper-3.4.0.tar", max compression
```

## Comparing `pymusiclooper-3.3.0.tar` & `pymusiclooper-3.4.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1067 2024-03-21 21:08:57.376999 pymusiclooper-3.3.0/LICENSE
--rw-r--r--   0        0        0     9359 2024-03-21 21:08:57.376999 pymusiclooper-3.3.0/README.md
--rw-r--r--   0        0        0       72 2024-03-21 21:08:57.376999 pymusiclooper-3.3.0/pymusiclooper/__init__.py
--rw-r--r--   0        0        0      212 2024-03-21 21:08:57.376999 pymusiclooper-3.3.0/pymusiclooper/__main__.py
--rw-r--r--   0        0        0    24198 2024-03-21 21:08:57.376999 pymusiclooper-3.3.0/pymusiclooper/analysis.py
--rw-r--r--   0        0        0     3749 2024-03-21 21:08:57.376999 pymusiclooper-3.3.0/pymusiclooper/audio.py
--rw-r--r--   0        0        0    12613 2024-03-21 21:08:57.376999 pymusiclooper-3.3.0/pymusiclooper/cli.py
--rw-r--r--   0        0        0     1953 2024-03-21 21:08:57.376999 pymusiclooper-3.3.0/pymusiclooper/console.py
--rw-r--r--   0        0        0    14568 2024-03-21 21:08:57.376999 pymusiclooper-3.3.0/pymusiclooper/core.py
--rw-r--r--   0        0        0      205 2024-03-21 21:08:57.376999 pymusiclooper-3.3.0/pymusiclooper/exceptions.py
--rw-r--r--   0        0        0    17841 2024-03-21 21:08:57.376999 pymusiclooper-3.3.0/pymusiclooper/handler.py
--rw-r--r--   0        0        0     6108 2024-03-21 21:08:57.376999 pymusiclooper-3.3.0/pymusiclooper/playback.py
--rw-r--r--   0        0        0     1933 2024-03-21 21:08:57.376999 pymusiclooper-3.3.0/pymusiclooper/utils.py
--rw-r--r--   0        0        0     2327 2024-03-21 21:08:57.376999 pymusiclooper-3.3.0/pymusiclooper/youtube.py
--rw-r--r--   0        0        0     1578 2024-03-21 21:08:57.376999 pymusiclooper-3.3.0/pyproject.toml
--rw-r--r--   0        0        0    11049 1970-01-01 00:00:00.000000 pymusiclooper-3.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-04-25 16:23:19.776152 pymusiclooper-3.4.0/LICENSE
+-rw-r--r--   0        0        0     9359 2024-04-25 16:23:19.776152 pymusiclooper-3.4.0/README.md
+-rw-r--r--   0        0        0       72 2024-04-25 16:23:19.776152 pymusiclooper-3.4.0/pymusiclooper/__init__.py
+-rw-r--r--   0        0        0      212 2024-04-25 16:23:19.776152 pymusiclooper-3.4.0/pymusiclooper/__main__.py
+-rw-r--r--   0        0        0    24198 2024-04-25 16:23:19.780153 pymusiclooper-3.4.0/pymusiclooper/analysis.py
+-rw-r--r--   0        0        0     3749 2024-04-25 16:23:19.780153 pymusiclooper-3.4.0/pymusiclooper/audio.py
+-rw-r--r--   0        0        0    12613 2024-04-25 16:23:19.780153 pymusiclooper-3.4.0/pymusiclooper/cli.py
+-rw-r--r--   0        0        0     1953 2024-04-25 16:23:19.780153 pymusiclooper-3.4.0/pymusiclooper/console.py
+-rw-r--r--   0        0        0    14568 2024-04-25 16:23:19.780153 pymusiclooper-3.4.0/pymusiclooper/core.py
+-rw-r--r--   0        0        0      205 2024-04-25 16:23:19.780153 pymusiclooper-3.4.0/pymusiclooper/exceptions.py
+-rw-r--r--   0        0        0    17841 2024-04-25 16:23:19.780153 pymusiclooper-3.4.0/pymusiclooper/handler.py
+-rw-r--r--   0        0        0     6108 2024-04-25 16:23:19.780153 pymusiclooper-3.4.0/pymusiclooper/playback.py
+-rw-r--r--   0        0        0     1933 2024-04-25 16:23:19.780153 pymusiclooper-3.4.0/pymusiclooper/utils.py
+-rw-r--r--   0        0        0     2327 2024-04-25 16:23:19.780153 pymusiclooper-3.4.0/pymusiclooper/youtube.py
+-rw-r--r--   0        0        0     1720 2024-04-25 16:23:19.780153 pymusiclooper-3.4.0/pyproject.toml
+-rw-r--r--   0        0        0    11020 1970-01-01 00:00:00.000000 pymusiclooper-3.4.0/PKG-INFO
```

### Comparing `pymusiclooper-3.3.0/LICENSE` & `pymusiclooper-3.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pymusiclooper-3.3.0/README.md` & `pymusiclooper-3.4.0/README.md`

 * *Files identical despite different names*

### Comparing `pymusiclooper-3.3.0/pymusiclooper/analysis.py` & `pymusiclooper-3.4.0/pymusiclooper/analysis.py`

 * *Files identical despite different names*

### Comparing `pymusiclooper-3.3.0/pymusiclooper/audio.py` & `pymusiclooper-3.4.0/pymusiclooper/audio.py`

 * *Files identical despite different names*

### Comparing `pymusiclooper-3.3.0/pymusiclooper/cli.py` & `pymusiclooper-3.4.0/pymusiclooper/cli.py`

 * *Files identical despite different names*

### Comparing `pymusiclooper-3.3.0/pymusiclooper/console.py` & `pymusiclooper-3.4.0/pymusiclooper/console.py`

 * *Files identical despite different names*

### Comparing `pymusiclooper-3.3.0/pymusiclooper/core.py` & `pymusiclooper-3.4.0/pymusiclooper/core.py`

 * *Files identical despite different names*

### Comparing `pymusiclooper-3.3.0/pymusiclooper/handler.py` & `pymusiclooper-3.4.0/pymusiclooper/handler.py`

 * *Files identical despite different names*

### Comparing `pymusiclooper-3.3.0/pymusiclooper/playback.py` & `pymusiclooper-3.4.0/pymusiclooper/playback.py`

 * *Files identical despite different names*

### Comparing `pymusiclooper-3.3.0/pymusiclooper/utils.py` & `pymusiclooper-3.4.0/pymusiclooper/utils.py`

 * *Files identical despite different names*

### Comparing `pymusiclooper-3.3.0/pymusiclooper/youtube.py` & `pymusiclooper-3.4.0/pymusiclooper/youtube.py`

 * *Files identical despite different names*

### Comparing `pymusiclooper-3.3.0/pyproject.toml` & `pymusiclooper-3.4.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,43 +1,45 @@
 [tool.poetry]
 name = "pymusiclooper"
-version = "3.3.0"
+version = "3.4.0"
 description = "Repeat music endlessly and create seamless music loops, with play/export/tagging support."
 license = "MIT"
 classifiers = [
   "Development Status :: 5 - Production/Stable",
   "Environment :: Console",
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3 :: Only",
-  "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
   "Topic :: Multimedia :: Sound/Audio",
   "Topic :: Multimedia :: Sound/Audio :: Analysis",
 ]
 repository = "https://github.com/arkrow/PyMusicLooper"
 readme = "README.md"
 authors = ["arkrow <arkrow@protonmail.com>"]
 
 [tool.poetry.dependencies]
-python = "^3.8"
-librosa = "^0.10.0"
-numpy = ">=1.24.0"
+python = "^3.9"
+librosa = "^0.10.1"
+numpy = ">=1.25.0"
+# Add scipy constraint temporarily as a workaround till librosa's 0.10.2 release
+# Fixes the scipy.signal.hann AttributeError since it was deprecated in scipy>=1.13.0 
+scipy = "<1.13.0"
 soundfile = ">=0.12.1"
 sounddevice = ">=0.4.6"
 setuptools = ">=67.0.0"
 rich-click = "^1.6.1"
 rich = ">= 13.4.2"
 pytaglib = ">=2.0.0"
-numba = "^0.57.0"
-yt-dlp = ">=2023.11.16"
+numba = ">=0.59.1"
+yt-dlp = ">=2024.4.9"
 click-params = "^0.4.1"
 click-option-group = "^0.5.6"
 lazy-loader = ">=0.3"
 
 [tool.poetry.scripts]
 pymusiclooper = 'pymusiclooper.__main__:cli'
```

### Comparing `pymusiclooper-3.3.0/PKG-INFO` & `pymusiclooper-3.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 Metadata-Version: 2.1
 Name: pymusiclooper
-Version: 3.3.0
+Version: 3.4.0
 Summary: Repeat music endlessly and create seamless music loops, with play/export/tagging support.
 Home-page: https://github.com/arkrow/PyMusicLooper
 License: MIT
 Author: arkrow
 Author-email: arkrow@protonmail.com
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Multimedia :: Sound/Audio
 Classifier: Topic :: Multimedia :: Sound/Audio :: Analysis
 Requires-Dist: click-option-group (>=0.5.6,<0.6.0)
 Requires-Dist: click-params (>=0.4.1,<0.5.0)
 Requires-Dist: lazy-loader (>=0.3)
-Requires-Dist: librosa (>=0.10.0,<0.11.0)
-Requires-Dist: numba (>=0.57.0,<0.58.0)
-Requires-Dist: numpy (>=1.24.0)
+Requires-Dist: librosa (>=0.10.1,<0.11.0)
+Requires-Dist: numba (>=0.59.1)
+Requires-Dist: numpy (>=1.25.0)
 Requires-Dist: pytaglib (>=2.0.0)
 Requires-Dist: rich (>=13.4.2)
 Requires-Dist: rich-click (>=1.6.1,<2.0.0)
+Requires-Dist: scipy (<1.13.0)
 Requires-Dist: setuptools (>=67.0.0)
 Requires-Dist: sounddevice (>=0.4.6)
 Requires-Dist: soundfile (>=0.12.1)
-Requires-Dist: yt-dlp (>=2023.11.16)
+Requires-Dist: yt-dlp (>=2024.4.9)
 Project-URL: Changelog, https://github.com/arkrow/PyMusicLooper/blob/master/CHANGELOG.md
 Project-URL: Repository, https://github.com/arkrow/PyMusicLooper
 Description-Content-Type: text/markdown
 
 # PyMusicLooper
 
 [![Downloads](https://static.pepy.tech/badge/pymusiclooper)](https://pepy.tech/project/pymusiclooper)
```


# Comparing `tmp/pyannote-onnx-0.0.3.tar.gz` & `tmp/pyannote-onnx-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyannote-onnx-0.0.3.tar", last modified: Fri Apr 12 06:31:44 2024, max compression
+gzip compressed data, was "pyannote-onnx-0.0.4.tar", last modified: Thu Apr 25 15:35:33 2024, max compression
```

## Comparing `pyannote-onnx-0.0.3.tar` & `pyannote-onnx-0.0.4.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-12 06:31:44.529967 pyannote-onnx-0.0.3/
--rw-r--r--   0 admin      (501) staff       (20)    11357 2024-04-12 01:55:28.000000 pyannote-onnx-0.0.3/LICENSE
--rw-r--r--   0 admin      (501) staff       (20)       64 2024-04-12 01:55:28.000000 pyannote-onnx-0.0.3/MANIFEST.in
--rw-r--r--   0 admin      (501) staff       (20)     1534 2024-04-12 06:31:44.529719 pyannote-onnx-0.0.3/PKG-INFO
--rw-r--r--   0 admin      (501) staff       (20)     1020 2024-04-12 01:55:28.000000 pyannote-onnx-0.0.3/README.md
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-12 06:31:44.525130 pyannote-onnx-0.0.3/pyannote_onnx/
--rw-r--r--   0 admin      (501) staff       (20)      636 2024-04-12 01:55:28.000000 pyannote-onnx-0.0.3/pyannote_onnx/__init__.py
--rw-r--r--   0 admin      (501) staff       (20)     1398 2024-04-12 01:55:28.000000 pyannote-onnx-0.0.3/pyannote_onnx/inference_session.py
--rw-r--r--   0 admin      (501) staff       (20)    13799 2024-04-12 06:29:25.000000 pyannote-onnx-0.0.3/pyannote_onnx/pyannote_onnx.py
--rw-r--r--   0 admin      (501) staff       (20)  5983836 2024-04-12 01:55:28.000000 pyannote-onnx-0.0.3/pyannote_onnx/segmentation-3.0.onnx
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-12 06:31:44.529433 pyannote-onnx-0.0.3/pyannote_onnx.egg-info/
--rw-r--r--   0 admin      (501) staff       (20)     1534 2024-04-12 06:31:44.000000 pyannote-onnx-0.0.3/pyannote_onnx.egg-info/PKG-INFO
--rw-r--r--   0 admin      (501) staff       (20)      407 2024-04-12 06:31:44.000000 pyannote-onnx-0.0.3/pyannote_onnx.egg-info/SOURCES.txt
--rw-r--r--   0 admin      (501) staff       (20)        1 2024-04-12 06:31:44.000000 pyannote-onnx-0.0.3/pyannote_onnx.egg-info/dependency_links.txt
--rw-r--r--   0 admin      (501) staff       (20)       42 2024-04-12 06:31:44.000000 pyannote-onnx-0.0.3/pyannote_onnx.egg-info/entry_points.txt
--rw-r--r--   0 admin      (501) staff       (20)       42 2024-04-12 06:31:44.000000 pyannote-onnx-0.0.3/pyannote_onnx.egg-info/requires.txt
--rw-r--r--   0 admin      (501) staff       (20)       14 2024-04-12 06:31:44.000000 pyannote-onnx-0.0.3/pyannote_onnx.egg-info/top_level.txt
--rw-r--r--   0 admin      (501) staff       (20)       42 2024-04-12 01:55:28.000000 pyannote-onnx-0.0.3/requirements.txt
--rw-r--r--   0 admin      (501) staff       (20)       38 2024-04-12 06:31:44.530010 pyannote-onnx-0.0.3/setup.cfg
--rw-r--r--   0 admin      (501) staff       (20)     1530 2024-04-12 06:30:37.000000 pyannote-onnx-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:35:33.367649 pyannote-onnx-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-25 15:35:33.000000 pyannote-onnx-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-25 15:35:33.000000 pyannote-onnx-0.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-04-25 15:35:33.367649 pyannote-onnx-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-04-25 15:35:33.000000 pyannote-onnx-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-25 15:35:33.000000 pyannote-onnx-0.0.4/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:35:33.359649 pyannote-onnx-0.0.4/pyannote_onnx/
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-25 15:35:33.000000 pyannote-onnx-0.0.4/pyannote_onnx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-04-25 15:35:33.000000 pyannote-onnx-0.0.4/pyannote_onnx/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-04-25 15:35:33.000000 pyannote-onnx-0.0.4/pyannote_onnx/inference_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13811 2024-04-25 15:35:33.000000 pyannote-onnx-0.0.4/pyannote_onnx/pyannote_onnx.py
+-rw-r--r--   0 runner    (1001) docker     (127)  5983836 2024-04-25 15:35:33.000000 pyannote-onnx-0.0.4/pyannote_onnx/segmentation-3.0.onnx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 15:35:33.367649 pyannote-onnx-0.0.4/pyannote_onnx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-04-25 15:35:33.000000 pyannote-onnx-0.0.4/pyannote_onnx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-25 15:35:33.000000 pyannote-onnx-0.0.4/pyannote_onnx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 15:35:33.000000 pyannote-onnx-0.0.4/pyannote_onnx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-25 15:35:33.000000 pyannote-onnx-0.0.4/pyannote_onnx.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-25 15:35:33.000000 pyannote-onnx-0.0.4/pyannote_onnx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-25 15:35:33.000000 pyannote-onnx-0.0.4/pyannote_onnx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-25 15:35:33.000000 pyannote-onnx-0.0.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 15:35:33.367649 pyannote-onnx-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-04-25 15:35:33.000000 pyannote-onnx-0.0.4/setup.py
```

### Comparing `pyannote-onnx-0.0.3/LICENSE` & `pyannote-onnx-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyannote-onnx-0.0.3/PKG-INFO` & `pyannote-onnx-0.0.4/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 Metadata-Version: 2.1
 Name: pyannote-onnx
-Version: 0.0.3
+Version: 0.0.4
 Summary: Pyannote ONNX
 Home-page: https://github.com/pengzhendong/pyannote-onnx
 Author: Zhendong Peng
 Author-email: pzd17@tsinghua.org.cn
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: click
-Requires-Dist: librosa
-Requires-Dist: numpy
-Requires-Dist: onnxruntime
-Requires-Dist: soundfile
 
 # Speaker Diarization
 
 > [pyannote-audio](https://github.com/pyannote/pyannote-audio) is an open-source toolkit written in Python for speaker diarization.
 
 `pyannote-onnx` is used to convert the [pretrained model](https://huggingface.co/pyannote/segmentation-3.0) defined in PyTorch into the ONNX format and then run it with [ONNX Runtime](https://github.com/microsoft/onnxruntime) (in C++ or Python).
 
@@ -33,7 +30,9 @@
 ```bash
 $ pip install torch onnx https://github.com/pyannote/pyannote-audio/archive/refs/heads/develop.zip
 $ python export_onnx.py pytorch_model.bin segmentation-3.0.onnx
 
 $ pip install -r requirements.txt
 $ python main.py data/test_16k.wav
 ```
+
+
```

### Comparing `pyannote-onnx-0.0.3/README.md` & `pyannote-onnx-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `pyannote-onnx-0.0.3/pyannote_onnx/__init__.py` & `pyannote-onnx-0.0.4/pyannote_onnx/__init__.py`

 * *Files identical despite different names*

### Comparing `pyannote-onnx-0.0.3/pyannote_onnx/inference_session.py` & `pyannote-onnx-0.0.4/pyannote_onnx/inference_session.py`

 * *Files identical despite different names*

### Comparing `pyannote-onnx-0.0.3/pyannote_onnx/pyannote_onnx.py` & `pyannote-onnx-0.0.4/pyannote_onnx/pyannote_onnx.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 from itertools import permutations
 from pathlib import Path
 from typing import Union
 
 import librosa
 import numpy as np
 import soundfile as sf
-from numpy.linalg import norm
 
 from .inference_session import PickableInferenceSession
 
 
 class PyannoteONNX:
     def __init__(self):
         # segmentation-3.0 classes:
@@ -90,16 +89,17 @@
         diffs = np.sum(
             np.abs(np.sum(np.array(perms)[:, : x.shape[0], :] - x, axis=1)), axis=1
         )
         return perms[np.argmin(diffs)]
 
     def __call__(self, x, step=5.0, return_chunk=False):
         step = int(step * self.sample_rate)
-        # overlap: [0.5 * duration, 0.9 * duration]
+        # step: [0.5 * duration, 0.9 * duration]
         step = max(min(step, 0.9 * self.duration // 10), self.duration // 2)
+        # overlap: [0.1 * duration, 0.5 * duration]
         overlap = self.sample2frame(self.duration - step)
         overlap_chunk = np.zeros((overlap, self.num_classes))
         windows = list(self.sliding_window(x, self.duration, step))
         for idx, (window_size, window) in enumerate(windows):
             ort_outs = np.exp(
                 self.session.run(None, {"input": window[None, None, :]})[0][0]
             )
@@ -207,19 +207,20 @@
         speeches: list of dicts
             list containing ends and beginnings of speech chunks (samples or seconds
             based on return_seconds)
         """
         wav, sr = librosa.load(wav_path, sr=self.sample_rate)
         speech_pad_samples = sr * speech_pad_ms // 1000
 
-        original_wav = wav
-        sample_rate = librosa.get_samplerate(wav_path)
-        if sample_rate != self.sample_rate:
+        sample_rate = sf.info(wav_path).samplerate
+        if sample_rate == self.sample_rate:
+            original_wav = wav
+        else:
             # load the wav with original sample rate for saving
-            original_wav, _ = librosa.load(wav_path, sr=sample_rate)
+            original_wav, _ = sf.read(wav_path)
         fn = partial(
             self.process_segment,
             wav=original_wav,
             sample_rate=sample_rate,
             save_path=save_path,
             flat_layout=flat_layout,
             speech_pad_samples=speech_pad_samples,
```

### Comparing `pyannote-onnx-0.0.3/pyannote_onnx/segmentation-3.0.onnx` & `pyannote-onnx-0.0.4/pyannote_onnx/segmentation-3.0.onnx`

 * *Files identical despite different names*

### Comparing `pyannote-onnx-0.0.3/pyannote_onnx.egg-info/PKG-INFO` & `pyannote-onnx-0.0.4/pyannote_onnx.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 Metadata-Version: 2.1
 Name: pyannote-onnx
-Version: 0.0.3
+Version: 0.0.4
 Summary: Pyannote ONNX
 Home-page: https://github.com/pengzhendong/pyannote-onnx
 Author: Zhendong Peng
 Author-email: pzd17@tsinghua.org.cn
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: click
-Requires-Dist: librosa
-Requires-Dist: numpy
-Requires-Dist: onnxruntime
-Requires-Dist: soundfile
 
 # Speaker Diarization
 
 > [pyannote-audio](https://github.com/pyannote/pyannote-audio) is an open-source toolkit written in Python for speaker diarization.
 
 `pyannote-onnx` is used to convert the [pretrained model](https://huggingface.co/pyannote/segmentation-3.0) defined in PyTorch into the ONNX format and then run it with [ONNX Runtime](https://github.com/microsoft/onnxruntime) (in C++ or Python).
 
@@ -33,7 +30,9 @@
 ```bash
 $ pip install torch onnx https://github.com/pyannote/pyannote-audio/archive/refs/heads/develop.zip
 $ python export_onnx.py pytorch_model.bin segmentation-3.0.onnx
 
 $ pip install -r requirements.txt
 $ python main.py data/test_16k.wav
 ```
+
+
```

### Comparing `pyannote-onnx-0.0.3/setup.py` & `pyannote-onnx-0.0.4/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,35 +12,32 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import os
 from setuptools import setup, find_packages
 
 
-with open("README.md", encoding="utf8") as fin:
-    long_description = fin.read()
-
-with open("requirements.txt", encoding="utf-8") as f:
+with open("requirements.txt", encoding="utf8") as f:
     requirements = f.readlines()
 
 setup(
     name="pyannote-onnx",
-    version=os.getenv("BUILD_VERSION") or "0.0.3",
+    version=open("VERSION", encoding="utf8").read(),
     author="Zhendong Peng",
     author_email="pzd17@tsinghua.org.cn",
-    long_description=long_description,
+    long_description=open("README.md", encoding="utf8").read(),
     long_description_content_type="text/markdown",
     description="Pyannote ONNX",
     url="https://github.com/pengzhendong/pyannote-onnx",
     packages=find_packages(),
     include_package_data=True,
     install_requires=requirements,
     entry_points={
         "console_scripts": [
-            "diarization = main:main",
+            "diarize = pyannote_onnx.cli:main",
         ]
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
         "Topic :: Scientific/Engineering",
     ],
```


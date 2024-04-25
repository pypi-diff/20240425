# Comparing `tmp/fasttrackpy-0.4.3.tar.gz` & `tmp/fasttrackpy-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fasttrackpy-0.4.3.tar", max compression
+gzip compressed data, was "fasttrackpy-0.4.4.tar", max compression
```

## Comparing `fasttrackpy-0.4.3.tar` & `fasttrackpy-0.4.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1072 2023-11-15 22:25:59.747254 fasttrackpy-0.4.3/LICENSE
--rw-r--r--   0        0        0      889 2024-03-14 21:53:55.296369 fasttrackpy-0.4.3/README.md
--rw-r--r--   0        0        0     1746 2024-04-15 14:22:29.506059 fasttrackpy-0.4.3/pyproject.toml
--rw-r--r--   0        0        0      629 2023-11-28 04:58:49.197727 fasttrackpy-0.4.3/src/fasttrackpy/__init__.py
--rw-r--r--   0        0        0    17445 2024-04-07 18:41:19.124172 fasttrackpy-0.4.3/src/fasttrackpy/cli.py
--rw-r--r--   0        0        0        0 2023-11-15 22:25:59.749448 fasttrackpy-0.4.3/src/fasttrackpy/patterns/__init__.py
--rw-r--r--   0        0        0     6223 2024-03-22 21:32:36.644068 fasttrackpy-0.4.3/src/fasttrackpy/patterns/audio_textgrid.py
--rw-r--r--   0        0        0     7550 2024-03-22 21:32:36.644304 fasttrackpy-0.4.3/src/fasttrackpy/patterns/corpus.py
--rw-r--r--   0        0        0     7249 2024-03-22 21:32:36.644532 fasttrackpy-0.4.3/src/fasttrackpy/patterns/just_audio.py
--rw-r--r--   0        0        0        0 2023-11-15 22:11:10.457070 fasttrackpy-0.4.3/src/fasttrackpy/processors/__init__.py
--rw-r--r--   0        0        0      844 2023-11-15 22:25:59.749799 fasttrackpy-0.4.3/src/fasttrackpy/processors/aggs.py
--rw-r--r--   0        0        0     1753 2023-11-15 22:25:59.749908 fasttrackpy-0.4.3/src/fasttrackpy/processors/losses.py
--rw-r--r--   0        0        0    12701 2024-04-15 14:21:09.838269 fasttrackpy-0.4.3/src/fasttrackpy/processors/outputs.py
--rw-r--r--   0        0        0     3285 2024-04-15 14:21:09.838641 fasttrackpy-0.4.3/src/fasttrackpy/processors/smoothers.py
--rw-r--r--   0        0        0        0 2023-11-27 01:47:20.549781 fasttrackpy-0.4.3/src/fasttrackpy/resources/config.yml
--rw-r--r--   0        0        0    19345 2024-03-22 21:32:36.644915 fasttrackpy-0.4.3/src/fasttrackpy/tracks.py
--rw-r--r--   0        0        0     2467 1970-01-01 00:00:00.000000 fasttrackpy-0.4.3/setup.py
--rw-r--r--   0        0        0     2250 1970-01-01 00:00:00.000000 fasttrackpy-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-11-15 22:25:59.747254 fasttrackpy-0.4.4/LICENSE
+-rw-r--r--   0        0        0      889 2024-03-14 21:53:55.296369 fasttrackpy-0.4.4/README.md
+-rw-r--r--   0        0        0     1746 2024-04-25 20:32:54.435824 fasttrackpy-0.4.4/pyproject.toml
+-rw-r--r--   0        0        0      629 2023-11-28 04:58:49.197727 fasttrackpy-0.4.4/src/fasttrackpy/__init__.py
+-rw-r--r--   0        0        0    17458 2024-04-25 20:32:54.436009 fasttrackpy-0.4.4/src/fasttrackpy/cli.py
+-rw-r--r--   0        0        0        0 2023-11-15 22:25:59.749448 fasttrackpy-0.4.4/src/fasttrackpy/patterns/__init__.py
+-rw-r--r--   0        0        0     6223 2024-03-22 21:32:36.644068 fasttrackpy-0.4.4/src/fasttrackpy/patterns/audio_textgrid.py
+-rw-r--r--   0        0        0     7550 2024-03-22 21:32:36.644304 fasttrackpy-0.4.4/src/fasttrackpy/patterns/corpus.py
+-rw-r--r--   0        0        0     7249 2024-03-22 21:32:36.644532 fasttrackpy-0.4.4/src/fasttrackpy/patterns/just_audio.py
+-rw-r--r--   0        0        0        0 2023-11-15 22:11:10.457070 fasttrackpy-0.4.4/src/fasttrackpy/processors/__init__.py
+-rw-r--r--   0        0        0      844 2023-11-15 22:25:59.749799 fasttrackpy-0.4.4/src/fasttrackpy/processors/aggs.py
+-rw-r--r--   0        0        0     1753 2023-11-15 22:25:59.749908 fasttrackpy-0.4.4/src/fasttrackpy/processors/losses.py
+-rw-r--r--   0        0        0    13195 2024-04-25 20:32:54.436214 fasttrackpy-0.4.4/src/fasttrackpy/processors/outputs.py
+-rw-r--r--   0        0        0     3285 2024-04-15 14:21:09.838641 fasttrackpy-0.4.4/src/fasttrackpy/processors/smoothers.py
+-rw-r--r--   0        0        0        0 2023-11-27 01:47:20.549781 fasttrackpy-0.4.4/src/fasttrackpy/resources/config.yml
+-rw-r--r--   0        0        0    20530 2024-04-25 20:32:54.436369 fasttrackpy-0.4.4/src/fasttrackpy/tracks.py
+-rw-r--r--   0        0        0     2467 1970-01-01 00:00:00.000000 fasttrackpy-0.4.4/setup.py
+-rw-r--r--   0        0        0     2250 1970-01-01 00:00:00.000000 fasttrackpy-0.4.4/PKG-INFO
```

### Comparing `fasttrackpy-0.4.3/LICENSE` & `fasttrackpy-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `fasttrackpy-0.4.3/README.md` & `fasttrackpy-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `fasttrackpy-0.4.3/pyproject.toml` & `fasttrackpy-0.4.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fasttrackpy"
-version = "0.4.3"
+version = "0.4.4"
 description = "A python implementation of FastTrack"
 authors = [
     "JoFrhwld <JoFrhwld@gmail.com>",
     "santiagobarreda <sbarreda@ucdavis.edu>"
 ]
 license = "MIT"
 readme = "README.md"
```

### Comparing `fasttrackpy-0.4.3/src/fasttrackpy/__init__.py` & `fasttrackpy-0.4.4/src/fasttrackpy/__init__.py`

 * *Files identical despite different names*

### Comparing `fasttrackpy-0.4.3/src/fasttrackpy/cli.py` & `fasttrackpy-0.4.4/src/fasttrackpy/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,15 +141,15 @@
         type=click.Choice(["winner", "all"]), 
         default="winner",
         help = "Whether to save just the winner, or all candidates."\
                " Defaults to 'winner'"
     ),
     cloup.option(
         "--data-output", 
-        type=click.Choice(["formants", "param"]), 
+        type=click.Choice(["formants", "param", "log_param"]), 
         default="formants",
         help = "Whether to save the formant data, "\
                "or smoothing parameter data."\
                " Defaults to 'formants'."   
     ),
     cloup.option(
         "--separate-output",
```

### Comparing `fasttrackpy-0.4.3/src/fasttrackpy/patterns/audio_textgrid.py` & `fasttrackpy-0.4.4/src/fasttrackpy/patterns/audio_textgrid.py`

 * *Files identical despite different names*

### Comparing `fasttrackpy-0.4.3/src/fasttrackpy/patterns/corpus.py` & `fasttrackpy-0.4.4/src/fasttrackpy/patterns/corpus.py`

 * *Files identical despite different names*

### Comparing `fasttrackpy-0.4.3/src/fasttrackpy/patterns/just_audio.py` & `fasttrackpy-0.4.4/src/fasttrackpy/patterns/just_audio.py`

 * *Files identical despite different names*

### Comparing `fasttrackpy-0.4.3/src/fasttrackpy/processors/aggs.py` & `fasttrackpy-0.4.4/src/fasttrackpy/processors/aggs.py`

 * *Files identical despite different names*

### Comparing `fasttrackpy-0.4.3/src/fasttrackpy/processors/losses.py` & `fasttrackpy-0.4.4/src/fasttrackpy/processors/losses.py`

 * *Files identical despite different names*

### Comparing `fasttrackpy-0.4.3/src/fasttrackpy/processors/outputs.py` & `fasttrackpy-0.4.4/src/fasttrackpy/processors/outputs.py`

 * *Files 3% similar despite different names*

```diff
@@ -96,14 +96,37 @@
         error = pl.lit(self.smooth_error)
     ).with_row_count(name = "param")
 
     param_df = add_metadata(self, param_df)
 
     return param_df
 
+def log_param_to_dataframe(self):
+    """Return data as a data frame
+
+    Returns:
+        (pl.DataFrame): A data frame
+    """
+
+    schema = [
+        f"F{x}" for x in
+        np.arange(self.log_parameters.shape[0])+1
+    ]
+    param_df = pl.DataFrame(
+        data = self.log_parameters,schema=schema
+    )
+
+    param_df = param_df.with_columns(
+        error = pl.lit(self.smooth_error)
+    ).with_row_count(name = "param")
+
+    param_df = add_metadata(self, param_df)
+
+    return param_df
+
 def get_big_df(self, output):
         all_df = [x.to_df(output = output) for x in self.candidates]
         all_df = [
             x.with_columns(
                 candidate = idx+1
             )
             for idx, x in enumerate(all_df)
```

### Comparing `fasttrackpy-0.4.3/src/fasttrackpy/processors/smoothers.py` & `fasttrackpy-0.4.4/src/fasttrackpy/processors/smoothers.py`

 * *Files identical despite different names*

### Comparing `fasttrackpy-0.4.3/src/fasttrackpy/tracks.py` & `fasttrackpy-0.4.4/src/fasttrackpy/tracks.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import parselmouth as pm
 import numpy as np
 from fasttrackpy.processors.smoothers import Smoother
 from fasttrackpy.processors.losses import Loss
 from fasttrackpy.processors.aggs import Agg
 from fasttrackpy.processors.outputs import formant_to_dataframe,\
                                            param_to_dataframe,\
+                                           log_param_to_dataframe,\
                                            get_big_df,\
                                            spectrogram,\
                                            candidate_spectrograms
 import matplotlib.pyplot as mp
 from aligned_textgrid import SequenceInterval
 from aligned_textgrid.sequences.tiers import TierGroup
 
@@ -148,19 +149,21 @@
             loss_fun=loss_fun,
             agg_fun=agg_fun
         )
         self.maximum_formant = maximum_formant
 
         self.formants, self.time_domain = self._track_formants()
         self.smoothed_list = self._smooth_formants()
+        self.smoothed_log_list = self._smooth_log_formants()
         self._file_name = None
         self._id = None
         self._group = None
         self._formant_df = None
         self._param_df = None
+        self._log_param_df = None
         self._interval = None
 
     def __repr__(self):
         return f"A formant track object. {self.formants.shape}"
 
     def _track_formants(self):
         formant_obj = self.sound.to_formant_burg(
@@ -186,26 +189,40 @@
 
     def _smooth_formants(self):
         smoothed_list = [
           self.smoother.smooth(x)
             for x in self.formants
         ]
         return smoothed_list
+    
+    def _smooth_log_formants(self):
+        smoothed_list = [
+            self.smoother.smooth(x)
+            for x in np.log(self.formants)
+        ]
+
+        return smoothed_list
 
     @property
     def smoothed_formants(self):
         return np.array(
             [x.smoothed for x in self.smoothed_list]
         )
 
     @property
     def parameters(self):
         return np.array(
             [x.params for x in self.smoothed_list]
         )
+    
+    @property
+    def log_parameters(self):
+        return np.array([
+            x.params for x in self.smoothed_log_list
+        ])
 
     @property
     def smooth_error(self):
         msqe =  self.loss_fun.calculate_loss(
             self.formants[0:self.n_formants],
             self.smoothed_formants[0:self.n_formants]
         )
@@ -251,43 +268,53 @@
         if isinstance(interval.within, TierGroup):
             return interval.within.name
 
         return self.__get_group(interval.within)
 
     def to_df(
             self,
-            output:Literal["formants", "param"] = "formants"
+            output:Literal["formants", "param", "log_param"] = "formants"
             ) -> pl.DataFrame:
         """Output either the formant values or the formant smoothing parameters \
         as a polars dataframe
 
         Args:
-            output (Literal['formants', 'param'], optional): Whether
+            output (Literal['formants', 'param', 'log_param'], optional): Whether
                 to output the formants or the smoothing parameters.
                 Defaults to "formants".
 
         Returns:
             (pl.DataFrame): A `polars.DataFrame`
         """
         if output == "formants"\
               and not isinstance(self._formant_df, pl.DataFrame):
             df =  formant_to_dataframe(self)
             self._formant_df = df
             return df
         if output == "formants":
             return self._formant_df
+
         if output == "param"\
             and not isinstance(self._param_df, pl.DataFrame):
             df =  param_to_dataframe(self)
             self._param_df = df
             return df
         if output == "param":
             return self._param_df
+        
+        if output == "log_param"\
+            and not isinstance(self._log_param_df, pl.DataFrame):
+            df = log_param_to_dataframe(self)
+            self._log_param_df = df
+            return df
+        
+        if output == "log_param":
+            return self._log_param_df
 
-        raise ValueError("output must be either 'formants' or 'param'")
+        raise ValueError("output must be 'formants', 'param', or 'log_param'")
 
     def spectrogram(self, **kwargs):
         """
         This will plot the spectrogram and formant tracks
         of a single candidate track. If a `file_name` is 
         provided, it will save the plot to disk.
 
@@ -418,14 +445,15 @@
         )
         self._file_name = None
         self._id = None
         self._label = None
         self._group = None
         self._formant_df = None
         self._param_df = None
+        self._log_param_df = None
         self._interval = None
 
         to_process = [
             {
                 "samples": self.samples,
                 "sampling_frequency": self.sampling_frequency,
                 "xmin": self.xmin,
@@ -500,22 +528,22 @@
         self.group = self.__get_group(interval)
         for c in self.candidates:
             c.interval = interval
 
     def to_df(
             self,
             which: Literal["winner", "all"] = "winner",
-            output: Literal["formants", "param"] = "formants"
+            output: Literal["formants", "param", "log_param"] = "formants"
             ) -> pl.DataFrame:
         """Return a polars dataframe of the candidate tracks
 
         Args:
             which (Literal['winner', 'all'], optional): Return just the winner
                 track data, or all candidates. Defaults to "winner".
-            output (Literal['formants', 'param'], optional): Whether
+            output (Literal['formants', 'param', 'log_param'], optional): Whether
                 to output the formants or the smoothing parameters.
                 Defaults to "formants".
 
         Returns:
             (pl.DataFrame): A `polars.DataFrame`
         """
         if which == "winner":
@@ -534,14 +562,23 @@
             and not isinstance(self._param_df, pl.DataFrame):
             big_df = get_big_df(self, output=output)
             self._param_df = big_df
             return big_df
 
         if output == "param":
             return self._param_df
+        
+        if output == "log_param"\
+            and not isinstance(self._log_param_df, pl.DataFrame):
+            big_df = get_big_df(self, output=output)
+            self._log_param_df = big_df
+            return big_df
+
+        if output == "log_param":
+            return self._log_param_df        
 
     def spectrograms(self, **kwargs):
         """ 
         This will plot a grid of the candidate formant
         tracks and their spectrograms. If a `file_name`
         is provided, it will save the plot to disk.
```

### Comparing `fasttrackpy-0.4.3/setup.py` & `fasttrackpy-0.4.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
  ':sys_platform == "win32"': ['python-magic-bin>=0.4.14,<0.5.0']}
 
 entry_points = \
 {'console_scripts': ['fasttrack = fasttrackpy.cli:fasttrack']}
 
 setup_kwargs = {
     'name': 'fasttrackpy',
-    'version': '0.4.3',
+    'version': '0.4.4',
     'description': 'A python implementation of FastTrack',
     'long_description': '# FastTrackPy\n[![PyPI](https://img.shields.io/pypi/v/fasttrackpy)](https://pypi.org/project/fasttrackpy/)\n[![Python CI](https://github.com/JoFrhwld/fasttrackpy/actions/workflows/test-and-run.yml/badge.svg)](https://github.com/JoFrhwld/fasttrackpy/actions/workflows/test-and-run.yml) [![codecov](https://codecov.io/gh/FastTrackiverse/fasttrackpy/graph/badge.svg?token=GOAWY4B5C8)](https://codecov.io/gh/FastTrackiverse/fasttrackpy) <a href="https://codeclimate.com/github/JoFrhwld/fasttrackpy/maintainability"><img src="https://api.codeclimate.com/v1/badges/6725fded174b21a3c59f/maintainability" /></a> [![DOI](https://zenodo.org/badge/580169086.svg)](https://zenodo.org/badge/latestdoi/580169086)\n\n\nGoal: A FastTrack python implementation with importable modules\n\n## Installation\n\n```bash\npip install fasttrackpy\n```\n\n## Usage\n\n```bash\nfasttrack --file audio.wav --output formants.csv\n```\n',
     'author': 'JoFrhwld',
     'author_email': 'JoFrhwld@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://fasttrackiverse.github.io/fasttrackpy/',
```

#### html2text {}

```diff
@@ -7,15 +7,15 @@
 parselmouth>=0.4.3,<0.5.0', 'pytest-cov>=4.1.0,<5.0.0', 'pytest>=7.4.3,<8.0.0',
 'pyyaml>=6.0.1,<7.0.0', 'tqdm>=4.66.1,<5.0.0'] extras_require = \ {':
 python_version >= "3.10" and python_version < "3.12"': ['scipy>=1.11.3,<2.0.0',
 'numpy>=1.26.1,<2.0.0'], ':sys_platform != "win32"': ['python-
 magic>=0.4.27,<0.5.0'], ':sys_platform == "win32"': ['python-magic-
 bin>=0.4.14,<0.5.0']} entry_points = \ {'console_scripts': ['fasttrack =
 fasttrackpy.cli:fasttrack']} setup_kwargs = { 'name': 'fasttrackpy', 'version':
-'0.4.3', 'description': 'A python implementation of FastTrack',
+'0.4.4', 'description': 'A python implementation of FastTrack',
 'long_description': '# FastTrackPy\n[![PyPI](https://img.shields.io/pypi/v/
 fasttrackpy)](https://pypi.org/project/fasttrackpy/)\n[![Python CI](https://
 github.com/JoFrhwld/fasttrackpy/actions/workflows/test-and-run.yml/badge.svg)]
 (https://github.com/JoFrhwld/fasttrackpy/actions/workflows/test-and-run.yml) [!
 [codecov](https://codecov.io/gh/FastTrackiverse/fasttrackpy/graph/
 badge.svg?token=GOAWY4B5C8)](https://codecov.io/gh/FastTrackiverse/fasttrackpy)
 _[_h_t_t_p_s_:_/_/_a_p_i_._c_o_d_e_c_l_i_m_a_t_e_._c_o_m_/_v_1_/_b_a_d_g_e_s_/_6_7_2_5_f_d_e_d_1_7_4_b_2_1_a_3_c_5_9_f_/_m_a_i_n_t_a_i_n_a_b_i_l_i_t_y_][!
```

### Comparing `fasttrackpy-0.4.3/PKG-INFO` & `fasttrackpy-0.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fasttrackpy
-Version: 0.4.3
+Version: 0.4.4
 Summary: A python implementation of FastTrack
 Home-page: https://fasttrackiverse.github.io/fasttrackpy/
 License: MIT
 Author: JoFrhwld
 Author-email: JoFrhwld@gmail.com
 Requires-Python: >=3.10,<3.12
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fasttrackpy Version: 0.4.3 Summary: A python
+Metadata-Version: 2.1 Name: fasttrackpy Version: 0.4.4 Summary: A python
 implementation of FastTrack Home-page: https://fasttrackiverse.github.io/
 fasttrackpy/ License: MIT Author: JoFrhwld Author-email: JoFrhwld@gmail.com
 Requires-Python: >=3.10,<3.12 Classifier: License :: OSI Approved :: MIT
 License Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aligned-textgrid (>=0.6.2,<0.7.0) Requires-Dist: click
 (>=8.1.7,<9.0.0) Requires-Dist: cloup (>=3.0.3,<4.0.0) Requires-Dist: joblib
```


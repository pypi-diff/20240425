# Comparing `tmp/mutwo.ekmelily-0.8.1.tar.gz` & `tmp/mutwo_ekmelily-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mutwo.ekmelily-0.8.1.tar", last modified: Thu Oct 19 22:15:38 2023, max compression
+gzip compressed data, was "mutwo_ekmelily-0.9.0.tar", last modified: Thu Apr 25 08:28:38 2024, max compression
```

## Comparing `mutwo.ekmelily-0.8.1.tar` & `mutwo_ekmelily-0.9.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-10-19 22:15:38.581422 mutwo.ekmelily-0.8.1/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    35149 2023-10-19 22:15:26.000000 mutwo.ekmelily-0.8.1/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1378 2023-10-19 22:15:38.581422 mutwo.ekmelily-0.8.1/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      801 2023-10-19 22:15:26.000000 mutwo.ekmelily-0.8.1/README.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-10-19 22:15:38.577422 mutwo.ekmelily-0.8.1/mutwo/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-10-19 22:15:38.581422 mutwo.ekmelily-0.8.1/mutwo/ekmelily_converters/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      167 2023-10-19 22:15:26.000000 mutwo.ekmelily-0.8.1/mutwo/ekmelily_converters/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2291 2023-10-19 22:15:26.000000 mutwo.ekmelily-0.8.1/mutwo/ekmelily_converters/configurations.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10825 2023-10-19 22:15:26.000000 mutwo.ekmelily-0.8.1/mutwo/ekmelily_converters/constants.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    37702 2023-10-19 22:15:26.000000 mutwo.ekmelily-0.8.1/mutwo/ekmelily_converters/ekmelily.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-10-19 22:15:38.581422 mutwo.ekmelily-0.8.1/mutwo/ekmelily_version/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      146 2023-10-19 22:15:26.000000 mutwo.ekmelily-0.8.1/mutwo/ekmelily_version/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-10-19 22:15:38.581422 mutwo.ekmelily-0.8.1/mutwo.ekmelily.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1378 2023-10-19 22:15:38.000000 mutwo.ekmelily-0.8.1/mutwo.ekmelily.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      424 2023-10-19 22:15:38.000000 mutwo.ekmelily-0.8.1/mutwo.ekmelily.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-10-19 22:15:38.000000 mutwo.ekmelily-0.8.1/mutwo.ekmelily.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       77 2023-10-19 22:15:38.000000 mutwo.ekmelily-0.8.1/mutwo.ekmelily.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        6 2023-10-19 22:15:38.000000 mutwo.ekmelily-0.8.1/mutwo.ekmelily.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      200 2023-10-19 22:15:26.000000 mutwo.ekmelily-0.8.1/pyproject.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-10-19 22:15:38.581422 mutwo.ekmelily-0.8.1/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1118 2023-10-19 22:15:26.000000 mutwo.ekmelily-0.8.1/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-25 08:28:38.828992 mutwo_ekmelily-0.9.0/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    35149 2024-04-25 08:28:24.000000 mutwo_ekmelily-0.9.0/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1378 2024-04-25 08:28:38.828992 mutwo_ekmelily-0.9.0/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      801 2024-04-25 08:28:24.000000 mutwo_ekmelily-0.9.0/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-25 08:28:38.824992 mutwo_ekmelily-0.9.0/mutwo/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-25 08:28:38.824992 mutwo_ekmelily-0.9.0/mutwo/ekmelily_converters/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      167 2024-04-25 08:28:24.000000 mutwo_ekmelily-0.9.0/mutwo/ekmelily_converters/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2291 2024-04-25 08:28:24.000000 mutwo_ekmelily-0.9.0/mutwo/ekmelily_converters/configurations.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10807 2024-04-25 08:28:24.000000 mutwo_ekmelily-0.9.0/mutwo/ekmelily_converters/constants.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    37672 2024-04-25 08:28:24.000000 mutwo_ekmelily-0.9.0/mutwo/ekmelily_converters/ekmelily.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-25 08:28:38.824992 mutwo_ekmelily-0.9.0/mutwo/ekmelily_version/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      146 2024-04-25 08:28:24.000000 mutwo_ekmelily-0.9.0/mutwo/ekmelily_version/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-25 08:28:38.824992 mutwo_ekmelily-0.9.0/mutwo.ekmelily.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1378 2024-04-25 08:28:38.000000 mutwo_ekmelily-0.9.0/mutwo.ekmelily.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      424 2024-04-25 08:28:38.000000 mutwo_ekmelily-0.9.0/mutwo.ekmelily.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-25 08:28:38.000000 mutwo_ekmelily-0.9.0/mutwo.ekmelily.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       77 2024-04-25 08:28:38.000000 mutwo_ekmelily-0.9.0/mutwo.ekmelily.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        6 2024-04-25 08:28:38.000000 mutwo_ekmelily-0.9.0/mutwo.ekmelily.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      200 2024-04-25 08:28:24.000000 mutwo_ekmelily-0.9.0/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-04-25 08:28:38.828992 mutwo_ekmelily-0.9.0/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1118 2024-04-25 08:28:24.000000 mutwo_ekmelily-0.9.0/setup.py
```

### Comparing `mutwo.ekmelily-0.8.1/LICENSE` & `mutwo_ekmelily-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mutwo.ekmelily-0.8.1/PKG-INFO` & `mutwo_ekmelily-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: mutwo.ekmelily
-Version: 0.8.1
+Version: 0.9.0
 Summary: ekmelily extension for event based framework for generative art
 Home-page: https://github.com/mutwo-org/mutwo.ekmelily
 Author: Levin Eric Zimmermann
 Author-email: levin.eric.zimmermann@posteo.eu
 License: GPL
 Project-URL: Documentation, https://mutwo-org.github.io
 Requires-Python: >=3.10, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: mutwo.core<2.0.0,>=1.0.0
-Requires-Dist: mutwo.music<1.0.0,>=0.19.0
+Requires-Dist: mutwo.core<3.0.0,>=2.0.0
+Requires-Dist: mutwo.music<1.0.0,>=0.27.0
 Provides-Extra: testing
 Requires-Dist: pytest>=7.1.1; extra == "testing"
 
 # mutwo.ekmelily
 
 [![Build Status](https://circleci.com/gh/mutwo-org/mutwo.ekmelily.svg?style=shield)](https://circleci.com/gh/mutwo-org/mutwo.ekmelily)
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
```

### Comparing `mutwo.ekmelily-0.8.1/README.md` & `mutwo_ekmelily-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `mutwo.ekmelily-0.8.1/mutwo/ekmelily_converters/configurations.py` & `mutwo_ekmelily-0.9.0/mutwo/ekmelily_converters/configurations.py`

 * *Files identical despite different names*

### Comparing `mutwo.ekmelily-0.8.1/mutwo/ekmelily_converters/constants.py` & `mutwo_ekmelily-0.9.0/mutwo/ekmelily_converters/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -324,15 +324,15 @@
         -fractions.Fraction(1, 2)
     ]: -50,
 }
 """Mapping of tempered accidental name to cent deviation."""
 
 
 PYTHAGOREAN_ACCIDENTAL_CENT_DEVIATION_SIZE = round(
-    (music_parameters.JustIntonationPitch((0, 7)).normalize(mutate=False).interval), 2  # type: ignore
+    (music_parameters.JustIntonationPitch((0, 7)).normalize().cents), 2  # type: ignore
 )
 """Step in cents for one pythagorean accidental (# or b)."""
 
 PYTHAGOREAN_ACCIDENTAL_TO_CENT_DEVIATION_DICT = {
     music_parameters.constants.PITCH_CLASS_MODIFICATION_TO_ACCIDENTAL_NAME_DICT[
         fractions.Fraction(0, 1)
     ]: 0,
@@ -350,15 +350,15 @@
         -fractions.Fraction(2, 1)
     ]: -2
     * PYTHAGOREAN_ACCIDENTAL_CENT_DEVIATION_SIZE,
 }
 """Step in cents mapping for each pythagorean accidental (# or b)."""
 
 DIFFERENCE_BETWEEN_PYTHAGOREAN_AND_TEMPERED_FIFTH = (
-    music_parameters.JustIntonationPitch("3/2").interval - 700
+    music_parameters.JustIntonationPitch("3/2").cents - 700
 )
 """The difference in cents between a just fifth (3/2) and
 a 12-EDO fifth. This constant is used in
 :class:`~mutwo.ekmelily_converters.HEJIEkmelilyTuningFileConverter`.
 """
 
 # Cleanup
```

### Comparing `mutwo.ekmelily-0.8.1/mutwo/ekmelily_converters/ekmelily.py` & `mutwo_ekmelily-0.9.0/mutwo/ekmelily_converters/ekmelily.py`

 * *Files 1% similar despite different names*

```diff
@@ -491,31 +491,31 @@
     :param otonality_indicator: String which indicates that the
         respective prime alteration is otonal. See
         :const:`~mutwo.ekmelily_converters.configurations.DEFAULT_OTONALITY_INDICATOR`
         for the default value.
     :type otonality_indicator: str, optional
     :param utonality_indicator: String which indicates that the
         respective prime alteration is utonal. See
-        :const:`~mutwo.ekmelily_converters.configurations.DEFAULT_OTONALITY_INDICATOR`
+        :const:`~mutwo.ekmelily_converters.configurations.DEFAULT_UTONALITY_INDICATOR`
         for the default value.
     :type utonality_indicator: str, optional
     :param exponent_to_exponent_indicator: Function to convert the
         exponent of a prime number to string which indicates the respective
         exponent. See
         :func:`~mutwo.ekmelily_converters.configurations.DEFAULT_EXPONENT_TO_EXPONENT_INDICATOR`
         for the default function.
     :type exponent_to_exponent_indicator: typing.Callable[[int], str], optional
     :param tempered_pitch_indicator: String which indicates that the
         respective accidental is tempered (12 EDO). See
         :const:`~mutwo.ekmelily_converters.configurations.DEFAULT_TEMPERED_PITCH_INDICATOR`
         for the default value.
     :type tempered_pitch_indicator: str, optional
     :param set_microtonal_tuning: If set to ``False`` the converter won't apply any
-        microtonal music_parameters. In this case all chromatic music_parameters will return normal
-        12EDO music_parameters. Default to ``True``.
+        microtonal pitches. In this case all chromatic pitches will return normal
+        12EDO pitches. Default to ``True``.
     :type set_microtonal_tuning: bool
     """
 
     def __init__(
         self,
         path: str = None,
         prime_to_highest_allowed_exponent: typing.Optional[dict[int, int]] = None,
@@ -705,15 +705,15 @@
             prime_to_heji_accidental_name[prime],
             exponent_to_exponent_indicator(abs(exponent) - 1),
         )
 
         cents_deviation = music_parameters.JustIntonationPitch(
             music_parameters.configurations.DEFAULT_PRIME_TO_COMMA_DICT[prime].ratio
             ** exponent
-        ).interval
+        ).cents
         return accidental_name, glyph, cents_deviation
 
     @staticmethod
     def _make_higher_prime_accidental(
         pythagorean_accidental: str,
         pythagorean_accidental_cents_deviation: float,
         exponents: tuple[int, ...],
```

### Comparing `mutwo.ekmelily-0.8.1/mutwo.ekmelily.egg-info/PKG-INFO` & `mutwo_ekmelily-0.9.0/mutwo.ekmelily.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: mutwo.ekmelily
-Version: 0.8.1
+Version: 0.9.0
 Summary: ekmelily extension for event based framework for generative art
 Home-page: https://github.com/mutwo-org/mutwo.ekmelily
 Author: Levin Eric Zimmermann
 Author-email: levin.eric.zimmermann@posteo.eu
 License: GPL
 Project-URL: Documentation, https://mutwo-org.github.io
 Requires-Python: >=3.10, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: mutwo.core<2.0.0,>=1.0.0
-Requires-Dist: mutwo.music<1.0.0,>=0.19.0
+Requires-Dist: mutwo.core<3.0.0,>=2.0.0
+Requires-Dist: mutwo.music<1.0.0,>=0.27.0
 Provides-Extra: testing
 Requires-Dist: pytest>=7.1.1; extra == "testing"
 
 # mutwo.ekmelily
 
 [![Build Status](https://circleci.com/gh/mutwo-org/mutwo.ekmelily.svg?style=shield)](https://circleci.com/gh/mutwo-org/mutwo.ekmelily)
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
```

### Comparing `mutwo.ekmelily-0.8.1/setup.py` & `mutwo_ekmelily-0.9.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,13 +25,13 @@
     packages=[
         package
         for package in setuptools.find_namespace_packages(include=["mutwo.*"])
         if package[:5] != "tests"
     ],
     setup_requires=[],
     install_requires=[
-        "mutwo.core>=1.0.0, <2.0.0",
-        "mutwo.music>=0.19.0, <1.0.0",
+        "mutwo.core>=2.0.0, <3.0.0",
+        "mutwo.music>=0.27.0, <1.0.0",
     ],
     extras_require=extras_require,
     python_requires=">=3.10, <4",
 )
```


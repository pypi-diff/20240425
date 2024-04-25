# Comparing `tmp/types-pyaudio-0.2.8.tar.gz` & `tmp/types-pyaudio-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-pyaudio-0.2.8.tar", last modified: Fri Jan  7 11:31:36 2022, max compression
+gzip compressed data, was "types-pyaudio-0.2.9.tar", last modified: Sun Jan 16 18:21:11 2022, max compression
```

## Comparing `types-pyaudio-0.2.8.tar` & `types-pyaudio-0.2.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-07 11:31:36.556038 types-pyaudio-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (121)      343 2022-01-07 11:31:36.000000 types-pyaudio-0.2.8/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)       21 2022-01-07 11:31:36.000000 types-pyaudio-0.2.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      859 2022-01-07 11:31:36.556038 types-pyaudio-0.2.8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-07 11:31:36.556038 types-pyaudio-0.2.8/pyaudio-stubs/
--rw-r--r--   0 runner    (1001) docker     (121)       81 2022-01-07 11:31:36.000000 types-pyaudio-0.2.8/pyaudio-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (121)     6372 2022-01-07 11:31:36.000000 types-pyaudio-0.2.8/pyaudio-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-01-07 11:31:36.556038 types-pyaudio-0.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1179 2022-01-07 11:31:36.000000 types-pyaudio-0.2.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-07 11:31:36.556038 types-pyaudio-0.2.8/types_pyaudio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      859 2022-01-07 11:31:36.000000 types-pyaudio-0.2.8/types_pyaudio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      236 2022-01-07 11:31:36.000000 types-pyaudio-0.2.8/types_pyaudio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-07 11:31:36.000000 types-pyaudio-0.2.8/types_pyaudio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-01-07 11:31:36.000000 types-pyaudio-0.2.8/types_pyaudio.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-16 18:21:11.639971 types-pyaudio-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (121)      412 2022-01-16 18:21:11.000000 types-pyaudio-0.2.9/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (121)       21 2022-01-16 18:21:11.000000 types-pyaudio-0.2.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)      859 2022-01-16 18:21:11.639971 types-pyaudio-0.2.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-16 18:21:11.639971 types-pyaudio-0.2.9/pyaudio-stubs/
+-rw-r--r--   0 runner    (1001) docker     (121)       81 2022-01-16 18:21:11.000000 types-pyaudio-0.2.9/pyaudio-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (121)     6024 2022-01-16 18:21:11.000000 types-pyaudio-0.2.9/pyaudio-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-01-16 18:21:11.639971 types-pyaudio-0.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1179 2022-01-16 18:21:11.000000 types-pyaudio-0.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-16 18:21:11.639971 types-pyaudio-0.2.9/types_pyaudio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)      859 2022-01-16 18:21:11.000000 types-pyaudio-0.2.9/types_pyaudio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      236 2022-01-16 18:21:11.000000 types-pyaudio-0.2.9/types_pyaudio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-16 18:21:11.000000 types-pyaudio-0.2.9/types_pyaudio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       14 2022-01-16 18:21:11.000000 types-pyaudio-0.2.9/types_pyaudio.egg-info/top_level.txt
```

### Comparing `types-pyaudio-0.2.8/PKG-INFO` & `types-pyaudio-0.2.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-pyaudio
-Version: 0.2.8
+Version: 0.2.9
 Summary: Typing stubs for pyaudio
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Typing :: Stubs Only
 Description-Content-Type: text/markdown
@@ -14,10 +14,10 @@
 This is a PEP 561 type stub package for the `pyaudio` package.
 It can be used by type-checking tools like mypy, PyCharm, pytype etc. to check code
 that uses `pyaudio`. The source for this package can be found at
 https://github.com/python/typeshed/tree/master/stubs/pyaudio. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/master/README.md for more details.
-This package was generated from typeshed commit `032e6ee90cbb938259a2aa2183966502de19108e`.
+This package was generated from typeshed commit `85318d1b215a32825fd4ecb7fa6466fe75f7c428`.
```

### Comparing `types-pyaudio-0.2.8/pyaudio-stubs/__init__.pyi` & `types-pyaudio-0.2.9/pyaudio-stubs/__init__.pyi`

 * *Files 21% similar despite different names*

```diff
@@ -1,72 +1,72 @@
 from typing import Callable, Mapping, Optional, Sequence, Union
 from typing_extensions import Final
 
-paFloat32: Final[int] = ...
-paInt32: Final[int] = ...
-paInt24: Final[int] = ...
-paInt16: Final[int] = ...
-paInt8: Final[int] = ...
-paUInt8: Final[int] = ...
-paCustomFormat: Final[int] = ...
-
-paInDevelopment: Final[int] = ...
-paDirectSound: Final[int] = ...
-paMME: Final[int] = ...
-paASIO: Final[int] = ...
-paSoundManager: Final[int] = ...
-paCoreAudio: Final[int] = ...
-paOSS: Final[int] = ...
-paALSA: Final[int] = ...
-paAL: Final[int] = ...
-paBeOS: Final[int] = ...
-paWDMKS: Final[int] = ...
-paJACK: Final[int] = ...
-paWASAPI: Final[int] = ...
-paNoDevice: Final[int] = ...
-
-paNoError: Final[int] = ...
-paNotInitialized: Final[int] = ...
-paUnanticipatedHostError: Final[int] = ...
-paInvalidChannelCount: Final[int] = ...
-paInvalidSampleRate: Final[int] = ...
-paInvalidDevice: Final[int] = ...
-paInvalidFlag: Final[int] = ...
-paSampleFormatNotSupported: Final[int] = ...
-paBadIODeviceCombination: Final[int] = ...
-paInsufficientMemory: Final[int] = ...
-paBufferTooBig: Final[int] = ...
-paBufferTooSmall: Final[int] = ...
-paNullCallback: Final[int] = ...
-paBadStreamPtr: Final[int] = ...
-paTimedOut: Final[int] = ...
-paInternalError: Final[int] = ...
-paDeviceUnavailable: Final[int] = ...
-paIncompatibleHostApiSpecificStreamInfo: Final[int] = ...
-paStreamIsStopped: Final[int] = ...
-paStreamIsNotStopped: Final[int] = ...
-paInputOverflowed: Final[int] = ...
-paOutputUnderflowed: Final[int] = ...
-paHostApiNotFound: Final[int] = ...
-paInvalidHostApi: Final[int] = ...
-paCanNotReadFromACallbackStream: Final[int] = ...
-paCanNotWriteToACallbackStream: Final[int] = ...
-paCanNotReadFromAnOutputOnlyStream: Final[int] = ...
-paCanNotWriteToAnInputOnlyStream: Final[int] = ...
-paIncompatibleStreamHostApi: Final[int] = ...
-
-paContinue: Final[int] = ...
-paComplete: Final[int] = ...
-paAbort: Final[int] = ...
-
-paInputUnderflow: Final[int] = ...
-paInputOverflow: Final[int] = ...
-paOutputUnderflow: Final[int] = ...
-paOutputOverflow: Final[int] = ...
-paPrimingOutput: Final[int] = ...
+paFloat32: Final[int]
+paInt32: Final[int]
+paInt24: Final[int]
+paInt16: Final[int]
+paInt8: Final[int]
+paUInt8: Final[int]
+paCustomFormat: Final[int]
+
+paInDevelopment: Final[int]
+paDirectSound: Final[int]
+paMME: Final[int]
+paASIO: Final[int]
+paSoundManager: Final[int]
+paCoreAudio: Final[int]
+paOSS: Final[int]
+paALSA: Final[int]
+paAL: Final[int]
+paBeOS: Final[int]
+paWDMKS: Final[int]
+paJACK: Final[int]
+paWASAPI: Final[int]
+paNoDevice: Final[int]
+
+paNoError: Final[int]
+paNotInitialized: Final[int]
+paUnanticipatedHostError: Final[int]
+paInvalidChannelCount: Final[int]
+paInvalidSampleRate: Final[int]
+paInvalidDevice: Final[int]
+paInvalidFlag: Final[int]
+paSampleFormatNotSupported: Final[int]
+paBadIODeviceCombination: Final[int]
+paInsufficientMemory: Final[int]
+paBufferTooBig: Final[int]
+paBufferTooSmall: Final[int]
+paNullCallback: Final[int]
+paBadStreamPtr: Final[int]
+paTimedOut: Final[int]
+paInternalError: Final[int]
+paDeviceUnavailable: Final[int]
+paIncompatibleHostApiSpecificStreamInfo: Final[int]
+paStreamIsStopped: Final[int]
+paStreamIsNotStopped: Final[int]
+paInputOverflowed: Final[int]
+paOutputUnderflowed: Final[int]
+paHostApiNotFound: Final[int]
+paInvalidHostApi: Final[int]
+paCanNotReadFromACallbackStream: Final[int]
+paCanNotWriteToACallbackStream: Final[int]
+paCanNotReadFromAnOutputOnlyStream: Final[int]
+paCanNotWriteToAnInputOnlyStream: Final[int]
+paIncompatibleStreamHostApi: Final[int]
+
+paContinue: Final[int]
+paComplete: Final[int]
+paAbort: Final[int]
+
+paInputUnderflow: Final[int]
+paInputOverflow: Final[int]
+paOutputUnderflow: Final[int]
+paOutputOverflow: Final[int]
+paPrimingOutput: Final[int]
 
 paMacCoreStreamInfo: PaMacCoreStreamInfo
 
 # Auxiliary types
 _ChannelMap = Sequence[int]
 _PaHostApiInfo = Mapping[str, Union[str, int]]
 _PaDeviceInfo = Mapping[str, Union[str, int, float]]
```

### Comparing `types-pyaudio-0.2.8/setup.py` & `types-pyaudio-0.2.9/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,19 +8,19 @@
 This is a PEP 561 type stub package for the `pyaudio` package.
 It can be used by type-checking tools like mypy, PyCharm, pytype etc. to check code
 that uses `pyaudio`. The source for this package can be found at
 https://github.com/python/typeshed/tree/master/stubs/pyaudio. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/master/README.md for more details.
-This package was generated from typeshed commit `032e6ee90cbb938259a2aa2183966502de19108e`.
+This package was generated from typeshed commit `85318d1b215a32825fd4ecb7fa6466fe75f7c428`.
 '''.lstrip()
 
 setup(name=name,
-      version="0.2.8",
+      version="0.2.9",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       install_requires=[],
       packages=['pyaudio-stubs'],
       package_data={'pyaudio-stubs': ['__init__.pyi', 'METADATA.toml']},
```

### Comparing `types-pyaudio-0.2.8/types_pyaudio.egg-info/PKG-INFO` & `types-pyaudio-0.2.9/types_pyaudio.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-pyaudio
-Version: 0.2.8
+Version: 0.2.9
 Summary: Typing stubs for pyaudio
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Typing :: Stubs Only
 Description-Content-Type: text/markdown
@@ -14,10 +14,10 @@
 This is a PEP 561 type stub package for the `pyaudio` package.
 It can be used by type-checking tools like mypy, PyCharm, pytype etc. to check code
 that uses `pyaudio`. The source for this package can be found at
 https://github.com/python/typeshed/tree/master/stubs/pyaudio. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/master/README.md for more details.
-This package was generated from typeshed commit `032e6ee90cbb938259a2aa2183966502de19108e`.
+This package was generated from typeshed commit `85318d1b215a32825fd4ecb7fa6466fe75f7c428`.
```


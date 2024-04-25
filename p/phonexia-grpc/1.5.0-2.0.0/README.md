# Comparing `tmp/phonexia_grpc-1.5.0.tar.gz` & `tmp/phonexia_grpc-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phonexia_grpc-1.5.0.tar", max compression
+gzip compressed data, was "phonexia_grpc-2.0.0.tar", max compression
```

## Comparing `phonexia_grpc-1.5.0.tar` & `phonexia_grpc-2.0.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0    11358 2024-03-28 07:32:32.729742 phonexia_grpc-1.5.0/LICENSE
--rw-r--r--   0        0        0     1908 2024-03-28 07:32:50.336990 phonexia_grpc-1.5.0/phonexia/grpc/common/core_pb2.py
--rw-r--r--   0        0        0     5414 2024-03-28 07:32:50.336990 phonexia_grpc-1.5.0/phonexia/grpc/common/core_pb2.pyi
--rw-r--r--   0        0        0      159 2024-03-28 07:32:50.336990 phonexia_grpc-1.5.0/phonexia/grpc/common/core_pb2_grpc.py
--rw-r--r--   0        0        0     1939 2024-03-28 07:32:50.336990 phonexia_grpc-1.5.0/phonexia/grpc/common/health_check_pb2.py
--rw-r--r--   0        0        0     3380 2024-03-28 07:32:50.336990 phonexia_grpc-1.5.0/phonexia/grpc/common/health_check_pb2.pyi
--rw-r--r--   0        0        0     4471 2024-03-28 07:32:50.336990 phonexia_grpc-1.5.0/phonexia/grpc/common/health_check_pb2_grpc.py
--rw-r--r--   0        0        0     1847 2024-03-28 07:32:50.336990 phonexia_grpc-1.5.0/phonexia/grpc/common/licensing_pb2.py
--rw-r--r--   0        0        0     3198 2024-03-28 07:32:50.336990 phonexia_grpc-1.5.0/phonexia/grpc/common/licensing_pb2.pyi
--rw-r--r--   0        0        0     2681 2024-03-28 07:32:50.336990 phonexia_grpc-1.5.0/phonexia/grpc/common/licensing_pb2_grpc.py
--rw-r--r--   0        0        0     2515 2024-03-28 07:32:50.336990 phonexia_grpc-1.5.0/phonexia/grpc/technologies/gender_identification/v1/gender_identification_pb2.py
--rw-r--r--   0        0        0     4509 2024-03-28 07:32:50.336990 phonexia_grpc-1.5.0/phonexia/grpc/technologies/gender_identification/v1/gender_identification_pb2.pyi
--rw-r--r--   0        0        0     3474 2024-03-28 07:32:50.336990 phonexia_grpc-1.5.0/phonexia/grpc/technologies/gender_identification/v1/gender_identification_pb2_grpc.py
--rw-r--r--   0        0        0     2905 2024-03-28 07:32:50.336990 phonexia_grpc-1.5.0/phonexia/grpc/technologies/speaker_diarization/v1/speaker_diarization_pb2.py
--rw-r--r--   0        0        0     6003 2024-03-28 07:32:50.336990 phonexia_grpc-1.5.0/phonexia/grpc/technologies/speaker_diarization/v1/speaker_diarization_pb2.pyi
--rw-r--r--   0        0        0     3311 2024-03-28 07:32:50.336990 phonexia_grpc-1.5.0/phonexia/grpc/technologies/speaker_diarization/v1/speaker_diarization_pb2_grpc.py
--rw-r--r--   0        0        0     3680 2024-03-28 07:32:50.336990 phonexia_grpc-1.5.0/phonexia/grpc/technologies/speaker_identification/v1/speaker_identification_pb2.py
--rw-r--r--   0        0        0     7890 2024-03-28 07:32:50.336990 phonexia_grpc-1.5.0/phonexia/grpc/technologies/speaker_identification/v1/speaker_identification_pb2.pyi
--rw-r--r--   0        0        0     6602 2024-03-28 07:32:50.336990 phonexia_grpc-1.5.0/phonexia/grpc/technologies/speaker_identification/v1/speaker_identification_pb2_grpc.py
--rw-r--r--   0        0        0     4116 2024-03-28 07:32:50.336990 phonexia_grpc-1.5.0/phonexia/grpc/technologies/speech_to_text_whisper_enhanced/v1/speech_to_text_whisper_enhanced_pb2.py
--rw-r--r--   0        0        0     8939 2024-03-28 07:32:50.336990 phonexia_grpc-1.5.0/phonexia/grpc/technologies/speech_to_text_whisper_enhanced/v1/speech_to_text_whisper_enhanced_pb2.pyi
--rw-r--r--   0        0        0     6186 2024-03-28 07:32:50.336990 phonexia_grpc-1.5.0/phonexia/grpc/technologies/speech_to_text_whisper_enhanced/v1/speech_to_text_whisper_enhanced_pb2_grpc.py
--rw-r--r--   0        0        0     3259 2024-03-28 07:32:32.730742 phonexia_grpc-1.5.0/pypi-README.md
--rw-r--r--   0        0        0     1565 2024-03-28 07:32:50.694995 phonexia_grpc-1.5.0/pyproject.toml
--rw-r--r--   0        0        0     4468 1970-01-01 00:00:00.000000 phonexia_grpc-1.5.0/PKG-INFO
+-rw-r--r--   0        0        0    11358 2024-04-25 12:34:14.742177 phonexia_grpc-2.0.0/LICENSE
+-rw-r--r--   0        0        0     1910 2024-04-25 12:34:48.610693 phonexia_grpc-2.0.0/phonexia/grpc/common/core_pb2.py
+-rw-r--r--   0        0        0     5206 2024-04-25 12:34:48.610693 phonexia_grpc-2.0.0/phonexia/grpc/common/core_pb2.pyi
+-rw-r--r--   0        0        0     1145 2024-04-25 12:34:48.610693 phonexia_grpc-2.0.0/phonexia/grpc/common/core_pb2_grpc.py
+-rw-r--r--   0        0        0     1941 2024-04-25 12:34:48.610693 phonexia_grpc-2.0.0/phonexia/grpc/common/health_check_pb2.py
+-rw-r--r--   0        0        0     3337 2024-04-25 12:34:48.610693 phonexia_grpc-2.0.0/phonexia/grpc/common/health_check_pb2.pyi
+-rw-r--r--   0        0        0     5803 2024-04-25 12:34:48.610693 phonexia_grpc-2.0.0/phonexia/grpc/common/health_check_pb2_grpc.py
+-rw-r--r--   0        0        0     1849 2024-04-25 12:34:48.610693 phonexia_grpc-2.0.0/phonexia/grpc/common/licensing_pb2.py
+-rw-r--r--   0        0        0     3031 2024-04-25 12:34:48.610693 phonexia_grpc-2.0.0/phonexia/grpc/common/licensing_pb2.pyi
+-rw-r--r--   0        0        0     3841 2024-04-25 12:34:48.610693 phonexia_grpc-2.0.0/phonexia/grpc/common/licensing_pb2_grpc.py
+-rw-r--r--   0        0        0     5828 2024-04-25 12:34:48.610693 phonexia_grpc-2.0.0/phonexia/grpc/technologies/enhanced_speech_to_text_built_on_whisper/v1/enhanced_speech_to_text_built_on_whisper_pb2.py
+-rw-r--r--   0        0        0    14876 2024-04-25 12:34:48.610693 phonexia_grpc-2.0.0/phonexia/grpc/technologies/enhanced_speech_to_text_built_on_whisper/v1/enhanced_speech_to_text_built_on_whisper_pb2.pyi
+-rw-r--r--   0        0        0    10975 2024-04-25 12:34:48.610693 phonexia_grpc-2.0.0/phonexia/grpc/technologies/enhanced_speech_to_text_built_on_whisper/v1/enhanced_speech_to_text_built_on_whisper_pb2_grpc.py
+-rw-r--r--   0        0        0     2517 2024-04-25 12:34:48.611693 phonexia_grpc-2.0.0/phonexia/grpc/technologies/gender_identification/v1/gender_identification_pb2.py
+-rw-r--r--   0        0        0     4312 2024-04-25 12:34:48.611693 phonexia_grpc-2.0.0/phonexia/grpc/technologies/gender_identification/v1/gender_identification_pb2.pyi
+-rw-r--r--   0        0        0     4677 2024-04-25 12:34:48.611693 phonexia_grpc-2.0.0/phonexia/grpc/technologies/gender_identification/v1/gender_identification_pb2_grpc.py
+-rw-r--r--   0        0        0     2907 2024-04-25 12:34:48.611693 phonexia_grpc-2.0.0/phonexia/grpc/technologies/speaker_diarization/v1/speaker_diarization_pb2.py
+-rw-r--r--   0        0        0     5753 2024-04-25 12:34:48.611693 phonexia_grpc-2.0.0/phonexia/grpc/technologies/speaker_diarization/v1/speaker_diarization_pb2.pyi
+-rw-r--r--   0        0        0     4510 2024-04-25 12:34:48.611693 phonexia_grpc-2.0.0/phonexia/grpc/technologies/speaker_diarization/v1/speaker_diarization_pb2_grpc.py
+-rw-r--r--   0        0        0     3682 2024-04-25 12:34:48.611693 phonexia_grpc-2.0.0/phonexia/grpc/technologies/speaker_identification/v1/speaker_identification_pb2.py
+-rw-r--r--   0        0        0     7603 2024-04-25 12:34:48.611693 phonexia_grpc-2.0.0/phonexia/grpc/technologies/speaker_identification/v1/speaker_identification_pb2.pyi
+-rw-r--r--   0        0        0     7976 2024-04-25 12:34:48.611693 phonexia_grpc-2.0.0/phonexia/grpc/technologies/speaker_identification/v1/speaker_identification_pb2_grpc.py
+-rw-r--r--   0        0        0     3259 2024-04-25 12:34:14.742177 phonexia_grpc-2.0.0/pypi-README.md
+-rw-r--r--   0        0        0     1564 2024-04-25 12:34:49.016699 phonexia_grpc-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     4467 1970-01-01 00:00:00.000000 phonexia_grpc-2.0.0/PKG-INFO
```

### Comparing `phonexia_grpc-1.5.0/LICENSE` & `phonexia_grpc-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `phonexia_grpc-1.5.0/phonexia/grpc/common/core_pb2.py` & `phonexia_grpc-2.0.0/phonexia/grpc/common/core_pb2.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: phonexia/grpc/common/core.proto
-# Protobuf Python Version: 4.25.1
+# Protobuf Python Version: 5.26.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
@@ -16,16 +16,16 @@
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1fphonexia/grpc/common/core.proto\x12\x14phonexia.grpc.common\x1a\x1egoogle/protobuf/duration.proto\"M\n\x05\x41udio\x12\x0f\n\x07\x63ontent\x18\x01 \x01(\x0c\x12\x33\n\ntime_range\x18\x02 \x01(\x0b\x32\x1f.phonexia.grpc.common.TimeRange\"\x1d\n\nVoiceprint\x12\x0f\n\x07\x63ontent\x18\x01 \x01(\x0c\"C\n\x06Matrix\x12\x12\n\nrows_count\x18\x01 \x01(\x04\x12\x15\n\rcolumns_count\x18\x02 \x01(\x04\x12\x0e\n\x06values\x18\x03 \x03(\x02\"]\n\tTimeRange\x12(\n\x05start\x18\x01 \x01(\x0b\x32\x19.google.protobuf.Duration\x12&\n\x03\x65nd\x18\x02 \x01(\x0b\x32\x19.google.protobuf.Durationb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'phonexia.grpc.common.core_pb2', _globals)
-if _descriptor._USE_C_DESCRIPTORS == False:
-  DESCRIPTOR._options = None
+if not _descriptor._USE_C_DESCRIPTORS:
+  DESCRIPTOR._loaded_options = None
   _globals['_AUDIO']._serialized_start=89
   _globals['_AUDIO']._serialized_end=166
   _globals['_VOICEPRINT']._serialized_start=168
   _globals['_VOICEPRINT']._serialized_end=197
   _globals['_MATRIX']._serialized_start=199
   _globals['_MATRIX']._serialized_end=266
   _globals['_TIMERANGE']._serialized_start=268
```

### Comparing `phonexia_grpc-1.5.0/phonexia/grpc/common/core_pb2.pyi` & `phonexia_grpc-2.0.0/phonexia/grpc/common/core_pb2.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
-Copyright 2023 Phonexia s.r.o.
+Copyright 2024 Phonexia s.r.o.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
@@ -13,30 +13,26 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 
 Phonexia common message definitions for gRPC API.
 """
+
 import builtins
 import collections.abc
 import google.protobuf.descriptor
 import google.protobuf.duration_pb2
 import google.protobuf.internal.containers
 import google.protobuf.message
-import sys
-
-if sys.version_info >= (3, 8):
-    import typing as typing_extensions
-else:
-    import typing_extensions
+import typing
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-@typing_extensions.final
+@typing.final
 class Audio(google.protobuf.message.Message):
     """ Contains audio data in the supported format and encoding.
      Supported formats are <code>WAV</code> (various encoding), <code>FLAC</code>
      and <code>OGG_OPUS</code>. For best results, the audio source should be
      captured and transmitted using a lossless encoding (<code>FLAC</code> or
      <code>LINEAR16</code>). The accuracy of the speech technologies can be
      reduced if lossy codecs are used to capture or transmit audio, particularly
@@ -56,44 +52,45 @@
     @property
     def time_range(self) -> global___TimeRange:
         """Time range of the audio to process. If omitted, the
         whole audio is processed. If <code>start</code> is omitted, the
         audio is process from the beginning. If <code>end</code> is omitted,
         the audio is processed to the end.
         """
+
     def __init__(
         self,
         *,
         content: builtins.bytes = ...,
         time_range: global___TimeRange | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["time_range", b"time_range"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["content", b"content", "time_range", b"time_range"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["time_range", b"time_range"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["content", b"content", "time_range", b"time_range"]) -> None: ...
 
 global___Audio = Audio
 
-@typing_extensions.final
+@typing.final
 class Voiceprint(google.protobuf.message.Message):
     """Represents the result from voiceprint extraction."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     CONTENT_FIELD_NUMBER: builtins.int
     content: builtins.bytes
     """Voiceprint data bytes encoded in UBJSON format."""
     def __init__(
         self,
         *,
         content: builtins.bytes = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["content", b"content"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["content", b"content"]) -> None: ...
 
 global___Voiceprint = Voiceprint
 
-@typing_extensions.final
+@typing.final
 class Matrix(google.protobuf.message.Message):
     """Data type representing matrix of values. The matrix is represented as a
     linear array in row major format.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -103,42 +100,45 @@
     rows_count: builtins.int
     """Number of rows in the matrix."""
     columns_count: builtins.int
     """Number of columns in the matrix."""
     @property
     def values(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.float]:
         """Sequential list of matrix values in row major format."""
+
     def __init__(
         self,
         *,
         rows_count: builtins.int = ...,
         columns_count: builtins.int = ...,
         values: collections.abc.Iterable[builtins.float] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["columns_count", b"columns_count", "rows_count", b"rows_count", "values", b"values"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["columns_count", b"columns_count", "rows_count", b"rows_count", "values", b"values"]) -> None: ...
 
 global___Matrix = Matrix
 
-@typing_extensions.final
+@typing.final
 class TimeRange(google.protobuf.message.Message):
     """Data type representing time range."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     START_FIELD_NUMBER: builtins.int
     END_FIELD_NUMBER: builtins.int
     @property
     def start(self) -> google.protobuf.duration_pb2.Duration:
         """Start time of the time range."""
+
     @property
     def end(self) -> google.protobuf.duration_pb2.Duration:
         """End time of the time range."""
+
     def __init__(
         self,
         *,
         start: google.protobuf.duration_pb2.Duration | None = ...,
         end: google.protobuf.duration_pb2.Duration | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["end", b"end", "start", b"start"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["end", b"end", "start", b"start"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["end", b"end", "start", b"start"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["end", b"end", "start", b"start"]) -> None: ...
 
 global___TimeRange = TimeRange
```

### Comparing `phonexia_grpc-1.5.0/phonexia/grpc/common/health_check_pb2.py` & `phonexia_grpc-2.0.0/phonexia/grpc/common/health_check_pb2.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: phonexia/grpc/common/health_check.proto
-# Protobuf Python Version: 4.25.1
+# Protobuf Python Version: 5.26.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
@@ -15,16 +15,16 @@
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\'phonexia/grpc/common/health_check.proto\x12\x0egrpc.health.v1\"%\n\x12HealthCheckRequest\x12\x0f\n\x07service\x18\x01 \x01(\t\"\x94\x01\n\x13HealthCheckResponse\x12\x41\n\x06status\x18\x01 \x01(\x0e\x32\x31.grpc.health.v1.HealthCheckResponse.ServingStatus\":\n\rServingStatus\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x0b\n\x07SERVING\x10\x01\x12\x0f\n\x0bNOT_SERVING\x10\x02\x32\xae\x01\n\x06Health\x12P\n\x05\x43heck\x12\".grpc.health.v1.HealthCheckRequest\x1a#.grpc.health.v1.HealthCheckResponse\x12R\n\x05Watch\x12\".grpc.health.v1.HealthCheckRequest\x1a#.grpc.health.v1.HealthCheckResponse0\x01\x62\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'phonexia.grpc.common.health_check_pb2', _globals)
-if _descriptor._USE_C_DESCRIPTORS == False:
-  DESCRIPTOR._options = None
+if not _descriptor._USE_C_DESCRIPTORS:
+  DESCRIPTOR._loaded_options = None
   _globals['_HEALTHCHECKREQUEST']._serialized_start=59
   _globals['_HEALTHCHECKREQUEST']._serialized_end=96
   _globals['_HEALTHCHECKRESPONSE']._serialized_start=99
   _globals['_HEALTHCHECKRESPONSE']._serialized_end=247
   _globals['_HEALTHCHECKRESPONSE_SERVINGSTATUS']._serialized_start=189
   _globals['_HEALTHCHECKRESPONSE_SERVINGSTATUS']._serialized_end=247
   _globals['_HEALTH']._serialized_start=250
```

### Comparing `phonexia_grpc-1.5.0/phonexia/grpc/common/health_check_pb2.pyi` & `phonexia_grpc-2.0.0/phonexia/grpc/common/health_check_pb2.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
-Copyright 2023 Phonexia s.r.o.
+Copyright 2024 Phonexia s.r.o.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
@@ -13,47 +13,48 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 
 Health check definitions for gRPC API.
 """
+
 import builtins
 import google.protobuf.descriptor
 import google.protobuf.internal.enum_type_wrapper
 import google.protobuf.message
 import sys
 import typing
 
 if sys.version_info >= (3, 10):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-@typing_extensions.final
+@typing.final
 class HealthCheckRequest(google.protobuf.message.Message):
     """Request message for checking the health of a service."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     SERVICE_FIELD_NUMBER: builtins.int
     service: builtins.str
     """The name of the service to check."""
     def __init__(
         self,
         *,
         service: builtins.str = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["service", b"service"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["service", b"service"]) -> None: ...
 
 global___HealthCheckRequest = HealthCheckRequest
 
-@typing_extensions.final
+@typing.final
 class HealthCheckResponse(google.protobuf.message.Message):
     """Response message for checking the health of a service."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     class _ServingStatus:
         ValueType = typing.NewType("ValueType", builtins.int)
@@ -82,10 +83,10 @@
     status: global___HealthCheckResponse.ServingStatus.ValueType
     """The serving status of the checked service."""
     def __init__(
         self,
         *,
         status: global___HealthCheckResponse.ServingStatus.ValueType = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["status", b"status"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["status", b"status"]) -> None: ...
 
 global___HealthCheckResponse = HealthCheckResponse
```

### Comparing `phonexia_grpc-1.5.0/phonexia/grpc/common/licensing_pb2.py` & `phonexia_grpc-2.0.0/phonexia/grpc/common/licensing_pb2.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: phonexia/grpc/common/licensing.proto
-# Protobuf Python Version: 4.25.1
+# Protobuf Python Version: 5.26.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
@@ -15,16 +15,16 @@
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n$phonexia/grpc/common/licensing.proto\x12\x14phonexia.grpc.common\"\x16\n\x14LicensingInfoRequest\"\x8a\x01\n\x13LicensingInfoResult\x12\x13\n\x0bvalid_until\x18\x01 \x01(\t\x12\x10\n\x08is_valid\x18\x02 \x01(\x08\x12\x17\n\x0ftechnology_name\x18\x03 \x01(\t\x12\x33\n\nmodel_info\x18\x04 \x01(\x0b\x32\x1f.phonexia.grpc.common.ModelInfo\"*\n\tModelInfo\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\t2j\n\tLicensing\x12]\n\x04Info\x12*.phonexia.grpc.common.LicensingInfoRequest\x1a).phonexia.grpc.common.LicensingInfoResultb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'phonexia.grpc.common.licensing_pb2', _globals)
-if _descriptor._USE_C_DESCRIPTORS == False:
-  DESCRIPTOR._options = None
+if not _descriptor._USE_C_DESCRIPTORS:
+  DESCRIPTOR._loaded_options = None
   _globals['_LICENSINGINFOREQUEST']._serialized_start=62
   _globals['_LICENSINGINFOREQUEST']._serialized_end=84
   _globals['_LICENSINGINFORESULT']._serialized_start=87
   _globals['_LICENSINGINFORESULT']._serialized_end=225
   _globals['_MODELINFO']._serialized_start=227
   _globals['_MODELINFO']._serialized_end=269
   _globals['_LICENSING']._serialized_start=271
```

### Comparing `phonexia_grpc-1.5.0/phonexia/grpc/common/licensing_pb2.pyi` & `phonexia_grpc-2.0.0/phonexia/grpc/common/licensing_pb2.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
-Copyright 2023 Phonexia s.r.o.
+Copyright 2024 Phonexia s.r.o.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
@@ -13,37 +13,33 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 
 Phonexia licensing definitions for gRPC API.
 """
+
 import builtins
 import google.protobuf.descriptor
 import google.protobuf.message
-import sys
-
-if sys.version_info >= (3, 8):
-    import typing as typing_extensions
-else:
-    import typing_extensions
+import typing
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-@typing_extensions.final
+@typing.final
 class LicensingInfoRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     def __init__(
         self,
     ) -> None: ...
 
 global___LicensingInfoRequest = LicensingInfoRequest
 
-@typing_extensions.final
+@typing.final
 class LicensingInfoResult(google.protobuf.message.Message):
     """The top-level message returned to the client by <code>LicenseInfo</code>
     method.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -56,28 +52,29 @@
     is_valid: builtins.bool
     """License status, contains "false" if the license has expired."""
     technology_name: builtins.str
     """Name of the technology being licensed."""
     @property
     def model_info(self) -> global___ModelInfo:
         """Information about the licensed model."""
+
     def __init__(
         self,
         *,
         valid_until: builtins.str = ...,
         is_valid: builtins.bool = ...,
         technology_name: builtins.str = ...,
         model_info: global___ModelInfo | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["model_info", b"model_info"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["is_valid", b"is_valid", "model_info", b"model_info", "technology_name", b"technology_name", "valid_until", b"valid_until"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["model_info", b"model_info"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["is_valid", b"is_valid", "model_info", b"model_info", "technology_name", b"technology_name", "valid_until", b"valid_until"]) -> None: ...
 
 global___LicensingInfoResult = LicensingInfoResult
 
-@typing_extensions.final
+@typing.final
 class ModelInfo(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     NAME_FIELD_NUMBER: builtins.int
     VERSION_FIELD_NUMBER: builtins.int
     name: builtins.str
     """Name of the model."""
@@ -85,10 +82,10 @@
     """Version of the model."""
     def __init__(
         self,
         *,
         name: builtins.str = ...,
         version: builtins.str = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["name", b"name", "version", b"version"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["name", b"name", "version", b"version"]) -> None: ...
 
 global___ModelInfo = ModelInfo
```

### Comparing `phonexia_grpc-1.5.0/phonexia/grpc/technologies/gender_identification/v1/gender_identification_pb2.py` & `phonexia_grpc-2.0.0/phonexia/grpc/technologies/gender_identification/v1/gender_identification_pb2.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: phonexia/grpc/technologies/gender_identification/v1/gender_identification.proto
-# Protobuf Python Version: 4.25.1
+# Protobuf Python Version: 5.26.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
@@ -16,16 +16,16 @@
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\nOphonexia/grpc/technologies/gender_identification/v1/gender_identification.proto\x12\x33phonexia.grpc.technologies.gender_identification.v1\x1a\x1fphonexia/grpc/common/core.proto\"H\n\x0fIdentifyRequest\x12\x35\n\x0bvoiceprints\x18\x01 \x03(\x0b\x32 .phonexia.grpc.common.Voiceprint\"\x1a\n\x05Score\x12\x11\n\tscore_llr\x18\x01 \x01(\x02\"\xb2\x01\n\x0eIdentifyResult\x12N\n\nscore_male\x18\x01 \x01(\x0b\x32:.phonexia.grpc.technologies.gender_identification.v1.Score\x12P\n\x0cscore_female\x18\x02 \x01(\x0b\x32:.phonexia.grpc.technologies.gender_identification.v1.Score\"h\n\x10IdentifyResponse\x12T\n\x07results\x18\x01 \x03(\x0b\x32\x43.phonexia.grpc.technologies.gender_identification.v1.IdentifyResult2\xb4\x01\n\x14GenderIdentification\x12\x9b\x01\n\x08Identify\x12\x44.phonexia.grpc.technologies.gender_identification.v1.IdentifyRequest\x1a\x45.phonexia.grpc.technologies.gender_identification.v1.IdentifyResponse(\x01\x30\x01\x62\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'phonexia.grpc.technologies.gender_identification.v1.gender_identification_pb2', _globals)
-if _descriptor._USE_C_DESCRIPTORS == False:
-  DESCRIPTOR._options = None
+if not _descriptor._USE_C_DESCRIPTORS:
+  DESCRIPTOR._loaded_options = None
   _globals['_IDENTIFYREQUEST']._serialized_start=169
   _globals['_IDENTIFYREQUEST']._serialized_end=241
   _globals['_SCORE']._serialized_start=243
   _globals['_SCORE']._serialized_end=269
   _globals['_IDENTIFYRESULT']._serialized_start=272
   _globals['_IDENTIFYRESULT']._serialized_end=450
   _globals['_IDENTIFYRESPONSE']._serialized_start=452
```

### Comparing `phonexia_grpc-1.5.0/phonexia/grpc/technologies/gender_identification/v1/gender_identification_pb2.pyi` & `phonexia_grpc-2.0.0/phonexia/grpc/technologies/gender_identification/v1/gender_identification_pb2.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -13,51 +13,48 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 
 Phonexia Gender Identification gRPC API.
 """
+
 import builtins
 import collections.abc
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
 import google.protobuf.message
 import phonexia.grpc.common.core_pb2
-import sys
-
-if sys.version_info >= (3, 8):
-    import typing as typing_extensions
-else:
-    import typing_extensions
+import typing
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-@typing_extensions.final
+@typing.final
 class IdentifyRequest(google.protobuf.message.Message):
     """The top-level message sent by the client for the <code>Identify</code>
     method.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     VOICEPRINTS_FIELD_NUMBER: builtins.int
     @property
     def voiceprints(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[phonexia.grpc.common.core_pb2.Voiceprint]:
         """List of voiceprints for the identification."""
+
     def __init__(
         self,
         *,
         voiceprints: collections.abc.Iterable[phonexia.grpc.common.core_pb2.Voiceprint] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["voiceprints", b"voiceprints"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["voiceprints", b"voiceprints"]) -> None: ...
 
 global___IdentifyRequest = IdentifyRequest
 
-@typing_extensions.final
+@typing.final
 class Score(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     SCORE_LLR_FIELD_NUMBER: builtins.int
     score_llr: builtins.float
     """Log-likelihood ratio score. The LLR provides a quantitative measure of
     how much more likely the data is under one model (gender) compared
@@ -67,59 +64,62 @@
     the opposite.
     """
     def __init__(
         self,
         *,
         score_llr: builtins.float = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["score_llr", b"score_llr"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["score_llr", b"score_llr"]) -> None: ...
 
 global___Score = Score
 
-@typing_extensions.final
+@typing.final
 class IdentifyResult(google.protobuf.message.Message):
     """A gender identification result. It contains scores for respective genders."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     SCORE_MALE_FIELD_NUMBER: builtins.int
     SCORE_FEMALE_FIELD_NUMBER: builtins.int
     @property
     def score_male(self) -> global___Score:
         """Score for male."""
+
     @property
     def score_female(self) -> global___Score:
         """Score for female."""
+
     def __init__(
         self,
         *,
         score_male: global___Score | None = ...,
         score_female: global___Score | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["score_female", b"score_female", "score_male", b"score_male"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["score_female", b"score_female", "score_male", b"score_male"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["score_female", b"score_female", "score_male", b"score_male"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["score_female", b"score_female", "score_male", b"score_male"]) -> None: ...
 
 global___IdentifyResult = IdentifyResult
 
-@typing_extensions.final
+@typing.final
 class IdentifyResponse(google.protobuf.message.Message):
     """The top-level message returned to the client by the <code>Identify</code>
     method. It contains the result as one or more <code>IdentifyResult</code>
     messages.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     RESULTS_FIELD_NUMBER: builtins.int
     @property
     def results(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___IdentifyResult]:
         """Sequential list of results corresponding to sequential list of voiceprints
         in <code>IdentifyRequest</code>.
         """
+
     def __init__(
         self,
         *,
         results: collections.abc.Iterable[global___IdentifyResult] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["results", b"results"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["results", b"results"]) -> None: ...
 
 global___IdentifyResponse = IdentifyResponse
```

### Comparing `phonexia_grpc-1.5.0/phonexia/grpc/technologies/speaker_diarization/v1/speaker_diarization_pb2.py` & `phonexia_grpc-2.0.0/phonexia/grpc/technologies/speaker_diarization/v1/speaker_diarization_pb2.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: phonexia/grpc/technologies/speaker_diarization/v1/speaker_diarization.proto
-# Protobuf Python Version: 4.25.1
+# Protobuf Python Version: 5.26.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
@@ -17,16 +17,16 @@
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\nKphonexia/grpc/technologies/speaker_diarization/v1/speaker_diarization.proto\x12\x31phonexia.grpc.technologies.speaker_diarization.v1\x1a\x1fphonexia/grpc/common/core.proto\x1a\x1egoogle/protobuf/duration.proto\"\x8e\x01\n\x0e\x44iarizeRequest\x12*\n\x05\x61udio\x18\x01 \x01(\x0b\x32\x1b.phonexia.grpc.common.Audio\x12P\n\x06\x63onfig\x18\x02 \x01(\x0b\x32@.phonexia.grpc.technologies.speaker_diarization.v1.DiarizeConfig\"U\n\rDiarizeConfig\x12\x14\n\x0cmax_speakers\x18\x01 \x01(\x05\x12\x1b\n\x0etotal_speakers\x18\x02 \x01(\x05H\x00\x88\x01\x01\x42\x11\n\x0f_total_speakers\"\xb2\x01\n\x0f\x44iarizeResponse\x12\x16\n\x0espeakers_count\x18\x01 \x01(\x05\x12L\n\x08segments\x18\x02 \x03(\x0b\x32:.phonexia.grpc.technologies.speaker_diarization.v1.Segment\x12\x39\n\x16processed_audio_length\x18\x03 \x01(\x0b\x32\x19.google.protobuf.Duration\"y\n\x07Segment\x12\x12\n\nspeaker_id\x18\x01 \x01(\x05\x12-\n\nstart_time\x18\x02 \x01(\x0b\x32\x19.google.protobuf.Duration\x12+\n\x08\x65nd_time\x18\x03 \x01(\x0b\x32\x19.google.protobuf.Duration2\xa9\x01\n\x12SpeakerDiarization\x12\x92\x01\n\x07\x44iarize\x12\x41.phonexia.grpc.technologies.speaker_diarization.v1.DiarizeRequest\x1a\x42.phonexia.grpc.technologies.speaker_diarization.v1.DiarizeResponse(\x01\x62\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'phonexia.grpc.technologies.speaker_diarization.v1.speaker_diarization_pb2', _globals)
-if _descriptor._USE_C_DESCRIPTORS == False:
-  DESCRIPTOR._options = None
+if not _descriptor._USE_C_DESCRIPTORS:
+  DESCRIPTOR._loaded_options = None
   _globals['_DIARIZEREQUEST']._serialized_start=196
   _globals['_DIARIZEREQUEST']._serialized_end=338
   _globals['_DIARIZECONFIG']._serialized_start=340
   _globals['_DIARIZECONFIG']._serialized_end=425
   _globals['_DIARIZERESPONSE']._serialized_start=428
   _globals['_DIARIZERESPONSE']._serialized_end=606
   _globals['_SEGMENT']._serialized_start=608
```

### Comparing `phonexia_grpc-1.5.0/phonexia/grpc/technologies/speaker_diarization/v1/speaker_diarization_pb2.pyi` & `phonexia_grpc-2.0.0/phonexia/grpc/technologies/speaker_diarization/v1/speaker_diarization_pb2.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -13,56 +13,54 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 
 Phonexia Speaker Diarization gRPC API
 """
+
 import builtins
 import collections.abc
 import google.protobuf.descriptor
 import google.protobuf.duration_pb2
 import google.protobuf.internal.containers
 import google.protobuf.message
 import phonexia.grpc.common.core_pb2
-import sys
-
-if sys.version_info >= (3, 8):
-    import typing as typing_extensions
-else:
-    import typing_extensions
+import typing
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-@typing_extensions.final
+@typing.final
 class DiarizeRequest(google.protobuf.message.Message):
     """The top-level message sent by the client for the <code>Diarize</code> method."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     AUDIO_FIELD_NUMBER: builtins.int
     CONFIG_FIELD_NUMBER: builtins.int
     @property
     def audio(self) -> phonexia.grpc.common.core_pb2.Audio:
         """Audio to be diarized."""
+
     @property
     def config(self) -> global___DiarizeConfig:
         """Speaker diarization configuration."""
+
     def __init__(
         self,
         *,
         audio: phonexia.grpc.common.core_pb2.Audio | None = ...,
         config: global___DiarizeConfig | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["audio", b"audio", "config", b"config"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["audio", b"audio", "config", b"config"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["audio", b"audio", "config", b"config"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["audio", b"audio", "config", b"config"]) -> None: ...
 
 global___DiarizeRequest = DiarizeRequest
 
-@typing_extensions.final
+@typing.final
 class DiarizeConfig(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     MAX_SPEAKERS_FIELD_NUMBER: builtins.int
     TOTAL_SPEAKERS_FIELD_NUMBER: builtins.int
     max_speakers: builtins.int
     """Upper limit for the number of speakers in the audio.
@@ -77,21 +75,21 @@
     """
     def __init__(
         self,
         *,
         max_speakers: builtins.int = ...,
         total_speakers: builtins.int | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["_total_speakers", b"_total_speakers", "total_speakers", b"total_speakers"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["_total_speakers", b"_total_speakers", "max_speakers", b"max_speakers", "total_speakers", b"total_speakers"]) -> None: ...
-    def WhichOneof(self, oneof_group: typing_extensions.Literal["_total_speakers", b"_total_speakers"]) -> typing_extensions.Literal["total_speakers"] | None: ...
+    def HasField(self, field_name: typing.Literal["_total_speakers", b"_total_speakers", "total_speakers", b"total_speakers"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["_total_speakers", b"_total_speakers", "max_speakers", b"max_speakers", "total_speakers", b"total_speakers"]) -> None: ...
+    def WhichOneof(self, oneof_group: typing.Literal["_total_speakers", b"_total_speakers"]) -> typing.Literal["total_speakers"] | None: ...
 
 global___DiarizeConfig = DiarizeConfig
 
-@typing_extensions.final
+@typing.final
 class DiarizeResponse(google.protobuf.message.Message):
     """The top-level message returned to the client by the <code>Diarize</code>
     method.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -99,48 +97,52 @@
     SEGMENTS_FIELD_NUMBER: builtins.int
     PROCESSED_AUDIO_LENGTH_FIELD_NUMBER: builtins.int
     speakers_count: builtins.int
     """Detected number of speakers in the audio."""
     @property
     def segments(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___Segment]:
         """List of detected segments in the audio."""
+
     @property
     def processed_audio_length(self) -> google.protobuf.duration_pb2.Duration:
         """Total length of the processed audio."""
+
     def __init__(
         self,
         *,
         speakers_count: builtins.int = ...,
         segments: collections.abc.Iterable[global___Segment] | None = ...,
         processed_audio_length: google.protobuf.duration_pb2.Duration | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["processed_audio_length", b"processed_audio_length"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["processed_audio_length", b"processed_audio_length", "segments", b"segments", "speakers_count", b"speakers_count"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["processed_audio_length", b"processed_audio_length"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["processed_audio_length", b"processed_audio_length", "segments", b"segments", "speakers_count", b"speakers_count"]) -> None: ...
 
 global___DiarizeResponse = DiarizeResponse
 
-@typing_extensions.final
+@typing.final
 class Segment(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     SPEAKER_ID_FIELD_NUMBER: builtins.int
     START_TIME_FIELD_NUMBER: builtins.int
     END_TIME_FIELD_NUMBER: builtins.int
     speaker_id: builtins.int
     """Identifier of a speaker in the segment."""
     @property
     def start_time(self) -> google.protobuf.duration_pb2.Duration:
         """Start time of the segment."""
+
     @property
     def end_time(self) -> google.protobuf.duration_pb2.Duration:
         """End time of the segment."""
+
     def __init__(
         self,
         *,
         speaker_id: builtins.int = ...,
         start_time: google.protobuf.duration_pb2.Duration | None = ...,
         end_time: google.protobuf.duration_pb2.Duration | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["end_time", b"end_time", "start_time", b"start_time"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["end_time", b"end_time", "speaker_id", b"speaker_id", "start_time", b"start_time"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["end_time", b"end_time", "start_time", b"start_time"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["end_time", b"end_time", "speaker_id", b"speaker_id", "start_time", b"start_time"]) -> None: ...
 
 global___Segment = Segment
```

### Comparing `phonexia_grpc-1.5.0/phonexia/grpc/technologies/speaker_identification/v1/speaker_identification_pb2.py` & `phonexia_grpc-2.0.0/phonexia/grpc/technologies/speaker_identification/v1/speaker_identification_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: phonexia/grpc/technologies/speaker_identification/v1/speaker_identification.proto
-# Protobuf Python Version: 4.25.1
+# Protobuf Python Version: 5.26.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
@@ -17,16 +17,16 @@
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\nQphonexia/grpc/technologies/speaker_identification/v1/speaker_identification.proto\x12\x34phonexia.grpc.technologies.speaker_identification.v1\x1a\x1fphonexia/grpc/common/core.proto\x1a\x1egoogle/protobuf/duration.proto\"\x82\x01\n\x0e\x43ompareRequest\x12\x37\n\rvoiceprints_a\x18\x01 \x03(\x0b\x32 .phonexia.grpc.common.Voiceprint\x12\x37\n\rvoiceprints_b\x18\x02 \x03(\x0b\x32 .phonexia.grpc.common.Voiceprint\"?\n\x0f\x43ompareResponse\x12,\n\x06scores\x18\x01 \x01(\x0b\x32\x1c.phonexia.grpc.common.Matrix\"\x91\x01\n\x0e\x45xtractRequest\x12*\n\x05\x61udio\x18\x01 \x01(\x0b\x32\x1b.phonexia.grpc.common.Audio\x12S\n\x06\x63onfig\x18\x02 \x01(\x0b\x32\x43.phonexia.grpc.technologies.speaker_identification.v1.ExtractConfig\"A\n\rExtractConfig\x12\x30\n\rspeech_length\x18\x01 \x01(\x0b\x32\x19.google.protobuf.Duration\"w\n\rExtractResult\x12\x30\n\rspeech_length\x18\x01 \x01(\x0b\x32\x19.google.protobuf.Duration\x12\x34\n\nvoiceprint\x18\x02 \x01(\x0b\x32 .phonexia.grpc.common.Voiceprint\"\xa1\x01\n\x0f\x45xtractResponse\x12S\n\x06result\x18\x01 \x01(\x0b\x32\x43.phonexia.grpc.technologies.speaker_identification.v1.ExtractResult\x12\x39\n\x16processed_audio_length\x18\x02 \x01(\x0b\x32\x19.google.protobuf.Duration2\xb3\x01\n\x14VoiceprintComparison\x12\x9a\x01\n\x07\x43ompare\x12\x44.phonexia.grpc.technologies.speaker_identification.v1.CompareRequest\x1a\x45.phonexia.grpc.technologies.speaker_identification.v1.CompareResponse(\x01\x30\x01\x32\xb1\x01\n\x14VoiceprintExtraction\x12\x98\x01\n\x07\x45xtract\x12\x44.phonexia.grpc.technologies.speaker_identification.v1.ExtractRequest\x1a\x45.phonexia.grpc.technologies.speaker_identification.v1.ExtractResponse(\x01\x62\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'phonexia.grpc.technologies.speaker_identification.v1.speaker_identification_pb2', _globals)
-if _descriptor._USE_C_DESCRIPTORS == False:
-  DESCRIPTOR._options = None
+if not _descriptor._USE_C_DESCRIPTORS:
+  DESCRIPTOR._loaded_options = None
   _globals['_COMPAREREQUEST']._serialized_start=205
   _globals['_COMPAREREQUEST']._serialized_end=335
   _globals['_COMPARERESPONSE']._serialized_start=337
   _globals['_COMPARERESPONSE']._serialized_end=400
   _globals['_EXTRACTREQUEST']._serialized_start=403
   _globals['_EXTRACTREQUEST']._serialized_end=548
   _globals['_EXTRACTCONFIG']._serialized_start=550
```

### Comparing `phonexia_grpc-1.5.0/phonexia/grpc/technologies/speaker_identification/v1/speaker_identification_pb2.pyi` & `phonexia_grpc-2.0.0/phonexia/grpc/technologies/speaker_identification/v1/speaker_identification_pb2.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
-Copyright 2023 Phonexia s.r.o.
+Copyright 2024 Phonexia s.r.o.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
@@ -13,55 +13,53 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 
 Phonexia Speaker Identification gRPC API.
 """
+
 import builtins
 import collections.abc
 import google.protobuf.descriptor
 import google.protobuf.duration_pb2
 import google.protobuf.internal.containers
 import google.protobuf.message
 import phonexia.grpc.common.core_pb2
-import sys
-
-if sys.version_info >= (3, 8):
-    import typing as typing_extensions
-else:
-    import typing_extensions
+import typing
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-@typing_extensions.final
+@typing.final
 class CompareRequest(google.protobuf.message.Message):
     """The message sent by the client for the <code>Compare</code> method."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     VOICEPRINTS_A_FIELD_NUMBER: builtins.int
     VOICEPRINTS_B_FIELD_NUMBER: builtins.int
     @property
     def voiceprints_a(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[phonexia.grpc.common.core_pb2.Voiceprint]:
         """First list of voiceprints to be compared."""
+
     @property
     def voiceprints_b(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[phonexia.grpc.common.core_pb2.Voiceprint]:
         """Second list of voiceprints to be compared."""
+
     def __init__(
         self,
         *,
         voiceprints_a: collections.abc.Iterable[phonexia.grpc.common.core_pb2.Voiceprint] | None = ...,
         voiceprints_b: collections.abc.Iterable[phonexia.grpc.common.core_pb2.Voiceprint] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["voiceprints_a", b"voiceprints_a", "voiceprints_b", b"voiceprints_b"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["voiceprints_a", b"voiceprints_a", "voiceprints_b", b"voiceprints_b"]) -> None: ...
 
 global___CompareRequest = CompareRequest
 
-@typing_extensions.final
+@typing.final
 class CompareResponse(google.protobuf.message.Message):
     """The top-level message returned to the client by the <code>Compare</code>
     method. It contains comparison matrix of log-likelihood ratio (LLR) scores.
     Comparison matrix containing similarity scores between
     <code>voiceprints_a</code> and <code>voiceprints_b</code>. The element at
     row <code>i</code> and column <code>j</code> corresponds to the comparison
     result between <code>voiceprints_a[i]</code> and
@@ -73,117 +71,125 @@
     SCORES_FIELD_NUMBER: builtins.int
     @property
     def scores(self) -> phonexia.grpc.common.core_pb2.Matrix:
         """The similarity scores are expressed as log-likelihood ratio (LLR) values,
         which fall within the interval of <code>(-inf;+inf)</code>, with higher
         values indicating higher similarity.
         """
+
     def __init__(
         self,
         *,
         scores: phonexia.grpc.common.core_pb2.Matrix | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["scores", b"scores"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["scores", b"scores"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["scores", b"scores"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["scores", b"scores"]) -> None: ...
 
 global___CompareResponse = CompareResponse
 
-@typing_extensions.final
+@typing.final
 class ExtractRequest(google.protobuf.message.Message):
     """The top-level message sent by the client for the <code>Extract</code> method."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     AUDIO_FIELD_NUMBER: builtins.int
     CONFIG_FIELD_NUMBER: builtins.int
     @property
     def audio(self) -> phonexia.grpc.common.core_pb2.Audio:
         """Audio to extract voiceprints from."""
+
     @property
     def config(self) -> global___ExtractConfig:
         """Voiceprint extraction configuration."""
+
     def __init__(
         self,
         *,
         audio: phonexia.grpc.common.core_pb2.Audio | None = ...,
         config: global___ExtractConfig | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["audio", b"audio", "config", b"config"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["audio", b"audio", "config", b"config"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["audio", b"audio", "config", b"config"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["audio", b"audio", "config", b"config"]) -> None: ...
 
 global___ExtractRequest = ExtractRequest
 
-@typing_extensions.final
+@typing.final
 class ExtractConfig(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     SPEECH_LENGTH_FIELD_NUMBER: builtins.int
     @property
     def speech_length(self) -> google.protobuf.duration_pb2.Duration:
         """Specifies the maximum speech length from which the voiceprint will be
-        extracted. If there is less speech in the recording than the specified
-        duration, the voiceprint will be extracted from the entire recording.
+        extracted. If there is less speech in the audio than the specified
+        duration, the voiceprint will be extracted from the entire audio.
         """
+
     def __init__(
         self,
         *,
         speech_length: google.protobuf.duration_pb2.Duration | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["speech_length", b"speech_length"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["speech_length", b"speech_length"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["speech_length", b"speech_length"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["speech_length", b"speech_length"]) -> None: ...
 
 global___ExtractConfig = ExtractConfig
 
-@typing_extensions.final
+@typing.final
 class ExtractResult(google.protobuf.message.Message):
     """A voiceprint extraction result."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     SPEECH_LENGTH_FIELD_NUMBER: builtins.int
     VOICEPRINT_FIELD_NUMBER: builtins.int
     @property
     def speech_length(self) -> google.protobuf.duration_pb2.Duration:
         """Speech length from which the voiceprint was extracted."""
+
     @property
     def voiceprint(self) -> phonexia.grpc.common.core_pb2.Voiceprint:
         """Extracted voiceprint."""
+
     def __init__(
         self,
         *,
         speech_length: google.protobuf.duration_pb2.Duration | None = ...,
         voiceprint: phonexia.grpc.common.core_pb2.Voiceprint | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["speech_length", b"speech_length", "voiceprint", b"voiceprint"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["speech_length", b"speech_length", "voiceprint", b"voiceprint"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["speech_length", b"speech_length", "voiceprint", b"voiceprint"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["speech_length", b"speech_length", "voiceprint", b"voiceprint"]) -> None: ...
 
 global___ExtractResult = ExtractResult
 
-@typing_extensions.final
+@typing.final
 class ExtractResponse(google.protobuf.message.Message):
     """The top-level message returned to the client by the <code>Extract</code>
     method. It contains the result as zero or more <code>ExtractResult</code>
     messages.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     RESULT_FIELD_NUMBER: builtins.int
     PROCESSED_AUDIO_LENGTH_FIELD_NUMBER: builtins.int
     @property
     def result(self) -> global___ExtractResult:
         """Result containing the extracted voiceprint."""
+
     @property
     def processed_audio_length(self) -> google.protobuf.duration_pb2.Duration:
         """When available, total length of the processed audio.
         Set only if this is the last response in the stream.
         """
+
     def __init__(
         self,
         *,
         result: global___ExtractResult | None = ...,
         processed_audio_length: google.protobuf.duration_pb2.Duration | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["processed_audio_length", b"processed_audio_length", "result", b"result"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["processed_audio_length", b"processed_audio_length", "result", b"result"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["processed_audio_length", b"processed_audio_length", "result", b"result"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["processed_audio_length", b"processed_audio_length", "result", b"result"]) -> None: ...
 
 global___ExtractResponse = ExtractResponse
```

### Comparing `phonexia_grpc-1.5.0/phonexia/grpc/technologies/speaker_identification/v1/speaker_identification_pb2_grpc.py` & `phonexia_grpc-2.0.0/phonexia/grpc/technologies/speaker_identification/v1/speaker_identification_pb2_grpc.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,38 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
+import warnings
 
 from phonexia.grpc.technologies.speaker_identification.v1 import speaker_identification_pb2 as phonexia_dot_grpc_dot_technologies_dot_speaker__identification_dot_v1_dot_speaker__identification__pb2
 
+GRPC_GENERATED_VERSION = '1.63.0rc2'
+GRPC_VERSION = grpc.__version__
+EXPECTED_ERROR_RELEASE = '1.65.0'
+SCHEDULED_RELEASE_DATE = 'June 25, 2024'
+_version_not_supported = False
+
+try:
+    from grpc._utilities import first_version_is_lower
+    _version_not_supported = first_version_is_lower(GRPC_VERSION, GRPC_GENERATED_VERSION)
+except ImportError:
+    _version_not_supported = True
+
+if _version_not_supported:
+    warnings.warn(
+        f'The grpc package installed is at version {GRPC_VERSION},'
+        + f' but the generated code in phonexia/grpc/technologies/speaker_identification/v1/speaker_identification_pb2_grpc.py depends on'
+        + f' grpcio>={GRPC_GENERATED_VERSION}.'
+        + f' Please upgrade your grpc module to grpcio>={GRPC_GENERATED_VERSION}'
+        + f' or downgrade your generated code using grpcio-tools<={GRPC_VERSION}.'
+        + f' This warning will become an error in {EXPECTED_ERROR_RELEASE},'
+        + f' scheduled for release on {SCHEDULED_RELEASE_DATE}.',
+        RuntimeWarning
+    )
+
 
 class VoiceprintComparisonStub(object):
     """Service that implements voiceprint comparison.
     """
 
     def __init__(self, channel):
         """Constructor.
@@ -15,15 +40,15 @@
         Args:
             channel: A grpc.Channel.
         """
         self.Compare = channel.stream_stream(
                 '/phonexia.grpc.technologies.speaker_identification.v1.VoiceprintComparison/Compare',
                 request_serializer=phonexia_dot_grpc_dot_technologies_dot_speaker__identification_dot_v1_dot_speaker__identification__pb2.CompareRequest.SerializeToString,
                 response_deserializer=phonexia_dot_grpc_dot_technologies_dot_speaker__identification_dot_v1_dot_speaker__identification__pb2.CompareResponse.FromString,
-                )
+                _registered_method=True)
 
 
 class VoiceprintComparisonServicer(object):
     """Service that implements voiceprint comparison.
     """
 
     def Compare(self, request_iterator, context):
@@ -62,19 +87,29 @@
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.stream_stream(request_iterator, target, '/phonexia.grpc.technologies.speaker_identification.v1.VoiceprintComparison/Compare',
+        return grpc.experimental.stream_stream(
+            request_iterator,
+            target,
+            '/phonexia.grpc.technologies.speaker_identification.v1.VoiceprintComparison/Compare',
             phonexia_dot_grpc_dot_technologies_dot_speaker__identification_dot_v1_dot_speaker__identification__pb2.CompareRequest.SerializeToString,
             phonexia_dot_grpc_dot_technologies_dot_speaker__identification_dot_v1_dot_speaker__identification__pb2.CompareResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+            options,
+            channel_credentials,
+            insecure,
+            call_credentials,
+            compression,
+            wait_for_ready,
+            timeout,
+            metadata,
+            _registered_method=True)
 
 
 class VoiceprintExtractionStub(object):
     """Service that implements voiceprint extraction.
     """
 
     def __init__(self, channel):
@@ -83,15 +118,15 @@
         Args:
             channel: A grpc.Channel.
         """
         self.Extract = channel.stream_unary(
                 '/phonexia.grpc.technologies.speaker_identification.v1.VoiceprintExtraction/Extract',
                 request_serializer=phonexia_dot_grpc_dot_technologies_dot_speaker__identification_dot_v1_dot_speaker__identification__pb2.ExtractRequest.SerializeToString,
                 response_deserializer=phonexia_dot_grpc_dot_technologies_dot_speaker__identification_dot_v1_dot_speaker__identification__pb2.ExtractResponse.FromString,
-                )
+                _registered_method=True)
 
 
 class VoiceprintExtractionServicer(object):
     """Service that implements voiceprint extraction.
     """
 
     def Extract(self, request_iterator, context):
@@ -128,12 +163,22 @@
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.stream_unary(request_iterator, target, '/phonexia.grpc.technologies.speaker_identification.v1.VoiceprintExtraction/Extract',
+        return grpc.experimental.stream_unary(
+            request_iterator,
+            target,
+            '/phonexia.grpc.technologies.speaker_identification.v1.VoiceprintExtraction/Extract',
             phonexia_dot_grpc_dot_technologies_dot_speaker__identification_dot_v1_dot_speaker__identification__pb2.ExtractRequest.SerializeToString,
             phonexia_dot_grpc_dot_technologies_dot_speaker__identification_dot_v1_dot_speaker__identification__pb2.ExtractResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+            options,
+            channel_credentials,
+            insecure,
+            call_credentials,
+            compression,
+            wait_for_ready,
+            timeout,
+            metadata,
+            _registered_method=True)
```

### Comparing `phonexia_grpc-1.5.0/pypi-README.md` & `phonexia_grpc-2.0.0/pypi-README.md`

 * *Files identical despite different names*

### Comparing `phonexia_grpc-1.5.0/pyproject.toml` & `phonexia_grpc-2.0.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "phonexia-grpc"
-version = "1.5.0"
+version = "2.0.0"
 description = "Library for communication with microservices developed by phonexia using grpc application interface."
 readme = "pypi-README.md"
 keywords = ["grpc", "voice", "voice-biometry", "speech", "language", "STT", "whisper"]
 authors = ["Phonexia s.r.o. <info@phonexia.com>"]
 license = "Apache-2.0"
 packages = [
     { include = "phonexia" },
@@ -31,21 +31,21 @@
 [[tool.poetry.source]]
 name = "PyPI"
 priority = "default"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 grpcio = "^1.59.0"
-protobuf = "^4.25.1"
+protobuf = "^5.0.0"
 mypy-protobuf = "^3.5.0"
 grpc-stubs = "^1.53.0.2"
 
 [tool.poetry.group.dev.dependencies]
 grpcio-tools = "^1.59.2"
-ruff = "^0.3.0"
+ruff = "^0.4.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.setuptools.package-data]
 phonexia = ["py.typed"]
```

### Comparing `phonexia_grpc-1.5.0/PKG-INFO` & `phonexia_grpc-2.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phonexia-grpc
-Version: 1.5.0
+Version: 2.0.0
 Summary: Library for communication with microservices developed by phonexia using grpc application interface.
 License: Apache-2.0
 Keywords: grpc,voice,voice-biometry,speech,language,STT,whisper
 Author: Phonexia s.r.o.
 Author-email: info@phonexia.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: grpc-stubs (>=1.53.0.2,<2.0.0.0)
 Requires-Dist: grpcio (>=1.59.0,<2.0.0)
 Requires-Dist: mypy-protobuf (>=3.5.0,<4.0.0)
-Requires-Dist: protobuf (>=4.25.1,<5.0.0)
+Requires-Dist: protobuf (>=5.0.0,<6.0.0)
 Project-URL: Changelog, https://github.com/phonexia/protofiles/blob/main/CHANGELOG.md
 Project-URL: Homepage, https://phonexia.com
 Project-URL: Issues, https://phonexia.atlassian.net/servicedesk/customer/portal/15/group/20/create/40
 Project-URL: Source, https://github.com/phonexia/protofiles
 Description-Content-Type: text/markdown
 
 ![](https://www.phonexia.com/wp-content/uploads/phonexia-logo-transparent-500px.png)
```


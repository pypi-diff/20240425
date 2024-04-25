# Comparing `tmp/ovos_listener-0.0.2a9-py3-none-any.whl.zip` & `tmp/ovos_listener-0.0.3a1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,23 @@
-Zip file size: 5849 bytes, number of entries: 6
--rw-r--r--  2.0 unx    11423 b- defN 23-Apr-15 03:20 ovos_listener-0.0.2a9.dist-info/LICENSE.md
--rw-r--r--  2.0 unx     1067 b- defN 23-Apr-15 03:20 ovos_listener-0.0.2a9.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-15 03:20 ovos_listener-0.0.2a9.dist-info/WHEEL
--rw-r--r--  2.0 unx       63 b- defN 23-Apr-15 03:20 ovos_listener-0.0.2a9.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        1 b- defN 23-Apr-15 03:20 ovos_listener-0.0.2a9.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      532 b- defN 23-Apr-15 03:20 ovos_listener-0.0.2a9.dist-info/RECORD
-6 files, 13178 bytes uncompressed, 4871 bytes compressed:  63.0%
+Zip file size: 111523 bytes, number of entries: 21
+-rw-r--r--  2.0 unx    19240 b- defN 24-Apr-25 02:19 ovos_listener/__init__.py
+-rw-r--r--  2.0 unx     1408 b- defN 24-Apr-25 02:19 ovos_listener/__main__.py
+-rw-r--r--  2.0 unx     4853 b- defN 24-Apr-25 02:19 ovos_listener/arecord.py
+-rw-r--r--  2.0 unx     1853 b- defN 24-Apr-25 02:19 ovos_listener/data_structures.py
+-rw-r--r--  2.0 unx      433 b- defN 24-Apr-25 02:19 ovos_listener/hotword_factory.py
+-rw-r--r--  2.0 unx    19205 b- defN 24-Apr-25 02:19 ovos_listener/listener.py
+-rw-r--r--  2.0 unx    38858 b- defN 24-Apr-25 02:19 ovos_listener/mic.py
+-rw-r--r--  2.0 unx    16205 b- defN 24-Apr-25 02:19 ovos_listener/service.py
+-rw-r--r--  2.0 unx    14421 b- defN 24-Apr-25 02:19 ovos_listener/silence.py
+-rw-r--r--  2.0 unx      428 b- defN 24-Apr-25 02:19 ovos_listener/stt.py
+-rw-r--r--  2.0 unx     1340 b- defN 24-Apr-25 02:19 ovos_listener/utils.py
+-rw-r--r--  2.0 unx      114 b- defN 24-Apr-25 02:19 ovos_listener/version.py
+-rw-r--r--  2.0 unx     6268 b- defN 24-Apr-25 02:19 ovos_listener/res/snd/acknowledge.mp3
+-rw-r--r--  2.0 unx    13290 b- defN 24-Apr-25 02:19 ovos_listener/res/snd/error.mp3
+-rw-r--r--  2.0 unx    67090 b- defN 24-Apr-25 02:19 ovos_listener/res/snd/start_listening.wav
+-rw-r--r--  2.0 unx    11423 b- defN 24-Apr-25 02:19 ovos_listener-0.0.3a1.dist-info/LICENSE.md
+-rw-r--r--  2.0 unx      981 b- defN 24-Apr-25 02:19 ovos_listener-0.0.3a1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-25 02:19 ovos_listener-0.0.3a1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       63 b- defN 24-Apr-25 02:19 ovos_listener-0.0.3a1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       14 b- defN 24-Apr-25 02:19 ovos_listener-0.0.3a1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1797 b- defN 24-Apr-25 02:19 ovos_listener-0.0.3a1.dist-info/RECORD
+21 files, 219376 bytes uncompressed, 108593 bytes compressed:  50.5%
```

## zipnote {}

```diff
@@ -1,19 +1,64 @@
-Filename: ovos_listener-0.0.2a9.dist-info/LICENSE.md
+Filename: ovos_listener/__init__.py
 Comment: 
 
-Filename: ovos_listener-0.0.2a9.dist-info/METADATA
+Filename: ovos_listener/__main__.py
 Comment: 
 
-Filename: ovos_listener-0.0.2a9.dist-info/WHEEL
+Filename: ovos_listener/arecord.py
 Comment: 
 
-Filename: ovos_listener-0.0.2a9.dist-info/entry_points.txt
+Filename: ovos_listener/data_structures.py
 Comment: 
 
-Filename: ovos_listener-0.0.2a9.dist-info/top_level.txt
+Filename: ovos_listener/hotword_factory.py
 Comment: 
 
-Filename: ovos_listener-0.0.2a9.dist-info/RECORD
+Filename: ovos_listener/listener.py
+Comment: 
+
+Filename: ovos_listener/mic.py
+Comment: 
+
+Filename: ovos_listener/service.py
+Comment: 
+
+Filename: ovos_listener/silence.py
+Comment: 
+
+Filename: ovos_listener/stt.py
+Comment: 
+
+Filename: ovos_listener/utils.py
+Comment: 
+
+Filename: ovos_listener/version.py
+Comment: 
+
+Filename: ovos_listener/res/snd/acknowledge.mp3
+Comment: 
+
+Filename: ovos_listener/res/snd/error.mp3
+Comment: 
+
+Filename: ovos_listener/res/snd/start_listening.wav
+Comment: 
+
+Filename: ovos_listener-0.0.3a1.dist-info/LICENSE.md
+Comment: 
+
+Filename: ovos_listener-0.0.3a1.dist-info/METADATA
+Comment: 
+
+Filename: ovos_listener-0.0.3a1.dist-info/WHEEL
+Comment: 
+
+Filename: ovos_listener-0.0.3a1.dist-info/entry_points.txt
+Comment: 
+
+Filename: ovos_listener-0.0.3a1.dist-info/top_level.txt
+Comment: 
+
+Filename: ovos_listener-0.0.3a1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `ovos_listener-0.0.2a9.dist-info/LICENSE.md` & `ovos_listener-0.0.3a1.dist-info/LICENSE.md`

 * *Files identical despite different names*

## Comparing `ovos_listener-0.0.2a9.dist-info/METADATA` & `ovos_listener-0.0.3a1.dist-info/METADATA`

 * *Files 21% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 Metadata-Version: 2.1
 Name: ovos-listener
-Version: 0.0.2a9
+Version: 0.0.3a1
 Summary: ovos-core listener daemon client
 Home-page: https://github.com/OpenVoiceOS/ovos-listener
 Author: UNKNOWN
 Author-email: UNKNOWN
 License: Apache-2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
-Requires-Dist: SpeechRecognition (>=3.8.1)
-Requires-Dist: PyAudio (~=0.2)
+Requires-Dist: SpeechRecognition >=3.8.1
+Requires-Dist: PyAudio ~=0.2
 Requires-Dist: ovos-vad-plugin-webrtcvad
-Requires-Dist: ovos-ww-plugin-pocketsphinx (>=0.1.3,~=0.1)
-Requires-Dist: ovos-ww-plugin-precise-lite (>=0.1.2a3,~=0.1)
-Requires-Dist: ovos-ww-plugin-precise (>=0.1.1,~=0.1)
+Requires-Dist: ovos-ww-plugin-pocketsphinx >=0.1.3,~=0.1
+Requires-Dist: ovos-ww-plugin-precise-lite >=0.1.2,~=0.1
 Requires-Dist: ovos-ww-plugin-vosk
-Requires-Dist: ovos-stt-plugin-server (>=0.0.2,~=0.0)
-Requires-Dist: ovos-stt-plugin-vosk (~=0.1)
-Requires-Dist: ovos-utils (>=0.0.31a3,~=0.0)
-Requires-Dist: ovos-bus-client (>=0.0.3a16,~=0.0)
-Requires-Dist: ovos-plugin-manager (>=0.0.23a5,~=0.0)
-Requires-Dist: ovos-config (>=0.0.8a3,~=0.0)
-Requires-Dist: ovos-backend-client (>=0.0.7a2,~=0.0)
+Requires-Dist: ovos-stt-plugin-server >=0.0.2,~=0.0
+Requires-Dist: ovos-stt-plugin-vosk ~=0.1
+Requires-Dist: ovos-utils >=0.0.31,~=0.0
+Requires-Dist: ovos-bus-client >=0.0.3a16,~=0.0
+Requires-Dist: ovos-plugin-manager >=0.0.23,~=0.0
+Requires-Dist: ovos-config >=0.0.8,~=0.0
+Requires-Dist: ovos-backend-client >=0.0.7,~=0.0
 
 UNKNOWN
```


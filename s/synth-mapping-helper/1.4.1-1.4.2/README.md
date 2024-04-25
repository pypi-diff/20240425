# Comparing `tmp/synth_mapping_helper-1.4.1.tar.gz` & `tmp/synth_mapping_helper-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "synth_mapping_helper-1.4.1.tar", last modified: Sun Apr 21 13:45:18 2024, max compression
+gzip compressed data, was "synth_mapping_helper-1.4.2.tar", last modified: Thu Apr 25 20:21:50 2024, max compression
```

## Comparing `synth_mapping_helper-1.4.1.tar` & `synth_mapping_helper-1.4.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:45:18.812765 synth_mapping_helper-1.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-21 13:45:07.000000 synth_mapping_helper-1.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-21 13:45:07.000000 synth_mapping_helper-1.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5557 2024-04-21 13:45:18.812765 synth_mapping_helper-1.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2873 2024-04-21 13:45:07.000000 synth_mapping_helper-1.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-04-21 13:45:07.000000 synth_mapping_helper-1.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-21 13:45:18.812765 synth_mapping_helper-1.4.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:45:18.804765 synth_mapping_helper-1.4.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:45:18.808765 synth_mapping_helper-1.4.1/src/synth_mapping_helper/
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-21 13:45:07.000000 synth_mapping_helper-1.4.1/src/synth_mapping_helper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28847 2024-04-21 13:45:07.000000 synth_mapping_helper-1.4.1/src/synth_mapping_helper/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    28170 2024-04-21 13:45:07.000000 synth_mapping_helper-1.4.1/src/synth_mapping_helper/companion.py
--rw-r--r--   0 runner    (1001) docker     (127)    14573 2024-04-21 13:45:07.000000 synth_mapping_helper-1.4.1/src/synth_mapping_helper/finalize.py
--rw-r--r--   0 runner    (1001) docker     (127)     5849 2024-04-21 13:45:07.000000 synth_mapping_helper-1.4.1/src/synth_mapping_helper/gui.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:45:18.812765 synth_mapping_helper-1.4.1/src/synth_mapping_helper/gui_tabs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 13:45:07.000000 synth_mapping_helper-1.4.1/src/synth_mapping_helper/gui_tabs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3936 2024-04-21 13:45:07.000000 synth_mapping_helper-1.4.1/src/synth_mapping_helper/gui_tabs/autobackup.py
--rw-r--r--   0 runner    (1001) docker     (127)     8812 2024-04-21 13:45:07.000000 synth_mapping_helper-1.4.1/src/synth_mapping_helper/gui_tabs/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)    35909 2024-04-21 13:45:07.000000 synth_mapping_helper-1.4.1/src/synth_mapping_helper/gui_tabs/dashboard.py
--rw-r--r--   0 runner    (1001) docker     (127)    14431 2024-04-21 13:45:07.000000 synth_mapping_helper-1.4.1/src/synth_mapping_helper/gui_tabs/file_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-04-21 13:45:07.000000 synth_mapping_helper-1.4.1/src/synth_mapping_helper/gui_tabs/local_dir_picker.py
--rw-r--r--   0 runner    (1001) docker     (127)     8895 2024-04-21 13:45:07.000000 synth_mapping_helper-1.4.1/src/synth_mapping_helper/gui_tabs/map_render.py
--rw-r--r--   0 runner    (1001) docker     (127)    26721 2024-04-21 13:45:07.000000 synth_mapping_helper-1.4.1/src/synth_mapping_helper/gui_tabs/stacking.py
--rw-r--r--   0 runner    (1001) docker     (127)    18510 2024-04-21 13:45:07.000000 synth_mapping_helper-1.4.1/src/synth_mapping_helper/gui_tabs/text_gen.py
--rw-r--r--   0 runner    (1001) docker     (127)     3426 2024-04-21 13:45:07.000000 synth_mapping_helper-1.4.1/src/synth_mapping_helper/gui_tabs/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3478 2024-04-21 13:45:07.000000 synth_mapping_helper-1.4.1/src/synth_mapping_helper/gui_tabs/version.py
--rw-r--r--   0 runner    (1001) docker     (127)    41790 2024-04-21 13:45:07.000000 synth_mapping_helper-1.4.1/src/synth_mapping_helper/gui_tabs/wall_art.py
--rw-r--r--   0 runner    (1001) docker     (127)     5805 2024-04-21 13:45:07.000000 synth_mapping_helper-1.4.1/src/synth_mapping_helper/movement.py
--rw-r--r--   0 runner    (1001) docker     (127)     8139 2024-04-21 13:45:07.000000 synth_mapping_helper-1.4.1/src/synth_mapping_helper/pattern_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)    15230 2024-04-21 13:45:07.000000 synth_mapping_helper-1.4.1/src/synth_mapping_helper/rails.py
--rw-r--r--   0 runner    (1001) docker     (127)    27884 2024-04-21 13:45:07.000000 synth_mapping_helper-1.4.1/src/synth_mapping_helper/synth_format.py
--rw-r--r--   0 runner    (1001) docker     (127)     5006 2024-04-21 13:45:07.000000 synth_mapping_helper-1.4.1/src/synth_mapping_helper/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:45:18.812765 synth_mapping_helper-1.4.1/src/synth_mapping_helper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5557 2024-04-21 13:45:18.000000 synth_mapping_helper-1.4.1/src/synth_mapping_helper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-04-21 13:45:18.000000 synth_mapping_helper-1.4.1/src/synth_mapping_helper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 13:45:18.000000 synth_mapping_helper-1.4.1/src/synth_mapping_helper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-21 13:45:18.000000 synth_mapping_helper-1.4.1/src/synth_mapping_helper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-21 13:45:18.000000 synth_mapping_helper-1.4.1/src/synth_mapping_helper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-21 13:45:18.000000 synth_mapping_helper-1.4.1/src/synth_mapping_helper.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:45:18.812765 synth_mapping_helper-1.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-21 13:45:07.000000 synth_mapping_helper-1.4.1/tests/test_synth_format.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:21:50.248148 synth_mapping_helper-1.4.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-25 20:21:34.000000 synth_mapping_helper-1.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-25 20:21:34.000000 synth_mapping_helper-1.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5557 2024-04-25 20:21:50.248148 synth_mapping_helper-1.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2873 2024-04-25 20:21:34.000000 synth_mapping_helper-1.4.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-04-25 20:21:34.000000 synth_mapping_helper-1.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-25 20:21:50.252148 synth_mapping_helper-1.4.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:21:50.244148 synth_mapping_helper-1.4.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:21:50.244148 synth_mapping_helper-1.4.2/src/synth_mapping_helper/
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-25 20:21:34.000000 synth_mapping_helper-1.4.2/src/synth_mapping_helper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28847 2024-04-25 20:21:34.000000 synth_mapping_helper-1.4.2/src/synth_mapping_helper/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28170 2024-04-25 20:21:34.000000 synth_mapping_helper-1.4.2/src/synth_mapping_helper/companion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14573 2024-04-25 20:21:34.000000 synth_mapping_helper-1.4.2/src/synth_mapping_helper/finalize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5849 2024-04-25 20:21:34.000000 synth_mapping_helper-1.4.2/src/synth_mapping_helper/gui.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:21:50.248148 synth_mapping_helper-1.4.2/src/synth_mapping_helper/gui_tabs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 20:21:34.000000 synth_mapping_helper-1.4.2/src/synth_mapping_helper/gui_tabs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3936 2024-04-25 20:21:34.000000 synth_mapping_helper-1.4.2/src/synth_mapping_helper/gui_tabs/autobackup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8812 2024-04-25 20:21:34.000000 synth_mapping_helper-1.4.2/src/synth_mapping_helper/gui_tabs/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35909 2024-04-25 20:21:34.000000 synth_mapping_helper-1.4.2/src/synth_mapping_helper/gui_tabs/dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14431 2024-04-25 20:21:34.000000 synth_mapping_helper-1.4.2/src/synth_mapping_helper/gui_tabs/file_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-04-25 20:21:34.000000 synth_mapping_helper-1.4.2/src/synth_mapping_helper/gui_tabs/local_dir_picker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8895 2024-04-25 20:21:34.000000 synth_mapping_helper-1.4.2/src/synth_mapping_helper/gui_tabs/map_render.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26721 2024-04-25 20:21:34.000000 synth_mapping_helper-1.4.2/src/synth_mapping_helper/gui_tabs/stacking.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18510 2024-04-25 20:21:34.000000 synth_mapping_helper-1.4.2/src/synth_mapping_helper/gui_tabs/text_gen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3426 2024-04-25 20:21:34.000000 synth_mapping_helper-1.4.2/src/synth_mapping_helper/gui_tabs/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3478 2024-04-25 20:21:34.000000 synth_mapping_helper-1.4.2/src/synth_mapping_helper/gui_tabs/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41790 2024-04-25 20:21:34.000000 synth_mapping_helper-1.4.2/src/synth_mapping_helper/gui_tabs/wall_art.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5805 2024-04-25 20:21:34.000000 synth_mapping_helper-1.4.2/src/synth_mapping_helper/movement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8139 2024-04-25 20:21:34.000000 synth_mapping_helper-1.4.2/src/synth_mapping_helper/pattern_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15230 2024-04-25 20:21:34.000000 synth_mapping_helper-1.4.2/src/synth_mapping_helper/rails.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28593 2024-04-25 20:21:34.000000 synth_mapping_helper-1.4.2/src/synth_mapping_helper/synth_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5006 2024-04-25 20:21:34.000000 synth_mapping_helper-1.4.2/src/synth_mapping_helper/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:21:50.248148 synth_mapping_helper-1.4.2/src/synth_mapping_helper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5557 2024-04-25 20:21:50.000000 synth_mapping_helper-1.4.2/src/synth_mapping_helper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-04-25 20:21:50.000000 synth_mapping_helper-1.4.2/src/synth_mapping_helper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 20:21:50.000000 synth_mapping_helper-1.4.2/src/synth_mapping_helper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-25 20:21:50.000000 synth_mapping_helper-1.4.2/src/synth_mapping_helper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-25 20:21:50.000000 synth_mapping_helper-1.4.2/src/synth_mapping_helper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-25 20:21:50.000000 synth_mapping_helper-1.4.2/src/synth_mapping_helper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:21:50.248148 synth_mapping_helper-1.4.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-25 20:21:34.000000 synth_mapping_helper-1.4.2/tests/test_synth_format.py
```

### Comparing `synth_mapping_helper-1.4.1/LICENSE` & `synth_mapping_helper-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `synth_mapping_helper-1.4.1/PKG-INFO` & `synth_mapping_helper-1.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synth_mapping_helper
-Version: 1.4.1
+Version: 1.4.2
 Summary: Toolbox for manipulating the JSON-Format used by Synth Riders Beatmap Editor in the clipboard
 Author: adosikas
 License: MIT License
         
         Copyright (c) 2024 adosikas
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `synth_mapping_helper-1.4.1/README.md` & `synth_mapping_helper-1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `synth_mapping_helper-1.4.1/pyproject.toml` & `synth_mapping_helper-1.4.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `synth_mapping_helper-1.4.1/src/synth_mapping_helper/cli.py` & `synth_mapping_helper-1.4.2/src/synth_mapping_helper/cli.py`

 * *Files identical despite different names*

### Comparing `synth_mapping_helper-1.4.1/src/synth_mapping_helper/companion.py` & `synth_mapping_helper-1.4.2/src/synth_mapping_helper/companion.py`

 * *Files identical despite different names*

### Comparing `synth_mapping_helper-1.4.1/src/synth_mapping_helper/finalize.py` & `synth_mapping_helper-1.4.2/src/synth_mapping_helper/finalize.py`

 * *Files identical despite different names*

### Comparing `synth_mapping_helper-1.4.1/src/synth_mapping_helper/gui.py` & `synth_mapping_helper-1.4.2/src/synth_mapping_helper/gui.py`

 * *Files identical despite different names*

### Comparing `synth_mapping_helper-1.4.1/src/synth_mapping_helper/gui_tabs/autobackup.py` & `synth_mapping_helper-1.4.2/src/synth_mapping_helper/gui_tabs/autobackup.py`

 * *Files identical despite different names*

### Comparing `synth_mapping_helper-1.4.1/src/synth_mapping_helper/gui_tabs/commands.py` & `synth_mapping_helper-1.4.2/src/synth_mapping_helper/gui_tabs/commands.py`

 * *Files identical despite different names*

### Comparing `synth_mapping_helper-1.4.1/src/synth_mapping_helper/gui_tabs/dashboard.py` & `synth_mapping_helper-1.4.2/src/synth_mapping_helper/gui_tabs/dashboard.py`

 * *Files identical despite different names*

### Comparing `synth_mapping_helper-1.4.1/src/synth_mapping_helper/gui_tabs/file_utils.py` & `synth_mapping_helper-1.4.2/src/synth_mapping_helper/gui_tabs/file_utils.py`

 * *Files identical despite different names*

### Comparing `synth_mapping_helper-1.4.1/src/synth_mapping_helper/gui_tabs/local_dir_picker.py` & `synth_mapping_helper-1.4.2/src/synth_mapping_helper/gui_tabs/local_dir_picker.py`

 * *Files identical despite different names*

### Comparing `synth_mapping_helper-1.4.1/src/synth_mapping_helper/gui_tabs/map_render.py` & `synth_mapping_helper-1.4.2/src/synth_mapping_helper/gui_tabs/map_render.py`

 * *Files identical despite different names*

### Comparing `synth_mapping_helper-1.4.1/src/synth_mapping_helper/gui_tabs/stacking.py` & `synth_mapping_helper-1.4.2/src/synth_mapping_helper/gui_tabs/stacking.py`

 * *Files identical despite different names*

### Comparing `synth_mapping_helper-1.4.1/src/synth_mapping_helper/gui_tabs/text_gen.py` & `synth_mapping_helper-1.4.2/src/synth_mapping_helper/gui_tabs/text_gen.py`

 * *Files identical despite different names*

### Comparing `synth_mapping_helper-1.4.1/src/synth_mapping_helper/gui_tabs/utils.py` & `synth_mapping_helper-1.4.2/src/synth_mapping_helper/gui_tabs/utils.py`

 * *Files identical despite different names*

### Comparing `synth_mapping_helper-1.4.1/src/synth_mapping_helper/gui_tabs/version.py` & `synth_mapping_helper-1.4.2/src/synth_mapping_helper/gui_tabs/version.py`

 * *Files identical despite different names*

### Comparing `synth_mapping_helper-1.4.1/src/synth_mapping_helper/gui_tabs/wall_art.py` & `synth_mapping_helper-1.4.2/src/synth_mapping_helper/gui_tabs/wall_art.py`

 * *Files identical despite different names*

### Comparing `synth_mapping_helper-1.4.1/src/synth_mapping_helper/movement.py` & `synth_mapping_helper-1.4.2/src/synth_mapping_helper/movement.py`

 * *Files identical despite different names*

### Comparing `synth_mapping_helper-1.4.1/src/synth_mapping_helper/pattern_generation.py` & `synth_mapping_helper-1.4.2/src/synth_mapping_helper/pattern_generation.py`

 * *Files identical despite different names*

### Comparing `synth_mapping_helper-1.4.1/src/synth_mapping_helper/rails.py` & `synth_mapping_helper-1.4.2/src/synth_mapping_helper/rails.py`

 * *Files identical despite different names*

### Comparing `synth_mapping_helper-1.4.1/src/synth_mapping_helper/synth_format.py` & `synth_mapping_helper-1.4.2/src/synth_mapping_helper/synth_format.py`

 * *Files 2% similar despite different names*

```diff
@@ -144,14 +144,26 @@
     return r64 if abs(time-r64) <= abs(time-r48) else round(r48, 11)
 
 def round_tick_for_json_index(time: float) -> float | int:
     # same as above, but for notes dict, which uses int when possible
     if time.is_integer():
         return int(time)
     return round_tick_for_json(time)
+
+# Hacky classes used to trick ZipFile._open_to_write
+class _TrueInt(int):
+    # this makes it think there are already flags, so it doesn't add "permissions: ?rw-------"
+    def __bool__(self):
+        return True
+class _NonAsciiStr(str):
+    # this makes it think the filename is not ascii, so it adds the UTF8 flag
+    def encode(self, encoding: str = None) -> bytes:
+        if encoding == "ascii":
+            raise UnicodeEncodeError(encoding, self, 0, 0, "dummy error to trick ZipFile._open_to_write")
+        return super().encode(encoding=encoding)
     
 
 @dataclasses.dataclass
 class DataContainer:
     bpm: float = 60.0
     right: SINGLE_COLOR_NOTES = dataclasses.field(default_factory=dict)
     left: SINGLE_COLOR_NOTES = dataclasses.field(default_factory=dict)
@@ -362,22 +374,14 @@
                 if diff_removed:
                     self.errors[diff] = diff_removed
 
     def save_as(self, output_file: Union[Path, BytesIO]) -> None:
         out_buffer = output_file if isinstance(output_file, BytesIO) else BytesIO()  # buffer output zip file in memory, only write on success
         in_bio = self.input_file if isinstance(self.input_file, BytesIO) else BytesIO(self.input_file.read_bytes())
         with ZipFile(in_bio) as inzip, ZipFile(out_buffer, "w") as outzip:
-            # copy all content except beatmap json
-            outzip.comment = inzip.comment
-            for info in inzip.infolist():
-                if info.filename == BEATMAP_JSON_FILE:
-                    beatmap_info = info
-                else:
-                    outzip.writestr(info, inzip.read(info.filename))
-
             beatmap = json.loads(inzip.read(BEATMAP_JSON_FILE))
             beatmap["BPM"] = self.bpm
             beatmap["Offset"] = self.offset_ms
             beatmap["ModifiedTime"] = int(time.time())
 
             beatmap["Bookmarks"]["BookmarksList"] = [
                 {"time": round_tick_for_json(t * 64), "name": n}
@@ -412,15 +416,26 @@
                 for t, wall_list in walls.items():
                     beatmap[t.capitalize()][diff] = wall_list
                 beatmap["Lights"][diff] = [round_tick_for_json(t * 64) for t in data.lights]
                 beatmap["Effects"][diff] = [round_tick_for_json(t * 64) for t in data.effects]
 
             # write modified beatmap json, in a way that closely mirrors the editor
             beatmap_json = json.dumps(beatmap, indent=2, allow_nan=False)
-            outzip.writestr(beatmap_info, codecs.BOM_UTF8 + beatmap_json.encode("utf-8").replace(b"\n", b"\r\n"))
+        
+            # copy all content verbatim except beatmap json
+            outzip.comment = inzip.comment
+            for info in inzip.infolist():
+                # trick write logic to make output work on Quest
+                info.external_attr = _TrueInt(0)
+                info.filename = _NonAsciiStr(info.filename)
+
+                if info.filename == BEATMAP_JSON_FILE:
+                    outzip.writestr(info, codecs.BOM_UTF8 + beatmap_json.encode("utf-8").replace(b"\n", b"\r\n"))
+                else:
+                    outzip.writestr(info, inzip.read(info.filename))
         # write output zip
         if isinstance(output_file, BytesIO):
             output_file.seek(0)
         else:
             output_file.write_bytes(out_buffer.getbuffer())
 
     def change_bpm(self, bpm: float) -> None:
```

### Comparing `synth_mapping_helper-1.4.1/src/synth_mapping_helper/utils.py` & `synth_mapping_helper-1.4.2/src/synth_mapping_helper/utils.py`

 * *Files identical despite different names*

### Comparing `synth_mapping_helper-1.4.1/src/synth_mapping_helper.egg-info/PKG-INFO` & `synth_mapping_helper-1.4.2/src/synth_mapping_helper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synth_mapping_helper
-Version: 1.4.1
+Version: 1.4.2
 Summary: Toolbox for manipulating the JSON-Format used by Synth Riders Beatmap Editor in the clipboard
 Author: adosikas
 License: MIT License
         
         Copyright (c) 2024 adosikas
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `synth_mapping_helper-1.4.1/src/synth_mapping_helper.egg-info/SOURCES.txt` & `synth_mapping_helper-1.4.2/src/synth_mapping_helper.egg-info/SOURCES.txt`

 * *Files identical despite different names*


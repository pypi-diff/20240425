# Comparing `tmp/eosets-0.2.0.tar.gz` & `tmp/eosets-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eosets-0.2.0.tar", last modified: Wed Apr 24 13:17:47 2024, max compression
+gzip compressed data, was "eosets-0.2.1.tar", last modified: Thu Apr 25 13:47:51 2024, max compression
```

## Comparing `eosets-0.2.0.tar` & `eosets-0.2.1.tar`

### file list

```diff
@@ -1,25 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:17:47.578109 eosets-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)    10166 2024-04-24 13:17:39.000000 eosets-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-24 13:17:39.000000 eosets-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-04-24 13:17:39.000000 eosets-0.2.0/NOTICE
--rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-04-24 13:17:47.578109 eosets-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      787 2024-04-24 13:17:39.000000 eosets-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:17:47.574109 eosets-0.2.0/eosets/
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-24 13:17:39.000000 eosets-0.2.0/eosets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-04-24 13:17:39.000000 eosets-0.2.0/eosets/__meta__.py
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-24 13:17:39.000000 eosets-0.2.0/eosets/env_vars.py
--rw-r--r--   0 runner    (1001) docker     (127)      933 2024-04-24 13:17:39.000000 eosets-0.2.0/eosets/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    17577 2024-04-24 13:17:39.000000 eosets-0.2.0/eosets/mosaic.py
--rw-r--r--   0 runner    (1001) docker     (127)    19829 2024-04-24 13:17:39.000000 eosets-0.2.0/eosets/pair.py
--rw-r--r--   0 runner    (1001) docker     (127)    16006 2024-04-24 13:17:39.000000 eosets-0.2.0/eosets/series.py
--rw-r--r--   0 runner    (1001) docker     (127)    13465 2024-04-24 13:17:39.000000 eosets-0.2.0/eosets/set.py
--rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-24 13:17:39.000000 eosets-0.2.0/eosets/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:17:47.578109 eosets-0.2.0/eosets.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-04-24 13:17:47.000000 eosets-0.2.0/eosets.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-24 13:17:47.000000 eosets-0.2.0/eosets.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 13:17:47.000000 eosets-0.2.0/eosets.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-24 13:17:47.000000 eosets-0.2.0/eosets.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-24 13:17:47.000000 eosets-0.2.0/eosets.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-24 13:17:39.000000 eosets-0.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-24 13:17:47.578109 eosets-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-04-24 13:17:39.000000 eosets-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:47:51.100788 eosets-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    10166 2024-04-25 13:47:43.000000 eosets-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-25 13:47:43.000000 eosets-0.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-04-25 13:47:43.000000 eosets-0.2.1/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-04-25 13:47:51.104788 eosets-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-04-25 13:47:43.000000 eosets-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:47:51.100788 eosets-0.2.1/ci/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-25 13:47:43.000000 eosets-0.2.1/ci/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2943 2024-04-25 13:47:43.000000 eosets-0.2.1/ci/scripts_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2744 2024-04-25 13:47:43.000000 eosets-0.2.1/ci/test_mosaic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3936 2024-04-25 13:47:43.000000 eosets-0.2.1/ci/test_pair.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2840 2024-04-25 13:47:43.000000 eosets-0.2.1/ci/test_series.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:47:51.100788 eosets-0.2.1/eosets/
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-25 13:47:43.000000 eosets-0.2.1/eosets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-04-25 13:47:43.000000 eosets-0.2.1/eosets/__meta__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-25 13:47:43.000000 eosets-0.2.1/eosets/env_vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2024-04-25 13:47:43.000000 eosets-0.2.1/eosets/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17570 2024-04-25 13:47:43.000000 eosets-0.2.1/eosets/mosaic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19888 2024-04-25 13:47:43.000000 eosets-0.2.1/eosets/pair.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15999 2024-04-25 13:47:43.000000 eosets-0.2.1/eosets/series.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13464 2024-04-25 13:47:43.000000 eosets-0.2.1/eosets/set.py
+-rw-r--r--   0 runner    (1001) docker     (127)      879 2024-04-25 13:47:43.000000 eosets-0.2.1/eosets/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:47:51.100788 eosets-0.2.1/eosets.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-04-25 13:47:51.000000 eosets-0.2.1/eosets.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-25 13:47:51.000000 eosets-0.2.1/eosets.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 13:47:51.000000 eosets-0.2.1/eosets.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-25 13:47:51.000000 eosets-0.2.1/eosets.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-25 13:47:51.000000 eosets-0.2.1/eosets.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-25 13:47:43.000000 eosets-0.2.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-25 13:47:51.104788 eosets-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-04-25 13:47:43.000000 eosets-0.2.1/setup.py
```

### Comparing `eosets-0.2.0/LICENSE` & `eosets-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `eosets-0.2.0/NOTICE` & `eosets-0.2.1/NOTICE`

 * *Files identical despite different names*

### Comparing `eosets-0.2.0/PKG-INFO` & `eosets-0.2.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eosets
-Version: 0.2.0
+Version: 0.2.1
 Summary: This library aims to simplify any process working with different sets of EO data handled by EOReader.
 Home-page: UNKNOWN
 Author: ICube-SERTIT
 Author-email: dev-sertit@unistra.fr
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/sertit/eosets/issues/
 Project-URL: Documentation, https://eosets.readthedocs.io/en/latest/
```

### Comparing `eosets-0.2.0/README.md` & `eosets-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `eosets-0.2.0/eosets/__init__.py` & `eosets-0.2.1/eosets/__init__.py`

 * *Files identical despite different names*

### Comparing `eosets-0.2.0/eosets/__meta__.py` & `eosets-0.2.1/eosets/__meta__.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """
 **EOSets** library
 """
-__version__ = "0.2.0"
+__version__ = "0.2.1"
 __title__ = "eosets"
 __description__ = "This library aims to simplify any process working with different sets of EO data handled by EOReader."
 __author__ = "ICube-SERTIT"
 __author_email__ = "dev-sertit@unistra.fr"
 __url__ = "https://github.com/sertit/eosets"
 __license__ = "Apache 2.0"
 __copyright__ = "Copyright 2023, SERTIT-ICube - France, https://sertit.unistra.fr/"
```

### Comparing `eosets-0.2.0/eosets/env_vars.py` & `eosets-0.2.1/eosets/env_vars.py`

 * *Files identical despite different names*

### Comparing `eosets-0.2.0/eosets/exceptions.py` & `eosets-0.2.1/eosets/exceptions.py`

 * *Files identical despite different names*

### Comparing `eosets-0.2.0/eosets/mosaic.py` & `eosets-0.2.1/eosets/mosaic.py`

 * *Files 0% similar despite different names*

```diff
@@ -461,15 +461,15 @@
         band_ds = self.load(bands, pixel_size=pixel_size, **kwargs)
 
         # Stack bands
         if save_as_int:
             nodata = kwargs.get("nodata", UINT16_NODATA)
         else:
             nodata = kwargs.get("nodata", self.nodata)
-        stk, dtype = stack(bands, band_ds, save_as_int, nodata, **kwargs)
+        stk, dtype = stack(band_ds, save_as_int, nodata, **kwargs)
 
         # Update stack's attributes
         stk = self._update_attrs(stk, bands, **kwargs)
 
         # Write on disk
         if stack_path:
             LOGGER.debug("Saving stack")
```

### Comparing `eosets-0.2.0/eosets/pair.py` & `eosets-0.2.1/eosets/pair.py`

 * *Files 1% similar despite different names*

```diff
@@ -329,35 +329,29 @@
         window = kwargs.pop("window", self.footprint())
 
         # Load reference bands
         ref_ds: xr.Dataset = self.reference_mosaic.load(
             ref_bands_to_load, pixel_size=pixel_size, window=window, **kwargs
         )
 
-        ref_ds = ref_ds.drop_vars(
-            [band for band in ref_ds.keys() if band not in reference_bands]
-        )
-
-        ref_ds = self._update_xds_attrs(ref_ds, reference_bands)
-
         # Load secondary bands
         if self.has_secondary:
             sec_ds: xr.Dataset = self.secondary_mosaic.load(
                 sec_bands_to_load, pixel_size=pixel_size, window=window, **kwargs
             )
 
             # Load diff bands
             diff_dict = {}
             for band in diff_bands:
                 diff_path, exists = self._get_out_path(
                     f"{self.condensed_name}_d{to_str(band)[0]}.tif"
                 )
                 if exists:
                     diff_arr = read(
-                        path=diff_path,
+                        diff_path,
                         pixel_size=pixel_size,
                         resampling=resampling,
                         **kwargs,
                     )
                 else:
                     f"*** Loading d{to_str(band)} for {self.condensed_name} ***"
                     ref_arr = ref_ds[band]
@@ -386,15 +380,15 @@
                     write(diff_arr, diff_path)
 
                 diff_dict[band] = diff_arr
 
             # Collocate diff bands
             diff_dict = self._collocate_bands(diff_dict)
 
-            # Drop not wanted bands from reference and secondary datasets
+            # Drop not wanted bands from secondary dataset
             sec_ds = sec_ds.drop_vars(
                 [band for band in sec_ds.keys() if band not in secondary_bands]
             )
 
             # Create diff dataset
             coords = None
             if diff_dict:
@@ -408,14 +402,22 @@
             # Update attributes
             sec_ds = self._update_xds_attrs(sec_ds, secondary_bands)
             diff_ds = self._update_xds_attrs(diff_ds, diff_bands)
         else:
             sec_ds = xr.Dataset()
             diff_ds = xr.Dataset()
 
+        # Update reference dataset
+        # Drop not wanted bands from reference dataset
+        ref_ds = ref_ds.drop_vars(
+            [band for band in ref_ds.keys() if band not in reference_bands]
+        )
+
+        ref_ds = self._update_xds_attrs(ref_ds, reference_bands)
+
         return ref_ds, sec_ds, diff_ds
 
     def _update_attrs_constellation_specific(
         self, xarr: xr.DataArray, bands: list, **kwargs
     ) -> xr.DataArray:
         """
         Update attributes of the given array (constellation specific)
@@ -515,15 +517,15 @@
         band_ds = xr.merge([ref_ds, sec_ds, diff_ds])
 
         # Stack bands
         if save_as_int:
             nodata = kwargs.get("nodata", UINT16_NODATA)
         else:
             nodata = kwargs.get("nodata", self.nodata)
-        stk, dtype = stack(all_bands, band_ds, save_as_int, nodata, **kwargs)
+        stk, dtype = stack(band_ds, save_as_int, nodata, **kwargs)
 
         # Update stack's attributes
         stk = self._update_attrs(stk, all_bands, **kwargs)
 
         # Write on disk
         if stack_path:
             LOGGER.debug("Saving stack")
```

### Comparing `eosets-0.2.0/eosets/series.py` & `eosets-0.2.1/eosets/series.py`

 * *Files 0% similar despite different names*

```diff
@@ -434,15 +434,15 @@
                 )
 
         # Stack bands
         if save_as_int:
             nodata = kwargs.get("nodata", UINT16_NODATA)
         else:
             nodata = kwargs.get("nodata", self.nodata)
-        stk, dtype = stack(bands, band_ds, save_as_int, nodata, **kwargs)
+        stk, dtype = stack(band_ds, save_as_int, nodata, **kwargs)
 
         # Update stack's attributes
         stk = self._update_attrs(stk, new_bands, **kwargs)
 
         # Write on disk
         if stack_path:
             LOGGER.debug("Saving stack")
```

### Comparing `eosets-0.2.0/eosets/set.py` & `eosets-0.2.1/eosets/set.py`

 * *Files 0% similar despite different names*

```diff
@@ -188,15 +188,15 @@
         old_tmp_process = self._tmp_process
         self._set_tmp_process()
 
         # Update for every sets
         self._manage_output()
 
         # Move all files from old process folder into the new one
-        for file in files.listdir_abspath(old_tmp_process):
+        for file in path.listdir_abspath(old_tmp_process):
             try:
                 shutil.move(str(file), self._tmp_process)
             except shutil.Error:
                 # Don't overwrite file
                 pass
 
         # Remove old output if existing into the new output
```

### Comparing `eosets-0.2.0/eosets/utils.py` & `eosets-0.2.1/eosets/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,8 +19,8 @@
 from eoreader import utils
 from sertit import types
 
 AnyPathType = types.AnyPathType
 
 read = utils.read
 write = utils.write
-stack = utils.stack_dict
+stack = utils.stack
```

### Comparing `eosets-0.2.0/eosets.egg-info/PKG-INFO` & `eosets-0.2.1/eosets.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eosets
-Version: 0.2.0
+Version: 0.2.1
 Summary: This library aims to simplify any process working with different sets of EO data handled by EOReader.
 Home-page: UNKNOWN
 Author: ICube-SERTIT
 Author-email: dev-sertit@unistra.fr
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/sertit/eosets/issues/
 Project-URL: Documentation, https://eosets.readthedocs.io/en/latest/
```

### Comparing `eosets-0.2.0/setup.py` & `eosets-0.2.1/setup.py`

 * *Files identical despite different names*


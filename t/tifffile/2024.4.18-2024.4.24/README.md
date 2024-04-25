# Comparing `tmp/tifffile-2024.4.18.tar.gz` & `tmp/tifffile-2024.4.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tifffile-2024.4.18.tar", last modified: Thu Apr 18 02:07:18 2024, max compression
+gzip compressed data, was "tifffile-2024.4.24.tar", last modified: Thu Apr 25 03:05:10 2024, max compression
```

## Comparing `tifffile-2024.4.18.tar` & `tifffile-2024.4.24.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2024-04-18 02:07:18.260378 tifffile-2024.4.18/
--rw-rw-rw-   0        0        0      324 2019-07-10 16:43:27.000000 tifffile-2024.4.18/ACKNOWLEDGEMENTS.rst
--rw-rw-rw-   0        0        0    37954 2024-04-18 02:07:16.000000 tifffile-2024.4.18/CHANGES.rst
--rw-rw-rw-   0        0        0     1559 2024-04-18 02:07:16.000000 tifffile-2024.4.18/LICENSE
--rw-rw-rw-   0        0        0      569 2023-08-11 02:48:51.000000 tifffile-2024.4.18/MANIFEST.in
--rw-rw-rw-   0        0        0    31748 2024-04-18 02:07:18.260378 tifffile-2024.4.18/PKG-INFO
--rw-rw-rw-   0        0        0    30506 2024-04-18 02:07:16.000000 tifffile-2024.4.18/README.rst
-drwxrwxrwx   0        0        0        0 2024-04-18 02:07:18.260378 tifffile-2024.4.18/docs/
-drwxrwxrwx   0        0        0        0 2024-04-18 02:07:18.260378 tifffile-2024.4.18/docs/_static/
--rw-rw-rw-   0        0        0      127 2022-05-28 19:33:31.000000 tifffile-2024.4.18/docs/_static/custom.css
--rw-rw-rw-   0        0        0     1098 2023-12-25 06:05:35.000000 tifffile-2024.4.18/docs/conf.py
--rw-rw-rw-   0        0        0     3644 2023-08-12 18:29:44.000000 tifffile-2024.4.18/docs/make.py
-drwxrwxrwx   0        0        0        0 2024-04-18 02:07:18.260378 tifffile-2024.4.18/examples/
--rw-rw-rw-   0        0        0    15113 2024-02-12 18:46:43.000000 tifffile-2024.4.18/examples/earthbigdata.py
--rw-rw-rw-   0        0        0     2542 2024-01-28 18:02:54.000000 tifffile-2024.4.18/examples/issue125.py
--rw-rw-rw-   0        0        0       42 2024-04-18 02:07:18.260378 tifffile-2024.4.18/setup.cfg
--rw-rw-rw-   0        0        0     3936 2023-10-18 16:48:53.000000 tifffile-2024.4.18/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-18 02:07:18.260378 tifffile-2024.4.18/tests/
--rw-rw-rw-   0        0        0     1603 2023-08-30 07:20:06.000000 tifffile-2024.4.18/tests/conftest.py
--rw-rw-rw-   0        0        0   744257 2024-04-18 01:23:55.000000 tifffile-2024.4.18/tests/test_tifffile.py
-drwxrwxrwx   0        0        0        0 2024-04-18 02:07:18.260378 tifffile-2024.4.18/tifffile/
--rw-rw-rw-   0        0        0      110 2024-01-28 01:29:32.000000 tifffile-2024.4.18/tifffile/__init__.py
--rw-rw-rw-   0        0        0      135 2020-01-01 02:31:36.000000 tifffile-2024.4.18/tifffile/__main__.py
--rw-rw-rw-   0        0        0    11827 2024-01-29 05:07:27.000000 tifffile-2024.4.18/tifffile/_imagecodecs.py
--rw-rw-rw-   0        0        0    61794 2023-07-03 00:17:39.000000 tifffile-2024.4.18/tifffile/geodb.py
--rw-rw-rw-   0        0        0      680 2023-07-03 00:17:47.000000 tifffile-2024.4.18/tifffile/lsm2bin.py
--rw-rw-rw-   0        0        0     5904 2024-01-29 17:41:17.000000 tifffile-2024.4.18/tifffile/numcodecs.py
--rw-rw-rw-   0        0        0        0 2023-08-11 00:10:50.000000 tifffile-2024.4.18/tifffile/py.typed
--rw-rw-rw-   0        0        0     2410 2023-07-03 00:18:03.000000 tifffile-2024.4.18/tifffile/tiff2fsspec.py
--rw-rw-rw-   0        0        0     1437 2023-07-03 00:18:11.000000 tifffile-2024.4.18/tifffile/tiffcomment.py
--rw-rw-rw-   0        0        0   888468 2024-04-18 01:45:15.000000 tifffile-2024.4.18/tifffile/tifffile.py
-drwxrwxrwx   0        0        0        0 2024-04-18 02:07:18.260378 tifffile-2024.4.18/tifffile.egg-info/
--rw-rw-rw-   0        0        0    31748 2024-04-18 02:07:17.000000 tifffile-2024.4.18/tifffile.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      617 2024-04-18 02:07:18.000000 tifffile-2024.4.18/tifffile.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-18 02:07:17.000000 tifffile-2024.4.18/tifffile.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      155 2024-04-18 02:07:17.000000 tifffile-2024.4.18/tifffile.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       75 2024-04-18 02:07:17.000000 tifffile-2024.4.18/tifffile.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-18 02:07:17.000000 tifffile-2024.4.18/tifffile.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-25 03:05:10.077372 tifffile-2024.4.24/
+-rw-rw-rw-   0        0        0      324 2019-07-10 16:43:27.000000 tifffile-2024.4.24/ACKNOWLEDGEMENTS.rst
+-rw-rw-rw-   0        0        0    38017 2024-04-25 03:05:08.000000 tifffile-2024.4.24/CHANGES.rst
+-rw-rw-rw-   0        0        0     1559 2024-04-25 03:05:08.000000 tifffile-2024.4.24/LICENSE
+-rw-rw-rw-   0        0        0      569 2023-08-11 02:48:51.000000 tifffile-2024.4.24/MANIFEST.in
+-rw-rw-rw-   0        0        0    31811 2024-04-25 03:05:10.077372 tifffile-2024.4.24/PKG-INFO
+-rw-rw-rw-   0        0        0    30569 2024-04-25 03:05:08.000000 tifffile-2024.4.24/README.rst
+drwxrwxrwx   0        0        0        0 2024-04-25 03:05:10.061868 tifffile-2024.4.24/docs/
+drwxrwxrwx   0        0        0        0 2024-04-25 03:05:10.061868 tifffile-2024.4.24/docs/_static/
+-rw-rw-rw-   0        0        0      127 2022-05-28 19:33:31.000000 tifffile-2024.4.24/docs/_static/custom.css
+-rw-rw-rw-   0        0        0     1098 2023-12-25 06:05:35.000000 tifffile-2024.4.24/docs/conf.py
+-rw-rw-rw-   0        0        0     3644 2023-08-12 18:29:44.000000 tifffile-2024.4.24/docs/make.py
+drwxrwxrwx   0        0        0        0 2024-04-25 03:05:10.061868 tifffile-2024.4.24/examples/
+-rw-rw-rw-   0        0        0    15113 2024-02-12 18:46:43.000000 tifffile-2024.4.24/examples/earthbigdata.py
+-rw-rw-rw-   0        0        0     2542 2024-01-28 18:02:54.000000 tifffile-2024.4.24/examples/issue125.py
+-rw-rw-rw-   0        0        0       42 2024-04-25 03:05:10.077372 tifffile-2024.4.24/setup.cfg
+-rw-rw-rw-   0        0        0     3936 2023-10-18 16:48:53.000000 tifffile-2024.4.24/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-25 03:05:10.077372 tifffile-2024.4.24/tests/
+-rw-rw-rw-   0        0        0     1603 2023-08-30 07:20:06.000000 tifffile-2024.4.24/tests/conftest.py
+-rw-rw-rw-   0        0        0   744389 2024-04-25 03:03:32.000000 tifffile-2024.4.24/tests/test_tifffile.py
+drwxrwxrwx   0        0        0        0 2024-04-25 03:05:10.077372 tifffile-2024.4.24/tifffile/
+-rw-rw-rw-   0        0        0      110 2024-01-28 01:29:32.000000 tifffile-2024.4.24/tifffile/__init__.py
+-rw-rw-rw-   0        0        0      135 2020-01-01 02:31:36.000000 tifffile-2024.4.24/tifffile/__main__.py
+-rw-rw-rw-   0        0        0    11865 2024-04-25 00:49:56.000000 tifffile-2024.4.24/tifffile/_imagecodecs.py
+-rw-rw-rw-   0        0        0    61794 2023-07-03 00:17:39.000000 tifffile-2024.4.24/tifffile/geodb.py
+-rw-rw-rw-   0        0        0      680 2023-07-03 00:17:47.000000 tifffile-2024.4.24/tifffile/lsm2bin.py
+-rw-rw-rw-   0        0        0     5904 2024-01-29 17:41:17.000000 tifffile-2024.4.24/tifffile/numcodecs.py
+-rw-rw-rw-   0        0        0        0 2023-08-11 00:10:50.000000 tifffile-2024.4.24/tifffile/py.typed
+-rw-rw-rw-   0        0        0     2410 2023-07-03 00:18:03.000000 tifffile-2024.4.24/tifffile/tiff2fsspec.py
+-rw-rw-rw-   0        0        0     1437 2023-07-03 00:18:11.000000 tifffile-2024.4.24/tifffile/tiffcomment.py
+-rw-rw-rw-   0        0        0   888550 2024-04-25 03:02:37.000000 tifffile-2024.4.24/tifffile/tifffile.py
+drwxrwxrwx   0        0        0        0 2024-04-25 03:05:10.077372 tifffile-2024.4.24/tifffile.egg-info/
+-rw-rw-rw-   0        0        0    31811 2024-04-25 03:05:09.000000 tifffile-2024.4.24/tifffile.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      617 2024-04-25 03:05:10.000000 tifffile-2024.4.24/tifffile.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 03:05:09.000000 tifffile-2024.4.24/tifffile.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      155 2024-04-25 03:05:09.000000 tifffile-2024.4.24/tifffile.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       75 2024-04-25 03:05:09.000000 tifffile-2024.4.24/tifffile.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-25 03:05:09.000000 tifffile-2024.4.24/tifffile.egg-info/top_level.txt
```

### Comparing `tifffile-2024.4.18/CHANGES.rst` & `tifffile-2024.4.24/CHANGES.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 Revisions
 ---------
 
-2024.4.18
+2024.4.24
 
 - Pass 5077 tests.
+- Fix compatibility issue with numpy 2 (#252).
+
+2024.4.18
+
 - Fix write_fsspec when last row of tiles is missing in Philips slide (#249).
 - Add option not to quote file names in write_fsspec.
 - Allow compress bilevel images with deflate, LZMA, and Zstd.
 
 2024.2.12
 
 - Deprecate dtype, add chunkdtype parameter in FileSequence.asarray.
```

### Comparing `tifffile-2024.4.18/LICENSE` & `tifffile-2024.4.24/LICENSE`

 * *Files identical despite different names*

### Comparing `tifffile-2024.4.18/MANIFEST.in` & `tifffile-2024.4.24/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `tifffile-2024.4.18/PKG-INFO` & `tifffile-2024.4.24/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tifffile
-Version: 2024.4.18
+Version: 2024.4.24
 Summary: Read and write TIFF files
 Home-page: https://www.cgohlke.com
 Author: Christoph Gohlke
 Author-email: cgohlke@cgohlke.com
 License: BSD
 Project-URL: Bug Tracker, https://github.com/cgohlke/tifffile/issues
 Project-URL: Source Code, https://github.com/cgohlke/tifffile
@@ -59,15 +59,15 @@
 Tifffile can also be used to inspect TIFF structures, read image data from
 multi-dimensional file sequences, write fsspec ReferenceFileSystem for
 TIFF files and image file sequences, patch TIFF tag values, and parse
 many proprietary metadata formats.
 
 :Author: `Christoph Gohlke <https://www.cgohlke.com>`_
 :License: BSD 3-Clause
-:Version: 2024.4.18
+:Version: 2024.4.24
 :DOI: `10.5281/zenodo.6795860 <https://doi.org/10.5281/zenodo.6795860>`_
 
 Quickstart
 ----------
 
 Install the tifffile package and all dependencies from the
 `Python Package Index <https://pypi.org/project/tifffile/>`_::
@@ -111,17 +111,21 @@
   (required only for opening Zarr stores)
 - `Fsspec <https://pypi.org/project/fsspec/>`_ 2024.3.1
   (required only for opening ReferenceFileSystem files)
 
 Revisions
 ---------
 
-2024.4.18
+2024.4.24
 
 - Pass 5077 tests.
+- Fix compatibility issue with numpy 2 (#252).
+
+2024.4.18
+
 - Fix write_fsspec when last row of tiles is missing in Philips slide (#249).
 - Add option not to quote file names in write_fsspec.
 - Allow compress bilevel images with deflate, LZMA, and Zstd.
 
 2024.2.12
 
 - Deprecate dtype, add chunkdtype parameter in FileSequence.asarray.
```

### Comparing `tifffile-2024.4.18/README.rst` & `tifffile-2024.4.24/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 Tifffile can also be used to inspect TIFF structures, read image data from
 multi-dimensional file sequences, write fsspec ReferenceFileSystem for
 TIFF files and image file sequences, patch TIFF tag values, and parse
 many proprietary metadata formats.
 
 :Author: `Christoph Gohlke <https://www.cgohlke.com>`_
 :License: BSD 3-Clause
-:Version: 2024.4.18
+:Version: 2024.4.24
 :DOI: `10.5281/zenodo.6795860 <https://doi.org/10.5281/zenodo.6795860>`_
 
 Quickstart
 ----------
 
 Install the tifffile package and all dependencies from the
 `Python Package Index <https://pypi.org/project/tifffile/>`_::
@@ -78,17 +78,21 @@
   (required only for opening Zarr stores)
 - `Fsspec <https://pypi.org/project/fsspec/>`_ 2024.3.1
   (required only for opening ReferenceFileSystem files)
 
 Revisions
 ---------
 
-2024.4.18
+2024.4.24
 
 - Pass 5077 tests.
+- Fix compatibility issue with numpy 2 (#252).
+
+2024.4.18
+
 - Fix write_fsspec when last row of tiles is missing in Philips slide (#249).
 - Add option not to quote file names in write_fsspec.
 - Allow compress bilevel images with deflate, LZMA, and Zstd.
 
 2024.2.12
 
 - Deprecate dtype, add chunkdtype parameter in FileSequence.asarray.
```

### Comparing `tifffile-2024.4.18/docs/conf.py` & `tifffile-2024.4.24/docs/conf.py`

 * *Files identical despite different names*

### Comparing `tifffile-2024.4.18/docs/make.py` & `tifffile-2024.4.24/docs/make.py`

 * *Files identical despite different names*

### Comparing `tifffile-2024.4.18/examples/earthbigdata.py` & `tifffile-2024.4.24/examples/earthbigdata.py`

 * *Files identical despite different names*

### Comparing `tifffile-2024.4.18/examples/issue125.py` & `tifffile-2024.4.24/examples/issue125.py`

 * *Files identical despite different names*

### Comparing `tifffile-2024.4.18/setup.py` & `tifffile-2024.4.24/setup.py`

 * *Files identical despite different names*

### Comparing `tifffile-2024.4.18/tests/conftest.py` & `tifffile-2024.4.24/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `tifffile-2024.4.18/tests/test_tifffile.py` & `tifffile-2024.4.24/tests/test_tifffile.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 # mypy: check-untyped-defs=False
 
 """Unittests for the tifffile package.
 
 Public data files can be requested from the author.
 Private data files are not available due to size and copyright restrictions.
 
-:Version: 2024.4.18
+:Version: 2024.4.24
 
 """
 
 import binascii
 import datetime
 import glob
 import json
@@ -2578,28 +2578,30 @@
             tags = tif.pages.first.tags
             assert 322 not in tags
             assert 34665 not in tags
             assert tags.get(270, index=1) is None
             assert tags[266].value == 1
 
 
-@pytest.mark.skipif(SKIP_PRIVATE, reason=REASON)
+@pytest.mark.skipif(
+    SKIP_PRIVATE or SKIP_CODECS or not imagecodecs.JPEG, reason=REASON
+)
 def test_issue_invalid_predictor(caplog):
     """Test decoding JPEG compression with invalid predictor tag."""
     fname = private_file('issues/invalid_predictor.tiff')
     with TiffFile(fname) as tif:
         page = tif.pages.first
         assert page.predictor == 58240
         assert page.compression == 7
         data = page.asarray()
         assert 'ignoring predictor' in caplog.text
         assert data.shape == (1275, 1650, 4)
 
 
-@pytest.mark.skipif(SKIP_PRIVATE, reason=REASON)
+@pytest.mark.skipif(SKIP_PRIVATE or SKIP_CODECS, reason=REASON)
 def test_issue_ome_missing_frames():
     """Test read OME TIFF with missing pages at end."""
     # https://github.com/cgohlke/tifffile/issues/199
     fname = private_file('issues/stack_t24_y2048_x2448.tiff')
     with TiffFile(fname) as tif:
         assert tif.is_ome
         assert tif.byteorder == '<'
@@ -5231,19 +5233,19 @@
         [
             [1, 666, 1431655765, 62],
             [2, 16601, 1431655765, 32],
             [3, 16441, 2863311530, 30],
         ],
         dtype='uint32',
     )
-    if int(numpy.__version__.split('.')[1]) < 23:
-        with pytest.raises(NotImplementedError):
-            bitorder_decode(data[1:, 1:3])
-    else:
-        assert_array_equal(bitorder_decode(data[1:, 1:3]), reverse[1:, 1:3])
+    # if int(numpy.__version__.split('.')[1]) < 23:
+    #     with pytest.raises(NotImplementedError):
+    #         bitorder_decode(data[1:, 1:3])
+    # else:
+    assert_array_equal(bitorder_decode(data[1:, 1:3]), reverse[1:, 1:3])
 
 
 @pytest.mark.parametrize(
     'kind',
     ['u1', 'u2', 'u4', 'u8', 'i1', 'i2', 'i4', 'i8', 'f4', 'f8', 'B'],
 )
 @pytest.mark.parametrize('byteorder', ['>', '<'])
@@ -13160,15 +13162,15 @@
     store = imread(fname, key=1, series=0, level=2, aszarr=True)
     z = zarr.open(store, mode='r')
     image = z[:]
     del z
     assert_array_equal(image, data)
 
 
-@pytest.mark.skipif(SKIP_PRIVATE, reason=REASON)
+@pytest.mark.skipif(SKIP_PRIVATE or SKIP_CODECS, reason=REASON)
 def test_read_eer(caplog):
     """Test read EER metadata."""
     # https://github.com/fei-company/EerReaderLib/issues/1
     fname = private_file('EER/Example_1.eer')
     with TiffFile(fname) as tif:
         assert not caplog.text  # no warning
         assert tif.is_bigtiff
@@ -15531,15 +15533,16 @@
             assert__str__(tif)
 
 
 @pytest.mark.skipif(IS_BE, reason=REASON)
 def test_write_write_bigendian():
     """Test write big endian file."""
     # also test memory mapping non-native byte order
-    data = random_data(numpy.float32, (2, 3, 219, 301)).newbyteorder()
+    data = random_data(numpy.float32, (2, 3, 219, 301))
+    data = data.view(data.dtype.newbyteorder())
     data = numpy.nan_to_num(data, copy=False)
     with TempFileName('write_bigendian') as fname:
         imwrite(fname, data, planarconfig=SEPARATE, photometric=RGB)
         assert_valid_tiff(fname)
         with TiffFile(fname) as tif:
             assert len(tif.pages) == 2
             assert len(tif.series) == 1
@@ -18468,15 +18471,15 @@
         elif method == 'manual':
             # manually write omexml to first page and data to individual pages
             # process OME-XML
             omexml = omexml.replace(
                 '4D-series.ome.tiff', os.path.split(fname)[-1]
             )
             # omexml = omexml.replace('BigEndian="true"', 'BigEndian="false"')
-            data = data.newbyteorder('>')
+            data = data.view(data.dtype.newbyteorder('>'))
             # save image planes in the order referenced in the OME-XML
             # make sure storage options (compression, byteorder, photometric)
             #   match OME-XML
             # write OME-XML to first page only
             with TiffWriter(fname, byteorder='>') as tif:
                 for i, image in enumerate(pages()):
                     description = omexml if i == 0 else None
```

### Comparing `tifffile-2024.4.18/tifffile/_imagecodecs.py` & `tifffile-2024.4.24/tifffile/_imagecodecs.py`

 * *Files 1% similar despite different names*

```diff
@@ -191,15 +191,16 @@
     if dtype.kind == 'f':
         data = data.view(f'{dtype.byteorder}u{dtype.itemsize}')
     diff = numpy.diff(data, axis=axis)
     key: list[int | slice] = [slice(None)] * data.ndim
     key[axis] = 0
     diff = numpy.insert(diff, 0, data[tuple(key)], axis=axis)
     if not data.dtype.isnative:
-        diff = diff.byteswap(True).newbyteorder()
+        diff = diff.byteswap(True)
+        diff = diff.view(diff.dtype.newbyteorder())
     if dtype.kind == 'f':
         return diff.view(dtype)
     return diff
 
 
 @overload
 def delta_decode(
```

### Comparing `tifffile-2024.4.18/tifffile/geodb.py` & `tifffile-2024.4.24/tifffile/geodb.py`

 * *Files identical despite different names*

### Comparing `tifffile-2024.4.18/tifffile/lsm2bin.py` & `tifffile-2024.4.24/tifffile/lsm2bin.py`

 * *Files identical despite different names*

### Comparing `tifffile-2024.4.18/tifffile/numcodecs.py` & `tifffile-2024.4.24/tifffile/numcodecs.py`

 * *Files identical despite different names*

### Comparing `tifffile-2024.4.18/tifffile/tiff2fsspec.py` & `tifffile-2024.4.24/tifffile/tiff2fsspec.py`

 * *Files identical despite different names*

### Comparing `tifffile-2024.4.18/tifffile/tiffcomment.py` & `tifffile-2024.4.24/tifffile/tiffcomment.py`

 * *Files identical despite different names*

### Comparing `tifffile-2024.4.18/tifffile/tifffile.py` & `tifffile-2024.4.24/tifffile/tifffile.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 Tifffile can also be used to inspect TIFF structures, read image data from
 multi-dimensional file sequences, write fsspec ReferenceFileSystem for
 TIFF files and image file sequences, patch TIFF tag values, and parse
 many proprietary metadata formats.
 
 :Author: `Christoph Gohlke <https://www.cgohlke.com>`_
 :License: BSD 3-Clause
-:Version: 2024.4.18
+:Version: 2024.4.24
 :DOI: `10.5281/zenodo.6795860 <https://doi.org/10.5281/zenodo.6795860>`_
 
 Quickstart
 ----------
 
 Install the tifffile package and all dependencies from the
 `Python Package Index <https://pypi.org/project/tifffile/>`_::
@@ -108,17 +108,21 @@
   (required only for opening Zarr stores)
 - `Fsspec <https://pypi.org/project/fsspec/>`_ 2024.3.1
   (required only for opening ReferenceFileSystem files)
 
 Revisions
 ---------
 
-2024.4.18
+2024.4.24
 
 - Pass 5077 tests.
+- Fix compatibility issue with numpy 2 (#252).
+
+2024.4.18
+
 - Fix write_fsspec when last row of tiles is missing in Philips slide (#249).
 - Add option not to quote file names in write_fsspec.
 - Allow compress bilevel images with deflate, LZMA, and Zstd.
 
 2024.2.12
 
 - Deprecate dtype, add chunkdtype parameter in FileSequence.asarray.
@@ -828,15 +832,15 @@
 
     $ python -m tifffile temp.ome.tif
 
 """
 
 from __future__ import annotations
 
-__version__ = '2024.4.18'
+__version__ = '2024.4.24'
 
 __all__ = [
     'TiffFile',
     'TiffFileError',
     'TiffFrame',
     'TiffPage',
     'TiffPages',
@@ -12914,16 +12918,16 @@
             ValueError:
                 ZarrTiffStore cannot be represented as ReferenceFileSystem
                 due to features that are not supported by Zarr, Numcodecs,
                 or Imagecodecs:
 
                 - compressors, such as CCITT
                 - filters, such as bitorder reversal, packed integers
-                - dtypes, such as float24
-                - JPEGTables in multi-page files
+                - dtypes, such as float24, complex integers
+                - JPEGTables in multi-page series
                 - incomplete chunks, such as `imagelength % rowsperstrip != 0`
 
                 Files containing incomplete tiles may fail at runtime.
 
         Notes:
             Parameters `_shape`,  `_axes`, `_index`, `_append`, and `_close`
             are an experimental API for joining the ReferenceFileSystems of
```

### Comparing `tifffile-2024.4.18/tifffile.egg-info/PKG-INFO` & `tifffile-2024.4.24/tifffile.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tifffile
-Version: 2024.4.18
+Version: 2024.4.24
 Summary: Read and write TIFF files
 Home-page: https://www.cgohlke.com
 Author: Christoph Gohlke
 Author-email: cgohlke@cgohlke.com
 License: BSD
 Project-URL: Bug Tracker, https://github.com/cgohlke/tifffile/issues
 Project-URL: Source Code, https://github.com/cgohlke/tifffile
@@ -59,15 +59,15 @@
 Tifffile can also be used to inspect TIFF structures, read image data from
 multi-dimensional file sequences, write fsspec ReferenceFileSystem for
 TIFF files and image file sequences, patch TIFF tag values, and parse
 many proprietary metadata formats.
 
 :Author: `Christoph Gohlke <https://www.cgohlke.com>`_
 :License: BSD 3-Clause
-:Version: 2024.4.18
+:Version: 2024.4.24
 :DOI: `10.5281/zenodo.6795860 <https://doi.org/10.5281/zenodo.6795860>`_
 
 Quickstart
 ----------
 
 Install the tifffile package and all dependencies from the
 `Python Package Index <https://pypi.org/project/tifffile/>`_::
@@ -111,17 +111,21 @@
   (required only for opening Zarr stores)
 - `Fsspec <https://pypi.org/project/fsspec/>`_ 2024.3.1
   (required only for opening ReferenceFileSystem files)
 
 Revisions
 ---------
 
-2024.4.18
+2024.4.24
 
 - Pass 5077 tests.
+- Fix compatibility issue with numpy 2 (#252).
+
+2024.4.18
+
 - Fix write_fsspec when last row of tiles is missing in Philips slide (#249).
 - Add option not to quote file names in write_fsspec.
 - Allow compress bilevel images with deflate, LZMA, and Zstd.
 
 2024.2.12
 
 - Deprecate dtype, add chunkdtype parameter in FileSequence.asarray.
```

### Comparing `tifffile-2024.4.18/tifffile.egg-info/SOURCES.txt` & `tifffile-2024.4.24/tifffile.egg-info/SOURCES.txt`

 * *Files identical despite different names*


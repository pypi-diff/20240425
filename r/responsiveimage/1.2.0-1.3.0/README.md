# Comparing `tmp/responsiveimage-1.2.0.tar.gz` & `tmp/responsiveimage-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "responsiveimage-1.2.0.tar", last modified: Tue Nov 21 15:57:03 2023, max compression
+gzip compressed data, was "responsiveimage-1.3.0.tar", last modified: Thu Apr 25 17:35:17 2024, max compression
```

## Comparing `responsiveimage-1.2.0.tar` & `responsiveimage-1.3.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-11-21 15:57:03.060353 responsiveimage-1.2.0/
--rw-rw-rw-   0        0        0     1069 2023-09-28 16:10:00.000000 responsiveimage-1.2.0/LICENSE
--rw-rw-rw-   0        0        0     4274 2023-11-21 15:57:03.060353 responsiveimage-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     3554 2023-11-21 15:38:24.000000 responsiveimage-1.2.0/README.md
--rw-rw-rw-   0        0        0     1006 2023-11-21 15:54:46.000000 responsiveimage-1.2.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-11-21 15:57:03.060353 responsiveimage-1.2.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-11-21 15:57:03.031858 responsiveimage-1.2.0/src/
-drwxrwxrwx   0        0        0        0 2023-11-21 15:57:03.054343 responsiveimage-1.2.0/src/responsiveimage/
--rw-rw-rw-   0        0        0      165 2023-09-28 16:10:00.000000 responsiveimage-1.2.0/src/responsiveimage/__init__.py
--rw-rw-rw-   0        0        0     5904 2023-11-21 15:50:53.000000 responsiveimage-1.2.0/src/responsiveimage/__main__.py
--rw-rw-rw-   0        0        0     2485 2023-11-20 11:18:17.000000 responsiveimage-1.2.0/src/responsiveimage/argsResponsiveImage.py
--rw-rw-rw-   0        0        0     1095 2023-11-19 19:34:45.000000 responsiveimage-1.2.0/src/responsiveimage/copy_image.py
--rw-rw-rw-   0        0        0     2734 2023-10-15 16:31:02.000000 responsiveimage-1.2.0/src/responsiveimage/exif.py
--rw-rw-rw-   0        0        0     1122 2023-11-19 19:20:46.000000 responsiveimage-1.2.0/src/responsiveimage/jpg.py
--rw-rw-rw-   0        0        0     2889 2023-11-19 19:34:45.000000 responsiveimage-1.2.0/src/responsiveimage/mp4.py
--rw-rw-rw-   0        0        0     3954 2023-11-19 19:34:45.000000 responsiveimage-1.2.0/src/responsiveimage/pil_image.py
--rw-rw-rw-   0        0        0      864 2023-11-19 19:20:36.000000 responsiveimage-1.2.0/src/responsiveimage/png.py
--rw-rw-rw-   0        0        0      877 2023-11-19 19:20:32.000000 responsiveimage-1.2.0/src/responsiveimage/webp.py
-drwxrwxrwx   0        0        0        0 2023-11-21 15:57:03.060353 responsiveimage-1.2.0/src/responsiveimage.egg-info/
--rw-rw-rw-   0        0        0     4274 2023-11-21 15:57:03.000000 responsiveimage-1.2.0/src/responsiveimage.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      557 2023-11-21 15:57:03.000000 responsiveimage-1.2.0/src/responsiveimage.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-11-21 15:57:03.000000 responsiveimage-1.2.0/src/responsiveimage.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-11-21 15:57:03.000000 responsiveimage-1.2.0/src/responsiveimage.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-11-21 15:57:03.000000 responsiveimage-1.2.0/src/responsiveimage.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-25 17:35:16.841293 responsiveimage-1.3.0/
+-rw-rw-rw-   0        0        0     1069 2023-09-28 16:10:00.000000 responsiveimage-1.3.0/LICENSE
+-rw-rw-rw-   0        0        0     4315 2024-04-25 17:35:16.839296 responsiveimage-1.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3595 2024-04-25 17:32:29.000000 responsiveimage-1.3.0/README.md
+-rw-rw-rw-   0        0        0     1006 2024-04-25 17:32:00.000000 responsiveimage-1.3.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-25 17:35:16.841293 responsiveimage-1.3.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-25 17:35:16.577843 responsiveimage-1.3.0/src/
+drwxrwxrwx   0        0        0        0 2024-04-25 17:35:16.640085 responsiveimage-1.3.0/src/responsiveimage/
+-rw-rw-rw-   0        0        0      165 2023-09-28 16:10:00.000000 responsiveimage-1.3.0/src/responsiveimage/__init__.py
+-rw-rw-rw-   0        0        0     7405 2024-04-25 17:26:19.000000 responsiveimage-1.3.0/src/responsiveimage/__main__.py
+-rw-rw-rw-   0        0        0     2421 2024-04-25 16:15:58.000000 responsiveimage-1.3.0/src/responsiveimage/argsResponsiveImage.py
+-rw-rw-rw-   0        0        0     1098 2024-04-25 16:17:24.000000 responsiveimage-1.3.0/src/responsiveimage/copy_image.py
+-rw-rw-rw-   0        0        0     2734 2023-10-15 16:31:02.000000 responsiveimage-1.3.0/src/responsiveimage/exif.py
+-rw-rw-rw-   0        0        0     1122 2023-11-19 19:20:46.000000 responsiveimage-1.3.0/src/responsiveimage/jpg.py
+-rw-rw-rw-   0        0        0     2898 2024-04-25 16:16:48.000000 responsiveimage-1.3.0/src/responsiveimage/mp4.py
+-rw-rw-rw-   0        0        0     3957 2024-04-25 16:16:52.000000 responsiveimage-1.3.0/src/responsiveimage/pil_image.py
+-rw-rw-rw-   0        0        0      864 2023-11-19 19:20:36.000000 responsiveimage-1.3.0/src/responsiveimage/png.py
+-rw-rw-rw-   0        0        0      877 2023-11-19 19:20:32.000000 responsiveimage-1.3.0/src/responsiveimage/webp.py
+drwxrwxrwx   0        0        0        0 2024-04-25 17:35:16.802668 responsiveimage-1.3.0/src/responsiveimage.egg-info/
+-rw-rw-rw-   0        0        0     4315 2024-04-25 17:35:16.000000 responsiveimage-1.3.0/src/responsiveimage.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      557 2024-04-25 17:35:16.000000 responsiveimage-1.3.0/src/responsiveimage.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 17:35:16.000000 responsiveimage-1.3.0/src/responsiveimage.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-04-25 17:35:16.000000 responsiveimage-1.3.0/src/responsiveimage.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-04-25 17:35:16.000000 responsiveimage-1.3.0/src/responsiveimage.egg-info/top_level.txt
```

### Comparing `responsiveimage-1.2.0/LICENSE` & `responsiveimage-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `responsiveimage-1.2.0/PKG-INFO` & `responsiveimage-1.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: responsiveimage
-Version: 1.2.0
+Version: 1.3.0
 Summary: Create different scaled versions of an image, in webp, jpg, png, svg,... to be used on resposive website
 Author-email: Pascal Brand <pascal.brand38@gmail.com>
 License: UNKNOWN
 Project-URL: Homepage, https://github.com/pascal-brand38/py-responsiveimage
 Project-URL: Bug Tracker, https://github.com/pascal-brand38/py-responsiveimage/issues
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -86,14 +86,17 @@
 * ```--force```: recreate the scaled versions of the images, even when they exist.
 
 <br>
 
 _____________________
 # Releases
 
+## 1.3.0
+* Multiprocessing on images
+
 ## 1.2.0
 * Supported formats:
   webp, jpg, png, gif and svg, mp4, mts, avi, wmv, mov
 * New options:
   * --format
   * --recursive
```

### Comparing `responsiveimage-1.2.0/README.md` & `responsiveimage-1.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -68,14 +68,17 @@
 * ```--force```: recreate the scaled versions of the images, even when they exist.
 
 <br>
 
 _____________________
 # Releases
 
+## 1.3.0
+* Multiprocessing on images
+
 ## 1.2.0
 * Supported formats:
   webp, jpg, png, gif and svg, mp4, mts, avi, wmv, mov
 * New options:
   * --format
   * --recursive
```

### Comparing `responsiveimage-1.2.0/pyproject.toml` & `responsiveimage-1.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 000000a0: 2064 6966 6665 7265 6e74 2073 6361 6c65   different scale
 000000b0: 6420 7665 7273 696f 6e73 206f 6620 616e  d versions of an
 000000c0: 2069 6d61 6765 2c20 696e 2077 6562 702c   image, in webp,
 000000d0: 206a 7067 2c20 706e 672c 2073 7667 2c2e   jpg, png, svg,.
 000000e0: 2e2e 2074 6f20 6265 2075 7365 6420 6f6e  .. to be used on
 000000f0: 2072 6573 706f 7369 7665 2077 6562 7369   resposive websi
 00000100: 7465 220d 0a20 2076 6572 7369 6f6e 203d  te"..  version =
-00000110: 2022 312e 322e 3022 0d0a 2020 6175 7468   "1.2.0"..  auth
+00000110: 2022 312e 332e 3022 0d0a 2020 6175 7468   "1.3.0"..  auth
 00000120: 6f72 7320 3d20 5b0d 0a20 2020 207b 206e  ors = [..    { n
 00000130: 616d 653d 2250 6173 6361 6c20 4272 616e  ame="Pascal Bran
 00000140: 6422 2c20 656d 6169 6c3d 2270 6173 6361  d", email="pasca
 00000150: 6c2e 6272 616e 6433 3840 676d 6169 6c2e  l.brand38@gmail.
 00000160: 636f 6d22 207d 2c0d 0a20 205d 0d0a 2020  com" },..  ]..  
 00000170: 7265 6164 6d65 203d 2022 5245 4144 4d45  readme = "README
 00000180: 2e6d 6422 0d0a 2020 7265 7175 6972 6573  .md"..  requires
```

### Comparing `responsiveimage-1.2.0/src/responsiveimage/argsResponsiveImage.py` & `responsiveimage-1.3.0/src/responsiveimage/argsResponsiveImage.py`

 * *Files 4% similar despite different names*

```diff
@@ -64,23 +64,21 @@
         'subsampling': '4:2:0',
         },
       'webp': {
         'quality': 80,
       }
     }
 
-  def inc(self) -> None:
+  def add(self, nb) -> None:
     '''
     increment the number of processed images
     '''
-    if self.nb is not None:
-      self.nb = self.nb + 1
+    self.nb = self.nb + nb
 
-  def print(self, filename: str, processed: bool) -> None:
+  def print(self, filename: str, processed: bool, nb: int) -> None:
     '''
     verbose the number of processed images
     '''
-    if self.nb is not None:
-      if (processed):
-        print('  + ' + str(self.nb) + ' ' + filename)
-      else:
-        print('  - ' + str(self.nb) + ' ' + filename)
+    if (processed):
+      print('  + ' + str(nb) + ' ' + filename)
+    else:
+      print('  - ' + str(nb) + ' ' + filename)
```

### Comparing `responsiveimage-1.2.0/src/responsiveimage/copy_image.py` & `responsiveimage-1.3.0/src/responsiveimage/copy_image.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,19 +18,18 @@
   if (not os.path.isfile(filename_dst) or (not filecmp.cmp(filename_src, filename_dst))):
     try:
       shutil.copy2(filename_src, filename_dst)
     except:
       print('   === cannot copy ' + filename_src + ' to ' + filename_dst)
 
 
-def responsive(args: argsResponsiveImage.argsResponsiveImage, filename, filetype: str) -> None:
+def responsive(args: argsResponsiveImage.argsResponsiveImage, filename, filetype: str, nb: int) -> None:
   '''
   get the responsive version of the image by copying it only
   used for gif and svg
   '''
-  args.inc()
   if (not args.args.force) and (os.path.isfile(os.path.join(args.args.dst_dir, filename))):
-    args.print(filename, False)
+    args.print(filename, False, nb)
     return
 
-  args.print(filename, True)
+  args.print(filename, True, nb)
   _copy_file(os.path.join(args.args.src_dir, filename), os.path.join(args.args.dst_dir, filename))
```

### Comparing `responsiveimage-1.2.0/src/responsiveimage/exif.py` & `responsiveimage-1.3.0/src/responsiveimage/exif.py`

 * *Files identical despite different names*

### Comparing `responsiveimage-1.2.0/src/responsiveimage/jpg.py` & `responsiveimage-1.3.0/src/responsiveimage/jpg.py`

 * *Files identical despite different names*

### Comparing `responsiveimage-1.2.0/src/responsiveimage/mp4.py` & `responsiveimage-1.3.0/src/responsiveimage/mp4.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,41 +8,39 @@
 
 import os
 import shutil
 import subprocess
 import tempfile
 from . import argsResponsiveImage
 
-def responsive(args: argsResponsiveImage.argsResponsiveImage, filename: str) -> None:
+def responsive(args: argsResponsiveImage.argsResponsiveImage, filename: str, nb: int) -> None:
   '''
   process mp4 file filename (only the filename, without src_dir)
 
   if args.args.mp4_as_gif:
   - create animated gif and webp
 
   otherwise
   - rescale mp4 (TODO: right now 1024)
   '''
 
-  args.inc()
-
   srcFullFilename = os.path.join(args.args.src_dir, filename)
   dstFullFilename = os.path.join(args.args.dst_dir, filename)
 
   if args.args.mp4_as_gif:
     (dstName, _) = os.path.splitext(dstFullFilename)
 
     filename_gif = dstName +'.gif'
     filename_webp = dstName +'.webp'
 
     if (not args.args.force) and (os.path.isfile(filename_gif)) and (os.path.isfile(filename_webp)):
-      args.print(filename, False)
+      args.print(filename, False, nb)
       return
 
-    args.print(filename, True)
+    args.print(filename, True, nb)
 
     # mp4 -> gif: https://superuser.com/questions/556029/how-do-i-convert-a-video-to-gif-using-ffmpeg-with-reasonable-quality
     palette = tempfile.gettempdir() + '/palette.png'
     filters='fps=2,scale=-1:-1:flags=lanczos'
 
     subprocess.call([
       'ffmpeg',
@@ -73,17 +71,17 @@
       '-loop', '0',
       '-compression_level', '6',
       filename_webp])
 
   else:
 
     if (not args.args.force) and (os.path.isfile(dstFullFilename)):
-      args.print(filename, False)
+      args.print(filename, False, nb)
       return
-    args.print(filename, True)
+    args.print(filename, True, nb)
 
     # -vf option: https://trac.ffmpeg.org/wiki/Scaling
     # pad: cf. https://stackoverflow.com/questions/20847674/ffmpeg-libx264-height-not-divisible-by-2
     subprocess.call([
       'ffmpeg',
       '-y',
       '-i', srcFullFilename,
```

### Comparing `responsiveimage-1.2.0/src/responsiveimage/pil_image.py` & `responsiveimage-1.3.0/src/responsiveimage/pil_image.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,23 +64,22 @@
   if (values[3] > image_org.height):
     return image_org
 
   return image_org.crop((values[0], values[1], values[2], values[3]))
 
 
 
-def responsive(args: argsResponsiveImage.argsResponsiveImage, filename: str, filetype: str) -> None:
+def responsive(args: argsResponsiveImage.argsResponsiveImage, filename: str, filetype: str, nb: int) -> None:
   '''
   create responsive version of the images
   '''
-  args.inc()
   if (not args.args.force) and (not missingOutput(args, filename, filetype)):
-    args.print(filename, False)
+    args.print(filename, False, nb)
     return
-  args.print(filename, True)
+  args.print(filename, True, nb)
 
   srcFullFilename = os.path.join(args.args.src_dir, filename)
   image_org = Image.open(srcFullFilename)
   image_org = crop(image_org, args.args.crop)
 
   (srcName, srcExt) = os.path.splitext(filename)
```

### Comparing `responsiveimage-1.2.0/src/responsiveimage/png.py` & `responsiveimage-1.3.0/src/responsiveimage/png.py`

 * *Files identical despite different names*

### Comparing `responsiveimage-1.2.0/src/responsiveimage/webp.py` & `responsiveimage-1.3.0/src/responsiveimage/webp.py`

 * *Files identical despite different names*

### Comparing `responsiveimage-1.2.0/src/responsiveimage.egg-info/PKG-INFO` & `responsiveimage-1.3.0/src/responsiveimage.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: responsiveimage
-Version: 1.2.0
+Version: 1.3.0
 Summary: Create different scaled versions of an image, in webp, jpg, png, svg,... to be used on resposive website
 Author-email: Pascal Brand <pascal.brand38@gmail.com>
 License: UNKNOWN
 Project-URL: Homepage, https://github.com/pascal-brand38/py-responsiveimage
 Project-URL: Bug Tracker, https://github.com/pascal-brand38/py-responsiveimage/issues
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -86,14 +86,17 @@
 * ```--force```: recreate the scaled versions of the images, even when they exist.
 
 <br>
 
 _____________________
 # Releases
 
+## 1.3.0
+* Multiprocessing on images
+
 ## 1.2.0
 * Supported formats:
   webp, jpg, png, gif and svg, mp4, mts, avi, wmv, mov
 * New options:
   * --format
   * --recursive
```

### Comparing `responsiveimage-1.2.0/src/responsiveimage.egg-info/SOURCES.txt` & `responsiveimage-1.3.0/src/responsiveimage.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/fisspy-1.0.5.tar.gz` & `tmp/fisspy-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fisspy-1.0.5.tar", last modified: Tue Apr 23 12:49:07 2024, max compression
+gzip compressed data, was "fisspy-1.0.6.tar", last modified: Thu Apr 25 11:55:19 2024, max compression
```

## Comparing `fisspy-1.0.5.tar` & `fisspy-1.0.6.tar`

### file list

```diff
@@ -1,58 +1,57 @@
-drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-23 12:49:07.569193 fisspy-1.0.5/
--rw-r--r--   0 jhkang     (501) staff       (20)     1305 2023-07-14 01:35:52.000000 fisspy-1.0.5/LICENSE.txt
--rw-r--r--   0 jhkang     (501) staff       (20)      257 2024-04-23 12:49:07.569070 fisspy-1.0.5/PKG-INFO
--rw-r--r--   0 jhkang     (501) staff       (20)     1988 2024-04-23 12:48:39.000000 fisspy-1.0.5/README.md
-drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-23 12:49:07.557470 fisspy-1.0.5/fisspy/
--rw-r--r--   0 jhkang     (501) staff       (20)      386 2024-04-23 12:45:48.000000 fisspy-1.0.5/fisspy/__init__.py
-drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-23 12:49:07.559018 fisspy-1.0.5/fisspy/align/
--rw-r--r--   0 jhkang     (501) staff       (20)       44 2024-04-20 02:57:09.000000 fisspy-1.0.5/fisspy/align/__init__.py
--rw-r--r--   0 jhkang     (501) staff       (20)    14687 2024-04-22 08:27:59.000000 fisspy-1.0.5/fisspy/align/alignment.py
--rw-r--r--   0 jhkang     (501) staff       (20)    11470 2024-04-20 02:57:09.000000 fisspy-1.0.5/fisspy/align/base.py
-drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-23 12:49:07.561262 fisspy-1.0.5/fisspy/analysis/
--rw-r--r--   0 jhkang     (501) staff       (20)      317 2024-04-20 02:57:09.000000 fisspy-1.0.5/fisspy/analysis/__init__.py
--rw-r--r--   0 jhkang     (501) staff       (20)    12577 2024-04-20 02:57:09.000000 fisspy-1.0.5/fisspy/analysis/doppler.py
--rw-r--r--   0 jhkang     (501) staff       (20)     1030 2024-04-20 02:57:09.000000 fisspy-1.0.5/fisspy/analysis/filter.py
--rw-r--r--   0 jhkang     (501) staff       (20)     2988 2024-04-21 06:20:03.000000 fisspy-1.0.5/fisspy/analysis/forecast.py
--rw-r--r--   0 jhkang     (501) staff       (20)    15224 2024-04-20 02:57:09.000000 fisspy-1.0.5/fisspy/analysis/ofe.py
--rw-r--r--   0 jhkang     (501) staff       (20)    35503 2024-04-22 08:27:41.000000 fisspy-1.0.5/fisspy/analysis/tdmap.py
--rw-r--r--   0 jhkang     (501) staff       (20)    33899 2024-04-20 03:48:27.000000 fisspy-1.0.5/fisspy/analysis/wavelet.py
--rw-r--r--   0 jhkang     (501) staff       (20)    19011 2023-07-14 01:35:52.000000 fisspy-1.0.5/fisspy/cm.py
-drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-23 12:49:07.562753 fisspy-1.0.5/fisspy/correction/
--rw-r--r--   0 jhkang     (501) staff       (20)       51 2024-04-20 02:57:09.000000 fisspy-1.0.5/fisspy/correction/__init__.py
--rw-r--r--   0 jhkang     (501) staff       (20)    11372 2024-04-20 02:57:09.000000 fisspy-1.0.5/fisspy/correction/correction.py
--rw-r--r--   0 jhkang     (501) staff       (20)     2337 2024-04-20 02:57:09.000000 fisspy-1.0.5/fisspy/correction/get_inform.py
-drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-23 12:49:07.563762 fisspy-1.0.5/fisspy/data/
--rw-r--r--   0 jhkang     (501) staff       (20)       64 2023-07-25 08:49:17.000000 fisspy-1.0.5/fisspy/data/__init__.py
--rw-r--r--   0 jhkang     (501) staff       (20)     1072 2023-07-25 08:49:17.000000 fisspy-1.0.5/fisspy/data/_sample.py
--rw-r--r--   0 jhkang     (501) staff       (20)     2965 2023-07-25 08:49:17.000000 fisspy-1.0.5/fisspy/data/download.py
--rw-r--r--   0 jhkang     (501) staff       (20)      394 2023-07-14 01:35:52.000000 fisspy-1.0.5/fisspy/data/sample.py
-drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-23 12:49:07.564868 fisspy-1.0.5/fisspy/image/
--rw-r--r--   0 jhkang     (501) staff       (20)      110 2024-04-20 02:57:09.000000 fisspy-1.0.5/fisspy/image/__init__.py
--rw-r--r--   0 jhkang     (501) staff       (20)    12576 2024-04-20 02:57:09.000000 fisspy-1.0.5/fisspy/image/base.py
--rw-r--r--   0 jhkang     (501) staff       (20)    29760 2024-04-20 02:57:09.000000 fisspy-1.0.5/fisspy/image/interactive_image.py
--rw-r--r--   0 jhkang     (501) staff       (20)     7860 2024-04-20 02:57:09.000000 fisspy-1.0.5/fisspy/image/raster_set.py
-drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-23 12:49:07.565299 fisspy-1.0.5/fisspy/inversion/
--rw-r--r--   0 jhkang     (501) staff       (20)        0 2024-04-20 02:57:09.000000 fisspy-1.0.5/fisspy/inversion/__init__.py
--rw-r--r--   0 jhkang     (501) staff       (20)      181 2024-04-20 02:57:09.000000 fisspy-1.0.5/fisspy/inversion/_mlsi.py
-drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-23 12:49:07.565782 fisspy-1.0.5/fisspy/io/
--rw-r--r--   0 jhkang     (501) staff       (20)      320 2023-07-14 01:35:52.000000 fisspy-1.0.5/fisspy/io/__init__.py
--rw-r--r--   0 jhkang     (501) staff       (20)    15840 2023-07-14 01:35:52.000000 fisspy-1.0.5/fisspy/io/read.py
--rw-r--r--   0 jhkang     (501) staff       (20)     4974 2024-04-20 02:57:09.000000 fisspy-1.0.5/fisspy/makevideo.py
-drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-23 12:49:07.567543 fisspy-1.0.5/fisspy/preprocess/
--rw-r--r--   0 jhkang     (501) staff       (20)       29 2024-04-20 02:57:09.000000 fisspy-1.0.5/fisspy/preprocess/__init__.py
--rw-r--r--   0 jhkang     (501) staff       (20)    52473 2024-04-20 02:57:09.000000 fisspy-1.0.5/fisspy/preprocess/proc_base.py
--rw-r--r--   0 jhkang     (501) staff       (20)   143266 2024-04-20 02:57:09.000000 fisspy-1.0.5/fisspy/preprocess/proc_gui.py
--rw-r--r--   0 jhkang     (501) staff       (20)     1685 2024-04-20 02:57:09.000000 fisspy-1.0.5/fisspy/preprocess/t_y_sh.py
-drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-23 12:49:07.568734 fisspy-1.0.5/fisspy/read/
--rw-r--r--   0 jhkang     (501) staff       (20)      195 2024-04-20 02:57:09.000000 fisspy-1.0.5/fisspy/read/__init__.py
--rw-r--r--   0 jhkang     (501) staff       (20)    49070 2024-04-23 12:44:46.000000 fisspy-1.0.5/fisspy/read/read_factory.py
--rw-r--r--   0 jhkang     (501) staff       (20)     6813 2024-04-20 02:57:09.000000 fisspy-1.0.5/fisspy/read/readbase.py
-drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-23 12:49:07.558377 fisspy-1.0.5/fisspy.egg-info/
--rw-r--r--   0 jhkang     (501) staff       (20)      257 2024-04-23 12:49:07.000000 fisspy-1.0.5/fisspy.egg-info/PKG-INFO
--rw-r--r--   0 jhkang     (501) staff       (20)     1100 2024-04-23 12:49:07.000000 fisspy-1.0.5/fisspy.egg-info/SOURCES.txt
--rw-r--r--   0 jhkang     (501) staff       (20)        1 2024-04-23 12:49:07.000000 fisspy-1.0.5/fisspy.egg-info/dependency_links.txt
--rw-r--r--   0 jhkang     (501) staff       (20)        1 2024-04-23 12:49:07.000000 fisspy-1.0.5/fisspy.egg-info/not-zip-safe
--rw-r--r--   0 jhkang     (501) staff       (20)      135 2024-04-23 12:49:07.000000 fisspy-1.0.5/fisspy.egg-info/requires.txt
--rw-r--r--   0 jhkang     (501) staff       (20)        7 2024-04-23 12:49:07.000000 fisspy-1.0.5/fisspy.egg-info/top_level.txt
--rw-r--r--   0 jhkang     (501) staff       (20)       38 2024-04-23 12:49:07.569234 fisspy-1.0.5/setup.cfg
--rw-r--r--   0 jhkang     (501) staff       (20)      580 2024-04-23 12:45:46.000000 fisspy-1.0.5/setup.py
+drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-25 11:55:19.726634 fisspy-1.0.6/
+-rw-r--r--   0 jhkang     (501) staff       (20)     1305 2023-07-14 01:35:52.000000 fisspy-1.0.6/LICENSE.txt
+-rw-r--r--   0 jhkang     (501) staff       (20)      574 2024-04-25 11:55:19.726441 fisspy-1.0.6/PKG-INFO
+-rw-r--r--   0 jhkang     (501) staff       (20)     1988 2024-04-23 12:48:39.000000 fisspy-1.0.6/README.md
+drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-25 11:55:19.715932 fisspy-1.0.6/fisspy/
+-rw-r--r--   0 jhkang     (501) staff       (20)      430 2024-04-25 11:51:10.000000 fisspy-1.0.6/fisspy/__init__.py
+drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-25 11:55:19.717388 fisspy-1.0.6/fisspy/align/
+-rw-r--r--   0 jhkang     (501) staff       (20)       44 2024-04-20 02:57:09.000000 fisspy-1.0.6/fisspy/align/__init__.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    15179 2024-04-24 08:05:01.000000 fisspy-1.0.6/fisspy/align/alignment.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    11470 2024-04-25 11:40:56.000000 fisspy-1.0.6/fisspy/align/base.py
+drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-25 11:55:19.719058 fisspy-1.0.6/fisspy/analysis/
+-rw-r--r--   0 jhkang     (501) staff       (20)      317 2024-04-20 02:57:09.000000 fisspy-1.0.6/fisspy/analysis/__init__.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    12577 2024-04-25 11:37:49.000000 fisspy-1.0.6/fisspy/analysis/doppler.py
+-rw-r--r--   0 jhkang     (501) staff       (20)     1030 2024-04-20 02:57:09.000000 fisspy-1.0.6/fisspy/analysis/filter.py
+-rw-r--r--   0 jhkang     (501) staff       (20)     2988 2024-04-25 11:30:36.000000 fisspy-1.0.6/fisspy/analysis/forecast.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    15224 2024-04-20 02:57:09.000000 fisspy-1.0.6/fisspy/analysis/ofe.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    35498 2024-04-25 11:29:47.000000 fisspy-1.0.6/fisspy/analysis/tdmap.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    33907 2024-04-25 11:35:30.000000 fisspy-1.0.6/fisspy/analysis/wavelet.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    19011 2023-07-14 01:35:52.000000 fisspy-1.0.6/fisspy/cm.py
+drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-25 11:55:19.720080 fisspy-1.0.6/fisspy/correction/
+-rw-r--r--   0 jhkang     (501) staff       (20)       51 2024-04-20 02:57:09.000000 fisspy-1.0.6/fisspy/correction/__init__.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    11372 2024-04-20 02:57:09.000000 fisspy-1.0.6/fisspy/correction/correction.py
+-rw-r--r--   0 jhkang     (501) staff       (20)     2337 2024-04-20 02:57:09.000000 fisspy-1.0.6/fisspy/correction/get_inform.py
+drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-25 11:55:19.720992 fisspy-1.0.6/fisspy/data/
+-rw-r--r--   0 jhkang     (501) staff       (20)       64 2023-07-25 08:49:17.000000 fisspy-1.0.6/fisspy/data/__init__.py
+-rw-r--r--   0 jhkang     (501) staff       (20)     1072 2023-07-25 08:49:17.000000 fisspy-1.0.6/fisspy/data/_sample.py
+-rw-r--r--   0 jhkang     (501) staff       (20)     2965 2023-07-25 08:49:17.000000 fisspy-1.0.6/fisspy/data/download.py
+-rw-r--r--   0 jhkang     (501) staff       (20)      394 2023-07-14 01:35:52.000000 fisspy-1.0.6/fisspy/data/sample.py
+drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-25 11:55:19.721813 fisspy-1.0.6/fisspy/image/
+-rw-r--r--   0 jhkang     (501) staff       (20)       73 2024-04-25 10:45:58.000000 fisspy-1.0.6/fisspy/image/__init__.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    29769 2024-04-25 11:21:02.000000 fisspy-1.0.6/fisspy/image/interactive_image.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    11423 2024-04-25 11:54:55.000000 fisspy-1.0.6/fisspy/image/raster_set.py
+drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-25 11:55:19.722037 fisspy-1.0.6/fisspy/inversion/
+-rw-r--r--   0 jhkang     (501) staff       (20)        0 2024-04-20 02:57:09.000000 fisspy-1.0.6/fisspy/inversion/__init__.py
+-rw-r--r--   0 jhkang     (501) staff       (20)      181 2024-04-20 02:57:09.000000 fisspy-1.0.6/fisspy/inversion/_mlsi.py
+drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-25 11:55:19.722493 fisspy-1.0.6/fisspy/io/
+-rw-r--r--   0 jhkang     (501) staff       (20)      320 2023-07-14 01:35:52.000000 fisspy-1.0.6/fisspy/io/__init__.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    15840 2023-07-14 01:35:52.000000 fisspy-1.0.6/fisspy/io/read.py
+-rw-r--r--   0 jhkang     (501) staff       (20)     4974 2024-04-20 02:57:09.000000 fisspy-1.0.6/fisspy/makevideo.py
+drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-25 11:55:19.724257 fisspy-1.0.6/fisspy/preprocess/
+-rw-r--r--   0 jhkang     (501) staff       (20)       29 2024-04-20 02:57:09.000000 fisspy-1.0.6/fisspy/preprocess/__init__.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    52443 2024-04-25 11:18:41.000000 fisspy-1.0.6/fisspy/preprocess/proc_base.py
+-rw-r--r--   0 jhkang     (501) staff       (20)   143266 2024-04-20 02:57:09.000000 fisspy-1.0.6/fisspy/preprocess/proc_gui.py
+-rw-r--r--   0 jhkang     (501) staff       (20)     1685 2024-04-20 02:57:09.000000 fisspy-1.0.6/fisspy/preprocess/t_y_sh.py
+drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-25 11:55:19.726071 fisspy-1.0.6/fisspy/read/
+-rw-r--r--   0 jhkang     (501) staff       (20)      195 2024-04-20 02:57:09.000000 fisspy-1.0.6/fisspy/read/__init__.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    49069 2024-04-25 11:24:21.000000 fisspy-1.0.6/fisspy/read/read_factory.py
+-rw-r--r--   0 jhkang     (501) staff       (20)     6847 2024-04-25 06:03:54.000000 fisspy-1.0.6/fisspy/read/readbase.py
+drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-04-25 11:55:19.716693 fisspy-1.0.6/fisspy.egg-info/
+-rw-r--r--   0 jhkang     (501) staff       (20)      574 2024-04-25 11:55:19.000000 fisspy-1.0.6/fisspy.egg-info/PKG-INFO
+-rw-r--r--   0 jhkang     (501) staff       (20)     1079 2024-04-25 11:55:19.000000 fisspy-1.0.6/fisspy.egg-info/SOURCES.txt
+-rw-r--r--   0 jhkang     (501) staff       (20)        1 2024-04-25 11:55:19.000000 fisspy-1.0.6/fisspy.egg-info/dependency_links.txt
+-rw-r--r--   0 jhkang     (501) staff       (20)        1 2024-04-25 11:55:19.000000 fisspy-1.0.6/fisspy.egg-info/not-zip-safe
+-rw-r--r--   0 jhkang     (501) staff       (20)      137 2024-04-25 11:55:19.000000 fisspy-1.0.6/fisspy.egg-info/requires.txt
+-rw-r--r--   0 jhkang     (501) staff       (20)        7 2024-04-25 11:55:19.000000 fisspy-1.0.6/fisspy.egg-info/top_level.txt
+-rw-r--r--   0 jhkang     (501) staff       (20)       38 2024-04-25 11:55:19.726673 fisspy-1.0.6/setup.cfg
+-rw-r--r--   0 jhkang     (501) staff       (20)      582 2024-04-25 11:51:00.000000 fisspy-1.0.6/setup.py
```

### Comparing `fisspy-1.0.5/LICENSE.txt` & `fisspy-1.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.5/README.md` & `fisspy-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.5/fisspy/align/alignment.py` & `fisspy-1.0.6/fisspy/align/alignment.py`

 * *Files 3% similar despite different names*

```diff
@@ -307,20 +307,20 @@
     Parameters
     ----------
     data: `~numpy.ndarray`
         3-dimensional data array with the shape of (nt, ny, nx).
     fapar: `dict`
         File name of the alignpar.
     xmargin: `int`
-        margin for x-axis.
+        Margin for x-axis.
         The size of the x-axis increases to nx + 2*xmargin.
         If None, automatically calculate the margin.
         Default is None.
     ymargin: `int`
-        margin for y-axis
+        Margin for y-axis
         The size of the x-axis increases to ny + 2*ymargin.
         If None, automatically calculate the margin.
         Default is None.
     cubic: `bool`, (optional)
         Use cubic interpolation to determine the value in the aligned position.
         If False, use linear interpolation.
         Default is None.
@@ -365,30 +365,39 @@
                         dy=apar['dy'][i],
                         xmargin=xm, ymargin=ym,
                         cubic=cubic)
         cdata[i] = rimg
 
     return cdata
 
-def alignTwoDataCubes(dataA, dataB, faparA, faparB, cubic=False):
+def alignTwoDataCubes(dataA, dataB, faparA, faparB, xmargin=None, ymargin=None, cubic=False):
     """
     Align two 3D data cubes.
     Note that the data will be flip in the x axis to correct the mirror reversal.
-    Margin will be automatically calculated.
 
     Parameters
     ----------
     dataA: `~numpy.ndarray`
         3-dimensional data array for cam A with the shape of (nt, ny, nx).
     dataB: `~numpy.ndarray`
         3-dimensional data array for cam B with the shape of (nt, ny, nx).
     faparA: `str`
         File name of the alignpar for cam A.
     faparB: `str`
         File name of the alignpar for cam B.
+    xmargin: `int`, (optional)
+        Margin for x-axis.
+        The size of the x-axis increases to nx + 2*xmargin.
+        If None, automatically calculate the margin.
+        Default is None.
+    ymargin: `int`, (optional)
+        Margin for y-axis
+        The size of the x-axis increases to ny + 2*ymargin.
+        If None, automatically calculate the margin.
+        Default is None.
     cubic: `bool`, (optional)
         Use cubic interpolation to determine the value in the aligned position.
         If False, use linear interpolation.
         Default is None.
     
     Returns
     -------
@@ -397,16 +406,22 @@
     """
     nt, ny, nx = dataA.shape
     l = ((nx//2)**2+(ny//2)**2)**0.5
     aparA = readAlignPars(faparA)
     aparB = readAlignPars(faparB)
     ang0 = np.arctan2(ny//2,nx//2)
     ang = aparA['angle']+ang0
-    xm = int(l*np.cos(ang).max() - nx//2 + int(abs(aparB['dx'][100])) + 0.5)
-    ym = int(l*np.sin(ang).max() - ny//2 + int(abs(aparB['dy'][100])) + 0.5)
+    if xmargin is None:
+        xm = int(l*np.cos(ang).max() - nx//2 + int(abs(aparB['dx'][100])) + 0.5)
+    else:
+        xm = xmargin
+    if ymargin is None:
+        ym = int(l*np.sin(ang).max() - ny//2 + int(abs(aparB['dy'][100])) + 0.5)
+    else:
+        ym = ymargin
 
     cdataA = alignDataCube(dataA, faparA, xmargin=xm, ymargin=ym, cubic=cubic)
     cdataB = alignDataCube(dataB, faparB, xmargin=xm, ymargin=ym, cubic=cubic)
     return cdataA, cdataB
 
 def saveAlignCube(adata, time, sname, dt=None, dx=0.16*725, dy=0.16*725):
     """
```

### Comparing `fisspy-1.0.5/fisspy/align/base.py` & `fisspy-1.0.6/fisspy/align/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -103,17 +103,17 @@
     if cor:
         img = shiftImage(image, [-y, -x])
         xx = np.arange(nx) + x
         yy = np.arange(ny) + y
         kx = np.logical_and(xx >= 0, xx <= nx - 1)
         ky = np.logical_and(yy >= 0, yy <= ny - 1)
         roi = np.logical_and(kx, ky[:,None])
-        cor = (img*template)[roi].sum()/np.sqrt((img[roi]**2).sum() *
+        COR = (img*template)[roi].sum()/np.sqrt((img[roi]**2).sum() *
                       (template[roi]**2).sum())
-        return np.array([y, x]), cor
+        return np.array([y, x]), COR
     else:
         return np.array([y, x])
 
 def CoordinateTransform(x, y, xc, yc, angle, dx=0, dy=0, inv=False):
     """
     Coordinate transform from cartesian to polar coordinates or vice versa.
 
@@ -324,18 +324,18 @@
     x = np.arange(nx)
     y = np.arange(ny)[:,None]
     xa = np.arange(nx1)-xmargin
     ya = (np.arange(ny1)-ymargin)[:,None]
 
 
     if not xc:
-        xc = nx/2
+        XC = nx/2
     if not yc:
-        yc = ny/2
-    xt, yt = CoordinateTransform(xa, ya, xc, yc, angle, dx=dx, dy=dy)
+        YC = ny/2
+    xt, yt = CoordinateTransform(xa, ya, XC, YC, angle, dx=dx, dy=dy)
     return get_interpVal(img, x, y, xt, yt, missing=missing, cubic=cubic)
 
 def shiftImage(image, sh, missing=0, cubic=False):
     """
     Shift the given image.
 
     Parameters
```

### Comparing `fisspy-1.0.5/fisspy/analysis/doppler.py` & `fisspy-1.0.6/fisspy/analysis/doppler.py`

 * *Files 1% similar despite different names*

```diff
@@ -260,50 +260,50 @@
     elif rfm == 'cm':
         wc = wv[s]
         wc0 = np.copy(wc)
         more = data[posi0,s0] > 0.
         residual = np.zeros(na)
         dresid = np.zeros(na)
         if alpha is None:
-            alpha = 1
+            Alpha = 1
         sigmaratio = (0.1*data.mean())/hw
         while  (ref > 1e-4 or rep < 5)  and rep <  30 and more.sum() > 0:
             posi = posi0[more]
             wls = np.array((posi, wc[more]-hw)).T
             wrs = np.array((posi, wc[more]+hw)).T
 
             delta = (interp(wrs)-interp(wls)) 
             delta1d = (interp(wrs+dwv)-interp(wrs-dwv) -interp(wls+dwv)+interp(wls-dwv))/(2*dwv)
             
     #        delta2d = (interp(wrs+eps)-2*interp(wrs)+interp(wrs-eps) \
     #                   -interp(wls+eps)+ 2*interp(wls)-interp(wls-eps))/eps**2
             residual[more] = delta * delta1d   \
-                    + (wc[more] - wc0[more])*alpha*sigmaratio**2
-            dresid[more] = delta1d**2 + alpha*sigmaratio**2
+                    + (wc[more] - wc0[more])*Alpha*sigmaratio**2
+            dresid[more] = delta1d**2 + Alpha*sigmaratio**2
             dwc[more] = -0.4*residual[more]/dresid[more]
                 
             
             wc[more] += dwc[more]
             ref0 = abs(dwc)
             ref = ref0.max()
             intc[more] = 0.5*(interp(wls)+interp(wrs))
             #if rep ==0:
             #    print('intc[more].shape=', intc[more].shape)
             more = (ref0 > 1e-4) 
             rep += 1
         # print(f'rep={rep:3.0f}, more.sum={more.sum():3.0f}')
             
             if rep > 2:
-                alpha *= 0.1**(1./2.)
+                Alpha *= 0.1**(1./2.)
                 
-            alpha = np.maximum(alpha, 1.e-2)
+            Alpha = np.maximum(Alpha, 1.e-2)
 
     elif rfm == 'nrm': # Newton-Raphson Method
         if alpha is None:
-            alpha = 1
+            Alpha = 1
         wc = wv[s0].copy()
         while ref >1e-4 and rep < 30 and more.sum() > 0:
             posi = posi0[more]
             wl = np.array((posi, wc[more]-hw)).T
             wr = np.array((posi ,wc[more]+hw)).T
             Fl = interp(wl)
             Fr = interp(wr) 
@@ -315,27 +315,27 @@
             dFr = (Fr_p-Fr_n)/(2*dwv)
             dFl = (Fl_p-Fl_n)/(2*dwv)
             # dFl = ginterp(wl)
             # dFr = ginterp(wr)
             dF = dFr-dFl
             f = F**2
             df = 2*F*dF
-            dwc[more] = -alpha*f/(df+np.sign(df)*1e-3)
+            dwc[more] = -Alpha*f/(df+np.sign(df)*1e-3)
             # dwc[more] = -f/df
             
             wc[more] += dwc[more]
             ref0 = abs(dwc)
             ref = ref0.max()
             intc[more] = 0.5*(Fr+Fl)
             more = ref0 > 1e-4
             rep += 1
             
     elif rfm == 'hm': # Halley's method (modified NRM)
         if alpha is None:
-            alpha = 1
+            Alpha = 1
         wc = wv[s0].copy()
         while ref >1e-4 and rep < 30 and more.sum() > 0:
             posi = posi0[more]
             wl = np.array((posi, wc[more]-hw)).T
             wr = np.array((posi ,wc[more]+hw)).T
             Fl = interp(wl)
             Fr = interp(wr) 
@@ -348,15 +348,15 @@
             dFl = (Fl_p-Fl_n)/(2*dwv)
             dF = dFr-dFl
             dF2 = (Fr_p-2*Fr+Fr_n - (Fl_p-2*Fl+Fl_n))/dwv**2
             f = F**2
             df = 2*F*dF
             df2 = 2*(dF**2+F*dF2)
             denom = (df**2-0.5*f*df2)
-            dwc[more] = -alpha*f*df/(denom+np.sign(denom)*1e-3)
+            dwc[more] = -Alpha*f*df/(denom+np.sign(denom)*1e-3)
             
             wc[more] += dwc[more]
             ref0 = abs(dwc)
             ref = ref0.max()
             intc[more] = 0.5*(Fr+Fl)
             more = ref0 > 1e-4
             rep += 1
```

### Comparing `fisspy-1.0.5/fisspy/analysis/filter.py` & `fisspy-1.0.6/fisspy/analysis/filter.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.5/fisspy/analysis/forecast.py` & `fisspy-1.0.6/fisspy/analysis/forecast.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,22 +32,22 @@
         It must be larger elements then input data.
     tf : `~numpy.ndarray`
         Time the forecasted ARdata points.
     
     """
     if not dt:
         tmp = np.roll(time, -1) - time
-        dt = np.median(tmp[:-1])
+        DT = np.median(tmp[:-1])
     
     shape = data.shape
     if shape[0]!=len(time):
         raise ValueError('The size of data is different from the size of time.')
         
     t = (time-time[0])
-    tf = np.arange(t[0], t[-1], dt, dtype=float)
+    tf = np.arange(t[0], t[-1], DT, dtype=float)
     
     interp = interp1d(t, data, kind='cubic', axis=0)
     datai = interp(tf)
     shapei = datai.shape
     nt = len(tf)
     
     if data.ndim == 1:
@@ -57,22 +57,22 @@
     datat = datai.reshape((nt, nl))
 
     # shapei=datat.shape
     # datat=datat.reshape((shapei[0],np.prod(shapei[1:])))
     # shapet=datat.shape
     
     td = t - np.roll(t,1)
-    addi = np.where(td >= dt*1.5)[0]
+    addi = np.where(td >= DT*1.5)[0]
 
     nad = len(addi)
     if nad == 0:
         print("There is no empty element. Just interpolate to evenly sample the data.")
         return datai
 
-    npredict = (td[addi]/dt + 0.5).astype(int)-1
+    npredict = (td[addi]/DT + 0.5).astype(int)-1
     
     for i in range(nad):
         ts = np.abs(tf - t[addi[i]-1]).argmin()+1
         te = ts+npredict[i]
         
         if ts//2 < 10:
             fskip = True
```

### Comparing `fisspy-1.0.5/fisspy/analysis/ofe.py` & `fisspy-1.0.6/fisspy/analysis/ofe.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.5/fisspy/analysis/tdmap.py` & `fisspy-1.0.6/fisspy/analysis/tdmap.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,16 +63,16 @@
         self.aspect = aspect
         self.nt, self.ny, self.nx = data.shape
         self.dx = dx
         self.dy = dy
         self.dt = dt
         self.clim = clim
         if cmap is None:
-            cmap = plt.cm.gray
-        self.cmap = cmap
+            Cmap = plt.cm.gray
+        self.cmap = Cmap
         self.analysis = None
         self.a_fig = None
         self.a_ax = None
         self.h_fig = None
         self.t = 0
         self.time = np.arange(0, self.nt)*self.dt
         self.slitPoint = []
@@ -88,30 +88,30 @@
         self.Tline_pos = []
         self.Ddistance = []
         self.Dline_pos = []
 
         # figure window label
         afl = plt.get_figlabels()
         if label is None:
-            label = 'Unknown'
-        if label in afl:
+            Label = 'Unknown'
+        if Label in afl:
             ii = 0
             tmp2 = []
             for aa in afl:
                 if aa.find('-TD') == -1:
                     continue
-                tmp = aa.split(f'{label}_case')
+                tmp = aa.split(f'{Label}_case')
                 if len(tmp) > 1:
                     ii += 1
                     tmp2 += [int(tmp[-1])]
             if ii == 0:
-                label = label+'_case2'
+                Label = Label+'_case2'
             else:
-                label = label+f'_caseq{max(tmp2)+1}'
-        self.label = label
+                Label = Label+f'_caseq{max(tmp2)+1}'
+        self.label = Label
 
         # make interpolation function
         smin = [0, 0, 0]
         smax = [(self.nt-1)*dt, (self.ny-1)*dy, (self.nx-1)*dx]
         order = data.shape
         self.interp = LinearSpline(smin, smax, order, data)
 
@@ -121,17 +121,17 @@
         l = -dx*0.5
         r = (self.nx - 0.5)*dx
         b = -dy*0.5
         t = (self.ny - 0.5)*dy
         self.extent = [l, r, b, t]
         
         if figsize is None:
-            figsize = [8,8*wratio+0.2]
+            fs = [8,8*wratio+0.2]
 
-        self.fig, self.ax = plt.subplots(figsize=figsize, dpi=dpi, num=self.label)
+        self.fig, self.ax = plt.subplots(figsize=fs, dpi=dpi, num=self.label)
         self.im = self.ax.imshow(self.data[self.t], self.cmap, extent=self.extent, origin='lower')
         if self.clim is not None:
             self.im.set_clim(self.clim)
         self.ax.set_title('t = 0 (sec)')
         self.ax.set_xlabel('X (km)')
         self.ax.set_ylabel('Y (km)')
         self.fig.canvas.mpl_connect('key_press_event', self._onKey)
@@ -444,32 +444,32 @@
         self.Dline_pos = []
         self.dTexts = []
         self.h_fig = None
 
         # figure window label
         afl = plt.get_figlabels()
         if label is None:
-            label = 'Unknown-TD'
+            Label = 'Unknown-TD'
         else:
-            label = label+'-TD'
-        if label in afl:
-            l0 = label.split('-TD')[0]
+            Label = Label+'-TD'
+        if Label in afl:
+            l0 = Label.split('-TD')[0]
             ii = 0
             tmp2 = []
             for aa in afl:
                 tmp = aa.split(f'{l0}_case')
                 if len(tmp) > 1:
                     ii += 1
                     tmp2 += [int(tmp[-1])]
             if ii == 0:
-                label = l0+'_case2-TD'
+                Label = l0+'_case2-TD'
             else:
                 print(1)
-                label = l0+f'_case{max(tmp2)+1}-TD'
-        self.label = label
+                Label = l0+f'_case{max(tmp2)+1}-TD'
+        self.label = Label
         l = -0.5*dt
         r = (self.nt - 0.5)*dt
         b = -dl*0.5
         t = (self.nl - 0.5)*dl
         extent = [l, r, b, t]
 
         # figsize = [19,8]
@@ -495,15 +495,15 @@
             ym = ymargin = yM/fy
 
             ys2 = ky*fy*(1-2.5*ym)
             xs2 = ys2*xl/(aspect*yl)
             fx = xs2/kx+ 2.5*xM
             xm = xmargin = xM/fx
         ym = ymargin = yM/fy
-        self.fig, self.ax = plt.subplots(figsize=[fx,fy], dpi=dpi, label=label)
+        self.fig, self.ax = plt.subplots(figsize=[fx,fy], dpi=dpi, label=self.label)
 
         self.ax.set_position([xmargin, ymargin, (1-2.5*xmargin)/9*8, (1-2.5*ymargin)/3*2])
         self.axT = self.fig.add_subplot(111, sharex=self.ax)
         self.axT.set_position([xmargin, ymargin*2+(1-2.5*ymargin)/3*2, (1-2.5*xmargin)/9*8, (1-2.5*ymargin)/3])
         self.axD = self.fig.add_subplot(111, sharey=self.ax)
         self.axD.set_position([xmargin*2+(1-2.5*xmargin)/9*8, ymargin, (1-2.5*xmargin)/9, (1-2.5*ymargin)/3*2])
         self.imTD = self.ax.imshow(TD, cmap, origin='lower', extent=extent, aspect=aspect)
```

### Comparing `fisspy-1.0.5/fisspy/analysis/wavelet.py` & `fisspy-1.0.6/fisspy/analysis/wavelet.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,21 +90,21 @@
         
         shape0 = np.array(data.shape)
         self.n0 = shape0[axis]
         shape = np.delete(shape0, axis)
         self.axis = axis
         
         if not s0:
-            s0 = 2*dt
+            S0 = 2*dt
         if not j:
-            j = int(np.log2(self.n0*dt/s0)/dj)
+            j = int(np.log2(self.n0*dt/S0)/dj)
         else:
             j=int(j)
         
-        self.s0 = s0
+        self.s0 = S0
         self.j = j
         self.dt = dt
         self.dj = dj
         self.mother = mother.upper()
         self.param = param
         self.pad = pad
         self.axis = axis
@@ -626,30 +626,30 @@
         self.axWavelet = self.fig.add_subplot(gs[2:5, :3], sharex=self.axData)
         self.axGlobal = self.fig.add_subplot(gs[2:5, 3], sharey=self.axWavelet)
         self.axScaleAvg = self.fig.add_subplot(gs[5:7, :3], sharex=self.axData)
         periodMax = self.period.max()
         periodMax = periodMax if periodMax<64 else 64
         
         if time is None:
-            time = self.dt*np.arange(n)
+            ttime = self.dt*np.arange(n)
         if levels is None:
-            levels = [0.05, 0.12,0.229,
+            Levels = [0.05, 0.12,0.229,
                       0.45]
             
         # Plot Time Series
         if title[0] is None:
             self.axData.set_title('a) Time Series')
         else:
             self.axData.set_title(title)
         self.axData.set_ylabel('Value')
         self.axData.minorticks_on()
         self.axData.tick_params(which='both', direction='in')
-        self.pData = self.axData.plot(time, self.data,
+        self.pData = self.axData.plot(ttime, self.data,
                                       color='k', lw=1.5)[0]
-        self.axData.set_xlim(time[0], time[-1])
+        self.axData.set_xlim(ttime[0], ttime[-1])
         
         # Contour Plot Wavelet Power Spectrum
         if title[1] is None:
             self.axWavelet.set_title('b) Wavelet Power Spectrum')
         else:
             self.axWavelet.set_title(title)
         self.axWavelet.set_ylabel('Period')
@@ -658,27 +658,27 @@
         self.axWavelet.tick_params(which='both', direction='in')
         self.axWavelet.set_yscale('symlog', basey=2)
         self.axWavelet.yaxis.set_major_formatter(ticker.ScalarFormatter())
         self.axWavelet.ticklabel_format(axis='y',style='plain')
         self.axWavelet.set_ylim(periodMax, 0.5)
         
         wpower = self.power/self.power.max()
-        self.contour = self.axWavelet.contourf(time, self.period,
-                                               wpower, len(levels),
+        self.contour = self.axWavelet.contourf(ttime, self.period,
+                                               wpower, len(Levels),
                                                colors=['w'])
         self.contourIm = self.axWavelet.contourf(self.contour,
-                                                 levels=levels,
+                                                 levels=Levels,
                                                  cmap=plt.cm.Spectral_r, extend='max')
         signif = self.waveSignif(self.data, sigtest=0, lag1=lag1, siglvl=0.90,
                                  gws=self.gws)
         sig90 = signif[:,None]
         sig90 = self.power/sig90
         
-        self.axWavelet.contour(time, self.period, sig90, [-99,1] ,colors='r')
-        self.axWavelet.fill_between(time, self.coi,
+        self.axWavelet.contour(ttime, self.period, sig90, [-99,1] ,colors='r')
+        self.axWavelet.fill_between(ttime, self.coi,
                                     self.period.max(), color='grey',
                                     alpha=0.4, hatch='x')
         
         # Plot Global Wavelet Spectrum
         if title[2] is None:
             self.axGlobal.set_title('c) Global')
         else:
@@ -713,15 +713,15 @@
         self.axScaleAvg.set_ylabel('Avg')
         self.axScaleAvg.minorticks_on()
         self.axScaleAvg.tick_params(which='both', direction='in')
         
         period_mask = (self.period >= 2)*(self.period < 8)
         power_norm = self.power/self.scale[:,None]
         power_avg = self.dj*self.dt/self.cdelta*power_norm[period_mask,:].sum(0)
-        self.pScaleAvg = self.axScaleAvg.plot(time,
+        self.pScaleAvg = self.axScaleAvg.plot(ttime,
                                               power_avg,
                                               color='k',
                                               lw=1.5)
         
         self.fig.tight_layout()
 
 
@@ -811,16 +811,16 @@
         >>> gCross = res.global_cross
         >>> gPhase = res.global_phase
         >>> power1 = res.power1
         >>> power2 = res.power2
         >>> time_out = res.time
         >>> scale_out = res.scale
         """
-        if not dt: dt = time1[1]-time1[0]
-        if not dj: dj = np.log2(scale1[1]/scale1[0])
+        if not dt: DT = time1[1]-time1[0]
+        if not dj: DJ = np.log2(scale1[1]/scale1[0])
         if time1 is time2:
             t1s = 0
             t1e = len(time1)
             t2s = t1s
             t2e = t1e
         else:
             otime_start = min([time1.min(),time2.min()])
@@ -852,32 +852,32 @@
         global1 = self.power1.sum(1)
         global2 = self.power2.sum(1)
         self.global_cross = self.cross_wavelet.sum(1)
         self.global_coher = np.abs(self.global_cross)**2/(global1*global2)
         self.global_phase = np.arctan(self.global_cross.imag/self.global_cross.real)*180./np.pi
         
         if not nosmooth:
-            nt = (4*self.scale/dt)//2*4+1
+            nt = (4*self.scale/DT)//2*4+1
             nt2 = nt[:,None]
             ntmax = nt.max()
             g = np.arange(ntmax) * np.ones((nj,1))
             wh = g >= nt2
-            time_wavelet = (g-nt2//2)*dt/self.scale[:,None]
+            time_wavelet = (g-nt2//2)*DT/self.scale[:,None]
             wave_func = np.exp(-time_wavelet**2/2)
             wave_func[wh] = 0
             wave_func = (wave_func/wave_func.sum(1)[:,None]).real
             self.cross_wavelet = _fastConv(self.cross_wavelet, wave_func, nt2)
             self.power1 = _fastConv(self.power1, wave_func, nt2)
             self.power2 = _fastConv(self.power2, wave_func, nt2)
             scales = self.scale[:, None]
             self.cross_wavelet /= scales
             self.power1 /= scales
             self.power2 /= scales
             
-            nw = int(0.6/dj/2 + 0.5)*2-1
+            nw = int(0.6/DJ/2 + 0.5)*2-1
             weight = np.ones(nw)/nw
             self.cross_wavelet = _fastConv2(self.cross_wavelet, weight)
             self.power1 = _fastConv2(self.power1,weight)
             self.power2 = _fastConv2(self.power2,weight)
             
             self.wave_phase = 180./np.pi*np.arctan(self.cross_wavelet.imag/self.cross_wavelet.real)
             power3=self.power1*self.power2
```

### Comparing `fisspy-1.0.5/fisspy/cm.py` & `fisspy-1.0.6/fisspy/cm.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.5/fisspy/correction/correction.py` & `fisspy-1.0.6/fisspy/correction/correction.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.5/fisspy/correction/get_inform.py` & `fisspy-1.0.6/fisspy/correction/get_inform.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.5/fisspy/data/_sample.py` & `fisspy-1.0.6/fisspy/data/_sample.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.5/fisspy/data/download.py` & `fisspy-1.0.6/fisspy/data/download.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.5/fisspy/image/interactive_image.py` & `fisspy-1.0.6/fisspy/image/interactive_image.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,21 +13,21 @@
     """
     Draw interactive FISS raster, spectrogram and profile for single band.
 
     Parameters
     ----------
     fiss: `fisspy.read.FISS`
         FISS class.
-    x : `float`
+    X : `float`
         X position that you draw a spectral profile.
         Default is image center.
-    y : `float`
+    Y : `float`
         Y position that you draw a spectral profile.
         Default is image center.
-    wv : `float`
+    WV : `float`
         Wavelength positin that you draw a raster images.
         Default is central wavelength.
     scale : `string`
         Scale method of colarbar limit.
         Default is minMax.
         option: 'minMax', 'std', 'log'
     sigFactor : `float`
@@ -38,28 +38,28 @@
         Default is True
 
     Other Parameters
     ----------------
     **kwargs : `~matplotlib.pyplot` properties
     """
 
-    def __init__(self, fiss, x=None, y=None, wv=None, scale='minMax',
+    def __init__(self, fiss, X=None, Y=None, WV=None, scale='minMax',
                  sigFactor=3, helpBox=True, **kwargs):
 
         try:
             plt.rcParams['keymap.back'].remove('left')
             plt.rcParams['keymap.forward'].remove('right')
         except:
             pass
 
-        if not x:
+        if not X:
             x = fiss.nx//2*fiss.xDelt
-        if not y:
+        if not Y:
             y = fiss.ny//2*fiss.yDelt
-        if not wv:
+        if not WV:
             wv = fiss.centralWavelength
         self.extentRaster = fiss.extentRaster
         self.extentSpectro = fiss.extentSpectro
         self.scale = scale
         self.sigFactor = sigFactor
         self.hw = kwargs.pop('hw', 0.05)
         self.xpix = round((x-fiss.xDelt/2)/fiss.xDelt)
@@ -189,15 +189,15 @@
         self.pointRaster = self.axRaster.scatter(self.x, self.y, 50,
                                                  marker='x',
                                                  color='r')
         self.axSpectro.set_aspect(adjustable='box', aspect='auto')
         self.fig.tight_layout()
         self.fig.canvas.mpl_connect('key_press_event', self._on_key)
 
-        plt.show()
+        self.fig.show()
 
     def _on_key(self, event):
 
         ### Interactive keyboard input
         # Position
         if event.key == 'ctrl+right' or event.key == 'cmd+right':
             if self.x < self._xMax:
@@ -371,15 +371,15 @@
         Show the interacitve key and simple explanation.
         Default is True
 
     Other Parameters
     ----------------
     **kwargs : `~matplotlib.pyplot` properties
     """
-    def __init__(self, fissA, fissB, x=None, y=None, wvA=None, wvB=None,
+    def __init__(self, fissA, fissB, X=None, Y=None, WVA=None, WVB=None,
                  scale='minMax', sigFactor=3, helpBox=True, **kwargs):
 
         try:
             plt.rcParams['keymap.back'].remove('left')
             plt.rcParams['keymap.forward'].remove('right')
         except:
             pass
@@ -405,21 +405,21 @@
 
         sh = alignOffset(self.fissB.data[:,:,50], self.fissA.data[:,:,-50])
         tmp = shiftImage3D(fissB.data.transpose(2, 0, 1), -sh).transpose(1,2,0)
         self.fissB.data = tmp
         tmp[tmp<10]=1
         del tmp
 
-        if not x:
+        if not X:
             x = self.nx//2*self.xDelt
-        if not y:
+        if not Y:
             y = self.ny//2*self.yDelt
-        if not wvA:
+        if not WVA:
             wvA = self.fissA.centralWavelength
-        if not wvB:
+        if not WVB:
             wvB = self.fissB.centralWavelength
         xpix = round((x-self.xDelt/2)/self.xDelt)
         ypix = round((y-self.yDelt/2)/self.yDelt)
         self.x = xpix*self.xDelt+self.xDelt/2
         self.y = ypix*self.yDelt+self.yDelt/2
         self.scale = scale
         self.sigFactor = sigFactor
@@ -541,17 +541,16 @@
                                                    marker='x',
                                                    color='r')
         self.pointRasterB = self.axRasterB.scatter(self.x, self.y, 50,
                                                    marker='x',
                                                    color='r')
         self.fig.tight_layout()
         self.fig.canvas.mpl_connect('key_press_event', self._on_key)
+        self.fig.show()
 
-
-        plt.show()
     def _on_key(self, event):
 
         if event.key == 'ctrl+right' or event.key == 'cmd+right':
             if self.x < self._xMax:
                 self.x += self.xDelt
             else:
                 self.x = self._xMin+self.xDelt//2
```

### Comparing `fisspy-1.0.5/fisspy/io/read.py` & `fisspy-1.0.6/fisspy/io/read.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.5/fisspy/makevideo.py` & `fisspy-1.0.6/fisspy/makevideo.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.5/fisspy/preprocess/proc_base.py` & `fisspy-1.0.6/fisspy/preprocess/proc_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1381,44 +1381,46 @@
         m = c_arr.mean()
         c_arr = np.nan_to_num(c_arr, True, m,m,m)
         # c_arr[c_arr == -np.inf] = 0
         # c_arr[c_arr == np.inf] = 0
 
         Eval, Evec = np.linalg.eig(c_arr)
         if ncoeff is None:
-            ncoeff = (Eval >= tol).sum()
-            ncoeff = ncoeff if ncoeff < 50 else 50
-            ncoeff = ncoeff if ncoeff > 30 else 30
-            print(f"eigenvalue[{ncoeff}]: {Eval[50]:.3f}")
-        Evec = Evec[:,:ncoeff].T
+            NC = (Eval >= tol).sum()
+            NC = NC if NC < 50 else 50
+            NC = NC if NC > 30 else 30
+            print(f"eigenvalue[{NC}]: {Eval[50]:.3f}")
+        else:
+            NC = ncoeff
+        Evec = Evec[:,:NC].T
 
         hdu = fits.PrimaryHDU(Evec.astype('float32'))
-        hdu.header['ncoeff'] = ncoeff
+        hdu.header['NC'] = NC
         hdu.header['date'] = h['date']
         hdu.writeto(pfile, overwrite=True)
         
         
     else:
         if Evec is None:
             opn = fits.open(pfile)
             ph = opn.header
             Evec = opn.data
 
-        ncoeff = Evec.shape[0]
+        NC = Evec.shape[0]
 
 
-    coeff = np.zeros((nx, ny, ncoeff+1))
+    coeff = np.zeros((nx, ny, NC+1))
     cfile = fproc.replace('.fts', '_c.fts')
     cfile = cfile.replace('proc', 'comp')
     wh = data < 1
     data[wh] = 1
     av = data.mean(2)
     data /= av[:,:,None]
-    coeff[:,:,ncoeff] = np.log10(av)
-    for i in range(ncoeff):
+    coeff[:,:,NC] = np.log10(av)
+    for i in range(NC):
         coeff[:,:,i] = (data[:,:,:]*Evec[i]).sum(2)
 
     bscale = np.abs(coeff).max()/2e4
     coeff = np.round(coeff/bscale)
 
 
     hdu = fits.PrimaryHDU(coeff.astype('int16'))
@@ -1427,20 +1429,20 @@
     for cards in h.cards:
         hdu.header.add_comment(f"{cards[0]} = {cards[1]} / {cards[2]}")
 
     hdu.writeto(cfile, overwrite=True)
 
     if ret and pfile is not None:
         c = coeff*bscale
-        spec = c[:,:,:ncoeff].dot(Evec)
+        spec = c[:,:,:NC].dot(Evec)
         spec *= 10**c[:,:,-1][:,:,None]
         if Eval is None:
             return Evec, spec, odata
         else:
-            return Evec, spec, odata, Eval[ncoeff]
+            return Evec, spec, odata, Eval[NC]
 
 def yf2sp(yf, tolRate=1):
     """
     Calculate the slit pattern using the y-directional Fringe pattern
     """
     d2y = np.gradient(np.gradient(yf,axis=0), axis=0).mean(1)
     pks = find_peaks(d2y[5:-5], d2y[5:-5].std()*tolRate)[0]+5
```

### Comparing `fisspy-1.0.5/fisspy/preprocess/proc_gui.py` & `fisspy-1.0.6/fisspy/preprocess/proc_gui.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.5/fisspy/preprocess/t_y_sh.py` & `fisspy-1.0.6/fisspy/preprocess/t_y_sh.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.0.5/fisspy/read/read_factory.py` & `fisspy-1.0.6/fisspy/read/read_factory.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import astropy.units as u
 import matplotlib.pyplot as plt
 from matplotlib import gridspec
 from matplotlib import ticker
 from .. import cm
 from .readbase import getRaster, getHeader, readFrame
 from ..analysis import lambdameter
-from ..image import interactive_image as II
+from ..image.interactive_image import singleBand
 from ..correction import LineName, wvCalib, smoothingProf, CorSLA
 from ..analysis import FourierFilter, Wavelet, makeTDmap
 
 __author__= "Juhyung Kang"
 __email__ = "jhkang0301@gmail.com"
 __all__ = ["rawData", "FISS", "FD", "calibData", "AlignCube"]
 
@@ -130,25 +130,25 @@
         try:
             plt.rcParams['keymap.back'].remove('left')
             plt.rcParams['keymap.forward'].remove('right')
         except:
             pass
 
         if not x:
-            x = self.nx//2*self.xDelt
+            X = self.nx//2*self.xDelt
         if not y:
-            y = self.ny//2*self.yDelt
+            Y = self.ny//2*self.yDelt
         if not wv:
-            wv = self.centralWavelength
-        self.x = x
-        self.y = y
+            WV = self.centralWavelength
+        self.x = X
+        self.y = Y
         self.wv = wv
         self.imInterp = kwargs.get('interpolation', 'bilinear')
         kwargs['interpolation'] = self.imInterp
-        self.iIm = II.singleBand(self, x, y, wv,
+        self.iIm = singleBand(self, X, Y, WV,
                                   scale=scale, sigFactor=sigFactor,
                                   helpBox=helpBox, **kwargs)  # Basic resource to make interactive image is `~fisspy.image.tdmap.TDmap`
         plt.show()
 
     def chRasterClim(self, cmin, cmax):
         self.iIm.chRasterClim(cmin, cmax)
 
@@ -489,26 +489,26 @@
         try:
             plt.rcParams['keymap.back'].remove('left')
             plt.rcParams['keymap.forward'].remove('right')
         except:
             pass
 
         if x is None:
-            x = self.nx//2*self.xDelt
+            X = self.nx//2*self.xDelt
         if y is None:
-            y = self.ny//2*self.yDelt
+            Y = self.ny//2*self.yDelt
         if wv is None:
-            wv = self.centralWavelength
-        self.x = x
-        self.y = y
-        self.wv = wv
+            WV = self.centralWavelength
+        self.x = X
+        self.y = Y
+        self.wv = WV
         self.imInterp = kwargs.get('interpolation', 'bilinear')
         self.cmap = kwargs.pop('cmap', self.cmap)
         kwargs['interpolation'] = self.imInterp
-        self.iIm = II.singleBand(self, x, y, wv,
+        self.iIm = singleBand(self, X, Y, WV,
                                   scale=scale, sigFactor=sigFactor,
                                   helpBox=helpBox, **kwargs)  # Basic resource to make interactive image is `~fisspy.image.tdmap.TDmap`
 
     def chRasterClim(self, cmin, cmax):
         self.iIm.chRasterClim(cmin, cmax)
 
     def chSpectroClim(self, cmin, cmax):
@@ -530,21 +530,21 @@
         try:
             plt.rcParams['keymap.back'].remove('left')
             plt.rcParams['keymap.forward'].remove('right')
         except:
             pass
 
         if x is None:
-            x = self.nx//2*self.xDelt
+            X = self.nx//2*self.xDelt
         if y is None:
-            y = self.ny//2*self.yDelt
+            Y = self.ny//2*self.yDelt
 
-        self.xpix = round((x-self.xDelt/2)/self.xDelt)
+        self.xpix = round((X-self.xDelt/2)/self.xDelt)
         self.x = self.xpix*self.xDelt+self.xDelt/2
-        self.ypix = round((y-self.yDelt/2)/self.yDelt)
+        self.ypix = round((Y-self.yDelt/2)/self.yDelt)
         self.y = self.ypix*self.yDelt+self.yDelt/2
 
         self.lambdameter(**kw)
         
         # figure setting
         self.fig = plt.figure(figsize=[18,7])
         gs = gridspec.GridSpec(1, 5)
```

### Comparing `fisspy-1.0.5/fisspy/read/readbase.py` & `fisspy-1.0.6/fisspy/read/readbase.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,21 +122,23 @@
         data = fits.getdata(file)[x1:x2]
     if y2 is None:
         data = data[:, y1:]
     else:
         data = data[:, y1:y2]
     ncoeff1 = data.shape[2] - 1
     if not ncoeff:
-        ncoeff = ncoeff1
-    elif ncoeff > ncoeff1:
-        ncoeff = ncoeff1
+        nc = ncoeff1
+    else:
+        nc = ncoeff
+    if nc > ncoeff1:
+        nc = ncoeff1
 
-    spec = np.dot(data[:,:,:ncoeff], pdata[:ncoeff,:])
+    spec = np.dot(data[...,:nc], pdata[:nc,:])
     # spec *= 10.**data[:,:,ncoeff][:,:,None]
-    spec *= 10.**data[:,:,-1][:,:,None]
+    spec *= 10.**data[...,-1][...,None]
     return spec
 
 def getHeader(file):
     """
     Get the FISS fts file header.
 
     Returns
@@ -219,11 +221,13 @@
         Referenced wavelengths.
     hw   : float
         A half-width of wavelength integration in unit of Angstrom.
         Default is 0.05
 
     """
     if hw < abs(wvDelt)/2.:
-        hw = abs(wvDelt)/2.
+        HW = abs(wvDelt)/2.
+    else:
+        HW = hw
 
-    s = np.abs(wave - wvPoint) <= hw
+    s = np.abs(wave - wvPoint) <= HW
     return data[:,:,s].mean(2)
```

### Comparing `fisspy-1.0.5/fisspy.egg-info/SOURCES.txt` & `fisspy-1.0.6/fisspy.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 fisspy/correction/correction.py
 fisspy/correction/get_inform.py
 fisspy/data/__init__.py
 fisspy/data/_sample.py
 fisspy/data/download.py
 fisspy/data/sample.py
 fisspy/image/__init__.py
-fisspy/image/base.py
 fisspy/image/interactive_image.py
 fisspy/image/raster_set.py
 fisspy/inversion/__init__.py
 fisspy/inversion/_mlsi.py
 fisspy/io/__init__.py
 fisspy/io/read.py
 fisspy/preprocess/__init__.py
```

### Comparing `fisspy-1.0.5/setup.py` & `fisspy-1.0.6/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 setup(
     name='fisspy',
-    version='1.0.5',
+    version='1.0.6',
     description='fisspy: Python analysis tools for GST/FISS',
     url='http://fiss.snu.ac.kr',
     author='Juhyung Kang',
     author_email='jhkang@astro.snu.ac.kr',
     license='BSD-2',
     python_requires='>=3.6',
     packages=find_packages(exclude=['docs', 'logo']),
-    install_requires=["numba", "numpy", "scipy>=1.5", "astropy>=5.0", "sunpy>=2.0.0", "matplotlib>=3.0", "interpolation>=2.2", "statsmodels", "beautifulsoup4", "pandas", "ffmpeg", "pyqt>=5.0"],
+    install_requires=["numba", "numpy", "scipy>=1.5", "astropy>=5.0", "sunpy>=2.0.0", "matplotlib>=3.0", "interpolation>=2.2.6", "statsmodels", "beautifulsoup4", "pandas", "ffmpeg", "pyqt>=5.0"],
     zip_safe=False
     )
```


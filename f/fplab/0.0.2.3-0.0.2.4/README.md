# Comparing `tmp/fplab-0.0.2.3.tar.gz` & `tmp/fplab-0.0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fplab-0.0.2.3.tar", last modified: Sun Apr 14 15:01:36 2024, max compression
+gzip compressed data, was "fplab-0.0.2.4.tar", last modified: Thu Apr 25 13:26:02 2024, max compression
```

## Comparing `fplab-0.0.2.3.tar` & `fplab-0.0.2.4.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxrwxrwx   0        0        0        0 2024-04-14 15:01:36.276972 fplab-0.0.2.3/
--rw-rw-rw-   0        0        0     1090 2024-03-31 02:38:30.000000 fplab-0.0.2.3/LICENSE.txt
--rw-rw-rw-   0        0        0      523 2024-04-14 15:01:36.276972 fplab-0.0.2.3/PKG-INFO
--rw-rw-rw-   0        0        0      862 2024-04-06 15:56:56.000000 fplab-0.0.2.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-14 15:01:36.166254 fplab-0.0.2.3/fplab/
--rw-rw-rw-   0        0        0        0 2024-03-02 09:02:14.000000 fplab-0.0.2.3/fplab/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-14 15:01:36.198217 fplab-0.0.2.3/fplab/enhancement/
--rw-rw-rw-   0        0        0        0 2024-03-31 08:36:57.000000 fplab-0.0.2.3/fplab/enhancement/__init__.py
--rw-rw-rw-   0        0        0     4472 2024-03-31 08:36:57.000000 fplab-0.0.2.3/fplab/enhancement/frequency.py
--rw-rw-rw-   0        0        0     4454 2024-03-31 13:48:46.000000 fplab-0.0.2.3/fplab/enhancement/spatial.py
-drwxrwxrwx   0        0        0        0 2024-04-14 15:01:36.198720 fplab-0.0.2.3/fplab/generation/
--rw-rw-rw-   0        0        0        0 2024-04-02 15:51:38.000000 fplab-0.0.2.3/fplab/generation/__init__.py
--rw-rw-rw-   0        0        0     6948 2024-04-06 06:07:55.000000 fplab-0.0.2.3/fplab/generation/tps.py
-drwxrwxrwx   0        0        0        0 2024-04-14 15:01:36.198720 fplab-0.0.2.3/fplab/intrinsic/
--rw-rw-rw-   0        0        0        0 2024-03-23 06:49:44.000000 fplab-0.0.2.3/fplab/intrinsic/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-14 15:01:36.217119 fplab-0.0.2.3/fplab/intrinsic/frequency/
--rw-rw-rw-   0        0        0        0 2024-03-02 09:02:14.000000 fplab-0.0.2.3/fplab/intrinsic/frequency/__init__.py
--rw-rw-rw-   0        0        0     7577 2024-03-31 08:36:57.000000 fplab-0.0.2.3/fplab/intrinsic/frequency/projection.py
--rw-rw-rw-   0        0        0    10795 2024-03-31 08:36:57.000000 fplab-0.0.2.3/fplab/intrinsic/frequency/tools.py
--rw-rw-rw-   0        0        0     3116 2024-04-07 04:59:12.000000 fplab-0.0.2.3/fplab/intrinsic/frequency/transform.py
-drwxrwxrwx   0        0        0        0 2024-04-14 15:01:36.217119 fplab-0.0.2.3/fplab/intrinsic/mask/
--rw-rw-rw-   0        0        0        0 2024-03-02 09:02:14.000000 fplab-0.0.2.3/fplab/intrinsic/mask/__init__.py
--rw-rw-rw-   0        0        0      855 2024-04-06 15:25:34.000000 fplab-0.0.2.3/fplab/intrinsic/mask/mask.py
-drwxrwxrwx   0        0        0        0 2024-04-14 15:01:36.231854 fplab-0.0.2.3/fplab/intrinsic/multiple/
--rw-rw-rw-   0        0        0        0 2024-03-23 07:06:33.000000 fplab-0.0.2.3/fplab/intrinsic/multiple/__init__.py
--rw-rw-rw-   0        0        0     6990 2024-04-07 05:24:47.000000 fplab-0.0.2.3/fplab/intrinsic/multiple/transform.py
-drwxrwxrwx   0        0        0        0 2024-04-14 15:01:36.233058 fplab-0.0.2.3/fplab/intrinsic/orientation/
--rw-rw-rw-   0        0        0        0 2024-03-02 09:02:14.000000 fplab-0.0.2.3/fplab/intrinsic/orientation/__init__.py
--rw-rw-rw-   0        0        0     6640 2024-04-06 09:18:53.000000 fplab-0.0.2.3/fplab/intrinsic/orientation/gradient.py
--rw-rw-rw-   0        0        0     6215 2024-04-07 04:39:10.000000 fplab-0.0.2.3/fplab/intrinsic/orientation/tools.py
-drwxrwxrwx   0        0        0        0 2024-04-14 15:01:36.248014 fplab-0.0.2.3/fplab/intrinsic/skeleton/
--rw-rw-rw-   0        0        0        0 2024-04-06 15:22:02.000000 fplab-0.0.2.3/fplab/intrinsic/skeleton/__init__.py
--rw-rw-rw-   0        0        0     1752 2024-04-06 16:14:50.000000 fplab-0.0.2.3/fplab/intrinsic/skeleton/skeleton.py
-drwxrwxrwx   0        0        0        0 2024-04-14 15:01:36.250504 fplab-0.0.2.3/fplab/matching/
--rw-rw-rw-   0        0        0        0 2024-03-29 01:34:29.000000 fplab-0.0.2.3/fplab/matching/__init__.py
--rw-rw-rw-   0        0        0     6956 2024-03-30 03:40:09.000000 fplab-0.0.2.3/fplab/matching/tools.py
-drwxrwxrwx   0        0        0        0 2024-04-14 15:01:36.250504 fplab-0.0.2.3/fplab/minutiae/
--rw-rw-rw-   0        0        0        0 2024-03-02 09:02:14.000000 fplab-0.0.2.3/fplab/minutiae/__init__.py
--rw-rw-rw-   0        0        0     6782 2024-04-14 14:52:02.000000 fplab-0.0.2.3/fplab/minutiae/tools.py
-drwxrwxrwx   0        0        0        0 2024-04-14 15:01:36.267968 fplab-0.0.2.3/fplab/tools/
--rw-rw-rw-   0        0        0        0 2024-03-02 09:02:14.000000 fplab-0.0.2.3/fplab/tools/__init__.py
--rw-rw-rw-   0        0        0    13732 2024-04-06 14:10:17.000000 fplab-0.0.2.3/fplab/tools/array.py
--rw-rw-rw-   0        0        0     5367 2024-04-06 14:01:28.000000 fplab-0.0.2.3/fplab/tools/image.py
--rw-rw-rw-   0        0        0    15076 2024-04-06 09:13:19.000000 fplab-0.0.2.3/fplab/tools/nbis.py
--rw-rw-rw-   0        0        0    15788 2024-04-06 14:10:17.000000 fplab-0.0.2.3/fplab/tools/tensor.py
-drwxrwxrwx   0        0        0        0 2024-04-14 15:01:36.181050 fplab-0.0.2.3/fplab.egg-info/
--rw-rw-rw-   0        0        0      523 2024-04-14 15:01:36.000000 fplab-0.0.2.3/fplab.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1025 2024-04-14 15:01:36.000000 fplab-0.0.2.3/fplab.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-14 15:01:36.000000 fplab-0.0.2.3/fplab.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-04-14 15:01:36.000000 fplab-0.0.2.3/fplab.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-14 15:01:36.278076 fplab-0.0.2.3/setup.cfg
--rw-rw-rw-   0        0        0      801 2024-04-07 13:12:45.000000 fplab-0.0.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-25 13:26:02.008452 fplab-0.0.2.4/
+-rw-rw-rw-   0        0        0     1090 2024-03-31 02:38:30.000000 fplab-0.0.2.4/LICENSE.txt
+-rw-rw-rw-   0        0        0      523 2024-04-25 13:26:02.008452 fplab-0.0.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0      862 2024-04-06 15:56:56.000000 fplab-0.0.2.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-25 13:26:01.909229 fplab-0.0.2.4/fplab/
+-rw-rw-rw-   0        0        0        0 2024-03-02 09:02:14.000000 fplab-0.0.2.4/fplab/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-25 13:26:01.925147 fplab-0.0.2.4/fplab/enhancement/
+-rw-rw-rw-   0        0        0        0 2024-03-31 08:36:57.000000 fplab-0.0.2.4/fplab/enhancement/__init__.py
+-rw-rw-rw-   0        0        0     4472 2024-03-31 08:36:57.000000 fplab-0.0.2.4/fplab/enhancement/frequency.py
+-rw-rw-rw-   0        0        0     4907 2024-04-25 13:22:26.000000 fplab-0.0.2.4/fplab/enhancement/spatial.py
+drwxrwxrwx   0        0        0        0 2024-04-25 13:26:01.932763 fplab-0.0.2.4/fplab/generation/
+-rw-rw-rw-   0        0        0        0 2024-04-02 15:51:38.000000 fplab-0.0.2.4/fplab/generation/__init__.py
+-rw-rw-rw-   0        0        0     6948 2024-04-06 06:07:55.000000 fplab-0.0.2.4/fplab/generation/tps.py
+drwxrwxrwx   0        0        0        0 2024-04-25 13:26:01.933766 fplab-0.0.2.4/fplab/intrinsic/
+-rw-rw-rw-   0        0        0        0 2024-03-23 06:49:44.000000 fplab-0.0.2.4/fplab/intrinsic/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-25 13:26:01.949600 fplab-0.0.2.4/fplab/intrinsic/frequency/
+-rw-rw-rw-   0        0        0        0 2024-03-02 09:02:14.000000 fplab-0.0.2.4/fplab/intrinsic/frequency/__init__.py
+-rw-rw-rw-   0        0        0     7577 2024-03-31 08:36:57.000000 fplab-0.0.2.4/fplab/intrinsic/frequency/projection.py
+-rw-rw-rw-   0        0        0    10795 2024-03-31 08:36:57.000000 fplab-0.0.2.4/fplab/intrinsic/frequency/tools.py
+-rw-rw-rw-   0        0        0     3116 2024-04-07 04:59:12.000000 fplab-0.0.2.4/fplab/intrinsic/frequency/transform.py
+drwxrwxrwx   0        0        0        0 2024-04-25 13:26:01.955455 fplab-0.0.2.4/fplab/intrinsic/mask/
+-rw-rw-rw-   0        0        0        0 2024-03-02 09:02:14.000000 fplab-0.0.2.4/fplab/intrinsic/mask/__init__.py
+-rw-rw-rw-   0        0        0      855 2024-04-06 15:25:34.000000 fplab-0.0.2.4/fplab/intrinsic/mask/mask.py
+drwxrwxrwx   0        0        0        0 2024-04-25 13:26:01.960742 fplab-0.0.2.4/fplab/intrinsic/multiple/
+-rw-rw-rw-   0        0        0        0 2024-03-23 07:06:33.000000 fplab-0.0.2.4/fplab/intrinsic/multiple/__init__.py
+-rw-rw-rw-   0        0        0     6990 2024-04-07 05:24:47.000000 fplab-0.0.2.4/fplab/intrinsic/multiple/transform.py
+drwxrwxrwx   0        0        0        0 2024-04-25 13:26:01.972586 fplab-0.0.2.4/fplab/intrinsic/orientation/
+-rw-rw-rw-   0        0        0        0 2024-03-02 09:02:14.000000 fplab-0.0.2.4/fplab/intrinsic/orientation/__init__.py
+-rw-rw-rw-   0        0        0     6640 2024-04-06 09:18:53.000000 fplab-0.0.2.4/fplab/intrinsic/orientation/gradient.py
+-rw-rw-rw-   0        0        0     6215 2024-04-07 04:39:10.000000 fplab-0.0.2.4/fplab/intrinsic/orientation/tools.py
+drwxrwxrwx   0        0        0        0 2024-04-25 13:26:01.978589 fplab-0.0.2.4/fplab/intrinsic/skeleton/
+-rw-rw-rw-   0        0        0        0 2024-04-06 15:22:02.000000 fplab-0.0.2.4/fplab/intrinsic/skeleton/__init__.py
+-rw-rw-rw-   0        0        0     1752 2024-04-06 16:14:50.000000 fplab-0.0.2.4/fplab/intrinsic/skeleton/skeleton.py
+drwxrwxrwx   0        0        0        0 2024-04-25 13:26:01.984213 fplab-0.0.2.4/fplab/matching/
+-rw-rw-rw-   0        0        0        0 2024-03-29 01:34:29.000000 fplab-0.0.2.4/fplab/matching/__init__.py
+-rw-rw-rw-   0        0        0     6956 2024-03-30 03:40:09.000000 fplab-0.0.2.4/fplab/matching/tools.py
+drwxrwxrwx   0        0        0        0 2024-04-25 13:26:01.986680 fplab-0.0.2.4/fplab/minutiae/
+-rw-rw-rw-   0        0        0        0 2024-03-02 09:02:14.000000 fplab-0.0.2.4/fplab/minutiae/__init__.py
+-rw-rw-rw-   0        0        0     6782 2024-04-14 14:52:02.000000 fplab-0.0.2.4/fplab/minutiae/tools.py
+drwxrwxrwx   0        0        0        0 2024-04-25 13:26:02.006341 fplab-0.0.2.4/fplab/tools/
+-rw-rw-rw-   0        0        0        0 2024-03-02 09:02:14.000000 fplab-0.0.2.4/fplab/tools/__init__.py
+-rw-rw-rw-   0        0        0    13732 2024-04-06 14:10:17.000000 fplab-0.0.2.4/fplab/tools/array.py
+-rw-rw-rw-   0        0        0     5367 2024-04-06 14:01:28.000000 fplab-0.0.2.4/fplab/tools/image.py
+-rw-rw-rw-   0        0        0    15076 2024-04-06 09:13:19.000000 fplab-0.0.2.4/fplab/tools/nbis.py
+-rw-rw-rw-   0        0        0    15788 2024-04-06 14:10:17.000000 fplab-0.0.2.4/fplab/tools/tensor.py
+drwxrwxrwx   0        0        0        0 2024-04-25 13:26:01.917947 fplab-0.0.2.4/fplab.egg-info/
+-rw-rw-rw-   0        0        0      523 2024-04-25 13:26:01.000000 fplab-0.0.2.4/fplab.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1025 2024-04-25 13:26:01.000000 fplab-0.0.2.4/fplab.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 13:26:01.000000 fplab-0.0.2.4/fplab.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-04-25 13:26:01.000000 fplab-0.0.2.4/fplab.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-25 13:26:02.008452 fplab-0.0.2.4/setup.cfg
+-rw-rw-rw-   0        0        0      801 2024-04-25 13:24:06.000000 fplab-0.0.2.4/setup.py
```

### Comparing `fplab-0.0.2.3/LICENSE.txt` & `fplab-0.0.2.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fplab-0.0.2.3/PKG-INFO` & `fplab-0.0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fplab
-Version: 0.0.2.3
+Version: 0.0.2.4
 Summary: Python3 Package for Fingerprint Processing
 Author: Yurun Wang
 Author-email: wangyurun@mail.sdu.edu.cn
 License: MIT
 Keywords: python,fingerprint
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fplab-0.0.2.3/README.md` & `fplab-0.0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `fplab-0.0.2.3/fplab/enhancement/frequency.py` & `fplab-0.0.2.4/fplab/enhancement/frequency.py`

 * *Files identical despite different names*

### Comparing `fplab-0.0.2.3/fplab/enhancement/spatial.py` & `fplab-0.0.2.4/fplab/enhancement/spatial.py`

 * *Files 8% similar despite different names*

```diff
@@ -79,53 +79,67 @@
     """1998年Hong提出的指纹指纹增强算法，复现了除分割外的处理过程"""
     o = ort_gradient.hong1998(im)
     f = frq_projection.hong1998(im, o, flag=("return",))
     out = gabor_filter(im, o, f)
     return out, o, f
 
 
-def get_diffusion_function(oa, c1, c2, s):
+def get_diffusion_function(oa, c1, c2, s, mk=None):
     """定义用于scipy.ndimage.generic_filter的自定义滤波函数，
     用于实现参数随像素位置变化的方向扩散滤波
-    oa是方向场，c1和c2是正交方向的权重，s是迭代步长"""
+    oa是方向场，c1和c2是正交方向的权重，s是迭代步长
+    mk为0处不做滤波，默认为全一数组"""
     # 扩散需要多次迭代，每次迭代同一位置使用的核是相同的
     # 预先计算这些核以减少运算量
+    if mk is None:
+        mka = np.ones_like(oa)
+    else:
+        mka = mk
     ft = np.ones((3, 3))
     k = []
     for i in range(oa.size):
         coordinates = np.unravel_index(i, oa.shape)
-        o = oa[coordinates]
-        cos, sin = np.cos(o), np.sin(o)
-        a = (c1-c2)*cos*cos+c2
-        b = (c1-c2)*cos*sin
-        c = (c1-c2)*sin*sin+c2
-        k.append(np.array([b, 2*a, -b, 2*c, -4*(c1+c2), 2*c, -b, 2*a, b])*s/2)
+        if mka[coordinates] == 0:
+            k.append(np.array([0., 0., 0., 0., 1., 0., 0., 0., 0.]))
+        else:
+            o = oa[coordinates]
+            cos, sin = np.cos(o), np.sin(o)
+            a = (c1-c2)*cos*cos+c2
+            b = (c1-c2)*cos*sin
+            c = (c1-c2)*sin*sin+c2
+            k.append(np.array([b, 2*a, -b, 2*c, -4*(c1+c2), 2*c, -b, 2*a, b])*s/2)
 
     class FilterFunction:
         def __init__(self):
             self.n = 0
 
         def __call__(self, in_elements):
             out = in_elements[4]+(k[self.n]*in_elements).sum()
             self.n = (self.n + 1) % oa.size
             return out
 
     return ft, FilterFunction()
 
 
-def diffusion_filter(im, ot, c1, c2, s, itn):
+def diffusion_filter(im, ot, c1, c2, s, itn, mk=None):
     """根据计算的方向场ot，对指纹图像im进行方向扩散增强
     c1和c2是正交方向的权重，s是迭代步长，itn是迭代次数
+    mk为0处不做滤波，默认为全一数组
     """
     # ima是原始图像
     ima = type_as(im, md="a")
     ima = ima_rgb2l(ima)
     ima = ima_minmax(ima)
     # ota存放着每一点的方向
     ota = type_as(ot, md="a")
-    ft, filter_func = get_diffusion_function(ota, c1, c2, s)
+    # 处理mask
+    if mk is None:
+        mka = np.ones_like(ota)
+    else:
+        mka = mk
+    ft, filter_func = get_diffusion_function(ota, c1, c2, s, mk=mka)
     for i in range(itn):
         ima = ndimage.generic_filter(ima, filter_func, footprint=ft)
     ima = type_as(ima, im)
     del ota, ft, filter_func
     gc.collect()
     return ima
```

### Comparing `fplab-0.0.2.3/fplab/generation/tps.py` & `fplab-0.0.2.4/fplab/generation/tps.py`

 * *Files identical despite different names*

### Comparing `fplab-0.0.2.3/fplab/intrinsic/frequency/projection.py` & `fplab-0.0.2.4/fplab/intrinsic/frequency/projection.py`

 * *Files identical despite different names*

### Comparing `fplab-0.0.2.3/fplab/intrinsic/frequency/tools.py` & `fplab-0.0.2.4/fplab/intrinsic/frequency/tools.py`

 * *Files identical despite different names*

### Comparing `fplab-0.0.2.3/fplab/intrinsic/frequency/transform.py` & `fplab-0.0.2.4/fplab/intrinsic/frequency/transform.py`

 * *Files identical despite different names*

### Comparing `fplab-0.0.2.3/fplab/intrinsic/mask/mask.py` & `fplab-0.0.2.4/fplab/intrinsic/mask/mask.py`

 * *Files identical despite different names*

### Comparing `fplab-0.0.2.3/fplab/intrinsic/multiple/transform.py` & `fplab-0.0.2.4/fplab/intrinsic/multiple/transform.py`

 * *Files identical despite different names*

### Comparing `fplab-0.0.2.3/fplab/intrinsic/orientation/gradient.py` & `fplab-0.0.2.4/fplab/intrinsic/orientation/gradient.py`

 * *Files identical despite different names*

### Comparing `fplab-0.0.2.3/fplab/intrinsic/orientation/tools.py` & `fplab-0.0.2.4/fplab/intrinsic/orientation/tools.py`

 * *Files identical despite different names*

### Comparing `fplab-0.0.2.3/fplab/intrinsic/skeleton/skeleton.py` & `fplab-0.0.2.4/fplab/intrinsic/skeleton/skeleton.py`

 * *Files identical despite different names*

### Comparing `fplab-0.0.2.3/fplab/matching/tools.py` & `fplab-0.0.2.4/fplab/matching/tools.py`

 * *Files identical despite different names*

### Comparing `fplab-0.0.2.3/fplab/minutiae/tools.py` & `fplab-0.0.2.4/fplab/minutiae/tools.py`

 * *Files identical despite different names*

### Comparing `fplab-0.0.2.3/fplab/tools/array.py` & `fplab-0.0.2.4/fplab/tools/array.py`

 * *Files identical despite different names*

### Comparing `fplab-0.0.2.3/fplab/tools/image.py` & `fplab-0.0.2.4/fplab/tools/image.py`

 * *Files identical despite different names*

### Comparing `fplab-0.0.2.3/fplab/tools/nbis.py` & `fplab-0.0.2.4/fplab/tools/nbis.py`

 * *Files identical despite different names*

### Comparing `fplab-0.0.2.3/fplab/tools/tensor.py` & `fplab-0.0.2.4/fplab/tools/tensor.py`

 * *Files identical despite different names*

### Comparing `fplab-0.0.2.3/fplab.egg-info/PKG-INFO` & `fplab-0.0.2.4/fplab.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fplab
-Version: 0.0.2.3
+Version: 0.0.2.4
 Summary: Python3 Package for Fingerprint Processing
 Author: Yurun Wang
 Author-email: wangyurun@mail.sdu.edu.cn
 License: MIT
 Keywords: python,fingerprint
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fplab-0.0.2.3/fplab.egg-info/SOURCES.txt` & `fplab-0.0.2.4/fplab.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fplab-0.0.2.3/setup.py` & `fplab-0.0.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.2.3'
+VERSION = '0.0.2.4'
 DESCRIPTION = 'Python3 Package for Fingerprint Processing'
 LONG_DESCRIPTION = ('This is a python3 package for fingerprint processing,'
                     ' which can be used for fingerprint enhancement.')
 
 setup(
     name="fplab",
     version=VERSION,
```


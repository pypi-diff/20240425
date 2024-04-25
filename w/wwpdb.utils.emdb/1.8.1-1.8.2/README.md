# Comparing `tmp/wwpdb_utils_emdb-1.8.1.tar.gz` & `tmp/wwpdb_utils_emdb-1.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wwpdb_utils_emdb-1.8.1.tar", last modified: Wed Apr 24 16:17:20 2024, max compression
+gzip compressed data, was "wwpdb_utils_emdb-1.8.2.tar", last modified: Thu Apr 25 19:45:39 2024, max compression
```

## Comparing `wwpdb_utils_emdb-1.8.1.tar` & `wwpdb_utils_emdb-1.8.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-24 16:17:20.121608 wwpdb_utils_emdb-1.8.1/
--rw-r--r--   0 vsts      (1001) docker     (127)      106 2024-04-24 16:16:22.000000 wwpdb_utils_emdb-1.8.1/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (127)      960 2024-04-24 16:17:20.121608 wwpdb_utils_emdb-1.8.1/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)       46 2024-04-24 16:16:22.000000 wwpdb_utils_emdb-1.8.1/README.md
--rw-r--r--   0 vsts      (1001) docker     (127)      108 2024-04-24 16:17:20.121608 wwpdb_utils_emdb-1.8.1/setup.cfg
--rwxr-xr-x   0 vsts      (1001) docker     (127)     2310 2024-04-24 16:16:22.000000 wwpdb_utils_emdb-1.8.1/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-24 16:17:20.113608 wwpdb_utils_emdb-1.8.1/wwpdb/
--rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-04-24 16:16:22.000000 wwpdb_utils_emdb-1.8.1/wwpdb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-24 16:17:20.117608 wwpdb_utils_emdb-1.8.1/wwpdb/utils/
--rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-04-24 16:16:22.000000 wwpdb_utils_emdb-1.8.1/wwpdb/utils/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-24 16:17:20.117608 wwpdb_utils_emdb-1.8.1/wwpdb/utils/emdb/
--rw-r--r--   0 vsts      (1001) docker     (127)      322 2024-04-24 16:16:22.000000 wwpdb_utils_emdb-1.8.1/wwpdb/utils/emdb/EmdbSchema.py
--rw-r--r--   0 vsts      (1001) docker     (127)      145 2024-04-24 16:16:22.000000 wwpdb_utils_emdb-1.8.1/wwpdb/utils/emdb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-24 16:17:20.117608 wwpdb_utils_emdb-1.8.1/wwpdb/utils/emdb/atomcheck/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-24 16:16:22.000000 wwpdb_utils_emdb-1.8.1/wwpdb/utils/emdb/atomcheck/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7031 2024-04-24 16:16:22.000000 wwpdb_utils_emdb-1.8.1/wwpdb/utils/emdb/atomcheck/atomcheck.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-24 16:17:20.117608 wwpdb_utils_emdb-1.8.1/wwpdb/utils/emdb/checkemupload/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-24 16:16:22.000000 wwpdb_utils_emdb-1.8.1/wwpdb/utils/emdb/checkemupload/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    16398 2024-04-24 16:16:22.000000 wwpdb_utils_emdb-1.8.1/wwpdb/utils/emdb/checkemupload/checkemupload.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-24 16:17:20.121608 wwpdb_utils_emdb-1.8.1/wwpdb/utils/emdb/cif_emdb_translator/
--rwxr-xr-x   0 vsts      (1001) docker     (127)      139 2024-04-24 16:16:22.000000 wwpdb_utils_emdb-1.8.1/wwpdb/utils/emdb/cif_emdb_translator/README.md
--rwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-24 16:16:22.000000 wwpdb_utils_emdb-1.8.1/wwpdb/utils/emdb/cif_emdb_translator/__init__.py
--rwxr-xr-x   0 vsts      (1001) docker     (127)   676892 2024-04-24 16:16:22.000000 wwpdb_utils_emdb-1.8.1/wwpdb/utils/emdb/cif_emdb_translator/cif_emdb_translator.py
--rw-r--r--   0 vsts      (1001) docker     (127)  2304974 2024-04-24 16:16:22.000000 wwpdb_utils_emdb-1.8.1/wwpdb/utils/emdb/cif_emdb_translator/emdb.py
--rwxr-xr-x   0 vsts      (1001) docker     (127)     1196 2024-04-24 16:16:22.000000 wwpdb_utils_emdb-1.8.1/wwpdb/utils/emdb/cif_emdb_translator/simple_test.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2490 2024-04-24 16:16:22.000000 wwpdb_utils_emdb-1.8.1/wwpdb/utils/emdb/cif_emdb_translator/test_cif_to_xml_translator.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-24 16:17:20.121608 wwpdb_utils_emdb-1.8.1/wwpdb/utils/emdb/data/
--rw-r--r--   0 vsts      (1001) docker     (127)   221515 2024-04-24 16:16:22.000000 wwpdb_utils_emdb-1.8.1/wwpdb/utils/emdb/data/emdb-v3.xsd
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-24 16:17:20.121608 wwpdb_utils_emdb-1.8.1/wwpdb.utils.emdb.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)      960 2024-04-24 16:17:20.000000 wwpdb_utils_emdb-1.8.1/wwpdb.utils.emdb.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)      947 2024-04-24 16:17:20.000000 wwpdb_utils_emdb-1.8.1/wwpdb.utils.emdb.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-24 16:17:20.000000 wwpdb_utils_emdb-1.8.1/wwpdb.utils.emdb.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       87 2024-04-24 16:17:20.000000 wwpdb_utils_emdb-1.8.1/wwpdb.utils.emdb.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-24 16:17:05.000000 wwpdb_utils_emdb-1.8.1/wwpdb.utils.emdb.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (127)      101 2024-04-24 16:17:20.000000 wwpdb_utils_emdb-1.8.1/wwpdb.utils.emdb.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        6 2024-04-24 16:17:20.000000 wwpdb_utils_emdb-1.8.1/wwpdb.utils.emdb.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-25 19:45:39.864299 wwpdb_utils_emdb-1.8.2/
+-rw-r--r--   0 vsts      (1001) docker     (127)      106 2024-04-25 19:44:36.000000 wwpdb_utils_emdb-1.8.2/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (127)      960 2024-04-25 19:45:39.864299 wwpdb_utils_emdb-1.8.2/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)       46 2024-04-25 19:44:36.000000 wwpdb_utils_emdb-1.8.2/README.md
+-rw-r--r--   0 vsts      (1001) docker     (127)      108 2024-04-25 19:45:39.868299 wwpdb_utils_emdb-1.8.2/setup.cfg
+-rwxr-xr-x   0 vsts      (1001) docker     (127)     2310 2024-04-25 19:44:36.000000 wwpdb_utils_emdb-1.8.2/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-25 19:45:39.860299 wwpdb_utils_emdb-1.8.2/wwpdb/
+-rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-04-25 19:44:36.000000 wwpdb_utils_emdb-1.8.2/wwpdb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-25 19:45:39.860299 wwpdb_utils_emdb-1.8.2/wwpdb/utils/
+-rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-04-25 19:44:36.000000 wwpdb_utils_emdb-1.8.2/wwpdb/utils/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-25 19:45:39.860299 wwpdb_utils_emdb-1.8.2/wwpdb/utils/emdb/
+-rw-r--r--   0 vsts      (1001) docker     (127)      322 2024-04-25 19:44:36.000000 wwpdb_utils_emdb-1.8.2/wwpdb/utils/emdb/EmdbSchema.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      145 2024-04-25 19:44:36.000000 wwpdb_utils_emdb-1.8.2/wwpdb/utils/emdb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-25 19:45:39.860299 wwpdb_utils_emdb-1.8.2/wwpdb/utils/emdb/atomcheck/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-25 19:44:36.000000 wwpdb_utils_emdb-1.8.2/wwpdb/utils/emdb/atomcheck/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7031 2024-04-25 19:44:36.000000 wwpdb_utils_emdb-1.8.2/wwpdb/utils/emdb/atomcheck/atomcheck.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-25 19:45:39.860299 wwpdb_utils_emdb-1.8.2/wwpdb/utils/emdb/checkemupload/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-25 19:44:36.000000 wwpdb_utils_emdb-1.8.2/wwpdb/utils/emdb/checkemupload/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19243 2024-04-25 19:44:36.000000 wwpdb_utils_emdb-1.8.2/wwpdb/utils/emdb/checkemupload/checkemupload.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-25 19:45:39.864299 wwpdb_utils_emdb-1.8.2/wwpdb/utils/emdb/cif_emdb_translator/
+-rwxr-xr-x   0 vsts      (1001) docker     (127)      139 2024-04-25 19:44:36.000000 wwpdb_utils_emdb-1.8.2/wwpdb/utils/emdb/cif_emdb_translator/README.md
+-rwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-25 19:44:36.000000 wwpdb_utils_emdb-1.8.2/wwpdb/utils/emdb/cif_emdb_translator/__init__.py
+-rwxr-xr-x   0 vsts      (1001) docker     (127)   676892 2024-04-25 19:44:36.000000 wwpdb_utils_emdb-1.8.2/wwpdb/utils/emdb/cif_emdb_translator/cif_emdb_translator.py
+-rw-r--r--   0 vsts      (1001) docker     (127)  2304974 2024-04-25 19:44:36.000000 wwpdb_utils_emdb-1.8.2/wwpdb/utils/emdb/cif_emdb_translator/emdb.py
+-rwxr-xr-x   0 vsts      (1001) docker     (127)     1196 2024-04-25 19:44:36.000000 wwpdb_utils_emdb-1.8.2/wwpdb/utils/emdb/cif_emdb_translator/simple_test.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2490 2024-04-25 19:44:36.000000 wwpdb_utils_emdb-1.8.2/wwpdb/utils/emdb/cif_emdb_translator/test_cif_to_xml_translator.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-25 19:45:39.864299 wwpdb_utils_emdb-1.8.2/wwpdb/utils/emdb/data/
+-rw-r--r--   0 vsts      (1001) docker     (127)   221515 2024-04-25 19:44:36.000000 wwpdb_utils_emdb-1.8.2/wwpdb/utils/emdb/data/emdb-v3.xsd
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-25 19:45:39.864299 wwpdb_utils_emdb-1.8.2/wwpdb.utils.emdb.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)      960 2024-04-25 19:45:39.000000 wwpdb_utils_emdb-1.8.2/wwpdb.utils.emdb.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)      947 2024-04-25 19:45:39.000000 wwpdb_utils_emdb-1.8.2/wwpdb.utils.emdb.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-25 19:45:39.000000 wwpdb_utils_emdb-1.8.2/wwpdb.utils.emdb.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       87 2024-04-25 19:45:39.000000 wwpdb_utils_emdb-1.8.2/wwpdb.utils.emdb.egg-info/entry_points.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-25 19:45:26.000000 wwpdb_utils_emdb-1.8.2/wwpdb.utils.emdb.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (127)      101 2024-04-25 19:45:39.000000 wwpdb_utils_emdb-1.8.2/wwpdb.utils.emdb.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        6 2024-04-25 19:45:39.000000 wwpdb_utils_emdb-1.8.2/wwpdb.utils.emdb.egg-info/top_level.txt
```

### Comparing `wwpdb_utils_emdb-1.8.1/PKG-INFO` & `wwpdb_utils_emdb-1.8.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwpdb.utils.emdb
-Version: 1.8.1
+Version: 1.8.2
 Summary: wwPDB EMDB to XML converter
 Home-page: https://github.com/rcsb/py-wwpdb_utils_config
 Author: Ezra Peisach
 Author-email: ezra.peisach@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `wwpdb_utils_emdb-1.8.1/setup.py` & `wwpdb_utils_emdb-1.8.2/setup.py`

 * *Files identical despite different names*

### Comparing `wwpdb_utils_emdb-1.8.1/wwpdb/utils/emdb/atomcheck/atomcheck.py` & `wwpdb_utils_emdb-1.8.2/wwpdb/utils/emdb/atomcheck/atomcheck.py`

 * *Files identical despite different names*

### Comparing `wwpdb_utils_emdb-1.8.1/wwpdb/utils/emdb/checkemupload/checkemupload.py` & `wwpdb_utils_emdb-1.8.2/wwpdb/utils/emdb/checkemupload/checkemupload.py`

 * *Files 6% similar despite different names*

```diff
@@ -72,15 +72,16 @@
                         self.nstarts[crsindices[0]],
                         self.nstarts[crsindices[1]],
                         self.nstarts[crsindices[2]]
                     )).tolist()
         except FileNotFoundError:
             raise FileNotFoundError(f"File not found: {self.file}")  # pylint: disable=raise-missing-from
         except Exception as e:
-            raise Exception(f"An error occurred while loading the file: {str(e)}")  # pylint: disable=broad-exception-raised,raise-missing-from
+            raise Exception(
+                f"An error occurred while loading the file: {str(e)}")  # pylint: disable=broad-exception-raised,raise-missing-from
 
     def md5_checksum(self):
         """
         Calculate the MD5 checksum of the map file.
         """
         hash_md5 = hashlib.md5()
         with open(self.file, "rb") as f:
@@ -225,38 +226,95 @@
             model (Model, optional): Structural model. Defaults to None.
         """
         self.em_map = em_map
         self.half_maps = half_maps
         self.model = model
 
     def _map_matrix(self, apixs, angs):
-        # Convert angles to radians
-        angs = [math.radians(ang) for ang in angs]
-        cos_alpha, cos_beta, cos_gamma = [math.cos(ang) for ang in angs]
-        sin_alpha, sin_beta, sin_gamma = [math.sin(ang) for ang in angs]
-        matrix = np.array([
-            [apixs[0], apixs[1] * cos_gamma, apixs[2] * cos_beta],
-            [0, apixs[1] * sin_gamma, -apixs[2] * sin_beta * cos_alpha],
-            [0, 0, apixs[2] * sin_beta * sin_alpha]
-        ])
+        """
+        calculate the matrix to transform Cartesian coordinates to fractional coordinates
+        (check the definination to see the matrix formular)
+        :param apixs: array of apix lenght
+        :param angs: array of anglex in alpha, beta, gamma order
+        :return: array of matrix
+        """
+
+        ang = (angs[0] * math.pi / 180, angs[1] * math.pi / 180, angs[2] * math.pi / 180)
+        insidesqrt = (1 + 2 * math.cos(ang[0]) * math.cos(ang[1]) * math.cos(ang[2]) - math.cos(ang[0]) ** 2 - math.cos(ang[1]) ** 2 - math.cos(ang[2]) ** 2)
+        cellvolume = apixs[0] * apixs[1] * apixs[2] * math.sqrt(insidesqrt)
+
+        m11 = 1 / apixs[0]
+        m12 = -math.cos(ang[2]) / (apixs[0] * math.sin(ang[2]))
+
+        m13 = apixs[1] * apixs[2] * (math.cos(ang[0]) * math.cos(ang[2]) - math.cos(ang[1])) / (cellvolume * math.sin(ang[2]))
+        m21 = 0
+        m22 = 1 / (apixs[1] * math.sin(ang[2]))
+        m23 = apixs[0] * apixs[2] * (math.cos(ang[1]) * math.cos(ang[2]) - math.cos(ang[0])) / (cellvolume * math.sin(ang[2]))
+        m31 = 0
+        m32 = 0
+        m33 = apixs[0] * apixs[1] * math.sin(ang[2]) / cellvolume
+        prematrix = [[m11, m12, m13], [m21, m22, m23], [m31, m32, m33]]
+        matrix = np.asarray(prematrix)
+
         return matrix
 
     def _matrix_indices(self, apixs, onecoor):
         angs = [self.em_map.header.cellb.alpha, self.em_map.header.cellb.beta, self.em_map.header.cellb.gamma]
         matrix = self._map_matrix(apixs, angs)
         result = matrix.dot(np.asarray(onecoor))
         return result[0] - self.em_map.nstarts[0], result[1] - self.em_map.nstarts[1], result[2] - self.em_map.nstarts[
             2]
 
+    def header_check(self):
+        crs = (self.em_map.header.mapc, self.em_map.header.mapr, self.em_map.header.maps)
+        crsindices = (crs.index(1), crs.index(2), crs.index(3))
+        self.nstarts = (self.em_map.header.nxstart, self.em_map.header.nystart, self.em_map.header.nzstart)
+        self.nxyz = (self.em_map.header.nx, self.em_map.header.ny, self.em_map.header.nz)
+
+        if crs != (1, 2, 3):
+            self.nxyz = (self.nxyz[crsindices[0]], self.nxyz[crsindices[1]], self.nxyz[crsindices[2]])
+            self.nstarts = (self.nstarts[crsindices[0]], self.nstarts[crsindices[1]], self.nstarts[crsindices[2]])
+
     def _get_indices(self, onecoor):
-        apixs = [self.em_map.header.cella.x / self.em_map.nxyz[0],
-                 self.em_map.header.cella.y / self.em_map.nxyz[1],
-                 self.em_map.header.cella.z / self.em_map.nxyz[2]]
-        oneindex = self._matrix_indices(apixs, onecoor)
-        return oneindex, self.em_map.nxyz
+        """
+                Find one atom's indices correspoding to its cubic or plane
+                the 8 (cubic) or 4 (plane) indices are saved in indices variable
+            :param onecoor: List contains the atom coordinates in (x, y, z) order
+            :return: Tuple contains two list of index: first has the 8 or 4 indices in the cubic;second has the float index of the input atom
+            """
+
+        zdim = self.em_map.header.cella.z
+        znintervals = self.em_map.header.mz
+        z_apix = zdim / znintervals
+
+        ydim = self.em_map.header.cella.y
+        ynintervals = self.em_map.header.my
+        y_apix = ydim / ynintervals
+
+        xdim = self.em_map.header.cella.x
+        xnintervals = self.em_map.header.mx
+        x_apix = xdim / xnintervals
+
+        self.header_check()
+        # map_xsize, map_ysize, map_zsize = self.nxyz
+        nxstart, nystart, nzstart = self.nstarts
+
+        if self.em_map.header.cellb.alpha == self.em_map.header.cellb.beta == self.em_map.header.cellb.gamma == 90.:
+            # crs = [self.em_map.header.mapc, self.em_map.header.mapr, self.em_map.header.maps]
+            # ordinds = [crs.index(1), crs.index(2), crs.index(3)]
+            zindex = float(onecoor[2] - self.em_map.header.origin.z) / z_apix - nzstart
+            yindex = float(onecoor[1] - self.em_map.header.origin.y) / y_apix - nystart
+            xindex = float(onecoor[0] - self.em_map.header.origin.x) / x_apix - nxstart
+        else:
+            apixs = [x_apix, y_apix, z_apix]
+            xindex, yindex, zindex = self._matrix_indices(apixs, onecoor)
+
+        oneindex = [xindex, yindex, zindex]
+
+        return oneindex, self.nxyz
 
     def _compare_maps(self, map1, map2):
         result = {
             'em_volumes': [
                 {
                     'name': os.path.basename(map1.file),
                     'checksum': map1.hash
@@ -313,15 +371,15 @@
         return result
 
     def _get_atoms_outside(self):
         num_atoms_outside = 0  # Initialize counter for atoms outside the primary map
         for atom in self.model.structure:
             atom_index, nxyz = self._get_indices(atom)
             # Check if the atom is outside the primary map boundaries
-            if any(coord < 0 or coord >= nxyz[i] for i, coord in enumerate(atom_index)):
+            if any(coord < 0 or coord > nxyz[i] - 1 for i, coord in enumerate(atom_index)):
                 num_atoms_outside += 1
         # Calculate the fraction of atoms outside the primary map
         fraction_atoms_outside = num_atoms_outside / len(self.model.structure)
         return num_atoms_outside, fraction_atoms_outside
 
     def check(self):
         """
@@ -341,16 +399,18 @@
 
         if self.half_maps:
             if len(self.half_maps) != 2:
                 raise Exception("Two half maps must be provided.")  # pylint: disable=broad-exception-raised
             if not all(os.path.isfile(half_map.file) for half_map in self.half_maps):
                 raise FileNotFoundError("One or more half maps not found.")
             result.update({
-                'half_maps_to_each_other': self._compare_maps(self.half_maps[0], self.half_maps[1]),  # Compare half maps to each other
-                'primary_map_to_half_maps': [self._compare_maps(self.em_map, half_map) for half_map in self.half_maps]  # Compare primary map to each half map
+                'half_maps_to_each_other': self._compare_maps(self.half_maps[0], self.half_maps[1]),
+                # Compare half maps to each other
+                'primary_map_to_half_maps': [self._compare_maps(self.em_map, half_map) for half_map in self.half_maps]
+                # Compare primary map to each half map
             })
 
         if self.model and self.model.structure:
             num_atoms_outside, fraction_atoms_outside = self._get_atoms_outside()
             result['map_to_model'] = {
                 'num_atoms_outside': num_atoms_outside,
                 # Calculate the fraction of atoms outside the primary map
```

### Comparing `wwpdb_utils_emdb-1.8.1/wwpdb/utils/emdb/cif_emdb_translator/cif_emdb_translator.py` & `wwpdb_utils_emdb-1.8.2/wwpdb/utils/emdb/cif_emdb_translator/cif_emdb_translator.py`

 * *Files identical despite different names*

### Comparing `wwpdb_utils_emdb-1.8.1/wwpdb/utils/emdb/cif_emdb_translator/emdb.py` & `wwpdb_utils_emdb-1.8.2/wwpdb/utils/emdb/cif_emdb_translator/emdb.py`

 * *Files identical despite different names*

### Comparing `wwpdb_utils_emdb-1.8.1/wwpdb/utils/emdb/cif_emdb_translator/simple_test.py` & `wwpdb_utils_emdb-1.8.2/wwpdb/utils/emdb/cif_emdb_translator/simple_test.py`

 * *Files identical despite different names*

### Comparing `wwpdb_utils_emdb-1.8.1/wwpdb/utils/emdb/cif_emdb_translator/test_cif_to_xml_translator.py` & `wwpdb_utils_emdb-1.8.2/wwpdb/utils/emdb/cif_emdb_translator/test_cif_to_xml_translator.py`

 * *Files identical despite different names*

### Comparing `wwpdb_utils_emdb-1.8.1/wwpdb/utils/emdb/data/emdb-v3.xsd` & `wwpdb_utils_emdb-1.8.2/wwpdb/utils/emdb/data/emdb-v3.xsd`

 * *Files identical despite different names*

### Comparing `wwpdb_utils_emdb-1.8.1/wwpdb.utils.emdb.egg-info/PKG-INFO` & `wwpdb_utils_emdb-1.8.2/wwpdb.utils.emdb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwpdb.utils.emdb
-Version: 1.8.1
+Version: 1.8.2
 Summary: wwPDB EMDB to XML converter
 Home-page: https://github.com/rcsb/py-wwpdb_utils_config
 Author: Ezra Peisach
 Author-email: ezra.peisach@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `wwpdb_utils_emdb-1.8.1/wwpdb.utils.emdb.egg-info/SOURCES.txt` & `wwpdb_utils_emdb-1.8.2/wwpdb.utils.emdb.egg-info/SOURCES.txt`

 * *Files identical despite different names*


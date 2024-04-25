# Comparing `tmp/pytRIBS-0.1.1.tar.gz` & `tmp/pytribs-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytRIBS-0.1.1.tar", last modified: Tue Feb 20 22:06:30 2024, max compression
+gzip compressed data, was "pytribs-0.2.0.tar", last modified: Thu Apr 25 20:54:56 2024, max compression
```

## Comparing `pytRIBS-0.1.1.tar` & `pytribs-0.2.0.tar`

### file list

```diff
@@ -1,30 +1,36 @@
-drwxr-xr-x   0 lraming    (503) staff       (20)        0 2024-02-20 22:06:30.486330 pytRIBS-0.1.1/
--rw-r--r--   0 lraming    (503) staff       (20)    18005 2024-02-20 18:31:47.000000 pytRIBS-0.1.1/LICENSE
--rw-r--r--   0 lraming    (503) staff       (20)     1075 2024-02-20 22:06:30.486084 pytRIBS-0.1.1/PKG-INFO
--rw-r--r--   0 lraming    (503) staff       (20)      432 2024-02-20 22:02:31.000000 pytRIBS-0.1.1/README.md
--rw-r--r--   0 lraming    (503) staff       (20)      721 2024-02-20 22:04:55.000000 pytRIBS-0.1.1/pyproject.toml
-drwxr-xr-x   0 lraming    (503) staff       (20)        0 2024-02-20 22:06:30.482811 pytRIBS-0.1.1/pytRIBS/
--rw-r--r--   0 lraming    (503) staff       (20)        0 2024-02-20 18:12:44.000000 pytRIBS-0.1.1/pytRIBS/__init__.py
-drwxr-xr-x   0 lraming    (503) staff       (20)        0 2024-02-20 22:06:30.484091 pytRIBS-0.1.1/pytRIBS/mixins/
--rw-r--r--   0 lraming    (503) staff       (20)        0 2024-02-20 18:12:44.000000 pytRIBS-0.1.1/pytRIBS/mixins/__init__.py
--rw-r--r--   0 lraming    (503) staff       (20)    24337 2024-02-20 18:12:44.000000 pytRIBS-0.1.1/pytRIBS/mixins/infile_mixin.py
--rw-r--r--   0 lraming    (503) staff       (20)    17267 2024-02-20 18:12:44.000000 pytRIBS-0.1.1/pytRIBS/mixins/shared_mixin.py
-drwxr-xr-x   0 lraming    (503) staff       (20)        0 2024-02-20 22:06:30.484879 pytRIBS-0.1.1/pytRIBS/model/
--rw-r--r--   0 lraming    (503) staff       (20)        0 2024-02-20 18:12:44.000000 pytRIBS-0.1.1/pytRIBS/model/__init__.py
--rw-r--r--   0 lraming    (503) staff       (20)     7059 2024-02-20 18:12:44.000000 pytRIBS-0.1.1/pytRIBS/model/aux.py
--rw-r--r--   0 lraming    (503) staff       (20)     5522 2024-02-20 18:12:44.000000 pytRIBS-0.1.1/pytRIBS/model/diagnose.py
--rw-r--r--   0 lraming    (503) staff       (20)    20306 2024-02-20 18:12:44.000000 pytRIBS-0.1.1/pytRIBS/model/inout.py
--rw-r--r--   0 lraming    (503) staff       (20)    13731 2024-02-20 18:20:48.000000 pytRIBS-0.1.1/pytRIBS/model/preprocess.py
-drwxr-xr-x   0 lraming    (503) staff       (20)        0 2024-02-20 22:06:30.485397 pytRIBS-0.1.1/pytRIBS/results/
--rw-r--r--   0 lraming    (503) staff       (20)        0 2024-02-20 18:12:44.000000 pytRIBS-0.1.1/pytRIBS/results/__init__.py
--rw-r--r--   0 lraming    (503) staff       (20)        3 2024-02-20 18:12:44.000000 pytRIBS-0.1.1/pytRIBS/results/post.py
--rw-r--r--   0 lraming    (503) staff       (20)    12675 2024-02-20 18:12:44.000000 pytRIBS-0.1.1/pytRIBS/results/waterbalance.py
--rw-r--r--   0 lraming    (503) staff       (20)     2510 2024-02-20 18:20:48.000000 pytRIBS-0.1.1/pytRIBS/tmodel.py
--rw-r--r--   0 lraming    (503) staff       (20)     9999 2024-02-20 18:12:44.000000 pytRIBS-0.1.1/pytRIBS/tresults.py
-drwxr-xr-x   0 lraming    (503) staff       (20)        0 2024-02-20 22:06:30.485729 pytRIBS-0.1.1/pytRIBS.egg-info/
--rw-r--r--   0 lraming    (503) staff       (20)     1075 2024-02-20 22:06:30.000000 pytRIBS-0.1.1/pytRIBS.egg-info/PKG-INFO
--rw-r--r--   0 lraming    (503) staff       (20)      541 2024-02-20 22:06:30.000000 pytRIBS-0.1.1/pytRIBS.egg-info/SOURCES.txt
--rw-r--r--   0 lraming    (503) staff       (20)        1 2024-02-20 22:06:30.000000 pytRIBS-0.1.1/pytRIBS.egg-info/dependency_links.txt
--rw-r--r--   0 lraming    (503) staff       (20)       70 2024-02-20 22:06:30.000000 pytRIBS-0.1.1/pytRIBS.egg-info/requires.txt
--rw-r--r--   0 lraming    (503) staff       (20)        8 2024-02-20 22:06:30.000000 pytRIBS-0.1.1/pytRIBS.egg-info/top_level.txt
--rw-r--r--   0 lraming    (503) staff       (20)       38 2024-02-20 22:06:30.486398 pytRIBS-0.1.1/setup.cfg
+drwxr-xr-x   0 lraming    (503) staff       (20)        0 2024-04-25 20:54:56.300489 pytribs-0.2.0/
+-rw-r--r--   0 lraming    (503) staff       (20)    18005 2024-03-30 00:40:45.000000 pytribs-0.2.0/LICENSE
+-rw-r--r--   0 lraming    (503) staff       (20)     1835 2024-04-25 20:54:56.300253 pytribs-0.2.0/PKG-INFO
+-rw-r--r--   0 lraming    (503) staff       (20)     1138 2024-04-25 20:49:07.000000 pytribs-0.2.0/README.md
+-rw-r--r--   0 lraming    (503) staff       (20)      760 2024-04-25 20:54:50.000000 pytribs-0.2.0/pyproject.toml
+drwxr-xr-x   0 lraming    (503) staff       (20)        0 2024-04-25 20:54:56.294355 pytribs-0.2.0/pytRIBS/
+-rw-r--r--   0 lraming    (503) staff       (20)        0 2024-03-30 00:40:45.000000 pytribs-0.2.0/pytRIBS/__init__.py
+drwxr-xr-x   0 lraming    (503) staff       (20)        0 2024-04-25 20:54:56.295531 pytribs-0.2.0/pytRIBS/aux/
+-rw-r--r--   0 lraming    (503) staff       (20)        0 2024-03-30 00:40:45.000000 pytribs-0.2.0/pytRIBS/aux/__init__.py
+-rw-r--r--   0 lraming    (503) staff       (20)    16128 2024-03-30 00:40:45.000000 pytribs-0.2.0/pytRIBS/aux/tol_colors.py
+drwxr-xr-x   0 lraming    (503) staff       (20)        0 2024-04-25 20:54:56.296360 pytribs-0.2.0/pytRIBS/mixins/
+-rw-r--r--   0 lraming    (503) staff       (20)        0 2024-03-30 00:40:45.000000 pytribs-0.2.0/pytRIBS/mixins/__init__.py
+-rw-r--r--   0 lraming    (503) staff       (20)    29738 2024-04-08 22:28:13.000000 pytribs-0.2.0/pytRIBS/mixins/infile_mixin.py
+-rw-r--r--   0 lraming    (503) staff       (20)    20162 2024-03-30 00:40:45.000000 pytribs-0.2.0/pytRIBS/mixins/shared_mixin.py
+drwxr-xr-x   0 lraming    (503) staff       (20)        0 2024-04-25 20:54:56.297870 pytribs-0.2.0/pytRIBS/model/
+-rw-r--r--   0 lraming    (503) staff       (20)        0 2024-03-30 00:40:45.000000 pytribs-0.2.0/pytRIBS/model/__init__.py
+-rw-r--r--   0 lraming    (503) staff       (20)     7059 2024-03-30 00:40:45.000000 pytribs-0.2.0/pytRIBS/model/aux.py
+-rw-r--r--   0 lraming    (503) staff       (20)     5522 2024-03-30 00:40:45.000000 pytribs-0.2.0/pytRIBS/model/diagnose.py
+-rw-r--r--   0 lraming    (503) staff       (20)    29398 2024-04-24 23:54:17.000000 pytribs-0.2.0/pytRIBS/model/inout.py
+-rw-r--r--   0 lraming    (503) staff       (20)    28724 2024-04-24 23:27:57.000000 pytribs-0.2.0/pytRIBS/model/preprocess.py
+drwxr-xr-x   0 lraming    (503) staff       (20)        0 2024-04-25 20:54:56.298684 pytribs-0.2.0/pytRIBS/results/
+-rw-r--r--   0 lraming    (503) staff       (20)        0 2024-03-30 00:40:45.000000 pytribs-0.2.0/pytRIBS/results/__init__.py
+-rw-r--r--   0 lraming    (503) staff       (20)        3 2024-03-30 00:40:45.000000 pytribs-0.2.0/pytRIBS/results/post.py
+-rw-r--r--   0 lraming    (503) staff       (20)    12450 2024-04-24 23:27:57.000000 pytribs-0.2.0/pytRIBS/results/waterbalance.py
+drwxr-xr-x   0 lraming    (503) staff       (20)        0 2024-04-25 20:54:56.299292 pytribs-0.2.0/pytRIBS/scratch/
+-rw-r--r--   0 lraming    (503) staff       (20)       98 2024-04-24 23:29:13.000000 pytribs-0.2.0/pytRIBS/scratch/debug.py
+-rw-r--r--   0 lraming    (503) staff       (20)     2467 2024-04-08 21:51:37.000000 pytribs-0.2.0/pytRIBS/scratch/print_input_template.py
+-rw-r--r--   0 lraming    (503) staff       (20)     2511 2024-04-25 19:08:01.000000 pytribs-0.2.0/pytRIBS/tmodel.py
+-rw-r--r--   0 lraming    (503) staff       (20)    12970 2024-03-30 00:40:45.000000 pytribs-0.2.0/pytRIBS/tresults.py
+drwxr-xr-x   0 lraming    (503) staff       (20)        0 2024-04-25 20:54:56.299950 pytribs-0.2.0/pytRIBS.egg-info/
+-rw-r--r--   0 lraming    (503) staff       (20)     1835 2024-04-25 20:54:56.000000 pytribs-0.2.0/pytRIBS.egg-info/PKG-INFO
+-rw-r--r--   0 lraming    (503) staff       (20)      656 2024-04-25 20:54:56.000000 pytribs-0.2.0/pytRIBS.egg-info/SOURCES.txt
+-rw-r--r--   0 lraming    (503) staff       (20)        1 2024-04-25 20:54:56.000000 pytribs-0.2.0/pytRIBS.egg-info/dependency_links.txt
+-rw-r--r--   0 lraming    (503) staff       (20)       97 2024-04-25 20:54:56.000000 pytribs-0.2.0/pytRIBS.egg-info/requires.txt
+-rw-r--r--   0 lraming    (503) staff       (20)        8 2024-04-25 20:54:56.000000 pytribs-0.2.0/pytRIBS.egg-info/top_level.txt
+-rw-r--r--   0 lraming    (503) staff       (20)       38 2024-04-25 20:54:56.300539 pytribs-0.2.0/setup.cfg
```

### Comparing `pytRIBS-0.1.1/LICENSE` & `pytribs-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytRIBS-0.1.1/pyproject.toml` & `pytribs-0.2.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -15,13 +15,15 @@
     "numpy",
     "pandas",
     "matplotlib",
     "geopandas",
     "shapely",
     "rasterio",
     "scipy",
-    "rosetta-soil"
+    "rosetta-soil",
+    "owslib",
+    "matplotlib_scalebar"
 ]
-version = "0.1.1"
+version = "0.2.0"
 
 [project.urls]
-Repository = "https://github.com/WrenRaming/pytRIBS"
+Repository = "https://github.com/tribshms/pytRIBS"
```

### Comparing `pytRIBS-0.1.1/pytRIBS/mixins/shared_mixin.py` & `pytribs-0.2.0/pytRIBS/mixins/shared_mixin.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # shared_mixin.py
 import os
 import glob
 import numpy as np
 
 import geopandas as gpd
 import pandas as pd
+import pyvista as pv
 from shapely.geometry import LineString
 from shapely.geometry import Point
 from shapely.geometry import Polygon
 
 
 class SharedMixin:
     """
@@ -168,14 +169,15 @@
             if len(node_ids) != size:
                 print("Warning: Array size does not match the specified size in the file.")
 
             return node_ids
         except FileNotFoundError:
             print(f"Error: File '{file_path}' not found.")
             return []
+
     def read_reach_file(self, filename=None):
         """
         Returns GeoDataFrame containing reaches from tRIBS model domain.
         :param filename: Set to read _reach file specified from OUTFILENAME,but can be changed.
         :return: GeoDataFrame
         """
 
@@ -231,24 +233,28 @@
         parallel_voi_files = [f for f in os.listdir(outfilename) if 'voi.' in f]  # list of _voi.d+ files
 
         if len(parallel_voi_files) == 0:
             print(f"Cannot find voi files at: {outfilename}. Returning None")
             return None
 
         voi_list = []
+        processor_list = []
         # gdf = gpd.GeoDataFrame(columns=['ID', 'geometry'])
 
         for file in parallel_voi_files:
             voi = self.read_voi_file(f"{outfilename}/{file}")
             if voi is not None:
                 voi_list.append(voi[0])
+                processor = int(file.split("voi.")[-1])  # Extract processor number from file name
+                processor_list.extend(np.ones(len(voi[0])) * int(processor))
             else:
                 print(f'Voi file {file} is empty.')
 
         combined_gdf = gpd.pd.concat(voi_list, ignore_index=True)
+        combined_gdf['processor'] = processor_list  # Add 'processor' column
         combined_gdf = combined_gdf.sort_values(by='ID')
 
         if join is not None:
             combined_gdf = combined_gdf.merge(join, on="ID", how="inner")
 
             # Check for non-matching IDs
             non_matching_ids = join[~join["ID"].isin(combined_gdf["ID"])]
@@ -337,15 +343,15 @@
 
             elif os.path.exists(dynfile):
                 print("Cannot find dynamic output file:" + dynfile)
                 break
 
         return dyn_data
 
-    def mesh2vtk(self,outfile):
+    def mesh2vtk(self, outfile):
         """
 
         :return:
         """
         outfilename = self.options["outfilename"]["value"]
         last_slash_index = outfilename.rfind('/')
         directory_path = outfilename[:last_slash_index + 1]
@@ -368,28 +374,28 @@
             print(f'Cannot find z file at: {directory_path}. Exiting.')
             return
 
         # read in node,tri,z files:
         try:
 
             with open(node_file[0], 'r') as f:
-                lines = f.readlines() #skip first since it's relic feature
+                lines = f.readlines()  # skip first since it's relic feature
 
                 # Check if there's at least one line
                 if lines:
                     num_nodes = int(lines[1])
                     store_nodes = np.zeros((num_nodes, 2))
-                    boundary_code = np.zeros((num_nodes,1))
+                    boundary_code = np.zeros((num_nodes, 1))
 
                     # Iterate from the second line onward
                     for l in range(2, num_nodes + 2):
                         line = lines[l].split()
                         store_nodes[l - 2, 0] = float(line[0])
                         store_nodes[l - 2, 1] = float(line[1])
-                        boundary_code[l-2,0] = float(line[3])
+                        boundary_code[l - 2, 0] = float(line[3])
 
             with open(tri_file[0], 'r') as f:
                 lines = f.readlines()
 
                 # Check if there's at least one line
                 if lines:
                     num_tri = int(lines[1])
@@ -418,43 +424,117 @@
             with open(outfile, 'w') as f:
                 f.write("# vtk DataFile Version 3.0\n")
                 f.write("tRIBS\n")
                 f.write("ASCII\n")
                 f.write("DATASET UNSTRUCTURED_GRID\n")
                 f.write('POINTS {0:10d} float\n'.format(num_nodes))
                 for I in range(num_nodes):
-                    f.write("{0:15.5f} {1:15.5f} {2:15.5f}\n".format(store_nodes[I, 0], store_nodes[I, 1], store_z[I, 0]))
+                    f.write(
+                        "{0:15.5f} {1:15.5f} {2:15.5f}\n".format(store_nodes[I, 0], store_nodes[I, 1], store_z[I, 0]))
 
-                f.write("CELLS {0:10d} {1:10d}\n".format(num_tri, 4*num_tri))
+                f.write("CELLS {0:10d} {1:10d}\n".format(num_tri, 4 * num_tri))
                 for I in range(num_tri):
-                    f.write('3 {0:10d} {1:10d} {2:10d}\n'.format(int(store_tri[I, 0]) , int(store_tri[I, 1]), int(store_tri[I, 2]) ))
+                    f.write('3 {0:10d} {1:10d} {2:10d}\n'.format(int(store_tri[I, 0]), int(store_tri[I, 1]),
+                                                                 int(store_tri[I, 2])))
 
                 f.write("CELL_TYPES {0:10d}\n".format(num_tri))
                 for I in range(num_tri):
                     f.write("5\n")
 
                 f.write("POINT_DATA {0:10d}\n".format(num_nodes))
                 f.write("SCALARS Altitude float 1\n")
                 f.write("LOOKUP_TABLE default\n")
                 for I in range(num_nodes):
-                    if boundary_code[I,0] == 1:
-                        f.write('NaN'+'\n')
+                    if boundary_code[I, 0] == 1:
+                        f.write('NaN' + '\n')
                     else:
                         f.write(str(store_z[I, 0]) + "\n")
 
                 f.write('SCALARS BC_code float 1\n')
                 f.write('LOOKUP_TABLE BC_LUT\n')
 
                 for I in range(num_nodes):
-                    f.write(str(float(boundary_code[I,0]))+'\n')
+                    f.write(str(float(boundary_code[I, 0])) + '\n')
 
                 # possible to add additional scalars
                 # f.write("SCALARS Shear_stress float 1\n")
                 # f.write("LOOKUP_TABLE default\n")
                 # for I in range(num_nodes):
                 #     f.write(str(TABTAU[I, 0]) + "\n")
 
         except FileNotFoundError:
             return
 
+    @staticmethod
+    def plot_mesh(mesh, scalar=None, **kwargs):
+
+        """
+
+        """
+        if isinstance(mesh, str):
+            # check if path exists
+            mesh = pv.read(mesh)
+
+        if scalar is None:
+            scalar = mesh.get_array('Altitude')
+
+        # set closed points or cells to nan
+        if len(scalar) == mesh.n_points:
+            scalar[mesh['BC_code'] == 1] = np.nan
+        elif len(scalar) == mesh.n_cells:
+            extracted = mesh.extract_points(mesh['BC_code'] == 1, adjacent_cells=True)
+            scalar[extracted.cell_data['vtkOriginalCellIds']] = np.nan
+        else:
+            print("Scalar dimensions must match either the number of points or cells in the mesh.")
+
+        plotter = pv.Plotter()
+        plotter.add_mesh(mesh, scalars=scalar, **kwargs)
+
+        plotter.show()
+
+        return plotter
+
+    # This assumes that get_invariant_properties() has been called since requires vornoi? D
+
+    def get_invariant_properties(self):
 
+        parallel_flag = int(self.options["parallelmode"]['value'])
 
+        # read in integrated spatial vars for waterbalance calcs and spatial maps
+        if parallel_flag == 1:
+            temp = self.merge_parallel_spatial_files(suffix="_00i",dtime=int(self.options['runtime']['value']))
+
+            runtime = self.options["runtime"]["value"]
+
+            while len(runtime) < 4:
+                runtime = '0' + runtime
+
+            self.int_spatial_vars = temp[runtime]
+
+        elif parallel_flag == 0:
+            runtime = self.options["runtime"]["value"]
+
+            if len(runtime) < 4:
+                while len(runtime) < 4:
+                    runtime = '0' + runtime
+
+            outfilename = self.options["outfilename"]["value"]
+            intfile = f"{outfilename}.{runtime}_00i"
+
+            self.int_spatial_vars = pd.read_csv(intfile)
+
+            # Note one could use max CAr, but it overestimates area according to Voi geomerty
+            self.int_spatial_vars['weight'] = self.int_spatial_vars.VAr.values / self.int_spatial_vars.VAr.sum()
+
+        else:
+            print('Unable To Read Integrated Spatial File (*_00i).')
+            self.int_spatial_vars = None
+
+        # read in voronoi files only once
+        if parallel_flag == 1:
+            self.voronoi = self.merge_parallel_voi()
+
+        elif parallel_flag == 0:
+            self.voronoi, _ = self.read_voi_file()
+        else:
+            print('Unable To Load Voi File(s).')
+            self.voronoi = None
```

### Comparing `pytRIBS-0.1.1/pytRIBS/model/aux.py` & `pytribs-0.2.0/pytRIBS/model/aux.py`

 * *Files identical despite different names*

### Comparing `pytRIBS-0.1.1/pytRIBS/model/diagnose.py` & `pytribs-0.2.0/pytRIBS/model/diagnose.py`

 * *Files identical despite different names*

### Comparing `pytRIBS-0.1.1/pytRIBS/model/preprocess.py` & `pytribs-0.2.0/pytRIBS/tresults.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,298 +1,309 @@
+import glob
 import os
-import numpy as np
-from scipy.optimize import curve_fit
-from rosetta import rosetta, SoilData
+import re
 
-from pytRIBS.model.inout import InOut
+import numpy as np
+import pandas as pd
+from matplotlib import pyplot as plt
+from matplotlib.animation import FuncAnimation
+from mpl_toolkits.axes_grid1 import make_axes_locatable
 
+from pytRIBS.mixins.infile_mixin import InfileMixin
+from pytRIBS.mixins.shared_mixin import SharedMixin
+from pytRIBS.results.waterbalance import WaterBalance
 
-### PREPROCESSIN
-# 1 delineate watersheds (pyshed)
-# 1.create points file for hydrological conditioned tin Mesh
-# 2 ingest soil and land use (pyshed)
-# 3 apply pedotransfer functions
-# others?
 
-class Preprocess(InOut):
+class Results(InfileMixin, SharedMixin, WaterBalance):
     """
+    A tRIBS Results Class.
+
+    This class provides a framework for analyzing and visualizing individual tRIBS simulations. It takes an instance of
+    Class Simulation and provides time-series and water balance analysis of the model results.
+
 
+    Attributes:
+
+    Methods:
+
+    Example:
+        Provide an example of how to create and use an instance of this class
     """
 
-    # coding=utf-8
-    # This script computes soil textural class using the USDA Soil Triangle and soil parameters required for tRIBS
-    # using the Rosetta Python package.
-    # Manual modifications will need to be to adjust how rasters are read in if script is applied elsewhere,
-    # unit conversions, number of soil properties fed into Rosetta, and assumptions used.
-    # Josh Cederstrom October 2022
+    def __init__(self, input_file, EPSG=None, UTM_Zone=None):
+        # setup model paths and options for Result Class
+        self.options = self.create_input_file()  # input options for tRIBS model run
+        self.read_input_file(input_file)
+
+        # attributes for analysis, plotting, and archiving model results
+        self.element = {}
+        self.mrf = {'mrf': None, 'waterbalance': None}
+        self.geo = {"UTM_Zone": UTM_Zone, "EPSG": EPSG,
+                    "Projection": None}  # Geographic properties of tRIBS model domain.
 
-    # Compute Soil Texture Class
-    @staticmethod
-    def soiltexturalclass(sand, clay):
+        self.get_invariant_properties()  # shared
+
+    def get_mrf_results(self, mrf_file=None):
         """
-        Returns USDA soil textural class given percent sand and clay.
-        :param sand:
-        :param clay: Location to write input file to.
+
         """
-        silt = 100 - sand - clay
+        if mrf_file is None:
+            runtime = self.options["runtime"]["value"]
 
-        if sand + clay > 100 or sand < 0 or clay < 0:
-            raise ValueError('Inputs add up to more than 100% or are negative')
-        elif silt + 1.5 * clay < 15:
-            textural_class = 1  # sand
-        elif silt + 1.5 * clay >= 15 and silt + 2 * clay < 30:
-            textural_class = 2  # loamy sand
-        elif (clay >= 7 and clay < 20 and sand > 52 and silt + 2 * clay >= 30) or (
-                clay < 7 and silt < 50 and silt + 2 * clay >= 30):
-            textural_class = 3  # sandy loam
-        elif clay >= 7 and clay < 27 and silt >= 28 and silt < 50 and sand <= 52:
-            textural_class = 4  # loam
-        elif (silt >= 50 and clay >= 12 and clay < 27) or (silt >= 50 and silt < 80 and clay < 12):
-            textural_class = 5  # silt loam
-        elif silt >= 80 and clay < 12:
-            textural_class = 6  # silt
-        elif clay >= 20 and clay < 35 and silt < 28 and sand > 45:
-            textural_class = 7  # 'sandy clay loam'
-        elif clay >= 27 and clay < 40 and sand > 20 and sand <= 45:
-            textural_class = 8  # 'clay loam'
-        elif clay >= 27 and clay < 40 and sand <= 20:
-            textural_class = 9  # 'silty clay loam'
-        elif clay >= 35 and sand > 45:
-            textural_class = 10  # 'sandy clay'
-        elif clay >= 40 and silt >= 40:
-            textural_class = 11  # 'silty clay'
-        elif clay >= 40 > silt and sand <= 45:
-            textural_class = 12
-        else:
-            textural_class = 'na'
+            while len(runtime) < 4:
+                runtime = '0' + runtime
 
-        return textural_class
+            mrf_file = self.options["outhydrofilename"]["value"] + runtime + "_00.mrf"
 
-    def process_raw_soil(self, grid_input, output=None, ks_only=False):
-        """
-        Writes ascii grids Ks, theta_s, theta_r, psib, and m from gridded soil data for % sand, silt, clay, bulk density, and volumetric water content at 33 and 1500 kPa.
+        # Read the first two rows to get column names and units
+        with open(mrf_file, 'r') as file:
+            column_names = file.readline().strip().split('\t')  # Assuming tab-separated data
+            units = file.readline().strip().split('\t')  # Assuming tab-separated data
 
-        Parameters:
-        - grid_input (list of dict or str): If a dictionary list, keys are "grid_type" and "path" for each soil property.
-                                    Format of dictionary list follows:
-                                    [{'type':'sand_fraction', 'path':'path/to/grid'},
-                                    {'type':'silt_fraction', 'path':'path/to/grid'},
-                                    {'type':'clay_fraction', 'path':'path/to/grid'},
-                                    {'type':'bulk_density', 'path':'path/to/grid'},
-                                    {'type':'vwc_33', 'path':'path/to/grid'},
-                                    {'type':'vwc_1500', 'path':'path/to/grid'}]
-
-                                    If a string is provided, it is treated as the path to a file containing the
-                                    configuration file must be written in json format.
-
-        - output (list, optional): List of output file names for different soil properties.
-        - ks_only True will only write rasters for ks, this is useful if using compute_decay_ks
-
-        Note:
-        - The 'grid_types' key should contain a list of dictionaries, each specifying a grid type and its corresponding file path.
-        - The 'output_files' key should contain a list of exactly 5 output file names for different soil properties.
-        - The file paths in 'grid_types' should be valid, and the 'output_files' list should have the correct size.
+        # Read the data into a DataFrame, skipping the first two rows
+        results_data_frame = pd.read_csv(mrf_file, skiprows=1, sep='\t')
+
+        # Assign column names to the DataFrame
+        results_data_frame.columns = column_names
+
+        # Add units as metadata
+        results_data_frame.attrs["units"] = units
+
+        # # update time from hourly time step to date
+        starting_date = self.options["startdate"]["value"]
+        date = self.convert_to_datetime(starting_date)
+        dt = pd.to_timedelta(results_data_frame['Time'], unit='h')
+        results_data_frame['Time'] = [date + step for step in dt]
+
+        self.mrf['mrf'] = results_data_frame.iloc[0:int(self.options['runtime']['value'])-1] # This is becasue currently v5.2 tribs has issues with mrf writing extra time steps
+
+    def get_element_results(self):
+        """
+        Function assigns a dictionary to self as self.element_results. The keys in the dictionary represent a data
+        frame with the content of the .invpixel file and each subsequent node. Key for .invpixel is "invar",
+        and for nodes is simply the node ID. For each node this function reads in element file and create data frame
+        of results and is assigned to the aforementioned dictionary. TODO:
         """
+        # List to store first integers
+        node_id = []
 
-        # Check if grid_input is a string (path to a config file)
-        if isinstance(grid_input, str):
-            # Read configuration from the file
-            config = self.read_json(grid_input)
-            grids = config['grid_types']
-            output_files = config['output_files']
-        elif isinstance(grid_input, list):
-            # Use provided dictionary
-            grids = grid_input
-            output_files = output or ['Ks.asc', 'theta_r.asc', 'theta_s.asc', 'psib.asc', 'm.asc']
+        # Path to the directory containing the files
+        directory_path = self.options["outfilename"]["value"]
+        # Find the last occurrence of '/'
+        last_slash_index = directory_path.rfind('/')
+
+        # Truncate the string at the last occurrence of '/'
+        directory_path = directory_path[:last_slash_index + 1]
+
+        # Search for files matching the pattern
+        if os.path.exists(directory_path):
+            file_list = glob.glob(directory_path + '*.*')
         else:
-            print('Invalid input format. Provide either a dictionary or a path to a configuration file.')
+            print('Cannot find results directory. Returning nothing.')
             return
 
-        # Check if each file specified in the dictionary or config exists
-        for g in grids:
-            grid_type, path = g['type'], g['path']
-            if not os.path.isfile(path):
-                raise FileNotFoundError(f'Cannot find: {path} for grid type: {grid_type}')
-
-        # Ensure output_files is a list of the correct size (5 elements)
-        if output_files is not None and (not isinstance(output_files, list) or len(output_files) != 5):
-            print('Output must be a list with 5 elements.')
+        if len(file_list) == 0:
+            print("Pixel files not found. Returning nothing.")
             return
 
-        sg250_data = None
-        size = None
-        geo_tiff = None
-
-        # Loop through specified file paths
-        for cnt, g in enumerate(grids):
-            grid_type, path = g['type'], g['path']
-            print(f"Ingesting {grid_type} from: {path}")
-            geo_tiff = self.read_ascii(path)
-            array = geo_tiff['data']
-            size = array.shape
-
-            if cnt == 0:
-                sg250_data = np.zeros((6, size[0], size[1]))
-
-            # each z layer follows:[sa (%), si (%), cl (%), bd (g/cm3), th33, th1500]
-            if grid_type == 'sand_fraction':
-                array = array / 1000 * 100  # convert SSC from g/kg to % SSC
-                sg250_data[0, :, :] = array
-            elif grid_type == 'silt_fraction':
-                array = array / 1000 * 100  # convert SSC from g/kg to % SSC
-                sg250_data[1, :, :] = array
-            elif grid_type == 'clay_fraction':
-                array = array / 1000 * 100  # convert SSC from g/kg to % SSC
-                sg250_data[2, :, :] = array
-            elif grid_type == 'bulk_density':
-                array = array / 100  # convert bulk density from cg/cm3 to g/cm3
-                sg250_data[3, :, :] = array
-            elif grid_type == 'vwc_33':
-                array = array / 1000  # convert bulk density from cg/cm3 to g/cm3
-                sg250_data[4, :, :] = array
-            elif grid_type == 'vwc_1500':
-                array = array / 1000 # convert bulk density from cg/cm3 to g/cm3
-                sg250_data[5, :, :] = array
-
-        profile = geo_tiff['profile']
-
-        # Initialize parameter grids, 3 grids - 1 mean values, 2 std deviations, 3 code/flag
-        theta_r, theta_s, ks, psib, m = np.zeros((3, *size)), np.zeros((3, *size)), np.zeros((3, *size)), np.zeros(
-            (1, *size)), np.zeros((1, *size))
-
-        # Loop through raster's and compute soil properties using rosetta-soil package
-        # Codes/Flags
-        # 2	sand, silt, clay (SSC)
-        # 3	SSC + bulk density (BD)
-        # 4	SSC + BD + field capacity water content (TH33)
-        # 5	SSC + BD + TH33 + wilting point water content (TH1500)
-        # -1 no result returned, inadequate or erroneous data
-        # each z layer follows:[sa (%), si (%), cl (%), bd (g/cm3), th33, th1500]
-        # i.e SoilData([sa (%), si (%), cl (%), bd (g/cm3), th33, th1500])
-
-        for i in range(0, size[0]):
-            for j in range(0, size[1]):
-                # Organize array for input into packag
-                data = [sg250_data[x, i, j] for x in np.arange(0, 6)]
-                soil_data = SoilData.from_array([data])
-                mean, stdev, codes = rosetta(3, soil_data)  # apply Rosetta version 3
-                theta_r[:, i, j] = [mean[0, 0], stdev[0, 0], codes[0]]
-                theta_s[:, i, j] = [mean[0, 1], stdev[0, 1], codes[0]]
-                # Convert ks from log10(cm/day) into mm/hr
-                ks[:, i, j] = [(10 ** mean[0, 4]) * 10 / 24, (10 ** stdev[0, 4]) * 10 / 24, codes[0]]
-
-                # Alpha parameter from rosetta corresponds approximately to the inverse of the air-entry value, cm−1
-                # https://doi.org/10.1029/2019MS001784
-                # Convert from log10(cm) into -1/mm
-                psib[0, i, j] = -1 / ((10 ** mean[0, 2]) * 10)
-
-                # Pore-size Distribution can be calculated from n using m = 1-1/n
-                # http://dx.doi.org/10.4236/ojss.2012.23025
-                # Convert from log10(n) into n
-                m[0, i, j] = 1 - (1 / (10 ** mean[0, 3]))
-
-        # for now only write out mean values
-        soil_prop = [ks[0, :, :], theta_r[0, :, :], theta_s[0, :, :], psib[0, :, :], m[0, :, :]]
-
-        if ks_only:
-            soi_raster = {'data': soil_prop[0], 'profile': profile}
-            self.write_ascii(soi_raster, output_files[0])
-        else:
-            for soil_property, name in zip(soil_prop, output_files):
-                soi_raster = {'data': soil_property, 'profile': profile}
-                self.write_ascii(soi_raster, name)
+        # Iterate through the files
+        for file_name in file_list:
+            file = file_name.split('/')[-1]
+            match = re.search(r'(\d+)\.pixel', file)
+            if match:
+                print(f"Reading in: {file}")
+                first_integer = int(match.group(1))
+                node_id.append(first_integer)
+                self.element.update(
+                    {first_integer: {'pixel': self.read_element_files(file_name), 'waterbalance': None}})
 
-    def compute_ks_decay(self, grid_input, output=None):
+    def read_element_files(self, element_results_file):
         """
-        Produces raster for the conductivity decay parameter f, following Ivanov et al., 2004.
-        :param dict grid_input: If a dictionary list, keys are "depth" and "path" for each soil property.
-                                Depth should be provided in units of mm.
-                                    Format of dictionary list follows (from shallowest to deepest):
-                                    [{'depth':25 , 'path':'path/to/25_mm_ks'},
-                                    ...
-                                    {'depth':800 , 'path':'path/to/800_mm_ks'},]
-
-                                    If a string is provided, it is treated as the path to a configuration file. The
-                                    configuration file must be written in json format.
-        :param str output: Location to save raster with conductivity decay parameter f.
+        Reads in .pixel from tRIBS model results and updates hourly timestep to time
         """
-        # Check if grid_input is a string (path to a config file)
-        if isinstance(grid_input, str):
-            # Read configuration from the file
-            config = self.read_json(grid_input)
-            grids = config['grid_depth']
-            output_file = config['output_file']
-        elif isinstance(grid_input, list):
-            # Use provided dictionary
-            grids = grid_input
-            output_file = output or ['f.asc']
-        else:
-            print('Invalid input format. Provide either a dictionary or a path to a configuration file.')
-            return
 
-        # Check if each file specified in the dictionary or config exists
-        for g in grids:
-            grid_type, path = g['depth'], g['path']
-            if not os.path.isfile(path):
-                raise FileNotFoundError(f'Cannot find: {path} for grid type: {grid_type}')
-
-        ks_data = None
-        size = None
-        raster = None
-        depth_vec = np.zeros(len(grids))
-
-        # Loop through specified file paths
-        for cnt, g in enumerate(grids):
-            depth, path = g['depth'], g['path']
-            print(f"Ingesting Ks grid at {depth} from: {path}")
-            raster = self.read_ascii(path)
-            array = raster['data']
-            depth_vec[cnt] = depth
-
-            if cnt == 0:
-                size = array.shape
-                ks_data = np.zeros((len(grids), size[0], size[1]))
-                ks_data[cnt, :, :] = array
-            else:
-                ks_data[cnt, :, :] = array
+        results_data_frame = pd.read_csv(element_results_file, sep=r"\s+", header=0)
+
+        # update time from hourly time step to date
+        starting_date = self.options["startdate"]["value"]
+        date = self.convert_to_datetime(starting_date)
+        dt = pd.to_timedelta(results_data_frame['Time_hr'], unit='h')
+        results_data_frame['Time'] = [date + step for step in dt]
+
+        return results_data_frame
 
-        # Ensure that ks grids are sorted from surface to the deepest depth
-        depth_sorted = np.argsort(depth_vec)
-        ks_data = ks_data[depth_sorted]
+    @staticmethod
+    def plot_water_balance(waterbalance, saved_fig=None):
+        """
+
+        :param saved_fig:
+       :param waterbalance:
+       :return:
+       """
+
+        # plt.style.use('bmh')
+        barwidth = 0.25
+        fig, ax = plt.subplots()
+
+        ax.bar(np.arange(len(waterbalance)) + barwidth, waterbalance['nP'], align='center', width=barwidth,
+               color='grey', label='nP')
+        rects = ax.patches
+
+        # Make some labels.
+        labels = ["%.0f" % (p - waterbalance) for p, waterbalance in
+                  zip(waterbalance['nP'], waterbalance['dS'] + waterbalance['nQ'] + waterbalance['nET'])]
+        netdiff = [p - waterbalance for p, waterbalance in
+                   zip(waterbalance['nP'], waterbalance['dS'] + waterbalance['nQ'] + waterbalance['nET'])]
+
+        for rect, label in zip(rects, labels):
+            height = rect.get_height()
+            ax.text(
+                rect.get_x() + rect.get_width() / 2, height + 5, label, ha="center", va="bottom"
+            )
+
+        ax.text(len(waterbalance.index), max(waterbalance.nP), "mean difference: " + "%.0f" % np.mean(netdiff))
+
+        waterbalance.plot.bar(ax=ax, y=["nQ", "nET", "dS"], stacked=True, width=barwidth,
+                              color=['tab:blue', 'tab:red', 'tab:cyan'])
+        ax.legend(bbox_to_anchor=(1.35, 0.85), loc='center right',
+                  labels=["Precip.", "Runoff", "Evapo. Trans.", "$\Delta$ Storage"])
+        ax.set_ylabel("Water Flux & $\Delta$ Storage (mm)")
+        ax.set_xticks(range(len(waterbalance.index)), waterbalance.index.strftime("%Y-%m"), rotation=45)
+        fig.autofmt_xdate()
+        plt.show()
+
+        if saved_fig is not None:
+            plt.savefig(saved_fig, bbox_inches='tight')
+
+        return fig, ax
+
+    def get_element_wb_dataframe(self, element_id):
+
+        pixel = self.element[element_id]
+        if isinstance(pixel, dict):
+            pixel = pixel['pixel']  # waterbalance calc already called
+
+        porosity = self.int_spatial_vars.loc[self.int_spatial_vars.ID == element_id, 'Porosity'].values[0]
+        element_area = self.int_spatial_vars.loc[self.int_spatial_vars.ID == element_id, 'VAr'].values[0]
+
+        df = pd.DataFrame({
+            'Time': pixel['Time'],
+            'Unsat_mm': pixel['Mu_mm'].values,
+            'Sat_mm': pixel['Nwt_mm'].values * porosity,
+            'CanopySWE_mm': 10 * pixel['IntSWEq_cm'].values,
+            'SWE_mm': 10 * pixel['SnWE_cm'].values,
+            'Canop_mm': pixel['CanStorage_mm'],
+            'P_mm_h': pixel['Rain_mm_h'],
+            'ET_mm_h': pixel['EvpTtrs_mm_h'] - (
+                    pixel['SnSub_cm'] * 10 + pixel['SnEvap_cm'] * 10 + pixel['IntSub_cm'] * 10),
+            'Qsurf_mm_h': pixel['Srf_Hour_mm'],
+            'Qunsat_mm_h': pixel['QpIn_mm_h'] - pixel['QpOut_mm_h'],
+            'Qsat_mm_h': pixel['GWflx_m3_h'] / element_area * 1000
+        })
+
+        return df
+
+    def get_mrf_wb_dataframe(self):
+        drainage_area = self.int_spatial_vars['VAr'].sum()  ## in m, TODO investigate why sum 'VAr' != max CAr ?
+        weights = self.int_spatial_vars['VAr'].values / drainage_area
+        porosity = np.sum(self.int_spatial_vars['Porosity'].values * weights)
+
+        mrf = self.mrf['mrf']
+
+        df = pd.DataFrame({
+            'Time': mrf['Time'],
+            'Unsat_mm': mrf['MSMU'].values * mrf['MDGW'].values * porosity,
+            'Sat_mm': mrf['MDGW'] * porosity,
+            'CanopySWE_mm': 10 * mrf['AvInSn'].values,
+            'SWE_mm': 10 * mrf['AvSWE'].values,
+            'Canop_mm': 0,  # not average canopy  storage
+            'P_mm_h': mrf['MAP'],
+            'ET_mm_h': mrf['MET'] - (mrf['AvSnSub'] * 10 + mrf['AvSnEvap'] * 10 + mrf['AvInSu'] * 10),
+            'Qsurf_mm_h': mrf['Srf'] * 3600 * 1000 / drainage_area,
+            'Qunsat_mm_h': 0,  # assumed zero, but not sure if correct?
+            'Qsat_mm_h': 0  # assumed zero, but not sure if correct?
+        })
+
+        return df
 
-        depth_vec = depth_vec[depth_sorted]
-        depth_vec = depth_vec.astype(float)  # ensure float for fitting
+    def create_animation(self, outfile, df_dict, frames, var, fps=4, vlims=None, nan_color='gray',
+                         nan_edge_color='red', cmap='viridis'):
+        """
+        Create and save an animation based on a dictionary of DataFrames of tRIBS dynamic files.
 
-        profile = raster['profile']  # for writing later
+        Parameters:
+            outfile (str): The file path for saving the animation, format is determined from file extension (.mp4,.gif,.avi,.html).
+            df_dict (dict): A dictionary where keys represent animation frames and values are DataFrames to be plotted.
+            frames (iterable): Iterable containing keys from df_dict representing the frames to include in the animation.
+            var (str): The column name in DataFrames to be plotted.
+            fps (int, optional): Frames per second for the animation (default is 4).
+            vlims (tuple, optional): Tuple containing minimum and maximum values for color normalization (default is None).
+            nan_color (str, optional): Color for NaN values in the plot (default is 'gray').
+            nan_edge_color (str, optional): Edge color for NaN values in the plot (default is 'red').
+
+        Returns:
+            None
+
+        Raises:
+            ValueError: If outfile is not a valid file path or frames is empty.
+
+        Notes:
+            - This method creates an animation by iterating over frames specified in the frames parameter.
+            - Each frame corresponds to a key in the df_dict dictionary, and the corresponding DataFrame is plotted.
+            - NaN values in the DataFrame are flagged with the specified nan_color and nan_edge_color.
+            - The animation format is dependent on the outfile extension with the specified frames per second (fps).
+
+        Example:
+            # Assuming instance is an instance of the class containing create_animation method
+            instance.create_animation("animation.gif", df_dict, frames=['0','1','2','3'], var="ET", fps=10)
+        """
 
-        # Initialize parameter grids
-        f_grid = np.zeros(np.shape(array))  # parameter grid
-        fcov = np.zeros(np.shape(array))  # coef of variance grid
+        def update_plot(key, ax, cax):
+            """
+            Update the plot for each frame in the animation.
+
+            Parameters:
+                key: The key representing the current frame in df_dict.
+                ax: The main axes object for the plot.
+                cax: The colorbar axes object.
+                df_dict: A dictionary containing DataFrames for each frame.
+                results_class: An instance of the class containing the voronoi attribute.
+                var: The variable to be plotted from DataFrames.
+                vlims: Tuple containing minimum and maximum values for color normalization.
+
+            Returns:
+                None
+            """
+            ax.clear()
+
+            df = df_dict[key]
+            gdf = self.voronoi.copy()
+            gdf = gdf.merge(df, on="ID", how="inner")
 
-        # Loop through raster's and compute soil properties using rosetta-soil package
-        for i in range(0, size[0]):
-            for j in range(0, size[1]):
-                y = np.array([ks_data[n, i, j] for n in np.arange(0, len(grids))])
+            if vlims is not None:
+                gdf.plot(ax=ax, column=var, legend=True, cmap=cmap, vmin=min(vlims), vmax=max(vlims), cax=cax)
+            else:
+                gdf.plot(ax=ax, column=var, legend=True, cmap=cmap, cax=cax)
 
-                try:
-                    # ensure float
-                    y = y.astype(float)
-                except ValueError:
-                    raise ValueError("Input data must be convertible to float")
+            # flag and plot nans
+            if len(gdf[gdf[var].isnull()]) != 0:
+                gdf[gdf[var].isnull()].plot(ax=ax, color=nan_color, edgecolor=nan_edge_color)
 
-                k0 = y[0]
+            ax.set_title(f'{var}: {key}')
 
-                # define exponential decay function, Ivanov et al. (2004) eqn 17
-                decay = lambda x, f, k=k0: k * (f * x / (np.exp(f * x) - 1.0))
+            plt.axis('off')
+            plt.xticks([])  # Remove x-axis ticks and labels
+            plt.yticks([])  # Remove y-axis ticks and labels
 
-                # perform curve fitting, set limits on f and surface Ksat for stability
-                minf, maxf = 1E-7, k0 - 1E-5
-                minks = 1
+        # Create a figure and axis
+        fig, ax = plt.subplots()
+        divider = make_axes_locatable(ax)
+        cax = divider.append_axes("right", size="5%", pad=0.1)
 
-                param, param_cov = curve_fit(decay, depth_vec, y, bounds = ([minf, maxf],[minks, k0]))
+        # Create the animation
+        animation = FuncAnimation(fig, update_plot, frames=frames, fargs=(ax, cax),
+                                  repeat=False)
 
-                # Write Curve fitting results to grid
-                f_grid[i, j] = param[0]
-                fcov[i, j] = param_cov[0, 0]
+        # To save the animation as a GIF
+        animation.save(outfile, fps=fps)
 
-        f_raster = {'data': f_grid, 'profile': profile}
-        self.write_ascii(f_raster, output_file[0])
+        plt.show()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pytRIBS-0.1.1/pytRIBS/results/waterbalance.py` & `pytribs-0.2.0/pytRIBS/results/waterbalance.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import pandas as pd
 from matplotlib import pyplot as plt
 
 class WaterBalance:
     def get_mrf_water_balance(self, method):
         """
         """
-        waterbalance = self._run_mrf_water_balance(self,method)
+        waterbalance = self._run_mrf_water_balance(method)
         self.mrf['waterbalance'] = waterbalance
     
     
     def get_element_water_balance(self, method):
         """
         Calculate water balance for elements in the model.
     
@@ -27,22 +27,15 @@
         """
     
         node_file = self.options["nodeoutputlist"]["value"]
         nodes = self.read_node_list(node_file)
     
         for n in nodes:
             n = int(n)
-    
-            if isinstance(self.element[n], dict):
-                data = self.element[n]['pixel']  # waterbalance calcs have already been run
-            else:
-                data = self.element[n]
-    
-    
-            waterbalance = self._run_element_water_balance(self, n, method)
+            waterbalance = self._run_element_water_balance(n, method)
             self.element[n]["waterbalance"] = waterbalance
     
     
     # WATER BALANCE FUNCTIONS
     def _run_element_water_balance(self, element_id, method):
         """
```

### Comparing `pytRIBS-0.1.1/pytRIBS/tmodel.py` & `pytribs-0.2.0/pytRIBS/tmodel.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 
     """
 
     def __init__(self):
         # attributes
         self.options = self.create_input_file()  # input options for tRIBS model run
         self.geo = {"UTM_Zone": None, "EPSG": None, "Projection": None}
-        self.area = None
+        #self.area = None
 
     # SIMULATION METHODS
     def __getattr__(self, name):
         if name in self.options:
             return self.options[name]
         raise AttributeError(f"'{self.__class__.__name__}' object has no attribute '{name}'")
```

### Comparing `pytRIBS-0.1.1/pytRIBS.egg-info/SOURCES.txt` & `pytribs-0.2.0/pytRIBS.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -5,18 +5,22 @@
 pytRIBS/tmodel.py
 pytRIBS/tresults.py
 pytRIBS.egg-info/PKG-INFO
 pytRIBS.egg-info/SOURCES.txt
 pytRIBS.egg-info/dependency_links.txt
 pytRIBS.egg-info/requires.txt
 pytRIBS.egg-info/top_level.txt
+pytRIBS/aux/__init__.py
+pytRIBS/aux/tol_colors.py
 pytRIBS/mixins/__init__.py
 pytRIBS/mixins/infile_mixin.py
 pytRIBS/mixins/shared_mixin.py
 pytRIBS/model/__init__.py
 pytRIBS/model/aux.py
 pytRIBS/model/diagnose.py
 pytRIBS/model/inout.py
 pytRIBS/model/preprocess.py
 pytRIBS/results/__init__.py
 pytRIBS/results/post.py
-pytRIBS/results/waterbalance.py
+pytRIBS/results/waterbalance.py
+pytRIBS/scratch/debug.py
+pytRIBS/scratch/print_input_template.py
```


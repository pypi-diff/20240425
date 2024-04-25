# Comparing `tmp/ttclust-4.8.4.tar.gz` & `tmp/ttclust-4.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\ttclust-4.8.4.tar", last modified: Sat Feb  6 15:58:28 2021, max compression
+gzip compressed data, was "dist\ttclust-4.9.0.tar", last modified: Thu Mar  4 21:43:22 2021, max compression
```

## Comparing `ttclust-4.8.4.tar` & `ttclust-4.9.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2021-02-06 15:58:28.462312 ttclust-4.8.4/
--rw-rw-rw-   0        0        0      375 2021-02-06 15:58:28.461312 ttclust-4.8.4/PKG-INFO
--rw-rw-rw-   0        0        0    15222 2020-11-04 16:28:04.000000 ttclust-4.8.4/README.md
--rw-rw-rw-   0        0        0       42 2021-02-06 15:58:28.462312 ttclust-4.8.4/setup.cfg
--rw-rw-rw-   0        0        0     1233 2021-02-06 15:50:39.000000 ttclust-4.8.4/setup.py
-drwxrwxrwx   0        0        0        0 2021-02-06 15:58:28.447811 ttclust-4.8.4/ttclust/
--rw-rw-rw-   0        0        0       32 2020-02-15 16:21:47.000000 ttclust-4.8.4/ttclust/__init__.py
--rw-rw-rw-   0        0        0    49986 2021-02-06 15:41:36.000000 ttclust-4.8.4/ttclust/ttclust.py
--rw-rw-rw-   0        0        0       23 2021-02-06 15:58:28.000000 ttclust-4.8.4/ttclust/version.py
-drwxrwxrwx   0        0        0        0 2021-02-06 15:58:28.459313 ttclust-4.8.4/ttclust.egg-info/
--rw-rw-rw-   0        0        0      375 2021-02-06 15:58:28.000000 ttclust-4.8.4/ttclust.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      264 2021-02-06 15:58:28.000000 ttclust-4.8.4/ttclust.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-02-06 15:58:28.000000 ttclust-4.8.4/ttclust.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2021-02-06 15:58:28.000000 ttclust-4.8.4/ttclust.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      120 2021-02-06 15:58:28.000000 ttclust-4.8.4/ttclust.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2021-02-06 15:58:28.000000 ttclust-4.8.4/ttclust.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2021-03-04 21:43:22.000000 ttclust-4.9.0/
+-rw-rw-rw-   0        0        0      375 2021-03-04 21:43:22.000000 ttclust-4.9.0/PKG-INFO
+-rw-rw-rw-   0        0        0    15222 2020-11-04 16:28:04.000000 ttclust-4.9.0/README.md
+-rw-rw-rw-   0        0        0       42 2021-03-04 21:43:22.000000 ttclust-4.9.0/setup.cfg
+-rw-rw-rw-   0        0        0     1266 2021-03-04 21:42:55.000000 ttclust-4.9.0/setup.py
+drwxrwxrwx   0        0        0        0 2021-03-04 21:43:22.000000 ttclust-4.9.0/ttclust/
+-rw-rw-rw-   0        0        0       32 2020-02-15 16:21:47.000000 ttclust-4.9.0/ttclust/__init__.py
+-rw-rw-rw-   0        0        0    50657 2021-03-04 21:31:35.000000 ttclust-4.9.0/ttclust/ttclust.py
+-rw-rw-rw-   0        0        0       23 2021-03-04 21:43:22.000000 ttclust-4.9.0/ttclust/version.py
+drwxrwxrwx   0        0        0        0 2021-03-04 21:43:22.000000 ttclust-4.9.0/ttclust.egg-info/
+-rw-rw-rw-   0        0        0      375 2021-03-04 21:43:22.000000 ttclust-4.9.0/ttclust.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      264 2021-03-04 21:43:22.000000 ttclust-4.9.0/ttclust.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2021-03-04 21:43:22.000000 ttclust-4.9.0/ttclust.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2021-03-04 21:43:22.000000 ttclust-4.9.0/ttclust.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      127 2021-03-04 21:43:22.000000 ttclust-4.9.0/ttclust.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2021-03-04 21:43:22.000000 ttclust-4.9.0/ttclust.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `ttclust-4.8.4/README.md` & `ttclust-4.9.0/README.md`

 * *Files identical despite different names*

### Comparing `ttclust-4.8.4/setup.py` & `ttclust-4.9.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 MAJOR = 4
-MINOR = 8
-PATCH = 4
+MINOR = 9
+PATCH = 0
 VERSION = "{}.{}.{}".format(MAJOR, MINOR, PATCH)
 
 with open("ttclust/version.py", "w") as f:
     f.write("__version__ = '{}'\n".format(VERSION))
 
 
 setup(
@@ -26,14 +26,15 @@
                       'matplotlib',
                       'numpy',
                       'prettytable',
                       'pandas',
                       'scipy >= 0.18',
                       'scikit-learn',
                       'numba',
+                      'hashlib'
                       'mdtraj >= 1.7'],
 
     entry_points={'console_scripts':['ttclust=ttclust.ttclust:main']},
         #'gui_scripts':['ttclustGUI=ttclust.ttclustGUI:main'],
```

### Comparing `ttclust-4.8.4/ttclust/ttclust.py` & `ttclust-4.9.0/ttclust/ttclust.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 import matplotlib.pyplot as plt
 import mdtraj as md
 import numpy as np
 import operator
 import progressbar as pg
 import scipy.cluster.hierarchy as sch
 from numba import jit, prange
+from hashlib import md5
 
 
 try:
     # This if the "builded" import version
     from .version import __version__
 except:
     # for usage from sources
@@ -258,31 +259,41 @@
         else:
             print("NOTE : Nucleic acids found.")
             print("       Automatic switch to nucleic acid mode")
 
     return selection
 
 
-def save_dist_mat(distmat, rmsd_string):
+def save_dist_mat(distmat, rmsd_string, maxtrixtype):
     """
     DESCRIPTION
     Save the numpy matrix to reused afterward
     ----
     Args:
         distmat (numpy matrix): distance matrix
         rmsd_string (str) : selection string for rmsd calculation
     return:
         None
     """
     if rmsd_string:
         name = rmsd_string.replace(" ", "_")
+
     else:
         name = "matrix_all"
-    np.save(name, distmat)
-    printScreenLogfile("Saving distance matrix : {0}.npy".format(name))
+
+    try:
+        np.save(name, distmat)
+        printScreenLogfile("Saving {0} : {1}.npy".format(maxtrixtype, name))
+    except OSError as error:
+        print("Selection line too long to be used as filename. TTClust will hash it")
+        namehashed = md5(name.encode()).hexdigest()
+        print(f"{name} -> {namehashed}")
+        np.save(namehashed, distmat)
+        printScreenLogfile("Saving {0}: {1}.npy".format(maxtrixtype, namehashed))
+
 
 
 def reorder_cluster(clusters):
     """
     DESCRIPTION
     Reorder the clusters number to have the first frame belonging to the
     cluster 1.
@@ -408,15 +419,15 @@
     elif choice.upper() == "N":  # don't want to use it.. Recalculate!
         print("Calculation mode activated")
         return None
     elif choice.upper() == "O":  # I want to use another npy distance matrix
         npy_files = glob.glob("*.npy")
         for i, file in enumerate(npy_files):
             print("  {0} - {1}".format(i + 1, file))
-        print(" -->Please chooce and press Enter")
+        print(" -->Please choose and press Enter")
         # Check if the user give a good answer
         choice_file = input()
         try:
             name = npy_files[int(choice_file) - 1]
             return name
         except:
             print("I didn't understand. Please try again")
@@ -436,20 +447,26 @@
         rmsd_string (str) : name of the numpy matrix
     """
     if rmsd_string:
         name = rmsd_string.replace(" ", "_")
     else:
         name = "matrix_all"
     # Searching all npy file in the folder
-    npy_files = glob.glob("*.npy")
+    namehashed = md5(name.encode()).hexdigest()
+    namehashed += '.npy'
+
     if not name[-4:] == ".npy":
         name += ".npy"
 
+    npy_files = glob.glob("*.npy")
+
     if name in npy_files and not args["interactive"].lower() == "n":
         return ask_choice(args, name)
+    elif namehashed in npy_files and not args["interactive"].lower() == "n":
+        return ask_choice(args, namehashed)
     else:
         return None
 
 
 def calculate_representative_frame_spread(clusters_list, DM):
     """
     DESCRIPTION
@@ -564,15 +581,15 @@
             pbar.update(counter)
             counter += 1
         pbar.finish()
 
 
         # Finaly, we save the matrix if we want to load it again afterward
         print("Calculation ended - saving distance matrix")
-        save_dist_mat(distances, args["select_rmsd"])
+        save_dist_mat(distances, args["select_rmsd"], "distance matrix")
 
         return distances
 
 
 def onclick(event):
     """
     DESCRIPTION
@@ -689,15 +706,15 @@
     cutoff = args["cutoff"]
     ncluster = args["ngroup"]
     # Creation of the distance matrix
 
     if select_rmsd == None:
         select_rmsd = "None"
 
-    linkage_file = search_dist_mat(untouch_select_rmsd + " linkage " + args["method"], args)
+    linkage_file = search_dist_mat(select_align+'--'+untouch_select_rmsd + " linkage " + args["method"], args)
 
     if linkage_file:
         linkage = np.load(linkage_file)
     else:
         print("         Matrix shape: {}".format(distances.shape))
         print("         Scipy linkage in progress. Please wait. It can be long")
         # linkage method from https://docs.scipy.org/doc/scipy/reference/generated/scipy.cluster.hierarchy.linkage.html
@@ -707,15 +724,15 @@
         else:
             printScreenLogfile("ERROR : method name given for clustering didn't recognized")
             printScreenLogfile("      : methods are : single; complete; average; weighted; centroid; ward.")
             printScreenLogfile("      : check https://docs.scipy.org/doc/scipy/reference/generated/scipy.cluster.hierarchy.linkage.html")
             sys.exit(1)
         print("         >Done!")
         print("         ...Saving linkage matrix...")
-        save_dist_mat(linkage, untouch_select_rmsd + " linkage " + args["method"])
+        save_dist_mat(linkage, select_align+'--'+untouch_select_rmsd + " linkage " + args["method"], "linkage matrix")
         print("         >Done!")
 
     # if a cuttof for distance cuting is given
     if cutoff:
         clustering_result = sch.fcluster(linkage, cutoff, "distance")
     # otherwise we choose it on the screen by cliking on the matplotlib windows
     # If a number of wanted cluster is given
```


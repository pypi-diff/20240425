# Comparing `tmp/nt2py-0.2.1.tar.gz` & `tmp/nt2py-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nt2py-0.2.1.tar", last modified: Thu Jan 25 10:24:47 2024, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `nt2py-0.2.1.tar` & `nt2py-0.3.0.tar`

### file list

```diff
@@ -1,27 +1,12 @@
-drwxr-xr-x   0 hayk      (1000) hayk      (1000)        0 2024-01-25 10:24:47.554218 nt2py-0.2.1/
-drwxr-xr-x   0 hayk      (1000) hayk      (1000)        0 2024-01-25 10:24:47.544218 nt2py-0.2.1/.github/
-drwxr-xr-x   0 hayk      (1000) hayk      (1000)        0 2024-01-25 10:24:47.554218 nt2py-0.2.1/.github/workflows/
--rw-r--r--   0 hayk      (1000) hayk      (1000)      347 2023-12-29 09:10:54.000000 nt2py-0.2.1/.github/workflows/publish.yml
--rw-r--r--   0 hayk      (1000) hayk      (1000)     3072 2023-12-29 09:22:46.000000 nt2py-0.2.1/.gitignore
--rw-r--r--   0 hayk      (1000) hayk      (1000)     1501 2023-12-29 09:05:37.000000 nt2py-0.2.1/LICENSE
--rw-r--r--   0 hayk      (1000) hayk      (1000)       56 2023-12-29 08:57:29.000000 nt2py-0.2.1/MANIFEST.in
--rw-r--r--   0 hayk      (1000) hayk      (1000)     1349 2024-01-25 10:24:47.554218 nt2py-0.2.1/PKG-INFO
--rw-r--r--   0 hayk      (1000) hayk      (1000)      804 2023-12-29 09:33:26.000000 nt2py-0.2.1/README.md
-drwxr-xr-x   0 hayk      (1000) hayk      (1000)        0 2024-01-25 10:24:47.554218 nt2py-0.2.1/dist/
--rw-r--r--   0 hayk      (1000) hayk      (1000)    14772 2023-12-29 09:29:20.000000 nt2py-0.2.1/dist/nt2py-0.2.tar.gz
-drwxr-xr-x   0 hayk      (1000) hayk      (1000)        0 2024-01-25 10:24:47.554218 nt2py-0.2.1/nt2/
--rw-r--r--   0 hayk      (1000) hayk      (1000)       24 2024-01-25 10:24:18.000000 nt2py-0.2.1/nt2/__init__.py
--rw-r--r--   0 hayk      (1000) hayk      (1000)     3754 2023-12-29 08:54:18.000000 nt2py-0.2.1/nt2/export.py
--rw-r--r--   0 hayk      (1000) hayk      (1000)     3409 2023-12-29 08:54:18.000000 nt2py-0.2.1/nt2/plot.py
--rw-r--r--   0 hayk      (1000) hayk      (1000)    29727 2023-12-29 08:54:18.000000 nt2py-0.2.1/nt2/read.py
-drwxr-xr-x   0 hayk      (1000) hayk      (1000)        0 2024-01-25 10:24:47.554218 nt2py-0.2.1/nt2py.egg-info/
--rw-r--r--   0 hayk      (1000) hayk      (1000)     1349 2024-01-25 10:24:47.000000 nt2py-0.2.1/nt2py.egg-info/PKG-INFO
--rw-r--r--   0 hayk      (1000) hayk      (1000)      369 2024-01-25 10:24:47.000000 nt2py-0.2.1/nt2py.egg-info/SOURCES.txt
--rw-r--r--   0 hayk      (1000) hayk      (1000)        1 2024-01-25 10:24:47.000000 nt2py-0.2.1/nt2py.egg-info/dependency_links.txt
--rw-r--r--   0 hayk      (1000) hayk      (1000)        1 2023-12-29 09:29:20.000000 nt2py-0.2.1/nt2py.egg-info/not-zip-safe
--rw-r--r--   0 hayk      (1000) hayk      (1000)       72 2024-01-25 10:24:47.000000 nt2py-0.2.1/nt2py.egg-info/requires.txt
--rw-r--r--   0 hayk      (1000) hayk      (1000)        4 2024-01-25 10:24:47.000000 nt2py-0.2.1/nt2py.egg-info/top_level.txt
--rw-r--r--   0 hayk      (1000) hayk      (1000)      124 2023-12-29 08:58:18.000000 nt2py-0.2.1/pyproject.toml
--rw-r--r--   0 hayk      (1000) hayk      (1000)      772 2023-12-29 08:54:18.000000 nt2py-0.2.1/requirements.txt
--rw-r--r--   0 hayk      (1000) hayk      (1000)      470 2024-01-25 10:24:47.554218 nt2py-0.2.1/setup.cfg
--rw-r--r--   0 hayk      (1000) hayk      (1000)      256 2023-12-29 08:55:52.000000 nt2py-0.2.1/setup.py
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 nt2py-0.3.0/MANIFEST.in
+-rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 nt2py-0.3.0/requirements.txt
+-rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 nt2py-0.3.0/.github/workflows/publish.yml
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 nt2py-0.3.0/nt2/__init__.py
+-rw-r--r--   0        0        0     3754 2020-02-02 00:00:00.000000 nt2py-0.3.0/nt2/export.py
+-rw-r--r--   0        0        0     3409 2020-02-02 00:00:00.000000 nt2py-0.3.0/nt2/plot.py
+-rw-r--r--   0        0        0    29838 2020-02-02 00:00:00.000000 nt2py-0.3.0/nt2/read.py
+-rw-r--r--   0        0        0     3083 2020-02-02 00:00:00.000000 nt2py-0.3.0/.gitignore
+-rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 nt2py-0.3.0/LICENSE
+-rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 nt2py-0.3.0/README.md
+-rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 nt2py-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3749 2020-02-02 00:00:00.000000 nt2py-0.3.0/PKG-INFO
```

### Comparing `nt2py-0.2.1/.gitignore` & `nt2py-0.3.0/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -153,7 +153,9 @@
 
 # PyCharm
 #  JetBrains specific template is maintained in a separate JetBrains.gitignore that can
 #  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
 #  and can be added to the global gitignore or merged into this file.  For a more nuclear
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
 #.idea/
+test/
+temp/
```

### Comparing `nt2py-0.2.1/LICENSE` & `nt2py-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nt2py-0.2.1/README.md` & `nt2py-0.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-## nt2
+## nt2.py
 
 Python package for visualization and post-processing of the [`Entity`](https://github.com/entity-toolkit/entity) simulation data. For usage, please refer to the [documentation](https://entity-toolkit.github.io/entity/howto/vis/#nt2py). The package is distributed via [`PyPI`](https://pypi.org/project/nt2py/):
 
 ```sh
 pip install nt2py
 ```
 
@@ -12,8 +12,8 @@
 2. Context-aware data manipulation with [`xarray`](http://xarray.pydata.org/en/stable/).
 3. Parellel plotting and movie generation with [`multiprocessing`](https://docs.python.org/3/library/multiprocessing.html) and [`ffmpeg`](https://ffmpeg.org/).
 
 ### TODO
 
 - [ ] Unit tests
 - [ ] Plugins for other simulation data formats
-- [ ] Usage examples
+- [ ] Usage examples
```

### Comparing `nt2py-0.2.1/nt2/export.py` & `nt2py-0.3.0/nt2/export.py`

 * *Files identical despite different names*

### Comparing `nt2py-0.2.1/nt2/plot.py` & `nt2py-0.3.0/nt2/plot.py`

 * *Files identical despite different names*

### Comparing `nt2py-0.2.1/nt2/read.py` & `nt2py-0.3.0/nt2/read.py`

 * *Files 4% similar despite different names*

```diff
@@ -585,82 +585,81 @@
         QuantityDict = {
             "Ttt": "E",
             "Ttx": "Px",
             "Tty": "Py",
             "Ttz": "Pz",
         }
         CoordinateDict = {
-            "cartesian": {"x": "x", "y": "y", "z": "z", "1": "x", "2": "y", "3": "z"},
-            "spherical": {
+            "cart": {"x": "x", "y": "y", "z": "z", "1": "x", "2": "y", "3": "z"},
+            "sph": {
                 "r": "r",
                 "theta": "θ" if useGreek else "th",
                 "phi": "φ" if useGreek else "ph",
                 "1": "r",
                 "2": "θ" if useGreek else "th",
                 "3": "φ" if useGreek else "ph",
             },
         }
         PrtlDict = {
-            "cartesian": {
+            "cart": {
                 "X1": "x",
                 "X2": "y",
                 "X3": "z",
                 "U1": "ux",
                 "U2": "uy",
                 "U3": "uz",
             },
-            "spherical": {
+            "sph": {
                 "X1": "r",
                 "X2": "θ" if useGreek else "th",
                 "X3": "φ" if useGreek else "ph",
                 "U1": "ur",
                 "U2": "uΘ" if useGreek else "uth",
                 "U3": "uφ" if useGreek else "uph",
             },
         }
         self.fname = fname
         try:
             self.file = h5py.File(self.fname, "r")
         except OSError:
             raise OSError(f"Could not open file {self.fname}")
         step0 = list(self.file.keys())[0]
-        nsteps = int(self.file.attrs["NumSteps"])
+        nsteps = len(self.file.keys())
         ngh = int(self.file.attrs["NGhosts"])
         layout = "right" if self.file.attrs["LayoutRight"] == 1 else "left"
         dimension = int(self.file.attrs["Dimension"])
         coordinates = self.file.attrs["Coordinates"].decode("UTF-8")
-        if coordinates == "qspherical":
-            coordinates = "spherical"
-        if coordinates == "spherical":
+        if coordinates == "qsph":
+            coordinates = "sph"
+        if coordinates == "sph":
             self.metric = SphericalMetric()
         else:
             self.metric = MinkowskiMetric()
         coords = list(CoordinateDict[coordinates].values())[::-1][-dimension:]
         # cell-centered coords
-        cc_coords = {
-            c: EdgeToCenter(self.file.attrs[f"X{i+1}"])
-            for i, c in enumerate(coords[::-1])
-        }
-        # upper and lower limits of the cell
+        cc_coords = {c: self.file[step0][f"X{i+1}"] for i, c in enumerate(coords[::-1])}
+        # cell edges
         cell_1 = {
             f"{c}_1": (
                 c,
-                self.file.attrs[f"X{i+1}"][:-1],
+                self.file[step0][f"X{i+1}e"][:-1],
             )
             for i, c in enumerate(coords[::-1])
         }
         cell_2 = {
             f"{c}_2": (
                 c,
-                self.file.attrs[f"X{i+1}"][1:],
+                self.file[step0][f"X{i+1}e"][1:],
             )
             for i, c in enumerate(coords[::-1])
         }
 
-        times = np.array([self.file[f"Step{s}"]["Time"][()] for s in range(nsteps)])
+        times = np.array(
+            [self.file[f"Step{s}"]["Time"][()] for s in range(nsteps)], dtype=float
+        )
 
         if dimension == 1:
             noghosts = slice(ngh, -ngh) if ngh > 0 else slice(None)
         elif dimension == 2:
             noghosts = (slice(ngh, -ngh), slice(ngh, -ngh)) if ngh > 0 else slice(None)
         elif dimension == 3:
             noghosts = (
@@ -696,17 +695,19 @@
                     np.transpose(self.file[f"Step{s}/{k}"])
                     if layout == "right"
                     else self.file[f"Step{s}/{k}"]
                 )
                 dask_arrays.append(array[noghosts])
 
             k_ = reduce(
-                lambda x, y: x.replace(*y)
-                if "_" not in x
-                else "_".join([x.split("_")[0].replace(*y)] + x.split("_")[1:]),
+                lambda x, y: (
+                    x.replace(*y)
+                    if "_" not in x
+                    else "_".join([x.split("_")[0].replace(*y)] + x.split("_")[1:])
+                ),
                 [k, *list(CoordinateDict[coordinates].items())],
             )
             k_ = reduce(
                 lambda x, y: x.replace(*y),
                 [k_, *list(QuantityDict.items())],
             )
             x = xr.DataArray(
@@ -718,76 +719,76 @@
                     **cc_coords,
                     **cell_1,
                     **cell_2,
                 },
             )
             self.dataset[k_] = x
 
-        prtls = [
-            k
-            for k in self.file[step0].keys()
-            if (k.startswith("X") or k.startswith("U") or k.startswith("W"))
-        ]
-
-        species = np.unique(
-            [int(pq.split("_")[1]) for pq in self.file[step0].keys() if pq in prtls]
-        )
-
-        def list_to_ragged(arr):
-            max_len = np.max([len(a) for a in arr])
-            return map(
-                lambda a: np.concatenate([a, np.full(max_len - len(a), np.nan)]), arr
-            )
+        # prtls = [
+        #     k
+        #     for k in self.file[step0].keys()
+        #     if (k.startswith("X") or k.startswith("U") or k.startswith("W"))
+        # ]
+
+        # species = np.unique(
+        #     [int(pq.split("_")[1]) for pq in self.file[step0].keys() if pq in prtls]
+        # )
+
+        # def list_to_ragged(arr):
+        #     max_len = np.max([len(a) for a in arr])
+        #     return map(
+        #         lambda a: np.concatenate([a, np.full(max_len - len(a), np.nan)]), arr
+        #     )
 
         self._particles = {}
-        for s in species:
-            prtl_data = {}
-            for q in [
-                f"X1_{s}",
-                f"X2_{s}",
-                f"X3_{s}",
-                f"U1_{s}",
-                f"U2_{s}",
-                f"U3_{s}",
-                f"W_{s}",
-            ]:
-                if q[0] in ["X", "U"]:
-                    q_ = PrtlDict[coordinates][q.split("_")[0]]
-                else:
-                    q_ = q.split("_")[0]
-                if q not in prtls:
-                    continue
-                if q not in prtl_data.keys():
-                    prtl_data[q_] = []
-                for k in range(nsteps):
-                    step_k = f"Step{k}"
-                    if q in self.file[step_k].keys():
-                        prtl_data[q_].append(self.file[step_k][q])
-                    else:
-                        prtl_data[q_].append(np.full_like(prtl_data[q_][-1], np.nan))
-                prtl_data[q_] = list_to_ragged(prtl_data[q_])
-                prtl_data[q_] = da.from_array(list(prtl_data[q_]))
-                prtl_data[q_] = xr.DataArray(
-                    prtl_data[q_], dims=["t", "id"], name=q_, coords={"t": times}
-                )
-            if coordinates == "spherical":
-                prtl_data["x"] = (
-                    prtl_data[PrtlDict[coordinates]["X1"]]
-                    * np.sin(prtl_data[PrtlDict[coordinates]["X2"]])
-                    * np.cos(prtl_data[PrtlDict[coordinates]["X3"]])
-                )
-                prtl_data["y"] = (
-                    prtl_data[PrtlDict[coordinates]["X1"]]
-                    * np.sin(prtl_data[PrtlDict[coordinates]["X2"]])
-                    * np.sin(prtl_data[PrtlDict[coordinates]["X3"]])
-                )
-                prtl_data["z"] = prtl_data[PrtlDict[coordinates]["X1"]] * np.cos(
-                    prtl_data[PrtlDict[coordinates]["X2"]]
-                )
-            self._particles[s] = xr.Dataset(prtl_data)
+        # for s in species:
+        #     prtl_data = {}
+        #     for q in [
+        #         f"X1_{s}",
+        #         f"X2_{s}",
+        #         f"X3_{s}",
+        #         f"U1_{s}",
+        #         f"U2_{s}",
+        #         f"U3_{s}",
+        #         f"W_{s}",
+        #     ]:
+        #         if q[0] in ["X", "U"]:
+        #             q_ = PrtlDict[coordinates][q.split("_")[0]]
+        #         else:
+        #             q_ = q.split("_")[0]
+        #         if q not in prtls:
+        #             continue
+        #         if q not in prtl_data.keys():
+        #             prtl_data[q_] = []
+        #         for k in range(nsteps):
+        #             step_k = f"Step{k}"
+        #             if q in self.file[step_k].keys():
+        #                 prtl_data[q_].append(self.file[step_k][q])
+        #             else:
+        #                 prtl_data[q_].append(np.full_like(prtl_data[q_][-1], np.nan))
+        #         prtl_data[q_] = list_to_ragged(prtl_data[q_])
+        #         prtl_data[q_] = da.from_array(list(prtl_data[q_]))
+        #         prtl_data[q_] = xr.DataArray(
+        #             prtl_data[q_], dims=["t", "id"], name=q_, coords={"t": times}
+        #         )
+        #     if coordinates == "spherical":
+        #         prtl_data["x"] = (
+        #             prtl_data[PrtlDict[coordinates]["X1"]]
+        #             * np.sin(prtl_data[PrtlDict[coordinates]["X2"]])
+        #             * np.cos(prtl_data[PrtlDict[coordinates]["X3"]])
+        #         )
+        #         prtl_data["y"] = (
+        #             prtl_data[PrtlDict[coordinates]["X1"]]
+        #             * np.sin(prtl_data[PrtlDict[coordinates]["X2"]])
+        #             * np.sin(prtl_data[PrtlDict[coordinates]["X3"]])
+        #         )
+        #         prtl_data["z"] = prtl_data[PrtlDict[coordinates]["X1"]] * np.cos(
+        #             prtl_data[PrtlDict[coordinates]["X2"]]
+        #         )
+        #     self._particles[s] = xr.Dataset(prtl_data)
 
     def __del__(self):
         self.file.close()
 
     def __getattr__(self, name):
         return getattr(self.dataset, name)
 
@@ -874,23 +875,23 @@
         import numpy as np
 
         if makeframes:
             makemovie = all(
                 exp.makeFrames(
                     plot,
                     np.arange(len(self.t)),
-                    f"{self.attrs['Title']}/frames",
+                    f"{self.attrs['simulation.name']}/frames",
                     data=self,
                     num_cpus=kwargs.pop("num_cpus", None),
                 )
             )
         else:
             makemovie = True
         if makemovie:
             exp.makeMovie(
-                input=f"{self.attrs['Title']}/frames/",
+                input=f"{self.attrs['simulation.name']}/frames/",
                 overwrite=True,
-                output=f"{self.attrs['Title']}.mp4",
+                output=f"{self.attrs['simulation.name']}.mp4",
                 number=5,
                 **kwargs,
             )
             return True
```

### Comparing `nt2py-0.2.1/requirements.txt` & `nt2py-0.3.0/requirements.txt`

 * *Files identical despite different names*


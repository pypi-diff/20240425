# Comparing `tmp/brainrender-2.1.7.tar.gz` & `tmp/brainrender-2.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brainrender-2.1.7.tar", last modified: Thu Apr 18 11:17:28 2024, max compression
+gzip compressed data, was "brainrender-2.1.8.tar", last modified: Thu Apr 25 10:58:19 2024, max compression
```

## Comparing `brainrender-2.1.7.tar` & `brainrender-2.1.8.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:17:28.396255 brainrender-2.1.7/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:17:28.380255 brainrender-2.1.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:17:28.380255 brainrender-2.1.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-04-18 11:17:22.000000 brainrender-2.1.7/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-04-18 11:17:22.000000 brainrender-2.1.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-04-18 11:17:22.000000 brainrender-2.1.7/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-04-18 11:17:22.000000 brainrender-2.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-18 11:17:22.000000 brainrender-2.1.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5894 2024-04-18 11:17:28.396255 brainrender-2.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3801 2024-04-18 11:17:22.000000 brainrender-2.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:17:28.384255 brainrender-2.1.7/brainrender/
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-04-18 11:17:22.000000 brainrender-2.1.7/brainrender/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-04-18 11:17:22.000000 brainrender-2.1.7/brainrender/_colors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-04-18 11:17:22.000000 brainrender-2.1.7/brainrender/_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-04-18 11:17:22.000000 brainrender-2.1.7/brainrender/_jupyter.py
--rw-r--r--   0 runner    (1001) docker     (127)      956 2024-04-18 11:17:22.000000 brainrender-2.1.7/brainrender/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-04-18 11:17:22.000000 brainrender-2.1.7/brainrender/_video.py
--rw-r--r--   0 runner    (1001) docker     (127)     7146 2024-04-18 11:17:22.000000 brainrender-2.1.7/brainrender/actor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:17:28.384255 brainrender-2.1.7/brainrender/actors/
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-18 11:17:22.000000 brainrender-2.1.7/brainrender/actors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-18 11:17:22.000000 brainrender-2.1.7/brainrender/actors/cylinder.py
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-18 11:17:22.000000 brainrender-2.1.7/brainrender/actors/line.py
--rw-r--r--   0 runner    (1001) docker     (127)     3118 2024-04-18 11:17:22.000000 brainrender-2.1.7/brainrender/actors/neurons.py
--rw-r--r--   0 runner    (1001) docker     (127)     5027 2024-04-18 11:17:22.000000 brainrender-2.1.7/brainrender/actors/points.py
--rw-r--r--   0 runner    (1001) docker     (127)     2443 2024-04-18 11:17:22.000000 brainrender-2.1.7/brainrender/actors/ruler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-04-18 11:17:22.000000 brainrender-2.1.7/brainrender/actors/streamlines.py
--rw-r--r--   0 runner    (1001) docker     (127)     3875 2024-04-18 11:17:22.000000 brainrender-2.1.7/brainrender/actors/volume.py
--rw-r--r--   0 runner    (1001) docker     (127)     5077 2024-04-18 11:17:22.000000 brainrender-2.1.7/brainrender/atlas.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:17:28.384255 brainrender-2.1.7/brainrender/atlas_specific/
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-18 11:17:22.000000 brainrender-2.1.7/brainrender/atlas_specific/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:17:28.384255 brainrender-2.1.7/brainrender/atlas_specific/allen_brain_atlas/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:17:28.388255 brainrender-2.1.7/brainrender/atlas_specific/allen_brain_atlas/gene_expression/
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-18 11:17:22.000000 brainrender-2.1.7/brainrender/atlas_specific/allen_brain_atlas/gene_expression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5921 2024-04-18 11:17:22.000000 brainrender-2.1.7/brainrender/atlas_specific/allen_brain_atlas/gene_expression/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-04-18 11:17:22.000000 brainrender-2.1.7/brainrender/atlas_specific/allen_brain_atlas/gene_expression/ge_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-04-18 11:17:22.000000 brainrender-2.1.7/brainrender/atlas_specific/allen_brain_atlas/streamlines.py
--rw-r--r--   0 runner    (1001) docker     (127)     3107 2024-04-18 11:17:22.000000 brainrender-2.1.7/brainrender/camera.py
--rw-r--r--   0 runner    (1001) docker     (127)      926 2024-04-18 11:17:22.000000 brainrender-2.1.7/brainrender/cameras.py
--rw-r--r--   0 runner    (1001) docker     (127)    12817 2024-04-18 11:17:22.000000 brainrender-2.1.7/brainrender/render.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:17:28.396255 brainrender-2.1.7/brainrender/resources/
--rw-r--r--   0 runner    (1001) docker     (127)  3474788 2024-04-18 11:17:22.000000 brainrender-2.1.7/brainrender/resources/CC_134_1_ch1inj.obj
--rw-r--r--   0 runner    (1001) docker     (127)  3117970 2024-04-18 11:17:22.000000 brainrender-2.1.7/brainrender/resources/CC_134_2_ch1inj.obj
--rw-r--r--   0 runner    (1001) docker     (127)   126927 2024-04-18 11:17:22.000000 brainrender-2.1.7/brainrender/resources/neuron1.swc
--rw-r--r--   0 runner    (1001) docker     (127)    46208 2024-04-18 11:17:22.000000 brainrender-2.1.7/brainrender/resources/probe_1_striatum.npy
--rw-r--r--   0 runner    (1001) docker     (127)    46208 2024-04-18 11:17:22.000000 brainrender-2.1.7/brainrender/resources/probe_2_RSP.npy
--rw-r--r--   0 runner    (1001) docker     (127)    24128 2024-04-18 11:17:22.000000 brainrender-2.1.7/brainrender/resources/random_cells.h5
--rw-r--r--   0 runner    (1001) docker     (127)    24128 2024-04-18 11:17:22.000000 brainrender-2.1.7/brainrender/resources/random_cells.npy
--rw-r--r--   0 runner    (1001) docker     (127)   637432 2024-04-18 11:17:22.000000 brainrender-2.1.7/brainrender/resources/volume.npy
--rw-r--r--   0 runner    (1001) docker     (127)    14186 2024-04-18 11:17:22.000000 brainrender-2.1.7/brainrender/scene.py
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-04-18 11:17:22.000000 brainrender-2.1.7/brainrender/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)    13755 2024-04-18 11:17:22.000000 brainrender-2.1.7/brainrender/video.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:17:28.396255 brainrender-2.1.7/brainrender.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5894 2024-04-18 11:17:28.000000 brainrender-2.1.7/brainrender.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-04-18 11:17:28.000000 brainrender-2.1.7/brainrender.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 11:17:28.000000 brainrender-2.1.7/brainrender.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-18 11:17:28.000000 brainrender-2.1.7/brainrender.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-18 11:17:28.000000 brainrender-2.1.7/brainrender.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2988 2024-04-18 11:17:22.000000 brainrender-2.1.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 11:17:28.396255 brainrender-2.1.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:58:19.361909 brainrender-2.1.8/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:58:19.341909 brainrender-2.1.8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:58:19.341909 brainrender-2.1.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2135 2024-04-25 10:58:15.000000 brainrender-2.1.8/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-04-25 10:58:15.000000 brainrender-2.1.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-04-25 10:58:15.000000 brainrender-2.1.8/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-04-25 10:58:15.000000 brainrender-2.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-25 10:58:15.000000 brainrender-2.1.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6005 2024-04-25 10:58:19.361909 brainrender-2.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3912 2024-04-25 10:58:15.000000 brainrender-2.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:58:19.345908 brainrender-2.1.8/brainrender/
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-04-25 10:58:15.000000 brainrender-2.1.8/brainrender/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-04-25 10:58:15.000000 brainrender-2.1.8/brainrender/_colors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-04-25 10:58:15.000000 brainrender-2.1.8/brainrender/_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-04-25 10:58:15.000000 brainrender-2.1.8/brainrender/_jupyter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      956 2024-04-25 10:58:15.000000 brainrender-2.1.8/brainrender/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-04-25 10:58:15.000000 brainrender-2.1.8/brainrender/_video.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7146 2024-04-25 10:58:15.000000 brainrender-2.1.8/brainrender/actor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:58:19.349908 brainrender-2.1.8/brainrender/actors/
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-25 10:58:15.000000 brainrender-2.1.8/brainrender/actors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-25 10:58:15.000000 brainrender-2.1.8/brainrender/actors/cylinder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-25 10:58:15.000000 brainrender-2.1.8/brainrender/actors/line.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3118 2024-04-25 10:58:15.000000 brainrender-2.1.8/brainrender/actors/neurons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5027 2024-04-25 10:58:15.000000 brainrender-2.1.8/brainrender/actors/points.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2443 2024-04-25 10:58:15.000000 brainrender-2.1.8/brainrender/actors/ruler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-04-25 10:58:15.000000 brainrender-2.1.8/brainrender/actors/streamlines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3875 2024-04-25 10:58:15.000000 brainrender-2.1.8/brainrender/actors/volume.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5077 2024-04-25 10:58:15.000000 brainrender-2.1.8/brainrender/atlas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:58:19.349908 brainrender-2.1.8/brainrender/atlas_specific/
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-25 10:58:15.000000 brainrender-2.1.8/brainrender/atlas_specific/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:58:19.349908 brainrender-2.1.8/brainrender/atlas_specific/allen_brain_atlas/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:58:19.349908 brainrender-2.1.8/brainrender/atlas_specific/allen_brain_atlas/gene_expression/
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-25 10:58:15.000000 brainrender-2.1.8/brainrender/atlas_specific/allen_brain_atlas/gene_expression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5921 2024-04-25 10:58:15.000000 brainrender-2.1.8/brainrender/atlas_specific/allen_brain_atlas/gene_expression/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-04-25 10:58:15.000000 brainrender-2.1.8/brainrender/atlas_specific/allen_brain_atlas/gene_expression/ge_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-04-25 10:58:15.000000 brainrender-2.1.8/brainrender/atlas_specific/allen_brain_atlas/streamlines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3107 2024-04-25 10:58:15.000000 brainrender-2.1.8/brainrender/camera.py
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-04-25 10:58:15.000000 brainrender-2.1.8/brainrender/cameras.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12962 2024-04-25 10:58:15.000000 brainrender-2.1.8/brainrender/render.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:58:19.357909 brainrender-2.1.8/brainrender/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)  3474788 2024-04-25 10:58:15.000000 brainrender-2.1.8/brainrender/resources/CC_134_1_ch1inj.obj
+-rw-r--r--   0 runner    (1001) docker     (127)  3117970 2024-04-25 10:58:15.000000 brainrender-2.1.8/brainrender/resources/CC_134_2_ch1inj.obj
+-rw-r--r--   0 runner    (1001) docker     (127)   126927 2024-04-25 10:58:15.000000 brainrender-2.1.8/brainrender/resources/neuron1.swc
+-rw-r--r--   0 runner    (1001) docker     (127)    46208 2024-04-25 10:58:15.000000 brainrender-2.1.8/brainrender/resources/probe_1_striatum.npy
+-rw-r--r--   0 runner    (1001) docker     (127)    46208 2024-04-25 10:58:15.000000 brainrender-2.1.8/brainrender/resources/probe_2_RSP.npy
+-rw-r--r--   0 runner    (1001) docker     (127)    24128 2024-04-25 10:58:15.000000 brainrender-2.1.8/brainrender/resources/random_cells.h5
+-rw-r--r--   0 runner    (1001) docker     (127)    24128 2024-04-25 10:58:15.000000 brainrender-2.1.8/brainrender/resources/random_cells.npy
+-rw-r--r--   0 runner    (1001) docker     (127)   637432 2024-04-25 10:58:15.000000 brainrender-2.1.8/brainrender/resources/volume.npy
+-rw-r--r--   0 runner    (1001) docker     (127)    14186 2024-04-25 10:58:15.000000 brainrender-2.1.8/brainrender/scene.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-04-25 10:58:15.000000 brainrender-2.1.8/brainrender/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13755 2024-04-25 10:58:15.000000 brainrender-2.1.8/brainrender/video.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:58:19.357909 brainrender-2.1.8/brainrender.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6005 2024-04-25 10:58:19.000000 brainrender-2.1.8/brainrender.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-04-25 10:58:19.000000 brainrender-2.1.8/brainrender.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 10:58:19.000000 brainrender-2.1.8/brainrender.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-25 10:58:19.000000 brainrender-2.1.8/brainrender.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-25 10:58:19.000000 brainrender-2.1.8/brainrender.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2988 2024-04-25 10:58:15.000000 brainrender-2.1.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 10:58:19.361909 brainrender-2.1.8/setup.cfg
```

### Comparing `brainrender-2.1.7/.github/workflows/test_and_deploy.yml` & `brainrender-2.1.8/.github/workflows/test_and_deploy.yml`

 * *Files 9% similar despite different names*

```diff
@@ -57,14 +57,15 @@
       - uses: FedericoCarboni/setup-ffmpeg@v2
         id: setup-ffmpeg
 
       # Run tests
       - uses: neuroinformatics-unit/actions/test@v2
         with:
           python-version: ${{ matrix.python-version }}
+          secret-codecov-token: ${{ secrets.CODECOV_TOKEN }}
 
   build_sdist_wheels:
     name: Build source distribution
     needs: [test]
     if: github.event_name == 'push' && github.ref_type == 'tag'
     runs-on: ubuntu-latest
     steps:
```

### Comparing `brainrender-2.1.7/.gitignore` & `brainrender-2.1.8/.gitignore`

 * *Files identical despite different names*

### Comparing `brainrender-2.1.7/CITATION.cff` & `brainrender-2.1.8/CITATION.cff`

 * *Files identical despite different names*

### Comparing `brainrender-2.1.7/LICENSE` & `brainrender-2.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `brainrender-2.1.7/brainrender/__init__.py` & `brainrender-2.1.8/brainrender/__init__.py`

 * *Files identical despite different names*

### Comparing `brainrender-2.1.7/brainrender/_colors.py` & `brainrender-2.1.8/brainrender/_colors.py`

 * *Files identical despite different names*

### Comparing `brainrender-2.1.7/brainrender/_io.py` & `brainrender-2.1.8/brainrender/_io.py`

 * *Files identical despite different names*

### Comparing `brainrender-2.1.7/brainrender/_jupyter.py` & `brainrender-2.1.8/brainrender/_jupyter.py`

 * *Files identical despite different names*

### Comparing `brainrender-2.1.7/brainrender/_utils.py` & `brainrender-2.1.8/brainrender/_utils.py`

 * *Files identical despite different names*

### Comparing `brainrender-2.1.7/brainrender/_video.py` & `brainrender-2.1.8/brainrender/_video.py`

 * *Files identical despite different names*

### Comparing `brainrender-2.1.7/brainrender/actor.py` & `brainrender-2.1.8/brainrender/actor.py`

 * *Files identical despite different names*

### Comparing `brainrender-2.1.7/brainrender/actors/cylinder.py` & `brainrender-2.1.8/brainrender/actors/cylinder.py`

 * *Files identical despite different names*

### Comparing `brainrender-2.1.7/brainrender/actors/line.py` & `brainrender-2.1.8/brainrender/actors/line.py`

 * *Files identical despite different names*

### Comparing `brainrender-2.1.7/brainrender/actors/neurons.py` & `brainrender-2.1.8/brainrender/actors/neurons.py`

 * *Files identical despite different names*

### Comparing `brainrender-2.1.7/brainrender/actors/points.py` & `brainrender-2.1.8/brainrender/actors/points.py`

 * *Files identical despite different names*

### Comparing `brainrender-2.1.7/brainrender/actors/ruler.py` & `brainrender-2.1.8/brainrender/actors/ruler.py`

 * *Files identical despite different names*

### Comparing `brainrender-2.1.7/brainrender/actors/streamlines.py` & `brainrender-2.1.8/brainrender/actors/streamlines.py`

 * *Files identical despite different names*

### Comparing `brainrender-2.1.7/brainrender/actors/volume.py` & `brainrender-2.1.8/brainrender/actors/volume.py`

 * *Files identical despite different names*

### Comparing `brainrender-2.1.7/brainrender/atlas.py` & `brainrender-2.1.8/brainrender/atlas.py`

 * *Files identical despite different names*

### Comparing `brainrender-2.1.7/brainrender/atlas_specific/allen_brain_atlas/gene_expression/api.py` & `brainrender-2.1.8/brainrender/atlas_specific/allen_brain_atlas/gene_expression/api.py`

 * *Files identical despite different names*

### Comparing `brainrender-2.1.7/brainrender/atlas_specific/allen_brain_atlas/gene_expression/ge_utils.py` & `brainrender-2.1.8/brainrender/atlas_specific/allen_brain_atlas/gene_expression/ge_utils.py`

 * *Files identical despite different names*

### Comparing `brainrender-2.1.7/brainrender/atlas_specific/allen_brain_atlas/streamlines.py` & `brainrender-2.1.8/brainrender/atlas_specific/allen_brain_atlas/streamlines.py`

 * *Files identical despite different names*

### Comparing `brainrender-2.1.7/brainrender/camera.py` & `brainrender-2.1.8/brainrender/camera.py`

 * *Files identical despite different names*

### Comparing `brainrender-2.1.7/brainrender/cameras.py` & `brainrender-2.1.8/brainrender/cameras.py`

 * *Files identical despite different names*

### Comparing `brainrender-2.1.7/brainrender/render.py` & `brainrender-2.1.8/brainrender/render.py`

 * *Files 4% similar despite different names*

```diff
@@ -343,17 +343,19 @@
         :param scale: float, >1 for higher resolution
         """
 
         if not self.is_rendered:
             self.render(interactive=False)
 
         timestamp = datetime.now().strftime("%Y%m%d_%H%M%S")
-        name = name or f"brainrender_screenshot_{timestamp}"
-        if ".png" not in name:
-            name += ".png"
+        name = Path(name or f"brainrender_screenshot_{timestamp}")
+
+        # If no suffix is provided or it an unsupported format, default to .png
+        if name.suffix not in [".png", ".eps", ".pdf", ".svg", ".jpg"]:
+            name = name.with_suffix(".png")
 
         scale = scale or settings.SCREENSHOT_SCALE
 
         print(f"\nSaving new screenshot at {name}\n")
 
         savepath = str(self.screenshots_folder / name)
         logger.debug(f"Saving scene at {savepath}")
```

### Comparing `brainrender-2.1.7/brainrender/resources/CC_134_1_ch1inj.obj` & `brainrender-2.1.8/brainrender/resources/CC_134_1_ch1inj.obj`

 * *Files identical despite different names*

### Comparing `brainrender-2.1.7/brainrender/resources/CC_134_2_ch1inj.obj` & `brainrender-2.1.8/brainrender/resources/CC_134_2_ch1inj.obj`

 * *Files identical despite different names*

### Comparing `brainrender-2.1.7/brainrender/resources/neuron1.swc` & `brainrender-2.1.8/brainrender/resources/neuron1.swc`

 * *Files identical despite different names*

### Comparing `brainrender-2.1.7/brainrender/resources/probe_1_striatum.npy` & `brainrender-2.1.8/brainrender/resources/probe_1_striatum.npy`

 * *Files identical despite different names*

### Comparing `brainrender-2.1.7/brainrender/resources/probe_2_RSP.npy` & `brainrender-2.1.8/brainrender/resources/probe_2_RSP.npy`

 * *Files identical despite different names*

### Comparing `brainrender-2.1.7/brainrender/resources/random_cells.h5` & `brainrender-2.1.8/brainrender/resources/random_cells.h5`

 * *Files identical despite different names*

### Comparing `brainrender-2.1.7/brainrender/resources/random_cells.npy` & `brainrender-2.1.8/brainrender/resources/random_cells.npy`

 * *Files identical despite different names*

### Comparing `brainrender-2.1.7/brainrender/resources/volume.npy` & `brainrender-2.1.8/brainrender/resources/volume.npy`

 * *Files identical despite different names*

### Comparing `brainrender-2.1.7/brainrender/scene.py` & `brainrender-2.1.8/brainrender/scene.py`

 * *Files identical despite different names*

### Comparing `brainrender-2.1.7/brainrender/settings.py` & `brainrender-2.1.8/brainrender/settings.py`

 * *Files identical despite different names*

### Comparing `brainrender-2.1.7/brainrender/video.py` & `brainrender-2.1.8/brainrender/video.py`

 * *Files identical despite different names*

### Comparing `brainrender-2.1.7/brainrender.egg-info/SOURCES.txt` & `brainrender-2.1.8/brainrender.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `brainrender-2.1.7/pyproject.toml` & `brainrender-2.1.8/pyproject.toml`

 * *Files identical despite different names*


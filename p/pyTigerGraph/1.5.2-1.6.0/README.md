# Comparing `tmp/pyTigerGraph-1.5.2.tar.gz` & `tmp/pytigergraph-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyTigerGraph-1.5.2.tar", last modified: Thu Feb 15 19:41:12 2024, max compression
+gzip compressed data, was "pytigergraph-1.6.0.tar", last modified: Thu Apr 25 17:49:47 2024, max compression
```

## Comparing `pyTigerGraph-1.5.2.tar` & `pytigergraph-1.6.0.tar`

### file list

```diff
@@ -1,115 +1,115 @@
-drwxr-xr-x   0 parkererickson   (502) staff       (20)        0 2024-02-15 19:41:12.006832 pyTigerGraph-1.5.2/
--rw-r--r--   0 parkererickson   (502) staff       (20)     3880 2024-02-15 19:41:12.006205 pyTigerGraph-1.5.2/PKG-INFO
--rw-r--r--   0 parkererickson   (502) staff       (20)     2520 2023-09-12 17:29:53.000000 pyTigerGraph-1.5.2/README.md
-drwxr-xr-x   0 parkererickson   (502) staff       (20)        0 2024-02-15 19:41:11.922514 pyTigerGraph-1.5.2/pyTigerGraph/
--rw-r--r--   0 parkererickson   (502) staff       (20)      108 2024-02-15 19:40:45.000000 pyTigerGraph-1.5.2/pyTigerGraph/__init__.py
-drwxr-xr-x   0 parkererickson   (502) staff       (20)        0 2024-02-15 19:41:11.924628 pyTigerGraph-1.5.2/pyTigerGraph/ai/
--rw-r--r--   0 parkererickson   (502) staff       (20)        0 2024-02-15 19:40:45.000000 pyTigerGraph-1.5.2/pyTigerGraph/ai/__init__.py
--rw-r--r--   0 parkererickson   (502) staff       (20)     3036 2024-02-15 19:40:45.000000 pyTigerGraph-1.5.2/pyTigerGraph/ai/ai.py
--rw-r--r--   0 parkererickson   (502) staff       (20)     5533 2023-09-20 21:20:42.000000 pyTigerGraph-1.5.2/pyTigerGraph/datasets.py
-drwxr-xr-x   0 parkererickson   (502) staff       (20)        0 2024-02-15 19:41:11.935234 pyTigerGraph-1.5.2/pyTigerGraph/gds/
--rw-r--r--   0 parkererickson   (502) staff       (20)      211 2023-05-19 15:14:44.000000 pyTigerGraph-1.5.2/pyTigerGraph/gds/__init__.py
-drwxr-xr-x   0 parkererickson   (502) staff       (20)        0 2024-02-15 19:41:11.947184 pyTigerGraph-1.5.2/pyTigerGraph/gds/__pycache__/
--rw-r--r--   0 parkererickson   (502) staff       (20)      398 2023-04-27 20:50:55.000000 pyTigerGraph-1.5.2/pyTigerGraph/gds/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 parkererickson   (502) staff       (20)    96874 2023-04-28 00:26:42.000000 pyTigerGraph-1.5.2/pyTigerGraph/gds/__pycache__/dataloaders.cpython-39.pyc
--rw-r--r--   0 parkererickson   (502) staff       (20)    19922 2023-01-13 15:10:11.000000 pyTigerGraph-1.5.2/pyTigerGraph/gds/__pycache__/featurizer.cpython-39.pyc
--rw-r--r--   0 parkererickson   (502) staff       (20)    51764 2023-01-13 15:10:10.000000 pyTigerGraph-1.5.2/pyTigerGraph/gds/__pycache__/gds.cpython-39.pyc
--rw-r--r--   0 parkererickson   (502) staff       (20)    19285 2023-04-28 00:26:42.000000 pyTigerGraph-1.5.2/pyTigerGraph/gds/__pycache__/metrics.cpython-39.pyc
--rw-r--r--   0 parkererickson   (502) staff       (20)     9232 2023-01-13 15:10:11.000000 pyTigerGraph-1.5.2/pyTigerGraph/gds/__pycache__/splitters.cpython-39.pyc
--rw-r--r--   0 parkererickson   (502) staff       (20)     9288 2023-04-28 00:26:42.000000 pyTigerGraph-1.5.2/pyTigerGraph/gds/__pycache__/trainer.cpython-39.pyc
--rw-r--r--   0 parkererickson   (502) staff       (20)     5470 2023-04-28 00:26:42.000000 pyTigerGraph-1.5.2/pyTigerGraph/gds/__pycache__/utilities.cpython-39.pyc
--rw-r--r--   0 parkererickson   (502) staff       (20)   190405 2023-09-12 17:29:53.000000 pyTigerGraph-1.5.2/pyTigerGraph/gds/dataloaders.py
--rw-r--r--   0 parkererickson   (502) staff       (20)    34967 2023-09-20 14:11:13.000000 pyTigerGraph-1.5.2/pyTigerGraph/gds/featurizer.py
--rw-r--r--   0 parkererickson   (502) staff       (20)    91456 2023-09-12 17:29:53.000000 pyTigerGraph-1.5.2/pyTigerGraph/gds/gds.py
-drwxr-xr-x   0 parkererickson   (502) staff       (20)        0 2024-02-15 19:41:11.879928 pyTigerGraph-1.5.2/pyTigerGraph/gds/gsql/
-drwxr-xr-x   0 parkererickson   (502) staff       (20)        0 2024-02-15 19:41:11.951811 pyTigerGraph-1.5.2/pyTigerGraph/gds/gsql/dataloaders/
--rw-r--r--   0 parkererickson   (502) staff       (20)    10792 2023-09-12 17:29:53.000000 pyTigerGraph-1.5.2/pyTigerGraph/gds/gsql/dataloaders/edge_loader.gsql
--rw-r--r--   0 parkererickson   (502) staff       (20)    12302 2023-09-12 17:29:53.000000 pyTigerGraph-1.5.2/pyTigerGraph/gds/gsql/dataloaders/edge_nei_loader.gsql
--rw-r--r--   0 parkererickson   (502) staff       (20)      242 2023-05-19 19:02:11.000000 pyTigerGraph-1.5.2/pyTigerGraph/gds/gsql/dataloaders/get_anchors.gsql
--rw-r--r--   0 parkererickson   (502) staff       (20)     5048 2023-05-19 19:02:11.000000 pyTigerGraph-1.5.2/pyTigerGraph/gds/gsql/dataloaders/graph_loader.gsql
--rw-r--r--   0 parkererickson   (502) staff       (20)     7804 2023-05-19 19:02:11.000000 pyTigerGraph-1.5.2/pyTigerGraph/gds/gsql/dataloaders/hgt_loader.gsql
--rw-r--r--   0 parkererickson   (502) staff       (20)     8364 2023-05-19 19:02:11.000000 pyTigerGraph-1.5.2/pyTigerGraph/gds/gsql/dataloaders/neighbor_loader.gsql
--rw-r--r--   0 parkererickson   (502) staff       (20)     8697 2023-05-19 19:02:11.000000 pyTigerGraph-1.5.2/pyTigerGraph/gds/gsql/dataloaders/nodepiece_loader.gsql
--rw-r--r--   0 parkererickson   (502) staff       (20)     5929 2023-05-19 19:02:11.000000 pyTigerGraph-1.5.2/pyTigerGraph/gds/gsql/dataloaders/vertex_loader.gsql
-drwxr-xr-x   0 parkererickson   (502) staff       (20)        0 2024-02-15 19:41:11.953289 pyTigerGraph-1.5.2/pyTigerGraph/gds/gsql/splitters/
--rw-r--r--   0 parkererickson   (502) staff       (20)     1546 2023-04-24 16:45:07.000000 pyTigerGraph-1.5.2/pyTigerGraph/gds/gsql/splitters/random_anchor_selection.gsql
--rw-r--r--   0 parkererickson   (502) staff       (20)     2727 2023-05-03 19:52:07.000000 pyTigerGraph-1.5.2/pyTigerGraph/gds/gsql/splitters/random_edge_split.gsql
--rw-r--r--   0 parkererickson   (502) staff       (20)     2715 2023-05-03 19:52:07.000000 pyTigerGraph-1.5.2/pyTigerGraph/gds/gsql/splitters/random_vertex_split.gsql
--rw-r--r--   0 parkererickson   (502) staff       (20)    22448 2023-05-19 19:02:11.000000 pyTigerGraph-1.5.2/pyTigerGraph/gds/metrics.py
-drwxr-xr-x   0 parkererickson   (502) staff       (20)        0 2024-02-15 19:41:11.957575 pyTigerGraph-1.5.2/pyTigerGraph/gds/models/
--rw-r--r--   0 parkererickson   (502) staff       (20)    13081 2023-05-19 19:02:11.000000 pyTigerGraph-1.5.2/pyTigerGraph/gds/models/GraphSAGE.py
--rw-r--r--   0 parkererickson   (502) staff       (20)     5949 2023-05-19 19:02:11.000000 pyTigerGraph-1.5.2/pyTigerGraph/gds/models/NodePieceMLP.py
--rw-r--r--   0 parkererickson   (502) staff       (20)       50 2023-05-19 19:02:11.000000 pyTigerGraph-1.5.2/pyTigerGraph/gds/models/__init__.py
-drwxr-xr-x   0 parkererickson   (502) staff       (20)        0 2024-02-15 19:41:11.961205 pyTigerGraph-1.5.2/pyTigerGraph/gds/models/__pycache__/
--rw-r--r--   0 parkererickson   (502) staff       (20)     6025 2023-04-28 00:32:54.000000 pyTigerGraph-1.5.2/pyTigerGraph/gds/models/__pycache__/GraphSAGE.cpython-39.pyc
--rw-r--r--   0 parkererickson   (502) staff       (20)     3741 2023-04-28 00:26:44.000000 pyTigerGraph-1.5.2/pyTigerGraph/gds/models/__pycache__/NodePieceMLP.cpython-39.pyc
--rw-r--r--   0 parkererickson   (502) staff       (20)      230 2023-04-28 00:26:42.000000 pyTigerGraph-1.5.2/pyTigerGraph/gds/models/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 parkererickson   (502) staff       (20)     1807 2023-04-28 00:26:42.000000 pyTigerGraph-1.5.2/pyTigerGraph/gds/models/__pycache__/base_model.cpython-39.pyc
--rw-r--r--   0 parkererickson   (502) staff       (20)     1286 2023-05-19 19:02:11.000000 pyTigerGraph-1.5.2/pyTigerGraph/gds/models/base_model.py
--rw-r--r--   0 parkererickson   (502) staff       (20)     9661 2023-01-09 15:28:36.000000 pyTigerGraph-1.5.2/pyTigerGraph/gds/splitters.py
--rw-r--r--   0 parkererickson   (502) staff       (20)    17904 2023-06-08 21:32:52.000000 pyTigerGraph-1.5.2/pyTigerGraph/gds/trainer.py
-drwxr-xr-x   0 parkererickson   (502) staff       (20)        0 2024-02-15 19:41:11.962594 pyTigerGraph-1.5.2/pyTigerGraph/gds/transforms/
--rw-r--r--   0 parkererickson   (502) staff       (20)        0 2023-05-03 19:52:07.000000 pyTigerGraph-1.5.2/pyTigerGraph/gds/transforms/__init__.py
-drwxr-xr-x   0 parkererickson   (502) staff       (20)        0 2024-02-15 19:41:11.963782 pyTigerGraph-1.5.2/pyTigerGraph/gds/transforms/__pycache__/
--rw-r--r--   0 parkererickson   (502) staff       (20)      165 2023-04-27 20:50:55.000000 pyTigerGraph-1.5.2/pyTigerGraph/gds/transforms/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 parkererickson   (502) staff       (20)     8138 2023-04-27 20:50:55.000000 pyTigerGraph-1.5.2/pyTigerGraph/gds/transforms/__pycache__/pyg_transforms.cpython-39.pyc
--rw-r--r--   0 parkererickson   (502) staff       (20)     2158 2023-05-19 19:02:11.000000 pyTigerGraph-1.5.2/pyTigerGraph/gds/transforms/nodepiece_transforms.py
--rw-r--r--   0 parkererickson   (502) staff       (20)     9955 2023-05-19 19:02:11.000000 pyTigerGraph-1.5.2/pyTigerGraph/gds/transforms/pyg_transforms.py
--rw-r--r--   0 parkererickson   (502) staff       (20)     9349 2023-09-12 17:29:53.000000 pyTigerGraph-1.5.2/pyTigerGraph/gds/utilities.py
--rw-r--r--   0 parkererickson   (502) staff       (20)     2887 2024-02-15 19:40:45.000000 pyTigerGraph-1.5.2/pyTigerGraph/pyTigerGraph.py
--rw-r--r--   0 parkererickson   (502) staff       (20)    18422 2024-02-15 19:40:45.000000 pyTigerGraph-1.5.2/pyTigerGraph/pyTigerGraphAuth.py
--rw-r--r--   0 parkererickson   (502) staff       (20)    16915 2023-09-12 17:29:53.000000 pyTigerGraph-1.5.2/pyTigerGraph/pyTigerGraphBase.py
--rw-r--r--   0 parkererickson   (502) staff       (20)     3910 2022-12-07 20:53:19.000000 pyTigerGraph-1.5.2/pyTigerGraph/pyTigerGraphDataset.py
--rw-r--r--   0 parkererickson   (502) staff       (20)    47508 2024-02-13 21:15:02.000000 pyTigerGraph-1.5.2/pyTigerGraph/pyTigerGraphEdge.py
--rw-r--r--   0 parkererickson   (502) staff       (20)      265 2022-04-21 16:09:16.000000 pyTigerGraph-1.5.2/pyTigerGraph/pyTigerGraphException.py
--rw-r--r--   0 parkererickson   (502) staff       (20)     8184 2023-09-12 17:29:53.000000 pyTigerGraph-1.5.2/pyTigerGraph/pyTigerGraphGSQL.py
--rw-r--r--   0 parkererickson   (502) staff       (20)     3631 2022-11-02 21:02:01.000000 pyTigerGraph-1.5.2/pyTigerGraph/pyTigerGraphLoading.py
--rw-r--r--   0 parkererickson   (502) staff       (20)    11419 2022-11-02 21:02:01.000000 pyTigerGraph-1.5.2/pyTigerGraph/pyTigerGraphPath.py
--rw-r--r--   0 parkererickson   (502) staff       (20)    26454 2023-05-03 19:52:07.000000 pyTigerGraph-1.5.2/pyTigerGraph/pyTigerGraphQuery.py
--rw-r--r--   0 parkererickson   (502) staff       (20)     9312 2023-12-11 22:02:16.000000 pyTigerGraph-1.5.2/pyTigerGraph/pyTigerGraphSchema.py
--rw-r--r--   0 parkererickson   (502) staff       (20)     2184 2022-11-02 21:02:01.000000 pyTigerGraph-1.5.2/pyTigerGraph/pyTigerGraphUDT.py
--rw-r--r--   0 parkererickson   (502) staff       (20)    12154 2023-05-19 19:02:11.000000 pyTigerGraph-1.5.2/pyTigerGraph/pyTigerGraphUtils.py
--rw-r--r--   0 parkererickson   (502) staff       (20)    32833 2023-04-24 16:45:07.000000 pyTigerGraph-1.5.2/pyTigerGraph/pyTigerGraphVertex.py
--rw-r--r--   0 parkererickson   (502) staff       (20)    29259 2024-02-05 14:47:15.000000 pyTigerGraph-1.5.2/pyTigerGraph/schema.py
--rw-r--r--   0 parkererickson   (502) staff       (20)     3930 2022-11-15 18:52:57.000000 pyTigerGraph-1.5.2/pyTigerGraph/visualization.py
-drwxr-xr-x   0 parkererickson   (502) staff       (20)        0 2024-02-15 19:41:12.002582 pyTigerGraph-1.5.2/pyTigerGraph.egg-info/
--rw-r--r--   0 parkererickson   (502) staff       (20)     3880 2024-02-15 19:41:11.000000 pyTigerGraph-1.5.2/pyTigerGraph.egg-info/PKG-INFO
--rw-r--r--   0 parkererickson   (502) staff       (20)     3670 2024-02-15 19:41:11.000000 pyTigerGraph-1.5.2/pyTigerGraph.egg-info/SOURCES.txt
--rw-r--r--   0 parkererickson   (502) staff       (20)        1 2024-02-15 19:41:11.000000 pyTigerGraph-1.5.2/pyTigerGraph.egg-info/dependency_links.txt
--rw-r--r--   0 parkererickson   (502) staff       (20)       58 2024-02-15 19:41:11.000000 pyTigerGraph-1.5.2/pyTigerGraph.egg-info/requires.txt
--rw-r--r--   0 parkererickson   (502) staff       (20)       19 2024-02-15 19:41:11.000000 pyTigerGraph-1.5.2/pyTigerGraph.egg-info/top_level.txt
--rw-r--r--   0 parkererickson   (502) staff       (20)      229 2022-04-20 17:25:11.000000 pyTigerGraph-1.5.2/pyproject.toml
--rw-r--r--   0 parkererickson   (502) staff       (20)       78 2024-02-15 19:41:12.007575 pyTigerGraph-1.5.2/setup.cfg
--rw-r--r--   0 parkererickson   (502) staff       (20)     2548 2023-09-20 14:11:41.000000 pyTigerGraph-1.5.2/setup.py
-drwxr-xr-x   0 parkererickson   (502) staff       (20)        0 2024-02-15 19:41:12.001712 pyTigerGraph-1.5.2/tests/
--rw-r--r--   0 parkererickson   (502) staff       (20)        0 2022-04-20 17:25:11.000000 pyTigerGraph-1.5.2/tests/__init__.py
--rw-r--r--   0 parkererickson   (502) staff       (20)     1481 2022-12-12 17:45:12.000000 pyTigerGraph-1.5.2/tests/pyTigerGraphUnitTest.py
--rw-r--r--   0 parkererickson   (502) staff       (20)     6728 2023-09-12 17:29:58.000000 pyTigerGraph-1.5.2/tests/test_OGM.py
--rw-r--r--   0 parkererickson   (502) staff       (20)     2037 2022-12-07 20:53:19.000000 pyTigerGraph-1.5.2/tests/test_datasets.py
--rw-r--r--   0 parkererickson   (502) staff       (20)    33173 2023-09-12 17:29:53.000000 pyTigerGraph-1.5.2/tests/test_gds_BaseLoader.py
--rw-r--r--   0 parkererickson   (502) staff       (20)    10755 2023-09-12 17:29:53.000000 pyTigerGraph-1.5.2/tests/test_gds_EdgeLoader.py
--rw-r--r--   0 parkererickson   (502) staff       (20)     5677 2022-12-12 17:45:12.000000 pyTigerGraph-1.5.2/tests/test_gds_EdgeNeighborLoader.py
--rw-r--r--   0 parkererickson   (502) staff       (20)     7448 2023-05-03 19:52:07.000000 pyTigerGraph-1.5.2/tests/test_gds_GDS.py
--rw-r--r--   0 parkererickson   (502) staff       (20)    17297 2022-12-12 17:59:45.000000 pyTigerGraph-1.5.2/tests/test_gds_GraphLoader.py
--rw-r--r--   0 parkererickson   (502) staff       (20)     4700 2023-05-19 19:02:11.000000 pyTigerGraph-1.5.2/tests/test_gds_GraphSAGE.py
--rw-r--r--   0 parkererickson   (502) staff       (20)     7362 2023-02-16 15:58:12.000000 pyTigerGraph-1.5.2/tests/test_gds_HGTLoader.py
--rw-r--r--   0 parkererickson   (502) staff       (20)    33875 2023-05-03 19:52:07.000000 pyTigerGraph-1.5.2/tests/test_gds_NeighborLoader.py
--rw-r--r--   0 parkererickson   (502) staff       (20)     3443 2023-05-19 19:02:11.000000 pyTigerGraph-1.5.2/tests/test_gds_NodePiece.py
--rw-r--r--   0 parkererickson   (502) staff       (20)    11380 2023-04-21 18:31:54.000000 pyTigerGraph-1.5.2/tests/test_gds_NodePieceLoader.py
--rw-r--r--   0 parkererickson   (502) staff       (20)     4190 2023-05-03 19:52:07.000000 pyTigerGraph-1.5.2/tests/test_gds_Trainer.py
--rw-r--r--   0 parkererickson   (502) staff       (20)    11773 2023-02-16 15:58:12.000000 pyTigerGraph-1.5.2/tests/test_gds_VertexLoader.py
--rw-r--r--   0 parkererickson   (502) staff       (20)    14864 2023-02-16 15:58:12.000000 pyTigerGraph-1.5.2/tests/test_gds_featurizer.py
--rw-r--r--   0 parkererickson   (502) staff       (20)     7436 2023-05-03 19:52:07.000000 pyTigerGraph-1.5.2/tests/test_gds_metrics.py
--rw-r--r--   0 parkererickson   (502) staff       (20)     8349 2023-01-09 15:28:36.000000 pyTigerGraph-1.5.2/tests/test_gds_splitters.py
--rw-r--r--   0 parkererickson   (502) staff       (20)     5404 2023-05-03 19:52:07.000000 pyTigerGraph-1.5.2/tests/test_gds_transforms.py
--rw-r--r--   0 parkererickson   (502) staff       (20)     2498 2023-05-03 19:52:07.000000 pyTigerGraph-1.5.2/tests/test_gds_utilities.py
--rw-r--r--   0 parkererickson   (502) staff       (20)     2847 2022-12-12 17:45:12.000000 pyTigerGraph-1.5.2/tests/test_pyTigerGraphAuth.py
--rw-r--r--   0 parkererickson   (502) staff       (20)     2860 2022-12-12 17:45:12.000000 pyTigerGraph-1.5.2/tests/test_pyTigerGraphBase.py
--rw-r--r--   0 parkererickson   (502) staff       (20)    14229 2023-02-20 22:23:49.000000 pyTigerGraph-1.5.2/tests/test_pyTigerGraphEdge.py
--rw-r--r--   0 parkererickson   (502) staff       (20)     2300 2023-05-19 19:02:11.000000 pyTigerGraph-1.5.2/tests/test_pyTigerGraphGSQL.py
--rw-r--r--   0 parkererickson   (502) staff       (20)     6631 2022-12-12 17:45:12.000000 pyTigerGraph-1.5.2/tests/test_pyTigerGraphPath.py
--rw-r--r--   0 parkererickson   (502) staff       (20)     4156 2023-05-03 19:52:07.000000 pyTigerGraph-1.5.2/tests/test_pyTigerGraphQuery.py
--rw-r--r--   0 parkererickson   (502) staff       (20)    11977 2023-12-11 22:02:16.000000 pyTigerGraph-1.5.2/tests/test_pyTigerGraphSchema.py
--rw-r--r--   0 parkererickson   (502) staff       (20)      804 2023-12-11 22:02:16.000000 pyTigerGraph-1.5.2/tests/test_pyTigerGraphUDT.py
--rw-r--r--   0 parkererickson   (502) staff       (20)     2526 2023-05-03 19:52:07.000000 pyTigerGraph-1.5.2/tests/test_pyTigerGraphUtils.py
--rw-r--r--   0 parkererickson   (502) staff       (20)     9548 2023-04-24 16:45:07.000000 pyTigerGraph-1.5.2/tests/test_pyTigerGraphVertex.py
+drwxr-xr-x   0 parkererickson   (502) staff       (20)        0 2024-04-25 17:49:47.742511 pytigergraph-1.6.0/
+-rw-r--r--   0 parkererickson   (502) staff       (20)     3880 2024-04-25 17:49:47.742381 pytigergraph-1.6.0/PKG-INFO
+-rw-r--r--   0 parkererickson   (502) staff       (20)     2520 2023-09-12 17:29:53.000000 pytigergraph-1.6.0/README.md
+drwxr-xr-x   0 parkererickson   (502) staff       (20)        0 2024-04-25 17:49:47.705043 pytigergraph-1.6.0/pyTigerGraph/
+-rw-r--r--   0 parkererickson   (502) staff       (20)      108 2024-04-25 17:48:30.000000 pytigergraph-1.6.0/pyTigerGraph/__init__.py
+drwxr-xr-x   0 parkererickson   (502) staff       (20)        0 2024-04-25 17:49:47.707028 pytigergraph-1.6.0/pyTigerGraph/ai/
+-rw-r--r--   0 parkererickson   (502) staff       (20)        0 2024-02-15 19:40:45.000000 pytigergraph-1.6.0/pyTigerGraph/ai/__init__.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)    13295 2024-04-25 17:30:30.000000 pytigergraph-1.6.0/pyTigerGraph/ai/ai.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)     5533 2023-09-20 21:20:42.000000 pytigergraph-1.6.0/pyTigerGraph/datasets.py
+drwxr-xr-x   0 parkererickson   (502) staff       (20)        0 2024-04-25 17:49:47.713024 pytigergraph-1.6.0/pyTigerGraph/gds/
+-rw-r--r--   0 parkererickson   (502) staff       (20)      211 2023-05-19 15:14:44.000000 pytigergraph-1.6.0/pyTigerGraph/gds/__init__.py
+drwxr-xr-x   0 parkererickson   (502) staff       (20)        0 2024-04-25 17:49:47.717748 pytigergraph-1.6.0/pyTigerGraph/gds/__pycache__/
+-rw-r--r--   0 parkererickson   (502) staff       (20)      398 2023-04-27 20:50:55.000000 pytigergraph-1.6.0/pyTigerGraph/gds/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 parkererickson   (502) staff       (20)    96874 2023-04-28 00:26:42.000000 pytigergraph-1.6.0/pyTigerGraph/gds/__pycache__/dataloaders.cpython-39.pyc
+-rw-r--r--   0 parkererickson   (502) staff       (20)    19922 2023-01-13 15:10:11.000000 pytigergraph-1.6.0/pyTigerGraph/gds/__pycache__/featurizer.cpython-39.pyc
+-rw-r--r--   0 parkererickson   (502) staff       (20)    51764 2023-01-13 15:10:10.000000 pytigergraph-1.6.0/pyTigerGraph/gds/__pycache__/gds.cpython-39.pyc
+-rw-r--r--   0 parkererickson   (502) staff       (20)    19285 2023-04-28 00:26:42.000000 pytigergraph-1.6.0/pyTigerGraph/gds/__pycache__/metrics.cpython-39.pyc
+-rw-r--r--   0 parkererickson   (502) staff       (20)     9232 2023-01-13 15:10:11.000000 pytigergraph-1.6.0/pyTigerGraph/gds/__pycache__/splitters.cpython-39.pyc
+-rw-r--r--   0 parkererickson   (502) staff       (20)     9288 2023-04-28 00:26:42.000000 pytigergraph-1.6.0/pyTigerGraph/gds/__pycache__/trainer.cpython-39.pyc
+-rw-r--r--   0 parkererickson   (502) staff       (20)     5470 2023-04-28 00:26:42.000000 pytigergraph-1.6.0/pyTigerGraph/gds/__pycache__/utilities.cpython-39.pyc
+-rw-r--r--   0 parkererickson   (502) staff       (20)   190405 2023-09-12 17:29:53.000000 pytigergraph-1.6.0/pyTigerGraph/gds/dataloaders.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)    34967 2023-09-20 14:11:13.000000 pytigergraph-1.6.0/pyTigerGraph/gds/featurizer.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)    91456 2023-09-12 17:29:53.000000 pytigergraph-1.6.0/pyTigerGraph/gds/gds.py
+drwxr-xr-x   0 parkererickson   (502) staff       (20)        0 2024-04-25 17:49:47.695014 pytigergraph-1.6.0/pyTigerGraph/gds/gsql/
+drwxr-xr-x   0 parkererickson   (502) staff       (20)        0 2024-04-25 17:49:47.721199 pytigergraph-1.6.0/pyTigerGraph/gds/gsql/dataloaders/
+-rw-r--r--   0 parkererickson   (502) staff       (20)    10792 2023-09-12 17:29:53.000000 pytigergraph-1.6.0/pyTigerGraph/gds/gsql/dataloaders/edge_loader.gsql
+-rw-r--r--   0 parkererickson   (502) staff       (20)    12302 2023-09-12 17:29:53.000000 pytigergraph-1.6.0/pyTigerGraph/gds/gsql/dataloaders/edge_nei_loader.gsql
+-rw-r--r--   0 parkererickson   (502) staff       (20)      242 2023-05-19 19:02:11.000000 pytigergraph-1.6.0/pyTigerGraph/gds/gsql/dataloaders/get_anchors.gsql
+-rw-r--r--   0 parkererickson   (502) staff       (20)     5048 2023-05-19 19:02:11.000000 pytigergraph-1.6.0/pyTigerGraph/gds/gsql/dataloaders/graph_loader.gsql
+-rw-r--r--   0 parkererickson   (502) staff       (20)     7804 2023-05-19 19:02:11.000000 pytigergraph-1.6.0/pyTigerGraph/gds/gsql/dataloaders/hgt_loader.gsql
+-rw-r--r--   0 parkererickson   (502) staff       (20)     8364 2023-05-19 19:02:11.000000 pytigergraph-1.6.0/pyTigerGraph/gds/gsql/dataloaders/neighbor_loader.gsql
+-rw-r--r--   0 parkererickson   (502) staff       (20)     8697 2023-05-19 19:02:11.000000 pytigergraph-1.6.0/pyTigerGraph/gds/gsql/dataloaders/nodepiece_loader.gsql
+-rw-r--r--   0 parkererickson   (502) staff       (20)     5929 2023-05-19 19:02:11.000000 pytigergraph-1.6.0/pyTigerGraph/gds/gsql/dataloaders/vertex_loader.gsql
+drwxr-xr-x   0 parkererickson   (502) staff       (20)        0 2024-04-25 17:49:47.722076 pytigergraph-1.6.0/pyTigerGraph/gds/gsql/splitters/
+-rw-r--r--   0 parkererickson   (502) staff       (20)     1546 2023-04-24 16:45:07.000000 pytigergraph-1.6.0/pyTigerGraph/gds/gsql/splitters/random_anchor_selection.gsql
+-rw-r--r--   0 parkererickson   (502) staff       (20)     2727 2023-05-03 19:52:07.000000 pytigergraph-1.6.0/pyTigerGraph/gds/gsql/splitters/random_edge_split.gsql
+-rw-r--r--   0 parkererickson   (502) staff       (20)     2715 2023-05-03 19:52:07.000000 pytigergraph-1.6.0/pyTigerGraph/gds/gsql/splitters/random_vertex_split.gsql
+-rw-r--r--   0 parkererickson   (502) staff       (20)    22448 2023-05-19 19:02:11.000000 pytigergraph-1.6.0/pyTigerGraph/gds/metrics.py
+drwxr-xr-x   0 parkererickson   (502) staff       (20)        0 2024-04-25 17:49:47.723279 pytigergraph-1.6.0/pyTigerGraph/gds/models/
+-rw-r--r--   0 parkererickson   (502) staff       (20)    13081 2023-05-19 19:02:11.000000 pytigergraph-1.6.0/pyTigerGraph/gds/models/GraphSAGE.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)     5949 2023-05-19 19:02:11.000000 pytigergraph-1.6.0/pyTigerGraph/gds/models/NodePieceMLP.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)       50 2023-05-19 19:02:11.000000 pytigergraph-1.6.0/pyTigerGraph/gds/models/__init__.py
+drwxr-xr-x   0 parkererickson   (502) staff       (20)        0 2024-04-25 17:49:47.725093 pytigergraph-1.6.0/pyTigerGraph/gds/models/__pycache__/
+-rw-r--r--   0 parkererickson   (502) staff       (20)     6025 2023-04-28 00:32:54.000000 pytigergraph-1.6.0/pyTigerGraph/gds/models/__pycache__/GraphSAGE.cpython-39.pyc
+-rw-r--r--   0 parkererickson   (502) staff       (20)     3741 2023-04-28 00:26:44.000000 pytigergraph-1.6.0/pyTigerGraph/gds/models/__pycache__/NodePieceMLP.cpython-39.pyc
+-rw-r--r--   0 parkererickson   (502) staff       (20)      230 2023-04-28 00:26:42.000000 pytigergraph-1.6.0/pyTigerGraph/gds/models/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 parkererickson   (502) staff       (20)     1807 2023-04-28 00:26:42.000000 pytigergraph-1.6.0/pyTigerGraph/gds/models/__pycache__/base_model.cpython-39.pyc
+-rw-r--r--   0 parkererickson   (502) staff       (20)     1286 2023-05-19 19:02:11.000000 pytigergraph-1.6.0/pyTigerGraph/gds/models/base_model.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)     9661 2023-01-09 15:28:36.000000 pytigergraph-1.6.0/pyTigerGraph/gds/splitters.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)    17904 2023-06-08 21:32:52.000000 pytigergraph-1.6.0/pyTigerGraph/gds/trainer.py
+drwxr-xr-x   0 parkererickson   (502) staff       (20)        0 2024-04-25 17:49:47.726002 pytigergraph-1.6.0/pyTigerGraph/gds/transforms/
+-rw-r--r--   0 parkererickson   (502) staff       (20)        0 2023-05-03 19:52:07.000000 pytigergraph-1.6.0/pyTigerGraph/gds/transforms/__init__.py
+drwxr-xr-x   0 parkererickson   (502) staff       (20)        0 2024-04-25 17:49:47.726622 pytigergraph-1.6.0/pyTigerGraph/gds/transforms/__pycache__/
+-rw-r--r--   0 parkererickson   (502) staff       (20)      165 2023-04-27 20:50:55.000000 pytigergraph-1.6.0/pyTigerGraph/gds/transforms/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 parkererickson   (502) staff       (20)     8138 2023-04-27 20:50:55.000000 pytigergraph-1.6.0/pyTigerGraph/gds/transforms/__pycache__/pyg_transforms.cpython-39.pyc
+-rw-r--r--   0 parkererickson   (502) staff       (20)     2158 2023-05-19 19:02:11.000000 pytigergraph-1.6.0/pyTigerGraph/gds/transforms/nodepiece_transforms.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)     9955 2023-05-19 19:02:11.000000 pytigergraph-1.6.0/pyTigerGraph/gds/transforms/pyg_transforms.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)     9349 2023-09-12 17:29:53.000000 pytigergraph-1.6.0/pyTigerGraph/gds/utilities.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)     2887 2024-02-15 19:40:45.000000 pytigergraph-1.6.0/pyTigerGraph/pyTigerGraph.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)    18422 2024-02-15 19:40:45.000000 pytigergraph-1.6.0/pyTigerGraph/pyTigerGraphAuth.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)    17852 2024-04-17 17:11:16.000000 pytigergraph-1.6.0/pyTigerGraph/pyTigerGraphBase.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)     3910 2022-12-07 20:53:19.000000 pytigergraph-1.6.0/pyTigerGraph/pyTigerGraphDataset.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)    47518 2024-04-10 22:57:02.000000 pytigergraph-1.6.0/pyTigerGraph/pyTigerGraphEdge.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)      265 2022-04-21 16:09:16.000000 pytigergraph-1.6.0/pyTigerGraph/pyTigerGraphException.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)     8184 2023-09-12 17:29:53.000000 pytigergraph-1.6.0/pyTigerGraph/pyTigerGraphGSQL.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)     3631 2022-11-02 21:02:01.000000 pytigergraph-1.6.0/pyTigerGraph/pyTigerGraphLoading.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)    11419 2022-11-02 21:02:01.000000 pytigergraph-1.6.0/pyTigerGraph/pyTigerGraphPath.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)    31266 2024-04-21 17:15:36.000000 pytigergraph-1.6.0/pyTigerGraph/pyTigerGraphQuery.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)     9312 2023-12-11 22:02:16.000000 pytigergraph-1.6.0/pyTigerGraph/pyTigerGraphSchema.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)     2184 2022-11-02 21:02:01.000000 pytigergraph-1.6.0/pyTigerGraph/pyTigerGraphUDT.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)    12138 2024-04-25 13:56:30.000000 pytigergraph-1.6.0/pyTigerGraph/pyTigerGraphUtils.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)    32833 2023-04-24 16:45:07.000000 pytigergraph-1.6.0/pyTigerGraph/pyTigerGraphVertex.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)    29259 2024-02-05 14:47:15.000000 pytigergraph-1.6.0/pyTigerGraph/schema.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)     3930 2022-11-15 18:52:57.000000 pytigergraph-1.6.0/pyTigerGraph/visualization.py
+drwxr-xr-x   0 parkererickson   (502) staff       (20)        0 2024-04-25 17:49:47.741400 pytigergraph-1.6.0/pyTigerGraph.egg-info/
+-rw-r--r--   0 parkererickson   (502) staff       (20)     3880 2024-04-25 17:49:47.000000 pytigergraph-1.6.0/pyTigerGraph.egg-info/PKG-INFO
+-rw-r--r--   0 parkererickson   (502) staff       (20)     3670 2024-04-25 17:49:47.000000 pytigergraph-1.6.0/pyTigerGraph.egg-info/SOURCES.txt
+-rw-r--r--   0 parkererickson   (502) staff       (20)        1 2024-04-25 17:49:47.000000 pytigergraph-1.6.0/pyTigerGraph.egg-info/dependency_links.txt
+-rw-r--r--   0 parkererickson   (502) staff       (20)       58 2024-04-25 17:49:47.000000 pytigergraph-1.6.0/pyTigerGraph.egg-info/requires.txt
+-rw-r--r--   0 parkererickson   (502) staff       (20)       19 2024-04-25 17:49:47.000000 pytigergraph-1.6.0/pyTigerGraph.egg-info/top_level.txt
+-rw-r--r--   0 parkererickson   (502) staff       (20)      229 2022-04-20 17:25:11.000000 pytigergraph-1.6.0/pyproject.toml
+-rw-r--r--   0 parkererickson   (502) staff       (20)       78 2024-04-25 17:49:47.742968 pytigergraph-1.6.0/setup.cfg
+-rw-r--r--   0 parkererickson   (502) staff       (20)     2548 2023-09-20 14:11:41.000000 pytigergraph-1.6.0/setup.py
+drwxr-xr-x   0 parkererickson   (502) staff       (20)        0 2024-04-25 17:49:47.740824 pytigergraph-1.6.0/tests/
+-rw-r--r--   0 parkererickson   (502) staff       (20)        0 2022-04-20 17:25:11.000000 pytigergraph-1.6.0/tests/__init__.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)     1481 2022-12-12 17:45:12.000000 pytigergraph-1.6.0/tests/pyTigerGraphUnitTest.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)     6728 2023-09-12 17:29:58.000000 pytigergraph-1.6.0/tests/test_OGM.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)     2037 2022-12-07 20:53:19.000000 pytigergraph-1.6.0/tests/test_datasets.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)    33173 2023-09-12 17:29:53.000000 pytigergraph-1.6.0/tests/test_gds_BaseLoader.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)    10755 2023-09-12 17:29:53.000000 pytigergraph-1.6.0/tests/test_gds_EdgeLoader.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)     5677 2022-12-12 17:45:12.000000 pytigergraph-1.6.0/tests/test_gds_EdgeNeighborLoader.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)     7448 2023-05-03 19:52:07.000000 pytigergraph-1.6.0/tests/test_gds_GDS.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)    17297 2022-12-12 17:59:45.000000 pytigergraph-1.6.0/tests/test_gds_GraphLoader.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)     4700 2023-05-19 19:02:11.000000 pytigergraph-1.6.0/tests/test_gds_GraphSAGE.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)     7362 2023-02-16 15:58:12.000000 pytigergraph-1.6.0/tests/test_gds_HGTLoader.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)    33875 2023-05-03 19:52:07.000000 pytigergraph-1.6.0/tests/test_gds_NeighborLoader.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)     3443 2023-05-19 19:02:11.000000 pytigergraph-1.6.0/tests/test_gds_NodePiece.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)    11380 2023-04-21 18:31:54.000000 pytigergraph-1.6.0/tests/test_gds_NodePieceLoader.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)     4190 2023-05-03 19:52:07.000000 pytigergraph-1.6.0/tests/test_gds_Trainer.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)    11773 2023-02-16 15:58:12.000000 pytigergraph-1.6.0/tests/test_gds_VertexLoader.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)    14864 2023-02-16 15:58:12.000000 pytigergraph-1.6.0/tests/test_gds_featurizer.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)     7436 2023-05-03 19:52:07.000000 pytigergraph-1.6.0/tests/test_gds_metrics.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)     8349 2023-01-09 15:28:36.000000 pytigergraph-1.6.0/tests/test_gds_splitters.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)     5404 2023-05-03 19:52:07.000000 pytigergraph-1.6.0/tests/test_gds_transforms.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)     2498 2023-05-03 19:52:07.000000 pytigergraph-1.6.0/tests/test_gds_utilities.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)     2847 2022-12-12 17:45:12.000000 pytigergraph-1.6.0/tests/test_pyTigerGraphAuth.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)     2860 2022-12-12 17:45:12.000000 pytigergraph-1.6.0/tests/test_pyTigerGraphBase.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)    14229 2023-02-20 22:23:49.000000 pytigergraph-1.6.0/tests/test_pyTigerGraphEdge.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)     2300 2023-05-19 19:02:11.000000 pytigergraph-1.6.0/tests/test_pyTigerGraphGSQL.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)     6631 2022-12-12 17:45:12.000000 pytigergraph-1.6.0/tests/test_pyTigerGraphPath.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)     4156 2023-05-03 19:52:07.000000 pytigergraph-1.6.0/tests/test_pyTigerGraphQuery.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)    11977 2023-12-11 22:02:16.000000 pytigergraph-1.6.0/tests/test_pyTigerGraphSchema.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)      804 2023-12-11 22:02:16.000000 pytigergraph-1.6.0/tests/test_pyTigerGraphUDT.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)     2526 2023-05-03 19:52:07.000000 pytigergraph-1.6.0/tests/test_pyTigerGraphUtils.py
+-rw-r--r--   0 parkererickson   (502) staff       (20)     9548 2023-04-24 16:45:07.000000 pytigergraph-1.6.0/tests/test_pyTigerGraphVertex.py
```

### Comparing `pyTigerGraph-1.5.2/PKG-INFO` & `pytigergraph-1.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyTigerGraph
-Version: 1.5.2
+Version: 1.6.0
 Summary: Library to connect to TigerGraph databases
 Home-page: https://docs.tigergraph.com/pytigergraph/current/intro/
 Download-URL: 
 Author: TigerGraph Inc.
 Author-email: support@tigergraph.com
 License: Apache 2
 Project-URL: Bug Reports, https://github.com/tigergraph/pyTigerGraph/issues
```

### Comparing `pyTigerGraph-1.5.2/README.md` & `pytigergraph-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.5.2/pyTigerGraph/datasets.py` & `pytigergraph-1.6.0/pyTigerGraph/datasets.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.5.2/pyTigerGraph/gds/__pycache__/dataloaders.cpython-39.pyc` & `pytigergraph-1.6.0/pyTigerGraph/gds/__pycache__/dataloaders.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.5.2/pyTigerGraph/gds/__pycache__/featurizer.cpython-39.pyc` & `pytigergraph-1.6.0/pyTigerGraph/gds/__pycache__/featurizer.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.5.2/pyTigerGraph/gds/__pycache__/gds.cpython-39.pyc` & `pytigergraph-1.6.0/pyTigerGraph/gds/__pycache__/gds.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.5.2/pyTigerGraph/gds/__pycache__/metrics.cpython-39.pyc` & `pytigergraph-1.6.0/pyTigerGraph/gds/__pycache__/metrics.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.5.2/pyTigerGraph/gds/__pycache__/splitters.cpython-39.pyc` & `pytigergraph-1.6.0/pyTigerGraph/gds/__pycache__/splitters.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.5.2/pyTigerGraph/gds/__pycache__/trainer.cpython-39.pyc` & `pytigergraph-1.6.0/pyTigerGraph/gds/__pycache__/trainer.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.5.2/pyTigerGraph/gds/__pycache__/utilities.cpython-39.pyc` & `pytigergraph-1.6.0/pyTigerGraph/gds/__pycache__/utilities.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.5.2/pyTigerGraph/gds/dataloaders.py` & `pytigergraph-1.6.0/pyTigerGraph/gds/dataloaders.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.5.2/pyTigerGraph/gds/featurizer.py` & `pytigergraph-1.6.0/pyTigerGraph/gds/featurizer.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.5.2/pyTigerGraph/gds/gds.py` & `pytigergraph-1.6.0/pyTigerGraph/gds/gds.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.5.2/pyTigerGraph/gds/gsql/dataloaders/edge_loader.gsql` & `pytigergraph-1.6.0/pyTigerGraph/gds/gsql/dataloaders/edge_loader.gsql`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.5.2/pyTigerGraph/gds/gsql/dataloaders/edge_nei_loader.gsql` & `pytigergraph-1.6.0/pyTigerGraph/gds/gsql/dataloaders/edge_nei_loader.gsql`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.5.2/pyTigerGraph/gds/gsql/dataloaders/graph_loader.gsql` & `pytigergraph-1.6.0/pyTigerGraph/gds/gsql/dataloaders/graph_loader.gsql`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.5.2/pyTigerGraph/gds/gsql/dataloaders/hgt_loader.gsql` & `pytigergraph-1.6.0/pyTigerGraph/gds/gsql/dataloaders/hgt_loader.gsql`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.5.2/pyTigerGraph/gds/gsql/dataloaders/neighbor_loader.gsql` & `pytigergraph-1.6.0/pyTigerGraph/gds/gsql/dataloaders/neighbor_loader.gsql`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.5.2/pyTigerGraph/gds/gsql/dataloaders/nodepiece_loader.gsql` & `pytigergraph-1.6.0/pyTigerGraph/gds/gsql/dataloaders/nodepiece_loader.gsql`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.5.2/pyTigerGraph/gds/gsql/dataloaders/vertex_loader.gsql` & `pytigergraph-1.6.0/pyTigerGraph/gds/gsql/dataloaders/vertex_loader.gsql`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.5.2/pyTigerGraph/gds/gsql/splitters/random_anchor_selection.gsql` & `pytigergraph-1.6.0/pyTigerGraph/gds/gsql/splitters/random_anchor_selection.gsql`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.5.2/pyTigerGraph/gds/gsql/splitters/random_edge_split.gsql` & `pytigergraph-1.6.0/pyTigerGraph/gds/gsql/splitters/random_edge_split.gsql`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.5.2/pyTigerGraph/gds/gsql/splitters/random_vertex_split.gsql` & `pytigergraph-1.6.0/pyTigerGraph/gds/gsql/splitters/random_vertex_split.gsql`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.5.2/pyTigerGraph/gds/metrics.py` & `pytigergraph-1.6.0/pyTigerGraph/gds/metrics.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.5.2/pyTigerGraph/gds/models/GraphSAGE.py` & `pytigergraph-1.6.0/pyTigerGraph/gds/models/GraphSAGE.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.5.2/pyTigerGraph/gds/models/NodePieceMLP.py` & `pytigergraph-1.6.0/pyTigerGraph/gds/models/NodePieceMLP.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.5.2/pyTigerGraph/gds/models/__pycache__/GraphSAGE.cpython-39.pyc` & `pytigergraph-1.6.0/pyTigerGraph/gds/models/__pycache__/GraphSAGE.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.5.2/pyTigerGraph/gds/models/__pycache__/NodePieceMLP.cpython-39.pyc` & `pytigergraph-1.6.0/pyTigerGraph/gds/models/__pycache__/NodePieceMLP.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.5.2/pyTigerGraph/gds/models/__pycache__/base_model.cpython-39.pyc` & `pytigergraph-1.6.0/pyTigerGraph/gds/models/__pycache__/base_model.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.5.2/pyTigerGraph/gds/models/base_model.py` & `pytigergraph-1.6.0/pyTigerGraph/gds/models/base_model.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.5.2/pyTigerGraph/gds/splitters.py` & `pytigergraph-1.6.0/pyTigerGraph/gds/splitters.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.5.2/pyTigerGraph/gds/trainer.py` & `pytigergraph-1.6.0/pyTigerGraph/gds/trainer.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.5.2/pyTigerGraph/gds/transforms/__pycache__/pyg_transforms.cpython-39.pyc` & `pytigergraph-1.6.0/pyTigerGraph/gds/transforms/__pycache__/pyg_transforms.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.5.2/pyTigerGraph/gds/transforms/nodepiece_transforms.py` & `pytigergraph-1.6.0/pyTigerGraph/gds/transforms/nodepiece_transforms.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.5.2/pyTigerGraph/gds/transforms/pyg_transforms.py` & `pytigergraph-1.6.0/pyTigerGraph/gds/transforms/pyg_transforms.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.5.2/pyTigerGraph/gds/utilities.py` & `pytigergraph-1.6.0/pyTigerGraph/gds/utilities.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.5.2/pyTigerGraph/pyTigerGraph.py` & `pytigergraph-1.6.0/pyTigerGraph/pyTigerGraph.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.5.2/pyTigerGraph/pyTigerGraphAuth.py` & `pytigergraph-1.6.0/pyTigerGraph/pyTigerGraphAuth.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.5.2/pyTigerGraph/pyTigerGraphBase.py` & `pytigergraph-1.6.0/pyTigerGraph/pyTigerGraphBase.py`

 * *Files 3% similar despite different names*

```diff
@@ -274,15 +274,15 @@
         if headers:
             _headers.update(headers)
         if self.awsIamHeaders:
             if url.startswith(self.gsUrl + "/gsqlserver/"):
                 _headers.update(self.awsIamHeaders)
         if self.responseConfigHeader:
             _headers.update(self.responseConfigHeader)
-        if method == "POST" or method == "PUT":
+        if method == "POST" or method == "PUT" or method == "DELETE":
             _data = data
         else:
             _data = None
 
         if self.useCert is True or self.certPath is not None:
             verify = False
         else:
@@ -383,16 +383,40 @@
         res = self._req("POST", url, authMode, headers, data, resKey, skipCheck, params, jsonData=jsonData)
 
         if logger.level == logging.DEBUG:
             logger.debug("return: " + str(res))
         logger.info("exit: _post")
 
         return res
+    
+    def _put(self, url: str, authMode: str = "token", data = None, resKey=None, jsonData=False) -> Union[dict, list]:
+        """Generic PUT method.
 
-    def _delete(self, url: str, authMode: str = "token") -> Union[dict, list]:
+        Args:
+            url:
+                Complete REST++ API URL including path and parameters.
+            authMode:
+                Authentication mode, either `"token"` (default) or `"pwd"`.
+
+        Returns:
+            The response from the request (as a dictionary).
+        """
+        logger.info("entry: _put")
+        if logger.level == logging.DEBUG:
+            logger.debug("params: " + self._locals(locals()))
+
+        res = self._req("PUT", url, authMode, data=data, resKey=resKey, jsonData=jsonData)
+
+        if logger.level == logging.DEBUG:
+            logger.debug("return: " + str(res))
+        logger.info("exit: _put")
+
+        return res
+
+    def _delete(self, url: str, authMode: str = "token", data: dict = None, resKey=None, jsonData=False) -> Union[dict, list]:
         """Generic DELETE method.
 
         Args:
             url:
                 Complete REST++ API URL including path and parameters.
             authMode:
                 Authentication mode, either `"token"` (default) or `"pwd"`.
@@ -400,15 +424,15 @@
         Returns:
             The response from the request (as a dictionary).
         """
         logger.info("entry: _delete")
         if logger.level == logging.DEBUG:
             logger.debug("params: " + self._locals(locals()))
 
-        res = self._req("DELETE", url, authMode)
+        res = self._req("DELETE", url, authMode, data=data, resKey=resKey, jsonData=jsonData)
 
         if logger.level == logging.DEBUG:
             logger.debug("return: " + str(res))
         logger.info("exit: _delete")
 
         return res
```

### Comparing `pyTigerGraph-1.5.2/pyTigerGraph/pyTigerGraphDataset.py` & `pytigergraph-1.6.0/pyTigerGraph/pyTigerGraphDataset.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.5.2/pyTigerGraph/pyTigerGraphEdge.py` & `pytigergraph-1.6.0/pyTigerGraph/pyTigerGraphEdge.py`

 * *Files 0% similar despite different names*

```diff
@@ -603,19 +603,19 @@
                         for k2, v2 in v1.items():
                             if c2 > 0:
                                 ret += ","
                             c3 = 0
                             for v3 in v2:
                                 if c3 > 0:
                                     ret += ","
-                                ret += '"' + k2 + '":' + json.dumps(v3)
+                                ret += json.dumps(k2) + ':' + json.dumps(v3)
                                 c3 += 1
                             c2 += 1
                     else:
-                        ret += '"' + k1 + '":' + _dumps(data[k1])
+                        ret += json.dumps(k1) + ':' + _dumps(data[k1])
                     c1 += 1
             return "{" + ret + "}"
 
         logger.info("entry: upsertEdges")
         if logger.level == logging.DEBUG:
             logger.debug("params: " + self._locals(locals()))
```

### Comparing `pyTigerGraph-1.5.2/pyTigerGraph/pyTigerGraphGSQL.py` & `pytigergraph-1.6.0/pyTigerGraph/pyTigerGraphGSQL.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.5.2/pyTigerGraph/pyTigerGraphLoading.py` & `pytigergraph-1.6.0/pyTigerGraph/pyTigerGraphLoading.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.5.2/pyTigerGraph/pyTigerGraphPath.py` & `pytigergraph-1.6.0/pyTigerGraph/pyTigerGraphPath.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.5.2/pyTigerGraph/pyTigerGraphQuery.py` & `pytigergraph-1.6.0/pyTigerGraph/pyTigerGraphQuery.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 The functions on this page run installed or interpret queries in TigerGraph.
 All functions in this module are called as methods on a link:https://docs.tigergraph.com/pytigergraph/current/core-functions/base[`TigerGraphConnection` object].
 """
 import json
 import logging
 from datetime import datetime
 
-from typing import TYPE_CHECKING, Union
+from typing import TYPE_CHECKING, Union, Optional
 
 if TYPE_CHECKING:
     import pandas as pd
 
 from pyTigerGraph.pyTigerGraphException import TigerGraphException
 from pyTigerGraph.pyTigerGraphSchema import pyTigerGraphSchema
 from pyTigerGraph.pyTigerGraphUtils import pyTigerGraphUtils
@@ -587,7 +587,117 @@
                          str(seconds) + "&segment=" + str(segments), resKey="")
 
         if logger.level == logging.DEBUG:
             logger.debug("return: " + str(ret))
         logger.info("exit: getStatistics")
 
         return ret
+
+    def describeQuery(self, queryName: str, queryDescription: str, parameterDescriptions: dict = {}):
+        """Add a query description and parameter descriptions. Only supported on versions of TigerGraph >= 4.0.0.
+        
+        Args:
+            queryName:
+                The name of the query to describe.
+            queryDescription:
+                A description of the query.
+            parameterDescriptions (optional):
+                A dictionary of parameter descriptions. The keys are the parameter names and the values are the descriptions.
+        
+        Returns:
+            The response from the database.
+        """
+        logger.info("entry: describeQuery")
+        self.ver = self.getVer()
+        major_ver, minor_ver, patch_ver = self.ver.split(".")
+        if int(major_ver) < 4:
+            logger.info("exit: describeQuery")
+            raise TigerGraphException("This function is only supported on versions of TigerGraph >= 4.0.0.", 0)
+        
+        if parameterDescriptions:
+            params = {"queries": [
+                {"queryName": queryName,
+                "description": queryDescription,
+                "parameters": [{"paramName": k, "description": v} for k, v in parameterDescriptions.items()]}
+            ]}
+        else:
+            params = {"queries": [
+                {"queryName": queryName,
+                "description": queryDescription}
+            ]}
+        if logger.level == logging.DEBUG:
+            logger.debug("params: " + params)
+        res = self._put(self.gsUrl+"/gsqlserver/gsql/description?graph="+self.graphname, data=params, authMode="pwd", jsonData=True)
+
+        if logger.level == logging.DEBUG:
+            logger.debug("return: " + str(res))
+        logger.info("exit: describeQuery")
+
+        return res
+    
+    def getQueryDescription(self, queryName: Optional[Union[str, list]] = "all"):
+        """Get the description of a query. Only supported on versions of TigerGraph >= 4.0.0.
+        
+        Args:
+            queryName:
+                The name of the query to get the description of. 
+                If multiple query descriptions are desired, pass a list of query names.
+                If set to "all", returns the description of all queries.
+        
+        Returns:
+            The description of the query(ies).
+        """
+        logger.info("entry: getQueryDescription")
+        self.ver = self.getVer()
+        major_ver, minor_ver, patch_ver = self.ver.split(".")
+        if int(major_ver) < 4:
+            logger.info("exit: getQueryDescription")
+            raise TigerGraphException("This function is only supported on versions of TigerGraph >= 4.0.0.", 0)
+        
+        if logger.level == logging.DEBUG:
+            logger.debug("params: " + self._locals(locals()))
+        
+        if isinstance(queryName, list):
+            queryName = ",".join(queryName)
+
+        res = self._get(self.gsUrl+"/gsqlserver/gsql/description?graph="+self.graphname+"&query="+queryName, authMode="pwd", resKey=None)
+        if not res["error"]:
+            if logger.level == logging.DEBUG:
+                logger.debug("exit: getQueryDescription")
+            return res["queries"]
+        else:
+            raise TigerGraphException(res["message"], res["code"])
+        
+    def dropQueryDescription(self, queryName: str, dropParamDescriptions: bool = True):
+        """Drop the description of a query. Only supported on versions of TigerGraph >= 4.0.0.
+        
+        Args:
+            queryName:
+                The name of the query to drop the description of.
+                If set to "*", drops the description of all queries.
+            dropParamDescriptions:
+                Whether to drop the parameter descriptions as well. Defaults to True.
+        
+        Returns:
+            The response from the database.
+        """
+        logger.info("entry: dropQueryDescription")
+        self.ver = self.getVer()
+        major_ver, minor_ver, patch_ver = self.ver.split(".")
+        if int(major_ver) < 4:
+            logger.info("exit: describeQuery")
+            raise TigerGraphException("This function is only supported on versions of TigerGraph >= 4.0.0.", 0)
+        
+        if logger.level == logging.DEBUG:
+            logger.debug("params: " + self._locals(locals()))
+        if dropParamDescriptions:
+            params = {"queries": [queryName], "queryParameters": [queryName+".*"]}
+        else:
+            params = {"queries": [queryName]}
+        print(params)
+        res = self._delete(self.gsUrl+"/gsqlserver/gsql/description?graph="+self.graphname, authMode="pwd", data=params, jsonData=True)
+        
+        if logger.level == logging.DEBUG:
+            logger.debug("return: " + str(res))
+        logger.info("exit: dropQueryDescription")
+        
+        return res
```

### Comparing `pyTigerGraph-1.5.2/pyTigerGraph/pyTigerGraphSchema.py` & `pytigergraph-1.6.0/pyTigerGraph/pyTigerGraphSchema.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.5.2/pyTigerGraph/pyTigerGraphUDT.py` & `pytigergraph-1.6.0/pyTigerGraph/pyTigerGraphUDT.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.5.2/pyTigerGraph/pyTigerGraphUtils.py` & `pytigergraph-1.6.0/pyTigerGraph/pyTigerGraphUtils.py`

 * *Files 0% similar despite different names*

```diff
@@ -88,15 +88,15 @@
             - `GET /version`
                 See xref:tigergraph-server:API:built-in-endpoints.adoc#_show_component_versions[Show component versions]
         """
         logger.info("entry: getVersion")
         if logger.level == logging.DEBUG:
             logger.debug("params: " + self._locals(locals()))
 
-        response = self._get(self.restppUrl+"/version/"+self.graphname, strictJson=False, resKey="message")
+        response = self._get(self.restppUrl+"/version", strictJson=False, resKey="message")
        
         if raw:
             return response
         res = response.split("\n")
         components = []
         for i in range(len(res)):
             if 2 < i < len(res) - 1:
```

### Comparing `pyTigerGraph-1.5.2/pyTigerGraph/pyTigerGraphVertex.py` & `pytigergraph-1.6.0/pyTigerGraph/pyTigerGraphVertex.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.5.2/pyTigerGraph/schema.py` & `pytigergraph-1.6.0/pyTigerGraph/schema.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.5.2/pyTigerGraph/visualization.py` & `pytigergraph-1.6.0/pyTigerGraph/visualization.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.5.2/pyTigerGraph.egg-info/PKG-INFO` & `pytigergraph-1.6.0/pyTigerGraph.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyTigerGraph
-Version: 1.5.2
+Version: 1.6.0
 Summary: Library to connect to TigerGraph databases
 Home-page: https://docs.tigergraph.com/pytigergraph/current/intro/
 Download-URL: 
 Author: TigerGraph Inc.
 Author-email: support@tigergraph.com
 License: Apache 2
 Project-URL: Bug Reports, https://github.com/tigergraph/pyTigerGraph/issues
```

### Comparing `pyTigerGraph-1.5.2/pyTigerGraph.egg-info/SOURCES.txt` & `pytigergraph-1.6.0/pyTigerGraph.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.5.2/setup.py` & `pytigergraph-1.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.5.2/tests/pyTigerGraphUnitTest.py` & `pytigergraph-1.6.0/tests/pyTigerGraphUnitTest.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.5.2/tests/test_OGM.py` & `pytigergraph-1.6.0/tests/test_OGM.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.5.2/tests/test_datasets.py` & `pytigergraph-1.6.0/tests/test_datasets.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.5.2/tests/test_gds_BaseLoader.py` & `pytigergraph-1.6.0/tests/test_gds_BaseLoader.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.5.2/tests/test_gds_EdgeLoader.py` & `pytigergraph-1.6.0/tests/test_gds_EdgeLoader.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.5.2/tests/test_gds_EdgeNeighborLoader.py` & `pytigergraph-1.6.0/tests/test_gds_EdgeNeighborLoader.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.5.2/tests/test_gds_GDS.py` & `pytigergraph-1.6.0/tests/test_gds_GDS.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.5.2/tests/test_gds_GraphLoader.py` & `pytigergraph-1.6.0/tests/test_gds_GraphLoader.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.5.2/tests/test_gds_GraphSAGE.py` & `pytigergraph-1.6.0/tests/test_gds_GraphSAGE.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.5.2/tests/test_gds_HGTLoader.py` & `pytigergraph-1.6.0/tests/test_gds_HGTLoader.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.5.2/tests/test_gds_NeighborLoader.py` & `pytigergraph-1.6.0/tests/test_gds_NeighborLoader.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.5.2/tests/test_gds_NodePiece.py` & `pytigergraph-1.6.0/tests/test_gds_NodePiece.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.5.2/tests/test_gds_NodePieceLoader.py` & `pytigergraph-1.6.0/tests/test_gds_NodePieceLoader.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.5.2/tests/test_gds_Trainer.py` & `pytigergraph-1.6.0/tests/test_gds_Trainer.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.5.2/tests/test_gds_VertexLoader.py` & `pytigergraph-1.6.0/tests/test_gds_VertexLoader.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.5.2/tests/test_gds_featurizer.py` & `pytigergraph-1.6.0/tests/test_gds_featurizer.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.5.2/tests/test_gds_metrics.py` & `pytigergraph-1.6.0/tests/test_gds_metrics.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.5.2/tests/test_gds_splitters.py` & `pytigergraph-1.6.0/tests/test_gds_splitters.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.5.2/tests/test_gds_transforms.py` & `pytigergraph-1.6.0/tests/test_gds_transforms.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.5.2/tests/test_gds_utilities.py` & `pytigergraph-1.6.0/tests/test_gds_utilities.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.5.2/tests/test_pyTigerGraphAuth.py` & `pytigergraph-1.6.0/tests/test_pyTigerGraphAuth.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.5.2/tests/test_pyTigerGraphBase.py` & `pytigergraph-1.6.0/tests/test_pyTigerGraphBase.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.5.2/tests/test_pyTigerGraphEdge.py` & `pytigergraph-1.6.0/tests/test_pyTigerGraphEdge.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.5.2/tests/test_pyTigerGraphGSQL.py` & `pytigergraph-1.6.0/tests/test_pyTigerGraphGSQL.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.5.2/tests/test_pyTigerGraphPath.py` & `pytigergraph-1.6.0/tests/test_pyTigerGraphPath.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.5.2/tests/test_pyTigerGraphQuery.py` & `pytigergraph-1.6.0/tests/test_pyTigerGraphQuery.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.5.2/tests/test_pyTigerGraphSchema.py` & `pytigergraph-1.6.0/tests/test_pyTigerGraphSchema.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.5.2/tests/test_pyTigerGraphUDT.py` & `pytigergraph-1.6.0/tests/test_pyTigerGraphUDT.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.5.2/tests/test_pyTigerGraphUtils.py` & `pytigergraph-1.6.0/tests/test_pyTigerGraphUtils.py`

 * *Files identical despite different names*

### Comparing `pyTigerGraph-1.5.2/tests/test_pyTigerGraphVertex.py` & `pytigergraph-1.6.0/tests/test_pyTigerGraphVertex.py`

 * *Files identical despite different names*


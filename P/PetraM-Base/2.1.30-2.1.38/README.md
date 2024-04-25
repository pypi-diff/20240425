# Comparing `tmp/PetraM_Base-2.1.30.tar.gz` & `tmp/petram_base-2.1.38.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PetraM_Base-2.1.30.tar", last modified: Wed Jan 24 19:40:46 2024, max compression
+gzip compressed data, was "petram_base-2.1.38.tar", last modified: Thu Apr 25 14:12:41 2024, max compression
```

## Comparing `PetraM_Base-2.1.30.tar` & `petram_base-2.1.38.tar`

### file list

```diff
@@ -1,296 +1,300 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 19:40:46.536417 PetraM_Base-2.1.30/
--rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-01-24 19:40:46.536417 PetraM_Base-2.1.30/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 19:40:46.536417 PetraM_Base-2.1.30/PetraM_Base.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-01-24 19:40:46.000000 PetraM_Base-2.1.30/PetraM_Base.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9838 2024-01-24 19:40:46.000000 PetraM_Base-2.1.30/PetraM_Base.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-24 19:40:46.000000 PetraM_Base-2.1.30/PetraM_Base.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-01-24 19:40:46.000000 PetraM_Base-2.1.30/PetraM_Base.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 19:40:46.488417 PetraM_Base-2.1.30/petram/
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 19:40:46.488417 PetraM_Base-2.1.30/petram/data/
--rw-r--r--   0 runner    (1001) docker     (127)     9519 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/data/BilinearOps
--rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/data/LinearOps
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 19:40:46.504417 PetraM_Base-2.1.30/petram/data/icon/
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/data/icon/domain.png
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/data/icon/dot.png
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/data/icon/dot_bk.png
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/data/icon/face.png
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/data/icon/face_bk.png
--rw-r--r--   0 runner    (1001) docker     (127)    15140 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/data/icon/form_BoundaryFlowIntegrator.png
--rw-r--r--   0 runner    (1001) docker     (127)     6804 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/data/icon/form_BoundaryLFIntegrator.png
--rw-r--r--   0 runner    (1001) docker     (127)     5728 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/data/icon/form_BoundaryMassIntegrator.png
--rw-r--r--   0 runner    (1001) docker     (127)     8366 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/data/icon/form_BoundaryNormalLFIntegrator.png
--rw-r--r--   0 runner    (1001) docker     (127)     7960 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/data/icon/form_BoundaryTangentialLFIntegrator.png
--rw-r--r--   0 runner    (1001) docker     (127)     6699 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/data/icon/form_ConvectionIntegrator.png
--rw-r--r--   0 runner    (1001) docker     (127)     9089 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/data/icon/form_CurlCurlIntegrator.png
--rw-r--r--   0 runner    (1001) docker     (127)     8603 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/data/icon/form_DerivativeIntegrator1.png
--rw-r--r--   0 runner    (1001) docker     (127)     8603 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/data/icon/form_DerivativeIntegrator2.png
--rw-r--r--   0 runner    (1001) docker     (127)     8603 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/data/icon/form_DerivativeIntegrator3.png
--rw-r--r--   0 runner    (1001) docker     (127)     9036 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/data/icon/form_DiffusionIntegrator.png
--rw-r--r--   0 runner    (1001) docker     (127)     9501 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/data/icon/form_DivDivIntegrator.png
--rw-r--r--   0 runner    (1001) docker     (127)     6804 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/data/icon/form_DomainLFIntegrator.png
--rw-r--r--   0 runner    (1001) docker     (127)     8689 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/data/icon/form_ElasticityIntegrator.png
--rw-r--r--   0 runner    (1001) docker     (127)     7598 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/data/icon/form_GroupConvectionIntegrator.png
--rw-r--r--   0 runner    (1001) docker     (127)     7305 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/data/icon/form_MassIntegrator.png
--rw-r--r--   0 runner    (1001) docker     (127)     9665 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/data/icon/form_MixedCrossCurlCurlIntegrator.png
--rw-r--r--   0 runner    (1001) docker     (127)     9461 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/data/icon/form_MixedCrossCurlGradIntegrator.png
--rw-r--r--   0 runner    (1001) docker     (127)     9128 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/data/icon/form_MixedCrossCurlIntegrator.png
--rw-r--r--   0 runner    (1001) docker     (127)     9404 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/data/icon/form_MixedCrossGradCurlIntegrator.png
--rw-r--r--   0 runner    (1001) docker     (127)     9751 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/data/icon/form_MixedCrossGradGradIntegrator.png
--rw-r--r--   0 runner    (1001) docker     (127)     9324 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/data/icon/form_MixedCrossGradIntegrator.png
--rw-r--r--   0 runner    (1001) docker     (127)     8647 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/data/icon/form_MixedCrossProductIntegrator.png
--rw-r--r--   0 runner    (1001) docker     (127)     9089 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/data/icon/form_MixedCurlCurlIntegrator.png
--rw-r--r--   0 runner    (1001) docker     (127)     8590 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/data/icon/form_MixedDirectionalDerivativeIntegrator.png
--rw-r--r--   0 runner    (1001) docker     (127)     9776 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/data/icon/form_MixedDivGradIntegrator.png
--rw-r--r--   0 runner    (1001) docker     (127)     8133 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/data/icon/form_MixedDotProductIntegrator.png
--rw-r--r--   0 runner    (1001) docker     (127)     9748 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/data/icon/form_MixedGradDivIntegrator.png
--rw-r--r--   0 runner    (1001) docker     (127)     9036 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/data/icon/form_MixedGradGradIntegrator.png
--rw-r--r--   0 runner    (1001) docker     (127)     9758 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/data/icon/form_MixedScalarCrossCurlIntegrator.png
--rw-r--r--   0 runner    (1001) docker     (127)     9056 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/data/icon/form_MixedScalarCrossGradIntegrator.png
--rw-r--r--   0 runner    (1001) docker     (127)     8604 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/data/icon/form_MixedScalarCrossProductIntegrator.png
--rw-r--r--   0 runner    (1001) docker     (127)     9034 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/data/icon/form_MixedScalarCurlIntegrator.png
--rw-r--r--   0 runner    (1001) docker     (127)     9842 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/data/icon/form_MixedScalarDerivativeIntegrator.png
--rw-r--r--   0 runner    (1001) docker     (127)     8567 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/data/icon/form_MixedScalarDivergenceIntegrator.png
--rw-r--r--   0 runner    (1001) docker     (127)     7305 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/data/icon/form_MixedScalarMassIntegrator.png
--rw-r--r--   0 runner    (1001) docker     (127)     9344 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/data/icon/form_MixedScalarWeakCrossProductIntegrator.png
--rw-r--r--   0 runner    (1001) docker     (127)     9509 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/data/icon/form_MixedScalarWeakCurlCrossIntegrator.png
--rw-r--r--   0 runner    (1001) docker     (127)    10015 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/data/icon/form_MixedScalarWeakCurlIntegrator.png
--rw-r--r--   0 runner    (1001) docker     (127)    10301 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/data/icon/form_MixedScalarWeakDerivativeIntegrator.png
--rw-r--r--   0 runner    (1001) docker     (127)     9064 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/data/icon/form_MixedScalarWeakDivergenceIntegrator.png
--rw-r--r--   0 runner    (1001) docker     (127)     9001 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/data/icon/form_MixedScalarWeakGradientIntegrator.png
--rw-r--r--   0 runner    (1001) docker     (127)     9089 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/data/icon/form_MixedVectorCurlIntegrator.png
--rw-r--r--   0 runner    (1001) docker     (127)     8915 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/data/icon/form_MixedVectorDivergenceIntegrator.png
--rw-r--r--   0 runner    (1001) docker     (127)     8357 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/data/icon/form_MixedVectorGradientIntegrator.png
--rw-r--r--   0 runner    (1001) docker     (127)     7674 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/data/icon/form_MixedVectorMassIntegrator.png
--rw-r--r--   0 runner    (1001) docker     (127)     7911 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/data/icon/form_MixedVectorProductIntegrator.png
--rw-r--r--   0 runner    (1001) docker     (127)     9446 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/data/icon/form_MixedVectorWeakCurlIntegrator.png
--rw-r--r--   0 runner    (1001) docker     (127)     9051 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/data/icon/form_MixedVectorWeakDivergenceIntegrator.png
--rw-r--r--   0 runner    (1001) docker     (127)     9509 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/data/icon/form_MixedWeakCurlCrossIntegrator.png
--rw-r--r--   0 runner    (1001) docker     (127)    10037 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/data/icon/form_MixedWeakDivCrossIntegrator.png
--rw-r--r--   0 runner    (1001) docker     (127)     9520 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/data/icon/form_MixedWeakGradDotIntegrator.png
--rw-r--r--   0 runner    (1001) docker     (127)     8289 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/data/icon/form_VectorBoundaryFluxLFIntegrator.png
--rw-r--r--   0 runner    (1001) docker     (127)     7345 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/data/icon/form_VectorBoundaryLFIntegrator.png
--rw-r--r--   0 runner    (1001) docker     (127)     7441 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/data/icon/form_VectorCurlCurlIntegrator.png
--rw-r--r--   0 runner    (1001) docker     (127)     7035 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/data/icon/form_VectorDiffusionIntegrator.png
--rw-r--r--   0 runner    (1001) docker     (127)     6615 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/data/icon/form_VectorDivergenceIntegrator.png
--rw-r--r--   0 runner    (1001) docker     (127)     7345 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/data/icon/form_VectorDomainLFIntegrator.png
--rw-r--r--   0 runner    (1001) docker     (127)     8289 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/data/icon/form_VectorFEBoundaryFluxLFIntegrator.png
--rw-r--r--   0 runner    (1001) docker     (127)     8938 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/data/icon/form_VectorFEBoundaryTangentLFIntegrator.png
--rw-r--r--   0 runner    (1001) docker     (127)     8846 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/data/icon/form_VectorFECurlIntegrator.png
--rw-r--r--   0 runner    (1001) docker     (127)     6615 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/data/icon/form_VectorFEDivergenceIntegrator.png
--rw-r--r--   0 runner    (1001) docker     (127)     7345 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/data/icon/form_VectorFEDomainLFIntegrator.png
--rw-r--r--   0 runner    (1001) docker     (127)     7674 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/data/icon/form_VectorFEMassIntegrator.png
--rw-r--r--   0 runner    (1001) docker     (127)     6680 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/data/icon/form_VectorFEWeakDivergenceIntegrator.png
--rw-r--r--   0 runner    (1001) docker     (127)     5952 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/data/icon/form_VectorMassIntegrator.png
--rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/data/icon/form_none.png
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/data/icon/hide.png
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/data/icon/line.png
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/data/icon/line_bk.png
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/data/icon/show.png
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/data/icon/showall.png
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/data/icon/solid.png
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/data/icon/transparent.png
--rw-r--r--   0 runner    (1001) docker     (127)     7301 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/debug.py
--rw-r--r--   0 runner    (1001) docker     (127)   146632 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/engine.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 19:40:46.504417 PetraM_Base-2.1.30/petram/ext/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/ext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 19:40:46.512417 PetraM_Base-2.1.30/petram/helper/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/helper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    51502 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/helper/block_matrix.py
--rw-r--r--   0 runner    (1001) docker     (127)     2406 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/helper/boundary_refinement.py
--rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/helper/cdict.py
--rw-r--r--   0 runner    (1001) docker     (127)     5593 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/helper/chypre_to_pymatrix.py
--rw-r--r--   0 runner    (1001) docker     (127)    27003 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/helper/convolve.py
--rw-r--r--   0 runner    (1001) docker     (127)     4525 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/helper/direct_wrapper_call.py
--rw-r--r--   0 runner    (1001) docker     (127)    44049 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/helper/dof_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/helper/dof_mapping_matrix.py
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/helper/dot_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/helper/driver_path.py
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/helper/dummy_mpi.py
--rw-r--r--   0 runner    (1001) docker     (127)     4550 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/helper/element_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     3049 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/helper/eval_deriv.py
--rw-r--r--   0 runner    (1001) docker     (127)     3921 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/helper/eval_shape.py
--rw-r--r--   0 runner    (1001) docker     (127)     3597 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/helper/expression.py
--rw-r--r--   0 runner    (1001) docker     (127)     6182 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/helper/find_dof_map.py
--rw-r--r--   0 runner    (1001) docker     (127)    12438 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/helper/find_dof_map_h1.py
--rw-r--r--   0 runner    (1001) docker     (127)    17162 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/helper/find_dof_map_nd.py
--rw-r--r--   0 runner    (1001) docker     (127)     7167 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/helper/formholder.py
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/helper/functions.py
--rw-r--r--   0 runner    (1001) docker     (127)    12545 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/helper/geom.py
--rw-r--r--   0 runner    (1001) docker     (127)     5731 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/helper/global_named_list.py
--rw-r--r--   0 runner    (1001) docker     (127)    17496 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/helper/hcurl_normal.py
--rw-r--r--   0 runner    (1001) docker     (127)     8838 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/helper/hierarchical_finite_element_spaces.py
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/helper/init_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/helper/load_mfem.py
--rw-r--r--   0 runner    (1001) docker     (127)     5155 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/helper/matrix_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/helper/memory_report.py
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/helper/mpi_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    15226 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/helper/mpi_recipes.py
--rw-r--r--   0 runner    (1001) docker     (127)    12591 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/helper/numba_interp.py
--rw-r--r--   0 runner    (1001) docker     (127)     8240 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/helper/numba_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    32748 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/helper/operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     8646 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/helper/phys_module_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/helper/pickle_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    19046 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/helper/preconditioners.py
--rw-r--r--   0 runner    (1001) docker     (127)     5888 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/helper/projection.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/helper/restricte_integrator.py
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/helper/right_broadcast.py
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/helper/test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3553 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/helper/validator_input.py
--rw-r--r--   0 runner    (1001) docker     (127)    88252 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/helper/variables.py
--rw-r--r--   0 runner    (1001) docker     (127)     4506 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/init_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 19:40:46.516417 PetraM_Base-2.1.30/petram/mesh/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/mesh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5244 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/mesh/composite.py
--rw-r--r--   0 runner    (1001) docker     (127)     4458 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/mesh/find_edges.py
--rw-r--r--   0 runner    (1001) docker     (127)     5012 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/mesh/find_loop.py
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/mesh/find_vertex.py
--rw-r--r--   0 runner    (1001) docker     (127)    21368 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/mesh/geo_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     7976 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/mesh/make_simplemesh.py
--rw-r--r--   0 runner    (1001) docker     (127)     3559 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/mesh/mesh_extension.py
--rw-r--r--   0 runner    (1001) docker     (127)     6253 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/mesh/mesh_inspect.py
--rw-r--r--   0 runner    (1001) docker     (127)    38967 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/mesh/mesh_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     9111 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/mesh/mesh_sel_buttons.py
--rw-r--r--   0 runner    (1001) docker     (127)    28650 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/mesh/mesh_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/mesh/mesh_viewer.py
--rw-r--r--   0 runner    (1001) docker     (127)    22038 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/mesh/nastran2mfem.py
--rw-r--r--   0 runner    (1001) docker     (127)    26567 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/mesh/partial_mesh.py
--rw-r--r--   0 runner    (1001) docker     (127)     8352 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/mesh/plot_mesh.py
--rw-r--r--   0 runner    (1001) docker     (127)     4954 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/mesh/pumimesh_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5906 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/mesh/read_mfemmesh.py
--rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/mesh/read_mfemmesh1.py
--rw-r--r--   0 runner    (1001) docker     (127)     4678 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/mesh/read_mfemmesh2.py
--rw-r--r--   0 runner    (1001) docker     (127)     5982 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/mesh/read_mfemmesh2_old.py
--rw-r--r--   0 runner    (1001) docker     (127)     8380 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/mesh/read_mfemmesh3.py
--rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/mesh/refined_mfem_geom.py
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/mfem_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    16550 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/mfem_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    66666 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/mfem_viewer.py
--rw-r--r--   0 runner    (1001) docker     (127)    34766 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/model.py
--rw-r--r--   0 runner    (1001) docker     (127)    12526 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/namespace_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 19:40:46.520417 PetraM_Base-2.1.30/petram/phys/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/phys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8931 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/phys/aux_operator.py
--rw-r--r--   0 runner    (1001) docker     (127)    13323 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/phys/aux_variable.py
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/phys/bc.py
--rw-r--r--   0 runner    (1001) docker     (127)    18920 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/phys/coefficient.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 19:40:46.520417 PetraM_Base-2.1.30/petram/phys/distance/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/phys/distance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7246 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/phys/distance/distance_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3309 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/phys/distance/wall.py
--rw-r--r--   0 runner    (1001) docker     (127)    41234 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/phys/numba_coefficient.py
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/phys/phys.py
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/phys/phys_const.py
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/phys/phys_cont.py
--rw-r--r--   0 runner    (1001) docker     (127)    45035 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/phys/phys_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/phys/projection.py
--rw-r--r--   0 runner    (1001) docker     (127)    21717 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/phys/pycomplex_coefficient.py
--rw-r--r--   0 runner    (1001) docker     (127)    22796 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/phys/vtable.py
--rw-r--r--   0 runner    (1001) docker     (127)    19102 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/phys/weakform.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 19:40:46.520417 PetraM_Base-2.1.30/petram/phys/wf/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/phys/wf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2790 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/phys/wf/pix_gen.py
--rw-r--r--   0 runner    (1001) docker     (127)     7801 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/phys/wf/wf_constraints.py
--rw-r--r--   0 runner    (1001) docker     (127)    13017 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/phys/wf/wf_essential.py
--rw-r--r--   0 runner    (1001) docker     (127)    10615 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/phys/wf/wf_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/phys/wf/wf_natural.py
--rw-r--r--   0 runner    (1001) docker     (127)     6153 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/phys/wf/wf_pairs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 19:40:46.524417 PetraM_Base-2.1.30/petram/pi/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/pi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    46766 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/pi/dlg_edit_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3426 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/pi/dlg_plot_expr.py
--rw-r--r--   0 runner    (1001) docker     (127)   112468 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/pi/dlg_plot_sol.py
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/pi/dlg_progressbar.py
--rw-r--r--   0 runner    (1001) docker     (127)     7905 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/pi/dlg_submit_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/pi/ns_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/pi/pfz2script.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 19:40:46.524417 PetraM_Base-2.1.30/petram/pi/project_scripts/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/pi/project_scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/pi/project_scripts/convert_mesh.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 19:40:46.528417 PetraM_Base-2.1.30/petram/pi/project_scripts/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/pi/project_scripts/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/pi/project_scripts/helpers/call_glvis.py
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/pi/project_scripts/helpers/clear_sol.py
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/pi/project_scripts/helpers/convert_mfem_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/pi/project_scripts/helpers/create_ns.py
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/pi/project_scripts/helpers/eval_expr.py
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/pi/project_scripts/helpers/init_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/pi/project_scripts/helpers/make_new_sol.py
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/pi/project_scripts/helpers/move_to_petram.py
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/pi/project_scripts/helpers/rebuild_ns.py
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/pi/project_scripts/helpers/reset_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/pi/project_scripts/helpers/save_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/pi/project_scripts/helpers/select_sol.py
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/pi/project_scripts/helpers/start_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     2779 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/pi/project_scripts/run_parallel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2850 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/pi/project_scripts/run_serial.py
--rw-r--r--   0 runner    (1001) docker     (127)     8168 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/pi/sel_buttons.py
--rw-r--r--   0 runner    (1001) docker     (127)    17017 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/pi/selection_palette.py
--rw-r--r--   0 runner    (1001) docker     (127)     4045 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/pi/shell_commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/pi/simple_frame_plus.py
--rw-r--r--   0 runner    (1001) docker     (127)     3092 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/pi/widget_forms.py
--rw-r--r--   0 runner    (1001) docker     (127)     6400 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/pi/widget_init.py
--rw-r--r--   0 runner    (1001) docker     (127)     5627 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/pi/widget_nl.py
--rw-r--r--   0 runner    (1001) docker     (127)     4952 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/pi/widget_smoother.py
--rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/pi/widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 19:40:46.528417 PetraM_Base-2.1.30/petram/postprocess/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/postprocess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14386 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/postprocess/discrt_v_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)    10015 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/postprocess/discrt_v_interpolator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5777 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/postprocess/pp_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     9235 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/postprocess/project_solution.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 19:40:46.528417 PetraM_Base-2.1.30/petram/remote/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12098 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/remote/client_script.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 19:40:46.532417 PetraM_Base-2.1.30/petram/sol/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/sol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10989 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/sol/bdr_nodal_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5598 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/sol/edge_nodal_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/sol/evaluator_agent.py
--rw-r--r--   0 runner    (1001) docker     (127)    12681 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/sol/evaluator_cs.py
--rw-r--r--   0 runner    (1001) docker     (127)    22523 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/sol/evaluator_mp.py
--rw-r--r--   0 runner    (1001) docker     (127)     8017 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/sol/evaluator_single.py
--rw-r--r--   0 runner    (1001) docker     (127)    11009 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/sol/evaluators.py
--rw-r--r--   0 runner    (1001) docker     (127)     3543 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/sol/integral_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/sol/listsoldir.py
--rw-r--r--   0 runner    (1001) docker     (127)     7639 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/sol/ncedge_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)     9130 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/sol/ncface_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5307 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/sol/nodal_refinement.py
--rw-r--r--   0 runner    (1001) docker     (127)    10149 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/sol/pointcloud_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4720 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/sol/probe.py
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/sol/probe_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6335 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/sol/slice_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6581 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/sol/solsets.py
--rw-r--r--   0 runner    (1001) docker     (127)     4894 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/sol/test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 19:40:46.536417 PetraM_Base-2.1.30/petram/solver/
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/solver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/solver/ams_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     7165 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/solver/block_smoother.py
--rw-r--r--   0 runner    (1001) docker     (127)     7581 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/solver/distance_solver.py
--rw-r--r--   0 runner    (1001) docker     (127)    15664 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/solver/gmres_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    24493 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/solver/iterative_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    15413 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/solver/krylov.py
--rw-r--r--   0 runner    (1001) docker     (127)     9389 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/solver/linearsystem_reducer.py
--rw-r--r--   0 runner    (1001) docker     (127)    22917 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/solver/mg_solver_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    43380 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/solver/ml_solver_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    45971 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/solver/mumps_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    27077 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/solver/nl_solver_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    14828 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/solver/parametric.py
--rw-r--r--   0 runner    (1001) docker     (127)     4938 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/solver/parametric_scanner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/solver/set_var.py
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/solver/solinit_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3559 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/solver/solve_loop.py
--rw-r--r--   0 runner    (1001) docker     (127)    15237 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/solver/solver_controls.py
--rw-r--r--   0 runner    (1001) docker     (127)    32313 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/solver/solver_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3703 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/solver/solver_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3191 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/solver/std_meshadapt_solver_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    10436 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/solver/std_solver_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     9191 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/solver/std_solver_model_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/solver/std_solver_model_v3.py
--rw-r--r--   0 runner    (1001) docker     (127)    24874 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/solver/strumpack_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    25639 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/solver/timedomain_solver_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     7316 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/petram/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-24 19:40:46.536417 PetraM_Base-2.1.30/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-01-24 19:40:38.000000 PetraM_Base-2.1.30/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:12:41.209069 petram_base-2.1.38/
+-rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-04-25 14:12:33.000000 petram_base-2.1.38/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-04-25 14:12:41.209069 petram_base-2.1.38/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:12:41.209069 petram_base-2.1.38/PetraM_Base.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-04-25 14:12:41.000000 petram_base-2.1.38/PetraM_Base.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9968 2024-04-25 14:12:41.000000 petram_base-2.1.38/PetraM_Base.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 14:12:41.000000 petram_base-2.1.38/PetraM_Base.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-25 14:12:41.000000 petram_base-2.1.38/PetraM_Base.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-04-25 14:12:33.000000 petram_base-2.1.38/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:12:41.165069 petram_base-2.1.38/petram/
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:12:41.165069 petram_base-2.1.38/petram/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     9519 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/data/BilinearOps
+-rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/data/LinearOps
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:12:41.177069 petram_base-2.1.38/petram/data/icon/
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/data/icon/domain.png
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/data/icon/dot.png
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/data/icon/dot_bk.png
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/data/icon/face.png
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/data/icon/face_bk.png
+-rw-r--r--   0 runner    (1001) docker     (127)    15140 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/data/icon/form_BoundaryFlowIntegrator.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6804 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/data/icon/form_BoundaryLFIntegrator.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5728 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/data/icon/form_BoundaryMassIntegrator.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8366 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/data/icon/form_BoundaryNormalLFIntegrator.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7960 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/data/icon/form_BoundaryTangentialLFIntegrator.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6699 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/data/icon/form_ConvectionIntegrator.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9089 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/data/icon/form_CurlCurlIntegrator.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8603 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/data/icon/form_DerivativeIntegrator1.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8603 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/data/icon/form_DerivativeIntegrator2.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8603 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/data/icon/form_DerivativeIntegrator3.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9036 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/data/icon/form_DiffusionIntegrator.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9501 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/data/icon/form_DivDivIntegrator.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6804 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/data/icon/form_DomainLFIntegrator.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8689 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/data/icon/form_ElasticityIntegrator.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7598 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/data/icon/form_GroupConvectionIntegrator.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7305 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/data/icon/form_MassIntegrator.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9665 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/data/icon/form_MixedCrossCurlCurlIntegrator.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9461 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/data/icon/form_MixedCrossCurlGradIntegrator.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9128 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/data/icon/form_MixedCrossCurlIntegrator.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9404 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/data/icon/form_MixedCrossGradCurlIntegrator.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9751 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/data/icon/form_MixedCrossGradGradIntegrator.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9324 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/data/icon/form_MixedCrossGradIntegrator.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8647 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/data/icon/form_MixedCrossProductIntegrator.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9089 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/data/icon/form_MixedCurlCurlIntegrator.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8590 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/data/icon/form_MixedDirectionalDerivativeIntegrator.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9776 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/data/icon/form_MixedDivGradIntegrator.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8133 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/data/icon/form_MixedDotProductIntegrator.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9748 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/data/icon/form_MixedGradDivIntegrator.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9036 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/data/icon/form_MixedGradGradIntegrator.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9758 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/data/icon/form_MixedScalarCrossCurlIntegrator.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9056 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/data/icon/form_MixedScalarCrossGradIntegrator.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8604 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/data/icon/form_MixedScalarCrossProductIntegrator.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9034 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/data/icon/form_MixedScalarCurlIntegrator.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9842 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/data/icon/form_MixedScalarDerivativeIntegrator.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8567 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/data/icon/form_MixedScalarDivergenceIntegrator.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7305 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/data/icon/form_MixedScalarMassIntegrator.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9344 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/data/icon/form_MixedScalarWeakCrossProductIntegrator.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9509 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/data/icon/form_MixedScalarWeakCurlCrossIntegrator.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10015 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/data/icon/form_MixedScalarWeakCurlIntegrator.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10301 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/data/icon/form_MixedScalarWeakDerivativeIntegrator.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9064 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/data/icon/form_MixedScalarWeakDivergenceIntegrator.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9001 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/data/icon/form_MixedScalarWeakGradientIntegrator.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9089 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/data/icon/form_MixedVectorCurlIntegrator.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8915 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/data/icon/form_MixedVectorDivergenceIntegrator.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8357 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/data/icon/form_MixedVectorGradientIntegrator.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7674 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/data/icon/form_MixedVectorMassIntegrator.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7911 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/data/icon/form_MixedVectorProductIntegrator.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9446 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/data/icon/form_MixedVectorWeakCurlIntegrator.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9051 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/data/icon/form_MixedVectorWeakDivergenceIntegrator.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9509 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/data/icon/form_MixedWeakCurlCrossIntegrator.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10037 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/data/icon/form_MixedWeakDivCrossIntegrator.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9520 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/data/icon/form_MixedWeakGradDotIntegrator.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8289 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/data/icon/form_VectorBoundaryFluxLFIntegrator.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7345 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/data/icon/form_VectorBoundaryLFIntegrator.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7441 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/data/icon/form_VectorCurlCurlIntegrator.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7035 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/data/icon/form_VectorDiffusionIntegrator.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6615 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/data/icon/form_VectorDivergenceIntegrator.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7345 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/data/icon/form_VectorDomainLFIntegrator.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8289 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/data/icon/form_VectorFEBoundaryFluxLFIntegrator.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8938 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/data/icon/form_VectorFEBoundaryTangentLFIntegrator.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8846 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/data/icon/form_VectorFECurlIntegrator.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6615 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/data/icon/form_VectorFEDivergenceIntegrator.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7345 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/data/icon/form_VectorFEDomainLFIntegrator.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7674 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/data/icon/form_VectorFEMassIntegrator.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6680 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/data/icon/form_VectorFEWeakDivergenceIntegrator.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5952 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/data/icon/form_VectorMassIntegrator.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/data/icon/form_none.png
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/data/icon/hide.png
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/data/icon/line.png
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/data/icon/line_bk.png
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/data/icon/show.png
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/data/icon/showall.png
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/data/icon/solid.png
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/data/icon/transparent.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7332 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)   152105 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/engine.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:12:41.177069 petram_base-2.1.38/petram/ext/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/ext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:12:41.185069 petram_base-2.1.38/petram/helper/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/helper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51784 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/helper/block_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2406 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/helper/boundary_refinement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/helper/cdict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5593 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/helper/chypre_to_pymatrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27003 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/helper/convolve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/helper/densemat2pymat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4525 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/helper/direct_wrapper_call.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43920 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/helper/dof_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/helper/dof_mapping_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/helper/dot_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/helper/driver_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/helper/dummy_mpi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4550 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/helper/element_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3049 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/helper/eval_deriv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3921 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/helper/eval_shape.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3597 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/helper/expression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6182 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/helper/find_dof_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12438 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/helper/find_dof_map_h1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17162 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/helper/find_dof_map_nd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7167 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/helper/formholder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/helper/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12545 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/helper/geom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5731 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/helper/global_named_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17496 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/helper/hcurl_normal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8838 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/helper/hierarchical_finite_element_spaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/helper/init_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/helper/load_mfem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5155 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/helper/matrix_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/helper/memory_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/helper/mpi_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15226 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/helper/mpi_recipes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12591 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/helper/numba_interp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8348 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/helper/numba_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32891 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/helper/operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8742 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/helper/phys_module_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/helper/pickle_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19046 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/helper/preconditioners.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5888 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/helper/projection.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/helper/restricte_integrator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/helper/right_broadcast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/helper/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3553 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/helper/validator_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)    94176 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/helper/variables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4506 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/init_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:12:41.189069 petram_base-2.1.38/petram/mesh/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/mesh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5244 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/mesh/composite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4458 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/mesh/find_edges.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5012 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/mesh/find_loop.py
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/mesh/find_vertex.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21368 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/mesh/geo_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7976 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/mesh/make_simplemesh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3559 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/mesh/mesh_extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6253 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/mesh/mesh_inspect.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39586 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/mesh/mesh_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9111 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/mesh/mesh_sel_buttons.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28650 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/mesh/mesh_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/mesh/mesh_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22038 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/mesh/nastran2mfem.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26567 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/mesh/partial_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8352 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/mesh/plot_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4954 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/mesh/pumimesh_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5906 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/mesh/read_mfemmesh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/mesh/read_mfemmesh1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4678 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/mesh/read_mfemmesh2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5982 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/mesh/read_mfemmesh2_old.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8380 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/mesh/read_mfemmesh3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/mesh/refined_mfem_geom.py
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/mfem_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16429 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/mfem_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66666 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/mfem_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34761 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12938 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/namespace_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:12:41.193069 petram_base-2.1.38/petram/phys/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/phys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8707 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/phys/aux_operator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13486 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/phys/aux_variable.py
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/phys/bc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20542 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/phys/coefficient.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:12:41.193069 petram_base-2.1.38/petram/phys/distance/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/phys/distance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7246 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/phys/distance/distance_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3309 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/phys/distance/wall.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41518 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/phys/numba_coefficient.py
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/phys/phys.py
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/phys/phys_const.py
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/phys/phys_cont.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46765 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/phys/phys_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/phys/projection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21717 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/phys/pycomplex_coefficient.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4903 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/phys/variable_coupling.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22796 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/phys/vtable.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19102 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/phys/weakform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:12:41.193069 petram_base-2.1.38/petram/phys/wf/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/phys/wf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2790 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/phys/wf/pix_gen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7801 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/phys/wf/wf_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13017 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/phys/wf/wf_essential.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10615 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/phys/wf/wf_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/phys/wf/wf_natural.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6153 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/phys/wf/wf_pairs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:12:41.197069 petram_base-2.1.38/petram/pi/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/pi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46766 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/pi/dlg_edit_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3426 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/pi/dlg_plot_expr.py
+-rw-r--r--   0 runner    (1001) docker     (127)   112653 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/pi/dlg_plot_sol.py
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/pi/dlg_progressbar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7905 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/pi/dlg_submit_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/pi/ns_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/pi/pfz2script.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:12:41.197069 petram_base-2.1.38/petram/pi/project_scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/pi/project_scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/pi/project_scripts/convert_mesh.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:12:41.201069 petram_base-2.1.38/petram/pi/project_scripts/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/pi/project_scripts/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/pi/project_scripts/helpers/call_glvis.py
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/pi/project_scripts/helpers/clear_sol.py
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/pi/project_scripts/helpers/convert_mfem_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/pi/project_scripts/helpers/create_ns.py
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/pi/project_scripts/helpers/eval_expr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/pi/project_scripts/helpers/init_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/pi/project_scripts/helpers/make_new_sol.py
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/pi/project_scripts/helpers/move_to_petram.py
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/pi/project_scripts/helpers/rebuild_ns.py
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/pi/project_scripts/helpers/reset_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/pi/project_scripts/helpers/save_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/pi/project_scripts/helpers/select_sol.py
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/pi/project_scripts/helpers/start_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2779 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/pi/project_scripts/run_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2850 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/pi/project_scripts/run_serial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8168 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/pi/sel_buttons.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17017 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/pi/selection_palette.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4045 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/pi/shell_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/pi/simple_frame_plus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3092 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/pi/widget_forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6400 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/pi/widget_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5627 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/pi/widget_nl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4755 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/pi/widget_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4952 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/pi/widget_smoother.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/pi/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:12:41.201069 petram_base-2.1.38/petram/postprocess/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/postprocess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14386 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/postprocess/discrt_v_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10015 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/postprocess/discrt_v_interpolator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5777 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/postprocess/pp_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9235 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/postprocess/project_solution.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:12:41.201069 petram_base-2.1.38/petram/remote/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12098 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/remote/client_script.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:12:41.205069 petram_base-2.1.38/petram/sol/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/sol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12203 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/sol/bdr_nodal_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5598 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/sol/edge_nodal_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/sol/evaluator_agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12681 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/sol/evaluator_cs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22480 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/sol/evaluator_mp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8017 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/sol/evaluator_single.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11010 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/sol/evaluators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3543 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/sol/integral_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/sol/listsoldir.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8484 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/sol/ncedge_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9975 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/sol/ncface_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5307 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/sol/nodal_refinement.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11070 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/sol/pointcloud_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4827 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/sol/probe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/sol/probe_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6335 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/sol/slice_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6581 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/sol/solsets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4894 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/sol/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:12:41.209069 petram_base-2.1.38/petram/solver/
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/solver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/solver/ams_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7165 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/solver/block_smoother.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7581 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/solver/distance_solver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20989 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/solver/egn_solver_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15664 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/solver/gmres_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22440 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/solver/iterative_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14278 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/solver/krylov.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9389 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/solver/linearsystem_reducer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22917 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/solver/mg_solver_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43412 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/solver/ml_solver_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45045 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/solver/mumps_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27200 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/solver/nl_solver_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14903 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/solver/parametric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5415 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/solver/parametric_scanner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/solver/set_var.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/solver/solinit_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3559 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/solver/solve_loop.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15237 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/solver/solver_controls.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34170 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/solver/solver_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5908 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/solver/solver_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3191 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/solver/std_meshadapt_solver_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10605 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/solver/std_solver_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9191 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/solver/std_solver_model_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/solver/std_solver_model_v3.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26454 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/solver/strumpack_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25617 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/solver/timedomain_solver_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7316 2024-04-25 14:12:33.000000 petram_base-2.1.38/petram/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 14:12:41.209069 petram_base-2.1.38/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-04-25 14:12:33.000000 petram_base-2.1.38/setup.py
```

### Comparing `PetraM_Base-2.1.30/LICENSE` & `petram_base-2.1.38/LICENSE`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/PKG-INFO` & `petram_base-2.1.38/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: PetraM_Base
-Version: 2.1.30
+Version: 2.1.38
 Summary: PetraM base package
 Home-page: https://github.com/piScope/PetraM
 Author: S. Shiraiwa
 Author-email: shiraiwa@prenceton.edu
 License: GNUv3
 Keywords: MFEM physics
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3.6
+Description-Content-Type: text/markdown
 License-File: LICENSE
 
-<img align="right" width="300" height="300" src="https://github.com/piScope/PetraM_Base/blob/job_submission_adjustment/resources/app_logo.png">
+<img align="right" width="300" height="300" src="https://github.com/piScope/PetraM_Base/blob/master/resources/app_logo.png?raw=true">
 
 ## PetraM_Base (Base Package for Petra-M)
 
 Petra-M (Physics Equation Translator for MFEM) is a physics layer built
 on the top of PyMFEM, a python wrapper for Modular FEM library
 (MFEM: http://mfem.org).
```

### Comparing `PetraM_Base-2.1.30/PetraM_Base.egg-info/PKG-INFO` & `petram_base-2.1.38/PetraM_Base.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: PetraM_Base
-Version: 2.1.30
+Version: 2.1.38
 Summary: PetraM base package
 Home-page: https://github.com/piScope/PetraM
 Author: S. Shiraiwa
 Author-email: shiraiwa@prenceton.edu
 License: GNUv3
 Keywords: MFEM physics
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3.6
+Description-Content-Type: text/markdown
 License-File: LICENSE
 
-<img align="right" width="300" height="300" src="https://github.com/piScope/PetraM_Base/blob/job_submission_adjustment/resources/app_logo.png">
+<img align="right" width="300" height="300" src="https://github.com/piScope/PetraM_Base/blob/master/resources/app_logo.png?raw=true">
 
 ## PetraM_Base (Base Package for Petra-M)
 
 Petra-M (Physics Equation Translator for MFEM) is a physics layer built
 on the top of PyMFEM, a python wrapper for Modular FEM library
 (MFEM: http://mfem.org).
```

### Comparing `PetraM_Base-2.1.30/PetraM_Base.egg-info/SOURCES.txt` & `petram_base-2.1.38/PetraM_Base.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -99,14 +99,15 @@
 petram/ext/__init__.py
 petram/helper/__init__.py
 petram/helper/block_matrix.py
 petram/helper/boundary_refinement.py
 petram/helper/cdict.py
 petram/helper/chypre_to_pymatrix.py
 petram/helper/convolve.py
+petram/helper/densemat2pymat.py
 petram/helper/direct_wrapper_call.py
 petram/helper/dof_map.py
 petram/helper/dof_mapping_matrix.py
 petram/helper/dot_dict.py
 petram/helper/driver_path.py
 petram/helper/dummy_mpi.py
 petram/helper/element_map.py
@@ -171,14 +172,15 @@
 petram/phys/numba_coefficient.py
 petram/phys/phys.py
 petram/phys/phys_const.py
 petram/phys/phys_cont.py
 petram/phys/phys_model.py
 petram/phys/projection.py
 petram/phys/pycomplex_coefficient.py
+petram/phys/variable_coupling.py
 petram/phys/vtable.py
 petram/phys/weakform.py
 petram/phys/distance/__init__.py
 petram/phys/distance/distance_model.py
 petram/phys/distance/wall.py
 petram/phys/wf/__init__.py
 petram/phys/wf/pix_gen.py
@@ -198,14 +200,15 @@
 petram/pi/sel_buttons.py
 petram/pi/selection_palette.py
 petram/pi/shell_commands.py
 petram/pi/simple_frame_plus.py
 petram/pi/widget_forms.py
 petram/pi/widget_init.py
 petram/pi/widget_nl.py
+petram/pi/widget_parameters.py
 petram/pi/widget_smoother.py
 petram/pi/widgets.py
 petram/pi/project_scripts/__init__.py
 petram/pi/project_scripts/convert_mesh.py
 petram/pi/project_scripts/run_parallel.py
 petram/pi/project_scripts/run_serial.py
 petram/pi/project_scripts/helpers/__init__.py
@@ -248,14 +251,15 @@
 petram/sol/slice_evaluator.py
 petram/sol/solsets.py
 petram/sol/test.py
 petram/solver/__init__.py
 petram/solver/ams_model.py
 petram/solver/block_smoother.py
 petram/solver/distance_solver.py
+petram/solver/egn_solver_model.py
 petram/solver/gmres_model.py
 petram/solver/iterative_model.py
 petram/solver/krylov.py
 petram/solver/linearsystem_reducer.py
 petram/solver/mg_solver_model.py
 petram/solver/ml_solver_model.py
 petram/solver/mumps_model.py
```

### Comparing `PetraM_Base-2.1.30/README.md` & `petram_base-2.1.38/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-<img align="right" width="300" height="300" src="https://github.com/piScope/PetraM_Base/blob/job_submission_adjustment/resources/app_logo.png">
+<img align="right" width="300" height="300" src="https://github.com/piScope/PetraM_Base/blob/master/resources/app_logo.png?raw=true">
 
 ## PetraM_Base (Base Package for Petra-M)
 
 Petra-M (Physics Equation Translator for MFEM) is a physics layer built
 on the top of PyMFEM, a python wrapper for Modular FEM library
 (MFEM: http://mfem.org).
```

### Comparing `PetraM_Base-2.1.30/petram/data/BilinearOps` & `petram_base-2.1.38/petram/data/BilinearOps`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/data/LinearOps` & `petram_base-2.1.38/petram/data/LinearOps`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/data/icon/form_BoundaryFlowIntegrator.png` & `petram_base-2.1.38/petram/data/icon/form_BoundaryFlowIntegrator.png`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/data/icon/form_BoundaryLFIntegrator.png` & `petram_base-2.1.38/petram/data/icon/form_BoundaryLFIntegrator.png`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/data/icon/form_BoundaryMassIntegrator.png` & `petram_base-2.1.38/petram/data/icon/form_BoundaryMassIntegrator.png`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/data/icon/form_BoundaryNormalLFIntegrator.png` & `petram_base-2.1.38/petram/data/icon/form_BoundaryNormalLFIntegrator.png`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/data/icon/form_BoundaryTangentialLFIntegrator.png` & `petram_base-2.1.38/petram/data/icon/form_BoundaryTangentialLFIntegrator.png`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/data/icon/form_ConvectionIntegrator.png` & `petram_base-2.1.38/petram/data/icon/form_ConvectionIntegrator.png`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/data/icon/form_CurlCurlIntegrator.png` & `petram_base-2.1.38/petram/data/icon/form_CurlCurlIntegrator.png`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/data/icon/form_DerivativeIntegrator1.png` & `petram_base-2.1.38/petram/data/icon/form_DerivativeIntegrator1.png`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/data/icon/form_DerivativeIntegrator2.png` & `petram_base-2.1.38/petram/data/icon/form_DerivativeIntegrator2.png`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/data/icon/form_DerivativeIntegrator3.png` & `petram_base-2.1.38/petram/data/icon/form_DerivativeIntegrator3.png`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/data/icon/form_DiffusionIntegrator.png` & `petram_base-2.1.38/petram/data/icon/form_DiffusionIntegrator.png`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/data/icon/form_DivDivIntegrator.png` & `petram_base-2.1.38/petram/data/icon/form_DivDivIntegrator.png`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/data/icon/form_DomainLFIntegrator.png` & `petram_base-2.1.38/petram/data/icon/form_DomainLFIntegrator.png`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/data/icon/form_ElasticityIntegrator.png` & `petram_base-2.1.38/petram/data/icon/form_ElasticityIntegrator.png`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/data/icon/form_GroupConvectionIntegrator.png` & `petram_base-2.1.38/petram/data/icon/form_GroupConvectionIntegrator.png`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/data/icon/form_MassIntegrator.png` & `petram_base-2.1.38/petram/data/icon/form_MassIntegrator.png`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/data/icon/form_MixedCrossCurlCurlIntegrator.png` & `petram_base-2.1.38/petram/data/icon/form_MixedCrossCurlCurlIntegrator.png`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/data/icon/form_MixedCrossCurlGradIntegrator.png` & `petram_base-2.1.38/petram/data/icon/form_MixedCrossCurlGradIntegrator.png`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/data/icon/form_MixedCrossCurlIntegrator.png` & `petram_base-2.1.38/petram/data/icon/form_MixedCrossCurlIntegrator.png`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/data/icon/form_MixedCrossGradCurlIntegrator.png` & `petram_base-2.1.38/petram/data/icon/form_MixedCrossGradCurlIntegrator.png`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/data/icon/form_MixedCrossGradGradIntegrator.png` & `petram_base-2.1.38/petram/data/icon/form_MixedCrossGradGradIntegrator.png`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/data/icon/form_MixedCrossGradIntegrator.png` & `petram_base-2.1.38/petram/data/icon/form_MixedCrossGradIntegrator.png`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/data/icon/form_MixedCrossProductIntegrator.png` & `petram_base-2.1.38/petram/data/icon/form_MixedCrossProductIntegrator.png`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/data/icon/form_MixedCurlCurlIntegrator.png` & `petram_base-2.1.38/petram/data/icon/form_MixedCurlCurlIntegrator.png`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/data/icon/form_MixedDirectionalDerivativeIntegrator.png` & `petram_base-2.1.38/petram/data/icon/form_MixedDirectionalDerivativeIntegrator.png`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/data/icon/form_MixedDivGradIntegrator.png` & `petram_base-2.1.38/petram/data/icon/form_MixedDivGradIntegrator.png`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/data/icon/form_MixedDotProductIntegrator.png` & `petram_base-2.1.38/petram/data/icon/form_MixedDotProductIntegrator.png`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/data/icon/form_MixedGradDivIntegrator.png` & `petram_base-2.1.38/petram/data/icon/form_MixedGradDivIntegrator.png`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/data/icon/form_MixedGradGradIntegrator.png` & `petram_base-2.1.38/petram/data/icon/form_MixedGradGradIntegrator.png`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/data/icon/form_MixedScalarCrossCurlIntegrator.png` & `petram_base-2.1.38/petram/data/icon/form_MixedScalarCrossCurlIntegrator.png`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/data/icon/form_MixedScalarCrossGradIntegrator.png` & `petram_base-2.1.38/petram/data/icon/form_MixedScalarCrossGradIntegrator.png`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/data/icon/form_MixedScalarCrossProductIntegrator.png` & `petram_base-2.1.38/petram/data/icon/form_MixedScalarCrossProductIntegrator.png`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/data/icon/form_MixedScalarCurlIntegrator.png` & `petram_base-2.1.38/petram/data/icon/form_MixedScalarCurlIntegrator.png`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/data/icon/form_MixedScalarDerivativeIntegrator.png` & `petram_base-2.1.38/petram/data/icon/form_MixedScalarDerivativeIntegrator.png`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/data/icon/form_MixedScalarDivergenceIntegrator.png` & `petram_base-2.1.38/petram/data/icon/form_MixedScalarDivergenceIntegrator.png`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/data/icon/form_MixedScalarMassIntegrator.png` & `petram_base-2.1.38/petram/data/icon/form_MixedScalarMassIntegrator.png`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/data/icon/form_MixedScalarWeakCrossProductIntegrator.png` & `petram_base-2.1.38/petram/data/icon/form_MixedScalarWeakCrossProductIntegrator.png`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/data/icon/form_MixedScalarWeakCurlCrossIntegrator.png` & `petram_base-2.1.38/petram/data/icon/form_MixedScalarWeakCurlCrossIntegrator.png`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/data/icon/form_MixedScalarWeakCurlIntegrator.png` & `petram_base-2.1.38/petram/data/icon/form_MixedScalarWeakCurlIntegrator.png`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/data/icon/form_MixedScalarWeakDerivativeIntegrator.png` & `petram_base-2.1.38/petram/data/icon/form_MixedScalarWeakDerivativeIntegrator.png`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/data/icon/form_MixedScalarWeakDivergenceIntegrator.png` & `petram_base-2.1.38/petram/data/icon/form_MixedScalarWeakDivergenceIntegrator.png`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/data/icon/form_MixedScalarWeakGradientIntegrator.png` & `petram_base-2.1.38/petram/data/icon/form_MixedScalarWeakGradientIntegrator.png`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/data/icon/form_MixedVectorCurlIntegrator.png` & `petram_base-2.1.38/petram/data/icon/form_MixedVectorCurlIntegrator.png`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/data/icon/form_MixedVectorDivergenceIntegrator.png` & `petram_base-2.1.38/petram/data/icon/form_MixedVectorDivergenceIntegrator.png`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/data/icon/form_MixedVectorGradientIntegrator.png` & `petram_base-2.1.38/petram/data/icon/form_MixedVectorGradientIntegrator.png`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/data/icon/form_MixedVectorMassIntegrator.png` & `petram_base-2.1.38/petram/data/icon/form_MixedVectorMassIntegrator.png`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/data/icon/form_MixedVectorProductIntegrator.png` & `petram_base-2.1.38/petram/data/icon/form_MixedVectorProductIntegrator.png`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/data/icon/form_MixedVectorWeakCurlIntegrator.png` & `petram_base-2.1.38/petram/data/icon/form_MixedVectorWeakCurlIntegrator.png`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/data/icon/form_MixedVectorWeakDivergenceIntegrator.png` & `petram_base-2.1.38/petram/data/icon/form_MixedVectorWeakDivergenceIntegrator.png`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/data/icon/form_MixedWeakCurlCrossIntegrator.png` & `petram_base-2.1.38/petram/data/icon/form_MixedWeakCurlCrossIntegrator.png`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/data/icon/form_MixedWeakDivCrossIntegrator.png` & `petram_base-2.1.38/petram/data/icon/form_MixedWeakDivCrossIntegrator.png`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/data/icon/form_MixedWeakGradDotIntegrator.png` & `petram_base-2.1.38/petram/data/icon/form_MixedWeakGradDotIntegrator.png`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/data/icon/form_VectorBoundaryFluxLFIntegrator.png` & `petram_base-2.1.38/petram/data/icon/form_VectorBoundaryFluxLFIntegrator.png`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/data/icon/form_VectorBoundaryLFIntegrator.png` & `petram_base-2.1.38/petram/data/icon/form_VectorBoundaryLFIntegrator.png`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/data/icon/form_VectorCurlCurlIntegrator.png` & `petram_base-2.1.38/petram/data/icon/form_VectorCurlCurlIntegrator.png`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/data/icon/form_VectorDiffusionIntegrator.png` & `petram_base-2.1.38/petram/data/icon/form_VectorDiffusionIntegrator.png`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/data/icon/form_VectorDivergenceIntegrator.png` & `petram_base-2.1.38/petram/data/icon/form_VectorDivergenceIntegrator.png`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/data/icon/form_VectorDomainLFIntegrator.png` & `petram_base-2.1.38/petram/data/icon/form_VectorDomainLFIntegrator.png`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/data/icon/form_VectorFEBoundaryFluxLFIntegrator.png` & `petram_base-2.1.38/petram/data/icon/form_VectorFEBoundaryFluxLFIntegrator.png`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/data/icon/form_VectorFEBoundaryTangentLFIntegrator.png` & `petram_base-2.1.38/petram/data/icon/form_VectorFEBoundaryTangentLFIntegrator.png`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/data/icon/form_VectorFECurlIntegrator.png` & `petram_base-2.1.38/petram/data/icon/form_VectorFECurlIntegrator.png`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/data/icon/form_VectorFEDivergenceIntegrator.png` & `petram_base-2.1.38/petram/data/icon/form_VectorFEDivergenceIntegrator.png`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/data/icon/form_VectorFEDomainLFIntegrator.png` & `petram_base-2.1.38/petram/data/icon/form_VectorFEDomainLFIntegrator.png`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/data/icon/form_VectorFEMassIntegrator.png` & `petram_base-2.1.38/petram/data/icon/form_VectorFEMassIntegrator.png`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/data/icon/form_VectorFEWeakDivergenceIntegrator.png` & `petram_base-2.1.38/petram/data/icon/form_VectorFEWeakDivergenceIntegrator.png`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/data/icon/form_VectorMassIntegrator.png` & `petram_base-2.1.38/petram/data/icon/form_VectorMassIntegrator.png`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/data/icon/form_none.png` & `petram_base-2.1.38/petram/data/icon/form_none.png`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/data/icon/hide.png` & `petram_base-2.1.38/petram/data/icon/hide.png`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/debug.py` & `petram_base-2.1.38/petram/debug.py`

 * *Files 0% similar despite different names*

```diff
@@ -266,8 +266,8 @@
         traceback.print_stack()
         dprint1(message)
     elif get_allow_python_function_coefficient() == "ignore":
         pass
     elif get_allow_python_function_coefficient() == "always use Python coeff.":
         pass
     elif get_allow_python_function_coefficient() == "error":
-        assert False, message
+        assert False, message + " (Python mode not allowed)"
```

### Comparing `PetraM_Base-2.1.30/petram/engine.py` & `petram_base-2.1.38/petram/engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,17 +24,17 @@
 
 from petram.model import Domain, Bdry, Point, Pair
 
 import petram.debug
 dprint1, dprint2, dprint3 = petram.debug.init_dprints('Engine')
 
 # if you need to turn a specific warning to exception
-#import scipy.sparse
-#import warnings
-#warnings.filterwarnings('error', category=scipy.sparse.SparseEfficiencyWarning)
+# import scipy.sparse
+# import warnings
+# warnings.filterwarnings('error', category=scipy.sparse.SparseEfficiencyWarning)
 
 
 def iter_phys(phys_targets, *args):
     for phys in phys_targets:
         yield [phys] + [a[phys] for a in args]
 
 
@@ -107,16 +107,16 @@
     def initialize_datastorage(self):
         self.is_assembled = False
         self.is_initialized = False
         self.meshes = []
         self.emeshes = []
         self.emesh_data = None
         # place holder max level 10
-        #self._fec_storage = {}
-        #self._fes_storage = {}
+        # self._fec_storage = {}
+        # self._fes_storage = {}
         self.pp_extra = {}
         self.alloc_flag = {}
         self.initialize_fespaces()
 
     def initialize_fespaces(self):
         from petram.helper.hierarchical_finite_element_spaces import HierarchicalFiniteElementSpaces
         self._fespace_hierarchy = HierarchicalFiniteElementSpaces(owner=self)
@@ -233,14 +233,15 @@
                           for k in range(n_mat)])
         self._i_x.append([FormBlock(n_rfes, new=self.alloc_gf)
                           for k in range(n_mat)])
         self._r_b.append(FormBlock(n_fes, new=self.alloc_lf))
         self._i_b.append(FormBlock(n_fes, new=self.alloc_lf))
 
         self._extras.append([None for i in range(n_mat)])
+        self._cextras.append([None for i in range(n_mat)])
         self._aux_ops.append([None for i in range(n_mat)])
 
         self._interps.append({})
         self._projections.append({})
         self._projections_hash.append({})
         self._gl_ess_tdofs.append({n: [] for n in self.fes_vars})
         self._ess_tdofs.append({n: [] for n in self.fes_vars})
@@ -251,14 +252,15 @@
         self._r_at = []
         self._i_at = []
         self._r_b = []
         self._i_b = []
         self._r_x = []
         self._i_x = []
         self._extras = []
+        self._cextras = []
         self._aux_ops = []
         self._interps = []
         self._projections = []
         self._projections_hash = []
         self._gl_ess_tdofs = []
         self._ess_tdofs = []
 
@@ -371,14 +373,22 @@
         return self._extras[self._level_idx][self._access_idx]
 
     @extras.setter
     def extras(self, v):
         self._extras[self._level_idx][self._access_idx] = v
 
     @property
+    def cextras(self):
+        return self._cextras[self._level_idx][self._access_idx]
+
+    @cextras.setter
+    def cextras(self, v):
+        self._cextras[self._level_idx][self._access_idx] = v
+
+    @property
     def aux_ops(self):
         return self._aux_ops[self._level_idx][self._access_idx]
 
     @aux_ops.setter
     def aux_ops(self, v):
         self._aux_ops[self._level_idx][self._access_idx] = v
 
@@ -803,27 +813,31 @@
                         init_value=0.0, init_path='', init_dwc=("", ""), init_var=""):
         # mode
         #  0: zero
         #  1: init to constant
         #  2: use init panel values
         #  3: load file
         #  4: do nothing
-        dprint1("run_apply_init0", phys_range, mode)
+        dprint1("run_apply_init0", phys_range, mode, init_var)
+
+        init_var_names = [x.strip() for x in init_var.split(",")]
         for j in range(self.n_matrix):
             self.access_idx = j
             if not self.is_matrix_active(j):
                 continue
 
             if mode in [0, 1, 2, 3, 4]:
                 for phys in phys_range:
                     names = phys.dep_vars
                     if mode == 0:
                         for name in names:
-                            if init_var != "" and name != init_var:
+                            if init_var != "" and name not in init_var_names:
                                 continue
+                            dprint1(
+                                "applying value=0 to entire discrete space:" + name, init_value)
 
                             r_ifes = self.r_ifes(name)
                             rgf = self.r_x[r_ifes]
                             igf = self.i_x[r_ifes]
                             rgf.Assign(0.0)
                             if igf is not None:
                                 igf.Assign(0.0)
@@ -832,15 +846,15 @@
                     elif mode == 1:
                         from petram.helper.variables import project_variable_to_gf
 
                         global_ns = phys._global_ns.copy()
                         for key in self.model.root()._variables:
                             global_ns[key] = self.model.root()._variables[key]
                         for name in names:
-                            if init_var != "" and name != init_var:
+                            if init_var != "" and name not in init_var_names:
                                 continue
                             r_ifes = self.r_ifes(name)
                             rgf = self.r_x[r_ifes]
                             igf = self.i_x[r_ifes]
                             ind_vars = phys.ind_vars
                             dprint1(
                                 "applying init value to entire discrete space:" + name, init_value)
@@ -898,20 +912,25 @@
                     if igf is not None:
                         igf.Assign(0.0)
 
     def run_apply_init(self, phys_range, inits=None):
         if len(inits) == 0:
             self.run_apply_init_autozero(phys_range)
         else:
+            all_tmp = []
             for init in inits:
                 tmp = init.run(self)
-                phys_range = [phys for phys in phys_range if not phys in tmp]
-            if len(phys_range) > 0:
+                for x in tmp:
+                    if x not in all_tmp:
+                        all_tmp.append(x)
+            xphys_range = [phys.name() for phys in phys_range if not phys in all_tmp]
+            if len(xphys_range) > 0:
                 dprint1(
-                    "!!!!! These phys are not initiazliaed (FES variable is not available)!!!!!", phys_range)
+                    "!!!!! These phys are not initiazliaed (FES variable is not available)!!!!!",
+                    xphys_range)
 
     def run_apply_essential(self, phys_target, phys_range, update=False):
         L = len(self.r_dep_vars)
         self.mask_X = np.array([not update]*L*self.n_matrix,
                                dtype=bool).reshape(-1, L)
 
         self.gl_ess_tdofs = {n: ([], []) for n in self.fes_vars}
@@ -939,15 +958,16 @@
                                dtype=bool).reshape(-1, R, C)
 
         for phys in phys_target:
             self.assemble_interp(phys)  # global interpolation (periodic BC)
             # global interpolation (mesh coupling)
             self.assemble_projection(phys)
 
-        self.extras_mm = {}
+        self.extras_mm = {}       # FES-extra connection
+        self.cextras_mm = {}      # extra-extra connection
 
         for j in range(self.n_matrix):
             self.access_idx = j
             for phys in phys_target:
                 for mm in phys.walk_enabled():
                     mm.compile_coeffs()
 
@@ -977,14 +997,16 @@
                     try:
                         form.Assemble(0)
                     except BaseException:
                         print("failed to assemble (r, c) = ", r1, c1)
                         raise
 
             self.extras = {}
+            self.cextras = {}
+
             updated_extra = []
             for phys in phys_target:
                 keys_to_update = self.extra_update_check_M(phys, phys_range)
 
                 if update:
                     self.assemble_extra(phys, phys_range, keys_to_update)
                 else:
@@ -1022,15 +1044,15 @@
                                dtype=bool).reshape(-1, R, C)
 
         for phys in phys_target:
             self.assemble_interp(phys)  # global interpolation (periodic BC)
             # global interpolation (mesh coupling)
             self.assemble_projection(phys)
 
-        #self.extras_mm = {}
+        # self.extras_mm = {}
 
         for j in range(self.n_matrix):
             self.access_idx = j
             if not self.is_matrix_active(j):
                 continue
 
             # self.extras = {} (we keep old extra and update only where it is needed)
@@ -1139,39 +1161,89 @@
 
         # B.save_to_file("B")
         # M[0].save_to_file("M0")
         # M[1].save_to_file("M1")
         # X[0].save_to_file("X0")
         A2, isAnew = compute_A(M, B, X,
                                self.mask_M,
-                               self.mask_B)  # solver determins A
+                               self.mask_B)  # solver determines A
 
         if isAnew:
             # generate Ae and eliminated A
             A, Ae = self.fill_BCeliminate_matrix(A2, B,
                                                  inplace=inplace,
                                                  update=update)
 
         RHS = compute_rhs(M, B, X)          # solver determins RHS
         RHS = self.eliminateBC(Ae, X[0], RHS)  # modify RHS and
 
         # A and RHS is modifedy by global DoF coupling P
         A, RHS = self.apply_interp(A, RHS)
 
-        # RHS.save_to_file("RHS")
-        # M[0].save_to_file("M0there2")
-        # M[1].save_to_file("M1")
-        # X[0].save_to_file("X0")
-        # RHS.save_to_file("RHS")
-
         # = [A, X, RHS, Ae,  B,  M, self.dep_vars[:]]
         self.assembled_blocks = [A, X, RHS, Ae,  B,  M, self.dep_vars[:]]
 
         return self.assembled_blocks, M_changed
 
+    def run_assemble_blocks_egn(self, inplace=True, update=False):
+        '''
+        Generate blocks for eigenvalue  problem.
+        Quadratic eigenvalue problem is assumed
+        l^2 K + l C +  M = 0
+
+        where K = M[2], C = M[1] and M = M[0], respectively
+
+        for now M[2] = 0
+
+        output is AA and BB to defien a linearlized general eigenvalue prob.
+          AA x = l BB x
+        '''
+        if update:
+            M = self.assembled_blocks[5]
+            B = self.assembled_blocks[4]
+            X = self.assembled_blocks[1]
+            Ae = self.assembled_blocks[3]
+            A = self.assembled_blocks[0]
+        else:
+            M, B = self.prepare_M_B_blocks()
+            X = self.assembled_blocks[1]
+            Ae = None
+
+        M, B, M_changed = self.fill_M_B_blocks(M, B, update=update)
+
+        if len(M) < 3:
+            assert False, "Eigenvalue problem is not well defined"
+
+        is_quad = False
+        if not M[1].is_zero:
+            assert False, "Quadratic Eigenvalue problem is not yet supported"
+            is_quad = True
+        else:
+            CC = None
+
+        KK = M[2]
+        isKKnew = np.any(self.mask_M[2])
+        MM = M[0]
+        isMMnew = np.any(self.mask_M[0])
+
+        if isMMnew:
+            MM = self.eliminate_BC_egn(MM, diag=1.0, inplace=inplace)
+        if isKKnew:
+            KK = self.eliminate_BC_egn(KK, diag=1e-300, inplace=inplace)
+
+        if is_quad:
+            pass
+        else:
+            AA = MM
+            BB = KK
+
+        self.assembled_blocks = [AA, BB,  X, B,  M, self.dep_vars[:]]
+
+        return self.assembled_blocks, M_changed
+
     def run_update_B_blocks(self):
         '''
         assemble M, B, X blockmatrices.
 
         in parallel, inplace = False makes sure that blocks in A and RHS  
         are not shared by M, B, X
         '''
@@ -1573,16 +1645,16 @@
                 continue
 
             loc_list = mm.get_mixedbf_loc()
 
             for loc in loc_list:
                 r, c, is_trans, is_conj = loc
                 if isinstance(r, int):
-                    #idx1 = phys_offset + r
-                    #idx2 = rphys_offset + c
+                    # idx1 = phys_offset + r
+                    # idx2 = rphys_offset + c
                     idx1 = self.ifes(phys.dep_vars[r])
                     idx2 = self.r_ifes(phys.dep_vars[c])
                 else:
                     idx1 = self.ifes(r)
                     idx2 = self.r_ifes(c)
                 if loc[2] < 0:
                     idx1, idx2 = idx2, idx1
@@ -1627,16 +1699,16 @@
             for loc in loc_list:
                 r, c, is_trans, is_conj = loc
 
                 is_trans = (is_trans < 0)
                 is_conj = (is_conj == -1)
 
                 if isinstance(r, int):
-                    #idx1 = phys_offset + r
-                    #idx2 = rphys_offset + c
+                    # idx1 = phys_offset + r
+                    # idx2 = rphys_offset + c
                     idx1 = self.ifes(phys.dep_vars[r])
                     idx2 = self.r_ifes(phys.dep_vars[c])
                 else:
                     idx1 = self.ifes(r)
                     idx2 = self.r_ifes(c)
 
                 if is_trans:
@@ -1731,14 +1803,21 @@
 
                     if key in self.extras and keys_to_update is None:
                         assert False, "extra with key= " + \
                             str(key) + " already exists."
                     self.extras[key] = tmp
                     self.extras_mm[key] = mm.fullpath()
 
+            if mm.has_extra_coupling():
+                extra_name, coupled_names = mm.extra_coupling_names()
+                for n in coupled_names:
+                    t1, t2 = mm.get_extra_coupling(n)
+                    key = (extra_name, n)
+                    self.cextras[key] = (t1, t2)
+
     def _extra_update_check(self, phys, phys_range, mode='B'):
         updated_name = []
         for mm in phys.walk():
             if not mm.enabled:
                 continue
             for phys2 in phys_range:
                 names = phys2.dep_vars
@@ -1930,18 +2009,25 @@
 
                 T1 = self.t1_2_T1(t1, x)
                 T2 = self.t2_2_T2(t2, x)
 
                 if r1 != -1:
                     M[k][r1, c1] = T1 if M[k][r1, c1] is None else M[k][r1, c1]+T1
                 M[k][r, c] = T2 if M[k][r, c] is None else M[k][r, c]+T2
-                #M[k][r,r] = t3 if M[k][r,r] is None else M[k][r,r]+t3
+                # M[k][r,r] = t3 if M[k][r,r] is None else M[k][r,r]+t3
                 M[k][r, c1] = t3 if M[k][r, c1] is None else M[k][r, c1]+t3
 
-            #print("aux", k, self.aux_ops.keys())
+            for extra_name1, extra_name2 in self.cextras.keys():
+                r = self.dep_var_offset(extra_name1)
+                c = self.r_dep_var_offset(extra_name2)
+                t1, t2 = self.cextras[(extra_name1, extra_name2)]
+                M[k][r, c] = t1 if M[k][r, c] is None else M[k][r, c]+t1
+                M[k][c, r] = t2 if M[k][c, r] is None else M[k][c, r]+t2
+
+            # print("aux", k, self.aux_ops.keys())
             for key in self.aux_ops.keys():
                 testname, trialname, mm_fullpath = key
                 r = self.dep_var_offset(testname)
                 c = self.r_dep_var_offset(trialname)
                 if update and not self.mask_M[k, r, c]:
                     continue
 
@@ -2116,14 +2202,16 @@
                 if AeX[idx, 0] is not None:
                     AeX[idx, 0].resetRow(gl_ess_tdof1)
 
             RHS = RHS - AeX
         except:
             print("Ae", Ae)
             print("X", X)
+            print("AeX", AeX)
+            print("RHS", RHS)
             raise
 
         for name in self.gl_ess_tdofs:
             if not name in self._dep_vars:
                 continue
 
             idx = self.dep_var_offset(name)
@@ -2133,14 +2221,78 @@
 
             x1 = X[ridx].get_elements(gl_ess_tdof1)
             x2 = RHS[idx].get_elements(gl_ess_tdof1)
             RHS[idx].set_elements(gl_ess_tdof1, x1*x2)
 
         return RHS
 
+    def eliminate_BC_egn(self, A, diag=1.0, inplace=True):
+        '''
+        essential BC elimination for eigenmode solver
+        '''
+        diagpolicy = self.get_diagpolicy()
+
+        nblock1 = A.shape[0]
+        nblock2 = A.shape[1]
+
+        for name in self.gl_ess_tdofs:
+            # we do elimination only for the varialbes to be solved
+            if not name in self._dep_vars:
+                continue
+
+            gl_ess_tdof1, gl_ess_tdof2 = self.gl_ess_tdofs[name]
+            ess_tdof1, ess_tdof2 = self.ess_tdofs[name]
+            idx1 = self.dep_var_offset(name)
+            idx2 = self.r_dep_var_offset(name)
+
+            if A[idx1, idx2] is None:
+                A.add_empty_square_block(idx1, idx2)
+
+            if A[idx1, idx2] is not None:
+                # note: this check is necessary, since in parallel environment,
+                # add_empty_square_block could not create any block because
+                # locally number or rows is zero.
+                if self.get_autofill_diag():
+                    self.fill_empty_diag(A[idx1, idx2])
+
+                A[idx1, idx2] = A[idx1, idx2].resetRow(
+                    gl_ess_tdof1, inplace=inplace)
+                A[idx1, idx2] = A[idx1, idx2].resetCol(
+                    gl_ess_tdof1, inplace=inplace)
+                A[idx1, idx2].setDiag(gl_ess_tdof1, diag)
+
+            '''
+            note: minor differece between serial/parallel
+ 
+            Aee in serial ana parallel are not equal. The definition of Aee in MFEM is
+            A_original = Aee + A, where A_diag is set to one for Esseential DoF
+            In the serial mode, Aee_diag is not properly set. But this element
+            does not impact the final RHS.
+            '''
+            for j in range(nblock2):
+                if j == idx2:
+                    continue
+                if A[idx1, j] is None:
+                    continue
+
+                A[idx1, j] = A[idx1, j].resetRow(gl_ess_tdof1, inplace=inplace)
+                if not (idx1, j) in self._aux_essential and len(gl_ess_tdof2) > 0:
+                    A[idx1, j] = A[idx1, j].resetRow(
+                        gl_ess_tdof2, inplace=inplace)
+
+            for j in range(nblock1):
+                if j == idx1:
+                    continue
+                if A[j, idx2] is None:
+                    continue
+
+                A[j, idx2] = A[j, idx2].resetCol(gl_ess_tdof1, inplace=inplace)
+
+        return A
+
     def collect_local_ess_TDofs(self, opr, format, is_complex):
         '''
         Find essential TDoFs index in solution block vector
 
         this method assumes format is either (blk_interleave, blk_merged, blk_merged_s)
         '''
         nblock1 = opr.NumColBlocks()
@@ -2186,15 +2338,15 @@
         if P is not None: 
               [ P A P^t  P B ][y]   [P b]
               [              ][ ] = [   ]
               [ C P^t     D  ][l]   [ c ]
         and 
              x  = P^t y
         '''
-        #import traceback
+        # import traceback
         # traceback.print_stack()
         for name in self.interps:
             idx1 = self.dep_var_offset(name)
             idx2 = self.r_dep_var_offset(name)
             P, nonzeros, zeros = self.interps[name]
             if P is None:
                 continue
@@ -2354,15 +2506,15 @@
         return B
     #
     #  processing solution
     #
 
     def split_sol_array(self, sol):
         s = [None]*len(self.r_fes_vars)
-        #nicePrint("sol", sol, self._rdep_vars)
+        # nicePrint("sol", sol, self._rdep_vars)
         for name in self.fes_vars:
             # print name
             j = self.r_dep_var_offset(name)
             sol_section = sol[j, 0]
 
             if name in self.interps:
                 P, nonzeros, zeros = self.interps[name]
@@ -2373,15 +2525,15 @@
             s[ifes] = sol_section
             sol[j, 0] = sol_section
 
         e = []
         for name in self.dep_vars:
             if not self.isFESvar(name):
                 e.append(sol[self.dep_var_offset(name)])
-        #nicePrint(s, e)
+        # nicePrint(s, e)
         return s, e
 
     def recover_sol(self, sol, access_idx=0):
         self.access_idx = access_idx
 
         for k, s in enumerate(sol):
             if s is None:
@@ -2436,15 +2588,15 @@
                 mm.postprocess_extra(None, t5, ret[extra_name])
             else:
                 mm.postprocess_extra(data, t5, ret[extra_name])
             '''
         for k in ret:
             tmp = {x: ret[k][x].flatten() for x in ret[k]}
             tmp2 = {x: ret[k][x].flatten() for x in ret[k] if x in print_flag}
-            dprint1("extra (diagnostic)", tmp2)
+            dprint1("extra (diagnostic) (at rank=0)", tmp2)
         return ret
 
     #
     #  save to file
     #
 
     def save_sol_to_file(self, phys_target, skip_mesh=False,
@@ -2581,15 +2733,15 @@
         self.save_extra_to_file(extra, extrafile_name=name + '.data')
 
     #
     #  helper methods
     #
     def assign_phys_pp_sel_index(self):
         if len(self.meshes) == 0:
-            #dprint1('!!!! mesh is None !!!!')
+            # dprint1('!!!! mesh is None !!!!')
             return
         all_phys = [self.model['Phys'][k] for
                     k in self.model['Phys'].keys()]
         all_pp = []
         for k in self.model['PostProcess']:
             for kk in self.model['PostProcess'][k]:
                 all_pp.append(self.model['PostProcess'][k][kk])
@@ -2608,15 +2760,15 @@
             alls = list(ec['surf2line']) if ec['surf2line'] is not None else []
             alle = list(ec['line2vert']) if ec['line2vert'] is not None else []
 
             p.update_dom_selection(all_sel=(allv, alls, alle))
 
     def assign_sel_index(self, phys=None):
         if len(self.meshes) == 0:
-            #dprint1('!!!! mesh is None !!!!')
+            # dprint1('!!!! mesh is None !!!!')
             return
         if phys is None:
             all_phys = [self.model['Phys'][k] for
                         k in self.model['Phys'].keys()]
         else:
             all_phys = [phys]
 
@@ -2768,15 +2920,15 @@
             if len(ptx1) > 0:
                 tmp = self.get_point_essential_tdofs(fespace, ptx1)
                 self.ess_tdofs[name][0].extend(tmp)
             if len(ptx2) > 0:
                 tmp = self.get_point_essential_tdofs(fespace, ptx2)
                 self.ess_tdofs[name][1].extend(tmp)
 
-            #print(name, len(self.ess_tdofs[name]))
+            # print(name, len(self.ess_tdofs[name]))
         return
 
     def allocate_fespace(self, phys):
         num_fec = len(phys.get_fec())
 
         count = 0
         for name, elem in phys.get_fec():
@@ -2804,15 +2956,15 @@
         sdim = mesh.SpaceDimension()
         dim = mesh.Dimension()
 
         is_new = False
         key = (emesh_idx, elem, order, dim, sdim, vdim, isParMesh)
         dkey = ("emesh_idx", "elem", "order",
                 "dim", "sdim", "vdim", "isParMesh")
-        #dprint1("Allocate/Reuse fec/fes:", {d: v for d, v in zip(dkey, key)})
+        # dprint1("Allocate/Reuse fec/fes:", {d: v for d, v in zip(dkey, key)})
 
         dprint1("Looking for already allocated fespaces ", name)
         if name in self.fespaces:
             fes1 = self.fespaces[name]
             isFESparallel = hasattr(fes1, 'GroupComm')
             if isFESparallel == isParMesh:
                 return False, fes1
@@ -2835,15 +2987,15 @@
                                     parameters=(emesh_idx, element, order, fecdim, vdim))
         fes1 = self.fespaces[name]
 
         return True, fes1
 
     # mesh.GetEdgeVertexTable()
     #        self._fes_storage[key] = fes
-        #self.add_fec_fes(name, fec, fes)
+        # self.add_fec_fes(name, fec, fes)
 
     # def add_fec_fes(self, name, fec, fes):
     #    self.fec[name] = fec
     #    self.fespaces[name] = fes
     def prepare_refined_level(self, phys, mode, inc=1, refine_dom=None):
         '''
         mode = 'H' or 'P'
@@ -2909,15 +3061,15 @@
             dprint1(
                 "fes1 and fes2 are on different mesh. Constructing a DoF map.", name1, name2)
             dprint1("info1", info1)
             dprint1("info2", info2)
 
             name = name2 + '_to_' + name1
             namehash = str(hash(tuple(info1.items()))) + \
-                "___" + str(hash(tuple(info1.items())))
+                "___" + str(hash(tuple(info2.items())))
             self.projections_hash[name] = namehash
 
             if abs(info1["dim"]-info2["dim"]) > 1:
                 assert False, "does not support direct mapping from volume to edge (or face to vertex)"
 
             from petram.helper.projection import simple_projection, fes_mapping
 
@@ -2933,30 +3085,30 @@
                 fes1 = fes2
                 fes2 = _fes2
                 transpose = True
             '''
             el, order, mbfdim = fes_mapping(info2["element"], info2["order"], info2["dim"],
                                             info1["dim"])
 
-            #emesh_idx = info2["emesh_idx"] if mbfdim == 1 else info1["emesh_idx"]
+            # emesh_idx = info2["emesh_idx"] if mbfdim == 1 else info1["emesh_idx"]
             emesh_idx = info1["emesh_idx"]
             is_new, fes = self.get_or_allocate_fecfes(name,
                                                       emesh_idx,
                                                       el,
                                                       order,
                                                       info2["vdim"])
 
             if namehash not in self.projections:
                 if info2["dim"]-info1["dim"] == 1:  # (ex)volume to surface
                     mode = "boundary"
                 elif info2["dim"]-info1["dim"] == 0:
                     mode = "domain"
                 else:
                     mode = "domain"
-                #assert False, "should not come here."
+                # assert False, "should not come here."
 
                 # fes2  -> fes (intermediate space using fes1's mesh)
                 p = simple_projection(fes2, fes, mode)
 
                 self.projections[namehash] = p
                 '''
                 if transpose:
@@ -2986,15 +3138,15 @@
 
                 except Exception as e:
                     node._global_ns = {}
                     m = traceback.format_exc()
                     errors.append("failed to build ns for " + node.fullname() +
                                   "\n" + m)
             else:
-                #node._global_ns = None
+                # node._global_ns = None
                 node._local_ns = self.model.root()._variables
 
         if len(errors) > 0:
             dprint1("\n".join(errors), notrim=True)
             assert False, "\n".join(errors)
 
     def preprocess_ns(self, ns_folder, data_folder):
@@ -3019,15 +3171,15 @@
         if self.emesh_data is None:
             self.reset_emesh_data()
 
     def run_mesh_serial(self, meshmodel=None,
                         skip_refine=False):
 
         from petram.mesh.mesh_model import MeshFile, MFEMMesh
-        #from petram.mesh.mesh_extension import MeshExt
+        # from petram.mesh.mesh_extension import MeshExt
         from petram.mesh.mesh_utils import get_extended_connectivity
 
         self.meshes = []
         self.prep_emesh_data_ifneeded()
         # if self.emesh_data is None:
         #    self.emesh_data = MeshExt()
         self.emeshes = []
@@ -3766,15 +3918,15 @@
         return a.SpMat()
 
     def b2B(self, b):  # FormLinearSystem w/o elimination
         fes = b.FESpace()
         B = mfem.Vector()
         if not fes.Conforming():
             P = fes.GetConformingProlongation()
-            #R = fes.GetConformingRestriction()
+            # R = fes.GetConformingRestriction()
             # if R is not None:
             if P is not None:
                 B.SetSize(P.Width())
                 P.MultTranspose(b, B)
             else:
                 B.NewDataAndSize(b.GetData(), b.Size())
         else:
@@ -3847,15 +3999,15 @@
         A is ScipyCoo (this one fully supports complex)
         '''
         csr = A.tocsr()
         csr.eliminate_zeros()
         zerorows = np.where(np.diff(csr.indptr) == 0)[0]
         if len(zerorows) == csr.shape[0]:
             dprint1(
-                "!!! skipping fill_empty_diag: this diagonal block is compltely zero")
+                "!!! skipping fill_empty_diag: this diagonal block is completely zero")
             return
         lil = A.tolil()
         lil[zerorows, zerorows] = 1.0
         coo = lil.tocoo()
         A.data = coo.data
         A.row = coo.row
         A.col = coo.col
@@ -3928,15 +4080,15 @@
                             smesh = srefine.run(smesh)
 
                         self.base_meshes[idx] = mfem.ParMesh(
                             MPI.COMM_WORLD, smesh, parts)
                         self.meshes[idx] = self.base_meshes[idx]
                         target = self.meshes[idx]
 
-                        #self.base_meshes[idx] = self.meshes[idx]
+                        # self.base_meshes[idx] = self.meshes[idx]
                     else:
                         if hasattr(o, 'run') and target is not None:
                             if o.isSerialRefinement:
                                 continue
                             target = self.new_mesh_from_mesh(target)
                             self.meshes[idx] = o.run(target)
                             target = self.meshes[idx]
@@ -4064,28 +4216,28 @@
         if P is not None:
             sol0 = (P.transpose()).dot(sol0)
         return sol0
 
     def collect_all_ess_tdof(self, M=None):
         from mpi4py import MPI
 
-        #gl_ess_tdofs = []
+        # gl_ess_tdofs = []
         # for name in phys.dep_vars:
         #    fes = self.fespaces[name]
 
         for name in self.ess_tdofs:
             tdof1, tdof2 = self.ess_tdofs[name]
             myoffset = self.fespaces[name].GetMyTDofOffset()
             data1 = (np.array(tdof1) + myoffset).astype(np.int32)
             data2 = (np.array(tdof2) + myoffset).astype(np.int32)
 
             gl_ess_tdof1 = allgather_vector(data1, MPI.INT)
             gl_ess_tdof2 = allgather_vector(data2, MPI.INT)
             MPI.COMM_WORLD.Barrier()
-            #gl_ess_tdofs.append((name, gl_ess_tdof))
+            # gl_ess_tdofs.append((name, gl_ess_tdof))
             # TO-DO intArray must accept np.int32
             gtdofs1 = [int(x) for x in gl_ess_tdof1]
             gtdofs2 = [int(x) for x in gl_ess_tdof2]
             self.gl_ess_tdofs[name] = (gtdofs1, gtdofs2)
 
     def mkdir(self, path):
         from mpi4py import MPI
```

### Comparing `PetraM_Base-2.1.30/petram/helper/block_matrix.py` & `petram_base-2.1.38/petram/helper/block_matrix.py`

 * *Files 0% similar despite different names*

```diff
@@ -348,14 +348,25 @@
                hypre
         '''
         self.block = [[None] * shape[1] for x in range(shape[0])]
         self.kind = kind
         self.shape = shape
         self.complex = complex
 
+    @property
+    def is_zero(self):
+        '''
+        check if block is completely zero
+        '''
+        for i in range(self.shape[0]):
+            for j in range(self.shape[1]):
+                if self[i, j] is not None:
+                    return False
+        return True
+
     def __getitem__(self, idx):
         try:
             r, c = idx
         except BaseException:
             r = idx
             c = 0
         if isinstance(r, slice):
```

### Comparing `PetraM_Base-2.1.30/petram/helper/boundary_refinement.py` & `petram_base-2.1.38/petram/helper/boundary_refinement.py`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/helper/cdict.py` & `petram_base-2.1.38/petram/helper/cdict.py`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/helper/chypre_to_pymatrix.py` & `petram_base-2.1.38/petram/helper/chypre_to_pymatrix.py`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/helper/convolve.py` & `petram_base-2.1.38/petram/helper/convolve.py`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/helper/direct_wrapper_call.py` & `petram_base-2.1.38/petram/helper/direct_wrapper_call.py`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/helper/dof_map.py` & `petram_base-2.1.38/petram/helper/dof_map.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,28 +8,28 @@
 
      fes1 : source
      fes2 : dest (size of fes2 can be smaller)
 
      For periodic BC, DoF corresponts to y_dest will be eliminated
      from the final linear system.
 
-        Since, mapping is 
+        Since, mapping is
            [1,  0][y_src ]   [y_src]
            [     ][      ] = []
            [M,  0][void  ]   [y_dest]
 
         A linear system below
              [y_src ]   [b1]
            A [      ] = [  ]
              [y_dest]   [b2]
         becomes
            Pt A P [y_src] = [b1 + Mt b2]
 
      For H1, L2 element M^-1 = M^t,
-     For ND, and RT, M^-1 needs inversion. 
+     For ND, and RT, M^-1 needs inversion.
 '''
 
 import numpy as np
 import scipy
 import bisect
 import warnings
 import traceback
@@ -343,25 +343,25 @@
     return pt2all,  pto2all, k2all, sh2all, map_1_2
 
 
 def redistribute_external_entry(external_entry, rstart):
     #  redistribute external entry. first regroup
     #  entries to the destination. then all-to-all
 
+
     rstarts = comm.allgather(rstart)
     dests = [bisect.bisect_right(rstarts, r)for r, c, d in external_entry]
 
     data = [[] for x in range(num_proc)]
     for i, d in zip(dests, external_entry):
         data[i].append(d)
 
     external_entry = sum(comm.alltoall(data), [])
     return np.array(external_entry)
 
-
 def map_dof_scalar(map, fes1, fes2, pt1all, pt2all, pto1all, pto2all,
                    k1all, k2all, sh1all, sh2all, map_1_2,
                    trans1, trans2, tol, tdof, rstart):
 
     dprint1("map_dof_scalar1", debug.format_memory_usage())
 
     pt = []
@@ -457,29 +457,31 @@
 
         if len(external_entry.shape) == 2:
             idx1 = np.in1d(external_entry[:, 0], subvdofs1, invert=True)
             val, idx2 = np.unique(external_entry[idx1, 0], return_index=True)
             external_entry = external_entry[idx1][idx2]
 
             for r, c, d in external_entry:
+                r = int(r)
+                c = int(c)
                 # if not r in subvdofs1:
                 num_entry = num_entry + 1
                 map[r-rstart, c] = d
 
                 #print("adding",myid, r,  c, d )
                 # subvdofs1.append(r)
 
         dprint1("map_dof_scalar3", debug.format_memory_usage())
         '''
-        external_entry =  sum(comm.allgather(external_entry),[])           
+        external_entry =  sum(comm.allgather(external_entry),[])
         for r, c, d in external_entry:
            h = map.shape[0]
            if (r - rstart >= 0 and r - rstart < h and
                not r  in subvdofs1):
-               num_entry = num_entry + 1                                 
+               num_entry = num_entry + 1
                print("adding",myid, r,  c, d )
                map[r-rstart, c] = d
                subvdofs1.append(r)
         '''
         total_entry = sum(allgather(num_entry))
         total_pts = sum(allgather(num_pts))
         if sum(allgather(map.nnz)) != total_entry:
@@ -706,19 +708,19 @@
                 m1 = np.transpose(np.vstack(v1))
                 m2 = np.transpose(np.vstack(v2))
                 m = np.dot(np.linalg.inv(m1), m2)
                 m = np.around(np.linalg.inv(m), decimals = decimals)
                 num2 = make_entry(newk1[dd[0],[1,2]], newk2[d[0],2], m[0,0], num2)
                 num2 = make_entry(newk1[dd[0],[1,2]], newk2[d[1],2], m[1,0], num2)
                 num2 = make_entry(newk1[dd[0],[1,2]], newk2[d[2],2], m[2,0], num2)
-                                  
+
                 num2 = make_entry(newk1[dd[1],[1,2]], newk2[d[0],2], m[0,1], num2)
                 num2 = make_entry(newk1[dd[1],[1,2]], newk2[d[1],2], m[1,1], num2)
                 num2 = make_entry(newk1[dd[1],[1,2]], newk2[d[2],2], m[2,1], num2)
-                                  
+
                 num2 = make_entry(newk1[dd[2],[1,2]], newk2[d[0],2], m[0,2], num2)
                 num2 = make_entry(newk1[dd[2],[1,2]], newk2[d[1],2], m[1,2], num2)
                 num2 = make_entry(newk1[dd[2],[1,2]], newk2[d[2],2], m[2,2], num2)
                 '''
                 if old_mapping:
                     m1 = np.transpose(np.vstack(v1))
                     m2 = np.transpose(np.vstack(v2))
@@ -753,15 +755,15 @@
                 num2 = make_entry(newk1[dd[2], [1, 2]],
                                   newk2[d[2], 2], m[2, 2], num2)
 
             else:
                 print(pt1, pt2)
                 '''
                  newk1 = k1all[k0] #(i local DoF, global DoF)
-                 sh1 = sh1all[k0]           
+                 sh1 = sh1all[k0]
                  pto2 = pto2all[k2]
                  newk2 = k2all[k2]
                  sh2 = sh2all[k2]
                 '''
                 # to do support three vectors
                 raise AssertionError("more than three dofs at same place")
         subvdofs2.extend([s for k, v, s in newk2])
@@ -779,29 +781,30 @@
 
         if len(external_entry.shape) == 2:
             idx1 = np.in1d(external_entry[:, 0], subvdofs1, invert=True)
             val, idx2 = np.unique(external_entry[idx1, 0], return_index=True)
             external_entry = external_entry[idx1][idx2]
 
             for r, c, d in external_entry:
+                r = int(r)
+                c = int(c)
                 # if not r in subvdofs1:
                 num_entry = num_entry + 1
-                #print("adding",myid, r,  c, d )
                 map[r-rstart, c] = d
                 # subvdofs1.append(r)
 
         dprint1("map_dof_vector3", debug.format_memory_usage())
-        '''        
+        '''
         external_entry =  sum(comm.allgather(external_entry),[])
-        #nicePrint(external_entry)        
+        #nicePrint(external_entry)
         for r, c, d in external_entry:
            h = map.shape[0]
            if (r - rstart >= 0 and r - rstart < h and
                not r  in subvdofs1):
-               num_entry = num_entry + 1                                 
+               num_entry = num_entry + 1
                print("adding",myid, r,  c, d )
                map[r-rstart, c] = d
                subvdofs1.append(r)
         '''
         total_entry = sum(allgather(num_entry))
         total_pts = sum(allgather(num_pts))
         if sum(allgather(map.nnz)) != total_entry:
@@ -910,15 +913,15 @@
     data = pt1all, pt2all, pto1all, pto2all, k1all, k2all, sh1all, sh2all,
 
     return data, map_1_2
 
 
 def get_empty_map(fes1, fes2, is_complex=False):
     '''
-    empty matrix (fes1: test, fes2: 
+    empty matrix (fes1: test, fes2:
     '''
     if use_parallel:
         fesize1 = fes1.GetTrueVSize()
         fesize2 = fes2.GlobalTrueVSize()
         rstart = fes1.GetMyTDofOffset()
     else:
         fesize1 = fes1.GetNDofs()
@@ -1012,15 +1015,15 @@
     if R is not None:
         assert False, "Non-conforming mesh not supported"
     '''
     If R is not none. we have to do something like this...
         VDof2TDof = np.zeros(fes.GetNDofs(), dtype=int)
         for i, j in enumerate(R.GetJArray()):
             VDof2TDof[j] = i
-        TDof2Vdof = R.GetJArray().copy()            
+        TDof2Vdof = R.GetJArray().copy()
     '''
     mesh = fes1.GetMesh()
     battrs = {battr: k for k, battr in enumerate(mesh.GetBdrAttributeArray())}
 
     vdofs1 = [fes1.GetBdrElementVDofs(
         battrs[i])[0] if i in battrs else -1 for i in idx1]
     vdofs2 = [fes2.GetBdrElementVDofs(
@@ -1162,15 +1165,15 @@
 
 
 def projection_matrix(idx1,  idx2,  fes, tdof1, fes2=None, tdof2=None,
                       trans1=None, trans2=None, dphase=0.0, weight=None,
                       tol=1e-7, mode='surface', filldiag=True,
                       old_mapping=True):
     '''
-     map: destinatiom mapping 
+     map: destinatiom mapping
      smap: source mapping
 
      old_mapping: True : periodic boundary conditions are implemented this way
                          x = M*y
                   False: projection operator should use this flag.
                          y = M*x
         the difference is only when mapping two/three DoFs sitting at the
```

### Comparing `PetraM_Base-2.1.30/petram/helper/dof_mapping_matrix.py` & `petram_base-2.1.38/petram/helper/dof_mapping_matrix.py`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/helper/dot_dict.py` & `petram_base-2.1.38/petram/helper/dot_dict.py`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/helper/dummy_mpi.py` & `petram_base-2.1.38/petram/helper/dummy_mpi.py`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/helper/element_map.py` & `petram_base-2.1.38/petram/helper/element_map.py`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/helper/eval_deriv.py` & `petram_base-2.1.38/petram/helper/eval_deriv.py`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/helper/eval_shape.py` & `petram_base-2.1.38/petram/helper/eval_shape.py`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/helper/expression.py` & `petram_base-2.1.38/petram/helper/expression.py`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/helper/find_dof_map.py` & `petram_base-2.1.38/petram/helper/find_dof_map.py`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/helper/find_dof_map_h1.py` & `petram_base-2.1.38/petram/helper/find_dof_map_h1.py`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/helper/find_dof_map_nd.py` & `petram_base-2.1.38/petram/helper/find_dof_map_nd.py`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/helper/formholder.py` & `petram_base-2.1.38/petram/helper/formholder.py`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/helper/geom.py` & `petram_base-2.1.38/petram/helper/geom.py`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/helper/global_named_list.py` & `petram_base-2.1.38/petram/helper/global_named_list.py`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/helper/hcurl_normal.py` & `petram_base-2.1.38/petram/helper/hcurl_normal.py`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/helper/hierarchical_finite_element_spaces.py` & `petram_base-2.1.38/petram/helper/hierarchical_finite_element_spaces.py`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/helper/matrix_file.py` & `petram_base-2.1.38/petram/helper/matrix_file.py`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/helper/memory_report.py` & `petram_base-2.1.38/petram/helper/memory_report.py`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/helper/mpi_recipes.py` & `petram_base-2.1.38/petram/helper/mpi_recipes.py`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/helper/numba_interp.py` & `petram_base-2.1.38/petram/helper/numba_interp.py`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/helper/numba_utils.py` & `petram_base-2.1.38/petram/helper/numba_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,15 +40,16 @@
             t1 = '    arrr' + \
                 str(count) + ' = farray(data[' + \
                 str(count) + "], "+str(size) + ", np.float64)"
             t2 = '    arri' + \
                 str(count) + ' = farray(data[' + \
                 str(count+1) + "], "+str(size) + ", np.float64)"
 
-            if len(size) == 1 and size[0] == 1:
+            #if len(size) == 1 and size[0] == 1:
+            if kind == 0:
                 t1 += '[0]'
                 t2 += '[0]'
 
             t3 = '    arr'+str(count) + ' = arrr' + \
                 str(count) + "+1j*arri" + str(count)
 
             text.extend((t1, t2, t3))
@@ -56,15 +57,16 @@
             count = count + 2
 
         else:
             t = '    arr' + \
                 str(count) + ' = farray(data[' + \
                 str(count) + "], "+str(size) + ", np.float64)"
 
-            if len(size) == 1 and size[0] == 1:
+            #if len(size) == 1 and size[0] == 1:
+            if kind == 0:
                 t += '[0]'
 
             text.append(t)
 
             params_line += 'arr'+str(count)+','
             count = count + 1
 
@@ -128,15 +130,16 @@
         if s:
             t1 = '    arrr' + \
                 str(count) + ' = farray(data[' + \
                 str(count) + "], "+str(size) + ", np.float64)"
             t2 = '    arri' + \
                 str(count) + ' = farray(data[' + \
                 str(count+1) + "], "+str(size) + ", np.float64)"
-            if len(size) == 1 and size[0] == 1:
+            #if len(size) == 1 and size[0] == 1:
+            if kind == 0:
                 t1 += '[0]'
                 t2 += '[0]'
 
             t3 = '    arr'+str(count) + ' = arrr' + \
                 str(count) + "+1j*arri" + str(count)
 
             text.extend((t1, t2, t3))
@@ -144,15 +147,16 @@
             count = count + 2
         else:
             if not isinstance(size, tuple):
                 size = (size, )
             t = '    arr' + \
                 str(count) + ' = farray(data[' + \
                 str(count) + "]," + str(size) + ", np.float64)"
-            if len(size) == 1 and size[0] == 1:
+            #if len(size) == 1 and size[0] == 1:
+            if kind == 0:
                 t += '[0]'
 
             text.append(t)
             params_line += 'arr'+str(count)+','
             count = count + 1
 
     outsize = setting["outsize"]
```

### Comparing `PetraM_Base-2.1.30/petram/helper/operators.py` & `petram_base-2.1.38/petram/helper/operators.py`

 * *Files 2% similar despite different names*

```diff
@@ -301,21 +301,22 @@
         fes1 = self._fes1()
         fes2 = fes1 if self._fes2 is None else self._fes2()
 
         c_coeff = self._c_coeff
 
         from petram.phys.phys_model import PhysConstant
         coeff = 0.
+
         if c_coeff[0] is not None:
             assert isinstance(
-                c_coeff[0], PhysConstant), "projection supports only constant scalr coefficient"
+                c_coeff[0], PhysConstant), "Identity supports only constant scalar coefficient. (Got "+str(type(c_coeff[0])) + ")"
             coeff += c_coeff[0].value
         if c_coeff[1] is not None:
             assert isinstance(
-                c_coeff[1], PhysConstant), "projection supports only constant scalr coefficient"
+                c_coeff[1], PhysConstant), "Identity supports only constant scalar coefficient. (Got "+str(type(c_coeff[1])) + ")"
             coeff += 1j*c_coeff[1].value
 
         mat = make_diagonal_mat(engine, fes1, fes2, 1.0)
 
         return mat*coeff
 
 class Zero(Operator):
@@ -527,19 +528,19 @@
 
         c_coeff = self._c_coeff
 
         from petram.phys.phys_model import PhysConstant
         coeff = 0.
         if c_coeff[0] is not None:
             assert isinstance(
-                c_coeff[0], PhysConstant), "projection supports only constant scalr coefficient"
+                c_coeff[0], PhysConstant), "projection supports only constant scalar coefficient + (Got "+str(type(c_coeff[0])) + ")"
             coeff += c_coeff[0].value
         if c_coeff[1] is not None:
             assert isinstance(
-                c_coeff[1], PhysConstant), "projection supports only constant scalr coefficient"
+                c_coeff[1], PhysConstant), "projection supports only constant scalar coefficient + (Got "+str(type(c_coeff[1])) + ")"
             coeff += 1j*c_coeff[1].value
 
         dim1 = self.fes1.GetMesh().Dimension()
         dim2 = self.fes2.GetMesh().Dimension()
 
         projmode = ""
         if dim2 == 3:
```

### Comparing `PetraM_Base-2.1.30/petram/helper/phys_module_util.py` & `petram_base-2.1.38/petram/helper/phys_module_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,15 +80,17 @@
         warnings.warn('Can not find path for :' + mname)
         raise
 
     constraints = {'domain': [], 'bdry': [],
                    'edge': [], 'pointt': [], 'pair': []}
 
     for p in paths:
-        for f in listdir(p):
+        tmp = [(basename(x), x) for x in listdir(p)]
+        dirlist = [x[1] for x in sorted(tmp)]
+        for f in dirlist:
             name = basename(f)
             if not name.endswith('py'):
                 continue
             if name.startswith('_'):
                 continue
             name = name[:-3]
             mname2 = mname + '.' + name
```

### Comparing `PetraM_Base-2.1.30/petram/helper/pickle_wrapper.py` & `petram_base-2.1.38/petram/helper/pickle_wrapper.py`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/helper/preconditioners.py` & `petram_base-2.1.38/petram/helper/preconditioners.py`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/helper/projection.py` & `petram_base-2.1.38/petram/helper/projection.py`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/helper/right_broadcast.py` & `petram_base-2.1.38/petram/helper/right_broadcast.py`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/helper/test.py` & `petram_base-2.1.38/petram/helper/test.py`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/helper/validator_input.py` & `petram_base-2.1.38/petram/helper/validator_input.py`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/helper/variables.py` & `petram_base-2.1.38/petram/helper/variables.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,14 +40,15 @@
        return 1-0.1j
 
     @variable.array(complex=True,shape=(2,))
     def atest(x, y, z):
        return np.array([1-0.1j,1-0.1j])
 
 '''
+from petram.solver.parametric_scanner import Scan
 import numpy as np
 import weakref
 import types
 import traceback
 from weakref import WeakKeyDictionary as WKD
 from weakref import WeakValueDictionary as WVD
 
@@ -59,69 +60,73 @@
 
 import petram.debug
 dprint1, dprint2, dprint3 = petram.debug.init_dprints('Variables')
 
 
 class _decorator(object):
     @staticmethod
-    def float(func=None, *, dependency=None, grad=None, curl=None, div=None, td=False):
+    def float(func=None, *, dependency=None, grad=None, curl=None, div=None, td=False,
+              params=None):
         '''
         this form allows for using both
         @float
         @float()
         '''
         def wrapper(func):
             def dec(*args, **kwargs):
                 obj = PyFunctionVariable(func,
                                          complex=False,
                                          dependency=dependency,
                                          grad=grad,
                                          curl=curl,
-                                         div=div)
+                                         div=div,
+                                         params=params)
                 return obj
             return dec(func)
         if func:
             return wrapper(func)
         else:
             return wrapper
 
     @staticmethod
-    def complex(func=None, *, dependency=None, grad=None, curl=None, div=None, td=False):
+    def complex(func=None, *, dependency=None, grad=None, curl=None, div=None, td=False,
+                params=None):
         '''
         this form allows for using both
         @complex
         @complex()
         '''
         def wrapper(func):
             def dec(*args, **kwargs):
                 obj = PyFunctionVariable(func,
                                          complex=True,
                                          dependency=dependency,
                                          grad=grad,
                                          curl=curl,
-                                         div=div)
-
+                                         div=div,
+                                         params=params)
                 return obj
             return dec(func)
         if func:
             return wrapper(func)
         else:
             return wrapper
 
     @staticmethod
     def array(complex=False, shape=(1,), dependency=None, grad=None,
-              curl=None, div=None, td=False):
+              curl=None, div=None, td=False, params=None):
         def dec(func):
             obj = PyFunctionVariable(func,
                                      complex=complex,
                                      shape=shape,
                                      dependency=dependency,
                                      grad=grad,
                                      curl=curl,
-                                     div=div,)
+                                     div=div,
+                                     params=params)
             return obj
         return dec
 
 
 class _decorator_jit(object):
 
     @staticmethod
@@ -213,15 +218,15 @@
     return a
 
 
 def cosd(x): return np.cos(x * np.pi / 180.)
 def sind(x): return np.sin(x * np.pi / 180.)
 def tand(x): return np.tan(x * np.pi / 180.)
 
-
+from petram.solver.parametric_scanner import Scan
 var_g = {'sin': np.sin,
          'cos': np.cos,
          'tan': np.tan,
          'cosd': cosd,
          'sind': sind,
          'tand': tand,
          'arctan': np.arctan,
@@ -241,21 +246,23 @@
          'array': np.array,
          'cross': np.cross,
          'pi': np.pi,
          'min': np.max,
          'min': np.min,
          'sign': np.sign,
          'ones': np.ones,
+         'eye':np.eye,
          'diag': np.diag,
          'zeros': np.zeros,
          'nan': np.nan,
          'inf': np.inf,
          'inv': np.linalg.inv,
          'linspace': np.linspace,
-         'logspace': np.logspace}
+         'logspace': np.logspace,
+         'Scan': Scan}
 
 
 def check_vectorfe_in_lowdim(gf):
     # check if this is VectorFE in lower dimensionality
 
     fes = gf.FESpace()
     sdim = fes.GetMesh().SpaceDimension()
@@ -384,15 +391,16 @@
     def __abs__(self):
         return self().__abs__()
 
     def __getitem__(self, idx):
         return self()[idx]
 
     def get_names(self):
-        return []
+        return list(set(list(self.dependency) + list(self.div) +
+                        list(self.curl) + list(self.grad)))
 
     def get_emesh_idx(self, idx=None, g=None):
         if idx is None:
             idx = []
         return idx
 
     def ncface_values(self, ifaces=None, irs=None,
@@ -677,15 +685,15 @@
         if len(ll_name) > 0:
             value = np.array([eval(self.co, var_g2, dict(zip(ll_name, v)))
                               for v in zip(*ll_value)])
         else:
             for k, name in enumerate(self.ind_vars):
                 l[name] = locs[..., k]
             value = np.array(eval_code(self.co, var_g2, l), copy=False)
-            if value.ndim > 1:
+            if value.ndim > 0:
                 value = np.stack([value] * size)
         #value = np.array(eval_code(self.co, var_g, l), copy=False)
         from petram.helper.right_broadcast import multi
 
         ret = multi(ret, value)
         #print("return (expr)", ret.shape)
 
@@ -719,17 +727,16 @@
         if len(ll_name) > 0:
             value = np.array([eval(self.co, var_g2, dict(zip(ll_name, v)))
                               for v in zip(*ll_value)])
         else:
             for k, name in enumerate(self.ind_vars):
                 l[name] = locs[..., k]
             value = np.array(eval_code(self.co, var_g2, l), copy=False)
-            if value.ndim > 1:
+            if value.ndim > 0:
                 value = np.stack([value] * size)
-
         return value
 
     def ncface_values(self, *args, **kwargs):
         return self._ncx_values('ncface_values', *args, **kwargs)
 
     def ncedge_values(self, *args, **kwargs):
         return self._ncx_values('ncedge_values', *args, **kwargs)
@@ -756,15 +763,16 @@
         if len(ll_name) > 0:
             value = np.array([eval(self.co, var_g2, dict(zip(ll_name, v)))
                               for v in zip(*ll_value)])
         else:
             for k, name in enumerate(self.ind_vars):
                 l[name] = locs[..., k]
             value = np.array(eval_code(self.co, var_g2, l), copy=False)
-            if value.ndim > 1:
+            if value.ndim > 0:
+                size = counts
                 value = np.stack([value] * size)
 
         return value
 
 
 class DomainVariable(Variable):
     def __init__(self, expr='', ind_vars=None, domains=None,
@@ -1022,33 +1030,66 @@
             else:
                 idx = np.in1d(valid_attrs, domains)
                 ret[idx] = v[idx]
 
         return ret
 
 
+def _copy_func_and_apply_params(f, params):
+    import copy
+    import types
+    import functools
+
+    """Based on https://stackoverflow.com/a/13503277/2988730 (@unutbu)"""
+    globals = f.__globals__.copy()
+    for k in params:
+        globals[k] = params[k]
+    g = types.FunctionType(f.__code__, globals, name=f.__name__,
+                           argdefs=f.__defaults__, closure=f.__closure__)
+    g = functools.update_wrapper(g, f)
+    g.__module__ = f.__module__
+    g.__kwdefaults__ = copy.copy(f.__kwdefaults__)
+    return g
+
+
+def _get_kwargs(func):
+    from inspect import signature
+    sig = signature(func)
+
+    kwnames = [x for x in sig.parameters
+               if sig.parameters[x].default != sig.parameters[x].empty]
+    return kwnames
+    dep2kw = dict(zip(self.dependency, kwnames))
+
+
 class PyFunctionVariable(Variable):
     def __init__(self, func, complex=False, shape=tuple(), dependency=None,
-                 grad=None, curl=None, div=None):
+                 grad=None, curl=None, div=None, params=None):
         super(
             PyFunctionVariable,
             self).__init__(complex=complex,
                            dependency=dependency,
                            grad=grad,
                            curl=curl,
                            div=div)
-
+        if params is not None:
+            func = _copy_func_and_apply_params(func, params)
         self.func = func
         self.t = None
         self.x = (0, 0, 0)
         self.shape = shape
 
     def __repr__(self):
         return "PyFunction"
 
+    def _get_dep2kw(self):
+        kwnames = _get_kwargs(self.func)
+        dep2kw = dict(zip(self.dependency, kwnames))
+        return dep2kw
+
     def set_point(self, T, ip, g, l, t=None):
         self.x = T.Transform(ip)
         self.t = t
 
     def __call__(self, **kwargs):
         if self.t is not None:
             args = tuple(np.hstack((self.x, t)))
@@ -1060,41 +1101,53 @@
         return np.array(self.func(*args, **kwargs), copy=False)
 
     def nodal_values(self, iele=None, el2v=None, locs=None,
                      wverts=None, elvertloc=None, g=None, knowns=None,
                      **kwargs):
         # elattr = None, el2v = None,
         # wverts = None, locs = None, g = None
+
         if locs is None:
             return
         if g is None:
             g = {}
         if knowns is None:
             knowns = WKD()
 
         size = len(wverts)
         shape = [size] + list(self.shape)
 
         dtype = np.complex128 if self.complex else np.float64
         ret = np.zeros(shape, dtype=dtype)
         wverts = np.zeros(size)
 
+        dep2kw = self._get_dep2kw()
+
         for kk, m, loc in zip(iele, el2v, elvertloc):
             if kk < 0:
                 continue
             for pair, xyz in zip(m, loc):
                 idx = pair[1]
                 for n in self.dependency:
                     if not g[n] in knowns:
                         knowns[g[n]] = g[n].nodal_values(iele=iele, el2v=el2v,
                                                          locs=locs, wverts=wverts,
                                                          elvertloc=elvertloc,
                                                          g=g, knows=knowns,
                                                          **kwargs)
-                kwargs = {n: knowns[g[n]][idx] for n in self.dependency}
+
+                kwargs = {dep2kw[n]: knowns[g[n]][idx]
+                          for n in self.dependency}
+                for n in self.grad:
+                    kwargs['grad'+n] = knowns[g['grad'+n]][idx]
+                for n in self.curl:
+                    kwargs['curl'+n] = knowns[g['curl'+n]][idx]
+                for n in self.div:
+                    kwargs['div'+n] = knowns[g['div'+n]][idx]
+
                 ret[idx] = ret[idx] + self.func(*xyz, **kwargs)
                 wverts[idx] = wverts[idx] + 1
         ret = np.stack([x for x in ret if x is not None])
 
         idx = np.where(wverts == 0)[0]
         wverts[idx] = 1.0
 
@@ -1112,14 +1165,17 @@
             g = {}
         if knowns is None:
             knowns = WKD()
 
         dtype = np.complex128 if self.complex else np.float64
 
         ret = [None] * len(locs)
+
+        dep2kw = self._get_dep2kw()
+
         for idx, xyz in enumerate(locs):
             '''
             for n in self.dependency:
                 g[n].local_value = knowns[g[n]][idx]
                 # putting the dependency variable to functions global.
                 # this may not ideal, since there is potential danger
                 # of name conflict?
@@ -1130,15 +1186,22 @@
                     m = getattr(g[n], method)
                     knowns[g[n]] = m(ifaces=ifaces, irs=irs,
                                      gtypes=gtypes, g=g,
                                      attr1=attr1, attr2=attr2,
                                      locs=locs, knows=knowns,
                                      **kwargs)
 
-            kwargs = {n: knowns[g[n]][idx] for n in self.dependency}
+            kwargs = {dep2kw[n]: knowns[g[n]][idx] for n in self.dependency}
+            for n in self.grad:
+                kwargs['grad'+n] = knowns[g['grad'+n]][idx]
+            for n in self.curl:
+                kwargs['curl'+n] = knowns[g['curl'+n]][idx]
+            for n in self.div:
+                kwargs['div'+n] = knowns[g['div'+n]][idx]
+
             ret[idx] = self.func(*xyz, **kwargs)
 
         ret = np.stack(ret).astype(dtype, copy=False)
 
         return ret
 
     def ncface_values(self, *args, **kwargs):
@@ -1161,14 +1224,16 @@
 
         shape = [counts] + list(self.shape)
         dtype = np.complex128 if self.complex else np.float64
         ret = np.zeros(shape, dtype=dtype)
 
         valid_attrs = attrs[attrs != -1]
 
+        dep2kw = self._get_dep2kw()
+
         jj = 0
         for i in range(counts):
             if valid_attrs[i] == -1:
                 continue
             if (current_domains is not None and
                     not valid_attrs[i] in current_domains):
                 continue
@@ -1177,15 +1242,22 @@
                 if not g[n] in knowns:
                     knowns[g[n]] = g[n].point_values(counts=counts, locs=locs, points=points,
                                                      attrs=attrs, elem_ids=elem_ids,
                                                      mesh=mesh, int_points=int_points, g=g,
                                                      knowns=knowns, current_domains=current_domains)
 
             xyz = tuple(locs[i])
-            kwargs = {n: knowns[g[n]][i] for n in self.dependency}
+            kwargs = {dep2kw[n]: knowns[g[n]][i] for n in self.dependency}
+            for n in self.grad:
+                kwargs['grad'+n] = knowns[g['grad'+n]][i]
+            for n in self.curl:
+                kwargs['curl'+n] = knowns[g['curl'+n]][i]
+            for n in self.div:
+                kwargs['div'+n] = knowns[g['div'+n]][i]
+
             value = self.func(*xyz, **kwargs)
 
             ret[i, ...] = value
 
         return ret
 
 
@@ -1317,14 +1389,15 @@
         for i, gtype, in zip(ifaces, gtypes):
             T = m(i)
             ir = irs[gtype]
             nv = ir.GetNPoints()
 
             for j in range(nv):
                 ip = ir.IntPoint(j)
+                T.SetIntPoint(ip)
 
                 if (self.coeff[0] is not None and
                         self.coeff[1] is not None):
                     value = (np.array(call_eval(self.coeff[0], T, ip)) +
                              1j * np.array(call_eval(self.coeff[1], T, ip)))
                 elif self.coeff[0] is not None:
                     value = np.array(call_eval(self.coeff[0], T, ip))
@@ -1356,14 +1429,15 @@
         for i, gtype, in zip(ifaces, gtypes):
             T = m(i)
             ir = irs[gtype]
             nv = ir.GetNPoints()
 
             for j in range(nv):
                 ip = ir.IntPoint(j)
+                T.SetIntPoint(ip)
 
                 if (self.coeff[0] is not None and
                         self.coeff[1] is not None):
                     value = (np.array(call_eval(self.coeff[0], T, ip)) +
                              1j * np.array(call_eval(self.coeff[1], T, ip)))
                 elif self.coeff[0] is not None:
                     value = np.array(call_eval(self.coeff[0], T, ip))
@@ -1390,14 +1464,15 @@
         for i in range(len(attrs)):
             if attrs[i] == -1:
                 continue
 
             iele = elem_ids[i]
             T = mesh.GetElementTransformation(iele)
             ip = int_points[i]
+            T.SetIntPoint(ip)
 
             if (self.coeff[0] is not None and
                     self.coeff[1] is not None):
                 value = (np.array(call_eval(self.coeff[0], T, ip)) +
                          1j * np.array(call_eval(self.coeff[1], T, ip)))
             elif self.coeff[0] is not None:
                 value = np.array(call_eval(self.coeff[0], T, ip))
@@ -1429,14 +1504,15 @@
             assert False, "unknown kind of Coefficient. Must be scalar/vector/matrix"
         return call_eval
 
 
 class NumbaCoefficientVariable(CoefficientVariable):
     def __init__(self, func, complex=False, shape=tuple(), dependency=None,
                  grad=None, curl=None, div=None, td=False, params=None):
+
         super(
             CoefficientVariable,
             self).__init__(complex=complex,
                            dependency=dependency,
                            grad=grad,
                            curl=curl,
                            div=div)
@@ -1454,14 +1530,21 @@
         elif len(self.shape) == 2:
             self.kind = 'matrix'
         else:
             assert False, "unsupported shape"
 
         self._jitted = None
 
+    def has_dependency(self):
+        return ((len(self.dependency) + len(self.grad) +
+                 len(self.div) + len(self.curl)) > 0)
+
+    def forget_jitted_coefficient(self):
+        self._jitted = None
+
     def get_jitted_coefficient(self, ind_vars, locals):
 
         if self._jitted is not None:
             dprint1("(Note) this numba coefficient is already compiled", self.func)
             return self._jitted
 
         from petram.phys.numba_coefficient import NumbaCoefficient
@@ -1513,14 +1596,29 @@
         dep = []
 
         for d in self.dependency:
             dd = locals[d].get_jitted_coefficient(ind_vars, locals)
             if dd is None:
                 return
             dep.append(dd)
+        for d in self.grad:
+            dd = locals[d].get_jitted_grad_coefficient(ind_vars, locals)
+            if dd is None:
+                return
+            dep.append(dd)
+        for d in self.curl:
+            dd = locals[d].get_jitted_curl_coefficient(ind_vars, locals)
+            if dd is None:
+                return
+            dep.append(dd)
+        for d in self.div:
+            dd = locals[d].get_jitted_div_coefficient(ind_vars, locals)
+            if dd is None:
+                return
+            dep.append(dd)
 
         from petram.mfem_config import numba_debug, use_parallel
         if use_parallel:
             from mpi4py import MPI
             myid = MPI.COMM_WORLD.rank
         else:
             myid = 0
@@ -1535,14 +1633,16 @@
                          debug=numba_debug,
                          **kwargs)
         self._jitted = wrapper(self.func)
         return self._jitted
 
     def set_coeff(self, ind_vars, locals):
         coeff = self.get_jitted_coefficient(ind_vars, locals)
+        if coeff is None:
+            assert False, "Failed to generate JITed coefficient"
         if self.complex:
             self.coeff = (coeff.real, coeff.imag)
         else:
             self.coeff = (coeff, None)
 
 
 class GridFunctionVariable(Variable):
@@ -1554,61 +1654,121 @@
         self.dim = gf_real.VectorDim()
         self.comp = comp
         self.isGFSet = False
         self.isDerived = False
         self.deriv = deriv if deriv is not None else self._def_deriv
         self.deriv_args = (gf_real, gf_imag)
 
-        self._curl = None
-        self._div = None
-        self._grad = None
+        self._grad_gf = None
+        self._curl_gf = None
+        self._div_gf = None
 
     def _def_deriv(self, *args):
         return args[0], args[1], None
 
-    def eval_grad(self):
-        if self._grad is None:
+    def _set_grad_gf(self):
+        self.set_gfr_gfi()
+        if self._grad_gf is None:
             grad_r = mfem.GradientGridFunctionCoefficient(self.gfr)
             if self.gfi is not None:
-                grad_i = mfem.GradientVectorGridFunctionCoefficient(self.gfi)
+                grad_i = mfem.GradientGridFunctionCoefficient(self.gfi)
             else:
                 grad_i = None
             self._grad_gf = (grad_r, grad_i)
+
+    def _set_div_gf(self):
+        self.set_gfr_gfi()
+        if self._div_gf is None:
+            div_r = mfem.DivergenceGridFunctionCoefficient(self.gfr)
+            if self.gfi is not None:
+                div_i = mfem.DivergenceGridFunctionCoefficient(self.gfi)
+            else:
+                div_i = None
+            self._div_gf = (div_r, div_i)
+
+    def _set_curl_gf(self):
+        self.set_gfr_gfi()
+        if self._curl_gf is None:
+            curl_r = mfem.CurlGridFunctionCoefficient(self.gfr)
+            if self.gfi is not None:
+                curl_i = mfem.CurlGridFunctionCoefficient(self.gfi)
+            else:
+                curl_i = None
+            self._curl_gf = (curl_r, curl_i)
+
+    def generate_grad_variable(self):
+        self._set_grad_gf()
+
+        def func(*args, **kargs):
+            return self._grad_gf
+        func.kind = 'vector'
+        l = {}
+        return CoefficientVariable(func, l)
+
+    def generate_curl_variable(self):
+        self._set_curl_gf()
+
+        def func(*args, **kargs):
+            return self._curl_gf
+        func.kind = 'vector'
+        l = {}
+        return CoefficientVariable(func, l)
+
+    def generate_div_variable(self):
+        self._set_div_gf()
+
+        def func(*args, **kargs):
+            return self._div_gf
+        func.kind = 'scalar'
+        l = {}
+        return CoefficientVariable(func, l)
+
+    def get_jitted_grad_coefficient(self, ind_vars, locals):
+        self._set_grad_gf()
+        if self._grad_gf[1] is None:
+            return self._grad_gf[0]
+        else:
+            return (self._grad_gf[0], self._grad_gf[1])
+
+    def get_jitted_curl_coefficient(self, ind_vars, locals):
+        self._set_curl_gf()
+        if self._curl_gf[1] is None:
+            return self._curl_gf[0]
+        else:
+            return (self._curl_gf[0], self._curl_gf[1])
+
+    def get_jitted_div_coefficient(self, ind_vars, locals):
+        self._set_div_gf()
+        if self._div_gf[1] is None:
+            return self._div_gf[0]
+        else:
+            return (self._div_gf[0], self._div_gf[1])
+
+    def eval_grad(self):
+        self._set_grad_gf()
         v = mfem.Vector()
         self._grad_gf[0].Eval(v, self.T, self.ip)
         ret = v.GetDataArray().copy()
         if self._grad_gf[1] is not None:
             self._grad_gf[1].Eval(v, self.T, self.ip)
             ret = ret + 1j*v.GetDataArray()
         return ret
 
     def eval_curl(self):
-        if self._curl is None:
-            curl_r = mfem.CurlGridFunctionCoefficient(self.gfr)
-            if self.gfi is not None:
-                curl_i = mfem.CurlVectorGridFunctionCoefficient(self.gfi)
-            else:
-                curl_i = None
-            self._curl_gf = (curl_r, curl_i)
+        self._set_curl_gf()
         v = mfem.Vector()
         self._curl_gf[0].Eval(v, self.T, self.ip)
         ret = v.GetDataArray().copy()
         if self._curl_gf[1] is not None:
             self._curl_gf[1].Eval(v, self.T, self.ip)
             ret = ret + 1j*v.GetDataArray()
         return ret
 
     def eval_div(self):
-        if self._div is None:
-            div_r = mfem.DivergenceGridFunctionCoefficient(self.gfr)
-            if self.gfi is not None:
-                div_i = mfem.DivergenceVectorGridFunctionCoefficient(self.gfi)
-            else:
-                div_i = None
-            self._div_gf = (div_r, div_i)
+        self._set_div_gf()
         v = mfem.Vector()
         self._div_gf[0].Eval(v, self.T, self.ip)
         ret = v.GetDataArray().copy()
         if self._div_gf[1] is not None:
             self._div_gf[1].Eval(v, self.T, self.ip)
             ret = ret + 1j*v.GetDataArray()
         return ret
@@ -1841,14 +2001,15 @@
             data.append(v)
         data = np.hstack(data)
 
         return data
 
     def ncedge_values(self, ifaces=None, irs=None,
                       gtypes=None, **kwargs):
+
         if not self.isDerived:
             self.set_funcs()
 
         name = self.gfr.FESpace().FEColl().Name()
         ndim = self.gfr.FESpace().GetMesh().Dimension()
 
         isVector = False
@@ -2058,15 +2219,15 @@
                                  for func_r, func_i
                                  in zip(self.func_r, self.func_i)])
 
     def nodal_values(self, iele=None, el2v=None, wverts=None,
                      **kwargs):
         # iele = None, elattr = None, el2v = None,
         # wverts = None, locs = None, g = None
-        #print("grid vector nodal")
+
         if iele is None:
             return
         if not self.isDerived:
             self.set_funcs()
 
         size = len(wverts)
 
@@ -2187,14 +2348,26 @@
                 val = val + dd
 
             data[jj, :] = val
             jj = jj + 1
 
         return data
 
+    def get_jitted_coefficient(self, ind_vars, locals):
+        if not self.isDerived:
+            self.set_funcs()
+
+        if isinstance(self.func_r, mfem.VectorCoefficient):
+            if self.func_i is None:
+                return self.func_r
+            else:
+                return (self.func_r, self.func_i)
+        else:
+            assert False, "Not Implemented (should return VectorCoefficient?)"
+
 
 '''
 
 Surf Variable:
  Regular Variable + Surface Geometry (n, nx, ny, nz)
 
 '''
@@ -2489,25 +2662,38 @@
     fec = fes.FEColl().Name()
 
     if (fec.startswith('ND') or fec.startswith('RT')):
         coeff_dim = sdim
     else:
         coeff_dim = vdim
 
+    return_complex = bool(gfi is not None)
+
     def project_coeff(gf, coeff_dim, c, ind_vars, real):
         if coeff_dim > 1:
             #print("vector coeff", c)
             coeff = VCoeff(coeff_dim, c, ind_vars,
-                           local_ns, global_ns, real=real)
+                           local_ns, global_ns,
+                           return_complex=return_complex,
+                           real=real)
         else:
             #print("coeff", c)
             coeff = SCoeff(c, ind_vars,
-                           local_ns, global_ns, real=real)
-
-        gf.ProjectCoefficient(coeff)
+                           local_ns, global_ns,
+                           return_complex=return_complex,
+                           real=real)
+
+        if hasattr(coeff, 'get_real_coefficient'):
+            if real:
+                cc = coeff.get_real_coefficient()
+            else:
+                cc = coeff.get_imag_coefficient()
+        else:
+            cc = coeff
+        gf.ProjectCoefficient(cc)
 
     project_coeff(gfr, coeff_dim, c, ind_vars, True)
     if gfi is not None:
         project_coeff(gfi, coeff_dim, c, ind_vars, False)
 
 
 '''
```

### Comparing `PetraM_Base-2.1.30/petram/init_model.py` & `petram_base-2.1.38/petram/init_model.py`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/mesh/composite.py` & `petram_base-2.1.38/petram/mesh/composite.py`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/mesh/find_edges.py` & `petram_base-2.1.38/petram/mesh/find_edges.py`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/mesh/find_loop.py` & `petram_base-2.1.38/petram/mesh/find_loop.py`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/mesh/find_vertex.py` & `petram_base-2.1.38/petram/mesh/find_vertex.py`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/mesh/geo_plot.py` & `petram_base-2.1.38/petram/mesh/geo_plot.py`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/mesh/make_simplemesh.py` & `petram_base-2.1.38/petram/mesh/make_simplemesh.py`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/mesh/mesh_extension.py` & `petram_base-2.1.38/petram/mesh/mesh_extension.py`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/mesh/mesh_inspect.py` & `petram_base-2.1.38/petram/mesh/mesh_inspect.py`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/mesh/mesh_model.py` & `petram_base-2.1.38/petram/mesh/mesh_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -424,14 +424,15 @@
 
     def attribute_set(self, v):
         v = super(MeshFile, self).attribute_set(v)
         v['path'] = ''
         v['generate_edges'] = 1
         v['refine'] = True
         v['fix_orientation'] = True
+        v['fix_numbering'] = False
 
         return v
 
     def panel1_param(self):
         if not hasattr(self, "_mesh_char"):
             self._mesh_char = ''
         wc = "ANY|*|MFEM|*.mesh|GMSH|*.gmsh"
@@ -440,34 +441,38 @@
                "note: ~ and environmental variables are expanded. \n    In addition, {petram}=$PetraM, {mfem}=PyMFEM, \n     {home}=~ ,{model}=project file dir.",
                2,
                None],
               [None, self.generate_edges == 1,
                3, {"text": "Generate edges"}],
               [None, self.refine == 1, 3, {"text": "Refine"}],
               [None, self.fix_orientation, 3, {"text": "FixOrientation"}],
+              [None, self.fix_numbering, 3, {
+                  "text": "Fix Attr/BdrAttr Numbering"}],
               [None, self._mesh_char, 2, None], ]
 
         p2 = MeshGenerator.panel1_param(self)
         return p1[:-1] + p2 + p1[-1:]
 
     def get_panel1_value(self):
         v1 = [self.path, None, self.generate_edges,
-              self.refine, self.fix_orientation, None]
+              self.refine, self.fix_orientation,
+              self.fix_numbering, None]
 
         v2 = MeshGenerator.get_panel1_value(self)
 
         return v1[:-1] + v2 + v1[-1:]
 
     def import_panel1_value(self, v):
         self.path = str(v[0])
         self.generate_edges = 1 if v[2] else 0
         self.refine = 1 if v[3] else 0
         self.fix_orientation = v[4]
+        self.fix_numbering = v[5]
 
-        MeshGenerator.import_panel1_value(self, v[4:-1])
+        MeshGenerator.import_panel1_value(self, v[5:-1])
 
     def use_relative_path(self):
         self._path_bk = self.path
 
         try:
             self.path = os.path.basename(self.get_real_path())
         except AssertionError as error:
@@ -532,14 +537,24 @@
         if not os.path.exists(path):
             print("mesh file does not exists : " + path + " in " + os.getcwd())
             return None
         args = (path, self.generate_edges, self.refine, self.fix_orientation)
 
         mesh = mfem.Mesh(*args)
 
+        if self.fix_numbering:
+            attr = mesh.GetAttributeArray()
+            _c, attr = np.unique(attr, return_inverse=True)
+            for i, k in enumerate(attr):
+                mesh.SetAttribute(i, k+1)
+            attr = mesh.GetBdrAttributeArray()
+            _c, attr = np.unique(attr, return_inverse=True)
+            for i, k in enumerate(attr):
+                mesh.SetBdrAttribute(i, k+1)
+
         if self.enforce_ncmesh:
             mesh.EnsureNCMesh()
 
         self.parent.sdim = mesh.SpaceDimension()
         self._mesh_char = format_mesh_characteristic(mesh)
         try:
             mesh.GetNBE()
```

### Comparing `PetraM_Base-2.1.30/petram/mesh/mesh_sel_buttons.py` & `petram_base-2.1.38/petram/mesh/mesh_sel_buttons.py`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/mesh/mesh_utils.py` & `petram_base-2.1.38/petram/mesh/mesh_utils.py`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/mesh/nastran2mfem.py` & `petram_base-2.1.38/petram/mesh/nastran2mfem.py`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/mesh/partial_mesh.py` & `petram_base-2.1.38/petram/mesh/partial_mesh.py`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/mesh/plot_mesh.py` & `petram_base-2.1.38/petram/mesh/plot_mesh.py`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/mesh/pumimesh_model.py` & `petram_base-2.1.38/petram/mesh/pumimesh_model.py`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/mesh/read_mfemmesh.py` & `petram_base-2.1.38/petram/mesh/read_mfemmesh.py`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/mesh/read_mfemmesh1.py` & `petram_base-2.1.38/petram/mesh/read_mfemmesh1.py`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/mesh/read_mfemmesh2.py` & `petram_base-2.1.38/petram/mesh/read_mfemmesh2.py`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/mesh/read_mfemmesh2_old.py` & `petram_base-2.1.38/petram/mesh/read_mfemmesh2_old.py`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/mesh/read_mfemmesh3.py` & `petram_base-2.1.38/petram/mesh/read_mfemmesh3.py`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/mesh/refined_mfem_geom.py` & `petram_base-2.1.38/petram/mesh/refined_mfem_geom.py`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/mfem_model.py` & `petram_base-2.1.38/petram/mfem_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -197,18 +197,14 @@
 
     def make_solvars(self, solsets, g=None):
         from petram.mesh.mesh_utils import (get_extended_connectivity,
                                             get_reverse_connectivity)
         from petram.helper.variables import Variable
         from petram.helper.variables import add_scalar
 
-        for phys in self.iter_enabled():
-            for mm in phys.walk_enabled():
-                mm.compile_coeffs()
-
         solvars = [None] * len(solsets)
         if g is None:
             g = {}
         for k, v in enumerate(solsets):
             mesh, soldict = v
 
             get_extended_connectivity(mesh[0])
```

### Comparing `PetraM_Base-2.1.30/petram/mfem_viewer.py` & `petram_base-2.1.38/petram/mfem_viewer.py`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/model.py` & `petram_base-2.1.38/petram/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -492,15 +492,15 @@
     def panel2_tabname(self):
         return "Selection"
 
     def panel3_tabname(self):
         return "Init."
 
     def panel4_tabname(self):
-        return "Time Dep./NL."
+        return "Contrib."
 
     def panel1_param(self):
         return []
 
     def panel2_param(self):
         return []
```

### Comparing `PetraM_Base-2.1.30/petram/namespace_mixin.py` & `petram_base-2.1.38/petram/namespace_mixin.py`

 * *Files 4% similar despite different names*

```diff
@@ -175,15 +175,18 @@
 
     def preprocess_ns(self, ns_folder, data_folder):
         if self.get_ns_name() is None:
             return
 
         ns_script = ns_folder.get_child(name=self.ns_name+'_ns')
         if ns_script is None:
-            raise ValueError("namespace script is not found")
+            self.ns_string = None
+            self.dataset = None
+            return
+            #raise ValueError("namespace script is not found")
         err_string = ns_script.reload_script()
         if err_string != '' and err_string is not None:
             assert False, err_string
 
         self.ns_string = ns_script._script._script
 
         data = data_folder.get_child(name=self.ns_name+'_data')
@@ -210,25 +213,31 @@
         for name, tname,  validator in exprs:
             if targets is not None and not tname in targets:
                 continue
             try:
                 void = {}
                 x = eval(str(getattr(self, tname)), self._global_ns, void)
             except:
-                import traceback
-                traceback.print_exc()
+                if targets is not None:
+                    # print error if it fails in the second run
+                    import traceback
+                    traceback.print_exc()
                 invalid_expr.append(tname)
+                invalid_expr.append(name)
                 continue
             try:
                 if validator is not None:
                     x = validator(x)
             except:
-                import traceback
-                traceback.print_exc()
+                if targets is not None:
+                    # print error if it fails in the second run
+                    import traceback
+                    traceback.print_exc()
                 invalid_expr.append(tname)
+                invalid_expr.append(name)
                 continue
             result[name] = x
 
         return result, invalid_expr
 
     def eval_ns(self):
         chain = self.get_ns_chain()
@@ -302,17 +311,17 @@
                     try:
                         if p.dataset is not None:
                             for k in p.dataset:
                                 g[k] = p.dataset[k]
                         for k in p.attribute_mirror_ns():
                             g[k] = chain[-2]._global_ns[k]
                         if (p.ns_string != '' and p.ns_string is not None):
-                            #exec(p.ns_string, g, ll)
-                            #for k in ll: g[k] = ll[k]
-                            exec(p.ns_string, g)
+                            #exec(p.ns_string, g)
+                            #print("updating with ns", p)
+                            g.update(p._global_ns)
 
                     except Exception as e:
                         import traceback
                         assert False, traceback.format_exc()
             if self.dataset is not None:
                 for k in self.dataset:
                     g[k] = self.dataset[k]
@@ -337,15 +346,15 @@
         # step 4 run namespace scripts otherise exit
         for k in l:
             g[k] = l[k]  # copying default ns
 
         try:
             l = {}
             if (self.ns_string != '' and self.ns_string is not None):
-                #exec(self.ns_string, g, l)
+                #print("executing...", self, self.ns_string)
                 exec(self.ns_string, g)
             else:
                 pass  # return
         except Exception as e:
             import traceback
             assert False, traceback.format_exc()
```

### Comparing `PetraM_Base-2.1.30/petram/phys/aux_operator.py` & `petram_base-2.1.38/petram/phys/aux_operator.py`

 * *Files 2% similar despite different names*

```diff
@@ -214,21 +214,19 @@
 
             cotype = self.coeff_type[0]
             c_coeff1 = self.get_coefficient_from_expression(coeff, cotype,
                                                             use_dual=False,
                                                             real=True,
                                                             is_conj=False)
             if is_complex:
-                c_coeff2 = self.get_coefficient_from_expression(coeff, cotype,
-                                                                use_dual=False,
-                                                                real=False,
-                                                                is_conj=False)
+                c_coeff = (c_coeff1.get_real_coefficient(),
+                           c_coeff1.get_imag_coefficient(),)
+
             else:
-                c_coeff2 = None
-            c_coeff = (c_coeff1, c_coeff2)
+                c_coeff = (c_coeff1, None)
 
             expr = Expression(oprt, engine=engine, trial=fes1, test=fes2,
                               trial_ess_tdof=trial_ess_tdof,
                               test_ess_tdof=test_ess_tdof,
                               ind_vars=ind_vars,
                               is_complex=is_complex,
                               c_coeff=c_coeff)
```

### Comparing `PetraM_Base-2.1.30/petram/phys/aux_variable.py` & `petram_base-2.1.38/petram/phys/aux_variable.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 from petram.model import Domain, Bdry, ModelDict
 from petram.phys.vtable import VtableElement, Vtable
 
 
 import petram.debug
 dprint1, dprint2, dprint3 = petram.debug.init_dprints('AUX_Variable')
 
-#groups = ['Domain', 'Boundary', 'Edge', 'Point', 'Pair']
+# groups = ['Domain', 'Boundary', 'Edge', 'Point', 'Pair']
 groups = ['Domain', 'Boundary', 'Pair']
 
 data0 = [("oprt_diag", VtableElement("oprt_diag", type='array',
                                      guilabel="diag", default="0.0",
                                      tip="oprator (diag)",)),
          ("rhs_vec", VtableElement("rhs_vec", type='array',
                                    guilabel="rhs", default="0.0",
@@ -50,15 +50,15 @@
         v["jmatrix_config"] = None
         v = self.vt_diag_rhs.attribute_set(v)
 
         if not hasattr(self, '_vt_array'):
             self._vt_array = []
         for vt in self.vt_array:
             v = vt.attribute_set(v)
-            #vv = vt.attribute_set({})
+            # vv = vt.attribute_set({})
             # for key in vv:
             #    if hasattr(self, key): vv[key] = getattr(self, key)
             #    v[key] = vv[key]
         return v
 
     def save_attribute_set(self, skip_def_check):
         attrs = super(AUX_Variable, self).save_attribute_set(skip_def_check)
@@ -236,15 +236,15 @@
         else:
             self.aux_connection[max(keys)+1] = (pnames[0], 0)
         evt.GetEventObject().TopLevelParent.OnItemSelChanged()
 
     def onRmConnection(self, evt):
         if len(self._vt_array) < 1:
             return
-        keys = self.aux_connection.keys()
+        keys = list(self.aux_connection.keys())
         del self.aux_connection[keys[-1]]
         self._vt_array = self._vt_array[:-1]
         evt.GetEventObject().TopLevelParent.OnItemSelChanged()
 
     def has_extra_DoF2(self, kfes, phys, jmatrix):
         if not self.timestep_config[jmatrix]:
             return False
@@ -330,33 +330,41 @@
                                   ind_vars=ind_vars, is_complex=is_complex)
                 t2 = expr.assemble(g=self._global_ns)
                 if diag_size > -1:
                     # print t1.shape, t2.shape
                     assert diag_size == t2.shape[1], "t1 and t2 shapes are inconsistent"
                 diag_size = t2.shape[1]
 
+
+        if diag_size < 0:
+            diag_size = len(np.atleast_1d(rhs_vec))
+
         from mfem.common.chypre import IdentityPyMat, Array2PyVec
         if diag is not None:
             if not self.get_root_phys().is_complex():
                 diag = diag.real
             t3 = IdentityPyMat(diag_size, diag=diag)
 
         # all node does do the same job, but Array2PyVec will use the data from
         # root node.
 
-        rhs = np.atleast_1d(rhs_vec).astype(float)
+        rhs = np.atleast_1d(rhs_vec)
         if diag_size != 1 and len(rhs) == 1:
             rhs = np.hstack([rhs[0]]*diag_size).flatten()
 
         if self.get_root_phys().is_complex():
-            rhs = rhs.astype(complex, copy=False)
-        if not self.get_root_phys().is_complex():
+            rhs = np.atleast_1d(rhs).astype(complex)
+        else:
             if np.iscomplexobj(rhs):
                 rhs = rhs.real
 
+        #if not self.get_root_phys().is_complex():
+        #    if np.iscomplexobj(rhs):
+        #        rhs = rhs.real
+
         t4 = Array2PyVec(rhs)
 
         '''
         Format of extra.
         [M,  t2]   [  ]
         [      ] = [  ]
         [t1, t3]   [t4]
```

### Comparing `PetraM_Base-2.1.30/petram/phys/coefficient.py` & `petram_base-2.1.38/petram/phys/coefficient.py`

 * *Files 3% similar despite different names*

```diff
@@ -171,58 +171,101 @@
 
             if return_mfem_constant:
                 return mfem.MatrixConstantCoefficient(e)
             else:
                 return PhysMatrixConstant(e)
 
 
-def DCoeff(dim, exprs, ind_vars, l, g,
+def DCoeff(dim, exprs, ind_vars, l, g, return_complex=False,
            return_mfem_constant=False, **kwargs):
     if isinstance(exprs, str):
         exprs = [exprs]
     if isinstance(exprs, NativeCoefficientGenBase):
         exprs = [exprs]
 
-    class DCoeff(MatrixPhysCoefficient):
-        def __init__(self, *args, **kwargs):
-            self.conj = kwargs.pop('conj', False)
-            self.scale = kwargs.pop('scale', 1.0)
-            self.space_dim = args[0]
-            super(DCoeff, self).__init__(*args, **kwargs)
+    class DCoeff_Base(object):
+        def __init__(self, conj=False, scale=1.0):
+            self.conj = conj
+            self.scale = scale
 
-        def EvalValue(self, x):
-            from petram.phys.phys_model import Coefficient_Evaluator
-            val = Coefficient_Evaluator.EvalValue(self, x)
-            val = np.diag(val)
+        def proc_value(self, val):
             val = val * self.scale
             if self.conj:
                 val = np.conj(val)
+            return val
 
+    class DCoeff(MatrixPhysCoefficient, DCoeff_Base):
+        def __init__(self, sdim, exprs, ind_vars, l, g,
+                     conj=False, scale=1.0, **kwargs):
+            DCoeff_Base.__init__(self, conj=conj, scale=scale)
+            MatrixPhysCoefficient.__init__(
+                self, sdim, exprs, ind_vars, l, g, **kwargs)
+
+        def EvalValue(self, x):
+            from petram.phys.phys_model import Coefficient_Evaluator
+            val = Coefficient_Evaluator.EvalValue(self, x)
+            val = np.diag(val)
+            val = self.proc_value(val)
             if np.iscomplexobj(val):
                 if self.real:
                     return val.real
                 else:
                     return val.imag
             elif not self.real:
                 return val * 0.0
             else:
                 return val
 
+    class DCoeffCC(Coefficient_Evaluator, DCoeff_Base, CC_Matrix):
+        def __init__(self, dim, exprs, ind_vars, l,
+                     g, conj=False, scale=1.0, **kwargs):
+            DCoeff_Base.__init__(self, conj=conj, scale=scale)
+            # real is not used...
+            Coefficient_Evaluator.__init__(
+                self, exprs, ind_vars, l, g, real=True)
+            CC_Matrix.__init__(self, dim, dim)
+
+        def eval(self, T, ip):
+            for n, v in self.variables:
+                v.set_point(T, ip, self.g, self.l)
+            x = T.Transform(ip)
+            val = Coefficient_Evaluator.EvalValue(self, x)
+            val = np.diag(val)
+            return self.proc_value(val)
+
+            raise NotImplementedError
+
     conj = kwargs.get('conj', False)
     real = kwargs.get('real', True)
     scale = kwargs.get('scale', 1.0)
 
     #print("matrix exprs", exprs)
 
     if any([isinstance(ee, str) for ee in exprs]):
-        from petram.mfem_config import allow_python_function_coefficient
-        if allow_python_function_coefficient != "allow":
-            print("JIT is not supported in DCoeff")
-            assert False, "can not jit coefficient"
-        return DCoeff(dim, exprs, ind_vars, l, g, **kwargs)
+        from petram.phys.numba_coefficient import expr_to_numba_coeff
+
+        coeff = expr_to_numba_coeff(exprs, mfem.jit.matrix,
+                                    ind_vars, conj, scale, g, l,
+                                    return_complex, shape=(dim, dim),
+                                    diag_mode=True)
+        if coeff is None:
+            msg = "JIT is not possbile. Continuing with Python mode"
+            handle_allow_python_function_coefficient(msg)
+        else:
+            if return_complex:
+                return coeff
+            else:
+                if real:
+                    return coeff.real
+                else:
+                    return coeff.imag
+        if return_complex:
+            return DCCoeff(dim, exprs, ind_vars, l, g, **kwargs)
+        else:
+            return DCoeff(dim, exprs, ind_vars, l, g, **kwargs)
     else:
         e = exprs
 
         if isinstance(e[0], NativeCoefficientGenBase):
             return call_nativegen(e[0], l, g, real, conj, scale)
 
         e = e * scale
```

### Comparing `PetraM_Base-2.1.30/petram/phys/distance/distance_model.py` & `petram_base-2.1.38/petram/phys/distance/distance_model.py`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/phys/distance/wall.py` & `petram_base-2.1.38/petram/phys/distance/wall.py`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/phys/numba_coefficient.py` & `petram_base-2.1.38/petram/phys/numba_coefficient.py`

 * *Files 2% similar despite different names*

```diff
@@ -792,28 +792,30 @@
 
 '''
 
 
 def _expr_to_numba_coeff(txt, jitter, ind_vars, conj, scale, g, l,
                          return_complex, **kwargs):
 
+    diag_mode = kwargs.pop("diag_mode", False)
+
     ind_vars = [xx.strip() for xx in ind_vars.split(',')]
     code = compile(txt.strip(), '<string>', 'eval')
     names = code.co_names
 
     dependency = []
     dep_names = []
 
     l = l.copy()
     for n in g:
         if isinstance(g[n], Variable):
             if n not in l:
                 l[n] = g[n]
             else:
-                assert False, "name confict: " + n + " is defined in local namespace"
+                assert False, "name conflict: " + n + " is defined in local namespace"
 
     for n in names:
         if n in ind_vars:
             continue
 
         dep = None
         if n in l:
@@ -856,17 +858,24 @@
         f0 += '):'
 
         func_txt = [f0]
         for k, xx in enumerate(ind_vars):
             func_txt.append("   " + xx + " = ptx[" + str(k) + "]")
         if objmode:
             func_txt.append("   with objmode(_out_='"+return_type+"'):")
-            func_txt.append("       _out_ =" + txt)
+            if diag_mode:
+                func_txt.append("       _out_ = np.diag(" + txt + ")")
+            else:
+                func_txt.append("       _out_ =" + txt)
         else:
-            func_txt.append("   _out_ =" + txt)
+            if diag_mode:
+                func_txt.append("   _out_ = np.diag(" + txt + ")")
+            else:
+                func_txt.append("   _out_ =" + txt)
+
         func_txt.append("   if isinstance(_out_, list):")
         func_txt.append("         _out_ = np.array(_out_)")
         func_txt.append("   elif isinstance(_out_, tuple):")
         func_txt.append("         _out_ = np.array(_out_)")
         if scale != 1:
             func_txt.append("   _out_ = _out_ * " + str(scale))
         if conj:
```

### Comparing `PetraM_Base-2.1.30/petram/phys/phys.py` & `petram_base-2.1.38/petram/phys/phys.py`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/phys/phys_const.py` & `petram_base-2.1.38/petram/phys/phys_const.py`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/phys/phys_model.py` & `petram_base-2.1.38/petram/phys/phys_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,18 +22,23 @@
 dprint1, dprint2, dprint3 = debug.init_dprints('Phys')
 
 if use_parallel:
     import mfem.par as mfem
 else:
     import mfem.ser as mfem
 
+# constant
 
-# not that PyCoefficient return only real number array
+up2 = "\u00B2"  # upper script of 2
+lam = "\u03BB"  # lambda
+txt_dudt = 'du/dt or ' + lam + 'u'
+txt_du2dt2 = 'd' + up2 + "u/dt" + up2 + ' or ' + lam + up2 + "u"
 
 
+# not that PyCoefficient return only real number array
 class PhysConstant(mfem.ConstantCoefficient):
     def __init__(self, value):
         self.value = value
         mfem.ConstantCoefficient.__init__(self, value)
 
     def __repr__(self):
         return self.__class__.__name__ + "(" + str(self.value) + ")"
@@ -64,20 +69,20 @@
 def try_eval(exprs, l, g):
     '''
     first evaulate as it is
     if the result is list.. return
     if not evaluate w/o knowing any Variables
     '''
     try:
-        value = eval(exprs, l, g)
+        value = eval(exprs, g, l)
         if isinstance(value, list):
             return True, [value]
         ll = [x for x in l if not isinstance(x, Variable)]
         gg = [x for x in g if not isinstance(x, Variable)]
-        value = eval(exprs, ll, gg)
+        value = eval(exprs, gg, ll)
         return True, [value]
     except BaseException:
         return False, exprs
 
 
 class Coefficient_Evaluator(object):
     def __init__(self, exprs, ind_vars, l, g, real=True):
@@ -91,52 +96,62 @@
 
            matrix
               given as string like '[0, 1, 2, 3, 4]'
               if variable is used it is become string element '['=variable', 1, 2, 3, 4]'
               if =Varialbe in matrix form, it is passed as [['Variable']]
         '''
         flag, exprs = try_eval(exprs, l, g)
-        #print("after try_eval", flag, exprs)
+
+        # print("after try_eval", flag, exprs)
         if not flag:
             if isinstance(exprs, str):
                 exprs = [exprs]
             # elif isinstance(exprs, float):
             #    exprs = [exprs]
             # elif isinstance(exprs, long):
             #    exprs = [exprs]
             elif isinstance(exprs, numbers.Number):
                 exprs = [exprs]
             else:
                 pass
         if isinstance(exprs, list) and isinstance(exprs[0], list):
             exprs = exprs[0]
-        #dprint1("final exprs", exprs)
+        # dprint1("final exprs", exprs)
         self.l = {}
+
         # TODO g must be copied since some may passs _global_ns.
         # (I don't do it now since it requires a substantial testing)
-        self.g = g
+        # (2024 this needs to be copied for parametric scan works)
+        self.g = g.copy()
+
         for key in l.keys():
             self.g[key] = l[key]
         self.real = real
         self.variables = []
 
         self.co = []
 
         for expr in exprs:
             if isinstance(expr, str):
                 code = compile(expr.strip(), '<string>', 'eval')
                 names = code.co_names
                 for n in names:
-                    if (n in g and isinstance(g[n], NativeCoefficientGenBase)):
-                        coeff_var = CoefficientVariable(g[n], l, g)
+                    if (n in self.g and isinstance(self.g[n], NativeCoefficientGenBase)):
+                        coeff_var = CoefficientVariable(self.g[n], l, self.g)
                         self.variables.append((n, coeff_var))
-                    elif n in g and isinstance(g[n], Variable):
-                        self.variables.append((n, g[n]))
-                        for nn in g[n].dependency:
-                            self.variables.append((nn, g[nn]))
+                    elif n in self.g and isinstance(self.g[n], Variable):
+                        self.variables.append((n, self.g[n]))
+                        for nn in self.g[n].dependency:
+                            self.variables.append((nn, self.g[nn]))
+                        for nn in self.g[n].div:
+                            self.variables.append((nn, self.g[nn]))
+                        for nn in self.g[n].curl:
+                            self.variables.append((nn, self.g[nn]))
+                        for nn in self.g[n].grad:
+                            self.variables.append((nn, self.g[nn]))
                     else:
                         pass
                 self.co.append(code)
             else:
                 self.co.append(expr)
 
         # 'x, y, z' -> 'x', 'y', 'z'
@@ -479,14 +494,35 @@
         default, return true for B not M
         '''
         if self._update_flag:
             if mode == 'B':
                 return True
         return False
 
+    def has_extra_coupling(self):
+        '''
+        True if it define coupling between Lagrange multipliers
+        '''
+        return False
+
+    def extra_coupling_names(self):
+        '''
+        return its own extra_name, and paired (coupled) extra_names
+        '''
+        return None, []
+
+    def get_extra_coupling(self, target_name):
+        '''
+        [    t2][paired extra]
+        [t1    ][extra]
+        t1 = (size of extra, size of targert_extra)
+        t2 = (size of target_extra, size of extra)
+        '''
+        return None, None
+
     def has_bf_contribution(self, kfes):
         return False
 
     def has_bf_contribution2(self, kfes, jmatrix):
         '''
         subclass has to overwrite this if extra DoF can couple
         with other FES.
@@ -689,17 +725,17 @@
 
     def panel4_param(self):
         setting = {"text": ' '}
         if self.has_essential:
             ll = [['', False, 3, {"text": "Time dependent"}], ]
 
         else:
-            ll = [['y(t)', True, 3, {"text": ""}],
-                  ['dy/dt', False, 3, {"text": ""}],
-                  ['d2y/dt2', False, 3, {"text": ""}],
+            ll = [['u', True, 3, {"text": ""}],
+                  [txt_dudt, False, 3, {"text": ""}],
+                  [txt_du2dt2, False, 3, {"text": ""}],
                   ['Gradient', False, 3, {"text": ""}],
                   ['Varying (in time/for loop) Term.', False, 3, {"text": ""}], ]
         if self.allow_custom_intorder:
             ll.append(['Increase int. order', '0', 400, ''])
         return ll
 
     def panel4_tip(self):
@@ -948,50 +984,57 @@
         from petram.phys.coefficient import SCoeff, VCoeff, DCoeff, MCoeff
 
         if self.get_root_phys().vdim > 1:
             dim = self.get_root_phys().vdim
         else:
             dim = self.get_root_phys().geom_dim
 
+        return_complex = self.get_root_phys().is_complex()
+
         if cotype == 'S':
             # for b in self.itg_choice():
             #   if b[0] == self.integrator: break
             # if not "S*2" in b[3]:
             if not use_dual:
                 c_coeff = SCoeff(c, self.get_root_phys().ind_vars,
                                  self._local_ns, self._global_ns,
+                                 return_complex=return_complex,
                                  real=real, conj=is_conj)
             else:  # so far this is only for an elastic integrator
                 c_coeff = (SCoeff(c, self.get_root_phys().ind_vars,
                                   self._local_ns, self._global_ns,
+                                  return_complex=return_complex,
                                   real=real, conj=is_conj, component=0),
                            SCoeff(c, self.get_root_phys().ind_vars,
                                   self._local_ns, self._global_ns,
+                                  return_complex=return_complex,
                                   real=real, conj=is_conj, component=1))
         elif cotype == 'V':
             c_coeff = VCoeff(dim, c, self.get_root_phys().ind_vars,
                              self._local_ns, self._global_ns,
+                             return_complex=return_complex,
                              real=real, conj=is_conj)
         elif cotype == 'M':
             c_coeff = MCoeff(dim, c, self.get_root_phys().ind_vars,
                              self._local_ns, self._global_ns,
+                             return_complex=return_complex,
                              real=real, conj=is_conj)
         elif cotype == 'D':
             c_coeff = DCoeff(dim, c, self.get_root_phys().ind_vars,
                              self._local_ns, self._global_ns,
+                             return_complex=return_complex,
                              real=real, conj=is_conj)
         return c_coeff
 
     def compile_coeffs(self, *kargs):
         '''
         jit compile coefficient
         '''
         pass
 
-
 data = [("order", VtableElement("order", type='int',
                                 guilabel="order", no_func=True,
                                 default=1, tip="element order",))]
 
 
 class PhysModule(Phys):
     hide_ns_menu = False
@@ -1217,28 +1260,29 @@
 
         # (note) BilinearForm does not suppoert delta coefficent
         return [WF_WeakPointBilinConstraint, WF_WeakPointLinConstraint]
 
     def get_possible_child(self):
         from petram.phys.aux_variable import AUX_Variable
         from petram.phys.aux_operator import AUX_Operator
-        return [AUX_Variable, AUX_Operator]
+        from petram.phys.variable_coupling import VariableCoupling
+        return [AUX_Variable, AUX_Operator, VariableCoupling]
 
     def get_possible_pair(self):
         from petram.phys.projection import BdrProjection, DomainProjection
         return [DomainProjection, BdrProjection, ]
 
     def soldict_to_solvars(self, soldict, variables):
         keys = list(soldict)
         depvars = self.dep_vars
         suffix = self.dep_vars_suffix
         ind_vars = [x.strip() for x in self.ind_vars.split(',')]
 
         for k in keys:
-            n = k.split('_')[0]
+            n = "_".join(k.split('_')[:-1])
             if n in depvars:
                 sol = soldict[k]
                 solr = sol[0]
                 soli = sol[1] if len(sol) > 1 else None
                 self.add_variables(variables, n, solr, soli)
 
         # collect all definition (domain specific expressions) from children
@@ -1247,15 +1291,14 @@
                 continue
             if mm is self:
                 continue
 
             mm.add_domain_variables(variables, n, suffix, ind_vars)
             mm.add_bdr_variables(variables, n, suffix, ind_vars)
 
-
     def onItemSelChanged(self, evt):
         '''
         GUI response when model object is selected in
         the dlg_edit_model
         '''
         viewer = evt.GetEventObject().GetTopLevelParent().GetParent()
         viewer.set_view_mode('phys', self)
```

### Comparing `PetraM_Base-2.1.30/petram/phys/projection.py` & `petram_base-2.1.38/petram/phys/projection.py`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/phys/pycomplex_coefficient.py` & `petram_base-2.1.38/petram/phys/pycomplex_coefficient.py`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/phys/vtable.py` & `petram_base-2.1.38/petram/phys/vtable.py`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/phys/weakform.py` & `petram_base-2.1.38/petram/phys/weakform.py`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/phys/wf/pix_gen.py` & `petram_base-2.1.38/petram/phys/wf/pix_gen.py`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/phys/wf/wf_constraints.py` & `petram_base-2.1.38/petram/phys/wf/wf_constraints.py`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/phys/wf/wf_essential.py` & `petram_base-2.1.38/petram/phys/wf/wf_essential.py`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/phys/wf/wf_model.py` & `petram_base-2.1.38/petram/phys/wf/wf_model.py`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/phys/wf/wf_natural.py` & `petram_base-2.1.38/petram/phys/wf/wf_natural.py`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/phys/wf/wf_pairs.py` & `petram_base-2.1.38/petram/phys/wf/wf_pairs.py`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/pi/dlg_edit_model.py` & `petram_base-2.1.38/petram/pi/dlg_edit_model.py`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/pi/dlg_plot_expr.py` & `petram_base-2.1.38/petram/pi/dlg_plot_expr.py`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/pi/dlg_plot_sol.py` & `petram_base-2.1.38/petram/pi/dlg_plot_sol.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,21 +35,27 @@
 
 def setup_figure(fig, fig2):
     fig.nsec(1)
     fig.threed('on')
     fig.property(fig.get_axes(0), 'axis', False)
     fig.get_page(0).set_nomargin(True)
     fig.property(fig.get_page(0), 'bgcolor', 'white')
+
+    aspect = fig2.property(fig2.get_axes(0), 'aspect')
+    fig.property(fig.get_axes(0), 'aspect', aspect)
+
     xlim = fig2.xlim()
     ylim = fig2.ylim()
     zlim = fig2.zlim()
     fig.xlim(xlim)
     fig.ylim(ylim)
     fig.zlim(zlim)
 
+    fig.view('noclip')
+
 
 def read_solinfo_remote(user, server, path):
     txt = "$PetraM/bin/get_soldir_info.sh " + path
     command = ["ssh",  "-o",
                "PasswordAuthentication=no",
                "-o",
                "PreferredAuthentications=publickey",
@@ -229,17 +235,17 @@
             p.SetSizer(vbox)
 
             choices = list(mfem_model['Phys'])
             choices = [mfem_model['Phys'][c].fullpath() for c in choices]
 
             if len(choices) == 0:
                 choices = ['no physcs in mode']
-            ll = [['x', 'x', 0, {}],
-                  ['y', 'y', 0, {}],
-                  ['z', 'z', 0, {}],
+            ll = [['x', 'x', 500, {}],
+                  ['y', 'y', 500, {}],
+                  ['z', 'z', 500, {}],
                   ['Boundary Index', text, 0, {}],
                   ['NameSpace', choices[0], 4, {'style': wx.CB_READONLY,
                                                 'choices': choices}],
                   ['Color', ['blue', 'none'], 506, {}],
                   [None, True, 3, {"text": 'merge solutions'}],
                   [None, True, 3, {"text": 'keep surface separated'}],
                   [None, True, 3, {"text": 'show edge only'}], ]
@@ -287,15 +293,15 @@
                                     'choices': ['XYZ', 'Line  '],
                                     'cb_tip': "Point could generation mode",
                                     'call_fit': False},
                                    {'elp': elp1, 'tip': tip1},
                                    {'elp': elp2, 'tip': tip2},)]
             ll = [
                 [
-                    'Expression', '', 0, {}], ss, [
+                    'Expression', '', 500, {}], ss, [
                     'Selection', 'all', 4, {
                         'style': wx.CB_DROPDOWN, 'choices': [
                             'all', 'visible', 'hidden']}], [
                         'NameSpace', choices[0], 4, {
                             'style': wx.CB_READONLY, 'choices': choices}], [
                                 None, False, 3, {
                                     "text": 'dynamic extension'}], ]
@@ -623,15 +629,15 @@
                      {"choices": [self.config['cs_soldir'], ],
                       "choices_cb": self.remote_sollist, }],
                     ["Sub dir.", "None", 4, {"style": wx.CB_READONLY,
                                              "choices": ["", ]}, ],
                     [None, None, 141, {"alignright": True,
                                        "func": self.OnLoadRemoteSol,
                                        "noexpand": True,
-                                       "label": "Reload choices"}],]
+                                       "label": "Reload choices"}], ]
 
             tip3 = ("Remote server name",
                     "Numboer of worker processes on remoter server",
                     "Solution directory",
                     "Subdirectory",
                     None,)
 
@@ -1317,27 +1323,26 @@
             # if verts is 1D, treat it 2D plot even if data_x is None
             if data[0][0].shape[1] == 1:
                 data_x = [(None, verts[:, 0]) for verts, cdata, adata in data]
                 data = [(None, cdata) for verts, cdata, adata in data]
 
         if data_x is None:
             v = figure(viewer=cls)
-            v.update(False)
             v.title(expr + ':' + str(battrs))
             setup_figure(v, self.GetParent())
+
+            v.update(False)
             for verts, cdata, adata in data:
                 if cls is None:
                     v.solid(verts, adata, cz=True, cdata=cdata.astype(float),
                             shade='linear')
                 else:
                     v.solid(verts, adata, cz=True, cdata=cdata,
                             shade='linear')
             v.update(True)
-            v.view('noclip')
-            v.view('equal')
             v.update(False)
             ax = self.GetParent().get_axes()
             param = ax.get_axes3d_viewparam(ax._artists[0])
             ax2 = v.get_axes()
             ax2.set_axes3d_viewparam(param, ax2._artists[0])
             v.lighting(light=0.5)
             v.update(True)
@@ -1473,16 +1478,17 @@
             battrs,
             scale,
             cls=None,
             expr='',
             use_pointfill=False):
         from ifigure.interactive import figure
         viewer = figure(viewer=cls)
-        viewer.update(False)
         setup_figure(viewer, self.GetParent())
+
+        viewer.update(False)
         viewer.suptitle(expr + ':' + str(battrs))
 
         dd = defaultdict(list)
         # regroup to sepparte triangles and quads.
         for k, datasets in enumerate(data):
             v, c, i = datasets  # verts, cdata, idata
             idx = i.shape[-1]
@@ -1512,16 +1518,14 @@
             else:
                 obj = viewer.solid(verts, idata, array_idx=array_idx,
                                    cz=True, cdata=cdata, shade='linear',
                                    use_pointfill=use_pointfill)
                 obj.set_gl_hl_use_array_idx(True)
 
         viewer.update(True)
-        viewer.view('noclip')
-        viewer.view('equal')
         viewer.update(False)
         ax = self.GetParent().get_axes()
         param = ax.get_axes3d_viewparam(ax._artists[0])
         ax2 = viewer.get_axes()
         ax2.set_axes3d_viewparam(param, ax2._artists[0])
         viewer.lighting(light=0.5)
         viewer.update(True)
@@ -1773,33 +1777,33 @@
             param,
             cls=None,
             expr=False):
         value = self.elps['Points'] .GetValue()
 
         from ifigure.interactive import figure
         viewer = figure(viewer=cls)
+        setup_figure(viewer, self.GetParent())
+
         viewer.update(False)
         viewer.suptitle(expr + ':' + str(attrs))
 
         if param['pc_type'] == 'line':
             pc_param = param['pc_param']
             sp = np.array(pc_param[0])
             ep = np.array(pc_param[1])
             num = pc_param[2]
             ii = np.linspace(0, 1., num)
             ptx = np.vstack([sp * (1 - i) + ep * i for i in ii])
             if ptx.shape(-1) == 3:
-                setup_figure(viewer, self.GetParent())
+                #setup_figure(viewer, self.GetParent())
                 viewer.plot(ptx[:, 0], ptx[:, 1], ptx[:, 2],
                             c=data.real, cz=True)
             else:
                 viewer.plot(data.real)
 
-        viewer.view('noclip')
-        viewer.view('equal')
         ax = self.GetParent().get_axes()
         param = ax.get_axes3d_viewparam(ax._artists[0])
         ax2 = viewer.get_axes()
         ax2.set_axes3d_viewparam(param, ax2._artists[0])
         viewer.lighting(light=0.5)
         viewer.update(True)
 
@@ -2002,25 +2006,24 @@
         kwargs = {'facecolor': c1,
                   'edgecolor': c2, }
         if c2 == (0, 0, 0, 0):
             kwargs['linewidth'] = 0.
 
         from ifigure.interactive import figure
         v = figure()
-        v.update(False)
         setup_figure(v, self.GetParent())
+
+        v.update(False)
         v.suptitle('Boundary ' + str(battrs))
         for xdata, ydata, zdata in zip(x, y, z):
             verts = np.vstack((xdata[1], ydata[1], zdata[1])).transpose()
             adata = xdata[2]
             v.solid(verts, adata, **kwargs)
 
         v.update(True)
-        v.view('noclip')
-        v.view('equal')
         v.update(False)
         ax = self.GetParent().get_axes()
         param = ax.get_axes3d_viewparam(ax._artists[0])
         ax2 = v.get_axes()
         ax2.set_axes3d_viewparam(param, ax2._artists[0])
         v.lighting(light=0.5)
         v.update(True)
@@ -2113,17 +2116,19 @@
                             cls=cls)
 
     def make_plot_bdrarrow(self, u, v, w, battrs, value,
                            expr_u='', expr_v='', expr_w='',
                            cls=None):
 
         from ifigure.interactive import figure
+
         viewer = figure(viewer=cls)
-        viewer.update(False)
         setup_figure(viewer, self.GetParent())
+
+        viewer.update(False)
         viewer.suptitle(
             '[' + ','.join((expr_u, expr_v, expr_w)) + '] : ' + str(battrs))
 
         allxyz = np.vstack([udata[0] for udata in u])
         dx = np.max(allxyz[:, 0]) - np.min(allxyz[:, 0])
         if allxyz.shape[1] > 1:
             dy = np.max(allxyz[:, 1]) - np.min(allxyz[:, 1])
@@ -2155,16 +2160,15 @@
             else:
                 z = x * 0.
 
             viewer.quiver3d(x, y, z, u[idx], v[idx], w[idx],
                             length=length)
 
         viewer.update(True)
-        viewer.view('noclip')
-        viewer.view('equal')
+
         viewer.update(False)
         ax = self.GetParent().get_axes()
         param = ax.get_axes3d_viewparam(ax._artists[0])
         ax2 = viewer.get_axes()
         ax2.set_axes3d_viewparam(param, ax2._artists[0])
         viewer.lighting(light=0.5)
         viewer.update(True)
@@ -2367,46 +2371,47 @@
                     dataset,
                     cls=cls,
                     expr=expr)
 
     def make_plot_slice(self, dataset, battrsset, cls=None, expr=''):
         from ifigure.interactive import figure
         v = figure(viewer=cls)
-        v.update(False)
         setup_figure(v, self.GetParent())
 
+        v.update(False)
+
         first = True
         for data,  battrs in zip(dataset, battrsset):
             if first:
                 v.suptitle(expr + ':' + str(battrs))
                 first = False
             for verts, cdata, adata in data:
                 if cls is None:
                     v.solid(verts, adata, cz=True, cdata=cdata.astype(float),
                             shade='linear')
                 else:
                     v.solid(verts, adata, cz=True, cdata=cdata, shade='linear')
 
         v.update(True)
-        v.view('noclip')
-        v.view('equal')
+
         v.update(False)
         ax = self.GetParent().get_axes()
         param = ax.get_axes3d_viewparam(ax._artists[0])
         ax2 = v.get_axes()
         ax2.set_axes3d_viewparam(param, ax2._artists[0])
         v.lighting(light=0.5)
         v.update(True)
 
     def make_plot_pc_slice(self, dataset, cls=None, expr=False):
 
         from ifigure.interactive import figure
         viewer = figure(viewer=cls)
-        viewer.update(False)
         setup_figure(viewer, self.GetParent())
+
+        viewer.update(False)
         viewer.threed('on')
 
         first = True
         for d in dataset:
             data = d['data']
             attrs_out = d['attrs_out']
             attrs = d['attrs']
@@ -2424,16 +2429,14 @@
                         attrs_out, attrs, invert=True))
             else:
                 data = np.ma.masked_array(
                     data, mask=np.in1d(
                         attrs_out, attrs, invert=True))
             viewer.image(x, y, data, im_axes=im_axes, im_center=im_center)
 
-            viewer.view('noclip')
-            viewer.view('equal')
             ax = self.GetParent().get_axes()
             param = ax.get_axes3d_viewparam(ax._artists[0])
             ax2 = viewer.get_axes()
             ax2.set_axes3d_viewparam(param, ax2._artists[0])
             viewer.lighting(light=0.5)
 
         viewer.update(True)
@@ -2513,21 +2516,34 @@
         expr = str(value[0]).strip()
         xexpr = str(value[1]).strip()
 
         xdata, data = self.eval_probe(mode='plot')
         if data is None:
             wx.CallAfter(self.set_title_no_status)
             return
+        if xdata is None:
+            wx.CallAfter(self.set_title_no_status)
+            return
+        if len(data.shape) == 0:
+            wx.CallAfter(self.set_title_no_status)
+            return
+
         self.post_threadend(
             self.make_plot_probe, (xdata, data), expr=expr, xexpr=xexpr)
 
     def onExportProbe(self, evt):
         value = self.elps['Probe'] .GetValue()
         xdata, data = self.eval_probe(mode='plot')
 
+        if data is None:
+            return
+        if xdata is None:
+            return
+        if len(data.shape) == 0:
+            return
         data = {'xdata': xdata, 'data': data}
         self.export_to_piScope_shell(data, 'probe_data')
 
     def make_plot_probe(self, data, expr='', xexpr='', cls=None):
         from ifigure.interactive import figure
         v = figure(viewer=cls)
         v.update(False)
@@ -2640,14 +2656,15 @@
 
     def evaluate_sol_bdr(self, expr, battrs, phys_path, do_merge1, do_merge2,
                          **kwargs):
         '''
         evaluate sol using boundary evaluator
         '''
         model = self.GetParent().model
+
         solfiles = self.get_model_soldfiles()
         mfem_model = model.param.getvar('mfem_model')
         phys_ns = mfem_model[str(phys_path)]._global_ns.copy()
 
         if solfiles is None:
             wx.CallAfter(dialog.showtraceback, parent=self,
                          txt='Solution does not exist',
@@ -3022,15 +3039,16 @@
         app = wx.GetApp().TopWindow
         app.shell.lvar[dataname] = data
         app.shell.SendShellEnterEvent()
         ret = dialog.message(app, dataname + ' is exported', 'Export', 0)
 
     def get_model_soldfiles(self):
         model = self.GetParent().model
-        solfiles = model.variables.getvar('solfiles')
         soldir = model.variables.getvar('remote_soldir')
 
         if not self.config['use_cs']:
+            self.load_sol_if_needed()
+            solfiles = model.variables.getvar('solfiles')
             return solfiles
         else:
             soldir = os.path.join(soldir, self.config["cs_solsubdir"])
             return soldir
```

### Comparing `PetraM_Base-2.1.30/petram/pi/dlg_submit_job.py` & `petram_base-2.1.38/petram/pi/dlg_submit_job.py`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/pi/ns_utils.py` & `petram_base-2.1.38/petram/pi/ns_utils.py`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/pi/pfz2script.py` & `petram_base-2.1.38/petram/pi/pfz2script.py`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/pi/project_scripts/convert_mesh.py` & `petram_base-2.1.38/petram/pi/project_scripts/convert_mesh.py`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/pi/project_scripts/helpers/call_glvis.py` & `petram_base-2.1.38/petram/pi/project_scripts/helpers/call_glvis.py`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/pi/project_scripts/helpers/eval_expr.py` & `petram_base-2.1.38/petram/pi/project_scripts/helpers/eval_expr.py`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/pi/project_scripts/run_parallel.py` & `petram_base-2.1.38/petram/pi/project_scripts/run_parallel.py`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/pi/project_scripts/run_serial.py` & `petram_base-2.1.38/petram/pi/project_scripts/run_serial.py`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/pi/sel_buttons.py` & `petram_base-2.1.38/petram/pi/sel_buttons.py`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/pi/selection_palette.py` & `petram_base-2.1.38/petram/pi/selection_palette.py`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/pi/shell_commands.py` & `petram_base-2.1.38/petram/pi/shell_commands.py`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/pi/simple_frame_plus.py` & `petram_base-2.1.38/petram/pi/simple_frame_plus.py`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/pi/widget_forms.py` & `petram_base-2.1.38/petram/pi/widget_forms.py`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/pi/widget_init.py` & `petram_base-2.1.38/petram/pi/widget_init.py`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/pi/widget_nl.py` & `petram_base-2.1.38/petram/pi/widget_nl.py`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/pi/widget_smoother.py` & `petram_base-2.1.38/petram/pi/widget_smoother.py`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/pi/widgets.py` & `petram_base-2.1.38/petram/pi/widgets.py`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/postprocess/discrt_v_integration.py` & `petram_base-2.1.38/petram/postprocess/discrt_v_integration.py`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/postprocess/discrt_v_interpolator.py` & `petram_base-2.1.38/petram/postprocess/discrt_v_interpolator.py`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/postprocess/pp_model.py` & `petram_base-2.1.38/petram/postprocess/pp_model.py`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/postprocess/project_solution.py` & `petram_base-2.1.38/petram/postprocess/project_solution.py`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/remote/client_script.py` & `petram_base-2.1.38/petram/remote/client_script.py`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/sol/bdr_nodal_evaluator.py` & `petram_base-2.1.38/petram/sol/bdr_nodal_evaluator.py`

 * *Files 5% similar despite different names*

```diff
@@ -110,14 +110,20 @@
     idx = []
 
     for n in names:
         if ((n in g and isinstance(g[n], NativeCoefficientGenBase)) or
                 (n in g and isinstance(g[n], Variable))):
             for nn in g[n].dependency:
                 idx = g[nn].get_emesh_idx(idx, g=g)
+            for nn in g[n].grad:
+                idx = g[nn].get_emesh_idx(idx, g=g)
+            for nn in g[n].div:
+                idx = g[nn].get_emesh_idx(idx, g=g)
+            for nn in g[n].curl:
+                idx = g[nn].get_emesh_idx(idx, g=g)
 
             idx.extend(g[n].get_emesh_idx(idx, g=g))
 
     if len(idx) == 0:
         # if expression has no emehs dependence return default.
         idx = [default]
     return list(set(idx))
@@ -167,14 +173,15 @@
     code = compile(expr, '<string>', 'eval')
     names = code.co_names
 
     g = {}
 
     for key in phys._global_ns.keys():
         g[key] = phys._global_ns[key]
+
     for key in solvars.keys():
         g[key] = solvars[key]
 
     ll_name = []
     ll_value = []
     var_g2 = var_g.copy()
 
@@ -195,21 +202,47 @@
     for n in all_names:
         if (n in g and isinstance(g[n], NativeCoefficientGenBase)):
             g[n+"_coeff"] = CoefficientVariable(g[n], g)
             new_names.append(n+"_coeff")
             name_translation[n+"_coeff"] = n
 
         elif (n in g and isinstance(g[n], NumbaCoefficientVariable)):
+            for x in g[n].dependency:
+                new_names.append(x)
+                name_translation[x] = x
+
             ind_vars = [xx.strip() for xx in phys.ind_vars.split(',')]
+            if g[n].has_dependency():
+                g[n].forget_jitted_coefficient()
             g[n].set_coeff(ind_vars, g)
             new_names.append(n)
             name_translation[n] = n
 
         elif (n in g and isinstance(g[n], Variable)):
-            new_names.extend(g[n].dependency)
+            for x in g[n].dependency:
+                new_names.append(x)
+                name_translation[x] = x
+
+            for x in g[n].grad:
+                new_names.append('grad'+x)
+                name_translation['grad'+x] = 'grad'+x
+                if 'grad'+x not in g:
+                    g['grad'+x] = g[x].generate_grad_variable()
+
+            for x in g[n].curl:
+                new_names.append('curl'+x)
+                name_translation['curl'+x] = 'curl'+x
+                if 'curl'+x not in g:
+                    g['curl'+x] = g[x].generate_curl_variable()
+            for x in g[n].div:
+                new_names.append('div'+x)
+                name_translation['div'+x] = 'div'+x
+                if 'div'+x not in g:
+                    g['div'+x] = g[x].generate_div_variable()
+
             new_names.append(n)
             name_translation[n] = n
 
         elif n in g:
             new_names.append(n)
             name_translation[n] = n
```

### Comparing `PetraM_Base-2.1.30/petram/sol/edge_nodal_evaluator.py` & `petram_base-2.1.38/petram/sol/edge_nodal_evaluator.py`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/sol/evaluator_agent.py` & `petram_base-2.1.38/petram/sol/evaluator_agent.py`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/sol/evaluator_cs.py` & `petram_base-2.1.38/petram/sol/evaluator_cs.py`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/sol/evaluator_mp.py` & `petram_base-2.1.38/petram/sol/evaluator_mp.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,14 @@
         self.task_queue = task_queue
         self.result_queue = result_queue
         self.text_queue = text_queue        
         self.myid = myid
         self.rank = rank
         self.agents = {}
         self.logfile = logfile
-        print("log file")
         #self.logfile = 'log'
         self.use_stringio = False
         self.solfiles = None
         
         ## enable it when checking performance        
         self.use_profiler = False
 
@@ -197,15 +196,14 @@
         #end of while
         self.task_queue.close()
         self.result_queue.close()
         
     def set_solfiles(self, solfiles):
         st, et = data_partition(len(solfiles.set), self.rank, self.myid)
         s = solfiles[st:et]
-        print(s)
         if len(s) > 0:
             self.solfiles_real = s
             self.solfiles = s
         else:
             self.solfiles = None
 
     def set_model(self, model_path):
```

### Comparing `PetraM_Base-2.1.30/petram/sol/evaluator_single.py` & `petram_base-2.1.38/petram/sol/evaluator_single.py`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/sol/evaluators.py` & `petram_base-2.1.38/petram/sol/evaluators.py`

 * *Files 0% similar despite different names*

```diff
@@ -159,14 +159,15 @@
         solsets = Solsets(self.solfiles)
 
         print("reading sol variables")
         if self.solfiles.has_parametic_data:
             self.set_parametric_data()
 
         phys_root = self.mfem_model()["Phys"]
+
         solvars = phys_root.make_solvars(solsets.set)
 
         # Setting _emesh_idx from emesh_idx in GridFunction
         for phys in phys_root:
             vnames = phys_root[phys].dep_vars
             gf_var = None
             for name in vnames:
```

### Comparing `PetraM_Base-2.1.30/petram/sol/integral_evaluator.py` & `petram_base-2.1.38/petram/sol/integral_evaluator.py`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/sol/listsoldir.py` & `petram_base-2.1.38/petram/sol/listsoldir.py`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/sol/ncedge_evaluator.py` & `petram_base-2.1.38/petram/sol/ncedge_evaluator.py`

 * *Files 7% similar despite different names*

```diff
@@ -71,20 +71,43 @@
         if (n in g and isinstance(g[n], NativeCoefficientGenBase)):
             g[n+"_coeff"] = CoefficientVariable(g[n], g)
             new_names.append(n+"_coeff")
             name_translation[n+"_coeff"] = n
 
         elif (n in g and isinstance(g[n], NumbaCoefficientVariable)):
             ind_vars = [xx.strip() for xx in phys.ind_vars.split(',')]
+            if g[n].has_dependency():
+                g[n].forget_jitted_coefficient()
             g[n].set_coeff(ind_vars, g)
             new_names.append(n)
             name_translation[n] = n
 
         elif (n in g and isinstance(g[n], Variable)):
-            new_names.extend(g[n].dependency)
+            for x in g[n].dependency:
+                new_names.append(x)
+                name_translation[x] = x
+
+            for x in g[n].grad:
+                new_names.append('grad'+x)
+                name_translation['grad'+x] = 'grad'+x
+                if 'grad'+x not in g:
+                    g['grad'+x] = g[x].generate_grad_variable()
+
+            for x in g[n].curl:
+                new_names.append('curl'+x)
+                name_translation['curl'+x] = 'curl'+x
+                if 'curl'+x not in g:
+                    g['curl'+x] = g[x].generate_curl_variable()
+
+            for x in g[n].div:
+                new_names.append('div'+x)
+                name_translation['div'+x] = 'div'+x
+                if 'div'+x not in g:
+                    g['div'+x] = g[x].generate_div_variable()
+
             new_names.append(n)
             name_translation[n] = n
 
         elif n in g:
             new_names.append(n)
             name_translation[n] = n
```

### Comparing `PetraM_Base-2.1.30/petram/sol/ncface_evaluator.py` & `petram_base-2.1.38/petram/sol/ncface_evaluator.py`

 * *Files 5% similar despite different names*

```diff
@@ -72,20 +72,43 @@
         if (n in g and isinstance(g[n], NativeCoefficientGenBase)):
             g[n+"_coeff"] = CoefficientVariable(g[n], g)
             new_names.append(n+"_coeff")
             name_translation[n+"_coeff"] = n
 
         elif (n in g and isinstance(g[n], NumbaCoefficientVariable)):
             ind_vars = [xx.strip() for xx in phys.ind_vars.split(',')]
+            if g[n].has_dependency():
+                g[n].forget_jitted_coefficient()
             g[n].set_coeff(ind_vars, g)
             new_names.append(n)
             name_translation[n] = n
 
         elif (n in g and isinstance(g[n], Variable)):
-            new_names.extend(g[n].dependency)
+            for x in g[n].dependency:
+                new_names.append(x)
+                name_translation[x] = x
+
+            for x in g[n].grad:
+                new_names.append('grad'+x)
+                name_translation['grad'+x] = 'grad'+x
+                if 'grad'+x not in g:
+                    g['grad'+x] = g[x].generate_grad_variable()
+
+            for x in g[n].curl:
+                new_names.append('curl'+x)
+                name_translation['curl'+x] = 'curl'+x
+                if 'curl'+x not in g:
+                    g['curl'+x] = g[x].generate_curl_variable()
+
+            for x in g[n].div:
+                new_names.append('div'+x)
+                name_translation['div'+x] = 'div'+x
+                if 'div'+x not in g:
+                    g['div'+x] = g[x].generate_div_variable()
+
             new_names.append(n)
             name_translation[n] = n
 
         elif n in g:
             new_names.append(n)
             name_translation[n] = n
```

### Comparing `PetraM_Base-2.1.30/petram/sol/nodal_refinement.py` & `petram_base-2.1.38/petram/sol/nodal_refinement.py`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/sol/pointcloud_evaluator.py` & `petram_base-2.1.38/petram/sol/pointcloud_evaluator.py`

 * *Files 18% similar despite different names*

```diff
@@ -210,20 +210,43 @@
             if (n in g and isinstance(g[n], NativeCoefficientGenBase)):
                 g[n+"_coeff"] = CoefficientVariable(g[n], g)
                 new_names.append(n+"_coeff")
                 name_translation[n+"_coeff"] = n
 
             elif (n in g and isinstance(g[n], NumbaCoefficientVariable)):
                 ind_vars = [xx.strip() for xx in phys.ind_vars.split(',')]
+                if g[n].has_dependency():
+                    g[n].forget_jitted_coefficient()
                 g[n].set_coeff(ind_vars, g)
                 new_names.append(n)
                 name_translation[n] = n
 
             elif (n in g and isinstance(g[n], Variable)):
-                new_names.extend(g[n].dependency)
+                for x in g[n].dependency:
+                    new_names.append(x)
+                    name_translation[x] = x
+
+                for x in g[n].grad:
+                    new_names.append('grad'+x)
+                    name_translation['grad'+x] = 'grad'+x
+                    if 'grad'+x not in g:
+                        g['grad'+x] = g[x].generate_grad_variable()
+
+                for x in g[n].curl:
+                    new_names.append('curl'+x)
+                    name_translation['curl'+x] = 'curl'+x
+                    if 'curl'+x not in g:
+                        g['curl'+x] = g[x].generate_curl_variable()
+
+                for x in g[n].div:
+                    new_names.append('div'+x)
+                    name_translation['div'+x] = 'div'+x
+                    if 'div'+x not in g:
+                        g['div'+x] = g[x].generate_div_variable()
+
                 new_names.append(n)
                 name_translation[n] = n
 
             elif n in g:
                 new_names.append(n)
                 name_translation[n] = n
```

### Comparing `PetraM_Base-2.1.30/petram/sol/probe.py` & `petram_base-2.1.38/petram/sol/probe.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,21 +96,24 @@
         self.name = name
         self.xnames = ['time'] if xnames is None else xnames
         self.sig = []
         self.t = []
         self.idx = idx
         self.finalized = False
 
-    def write_file(self, filename=None, format=1):
+    def write_file(self, filename=None, format=1, nosmyid=False):
         valid = self.finalize()
         if not valid:
             return
 
         if filename is None:
-            filename = 'probe_'+self.name + smyid
+            if nosmyid:
+                filename = 'probe_'+self.name
+            else:
+                filename = 'probe_'+self.name + smyid
 
         fid = open(filename, 'w')
 
         if format == 0:
             fid.write("format : 0\n")
         else:
             fid.write("format : 1\n")
```

### Comparing `PetraM_Base-2.1.30/petram/sol/probe_evaluator.py` & `petram_base-2.1.38/petram/sol/probe_evaluator.py`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/sol/slice_evaluator.py` & `petram_base-2.1.38/petram/sol/slice_evaluator.py`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/sol/solsets.py` & `petram_base-2.1.38/petram/sol/solsets.py`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/sol/test.py` & `petram_base-2.1.38/petram/sol/test.py`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/solver/ams_model.py` & `petram_base-2.1.38/petram/solver/ams_model.py`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/solver/block_smoother.py` & `petram_base-2.1.38/petram/solver/block_smoother.py`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/solver/distance_solver.py` & `petram_base-2.1.38/petram/solver/distance_solver.py`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/solver/gmres_model.py` & `petram_base-2.1.38/petram/solver/gmres_model.py`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/solver/iterative_model.py` & `petram_base-2.1.38/petram/solver/iterative_model.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     myid = MPI.COMM_WORLD.rank
     smyid = '{:0>6d}'.format(myid)
     from mfem.common.mpi_debug import nicePrint
 
 else:
     import mfem.ser as mfem
     default_kind = 'scipy'
+    num_proc = 1
 
 SparseSmootherCls = {"Jacobi": (mfem.DSmoother, 0),
                      "l1Jacobi": (mfem.DSmoother, 1),
                      "lumpedJacobi": (mfem.DSmoother, 2),
                      "GS": (mfem.GSSmoother, 0),
                      "forwardGS": (mfem.GSSmoother, 1),
                      "backwardGS": (mfem.GSSmoother, 2),
@@ -106,15 +107,16 @@
                                                    {'elp': [smp1, ]}], ],
                 [None, self.write_mat, 3, {"text": "write matrix"}],
                 [None, self.assert_no_convergence, 3,
                     {"text": "check converegence"}],
                 [None, self.use_ls_reducer, 3, {
                     "text": "Reduce linear system when possible"}],
                 [None, (self.merge_real_imag, (self.use_block_symmetric,)),
-                 27, ({"text": "Use ComplexOperator"}, {"elp": mm},)], ]
+                 27, ({"text": "Use ComplexOperator"}, {"elp": mm},)],
+                ["use dist, SOL (dev.)", self.use_dist_sol, 3, {"text": ""}], ]
 
     def get_panel1_value(self):
         # this will set _mat_weight
         from petram.solver.solver_model import SolveStep
         p = self.parent
         while not isinstance(p, SolveStep):
             p = p.parent
@@ -147,15 +149,16 @@
                    single1in, single1in, mumpsin], ]
         value = ([self.solver_type, single1, single2, single2,
                   single1, single1, single1,
                   nested],
                  (self.adv_mode, [self.adv_prc, ], [self.preconditioners, ]),
                  self.write_mat, self.assert_no_convergence,
                  self.use_ls_reducer,
-                 (self.merge_real_imag, [self.use_block_symmetric, ]),)
+                 (self.merge_real_imag, [self.use_block_symmetric, ]),
+                 self.use_dist_sol)
 
         return value
 
     def import_panel1_value(self, v):
         self.solver_type = str(v[0][0])
         idx = choices_a.index(self.solver_type)
         vv = v[0][idx + 1]
@@ -183,14 +186,15 @@
         self.write_mat = bool(v[2])
         self.assert_no_convergence = bool(v[3])
         self.use_ls_reducer = bool(v[4])
         self.adv_mode = v[1][0]
         self.adv_prc = v[1][1][0]
         self.merge_real_imag = bool(v[5][0])
         self.use_block_symmetric = bool(v[5][1][0])
+        self.use_dist_sol = bool(v[6])
 
     def attribute_set(self, v):
         v = super(Iterative, self).attribute_set(v)
         v['solver_type'] = 'GMRES'
         v['log_level'] = 0
         v['maxiter'] = 200
         v['reltol'] = 1e-7
@@ -255,23 +259,24 @@
             return self.real_to_complex_interleaved(solall, M)
 
     def real_to_complex_interleaved(self, solall, M):
         if use_parallel:
             from mpi4py import MPI
             myid = MPI.COMM_WORLD.rank
 
-            offset = M.RowOffsets().ToList()
-            of = [np.sum(MPI.COMM_WORLD.allgather(np.int32(o)))
-                  for o in offset]
-            if myid != 0:
-                return
+            of = M.RowOffsets().ToList()
+
+            if not self.use_dist_sol:
+                of = [np.sum(MPI.COMM_WORLD.allgather(np.int32(o)))
+                      for o in of]
+                if myid != 0:
+                    return
 
         else:
-            offset = M.RowOffsets()
-            of = offset.ToList()
+            of = M.RowOffsets().ToList()
 
         rows = M.NumRowBlocks()
         s = solall.shape
         nb = rows // 2
         i = 0
         pt = 0
         result = np.zeros((s[0] // 2, s[1]), dtype='complex')
@@ -285,23 +290,23 @@
         return result
 
     def real_to_complex_merged(self, solall, M):
         if use_parallel:
             from mpi4py import MPI
             myid = MPI.COMM_WORLD.rank
 
-            offset = M.RowOffsets().ToList()
-            of = [np.sum(MPI.COMM_WORLD.allgather(np.int32(o)))
-                  for o in offset]
-            if myid != 0:
-                return
-
+            of = M.RowOffsets().ToList()
+            if not self.use_dist_sol:
+                of = [np.sum(MPI.COMM_WORLD.allgather(np.int32(o)))
+                      for o in of]
+                if myid != 0:
+                    return
         else:
-            offset = M.RowOffsets()
-            of = offset.ToList()
+            of = M.RowOffsets().ToList()
+
         dprint1(of)
         rows = M.NumRowBlocks()
         s = solall.shape
         i = 0
         pt = 0
         result = np.zeros((s[0] // 2, s[1]), dtype='complex')
         for i in range(rows):
@@ -527,14 +532,18 @@
             self. write_mat(A, b, x, "." + smyid)
 
         sol = []
 
         # solve the problem and gather solution to head node...
         # may not be the best approach
 
+        distributed_sol = (use_parallel and
+                           num_proc > 1 and
+                           self.gui.use_dist_sol)
+
         from petram.helper.mpi_recipes import gather_vector
         offset = A.RowOffsets()
         for bb in b:
             rows = MPI.COMM_WORLD.allgather(np.int32(bb.Size()))
             #rowstarts = np.hstack((0, np.cumsum(rows)))
             dprint1("row offset", offset.ToList())
             if x is None:
@@ -550,36 +559,42 @@
                     self.gui.set_solve_error(
                         (True, "No Convergence: " + self.gui.name()))
                     assert False, "No convergence"
             else:
                 self.call_mult(self.solver, bb, xx)
 
             s = []
-            for i in range(offset.Size() - 1):
-                v = xx.GetBlock(i).GetDataArray()
-                if self.gui.merge_real_imag:
-                    w = int(len(v) // 2)
-                    vv1 = gather_vector(v[:w])
-                    vv2 = gather_vector(v[w:])
-                    vv = np.hstack((vv1, vv2))
-                else:
-                    vv = gather_vector(v)
-                if myid == 0:
+            if distributed_sol:
+                for i in range(offset.Size() - 1):
+                    vv = xx.GetBlock(i).GetDataArray()
                     s.append(vv)
-                else:
-                    pass
-            if myid == 0:
                 sol.append(np.hstack(s))
+            else:
+                for i in range(offset.Size() - 1):
+                    v = xx.GetBlock(i).GetDataArray()
+                    if self.gui.merge_real_imag:
+                        w = int(len(v) // 2)
+                        vv1 = gather_vector(v[:w])
+                        vv2 = gather_vector(v[w:])
+                        vv = np.hstack((vv1, vv2))
+                    else:
+                        vv = gather_vector(v)
+                    if myid == 0:
+                        s.append(vv)
+                    else:
+                        pass
+                if myid == 0:
+                    sol.append(np.hstack(s))
 
-        if myid == 0:
-            sol = np.transpose(np.vstack(sol))
-            return sol
-        else:
+        if myid != 0 and not distributed_sol:
             return None
 
+        sol = np.transpose(np.vstack(sol))
+        return sol
+
     def solve_serial(self, A, b, x=None):
         if self.gui.write_mat:
             self. write_mat(A, b, x)
 
         #M = self.M
         solver = self.solver
 
@@ -596,78 +611,7 @@
                 #   print x.GetBlock(j).GetDataArray()
                 #assert False, "must implement this"
             self.call_mult(solver, bb, xx)
 
             sol.append(xx.GetDataArray().copy())
         sol = np.transpose(np.vstack(sol))
         return sol
-
-        '''
-        prcs = dict(self.gui.preconditioners)
-        name = self.Aname
-        assert not self.gui.parent.is_complex(), "can not solve complex"
-        if self.gui.parent.is_converted_from_complex():
-           name = sum([[n, n] for n in name], [])
-
-
-        for k, n in enumerate(name):
-
-           prc = prcs[n][0]
-           if prc == "None": continue
-           name = "".join([tmp for tmp in prc if not tmp.isdigit()])
-           A0 = get_block(A, k, k)
-           cls = SparseSmootherCls[name][0]
-           arg = SparseSmootherCls[name][1]
-           if name == 'MUMPS':
-               invA0 = cls(A0, gui=self.gui[prc], engine=self.engine)
-
-           elif name.startswith('schur'):
-               args = name.split("(")[-1].split(")")[0].split(",")
-               dprint1("setting up schur for ", args)
-               if len(args) > 1:
-                   assert False, "not yet supported"
-               for arg in args:
-                    r1 = self.engine.dep_var_offset(arg.strip())
-                    c1 = self.engine.r_dep_var_offset(arg.strip())
-                    B  =  get_block(A, k, c1)
-                    Bt =  get_block(A, r1, k)
-                    B0 = get_block(A, r1, c1)
-                    Md = mfem.Vector(M0.Height())
-                    B0.GetDiag(Md)
-                    for i in range(Md.Size()):
-                        if Md[i] != 0.:
-                            Bt.ScaleRow(i, 1/Md[i])
-                        else:
-                            assert False, "diagnal element of matrix is zero"
-
-                    S = mfem.Mult(B, Bt)
-                    invA0 = mfem.DSmoother(S)
-                    invA0.iterative_mode = False
-
-           else:
-               invA0 = cls(A0, arg)
-           invA0.iterative_mode = False
-           M.SetDiagonalBlock(k, invA0)
-        '''
-        '''
-        We should support Shur complement type preconditioner
-        if offset.Size() > 2:
-            B =  get_block(A, 1, 0)
-            MinvBt = get_block(A, 0, 1)
-            Md = mfem.Vector(get_block(A, 0, 0).Height())
-            get_block(A, 0, 0).GetDiag(Md)
-            for i in range(Md.Size()):
-                if Md[i] != 0.:
-                    MinvBt.ScaleRow(i, 1/Md[i])
-                else:
-                    assert False, "diagnal element of matrix is zero"
-            S = mfem.Mult(B, MinvBt)
-            S.iterative_mode = False
-            SS = mfem.DSmoother(S)
-            SS.iterative_mode = False
-            M.SetDiagonalBlock(1, SS)
-        '''
-
-        '''
-        int GMRES(const Operator &A, Vector &x, const Vector &b, Solver &M,
-          int &max_iter, int m, double &tol, double atol, int printit)
-        '''
```

### Comparing `PetraM_Base-2.1.30/petram/solver/krylov.py` & `petram_base-2.1.38/petram/solver/krylov.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 '''
 from petram.solver.mumps_model import MUMPSPreconditioner
 from petram.mfem_config import use_parallel
 import numpy as np
 
 from petram.debug import flush_stdout
 from petram.namespace_mixin import NS_mixin
-from .solver_model import LinearSolverModel, LinearSolver
+from petram.solver.solver_model import LinearSolverModel, LinearSolver
 
 import petram.debug as debug
 dprint1, dprint2, dprint3 = debug.init_dprints('KrylovModel')
 
 if use_parallel:
     from petram.helper.mpi_recipes import *
     from mfem.common.parcsr_extra import *
@@ -203,15 +203,14 @@
         return result
 
     def prepare_preconditioner(self, opr, engine):
         for x in self.iter_enabled():
             if isinstance(x, LinearSolverModel):
                 return x.prepare_solver(opr, engine)
 
-
     def do_prepare_solver(self, opr, engine):
         cls = getattr(mfem, self.solver_type + 'Solver')
         args = (MPI.COMM_WORLD,) if use_parallel else ()
 
         solver = cls(*args)
         solver.SetAbsTol(self.abstol)
         solver.SetRelTol(self.reltol)
@@ -229,48 +228,16 @@
 
         if M is not None:
             solver.SetPreconditioner(M)
             solver._prc = M
         return solver
 
     def write_matrix(self, A=None, b=None, x=None, suffix=smyid):
-        def get_block(Op, i, j):
-            try:
-                return Op._linked_op[(i, j)]
-            except KeyError:
-                return None
-
-        offset = A.RowOffsets()
-        rows = A.NumRowBlocks()
-        cols = A.NumColBlocks()
-        if suffix != '':
-            suffix = '.'+suffix
-
-        if A is not None:
-            for i in range(cols):
-                for j in range(rows):
-                    m = get_block(A, i, j)
-                    if m is None:
-                        continue
-                    if isinstance(m, mfem.ComplexOperator):
-                        m1 = m._real_operator
-                        m2 = m._imag_operator
-                        m1.Print('matrix_Re_' + str(i) + '_' + str(j))
-                        m2.Print('matrix_Im_' + str(i) + '_' + str(j))
-                    else:
-                        m.Print('matrix_' + str(i) + '_' + str(j))
-        if b is not None:
-            for i, bb in enumerate(b):
-                for j in range(rows):
-                    v = bb.GetBlock(j)
-                    v.Print('rhs_' + str(i) + '_' + str(j) + suffix)
-        if x is not None:
-            for j in range(rows):
-                xx = x.GetBlock(j)
-                xx.Print('x_' + str(i) + '_' + str(j) + suffix)
+        from petram.solver.solver_utils import write_blockoperator
+        write_blockoperator(A=A, b=b, x=x, suffix=suffix)
 
     def prepare_solver(self, opr, engine):
         solver = self.do_prepare_solver(opr, engine)
         solver.iterative_mode = True
 
         return solver
```

### Comparing `PetraM_Base-2.1.30/petram/solver/linearsystem_reducer.py` & `petram_base-2.1.38/petram/solver/linearsystem_reducer.py`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/solver/mg_solver_model.py` & `petram_base-2.1.38/petram/solver/mg_solver_model.py`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/solver/ml_solver_model.py` & `petram_base-2.1.38/petram/solver/ml_solver_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from petram.solver.strumpack_model import Strumpack
+from petram.solver.strumpack_model import StrumpackMFEMSolverModel
 from petram.solver.mumps_model import MUMPSMFEMSolverModel
 from petram.solver.krylov import KrylovModel, StationaryRefinementModel
 import os
 import warnings
 
 import numpy as np
 
@@ -268,15 +268,15 @@
     def fancy_tree_name(self):
         return 'Direct'
 
     def get_info_str(self):
         return 'MUMPS:Lv0'
 
 
-class CoarseStrumpack(Strumpack, CoarsestLvlSolver):
+class CoarseStrumpack(StrumpackMFEMSolverModel, CoarsestLvlSolver):
     @classmethod
     def fancy_menu_name(self):
         return 'STRUMPACK'
 
     @classmethod
     def fancy_tree_name(self):
         return 'Direct'
@@ -338,15 +338,15 @@
 class MultiLvlStationarySolver(StdSolver):
     @classmethod
     def fancy_menu_name(self):
         return 'Stationary(MultiLevel)'
 
     @classmethod
     def fancy_tree_name(self):
-        return 'Stationary'
+        return 'MLStationary'
 
     def attribute_set(self, v):
         super(MultiLvlSolver, self).attribute_set(v)
         v['merge_real_imag'] = True
         v['use_block_symmetric'] = False
         v["presmoother_count"] = "1"
         v["postsmoother_count"] = "1"
```

### Comparing `PetraM_Base-2.1.30/petram/solver/mumps_model.py` & `petram_base-2.1.38/petram/solver/mumps_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,15 @@
                 ["static pivot thr. (CNTL4)", self.cntl4, 0, {}],
                 ["Itr. refinement (ICNTL10)", self.icntl10, 0, {}],
                 ["refinement stop Cond. (CNTL2)", self.cntl2, 0, {}],
                 ["permutation/scaling Opt.(ICNTL6)", self.icntl6, 0, {}],
                 ["scaling strategy (ICNTL8)", self.icntl8, 0, {}],
                 ["write inverse", self.write_inv, 3, {"text": ""}],
                 ["use float32", self.use_single_precision, 3, {"text": ""}],
-                ["use dist, RHS (only for MLsolver)",
+                ["use dist, RHS (dev.)",
                  self.use_dist_rhs, 3, {"text": ""}],
                 ["use dist, SOL (dev.)", self.use_dist_sol, 3, {"text": ""}], ]
 
     def get_panel1_value(self):
         return (int(self.log_level), self.ordering, self.out_of_core,
                 self.error_ana, self.write_mat, self.write_fac,
                 self.restore_fac, self.factor_path,
@@ -127,15 +127,14 @@
         v['icntl10'] = 'default'
         v['cntl2'] = 'default'
         v['icntl6'] = 'default'
         v['icntl8'] = 'default'
         v['use_single_precision'] = False
         v['write_inv'] = False
         v['use_dist_rhs'] = False
-        v['use_dist_sol'] = True
 
         # make sure that old data type (data was stored as int) is converted to
         # string
         if hasattr(self, "icntl14"):
             self.icntl14 = str(self.icntl14)
         if hasattr(self, "icntl23"):
             self.icntl23 = str(self.icntl23)
@@ -166,15 +165,15 @@
         try:
             from mpi4py import MPI
         except BaseException:
             from petram.helper.dummy_mpi import MPI
         myid = MPI.COMM_WORLD.rank
         nproc = MPI.COMM_WORLD.size
 
-        if myid == 0:
+        if solall is not None:
             s = solall.shape[0]
             solall = solall[:s // 2, :] + 1j * solall[s // 2:, :]
             return solall
 
     def __del__(self):
         if self.s is not None:
             self.s.finish()
@@ -232,15 +231,16 @@
         return ["blk_interleave",
                 "blk_merged_s",
                 "blk_merged", ]
 
     def prepare_solver(self, opr, engine):
         solver = MUMPSBlockPreconditioner(opr,
                                           gui=self,
-                                          engine=engine,)
+                                          engine=engine,
+                                          silent=True)
         solver.SetOperator(opr)
         return solver
 
 
 class MUMPSPreconditionerModel(MUMPSBase):
     '''
     This one is to use MUMPS in iterative solver
@@ -261,15 +261,16 @@
         return ["blk_interleave",
                 "blk_merged_s",
                 "blk_merged", ]
 
     def prepare_solver(self, opr, engine):
         prc = MUMPSPreconditioner(opr,
                                   gui=self,
-                                  engine=engine)
+                                  engine=engine,
+                                  silent=True)
         return prc
 
 
 class MUMPSSolver(LinearSolver):
     is_iterative = False
 
     def __init__(self, *args, **kwargs):
@@ -399,15 +400,15 @@
 
         self.s = s
         self.is_complex = is_complex
         self.data_array = data_array
 
         gui = self.gui
         # No outputs
-        if gui.log_level == 0:
+        if gui.log_level <= 0:
             s.set_icntl(1, -1)
             s.set_icntl(2, -1)
             s.set_icntl(3, -1)
             s.set_icntl(4, 0)
         elif gui.log_level == 1:
             pass
         else:
@@ -902,21 +903,22 @@
         if self.gui.icntl10.lower() != 'default':       # iterative refinement
             s.set_icntl(10, convert2int(self.gui.icntl10))
 
         if self.gui.cntl2.lower() != 'default':
             # stopping criterion for iterative refinement
             s.set_cntl(2, convert2float(self.gui.cntl2))
 
-        if self.silent or self.gui.log_level >= 10:
+        if self.gui.log_level >= 10 or self.gui.log_level <= 0:
             s.set_icntl(1, -1)
             s.set_icntl(2, -1)
             s.set_icntl(3, -1)
             s.set_icntl(4, 0)
         else:
-            dprint1("job3", debug.format_memory_usage())
+            if not self.silent:
+                dprint1("job3", debug.format_memory_usage())
 
         if not distributed_rhs and not distributed_sol:
             self.set_error_analysis(s)
 
         s.set_job(3)
         s.run()
 
@@ -1095,105 +1097,59 @@
         if self.is_complex_operator:
             s = np.hstack((s.real.flatten(), s.imag.flatten()))
 
         #nicePrint(s.shape, y.Size())
         y.Assign(s.flatten().astype(float, copy=False))
 
 
-def check_block_operator(A):
-    from petram.solver.strumpack_model import get_block
-
-    rows = A.NumRowBlocks()
-    cols = A.NumColBlocks()
-
-    is_complex = False
-    is_parallel = False
-    for i in range(rows):
-        for j in range(cols):
-            m = get_block(A, i, j)
-            if m is None:
-                continue
-            if isinstance(m, mfem.ComplexOperator):
-                is_complex = True
-                check = m._real_operator
-            else:
-                check = m
-            if not isinstance(check, mfem.SparseMatrix):
-                is_parallel = True
-
-    return is_complex, is_parallel
-
-
 class MUMPSBlockPreconditioner(mfem.Solver):
     def __init__(self, opr, gui=None, engine=None, silent=False, **kwargs):
         self.gui = gui
         self.engine = engine
         self.silent = silent
         self.is_complex_operator = False
         if opr is not None:
             self._opr = weakref.ref(opr)
         else:
             self._opr = None
         self.irhs_loc = None
         super(MUMPSBlockPreconditioner, self).__init__()
 
     def real_to_complex(self, x):
-        '''
-        if use_parallel:
-           from mpi4py import MPI
-           myid     = MPI.COMM_WORLD.rank
-
-
-           offset = M.RowOffsets().ToList()
-           of = [np.sum(MPI.COMM_WORLD.allgather(np.int32(o))) for o in offset]
-           if myid != 0: return
-
-        else:
-            pass
-        '''
-
         rows = len(self.block_size)
         of = self.block_offset
         pt = 0
         x2 = np.zeros(of[-1] // 2, dtype=self.dtype)
 
         for i in range(rows):
             l = of[i + 1] - of[i]
             w = int(l // 2)
             x2[pt:pt + w] = x[of[i]:of[i] + w] + 1j * x[(of[i] + w):of[i + 1]]
             pt = pt + w
 
         return x2
 
     def complex_to_real(self, y):
-        '''
-        if use_parallel:
-           from mpi4py import MPI
-           myid     = MPI.COMM_WORLD.rank
-
-
-           offset = M.RowOffsets().ToList()
-           of = [np.sum(MPI.COMM_WORLD.allgather(np.int32(o))) for o in offset]
-           if myid != 0: return
-
-        else:
-            pass
-        '''
         rows = len(self.block_size)
         of = self.block_offset
         pt = 0
-        y2 = np.zeros(of[-1], dtype=np.float)
+
+        if self.gui.use_single_precision:
+            dtype = np.float32
+        else:
+            dtype = np.float64
+
+        y2 = np.zeros(of[-1], dtype=dtype)
         for i in range(rows):
             l = of[i + 1] - of[i]
             w = int(l // 2)
             y2[of[i]:(of[i] + w)] = y[pt:pt + w].real
             y2[(of[i] + w):(of[i] + w + w)] = y[pt:pt + w].imag
             pt = pt + w
 
-        #assert False, "test"
         return y2
 
     def Mult(self, x, y):
         if use_parallel:
             from petram.helper.mpi_recipes import (gather_vector,
                                                    scatter_vector,
                                                    allgather_vector)
@@ -1215,17 +1171,14 @@
             if self.gui.use_dist_rhs:
                 xx = np.atleast_2d(vec).transpose()
             else:
                 xx = gather_vector(vec)
                 if myid == 0:
                     xx = np.atleast_2d(xx).transpose()
 
-        # if myid == 0:
-        #    print("xx shape (at node-0)", xx.shape)
-
         s = [solver.Mult(xx) for solver in self.solver]
 
         if self.row_offset != -1:
             # if myid == 0:
             #w = [0.8*np.exp(1j*77/180*np.pi), np.exp(-1j*60/180*np.pi)*1.2]
             w = [1]*len(s)
             s = [xx.flatten()*w[i] for i, xx in enumerate(s)]
@@ -1258,15 +1211,15 @@
             smyid = '{:0>6d}'.format(myid)
 
         #opr = mfem.Opr2BlockOpr(opr)
         #self._opr = weakref.ref(opr)
 
         opr = self._opr()
         from petram.solver.strumpack_model import build_csr_local
-
+        from petram.solver.solver_utils import check_block_operator
         is_complex, is_parallel = check_block_operator(opr)
 
         if is_complex:
             if self.gui.use_single_precision:
                 dtype = np.complex64
             else:
                 dtype = np.complex128
@@ -1313,23 +1266,25 @@
         else:
             self.irhs_loc = None
 
         self.solver = []
 
         if not self.gui.restore_fac:
             solver = MUMPSSolver(self.gui, self.engine)
+            solver.set_silent(self.silent)
             solver.AllocSolver(self.is_complex_operator,
                                self.gui.use_single_precision)
             solver.SetOperator(gcoo, is_parallel)
             solver.keep_sol_distributed = True
             self.solver.append(solver)
         else:
             pathes = self.gui.factor_path.split(',')
             for i in range(len(pathes)):
                 solver = MUMPSSolver(self.gui, self.engine)
+                solver.set_silent(self.silent)
                 solver.AllocSolver(self.is_complex_operator,
                                    self.gui.use_single_precision)
                 solver.SetOperator(gcoo, is_parallel, ifactor=i)
                 solver.keep_sol_distributed = True
                 self.solver.append(solver)
 
         self.is_parallel = is_parallel
@@ -1353,15 +1308,14 @@
     root node.
     '''
     is_iterative = True
 
     def __init__(self, *args, **kwargs):
         super(MUMPSBlockSolver, self).__init__(*args, **kwargs)
         self.silent = False
-        self.keep_sol_distributed = False
 
     def SetOperator(self, A, dist, name=None, ifactor=0):
         solver = MUMPSBlockPreconditioner(A,
                                           gui=self.gui,
                                           engine=self.engine,)
         solver.SetOperator(A)
         self._solver = solver
@@ -1370,15 +1324,18 @@
         self._solver.Mult(b[0], x)
 
         if use_parallel:
             from mpi4py import MPI
             from petram.helper.mpi_recipes import (gather_vector,
                                                    allgather_vector)
             myid = MPI.COMM_WORLD.rank
-
-            xx = gather_vector(x.GetDataArray())
-            if myid == 0:
-                xx = np.atleast_2d(xx).transpose()
+            if self.gui.use_dist_sol:
+                xx = x.GetDataArray()
+            else:
+                xx = gather_vector(x.GetDataArray())
+            if xx is not None:
+               xx = np.atleast_2d(xx).transpose()
         else:
             xx = x.GetDataArray().copy().reshape(-1, 1)
 
         return xx
+
```

### Comparing `PetraM_Base-2.1.30/petram/solver/nl_solver_model.py` & `petram_base-2.1.38/petram/solver/nl_solver_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -364,14 +364,15 @@
 
         depvars = [x for i, x in enumerate(depvars) if mask[0][i]]
 
         if update_operator:
             opr = self.adjust_operator(A, M, mask)   # add Jacobian for Newtown
             AA = engine.finalize_matrix(opr, mask, not self.phys_real,
                                         format=self.ls_type)
+            self._AA = AA
 
         BB = engine.finalize_rhs([RHS], A, X[0], mask, not self.phys_real,
                                  format=self.ls_type,
                                  use_residual=True)
 
         if self.linearsolver is None:
             linearsolver = self.allocate_linearsolver(
@@ -404,16 +405,16 @@
 
         return solall
 
     def update_x(self, solall):
         A, X, RHS, Ae, B, M, depvars = self.blocks
         mask = self.blk_mask
 
-        A.reformat_central_mat(
-            solall, 0, X[0], mask, alpha=self._alpha, beta=self._beta)
+        self.reformat_mat(A, self._AA, solall, 0, X[0], mask,
+                          alpha=self._alpha, beta=self._beta)
         self.sol = X[0]
 
         # store probe signal (use t=0.0 in std_solver)
         for p in self.probe:
             p.append_sol(X[0])
 
         self._kiter = self._kiter + 1
@@ -756,24 +757,25 @@
                 self._converged = False
                 self._fixed_damping = True
 
         if self._done:
             if self._converged:
                 dprint1("converged ("+self.scheme_name + ") #iter=", self.kiter)
                 dprint1("final error |err| = ", err)
-                dprint1("damping parameters", self.damping_record)
 
             else:
                 dprint1("no convergence ("+self.scheme_name+" interation)")
                 dprint1("damping parameters", self.damping_record)
 
             if self.verbose:
-                dprint1("err history = ", self.error_record)
-                dprint1("err^2 history (decomposition) = ", self.debug_data)
-                dprint1("residuals", self.residual_record)
+                dprint1("damping parameters", self.damping_record, notrim=True)
+                dprint1("err history = ", self.error_record, notrim=True)
+                dprint1("err^2 history (decomposition) = ",
+                        self.debug_data, notrim=True)
+                dprint1("residuals", self.residual_record, notrim=True)
 
     def save_probe(self):
         from petram.mfem_config import use_parallel
         if use_parallel:
             from mpi4py import MPI
         else:
             from petram.helper.dummy_mpi import MPI
```

### Comparing `PetraM_Base-2.1.30/petram/solver/parametric.py` & `petram_base-2.1.38/petram/solver/parametric.py`

 * *Files 1% similar despite different names*

```diff
@@ -347,25 +347,26 @@
         params = scanner.list_data()
 
         od = os.getcwd()
 
         filenames, probenames = list_probes(dirs[0])
 
         names = scanner.names
+
         probes = [Probe(n, xnames=names) for n in probenames]
 
         for param, dirname in zip(params, dirs):
             os.chdir(dirname)
             for f, p in zip(filenames, probes):
                 xdata, ydata = load_probe(f)
                 p.append_value(ydata, param)
 
         os.chdir(od)
         for p in probes:
-            p.write_file()
+            p.write_file(nosmyid=True)
             # else:
             #    dprint1("skipping summarizing probe data for ", p.name)
 
     def set_scanner_physmodel(self, scanner):
         solvers = self.get_active_solvers()
         phys_models = []
         for s in solvers:
@@ -399,7 +400,8 @@
         else:
             is_new_mesh = self.check_and_run_geom_mesh_gens(engine)
             if is_first or is_new_mesh:
                 engine.preprocess_modeldata()
             self._run_rhs_assembly(engine, solvers, scanner, is_first=is_first)
 
         self.collect_probe_signals(self.case_dirs, scanner)
+        scanner.collect_probe_signals(engine, self.case_dirs)
```

### Comparing `PetraM_Base-2.1.30/petram/solver/parametric_scanner.py` & `petram_base-2.1.38/petram/solver/parametric_scanner.py`

 * *Files 8% similar despite different names*

```diff
@@ -70,29 +70,36 @@
 
     def len(self):
         return self.max
 
     def save_scanner_data(self, solver):
         solver_name = solver.fullpath()
         data = self.list_data()
-        dprint1("saving parameter", os.getcwd())
+        dprint1("saving parameter", os.getcwd(), notrim=True)
         try:
             from mpi4py import MPI
         except ImportError:
             from petram.helper.dummy_mpi import MPI
         myid = MPI.COMM_WORLD.rank
 
         if myid == 0:
             fid = open("parametric_data_"+solver_name, "wb")
             dd = {"name": solver_name, "data": data}
             pickle.dump(dd, fid)
             fid.close()
 
         MPI.COMM_WORLD.Barrier()
 
+    def collect_probe_signals(self, engine, dirs):
+        '''
+        scanner can implement its own probe collections
+        '''
+        raise NotImplementedError(
+            "subclass needs to be provide this method")
+
     def set_model(self, data):
         raise NotImplementedError(
             "set model for parametric scanner needs to be given in subclass")
 
     @property
     def names(self):
         '''
@@ -169,9 +176,17 @@
     @property
     def names(self):
         '''
         suposed to return parameternames
         '''
         return self._names
 
+    def collect_probe_data(self, engine, dirs):
+        pass
+
+    def collect_probe_signals(self, engine, dirs):
+        import warnings
+        warnings.warn(
+            "collect_probe_signals is not used for SimpleScanner", UserWarning)
+
 
 Scan = SimpleScanner
```

### Comparing `PetraM_Base-2.1.30/petram/solver/set_var.py` & `petram_base-2.1.38/petram/solver/set_var.py`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/solver/solinit_model.py` & `petram_base-2.1.38/petram/solver/solinit_model.py`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/solver/solve_loop.py` & `petram_base-2.1.38/petram/solver/solve_loop.py`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/solver/solver_controls.py` & `petram_base-2.1.38/petram/solver/solver_controls.py`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/solver/solver_model.py` & `petram_base-2.1.38/petram/solver/solver_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,26 @@
+from mfem.common.mpi_debug import nicePrint
 from abc import ABC, abstractmethod
 import numpy as np
 import warnings
 import os
 from petram.model import Model
 import petram.debug as debug
 dprint1, dprint2, dprint3 = debug.init_dprints('Solver')
 
+
 '''
 
     Solver configurations
 
 
     (GUI)
 
     SolveStep:   This level defines the block matrix assembled at one time
-    Solve:       Solver solves a problem (linear or non-lienar or time-dependent or parametric),
+    Solver:      Solver solves a problem (linear or non-lienar or time-dependent or parametric),
                  using blocks defined in SolveStep
 
     LinterSolverModel:
                  LinearSolver solves a linear system.
                  Preconditioner is a child LinearSolver of LinearSolver
 
 
@@ -127,67 +129,73 @@
 
     def get_possible_child(self):
         #from solver.solinit_model import SolInit
         from petram.solver.std_solver_model import StdSolver
         from petram.solver.nl_solver_model import NLSolver
         from petram.solver.mg_solver_model import MGSolver
         from petram.solver.ml_solver_model import MultiLvlStationarySolver
+        from petram.solver.egn_solver_model import EgnSolver        
         from petram.solver.solver_controls import DWCCall, ForLoop
         from petram.solver.timedomain_solver_model import TimeDomain
         from petram.solver.set_var import SetVar
         from petram.solver.distance_solver import DistanceSolver
 
         try:
             from petram.solver.std_meshadapt_solver_model import StdMeshAdaptSolver
             return [MultiLvlStationarySolver,
                     TimeDomain,
                     DistanceSolver,
                     StdSolver,
                     StdMeshAdaptSolver,
                     NLSolver,
+                    EgnSolver,
                     # MGSolver,
                     ForLoop,
                     DWCCall, SetVar]
         except:
             return [MultiLvlStationarySolver,
                     TimeDomain,
                     DistanceSolver,
                     # MGSolver,
                     StdSolver,
                     NLSolver,
+                    EgnSolver,                    
                     ForLoop,
                     DWCCall, SetVar]
 
     def get_possible_child_menu(self):
         #from solver.solinit_model import SolInit
         from petram.solver.std_solver_model import StdSolver
         from petram.solver.nl_solver_model import NLSolver
         from petram.solver.mg_solver_model import MGSolver
         from petram.solver.ml_solver_model import MultiLvlStationarySolver
+        from petram.solver.egn_solver_model import EgnSolver
         from petram.solver.solver_controls import DWCCall, InnerForLoop
         from petram.solver.timedomain_solver_model import TimeDomain
         from petram.solver.set_var import SetVar
         from petram.solver.distance_solver import DistanceSolver
 
         try:
             from petram.solver.std_meshadapt_solver_model import StdMeshAdaptSolver
             return [("", StdSolver),
                     ("", MultiLvlStationarySolver),
                     ("", NLSolver),
                     ("", TimeDomain),
+                    #("", EgnSolver),
                     ("extra", DistanceSolver),
                     ("", StdMeshAdaptSolver),
                     ("", InnerForLoop),
                     ("", DWCCall),
                     ("!", SetVar)]
         except:
             return [("", StdSolver),
                     ("", MultiLvlStationarySolver),
                     ("", NLSolver),
                     ("", TimeDomain),
+                    #("", EgnSolver),
                     ("extra", DistanceSolver),
                     ("", InnerForLoop),
                     ("", DWCCall),
                     ("!", SetVar)]
 
     @property
     def solve_error(self):
@@ -637,16 +645,15 @@
 
     def get_linearsystem_type_from_solvermodel(self):
         raise NotImplementedError(
             "bug should not need this method")
 
     @abstractmethod
     def get_matrix_weight(self, *args, **kwargs):
-        raise NotImplementedError(
-            "bug should not need this method")
+        ...
 
     @abstractmethod
     def run(self, engine, is_first=True):
         ...
 
 
 class SolverInstance(ABC):
@@ -797,26 +804,55 @@
                 is_complex, engine)
         else:
             linearsolver = solver_model.allocate_solver(
                 False, engine)
 
         return linearsolver
 
+    def assemble_rhs(self):
+        raise NotImplementedError(
+            "assmemble_rhs should be implemented in subclass")
+
+    @abstractmethod
+    def assemble(self, inplace=True, update=False):
+        ...
+
     @abstractmethod
     def solve(self):
         ...
 
     @abstractmethod
     def compute_rhs(self, M, B, X):
         ...
 
     @abstractmethod
     def compute_A(self, M, B, X, mask_M, mask_B):
         ...
 
+    def reformat_mat(self, A, AA, solall, ksol, ret, mask, alpha=1, beta=0):
+        from petram.mfem_config import use_parallel
+        if use_parallel:
+            from mpi4py import MPI
+            is_sol_central = any(MPI.COMM_WORLD.allgather(solall is None))
+
+        else:
+            is_sol_central = True
+
+        if is_sol_central:
+            if not self.phys_real and self.gui.assemble_real:
+                solall = self.linearsolver_model.real_to_complex(solall, AA)
+            A.reformat_central_mat(
+                solall, ksol, ret, mask, alpha=alpha, beta=beta)
+        else:
+            if not self.phys_real and self.gui.assemble_real:
+                solall = self.linearsolver_model.real_to_complex(solall, AA)
+                #assert False, "this operation is not permitted"
+            A.reformat_distributed_mat(
+                solall, ksol, ret, mask, alpha=alpha, beta=beta)
+
 
 class TimeDependentSolverInstance(SolverInstance):
     def __init__(self, gui, engine):
         self.st = 0.0
         self.et = 1.0
         self.checkpoint = [0, 0.5, 1.0]
         self._icheckpoint = 0
@@ -877,35 +913,51 @@
 
 class LinearSolverModel(SolverBase):
     '''
     Model tree object for a linear solver
     '''
     is_iterative = True
 
+    def attribute_set(self, v):
+        v = super(LinearSolverModel, self).attribute_set(v)
+        v['use_dist_sol'] = True
+        return v
+
     def get_phys(self):
         return self.parent.get_phys()
 
     def get_phys_range(self):
         return self.parent.get_phys_range()
 
+    def get_solver(self):
+        '''
+        return Solver
+        ex) used to find assemble_real from linearsolver
+        '''
+        p = self.parent
+        while p is not None:
+            if isinstance(p, Solver):
+                return p
+            p = p.parent
+
     def allocate_solver(self, is_complex=False, engine=None):
         '''
         this method create LinearSolverInstance
 
         LinearSolverInstance is intermediate obect to prepare LinearSolver
         '''
         raise NotImplementedError(
             "bug. this method sould not be called")
 
-    def prepare_solver(self):
+    def prepare_solver(self, opr, engine):
         '''
         this method create LinearSolver. This should return MFEM LinearOperator
         '''
         raise NotImplementedError(
-            "bug. this method sould not be called")
+            "bug. this method sould not implemented in subclass.")
 
     def prepare_solver_with_multtranspose(self):
         '''
         this method create LinearSolver. This should return MFEM LinearOperator
         '''
         raise NotImplementedError(
             "bug. this method sould not be called")
@@ -990,15 +1042,15 @@
         #      for o in offset]
         # if myid != 0:
         #    return
 
     else:
         offset = M.RowOffsets()
         of = offset.ToList()
-
+    nicePrint(of)
     rows = M.NumRowBlocks()
     s = solall.shape
     nb = rows // 2
     i = 0
     pt = 0
     result = np.zeros((s[0] // 2, s[1]), dtype='complex')
     for j in range(nb):
@@ -1023,14 +1075,15 @@
         # if myid != 0:
         #    return
 
     else:
         offset = M.RowOffsets()
         of = offset.ToList()
 
+    nicePrint(of)
     rows = M.NumRowBlocks()
     s = solall.shape
     i = 0
     pt = 0
 
     result = np.zeros((s[0] // 2, s[1]), dtype='complex')
     for i in range(rows):
```

### Comparing `PetraM_Base-2.1.30/petram/solver/std_meshadapt_solver_model.py` & `petram_base-2.1.38/petram/solver/std_meshadapt_solver_model.py`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/solver/std_solver_model.py` & `petram_base-2.1.38/petram/solver/std_solver_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -243,15 +243,15 @@
         engine.copy_block_mask(mask)
 
         depvars = [x for i, x in enumerate(depvars) if mask[0][i]]
 
         if update_operator:
             AA = engine.finalize_matrix(A, mask, not self.phys_real,
                                         format=self.ls_type)
-
+            self._AA = AA
         BB = engine.finalize_rhs([RHS], A, X[0], mask, not self.phys_real,
                                  format=self.ls_type)
 
         if self.linearsolver is None:
             linearsolver = self.allocate_linearsolver(
                 self.gui.is_complex(), self. engine)
             self.linearsolver = linearsolver
@@ -286,24 +286,28 @@
         ss = MPI.COMM_WORLD.gather(ss)
         if ss is not None:
             dprint1("solshape", ', '.join(ss))
 
         # linearsolver.SetOperator(AA, dist = engine.is_matrix_distributed)
         # solall = linearsolver.Mult(BB, case_base=0)
 
-        is_sol_central = any(MPI.COMM_WORLD.allgather(solall is None))
+        self.reformat_mat(A, self._AA, solall, 0, X[0], mask)
+        '''
+        is_sol_central = (True if not use_parallel else
+                          any(MPI.COMM_WORLD.allgather(solall is None)))
+
         if is_sol_central:
             if not self.phys_real and self.gui.assemble_real:
                 solall = self.linearsolver_model.real_to_complex(solall, AA)
             A.reformat_central_mat(solall, 0, X[0], mask)
         else:
             if not self.phys_real and self.gui.assemble_real:
                 assert False, "this operation is not permitted"
             A.reformat_distributed_mat(solall, 0, X[0], mask)
-
+        '''
         self.sol = X[0]
 
         # store probe signal (use t=0.0 in std_solver)
         for p in self.probe:
             p.append_sol(X[0])
 
         return True
```

### Comparing `PetraM_Base-2.1.30/petram/solver/std_solver_model_v2.py` & `petram_base-2.1.38/petram/solver/std_solver_model_v2.py`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/petram/solver/strumpack_model.py` & `petram_base-2.1.38/petram/solver/strumpack_model.py`

 * *Files 7% similar despite different names*

```diff
@@ -200,47 +200,48 @@
         v["separator_ordering_level"] = "1 (default)"
         v["hodlr_butterfly_levels"] = "100 (default)"
         v["compression_rel_tol"] = "1e-4 (default)"
         v["compression_abs_tol"] = "1e-8 (default)"
         v["lossy_precision"] = "16 (default)"
         v["extra_options"] = ""
         v["use_64_int"] = False
-        v['use_dist_sol'] = True
 
         return v
 
     def does_linearsolver_choose_linearsystem_type(self):
         return True
 
     def linear_system_type(self, assemble_real, phys_real):
         if phys_real:
             return 'blk_interleave'
         else:
             return 'blk_merged'
 
     def real_to_complex(self, solall, M):
-        if self.parent.assemble_real:
+        solver = self.get_solver()
+        if solver.assemble_real:
             return self.real_to_complex_merged(solall, M)
         else:
             assert False, "should not come here"
 
     def real_to_complex_merged(self, solall, M):
         if use_parallel:
             from mpi4py import MPI
             myid = MPI.COMM_WORLD.rank
 
-            offset = M.RowOffsets().ToList()
-            of = [np.sum(MPI.COMM_WORLD.allgather(np.int32(o)))
-                  for o in offset]
-            if myid != 0:
-                return
+            of = M.RowOffsets().ToList()
 
+            if not self.use_dist_sol:
+                of = [np.sum(MPI.COMM_WORLD.allgather(np.int32(o)))
+                      for o in of]
+                if myid != 0:
+                    return
         else:
-            offset = M.RowOffsets()
-            of = offset.ToList()
+            of = M.RowOffsets().ToList()
+
         dprint1(of)
         rows = M.NumRowBlocks()
         s = solall.shape
         i = 0
         pt = 0
         result = np.zeros((s[0] // 2, s[1]), dtype='complex')
         for i in range(rows):
@@ -253,21 +254,14 @@
 
     def allocate_solver(self, is_complex=False, engine=None):
         solver = StrumpackSolver(self, engine)
         solver.AllocSolver(is_complex, self.use_single_precision)
         return solver
 
 
-def get_block(Op, i, j):
-    try:
-        return Op._linked_op[(i, j)]
-    except KeyError:
-        return None
-
-
 def build_csr_local(A, dtype, is_complex):
     '''
     build CSR form of A as a single
     matrix
     '''
     # print("build_csr_local", dtype, is_complex)
     offset = np.array(A.RowOffsets().ToList(), dtype=int)
@@ -329,20 +323,21 @@
     newi = []
     newj = []
     newd = []
     nrows = np.sum(local_size)
     ncols = np.sum(global_size)
 
     from scipy.sparse import bmat
+    from petram.solver.solver_utils import get_operator_block
 
     elements = [None] * rows
     elements = [elements.copy() for x in range(cols)]
     for i in range(rows):
         for j in range(cols):
-            m = get_block(A, i, j)
+            m = get_operator_block(A, i, j)
             if m is None:
                 continue
             if use_parallel:
                 if isinstance(m, mfem.ComplexOperator):
                     if not is_complex:
                         mr, ilower = ToScipyCoo(m._real_operator)
                         mi, ilower = ToScipyCoo(m._imag_operator)
@@ -486,15 +481,15 @@
 
         if self.gui.separator_ordering_level.find('default') == -1:
             l = int(self.gui.separator_ordering_level.split('(')[0])
             opts.extend(["--sp_separator_ordering_level", str(l)])
 
         for x in self.gui.extra_options.split("\n"):
             opts.extend([x.strip()
-                        for x in x.split(" ") if len(x.strip()) > 0])
+                         for x in x.split(" ") if len(x.strip()) > 0])
 
         # opts.append("")
         return opts
 
     def AllocSolver(self, is_complex, use_single_precision):
         try:
             import STRUMPACK as ST
@@ -583,15 +578,16 @@
         row_offsets = self.row_offsets.ToList()
 
         MPI.COMM_WORLD.Barrier()
 
         dprint1("calling reorder", debug.format_memory_usage())
         ret = self.spss.reorder()
 
-        ret = np.sum(MPI.COMM_WORLD.allgather(int(ret != ST.STRUMPACK_SUCCESS)))
+        ret = np.sum(MPI.COMM_WORLD.allgather(
+            int(ret != ST.STRUMPACK_SUCCESS)))
         if ret > 0:
             assert False, "error during recordering (Strumpack)"
 
         MPI.COMM_WORLD.Barrier()
 
         dprint1("calling factor", debug.format_memory_usage())
         ret = self.spss.factor()
@@ -683,7 +679,56 @@
             return sol
         else:
             if myid == 0:
                 sol = np.transpose(np.vstack(sol))
                 return sol
             else:
                 return None
+
+
+class StrumpackMFEMSolverModel(Strumpack):
+    '''
+    This one is to use STRUMPACK in iterative solver
+    It creates MUMPSPreconditioner
+    '''
+
+    def prepare_solver(self, opr, engine):
+        solver = StrumpackBlockPreconditioner(opr,
+                                              gui=self,
+                                              engine=engine,
+                                              silent=True)
+        solver.SetOperator(opr)
+        return solver
+
+
+class StrumpackBlockPreconditioner(mfem.Solver):
+    def __init__(self, opr, gui=None, engine=None, silent=False, **kwargs):
+        self.gui = gui
+        self.engine = engine
+        self.silent = silent
+
+        self.is_complex_operator = False
+        self.is_parallel = False
+
+        self.solver = None
+        super(StrumpackBlockPreconditioner, self).__init__()
+
+    def Mult(self, x, y):
+        s = self.solver.Mult([x])
+        if self.is_complex_operator:
+            assert False, "StrumpackMFEM for Complex is not yet implemented"
+            #s = self.complex_to_real(s)
+
+        y.Assign(s.flatten().astype(float, copy=False))
+
+    def SetOperator(self, opr):
+        print('opr', opr)
+        from petram.solver.solver_utils import check_block_operator
+        is_complex, is_parallel = check_block_operator(opr)
+
+        solver = StrumpackSolver(self.gui, self.engine)
+        solver.AllocSolver(is_complex, self.gui.use_single_precision)
+        solver.SetOperator(opr, is_parallel)
+
+        self.is_complex_operator = is_complex
+        self.is_parallel = is_parallel
+        self.solver = solver
```

### Comparing `PetraM_Base-2.1.30/petram/solver/timedomain_solver_model.py` & `petram_base-2.1.38/petram/solver/timedomain_solver_model.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,145 +1,146 @@
 from __future__ import print_function
+from petram.solver.solver_model import TimeDependentSolverInstance
+from petram.solver.std_solver_model import StdSolver
 
 import os
 import numpy as np
 
 from petram.model import Model
 from .solver_model import Solver
 
 import petram.debug as debug
 dprint1, dprint2, dprint3 = debug.init_dprints("TimeDomainSolver")
 rprint = debug.regular_print('TimeDependentSolver')
 
 
-from petram.solver.std_solver_model import StdSolver
 class DerivedValue(StdSolver):
     def allocate_instance(self, engine):
-        from petram.solver.std_solver_model import StandardSolver        
+        from petram.solver.std_solver_model import StandardSolver
         instance = StandardSolver(self, engine)
-        instance.set_blk_mask()        
+        instance.set_blk_mask()
         return instance
-    
+
+
 class TimeStep():
     def __init__(self, data):
         self.data = list(np.atleast_1d(data))
-        
+
     def __call__(self, i):
         if i >= len(self.data):
             return self.data[-1]
         else:
-            return self.data[i]        
-    
+            return self.data[i]
+
+
 class TimeDomain(Solver):
     can_delete = True
     has_2nd_panel = False
 
     def attribute_set(self, v):
         v['st_et_nt'] = [0, 1, 5]
         v['time_step'] = 0.01
         v['time_step_cnk'] = 0.01
-        v['time_step_fe'] = 0.01                
+        v['time_step_fe'] = 0.01
         v['ts_method'] = "Backward Euler"
-        v['abe_minstep']= 0.01
-        v['abe_maxstep']= 1.0
-        v['use_dwc_cp']   = False   # check point
-        v['dwc_cp_name']   = ''              
-        v['dwc_cp_arg']   = ''      
-        v['use_dwc_ts']   = False   # every time step
-        v['dwc_ts_name']   = ''                      
-        v['dwc_ts_arg']   = ''      
-        
+        v['abe_minstep'] = 0.01
+        v['abe_maxstep'] = 1.0
+        v['use_dwc_cp'] = False   # check point
+        v['dwc_cp_name'] = ''
+        v['dwc_cp_arg'] = ''
+        v['use_dwc_ts'] = False   # every time step
+        v['dwc_ts_name'] = ''
+        v['dwc_ts_arg'] = ''
+
         super(TimeDomain, self).attribute_set(v)
         return v
-    
+
     def panel1_param(self):
-        elp_be =  [["dt", "", 0, {}],]
-        elp_abe =  [["min. dt", "", 0, {}],
-                    ["max. dt", "", 0, {}],]
+        elp_be = [["dt", "", 0, {}], ]
+        elp_abe = [["min. dt", "", 0, {}],
+                   ["max. dt", "", 0, {}], ]
         ret_cp = [["dwc",   self.dwc_cp_name,   0, {}],
-                  ["args.",   self.dwc_cp_arg,   0, {}],]
+                  ["args.",   self.dwc_cp_arg,   0, {}], ]
         value_cp = [self.dwc_cp_name, self.dwc_cp_arg]
         ret_ts = [["dwc",   self.dwc_ts_name,   0, {}],
-                  ["args.",   self.dwc_ts_arg,   0, {}],]
+                  ["args.",   self.dwc_ts_arg,   0, {}], ]
         value_ts = [self.dwc_ts_name, self.dwc_ts_arg]
-        
-        return [#["Initial value setting",   self.init_setting,  0, {},],
-                ["physics model",   self.phys_model,  0, {},],
-                ["start/end/#step",  "",  0, {},],
-                ["probes",   self.probe,  0, {},],                                
-                [None, None, 34, ({'text':'method','choices': ["Backward Euler",
-                                                               "CrankNicolson",
-                                                               "Forward Euler",
-                                                               "Adaptive BE"], 'call_fit':False},
-                                  {'elp':elp_be},
-                                  {'elp':elp_be},
-                                  {'elp':elp_be},                                                                    
-                                  {'elp':elp_abe},)],
-                [None, [False, value_cp], 27, [{'text':'Use DWC (check point)'},
-                                              {'elp': ret_cp}]],
-                [None, [False, value_ts], 27, [{'text':'Use DWC (time stepping)'},
-                                              {'elp': ret_ts}]],
-                [None,
-                 self.clear_wdir,  3, {"text":"clear working directory"}],
-                [None,
-                 self.init_only,  3, {"text":"initialize solution only"}], 
-                [None,
-                 self.assemble_real,  3, {"text":"convert to real matrix (complex prob.)"}],
-                [None,
-                 self.save_parmesh,  3, {"text":"save parallel mesh"}],
-                [None,
-                 self.use_profiler,  3, {"text":"use profiler"}],]
+
+        return [  # ["Initial value setting",   self.init_setting,  0, {},],
+            ["physics model",   self.phys_model,  0, {}, ],
+            ["start/end/#step",  "",  0, {}, ],
+            ["probes",   self.probe,  0, {}, ],
+            [None, None, 34, ({'text': 'method', 'choices': ["Backward Euler",
+                                                             "CrankNicolson",
+                                                             "Forward Euler",
+                                                             "Adaptive BE"], 'call_fit':False},
+                              {'elp': elp_be},
+                              {'elp': elp_be},
+                              {'elp': elp_be},
+                              {'elp': elp_abe},)],
+            [None, [False, value_cp], 27, [{'text': 'Use DWC (check point)'},
+                                           {'elp': ret_cp}]],
+            [None, [False, value_ts], 27, [{'text': 'Use DWC (time stepping)'},
+                                           {'elp': ret_ts}]],
+            [None,
+             self.clear_wdir,  3, {"text": "clear working directory"}],
+            [None,
+             self.init_only,  3, {"text": "initialize solution only"}],
+            [None,
+             self.assemble_real,  3, {"text": "convert to real matrix (complex prob.)"}],
+            [None,
+             self.save_parmesh,  3, {"text": "save parallel mesh"}],
+            [None,
+             self.use_profiler,  3, {"text": "use profiler"}], ]
 
     def get_panel1_value(self):
         st_et_nt = ", ".join([str(x) for x in self.st_et_nt])
-        return (#self.init_setting,
-                self.phys_model,
-                st_et_nt,
-                self.probe,                                
-                [self.ts_method,
-                 [str(self.time_step),],
-                 [str(self.time_step_cnk),],
-                 [str(self.time_step_fe),],                                  
-                 [str(self.abe_minstep), str(self.abe_maxstep),],
-                ],
-                [self.use_dwc_cp, [self.dwc_cp_name, self.dwc_cp_arg,]],
-                [self.use_dwc_ts, [self.dwc_ts_name, self.dwc_ts_arg,]],            
-                self.clear_wdir,
-                self.init_only,               
-                self.assemble_real,
-                self.save_parmesh,
-                self.use_profiler,)
+        return (  # self.init_setting,
+            self.phys_model,
+            st_et_nt,
+            self.probe,
+            [self.ts_method,
+             [str(self.time_step), ],
+             [str(self.time_step_cnk), ],
+             [str(self.time_step_fe), ],
+             [str(self.abe_minstep), str(self.abe_maxstep), ],
+             ],
+            [self.use_dwc_cp, [self.dwc_cp_name, self.dwc_cp_arg, ]],
+            [self.use_dwc_ts, [self.dwc_ts_name, self.dwc_ts_arg, ]],
+            self.clear_wdir,
+            self.init_only,
+            self.assemble_real,
+            self.save_parmesh,
+            self.use_profiler,)
 
-    
     def import_panel1_value(self, v):
-        #self.init_setting = str(v[0])        
+        #self.init_setting = str(v[0])
         self.phys_model = str(v[0])
         tmp = str(v[1]).split(',')
         st_et_nt = [tmp[0], tmp[1], ",".join(tmp[2:])]
         self.st_et_nt = [eval(x) for x in st_et_nt]
         self.probe = str(v[2])
         self.clear_wdir = v[6]
-        self.init_only = v[7]        
+        self.init_only = v[7]
         self.assemble_real = v[8]
         self.save_parmesh = v[9]
         self.use_profiler = v[10]
-        
+
         self.ts_method = str(v[3][0])
         self.time_step = str(v[3][1][0])
         self.time_step_cnk = str(v[3][2][0])
-        self.time_step_fe = str(v[3][3][0])                
-        self.abe_minstep  = float(v[3][4][0])
-        self.abe_maxstep  = float(v[3][4][1])
-        self.use_dwc_cp   = v[4][0]
-        self.dwc_cp_name  = v[4][1][0]                           
-        self.dwc_cp_arg   = v[4][1][1]         
-        self.use_dwc_ts   = v[5][0]
-        self.dwc_ts_name  = v[5][1][0]
-        self.dwc_ts_arg   = v[5][1][1]                           
-        
+        self.time_step_fe = str(v[3][3][0])
+        self.abe_minstep = float(v[3][4][0])
+        self.abe_maxstep = float(v[3][4][1])
+        self.use_dwc_cp = v[4][0]
+        self.dwc_cp_name = v[4][1][0]
+        self.dwc_cp_arg = v[4][1][1]
+        self.use_dwc_ts = v[5][0]
+        self.dwc_ts_name = v[5][1][0]
+        self.dwc_ts_arg = v[5][1][1]
 
     def get_possible_child(self):
         choice = []
         try:
             from petram.solver.mumps_model import MUMPS
             choice.append(MUMPS)
         except ImportError:
@@ -154,332 +155,346 @@
         try:
             from petram.solver.strumpack_model import SpSparse
             choice.append(SpSparse)
         except ImportError:
             pass
         choice.append(DerivedValue)
         return choice
-    
+
     def get_matrix_weight(self, timestep_config):
-        #timestep_weight):
+        # timestep_weight):
         #dt = float(self.time_step)
         #lns = self.root()['General']._global_ns.copy()
         #lns['dt'] = dt
         wt = [1 if x else 0 for x in timestep_config]
         return wt
 
     def get_child_solver(self):
         return self.derived_value_solver()
-    
+
     def derived_value_solver(self):
         return [self[key] for key in self
-                if isinstance(self[key],DerivedValue) and self[key].enabled]
-    
+                if isinstance(self[key], DerivedValue) and self[key].enabled]
+
     @debug.use_profiler
     def run(self, engine, is_first=True):
         if self.clear_wdir:
             engine.remove_solfiles()
 
-        fid = engine.open_file('checkpoint.'+self.parent.name()+'_'+self.name()+'.txt', 'w')
+        fid = engine.open_file(
+            'checkpoint.'+self.parent.name()+'_'+self.name()+'.txt', 'w')
         st, et, nt = self.st_et_nt
-        
+
         if self.ts_method == 'Backward Euler' or self.ts_method == 'Backward Eular':
             instance = FirstOrderBackwardEuler(self, engine)
             time_step = self.eval_text_in_global(self.time_step)
-            dprint1("time step configuration: " + str(self.time_step) + ':' +  str(time_step))            
+            dprint1("time step configuration: " +
+                    str(self.time_step) + ':' + str(time_step))
             instance.set_timestep(TimeStep(time_step))
-            
+
         elif self.ts_method == "CrankNicolson":
             instance = CrankNicolson(self, engine)
             time_step = self.eval_text_in_global(self.time_step_cnk)
-            dprint1("time step configuration: " + str(self.time_step_cnk) + ':' +  str(time_step))            
+            dprint1("time step configuration: " +
+                    str(self.time_step_cnk) + ':' + str(time_step))
             instance.set_timestep(TimeStep(time_step))
-            
+
         elif self.ts_method == "Forward Euler":
-            instance = FirstOrderForwardEuler(self, engine)            
+            instance = FirstOrderForwardEuler(self, engine)
             time_step = self.eval_text_in_global(self.time_step_fe)
-            dprint1("time step configuration: " + str(self.time_step_fe) + ':' +  str(time_step))            
+            dprint1("time step configuration: " +
+                    str(self.time_step_fe) + ':' + str(time_step))
             instance.set_timestep(TimeStep(time_step))
-            
+
         elif self.ts_method == "Adaptive BE":
             instance = FirstOrderBackwardEulerAT(self, engine)
             instance.set_timestep(self.abe_minstep)
             instance.set_maxtimestep(self.abe_maxstep)
         else:
-            assert False, "unknown stepping method: "+ self.ts_method
-            
+            assert False, "unknown stepping method: " + self.ts_method
+
         instance.set_start(st)
         instance.set_end(et)
         instance.set_checkpoint(np.linspace(st, et, nt))
 
         engine.sol = engine.assembled_blocks[1][0]
         instance.sol = engine.sol
         instance.time = st
-        
+
         if self.init_only:
             instance.write_checkpoint_solution()
-        
+
         else:
             if is_first:
-                instance.pre_assemble()                                
+                instance.pre_assemble()
                 instance.assemble()
-                
-            #instance.solve()            
-            #if is_first:
-            #self.prepare_form_sol_variables(engine)
+
+            # instance.solve()
+            # if is_first:
+            # self.prepare_form_sol_variables(engine)
             #finished = instance.init(self.init_only)
-            
-            instance.set_blk_mask()                        
+
+            instance.set_blk_mask()
             instance.configure_probes(self.probe)
-        
+
             for solver in self.derived_value_solver():
                 child = solver.allocate_instance(engine)
                 instance.add_child_instance(child)
-                
+
             finished = False
             if fid is not None:
                 fid.write(str(0)+':'+str(instance.time)+"\n")
             while not finished:
                 finished, cp_written = instance.step(is_first)
-                is_first=False
-                
+                is_first = False
+
                 if self.use_dwc_ts:
                     engine.call_dwc(self.get_phys_range(),
                                     method="timestep",
-                                    callername = self.name(),
-                                    dwcname = self.dwc_ts_name,
-                                    args = self.dwc_ts_arg,
-                                    time = instance.time)
-                if self.use_dwc_cp and cp_written:                
+                                    callername=self.name(),
+                                    dwcname=self.dwc_ts_name,
+                                    args=self.dwc_ts_arg,
+                                    time=instance.time)
+                if self.use_dwc_cp and cp_written:
                     engine.call_dwc(self.get_phys_range(),
                                     method="checkpoint",
-                                    callername = self.name(),
-                                    dwcname = self.dwc_cp_name, 
-                                    args = self.dwc_cp_arg,
-                                    time = instance.time,
-                                    icheckpoint = instance.icheckpoint-1)
+                                    callername=self.name(),
+                                    dwcname=self.dwc_cp_name,
+                                    args=self.dwc_cp_arg,
+                                    time=instance.time,
+                                    icheckpoint=instance.icheckpoint-1)
                 if cp_written:
                     instance.save_probe()
                     if fid is not None:
-                        fid.write(str(instance.icheckpoint-1)+':'+str(instance.time)+"\n")
+                        fid.write(str(instance.icheckpoint-1) +
+                                  ':'+str(instance.time)+"\n")
                         fid.flush()
-                        
-        instance.save_solution(ksol = 0,
-                               skip_mesh = False, 
-                               mesh_only = False,
+
+        instance.save_solution(ksol=0,
+                               skip_mesh=False,
+                               mesh_only=False,
                                save_parmesh=self.save_parmesh)
         instance.save_probe()
-        if fid is not None: fid.close()
-        
-        return is_first       
+        if fid is not None:
+            fid.close()
+
+        return is_first
 
-from petram.solver.solver_model import TimeDependentSolverInstance
 
 class FirstOrderBackwardEuler(TimeDependentSolverInstance):
     '''
     Fixed time step solver
     '''
+
     def __init__(self, gui, engine):
         TimeDependentSolverInstance.__init__(self, gui, engine)
         self.pre_assembled = False
         self.assembled = False
         self.counter = 0
-        self._dt_used_in_assemble = 0.0        
+        self._dt_used_in_assemble = 0.0
+
     @property
     def time_step(self):
         return self._time_step(self.counter)
 
     def set_blk_mask(self):
         super(FirstOrderBackwardEuler, self).set_blk_mask()
         phys_target = self.get_target_phys()
         time_deriv_vars = []
         for phys in phys_target:
-           dep_vars0 = phys.dep_vars0
-           dep_vars = phys.dep_vars
-           for x in dep_vars:
-               if not x in dep_vars0: time_deriv_vars.append(x)
+            dep_vars0 = phys.dep_vars0
+            dep_vars = phys.dep_vars
+            for x in dep_vars:
+                if not x in dep_vars0:
+                    time_deriv_vars.append(x)
         self.time_deriv_vars = time_deriv_vars
-        
+
         #self.fes_dt_mask = [False]*len(self.fes_mask)
-        #for name in time_deriv_vars:
+        # for name in time_deriv_vars:
         #     offset = self.engine.dep_var_offset(name)
         #     self.fes_dt_mask[offset] = True
 
         dprint1("time deivatives to be computed", time_deriv_vars)
-        
+
     def pre_assemble(self, update=False):
         engine = self.engine
         phys_target = self.get_phys()
-        phys_range  = self.get_phys_range()
-        
+        phys_range = self.get_phys_range()
+
         if not update:
             engine.run_verify_setting(phys_target, self.gui)
-            
+
         M_Updated = engine.run_assemble_mat(phys_target, phys_range,
-                                             update=update)
+                                            update=update)
         B_Updated = engine.run_assemble_b(phys_target, update=update)
         self.pre_assembled = True
 
         return M_Updated, B_Updated
 
-
     def compute_A(self, M, B, X, mask_M, mask_B):
         '''
         M/dt u_1 + K u_1 = M/dt u_0 + b
         '''
         one_dt = 1./float(self.time_step)
-        A = M[0]+ M[1]*one_dt
+        A = M[0] + M[1]*one_dt
         dprint1("A", A)
         return A, np.any(mask_M)
 
     def compute_rhs(self, M, B, X):
         one_dt = 1./float(self.time_step)
         MM = M[1]*one_dt
         RHS = MM.dot(self.engine.sol) + B
         dprint1("RHS", RHS)
         return RHS
 
     def assemble(self, update=False):
         blocks, M_changed = self.engine.run_assemble_blocks(self.compute_A,
-                                        self.compute_rhs,
-                                        inplace=False,
-                                        update=update)
+                                                            self.compute_rhs,
+                                                            inplace=False,
+                                                            update=update)
 
         #A, X, RHS, Ae, B, M, depvars = blocks
         self.assembled = True
         self._dt_used_in_assemble = self.time_step
         return M_changed
-        
+
     def step(self, is_first):
         engine = self.engine
         mask = self.blk_mask
         engine.copy_block_mask(mask)
-        
-        #if not self.pre_assembled:
+
+        # if not self.pre_assembled:
         #    assert False, "pre_assmeble must have been called"
-            
+
         if (self.counter == 0 and is_first):
             M_changed = True
         else:
             if self._dt_used_in_assemble != self.time_step:
                 engine.set_update_flag('UpdateAll')
             else:
-                engine.set_update_flag('TimeDependent')    
+                engine.set_update_flag('TimeDependent')
             engine.run_apply_essential(self.get_phys(), self.get_phys_range(),
                                        update=True)
-            engine.run_fill_X_block(update=True)        
+            engine.run_fill_X_block(update=True)
             M_updated, B_updated = self.pre_assemble(update=True)
             M_changed = self.assemble(update=True)
 
         A, X, RHS, Ae, B, M, depvars = self.blocks
         if M_changed or self.counter == 0:
             AA = engine.finalize_matrix(A, mask,
-                                        not self.phys_real, format = self.ls_type,
+                                        not self.phys_real, format=self.ls_type,
                                         verbose=False)
+            self._AA = AA
         BB = engine.finalize_rhs([RHS], A, X[-1], mask,
-                                     not self.phys_real, format = self.ls_type,
-                                     verbose=False)
+                                 not self.phys_real, format=self.ls_type,
+                                 verbose=False)
         if self.counter == 0:
             self.sol = engine.sol
             self.write_checkpoint_solution()
             self.icheckpoint += 1
 
         depvars = [x for i, x in enumerate(depvars) if mask[0][i]]
         if self.linearsolver is None:
             is_complex = self.gui.is_complex()
-            self.linearsolver  = self.linearsolver_model.allocate_solver(is_complex, engine)
+            self.linearsolver = self.linearsolver_model.allocate_solver(
+                is_complex, engine)
             M_changed = True
-            
+
         if M_changed:
-            self.linearsolver.SetOperator(AA, dist = engine.is_matrix_distributed,
-                                          name = depvars)
-            
+            self.linearsolver.SetOperator(AA, dist=engine.is_matrix_distributed,
+                                          name=depvars)
+
         if self.linearsolver.is_iterative:
             XX = engine.finalize_x(X[-1], RHS, mask, not self.phys_real,
-                                   format = self.ls_type)
+                                   format=self.ls_type)
         else:
             XX = None
         solall = self.linearsolver.Mult(BB, x=XX, case_base=engine.case_base)
         engine.case_base += len(BB)
-            
+
         if not self.phys_real and self.assemble_real:
             assert False, "this has to be debugged (convertion from real to complex)"
             solall = self.linearsolver_model.real_to_complex(solell, A)
 
-        A.reformat_central_mat(solall, 0, X[0], mask)
-
-        # this apply interpolation operator 
+        #A.reformat_central_mat(solall, 0, X[0], mask)
+        self.reformat_mat(A, self._AA, solall, 0, X[0], mask)
+        # this apply interpolation operator
         sol, sol_extra = engine.split_sol_array(X[0])
 
         for name in self.time_deriv_vars:
             offset1 = engine.dep_var_offset(name)       # vt
             offset2 = engine.dep_var_offset(name[:-1])  # v
-            X[0][offset1, 0] = (X[0][offset2, 0]-X[-1][offset2, 0])*(1./self.time_step)
+            X[0][offset1, 0] = (X[0][offset2, 0]-X[-1]
+                                [offset2, 0])*(1./self.time_step)
 
         for child in self.child_instance:
             # for now update_operator is True only for the first run.
-            child.solve(update_operator = (self.counter == 0))
+            child.solve(update_operator=(self.counter == 0))
 
         self.time = self.time + self.time_step
-        
+
         self.counter += 1
         for p in self.probe:
             p.append_sol(X[0], self.time)
 
-        
         # swap X[0] and X[-1] for next computing
-        tmp = X[0]; X[0] = X[-1]; X[-1]=tmp
+        tmp = X[0]
+        X[0] = X[-1]
+        X[-1] = tmp
         self.sol = X[-1]
         engine.sol = self.sol
 
         engine.recover_sol(sol, access_idx=-1)
-        ## ToDo. Provide a way to use Lagrange multipler in model
+        # ToDo. Provide a way to use Lagrange multipler in model
         extra_data = engine.process_extra(sol_extra)
 
         checkpoint_written = False
         if self.checkpoint[self.icheckpoint] < self.time:
             self.write_checkpoint_solution()
             self.icheckpoint += 1
             checkpoint_written = True
-            
-        dprint1("TimeStep ("+str(self.counter)+ "), t="+str(self.time)+"...done.")
-        dprint1(debug.format_memory_usage())        
+
+        dprint1("TimeStep ("+str(self.counter) + "), t=" +
+                str(self.time)+"...done.")
+        dprint1(debug.format_memory_usage())
         return self.time >= self.et, checkpoint_written
 
     def write_checkpoint_solution(self):
         dprint1("writing checkpoint t=" + str(self.time) +
-                "("+str(self.icheckpoint)+")")        
+                "("+str(self.icheckpoint)+")")
         od = os.getcwd()
-        path = os.path.join(od, 'checkpoint_' + self.gui.parent.name()+'_'+
+        path = os.path.join(od, 'checkpoint_' + self.gui.parent.name()+'_' +
                             self.gui.name()+'_'+str(self.icheckpoint))
-        self.engine.mkdir(path) 
+        self.engine.mkdir(path)
         os.chdir(path)
-        self.engine.cleancwd() 
+        self.engine.cleancwd()
         self.save_solution()
-        self.engine.symlink('../model.pmfm', 'model.pmfm')        
+        self.engine.symlink('../model.pmfm', 'model.pmfm')
         os.chdir(od)
-        
+
+
 class CrankNicolson(FirstOrderBackwardEuler):
     def compute_A(self, M, B, X, mask_M, mask_B):
         '''
         M/dt u_1 + K/2 u_1 = M/dt u_0 - K/2 u_0 + b
         '''
         one_dt = 1./float(self.time_step)
         #MM = M[1]*one_dt
-        A = M[0]*0.5+ M[1]*one_dt
+        A = M[0]*0.5 + M[1]*one_dt
         dprint1("A", A)
         return A, np.any(mask_M)
 
     def compute_rhs(self, M, B, X):
         one_dt = 1./float(self.time_step)
         MM = (-M[0]*0.5 + M[1]*one_dt)
         RHS = MM.dot(self.engine.sol) + B
         dprint1("RHS", RHS)
         return RHS
 
+
 class FirstOrderForwardEuler(FirstOrderBackwardEuler):
     def compute_A(self, M, B, X, mask_M, mask_B):
         '''
         M/dt u_1  = M/dt u_0 - K u_0 + b
         '''
         one_dt = 1./float(self.time_step)
         #MM = M[1]*one_dt
@@ -489,158 +504,187 @@
 
     def compute_rhs(self, M, B, X):
         one_dt = 1./float(self.time_step)
         MM = (-M[0] + M[1]*one_dt)
         RHS = MM.dot(self.engine.sol) + B
         dprint1("RHS", RHS)
         return RHS
-    
-    
+
+
 class FirstOrderBackwardEulerAT(FirstOrderBackwardEuler):
     def __init__(self, gui, engine):
         FirstOrderBackwardEuler.__init__(self, gui, engine)
-        self.linearsolver  = {}
+        self.linearsolver = {}
         self.blocks1 = {}
         self.sol1 = None
         self.sol2 = None
         self._time_step1 = 0
         self._time_step2 = -1
         self.maxstep = 0
 
     def set_maxtimestep(self, dt):
         self.max_timestep = dt
+
     @property
     def time_step1(self):
-        return (self.time_step_base)* 2**self._time_step1
+        return (self.time_step_base) * 2**self._time_step1
+
     @property
     def time_step2(self):
-        return (self.time_step_base)* 2**self._time_step2
-    
+        return (self.time_step_base) * 2**self._time_step2
+
+    @property
+    def time_step(self):
+        return self._time_step
+
+    @time_step.setter
+    def time_step(self, step):
+        self._time_step = step
+
     def set_timestep(self, time_step):
         self.time_step = time_step
         self.time_step_base = time_step
-        
-    def assemble(self,idt=None):
+
+    def assemble(self, idt=None):
         flag = False
         if idt is None:
             idt = 0
             flag = True
         self.blocks1[idt] = self.engine.run_assemble_blocks(self.compute_A,
                                                             self.compute_rhs,
-                                                            inplace=False)        
-        if flag:
-            self.blocks = self.blocks1[0]
-        else:
-            self.blocks = None
-            
-    def step(self):
+                                                            inplace=False)[0]
+        # if flag:
+        #    self.blocks = self.blocks1[0]
+        # else:
+        #    self.blocks = None
+
+    def step(self, is_first):
         dprint1("Entering step", self.time_step1)
+
         def get_A_BB(mode, sol, recompute_rhs=False):
-            if sol is None: sol = self.sol
+            if sol is None:
+                sol = self.sol
             idt = self._time_step1 if mode == 0 else self._time_step2
-            dt  = self.time_step1 if mode == 0 else self.time_step2
-            self.time_step = dt            
+            dt = self.time_step1 if mode == 0 else self.time_step2
+            self.time_step = dt
             if not idt in self.blocks1:
-                self.assemble(idt = idt)
+                self.assemble(idt=idt)
                 A, X, RHS, Ae, B, M, depvars = self.blocks1[idt]
-                BB = engine.finalize_rhs([RHS], not self.phys_real,
-                                         format = self.ls_type, verbose=False)
+                BB = engine.finalize_rhs([RHS], A, X[-1], mask,
+                                         not self.phys_real,
+                                         format=self.ls_type, verbose=False)
             else:
                 A, X, RHS, Ae, B, M, depvars = self.blocks1[idt]
                 if self.counter != 0 or recompute_rhs:
                     # recompute RHS
                     RHS = self.compute_rhs(M, B, [sol])
                     RHS = engine.eliminateBC(Ae, X[1], RHS)
                     RHS = engine.apply_interp(RHS=RHS)
-                BB = engine.finalize_rhs([RHS], not self.phys_real,
-                                         format = self.ls_type, verbose=False)
+                BB = engine.finalize_rhs([RHS], A, X[-1], mask,
+                                         not self.phys_real,
+                                         format=self.ls_type, verbose=False)
             if not idt in self.linearsolver:
-                AA = engine.finalize_matrix(A, not self.phys_real,
-                                            format = self.ls_type, verbose=False)
+                AA = engine.finalize_matrix(A, mask,
+                                            not self.phys_real,
+                                            format=self.ls_type, verbose=False)
+                self._AA = AA
                 if self.ls_type.startswith('coo'):
                     datatype = 'Z' if (AA.dtype == 'complex') else 'D'
                 else:
                     datatype = 'D'
-                self.linearsolver[idt]  = self.linearsolver_model.allocate_solver(datatype,
-                                                                                  engine)
+                self.linearsolver[idt] = self.linearsolver_model.allocate_solver(datatype,
+                                                                                 engine)
                 self.linearsolver[idt].SetOperator(AA,
-                                                   dist = engine.is_matrix_distributed,
-                                                   name = depvars)
-                
-            return A, BB
-            
+                                                   dist=engine.is_matrix_distributed,
+                                                   name=depvars)
+
+            return A, BB, X
+
         engine = self.engine
+        mask = self.blk_mask
+        engine.copy_block_mask(mask)
 
         if not self.pre_assembled:
             assert False, "pre_assmeble must have been called"
 
-        A, BB = get_A_BB(0, self.sol1)
+        A, BB, X = get_A_BB(0, self.sol1)
         solall = self.linearsolver[self._time_step1].Mult(BB)
-        sol1 = A.reformat_central_mat(solall, 0)
+
+        self.reformat_mat(A, self._AA, solall, 0, X[0], mask)
+        sol1 = X[0]
+        #sol1 = A.reformat_central_mat(solall, 0)
         print("check sample1 (0)", [p.current_value(sol1) for p in self.probe])
-        
-        A, BB = get_A_BB(1, self.sol2)
+
+        A, BB, X = get_A_BB(1, self.sol2)
         solall2 = self.linearsolver[self._time_step2].Mult(BB)
-        sol2 = A.reformat_central_mat(solall2, 0)
+        self.reformat_mat(A, self._AA, solall2, 0, X[0], mask)
+        sol2 = X[0]
+        #sol2 = A.reformat_central_mat(solall2, 0)
         print("check sample2 (1)", [p.current_value(sol2) for p in self.probe])
-        
-        A, BB = get_A_BB(1, sol2, recompute_rhs=True)
+
+        A, BB, X = get_A_BB(1, sol2, recompute_rhs=True)
         solall2 = self.linearsolver[self._time_step2].Mult(BB)
-        sol2 = A.reformat_central_mat(solall2, 0)
+        self.reformat_mat(A, self._AA, solall, 0, X[0], mask)
+        sol2 = X[0]
+        #sol2 = A.reformat_central_mat(solall2, 0)
         print("check sample2 (1)", [p.current_value(sol2) for p in self.probe])
 
-        sample1 = np.hstack([p.current_value(sol1) for p in self.probe]).flatten()
-        sample2 = np.hstack([p.current_value(sol2) for p in self.probe]).flatten()
-        
+        sample1 = np.hstack([p.current_value(sol1)
+                            for p in self.probe]).flatten()
+        sample2 = np.hstack([p.current_value(sol2)
+                            for p in self.probe]).flatten()
+
         from petram.mfem_config import use_parallel
         if use_parallel:
-             from petram.helper.mpi_recipes import allgather, allgather_vector
-             sample1 = allgather_vector(np.atleast_1d(sample1))
-             sample2 = allgather_vector(np.atleast_1d(sample2))
-             
-        delta=np.mean(np.abs(sample1-sample2)/np.abs(sample1+sample2)*2)
-    
+            from petram.helper.mpi_recipes import allgather, allgather_vector
+            sample1 = allgather_vector(np.atleast_1d(sample1))
+            sample2 = allgather_vector(np.atleast_1d(sample2))
+
+        delta = np.mean(np.abs(sample1-sample2)/np.abs(sample1+sample2)*2)
+
         threshold = 0.01
         if delta > threshold:
             dprint1("delta is large ", delta, sample1, sample2)
             if self._time_step1 > 0:
                 self._time_step1 -= 1
                 self._time_step2 -= 1
                 dprint1("next try....", self.time_step1, self.time_step2)
-                return False                
+                return False
             else:
-                dprint1("delta may be too large, but restricted by min time step")                
+                dprint1("delta may be too large, but restricted by min time step")
         else:
             dprint1("delta good  ", delta, sample1, sample2)
-        
+
         if not self.phys_real and self.assemble_real:
             assert False, "this has to be debugged (convertion from real to complex)"
             solall = self.linearsolver_model.real_to_complex(solell, A)
-            
+
         self.time = self.time + self.time_step1
         self.counter += 1
-        
-        self.sol = A.reformat_central_mat(solall, 0)
+
+        self.reformat_mat(A, self._AA, solall, 0, X[0], mask)
+        #self.sol = A.reformat_central_mat(solall, 0)
+        self.sol = X[0]
         self.sol1 = self.sol
-        self.sol2 = self.sol        
+        self.sol2 = self.sol
 
         for p in self.probe:
             p.append_sol(self.sol, self.time)
-                
+
+        checkpoint_written = False
         if self.checkpoint[self.icheckpoint] < self.time:
             self.write_checkpoint_solution()
             self.icheckpoint += 1
+            checkpoint_written = True
 
-        dprint1("TimeStep ("+str(self.counter)+ "), t="+str(self.time)+"...done.")
+        dprint1("TimeStep ("+str(self.counter) + "), t=" +
+                str(self.time)+"...done.")
         if delta < threshold/4:
-            dt_test = (self.time_step_base)* 2**(self._time_step1 + 1)
-            if self.max_timestep >  dt_test:
-                 self._time_step1 += 1
-                 self._time_step2 += 1
-                 dprint1("next try....", self.time_step1, self.time_step2)
+            dt_test = (self.time_step_base) * 2**(self._time_step1 + 1)
+            if self.max_timestep > dt_test:
+                self._time_step1 += 1
+                self._time_step2 += 1
+                dprint1("next try....", self.time_step1, self.time_step2)
             else:
-                 dprint1("delta is small, but restricted by max time step")
-        return self.time >= self.et
-                      
-
-
+                dprint1("delta is small, but restricted by max time step")
 
+        return self.time >= self.et, checkpoint_written
```

### Comparing `PetraM_Base-2.1.30/petram/utils.py` & `petram_base-2.1.38/petram/utils.py`

 * *Files identical despite different names*

### Comparing `PetraM_Base-2.1.30/setup.py` & `petram_base-2.1.38/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,18 +13,19 @@
 
 with open(path.join(here, 'README.md')) as f:
     long_description = f.read()
 
 setup(
     name='PetraM_Base',
 
-    version='2.1.30',
+    version='2.1.38',
 
     description='PetraM base package',
     long_description=long_description,
+    long_description_content_type = 'text/markdown',    
     url='https://github.com/piScope/PetraM',
     author='S. Shiraiwa',
     author_email='shiraiwa@prenceton.edu',
     license='GNUv3',
 
     classifiers=[
         #   3 - Alpha
```


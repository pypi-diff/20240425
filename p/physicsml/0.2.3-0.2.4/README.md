# Comparing `tmp/physicsml-0.2.3.tar.gz` & `tmp/physicsml-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "physicsml-0.2.3.tar", last modified: Tue Apr  9 10:47:13 2024, max compression
+gzip compressed data, was "physicsml-0.2.4.tar", last modified: Thu Apr 25 13:13:24 2024, max compression
```

## Comparing `physicsml-0.2.3.tar` & `physicsml-0.2.4.tar`

### file list

```diff
@@ -1,454 +1,456 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:13.019042 physicsml-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-04-09 10:46:47.000000 physicsml-0.2.3/.envrc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:12.935042 physicsml-0.2.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:12.951042 physicsml-0.2.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-09 10:46:47.000000 physicsml-0.2.3/.github/workflows/dev-ci-actions.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-09 10:46:47.000000 physicsml-0.2.3/.github/workflows/docs-build-deploy.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-04-09 10:46:47.000000 physicsml-0.2.3/.github/workflows/latest-tests.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-09 10:46:47.000000 physicsml-0.2.3/.github/workflows/main-ci-actions.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-04-09 10:46:47.000000 physicsml-0.2.3/.github/workflows/pinned-tests.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-09 10:46:47.000000 physicsml-0.2.3/.github/workflows/publish-package.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-09 10:46:47.000000 physicsml-0.2.3/.github/workflows/quality-typing-checks.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-09 10:46:47.000000 physicsml-0.2.3/.github/workflows/release-ci-actions.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-09 10:46:47.000000 physicsml-0.2.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-04-09 10:46:47.000000 physicsml-0.2.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-04-09 10:46:47.000000 physicsml-0.2.3/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-09 10:46:47.000000 physicsml-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4650 2024-04-09 10:47:13.019042 physicsml-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-04-09 10:46:47.000000 physicsml-0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:12.951042 physicsml-0.2.3/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-09 10:46:47.000000 physicsml-0.2.3/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-09 10:46:47.000000 physicsml-0.2.3/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:12.951042 physicsml-0.2.3/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:12.951042 physicsml-0.2.3/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     3348 2024-04-09 10:46:47.000000 physicsml-0.2.3/docs/source/_static/PhysicsML_Logo-01.svg
--rw-r--r--   0 runner    (1001) docker     (127)     7381 2024-04-09 10:46:47.000000 physicsml-0.2.3/docs/source/_static/PhysicsML_Logo_PhyML_logo full dark-cropped.svg
--rw-r--r--   0 runner    (1001) docker     (127)     7503 2024-04-09 10:46:47.000000 physicsml-0.2.3/docs/source/_static/PhysicsML_Logo_PhyML_logo full dark.svg
--rw-r--r--   0 runner    (1001) docker     (127)     7380 2024-04-09 10:46:47.000000 physicsml-0.2.3/docs/source/_static/PhysicsML_Logo_PhyML_logo full light-cropped.svg
--rw-r--r--   0 runner    (1001) docker     (127)     7502 2024-04-09 10:46:47.000000 physicsml-0.2.3/docs/source/_static/PhysicsML_Logo_PhyML_logo full light.svg
--rw-r--r--   0 runner    (1001) docker     (127)     7824 2024-04-09 10:46:47.000000 physicsml-0.2.3/docs/source/_static/PhysicsML_Logo_PhyML_logo text dark.svg
--rw-r--r--   0 runner    (1001) docker     (127)     7836 2024-04-09 10:46:47.000000 physicsml-0.2.3/docs/source/_static/PhysicsML_Logo_PhyML_logo text light.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-04-09 10:46:47.000000 physicsml-0.2.3/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-04-09 10:46:47.000000 physicsml-0.2.3/docs/source/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:12.935042 physicsml-0.2.3/docs/source/pages/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:12.951042 physicsml-0.2.3/docs/source/pages/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)     5631 2024-04-09 10:46:47.000000 physicsml-0.2.3/docs/source/pages/datasets/qm_datasets.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:12.951042 physicsml-0.2.3/docs/source/pages/features/
--rw-r--r--   0 runner    (1001) docker     (127)   489710 2024-04-09 10:46:48.000000 physicsml-0.2.3/docs/source/pages/features/gdb9_trunc.parquet
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-09 10:46:48.000000 physicsml-0.2.3/docs/source/pages/features/how_to_add_reps.md
--rw-r--r--   0 runner    (1001) docker     (127)     9303 2024-04-09 10:46:48.000000 physicsml-0.2.3/docs/source/pages/features/intro.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:12.955042 physicsml-0.2.3/docs/source/pages/models/
--rw-r--r--   0 runner    (1001) docker     (127)     4886 2024-04-09 10:46:48.000000 physicsml-0.2.3/docs/source/pages/models/allegro.md
--rw-r--r--   0 runner    (1001) docker     (127)     3349 2024-04-09 10:46:48.000000 physicsml-0.2.3/docs/source/pages/models/ani.md
--rw-r--r--   0 runner    (1001) docker     (127)    10655 2024-04-09 10:46:48.000000 physicsml-0.2.3/docs/source/pages/models/egnn.md
--rw-r--r--   0 runner    (1001) docker     (127)     6295 2024-04-09 10:46:48.000000 physicsml-0.2.3/docs/source/pages/models/how_to_add_models.md
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-09 10:46:48.000000 physicsml-0.2.3/docs/source/pages/models/intro.md
--rw-r--r--   0 runner    (1001) docker     (127)     8347 2024-04-09 10:46:48.000000 physicsml-0.2.3/docs/source/pages/models/mace.md
--rw-r--r--   0 runner    (1001) docker     (127)     8998 2024-04-09 10:46:48.000000 physicsml-0.2.3/docs/source/pages/models/nequip.md
--rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-04-09 10:46:48.000000 physicsml-0.2.3/docs/source/pages/models/tensor_net.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:12.955042 physicsml-0.2.3/docs/source/pages/philosophy/
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-09 10:46:48.000000 physicsml-0.2.3/docs/source/pages/philosophy/molflux.md
--rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-04-09 10:46:48.000000 physicsml-0.2.3/docs/source/pages/philosophy/philosophy.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:12.955042 physicsml-0.2.3/docs/source/pages/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-09 10:46:48.000000 physicsml-0.2.3/docs/source/pages/plugins/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     4578 2024-04-09 10:46:48.000000 physicsml-0.2.3/docs/source/pages/plugins/alanine-dipeptide-truncated.pdb
--rw-r--r--   0 runner    (1001) docker     (127)     3899 2024-04-09 10:46:48.000000 physicsml-0.2.3/docs/source/pages/plugins/ase.md
--rw-r--r--   0 runner    (1001) docker     (127)     5335 2024-04-09 10:46:48.000000 physicsml-0.2.3/docs/source/pages/plugins/openmm.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:12.955042 physicsml-0.2.3/docs/source/pages/structure/
--rw-r--r--   0 runner    (1001) docker     (127)     7237 2024-04-09 10:46:48.000000 physicsml-0.2.3/docs/source/pages/structure/lightning_layer.md
--rw-r--r--   0 runner    (1001) docker     (127)     4803 2024-04-09 10:46:48.000000 physicsml-0.2.3/docs/source/pages/structure/molflux_layer.md
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-09 10:46:48.000000 physicsml-0.2.3/docs/source/pages/structure/physicsml_structure.md
--rw-r--r--   0 runner    (1001) docker     (127)     6294 2024-04-09 10:46:48.000000 physicsml-0.2.3/docs/source/pages/structure/torch_layer.md
--rw-r--r--   0 runner    (1001) docker     (127)     2906 2024-04-09 10:46:48.000000 physicsml-0.2.3/docs/source/pages/structure/transfer_learning.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:12.959042 physicsml-0.2.3/docs/source/pages/tutorials/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-09 10:46:48.000000 physicsml-0.2.3/docs/source/pages/tutorials/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     7462 2024-04-09 10:46:48.000000 physicsml-0.2.3/docs/source/pages/tutorials/ani1x_energy_forces_training.md
--rw-r--r--   0 runner    (1001) docker     (127)  1610932 2024-04-09 10:46:48.000000 physicsml-0.2.3/docs/source/pages/tutorials/ani1x_truncated.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     9729 2024-04-09 10:46:48.000000 physicsml-0.2.3/docs/source/pages/tutorials/gdb9_training.md
--rw-r--r--   0 runner    (1001) docker     (127)   489710 2024-04-09 10:46:48.000000 physicsml-0.2.3/docs/source/pages/tutorials/gdb9_trunc.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     7678 2024-04-09 10:46:48.000000 physicsml-0.2.3/docs/source/pages/tutorials/gdb9_uncertainty.md
--rw-r--r--   0 runner    (1001) docker     (127)    10605 2024-04-09 10:46:48.000000 physicsml-0.2.3/docs/source/pages/tutorials/transfer_learning.md
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-09 10:46:48.000000 physicsml-0.2.3/environment.yml
--rwxr-xr-x   0 runner    (1001) docker     (127)     1053 2024-04-09 10:46:48.000000 physicsml-0.2.3/init_conda_venv.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      714 2024-04-09 10:46:48.000000 physicsml-0.2.3/init_python_venv.sh
--rw-r--r--   0 runner    (1001) docker     (127)    12217 2024-04-09 10:46:48.000000 physicsml-0.2.3/noxfile.py
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-09 10:46:48.000000 physicsml-0.2.3/openmm_env.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:12.939042 physicsml-0.2.3/pinned-versions/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:12.959042 physicsml-0.2.3/pinned-versions/3.10/
--rw-r--r--   0 runner    (1001) docker     (127)    12169 2024-04-09 10:46:48.000000 physicsml-0.2.3/pinned-versions/3.10/lockfile.ase.txt
--rw-r--r--   0 runner    (1001) docker     (127)    12168 2024-04-09 10:46:48.000000 physicsml-0.2.3/pinned-versions/3.10/lockfile.core.txt
--rw-r--r--   0 runner    (1001) docker     (127)    12237 2024-04-09 10:46:48.000000 physicsml-0.2.3/pinned-versions/3.10/lockfile.openeye.txt
--rw-r--r--   0 runner    (1001) docker     (127)    12172 2024-04-09 10:46:48.000000 physicsml-0.2.3/pinned-versions/3.10/lockfile.openmm.txt
--rw-r--r--   0 runner    (1001) docker     (127)    12171 2024-04-09 10:46:48.000000 physicsml-0.2.3/pinned-versions/3.10/lockfile.rdkit.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:12.959042 physicsml-0.2.3/pinned-versions/3.11/
--rw-r--r--   0 runner    (1001) docker     (127)    11991 2024-04-09 10:46:48.000000 physicsml-0.2.3/pinned-versions/3.11/lockfile.ase.txt
--rw-r--r--   0 runner    (1001) docker     (127)    11990 2024-04-09 10:46:48.000000 physicsml-0.2.3/pinned-versions/3.11/lockfile.core.txt
--rw-r--r--   0 runner    (1001) docker     (127)    12059 2024-04-09 10:46:48.000000 physicsml-0.2.3/pinned-versions/3.11/lockfile.openeye.txt
--rw-r--r--   0 runner    (1001) docker     (127)    11994 2024-04-09 10:46:48.000000 physicsml-0.2.3/pinned-versions/3.11/lockfile.openmm.txt
--rw-r--r--   0 runner    (1001) docker     (127)    11993 2024-04-09 10:46:48.000000 physicsml-0.2.3/pinned-versions/3.11/lockfile.rdkit.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:12.963042 physicsml-0.2.3/pinned-versions/3.8/
--rw-r--r--   0 runner    (1001) docker     (127)    13023 2024-04-09 10:46:48.000000 physicsml-0.2.3/pinned-versions/3.8/lockfile.ase.txt
--rw-r--r--   0 runner    (1001) docker     (127)    13022 2024-04-09 10:46:48.000000 physicsml-0.2.3/pinned-versions/3.8/lockfile.core.txt
--rw-r--r--   0 runner    (1001) docker     (127)    13193 2024-04-09 10:46:48.000000 physicsml-0.2.3/pinned-versions/3.8/lockfile.openeye.txt
--rw-r--r--   0 runner    (1001) docker     (127)    13026 2024-04-09 10:46:48.000000 physicsml-0.2.3/pinned-versions/3.8/lockfile.openmm.txt
--rw-r--r--   0 runner    (1001) docker     (127)    13025 2024-04-09 10:46:48.000000 physicsml-0.2.3/pinned-versions/3.8/lockfile.rdkit.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:12.963042 physicsml-0.2.3/pinned-versions/3.9/
--rw-r--r--   0 runner    (1001) docker     (127)    12324 2024-04-09 10:46:48.000000 physicsml-0.2.3/pinned-versions/3.9/lockfile.ase.txt
--rw-r--r--   0 runner    (1001) docker     (127)    12323 2024-04-09 10:46:48.000000 physicsml-0.2.3/pinned-versions/3.9/lockfile.core.txt
--rw-r--r--   0 runner    (1001) docker     (127)    12392 2024-04-09 10:46:48.000000 physicsml-0.2.3/pinned-versions/3.9/lockfile.openeye.txt
--rw-r--r--   0 runner    (1001) docker     (127)    12327 2024-04-09 10:46:48.000000 physicsml-0.2.3/pinned-versions/3.9/lockfile.openmm.txt
--rw-r--r--   0 runner    (1001) docker     (127)    12326 2024-04-09 10:46:48.000000 physicsml-0.2.3/pinned-versions/3.9/lockfile.rdkit.txt
--rw-r--r--   0 runner    (1001) docker     (127)     7505 2024-04-09 10:46:48.000000 physicsml-0.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 10:47:13.019042 physicsml-0.2.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:12.939042 physicsml-0.2.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:12.963042 physicsml-0.2.3/src/physicsml/
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:12.967042 physicsml-0.2.3/src/physicsml/backends/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2286 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/backends/backend_selector.py
--rw-r--r--   0 runner    (1001) docker     (127)     4970 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/backends/openeye_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     4927 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/backends/rdkit_backend.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:12.967042 physicsml-0.2.3/src/physicsml/featurisation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/featurisation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:12.967042 physicsml-0.2.3/src/physicsml/featurisation/physicsml_features/
--rw-r--r--   0 runner    (1001) docker     (127)     4246 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/featurisation/physicsml_features/atom_features.py
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/featurisation/physicsml_features/bond_features.py
--rw-r--r--   0 runner    (1001) docker     (127)     5600 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/featurisation/physicsml_features/physicsml_features.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:12.967042 physicsml-0.2.3/src/physicsml/lightning/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/lightning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3569 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/lightning/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5705 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/lightning/datamodule.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:12.967042 physicsml-0.2.3/src/physicsml/lightning/graph_datasets/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/lightning/graph_datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13126 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/lightning/graph_datasets/graph_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     5583 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/lightning/graph_datasets/neighbourhood_list_torch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:12.971042 physicsml-0.2.3/src/physicsml/lightning/graph_datasets/torch_nl_vendored/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/lightning/graph_datasets/torch_nl_vendored/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/lightning/graph_datasets/torch_nl_vendored/geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)    12716 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/lightning/graph_datasets/torch_nl_vendored/linked_cell.py
--rw-r--r--   0 runner    (1001) docker     (127)     2482 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/lightning/graph_datasets/torch_nl_vendored/naive_impl.py
--rw-r--r--   0 runner    (1001) docker     (127)     5236 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/lightning/graph_datasets/torch_nl_vendored/neighbor_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/lightning/graph_datasets/torch_nl_vendored/timer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/lightning/graph_datasets/torch_nl_vendored/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:12.971042 physicsml-0.2.3/src/physicsml/lightning/losses/
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/lightning/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10118 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/lightning/losses/barlow_twins_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/lightning/losses/construct_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/lightning/losses/loss_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/lightning/losses/masked_mse_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/lightning/losses/multitask_losses.py
--rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/lightning/losses/serial_bce_w_logits_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)      982 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/lightning/losses/stock_losses.py
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/lightning/losses/weighted_mse_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     4642 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/lightning/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6462 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/lightning/model_uncertainty.py
--rw-r--r--   0 runner    (1001) docker     (127)     6630 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/lightning/module.py
--rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/lightning/pre_batching_in_memory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/lightning/pre_batching_on_disk.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:12.971042 physicsml-0.2.3/src/physicsml/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:12.971042 physicsml-0.2.3/src/physicsml/models/allegro/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/allegro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4108 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/allegro/allegro_prism.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:12.971042 physicsml-0.2.3/src/physicsml/models/allegro/mean_var/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/allegro/mean_var/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/allegro/mean_var/default_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/allegro/mean_var/mean_var_allegro_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6496 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/allegro/mean_var/mean_var_allegro_module.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:12.975042 physicsml-0.2.3/src/physicsml/models/allegro/modules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/allegro/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24182 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/allegro/modules/allegro.py
--rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/allegro/modules/channels.py
--rw-r--r--   0 runner    (1001) docker     (127)    15463 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/allegro/modules/contract.py
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/allegro/modules/cutoffs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5427 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/allegro/modules/fc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2759 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/allegro/modules/layout.py
--rw-r--r--   0 runner    (1001) docker     (127)     8447 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/allegro/modules/linear.py
--rw-r--r--   0 runner    (1001) docker     (127)     3696 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/allegro/modules/radial.py
--rw-r--r--   0 runner    (1001) docker     (127)     5406 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/allegro/modules/spmm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:12.975042 physicsml-0.2.3/src/physicsml/models/allegro/supervised/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/allegro/supervised/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/allegro/supervised/allegro_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5639 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/allegro/supervised/allegro_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/allegro/supervised/default_configs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:12.975042 physicsml-0.2.3/src/physicsml/models/ani/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/ani/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4619 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/ani/ani_1_2_defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     5150 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/ani/ani_datamodule.py
--rw-r--r--   0 runner    (1001) docker     (127)     5859 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/ani/ani_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2826 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/ani/ani_prism.py
--rw-r--r--   0 runner    (1001) docker     (127)     2688 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/ani/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:12.975042 physicsml-0.2.3/src/physicsml/models/ani/ensemble/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/ani/ensemble/default_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/ani/ensemble/ensemble_ani_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     9754 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/ani/ensemble/ensemble_ani_module.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:12.975042 physicsml-0.2.3/src/physicsml/models/ani/mean_var/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/ani/mean_var/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/ani/mean_var/default_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/ani/mean_var/mean_var_ani_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     8955 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/ani/mean_var/mean_var_ani_module.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:12.979042 physicsml-0.2.3/src/physicsml/models/ani/supervised/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/ani/supervised/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/ani/supervised/ani_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     8395 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/ani/supervised/ani_module.py
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/ani/supervised/default_configs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:12.979042 physicsml-0.2.3/src/physicsml/models/egnn/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/egnn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:12.979042 physicsml-0.2.3/src/physicsml/models/egnn/adapter/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/egnn/adapter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/egnn/adapter/adapter_egnn_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6317 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/egnn/adapter/adapter_egnn_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     6599 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/egnn/adapter/adapter_egnn_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/egnn/adapter/default_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4251 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/egnn/egnn_prism.py
--rw-r--r--   0 runner    (1001) docker     (127)    15452 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/egnn/egnn_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:12.979042 physicsml-0.2.3/src/physicsml/models/egnn/mean_var/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/egnn/mean_var/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/egnn/mean_var/default_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/egnn/mean_var/mean_var_egnn_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6987 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/egnn/mean_var/mean_var_egnn_module.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:12.979042 physicsml-0.2.3/src/physicsml/models/egnn/ssf/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/egnn/ssf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/egnn/ssf/default_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/egnn/ssf/ssf_egnn_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6159 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/egnn/ssf/ssf_egnn_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     3689 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/egnn/ssf/ssf_egnn_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:12.983042 physicsml-0.2.3/src/physicsml/models/egnn/supervised/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/egnn/supervised/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/egnn/supervised/default_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/egnn/supervised/egnn_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6308 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/egnn/supervised/egnn_module.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:12.983042 physicsml-0.2.3/src/physicsml/models/mace/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/mace/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:12.983042 physicsml-0.2.3/src/physicsml/models/mace/adapter/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/mace/adapter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/mace/adapter/adapter_mace_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     8422 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/mace/adapter/adapter_mace_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     8480 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/mace/adapter/adapter_mace_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/mace/adapter/default_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4194 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/mace/mace_prism.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:12.983042 physicsml-0.2.3/src/physicsml/models/mace/mean_var/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/mace/mean_var/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/mace/mean_var/default_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/mace/mean_var/mean_var_mace_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     8887 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/mace/mean_var/mean_var_mace_module.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:12.983042 physicsml-0.2.3/src/physicsml/models/mace/modules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/mace/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3773 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/mace/modules/_activation.py
--rw-r--r--   0 runner    (1001) docker     (127)     8197 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/mace/modules/blocks.py
--rw-r--r--   0 runner    (1001) docker     (127)     4377 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/mace/modules/cg.py
--rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/mace/modules/irreps_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     8507 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/mace/modules/mace.py
--rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/mace/modules/radial.py
--rw-r--r--   0 runner    (1001) docker     (127)     9635 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/mace/modules/symmetric_contraction.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:12.987042 physicsml-0.2.3/src/physicsml/models/mace/ssf/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/mace/ssf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/mace/ssf/default_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/mace/ssf/ssf_mace_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     8236 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/mace/ssf/ssf_mace_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     6820 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/mace/ssf/ssf_mace_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:12.987042 physicsml-0.2.3/src/physicsml/models/mace/supervised/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/mace/supervised/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/mace/supervised/default_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/mace/supervised/mace_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     8133 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/mace/supervised/mace_module.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:12.987042 physicsml-0.2.3/src/physicsml/models/nequip/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/nequip/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:12.987042 physicsml-0.2.3/src/physicsml/models/nequip/adapter/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/nequip/adapter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/nequip/adapter/adapter_nequip_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6696 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/nequip/adapter/adapter_nequip_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     7075 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/nequip/adapter/adapter_nequip_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/nequip/adapter/default_configs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:12.987042 physicsml-0.2.3/src/physicsml/models/nequip/mean_var/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/nequip/mean_var/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/nequip/mean_var/default_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/nequip/mean_var/mean_var_nequip_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     7196 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/nequip/mean_var/mean_var_nequip_module.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:12.991042 physicsml-0.2.3/src/physicsml/models/nequip/modules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/nequip/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3773 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/nequip/modules/_activation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5727 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/nequip/modules/_gate.py
--rw-r--r--   0 runner    (1001) docker     (127)     3466 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/nequip/modules/convnet_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3683 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/nequip/modules/interaction_block.py
--rw-r--r--   0 runner    (1001) docker     (127)     5968 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/nequip/modules/nequip.py
--rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/nequip/modules/radial.py
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/nequip/modules/scale_shift.py
--rw-r--r--   0 runner    (1001) docker     (127)     4494 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/nequip/nequip_prism.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:12.991042 physicsml-0.2.3/src/physicsml/models/nequip/ssf/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/nequip/ssf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/nequip/ssf/default_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/nequip/ssf/ssf_nequip_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6522 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/nequip/ssf/ssf_nequip_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     5306 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/nequip/ssf/ssf_nequip_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:12.991042 physicsml-0.2.3/src/physicsml/models/nequip/supervised/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/nequip/supervised/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/nequip/supervised/default_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/nequip/supervised/nequip_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6431 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/nequip/supervised/nequip_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     4990 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/prism.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:12.991042 physicsml-0.2.3/src/physicsml/models/tensor_net/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/tensor_net/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:12.991042 physicsml-0.2.3/src/physicsml/models/tensor_net/modules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/tensor_net/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7368 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/tensor_net/modules/embedding.py
--rw-r--r--   0 runner    (1001) docker     (127)     3621 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/tensor_net/modules/interaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/tensor_net/modules/output.py
--rw-r--r--   0 runner    (1001) docker     (127)     3279 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/tensor_net/modules/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:12.991042 physicsml-0.2.3/src/physicsml/models/tensor_net/supervised/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/tensor_net/supervised/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/tensor_net/supervised/default_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/tensor_net/supervised/tensor_net_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4882 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/tensor_net/supervised/tensor_net_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     3593 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/models/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:12.991042 physicsml-0.2.3/src/physicsml/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:12.995042 physicsml-0.2.3/src/physicsml/plugins/ase/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/plugins/ase/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/plugins/ase/ase_ani.py
--rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/plugins/ase/ase_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     3717 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/plugins/ase/calculator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/plugins/ase/load.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:12.995042 physicsml-0.2.3/src/physicsml/plugins/openmm/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/plugins/openmm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/plugins/openmm/load.py
--rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/plugins/openmm/openmm_ani.py
--rw-r--r--   0 runner    (1001) docker     (127)     4571 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/plugins/openmm/openmm_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6285 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/plugins/openmm/openmm_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     5370 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/plugins/openmm/physicsml_potential.py
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     3130 2024-04-09 10:46:48.000000 physicsml-0.2.3/src/physicsml/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-09 10:47:12.000000 physicsml-0.2.3/src/physicsml/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:13.015042 physicsml-0.2.3/src/physicsml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4650 2024-04-09 10:47:12.000000 physicsml-0.2.3/src/physicsml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    16449 2024-04-09 10:47:12.000000 physicsml-0.2.3/src/physicsml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 10:47:12.000000 physicsml-0.2.3/src/physicsml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-04-09 10:47:12.000000 physicsml-0.2.3/src/physicsml.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-09 10:47:12.000000 physicsml-0.2.3/src/physicsml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-09 10:47:12.000000 physicsml-0.2.3/src/physicsml.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:12.995042 physicsml-0.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:12.995042 physicsml-0.2.3/tests/ase/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/ase/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9983 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/ase/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/ase/test_ase_ani.py
--rw-r--r--   0 runner    (1001) docker     (127)     2865 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/ase/test_ase_graph.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:12.999042 physicsml-0.2.3/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)     4578 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/data/alanine-dipeptide-truncated.pdb
--rw-r--r--   0 runner    (1001) docker     (127)   698696 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/data/ani1x.h5
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:12.999042 physicsml-0.2.3/tests/data/ani_model/
--rw-r--r--   0 runner    (1001) docker     (127)     5795 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/data/ani_model/featurisation_metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:12.999042 physicsml-0.2.3/tests/data/ani_model/model_artefacts/
--rw-r--r--   0 runner    (1001) docker     (127)  1320280 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/data/ani_model/model_artefacts/module_checkpoint.ckpt
--rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/data/ani_model/model_config.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:12.999042 physicsml-0.2.3/tests/data/egnn_model/
--rw-r--r--   0 runner    (1001) docker     (127)     5795 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/data/egnn_model/featurisation_metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:12.999042 physicsml-0.2.3/tests/data/egnn_model/model_artefacts/
--rw-r--r--   0 runner    (1001) docker     (127)    52081 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/data/egnn_model/model_artefacts/module_checkpoint.ckpt
--rw-r--r--   0 runner    (1001) docker     (127)     3496 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/data/egnn_model/model_config.json
--rw-r--r--   0 runner    (1001) docker     (127)    20277 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/data/gdb9.csv
--rw-r--r--   0 runner    (1001) docker     (127)    98022 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/data/gdb9.sdf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:13.003042 physicsml-0.2.3/tests/data/mace_model/
--rw-r--r--   0 runner    (1001) docker     (127)     5795 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/data/mace_model/featurisation_metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:13.003042 physicsml-0.2.3/tests/data/mace_model/model_artefacts/
--rw-r--r--   0 runner    (1001) docker     (127)   117170 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/data/mace_model/model_artefacts/module_checkpoint.ckpt
--rw-r--r--   0 runner    (1001) docker     (127)     3433 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/data/mace_model/model_config.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:13.003042 physicsml-0.2.3/tests/data/nequip_model/
--rw-r--r--   0 runner    (1001) docker     (127)     5795 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/data/nequip_model/featurisation_metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:13.003042 physicsml-0.2.3/tests/data/nequip_model/model_artefacts/
--rw-r--r--   0 runner    (1001) docker     (127)    86167 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/data/nequip_model/model_artefacts/module_checkpoint.ckpt
--rw-r--r--   0 runner    (1001) docker     (127)     3501 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/data/nequip_model/model_config.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:13.003042 physicsml-0.2.3/tests/openeye/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/openeye/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9987 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/openeye/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:13.003042 physicsml-0.2.3/tests/openeye/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/openeye/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:13.003042 physicsml-0.2.3/tests/openeye/core/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/openeye/core/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/openeye/core/data/test_datamodule.py
--rw-r--r--   0 runner    (1001) docker     (127)     6036 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/openeye/core/data/test_graph_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:13.003042 physicsml-0.2.3/tests/openeye/core/featurisation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/openeye/core/featurisation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4999 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/openeye/core/featurisation/test_physicsml_featurisation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:13.003042 physicsml-0.2.3/tests/openeye/integration/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/openeye/integration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:13.003042 physicsml-0.2.3/tests/openeye/integration/prism/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/openeye/integration/prism/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3258 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/openeye/integration/prism/test_egnn_prism.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:13.003042 physicsml-0.2.3/tests/openeye/integration/training/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/openeye/integration/training/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:13.003042 physicsml-0.2.3/tests/openeye/integration/training/egnn/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/openeye/integration/training/egnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/openeye/integration/training/egnn/test_egnn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:13.007043 physicsml-0.2.3/tests/openmm/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/openmm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9942 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/openmm/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    10818 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/openmm/test_openmm_ani.py
--rw-r--r--   0 runner    (1001) docker     (127)    16225 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/openmm/test_openmm_egnn.py
--rw-r--r--   0 runner    (1001) docker     (127)    16422 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/openmm/test_openmm_mace.py
--rw-r--r--   0 runner    (1001) docker     (127)    16903 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/openmm/test_openmm_nequip.py
--rw-r--r--   0 runner    (1001) docker     (127)     7399 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/openmm/test_openmm_nnp_potential.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:13.007043 physicsml-0.2.3/tests/rdkit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/rdkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9982 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/rdkit/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:13.007043 physicsml-0.2.3/tests/rdkit/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/rdkit/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:13.007043 physicsml-0.2.3/tests/rdkit/core/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/rdkit/core/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/rdkit/core/data/test_datamodule.py
--rw-r--r--   0 runner    (1001) docker     (127)     6036 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/rdkit/core/data/test_graph_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:13.007043 physicsml-0.2.3/tests/rdkit/core/featurisation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/rdkit/core/featurisation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4978 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/rdkit/core/featurisation/test_physicsml_featurisation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:13.007043 physicsml-0.2.3/tests/rdkit/integration/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/rdkit/integration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:13.007043 physicsml-0.2.3/tests/rdkit/integration/prism/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/rdkit/integration/prism/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3573 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/rdkit/integration/prism/test_allegro_prism.py
--rw-r--r--   0 runner    (1001) docker     (127)     2966 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/rdkit/integration/prism/test_ani_prism.py
--rw-r--r--   0 runner    (1001) docker     (127)     3258 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/rdkit/integration/prism/test_egnn_prism.py
--rw-r--r--   0 runner    (1001) docker     (127)     3346 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/rdkit/integration/prism/test_mace_prism.py
--rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/rdkit/integration/prism/test_nequip_prism.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:13.007043 physicsml-0.2.3/tests/rdkit/integration/training/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/rdkit/integration/training/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:13.011042 physicsml-0.2.3/tests/rdkit/integration/training/allegro/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/rdkit/integration/training/allegro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/rdkit/integration/training/allegro/test_allegro_energy_charges.py
--rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/rdkit/integration/training/allegro/test_allegro_forces.py
--rw-r--r--   0 runner    (1001) docker     (127)     3375 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/rdkit/integration/training/allegro/test_allegro_mean_var.py
--rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/rdkit/integration/training/allegro/test_allergo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:13.011042 physicsml-0.2.3/tests/rdkit/integration/training/ani/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/rdkit/integration/training/ani/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/rdkit/integration/training/ani/test_ani.py
--rw-r--r--   0 runner    (1001) docker     (127)     2877 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/rdkit/integration/training/ani/test_ani_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/rdkit/integration/training/ani/test_ani_forces.py
--rw-r--r--   0 runner    (1001) docker     (127)     2724 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/rdkit/integration/training/ani/test_ani_mean_var.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:13.011042 physicsml-0.2.3/tests/rdkit/integration/training/egnn/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/rdkit/integration/training/egnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2075 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/rdkit/integration/training/egnn/test_adapter_egnn.py
--rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/rdkit/integration/training/egnn/test_egnn.py
--rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/rdkit/integration/training/egnn/test_egnn_energy_charges.py
--rw-r--r--   0 runner    (1001) docker     (127)     2343 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/rdkit/integration/training/egnn/test_egnn_forces.py
--rw-r--r--   0 runner    (1001) docker     (127)     3024 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/rdkit/integration/training/egnn/test_egnn_mean_var.py
--rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/rdkit/integration/training/egnn/test_ssf_egnn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:13.011042 physicsml-0.2.3/tests/rdkit/integration/training/mace/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/rdkit/integration/training/mace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2165 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/rdkit/integration/training/mace/test_adapter_mace.py
--rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/rdkit/integration/training/mace/test_mace.py
--rw-r--r--   0 runner    (1001) docker     (127)     2985 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/rdkit/integration/training/mace/test_mace_energy_charges.py
--rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/rdkit/integration/training/mace/test_mace_forces.py
--rw-r--r--   0 runner    (1001) docker     (127)     3081 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/rdkit/integration/training/mace/test_mace_mean_var.py
--rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/rdkit/integration/training/mace/test_ssf_mace.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:13.015042 physicsml-0.2.3/tests/rdkit/integration/training/nequip/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/rdkit/integration/training/nequip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/rdkit/integration/training/nequip/test_adapter_nequip.py
--rw-r--r--   0 runner    (1001) docker     (127)     2121 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/rdkit/integration/training/nequip/test_nequip.py
--rw-r--r--   0 runner    (1001) docker     (127)     3089 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/rdkit/integration/training/nequip/test_nequip_energy_charges.py
--rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/rdkit/integration/training/nequip/test_nequip_forces.py
--rw-r--r--   0 runner    (1001) docker     (127)     3248 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/rdkit/integration/training/nequip/test_nequip_mean_var.py
--rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/rdkit/integration/training/nequip/test_ssf_nequip.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:47:13.015042 physicsml-0.2.3/tests/rdkit/integration/training/tensor_net/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/rdkit/integration/training/tensor_net/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/rdkit/integration/training/tensor_net/test_tensor_net.py
--rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/rdkit/integration/training/tensor_net/test_tensor_net_energy_charges.py
--rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-04-09 10:46:48.000000 physicsml-0.2.3/tests/rdkit/integration/training/tensor_net/test_tensor_net_forces.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.958828 physicsml-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-04-25 13:13:12.000000 physicsml-0.2.4/.envrc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.874827 physicsml-0.2.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.890828 physicsml-0.2.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-25 13:13:12.000000 physicsml-0.2.4/.github/workflows/dev-ci-actions.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-25 13:13:12.000000 physicsml-0.2.4/.github/workflows/docs-build-deploy.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-04-25 13:13:12.000000 physicsml-0.2.4/.github/workflows/latest-tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-25 13:13:12.000000 physicsml-0.2.4/.github/workflows/main-ci-actions.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-04-25 13:13:12.000000 physicsml-0.2.4/.github/workflows/pinned-tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-25 13:13:12.000000 physicsml-0.2.4/.github/workflows/publish-package.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-25 13:13:12.000000 physicsml-0.2.4/.github/workflows/quality-typing-checks.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-25 13:13:12.000000 physicsml-0.2.4/.github/workflows/release-ci-actions.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-25 13:13:12.000000 physicsml-0.2.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-04-25 13:13:12.000000 physicsml-0.2.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-04-25 13:13:12.000000 physicsml-0.2.4/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-25 13:13:12.000000 physicsml-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4594 2024-04-25 13:13:24.958828 physicsml-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-04-25 13:13:12.000000 physicsml-0.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.890828 physicsml-0.2.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-25 13:13:12.000000 physicsml-0.2.4/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-25 13:13:12.000000 physicsml-0.2.4/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.890828 physicsml-0.2.4/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.890828 physicsml-0.2.4/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     3348 2024-04-25 13:13:12.000000 physicsml-0.2.4/docs/source/_static/PhysicsML_Logo-01.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     7381 2024-04-25 13:13:12.000000 physicsml-0.2.4/docs/source/_static/PhysicsML_Logo_PhyML_logo full dark-cropped.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     7503 2024-04-25 13:13:12.000000 physicsml-0.2.4/docs/source/_static/PhysicsML_Logo_PhyML_logo full dark.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     7380 2024-04-25 13:13:12.000000 physicsml-0.2.4/docs/source/_static/PhysicsML_Logo_PhyML_logo full light-cropped.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     7502 2024-04-25 13:13:12.000000 physicsml-0.2.4/docs/source/_static/PhysicsML_Logo_PhyML_logo full light.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     7824 2024-04-25 13:13:12.000000 physicsml-0.2.4/docs/source/_static/PhysicsML_Logo_PhyML_logo text dark.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     7836 2024-04-25 13:13:12.000000 physicsml-0.2.4/docs/source/_static/PhysicsML_Logo_PhyML_logo text light.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-04-25 13:13:12.000000 physicsml-0.2.4/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-04-25 13:13:12.000000 physicsml-0.2.4/docs/source/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.878827 physicsml-0.2.4/docs/source/pages/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.890828 physicsml-0.2.4/docs/source/pages/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)     5631 2024-04-25 13:13:12.000000 physicsml-0.2.4/docs/source/pages/datasets/qm_datasets.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.894828 physicsml-0.2.4/docs/source/pages/features/
+-rw-r--r--   0 runner    (1001) docker     (127)   489710 2024-04-25 13:13:12.000000 physicsml-0.2.4/docs/source/pages/features/gdb9_trunc.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-25 13:13:12.000000 physicsml-0.2.4/docs/source/pages/features/how_to_add_reps.md
+-rw-r--r--   0 runner    (1001) docker     (127)     9303 2024-04-25 13:13:12.000000 physicsml-0.2.4/docs/source/pages/features/intro.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.894828 physicsml-0.2.4/docs/source/pages/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     5234 2024-04-25 13:13:12.000000 physicsml-0.2.4/docs/source/pages/models/allegro.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3805 2024-04-25 13:13:12.000000 physicsml-0.2.4/docs/source/pages/models/ani.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11315 2024-04-25 13:13:12.000000 physicsml-0.2.4/docs/source/pages/models/egnn.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6295 2024-04-25 13:13:12.000000 physicsml-0.2.4/docs/source/pages/models/how_to_add_models.md
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-25 13:13:12.000000 physicsml-0.2.4/docs/source/pages/models/intro.md
+-rw-r--r--   0 runner    (1001) docker     (127)     9091 2024-04-25 13:13:12.000000 physicsml-0.2.4/docs/source/pages/models/mace.md
+-rw-r--r--   0 runner    (1001) docker     (127)     9742 2024-04-25 13:13:12.000000 physicsml-0.2.4/docs/source/pages/models/nequip.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2049 2024-04-25 13:13:12.000000 physicsml-0.2.4/docs/source/pages/models/tensor_net.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.894828 physicsml-0.2.4/docs/source/pages/philosophy/
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-25 13:13:12.000000 physicsml-0.2.4/docs/source/pages/philosophy/molflux.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-04-25 13:13:12.000000 physicsml-0.2.4/docs/source/pages/philosophy/philosophy.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.894828 physicsml-0.2.4/docs/source/pages/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-25 13:13:12.000000 physicsml-0.2.4/docs/source/pages/plugins/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     4578 2024-04-25 13:13:12.000000 physicsml-0.2.4/docs/source/pages/plugins/alanine-dipeptide-truncated.pdb
+-rw-r--r--   0 runner    (1001) docker     (127)     3899 2024-04-25 13:13:12.000000 physicsml-0.2.4/docs/source/pages/plugins/ase.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5335 2024-04-25 13:13:12.000000 physicsml-0.2.4/docs/source/pages/plugins/openmm.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.894828 physicsml-0.2.4/docs/source/pages/structure/
+-rw-r--r--   0 runner    (1001) docker     (127)     7237 2024-04-25 13:13:12.000000 physicsml-0.2.4/docs/source/pages/structure/lightning_layer.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4803 2024-04-25 13:13:12.000000 physicsml-0.2.4/docs/source/pages/structure/molflux_layer.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-25 13:13:12.000000 physicsml-0.2.4/docs/source/pages/structure/physicsml_structure.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6294 2024-04-25 13:13:12.000000 physicsml-0.2.4/docs/source/pages/structure/torch_layer.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2906 2024-04-25 13:13:12.000000 physicsml-0.2.4/docs/source/pages/structure/transfer_learning.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.898828 physicsml-0.2.4/docs/source/pages/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-25 13:13:12.000000 physicsml-0.2.4/docs/source/pages/tutorials/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     7462 2024-04-25 13:13:12.000000 physicsml-0.2.4/docs/source/pages/tutorials/ani1x_energy_forces_training.md
+-rw-r--r--   0 runner    (1001) docker     (127)  1610932 2024-04-25 13:13:12.000000 physicsml-0.2.4/docs/source/pages/tutorials/ani1x_truncated.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     9729 2024-04-25 13:13:12.000000 physicsml-0.2.4/docs/source/pages/tutorials/gdb9_training.md
+-rw-r--r--   0 runner    (1001) docker     (127)   489710 2024-04-25 13:13:12.000000 physicsml-0.2.4/docs/source/pages/tutorials/gdb9_trunc.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     7678 2024-04-25 13:13:12.000000 physicsml-0.2.4/docs/source/pages/tutorials/gdb9_uncertainty.md
+-rw-r--r--   0 runner    (1001) docker     (127)    10605 2024-04-25 13:13:12.000000 physicsml-0.2.4/docs/source/pages/tutorials/transfer_learning.md
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-25 13:13:12.000000 physicsml-0.2.4/environment.yml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1053 2024-04-25 13:13:12.000000 physicsml-0.2.4/init_conda_venv.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      714 2024-04-25 13:13:12.000000 physicsml-0.2.4/init_python_venv.sh
+-rw-r--r--   0 runner    (1001) docker     (127)    12177 2024-04-25 13:13:12.000000 physicsml-0.2.4/noxfile.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.878827 physicsml-0.2.4/pinned-versions/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.902828 physicsml-0.2.4/pinned-versions/3.10/
+-rw-r--r--   0 runner    (1001) docker     (127)    11832 2024-04-25 13:13:12.000000 physicsml-0.2.4/pinned-versions/3.10/lockfile.ase.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11831 2024-04-25 13:13:12.000000 physicsml-0.2.4/pinned-versions/3.10/lockfile.core.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11900 2024-04-25 13:13:12.000000 physicsml-0.2.4/pinned-versions/3.10/lockfile.openeye.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11835 2024-04-25 13:13:12.000000 physicsml-0.2.4/pinned-versions/3.10/lockfile.openmm.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11834 2024-04-25 13:13:12.000000 physicsml-0.2.4/pinned-versions/3.10/lockfile.rdkit.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.902828 physicsml-0.2.4/pinned-versions/3.11/
+-rw-r--r--   0 runner    (1001) docker     (127)    11639 2024-04-25 13:13:12.000000 physicsml-0.2.4/pinned-versions/3.11/lockfile.ase.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11638 2024-04-25 13:13:12.000000 physicsml-0.2.4/pinned-versions/3.11/lockfile.core.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11707 2024-04-25 13:13:12.000000 physicsml-0.2.4/pinned-versions/3.11/lockfile.openeye.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11642 2024-04-25 13:13:12.000000 physicsml-0.2.4/pinned-versions/3.11/lockfile.openmm.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11641 2024-04-25 13:13:12.000000 physicsml-0.2.4/pinned-versions/3.11/lockfile.rdkit.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.902828 physicsml-0.2.4/pinned-versions/3.8/
+-rw-r--r--   0 runner    (1001) docker     (127)    12188 2024-04-25 13:13:12.000000 physicsml-0.2.4/pinned-versions/3.8/lockfile.ase.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    12187 2024-04-25 13:13:12.000000 physicsml-0.2.4/pinned-versions/3.8/lockfile.core.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    12358 2024-04-25 13:13:12.000000 physicsml-0.2.4/pinned-versions/3.8/lockfile.openeye.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    12191 2024-04-25 13:13:12.000000 physicsml-0.2.4/pinned-versions/3.8/lockfile.openmm.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    12190 2024-04-25 13:13:12.000000 physicsml-0.2.4/pinned-versions/3.8/lockfile.rdkit.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.902828 physicsml-0.2.4/pinned-versions/3.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    11956 2024-04-25 13:13:12.000000 physicsml-0.2.4/pinned-versions/3.9/lockfile.ase.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11955 2024-04-25 13:13:12.000000 physicsml-0.2.4/pinned-versions/3.9/lockfile.core.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    12024 2024-04-25 13:13:12.000000 physicsml-0.2.4/pinned-versions/3.9/lockfile.openeye.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11959 2024-04-25 13:13:12.000000 physicsml-0.2.4/pinned-versions/3.9/lockfile.openmm.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11958 2024-04-25 13:13:12.000000 physicsml-0.2.4/pinned-versions/3.9/lockfile.rdkit.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     7465 2024-04-25 13:13:12.000000 physicsml-0.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 13:13:24.958828 physicsml-0.2.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.878827 physicsml-0.2.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.902828 physicsml-0.2.4/src/physicsml/
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.906828 physicsml-0.2.4/src/physicsml/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2286 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/backends/backend_selector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4970 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/backends/openeye_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4927 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/backends/rdkit_backend.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.906828 physicsml-0.2.4/src/physicsml/featurisation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/featurisation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.906828 physicsml-0.2.4/src/physicsml/featurisation/physicsml_features/
+-rw-r--r--   0 runner    (1001) docker     (127)     4246 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/featurisation/physicsml_features/atom_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/featurisation/physicsml_features/bond_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5600 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/featurisation/physicsml_features/physicsml_features.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.906828 physicsml-0.2.4/src/physicsml/lightning/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/lightning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3569 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/lightning/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5705 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/lightning/datamodule.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.906828 physicsml-0.2.4/src/physicsml/lightning/graph_datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/lightning/graph_datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13126 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/lightning/graph_datasets/graph_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6038 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/lightning/graph_datasets/neighbourhood_list_torch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.910828 physicsml-0.2.4/src/physicsml/lightning/graph_datasets/torch_nl_vendored/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/lightning/graph_datasets/torch_nl_vendored/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/lightning/graph_datasets/torch_nl_vendored/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12716 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/lightning/graph_datasets/torch_nl_vendored/linked_cell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2482 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/lightning/graph_datasets/torch_nl_vendored/naive_impl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5236 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/lightning/graph_datasets/torch_nl_vendored/neighbor_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/lightning/graph_datasets/torch_nl_vendored/timer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/lightning/graph_datasets/torch_nl_vendored/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.910828 physicsml-0.2.4/src/physicsml/lightning/losses/
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/lightning/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10118 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/lightning/losses/barlow_twins_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/lightning/losses/construct_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/lightning/losses/loss_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/lightning/losses/masked_mse_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/lightning/losses/multitask_losses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/lightning/losses/serial_bce_w_logits_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/lightning/losses/stock_losses.py
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/lightning/losses/weighted_mse_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4642 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/lightning/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6462 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/lightning/model_uncertainty.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6630 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/lightning/module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/lightning/pre_batching_in_memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/lightning/pre_batching_on_disk.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.910828 physicsml-0.2.4/src/physicsml/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.910828 physicsml-0.2.4/src/physicsml/models/allegro/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/allegro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4108 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/allegro/allegro_prism.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.914828 physicsml-0.2.4/src/physicsml/models/allegro/mean_var/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/allegro/mean_var/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/allegro/mean_var/default_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/allegro/mean_var/mean_var_allegro_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6496 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/allegro/mean_var/mean_var_allegro_module.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.914828 physicsml-0.2.4/src/physicsml/models/allegro/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/allegro/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24182 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/allegro/modules/allegro.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/allegro/modules/channels.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15463 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/allegro/modules/contract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/allegro/modules/cutoffs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5427 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/allegro/modules/fc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2759 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/allegro/modules/layout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8447 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/allegro/modules/linear.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3696 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/allegro/modules/radial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5406 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/allegro/modules/spmm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.914828 physicsml-0.2.4/src/physicsml/models/allegro/supervised/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/allegro/supervised/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/allegro/supervised/allegro_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5639 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/allegro/supervised/allegro_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/allegro/supervised/default_configs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.914828 physicsml-0.2.4/src/physicsml/models/ani/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/ani/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4619 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/ani/ani_1_2_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5150 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/ani/ani_datamodule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5859 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/ani/ani_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2826 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/ani/ani_prism.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2688 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/ani/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.918828 physicsml-0.2.4/src/physicsml/models/ani/ensemble/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/ani/ensemble/default_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/ani/ensemble/ensemble_ani_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9790 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/ani/ensemble/ensemble_ani_module.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.918828 physicsml-0.2.4/src/physicsml/models/ani/mean_var/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/ani/mean_var/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/ani/mean_var/default_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/ani/mean_var/mean_var_ani_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8991 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/ani/mean_var/mean_var_ani_module.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.918828 physicsml-0.2.4/src/physicsml/models/ani/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/ani/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27070 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/ani/modules/aev.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.918828 physicsml-0.2.4/src/physicsml/models/ani/supervised/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/ani/supervised/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/ani/supervised/ani_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8431 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/ani/supervised/ani_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/ani/supervised/default_configs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.918828 physicsml-0.2.4/src/physicsml/models/egnn/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/egnn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.918828 physicsml-0.2.4/src/physicsml/models/egnn/adapter/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/egnn/adapter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/egnn/adapter/adapter_egnn_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6317 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/egnn/adapter/adapter_egnn_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6599 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/egnn/adapter/adapter_egnn_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/egnn/adapter/default_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4251 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/egnn/egnn_prism.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15452 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/egnn/egnn_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.922828 physicsml-0.2.4/src/physicsml/models/egnn/mean_var/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/egnn/mean_var/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/egnn/mean_var/default_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/egnn/mean_var/mean_var_egnn_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6987 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/egnn/mean_var/mean_var_egnn_module.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.922828 physicsml-0.2.4/src/physicsml/models/egnn/ssf/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/egnn/ssf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/egnn/ssf/default_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/egnn/ssf/ssf_egnn_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6159 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/egnn/ssf/ssf_egnn_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3689 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/egnn/ssf/ssf_egnn_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.922828 physicsml-0.2.4/src/physicsml/models/egnn/supervised/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/egnn/supervised/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/egnn/supervised/default_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/egnn/supervised/egnn_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6308 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/egnn/supervised/egnn_module.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.922828 physicsml-0.2.4/src/physicsml/models/mace/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/mace/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.922828 physicsml-0.2.4/src/physicsml/models/mace/adapter/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/mace/adapter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/mace/adapter/adapter_mace_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8422 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/mace/adapter/adapter_mace_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8480 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/mace/adapter/adapter_mace_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/mace/adapter/default_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4194 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/mace/mace_prism.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.922828 physicsml-0.2.4/src/physicsml/models/mace/mean_var/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/mace/mean_var/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/mace/mean_var/default_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/mace/mean_var/mean_var_mace_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8887 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/mace/mean_var/mean_var_mace_module.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.926828 physicsml-0.2.4/src/physicsml/models/mace/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/mace/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3773 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/mace/modules/_activation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8255 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/mace/modules/blocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4377 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/mace/modules/cg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/mace/modules/irreps_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8507 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/mace/modules/mace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/mace/modules/radial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9635 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/mace/modules/symmetric_contraction.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.926828 physicsml-0.2.4/src/physicsml/models/mace/ssf/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/mace/ssf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/mace/ssf/default_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/mace/ssf/ssf_mace_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8236 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/mace/ssf/ssf_mace_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6820 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/mace/ssf/ssf_mace_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.926828 physicsml-0.2.4/src/physicsml/models/mace/supervised/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/mace/supervised/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/mace/supervised/default_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/mace/supervised/mace_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8133 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/mace/supervised/mace_module.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.926828 physicsml-0.2.4/src/physicsml/models/nequip/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/nequip/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.926828 physicsml-0.2.4/src/physicsml/models/nequip/adapter/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/nequip/adapter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/nequip/adapter/adapter_nequip_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6696 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/nequip/adapter/adapter_nequip_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7075 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/nequip/adapter/adapter_nequip_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/nequip/adapter/default_configs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.930828 physicsml-0.2.4/src/physicsml/models/nequip/mean_var/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/nequip/mean_var/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/nequip/mean_var/default_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/nequip/mean_var/mean_var_nequip_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7196 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/nequip/mean_var/mean_var_nequip_module.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.930828 physicsml-0.2.4/src/physicsml/models/nequip/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/nequip/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3773 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/nequip/modules/_activation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5727 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/nequip/modules/_gate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3466 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/nequip/modules/convnet_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3683 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/nequip/modules/interaction_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5968 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/nequip/modules/nequip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/nequip/modules/radial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/nequip/modules/scale_shift.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4494 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/nequip/nequip_prism.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.930828 physicsml-0.2.4/src/physicsml/models/nequip/ssf/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/nequip/ssf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/nequip/ssf/default_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/nequip/ssf/ssf_nequip_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6522 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/nequip/ssf/ssf_nequip_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5306 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/nequip/ssf/ssf_nequip_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.930828 physicsml-0.2.4/src/physicsml/models/nequip/supervised/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/nequip/supervised/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/nequip/supervised/default_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/nequip/supervised/nequip_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6431 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/nequip/supervised/nequip_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4990 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/prism.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.930828 physicsml-0.2.4/src/physicsml/models/tensor_net/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/tensor_net/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.934828 physicsml-0.2.4/src/physicsml/models/tensor_net/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/tensor_net/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7351 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/tensor_net/modules/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3621 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/tensor_net/modules/interaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/tensor_net/modules/output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3279 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/tensor_net/modules/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.934828 physicsml-0.2.4/src/physicsml/models/tensor_net/supervised/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/tensor_net/supervised/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/tensor_net/supervised/default_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/tensor_net/supervised/tensor_net_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4882 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/tensor_net/supervised/tensor_net_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3593 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/models/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.934828 physicsml-0.2.4/src/physicsml/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.934828 physicsml-0.2.4/src/physicsml/plugins/ase/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/plugins/ase/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/plugins/ase/ase_ani.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/plugins/ase/ase_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3717 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/plugins/ase/calculator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/plugins/ase/load.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.934828 physicsml-0.2.4/src/physicsml/plugins/openmm/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/plugins/openmm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/plugins/openmm/load.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/plugins/openmm/openmm_ani.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4571 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/plugins/openmm/openmm_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6285 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/plugins/openmm/openmm_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5370 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/plugins/openmm/physicsml_potential.py
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     3130 2024-04-25 13:13:12.000000 physicsml-0.2.4/src/physicsml/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-25 13:13:24.000000 physicsml-0.2.4/src/physicsml/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.954828 physicsml-0.2.4/src/physicsml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4594 2024-04-25 13:13:24.000000 physicsml-0.2.4/src/physicsml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    16518 2024-04-25 13:13:24.000000 physicsml-0.2.4/src/physicsml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 13:13:24.000000 physicsml-0.2.4/src/physicsml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-04-25 13:13:24.000000 physicsml-0.2.4/src/physicsml.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-04-25 13:13:24.000000 physicsml-0.2.4/src/physicsml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-25 13:13:24.000000 physicsml-0.2.4/src/physicsml.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.934828 physicsml-0.2.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.938828 physicsml-0.2.4/tests/ase/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/ase/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9983 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/ase/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/ase/test_ase_ani.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2865 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/ase/test_ase_graph.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.938828 physicsml-0.2.4/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     4578 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/data/alanine-dipeptide-truncated.pdb
+-rw-r--r--   0 runner    (1001) docker     (127)   698696 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/data/ani1x.h5
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.938828 physicsml-0.2.4/tests/data/ani_model/
+-rw-r--r--   0 runner    (1001) docker     (127)     5795 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/data/ani_model/featurisation_metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.938828 physicsml-0.2.4/tests/data/ani_model/model_artefacts/
+-rw-r--r--   0 runner    (1001) docker     (127)  1320280 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/data/ani_model/model_artefacts/module_checkpoint.ckpt
+-rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/data/ani_model/model_config.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.942828 physicsml-0.2.4/tests/data/egnn_model/
+-rw-r--r--   0 runner    (1001) docker     (127)     5795 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/data/egnn_model/featurisation_metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.942828 physicsml-0.2.4/tests/data/egnn_model/model_artefacts/
+-rw-r--r--   0 runner    (1001) docker     (127)    52081 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/data/egnn_model/model_artefacts/module_checkpoint.ckpt
+-rw-r--r--   0 runner    (1001) docker     (127)     3496 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/data/egnn_model/model_config.json
+-rw-r--r--   0 runner    (1001) docker     (127)    20277 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/data/gdb9.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    98022 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/data/gdb9.sdf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.942828 physicsml-0.2.4/tests/data/mace_model/
+-rw-r--r--   0 runner    (1001) docker     (127)     5795 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/data/mace_model/featurisation_metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.942828 physicsml-0.2.4/tests/data/mace_model/model_artefacts/
+-rw-r--r--   0 runner    (1001) docker     (127)   117170 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/data/mace_model/model_artefacts/module_checkpoint.ckpt
+-rw-r--r--   0 runner    (1001) docker     (127)     3433 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/data/mace_model/model_config.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.942828 physicsml-0.2.4/tests/data/nequip_model/
+-rw-r--r--   0 runner    (1001) docker     (127)     5795 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/data/nequip_model/featurisation_metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.942828 physicsml-0.2.4/tests/data/nequip_model/model_artefacts/
+-rw-r--r--   0 runner    (1001) docker     (127)    86167 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/data/nequip_model/model_artefacts/module_checkpoint.ckpt
+-rw-r--r--   0 runner    (1001) docker     (127)     3501 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/data/nequip_model/model_config.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.942828 physicsml-0.2.4/tests/openeye/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/openeye/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9987 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/openeye/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.942828 physicsml-0.2.4/tests/openeye/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/openeye/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.942828 physicsml-0.2.4/tests/openeye/core/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/openeye/core/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/openeye/core/data/test_datamodule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6036 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/openeye/core/data/test_graph_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.946828 physicsml-0.2.4/tests/openeye/core/featurisation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/openeye/core/featurisation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4999 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/openeye/core/featurisation/test_physicsml_featurisation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.946828 physicsml-0.2.4/tests/openeye/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/openeye/integration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.946828 physicsml-0.2.4/tests/openeye/integration/prism/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/openeye/integration/prism/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3258 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/openeye/integration/prism/test_egnn_prism.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.946828 physicsml-0.2.4/tests/openeye/integration/training/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/openeye/integration/training/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.946828 physicsml-0.2.4/tests/openeye/integration/training/egnn/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/openeye/integration/training/egnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/openeye/integration/training/egnn/test_egnn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.946828 physicsml-0.2.4/tests/openmm/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/openmm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9942 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/openmm/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10818 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/openmm/test_openmm_ani.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16225 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/openmm/test_openmm_egnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16422 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/openmm/test_openmm_mace.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16903 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/openmm/test_openmm_nequip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7399 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/openmm/test_openmm_nnp_potential.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.946828 physicsml-0.2.4/tests/rdkit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/rdkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9982 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/rdkit/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.946828 physicsml-0.2.4/tests/rdkit/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/rdkit/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.946828 physicsml-0.2.4/tests/rdkit/core/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/rdkit/core/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/rdkit/core/data/test_datamodule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6036 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/rdkit/core/data/test_graph_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.946828 physicsml-0.2.4/tests/rdkit/core/featurisation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/rdkit/core/featurisation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4978 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/rdkit/core/featurisation/test_physicsml_featurisation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.950828 physicsml-0.2.4/tests/rdkit/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/rdkit/integration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.950828 physicsml-0.2.4/tests/rdkit/integration/prism/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/rdkit/integration/prism/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3573 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/rdkit/integration/prism/test_allegro_prism.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2966 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/rdkit/integration/prism/test_ani_prism.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3258 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/rdkit/integration/prism/test_egnn_prism.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3346 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/rdkit/integration/prism/test_mace_prism.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/rdkit/integration/prism/test_nequip_prism.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.950828 physicsml-0.2.4/tests/rdkit/integration/training/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/rdkit/integration/training/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.950828 physicsml-0.2.4/tests/rdkit/integration/training/allegro/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/rdkit/integration/training/allegro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/rdkit/integration/training/allegro/test_allegro_energy_charges.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/rdkit/integration/training/allegro/test_allegro_forces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3375 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/rdkit/integration/training/allegro/test_allegro_mean_var.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/rdkit/integration/training/allegro/test_allergo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.950828 physicsml-0.2.4/tests/rdkit/integration/training/ani/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/rdkit/integration/training/ani/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/rdkit/integration/training/ani/test_ani.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2877 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/rdkit/integration/training/ani/test_ani_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/rdkit/integration/training/ani/test_ani_forces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2724 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/rdkit/integration/training/ani/test_ani_mean_var.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.954828 physicsml-0.2.4/tests/rdkit/integration/training/egnn/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/rdkit/integration/training/egnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2075 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/rdkit/integration/training/egnn/test_adapter_egnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/rdkit/integration/training/egnn/test_egnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/rdkit/integration/training/egnn/test_egnn_energy_charges.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2343 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/rdkit/integration/training/egnn/test_egnn_forces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3024 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/rdkit/integration/training/egnn/test_egnn_mean_var.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/rdkit/integration/training/egnn/test_ssf_egnn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.954828 physicsml-0.2.4/tests/rdkit/integration/training/mace/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/rdkit/integration/training/mace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2165 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/rdkit/integration/training/mace/test_adapter_mace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/rdkit/integration/training/mace/test_mace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2985 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/rdkit/integration/training/mace/test_mace_energy_charges.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/rdkit/integration/training/mace/test_mace_forces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3081 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/rdkit/integration/training/mace/test_mace_mean_var.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/rdkit/integration/training/mace/test_ssf_mace.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.954828 physicsml-0.2.4/tests/rdkit/integration/training/nequip/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/rdkit/integration/training/nequip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/rdkit/integration/training/nequip/test_adapter_nequip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2121 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/rdkit/integration/training/nequip/test_nequip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3089 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/rdkit/integration/training/nequip/test_nequip_energy_charges.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/rdkit/integration/training/nequip/test_nequip_forces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3248 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/rdkit/integration/training/nequip/test_nequip_mean_var.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/rdkit/integration/training/nequip/test_ssf_nequip.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:24.954828 physicsml-0.2.4/tests/rdkit/integration/training/tensor_net/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/rdkit/integration/training/tensor_net/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/rdkit/integration/training/tensor_net/test_tensor_net.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/rdkit/integration/training/tensor_net/test_tensor_net_energy_charges.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-04-25 13:13:12.000000 physicsml-0.2.4/tests/rdkit/integration/training/tensor_net/test_tensor_net_forces.py
```

### Comparing `physicsml-0.2.3/.envrc` & `physicsml-0.2.4/.envrc`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/.github/workflows/docs-build-deploy.yaml` & `physicsml-0.2.4/.github/workflows/docs-build-deploy.yaml`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/.github/workflows/latest-tests.yaml` & `physicsml-0.2.4/.github/workflows/latest-tests.yaml`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/.github/workflows/pinned-tests.yaml` & `physicsml-0.2.4/.github/workflows/pinned-tests.yaml`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/.github/workflows/publish-package.yaml` & `physicsml-0.2.4/.github/workflows/publish-package.yaml`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/.github/workflows/quality-typing-checks.yaml` & `physicsml-0.2.4/.github/workflows/quality-typing-checks.yaml`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/.gitignore` & `physicsml-0.2.4/.gitignore`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/.pre-commit-config.yaml` & `physicsml-0.2.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/CHANGELOG.md` & `physicsml-0.2.4/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,26 @@
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/), and this project
 adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 ---------------------------------------------------------
 
 ## [Unreleased]
 
 ---------------------------------------------------------
+ ## [0.2.4] - 2024-04-24
+
+### Fixed
+
+* Added coordinate wrapping in the neighbour list computations of ANI and graphs
+
+## [0.2.3] - 2024-04-09
+
+## Changed
+
+* Remove torch < 2.1 pin
+
 ## [0.2.2] - 2024-04-05
 
 ## Fixed
 
 * Fixed problem with openmm precision (force cast positions to model dtype)
 
 ## [0.2.1] - 2024-04-03
```

### Comparing `physicsml-0.2.3/LICENSE` & `physicsml-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/PKG-INFO` & `physicsml-0.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: physicsml
-Version: 0.2.3
+Version: 0.2.4
 Summary: A package for all physics based/related models
 Author: Exscientia
 Maintainer: Exscientia
 Project-URL: documentation, https://github.com/exscientia/physicsml/issues
 Project-URL: repository, https://github.com/exscientia/physicsml.git
 Project-URL: issue-tracker, https://github.com/exscientia/physicsml/issues
 Project-URL: changelog, https://github.com/exscientia/physicsml/src/main/CHANGELOG.md
@@ -19,21 +19,19 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: molflux
-Requires-Dist: torch<2.1,>=2.0
+Requires-Dist: torch>=2.0
 Requires-Dist: lightning>=2.1
 Requires-Dist: torch-geometric>=2.5.0
-Requires-Dist: torch-nl
 Requires-Dist: e3nn
 Requires-Dist: torchani!=2.2.4
-Requires-Dist: tensorboard
 Provides-Extra: openeye
 Requires-Dist: openeye-toolkits<2023.0.0; python_version == "3.8" and extra == "openeye"
 Requires-Dist: openeye-toolkits; extra == "openeye"
 Provides-Extra: rdkit
 Requires-Dist: rdkit; extra == "rdkit"
 Provides-Extra: ase
 Requires-Dist: rdkit; extra == "ase"
```

### Comparing `physicsml-0.2.3/README.md` & `physicsml-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/docs/Makefile` & `physicsml-0.2.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/docs/make.bat` & `physicsml-0.2.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/docs/source/_static/PhysicsML_Logo-01.svg` & `physicsml-0.2.4/docs/source/_static/PhysicsML_Logo-01.svg`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/docs/source/_static/PhysicsML_Logo_PhyML_logo full dark-cropped.svg` & `physicsml-0.2.4/docs/source/_static/PhysicsML_Logo_PhyML_logo full dark-cropped.svg`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/docs/source/_static/PhysicsML_Logo_PhyML_logo full dark.svg` & `physicsml-0.2.4/docs/source/_static/PhysicsML_Logo_PhyML_logo full dark.svg`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/docs/source/_static/PhysicsML_Logo_PhyML_logo full light-cropped.svg` & `physicsml-0.2.4/docs/source/_static/PhysicsML_Logo_PhyML_logo full light-cropped.svg`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/docs/source/_static/PhysicsML_Logo_PhyML_logo full light.svg` & `physicsml-0.2.4/docs/source/_static/PhysicsML_Logo_PhyML_logo full light.svg`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/docs/source/_static/PhysicsML_Logo_PhyML_logo text dark.svg` & `physicsml-0.2.4/docs/source/_static/PhysicsML_Logo_PhyML_logo text dark.svg`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/docs/source/_static/PhysicsML_Logo_PhyML_logo text light.svg` & `physicsml-0.2.4/docs/source/_static/PhysicsML_Logo_PhyML_logo text light.svg`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/docs/source/conf.py` & `physicsml-0.2.4/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/docs/source/index.md` & `physicsml-0.2.4/docs/source/index.md`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/docs/source/pages/datasets/qm_datasets.md` & `physicsml-0.2.4/docs/source/pages/datasets/qm_datasets.md`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/docs/source/pages/features/gdb9_trunc.parquet` & `physicsml-0.2.4/docs/source/pages/features/gdb9_trunc.parquet`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/docs/source/pages/features/how_to_add_reps.md` & `physicsml-0.2.4/docs/source/pages/features/how_to_add_reps.md`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/docs/source/pages/features/intro.md` & `physicsml-0.2.4/docs/source/pages/features/intro.md`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/docs/source/pages/models/allegro.md` & `physicsml-0.2.4/docs/source/pages/models/allegro.md`

 * *Files 12% similar despite different names*

```diff
@@ -54,19 +54,18 @@
 
     Whether to embed the initial edge features.
 * ``latent_resnet: bool = True``
 
     Whether to use a latent resnet.
 * ``scaling_mean: float = 0.0``
 
-    The scaling mean of the output predictions
+    The scaling mean of the model output. This is usually computed as the mean of `(molecule_energy - molecule_self_energy) / molecule_num_atoms`
 * ``scaling_std: float = 1.0``
 
-    The scaling std of the output predictions.
-
+    The scaling std of the model output. This is usually computed as the std of `(molecule_energy - molecule_self_energy)`
 * ``compute_forces: bool = False``
 
     Whether to compute forces as the gradient of the ``y_graph_scalars`` and use those as the ``y_node_vector`` output.
 * ``y_node_scalars_loss_config: Optional[Dict] = None``
 
     The loss config for the ``y_node_scalars``.
 * ``y_node_vector_loss_config: Optional[Dict] = None``
@@ -130,19 +129,18 @@
 
     Whether to embed the initial edge features.
 * ``latent_resnet: bool = True``
 
     Whether to use a latent resnet.
 * ``scaling_mean: float = 0.0``
 
-    The scaling mean of the output predictions
+    The scaling mean of the model output. This is usually computed as the mean of `(molecule_energy - molecule_self_energy) / molecule_num_atoms`
 * ``scaling_std: float = 1.0``
 
-    The scaling std of the output predictions.
-
+    The scaling std of the model output. This is usually computed as the std of `(molecule_energy - molecule_self_energy)`
 * ``compute_forces: bool = False``
 
     Whether to compute forces as the gradient of the ``y_graph_scalars`` and use those as the ``y_node_vector`` output.
 * ``y_node_scalars_loss_config: Optional[Dict] = None``
 
     The loss config for the ``y_node_scalars``.
 * ``y_node_vector_loss_config: Optional[Dict] = None``
```

### Comparing `physicsml-0.2.3/docs/source/pages/models/ani.md` & `physicsml-0.2.4/docs/source/pages/models/ani.md`

 * *Files 12% similar despite different names*

```diff
@@ -13,18 +13,18 @@
 
     The ANI model to use.
     * ``"ani1"`` is for H, C, N, O
     * ``"ani2"`` is for H, C, N, O, S, F, Cl
     * ``"ani_spice"`` is for H, C, N, O, F, P, S, Cl, Br, I
 * ``scaling_mean: float = 0.0``
 
-    The scaling mean for the output predictions.
+    The scaling mean of the model output. This is usually computed as the mean of `(molecule_energy - molecule_self_energy)`
 * ``scaling_std: float = 1.0``
 
-    The scaling std for the output predictions
+    The scaling std of the model output. This is usually computed as the std of `(molecule_energy - molecule_self_energy)`
 * ``compute_forces: bool = False``
 
     Whether to compute forces as the gradient of the ``y_graph_scalars`` and use those as the ``y_node_vector`` output.
 * ``y_graph_scalars_loss_config: Optional[Dict] = None``
 
     The loss config for the ``y_graph_scalars``.
 * ``y_node_vector_loss_config: Optional[Dict] = None``
@@ -43,18 +43,18 @@
 
     The ANI model to use.
     * ``"ani1"`` is for H, C, N, O
     * ``"ani2"`` is for H, C, N, O, S, F, Cl
     * ``"ani_spice"`` is for H, C, N, O, F, P, S, Cl, Br, I
 * ``scaling_mean: float = 0.0``
 
-    The scaling mean for the output predictions.
+    The scaling mean of the model output. This is usually computed as the mean of `(molecule_energy - molecule_self_energy)`
 * ``scaling_std: float = 1.0``
 
-    The scaling std for the output predictions
+    The scaling std of the model output. This is usually computed as the std of `(molecule_energy - molecule_self_energy)`
 * ``compute_forces: bool = False``
 
     Whether to compute forces as the gradient of the ``y_graph_scalars`` and use those as the ``y_node_vector`` output.
 * ``y_node_vector_loss_config: Optional[Dict] = None``
 
     The loss config for the ``y_node_vector``.
 ```
@@ -72,18 +72,18 @@
     * ``"ani2"`` is for H, C, N, O, S, F, Cl
     * ``"ani_spice"`` is for H, C, N, O, F, P, S, Cl, Br, I
 * ``n_models: int = 4``
 
     The number of models in the ensemble.
 * ``scaling_mean: float = 0.0``
 
-    The scaling mean for the output predictions.
+    The scaling mean of the model output. This is usually computed as the mean of `(molecule_energy - molecule_self_energy)`
 * ``scaling_std: float = 1.0``
 
-    The scaling std for the output predictions
+    The scaling std of the model output. This is usually computed as the std of `(molecule_energy - molecule_self_energy)`
 * ``compute_forces: bool = False``
 
     Whether to compute forces as the gradient of the ``y_graph_scalars`` and use those as the ``y_node_vector`` output.
 * ``y_graph_scalars_loss_config: Optional[Dict] = None``
 
     The loss config for the ``y_graph_scalars``.
 * ``y_node_vector_loss_config: Optional[Dict] = None``
```

### Comparing `physicsml-0.2.3/docs/source/pages/models/egnn.md` & `physicsml-0.2.4/docs/source/pages/models/egnn.md`

 * *Files 8% similar despite different names*

```diff
@@ -52,18 +52,18 @@
 
     The activation function of the MLP outputs.
 * ``output_activation: Optional[str] = None``
 
     The activation function of the model output.
 * ``scaling_mean: float = 0.0``
 
-    The scaling mean of the model output.
+    The scaling mean of the model output. This is usually computed as the mean of `(molecule_energy - molecule_self_energy)`
 * ``scaling_std: float = 1.0``
 
-    The scaling std of the model output.
+    The scaling std of the model output. This is usually computed as the std of `(molecule_energy - molecule_self_energy)`
 * ``compute_forces: bool = False``
 
     Whether to compute forces as the gradient of the ``y_graph_scalars`` and use those as the ``y_node_vector`` output.
 * ``y_node_scalars_loss_config: Optional[Dict] = None``
 
     The loss config for the ``y_node_scalars``.
 * ``y_node_vector_loss_config: Optional[Dict] = None``
@@ -127,18 +127,18 @@
 
     The activation function of the MLP outputs.
 * ``output_activation: Optional[str] = None``
 
     The activation function of the model output.
 * ``scaling_mean: float = 0.0``
 
-    The scaling mean of the model output.
+    The scaling mean of the model output. This is usually computed as the mean of `(molecule_energy - molecule_self_energy)`
 * ``scaling_std: float = 1.0``
 
-    The scaling std of the model output.
+    The scaling std of the model output. This is usually computed as the std of `(molecule_energy - molecule_self_energy)`
 * ``compute_forces: bool = False``
 
     Whether to compute forces as the gradient of the ``y_graph_scalars`` and use those as the ``y_node_vector`` output.
 * ``y_node_scalars_loss_config: Optional[Dict] = None``
 
     The loss config for the ``y_node_scalars``.
 * ``y_node_vector_loss_config: Optional[Dict] = None``
@@ -199,18 +199,18 @@
 
     The activation function of the MLP outputs.
 * ``output_activation: Optional[str] = None``
 
     The activation function of the model output.
 * ``scaling_mean: float = 0.0``
 
-    The scaling mean of the model output.
+    The scaling mean of the model output. This is usually computed as the mean of `(molecule_energy - molecule_self_energy)`
 * ``scaling_std: float = 1.0``
 
-    The scaling std of the model output.
+    The scaling std of the model output. This is usually computed as the std of `(molecule_energy - molecule_self_energy)`
 * ``compute_forces: bool = False``
 
     Whether to compute forces as the gradient of the ``y_graph_scalars`` and use those as the ``y_node_vector`` output.
 * ``y_node_scalars_loss_config: Optional[Dict] = None``
 
     The loss config for the ``y_node_scalars``.
 * ``y_node_vector_loss_config: Optional[Dict] = None``
@@ -281,18 +281,18 @@
 
     The activation function of the MLP outputs.
 * ``output_activation: Optional[str] = None``
 
     The activation function of the model output.
 * ``scaling_mean: float = 0.0``
 
-    The scaling mean of the model output.
+    The scaling mean of the model output. This is usually computed as the mean of `(molecule_energy - molecule_self_energy)`
 * ``scaling_std: float = 1.0``
 
-    The scaling std of the model output.
+    The scaling std of the model output. This is usually computed as the std of `(molecule_energy - molecule_self_energy)`
 * ``compute_forces: bool = False``
 
     Whether to compute forces as the gradient of the ``y_graph_scalars`` and use those as the ``y_node_vector`` output.
 * ``y_node_scalars_loss_config: Optional[Dict] = None``
 
     The loss config for the ``y_node_scalars``.
 * ``y_node_vector_loss_config: Optional[Dict] = None``
```

### Comparing `physicsml-0.2.3/docs/source/pages/models/how_to_add_models.md` & `physicsml-0.2.4/docs/source/pages/models/how_to_add_models.md`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/docs/source/pages/models/intro.md` & `physicsml-0.2.4/docs/source/pages/models/intro.md`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/docs/source/pages/models/mace.md` & `physicsml-0.2.4/docs/source/pages/models/mace.md`

 * *Files 12% similar despite different names*

```diff
@@ -37,18 +37,18 @@
 
     The average number of neighbours in the dataset
 * ``correlation: int = 3``
 
     The highest correlation order.
 * ``scaling_mean: float = 0.0``
 
-    The scaling mean of the model output.
+    The scaling mean of the model output. This is usually computed as the mean of `(molecule_energy - molecule_self_energy) / molecule_num_atoms`
 * ``scaling_std: float = 1.0``
 
-    The scaling std of the model output.
+    The scaling std of the model output. This is usually computed as the std of `(molecule_energy - molecule_self_energy)`
 * ``compute_forces: bool = False``
 
     Whether to compute forces as the gradient of the ``y_graph_scalars`` and use those as the ``y_node_vector`` output.
 * ``y_node_scalars_loss_config: Optional[Dict] = None``
 
     The loss config for the ``y_node_scalars``.
 * ``y_node_vector_loss_config: Optional[Dict] = None``
@@ -97,18 +97,18 @@
 
     The average number of neighbours in the dataset
 * ``correlation: int = 3``
 
     The highest correlation order.
 * ``scaling_mean: float = 0.0``
 
-    The scaling mean of the model output.
+    The scaling mean of the model output. This is usually computed as the mean of `(molecule_energy - molecule_self_energy) / molecule_num_atoms`
 * ``scaling_std: float = 1.0``
 
-    The scaling std of the model output.
+    The scaling std of the model output. This is usually computed as the std of `(molecule_energy - molecule_self_energy)`
 * ``compute_forces: bool = False``
 
     Whether to compute forces as the gradient of the ``y_graph_scalars`` and use those as the ``y_node_vector`` output.
 * ``y_node_scalars_loss_config: Optional[Dict] = None``
 
     The loss config for the ``y_node_scalars``.
 * ``y_node_vector_loss_config: Optional[Dict] = None``
@@ -154,18 +154,18 @@
 
     The average number of neighbours in the dataset
 * ``correlation: int = 3``
 
     The highest correlation order.
 * ``scaling_mean: float = 0.0``
 
-    The scaling mean of the model output.
+    The scaling mean of the model output. This is usually computed as the mean of `(molecule_energy - molecule_self_energy) / molecule_num_atoms`
 * ``scaling_std: float = 1.0``
 
-    The scaling std of the model output.
+    The scaling std of the model output. This is usually computed as the std of `(molecule_energy - molecule_self_energy)`
 * ``compute_forces: bool = False``
 
     Whether to compute forces as the gradient of the ``y_graph_scalars`` and use those as the ``y_node_vector`` output.
 * ``y_node_scalars_loss_config: Optional[Dict] = None``
 
     The loss config for the ``y_node_scalars``.
 * ``y_node_vector_loss_config: Optional[Dict] = None``
@@ -221,18 +221,18 @@
 
     The ratio of the down layer in the adapters.
 * ``initial_s: float = 0.01``
 
     The starting value of the s parameter for combining the outputs from the adapters and the message passing backbone.
 * ``scaling_mean: float = 0.0``
 
-    The scaling mean of the model output.
+    The scaling mean of the model output. This is usually computed as the mean of `(molecule_energy - molecule_self_energy) / molecule_num_atoms`
 * ``scaling_std: float = 1.0``
 
-    The scaling std of the model output.
+    The scaling std of the model output. This is usually computed as the std of `(molecule_energy - molecule_self_energy)`
 * ``compute_forces: bool = False``
 
     Whether to compute forces as the gradient of the ``y_graph_scalars`` and use those as the ``y_node_vector`` output.
 * ``y_node_scalars_loss_config: Optional[Dict] = None``
 
     The loss config for the ``y_node_scalars``.
 * ``y_node_vector_loss_config: Optional[Dict] = None``
```

### Comparing `physicsml-0.2.3/docs/source/pages/models/nequip.md` & `physicsml-0.2.4/docs/source/pages/models/nequip.md`

 * *Files 13% similar despite different names*

```diff
@@ -45,18 +45,18 @@
 
     Whether to use a resnet.
 * ``avg_num_neighbours: Optional[float] = None``
 
     The average number of neighbours in the dataset.
 * ``scaling_mean: float = 0.0``
 
-    The scaling mean of the model output.
+    The scaling mean of the model output. This is usually computed as the mean of `(molecule_energy - molecule_self_energy) / molecule_num_atoms`
 * ``scaling_std: float = 1.0``
 
-    The scaling std of the model output.
+    The scaling std of the model output. This is usually computed as the std of `(molecule_energy - molecule_self_energy)`
 * ``compute_forces: bool = False``
 
     Whether to compute forces as the gradient of the ``y_graph_scalars`` and use those as the ``y_node_vector`` output.
 * ``y_node_scalars_loss_config: Optional[Dict] = None``
 
     The loss config for the ``y_node_scalars``.
 * ``y_node_vector_loss_config: Optional[Dict] = None``
@@ -114,18 +114,18 @@
 
     Whether to use a resnet.
 * ``avg_num_neighbours: Optional[float] = None``
 
     The average number of neighbours in the dataset.
 * ``scaling_mean: float = 0.0``
 
-    The scaling mean of the model output.
+    The scaling mean of the model output. This is usually computed as the mean of `(molecule_energy - molecule_self_energy) / molecule_num_atoms`
 * ``scaling_std: float = 1.0``
 
-    The scaling std of the model output.
+    The scaling std of the model output. This is usually computed as the std of `(molecule_energy - molecule_self_energy)`
 * ``compute_forces: bool = False``
 
     Whether to compute forces as the gradient of the ``y_graph_scalars`` and use those as the ``y_node_vector`` output.
 * ``y_node_scalars_loss_config: Optional[Dict] = None``
 
     The loss config for the ``y_node_scalars``.
 * ``y_node_vector_loss_config: Optional[Dict] = None``
@@ -180,18 +180,18 @@
 
     Whether to use a resnet.
 * ``avg_num_neighbours: Optional[float] = None``
 
     The average number of neighbours in the dataset.
 * ``scaling_mean: float = 0.0``
 
-    The scaling mean of the model output.
+    The scaling mean of the model output. This is usually computed as the mean of `(molecule_energy - molecule_self_energy) / molecule_num_atoms`
 * ``scaling_std: float = 1.0``
 
-    The scaling std of the model output.
+    The scaling std of the model output. This is usually computed as the std of `(molecule_energy - molecule_self_energy)`
 * ``compute_forces: bool = False``
 
     Whether to compute forces as the gradient of the ``y_graph_scalars`` and use those as the ``y_node_vector`` output.
 * ``y_node_scalars_loss_config: Optional[Dict] = None``
 
     The loss config for the ``y_node_scalars``.
 * ``y_node_vector_loss_config: Optional[Dict] = None``
@@ -250,18 +250,18 @@
 
     Whether to use a resnet.
 * ``avg_num_neighbours: Optional[float] = None``
 
     The average number of neighbours in the dataset.
 * ``scaling_mean: float = 0.0``
 
-    The scaling mean of the model output.
+    The scaling mean of the model output. This is usually computed as the mean of `(molecule_energy - molecule_self_energy) / molecule_num_atoms`
 * ``scaling_std: float = 1.0``
 
-    The scaling std of the model output.
+    The scaling std of the model output. This is usually computed as the std of `(molecule_energy - molecule_self_energy)`
 * ``compute_forces: bool = False``
 
     Whether to compute forces as the gradient of the ``y_graph_scalars`` and use those as the ``y_node_vector`` output.
 * ``y_node_scalars_loss_config: Optional[Dict] = None``
 
     The loss config for the ``y_node_scalars``.
 * ``y_node_vector_loss_config: Optional[Dict] = None``
```

### Comparing `physicsml-0.2.3/docs/source/pages/models/tensor_net.md` & `physicsml-0.2.4/docs/source/pages/models/tensor_net.md`

 * *Files 9% similar despite different names*

```diff
@@ -32,18 +32,18 @@
 
     The interaction MLP's hidden dimensions.
 * ``scalar_output_mlp_hidden_dims: List[int] = [256, 128]``
 
     The scalar output MLP's hidden dimensions.
 * ``scaling_mean: float = 0.0``
 
-    The scaling mean of the model output.
+    The scaling mean of the model output. This is usually computed as the mean of `(molecule_energy - molecule_self_energy)`
 * ``scaling_std: float = 1.0``
 
-    The scaling std of the model output.
+    The scaling std of the model output. This is usually computed as the std of `(molecule_energy - molecule_self_energy)`
 * ``compute_forces: bool = False``
 
     Whether to compute forces as the gradient of the ``y_graph_scalars`` and use those as the ``y_node_vector`` output.
 * ``y_node_scalars_loss_config: Optional[Dict] = None``
 
     The loss config for the ``y_node_scalars``.
 * ``y_node_vector_loss_config: Optional[Dict] = None``
```

### Comparing `physicsml-0.2.3/docs/source/pages/philosophy/molflux.md` & `physicsml-0.2.4/docs/source/pages/philosophy/molflux.md`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/docs/source/pages/philosophy/philosophy.md` & `physicsml-0.2.4/docs/source/pages/philosophy/philosophy.md`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/docs/source/pages/plugins/alanine-dipeptide-truncated.pdb` & `physicsml-0.2.4/docs/source/pages/plugins/alanine-dipeptide-truncated.pdb`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/docs/source/pages/plugins/ase.md` & `physicsml-0.2.4/docs/source/pages/plugins/ase.md`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/docs/source/pages/plugins/openmm.md` & `physicsml-0.2.4/docs/source/pages/plugins/openmm.md`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/docs/source/pages/structure/lightning_layer.md` & `physicsml-0.2.4/docs/source/pages/structure/lightning_layer.md`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/docs/source/pages/structure/molflux_layer.md` & `physicsml-0.2.4/docs/source/pages/structure/molflux_layer.md`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/docs/source/pages/structure/physicsml_structure.md` & `physicsml-0.2.4/docs/source/pages/structure/physicsml_structure.md`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/docs/source/pages/structure/torch_layer.md` & `physicsml-0.2.4/docs/source/pages/structure/torch_layer.md`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/docs/source/pages/structure/transfer_learning.md` & `physicsml-0.2.4/docs/source/pages/structure/transfer_learning.md`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/docs/source/pages/tutorials/ani1x_energy_forces_training.md` & `physicsml-0.2.4/docs/source/pages/tutorials/ani1x_energy_forces_training.md`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/docs/source/pages/tutorials/ani1x_truncated.parquet` & `physicsml-0.2.4/docs/source/pages/tutorials/ani1x_truncated.parquet`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/docs/source/pages/tutorials/gdb9_training.md` & `physicsml-0.2.4/docs/source/pages/tutorials/gdb9_training.md`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/docs/source/pages/tutorials/gdb9_trunc.parquet` & `physicsml-0.2.4/docs/source/pages/tutorials/gdb9_trunc.parquet`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/docs/source/pages/tutorials/gdb9_uncertainty.md` & `physicsml-0.2.4/docs/source/pages/tutorials/gdb9_uncertainty.md`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/docs/source/pages/tutorials/transfer_learning.md` & `physicsml-0.2.4/docs/source/pages/tutorials/transfer_learning.md`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/init_conda_venv.sh` & `physicsml-0.2.4/init_conda_venv.sh`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/init_python_venv.sh` & `physicsml-0.2.4/init_python_venv.sh`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/noxfile.py` & `physicsml-0.2.4/noxfile.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 PINNED_VERSIONS = "pinned-versions"
 COVERAGE_DIR = ".coverage"
 
 TEST_REPORTS_DIR = "test-reports"
 
 # all external utility tools used by our nox sessions
 BUILD_TOOLS = ["build"]
-COVERAGE_TOOLS = ["coverage[toml]", "coverage-badge"]
+COVERAGE_TOOLS = ["coverage[toml]<7.5", "coverage-badge"]
 FORMATTING_TOOLS = ["black[jupyter]~=23.0"]
 LINTING_TOOLS = ["ruff~=0.0.292"]
 LOCKFILE_TOOLS = ["pip-tools>=7.0.0"]  # default --resolver=backtracking
 
 EXTRAS = [None, "openmm", "rdkit", "ase", "openeye"]
 DONT_TEST = [None, "openeye", "openmm"]
 
@@ -274,17 +274,17 @@
 
     else:
         package_extras = ",".join(["tests"])
 
     # all tests requiring the extra are in their own dir and
     tests_target_dirs = [f"tests/{extra}"]
 
-    # Run tests
     session.install(f".[{package_extras}]", "--constraint", str(lockfile_path))
 
+    # Run tests
     coverage_datafile_path = resolve_coverage_datafile_path(python_version=session.python, extra=extra)
     junitxml_path = resolve_junitxml_path(python_version=session.python, extra=extra)
     session.run(
         "coverage",
         "run",
         f"--data-file={coverage_datafile_path}",
         "-m",
@@ -296,15 +296,15 @@
 
     # for parametrised runs, this will get run once at the end of all of them
     if notify:
         datafiles_dir = str(coverage_datafile_path.parent)
         session.notify(f"coverage_report-{session.python}", [datafiles_dir])
 
 
-@nox.session(venv_backend="conda", python=SUPPORTED_PYTHON_VERSIONS)
+@nox.session(python=SUPPORTED_PYTHON_VERSIONS)
 @nox.parametrize("extra", [e for e in EXTRAS if e not in DONT_TEST])
 def tests_run_latest(session: nox.Session, extra: Optional[str]) -> None:
     """Run tests against latest available dependencies.
 
     Examples:
         nox -s tests_run_latest-3.11
         nox -s "tests_run_latest-3.11(extra=None)"
@@ -316,15 +316,15 @@
     with tempfile.TemporaryDirectory() as tmp:
         scratch_output_lockfile_path = resolve_lockfile_path(python_version=session.python, extra=extra, rootdir=tmp)
         generate_lockfile(session, extra=extra, lockfile_path=scratch_output_lockfile_path)
 
         run_tests(session, *session.posargs, extra=extra, lockfile_path=scratch_output_lockfile_path, notify=False)
 
 
-@nox.session(venv_backend="conda", python=SUPPORTED_PYTHON_VERSIONS)
+@nox.session(python=SUPPORTED_PYTHON_VERSIONS)
 @nox.parametrize("extra", [e for e in EXTRAS if e not in DONT_TEST])
 def tests_run_pinned(session: nox.Session, extra: Optional[str]) -> None:
     """Run tests against pinned dependencies.
 
     These should already be present. If not, they can be generated / updated
     by running the `dependencies_pin` session.
```

### Comparing `physicsml-0.2.3/pinned-versions/3.10/lockfile.ase.txt` & `physicsml-0.2.4/pinned-versions/3.10/lockfile.core.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 #
 # This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
-#    nox -s dependencies_pin-3.10(extra='ase')
+#    nox -s dependencies_pin-3.10(extra=None)
 #
-absl-py==2.1.0
-    # via tensorboard
 accessible-pygments==0.0.4
     # via pydata-sphinx-theme
-aiohttp==3.9.3
+aiohttp==3.9.5
     # via
     #   datasets
     #   fsspec
     #   torch-geometric
 aiosignal==1.3.1
     # via aiohttp
 alabaster==0.7.16
@@ -41,67 +39,67 @@
     # via
     #   pydata-sphinx-theme
     #   sphinx
 beautifulsoup4==4.12.3
     # via
     #   pydata-sphinx-theme
     #   sphinx-toolbox
-boto3==1.34.45
+boto3==1.34.91
     # via
     #   cloudpathlib
     #   molflux
-botocore==1.34.45
+botocore==1.34.91
     # via
     #   boto3
     #   molflux
     #   s3transfer
 cachecontrol==0.14.0
     # via sphinx-toolbox
 certifi==2024.2.2
     # via requests
 charset-normalizer==3.3.2
     # via requests
 click==8.1.7
     # via jupyter-cache
-cloudpathlib==0.17.0
+cloudpathlib==0.18.1
     # via molflux
 colorama==0.4.6
     # via molflux
-comm==0.2.1
+comm==0.2.2
     # via
     #   ipykernel
     #   ipywidgets
-contourpy==1.2.0
+contourpy==1.2.1
     # via matplotlib
-coverage==7.4.1
+coverage==7.5.0
     # via
     #   coverage-badge
     #   physicsml (pyproject.toml)
-coverage-badge==1.1.0
+coverage-badge==1.1.1
     # via physicsml (pyproject.toml)
-cssutils==2.9.0
+cssutils==2.10.2
     # via dict2css
 cycler==0.12.1
     # via matplotlib
-datasets==2.17.1
+datasets==2.19.0
     # via
     #   evaluate
     #   molflux
 debugpy==1.8.1
     # via ipykernel
 decorator==5.1.1
     # via ipython
 dict2css==0.3.0.post1
     # via sphinx-toolbox
 dill==0.3.8
     # via
     #   datasets
     #   evaluate
     #   multiprocess
-docutils==0.20.1
+docutils==0.21.2
     # via
     #   myst-parser
     #   pydata-sphinx-theme
     #   sphinx
     #   sphinx-prompt
     #   sphinx-tabs
     #   sphinx-togglebutton
@@ -112,74 +110,73 @@
     #   apeye-core
     #   dict2css
     #   sphinx-toolbox
 e3nn==0.5.1
     # via physicsml (pyproject.toml)
 evaluate==0.4.1
     # via molflux
-exceptiongroup==1.2.0
+exceptiongroup==1.2.1
     # via
     #   ipython
     #   pytest
 executing==2.0.1
     # via stack-data
 fastjsonschema==2.19.1
     # via nbformat
-filelock==3.13.1
+filelock==3.13.4
     # via
     #   cachecontrol
     #   datasets
     #   huggingface-hub
     #   sphinx-toolbox
     #   torch
-fonttools==4.49.0
+fonttools==4.51.0
     # via matplotlib
 frozenlist==1.4.1
     # via
     #   aiohttp
     #   aiosignal
-fsspec==2023.10.0
+fsspec==2024.3.1
     # via
     #   datasets
     #   evaluate
     #   huggingface-hub
     #   lightning
     #   molflux
     #   pytorch-lightning
+    #   torch
     #   torch-geometric
-grpcio==1.60.1
-    # via tensorboard
-h5py==3.10.0
+h5py==3.11.0
     # via
     #   molflux
     #   physicsml (pyproject.toml)
 html5lib==1.1
     # via sphinx-toolbox
-huggingface-hub==0.20.3
+huggingface-hub==0.22.2
     # via
     #   datasets
     #   evaluate
-idna==3.6
+idna==3.7
     # via
     #   apeye-core
     #   requests
     #   yarl
 imagesize==1.4.1
     # via sphinx
 importlib-metadata==4.13.0
     # via
     #   jupyter-cache
     #   myst-nb
     #   qlient-core
     #   torchani
 iniconfig==2.0.0
     # via pytest
-ipykernel==6.29.2
+ipykernel==6.29.4
     # via myst-nb
-ipython==8.21.0
+ipython==8.23.0
     # via
     #   ipykernel
     #   ipywidgets
     #   myst-nb
 ipywidgets==8.1.2
     # via physicsml (pyproject.toml)
 jedi==0.19.1
@@ -191,66 +188,63 @@
     #   sphinx-jinja2-compat
     #   torch
     #   torch-geometric
 jmespath==1.0.1
     # via
     #   boto3
     #   botocore
-joblib==1.3.2
+joblib==1.4.0
     # via
     #   molflux
     #   scikit-learn
 jsonschema==4.21.1
     # via nbformat
 jsonschema-specifications==2023.12.1
     # via jsonschema
 jupyter-cache==1.0.0
     # via myst-nb
-jupyter-client==8.6.0
+jupyter-client==8.6.1
     # via
     #   ipykernel
     #   nbclient
-jupyter-core==5.7.1
+jupyter-core==5.7.2
     # via
     #   ipykernel
     #   jupyter-client
     #   nbclient
     #   nbformat
 jupyterlab-widgets==3.0.10
     # via ipywidgets
 jupytext==1.16.1
     # via physicsml (pyproject.toml)
 kiwisolver==1.4.5
     # via matplotlib
 lark-parser==0.12.0
     # via torchani
-lightning==2.2.0.post0
+lightning==2.2.3
     # via physicsml (pyproject.toml)
-lightning-utilities==0.10.1
+lightning-utilities==0.11.2
     # via
     #   lightning
     #   pytorch-lightning
     #   torchmetrics
-markdown==3.5.2
-    # via tensorboard
 markdown-it-py==3.0.0
     # via
     #   jupytext
     #   mdit-py-plugins
     #   myst-parser
 markupsafe==2.1.5
     # via
     #   jinja2
     #   sphinx-jinja2-compat
-    #   werkzeug
-matplotlib==3.8.3
+matplotlib==3.8.4
     # via
     #   ase
     #   physicsml (pyproject.toml)
-matplotlib-inline==0.1.6
+matplotlib-inline==0.1.7
     # via
     #   ipykernel
     #   ipython
 mdit-py-plugins==0.4.0
     # via
     #   jupytext
     #   myst-parser
@@ -260,43 +254,43 @@
     # via molflux
 molflux==0.3.0
     # via physicsml (pyproject.toml)
 more-itertools==10.2.0
     # via molflux
 mpmath==1.3.0
     # via sympy
-msgpack==1.0.7
+msgpack==1.0.8
     # via cachecontrol
 multidict==6.0.5
     # via
     #   aiohttp
     #   yarl
 multiprocess==0.70.16
     # via
     #   datasets
     #   evaluate
-myst-nb==1.0.0
+myst-nb==1.1.0
     # via physicsml (pyproject.toml)
-myst-parser==2.0.0
+myst-parser==3.0.0
     # via myst-nb
 natsort==8.4.0
     # via domdf-python-tools
-nbclient==0.9.0
+nbclient==0.10.0
     # via
     #   jupyter-cache
     #   myst-nb
-nbformat==5.9.2
+nbformat==5.10.4
     # via
     #   jupyter-cache
     #   jupytext
     #   myst-nb
     #   nbclient
 nest-asyncio==1.6.0
     # via ipykernel
-networkx==3.2.1
+networkx==3.3
     # via torch
 numpy==1.26.4
     # via
     #   ase
     #   contourpy
     #   datasets
     #   evaluate
@@ -307,22 +301,21 @@
     #   opt-einsum
     #   pandas
     #   pyarrow
     #   pytorch-lightning
     #   rdkit
     #   scikit-learn
     #   scipy
-    #   tensorboard
     #   torch-geometric
     #   torchmetrics
 opt-einsum==3.3.0
     # via opt-einsum-fx
 opt-einsum-fx==0.1.4
     # via e3nn
-packaging==23.2
+packaging==24.0
     # via
     #   datasets
     #   evaluate
     #   huggingface-hub
     #   ipykernel
     #   jupytext
     #   lightning
@@ -330,114 +323,111 @@
     #   matplotlib
     #   opt-einsum-fx
     #   pydata-sphinx-theme
     #   pytest
     #   pytorch-lightning
     #   sphinx
     #   torchmetrics
-pandas==2.2.0
+pandas==2.2.2
     # via
     #   datasets
     #   evaluate
     #   molflux
-parso==0.8.3
+parso==0.8.4
     # via jedi
 pexpect==4.9.0
     # via ipython
-pillow==10.2.0
+pillow==10.3.0
     # via
     #   matplotlib
     #   rdkit
-platformdirs==4.2.0
+platformdirs==4.2.1
     # via
     #   apeye
     #   jupyter-core
-pluggy==1.4.0
+pluggy==1.5.0
     # via pytest
 prompt-toolkit==3.0.43
     # via ipython
-protobuf==4.25.3
-    # via tensorboard
 psutil==5.9.8
     # via
     #   ipykernel
     #   torch-geometric
 ptyprocess==0.7.0
     # via pexpect
 pure-eval==0.2.2
     # via stack-data
-pyarrow==15.0.0
+pyarrow==16.0.0
     # via
     #   datasets
     #   molflux
 pyarrow-hotfix==0.6
     # via datasets
-pydantic==1.10.14
+pydantic==1.10.15
     # via molflux
 pydata-sphinx-theme==0.15.2
     # via sphinx-book-theme
 pygments==2.17.2
     # via
     #   accessible-pygments
     #   ipython
     #   pydata-sphinx-theme
     #   sphinx
     #   sphinx-prompt
     #   sphinx-tabs
-pyparsing==3.1.1
+pyparsing==3.1.2
     # via
     #   matplotlib
     #   torch-geometric
-pytest==8.0.1
+pytest==8.1.1
     # via physicsml (pyproject.toml)
-python-dateutil==2.8.2
+python-dateutil==2.9.0.post0
     # via
     #   botocore
     #   jupyter-client
     #   matplotlib
     #   molflux
     #   pandas
-pytorch-lightning==2.2.0.post0
+pytorch-lightning==2.2.3
     # via lightning
 pytz==2024.1
     # via pandas
 pyyaml==6.0.1
     # via
     #   datasets
     #   huggingface-hub
     #   jupyter-cache
     #   jupytext
     #   lightning
     #   molflux
     #   myst-nb
     #   myst-parser
     #   pytorch-lightning
-pyzmq==25.1.2
+pyzmq==26.0.2
     # via
     #   ipykernel
     #   jupyter-client
 qlient==1.0.0
     # via molflux
 qlient-core==1.0.1
     # via qlient
-rapidfuzz==3.6.1
+rapidfuzz==3.8.1
     # via thefuzz
 rdkit==2023.9.5
     # via physicsml (pyproject.toml)
-referencing==0.33.0
+referencing==0.35.0
     # via
     #   jsonschema
     #   jsonschema-specifications
 requests==2.31.0
     # via
     #   apeye
     #   cachecontrol
     #   datasets
     #   evaluate
-    #   fsspec
     #   huggingface-hub
     #   molflux
     #   qlient
     #   responses
     #   sphinx
     #   torch-geometric
     #   torchani
@@ -447,38 +437,37 @@
     # via
     #   jsonschema
     #   referencing
 ruamel-yaml==0.18.6
     # via sphinx-toolbox
 ruamel-yaml-clib==0.2.8
     # via ruamel-yaml
-s3transfer==0.10.0
+s3transfer==0.10.1
     # via boto3
-scikit-learn==1.4.1.post1
+scikit-learn==1.4.2
     # via
     #   molflux
     #   torch-geometric
-scipy==1.12.0
+scipy==1.13.0
     # via
     #   ase
     #   e3nn
     #   molflux
     #   scikit-learn
     #   torch-geometric
 six==1.16.0
     # via
     #   asttokens
     #   html5lib
     #   python-dateutil
-    #   tensorboard
 snowballstemmer==2.2.0
     # via sphinx
 soupsieve==2.5
     # via beautifulsoup4
-sphinx==7.2.6
+sphinx==7.3.7
     # via
     #   autodocsumm
     #   myst-nb
     #   myst-parser
     #   physicsml (pyproject.toml)
     #   pydata-sphinx-theme
     #   sphinx-autodoc-typehints
@@ -486,15 +475,15 @@
     #   sphinx-design
     #   sphinx-inline-tabs
     #   sphinx-prompt
     #   sphinx-sitemap
     #   sphinx-tabs
     #   sphinx-togglebutton
     #   sphinx-toolbox
-sphinx-autodoc-typehints==2.0.0
+sphinx-autodoc-typehints==2.1.0
     # via sphinx-toolbox
 sphinx-book-theme==1.1.2
     # via physicsml (pyproject.toml)
 sphinx-design==0.5.0
     # via physicsml (pyproject.toml)
 sphinx-inline-tabs==2023.4.21
     # via physicsml (pyproject.toml)
@@ -518,56 +507,53 @@
     # via sphinx
 sphinxcontrib-jsmath==1.0.1
     # via sphinx
 sphinxcontrib-qthelp==1.0.7
     # via sphinx
 sphinxcontrib-serializinghtml==1.1.10
     # via sphinx
-sqlalchemy==2.0.27
+sqlalchemy==2.0.29
     # via jupyter-cache
 stack-data==0.6.3
     # via ipython
 sympy==1.12
     # via
     #   e3nn
     #   torch
 tabulate==0.9.0
     # via
     #   jupyter-cache
     #   sphinx-toolbox
 tenacity==8.2.3
     # via molflux
-tensorboard==2.16.2
-    # via physicsml (pyproject.toml)
-tensorboard-data-server==0.7.2
-    # via tensorboard
 thefuzz==0.22.1
     # via molflux
-threadpoolctl==3.3.0
+threadpoolctl==3.4.0
     # via scikit-learn
 toml==0.10.2
     # via jupytext
 tomli==2.0.1
     # via
     #   coverage
     #   pytest
-torch==2.0.1
+    #   sphinx
+torch==2.3.0
     # via
     #   e3nn
     #   lightning
     #   opt-einsum-fx
     #   physicsml (pyproject.toml)
     #   pytorch-lightning
     #   torchani
     #   torchmetrics
-torch-geometric==2.5.0
+torch-geometric==2.5.3
     # via physicsml (pyproject.toml)
 torchani==2.2.3
     # via physicsml (pyproject.toml)
-torchmetrics==1.3.1
+torchmetrics==1.3.2
     # via
     #   lightning
     #   pytorch-lightning
 tornado==6.4
     # via
     #   ipykernel
     #   jupyter-client
@@ -576,63 +562,62 @@
     #   datasets
     #   evaluate
     #   huggingface-hub
     #   lightning
     #   molflux
     #   pytorch-lightning
     #   torch-geometric
-traitlets==5.14.1
+traitlets==5.14.3
     # via
     #   comm
     #   ipykernel
     #   ipython
     #   ipywidgets
     #   jupyter-client
     #   jupyter-core
     #   matplotlib-inline
     #   nbclient
     #   nbformat
-typing-extensions==4.9.0
+typing-extensions==4.11.0
     # via
     #   cloudpathlib
     #   domdf-python-tools
     #   huggingface-hub
+    #   ipython
     #   lightning
     #   lightning-utilities
     #   molflux
     #   myst-nb
     #   pydantic
     #   pydata-sphinx-theme
     #   pytorch-lightning
     #   sphinx-toolbox
     #   sqlalchemy
     #   torch
 tzdata==2024.1
     # via pandas
-urllib3==2.0.7
+urllib3==2.2.1
     # via
     #   botocore
     #   requests
     #   responses
 wcwidth==0.2.13
     # via prompt-toolkit
 webencodings==0.5.1
     # via html5lib
-websocket-client==1.7.0
+websocket-client==1.8.0
     # via qlient
-werkzeug==3.0.1
-    # via tensorboard
-wheel==0.42.0
+wheel==0.43.0
     # via sphinx-togglebutton
 widgetsnbextension==4.0.10
     # via ipywidgets
 xxhash==3.4.1
     # via
     #   datasets
     #   evaluate
 yarl==1.9.4
     # via aiohttp
-zipp==3.17.0
+zipp==3.18.1
     # via importlib-metadata
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `physicsml-0.2.3/pinned-versions/3.10/lockfile.core.txt` & `physicsml-0.2.4/pinned-versions/3.10/lockfile.openmm.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 #
 # This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
-#    nox -s dependencies_pin-3.10(extra=None)
+#    nox -s dependencies_pin-3.10(extra='openmm')
 #
-absl-py==2.1.0
-    # via tensorboard
 accessible-pygments==0.0.4
     # via pydata-sphinx-theme
-aiohttp==3.9.3
+aiohttp==3.9.5
     # via
     #   datasets
     #   fsspec
     #   torch-geometric
 aiosignal==1.3.1
     # via aiohttp
 alabaster==0.7.16
@@ -41,67 +39,67 @@
     # via
     #   pydata-sphinx-theme
     #   sphinx
 beautifulsoup4==4.12.3
     # via
     #   pydata-sphinx-theme
     #   sphinx-toolbox
-boto3==1.34.45
+boto3==1.34.91
     # via
     #   cloudpathlib
     #   molflux
-botocore==1.34.45
+botocore==1.34.91
     # via
     #   boto3
     #   molflux
     #   s3transfer
 cachecontrol==0.14.0
     # via sphinx-toolbox
 certifi==2024.2.2
     # via requests
 charset-normalizer==3.3.2
     # via requests
 click==8.1.7
     # via jupyter-cache
-cloudpathlib==0.17.0
+cloudpathlib==0.18.1
     # via molflux
 colorama==0.4.6
     # via molflux
-comm==0.2.1
+comm==0.2.2
     # via
     #   ipykernel
     #   ipywidgets
-contourpy==1.2.0
+contourpy==1.2.1
     # via matplotlib
-coverage==7.4.1
+coverage==7.5.0
     # via
     #   coverage-badge
     #   physicsml (pyproject.toml)
-coverage-badge==1.1.0
+coverage-badge==1.1.1
     # via physicsml (pyproject.toml)
-cssutils==2.9.0
+cssutils==2.10.2
     # via dict2css
 cycler==0.12.1
     # via matplotlib
-datasets==2.17.1
+datasets==2.19.0
     # via
     #   evaluate
     #   molflux
 debugpy==1.8.1
     # via ipykernel
 decorator==5.1.1
     # via ipython
 dict2css==0.3.0.post1
     # via sphinx-toolbox
 dill==0.3.8
     # via
     #   datasets
     #   evaluate
     #   multiprocess
-docutils==0.20.1
+docutils==0.21.2
     # via
     #   myst-parser
     #   pydata-sphinx-theme
     #   sphinx
     #   sphinx-prompt
     #   sphinx-tabs
     #   sphinx-togglebutton
@@ -112,74 +110,73 @@
     #   apeye-core
     #   dict2css
     #   sphinx-toolbox
 e3nn==0.5.1
     # via physicsml (pyproject.toml)
 evaluate==0.4.1
     # via molflux
-exceptiongroup==1.2.0
+exceptiongroup==1.2.1
     # via
     #   ipython
     #   pytest
 executing==2.0.1
     # via stack-data
 fastjsonschema==2.19.1
     # via nbformat
-filelock==3.13.1
+filelock==3.13.4
     # via
     #   cachecontrol
     #   datasets
     #   huggingface-hub
     #   sphinx-toolbox
     #   torch
-fonttools==4.49.0
+fonttools==4.51.0
     # via matplotlib
 frozenlist==1.4.1
     # via
     #   aiohttp
     #   aiosignal
-fsspec==2023.10.0
+fsspec==2024.3.1
     # via
     #   datasets
     #   evaluate
     #   huggingface-hub
     #   lightning
     #   molflux
     #   pytorch-lightning
+    #   torch
     #   torch-geometric
-grpcio==1.60.1
-    # via tensorboard
-h5py==3.10.0
+h5py==3.11.0
     # via
     #   molflux
     #   physicsml (pyproject.toml)
 html5lib==1.1
     # via sphinx-toolbox
-huggingface-hub==0.20.3
+huggingface-hub==0.22.2
     # via
     #   datasets
     #   evaluate
-idna==3.6
+idna==3.7
     # via
     #   apeye-core
     #   requests
     #   yarl
 imagesize==1.4.1
     # via sphinx
 importlib-metadata==4.13.0
     # via
     #   jupyter-cache
     #   myst-nb
     #   qlient-core
     #   torchani
 iniconfig==2.0.0
     # via pytest
-ipykernel==6.29.2
+ipykernel==6.29.4
     # via myst-nb
-ipython==8.21.0
+ipython==8.23.0
     # via
     #   ipykernel
     #   ipywidgets
     #   myst-nb
 ipywidgets==8.1.2
     # via physicsml (pyproject.toml)
 jedi==0.19.1
@@ -191,66 +188,63 @@
     #   sphinx-jinja2-compat
     #   torch
     #   torch-geometric
 jmespath==1.0.1
     # via
     #   boto3
     #   botocore
-joblib==1.3.2
+joblib==1.4.0
     # via
     #   molflux
     #   scikit-learn
 jsonschema==4.21.1
     # via nbformat
 jsonschema-specifications==2023.12.1
     # via jsonschema
 jupyter-cache==1.0.0
     # via myst-nb
-jupyter-client==8.6.0
+jupyter-client==8.6.1
     # via
     #   ipykernel
     #   nbclient
-jupyter-core==5.7.1
+jupyter-core==5.7.2
     # via
     #   ipykernel
     #   jupyter-client
     #   nbclient
     #   nbformat
 jupyterlab-widgets==3.0.10
     # via ipywidgets
 jupytext==1.16.1
     # via physicsml (pyproject.toml)
 kiwisolver==1.4.5
     # via matplotlib
 lark-parser==0.12.0
     # via torchani
-lightning==2.2.0.post0
+lightning==2.2.3
     # via physicsml (pyproject.toml)
-lightning-utilities==0.10.1
+lightning-utilities==0.11.2
     # via
     #   lightning
     #   pytorch-lightning
     #   torchmetrics
-markdown==3.5.2
-    # via tensorboard
 markdown-it-py==3.0.0
     # via
     #   jupytext
     #   mdit-py-plugins
     #   myst-parser
 markupsafe==2.1.5
     # via
     #   jinja2
     #   sphinx-jinja2-compat
-    #   werkzeug
-matplotlib==3.8.3
+matplotlib==3.8.4
     # via
     #   ase
     #   physicsml (pyproject.toml)
-matplotlib-inline==0.1.6
+matplotlib-inline==0.1.7
     # via
     #   ipykernel
     #   ipython
 mdit-py-plugins==0.4.0
     # via
     #   jupytext
     #   myst-parser
@@ -260,43 +254,43 @@
     # via molflux
 molflux==0.3.0
     # via physicsml (pyproject.toml)
 more-itertools==10.2.0
     # via molflux
 mpmath==1.3.0
     # via sympy
-msgpack==1.0.7
+msgpack==1.0.8
     # via cachecontrol
 multidict==6.0.5
     # via
     #   aiohttp
     #   yarl
 multiprocess==0.70.16
     # via
     #   datasets
     #   evaluate
-myst-nb==1.0.0
+myst-nb==1.1.0
     # via physicsml (pyproject.toml)
-myst-parser==2.0.0
+myst-parser==3.0.0
     # via myst-nb
 natsort==8.4.0
     # via domdf-python-tools
-nbclient==0.9.0
+nbclient==0.10.0
     # via
     #   jupyter-cache
     #   myst-nb
-nbformat==5.9.2
+nbformat==5.10.4
     # via
     #   jupyter-cache
     #   jupytext
     #   myst-nb
     #   nbclient
 nest-asyncio==1.6.0
     # via ipykernel
-networkx==3.2.1
+networkx==3.3
     # via torch
 numpy==1.26.4
     # via
     #   ase
     #   contourpy
     #   datasets
     #   evaluate
@@ -307,22 +301,21 @@
     #   opt-einsum
     #   pandas
     #   pyarrow
     #   pytorch-lightning
     #   rdkit
     #   scikit-learn
     #   scipy
-    #   tensorboard
     #   torch-geometric
     #   torchmetrics
 opt-einsum==3.3.0
     # via opt-einsum-fx
 opt-einsum-fx==0.1.4
     # via e3nn
-packaging==23.2
+packaging==24.0
     # via
     #   datasets
     #   evaluate
     #   huggingface-hub
     #   ipykernel
     #   jupytext
     #   lightning
@@ -330,114 +323,111 @@
     #   matplotlib
     #   opt-einsum-fx
     #   pydata-sphinx-theme
     #   pytest
     #   pytorch-lightning
     #   sphinx
     #   torchmetrics
-pandas==2.2.0
+pandas==2.2.2
     # via
     #   datasets
     #   evaluate
     #   molflux
-parso==0.8.3
+parso==0.8.4
     # via jedi
 pexpect==4.9.0
     # via ipython
-pillow==10.2.0
+pillow==10.3.0
     # via
     #   matplotlib
     #   rdkit
-platformdirs==4.2.0
+platformdirs==4.2.1
     # via
     #   apeye
     #   jupyter-core
-pluggy==1.4.0
+pluggy==1.5.0
     # via pytest
 prompt-toolkit==3.0.43
     # via ipython
-protobuf==4.25.3
-    # via tensorboard
 psutil==5.9.8
     # via
     #   ipykernel
     #   torch-geometric
 ptyprocess==0.7.0
     # via pexpect
 pure-eval==0.2.2
     # via stack-data
-pyarrow==15.0.0
+pyarrow==16.0.0
     # via
     #   datasets
     #   molflux
 pyarrow-hotfix==0.6
     # via datasets
-pydantic==1.10.14
+pydantic==1.10.15
     # via molflux
 pydata-sphinx-theme==0.15.2
     # via sphinx-book-theme
 pygments==2.17.2
     # via
     #   accessible-pygments
     #   ipython
     #   pydata-sphinx-theme
     #   sphinx
     #   sphinx-prompt
     #   sphinx-tabs
-pyparsing==3.1.1
+pyparsing==3.1.2
     # via
     #   matplotlib
     #   torch-geometric
-pytest==8.0.1
+pytest==8.1.1
     # via physicsml (pyproject.toml)
-python-dateutil==2.8.2
+python-dateutil==2.9.0.post0
     # via
     #   botocore
     #   jupyter-client
     #   matplotlib
     #   molflux
     #   pandas
-pytorch-lightning==2.2.0.post0
+pytorch-lightning==2.2.3
     # via lightning
 pytz==2024.1
     # via pandas
 pyyaml==6.0.1
     # via
     #   datasets
     #   huggingface-hub
     #   jupyter-cache
     #   jupytext
     #   lightning
     #   molflux
     #   myst-nb
     #   myst-parser
     #   pytorch-lightning
-pyzmq==25.1.2
+pyzmq==26.0.2
     # via
     #   ipykernel
     #   jupyter-client
 qlient==1.0.0
     # via molflux
 qlient-core==1.0.1
     # via qlient
-rapidfuzz==3.6.1
+rapidfuzz==3.8.1
     # via thefuzz
 rdkit==2023.9.5
     # via physicsml (pyproject.toml)
-referencing==0.33.0
+referencing==0.35.0
     # via
     #   jsonschema
     #   jsonschema-specifications
 requests==2.31.0
     # via
     #   apeye
     #   cachecontrol
     #   datasets
     #   evaluate
-    #   fsspec
     #   huggingface-hub
     #   molflux
     #   qlient
     #   responses
     #   sphinx
     #   torch-geometric
     #   torchani
@@ -447,38 +437,37 @@
     # via
     #   jsonschema
     #   referencing
 ruamel-yaml==0.18.6
     # via sphinx-toolbox
 ruamel-yaml-clib==0.2.8
     # via ruamel-yaml
-s3transfer==0.10.0
+s3transfer==0.10.1
     # via boto3
-scikit-learn==1.4.1.post1
+scikit-learn==1.4.2
     # via
     #   molflux
     #   torch-geometric
-scipy==1.12.0
+scipy==1.13.0
     # via
     #   ase
     #   e3nn
     #   molflux
     #   scikit-learn
     #   torch-geometric
 six==1.16.0
     # via
     #   asttokens
     #   html5lib
     #   python-dateutil
-    #   tensorboard
 snowballstemmer==2.2.0
     # via sphinx
 soupsieve==2.5
     # via beautifulsoup4
-sphinx==7.2.6
+sphinx==7.3.7
     # via
     #   autodocsumm
     #   myst-nb
     #   myst-parser
     #   physicsml (pyproject.toml)
     #   pydata-sphinx-theme
     #   sphinx-autodoc-typehints
@@ -486,15 +475,15 @@
     #   sphinx-design
     #   sphinx-inline-tabs
     #   sphinx-prompt
     #   sphinx-sitemap
     #   sphinx-tabs
     #   sphinx-togglebutton
     #   sphinx-toolbox
-sphinx-autodoc-typehints==2.0.0
+sphinx-autodoc-typehints==2.1.0
     # via sphinx-toolbox
 sphinx-book-theme==1.1.2
     # via physicsml (pyproject.toml)
 sphinx-design==0.5.0
     # via physicsml (pyproject.toml)
 sphinx-inline-tabs==2023.4.21
     # via physicsml (pyproject.toml)
@@ -518,56 +507,53 @@
     # via sphinx
 sphinxcontrib-jsmath==1.0.1
     # via sphinx
 sphinxcontrib-qthelp==1.0.7
     # via sphinx
 sphinxcontrib-serializinghtml==1.1.10
     # via sphinx
-sqlalchemy==2.0.27
+sqlalchemy==2.0.29
     # via jupyter-cache
 stack-data==0.6.3
     # via ipython
 sympy==1.12
     # via
     #   e3nn
     #   torch
 tabulate==0.9.0
     # via
     #   jupyter-cache
     #   sphinx-toolbox
 tenacity==8.2.3
     # via molflux
-tensorboard==2.16.2
-    # via physicsml (pyproject.toml)
-tensorboard-data-server==0.7.2
-    # via tensorboard
 thefuzz==0.22.1
     # via molflux
-threadpoolctl==3.3.0
+threadpoolctl==3.4.0
     # via scikit-learn
 toml==0.10.2
     # via jupytext
 tomli==2.0.1
     # via
     #   coverage
     #   pytest
-torch==2.0.1
+    #   sphinx
+torch==2.3.0
     # via
     #   e3nn
     #   lightning
     #   opt-einsum-fx
     #   physicsml (pyproject.toml)
     #   pytorch-lightning
     #   torchani
     #   torchmetrics
-torch-geometric==2.5.0
+torch-geometric==2.5.3
     # via physicsml (pyproject.toml)
 torchani==2.2.3
     # via physicsml (pyproject.toml)
-torchmetrics==1.3.1
+torchmetrics==1.3.2
     # via
     #   lightning
     #   pytorch-lightning
 tornado==6.4
     # via
     #   ipykernel
     #   jupyter-client
@@ -576,63 +562,62 @@
     #   datasets
     #   evaluate
     #   huggingface-hub
     #   lightning
     #   molflux
     #   pytorch-lightning
     #   torch-geometric
-traitlets==5.14.1
+traitlets==5.14.3
     # via
     #   comm
     #   ipykernel
     #   ipython
     #   ipywidgets
     #   jupyter-client
     #   jupyter-core
     #   matplotlib-inline
     #   nbclient
     #   nbformat
-typing-extensions==4.9.0
+typing-extensions==4.11.0
     # via
     #   cloudpathlib
     #   domdf-python-tools
     #   huggingface-hub
+    #   ipython
     #   lightning
     #   lightning-utilities
     #   molflux
     #   myst-nb
     #   pydantic
     #   pydata-sphinx-theme
     #   pytorch-lightning
     #   sphinx-toolbox
     #   sqlalchemy
     #   torch
 tzdata==2024.1
     # via pandas
-urllib3==2.0.7
+urllib3==2.2.1
     # via
     #   botocore
     #   requests
     #   responses
 wcwidth==0.2.13
     # via prompt-toolkit
 webencodings==0.5.1
     # via html5lib
-websocket-client==1.7.0
+websocket-client==1.8.0
     # via qlient
-werkzeug==3.0.1
-    # via tensorboard
-wheel==0.42.0
+wheel==0.43.0
     # via sphinx-togglebutton
 widgetsnbextension==4.0.10
     # via ipywidgets
 xxhash==3.4.1
     # via
     #   datasets
     #   evaluate
 yarl==1.9.4
     # via aiohttp
-zipp==3.17.0
+zipp==3.18.1
     # via importlib-metadata
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `physicsml-0.2.3/pinned-versions/3.10/lockfile.openeye.txt` & `physicsml-0.2.4/pinned-versions/3.10/lockfile.ase.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 #
 # This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
-#    nox -s dependencies_pin-3.10(extra='openeye')
+#    nox -s dependencies_pin-3.10(extra='ase')
 #
-absl-py==2.1.0
-    # via tensorboard
 accessible-pygments==0.0.4
     # via pydata-sphinx-theme
-aiohttp==3.9.3
+aiohttp==3.9.5
     # via
     #   datasets
     #   fsspec
     #   torch-geometric
 aiosignal==1.3.1
     # via aiohttp
 alabaster==0.7.16
@@ -41,67 +39,67 @@
     # via
     #   pydata-sphinx-theme
     #   sphinx
 beautifulsoup4==4.12.3
     # via
     #   pydata-sphinx-theme
     #   sphinx-toolbox
-boto3==1.34.45
+boto3==1.34.91
     # via
     #   cloudpathlib
     #   molflux
-botocore==1.34.45
+botocore==1.34.91
     # via
     #   boto3
     #   molflux
     #   s3transfer
 cachecontrol==0.14.0
     # via sphinx-toolbox
 certifi==2024.2.2
     # via requests
 charset-normalizer==3.3.2
     # via requests
 click==8.1.7
     # via jupyter-cache
-cloudpathlib==0.17.0
+cloudpathlib==0.18.1
     # via molflux
 colorama==0.4.6
     # via molflux
-comm==0.2.1
+comm==0.2.2
     # via
     #   ipykernel
     #   ipywidgets
-contourpy==1.2.0
+contourpy==1.2.1
     # via matplotlib
-coverage==7.4.1
+coverage==7.5.0
     # via
     #   coverage-badge
     #   physicsml (pyproject.toml)
-coverage-badge==1.1.0
+coverage-badge==1.1.1
     # via physicsml (pyproject.toml)
-cssutils==2.9.0
+cssutils==2.10.2
     # via dict2css
 cycler==0.12.1
     # via matplotlib
-datasets==2.17.1
+datasets==2.19.0
     # via
     #   evaluate
     #   molflux
 debugpy==1.8.1
     # via ipykernel
 decorator==5.1.1
     # via ipython
 dict2css==0.3.0.post1
     # via sphinx-toolbox
 dill==0.3.8
     # via
     #   datasets
     #   evaluate
     #   multiprocess
-docutils==0.20.1
+docutils==0.21.2
     # via
     #   myst-parser
     #   pydata-sphinx-theme
     #   sphinx
     #   sphinx-prompt
     #   sphinx-tabs
     #   sphinx-togglebutton
@@ -112,74 +110,73 @@
     #   apeye-core
     #   dict2css
     #   sphinx-toolbox
 e3nn==0.5.1
     # via physicsml (pyproject.toml)
 evaluate==0.4.1
     # via molflux
-exceptiongroup==1.2.0
+exceptiongroup==1.2.1
     # via
     #   ipython
     #   pytest
 executing==2.0.1
     # via stack-data
 fastjsonschema==2.19.1
     # via nbformat
-filelock==3.13.1
+filelock==3.13.4
     # via
     #   cachecontrol
     #   datasets
     #   huggingface-hub
     #   sphinx-toolbox
     #   torch
-fonttools==4.49.0
+fonttools==4.51.0
     # via matplotlib
 frozenlist==1.4.1
     # via
     #   aiohttp
     #   aiosignal
-fsspec==2023.10.0
+fsspec==2024.3.1
     # via
     #   datasets
     #   evaluate
     #   huggingface-hub
     #   lightning
     #   molflux
     #   pytorch-lightning
+    #   torch
     #   torch-geometric
-grpcio==1.60.1
-    # via tensorboard
-h5py==3.10.0
+h5py==3.11.0
     # via
     #   molflux
     #   physicsml (pyproject.toml)
 html5lib==1.1
     # via sphinx-toolbox
-huggingface-hub==0.20.3
+huggingface-hub==0.22.2
     # via
     #   datasets
     #   evaluate
-idna==3.6
+idna==3.7
     # via
     #   apeye-core
     #   requests
     #   yarl
 imagesize==1.4.1
     # via sphinx
 importlib-metadata==4.13.0
     # via
     #   jupyter-cache
     #   myst-nb
     #   qlient-core
     #   torchani
 iniconfig==2.0.0
     # via pytest
-ipykernel==6.29.2
+ipykernel==6.29.4
     # via myst-nb
-ipython==8.21.0
+ipython==8.23.0
     # via
     #   ipykernel
     #   ipywidgets
     #   myst-nb
 ipywidgets==8.1.2
     # via physicsml (pyproject.toml)
 jedi==0.19.1
@@ -191,66 +188,63 @@
     #   sphinx-jinja2-compat
     #   torch
     #   torch-geometric
 jmespath==1.0.1
     # via
     #   boto3
     #   botocore
-joblib==1.3.2
+joblib==1.4.0
     # via
     #   molflux
     #   scikit-learn
 jsonschema==4.21.1
     # via nbformat
 jsonschema-specifications==2023.12.1
     # via jsonschema
 jupyter-cache==1.0.0
     # via myst-nb
-jupyter-client==8.6.0
+jupyter-client==8.6.1
     # via
     #   ipykernel
     #   nbclient
-jupyter-core==5.7.1
+jupyter-core==5.7.2
     # via
     #   ipykernel
     #   jupyter-client
     #   nbclient
     #   nbformat
 jupyterlab-widgets==3.0.10
     # via ipywidgets
 jupytext==1.16.1
     # via physicsml (pyproject.toml)
 kiwisolver==1.4.5
     # via matplotlib
 lark-parser==0.12.0
     # via torchani
-lightning==2.2.0.post0
+lightning==2.2.3
     # via physicsml (pyproject.toml)
-lightning-utilities==0.10.1
+lightning-utilities==0.11.2
     # via
     #   lightning
     #   pytorch-lightning
     #   torchmetrics
-markdown==3.5.2
-    # via tensorboard
 markdown-it-py==3.0.0
     # via
     #   jupytext
     #   mdit-py-plugins
     #   myst-parser
 markupsafe==2.1.5
     # via
     #   jinja2
     #   sphinx-jinja2-compat
-    #   werkzeug
-matplotlib==3.8.3
+matplotlib==3.8.4
     # via
     #   ase
     #   physicsml (pyproject.toml)
-matplotlib-inline==0.1.6
+matplotlib-inline==0.1.7
     # via
     #   ipykernel
     #   ipython
 mdit-py-plugins==0.4.0
     # via
     #   jupytext
     #   myst-parser
@@ -260,43 +254,43 @@
     # via molflux
 molflux==0.3.0
     # via physicsml (pyproject.toml)
 more-itertools==10.2.0
     # via molflux
 mpmath==1.3.0
     # via sympy
-msgpack==1.0.7
+msgpack==1.0.8
     # via cachecontrol
 multidict==6.0.5
     # via
     #   aiohttp
     #   yarl
 multiprocess==0.70.16
     # via
     #   datasets
     #   evaluate
-myst-nb==1.0.0
+myst-nb==1.1.0
     # via physicsml (pyproject.toml)
-myst-parser==2.0.0
+myst-parser==3.0.0
     # via myst-nb
 natsort==8.4.0
     # via domdf-python-tools
-nbclient==0.9.0
+nbclient==0.10.0
     # via
     #   jupyter-cache
     #   myst-nb
-nbformat==5.9.2
+nbformat==5.10.4
     # via
     #   jupyter-cache
     #   jupytext
     #   myst-nb
     #   nbclient
 nest-asyncio==1.6.0
     # via ipykernel
-networkx==3.2.1
+networkx==3.3
     # via torch
 numpy==1.26.4
     # via
     #   ase
     #   contourpy
     #   datasets
     #   evaluate
@@ -307,24 +301,21 @@
     #   opt-einsum
     #   pandas
     #   pyarrow
     #   pytorch-lightning
     #   rdkit
     #   scikit-learn
     #   scipy
-    #   tensorboard
     #   torch-geometric
     #   torchmetrics
-openeye-toolkits==2023.2.3
-    # via physicsml (pyproject.toml)
 opt-einsum==3.3.0
     # via opt-einsum-fx
 opt-einsum-fx==0.1.4
     # via e3nn
-packaging==23.2
+packaging==24.0
     # via
     #   datasets
     #   evaluate
     #   huggingface-hub
     #   ipykernel
     #   jupytext
     #   lightning
@@ -332,114 +323,111 @@
     #   matplotlib
     #   opt-einsum-fx
     #   pydata-sphinx-theme
     #   pytest
     #   pytorch-lightning
     #   sphinx
     #   torchmetrics
-pandas==2.2.0
+pandas==2.2.2
     # via
     #   datasets
     #   evaluate
     #   molflux
-parso==0.8.3
+parso==0.8.4
     # via jedi
 pexpect==4.9.0
     # via ipython
-pillow==10.2.0
+pillow==10.3.0
     # via
     #   matplotlib
     #   rdkit
-platformdirs==4.2.0
+platformdirs==4.2.1
     # via
     #   apeye
     #   jupyter-core
-pluggy==1.4.0
+pluggy==1.5.0
     # via pytest
 prompt-toolkit==3.0.43
     # via ipython
-protobuf==4.25.3
-    # via tensorboard
 psutil==5.9.8
     # via
     #   ipykernel
     #   torch-geometric
 ptyprocess==0.7.0
     # via pexpect
 pure-eval==0.2.2
     # via stack-data
-pyarrow==15.0.0
+pyarrow==16.0.0
     # via
     #   datasets
     #   molflux
 pyarrow-hotfix==0.6
     # via datasets
-pydantic==1.10.14
+pydantic==1.10.15
     # via molflux
 pydata-sphinx-theme==0.15.2
     # via sphinx-book-theme
 pygments==2.17.2
     # via
     #   accessible-pygments
     #   ipython
     #   pydata-sphinx-theme
     #   sphinx
     #   sphinx-prompt
     #   sphinx-tabs
-pyparsing==3.1.1
+pyparsing==3.1.2
     # via
     #   matplotlib
     #   torch-geometric
-pytest==8.0.1
+pytest==8.1.1
     # via physicsml (pyproject.toml)
-python-dateutil==2.8.2
+python-dateutil==2.9.0.post0
     # via
     #   botocore
     #   jupyter-client
     #   matplotlib
     #   molflux
     #   pandas
-pytorch-lightning==2.2.0.post0
+pytorch-lightning==2.2.3
     # via lightning
 pytz==2024.1
     # via pandas
 pyyaml==6.0.1
     # via
     #   datasets
     #   huggingface-hub
     #   jupyter-cache
     #   jupytext
     #   lightning
     #   molflux
     #   myst-nb
     #   myst-parser
     #   pytorch-lightning
-pyzmq==25.1.2
+pyzmq==26.0.2
     # via
     #   ipykernel
     #   jupyter-client
 qlient==1.0.0
     # via molflux
 qlient-core==1.0.1
     # via qlient
-rapidfuzz==3.6.1
+rapidfuzz==3.8.1
     # via thefuzz
 rdkit==2023.9.5
     # via physicsml (pyproject.toml)
-referencing==0.33.0
+referencing==0.35.0
     # via
     #   jsonschema
     #   jsonschema-specifications
 requests==2.31.0
     # via
     #   apeye
     #   cachecontrol
     #   datasets
     #   evaluate
-    #   fsspec
     #   huggingface-hub
     #   molflux
     #   qlient
     #   responses
     #   sphinx
     #   torch-geometric
     #   torchani
@@ -449,38 +437,37 @@
     # via
     #   jsonschema
     #   referencing
 ruamel-yaml==0.18.6
     # via sphinx-toolbox
 ruamel-yaml-clib==0.2.8
     # via ruamel-yaml
-s3transfer==0.10.0
+s3transfer==0.10.1
     # via boto3
-scikit-learn==1.4.1.post1
+scikit-learn==1.4.2
     # via
     #   molflux
     #   torch-geometric
-scipy==1.12.0
+scipy==1.13.0
     # via
     #   ase
     #   e3nn
     #   molflux
     #   scikit-learn
     #   torch-geometric
 six==1.16.0
     # via
     #   asttokens
     #   html5lib
     #   python-dateutil
-    #   tensorboard
 snowballstemmer==2.2.0
     # via sphinx
 soupsieve==2.5
     # via beautifulsoup4
-sphinx==7.2.6
+sphinx==7.3.7
     # via
     #   autodocsumm
     #   myst-nb
     #   myst-parser
     #   physicsml (pyproject.toml)
     #   pydata-sphinx-theme
     #   sphinx-autodoc-typehints
@@ -488,15 +475,15 @@
     #   sphinx-design
     #   sphinx-inline-tabs
     #   sphinx-prompt
     #   sphinx-sitemap
     #   sphinx-tabs
     #   sphinx-togglebutton
     #   sphinx-toolbox
-sphinx-autodoc-typehints==2.0.0
+sphinx-autodoc-typehints==2.1.0
     # via sphinx-toolbox
 sphinx-book-theme==1.1.2
     # via physicsml (pyproject.toml)
 sphinx-design==0.5.0
     # via physicsml (pyproject.toml)
 sphinx-inline-tabs==2023.4.21
     # via physicsml (pyproject.toml)
@@ -520,56 +507,53 @@
     # via sphinx
 sphinxcontrib-jsmath==1.0.1
     # via sphinx
 sphinxcontrib-qthelp==1.0.7
     # via sphinx
 sphinxcontrib-serializinghtml==1.1.10
     # via sphinx
-sqlalchemy==2.0.27
+sqlalchemy==2.0.29
     # via jupyter-cache
 stack-data==0.6.3
     # via ipython
 sympy==1.12
     # via
     #   e3nn
     #   torch
 tabulate==0.9.0
     # via
     #   jupyter-cache
     #   sphinx-toolbox
 tenacity==8.2.3
     # via molflux
-tensorboard==2.16.2
-    # via physicsml (pyproject.toml)
-tensorboard-data-server==0.7.2
-    # via tensorboard
 thefuzz==0.22.1
     # via molflux
-threadpoolctl==3.3.0
+threadpoolctl==3.4.0
     # via scikit-learn
 toml==0.10.2
     # via jupytext
 tomli==2.0.1
     # via
     #   coverage
     #   pytest
-torch==2.0.1
+    #   sphinx
+torch==2.3.0
     # via
     #   e3nn
     #   lightning
     #   opt-einsum-fx
     #   physicsml (pyproject.toml)
     #   pytorch-lightning
     #   torchani
     #   torchmetrics
-torch-geometric==2.5.0
+torch-geometric==2.5.3
     # via physicsml (pyproject.toml)
 torchani==2.2.3
     # via physicsml (pyproject.toml)
-torchmetrics==1.3.1
+torchmetrics==1.3.2
     # via
     #   lightning
     #   pytorch-lightning
 tornado==6.4
     # via
     #   ipykernel
     #   jupyter-client
@@ -578,63 +562,62 @@
     #   datasets
     #   evaluate
     #   huggingface-hub
     #   lightning
     #   molflux
     #   pytorch-lightning
     #   torch-geometric
-traitlets==5.14.1
+traitlets==5.14.3
     # via
     #   comm
     #   ipykernel
     #   ipython
     #   ipywidgets
     #   jupyter-client
     #   jupyter-core
     #   matplotlib-inline
     #   nbclient
     #   nbformat
-typing-extensions==4.9.0
+typing-extensions==4.11.0
     # via
     #   cloudpathlib
     #   domdf-python-tools
     #   huggingface-hub
+    #   ipython
     #   lightning
     #   lightning-utilities
     #   molflux
     #   myst-nb
     #   pydantic
     #   pydata-sphinx-theme
     #   pytorch-lightning
     #   sphinx-toolbox
     #   sqlalchemy
     #   torch
 tzdata==2024.1
     # via pandas
-urllib3==2.0.7
+urllib3==2.2.1
     # via
     #   botocore
     #   requests
     #   responses
 wcwidth==0.2.13
     # via prompt-toolkit
 webencodings==0.5.1
     # via html5lib
-websocket-client==1.7.0
+websocket-client==1.8.0
     # via qlient
-werkzeug==3.0.1
-    # via tensorboard
-wheel==0.42.0
+wheel==0.43.0
     # via sphinx-togglebutton
 widgetsnbextension==4.0.10
     # via ipywidgets
 xxhash==3.4.1
     # via
     #   datasets
     #   evaluate
 yarl==1.9.4
     # via aiohttp
-zipp==3.17.0
+zipp==3.18.1
     # via importlib-metadata
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `physicsml-0.2.3/pinned-versions/3.10/lockfile.openmm.txt` & `physicsml-0.2.4/pinned-versions/3.10/lockfile.rdkit.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 #
 # This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
-#    nox -s dependencies_pin-3.10(extra='openmm')
+#    nox -s dependencies_pin-3.10(extra='rdkit')
 #
-absl-py==2.1.0
-    # via tensorboard
 accessible-pygments==0.0.4
     # via pydata-sphinx-theme
-aiohttp==3.9.3
+aiohttp==3.9.5
     # via
     #   datasets
     #   fsspec
     #   torch-geometric
 aiosignal==1.3.1
     # via aiohttp
 alabaster==0.7.16
@@ -41,67 +39,67 @@
     # via
     #   pydata-sphinx-theme
     #   sphinx
 beautifulsoup4==4.12.3
     # via
     #   pydata-sphinx-theme
     #   sphinx-toolbox
-boto3==1.34.45
+boto3==1.34.91
     # via
     #   cloudpathlib
     #   molflux
-botocore==1.34.45
+botocore==1.34.91
     # via
     #   boto3
     #   molflux
     #   s3transfer
 cachecontrol==0.14.0
     # via sphinx-toolbox
 certifi==2024.2.2
     # via requests
 charset-normalizer==3.3.2
     # via requests
 click==8.1.7
     # via jupyter-cache
-cloudpathlib==0.17.0
+cloudpathlib==0.18.1
     # via molflux
 colorama==0.4.6
     # via molflux
-comm==0.2.1
+comm==0.2.2
     # via
     #   ipykernel
     #   ipywidgets
-contourpy==1.2.0
+contourpy==1.2.1
     # via matplotlib
-coverage==7.4.1
+coverage==7.5.0
     # via
     #   coverage-badge
     #   physicsml (pyproject.toml)
-coverage-badge==1.1.0
+coverage-badge==1.1.1
     # via physicsml (pyproject.toml)
-cssutils==2.9.0
+cssutils==2.10.2
     # via dict2css
 cycler==0.12.1
     # via matplotlib
-datasets==2.17.1
+datasets==2.19.0
     # via
     #   evaluate
     #   molflux
 debugpy==1.8.1
     # via ipykernel
 decorator==5.1.1
     # via ipython
 dict2css==0.3.0.post1
     # via sphinx-toolbox
 dill==0.3.8
     # via
     #   datasets
     #   evaluate
     #   multiprocess
-docutils==0.20.1
+docutils==0.21.2
     # via
     #   myst-parser
     #   pydata-sphinx-theme
     #   sphinx
     #   sphinx-prompt
     #   sphinx-tabs
     #   sphinx-togglebutton
@@ -112,74 +110,73 @@
     #   apeye-core
     #   dict2css
     #   sphinx-toolbox
 e3nn==0.5.1
     # via physicsml (pyproject.toml)
 evaluate==0.4.1
     # via molflux
-exceptiongroup==1.2.0
+exceptiongroup==1.2.1
     # via
     #   ipython
     #   pytest
 executing==2.0.1
     # via stack-data
 fastjsonschema==2.19.1
     # via nbformat
-filelock==3.13.1
+filelock==3.13.4
     # via
     #   cachecontrol
     #   datasets
     #   huggingface-hub
     #   sphinx-toolbox
     #   torch
-fonttools==4.49.0
+fonttools==4.51.0
     # via matplotlib
 frozenlist==1.4.1
     # via
     #   aiohttp
     #   aiosignal
-fsspec==2023.10.0
+fsspec==2024.3.1
     # via
     #   datasets
     #   evaluate
     #   huggingface-hub
     #   lightning
     #   molflux
     #   pytorch-lightning
+    #   torch
     #   torch-geometric
-grpcio==1.60.1
-    # via tensorboard
-h5py==3.10.0
+h5py==3.11.0
     # via
     #   molflux
     #   physicsml (pyproject.toml)
 html5lib==1.1
     # via sphinx-toolbox
-huggingface-hub==0.20.3
+huggingface-hub==0.22.2
     # via
     #   datasets
     #   evaluate
-idna==3.6
+idna==3.7
     # via
     #   apeye-core
     #   requests
     #   yarl
 imagesize==1.4.1
     # via sphinx
 importlib-metadata==4.13.0
     # via
     #   jupyter-cache
     #   myst-nb
     #   qlient-core
     #   torchani
 iniconfig==2.0.0
     # via pytest
-ipykernel==6.29.2
+ipykernel==6.29.4
     # via myst-nb
-ipython==8.21.0
+ipython==8.23.0
     # via
     #   ipykernel
     #   ipywidgets
     #   myst-nb
 ipywidgets==8.1.2
     # via physicsml (pyproject.toml)
 jedi==0.19.1
@@ -191,66 +188,63 @@
     #   sphinx-jinja2-compat
     #   torch
     #   torch-geometric
 jmespath==1.0.1
     # via
     #   boto3
     #   botocore
-joblib==1.3.2
+joblib==1.4.0
     # via
     #   molflux
     #   scikit-learn
 jsonschema==4.21.1
     # via nbformat
 jsonschema-specifications==2023.12.1
     # via jsonschema
 jupyter-cache==1.0.0
     # via myst-nb
-jupyter-client==8.6.0
+jupyter-client==8.6.1
     # via
     #   ipykernel
     #   nbclient
-jupyter-core==5.7.1
+jupyter-core==5.7.2
     # via
     #   ipykernel
     #   jupyter-client
     #   nbclient
     #   nbformat
 jupyterlab-widgets==3.0.10
     # via ipywidgets
 jupytext==1.16.1
     # via physicsml (pyproject.toml)
 kiwisolver==1.4.5
     # via matplotlib
 lark-parser==0.12.0
     # via torchani
-lightning==2.2.0.post0
+lightning==2.2.3
     # via physicsml (pyproject.toml)
-lightning-utilities==0.10.1
+lightning-utilities==0.11.2
     # via
     #   lightning
     #   pytorch-lightning
     #   torchmetrics
-markdown==3.5.2
-    # via tensorboard
 markdown-it-py==3.0.0
     # via
     #   jupytext
     #   mdit-py-plugins
     #   myst-parser
 markupsafe==2.1.5
     # via
     #   jinja2
     #   sphinx-jinja2-compat
-    #   werkzeug
-matplotlib==3.8.3
+matplotlib==3.8.4
     # via
     #   ase
     #   physicsml (pyproject.toml)
-matplotlib-inline==0.1.6
+matplotlib-inline==0.1.7
     # via
     #   ipykernel
     #   ipython
 mdit-py-plugins==0.4.0
     # via
     #   jupytext
     #   myst-parser
@@ -260,43 +254,43 @@
     # via molflux
 molflux==0.3.0
     # via physicsml (pyproject.toml)
 more-itertools==10.2.0
     # via molflux
 mpmath==1.3.0
     # via sympy
-msgpack==1.0.7
+msgpack==1.0.8
     # via cachecontrol
 multidict==6.0.5
     # via
     #   aiohttp
     #   yarl
 multiprocess==0.70.16
     # via
     #   datasets
     #   evaluate
-myst-nb==1.0.0
+myst-nb==1.1.0
     # via physicsml (pyproject.toml)
-myst-parser==2.0.0
+myst-parser==3.0.0
     # via myst-nb
 natsort==8.4.0
     # via domdf-python-tools
-nbclient==0.9.0
+nbclient==0.10.0
     # via
     #   jupyter-cache
     #   myst-nb
-nbformat==5.9.2
+nbformat==5.10.4
     # via
     #   jupyter-cache
     #   jupytext
     #   myst-nb
     #   nbclient
 nest-asyncio==1.6.0
     # via ipykernel
-networkx==3.2.1
+networkx==3.3
     # via torch
 numpy==1.26.4
     # via
     #   ase
     #   contourpy
     #   datasets
     #   evaluate
@@ -307,22 +301,21 @@
     #   opt-einsum
     #   pandas
     #   pyarrow
     #   pytorch-lightning
     #   rdkit
     #   scikit-learn
     #   scipy
-    #   tensorboard
     #   torch-geometric
     #   torchmetrics
 opt-einsum==3.3.0
     # via opt-einsum-fx
 opt-einsum-fx==0.1.4
     # via e3nn
-packaging==23.2
+packaging==24.0
     # via
     #   datasets
     #   evaluate
     #   huggingface-hub
     #   ipykernel
     #   jupytext
     #   lightning
@@ -330,114 +323,111 @@
     #   matplotlib
     #   opt-einsum-fx
     #   pydata-sphinx-theme
     #   pytest
     #   pytorch-lightning
     #   sphinx
     #   torchmetrics
-pandas==2.2.0
+pandas==2.2.2
     # via
     #   datasets
     #   evaluate
     #   molflux
-parso==0.8.3
+parso==0.8.4
     # via jedi
 pexpect==4.9.0
     # via ipython
-pillow==10.2.0
+pillow==10.3.0
     # via
     #   matplotlib
     #   rdkit
-platformdirs==4.2.0
+platformdirs==4.2.1
     # via
     #   apeye
     #   jupyter-core
-pluggy==1.4.0
+pluggy==1.5.0
     # via pytest
 prompt-toolkit==3.0.43
     # via ipython
-protobuf==4.25.3
-    # via tensorboard
 psutil==5.9.8
     # via
     #   ipykernel
     #   torch-geometric
 ptyprocess==0.7.0
     # via pexpect
 pure-eval==0.2.2
     # via stack-data
-pyarrow==15.0.0
+pyarrow==16.0.0
     # via
     #   datasets
     #   molflux
 pyarrow-hotfix==0.6
     # via datasets
-pydantic==1.10.14
+pydantic==1.10.15
     # via molflux
 pydata-sphinx-theme==0.15.2
     # via sphinx-book-theme
 pygments==2.17.2
     # via
     #   accessible-pygments
     #   ipython
     #   pydata-sphinx-theme
     #   sphinx
     #   sphinx-prompt
     #   sphinx-tabs
-pyparsing==3.1.1
+pyparsing==3.1.2
     # via
     #   matplotlib
     #   torch-geometric
-pytest==8.0.1
+pytest==8.1.1
     # via physicsml (pyproject.toml)
-python-dateutil==2.8.2
+python-dateutil==2.9.0.post0
     # via
     #   botocore
     #   jupyter-client
     #   matplotlib
     #   molflux
     #   pandas
-pytorch-lightning==2.2.0.post0
+pytorch-lightning==2.2.3
     # via lightning
 pytz==2024.1
     # via pandas
 pyyaml==6.0.1
     # via
     #   datasets
     #   huggingface-hub
     #   jupyter-cache
     #   jupytext
     #   lightning
     #   molflux
     #   myst-nb
     #   myst-parser
     #   pytorch-lightning
-pyzmq==25.1.2
+pyzmq==26.0.2
     # via
     #   ipykernel
     #   jupyter-client
 qlient==1.0.0
     # via molflux
 qlient-core==1.0.1
     # via qlient
-rapidfuzz==3.6.1
+rapidfuzz==3.8.1
     # via thefuzz
 rdkit==2023.9.5
     # via physicsml (pyproject.toml)
-referencing==0.33.0
+referencing==0.35.0
     # via
     #   jsonschema
     #   jsonschema-specifications
 requests==2.31.0
     # via
     #   apeye
     #   cachecontrol
     #   datasets
     #   evaluate
-    #   fsspec
     #   huggingface-hub
     #   molflux
     #   qlient
     #   responses
     #   sphinx
     #   torch-geometric
     #   torchani
@@ -447,38 +437,37 @@
     # via
     #   jsonschema
     #   referencing
 ruamel-yaml==0.18.6
     # via sphinx-toolbox
 ruamel-yaml-clib==0.2.8
     # via ruamel-yaml
-s3transfer==0.10.0
+s3transfer==0.10.1
     # via boto3
-scikit-learn==1.4.1.post1
+scikit-learn==1.4.2
     # via
     #   molflux
     #   torch-geometric
-scipy==1.12.0
+scipy==1.13.0
     # via
     #   ase
     #   e3nn
     #   molflux
     #   scikit-learn
     #   torch-geometric
 six==1.16.0
     # via
     #   asttokens
     #   html5lib
     #   python-dateutil
-    #   tensorboard
 snowballstemmer==2.2.0
     # via sphinx
 soupsieve==2.5
     # via beautifulsoup4
-sphinx==7.2.6
+sphinx==7.3.7
     # via
     #   autodocsumm
     #   myst-nb
     #   myst-parser
     #   physicsml (pyproject.toml)
     #   pydata-sphinx-theme
     #   sphinx-autodoc-typehints
@@ -486,15 +475,15 @@
     #   sphinx-design
     #   sphinx-inline-tabs
     #   sphinx-prompt
     #   sphinx-sitemap
     #   sphinx-tabs
     #   sphinx-togglebutton
     #   sphinx-toolbox
-sphinx-autodoc-typehints==2.0.0
+sphinx-autodoc-typehints==2.1.0
     # via sphinx-toolbox
 sphinx-book-theme==1.1.2
     # via physicsml (pyproject.toml)
 sphinx-design==0.5.0
     # via physicsml (pyproject.toml)
 sphinx-inline-tabs==2023.4.21
     # via physicsml (pyproject.toml)
@@ -518,56 +507,53 @@
     # via sphinx
 sphinxcontrib-jsmath==1.0.1
     # via sphinx
 sphinxcontrib-qthelp==1.0.7
     # via sphinx
 sphinxcontrib-serializinghtml==1.1.10
     # via sphinx
-sqlalchemy==2.0.27
+sqlalchemy==2.0.29
     # via jupyter-cache
 stack-data==0.6.3
     # via ipython
 sympy==1.12
     # via
     #   e3nn
     #   torch
 tabulate==0.9.0
     # via
     #   jupyter-cache
     #   sphinx-toolbox
 tenacity==8.2.3
     # via molflux
-tensorboard==2.16.2
-    # via physicsml (pyproject.toml)
-tensorboard-data-server==0.7.2
-    # via tensorboard
 thefuzz==0.22.1
     # via molflux
-threadpoolctl==3.3.0
+threadpoolctl==3.4.0
     # via scikit-learn
 toml==0.10.2
     # via jupytext
 tomli==2.0.1
     # via
     #   coverage
     #   pytest
-torch==2.0.1
+    #   sphinx
+torch==2.3.0
     # via
     #   e3nn
     #   lightning
     #   opt-einsum-fx
     #   physicsml (pyproject.toml)
     #   pytorch-lightning
     #   torchani
     #   torchmetrics
-torch-geometric==2.5.0
+torch-geometric==2.5.3
     # via physicsml (pyproject.toml)
 torchani==2.2.3
     # via physicsml (pyproject.toml)
-torchmetrics==1.3.1
+torchmetrics==1.3.2
     # via
     #   lightning
     #   pytorch-lightning
 tornado==6.4
     # via
     #   ipykernel
     #   jupyter-client
@@ -576,63 +562,62 @@
     #   datasets
     #   evaluate
     #   huggingface-hub
     #   lightning
     #   molflux
     #   pytorch-lightning
     #   torch-geometric
-traitlets==5.14.1
+traitlets==5.14.3
     # via
     #   comm
     #   ipykernel
     #   ipython
     #   ipywidgets
     #   jupyter-client
     #   jupyter-core
     #   matplotlib-inline
     #   nbclient
     #   nbformat
-typing-extensions==4.9.0
+typing-extensions==4.11.0
     # via
     #   cloudpathlib
     #   domdf-python-tools
     #   huggingface-hub
+    #   ipython
     #   lightning
     #   lightning-utilities
     #   molflux
     #   myst-nb
     #   pydantic
     #   pydata-sphinx-theme
     #   pytorch-lightning
     #   sphinx-toolbox
     #   sqlalchemy
     #   torch
 tzdata==2024.1
     # via pandas
-urllib3==2.0.7
+urllib3==2.2.1
     # via
     #   botocore
     #   requests
     #   responses
 wcwidth==0.2.13
     # via prompt-toolkit
 webencodings==0.5.1
     # via html5lib
-websocket-client==1.7.0
+websocket-client==1.8.0
     # via qlient
-werkzeug==3.0.1
-    # via tensorboard
-wheel==0.42.0
+wheel==0.43.0
     # via sphinx-togglebutton
 widgetsnbextension==4.0.10
     # via ipywidgets
 xxhash==3.4.1
     # via
     #   datasets
     #   evaluate
 yarl==1.9.4
     # via aiohttp
-zipp==3.17.0
+zipp==3.18.1
     # via importlib-metadata
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `physicsml-0.2.3/pinned-versions/3.10/lockfile.rdkit.txt` & `physicsml-0.2.4/pinned-versions/3.10/lockfile.openeye.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 #
 # This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
-#    nox -s dependencies_pin-3.10(extra='rdkit')
+#    nox -s dependencies_pin-3.10(extra='openeye')
 #
-absl-py==2.1.0
-    # via tensorboard
 accessible-pygments==0.0.4
     # via pydata-sphinx-theme
-aiohttp==3.9.3
+aiohttp==3.9.5
     # via
     #   datasets
     #   fsspec
     #   torch-geometric
 aiosignal==1.3.1
     # via aiohttp
 alabaster==0.7.16
@@ -41,67 +39,67 @@
     # via
     #   pydata-sphinx-theme
     #   sphinx
 beautifulsoup4==4.12.3
     # via
     #   pydata-sphinx-theme
     #   sphinx-toolbox
-boto3==1.34.45
+boto3==1.34.91
     # via
     #   cloudpathlib
     #   molflux
-botocore==1.34.45
+botocore==1.34.91
     # via
     #   boto3
     #   molflux
     #   s3transfer
 cachecontrol==0.14.0
     # via sphinx-toolbox
 certifi==2024.2.2
     # via requests
 charset-normalizer==3.3.2
     # via requests
 click==8.1.7
     # via jupyter-cache
-cloudpathlib==0.17.0
+cloudpathlib==0.18.1
     # via molflux
 colorama==0.4.6
     # via molflux
-comm==0.2.1
+comm==0.2.2
     # via
     #   ipykernel
     #   ipywidgets
-contourpy==1.2.0
+contourpy==1.2.1
     # via matplotlib
-coverage==7.4.1
+coverage==7.5.0
     # via
     #   coverage-badge
     #   physicsml (pyproject.toml)
-coverage-badge==1.1.0
+coverage-badge==1.1.1
     # via physicsml (pyproject.toml)
-cssutils==2.9.0
+cssutils==2.10.2
     # via dict2css
 cycler==0.12.1
     # via matplotlib
-datasets==2.17.1
+datasets==2.19.0
     # via
     #   evaluate
     #   molflux
 debugpy==1.8.1
     # via ipykernel
 decorator==5.1.1
     # via ipython
 dict2css==0.3.0.post1
     # via sphinx-toolbox
 dill==0.3.8
     # via
     #   datasets
     #   evaluate
     #   multiprocess
-docutils==0.20.1
+docutils==0.21.2
     # via
     #   myst-parser
     #   pydata-sphinx-theme
     #   sphinx
     #   sphinx-prompt
     #   sphinx-tabs
     #   sphinx-togglebutton
@@ -112,74 +110,73 @@
     #   apeye-core
     #   dict2css
     #   sphinx-toolbox
 e3nn==0.5.1
     # via physicsml (pyproject.toml)
 evaluate==0.4.1
     # via molflux
-exceptiongroup==1.2.0
+exceptiongroup==1.2.1
     # via
     #   ipython
     #   pytest
 executing==2.0.1
     # via stack-data
 fastjsonschema==2.19.1
     # via nbformat
-filelock==3.13.1
+filelock==3.13.4
     # via
     #   cachecontrol
     #   datasets
     #   huggingface-hub
     #   sphinx-toolbox
     #   torch
-fonttools==4.49.0
+fonttools==4.51.0
     # via matplotlib
 frozenlist==1.4.1
     # via
     #   aiohttp
     #   aiosignal
-fsspec==2023.10.0
+fsspec==2024.3.1
     # via
     #   datasets
     #   evaluate
     #   huggingface-hub
     #   lightning
     #   molflux
     #   pytorch-lightning
+    #   torch
     #   torch-geometric
-grpcio==1.60.1
-    # via tensorboard
-h5py==3.10.0
+h5py==3.11.0
     # via
     #   molflux
     #   physicsml (pyproject.toml)
 html5lib==1.1
     # via sphinx-toolbox
-huggingface-hub==0.20.3
+huggingface-hub==0.22.2
     # via
     #   datasets
     #   evaluate
-idna==3.6
+idna==3.7
     # via
     #   apeye-core
     #   requests
     #   yarl
 imagesize==1.4.1
     # via sphinx
 importlib-metadata==4.13.0
     # via
     #   jupyter-cache
     #   myst-nb
     #   qlient-core
     #   torchani
 iniconfig==2.0.0
     # via pytest
-ipykernel==6.29.2
+ipykernel==6.29.4
     # via myst-nb
-ipython==8.21.0
+ipython==8.23.0
     # via
     #   ipykernel
     #   ipywidgets
     #   myst-nb
 ipywidgets==8.1.2
     # via physicsml (pyproject.toml)
 jedi==0.19.1
@@ -191,66 +188,63 @@
     #   sphinx-jinja2-compat
     #   torch
     #   torch-geometric
 jmespath==1.0.1
     # via
     #   boto3
     #   botocore
-joblib==1.3.2
+joblib==1.4.0
     # via
     #   molflux
     #   scikit-learn
 jsonschema==4.21.1
     # via nbformat
 jsonschema-specifications==2023.12.1
     # via jsonschema
 jupyter-cache==1.0.0
     # via myst-nb
-jupyter-client==8.6.0
+jupyter-client==8.6.1
     # via
     #   ipykernel
     #   nbclient
-jupyter-core==5.7.1
+jupyter-core==5.7.2
     # via
     #   ipykernel
     #   jupyter-client
     #   nbclient
     #   nbformat
 jupyterlab-widgets==3.0.10
     # via ipywidgets
 jupytext==1.16.1
     # via physicsml (pyproject.toml)
 kiwisolver==1.4.5
     # via matplotlib
 lark-parser==0.12.0
     # via torchani
-lightning==2.2.0.post0
+lightning==2.2.3
     # via physicsml (pyproject.toml)
-lightning-utilities==0.10.1
+lightning-utilities==0.11.2
     # via
     #   lightning
     #   pytorch-lightning
     #   torchmetrics
-markdown==3.5.2
-    # via tensorboard
 markdown-it-py==3.0.0
     # via
     #   jupytext
     #   mdit-py-plugins
     #   myst-parser
 markupsafe==2.1.5
     # via
     #   jinja2
     #   sphinx-jinja2-compat
-    #   werkzeug
-matplotlib==3.8.3
+matplotlib==3.8.4
     # via
     #   ase
     #   physicsml (pyproject.toml)
-matplotlib-inline==0.1.6
+matplotlib-inline==0.1.7
     # via
     #   ipykernel
     #   ipython
 mdit-py-plugins==0.4.0
     # via
     #   jupytext
     #   myst-parser
@@ -260,43 +254,43 @@
     # via molflux
 molflux==0.3.0
     # via physicsml (pyproject.toml)
 more-itertools==10.2.0
     # via molflux
 mpmath==1.3.0
     # via sympy
-msgpack==1.0.7
+msgpack==1.0.8
     # via cachecontrol
 multidict==6.0.5
     # via
     #   aiohttp
     #   yarl
 multiprocess==0.70.16
     # via
     #   datasets
     #   evaluate
-myst-nb==1.0.0
+myst-nb==1.1.0
     # via physicsml (pyproject.toml)
-myst-parser==2.0.0
+myst-parser==3.0.0
     # via myst-nb
 natsort==8.4.0
     # via domdf-python-tools
-nbclient==0.9.0
+nbclient==0.10.0
     # via
     #   jupyter-cache
     #   myst-nb
-nbformat==5.9.2
+nbformat==5.10.4
     # via
     #   jupyter-cache
     #   jupytext
     #   myst-nb
     #   nbclient
 nest-asyncio==1.6.0
     # via ipykernel
-networkx==3.2.1
+networkx==3.3
     # via torch
 numpy==1.26.4
     # via
     #   ase
     #   contourpy
     #   datasets
     #   evaluate
@@ -307,22 +301,23 @@
     #   opt-einsum
     #   pandas
     #   pyarrow
     #   pytorch-lightning
     #   rdkit
     #   scikit-learn
     #   scipy
-    #   tensorboard
     #   torch-geometric
     #   torchmetrics
+openeye-toolkits==2023.2.3
+    # via physicsml (pyproject.toml)
 opt-einsum==3.3.0
     # via opt-einsum-fx
 opt-einsum-fx==0.1.4
     # via e3nn
-packaging==23.2
+packaging==24.0
     # via
     #   datasets
     #   evaluate
     #   huggingface-hub
     #   ipykernel
     #   jupytext
     #   lightning
@@ -330,114 +325,111 @@
     #   matplotlib
     #   opt-einsum-fx
     #   pydata-sphinx-theme
     #   pytest
     #   pytorch-lightning
     #   sphinx
     #   torchmetrics
-pandas==2.2.0
+pandas==2.2.2
     # via
     #   datasets
     #   evaluate
     #   molflux
-parso==0.8.3
+parso==0.8.4
     # via jedi
 pexpect==4.9.0
     # via ipython
-pillow==10.2.0
+pillow==10.3.0
     # via
     #   matplotlib
     #   rdkit
-platformdirs==4.2.0
+platformdirs==4.2.1
     # via
     #   apeye
     #   jupyter-core
-pluggy==1.4.0
+pluggy==1.5.0
     # via pytest
 prompt-toolkit==3.0.43
     # via ipython
-protobuf==4.25.3
-    # via tensorboard
 psutil==5.9.8
     # via
     #   ipykernel
     #   torch-geometric
 ptyprocess==0.7.0
     # via pexpect
 pure-eval==0.2.2
     # via stack-data
-pyarrow==15.0.0
+pyarrow==16.0.0
     # via
     #   datasets
     #   molflux
 pyarrow-hotfix==0.6
     # via datasets
-pydantic==1.10.14
+pydantic==1.10.15
     # via molflux
 pydata-sphinx-theme==0.15.2
     # via sphinx-book-theme
 pygments==2.17.2
     # via
     #   accessible-pygments
     #   ipython
     #   pydata-sphinx-theme
     #   sphinx
     #   sphinx-prompt
     #   sphinx-tabs
-pyparsing==3.1.1
+pyparsing==3.1.2
     # via
     #   matplotlib
     #   torch-geometric
-pytest==8.0.1
+pytest==8.1.1
     # via physicsml (pyproject.toml)
-python-dateutil==2.8.2
+python-dateutil==2.9.0.post0
     # via
     #   botocore
     #   jupyter-client
     #   matplotlib
     #   molflux
     #   pandas
-pytorch-lightning==2.2.0.post0
+pytorch-lightning==2.2.3
     # via lightning
 pytz==2024.1
     # via pandas
 pyyaml==6.0.1
     # via
     #   datasets
     #   huggingface-hub
     #   jupyter-cache
     #   jupytext
     #   lightning
     #   molflux
     #   myst-nb
     #   myst-parser
     #   pytorch-lightning
-pyzmq==25.1.2
+pyzmq==26.0.2
     # via
     #   ipykernel
     #   jupyter-client
 qlient==1.0.0
     # via molflux
 qlient-core==1.0.1
     # via qlient
-rapidfuzz==3.6.1
+rapidfuzz==3.8.1
     # via thefuzz
 rdkit==2023.9.5
     # via physicsml (pyproject.toml)
-referencing==0.33.0
+referencing==0.35.0
     # via
     #   jsonschema
     #   jsonschema-specifications
 requests==2.31.0
     # via
     #   apeye
     #   cachecontrol
     #   datasets
     #   evaluate
-    #   fsspec
     #   huggingface-hub
     #   molflux
     #   qlient
     #   responses
     #   sphinx
     #   torch-geometric
     #   torchani
@@ -447,38 +439,37 @@
     # via
     #   jsonschema
     #   referencing
 ruamel-yaml==0.18.6
     # via sphinx-toolbox
 ruamel-yaml-clib==0.2.8
     # via ruamel-yaml
-s3transfer==0.10.0
+s3transfer==0.10.1
     # via boto3
-scikit-learn==1.4.1.post1
+scikit-learn==1.4.2
     # via
     #   molflux
     #   torch-geometric
-scipy==1.12.0
+scipy==1.13.0
     # via
     #   ase
     #   e3nn
     #   molflux
     #   scikit-learn
     #   torch-geometric
 six==1.16.0
     # via
     #   asttokens
     #   html5lib
     #   python-dateutil
-    #   tensorboard
 snowballstemmer==2.2.0
     # via sphinx
 soupsieve==2.5
     # via beautifulsoup4
-sphinx==7.2.6
+sphinx==7.3.7
     # via
     #   autodocsumm
     #   myst-nb
     #   myst-parser
     #   physicsml (pyproject.toml)
     #   pydata-sphinx-theme
     #   sphinx-autodoc-typehints
@@ -486,15 +477,15 @@
     #   sphinx-design
     #   sphinx-inline-tabs
     #   sphinx-prompt
     #   sphinx-sitemap
     #   sphinx-tabs
     #   sphinx-togglebutton
     #   sphinx-toolbox
-sphinx-autodoc-typehints==2.0.0
+sphinx-autodoc-typehints==2.1.0
     # via sphinx-toolbox
 sphinx-book-theme==1.1.2
     # via physicsml (pyproject.toml)
 sphinx-design==0.5.0
     # via physicsml (pyproject.toml)
 sphinx-inline-tabs==2023.4.21
     # via physicsml (pyproject.toml)
@@ -518,56 +509,53 @@
     # via sphinx
 sphinxcontrib-jsmath==1.0.1
     # via sphinx
 sphinxcontrib-qthelp==1.0.7
     # via sphinx
 sphinxcontrib-serializinghtml==1.1.10
     # via sphinx
-sqlalchemy==2.0.27
+sqlalchemy==2.0.29
     # via jupyter-cache
 stack-data==0.6.3
     # via ipython
 sympy==1.12
     # via
     #   e3nn
     #   torch
 tabulate==0.9.0
     # via
     #   jupyter-cache
     #   sphinx-toolbox
 tenacity==8.2.3
     # via molflux
-tensorboard==2.16.2
-    # via physicsml (pyproject.toml)
-tensorboard-data-server==0.7.2
-    # via tensorboard
 thefuzz==0.22.1
     # via molflux
-threadpoolctl==3.3.0
+threadpoolctl==3.4.0
     # via scikit-learn
 toml==0.10.2
     # via jupytext
 tomli==2.0.1
     # via
     #   coverage
     #   pytest
-torch==2.0.1
+    #   sphinx
+torch==2.3.0
     # via
     #   e3nn
     #   lightning
     #   opt-einsum-fx
     #   physicsml (pyproject.toml)
     #   pytorch-lightning
     #   torchani
     #   torchmetrics
-torch-geometric==2.5.0
+torch-geometric==2.5.3
     # via physicsml (pyproject.toml)
 torchani==2.2.3
     # via physicsml (pyproject.toml)
-torchmetrics==1.3.1
+torchmetrics==1.3.2
     # via
     #   lightning
     #   pytorch-lightning
 tornado==6.4
     # via
     #   ipykernel
     #   jupyter-client
@@ -576,63 +564,62 @@
     #   datasets
     #   evaluate
     #   huggingface-hub
     #   lightning
     #   molflux
     #   pytorch-lightning
     #   torch-geometric
-traitlets==5.14.1
+traitlets==5.14.3
     # via
     #   comm
     #   ipykernel
     #   ipython
     #   ipywidgets
     #   jupyter-client
     #   jupyter-core
     #   matplotlib-inline
     #   nbclient
     #   nbformat
-typing-extensions==4.9.0
+typing-extensions==4.11.0
     # via
     #   cloudpathlib
     #   domdf-python-tools
     #   huggingface-hub
+    #   ipython
     #   lightning
     #   lightning-utilities
     #   molflux
     #   myst-nb
     #   pydantic
     #   pydata-sphinx-theme
     #   pytorch-lightning
     #   sphinx-toolbox
     #   sqlalchemy
     #   torch
 tzdata==2024.1
     # via pandas
-urllib3==2.0.7
+urllib3==2.2.1
     # via
     #   botocore
     #   requests
     #   responses
 wcwidth==0.2.13
     # via prompt-toolkit
 webencodings==0.5.1
     # via html5lib
-websocket-client==1.7.0
+websocket-client==1.8.0
     # via qlient
-werkzeug==3.0.1
-    # via tensorboard
-wheel==0.42.0
+wheel==0.43.0
     # via sphinx-togglebutton
 widgetsnbextension==4.0.10
     # via ipywidgets
 xxhash==3.4.1
     # via
     #   datasets
     #   evaluate
 yarl==1.9.4
     # via aiohttp
-zipp==3.17.0
+zipp==3.18.1
     # via importlib-metadata
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `physicsml-0.2.3/pinned-versions/3.11/lockfile.ase.txt` & `physicsml-0.2.4/pinned-versions/3.11/lockfile.rdkit.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 #
 # This file is autogenerated by pip-compile with Python 3.11
 # by the following command:
 #
-#    nox -s dependencies_pin-3.11(extra='ase')
+#    nox -s dependencies_pin-3.11(extra='rdkit')
 #
-absl-py==2.1.0
-    # via tensorboard
 accessible-pygments==0.0.4
     # via pydata-sphinx-theme
-aiohttp==3.9.3
+aiohttp==3.9.5
     # via
     #   datasets
     #   fsspec
     #   torch-geometric
 aiosignal==1.3.1
     # via aiohttp
 alabaster==0.7.16
@@ -39,67 +37,67 @@
     # via
     #   pydata-sphinx-theme
     #   sphinx
 beautifulsoup4==4.12.3
     # via
     #   pydata-sphinx-theme
     #   sphinx-toolbox
-boto3==1.34.45
+boto3==1.34.91
     # via
     #   cloudpathlib
     #   molflux
-botocore==1.34.45
+botocore==1.34.91
     # via
     #   boto3
     #   molflux
     #   s3transfer
 cachecontrol==0.14.0
     # via sphinx-toolbox
 certifi==2024.2.2
     # via requests
 charset-normalizer==3.3.2
     # via requests
 click==8.1.7
     # via jupyter-cache
-cloudpathlib==0.17.0
+cloudpathlib==0.18.1
     # via molflux
 colorama==0.4.6
     # via molflux
-comm==0.2.1
+comm==0.2.2
     # via
     #   ipykernel
     #   ipywidgets
-contourpy==1.2.0
+contourpy==1.2.1
     # via matplotlib
-coverage==7.4.1
+coverage==7.5.0
     # via
     #   coverage-badge
     #   physicsml (pyproject.toml)
-coverage-badge==1.1.0
+coverage-badge==1.1.1
     # via physicsml (pyproject.toml)
-cssutils==2.9.0
+cssutils==2.10.2
     # via dict2css
 cycler==0.12.1
     # via matplotlib
-datasets==2.17.1
+datasets==2.19.0
     # via
     #   evaluate
     #   molflux
 debugpy==1.8.1
     # via ipykernel
 decorator==5.1.1
     # via ipython
 dict2css==0.3.0.post1
     # via sphinx-toolbox
 dill==0.3.8
     # via
     #   datasets
     #   evaluate
     #   multiprocess
-docutils==0.20.1
+docutils==0.21.2
     # via
     #   myst-parser
     #   pydata-sphinx-theme
     #   sphinx
     #   sphinx-prompt
     #   sphinx-tabs
     #   sphinx-togglebutton
@@ -114,66 +112,65 @@
     # via physicsml (pyproject.toml)
 evaluate==0.4.1
     # via molflux
 executing==2.0.1
     # via stack-data
 fastjsonschema==2.19.1
     # via nbformat
-filelock==3.13.1
+filelock==3.13.4
     # via
     #   cachecontrol
     #   datasets
     #   huggingface-hub
     #   sphinx-toolbox
     #   torch
-fonttools==4.49.0
+fonttools==4.51.0
     # via matplotlib
 frozenlist==1.4.1
     # via
     #   aiohttp
     #   aiosignal
-fsspec==2023.10.0
+fsspec==2024.3.1
     # via
     #   datasets
     #   evaluate
     #   huggingface-hub
     #   lightning
     #   molflux
     #   pytorch-lightning
+    #   torch
     #   torch-geometric
-grpcio==1.60.1
-    # via tensorboard
-h5py==3.10.0
+h5py==3.11.0
     # via
     #   molflux
     #   physicsml (pyproject.toml)
 html5lib==1.1
     # via sphinx-toolbox
-huggingface-hub==0.20.3
+huggingface-hub==0.22.2
     # via
     #   datasets
     #   evaluate
-idna==3.6
+idna==3.7
     # via
     #   apeye-core
     #   requests
     #   yarl
 imagesize==1.4.1
     # via sphinx
 importlib-metadata==4.13.0
     # via
     #   jupyter-cache
     #   myst-nb
     #   qlient-core
     #   torchani
 iniconfig==2.0.0
     # via pytest
-ipykernel==6.29.2
+ipykernel==6.29.4
     # via myst-nb
-ipython==8.21.0
+ipython==8.23.0
     # via
     #   ipykernel
     #   ipywidgets
     #   myst-nb
 ipywidgets==8.1.2
     # via physicsml (pyproject.toml)
 jedi==0.19.1
@@ -185,66 +182,63 @@
     #   sphinx-jinja2-compat
     #   torch
     #   torch-geometric
 jmespath==1.0.1
     # via
     #   boto3
     #   botocore
-joblib==1.3.2
+joblib==1.4.0
     # via
     #   molflux
     #   scikit-learn
 jsonschema==4.21.1
     # via nbformat
 jsonschema-specifications==2023.12.1
     # via jsonschema
 jupyter-cache==1.0.0
     # via myst-nb
-jupyter-client==8.6.0
+jupyter-client==8.6.1
     # via
     #   ipykernel
     #   nbclient
-jupyter-core==5.7.1
+jupyter-core==5.7.2
     # via
     #   ipykernel
     #   jupyter-client
     #   nbclient
     #   nbformat
 jupyterlab-widgets==3.0.10
     # via ipywidgets
 jupytext==1.16.1
     # via physicsml (pyproject.toml)
 kiwisolver==1.4.5
     # via matplotlib
 lark-parser==0.12.0
     # via torchani
-lightning==2.2.0.post0
+lightning==2.2.3
     # via physicsml (pyproject.toml)
-lightning-utilities==0.10.1
+lightning-utilities==0.11.2
     # via
     #   lightning
     #   pytorch-lightning
     #   torchmetrics
-markdown==3.5.2
-    # via tensorboard
 markdown-it-py==3.0.0
     # via
     #   jupytext
     #   mdit-py-plugins
     #   myst-parser
 markupsafe==2.1.5
     # via
     #   jinja2
     #   sphinx-jinja2-compat
-    #   werkzeug
-matplotlib==3.8.3
+matplotlib==3.8.4
     # via
     #   ase
     #   physicsml (pyproject.toml)
-matplotlib-inline==0.1.6
+matplotlib-inline==0.1.7
     # via
     #   ipykernel
     #   ipython
 mdit-py-plugins==0.4.0
     # via
     #   jupytext
     #   myst-parser
@@ -254,43 +248,43 @@
     # via molflux
 molflux==0.3.0
     # via physicsml (pyproject.toml)
 more-itertools==10.2.0
     # via molflux
 mpmath==1.3.0
     # via sympy
-msgpack==1.0.7
+msgpack==1.0.8
     # via cachecontrol
 multidict==6.0.5
     # via
     #   aiohttp
     #   yarl
 multiprocess==0.70.16
     # via
     #   datasets
     #   evaluate
-myst-nb==1.0.0
+myst-nb==1.1.0
     # via physicsml (pyproject.toml)
-myst-parser==2.0.0
+myst-parser==3.0.0
     # via myst-nb
 natsort==8.4.0
     # via domdf-python-tools
-nbclient==0.9.0
+nbclient==0.10.0
     # via
     #   jupyter-cache
     #   myst-nb
-nbformat==5.9.2
+nbformat==5.10.4
     # via
     #   jupyter-cache
     #   jupytext
     #   myst-nb
     #   nbclient
 nest-asyncio==1.6.0
     # via ipykernel
-networkx==3.2.1
+networkx==3.3
     # via torch
 numpy==1.26.4
     # via
     #   ase
     #   contourpy
     #   datasets
     #   evaluate
@@ -301,22 +295,21 @@
     #   opt-einsum
     #   pandas
     #   pyarrow
     #   pytorch-lightning
     #   rdkit
     #   scikit-learn
     #   scipy
-    #   tensorboard
     #   torch-geometric
     #   torchmetrics
 opt-einsum==3.3.0
     # via opt-einsum-fx
 opt-einsum-fx==0.1.4
     # via e3nn
-packaging==23.2
+packaging==24.0
     # via
     #   datasets
     #   evaluate
     #   huggingface-hub
     #   ipykernel
     #   jupytext
     #   lightning
@@ -324,114 +317,111 @@
     #   matplotlib
     #   opt-einsum-fx
     #   pydata-sphinx-theme
     #   pytest
     #   pytorch-lightning
     #   sphinx
     #   torchmetrics
-pandas==2.2.0
+pandas==2.2.2
     # via
     #   datasets
     #   evaluate
     #   molflux
-parso==0.8.3
+parso==0.8.4
     # via jedi
 pexpect==4.9.0
     # via ipython
-pillow==10.2.0
+pillow==10.3.0
     # via
     #   matplotlib
     #   rdkit
-platformdirs==4.2.0
+platformdirs==4.2.1
     # via
     #   apeye
     #   jupyter-core
-pluggy==1.4.0
+pluggy==1.5.0
     # via pytest
 prompt-toolkit==3.0.43
     # via ipython
-protobuf==4.25.3
-    # via tensorboard
 psutil==5.9.8
     # via
     #   ipykernel
     #   torch-geometric
 ptyprocess==0.7.0
     # via pexpect
 pure-eval==0.2.2
     # via stack-data
-pyarrow==15.0.0
+pyarrow==16.0.0
     # via
     #   datasets
     #   molflux
 pyarrow-hotfix==0.6
     # via datasets
-pydantic==1.10.14
+pydantic==1.10.15
     # via molflux
 pydata-sphinx-theme==0.15.2
     # via sphinx-book-theme
 pygments==2.17.2
     # via
     #   accessible-pygments
     #   ipython
     #   pydata-sphinx-theme
     #   sphinx
     #   sphinx-prompt
     #   sphinx-tabs
-pyparsing==3.1.1
+pyparsing==3.1.2
     # via
     #   matplotlib
     #   torch-geometric
-pytest==8.0.1
+pytest==8.1.1
     # via physicsml (pyproject.toml)
-python-dateutil==2.8.2
+python-dateutil==2.9.0.post0
     # via
     #   botocore
     #   jupyter-client
     #   matplotlib
     #   molflux
     #   pandas
-pytorch-lightning==2.2.0.post0
+pytorch-lightning==2.2.3
     # via lightning
 pytz==2024.1
     # via pandas
 pyyaml==6.0.1
     # via
     #   datasets
     #   huggingface-hub
     #   jupyter-cache
     #   jupytext
     #   lightning
     #   molflux
     #   myst-nb
     #   myst-parser
     #   pytorch-lightning
-pyzmq==25.1.2
+pyzmq==26.0.2
     # via
     #   ipykernel
     #   jupyter-client
 qlient==1.0.0
     # via molflux
 qlient-core==1.0.1
     # via qlient
-rapidfuzz==3.6.1
+rapidfuzz==3.8.1
     # via thefuzz
 rdkit==2023.9.5
     # via physicsml (pyproject.toml)
-referencing==0.33.0
+referencing==0.35.0
     # via
     #   jsonschema
     #   jsonschema-specifications
 requests==2.31.0
     # via
     #   apeye
     #   cachecontrol
     #   datasets
     #   evaluate
-    #   fsspec
     #   huggingface-hub
     #   molflux
     #   qlient
     #   responses
     #   sphinx
     #   torch-geometric
     #   torchani
@@ -441,38 +431,37 @@
     # via
     #   jsonschema
     #   referencing
 ruamel-yaml==0.18.6
     # via sphinx-toolbox
 ruamel-yaml-clib==0.2.8
     # via ruamel-yaml
-s3transfer==0.10.0
+s3transfer==0.10.1
     # via boto3
-scikit-learn==1.4.1.post1
+scikit-learn==1.4.2
     # via
     #   molflux
     #   torch-geometric
-scipy==1.12.0
+scipy==1.13.0
     # via
     #   ase
     #   e3nn
     #   molflux
     #   scikit-learn
     #   torch-geometric
 six==1.16.0
     # via
     #   asttokens
     #   html5lib
     #   python-dateutil
-    #   tensorboard
 snowballstemmer==2.2.0
     # via sphinx
 soupsieve==2.5
     # via beautifulsoup4
-sphinx==7.2.6
+sphinx==7.3.7
     # via
     #   autodocsumm
     #   myst-nb
     #   myst-parser
     #   physicsml (pyproject.toml)
     #   pydata-sphinx-theme
     #   sphinx-autodoc-typehints
@@ -480,15 +469,15 @@
     #   sphinx-design
     #   sphinx-inline-tabs
     #   sphinx-prompt
     #   sphinx-sitemap
     #   sphinx-tabs
     #   sphinx-togglebutton
     #   sphinx-toolbox
-sphinx-autodoc-typehints==2.0.0
+sphinx-autodoc-typehints==2.1.0
     # via sphinx-toolbox
 sphinx-book-theme==1.1.2
     # via physicsml (pyproject.toml)
 sphinx-design==0.5.0
     # via physicsml (pyproject.toml)
 sphinx-inline-tabs==2023.4.21
     # via physicsml (pyproject.toml)
@@ -512,52 +501,48 @@
     # via sphinx
 sphinxcontrib-jsmath==1.0.1
     # via sphinx
 sphinxcontrib-qthelp==1.0.7
     # via sphinx
 sphinxcontrib-serializinghtml==1.1.10
     # via sphinx
-sqlalchemy==2.0.27
+sqlalchemy==2.0.29
     # via jupyter-cache
 stack-data==0.6.3
     # via ipython
 sympy==1.12
     # via
     #   e3nn
     #   torch
 tabulate==0.9.0
     # via
     #   jupyter-cache
     #   sphinx-toolbox
 tenacity==8.2.3
     # via molflux
-tensorboard==2.16.2
-    # via physicsml (pyproject.toml)
-tensorboard-data-server==0.7.2
-    # via tensorboard
 thefuzz==0.22.1
     # via molflux
-threadpoolctl==3.3.0
+threadpoolctl==3.4.0
     # via scikit-learn
 toml==0.10.2
     # via jupytext
-torch==2.0.1
+torch==2.3.0
     # via
     #   e3nn
     #   lightning
     #   opt-einsum-fx
     #   physicsml (pyproject.toml)
     #   pytorch-lightning
     #   torchani
     #   torchmetrics
-torch-geometric==2.5.0
+torch-geometric==2.5.3
     # via physicsml (pyproject.toml)
 torchani==2.2.3
     # via physicsml (pyproject.toml)
-torchmetrics==1.3.1
+torchmetrics==1.3.2
     # via
     #   lightning
     #   pytorch-lightning
 tornado==6.4
     # via
     #   ipykernel
     #   jupyter-client
@@ -566,62 +551,61 @@
     #   datasets
     #   evaluate
     #   huggingface-hub
     #   lightning
     #   molflux
     #   pytorch-lightning
     #   torch-geometric
-traitlets==5.14.1
+traitlets==5.14.3
     # via
     #   comm
     #   ipykernel
     #   ipython
     #   ipywidgets
     #   jupyter-client
     #   jupyter-core
     #   matplotlib-inline
     #   nbclient
     #   nbformat
-typing-extensions==4.9.0
+typing-extensions==4.11.0
     # via
     #   domdf-python-tools
     #   huggingface-hub
+    #   ipython
     #   lightning
     #   lightning-utilities
     #   molflux
     #   myst-nb
     #   pydantic
     #   pydata-sphinx-theme
     #   pytorch-lightning
     #   sphinx-toolbox
     #   sqlalchemy
     #   torch
 tzdata==2024.1
     # via pandas
-urllib3==2.0.7
+urllib3==2.2.1
     # via
     #   botocore
     #   requests
     #   responses
 wcwidth==0.2.13
     # via prompt-toolkit
 webencodings==0.5.1
     # via html5lib
-websocket-client==1.7.0
+websocket-client==1.8.0
     # via qlient
-werkzeug==3.0.1
-    # via tensorboard
-wheel==0.42.0
+wheel==0.43.0
     # via sphinx-togglebutton
 widgetsnbextension==4.0.10
     # via ipywidgets
 xxhash==3.4.1
     # via
     #   datasets
     #   evaluate
 yarl==1.9.4
     # via aiohttp
-zipp==3.17.0
+zipp==3.18.1
     # via importlib-metadata
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `physicsml-0.2.3/pinned-versions/3.11/lockfile.core.txt` & `physicsml-0.2.4/pinned-versions/3.11/lockfile.openmm.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 #
 # This file is autogenerated by pip-compile with Python 3.11
 # by the following command:
 #
-#    nox -s dependencies_pin-3.11(extra=None)
+#    nox -s dependencies_pin-3.11(extra='openmm')
 #
-absl-py==2.1.0
-    # via tensorboard
 accessible-pygments==0.0.4
     # via pydata-sphinx-theme
-aiohttp==3.9.3
+aiohttp==3.9.5
     # via
     #   datasets
     #   fsspec
     #   torch-geometric
 aiosignal==1.3.1
     # via aiohttp
 alabaster==0.7.16
@@ -39,67 +37,67 @@
     # via
     #   pydata-sphinx-theme
     #   sphinx
 beautifulsoup4==4.12.3
     # via
     #   pydata-sphinx-theme
     #   sphinx-toolbox
-boto3==1.34.45
+boto3==1.34.91
     # via
     #   cloudpathlib
     #   molflux
-botocore==1.34.45
+botocore==1.34.91
     # via
     #   boto3
     #   molflux
     #   s3transfer
 cachecontrol==0.14.0
     # via sphinx-toolbox
 certifi==2024.2.2
     # via requests
 charset-normalizer==3.3.2
     # via requests
 click==8.1.7
     # via jupyter-cache
-cloudpathlib==0.17.0
+cloudpathlib==0.18.1
     # via molflux
 colorama==0.4.6
     # via molflux
-comm==0.2.1
+comm==0.2.2
     # via
     #   ipykernel
     #   ipywidgets
-contourpy==1.2.0
+contourpy==1.2.1
     # via matplotlib
-coverage==7.4.1
+coverage==7.5.0
     # via
     #   coverage-badge
     #   physicsml (pyproject.toml)
-coverage-badge==1.1.0
+coverage-badge==1.1.1
     # via physicsml (pyproject.toml)
-cssutils==2.9.0
+cssutils==2.10.2
     # via dict2css
 cycler==0.12.1
     # via matplotlib
-datasets==2.17.1
+datasets==2.19.0
     # via
     #   evaluate
     #   molflux
 debugpy==1.8.1
     # via ipykernel
 decorator==5.1.1
     # via ipython
 dict2css==0.3.0.post1
     # via sphinx-toolbox
 dill==0.3.8
     # via
     #   datasets
     #   evaluate
     #   multiprocess
-docutils==0.20.1
+docutils==0.21.2
     # via
     #   myst-parser
     #   pydata-sphinx-theme
     #   sphinx
     #   sphinx-prompt
     #   sphinx-tabs
     #   sphinx-togglebutton
@@ -114,66 +112,65 @@
     # via physicsml (pyproject.toml)
 evaluate==0.4.1
     # via molflux
 executing==2.0.1
     # via stack-data
 fastjsonschema==2.19.1
     # via nbformat
-filelock==3.13.1
+filelock==3.13.4
     # via
     #   cachecontrol
     #   datasets
     #   huggingface-hub
     #   sphinx-toolbox
     #   torch
-fonttools==4.49.0
+fonttools==4.51.0
     # via matplotlib
 frozenlist==1.4.1
     # via
     #   aiohttp
     #   aiosignal
-fsspec==2023.10.0
+fsspec==2024.3.1
     # via
     #   datasets
     #   evaluate
     #   huggingface-hub
     #   lightning
     #   molflux
     #   pytorch-lightning
+    #   torch
     #   torch-geometric
-grpcio==1.60.1
-    # via tensorboard
-h5py==3.10.0
+h5py==3.11.0
     # via
     #   molflux
     #   physicsml (pyproject.toml)
 html5lib==1.1
     # via sphinx-toolbox
-huggingface-hub==0.20.3
+huggingface-hub==0.22.2
     # via
     #   datasets
     #   evaluate
-idna==3.6
+idna==3.7
     # via
     #   apeye-core
     #   requests
     #   yarl
 imagesize==1.4.1
     # via sphinx
 importlib-metadata==4.13.0
     # via
     #   jupyter-cache
     #   myst-nb
     #   qlient-core
     #   torchani
 iniconfig==2.0.0
     # via pytest
-ipykernel==6.29.2
+ipykernel==6.29.4
     # via myst-nb
-ipython==8.21.0
+ipython==8.23.0
     # via
     #   ipykernel
     #   ipywidgets
     #   myst-nb
 ipywidgets==8.1.2
     # via physicsml (pyproject.toml)
 jedi==0.19.1
@@ -185,66 +182,63 @@
     #   sphinx-jinja2-compat
     #   torch
     #   torch-geometric
 jmespath==1.0.1
     # via
     #   boto3
     #   botocore
-joblib==1.3.2
+joblib==1.4.0
     # via
     #   molflux
     #   scikit-learn
 jsonschema==4.21.1
     # via nbformat
 jsonschema-specifications==2023.12.1
     # via jsonschema
 jupyter-cache==1.0.0
     # via myst-nb
-jupyter-client==8.6.0
+jupyter-client==8.6.1
     # via
     #   ipykernel
     #   nbclient
-jupyter-core==5.7.1
+jupyter-core==5.7.2
     # via
     #   ipykernel
     #   jupyter-client
     #   nbclient
     #   nbformat
 jupyterlab-widgets==3.0.10
     # via ipywidgets
 jupytext==1.16.1
     # via physicsml (pyproject.toml)
 kiwisolver==1.4.5
     # via matplotlib
 lark-parser==0.12.0
     # via torchani
-lightning==2.2.0.post0
+lightning==2.2.3
     # via physicsml (pyproject.toml)
-lightning-utilities==0.10.1
+lightning-utilities==0.11.2
     # via
     #   lightning
     #   pytorch-lightning
     #   torchmetrics
-markdown==3.5.2
-    # via tensorboard
 markdown-it-py==3.0.0
     # via
     #   jupytext
     #   mdit-py-plugins
     #   myst-parser
 markupsafe==2.1.5
     # via
     #   jinja2
     #   sphinx-jinja2-compat
-    #   werkzeug
-matplotlib==3.8.3
+matplotlib==3.8.4
     # via
     #   ase
     #   physicsml (pyproject.toml)
-matplotlib-inline==0.1.6
+matplotlib-inline==0.1.7
     # via
     #   ipykernel
     #   ipython
 mdit-py-plugins==0.4.0
     # via
     #   jupytext
     #   myst-parser
@@ -254,43 +248,43 @@
     # via molflux
 molflux==0.3.0
     # via physicsml (pyproject.toml)
 more-itertools==10.2.0
     # via molflux
 mpmath==1.3.0
     # via sympy
-msgpack==1.0.7
+msgpack==1.0.8
     # via cachecontrol
 multidict==6.0.5
     # via
     #   aiohttp
     #   yarl
 multiprocess==0.70.16
     # via
     #   datasets
     #   evaluate
-myst-nb==1.0.0
+myst-nb==1.1.0
     # via physicsml (pyproject.toml)
-myst-parser==2.0.0
+myst-parser==3.0.0
     # via myst-nb
 natsort==8.4.0
     # via domdf-python-tools
-nbclient==0.9.0
+nbclient==0.10.0
     # via
     #   jupyter-cache
     #   myst-nb
-nbformat==5.9.2
+nbformat==5.10.4
     # via
     #   jupyter-cache
     #   jupytext
     #   myst-nb
     #   nbclient
 nest-asyncio==1.6.0
     # via ipykernel
-networkx==3.2.1
+networkx==3.3
     # via torch
 numpy==1.26.4
     # via
     #   ase
     #   contourpy
     #   datasets
     #   evaluate
@@ -301,22 +295,21 @@
     #   opt-einsum
     #   pandas
     #   pyarrow
     #   pytorch-lightning
     #   rdkit
     #   scikit-learn
     #   scipy
-    #   tensorboard
     #   torch-geometric
     #   torchmetrics
 opt-einsum==3.3.0
     # via opt-einsum-fx
 opt-einsum-fx==0.1.4
     # via e3nn
-packaging==23.2
+packaging==24.0
     # via
     #   datasets
     #   evaluate
     #   huggingface-hub
     #   ipykernel
     #   jupytext
     #   lightning
@@ -324,114 +317,111 @@
     #   matplotlib
     #   opt-einsum-fx
     #   pydata-sphinx-theme
     #   pytest
     #   pytorch-lightning
     #   sphinx
     #   torchmetrics
-pandas==2.2.0
+pandas==2.2.2
     # via
     #   datasets
     #   evaluate
     #   molflux
-parso==0.8.3
+parso==0.8.4
     # via jedi
 pexpect==4.9.0
     # via ipython
-pillow==10.2.0
+pillow==10.3.0
     # via
     #   matplotlib
     #   rdkit
-platformdirs==4.2.0
+platformdirs==4.2.1
     # via
     #   apeye
     #   jupyter-core
-pluggy==1.4.0
+pluggy==1.5.0
     # via pytest
 prompt-toolkit==3.0.43
     # via ipython
-protobuf==4.25.3
-    # via tensorboard
 psutil==5.9.8
     # via
     #   ipykernel
     #   torch-geometric
 ptyprocess==0.7.0
     # via pexpect
 pure-eval==0.2.2
     # via stack-data
-pyarrow==15.0.0
+pyarrow==16.0.0
     # via
     #   datasets
     #   molflux
 pyarrow-hotfix==0.6
     # via datasets
-pydantic==1.10.14
+pydantic==1.10.15
     # via molflux
 pydata-sphinx-theme==0.15.2
     # via sphinx-book-theme
 pygments==2.17.2
     # via
     #   accessible-pygments
     #   ipython
     #   pydata-sphinx-theme
     #   sphinx
     #   sphinx-prompt
     #   sphinx-tabs
-pyparsing==3.1.1
+pyparsing==3.1.2
     # via
     #   matplotlib
     #   torch-geometric
-pytest==8.0.1
+pytest==8.1.1
     # via physicsml (pyproject.toml)
-python-dateutil==2.8.2
+python-dateutil==2.9.0.post0
     # via
     #   botocore
     #   jupyter-client
     #   matplotlib
     #   molflux
     #   pandas
-pytorch-lightning==2.2.0.post0
+pytorch-lightning==2.2.3
     # via lightning
 pytz==2024.1
     # via pandas
 pyyaml==6.0.1
     # via
     #   datasets
     #   huggingface-hub
     #   jupyter-cache
     #   jupytext
     #   lightning
     #   molflux
     #   myst-nb
     #   myst-parser
     #   pytorch-lightning
-pyzmq==25.1.2
+pyzmq==26.0.2
     # via
     #   ipykernel
     #   jupyter-client
 qlient==1.0.0
     # via molflux
 qlient-core==1.0.1
     # via qlient
-rapidfuzz==3.6.1
+rapidfuzz==3.8.1
     # via thefuzz
 rdkit==2023.9.5
     # via physicsml (pyproject.toml)
-referencing==0.33.0
+referencing==0.35.0
     # via
     #   jsonschema
     #   jsonschema-specifications
 requests==2.31.0
     # via
     #   apeye
     #   cachecontrol
     #   datasets
     #   evaluate
-    #   fsspec
     #   huggingface-hub
     #   molflux
     #   qlient
     #   responses
     #   sphinx
     #   torch-geometric
     #   torchani
@@ -441,38 +431,37 @@
     # via
     #   jsonschema
     #   referencing
 ruamel-yaml==0.18.6
     # via sphinx-toolbox
 ruamel-yaml-clib==0.2.8
     # via ruamel-yaml
-s3transfer==0.10.0
+s3transfer==0.10.1
     # via boto3
-scikit-learn==1.4.1.post1
+scikit-learn==1.4.2
     # via
     #   molflux
     #   torch-geometric
-scipy==1.12.0
+scipy==1.13.0
     # via
     #   ase
     #   e3nn
     #   molflux
     #   scikit-learn
     #   torch-geometric
 six==1.16.0
     # via
     #   asttokens
     #   html5lib
     #   python-dateutil
-    #   tensorboard
 snowballstemmer==2.2.0
     # via sphinx
 soupsieve==2.5
     # via beautifulsoup4
-sphinx==7.2.6
+sphinx==7.3.7
     # via
     #   autodocsumm
     #   myst-nb
     #   myst-parser
     #   physicsml (pyproject.toml)
     #   pydata-sphinx-theme
     #   sphinx-autodoc-typehints
@@ -480,15 +469,15 @@
     #   sphinx-design
     #   sphinx-inline-tabs
     #   sphinx-prompt
     #   sphinx-sitemap
     #   sphinx-tabs
     #   sphinx-togglebutton
     #   sphinx-toolbox
-sphinx-autodoc-typehints==2.0.0
+sphinx-autodoc-typehints==2.1.0
     # via sphinx-toolbox
 sphinx-book-theme==1.1.2
     # via physicsml (pyproject.toml)
 sphinx-design==0.5.0
     # via physicsml (pyproject.toml)
 sphinx-inline-tabs==2023.4.21
     # via physicsml (pyproject.toml)
@@ -512,52 +501,48 @@
     # via sphinx
 sphinxcontrib-jsmath==1.0.1
     # via sphinx
 sphinxcontrib-qthelp==1.0.7
     # via sphinx
 sphinxcontrib-serializinghtml==1.1.10
     # via sphinx
-sqlalchemy==2.0.27
+sqlalchemy==2.0.29
     # via jupyter-cache
 stack-data==0.6.3
     # via ipython
 sympy==1.12
     # via
     #   e3nn
     #   torch
 tabulate==0.9.0
     # via
     #   jupyter-cache
     #   sphinx-toolbox
 tenacity==8.2.3
     # via molflux
-tensorboard==2.16.2
-    # via physicsml (pyproject.toml)
-tensorboard-data-server==0.7.2
-    # via tensorboard
 thefuzz==0.22.1
     # via molflux
-threadpoolctl==3.3.0
+threadpoolctl==3.4.0
     # via scikit-learn
 toml==0.10.2
     # via jupytext
-torch==2.0.1
+torch==2.3.0
     # via
     #   e3nn
     #   lightning
     #   opt-einsum-fx
     #   physicsml (pyproject.toml)
     #   pytorch-lightning
     #   torchani
     #   torchmetrics
-torch-geometric==2.5.0
+torch-geometric==2.5.3
     # via physicsml (pyproject.toml)
 torchani==2.2.3
     # via physicsml (pyproject.toml)
-torchmetrics==1.3.1
+torchmetrics==1.3.2
     # via
     #   lightning
     #   pytorch-lightning
 tornado==6.4
     # via
     #   ipykernel
     #   jupyter-client
@@ -566,62 +551,61 @@
     #   datasets
     #   evaluate
     #   huggingface-hub
     #   lightning
     #   molflux
     #   pytorch-lightning
     #   torch-geometric
-traitlets==5.14.1
+traitlets==5.14.3
     # via
     #   comm
     #   ipykernel
     #   ipython
     #   ipywidgets
     #   jupyter-client
     #   jupyter-core
     #   matplotlib-inline
     #   nbclient
     #   nbformat
-typing-extensions==4.9.0
+typing-extensions==4.11.0
     # via
     #   domdf-python-tools
     #   huggingface-hub
+    #   ipython
     #   lightning
     #   lightning-utilities
     #   molflux
     #   myst-nb
     #   pydantic
     #   pydata-sphinx-theme
     #   pytorch-lightning
     #   sphinx-toolbox
     #   sqlalchemy
     #   torch
 tzdata==2024.1
     # via pandas
-urllib3==2.0.7
+urllib3==2.2.1
     # via
     #   botocore
     #   requests
     #   responses
 wcwidth==0.2.13
     # via prompt-toolkit
 webencodings==0.5.1
     # via html5lib
-websocket-client==1.7.0
+websocket-client==1.8.0
     # via qlient
-werkzeug==3.0.1
-    # via tensorboard
-wheel==0.42.0
+wheel==0.43.0
     # via sphinx-togglebutton
 widgetsnbextension==4.0.10
     # via ipywidgets
 xxhash==3.4.1
     # via
     #   datasets
     #   evaluate
 yarl==1.9.4
     # via aiohttp
-zipp==3.17.0
+zipp==3.18.1
     # via importlib-metadata
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `physicsml-0.2.3/pinned-versions/3.11/lockfile.openeye.txt` & `physicsml-0.2.4/pinned-versions/3.9/lockfile.openeye.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 #
-# This file is autogenerated by pip-compile with Python 3.11
+# This file is autogenerated by pip-compile with Python 3.9
 # by the following command:
 #
-#    nox -s dependencies_pin-3.11(extra='openeye')
+#    nox -s dependencies_pin-3.9(extra='openeye')
 #
-absl-py==2.1.0
-    # via tensorboard
 accessible-pygments==0.0.4
     # via pydata-sphinx-theme
-aiohttp==3.9.3
+aiohttp==3.9.5
     # via
     #   datasets
     #   fsspec
     #   torch-geometric
 aiosignal==1.3.1
     # via aiohttp
 alabaster==0.7.16
@@ -23,14 +21,16 @@
     # via apeye
 appnope==0.1.4
     # via ipykernel
 ase==3.22.1
     # via physicsml (pyproject.toml)
 asttokens==2.4.1
     # via stack-data
+async-timeout==4.0.3
+    # via aiohttp
 attrs==23.2.0
     # via
     #   aiohttp
     #   jsonschema
     #   jupyter-cache
     #   referencing
 autodocsumm==0.2.12
@@ -39,67 +39,67 @@
     # via
     #   pydata-sphinx-theme
     #   sphinx
 beautifulsoup4==4.12.3
     # via
     #   pydata-sphinx-theme
     #   sphinx-toolbox
-boto3==1.34.45
+boto3==1.34.91
     # via
     #   cloudpathlib
     #   molflux
-botocore==1.34.45
+botocore==1.34.91
     # via
     #   boto3
     #   molflux
     #   s3transfer
 cachecontrol==0.14.0
     # via sphinx-toolbox
 certifi==2024.2.2
     # via requests
 charset-normalizer==3.3.2
     # via requests
 click==8.1.7
     # via jupyter-cache
-cloudpathlib==0.17.0
+cloudpathlib==0.18.1
     # via molflux
 colorama==0.4.6
     # via molflux
-comm==0.2.1
+comm==0.2.2
     # via
     #   ipykernel
     #   ipywidgets
-contourpy==1.2.0
+contourpy==1.2.1
     # via matplotlib
-coverage==7.4.1
+coverage==7.5.0
     # via
     #   coverage-badge
     #   physicsml (pyproject.toml)
-coverage-badge==1.1.0
+coverage-badge==1.1.1
     # via physicsml (pyproject.toml)
-cssutils==2.9.0
+cssutils==2.10.2
     # via dict2css
 cycler==0.12.1
     # via matplotlib
-datasets==2.17.1
+datasets==2.19.0
     # via
     #   evaluate
     #   molflux
 debugpy==1.8.1
     # via ipykernel
 decorator==5.1.1
     # via ipython
 dict2css==0.3.0.post1
     # via sphinx-toolbox
 dill==0.3.8
     # via
     #   datasets
     #   evaluate
     #   multiprocess
-docutils==0.20.1
+docutils==0.21.2
     # via
     #   myst-parser
     #   pydata-sphinx-theme
     #   sphinx
     #   sphinx-prompt
     #   sphinx-tabs
     #   sphinx-togglebutton
@@ -110,70 +110,77 @@
     #   apeye-core
     #   dict2css
     #   sphinx-toolbox
 e3nn==0.5.1
     # via physicsml (pyproject.toml)
 evaluate==0.4.1
     # via molflux
+exceptiongroup==1.2.1
+    # via
+    #   ipython
+    #   pytest
 executing==2.0.1
     # via stack-data
 fastjsonschema==2.19.1
     # via nbformat
-filelock==3.13.1
+filelock==3.13.4
     # via
     #   cachecontrol
     #   datasets
     #   huggingface-hub
     #   sphinx-toolbox
     #   torch
-fonttools==4.49.0
+fonttools==4.51.0
     # via matplotlib
 frozenlist==1.4.1
     # via
     #   aiohttp
     #   aiosignal
-fsspec==2023.10.0
+fsspec==2024.3.1
     # via
     #   datasets
     #   evaluate
     #   huggingface-hub
     #   lightning
     #   molflux
     #   pytorch-lightning
+    #   torch
     #   torch-geometric
-grpcio==1.60.1
-    # via tensorboard
-h5py==3.10.0
+h5py==3.11.0
     # via
     #   molflux
     #   physicsml (pyproject.toml)
 html5lib==1.1
     # via sphinx-toolbox
-huggingface-hub==0.20.3
+huggingface-hub==0.22.2
     # via
     #   datasets
     #   evaluate
-idna==3.6
+idna==3.7
     # via
     #   apeye-core
     #   requests
     #   yarl
 imagesize==1.4.1
     # via sphinx
 importlib-metadata==4.13.0
     # via
     #   jupyter-cache
+    #   jupyter-client
     #   myst-nb
     #   qlient-core
+    #   sphinx
     #   torchani
+importlib-resources==6.4.0
+    # via matplotlib
 iniconfig==2.0.0
     # via pytest
-ipykernel==6.29.2
+ipykernel==6.29.4
     # via myst-nb
-ipython==8.21.0
+ipython==8.18.1
     # via
     #   ipykernel
     #   ipywidgets
     #   myst-nb
 ipywidgets==8.1.2
     # via physicsml (pyproject.toml)
 jedi==0.19.1
@@ -185,66 +192,63 @@
     #   sphinx-jinja2-compat
     #   torch
     #   torch-geometric
 jmespath==1.0.1
     # via
     #   boto3
     #   botocore
-joblib==1.3.2
+joblib==1.4.0
     # via
     #   molflux
     #   scikit-learn
 jsonschema==4.21.1
     # via nbformat
 jsonschema-specifications==2023.12.1
     # via jsonschema
 jupyter-cache==1.0.0
     # via myst-nb
-jupyter-client==8.6.0
+jupyter-client==8.6.1
     # via
     #   ipykernel
     #   nbclient
-jupyter-core==5.7.1
+jupyter-core==5.7.2
     # via
     #   ipykernel
     #   jupyter-client
     #   nbclient
     #   nbformat
 jupyterlab-widgets==3.0.10
     # via ipywidgets
 jupytext==1.16.1
     # via physicsml (pyproject.toml)
 kiwisolver==1.4.5
     # via matplotlib
 lark-parser==0.12.0
     # via torchani
-lightning==2.2.0.post0
+lightning==2.2.3
     # via physicsml (pyproject.toml)
-lightning-utilities==0.10.1
+lightning-utilities==0.11.2
     # via
     #   lightning
     #   pytorch-lightning
     #   torchmetrics
-markdown==3.5.2
-    # via tensorboard
 markdown-it-py==3.0.0
     # via
     #   jupytext
     #   mdit-py-plugins
     #   myst-parser
 markupsafe==2.1.5
     # via
     #   jinja2
     #   sphinx-jinja2-compat
-    #   werkzeug
-matplotlib==3.8.3
+matplotlib==3.8.4
     # via
     #   ase
     #   physicsml (pyproject.toml)
-matplotlib-inline==0.1.6
+matplotlib-inline==0.1.7
     # via
     #   ipykernel
     #   ipython
 mdit-py-plugins==0.4.0
     # via
     #   jupytext
     #   myst-parser
@@ -254,35 +258,35 @@
     # via molflux
 molflux==0.3.0
     # via physicsml (pyproject.toml)
 more-itertools==10.2.0
     # via molflux
 mpmath==1.3.0
     # via sympy
-msgpack==1.0.7
+msgpack==1.0.8
     # via cachecontrol
 multidict==6.0.5
     # via
     #   aiohttp
     #   yarl
 multiprocess==0.70.16
     # via
     #   datasets
     #   evaluate
-myst-nb==1.0.0
+myst-nb==1.1.0
     # via physicsml (pyproject.toml)
-myst-parser==2.0.0
+myst-parser==3.0.0
     # via myst-nb
 natsort==8.4.0
     # via domdf-python-tools
-nbclient==0.9.0
+nbclient==0.10.0
     # via
     #   jupyter-cache
     #   myst-nb
-nbformat==5.9.2
+nbformat==5.10.4
     # via
     #   jupyter-cache
     #   jupytext
     #   myst-nb
     #   nbclient
 nest-asyncio==1.6.0
     # via ipykernel
@@ -301,24 +305,23 @@
     #   opt-einsum
     #   pandas
     #   pyarrow
     #   pytorch-lightning
     #   rdkit
     #   scikit-learn
     #   scipy
-    #   tensorboard
     #   torch-geometric
     #   torchmetrics
 openeye-toolkits==2023.2.3
     # via physicsml (pyproject.toml)
 opt-einsum==3.3.0
     # via opt-einsum-fx
 opt-einsum-fx==0.1.4
     # via e3nn
-packaging==23.2
+packaging==24.0
     # via
     #   datasets
     #   evaluate
     #   huggingface-hub
     #   ipykernel
     #   jupytext
     #   lightning
@@ -326,114 +329,111 @@
     #   matplotlib
     #   opt-einsum-fx
     #   pydata-sphinx-theme
     #   pytest
     #   pytorch-lightning
     #   sphinx
     #   torchmetrics
-pandas==2.2.0
+pandas==2.2.2
     # via
     #   datasets
     #   evaluate
     #   molflux
-parso==0.8.3
+parso==0.8.4
     # via jedi
 pexpect==4.9.0
     # via ipython
-pillow==10.2.0
+pillow==10.3.0
     # via
     #   matplotlib
     #   rdkit
-platformdirs==4.2.0
+platformdirs==4.2.1
     # via
     #   apeye
     #   jupyter-core
-pluggy==1.4.0
+pluggy==1.5.0
     # via pytest
 prompt-toolkit==3.0.43
     # via ipython
-protobuf==4.25.3
-    # via tensorboard
 psutil==5.9.8
     # via
     #   ipykernel
     #   torch-geometric
 ptyprocess==0.7.0
     # via pexpect
 pure-eval==0.2.2
     # via stack-data
-pyarrow==15.0.0
+pyarrow==16.0.0
     # via
     #   datasets
     #   molflux
 pyarrow-hotfix==0.6
     # via datasets
-pydantic==1.10.14
+pydantic==1.10.15
     # via molflux
 pydata-sphinx-theme==0.15.2
     # via sphinx-book-theme
 pygments==2.17.2
     # via
     #   accessible-pygments
     #   ipython
     #   pydata-sphinx-theme
     #   sphinx
     #   sphinx-prompt
     #   sphinx-tabs
-pyparsing==3.1.1
+pyparsing==3.1.2
     # via
     #   matplotlib
     #   torch-geometric
-pytest==8.0.1
+pytest==8.1.1
     # via physicsml (pyproject.toml)
-python-dateutil==2.8.2
+python-dateutil==2.9.0.post0
     # via
     #   botocore
     #   jupyter-client
     #   matplotlib
     #   molflux
     #   pandas
-pytorch-lightning==2.2.0.post0
+pytorch-lightning==2.2.3
     # via lightning
 pytz==2024.1
     # via pandas
 pyyaml==6.0.1
     # via
     #   datasets
     #   huggingface-hub
     #   jupyter-cache
     #   jupytext
     #   lightning
     #   molflux
     #   myst-nb
     #   myst-parser
     #   pytorch-lightning
-pyzmq==25.1.2
+pyzmq==26.0.2
     # via
     #   ipykernel
     #   jupyter-client
 qlient==1.0.0
     # via molflux
 qlient-core==1.0.1
     # via qlient
-rapidfuzz==3.6.1
+rapidfuzz==3.8.1
     # via thefuzz
 rdkit==2023.9.5
     # via physicsml (pyproject.toml)
-referencing==0.33.0
+referencing==0.35.0
     # via
     #   jsonschema
     #   jsonschema-specifications
 requests==2.31.0
     # via
     #   apeye
     #   cachecontrol
     #   datasets
     #   evaluate
-    #   fsspec
     #   huggingface-hub
     #   molflux
     #   qlient
     #   responses
     #   sphinx
     #   torch-geometric
     #   torchani
@@ -443,38 +443,37 @@
     # via
     #   jsonschema
     #   referencing
 ruamel-yaml==0.18.6
     # via sphinx-toolbox
 ruamel-yaml-clib==0.2.8
     # via ruamel-yaml
-s3transfer==0.10.0
+s3transfer==0.10.1
     # via boto3
-scikit-learn==1.4.1.post1
+scikit-learn==1.4.2
     # via
     #   molflux
     #   torch-geometric
-scipy==1.12.0
+scipy==1.13.0
     # via
     #   ase
     #   e3nn
     #   molflux
     #   scikit-learn
     #   torch-geometric
 six==1.16.0
     # via
     #   asttokens
     #   html5lib
     #   python-dateutil
-    #   tensorboard
 snowballstemmer==2.2.0
     # via sphinx
 soupsieve==2.5
     # via beautifulsoup4
-sphinx==7.2.6
+sphinx==7.3.7
     # via
     #   autodocsumm
     #   myst-nb
     #   myst-parser
     #   physicsml (pyproject.toml)
     #   pydata-sphinx-theme
     #   sphinx-autodoc-typehints
@@ -482,15 +481,15 @@
     #   sphinx-design
     #   sphinx-inline-tabs
     #   sphinx-prompt
     #   sphinx-sitemap
     #   sphinx-tabs
     #   sphinx-togglebutton
     #   sphinx-toolbox
-sphinx-autodoc-typehints==2.0.0
+sphinx-autodoc-typehints==2.1.0
     # via sphinx-toolbox
 sphinx-book-theme==1.1.2
     # via physicsml (pyproject.toml)
 sphinx-design==0.5.0
     # via physicsml (pyproject.toml)
 sphinx-inline-tabs==2023.4.21
     # via physicsml (pyproject.toml)
@@ -514,52 +513,53 @@
     # via sphinx
 sphinxcontrib-jsmath==1.0.1
     # via sphinx
 sphinxcontrib-qthelp==1.0.7
     # via sphinx
 sphinxcontrib-serializinghtml==1.1.10
     # via sphinx
-sqlalchemy==2.0.27
+sqlalchemy==2.0.29
     # via jupyter-cache
 stack-data==0.6.3
     # via ipython
 sympy==1.12
     # via
     #   e3nn
     #   torch
 tabulate==0.9.0
     # via
     #   jupyter-cache
     #   sphinx-toolbox
 tenacity==8.2.3
     # via molflux
-tensorboard==2.16.2
-    # via physicsml (pyproject.toml)
-tensorboard-data-server==0.7.2
-    # via tensorboard
 thefuzz==0.22.1
     # via molflux
-threadpoolctl==3.3.0
+threadpoolctl==3.4.0
     # via scikit-learn
 toml==0.10.2
     # via jupytext
-torch==2.0.1
+tomli==2.0.1
+    # via
+    #   coverage
+    #   pytest
+    #   sphinx
+torch==2.3.0
     # via
     #   e3nn
     #   lightning
     #   opt-einsum-fx
     #   physicsml (pyproject.toml)
     #   pytorch-lightning
     #   torchani
     #   torchmetrics
-torch-geometric==2.5.0
+torch-geometric==2.5.3
     # via physicsml (pyproject.toml)
 torchani==2.2.3
     # via physicsml (pyproject.toml)
-torchmetrics==1.3.1
+torchmetrics==1.3.2
     # via
     #   lightning
     #   pytorch-lightning
 tornado==6.4
     # via
     #   ipykernel
     #   jupyter-client
@@ -568,62 +568,64 @@
     #   datasets
     #   evaluate
     #   huggingface-hub
     #   lightning
     #   molflux
     #   pytorch-lightning
     #   torch-geometric
-traitlets==5.14.1
+traitlets==5.14.3
     # via
     #   comm
     #   ipykernel
     #   ipython
     #   ipywidgets
     #   jupyter-client
     #   jupyter-core
     #   matplotlib-inline
     #   nbclient
     #   nbformat
-typing-extensions==4.9.0
+typing-extensions==4.11.0
     # via
+    #   cloudpathlib
     #   domdf-python-tools
     #   huggingface-hub
+    #   ipython
     #   lightning
     #   lightning-utilities
     #   molflux
     #   myst-nb
     #   pydantic
     #   pydata-sphinx-theme
     #   pytorch-lightning
     #   sphinx-toolbox
     #   sqlalchemy
     #   torch
 tzdata==2024.1
     # via pandas
-urllib3==2.0.7
+urllib3==1.26.18
     # via
     #   botocore
     #   requests
     #   responses
 wcwidth==0.2.13
     # via prompt-toolkit
 webencodings==0.5.1
     # via html5lib
-websocket-client==1.7.0
+websocket-client==1.8.0
     # via qlient
-werkzeug==3.0.1
-    # via tensorboard
-wheel==0.42.0
+wheel==0.43.0
     # via sphinx-togglebutton
 widgetsnbextension==4.0.10
     # via ipywidgets
 xxhash==3.4.1
     # via
     #   datasets
     #   evaluate
 yarl==1.9.4
     # via aiohttp
-zipp==3.17.0
-    # via importlib-metadata
+zipp==3.18.1
+    # via
+    #   importlib-metadata
+    #   importlib-resources
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `physicsml-0.2.3/pinned-versions/3.11/lockfile.openmm.txt` & `physicsml-0.2.4/pinned-versions/3.9/lockfile.rdkit.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 #
-# This file is autogenerated by pip-compile with Python 3.11
+# This file is autogenerated by pip-compile with Python 3.9
 # by the following command:
 #
-#    nox -s dependencies_pin-3.11(extra='openmm')
+#    nox -s dependencies_pin-3.9(extra='rdkit')
 #
-absl-py==2.1.0
-    # via tensorboard
 accessible-pygments==0.0.4
     # via pydata-sphinx-theme
-aiohttp==3.9.3
+aiohttp==3.9.5
     # via
     #   datasets
     #   fsspec
     #   torch-geometric
 aiosignal==1.3.1
     # via aiohttp
 alabaster==0.7.16
@@ -23,14 +21,16 @@
     # via apeye
 appnope==0.1.4
     # via ipykernel
 ase==3.22.1
     # via physicsml (pyproject.toml)
 asttokens==2.4.1
     # via stack-data
+async-timeout==4.0.3
+    # via aiohttp
 attrs==23.2.0
     # via
     #   aiohttp
     #   jsonschema
     #   jupyter-cache
     #   referencing
 autodocsumm==0.2.12
@@ -39,67 +39,67 @@
     # via
     #   pydata-sphinx-theme
     #   sphinx
 beautifulsoup4==4.12.3
     # via
     #   pydata-sphinx-theme
     #   sphinx-toolbox
-boto3==1.34.45
+boto3==1.34.91
     # via
     #   cloudpathlib
     #   molflux
-botocore==1.34.45
+botocore==1.34.91
     # via
     #   boto3
     #   molflux
     #   s3transfer
 cachecontrol==0.14.0
     # via sphinx-toolbox
 certifi==2024.2.2
     # via requests
 charset-normalizer==3.3.2
     # via requests
 click==8.1.7
     # via jupyter-cache
-cloudpathlib==0.17.0
+cloudpathlib==0.18.1
     # via molflux
 colorama==0.4.6
     # via molflux
-comm==0.2.1
+comm==0.2.2
     # via
     #   ipykernel
     #   ipywidgets
-contourpy==1.2.0
+contourpy==1.2.1
     # via matplotlib
-coverage==7.4.1
+coverage==7.5.0
     # via
     #   coverage-badge
     #   physicsml (pyproject.toml)
-coverage-badge==1.1.0
+coverage-badge==1.1.1
     # via physicsml (pyproject.toml)
-cssutils==2.9.0
+cssutils==2.10.2
     # via dict2css
 cycler==0.12.1
     # via matplotlib
-datasets==2.17.1
+datasets==2.19.0
     # via
     #   evaluate
     #   molflux
 debugpy==1.8.1
     # via ipykernel
 decorator==5.1.1
     # via ipython
 dict2css==0.3.0.post1
     # via sphinx-toolbox
 dill==0.3.8
     # via
     #   datasets
     #   evaluate
     #   multiprocess
-docutils==0.20.1
+docutils==0.21.2
     # via
     #   myst-parser
     #   pydata-sphinx-theme
     #   sphinx
     #   sphinx-prompt
     #   sphinx-tabs
     #   sphinx-togglebutton
@@ -110,70 +110,77 @@
     #   apeye-core
     #   dict2css
     #   sphinx-toolbox
 e3nn==0.5.1
     # via physicsml (pyproject.toml)
 evaluate==0.4.1
     # via molflux
+exceptiongroup==1.2.1
+    # via
+    #   ipython
+    #   pytest
 executing==2.0.1
     # via stack-data
 fastjsonschema==2.19.1
     # via nbformat
-filelock==3.13.1
+filelock==3.13.4
     # via
     #   cachecontrol
     #   datasets
     #   huggingface-hub
     #   sphinx-toolbox
     #   torch
-fonttools==4.49.0
+fonttools==4.51.0
     # via matplotlib
 frozenlist==1.4.1
     # via
     #   aiohttp
     #   aiosignal
-fsspec==2023.10.0
+fsspec==2024.3.1
     # via
     #   datasets
     #   evaluate
     #   huggingface-hub
     #   lightning
     #   molflux
     #   pytorch-lightning
+    #   torch
     #   torch-geometric
-grpcio==1.60.1
-    # via tensorboard
-h5py==3.10.0
+h5py==3.11.0
     # via
     #   molflux
     #   physicsml (pyproject.toml)
 html5lib==1.1
     # via sphinx-toolbox
-huggingface-hub==0.20.3
+huggingface-hub==0.22.2
     # via
     #   datasets
     #   evaluate
-idna==3.6
+idna==3.7
     # via
     #   apeye-core
     #   requests
     #   yarl
 imagesize==1.4.1
     # via sphinx
 importlib-metadata==4.13.0
     # via
     #   jupyter-cache
+    #   jupyter-client
     #   myst-nb
     #   qlient-core
+    #   sphinx
     #   torchani
+importlib-resources==6.4.0
+    # via matplotlib
 iniconfig==2.0.0
     # via pytest
-ipykernel==6.29.2
+ipykernel==6.29.4
     # via myst-nb
-ipython==8.21.0
+ipython==8.18.1
     # via
     #   ipykernel
     #   ipywidgets
     #   myst-nb
 ipywidgets==8.1.2
     # via physicsml (pyproject.toml)
 jedi==0.19.1
@@ -185,66 +192,63 @@
     #   sphinx-jinja2-compat
     #   torch
     #   torch-geometric
 jmespath==1.0.1
     # via
     #   boto3
     #   botocore
-joblib==1.3.2
+joblib==1.4.0
     # via
     #   molflux
     #   scikit-learn
 jsonschema==4.21.1
     # via nbformat
 jsonschema-specifications==2023.12.1
     # via jsonschema
 jupyter-cache==1.0.0
     # via myst-nb
-jupyter-client==8.6.0
+jupyter-client==8.6.1
     # via
     #   ipykernel
     #   nbclient
-jupyter-core==5.7.1
+jupyter-core==5.7.2
     # via
     #   ipykernel
     #   jupyter-client
     #   nbclient
     #   nbformat
 jupyterlab-widgets==3.0.10
     # via ipywidgets
 jupytext==1.16.1
     # via physicsml (pyproject.toml)
 kiwisolver==1.4.5
     # via matplotlib
 lark-parser==0.12.0
     # via torchani
-lightning==2.2.0.post0
+lightning==2.2.3
     # via physicsml (pyproject.toml)
-lightning-utilities==0.10.1
+lightning-utilities==0.11.2
     # via
     #   lightning
     #   pytorch-lightning
     #   torchmetrics
-markdown==3.5.2
-    # via tensorboard
 markdown-it-py==3.0.0
     # via
     #   jupytext
     #   mdit-py-plugins
     #   myst-parser
 markupsafe==2.1.5
     # via
     #   jinja2
     #   sphinx-jinja2-compat
-    #   werkzeug
-matplotlib==3.8.3
+matplotlib==3.8.4
     # via
     #   ase
     #   physicsml (pyproject.toml)
-matplotlib-inline==0.1.6
+matplotlib-inline==0.1.7
     # via
     #   ipykernel
     #   ipython
 mdit-py-plugins==0.4.0
     # via
     #   jupytext
     #   myst-parser
@@ -254,35 +258,35 @@
     # via molflux
 molflux==0.3.0
     # via physicsml (pyproject.toml)
 more-itertools==10.2.0
     # via molflux
 mpmath==1.3.0
     # via sympy
-msgpack==1.0.7
+msgpack==1.0.8
     # via cachecontrol
 multidict==6.0.5
     # via
     #   aiohttp
     #   yarl
 multiprocess==0.70.16
     # via
     #   datasets
     #   evaluate
-myst-nb==1.0.0
+myst-nb==1.1.0
     # via physicsml (pyproject.toml)
-myst-parser==2.0.0
+myst-parser==3.0.0
     # via myst-nb
 natsort==8.4.0
     # via domdf-python-tools
-nbclient==0.9.0
+nbclient==0.10.0
     # via
     #   jupyter-cache
     #   myst-nb
-nbformat==5.9.2
+nbformat==5.10.4
     # via
     #   jupyter-cache
     #   jupytext
     #   myst-nb
     #   nbclient
 nest-asyncio==1.6.0
     # via ipykernel
@@ -301,22 +305,21 @@
     #   opt-einsum
     #   pandas
     #   pyarrow
     #   pytorch-lightning
     #   rdkit
     #   scikit-learn
     #   scipy
-    #   tensorboard
     #   torch-geometric
     #   torchmetrics
 opt-einsum==3.3.0
     # via opt-einsum-fx
 opt-einsum-fx==0.1.4
     # via e3nn
-packaging==23.2
+packaging==24.0
     # via
     #   datasets
     #   evaluate
     #   huggingface-hub
     #   ipykernel
     #   jupytext
     #   lightning
@@ -324,114 +327,111 @@
     #   matplotlib
     #   opt-einsum-fx
     #   pydata-sphinx-theme
     #   pytest
     #   pytorch-lightning
     #   sphinx
     #   torchmetrics
-pandas==2.2.0
+pandas==2.2.2
     # via
     #   datasets
     #   evaluate
     #   molflux
-parso==0.8.3
+parso==0.8.4
     # via jedi
 pexpect==4.9.0
     # via ipython
-pillow==10.2.0
+pillow==10.3.0
     # via
     #   matplotlib
     #   rdkit
-platformdirs==4.2.0
+platformdirs==4.2.1
     # via
     #   apeye
     #   jupyter-core
-pluggy==1.4.0
+pluggy==1.5.0
     # via pytest
 prompt-toolkit==3.0.43
     # via ipython
-protobuf==4.25.3
-    # via tensorboard
 psutil==5.9.8
     # via
     #   ipykernel
     #   torch-geometric
 ptyprocess==0.7.0
     # via pexpect
 pure-eval==0.2.2
     # via stack-data
-pyarrow==15.0.0
+pyarrow==16.0.0
     # via
     #   datasets
     #   molflux
 pyarrow-hotfix==0.6
     # via datasets
-pydantic==1.10.14
+pydantic==1.10.15
     # via molflux
 pydata-sphinx-theme==0.15.2
     # via sphinx-book-theme
 pygments==2.17.2
     # via
     #   accessible-pygments
     #   ipython
     #   pydata-sphinx-theme
     #   sphinx
     #   sphinx-prompt
     #   sphinx-tabs
-pyparsing==3.1.1
+pyparsing==3.1.2
     # via
     #   matplotlib
     #   torch-geometric
-pytest==8.0.1
+pytest==8.1.1
     # via physicsml (pyproject.toml)
-python-dateutil==2.8.2
+python-dateutil==2.9.0.post0
     # via
     #   botocore
     #   jupyter-client
     #   matplotlib
     #   molflux
     #   pandas
-pytorch-lightning==2.2.0.post0
+pytorch-lightning==2.2.3
     # via lightning
 pytz==2024.1
     # via pandas
 pyyaml==6.0.1
     # via
     #   datasets
     #   huggingface-hub
     #   jupyter-cache
     #   jupytext
     #   lightning
     #   molflux
     #   myst-nb
     #   myst-parser
     #   pytorch-lightning
-pyzmq==25.1.2
+pyzmq==26.0.2
     # via
     #   ipykernel
     #   jupyter-client
 qlient==1.0.0
     # via molflux
 qlient-core==1.0.1
     # via qlient
-rapidfuzz==3.6.1
+rapidfuzz==3.8.1
     # via thefuzz
 rdkit==2023.9.5
     # via physicsml (pyproject.toml)
-referencing==0.33.0
+referencing==0.35.0
     # via
     #   jsonschema
     #   jsonschema-specifications
 requests==2.31.0
     # via
     #   apeye
     #   cachecontrol
     #   datasets
     #   evaluate
-    #   fsspec
     #   huggingface-hub
     #   molflux
     #   qlient
     #   responses
     #   sphinx
     #   torch-geometric
     #   torchani
@@ -441,38 +441,37 @@
     # via
     #   jsonschema
     #   referencing
 ruamel-yaml==0.18.6
     # via sphinx-toolbox
 ruamel-yaml-clib==0.2.8
     # via ruamel-yaml
-s3transfer==0.10.0
+s3transfer==0.10.1
     # via boto3
-scikit-learn==1.4.1.post1
+scikit-learn==1.4.2
     # via
     #   molflux
     #   torch-geometric
-scipy==1.12.0
+scipy==1.13.0
     # via
     #   ase
     #   e3nn
     #   molflux
     #   scikit-learn
     #   torch-geometric
 six==1.16.0
     # via
     #   asttokens
     #   html5lib
     #   python-dateutil
-    #   tensorboard
 snowballstemmer==2.2.0
     # via sphinx
 soupsieve==2.5
     # via beautifulsoup4
-sphinx==7.2.6
+sphinx==7.3.7
     # via
     #   autodocsumm
     #   myst-nb
     #   myst-parser
     #   physicsml (pyproject.toml)
     #   pydata-sphinx-theme
     #   sphinx-autodoc-typehints
@@ -480,15 +479,15 @@
     #   sphinx-design
     #   sphinx-inline-tabs
     #   sphinx-prompt
     #   sphinx-sitemap
     #   sphinx-tabs
     #   sphinx-togglebutton
     #   sphinx-toolbox
-sphinx-autodoc-typehints==2.0.0
+sphinx-autodoc-typehints==2.1.0
     # via sphinx-toolbox
 sphinx-book-theme==1.1.2
     # via physicsml (pyproject.toml)
 sphinx-design==0.5.0
     # via physicsml (pyproject.toml)
 sphinx-inline-tabs==2023.4.21
     # via physicsml (pyproject.toml)
@@ -512,52 +511,53 @@
     # via sphinx
 sphinxcontrib-jsmath==1.0.1
     # via sphinx
 sphinxcontrib-qthelp==1.0.7
     # via sphinx
 sphinxcontrib-serializinghtml==1.1.10
     # via sphinx
-sqlalchemy==2.0.27
+sqlalchemy==2.0.29
     # via jupyter-cache
 stack-data==0.6.3
     # via ipython
 sympy==1.12
     # via
     #   e3nn
     #   torch
 tabulate==0.9.0
     # via
     #   jupyter-cache
     #   sphinx-toolbox
 tenacity==8.2.3
     # via molflux
-tensorboard==2.16.2
-    # via physicsml (pyproject.toml)
-tensorboard-data-server==0.7.2
-    # via tensorboard
 thefuzz==0.22.1
     # via molflux
-threadpoolctl==3.3.0
+threadpoolctl==3.4.0
     # via scikit-learn
 toml==0.10.2
     # via jupytext
-torch==2.0.1
+tomli==2.0.1
+    # via
+    #   coverage
+    #   pytest
+    #   sphinx
+torch==2.3.0
     # via
     #   e3nn
     #   lightning
     #   opt-einsum-fx
     #   physicsml (pyproject.toml)
     #   pytorch-lightning
     #   torchani
     #   torchmetrics
-torch-geometric==2.5.0
+torch-geometric==2.5.3
     # via physicsml (pyproject.toml)
 torchani==2.2.3
     # via physicsml (pyproject.toml)
-torchmetrics==1.3.1
+torchmetrics==1.3.2
     # via
     #   lightning
     #   pytorch-lightning
 tornado==6.4
     # via
     #   ipykernel
     #   jupyter-client
@@ -566,62 +566,64 @@
     #   datasets
     #   evaluate
     #   huggingface-hub
     #   lightning
     #   molflux
     #   pytorch-lightning
     #   torch-geometric
-traitlets==5.14.1
+traitlets==5.14.3
     # via
     #   comm
     #   ipykernel
     #   ipython
     #   ipywidgets
     #   jupyter-client
     #   jupyter-core
     #   matplotlib-inline
     #   nbclient
     #   nbformat
-typing-extensions==4.9.0
+typing-extensions==4.11.0
     # via
+    #   cloudpathlib
     #   domdf-python-tools
     #   huggingface-hub
+    #   ipython
     #   lightning
     #   lightning-utilities
     #   molflux
     #   myst-nb
     #   pydantic
     #   pydata-sphinx-theme
     #   pytorch-lightning
     #   sphinx-toolbox
     #   sqlalchemy
     #   torch
 tzdata==2024.1
     # via pandas
-urllib3==2.0.7
+urllib3==1.26.18
     # via
     #   botocore
     #   requests
     #   responses
 wcwidth==0.2.13
     # via prompt-toolkit
 webencodings==0.5.1
     # via html5lib
-websocket-client==1.7.0
+websocket-client==1.8.0
     # via qlient
-werkzeug==3.0.1
-    # via tensorboard
-wheel==0.42.0
+wheel==0.43.0
     # via sphinx-togglebutton
 widgetsnbextension==4.0.10
     # via ipywidgets
 xxhash==3.4.1
     # via
     #   datasets
     #   evaluate
 yarl==1.9.4
     # via aiohttp
-zipp==3.17.0
-    # via importlib-metadata
+zipp==3.18.1
+    # via
+    #   importlib-metadata
+    #   importlib-resources
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `physicsml-0.2.3/pinned-versions/3.11/lockfile.rdkit.txt` & `physicsml-0.2.4/pinned-versions/3.9/lockfile.ase.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 #
-# This file is autogenerated by pip-compile with Python 3.11
+# This file is autogenerated by pip-compile with Python 3.9
 # by the following command:
 #
-#    nox -s dependencies_pin-3.11(extra='rdkit')
+#    nox -s dependencies_pin-3.9(extra='ase')
 #
-absl-py==2.1.0
-    # via tensorboard
 accessible-pygments==0.0.4
     # via pydata-sphinx-theme
-aiohttp==3.9.3
+aiohttp==3.9.5
     # via
     #   datasets
     #   fsspec
     #   torch-geometric
 aiosignal==1.3.1
     # via aiohttp
 alabaster==0.7.16
@@ -23,14 +21,16 @@
     # via apeye
 appnope==0.1.4
     # via ipykernel
 ase==3.22.1
     # via physicsml (pyproject.toml)
 asttokens==2.4.1
     # via stack-data
+async-timeout==4.0.3
+    # via aiohttp
 attrs==23.2.0
     # via
     #   aiohttp
     #   jsonschema
     #   jupyter-cache
     #   referencing
 autodocsumm==0.2.12
@@ -39,67 +39,67 @@
     # via
     #   pydata-sphinx-theme
     #   sphinx
 beautifulsoup4==4.12.3
     # via
     #   pydata-sphinx-theme
     #   sphinx-toolbox
-boto3==1.34.45
+boto3==1.34.91
     # via
     #   cloudpathlib
     #   molflux
-botocore==1.34.45
+botocore==1.34.91
     # via
     #   boto3
     #   molflux
     #   s3transfer
 cachecontrol==0.14.0
     # via sphinx-toolbox
 certifi==2024.2.2
     # via requests
 charset-normalizer==3.3.2
     # via requests
 click==8.1.7
     # via jupyter-cache
-cloudpathlib==0.17.0
+cloudpathlib==0.18.1
     # via molflux
 colorama==0.4.6
     # via molflux
-comm==0.2.1
+comm==0.2.2
     # via
     #   ipykernel
     #   ipywidgets
-contourpy==1.2.0
+contourpy==1.2.1
     # via matplotlib
-coverage==7.4.1
+coverage==7.5.0
     # via
     #   coverage-badge
     #   physicsml (pyproject.toml)
-coverage-badge==1.1.0
+coverage-badge==1.1.1
     # via physicsml (pyproject.toml)
-cssutils==2.9.0
+cssutils==2.10.2
     # via dict2css
 cycler==0.12.1
     # via matplotlib
-datasets==2.17.1
+datasets==2.19.0
     # via
     #   evaluate
     #   molflux
 debugpy==1.8.1
     # via ipykernel
 decorator==5.1.1
     # via ipython
 dict2css==0.3.0.post1
     # via sphinx-toolbox
 dill==0.3.8
     # via
     #   datasets
     #   evaluate
     #   multiprocess
-docutils==0.20.1
+docutils==0.21.2
     # via
     #   myst-parser
     #   pydata-sphinx-theme
     #   sphinx
     #   sphinx-prompt
     #   sphinx-tabs
     #   sphinx-togglebutton
@@ -110,70 +110,77 @@
     #   apeye-core
     #   dict2css
     #   sphinx-toolbox
 e3nn==0.5.1
     # via physicsml (pyproject.toml)
 evaluate==0.4.1
     # via molflux
+exceptiongroup==1.2.1
+    # via
+    #   ipython
+    #   pytest
 executing==2.0.1
     # via stack-data
 fastjsonschema==2.19.1
     # via nbformat
-filelock==3.13.1
+filelock==3.13.4
     # via
     #   cachecontrol
     #   datasets
     #   huggingface-hub
     #   sphinx-toolbox
     #   torch
-fonttools==4.49.0
+fonttools==4.51.0
     # via matplotlib
 frozenlist==1.4.1
     # via
     #   aiohttp
     #   aiosignal
-fsspec==2023.10.0
+fsspec==2024.3.1
     # via
     #   datasets
     #   evaluate
     #   huggingface-hub
     #   lightning
     #   molflux
     #   pytorch-lightning
+    #   torch
     #   torch-geometric
-grpcio==1.60.1
-    # via tensorboard
-h5py==3.10.0
+h5py==3.11.0
     # via
     #   molflux
     #   physicsml (pyproject.toml)
 html5lib==1.1
     # via sphinx-toolbox
-huggingface-hub==0.20.3
+huggingface-hub==0.22.2
     # via
     #   datasets
     #   evaluate
-idna==3.6
+idna==3.7
     # via
     #   apeye-core
     #   requests
     #   yarl
 imagesize==1.4.1
     # via sphinx
 importlib-metadata==4.13.0
     # via
     #   jupyter-cache
+    #   jupyter-client
     #   myst-nb
     #   qlient-core
+    #   sphinx
     #   torchani
+importlib-resources==6.4.0
+    # via matplotlib
 iniconfig==2.0.0
     # via pytest
-ipykernel==6.29.2
+ipykernel==6.29.4
     # via myst-nb
-ipython==8.21.0
+ipython==8.18.1
     # via
     #   ipykernel
     #   ipywidgets
     #   myst-nb
 ipywidgets==8.1.2
     # via physicsml (pyproject.toml)
 jedi==0.19.1
@@ -185,66 +192,63 @@
     #   sphinx-jinja2-compat
     #   torch
     #   torch-geometric
 jmespath==1.0.1
     # via
     #   boto3
     #   botocore
-joblib==1.3.2
+joblib==1.4.0
     # via
     #   molflux
     #   scikit-learn
 jsonschema==4.21.1
     # via nbformat
 jsonschema-specifications==2023.12.1
     # via jsonschema
 jupyter-cache==1.0.0
     # via myst-nb
-jupyter-client==8.6.0
+jupyter-client==8.6.1
     # via
     #   ipykernel
     #   nbclient
-jupyter-core==5.7.1
+jupyter-core==5.7.2
     # via
     #   ipykernel
     #   jupyter-client
     #   nbclient
     #   nbformat
 jupyterlab-widgets==3.0.10
     # via ipywidgets
 jupytext==1.16.1
     # via physicsml (pyproject.toml)
 kiwisolver==1.4.5
     # via matplotlib
 lark-parser==0.12.0
     # via torchani
-lightning==2.2.0.post0
+lightning==2.2.3
     # via physicsml (pyproject.toml)
-lightning-utilities==0.10.1
+lightning-utilities==0.11.2
     # via
     #   lightning
     #   pytorch-lightning
     #   torchmetrics
-markdown==3.5.2
-    # via tensorboard
 markdown-it-py==3.0.0
     # via
     #   jupytext
     #   mdit-py-plugins
     #   myst-parser
 markupsafe==2.1.5
     # via
     #   jinja2
     #   sphinx-jinja2-compat
-    #   werkzeug
-matplotlib==3.8.3
+matplotlib==3.8.4
     # via
     #   ase
     #   physicsml (pyproject.toml)
-matplotlib-inline==0.1.6
+matplotlib-inline==0.1.7
     # via
     #   ipykernel
     #   ipython
 mdit-py-plugins==0.4.0
     # via
     #   jupytext
     #   myst-parser
@@ -254,35 +258,35 @@
     # via molflux
 molflux==0.3.0
     # via physicsml (pyproject.toml)
 more-itertools==10.2.0
     # via molflux
 mpmath==1.3.0
     # via sympy
-msgpack==1.0.7
+msgpack==1.0.8
     # via cachecontrol
 multidict==6.0.5
     # via
     #   aiohttp
     #   yarl
 multiprocess==0.70.16
     # via
     #   datasets
     #   evaluate
-myst-nb==1.0.0
+myst-nb==1.1.0
     # via physicsml (pyproject.toml)
-myst-parser==2.0.0
+myst-parser==3.0.0
     # via myst-nb
 natsort==8.4.0
     # via domdf-python-tools
-nbclient==0.9.0
+nbclient==0.10.0
     # via
     #   jupyter-cache
     #   myst-nb
-nbformat==5.9.2
+nbformat==5.10.4
     # via
     #   jupyter-cache
     #   jupytext
     #   myst-nb
     #   nbclient
 nest-asyncio==1.6.0
     # via ipykernel
@@ -301,22 +305,21 @@
     #   opt-einsum
     #   pandas
     #   pyarrow
     #   pytorch-lightning
     #   rdkit
     #   scikit-learn
     #   scipy
-    #   tensorboard
     #   torch-geometric
     #   torchmetrics
 opt-einsum==3.3.0
     # via opt-einsum-fx
 opt-einsum-fx==0.1.4
     # via e3nn
-packaging==23.2
+packaging==24.0
     # via
     #   datasets
     #   evaluate
     #   huggingface-hub
     #   ipykernel
     #   jupytext
     #   lightning
@@ -324,114 +327,111 @@
     #   matplotlib
     #   opt-einsum-fx
     #   pydata-sphinx-theme
     #   pytest
     #   pytorch-lightning
     #   sphinx
     #   torchmetrics
-pandas==2.2.0
+pandas==2.2.2
     # via
     #   datasets
     #   evaluate
     #   molflux
-parso==0.8.3
+parso==0.8.4
     # via jedi
 pexpect==4.9.0
     # via ipython
-pillow==10.2.0
+pillow==10.3.0
     # via
     #   matplotlib
     #   rdkit
-platformdirs==4.2.0
+platformdirs==4.2.1
     # via
     #   apeye
     #   jupyter-core
-pluggy==1.4.0
+pluggy==1.5.0
     # via pytest
 prompt-toolkit==3.0.43
     # via ipython
-protobuf==4.25.3
-    # via tensorboard
 psutil==5.9.8
     # via
     #   ipykernel
     #   torch-geometric
 ptyprocess==0.7.0
     # via pexpect
 pure-eval==0.2.2
     # via stack-data
-pyarrow==15.0.0
+pyarrow==16.0.0
     # via
     #   datasets
     #   molflux
 pyarrow-hotfix==0.6
     # via datasets
-pydantic==1.10.14
+pydantic==1.10.15
     # via molflux
 pydata-sphinx-theme==0.15.2
     # via sphinx-book-theme
 pygments==2.17.2
     # via
     #   accessible-pygments
     #   ipython
     #   pydata-sphinx-theme
     #   sphinx
     #   sphinx-prompt
     #   sphinx-tabs
-pyparsing==3.1.1
+pyparsing==3.1.2
     # via
     #   matplotlib
     #   torch-geometric
-pytest==8.0.1
+pytest==8.1.1
     # via physicsml (pyproject.toml)
-python-dateutil==2.8.2
+python-dateutil==2.9.0.post0
     # via
     #   botocore
     #   jupyter-client
     #   matplotlib
     #   molflux
     #   pandas
-pytorch-lightning==2.2.0.post0
+pytorch-lightning==2.2.3
     # via lightning
 pytz==2024.1
     # via pandas
 pyyaml==6.0.1
     # via
     #   datasets
     #   huggingface-hub
     #   jupyter-cache
     #   jupytext
     #   lightning
     #   molflux
     #   myst-nb
     #   myst-parser
     #   pytorch-lightning
-pyzmq==25.1.2
+pyzmq==26.0.2
     # via
     #   ipykernel
     #   jupyter-client
 qlient==1.0.0
     # via molflux
 qlient-core==1.0.1
     # via qlient
-rapidfuzz==3.6.1
+rapidfuzz==3.8.1
     # via thefuzz
 rdkit==2023.9.5
     # via physicsml (pyproject.toml)
-referencing==0.33.0
+referencing==0.35.0
     # via
     #   jsonschema
     #   jsonschema-specifications
 requests==2.31.0
     # via
     #   apeye
     #   cachecontrol
     #   datasets
     #   evaluate
-    #   fsspec
     #   huggingface-hub
     #   molflux
     #   qlient
     #   responses
     #   sphinx
     #   torch-geometric
     #   torchani
@@ -441,38 +441,37 @@
     # via
     #   jsonschema
     #   referencing
 ruamel-yaml==0.18.6
     # via sphinx-toolbox
 ruamel-yaml-clib==0.2.8
     # via ruamel-yaml
-s3transfer==0.10.0
+s3transfer==0.10.1
     # via boto3
-scikit-learn==1.4.1.post1
+scikit-learn==1.4.2
     # via
     #   molflux
     #   torch-geometric
-scipy==1.12.0
+scipy==1.13.0
     # via
     #   ase
     #   e3nn
     #   molflux
     #   scikit-learn
     #   torch-geometric
 six==1.16.0
     # via
     #   asttokens
     #   html5lib
     #   python-dateutil
-    #   tensorboard
 snowballstemmer==2.2.0
     # via sphinx
 soupsieve==2.5
     # via beautifulsoup4
-sphinx==7.2.6
+sphinx==7.3.7
     # via
     #   autodocsumm
     #   myst-nb
     #   myst-parser
     #   physicsml (pyproject.toml)
     #   pydata-sphinx-theme
     #   sphinx-autodoc-typehints
@@ -480,15 +479,15 @@
     #   sphinx-design
     #   sphinx-inline-tabs
     #   sphinx-prompt
     #   sphinx-sitemap
     #   sphinx-tabs
     #   sphinx-togglebutton
     #   sphinx-toolbox
-sphinx-autodoc-typehints==2.0.0
+sphinx-autodoc-typehints==2.1.0
     # via sphinx-toolbox
 sphinx-book-theme==1.1.2
     # via physicsml (pyproject.toml)
 sphinx-design==0.5.0
     # via physicsml (pyproject.toml)
 sphinx-inline-tabs==2023.4.21
     # via physicsml (pyproject.toml)
@@ -512,52 +511,53 @@
     # via sphinx
 sphinxcontrib-jsmath==1.0.1
     # via sphinx
 sphinxcontrib-qthelp==1.0.7
     # via sphinx
 sphinxcontrib-serializinghtml==1.1.10
     # via sphinx
-sqlalchemy==2.0.27
+sqlalchemy==2.0.29
     # via jupyter-cache
 stack-data==0.6.3
     # via ipython
 sympy==1.12
     # via
     #   e3nn
     #   torch
 tabulate==0.9.0
     # via
     #   jupyter-cache
     #   sphinx-toolbox
 tenacity==8.2.3
     # via molflux
-tensorboard==2.16.2
-    # via physicsml (pyproject.toml)
-tensorboard-data-server==0.7.2
-    # via tensorboard
 thefuzz==0.22.1
     # via molflux
-threadpoolctl==3.3.0
+threadpoolctl==3.4.0
     # via scikit-learn
 toml==0.10.2
     # via jupytext
-torch==2.0.1
+tomli==2.0.1
+    # via
+    #   coverage
+    #   pytest
+    #   sphinx
+torch==2.3.0
     # via
     #   e3nn
     #   lightning
     #   opt-einsum-fx
     #   physicsml (pyproject.toml)
     #   pytorch-lightning
     #   torchani
     #   torchmetrics
-torch-geometric==2.5.0
+torch-geometric==2.5.3
     # via physicsml (pyproject.toml)
 torchani==2.2.3
     # via physicsml (pyproject.toml)
-torchmetrics==1.3.1
+torchmetrics==1.3.2
     # via
     #   lightning
     #   pytorch-lightning
 tornado==6.4
     # via
     #   ipykernel
     #   jupyter-client
@@ -566,62 +566,64 @@
     #   datasets
     #   evaluate
     #   huggingface-hub
     #   lightning
     #   molflux
     #   pytorch-lightning
     #   torch-geometric
-traitlets==5.14.1
+traitlets==5.14.3
     # via
     #   comm
     #   ipykernel
     #   ipython
     #   ipywidgets
     #   jupyter-client
     #   jupyter-core
     #   matplotlib-inline
     #   nbclient
     #   nbformat
-typing-extensions==4.9.0
+typing-extensions==4.11.0
     # via
+    #   cloudpathlib
     #   domdf-python-tools
     #   huggingface-hub
+    #   ipython
     #   lightning
     #   lightning-utilities
     #   molflux
     #   myst-nb
     #   pydantic
     #   pydata-sphinx-theme
     #   pytorch-lightning
     #   sphinx-toolbox
     #   sqlalchemy
     #   torch
 tzdata==2024.1
     # via pandas
-urllib3==2.0.7
+urllib3==1.26.18
     # via
     #   botocore
     #   requests
     #   responses
 wcwidth==0.2.13
     # via prompt-toolkit
 webencodings==0.5.1
     # via html5lib
-websocket-client==1.7.0
+websocket-client==1.8.0
     # via qlient
-werkzeug==3.0.1
-    # via tensorboard
-wheel==0.42.0
+wheel==0.43.0
     # via sphinx-togglebutton
 widgetsnbextension==4.0.10
     # via ipywidgets
 xxhash==3.4.1
     # via
     #   datasets
     #   evaluate
 yarl==1.9.4
     # via aiohttp
-zipp==3.17.0
-    # via importlib-metadata
+zipp==3.18.1
+    # via
+    #   importlib-metadata
+    #   importlib-resources
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `physicsml-0.2.3/pinned-versions/3.8/lockfile.ase.txt` & `physicsml-0.2.4/pinned-versions/3.8/lockfile.openeye.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 #
 # This file is autogenerated by pip-compile with Python 3.8
 # by the following command:
 #
-#    nox -s dependencies_pin-3.8(extra='ase')
+#    nox -s dependencies_pin-3.8(extra='openeye')
 #
-absl-py==2.1.0
-    # via tensorboard
 accessible-pygments==0.0.4
     # via pydata-sphinx-theme
-aiohttp==3.9.3
+aiohttp==3.9.5
     # via
     #   datasets
     #   fsspec
     #   torch-geometric
 aiosignal==1.3.1
     # via aiohttp
 alabaster==0.7.13
@@ -45,54 +43,52 @@
     #   sphinx
 backcall==0.2.0
     # via ipython
 beautifulsoup4==4.12.3
     # via
     #   pydata-sphinx-theme
     #   sphinx-toolbox
-boto3==1.34.45
+boto3==1.34.91
     # via
     #   cloudpathlib
     #   molflux
-botocore==1.34.45
+botocore==1.34.91
     # via
     #   boto3
     #   molflux
     #   s3transfer
 cachecontrol==0.14.0
     # via sphinx-toolbox
-cachetools==5.3.2
-    # via google-auth
 certifi==2024.2.2
     # via requests
 charset-normalizer==3.3.2
     # via requests
 click==8.1.7
     # via jupyter-cache
-cloudpathlib==0.17.0
+cloudpathlib==0.18.1
     # via molflux
 colorama==0.4.6
     # via molflux
-comm==0.2.1
+comm==0.2.2
     # via
     #   ipykernel
     #   ipywidgets
 contourpy==1.1.1
     # via matplotlib
-coverage==7.4.1
+coverage==7.5.0
     # via
     #   coverage-badge
     #   physicsml (pyproject.toml)
-coverage-badge==1.1.0
+coverage-badge==1.1.1
     # via physicsml (pyproject.toml)
-cssutils==2.9.0
+cssutils==2.10.2
     # via dict2css
 cycler==0.12.1
     # via matplotlib
-datasets==2.17.1
+datasets==2.19.0
     # via
     #   evaluate
     #   molflux
 debugpy==1.8.1
     # via ipykernel
 decorator==5.1.1
     # via ipython
@@ -117,85 +113,77 @@
     #   apeye-core
     #   dict2css
     #   sphinx-toolbox
 e3nn==0.5.1
     # via physicsml (pyproject.toml)
 evaluate==0.4.1
     # via molflux
-exceptiongroup==1.2.0
+exceptiongroup==1.2.1
     # via pytest
 executing==2.0.1
     # via stack-data
 fastjsonschema==2.19.1
     # via nbformat
-filelock==3.13.1
+filelock==3.13.4
     # via
     #   cachecontrol
     #   datasets
     #   huggingface-hub
     #   sphinx-toolbox
     #   torch
-fonttools==4.49.0
+fonttools==4.51.0
     # via matplotlib
 frozenlist==1.4.1
     # via
     #   aiohttp
     #   aiosignal
-fsspec==2023.10.0
+fsspec==2024.3.1
     # via
     #   datasets
     #   evaluate
     #   huggingface-hub
     #   lightning
     #   molflux
     #   pytorch-lightning
+    #   torch
     #   torch-geometric
-google-auth==2.28.0
-    # via
-    #   google-auth-oauthlib
-    #   tensorboard
-google-auth-oauthlib==1.0.0
-    # via tensorboard
-grpcio==1.60.1
-    # via tensorboard
-h5py==3.10.0
+h5py==3.11.0
     # via
     #   molflux
     #   physicsml (pyproject.toml)
 html5lib==1.1
     # via sphinx-toolbox
-huggingface-hub==0.20.3
+huggingface-hub==0.22.2
     # via
     #   datasets
     #   evaluate
-idna==3.6
+idna==3.7
     # via
     #   apeye-core
     #   requests
     #   yarl
 imagesize==1.4.1
     # via sphinx
 importlib-metadata==4.13.0
     # via
     #   domdf-python-tools
     #   jupyter-cache
     #   jupyter-client
-    #   markdown
     #   myst-nb
     #   qlient-core
     #   sphinx
     #   torchani
-importlib-resources==6.1.1
+importlib-resources==6.4.0
     # via
     #   jsonschema
     #   jsonschema-specifications
     #   matplotlib
 iniconfig==2.0.0
     # via pytest
-ipykernel==6.29.2
+ipykernel==6.29.4
     # via myst-nb
 ipython==8.12.3
     # via
     #   ipykernel
     #   ipywidgets
     #   myst-nb
 ipywidgets==8.1.2
@@ -209,66 +197,63 @@
     #   sphinx-jinja2-compat
     #   torch
     #   torch-geometric
 jmespath==1.0.1
     # via
     #   boto3
     #   botocore
-joblib==1.3.2
+joblib==1.4.0
     # via
     #   molflux
     #   scikit-learn
 jsonschema==4.21.1
     # via nbformat
 jsonschema-specifications==2023.12.1
     # via jsonschema
 jupyter-cache==0.6.1
     # via myst-nb
-jupyter-client==8.6.0
+jupyter-client==8.6.1
     # via
     #   ipykernel
     #   nbclient
-jupyter-core==5.7.1
+jupyter-core==5.7.2
     # via
     #   ipykernel
     #   jupyter-client
     #   nbclient
     #   nbformat
 jupyterlab-widgets==3.0.10
     # via ipywidgets
 jupytext==1.16.1
     # via physicsml (pyproject.toml)
 kiwisolver==1.4.5
     # via matplotlib
 lark-parser==0.12.0
     # via torchani
-lightning==2.2.0.post0
+lightning==2.2.3
     # via physicsml (pyproject.toml)
-lightning-utilities==0.10.1
+lightning-utilities==0.11.2
     # via
     #   lightning
     #   pytorch-lightning
     #   torchmetrics
-markdown==3.5.2
-    # via tensorboard
 markdown-it-py==2.2.0
     # via
     #   jupytext
     #   mdit-py-plugins
     #   myst-parser
 markupsafe==2.1.5
     # via
     #   jinja2
     #   sphinx-jinja2-compat
-    #   werkzeug
 matplotlib==3.7.5
     # via
     #   ase
     #   physicsml (pyproject.toml)
-matplotlib-inline==0.1.6
+matplotlib-inline==0.1.7
     # via
     #   ipykernel
     #   ipython
 mdit-py-plugins==0.3.5
     # via
     #   jupytext
     #   myst-parser
@@ -278,15 +263,15 @@
     # via molflux
 molflux==0.3.0
     # via physicsml (pyproject.toml)
 more-itertools==10.2.0
     # via molflux
 mpmath==1.3.0
     # via sympy
-msgpack==1.0.7
+msgpack==1.0.8
     # via cachecontrol
 multidict==6.0.5
     # via
     #   aiohttp
     #   yarl
 multiprocess==0.70.16
     # via
@@ -298,15 +283,15 @@
     # via myst-nb
 natsort==8.4.0
     # via domdf-python-tools
 nbclient==0.7.4
     # via
     #   jupyter-cache
     #   myst-nb
-nbformat==5.9.2
+nbformat==5.10.4
     # via
     #   jupyter-cache
     #   jupytext
     #   myst-nb
     #   nbclient
 nest-asyncio==1.6.0
     # via ipykernel
@@ -325,24 +310,25 @@
     #   opt-einsum
     #   pandas
     #   pyarrow
     #   pytorch-lightning
     #   rdkit
     #   scikit-learn
     #   scipy
-    #   tensorboard
     #   torch-geometric
     #   torchmetrics
-oauthlib==3.2.2
-    # via requests-oauthlib
+openeye-toolkits==2022.2.2 ; python_version == "3.8"
+    # via physicsml (pyproject.toml)
+openeye-toolkits-python3-osx-universal==2022.2.2
+    # via openeye-toolkits
 opt-einsum==3.3.0
     # via opt-einsum-fx
 opt-einsum-fx==0.1.4
     # via e3nn
-packaging==23.2
+packaging==24.0
     # via
     #   datasets
     #   evaluate
     #   huggingface-hub
     #   ipykernel
     #   jupytext
     #   lightning
@@ -355,82 +341,74 @@
     #   sphinx
     #   torchmetrics
 pandas==2.0.3
     # via
     #   datasets
     #   evaluate
     #   molflux
-parso==0.8.3
+parso==0.8.4
     # via jedi
 pexpect==4.9.0
     # via ipython
 pickleshare==0.7.5
     # via ipython
-pillow==10.2.0
+pillow==10.3.0
     # via
     #   matplotlib
     #   rdkit
 pkgutil-resolve-name==1.3.10
     # via jsonschema
-platformdirs==4.2.0
+platformdirs==4.2.1
     # via
     #   apeye
     #   jupyter-core
-pluggy==1.4.0
+pluggy==1.5.0
     # via pytest
 prompt-toolkit==3.0.43
     # via ipython
-protobuf==4.25.3
-    # via tensorboard
 psutil==5.9.8
     # via
     #   ipykernel
     #   torch-geometric
 ptyprocess==0.7.0
     # via pexpect
 pure-eval==0.2.2
     # via stack-data
-pyarrow==15.0.0
+pyarrow==16.0.0
     # via
     #   datasets
     #   molflux
 pyarrow-hotfix==0.6
     # via datasets
-pyasn1==0.5.1
-    # via
-    #   pyasn1-modules
-    #   rsa
-pyasn1-modules==0.3.0
-    # via google-auth
-pydantic==1.10.14
+pydantic==1.10.15
     # via molflux
 pydata-sphinx-theme==0.14.4
     # via sphinx-book-theme
 pygments==2.17.2
     # via
     #   accessible-pygments
     #   ipython
     #   pydata-sphinx-theme
     #   sphinx
     #   sphinx-prompt
     #   sphinx-tabs
-pyparsing==3.1.1
+pyparsing==3.1.2
     # via
     #   matplotlib
     #   torch-geometric
-pytest==8.0.1
+pytest==8.1.1
     # via physicsml (pyproject.toml)
-python-dateutil==2.8.2
+python-dateutil==2.9.0.post0
     # via
     #   botocore
     #   jupyter-client
     #   matplotlib
     #   molflux
     #   pandas
-pytorch-lightning==2.2.0.post0
+pytorch-lightning==2.2.3
     # via lightning
 pytz==2024.1
     # via
     #   babel
     #   pandas
 pyyaml==6.0.1
     # via
@@ -439,61 +417,54 @@
     #   jupyter-cache
     #   jupytext
     #   lightning
     #   molflux
     #   myst-nb
     #   myst-parser
     #   pytorch-lightning
-pyzmq==25.1.2
+pyzmq==26.0.2
     # via
     #   ipykernel
     #   jupyter-client
 qlient==1.0.0
     # via molflux
 qlient-core==1.0.1
     # via qlient
-rapidfuzz==3.6.1
+rapidfuzz==3.8.1
     # via thefuzz
 rdkit==2023.9.5
     # via physicsml (pyproject.toml)
-referencing==0.33.0
+referencing==0.35.0
     # via
     #   jsonschema
     #   jsonschema-specifications
 requests==2.31.0
     # via
     #   apeye
     #   cachecontrol
     #   datasets
     #   evaluate
-    #   fsspec
     #   huggingface-hub
     #   molflux
     #   qlient
-    #   requests-oauthlib
     #   responses
     #   sphinx
-    #   tensorboard
     #   torch-geometric
     #   torchani
-requests-oauthlib==1.3.1
-    # via google-auth-oauthlib
 responses==0.18.0
     # via evaluate
 rpds-py==0.18.0
     # via
     #   jsonschema
     #   referencing
-rsa==4.9
-    # via google-auth
 ruamel-yaml==0.18.6
     # via sphinx-toolbox
 ruamel-yaml-clib==0.2.8
     # via ruamel-yaml
-s3transfer==0.10.0
+s3transfer==0.10.1
     # via boto3
 scikit-learn==1.3.2
     # via
     #   molflux
     #   torch-geometric
 scipy==1.10.1
     # via
@@ -555,56 +526,52 @@
     # via sphinx
 sphinxcontrib-jsmath==1.0.1
     # via sphinx
 sphinxcontrib-qthelp==1.0.3
     # via sphinx
 sphinxcontrib-serializinghtml==1.1.5
     # via sphinx
-sqlalchemy==2.0.27
+sqlalchemy==2.0.29
     # via jupyter-cache
 stack-data==0.6.3
     # via ipython
 sympy==1.12
     # via
     #   e3nn
     #   torch
 tabulate==0.9.0
     # via
     #   jupyter-cache
     #   sphinx-toolbox
 tenacity==8.2.3
     # via molflux
-tensorboard==2.14.0
-    # via physicsml (pyproject.toml)
-tensorboard-data-server==0.7.2
-    # via tensorboard
 thefuzz==0.22.1
     # via molflux
-threadpoolctl==3.3.0
+threadpoolctl==3.4.0
     # via scikit-learn
 toml==0.10.2
     # via jupytext
 tomli==2.0.1
     # via
     #   coverage
     #   pytest
-torch==2.0.1
+torch==2.3.0
     # via
     #   e3nn
     #   lightning
     #   opt-einsum-fx
     #   physicsml (pyproject.toml)
     #   pytorch-lightning
     #   torchani
     #   torchmetrics
-torch-geometric==2.5.0
+torch-geometric==2.5.3
     # via physicsml (pyproject.toml)
 torchani==2.2.3
     # via physicsml (pyproject.toml)
-torchmetrics==1.3.1
+torchmetrics==1.3.2
     # via
     #   lightning
     #   pytorch-lightning
 tornado==6.4
     # via
     #   ipykernel
     #   jupyter-client
@@ -613,26 +580,26 @@
     #   datasets
     #   evaluate
     #   huggingface-hub
     #   lightning
     #   molflux
     #   pytorch-lightning
     #   torch-geometric
-traitlets==5.14.1
+traitlets==5.14.3
     # via
     #   comm
     #   ipykernel
     #   ipython
     #   ipywidgets
     #   jupyter-client
     #   jupyter-core
     #   matplotlib-inline
     #   nbclient
     #   nbformat
-typing-extensions==4.9.0
+typing-extensions==4.11.0
     # via
     #   cloudpathlib
     #   domdf-python-tools
     #   huggingface-hub
     #   ipython
     #   lightning
     #   lightning-utilities
@@ -653,30 +620,26 @@
     #   botocore
     #   requests
     #   responses
 wcwidth==0.2.13
     # via prompt-toolkit
 webencodings==0.5.1
     # via html5lib
-websocket-client==1.7.0
+websocket-client==1.8.0
     # via qlient
-werkzeug==3.0.1
-    # via tensorboard
-wheel==0.42.0
-    # via
-    #   sphinx-togglebutton
-    #   tensorboard
+wheel==0.43.0
+    # via sphinx-togglebutton
 widgetsnbextension==4.0.10
     # via ipywidgets
 xxhash==3.4.1
     # via
     #   datasets
     #   evaluate
 yarl==1.9.4
     # via aiohttp
-zipp==3.17.0
+zipp==3.18.1
     # via
     #   importlib-metadata
     #   importlib-resources
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `physicsml-0.2.3/pinned-versions/3.8/lockfile.core.txt` & `physicsml-0.2.4/pinned-versions/3.8/lockfile.ase.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 #
 # This file is autogenerated by pip-compile with Python 3.8
 # by the following command:
 #
-#    nox -s dependencies_pin-3.8(extra=None)
+#    nox -s dependencies_pin-3.8(extra='ase')
 #
-absl-py==2.1.0
-    # via tensorboard
 accessible-pygments==0.0.4
     # via pydata-sphinx-theme
-aiohttp==3.9.3
+aiohttp==3.9.5
     # via
     #   datasets
     #   fsspec
     #   torch-geometric
 aiosignal==1.3.1
     # via aiohttp
 alabaster==0.7.13
@@ -45,54 +43,52 @@
     #   sphinx
 backcall==0.2.0
     # via ipython
 beautifulsoup4==4.12.3
     # via
     #   pydata-sphinx-theme
     #   sphinx-toolbox
-boto3==1.34.45
+boto3==1.34.91
     # via
     #   cloudpathlib
     #   molflux
-botocore==1.34.45
+botocore==1.34.91
     # via
     #   boto3
     #   molflux
     #   s3transfer
 cachecontrol==0.14.0
     # via sphinx-toolbox
-cachetools==5.3.2
-    # via google-auth
 certifi==2024.2.2
     # via requests
 charset-normalizer==3.3.2
     # via requests
 click==8.1.7
     # via jupyter-cache
-cloudpathlib==0.17.0
+cloudpathlib==0.18.1
     # via molflux
 colorama==0.4.6
     # via molflux
-comm==0.2.1
+comm==0.2.2
     # via
     #   ipykernel
     #   ipywidgets
 contourpy==1.1.1
     # via matplotlib
-coverage==7.4.1
+coverage==7.5.0
     # via
     #   coverage-badge
     #   physicsml (pyproject.toml)
-coverage-badge==1.1.0
+coverage-badge==1.1.1
     # via physicsml (pyproject.toml)
-cssutils==2.9.0
+cssutils==2.10.2
     # via dict2css
 cycler==0.12.1
     # via matplotlib
-datasets==2.17.1
+datasets==2.19.0
     # via
     #   evaluate
     #   molflux
 debugpy==1.8.1
     # via ipykernel
 decorator==5.1.1
     # via ipython
@@ -117,85 +113,77 @@
     #   apeye-core
     #   dict2css
     #   sphinx-toolbox
 e3nn==0.5.1
     # via physicsml (pyproject.toml)
 evaluate==0.4.1
     # via molflux
-exceptiongroup==1.2.0
+exceptiongroup==1.2.1
     # via pytest
 executing==2.0.1
     # via stack-data
 fastjsonschema==2.19.1
     # via nbformat
-filelock==3.13.1
+filelock==3.13.4
     # via
     #   cachecontrol
     #   datasets
     #   huggingface-hub
     #   sphinx-toolbox
     #   torch
-fonttools==4.49.0
+fonttools==4.51.0
     # via matplotlib
 frozenlist==1.4.1
     # via
     #   aiohttp
     #   aiosignal
-fsspec==2023.10.0
+fsspec==2024.3.1
     # via
     #   datasets
     #   evaluate
     #   huggingface-hub
     #   lightning
     #   molflux
     #   pytorch-lightning
+    #   torch
     #   torch-geometric
-google-auth==2.28.0
-    # via
-    #   google-auth-oauthlib
-    #   tensorboard
-google-auth-oauthlib==1.0.0
-    # via tensorboard
-grpcio==1.60.1
-    # via tensorboard
-h5py==3.10.0
+h5py==3.11.0
     # via
     #   molflux
     #   physicsml (pyproject.toml)
 html5lib==1.1
     # via sphinx-toolbox
-huggingface-hub==0.20.3
+huggingface-hub==0.22.2
     # via
     #   datasets
     #   evaluate
-idna==3.6
+idna==3.7
     # via
     #   apeye-core
     #   requests
     #   yarl
 imagesize==1.4.1
     # via sphinx
 importlib-metadata==4.13.0
     # via
     #   domdf-python-tools
     #   jupyter-cache
     #   jupyter-client
-    #   markdown
     #   myst-nb
     #   qlient-core
     #   sphinx
     #   torchani
-importlib-resources==6.1.1
+importlib-resources==6.4.0
     # via
     #   jsonschema
     #   jsonschema-specifications
     #   matplotlib
 iniconfig==2.0.0
     # via pytest
-ipykernel==6.29.2
+ipykernel==6.29.4
     # via myst-nb
 ipython==8.12.3
     # via
     #   ipykernel
     #   ipywidgets
     #   myst-nb
 ipywidgets==8.1.2
@@ -209,66 +197,63 @@
     #   sphinx-jinja2-compat
     #   torch
     #   torch-geometric
 jmespath==1.0.1
     # via
     #   boto3
     #   botocore
-joblib==1.3.2
+joblib==1.4.0
     # via
     #   molflux
     #   scikit-learn
 jsonschema==4.21.1
     # via nbformat
 jsonschema-specifications==2023.12.1
     # via jsonschema
 jupyter-cache==0.6.1
     # via myst-nb
-jupyter-client==8.6.0
+jupyter-client==8.6.1
     # via
     #   ipykernel
     #   nbclient
-jupyter-core==5.7.1
+jupyter-core==5.7.2
     # via
     #   ipykernel
     #   jupyter-client
     #   nbclient
     #   nbformat
 jupyterlab-widgets==3.0.10
     # via ipywidgets
 jupytext==1.16.1
     # via physicsml (pyproject.toml)
 kiwisolver==1.4.5
     # via matplotlib
 lark-parser==0.12.0
     # via torchani
-lightning==2.2.0.post0
+lightning==2.2.3
     # via physicsml (pyproject.toml)
-lightning-utilities==0.10.1
+lightning-utilities==0.11.2
     # via
     #   lightning
     #   pytorch-lightning
     #   torchmetrics
-markdown==3.5.2
-    # via tensorboard
 markdown-it-py==2.2.0
     # via
     #   jupytext
     #   mdit-py-plugins
     #   myst-parser
 markupsafe==2.1.5
     # via
     #   jinja2
     #   sphinx-jinja2-compat
-    #   werkzeug
 matplotlib==3.7.5
     # via
     #   ase
     #   physicsml (pyproject.toml)
-matplotlib-inline==0.1.6
+matplotlib-inline==0.1.7
     # via
     #   ipykernel
     #   ipython
 mdit-py-plugins==0.3.5
     # via
     #   jupytext
     #   myst-parser
@@ -278,15 +263,15 @@
     # via molflux
 molflux==0.3.0
     # via physicsml (pyproject.toml)
 more-itertools==10.2.0
     # via molflux
 mpmath==1.3.0
     # via sympy
-msgpack==1.0.7
+msgpack==1.0.8
     # via cachecontrol
 multidict==6.0.5
     # via
     #   aiohttp
     #   yarl
 multiprocess==0.70.16
     # via
@@ -298,15 +283,15 @@
     # via myst-nb
 natsort==8.4.0
     # via domdf-python-tools
 nbclient==0.7.4
     # via
     #   jupyter-cache
     #   myst-nb
-nbformat==5.9.2
+nbformat==5.10.4
     # via
     #   jupyter-cache
     #   jupytext
     #   myst-nb
     #   nbclient
 nest-asyncio==1.6.0
     # via ipykernel
@@ -325,24 +310,21 @@
     #   opt-einsum
     #   pandas
     #   pyarrow
     #   pytorch-lightning
     #   rdkit
     #   scikit-learn
     #   scipy
-    #   tensorboard
     #   torch-geometric
     #   torchmetrics
-oauthlib==3.2.2
-    # via requests-oauthlib
 opt-einsum==3.3.0
     # via opt-einsum-fx
 opt-einsum-fx==0.1.4
     # via e3nn
-packaging==23.2
+packaging==24.0
     # via
     #   datasets
     #   evaluate
     #   huggingface-hub
     #   ipykernel
     #   jupytext
     #   lightning
@@ -355,82 +337,74 @@
     #   sphinx
     #   torchmetrics
 pandas==2.0.3
     # via
     #   datasets
     #   evaluate
     #   molflux
-parso==0.8.3
+parso==0.8.4
     # via jedi
 pexpect==4.9.0
     # via ipython
 pickleshare==0.7.5
     # via ipython
-pillow==10.2.0
+pillow==10.3.0
     # via
     #   matplotlib
     #   rdkit
 pkgutil-resolve-name==1.3.10
     # via jsonschema
-platformdirs==4.2.0
+platformdirs==4.2.1
     # via
     #   apeye
     #   jupyter-core
-pluggy==1.4.0
+pluggy==1.5.0
     # via pytest
 prompt-toolkit==3.0.43
     # via ipython
-protobuf==4.25.3
-    # via tensorboard
 psutil==5.9.8
     # via
     #   ipykernel
     #   torch-geometric
 ptyprocess==0.7.0
     # via pexpect
 pure-eval==0.2.2
     # via stack-data
-pyarrow==15.0.0
+pyarrow==16.0.0
     # via
     #   datasets
     #   molflux
 pyarrow-hotfix==0.6
     # via datasets
-pyasn1==0.5.1
-    # via
-    #   pyasn1-modules
-    #   rsa
-pyasn1-modules==0.3.0
-    # via google-auth
-pydantic==1.10.14
+pydantic==1.10.15
     # via molflux
 pydata-sphinx-theme==0.14.4
     # via sphinx-book-theme
 pygments==2.17.2
     # via
     #   accessible-pygments
     #   ipython
     #   pydata-sphinx-theme
     #   sphinx
     #   sphinx-prompt
     #   sphinx-tabs
-pyparsing==3.1.1
+pyparsing==3.1.2
     # via
     #   matplotlib
     #   torch-geometric
-pytest==8.0.1
+pytest==8.1.1
     # via physicsml (pyproject.toml)
-python-dateutil==2.8.2
+python-dateutil==2.9.0.post0
     # via
     #   botocore
     #   jupyter-client
     #   matplotlib
     #   molflux
     #   pandas
-pytorch-lightning==2.2.0.post0
+pytorch-lightning==2.2.3
     # via lightning
 pytz==2024.1
     # via
     #   babel
     #   pandas
 pyyaml==6.0.1
     # via
@@ -439,61 +413,54 @@
     #   jupyter-cache
     #   jupytext
     #   lightning
     #   molflux
     #   myst-nb
     #   myst-parser
     #   pytorch-lightning
-pyzmq==25.1.2
+pyzmq==26.0.2
     # via
     #   ipykernel
     #   jupyter-client
 qlient==1.0.0
     # via molflux
 qlient-core==1.0.1
     # via qlient
-rapidfuzz==3.6.1
+rapidfuzz==3.8.1
     # via thefuzz
 rdkit==2023.9.5
     # via physicsml (pyproject.toml)
-referencing==0.33.0
+referencing==0.35.0
     # via
     #   jsonschema
     #   jsonschema-specifications
 requests==2.31.0
     # via
     #   apeye
     #   cachecontrol
     #   datasets
     #   evaluate
-    #   fsspec
     #   huggingface-hub
     #   molflux
     #   qlient
-    #   requests-oauthlib
     #   responses
     #   sphinx
-    #   tensorboard
     #   torch-geometric
     #   torchani
-requests-oauthlib==1.3.1
-    # via google-auth-oauthlib
 responses==0.18.0
     # via evaluate
 rpds-py==0.18.0
     # via
     #   jsonschema
     #   referencing
-rsa==4.9
-    # via google-auth
 ruamel-yaml==0.18.6
     # via sphinx-toolbox
 ruamel-yaml-clib==0.2.8
     # via ruamel-yaml
-s3transfer==0.10.0
+s3transfer==0.10.1
     # via boto3
 scikit-learn==1.3.2
     # via
     #   molflux
     #   torch-geometric
 scipy==1.10.1
     # via
@@ -555,56 +522,52 @@
     # via sphinx
 sphinxcontrib-jsmath==1.0.1
     # via sphinx
 sphinxcontrib-qthelp==1.0.3
     # via sphinx
 sphinxcontrib-serializinghtml==1.1.5
     # via sphinx
-sqlalchemy==2.0.27
+sqlalchemy==2.0.29
     # via jupyter-cache
 stack-data==0.6.3
     # via ipython
 sympy==1.12
     # via
     #   e3nn
     #   torch
 tabulate==0.9.0
     # via
     #   jupyter-cache
     #   sphinx-toolbox
 tenacity==8.2.3
     # via molflux
-tensorboard==2.14.0
-    # via physicsml (pyproject.toml)
-tensorboard-data-server==0.7.2
-    # via tensorboard
 thefuzz==0.22.1
     # via molflux
-threadpoolctl==3.3.0
+threadpoolctl==3.4.0
     # via scikit-learn
 toml==0.10.2
     # via jupytext
 tomli==2.0.1
     # via
     #   coverage
     #   pytest
-torch==2.0.1
+torch==2.3.0
     # via
     #   e3nn
     #   lightning
     #   opt-einsum-fx
     #   physicsml (pyproject.toml)
     #   pytorch-lightning
     #   torchani
     #   torchmetrics
-torch-geometric==2.5.0
+torch-geometric==2.5.3
     # via physicsml (pyproject.toml)
 torchani==2.2.3
     # via physicsml (pyproject.toml)
-torchmetrics==1.3.1
+torchmetrics==1.3.2
     # via
     #   lightning
     #   pytorch-lightning
 tornado==6.4
     # via
     #   ipykernel
     #   jupyter-client
@@ -613,26 +576,26 @@
     #   datasets
     #   evaluate
     #   huggingface-hub
     #   lightning
     #   molflux
     #   pytorch-lightning
     #   torch-geometric
-traitlets==5.14.1
+traitlets==5.14.3
     # via
     #   comm
     #   ipykernel
     #   ipython
     #   ipywidgets
     #   jupyter-client
     #   jupyter-core
     #   matplotlib-inline
     #   nbclient
     #   nbformat
-typing-extensions==4.9.0
+typing-extensions==4.11.0
     # via
     #   cloudpathlib
     #   domdf-python-tools
     #   huggingface-hub
     #   ipython
     #   lightning
     #   lightning-utilities
@@ -653,30 +616,26 @@
     #   botocore
     #   requests
     #   responses
 wcwidth==0.2.13
     # via prompt-toolkit
 webencodings==0.5.1
     # via html5lib
-websocket-client==1.7.0
+websocket-client==1.8.0
     # via qlient
-werkzeug==3.0.1
-    # via tensorboard
-wheel==0.42.0
-    # via
-    #   sphinx-togglebutton
-    #   tensorboard
+wheel==0.43.0
+    # via sphinx-togglebutton
 widgetsnbextension==4.0.10
     # via ipywidgets
 xxhash==3.4.1
     # via
     #   datasets
     #   evaluate
 yarl==1.9.4
     # via aiohttp
-zipp==3.17.0
+zipp==3.18.1
     # via
     #   importlib-metadata
     #   importlib-resources
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `physicsml-0.2.3/pinned-versions/3.8/lockfile.openeye.txt` & `physicsml-0.2.4/pinned-versions/3.11/lockfile.core.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,203 +1,176 @@
 #
-# This file is autogenerated by pip-compile with Python 3.8
+# This file is autogenerated by pip-compile with Python 3.11
 # by the following command:
 #
-#    nox -s dependencies_pin-3.8(extra='openeye')
+#    nox -s dependencies_pin-3.11(extra=None)
 #
-absl-py==2.1.0
-    # via tensorboard
 accessible-pygments==0.0.4
     # via pydata-sphinx-theme
-aiohttp==3.9.3
+aiohttp==3.9.5
     # via
     #   datasets
     #   fsspec
     #   torch-geometric
 aiosignal==1.3.1
     # via aiohttp
-alabaster==0.7.13
+alabaster==0.7.16
     # via sphinx
 apeye==1.4.1
     # via sphinx-toolbox
 apeye-core==1.1.5
     # via apeye
 appnope==0.1.4
-    # via
-    #   ipykernel
-    #   ipython
+    # via ipykernel
 ase==3.22.1
     # via physicsml (pyproject.toml)
 asttokens==2.4.1
     # via stack-data
-async-timeout==4.0.3
-    # via aiohttp
 attrs==23.2.0
     # via
     #   aiohttp
     #   jsonschema
     #   jupyter-cache
     #   referencing
 autodocsumm==0.2.12
     # via sphinx-toolbox
 babel==2.14.0
     # via
     #   pydata-sphinx-theme
     #   sphinx
-backcall==0.2.0
-    # via ipython
 beautifulsoup4==4.12.3
     # via
     #   pydata-sphinx-theme
     #   sphinx-toolbox
-boto3==1.34.45
+boto3==1.34.91
     # via
     #   cloudpathlib
     #   molflux
-botocore==1.34.45
+botocore==1.34.91
     # via
     #   boto3
     #   molflux
     #   s3transfer
 cachecontrol==0.14.0
     # via sphinx-toolbox
-cachetools==5.3.2
-    # via google-auth
 certifi==2024.2.2
     # via requests
 charset-normalizer==3.3.2
     # via requests
 click==8.1.7
     # via jupyter-cache
-cloudpathlib==0.17.0
+cloudpathlib==0.18.1
     # via molflux
 colorama==0.4.6
     # via molflux
-comm==0.2.1
+comm==0.2.2
     # via
     #   ipykernel
     #   ipywidgets
-contourpy==1.1.1
+contourpy==1.2.1
     # via matplotlib
-coverage==7.4.1
+coverage==7.5.0
     # via
     #   coverage-badge
     #   physicsml (pyproject.toml)
-coverage-badge==1.1.0
+coverage-badge==1.1.1
     # via physicsml (pyproject.toml)
-cssutils==2.9.0
+cssutils==2.10.2
     # via dict2css
 cycler==0.12.1
     # via matplotlib
-datasets==2.17.1
+datasets==2.19.0
     # via
     #   evaluate
     #   molflux
 debugpy==1.8.1
     # via ipykernel
 decorator==5.1.1
     # via ipython
 dict2css==0.3.0.post1
     # via sphinx-toolbox
 dill==0.3.8
     # via
     #   datasets
     #   evaluate
     #   multiprocess
-docutils==0.19
+docutils==0.21.2
     # via
     #   myst-parser
     #   pydata-sphinx-theme
     #   sphinx
+    #   sphinx-prompt
     #   sphinx-tabs
     #   sphinx-togglebutton
     #   sphinx-toolbox
 domdf-python-tools==3.8.0.post2
     # via
     #   apeye
     #   apeye-core
     #   dict2css
     #   sphinx-toolbox
 e3nn==0.5.1
     # via physicsml (pyproject.toml)
 evaluate==0.4.1
     # via molflux
-exceptiongroup==1.2.0
-    # via pytest
 executing==2.0.1
     # via stack-data
 fastjsonschema==2.19.1
     # via nbformat
-filelock==3.13.1
+filelock==3.13.4
     # via
     #   cachecontrol
     #   datasets
     #   huggingface-hub
     #   sphinx-toolbox
     #   torch
-fonttools==4.49.0
+fonttools==4.51.0
     # via matplotlib
 frozenlist==1.4.1
     # via
     #   aiohttp
     #   aiosignal
-fsspec==2023.10.0
+fsspec==2024.3.1
     # via
     #   datasets
     #   evaluate
     #   huggingface-hub
     #   lightning
     #   molflux
     #   pytorch-lightning
+    #   torch
     #   torch-geometric
-google-auth==2.28.0
-    # via
-    #   google-auth-oauthlib
-    #   tensorboard
-google-auth-oauthlib==1.0.0
-    # via tensorboard
-grpcio==1.60.1
-    # via tensorboard
-h5py==3.10.0
+h5py==3.11.0
     # via
     #   molflux
     #   physicsml (pyproject.toml)
 html5lib==1.1
     # via sphinx-toolbox
-huggingface-hub==0.20.3
+huggingface-hub==0.22.2
     # via
     #   datasets
     #   evaluate
-idna==3.6
+idna==3.7
     # via
     #   apeye-core
     #   requests
     #   yarl
 imagesize==1.4.1
     # via sphinx
 importlib-metadata==4.13.0
     # via
-    #   domdf-python-tools
     #   jupyter-cache
-    #   jupyter-client
-    #   markdown
     #   myst-nb
     #   qlient-core
-    #   sphinx
     #   torchani
-importlib-resources==6.1.1
-    # via
-    #   jsonschema
-    #   jsonschema-specifications
-    #   matplotlib
 iniconfig==2.0.0
     # via pytest
-ipykernel==6.29.2
+ipykernel==6.29.4
     # via myst-nb
-ipython==8.12.3
+ipython==8.23.0
     # via
     #   ipykernel
     #   ipywidgets
     #   myst-nb
 ipywidgets==8.1.2
     # via physicsml (pyproject.toml)
 jedi==0.19.1
@@ -209,114 +182,111 @@
     #   sphinx-jinja2-compat
     #   torch
     #   torch-geometric
 jmespath==1.0.1
     # via
     #   boto3
     #   botocore
-joblib==1.3.2
+joblib==1.4.0
     # via
     #   molflux
     #   scikit-learn
 jsonschema==4.21.1
     # via nbformat
 jsonschema-specifications==2023.12.1
     # via jsonschema
-jupyter-cache==0.6.1
+jupyter-cache==1.0.0
     # via myst-nb
-jupyter-client==8.6.0
+jupyter-client==8.6.1
     # via
     #   ipykernel
     #   nbclient
-jupyter-core==5.7.1
+jupyter-core==5.7.2
     # via
     #   ipykernel
     #   jupyter-client
     #   nbclient
     #   nbformat
 jupyterlab-widgets==3.0.10
     # via ipywidgets
 jupytext==1.16.1
     # via physicsml (pyproject.toml)
 kiwisolver==1.4.5
     # via matplotlib
 lark-parser==0.12.0
     # via torchani
-lightning==2.2.0.post0
+lightning==2.2.3
     # via physicsml (pyproject.toml)
-lightning-utilities==0.10.1
+lightning-utilities==0.11.2
     # via
     #   lightning
     #   pytorch-lightning
     #   torchmetrics
-markdown==3.5.2
-    # via tensorboard
-markdown-it-py==2.2.0
+markdown-it-py==3.0.0
     # via
     #   jupytext
     #   mdit-py-plugins
     #   myst-parser
 markupsafe==2.1.5
     # via
     #   jinja2
     #   sphinx-jinja2-compat
-    #   werkzeug
-matplotlib==3.7.5
+matplotlib==3.8.4
     # via
     #   ase
     #   physicsml (pyproject.toml)
-matplotlib-inline==0.1.6
+matplotlib-inline==0.1.7
     # via
     #   ipykernel
     #   ipython
-mdit-py-plugins==0.3.5
+mdit-py-plugins==0.4.0
     # via
     #   jupytext
     #   myst-parser
 mdurl==0.1.2
     # via markdown-it-py
 mergedeep==1.3.4
     # via molflux
 molflux==0.3.0
     # via physicsml (pyproject.toml)
 more-itertools==10.2.0
     # via molflux
 mpmath==1.3.0
     # via sympy
-msgpack==1.0.7
+msgpack==1.0.8
     # via cachecontrol
 multidict==6.0.5
     # via
     #   aiohttp
     #   yarl
 multiprocess==0.70.16
     # via
     #   datasets
     #   evaluate
-myst-nb==0.17.2
+myst-nb==1.1.0
     # via physicsml (pyproject.toml)
-myst-parser==0.18.1
+myst-parser==3.0.0
     # via myst-nb
 natsort==8.4.0
     # via domdf-python-tools
-nbclient==0.7.4
+nbclient==0.10.0
     # via
     #   jupyter-cache
     #   myst-nb
-nbformat==5.9.2
+nbformat==5.10.4
     # via
     #   jupyter-cache
     #   jupytext
     #   myst-nb
     #   nbclient
 nest-asyncio==1.6.0
     # via ipykernel
-networkx==3.1
+networkx==3.3
     # via torch
-numpy==1.24.4
+numpy==1.26.4
     # via
     #   ase
     #   contourpy
     #   datasets
     #   evaluate
     #   h5py
     #   lightning
@@ -325,28 +295,21 @@
     #   opt-einsum
     #   pandas
     #   pyarrow
     #   pytorch-lightning
     #   rdkit
     #   scikit-learn
     #   scipy
-    #   tensorboard
     #   torch-geometric
     #   torchmetrics
-oauthlib==3.2.2
-    # via requests-oauthlib
-openeye-toolkits==2022.2.2 ; python_version == "3.8"
-    # via physicsml (pyproject.toml)
-openeye-toolkits-python3-osx-universal==2022.2.2
-    # via openeye-toolkits
 opt-einsum==3.3.0
     # via opt-einsum-fx
 opt-einsum-fx==0.1.4
     # via e3nn
-packaging==23.2
+packaging==24.0
     # via
     #   datasets
     #   evaluate
     #   huggingface-hub
     #   ipykernel
     #   jupytext
     #   lightning
@@ -354,156 +317,135 @@
     #   matplotlib
     #   opt-einsum-fx
     #   pydata-sphinx-theme
     #   pytest
     #   pytorch-lightning
     #   sphinx
     #   torchmetrics
-pandas==2.0.3
+pandas==2.2.2
     # via
     #   datasets
     #   evaluate
     #   molflux
-parso==0.8.3
+parso==0.8.4
     # via jedi
 pexpect==4.9.0
     # via ipython
-pickleshare==0.7.5
-    # via ipython
-pillow==10.2.0
+pillow==10.3.0
     # via
     #   matplotlib
     #   rdkit
-pkgutil-resolve-name==1.3.10
-    # via jsonschema
-platformdirs==4.2.0
+platformdirs==4.2.1
     # via
     #   apeye
     #   jupyter-core
-pluggy==1.4.0
+pluggy==1.5.0
     # via pytest
 prompt-toolkit==3.0.43
     # via ipython
-protobuf==4.25.3
-    # via tensorboard
 psutil==5.9.8
     # via
     #   ipykernel
     #   torch-geometric
 ptyprocess==0.7.0
     # via pexpect
 pure-eval==0.2.2
     # via stack-data
-pyarrow==15.0.0
+pyarrow==16.0.0
     # via
     #   datasets
     #   molflux
 pyarrow-hotfix==0.6
     # via datasets
-pyasn1==0.5.1
-    # via
-    #   pyasn1-modules
-    #   rsa
-pyasn1-modules==0.3.0
-    # via google-auth
-pydantic==1.10.14
+pydantic==1.10.15
     # via molflux
-pydata-sphinx-theme==0.14.4
+pydata-sphinx-theme==0.15.2
     # via sphinx-book-theme
 pygments==2.17.2
     # via
     #   accessible-pygments
     #   ipython
     #   pydata-sphinx-theme
     #   sphinx
     #   sphinx-prompt
     #   sphinx-tabs
-pyparsing==3.1.1
+pyparsing==3.1.2
     # via
     #   matplotlib
     #   torch-geometric
-pytest==8.0.1
+pytest==8.1.1
     # via physicsml (pyproject.toml)
-python-dateutil==2.8.2
+python-dateutil==2.9.0.post0
     # via
     #   botocore
     #   jupyter-client
     #   matplotlib
     #   molflux
     #   pandas
-pytorch-lightning==2.2.0.post0
+pytorch-lightning==2.2.3
     # via lightning
 pytz==2024.1
-    # via
-    #   babel
-    #   pandas
+    # via pandas
 pyyaml==6.0.1
     # via
     #   datasets
     #   huggingface-hub
     #   jupyter-cache
     #   jupytext
     #   lightning
     #   molflux
     #   myst-nb
     #   myst-parser
     #   pytorch-lightning
-pyzmq==25.1.2
+pyzmq==26.0.2
     # via
     #   ipykernel
     #   jupyter-client
 qlient==1.0.0
     # via molflux
 qlient-core==1.0.1
     # via qlient
-rapidfuzz==3.6.1
+rapidfuzz==3.8.1
     # via thefuzz
 rdkit==2023.9.5
     # via physicsml (pyproject.toml)
-referencing==0.33.0
+referencing==0.35.0
     # via
     #   jsonschema
     #   jsonschema-specifications
 requests==2.31.0
     # via
     #   apeye
     #   cachecontrol
     #   datasets
     #   evaluate
-    #   fsspec
     #   huggingface-hub
     #   molflux
     #   qlient
-    #   requests-oauthlib
     #   responses
     #   sphinx
-    #   tensorboard
     #   torch-geometric
     #   torchani
-requests-oauthlib==1.3.1
-    # via google-auth-oauthlib
 responses==0.18.0
     # via evaluate
 rpds-py==0.18.0
     # via
     #   jsonschema
     #   referencing
-rsa==4.9
-    # via google-auth
 ruamel-yaml==0.18.6
     # via sphinx-toolbox
 ruamel-yaml-clib==0.2.8
     # via ruamel-yaml
-s3transfer==0.10.0
+s3transfer==0.10.1
     # via boto3
-scikit-learn==1.3.2
+scikit-learn==1.4.2
     # via
     #   molflux
     #   torch-geometric
-scipy==1.10.1
+scipy==1.13.0
     # via
     #   ase
     #   e3nn
     #   molflux
     #   scikit-learn
     #   torch-geometric
 six==1.16.0
@@ -511,15 +453,15 @@
     #   asttokens
     #   html5lib
     #   python-dateutil
 snowballstemmer==2.2.0
     # via sphinx
 soupsieve==2.5
     # via beautifulsoup4
-sphinx==5.3.0
+sphinx==7.3.7
     # via
     #   autodocsumm
     #   myst-nb
     #   myst-parser
     #   physicsml (pyproject.toml)
     #   pydata-sphinx-theme
     #   sphinx-autodoc-typehints
@@ -527,88 +469,80 @@
     #   sphinx-design
     #   sphinx-inline-tabs
     #   sphinx-prompt
     #   sphinx-sitemap
     #   sphinx-tabs
     #   sphinx-togglebutton
     #   sphinx-toolbox
-sphinx-autodoc-typehints==1.23.0
+sphinx-autodoc-typehints==2.1.0
     # via sphinx-toolbox
-sphinx-book-theme==1.0.1
+sphinx-book-theme==1.1.2
     # via physicsml (pyproject.toml)
 sphinx-design==0.5.0
     # via physicsml (pyproject.toml)
 sphinx-inline-tabs==2023.4.21
     # via physicsml (pyproject.toml)
 sphinx-jinja2-compat==0.2.0.post1
     # via sphinx-toolbox
-sphinx-prompt==1.5.0
+sphinx-prompt==1.8.0
     # via sphinx-toolbox
 sphinx-sitemap==2.5.1
     # via physicsml (pyproject.toml)
 sphinx-tabs==3.4.5
     # via sphinx-toolbox
 sphinx-togglebutton==0.3.2
     # via physicsml (pyproject.toml)
 sphinx-toolbox==3.5.0
     # via physicsml (pyproject.toml)
-sphinxcontrib-applehelp==1.0.4
+sphinxcontrib-applehelp==1.0.8
     # via sphinx
-sphinxcontrib-devhelp==1.0.2
+sphinxcontrib-devhelp==1.0.6
     # via sphinx
-sphinxcontrib-htmlhelp==2.0.1
+sphinxcontrib-htmlhelp==2.0.5
     # via sphinx
 sphinxcontrib-jsmath==1.0.1
     # via sphinx
-sphinxcontrib-qthelp==1.0.3
+sphinxcontrib-qthelp==1.0.7
     # via sphinx
-sphinxcontrib-serializinghtml==1.1.5
+sphinxcontrib-serializinghtml==1.1.10
     # via sphinx
-sqlalchemy==2.0.27
+sqlalchemy==2.0.29
     # via jupyter-cache
 stack-data==0.6.3
     # via ipython
 sympy==1.12
     # via
     #   e3nn
     #   torch
 tabulate==0.9.0
     # via
     #   jupyter-cache
     #   sphinx-toolbox
 tenacity==8.2.3
     # via molflux
-tensorboard==2.14.0
-    # via physicsml (pyproject.toml)
-tensorboard-data-server==0.7.2
-    # via tensorboard
 thefuzz==0.22.1
     # via molflux
-threadpoolctl==3.3.0
+threadpoolctl==3.4.0
     # via scikit-learn
 toml==0.10.2
     # via jupytext
-tomli==2.0.1
-    # via
-    #   coverage
-    #   pytest
-torch==2.0.1
+torch==2.3.0
     # via
     #   e3nn
     #   lightning
     #   opt-einsum-fx
     #   physicsml (pyproject.toml)
     #   pytorch-lightning
     #   torchani
     #   torchmetrics
-torch-geometric==2.5.0
+torch-geometric==2.5.3
     # via physicsml (pyproject.toml)
 torchani==2.2.3
     # via physicsml (pyproject.toml)
-torchmetrics==1.3.1
+torchmetrics==1.3.2
     # via
     #   lightning
     #   pytorch-lightning
 tornado==6.4
     # via
     #   ipykernel
     #   jupyter-client
@@ -617,70 +551,61 @@
     #   datasets
     #   evaluate
     #   huggingface-hub
     #   lightning
     #   molflux
     #   pytorch-lightning
     #   torch-geometric
-traitlets==5.14.1
+traitlets==5.14.3
     # via
     #   comm
     #   ipykernel
     #   ipython
     #   ipywidgets
     #   jupyter-client
     #   jupyter-core
     #   matplotlib-inline
     #   nbclient
     #   nbformat
-typing-extensions==4.9.0
+typing-extensions==4.11.0
     # via
-    #   cloudpathlib
     #   domdf-python-tools
     #   huggingface-hub
     #   ipython
     #   lightning
     #   lightning-utilities
     #   molflux
     #   myst-nb
-    #   myst-parser
     #   pydantic
     #   pydata-sphinx-theme
     #   pytorch-lightning
     #   sphinx-toolbox
     #   sqlalchemy
     #   torch
-    #   torchmetrics
 tzdata==2024.1
     # via pandas
-urllib3==1.26.18
+urllib3==2.2.1
     # via
     #   botocore
     #   requests
     #   responses
 wcwidth==0.2.13
     # via prompt-toolkit
 webencodings==0.5.1
     # via html5lib
-websocket-client==1.7.0
+websocket-client==1.8.0
     # via qlient
-werkzeug==3.0.1
-    # via tensorboard
-wheel==0.42.0
-    # via
-    #   sphinx-togglebutton
-    #   tensorboard
+wheel==0.43.0
+    # via sphinx-togglebutton
 widgetsnbextension==4.0.10
     # via ipywidgets
 xxhash==3.4.1
     # via
     #   datasets
     #   evaluate
 yarl==1.9.4
     # via aiohttp
-zipp==3.17.0
-    # via
-    #   importlib-metadata
-    #   importlib-resources
+zipp==3.18.1
+    # via importlib-metadata
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `physicsml-0.2.3/pinned-versions/3.8/lockfile.openmm.txt` & `physicsml-0.2.4/pinned-versions/3.8/lockfile.core.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 #
 # This file is autogenerated by pip-compile with Python 3.8
 # by the following command:
 #
-#    nox -s dependencies_pin-3.8(extra='openmm')
+#    nox -s dependencies_pin-3.8(extra=None)
 #
-absl-py==2.1.0
-    # via tensorboard
 accessible-pygments==0.0.4
     # via pydata-sphinx-theme
-aiohttp==3.9.3
+aiohttp==3.9.5
     # via
     #   datasets
     #   fsspec
     #   torch-geometric
 aiosignal==1.3.1
     # via aiohttp
 alabaster==0.7.13
@@ -45,54 +43,52 @@
     #   sphinx
 backcall==0.2.0
     # via ipython
 beautifulsoup4==4.12.3
     # via
     #   pydata-sphinx-theme
     #   sphinx-toolbox
-boto3==1.34.45
+boto3==1.34.91
     # via
     #   cloudpathlib
     #   molflux
-botocore==1.34.45
+botocore==1.34.91
     # via
     #   boto3
     #   molflux
     #   s3transfer
 cachecontrol==0.14.0
     # via sphinx-toolbox
-cachetools==5.3.2
-    # via google-auth
 certifi==2024.2.2
     # via requests
 charset-normalizer==3.3.2
     # via requests
 click==8.1.7
     # via jupyter-cache
-cloudpathlib==0.17.0
+cloudpathlib==0.18.1
     # via molflux
 colorama==0.4.6
     # via molflux
-comm==0.2.1
+comm==0.2.2
     # via
     #   ipykernel
     #   ipywidgets
 contourpy==1.1.1
     # via matplotlib
-coverage==7.4.1
+coverage==7.5.0
     # via
     #   coverage-badge
     #   physicsml (pyproject.toml)
-coverage-badge==1.1.0
+coverage-badge==1.1.1
     # via physicsml (pyproject.toml)
-cssutils==2.9.0
+cssutils==2.10.2
     # via dict2css
 cycler==0.12.1
     # via matplotlib
-datasets==2.17.1
+datasets==2.19.0
     # via
     #   evaluate
     #   molflux
 debugpy==1.8.1
     # via ipykernel
 decorator==5.1.1
     # via ipython
@@ -117,85 +113,77 @@
     #   apeye-core
     #   dict2css
     #   sphinx-toolbox
 e3nn==0.5.1
     # via physicsml (pyproject.toml)
 evaluate==0.4.1
     # via molflux
-exceptiongroup==1.2.0
+exceptiongroup==1.2.1
     # via pytest
 executing==2.0.1
     # via stack-data
 fastjsonschema==2.19.1
     # via nbformat
-filelock==3.13.1
+filelock==3.13.4
     # via
     #   cachecontrol
     #   datasets
     #   huggingface-hub
     #   sphinx-toolbox
     #   torch
-fonttools==4.49.0
+fonttools==4.51.0
     # via matplotlib
 frozenlist==1.4.1
     # via
     #   aiohttp
     #   aiosignal
-fsspec==2023.10.0
+fsspec==2024.3.1
     # via
     #   datasets
     #   evaluate
     #   huggingface-hub
     #   lightning
     #   molflux
     #   pytorch-lightning
+    #   torch
     #   torch-geometric
-google-auth==2.28.0
-    # via
-    #   google-auth-oauthlib
-    #   tensorboard
-google-auth-oauthlib==1.0.0
-    # via tensorboard
-grpcio==1.60.1
-    # via tensorboard
-h5py==3.10.0
+h5py==3.11.0
     # via
     #   molflux
     #   physicsml (pyproject.toml)
 html5lib==1.1
     # via sphinx-toolbox
-huggingface-hub==0.20.3
+huggingface-hub==0.22.2
     # via
     #   datasets
     #   evaluate
-idna==3.6
+idna==3.7
     # via
     #   apeye-core
     #   requests
     #   yarl
 imagesize==1.4.1
     # via sphinx
 importlib-metadata==4.13.0
     # via
     #   domdf-python-tools
     #   jupyter-cache
     #   jupyter-client
-    #   markdown
     #   myst-nb
     #   qlient-core
     #   sphinx
     #   torchani
-importlib-resources==6.1.1
+importlib-resources==6.4.0
     # via
     #   jsonschema
     #   jsonschema-specifications
     #   matplotlib
 iniconfig==2.0.0
     # via pytest
-ipykernel==6.29.2
+ipykernel==6.29.4
     # via myst-nb
 ipython==8.12.3
     # via
     #   ipykernel
     #   ipywidgets
     #   myst-nb
 ipywidgets==8.1.2
@@ -209,66 +197,63 @@
     #   sphinx-jinja2-compat
     #   torch
     #   torch-geometric
 jmespath==1.0.1
     # via
     #   boto3
     #   botocore
-joblib==1.3.2
+joblib==1.4.0
     # via
     #   molflux
     #   scikit-learn
 jsonschema==4.21.1
     # via nbformat
 jsonschema-specifications==2023.12.1
     # via jsonschema
 jupyter-cache==0.6.1
     # via myst-nb
-jupyter-client==8.6.0
+jupyter-client==8.6.1
     # via
     #   ipykernel
     #   nbclient
-jupyter-core==5.7.1
+jupyter-core==5.7.2
     # via
     #   ipykernel
     #   jupyter-client
     #   nbclient
     #   nbformat
 jupyterlab-widgets==3.0.10
     # via ipywidgets
 jupytext==1.16.1
     # via physicsml (pyproject.toml)
 kiwisolver==1.4.5
     # via matplotlib
 lark-parser==0.12.0
     # via torchani
-lightning==2.2.0.post0
+lightning==2.2.3
     # via physicsml (pyproject.toml)
-lightning-utilities==0.10.1
+lightning-utilities==0.11.2
     # via
     #   lightning
     #   pytorch-lightning
     #   torchmetrics
-markdown==3.5.2
-    # via tensorboard
 markdown-it-py==2.2.0
     # via
     #   jupytext
     #   mdit-py-plugins
     #   myst-parser
 markupsafe==2.1.5
     # via
     #   jinja2
     #   sphinx-jinja2-compat
-    #   werkzeug
 matplotlib==3.7.5
     # via
     #   ase
     #   physicsml (pyproject.toml)
-matplotlib-inline==0.1.6
+matplotlib-inline==0.1.7
     # via
     #   ipykernel
     #   ipython
 mdit-py-plugins==0.3.5
     # via
     #   jupytext
     #   myst-parser
@@ -278,15 +263,15 @@
     # via molflux
 molflux==0.3.0
     # via physicsml (pyproject.toml)
 more-itertools==10.2.0
     # via molflux
 mpmath==1.3.0
     # via sympy
-msgpack==1.0.7
+msgpack==1.0.8
     # via cachecontrol
 multidict==6.0.5
     # via
     #   aiohttp
     #   yarl
 multiprocess==0.70.16
     # via
@@ -298,15 +283,15 @@
     # via myst-nb
 natsort==8.4.0
     # via domdf-python-tools
 nbclient==0.7.4
     # via
     #   jupyter-cache
     #   myst-nb
-nbformat==5.9.2
+nbformat==5.10.4
     # via
     #   jupyter-cache
     #   jupytext
     #   myst-nb
     #   nbclient
 nest-asyncio==1.6.0
     # via ipykernel
@@ -325,24 +310,21 @@
     #   opt-einsum
     #   pandas
     #   pyarrow
     #   pytorch-lightning
     #   rdkit
     #   scikit-learn
     #   scipy
-    #   tensorboard
     #   torch-geometric
     #   torchmetrics
-oauthlib==3.2.2
-    # via requests-oauthlib
 opt-einsum==3.3.0
     # via opt-einsum-fx
 opt-einsum-fx==0.1.4
     # via e3nn
-packaging==23.2
+packaging==24.0
     # via
     #   datasets
     #   evaluate
     #   huggingface-hub
     #   ipykernel
     #   jupytext
     #   lightning
@@ -355,82 +337,74 @@
     #   sphinx
     #   torchmetrics
 pandas==2.0.3
     # via
     #   datasets
     #   evaluate
     #   molflux
-parso==0.8.3
+parso==0.8.4
     # via jedi
 pexpect==4.9.0
     # via ipython
 pickleshare==0.7.5
     # via ipython
-pillow==10.2.0
+pillow==10.3.0
     # via
     #   matplotlib
     #   rdkit
 pkgutil-resolve-name==1.3.10
     # via jsonschema
-platformdirs==4.2.0
+platformdirs==4.2.1
     # via
     #   apeye
     #   jupyter-core
-pluggy==1.4.0
+pluggy==1.5.0
     # via pytest
 prompt-toolkit==3.0.43
     # via ipython
-protobuf==4.25.3
-    # via tensorboard
 psutil==5.9.8
     # via
     #   ipykernel
     #   torch-geometric
 ptyprocess==0.7.0
     # via pexpect
 pure-eval==0.2.2
     # via stack-data
-pyarrow==15.0.0
+pyarrow==16.0.0
     # via
     #   datasets
     #   molflux
 pyarrow-hotfix==0.6
     # via datasets
-pyasn1==0.5.1
-    # via
-    #   pyasn1-modules
-    #   rsa
-pyasn1-modules==0.3.0
-    # via google-auth
-pydantic==1.10.14
+pydantic==1.10.15
     # via molflux
 pydata-sphinx-theme==0.14.4
     # via sphinx-book-theme
 pygments==2.17.2
     # via
     #   accessible-pygments
     #   ipython
     #   pydata-sphinx-theme
     #   sphinx
     #   sphinx-prompt
     #   sphinx-tabs
-pyparsing==3.1.1
+pyparsing==3.1.2
     # via
     #   matplotlib
     #   torch-geometric
-pytest==8.0.1
+pytest==8.1.1
     # via physicsml (pyproject.toml)
-python-dateutil==2.8.2
+python-dateutil==2.9.0.post0
     # via
     #   botocore
     #   jupyter-client
     #   matplotlib
     #   molflux
     #   pandas
-pytorch-lightning==2.2.0.post0
+pytorch-lightning==2.2.3
     # via lightning
 pytz==2024.1
     # via
     #   babel
     #   pandas
 pyyaml==6.0.1
     # via
@@ -439,61 +413,54 @@
     #   jupyter-cache
     #   jupytext
     #   lightning
     #   molflux
     #   myst-nb
     #   myst-parser
     #   pytorch-lightning
-pyzmq==25.1.2
+pyzmq==26.0.2
     # via
     #   ipykernel
     #   jupyter-client
 qlient==1.0.0
     # via molflux
 qlient-core==1.0.1
     # via qlient
-rapidfuzz==3.6.1
+rapidfuzz==3.8.1
     # via thefuzz
 rdkit==2023.9.5
     # via physicsml (pyproject.toml)
-referencing==0.33.0
+referencing==0.35.0
     # via
     #   jsonschema
     #   jsonschema-specifications
 requests==2.31.0
     # via
     #   apeye
     #   cachecontrol
     #   datasets
     #   evaluate
-    #   fsspec
     #   huggingface-hub
     #   molflux
     #   qlient
-    #   requests-oauthlib
     #   responses
     #   sphinx
-    #   tensorboard
     #   torch-geometric
     #   torchani
-requests-oauthlib==1.3.1
-    # via google-auth-oauthlib
 responses==0.18.0
     # via evaluate
 rpds-py==0.18.0
     # via
     #   jsonschema
     #   referencing
-rsa==4.9
-    # via google-auth
 ruamel-yaml==0.18.6
     # via sphinx-toolbox
 ruamel-yaml-clib==0.2.8
     # via ruamel-yaml
-s3transfer==0.10.0
+s3transfer==0.10.1
     # via boto3
 scikit-learn==1.3.2
     # via
     #   molflux
     #   torch-geometric
 scipy==1.10.1
     # via
@@ -555,56 +522,52 @@
     # via sphinx
 sphinxcontrib-jsmath==1.0.1
     # via sphinx
 sphinxcontrib-qthelp==1.0.3
     # via sphinx
 sphinxcontrib-serializinghtml==1.1.5
     # via sphinx
-sqlalchemy==2.0.27
+sqlalchemy==2.0.29
     # via jupyter-cache
 stack-data==0.6.3
     # via ipython
 sympy==1.12
     # via
     #   e3nn
     #   torch
 tabulate==0.9.0
     # via
     #   jupyter-cache
     #   sphinx-toolbox
 tenacity==8.2.3
     # via molflux
-tensorboard==2.14.0
-    # via physicsml (pyproject.toml)
-tensorboard-data-server==0.7.2
-    # via tensorboard
 thefuzz==0.22.1
     # via molflux
-threadpoolctl==3.3.0
+threadpoolctl==3.4.0
     # via scikit-learn
 toml==0.10.2
     # via jupytext
 tomli==2.0.1
     # via
     #   coverage
     #   pytest
-torch==2.0.1
+torch==2.3.0
     # via
     #   e3nn
     #   lightning
     #   opt-einsum-fx
     #   physicsml (pyproject.toml)
     #   pytorch-lightning
     #   torchani
     #   torchmetrics
-torch-geometric==2.5.0
+torch-geometric==2.5.3
     # via physicsml (pyproject.toml)
 torchani==2.2.3
     # via physicsml (pyproject.toml)
-torchmetrics==1.3.1
+torchmetrics==1.3.2
     # via
     #   lightning
     #   pytorch-lightning
 tornado==6.4
     # via
     #   ipykernel
     #   jupyter-client
@@ -613,26 +576,26 @@
     #   datasets
     #   evaluate
     #   huggingface-hub
     #   lightning
     #   molflux
     #   pytorch-lightning
     #   torch-geometric
-traitlets==5.14.1
+traitlets==5.14.3
     # via
     #   comm
     #   ipykernel
     #   ipython
     #   ipywidgets
     #   jupyter-client
     #   jupyter-core
     #   matplotlib-inline
     #   nbclient
     #   nbformat
-typing-extensions==4.9.0
+typing-extensions==4.11.0
     # via
     #   cloudpathlib
     #   domdf-python-tools
     #   huggingface-hub
     #   ipython
     #   lightning
     #   lightning-utilities
@@ -653,30 +616,26 @@
     #   botocore
     #   requests
     #   responses
 wcwidth==0.2.13
     # via prompt-toolkit
 webencodings==0.5.1
     # via html5lib
-websocket-client==1.7.0
+websocket-client==1.8.0
     # via qlient
-werkzeug==3.0.1
-    # via tensorboard
-wheel==0.42.0
-    # via
-    #   sphinx-togglebutton
-    #   tensorboard
+wheel==0.43.0
+    # via sphinx-togglebutton
 widgetsnbextension==4.0.10
     # via ipywidgets
 xxhash==3.4.1
     # via
     #   datasets
     #   evaluate
 yarl==1.9.4
     # via aiohttp
-zipp==3.17.0
+zipp==3.18.1
     # via
     #   importlib-metadata
     #   importlib-resources
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `physicsml-0.2.3/pinned-versions/3.8/lockfile.rdkit.txt` & `physicsml-0.2.4/pinned-versions/3.8/lockfile.rdkit.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 #
 # This file is autogenerated by pip-compile with Python 3.8
 # by the following command:
 #
 #    nox -s dependencies_pin-3.8(extra='rdkit')
 #
-absl-py==2.1.0
-    # via tensorboard
 accessible-pygments==0.0.4
     # via pydata-sphinx-theme
-aiohttp==3.9.3
+aiohttp==3.9.5
     # via
     #   datasets
     #   fsspec
     #   torch-geometric
 aiosignal==1.3.1
     # via aiohttp
 alabaster==0.7.13
@@ -45,54 +43,52 @@
     #   sphinx
 backcall==0.2.0
     # via ipython
 beautifulsoup4==4.12.3
     # via
     #   pydata-sphinx-theme
     #   sphinx-toolbox
-boto3==1.34.45
+boto3==1.34.91
     # via
     #   cloudpathlib
     #   molflux
-botocore==1.34.45
+botocore==1.34.91
     # via
     #   boto3
     #   molflux
     #   s3transfer
 cachecontrol==0.14.0
     # via sphinx-toolbox
-cachetools==5.3.2
-    # via google-auth
 certifi==2024.2.2
     # via requests
 charset-normalizer==3.3.2
     # via requests
 click==8.1.7
     # via jupyter-cache
-cloudpathlib==0.17.0
+cloudpathlib==0.18.1
     # via molflux
 colorama==0.4.6
     # via molflux
-comm==0.2.1
+comm==0.2.2
     # via
     #   ipykernel
     #   ipywidgets
 contourpy==1.1.1
     # via matplotlib
-coverage==7.4.1
+coverage==7.5.0
     # via
     #   coverage-badge
     #   physicsml (pyproject.toml)
-coverage-badge==1.1.0
+coverage-badge==1.1.1
     # via physicsml (pyproject.toml)
-cssutils==2.9.0
+cssutils==2.10.2
     # via dict2css
 cycler==0.12.1
     # via matplotlib
-datasets==2.17.1
+datasets==2.19.0
     # via
     #   evaluate
     #   molflux
 debugpy==1.8.1
     # via ipykernel
 decorator==5.1.1
     # via ipython
@@ -117,85 +113,77 @@
     #   apeye-core
     #   dict2css
     #   sphinx-toolbox
 e3nn==0.5.1
     # via physicsml (pyproject.toml)
 evaluate==0.4.1
     # via molflux
-exceptiongroup==1.2.0
+exceptiongroup==1.2.1
     # via pytest
 executing==2.0.1
     # via stack-data
 fastjsonschema==2.19.1
     # via nbformat
-filelock==3.13.1
+filelock==3.13.4
     # via
     #   cachecontrol
     #   datasets
     #   huggingface-hub
     #   sphinx-toolbox
     #   torch
-fonttools==4.49.0
+fonttools==4.51.0
     # via matplotlib
 frozenlist==1.4.1
     # via
     #   aiohttp
     #   aiosignal
-fsspec==2023.10.0
+fsspec==2024.3.1
     # via
     #   datasets
     #   evaluate
     #   huggingface-hub
     #   lightning
     #   molflux
     #   pytorch-lightning
+    #   torch
     #   torch-geometric
-google-auth==2.28.0
-    # via
-    #   google-auth-oauthlib
-    #   tensorboard
-google-auth-oauthlib==1.0.0
-    # via tensorboard
-grpcio==1.60.1
-    # via tensorboard
-h5py==3.10.0
+h5py==3.11.0
     # via
     #   molflux
     #   physicsml (pyproject.toml)
 html5lib==1.1
     # via sphinx-toolbox
-huggingface-hub==0.20.3
+huggingface-hub==0.22.2
     # via
     #   datasets
     #   evaluate
-idna==3.6
+idna==3.7
     # via
     #   apeye-core
     #   requests
     #   yarl
 imagesize==1.4.1
     # via sphinx
 importlib-metadata==4.13.0
     # via
     #   domdf-python-tools
     #   jupyter-cache
     #   jupyter-client
-    #   markdown
     #   myst-nb
     #   qlient-core
     #   sphinx
     #   torchani
-importlib-resources==6.1.1
+importlib-resources==6.4.0
     # via
     #   jsonschema
     #   jsonschema-specifications
     #   matplotlib
 iniconfig==2.0.0
     # via pytest
-ipykernel==6.29.2
+ipykernel==6.29.4
     # via myst-nb
 ipython==8.12.3
     # via
     #   ipykernel
     #   ipywidgets
     #   myst-nb
 ipywidgets==8.1.2
@@ -209,66 +197,63 @@
     #   sphinx-jinja2-compat
     #   torch
     #   torch-geometric
 jmespath==1.0.1
     # via
     #   boto3
     #   botocore
-joblib==1.3.2
+joblib==1.4.0
     # via
     #   molflux
     #   scikit-learn
 jsonschema==4.21.1
     # via nbformat
 jsonschema-specifications==2023.12.1
     # via jsonschema
 jupyter-cache==0.6.1
     # via myst-nb
-jupyter-client==8.6.0
+jupyter-client==8.6.1
     # via
     #   ipykernel
     #   nbclient
-jupyter-core==5.7.1
+jupyter-core==5.7.2
     # via
     #   ipykernel
     #   jupyter-client
     #   nbclient
     #   nbformat
 jupyterlab-widgets==3.0.10
     # via ipywidgets
 jupytext==1.16.1
     # via physicsml (pyproject.toml)
 kiwisolver==1.4.5
     # via matplotlib
 lark-parser==0.12.0
     # via torchani
-lightning==2.2.0.post0
+lightning==2.2.3
     # via physicsml (pyproject.toml)
-lightning-utilities==0.10.1
+lightning-utilities==0.11.2
     # via
     #   lightning
     #   pytorch-lightning
     #   torchmetrics
-markdown==3.5.2
-    # via tensorboard
 markdown-it-py==2.2.0
     # via
     #   jupytext
     #   mdit-py-plugins
     #   myst-parser
 markupsafe==2.1.5
     # via
     #   jinja2
     #   sphinx-jinja2-compat
-    #   werkzeug
 matplotlib==3.7.5
     # via
     #   ase
     #   physicsml (pyproject.toml)
-matplotlib-inline==0.1.6
+matplotlib-inline==0.1.7
     # via
     #   ipykernel
     #   ipython
 mdit-py-plugins==0.3.5
     # via
     #   jupytext
     #   myst-parser
@@ -278,15 +263,15 @@
     # via molflux
 molflux==0.3.0
     # via physicsml (pyproject.toml)
 more-itertools==10.2.0
     # via molflux
 mpmath==1.3.0
     # via sympy
-msgpack==1.0.7
+msgpack==1.0.8
     # via cachecontrol
 multidict==6.0.5
     # via
     #   aiohttp
     #   yarl
 multiprocess==0.70.16
     # via
@@ -298,15 +283,15 @@
     # via myst-nb
 natsort==8.4.0
     # via domdf-python-tools
 nbclient==0.7.4
     # via
     #   jupyter-cache
     #   myst-nb
-nbformat==5.9.2
+nbformat==5.10.4
     # via
     #   jupyter-cache
     #   jupytext
     #   myst-nb
     #   nbclient
 nest-asyncio==1.6.0
     # via ipykernel
@@ -325,24 +310,21 @@
     #   opt-einsum
     #   pandas
     #   pyarrow
     #   pytorch-lightning
     #   rdkit
     #   scikit-learn
     #   scipy
-    #   tensorboard
     #   torch-geometric
     #   torchmetrics
-oauthlib==3.2.2
-    # via requests-oauthlib
 opt-einsum==3.3.0
     # via opt-einsum-fx
 opt-einsum-fx==0.1.4
     # via e3nn
-packaging==23.2
+packaging==24.0
     # via
     #   datasets
     #   evaluate
     #   huggingface-hub
     #   ipykernel
     #   jupytext
     #   lightning
@@ -355,82 +337,74 @@
     #   sphinx
     #   torchmetrics
 pandas==2.0.3
     # via
     #   datasets
     #   evaluate
     #   molflux
-parso==0.8.3
+parso==0.8.4
     # via jedi
 pexpect==4.9.0
     # via ipython
 pickleshare==0.7.5
     # via ipython
-pillow==10.2.0
+pillow==10.3.0
     # via
     #   matplotlib
     #   rdkit
 pkgutil-resolve-name==1.3.10
     # via jsonschema
-platformdirs==4.2.0
+platformdirs==4.2.1
     # via
     #   apeye
     #   jupyter-core
-pluggy==1.4.0
+pluggy==1.5.0
     # via pytest
 prompt-toolkit==3.0.43
     # via ipython
-protobuf==4.25.3
-    # via tensorboard
 psutil==5.9.8
     # via
     #   ipykernel
     #   torch-geometric
 ptyprocess==0.7.0
     # via pexpect
 pure-eval==0.2.2
     # via stack-data
-pyarrow==15.0.0
+pyarrow==16.0.0
     # via
     #   datasets
     #   molflux
 pyarrow-hotfix==0.6
     # via datasets
-pyasn1==0.5.1
-    # via
-    #   pyasn1-modules
-    #   rsa
-pyasn1-modules==0.3.0
-    # via google-auth
-pydantic==1.10.14
+pydantic==1.10.15
     # via molflux
 pydata-sphinx-theme==0.14.4
     # via sphinx-book-theme
 pygments==2.17.2
     # via
     #   accessible-pygments
     #   ipython
     #   pydata-sphinx-theme
     #   sphinx
     #   sphinx-prompt
     #   sphinx-tabs
-pyparsing==3.1.1
+pyparsing==3.1.2
     # via
     #   matplotlib
     #   torch-geometric
-pytest==8.0.1
+pytest==8.1.1
     # via physicsml (pyproject.toml)
-python-dateutil==2.8.2
+python-dateutil==2.9.0.post0
     # via
     #   botocore
     #   jupyter-client
     #   matplotlib
     #   molflux
     #   pandas
-pytorch-lightning==2.2.0.post0
+pytorch-lightning==2.2.3
     # via lightning
 pytz==2024.1
     # via
     #   babel
     #   pandas
 pyyaml==6.0.1
     # via
@@ -439,61 +413,54 @@
     #   jupyter-cache
     #   jupytext
     #   lightning
     #   molflux
     #   myst-nb
     #   myst-parser
     #   pytorch-lightning
-pyzmq==25.1.2
+pyzmq==26.0.2
     # via
     #   ipykernel
     #   jupyter-client
 qlient==1.0.0
     # via molflux
 qlient-core==1.0.1
     # via qlient
-rapidfuzz==3.6.1
+rapidfuzz==3.8.1
     # via thefuzz
 rdkit==2023.9.5
     # via physicsml (pyproject.toml)
-referencing==0.33.0
+referencing==0.35.0
     # via
     #   jsonschema
     #   jsonschema-specifications
 requests==2.31.0
     # via
     #   apeye
     #   cachecontrol
     #   datasets
     #   evaluate
-    #   fsspec
     #   huggingface-hub
     #   molflux
     #   qlient
-    #   requests-oauthlib
     #   responses
     #   sphinx
-    #   tensorboard
     #   torch-geometric
     #   torchani
-requests-oauthlib==1.3.1
-    # via google-auth-oauthlib
 responses==0.18.0
     # via evaluate
 rpds-py==0.18.0
     # via
     #   jsonschema
     #   referencing
-rsa==4.9
-    # via google-auth
 ruamel-yaml==0.18.6
     # via sphinx-toolbox
 ruamel-yaml-clib==0.2.8
     # via ruamel-yaml
-s3transfer==0.10.0
+s3transfer==0.10.1
     # via boto3
 scikit-learn==1.3.2
     # via
     #   molflux
     #   torch-geometric
 scipy==1.10.1
     # via
@@ -555,56 +522,52 @@
     # via sphinx
 sphinxcontrib-jsmath==1.0.1
     # via sphinx
 sphinxcontrib-qthelp==1.0.3
     # via sphinx
 sphinxcontrib-serializinghtml==1.1.5
     # via sphinx
-sqlalchemy==2.0.27
+sqlalchemy==2.0.29
     # via jupyter-cache
 stack-data==0.6.3
     # via ipython
 sympy==1.12
     # via
     #   e3nn
     #   torch
 tabulate==0.9.0
     # via
     #   jupyter-cache
     #   sphinx-toolbox
 tenacity==8.2.3
     # via molflux
-tensorboard==2.14.0
-    # via physicsml (pyproject.toml)
-tensorboard-data-server==0.7.2
-    # via tensorboard
 thefuzz==0.22.1
     # via molflux
-threadpoolctl==3.3.0
+threadpoolctl==3.4.0
     # via scikit-learn
 toml==0.10.2
     # via jupytext
 tomli==2.0.1
     # via
     #   coverage
     #   pytest
-torch==2.0.1
+torch==2.3.0
     # via
     #   e3nn
     #   lightning
     #   opt-einsum-fx
     #   physicsml (pyproject.toml)
     #   pytorch-lightning
     #   torchani
     #   torchmetrics
-torch-geometric==2.5.0
+torch-geometric==2.5.3
     # via physicsml (pyproject.toml)
 torchani==2.2.3
     # via physicsml (pyproject.toml)
-torchmetrics==1.3.1
+torchmetrics==1.3.2
     # via
     #   lightning
     #   pytorch-lightning
 tornado==6.4
     # via
     #   ipykernel
     #   jupyter-client
@@ -613,26 +576,26 @@
     #   datasets
     #   evaluate
     #   huggingface-hub
     #   lightning
     #   molflux
     #   pytorch-lightning
     #   torch-geometric
-traitlets==5.14.1
+traitlets==5.14.3
     # via
     #   comm
     #   ipykernel
     #   ipython
     #   ipywidgets
     #   jupyter-client
     #   jupyter-core
     #   matplotlib-inline
     #   nbclient
     #   nbformat
-typing-extensions==4.9.0
+typing-extensions==4.11.0
     # via
     #   cloudpathlib
     #   domdf-python-tools
     #   huggingface-hub
     #   ipython
     #   lightning
     #   lightning-utilities
@@ -653,30 +616,26 @@
     #   botocore
     #   requests
     #   responses
 wcwidth==0.2.13
     # via prompt-toolkit
 webencodings==0.5.1
     # via html5lib
-websocket-client==1.7.0
+websocket-client==1.8.0
     # via qlient
-werkzeug==3.0.1
-    # via tensorboard
-wheel==0.42.0
-    # via
-    #   sphinx-togglebutton
-    #   tensorboard
+wheel==0.43.0
+    # via sphinx-togglebutton
 widgetsnbextension==4.0.10
     # via ipywidgets
 xxhash==3.4.1
     # via
     #   datasets
     #   evaluate
 yarl==1.9.4
     # via aiohttp
-zipp==3.17.0
+zipp==3.18.1
     # via
     #   importlib-metadata
     #   importlib-resources
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `physicsml-0.2.3/pinned-versions/3.9/lockfile.ase.txt` & `physicsml-0.2.4/pinned-versions/3.9/lockfile.core.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 #
 # This file is autogenerated by pip-compile with Python 3.9
 # by the following command:
 #
-#    nox -s dependencies_pin-3.9(extra='ase')
+#    nox -s dependencies_pin-3.9(extra=None)
 #
-absl-py==2.1.0
-    # via tensorboard
 accessible-pygments==0.0.4
     # via pydata-sphinx-theme
-aiohttp==3.9.3
+aiohttp==3.9.5
     # via
     #   datasets
     #   fsspec
     #   torch-geometric
 aiosignal==1.3.1
     # via aiohttp
 alabaster==0.7.16
@@ -41,67 +39,67 @@
     # via
     #   pydata-sphinx-theme
     #   sphinx
 beautifulsoup4==4.12.3
     # via
     #   pydata-sphinx-theme
     #   sphinx-toolbox
-boto3==1.34.45
+boto3==1.34.91
     # via
     #   cloudpathlib
     #   molflux
-botocore==1.34.45
+botocore==1.34.91
     # via
     #   boto3
     #   molflux
     #   s3transfer
 cachecontrol==0.14.0
     # via sphinx-toolbox
 certifi==2024.2.2
     # via requests
 charset-normalizer==3.3.2
     # via requests
 click==8.1.7
     # via jupyter-cache
-cloudpathlib==0.17.0
+cloudpathlib==0.18.1
     # via molflux
 colorama==0.4.6
     # via molflux
-comm==0.2.1
+comm==0.2.2
     # via
     #   ipykernel
     #   ipywidgets
-contourpy==1.2.0
+contourpy==1.2.1
     # via matplotlib
-coverage==7.4.1
+coverage==7.5.0
     # via
     #   coverage-badge
     #   physicsml (pyproject.toml)
-coverage-badge==1.1.0
+coverage-badge==1.1.1
     # via physicsml (pyproject.toml)
-cssutils==2.9.0
+cssutils==2.10.2
     # via dict2css
 cycler==0.12.1
     # via matplotlib
-datasets==2.17.1
+datasets==2.19.0
     # via
     #   evaluate
     #   molflux
 debugpy==1.8.1
     # via ipykernel
 decorator==5.1.1
     # via ipython
 dict2css==0.3.0.post1
     # via sphinx-toolbox
 dill==0.3.8
     # via
     #   datasets
     #   evaluate
     #   multiprocess
-docutils==0.20.1
+docutils==0.21.2
     # via
     #   myst-parser
     #   pydata-sphinx-theme
     #   sphinx
     #   sphinx-prompt
     #   sphinx-tabs
     #   sphinx-togglebutton
@@ -112,77 +110,75 @@
     #   apeye-core
     #   dict2css
     #   sphinx-toolbox
 e3nn==0.5.1
     # via physicsml (pyproject.toml)
 evaluate==0.4.1
     # via molflux
-exceptiongroup==1.2.0
+exceptiongroup==1.2.1
     # via
     #   ipython
     #   pytest
 executing==2.0.1
     # via stack-data
 fastjsonschema==2.19.1
     # via nbformat
-filelock==3.13.1
+filelock==3.13.4
     # via
     #   cachecontrol
     #   datasets
     #   huggingface-hub
     #   sphinx-toolbox
     #   torch
-fonttools==4.49.0
+fonttools==4.51.0
     # via matplotlib
 frozenlist==1.4.1
     # via
     #   aiohttp
     #   aiosignal
-fsspec==2023.10.0
+fsspec==2024.3.1
     # via
     #   datasets
     #   evaluate
     #   huggingface-hub
     #   lightning
     #   molflux
     #   pytorch-lightning
+    #   torch
     #   torch-geometric
-grpcio==1.60.1
-    # via tensorboard
-h5py==3.10.0
+h5py==3.11.0
     # via
     #   molflux
     #   physicsml (pyproject.toml)
 html5lib==1.1
     # via sphinx-toolbox
-huggingface-hub==0.20.3
+huggingface-hub==0.22.2
     # via
     #   datasets
     #   evaluate
-idna==3.6
+idna==3.7
     # via
     #   apeye-core
     #   requests
     #   yarl
 imagesize==1.4.1
     # via sphinx
 importlib-metadata==4.13.0
     # via
     #   jupyter-cache
     #   jupyter-client
-    #   markdown
     #   myst-nb
     #   qlient-core
     #   sphinx
     #   torchani
-importlib-resources==6.1.1
+importlib-resources==6.4.0
     # via matplotlib
 iniconfig==2.0.0
     # via pytest
-ipykernel==6.29.2
+ipykernel==6.29.4
     # via myst-nb
 ipython==8.18.1
     # via
     #   ipykernel
     #   ipywidgets
     #   myst-nb
 ipywidgets==8.1.2
@@ -196,66 +192,63 @@
     #   sphinx-jinja2-compat
     #   torch
     #   torch-geometric
 jmespath==1.0.1
     # via
     #   boto3
     #   botocore
-joblib==1.3.2
+joblib==1.4.0
     # via
     #   molflux
     #   scikit-learn
 jsonschema==4.21.1
     # via nbformat
 jsonschema-specifications==2023.12.1
     # via jsonschema
 jupyter-cache==1.0.0
     # via myst-nb
-jupyter-client==8.6.0
+jupyter-client==8.6.1
     # via
     #   ipykernel
     #   nbclient
-jupyter-core==5.7.1
+jupyter-core==5.7.2
     # via
     #   ipykernel
     #   jupyter-client
     #   nbclient
     #   nbformat
 jupyterlab-widgets==3.0.10
     # via ipywidgets
 jupytext==1.16.1
     # via physicsml (pyproject.toml)
 kiwisolver==1.4.5
     # via matplotlib
 lark-parser==0.12.0
     # via torchani
-lightning==2.2.0.post0
+lightning==2.2.3
     # via physicsml (pyproject.toml)
-lightning-utilities==0.10.1
+lightning-utilities==0.11.2
     # via
     #   lightning
     #   pytorch-lightning
     #   torchmetrics
-markdown==3.5.2
-    # via tensorboard
 markdown-it-py==3.0.0
     # via
     #   jupytext
     #   mdit-py-plugins
     #   myst-parser
 markupsafe==2.1.5
     # via
     #   jinja2
     #   sphinx-jinja2-compat
-    #   werkzeug
-matplotlib==3.8.3
+matplotlib==3.8.4
     # via
     #   ase
     #   physicsml (pyproject.toml)
-matplotlib-inline==0.1.6
+matplotlib-inline==0.1.7
     # via
     #   ipykernel
     #   ipython
 mdit-py-plugins==0.4.0
     # via
     #   jupytext
     #   myst-parser
@@ -265,35 +258,35 @@
     # via molflux
 molflux==0.3.0
     # via physicsml (pyproject.toml)
 more-itertools==10.2.0
     # via molflux
 mpmath==1.3.0
     # via sympy
-msgpack==1.0.7
+msgpack==1.0.8
     # via cachecontrol
 multidict==6.0.5
     # via
     #   aiohttp
     #   yarl
 multiprocess==0.70.16
     # via
     #   datasets
     #   evaluate
-myst-nb==1.0.0
+myst-nb==1.1.0
     # via physicsml (pyproject.toml)
-myst-parser==2.0.0
+myst-parser==3.0.0
     # via myst-nb
 natsort==8.4.0
     # via domdf-python-tools
-nbclient==0.9.0
+nbclient==0.10.0
     # via
     #   jupyter-cache
     #   myst-nb
-nbformat==5.9.2
+nbformat==5.10.4
     # via
     #   jupyter-cache
     #   jupytext
     #   myst-nb
     #   nbclient
 nest-asyncio==1.6.0
     # via ipykernel
@@ -312,22 +305,21 @@
     #   opt-einsum
     #   pandas
     #   pyarrow
     #   pytorch-lightning
     #   rdkit
     #   scikit-learn
     #   scipy
-    #   tensorboard
     #   torch-geometric
     #   torchmetrics
 opt-einsum==3.3.0
     # via opt-einsum-fx
 opt-einsum-fx==0.1.4
     # via e3nn
-packaging==23.2
+packaging==24.0
     # via
     #   datasets
     #   evaluate
     #   huggingface-hub
     #   ipykernel
     #   jupytext
     #   lightning
@@ -335,114 +327,111 @@
     #   matplotlib
     #   opt-einsum-fx
     #   pydata-sphinx-theme
     #   pytest
     #   pytorch-lightning
     #   sphinx
     #   torchmetrics
-pandas==2.2.0
+pandas==2.2.2
     # via
     #   datasets
     #   evaluate
     #   molflux
-parso==0.8.3
+parso==0.8.4
     # via jedi
 pexpect==4.9.0
     # via ipython
-pillow==10.2.0
+pillow==10.3.0
     # via
     #   matplotlib
     #   rdkit
-platformdirs==4.2.0
+platformdirs==4.2.1
     # via
     #   apeye
     #   jupyter-core
-pluggy==1.4.0
+pluggy==1.5.0
     # via pytest
 prompt-toolkit==3.0.43
     # via ipython
-protobuf==4.25.3
-    # via tensorboard
 psutil==5.9.8
     # via
     #   ipykernel
     #   torch-geometric
 ptyprocess==0.7.0
     # via pexpect
 pure-eval==0.2.2
     # via stack-data
-pyarrow==15.0.0
+pyarrow==16.0.0
     # via
     #   datasets
     #   molflux
 pyarrow-hotfix==0.6
     # via datasets
-pydantic==1.10.14
+pydantic==1.10.15
     # via molflux
 pydata-sphinx-theme==0.15.2
     # via sphinx-book-theme
 pygments==2.17.2
     # via
     #   accessible-pygments
     #   ipython
     #   pydata-sphinx-theme
     #   sphinx
     #   sphinx-prompt
     #   sphinx-tabs
-pyparsing==3.1.1
+pyparsing==3.1.2
     # via
     #   matplotlib
     #   torch-geometric
-pytest==8.0.1
+pytest==8.1.1
     # via physicsml (pyproject.toml)
-python-dateutil==2.8.2
+python-dateutil==2.9.0.post0
     # via
     #   botocore
     #   jupyter-client
     #   matplotlib
     #   molflux
     #   pandas
-pytorch-lightning==2.2.0.post0
+pytorch-lightning==2.2.3
     # via lightning
 pytz==2024.1
     # via pandas
 pyyaml==6.0.1
     # via
     #   datasets
     #   huggingface-hub
     #   jupyter-cache
     #   jupytext
     #   lightning
     #   molflux
     #   myst-nb
     #   myst-parser
     #   pytorch-lightning
-pyzmq==25.1.2
+pyzmq==26.0.2
     # via
     #   ipykernel
     #   jupyter-client
 qlient==1.0.0
     # via molflux
 qlient-core==1.0.1
     # via qlient
-rapidfuzz==3.6.1
+rapidfuzz==3.8.1
     # via thefuzz
 rdkit==2023.9.5
     # via physicsml (pyproject.toml)
-referencing==0.33.0
+referencing==0.35.0
     # via
     #   jsonschema
     #   jsonschema-specifications
 requests==2.31.0
     # via
     #   apeye
     #   cachecontrol
     #   datasets
     #   evaluate
-    #   fsspec
     #   huggingface-hub
     #   molflux
     #   qlient
     #   responses
     #   sphinx
     #   torch-geometric
     #   torchani
@@ -452,38 +441,37 @@
     # via
     #   jsonschema
     #   referencing
 ruamel-yaml==0.18.6
     # via sphinx-toolbox
 ruamel-yaml-clib==0.2.8
     # via ruamel-yaml
-s3transfer==0.10.0
+s3transfer==0.10.1
     # via boto3
-scikit-learn==1.4.1.post1
+scikit-learn==1.4.2
     # via
     #   molflux
     #   torch-geometric
-scipy==1.12.0
+scipy==1.13.0
     # via
     #   ase
     #   e3nn
     #   molflux
     #   scikit-learn
     #   torch-geometric
 six==1.16.0
     # via
     #   asttokens
     #   html5lib
     #   python-dateutil
-    #   tensorboard
 snowballstemmer==2.2.0
     # via sphinx
 soupsieve==2.5
     # via beautifulsoup4
-sphinx==7.2.6
+sphinx==7.3.7
     # via
     #   autodocsumm
     #   myst-nb
     #   myst-parser
     #   physicsml (pyproject.toml)
     #   pydata-sphinx-theme
     #   sphinx-autodoc-typehints
@@ -491,15 +479,15 @@
     #   sphinx-design
     #   sphinx-inline-tabs
     #   sphinx-prompt
     #   sphinx-sitemap
     #   sphinx-tabs
     #   sphinx-togglebutton
     #   sphinx-toolbox
-sphinx-autodoc-typehints==2.0.0
+sphinx-autodoc-typehints==2.1.0
     # via sphinx-toolbox
 sphinx-book-theme==1.1.2
     # via physicsml (pyproject.toml)
 sphinx-design==0.5.0
     # via physicsml (pyproject.toml)
 sphinx-inline-tabs==2023.4.21
     # via physicsml (pyproject.toml)
@@ -523,56 +511,53 @@
     # via sphinx
 sphinxcontrib-jsmath==1.0.1
     # via sphinx
 sphinxcontrib-qthelp==1.0.7
     # via sphinx
 sphinxcontrib-serializinghtml==1.1.10
     # via sphinx
-sqlalchemy==2.0.27
+sqlalchemy==2.0.29
     # via jupyter-cache
 stack-data==0.6.3
     # via ipython
 sympy==1.12
     # via
     #   e3nn
     #   torch
 tabulate==0.9.0
     # via
     #   jupyter-cache
     #   sphinx-toolbox
 tenacity==8.2.3
     # via molflux
-tensorboard==2.16.2
-    # via physicsml (pyproject.toml)
-tensorboard-data-server==0.7.2
-    # via tensorboard
 thefuzz==0.22.1
     # via molflux
-threadpoolctl==3.3.0
+threadpoolctl==3.4.0
     # via scikit-learn
 toml==0.10.2
     # via jupytext
 tomli==2.0.1
     # via
     #   coverage
     #   pytest
-torch==2.0.1
+    #   sphinx
+torch==2.3.0
     # via
     #   e3nn
     #   lightning
     #   opt-einsum-fx
     #   physicsml (pyproject.toml)
     #   pytorch-lightning
     #   torchani
     #   torchmetrics
-torch-geometric==2.5.0
+torch-geometric==2.5.3
     # via physicsml (pyproject.toml)
 torchani==2.2.3
     # via physicsml (pyproject.toml)
-torchmetrics==1.3.1
+torchmetrics==1.3.2
     # via
     #   lightning
     #   pytorch-lightning
 tornado==6.4
     # via
     #   ipykernel
     #   jupyter-client
@@ -581,26 +566,26 @@
     #   datasets
     #   evaluate
     #   huggingface-hub
     #   lightning
     #   molflux
     #   pytorch-lightning
     #   torch-geometric
-traitlets==5.14.1
+traitlets==5.14.3
     # via
     #   comm
     #   ipykernel
     #   ipython
     #   ipywidgets
     #   jupyter-client
     #   jupyter-core
     #   matplotlib-inline
     #   nbclient
     #   nbformat
-typing-extensions==4.9.0
+typing-extensions==4.11.0
     # via
     #   cloudpathlib
     #   domdf-python-tools
     #   huggingface-hub
     #   ipython
     #   lightning
     #   lightning-utilities
@@ -619,28 +604,26 @@
     #   botocore
     #   requests
     #   responses
 wcwidth==0.2.13
     # via prompt-toolkit
 webencodings==0.5.1
     # via html5lib
-websocket-client==1.7.0
+websocket-client==1.8.0
     # via qlient
-werkzeug==3.0.1
-    # via tensorboard
-wheel==0.42.0
+wheel==0.43.0
     # via sphinx-togglebutton
 widgetsnbextension==4.0.10
     # via ipywidgets
 xxhash==3.4.1
     # via
     #   datasets
     #   evaluate
 yarl==1.9.4
     # via aiohttp
-zipp==3.17.0
+zipp==3.18.1
     # via
     #   importlib-metadata
     #   importlib-resources
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `physicsml-0.2.3/pinned-versions/3.9/lockfile.core.txt` & `physicsml-0.2.4/pinned-versions/3.9/lockfile.openmm.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 #
 # This file is autogenerated by pip-compile with Python 3.9
 # by the following command:
 #
-#    nox -s dependencies_pin-3.9(extra=None)
+#    nox -s dependencies_pin-3.9(extra='openmm')
 #
-absl-py==2.1.0
-    # via tensorboard
 accessible-pygments==0.0.4
     # via pydata-sphinx-theme
-aiohttp==3.9.3
+aiohttp==3.9.5
     # via
     #   datasets
     #   fsspec
     #   torch-geometric
 aiosignal==1.3.1
     # via aiohttp
 alabaster==0.7.16
@@ -41,67 +39,67 @@
     # via
     #   pydata-sphinx-theme
     #   sphinx
 beautifulsoup4==4.12.3
     # via
     #   pydata-sphinx-theme
     #   sphinx-toolbox
-boto3==1.34.45
+boto3==1.34.91
     # via
     #   cloudpathlib
     #   molflux
-botocore==1.34.45
+botocore==1.34.91
     # via
     #   boto3
     #   molflux
     #   s3transfer
 cachecontrol==0.14.0
     # via sphinx-toolbox
 certifi==2024.2.2
     # via requests
 charset-normalizer==3.3.2
     # via requests
 click==8.1.7
     # via jupyter-cache
-cloudpathlib==0.17.0
+cloudpathlib==0.18.1
     # via molflux
 colorama==0.4.6
     # via molflux
-comm==0.2.1
+comm==0.2.2
     # via
     #   ipykernel
     #   ipywidgets
-contourpy==1.2.0
+contourpy==1.2.1
     # via matplotlib
-coverage==7.4.1
+coverage==7.5.0
     # via
     #   coverage-badge
     #   physicsml (pyproject.toml)
-coverage-badge==1.1.0
+coverage-badge==1.1.1
     # via physicsml (pyproject.toml)
-cssutils==2.9.0
+cssutils==2.10.2
     # via dict2css
 cycler==0.12.1
     # via matplotlib
-datasets==2.17.1
+datasets==2.19.0
     # via
     #   evaluate
     #   molflux
 debugpy==1.8.1
     # via ipykernel
 decorator==5.1.1
     # via ipython
 dict2css==0.3.0.post1
     # via sphinx-toolbox
 dill==0.3.8
     # via
     #   datasets
     #   evaluate
     #   multiprocess
-docutils==0.20.1
+docutils==0.21.2
     # via
     #   myst-parser
     #   pydata-sphinx-theme
     #   sphinx
     #   sphinx-prompt
     #   sphinx-tabs
     #   sphinx-togglebutton
@@ -112,77 +110,75 @@
     #   apeye-core
     #   dict2css
     #   sphinx-toolbox
 e3nn==0.5.1
     # via physicsml (pyproject.toml)
 evaluate==0.4.1
     # via molflux
-exceptiongroup==1.2.0
+exceptiongroup==1.2.1
     # via
     #   ipython
     #   pytest
 executing==2.0.1
     # via stack-data
 fastjsonschema==2.19.1
     # via nbformat
-filelock==3.13.1
+filelock==3.13.4
     # via
     #   cachecontrol
     #   datasets
     #   huggingface-hub
     #   sphinx-toolbox
     #   torch
-fonttools==4.49.0
+fonttools==4.51.0
     # via matplotlib
 frozenlist==1.4.1
     # via
     #   aiohttp
     #   aiosignal
-fsspec==2023.10.0
+fsspec==2024.3.1
     # via
     #   datasets
     #   evaluate
     #   huggingface-hub
     #   lightning
     #   molflux
     #   pytorch-lightning
+    #   torch
     #   torch-geometric
-grpcio==1.60.1
-    # via tensorboard
-h5py==3.10.0
+h5py==3.11.0
     # via
     #   molflux
     #   physicsml (pyproject.toml)
 html5lib==1.1
     # via sphinx-toolbox
-huggingface-hub==0.20.3
+huggingface-hub==0.22.2
     # via
     #   datasets
     #   evaluate
-idna==3.6
+idna==3.7
     # via
     #   apeye-core
     #   requests
     #   yarl
 imagesize==1.4.1
     # via sphinx
 importlib-metadata==4.13.0
     # via
     #   jupyter-cache
     #   jupyter-client
-    #   markdown
     #   myst-nb
     #   qlient-core
     #   sphinx
     #   torchani
-importlib-resources==6.1.1
+importlib-resources==6.4.0
     # via matplotlib
 iniconfig==2.0.0
     # via pytest
-ipykernel==6.29.2
+ipykernel==6.29.4
     # via myst-nb
 ipython==8.18.1
     # via
     #   ipykernel
     #   ipywidgets
     #   myst-nb
 ipywidgets==8.1.2
@@ -196,66 +192,63 @@
     #   sphinx-jinja2-compat
     #   torch
     #   torch-geometric
 jmespath==1.0.1
     # via
     #   boto3
     #   botocore
-joblib==1.3.2
+joblib==1.4.0
     # via
     #   molflux
     #   scikit-learn
 jsonschema==4.21.1
     # via nbformat
 jsonschema-specifications==2023.12.1
     # via jsonschema
 jupyter-cache==1.0.0
     # via myst-nb
-jupyter-client==8.6.0
+jupyter-client==8.6.1
     # via
     #   ipykernel
     #   nbclient
-jupyter-core==5.7.1
+jupyter-core==5.7.2
     # via
     #   ipykernel
     #   jupyter-client
     #   nbclient
     #   nbformat
 jupyterlab-widgets==3.0.10
     # via ipywidgets
 jupytext==1.16.1
     # via physicsml (pyproject.toml)
 kiwisolver==1.4.5
     # via matplotlib
 lark-parser==0.12.0
     # via torchani
-lightning==2.2.0.post0
+lightning==2.2.3
     # via physicsml (pyproject.toml)
-lightning-utilities==0.10.1
+lightning-utilities==0.11.2
     # via
     #   lightning
     #   pytorch-lightning
     #   torchmetrics
-markdown==3.5.2
-    # via tensorboard
 markdown-it-py==3.0.0
     # via
     #   jupytext
     #   mdit-py-plugins
     #   myst-parser
 markupsafe==2.1.5
     # via
     #   jinja2
     #   sphinx-jinja2-compat
-    #   werkzeug
-matplotlib==3.8.3
+matplotlib==3.8.4
     # via
     #   ase
     #   physicsml (pyproject.toml)
-matplotlib-inline==0.1.6
+matplotlib-inline==0.1.7
     # via
     #   ipykernel
     #   ipython
 mdit-py-plugins==0.4.0
     # via
     #   jupytext
     #   myst-parser
@@ -265,35 +258,35 @@
     # via molflux
 molflux==0.3.0
     # via physicsml (pyproject.toml)
 more-itertools==10.2.0
     # via molflux
 mpmath==1.3.0
     # via sympy
-msgpack==1.0.7
+msgpack==1.0.8
     # via cachecontrol
 multidict==6.0.5
     # via
     #   aiohttp
     #   yarl
 multiprocess==0.70.16
     # via
     #   datasets
     #   evaluate
-myst-nb==1.0.0
+myst-nb==1.1.0
     # via physicsml (pyproject.toml)
-myst-parser==2.0.0
+myst-parser==3.0.0
     # via myst-nb
 natsort==8.4.0
     # via domdf-python-tools
-nbclient==0.9.0
+nbclient==0.10.0
     # via
     #   jupyter-cache
     #   myst-nb
-nbformat==5.9.2
+nbformat==5.10.4
     # via
     #   jupyter-cache
     #   jupytext
     #   myst-nb
     #   nbclient
 nest-asyncio==1.6.0
     # via ipykernel
@@ -312,22 +305,21 @@
     #   opt-einsum
     #   pandas
     #   pyarrow
     #   pytorch-lightning
     #   rdkit
     #   scikit-learn
     #   scipy
-    #   tensorboard
     #   torch-geometric
     #   torchmetrics
 opt-einsum==3.3.0
     # via opt-einsum-fx
 opt-einsum-fx==0.1.4
     # via e3nn
-packaging==23.2
+packaging==24.0
     # via
     #   datasets
     #   evaluate
     #   huggingface-hub
     #   ipykernel
     #   jupytext
     #   lightning
@@ -335,114 +327,111 @@
     #   matplotlib
     #   opt-einsum-fx
     #   pydata-sphinx-theme
     #   pytest
     #   pytorch-lightning
     #   sphinx
     #   torchmetrics
-pandas==2.2.0
+pandas==2.2.2
     # via
     #   datasets
     #   evaluate
     #   molflux
-parso==0.8.3
+parso==0.8.4
     # via jedi
 pexpect==4.9.0
     # via ipython
-pillow==10.2.0
+pillow==10.3.0
     # via
     #   matplotlib
     #   rdkit
-platformdirs==4.2.0
+platformdirs==4.2.1
     # via
     #   apeye
     #   jupyter-core
-pluggy==1.4.0
+pluggy==1.5.0
     # via pytest
 prompt-toolkit==3.0.43
     # via ipython
-protobuf==4.25.3
-    # via tensorboard
 psutil==5.9.8
     # via
     #   ipykernel
     #   torch-geometric
 ptyprocess==0.7.0
     # via pexpect
 pure-eval==0.2.2
     # via stack-data
-pyarrow==15.0.0
+pyarrow==16.0.0
     # via
     #   datasets
     #   molflux
 pyarrow-hotfix==0.6
     # via datasets
-pydantic==1.10.14
+pydantic==1.10.15
     # via molflux
 pydata-sphinx-theme==0.15.2
     # via sphinx-book-theme
 pygments==2.17.2
     # via
     #   accessible-pygments
     #   ipython
     #   pydata-sphinx-theme
     #   sphinx
     #   sphinx-prompt
     #   sphinx-tabs
-pyparsing==3.1.1
+pyparsing==3.1.2
     # via
     #   matplotlib
     #   torch-geometric
-pytest==8.0.1
+pytest==8.1.1
     # via physicsml (pyproject.toml)
-python-dateutil==2.8.2
+python-dateutil==2.9.0.post0
     # via
     #   botocore
     #   jupyter-client
     #   matplotlib
     #   molflux
     #   pandas
-pytorch-lightning==2.2.0.post0
+pytorch-lightning==2.2.3
     # via lightning
 pytz==2024.1
     # via pandas
 pyyaml==6.0.1
     # via
     #   datasets
     #   huggingface-hub
     #   jupyter-cache
     #   jupytext
     #   lightning
     #   molflux
     #   myst-nb
     #   myst-parser
     #   pytorch-lightning
-pyzmq==25.1.2
+pyzmq==26.0.2
     # via
     #   ipykernel
     #   jupyter-client
 qlient==1.0.0
     # via molflux
 qlient-core==1.0.1
     # via qlient
-rapidfuzz==3.6.1
+rapidfuzz==3.8.1
     # via thefuzz
 rdkit==2023.9.5
     # via physicsml (pyproject.toml)
-referencing==0.33.0
+referencing==0.35.0
     # via
     #   jsonschema
     #   jsonschema-specifications
 requests==2.31.0
     # via
     #   apeye
     #   cachecontrol
     #   datasets
     #   evaluate
-    #   fsspec
     #   huggingface-hub
     #   molflux
     #   qlient
     #   responses
     #   sphinx
     #   torch-geometric
     #   torchani
@@ -452,38 +441,37 @@
     # via
     #   jsonschema
     #   referencing
 ruamel-yaml==0.18.6
     # via sphinx-toolbox
 ruamel-yaml-clib==0.2.8
     # via ruamel-yaml
-s3transfer==0.10.0
+s3transfer==0.10.1
     # via boto3
-scikit-learn==1.4.1.post1
+scikit-learn==1.4.2
     # via
     #   molflux
     #   torch-geometric
-scipy==1.12.0
+scipy==1.13.0
     # via
     #   ase
     #   e3nn
     #   molflux
     #   scikit-learn
     #   torch-geometric
 six==1.16.0
     # via
     #   asttokens
     #   html5lib
     #   python-dateutil
-    #   tensorboard
 snowballstemmer==2.2.0
     # via sphinx
 soupsieve==2.5
     # via beautifulsoup4
-sphinx==7.2.6
+sphinx==7.3.7
     # via
     #   autodocsumm
     #   myst-nb
     #   myst-parser
     #   physicsml (pyproject.toml)
     #   pydata-sphinx-theme
     #   sphinx-autodoc-typehints
@@ -491,15 +479,15 @@
     #   sphinx-design
     #   sphinx-inline-tabs
     #   sphinx-prompt
     #   sphinx-sitemap
     #   sphinx-tabs
     #   sphinx-togglebutton
     #   sphinx-toolbox
-sphinx-autodoc-typehints==2.0.0
+sphinx-autodoc-typehints==2.1.0
     # via sphinx-toolbox
 sphinx-book-theme==1.1.2
     # via physicsml (pyproject.toml)
 sphinx-design==0.5.0
     # via physicsml (pyproject.toml)
 sphinx-inline-tabs==2023.4.21
     # via physicsml (pyproject.toml)
@@ -523,56 +511,53 @@
     # via sphinx
 sphinxcontrib-jsmath==1.0.1
     # via sphinx
 sphinxcontrib-qthelp==1.0.7
     # via sphinx
 sphinxcontrib-serializinghtml==1.1.10
     # via sphinx
-sqlalchemy==2.0.27
+sqlalchemy==2.0.29
     # via jupyter-cache
 stack-data==0.6.3
     # via ipython
 sympy==1.12
     # via
     #   e3nn
     #   torch
 tabulate==0.9.0
     # via
     #   jupyter-cache
     #   sphinx-toolbox
 tenacity==8.2.3
     # via molflux
-tensorboard==2.16.2
-    # via physicsml (pyproject.toml)
-tensorboard-data-server==0.7.2
-    # via tensorboard
 thefuzz==0.22.1
     # via molflux
-threadpoolctl==3.3.0
+threadpoolctl==3.4.0
     # via scikit-learn
 toml==0.10.2
     # via jupytext
 tomli==2.0.1
     # via
     #   coverage
     #   pytest
-torch==2.0.1
+    #   sphinx
+torch==2.3.0
     # via
     #   e3nn
     #   lightning
     #   opt-einsum-fx
     #   physicsml (pyproject.toml)
     #   pytorch-lightning
     #   torchani
     #   torchmetrics
-torch-geometric==2.5.0
+torch-geometric==2.5.3
     # via physicsml (pyproject.toml)
 torchani==2.2.3
     # via physicsml (pyproject.toml)
-torchmetrics==1.3.1
+torchmetrics==1.3.2
     # via
     #   lightning
     #   pytorch-lightning
 tornado==6.4
     # via
     #   ipykernel
     #   jupyter-client
@@ -581,26 +566,26 @@
     #   datasets
     #   evaluate
     #   huggingface-hub
     #   lightning
     #   molflux
     #   pytorch-lightning
     #   torch-geometric
-traitlets==5.14.1
+traitlets==5.14.3
     # via
     #   comm
     #   ipykernel
     #   ipython
     #   ipywidgets
     #   jupyter-client
     #   jupyter-core
     #   matplotlib-inline
     #   nbclient
     #   nbformat
-typing-extensions==4.9.0
+typing-extensions==4.11.0
     # via
     #   cloudpathlib
     #   domdf-python-tools
     #   huggingface-hub
     #   ipython
     #   lightning
     #   lightning-utilities
@@ -619,28 +604,26 @@
     #   botocore
     #   requests
     #   responses
 wcwidth==0.2.13
     # via prompt-toolkit
 webencodings==0.5.1
     # via html5lib
-websocket-client==1.7.0
+websocket-client==1.8.0
     # via qlient
-werkzeug==3.0.1
-    # via tensorboard
-wheel==0.42.0
+wheel==0.43.0
     # via sphinx-togglebutton
 widgetsnbextension==4.0.10
     # via ipywidgets
 xxhash==3.4.1
     # via
     #   datasets
     #   evaluate
 yarl==1.9.4
     # via aiohttp
-zipp==3.17.0
+zipp==3.18.1
     # via
     #   importlib-metadata
     #   importlib-resources
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `physicsml-0.2.3/pinned-versions/3.9/lockfile.openeye.txt` & `physicsml-0.2.4/pinned-versions/3.11/lockfile.openeye.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 #
-# This file is autogenerated by pip-compile with Python 3.9
+# This file is autogenerated by pip-compile with Python 3.11
 # by the following command:
 #
-#    nox -s dependencies_pin-3.9(extra='openeye')
+#    nox -s dependencies_pin-3.11(extra='openeye')
 #
-absl-py==2.1.0
-    # via tensorboard
 accessible-pygments==0.0.4
     # via pydata-sphinx-theme
-aiohttp==3.9.3
+aiohttp==3.9.5
     # via
     #   datasets
     #   fsspec
     #   torch-geometric
 aiosignal==1.3.1
     # via aiohttp
 alabaster==0.7.16
@@ -23,16 +21,14 @@
     # via apeye
 appnope==0.1.4
     # via ipykernel
 ase==3.22.1
     # via physicsml (pyproject.toml)
 asttokens==2.4.1
     # via stack-data
-async-timeout==4.0.3
-    # via aiohttp
 attrs==23.2.0
     # via
     #   aiohttp
     #   jsonschema
     #   jupyter-cache
     #   referencing
 autodocsumm==0.2.12
@@ -41,67 +37,67 @@
     # via
     #   pydata-sphinx-theme
     #   sphinx
 beautifulsoup4==4.12.3
     # via
     #   pydata-sphinx-theme
     #   sphinx-toolbox
-boto3==1.34.45
+boto3==1.34.91
     # via
     #   cloudpathlib
     #   molflux
-botocore==1.34.45
+botocore==1.34.91
     # via
     #   boto3
     #   molflux
     #   s3transfer
 cachecontrol==0.14.0
     # via sphinx-toolbox
 certifi==2024.2.2
     # via requests
 charset-normalizer==3.3.2
     # via requests
 click==8.1.7
     # via jupyter-cache
-cloudpathlib==0.17.0
+cloudpathlib==0.18.1
     # via molflux
 colorama==0.4.6
     # via molflux
-comm==0.2.1
+comm==0.2.2
     # via
     #   ipykernel
     #   ipywidgets
-contourpy==1.2.0
+contourpy==1.2.1
     # via matplotlib
-coverage==7.4.1
+coverage==7.5.0
     # via
     #   coverage-badge
     #   physicsml (pyproject.toml)
-coverage-badge==1.1.0
+coverage-badge==1.1.1
     # via physicsml (pyproject.toml)
-cssutils==2.9.0
+cssutils==2.10.2
     # via dict2css
 cycler==0.12.1
     # via matplotlib
-datasets==2.17.1
+datasets==2.19.0
     # via
     #   evaluate
     #   molflux
 debugpy==1.8.1
     # via ipykernel
 decorator==5.1.1
     # via ipython
 dict2css==0.3.0.post1
     # via sphinx-toolbox
 dill==0.3.8
     # via
     #   datasets
     #   evaluate
     #   multiprocess
-docutils==0.20.1
+docutils==0.21.2
     # via
     #   myst-parser
     #   pydata-sphinx-theme
     #   sphinx
     #   sphinx-prompt
     #   sphinx-tabs
     #   sphinx-togglebutton
@@ -112,79 +108,69 @@
     #   apeye-core
     #   dict2css
     #   sphinx-toolbox
 e3nn==0.5.1
     # via physicsml (pyproject.toml)
 evaluate==0.4.1
     # via molflux
-exceptiongroup==1.2.0
-    # via
-    #   ipython
-    #   pytest
 executing==2.0.1
     # via stack-data
 fastjsonschema==2.19.1
     # via nbformat
-filelock==3.13.1
+filelock==3.13.4
     # via
     #   cachecontrol
     #   datasets
     #   huggingface-hub
     #   sphinx-toolbox
     #   torch
-fonttools==4.49.0
+fonttools==4.51.0
     # via matplotlib
 frozenlist==1.4.1
     # via
     #   aiohttp
     #   aiosignal
-fsspec==2023.10.0
+fsspec==2024.3.1
     # via
     #   datasets
     #   evaluate
     #   huggingface-hub
     #   lightning
     #   molflux
     #   pytorch-lightning
+    #   torch
     #   torch-geometric
-grpcio==1.60.1
-    # via tensorboard
-h5py==3.10.0
+h5py==3.11.0
     # via
     #   molflux
     #   physicsml (pyproject.toml)
 html5lib==1.1
     # via sphinx-toolbox
-huggingface-hub==0.20.3
+huggingface-hub==0.22.2
     # via
     #   datasets
     #   evaluate
-idna==3.6
+idna==3.7
     # via
     #   apeye-core
     #   requests
     #   yarl
 imagesize==1.4.1
     # via sphinx
 importlib-metadata==4.13.0
     # via
     #   jupyter-cache
-    #   jupyter-client
-    #   markdown
     #   myst-nb
     #   qlient-core
-    #   sphinx
     #   torchani
-importlib-resources==6.1.1
-    # via matplotlib
 iniconfig==2.0.0
     # via pytest
-ipykernel==6.29.2
+ipykernel==6.29.4
     # via myst-nb
-ipython==8.18.1
+ipython==8.23.0
     # via
     #   ipykernel
     #   ipywidgets
     #   myst-nb
 ipywidgets==8.1.2
     # via physicsml (pyproject.toml)
 jedi==0.19.1
@@ -196,66 +182,63 @@
     #   sphinx-jinja2-compat
     #   torch
     #   torch-geometric
 jmespath==1.0.1
     # via
     #   boto3
     #   botocore
-joblib==1.3.2
+joblib==1.4.0
     # via
     #   molflux
     #   scikit-learn
 jsonschema==4.21.1
     # via nbformat
 jsonschema-specifications==2023.12.1
     # via jsonschema
 jupyter-cache==1.0.0
     # via myst-nb
-jupyter-client==8.6.0
+jupyter-client==8.6.1
     # via
     #   ipykernel
     #   nbclient
-jupyter-core==5.7.1
+jupyter-core==5.7.2
     # via
     #   ipykernel
     #   jupyter-client
     #   nbclient
     #   nbformat
 jupyterlab-widgets==3.0.10
     # via ipywidgets
 jupytext==1.16.1
     # via physicsml (pyproject.toml)
 kiwisolver==1.4.5
     # via matplotlib
 lark-parser==0.12.0
     # via torchani
-lightning==2.2.0.post0
+lightning==2.2.3
     # via physicsml (pyproject.toml)
-lightning-utilities==0.10.1
+lightning-utilities==0.11.2
     # via
     #   lightning
     #   pytorch-lightning
     #   torchmetrics
-markdown==3.5.2
-    # via tensorboard
 markdown-it-py==3.0.0
     # via
     #   jupytext
     #   mdit-py-plugins
     #   myst-parser
 markupsafe==2.1.5
     # via
     #   jinja2
     #   sphinx-jinja2-compat
-    #   werkzeug
-matplotlib==3.8.3
+matplotlib==3.8.4
     # via
     #   ase
     #   physicsml (pyproject.toml)
-matplotlib-inline==0.1.6
+matplotlib-inline==0.1.7
     # via
     #   ipykernel
     #   ipython
 mdit-py-plugins==0.4.0
     # via
     #   jupytext
     #   myst-parser
@@ -265,43 +248,43 @@
     # via molflux
 molflux==0.3.0
     # via physicsml (pyproject.toml)
 more-itertools==10.2.0
     # via molflux
 mpmath==1.3.0
     # via sympy
-msgpack==1.0.7
+msgpack==1.0.8
     # via cachecontrol
 multidict==6.0.5
     # via
     #   aiohttp
     #   yarl
 multiprocess==0.70.16
     # via
     #   datasets
     #   evaluate
-myst-nb==1.0.0
+myst-nb==1.1.0
     # via physicsml (pyproject.toml)
-myst-parser==2.0.0
+myst-parser==3.0.0
     # via myst-nb
 natsort==8.4.0
     # via domdf-python-tools
-nbclient==0.9.0
+nbclient==0.10.0
     # via
     #   jupyter-cache
     #   myst-nb
-nbformat==5.9.2
+nbformat==5.10.4
     # via
     #   jupyter-cache
     #   jupytext
     #   myst-nb
     #   nbclient
 nest-asyncio==1.6.0
     # via ipykernel
-networkx==3.2.1
+networkx==3.3
     # via torch
 numpy==1.26.4
     # via
     #   ase
     #   contourpy
     #   datasets
     #   evaluate
@@ -312,24 +295,23 @@
     #   opt-einsum
     #   pandas
     #   pyarrow
     #   pytorch-lightning
     #   rdkit
     #   scikit-learn
     #   scipy
-    #   tensorboard
     #   torch-geometric
     #   torchmetrics
 openeye-toolkits==2023.2.3
     # via physicsml (pyproject.toml)
 opt-einsum==3.3.0
     # via opt-einsum-fx
 opt-einsum-fx==0.1.4
     # via e3nn
-packaging==23.2
+packaging==24.0
     # via
     #   datasets
     #   evaluate
     #   huggingface-hub
     #   ipykernel
     #   jupytext
     #   lightning
@@ -337,114 +319,111 @@
     #   matplotlib
     #   opt-einsum-fx
     #   pydata-sphinx-theme
     #   pytest
     #   pytorch-lightning
     #   sphinx
     #   torchmetrics
-pandas==2.2.0
+pandas==2.2.2
     # via
     #   datasets
     #   evaluate
     #   molflux
-parso==0.8.3
+parso==0.8.4
     # via jedi
 pexpect==4.9.0
     # via ipython
-pillow==10.2.0
+pillow==10.3.0
     # via
     #   matplotlib
     #   rdkit
-platformdirs==4.2.0
+platformdirs==4.2.1
     # via
     #   apeye
     #   jupyter-core
-pluggy==1.4.0
+pluggy==1.5.0
     # via pytest
 prompt-toolkit==3.0.43
     # via ipython
-protobuf==4.25.3
-    # via tensorboard
 psutil==5.9.8
     # via
     #   ipykernel
     #   torch-geometric
 ptyprocess==0.7.0
     # via pexpect
 pure-eval==0.2.2
     # via stack-data
-pyarrow==15.0.0
+pyarrow==16.0.0
     # via
     #   datasets
     #   molflux
 pyarrow-hotfix==0.6
     # via datasets
-pydantic==1.10.14
+pydantic==1.10.15
     # via molflux
 pydata-sphinx-theme==0.15.2
     # via sphinx-book-theme
 pygments==2.17.2
     # via
     #   accessible-pygments
     #   ipython
     #   pydata-sphinx-theme
     #   sphinx
     #   sphinx-prompt
     #   sphinx-tabs
-pyparsing==3.1.1
+pyparsing==3.1.2
     # via
     #   matplotlib
     #   torch-geometric
-pytest==8.0.1
+pytest==8.1.1
     # via physicsml (pyproject.toml)
-python-dateutil==2.8.2
+python-dateutil==2.9.0.post0
     # via
     #   botocore
     #   jupyter-client
     #   matplotlib
     #   molflux
     #   pandas
-pytorch-lightning==2.2.0.post0
+pytorch-lightning==2.2.3
     # via lightning
 pytz==2024.1
     # via pandas
 pyyaml==6.0.1
     # via
     #   datasets
     #   huggingface-hub
     #   jupyter-cache
     #   jupytext
     #   lightning
     #   molflux
     #   myst-nb
     #   myst-parser
     #   pytorch-lightning
-pyzmq==25.1.2
+pyzmq==26.0.2
     # via
     #   ipykernel
     #   jupyter-client
 qlient==1.0.0
     # via molflux
 qlient-core==1.0.1
     # via qlient
-rapidfuzz==3.6.1
+rapidfuzz==3.8.1
     # via thefuzz
 rdkit==2023.9.5
     # via physicsml (pyproject.toml)
-referencing==0.33.0
+referencing==0.35.0
     # via
     #   jsonschema
     #   jsonschema-specifications
 requests==2.31.0
     # via
     #   apeye
     #   cachecontrol
     #   datasets
     #   evaluate
-    #   fsspec
     #   huggingface-hub
     #   molflux
     #   qlient
     #   responses
     #   sphinx
     #   torch-geometric
     #   torchani
@@ -454,38 +433,37 @@
     # via
     #   jsonschema
     #   referencing
 ruamel-yaml==0.18.6
     # via sphinx-toolbox
 ruamel-yaml-clib==0.2.8
     # via ruamel-yaml
-s3transfer==0.10.0
+s3transfer==0.10.1
     # via boto3
-scikit-learn==1.4.1.post1
+scikit-learn==1.4.2
     # via
     #   molflux
     #   torch-geometric
-scipy==1.12.0
+scipy==1.13.0
     # via
     #   ase
     #   e3nn
     #   molflux
     #   scikit-learn
     #   torch-geometric
 six==1.16.0
     # via
     #   asttokens
     #   html5lib
     #   python-dateutil
-    #   tensorboard
 snowballstemmer==2.2.0
     # via sphinx
 soupsieve==2.5
     # via beautifulsoup4
-sphinx==7.2.6
+sphinx==7.3.7
     # via
     #   autodocsumm
     #   myst-nb
     #   myst-parser
     #   physicsml (pyproject.toml)
     #   pydata-sphinx-theme
     #   sphinx-autodoc-typehints
@@ -493,15 +471,15 @@
     #   sphinx-design
     #   sphinx-inline-tabs
     #   sphinx-prompt
     #   sphinx-sitemap
     #   sphinx-tabs
     #   sphinx-togglebutton
     #   sphinx-toolbox
-sphinx-autodoc-typehints==2.0.0
+sphinx-autodoc-typehints==2.1.0
     # via sphinx-toolbox
 sphinx-book-theme==1.1.2
     # via physicsml (pyproject.toml)
 sphinx-design==0.5.0
     # via physicsml (pyproject.toml)
 sphinx-inline-tabs==2023.4.21
     # via physicsml (pyproject.toml)
@@ -525,56 +503,48 @@
     # via sphinx
 sphinxcontrib-jsmath==1.0.1
     # via sphinx
 sphinxcontrib-qthelp==1.0.7
     # via sphinx
 sphinxcontrib-serializinghtml==1.1.10
     # via sphinx
-sqlalchemy==2.0.27
+sqlalchemy==2.0.29
     # via jupyter-cache
 stack-data==0.6.3
     # via ipython
 sympy==1.12
     # via
     #   e3nn
     #   torch
 tabulate==0.9.0
     # via
     #   jupyter-cache
     #   sphinx-toolbox
 tenacity==8.2.3
     # via molflux
-tensorboard==2.16.2
-    # via physicsml (pyproject.toml)
-tensorboard-data-server==0.7.2
-    # via tensorboard
 thefuzz==0.22.1
     # via molflux
-threadpoolctl==3.3.0
+threadpoolctl==3.4.0
     # via scikit-learn
 toml==0.10.2
     # via jupytext
-tomli==2.0.1
-    # via
-    #   coverage
-    #   pytest
-torch==2.0.1
+torch==2.3.0
     # via
     #   e3nn
     #   lightning
     #   opt-einsum-fx
     #   physicsml (pyproject.toml)
     #   pytorch-lightning
     #   torchani
     #   torchmetrics
-torch-geometric==2.5.0
+torch-geometric==2.5.3
     # via physicsml (pyproject.toml)
 torchani==2.2.3
     # via physicsml (pyproject.toml)
-torchmetrics==1.3.1
+torchmetrics==1.3.2
     # via
     #   lightning
     #   pytorch-lightning
 tornado==6.4
     # via
     #   ipykernel
     #   jupyter-client
@@ -583,28 +553,27 @@
     #   datasets
     #   evaluate
     #   huggingface-hub
     #   lightning
     #   molflux
     #   pytorch-lightning
     #   torch-geometric
-traitlets==5.14.1
+traitlets==5.14.3
     # via
     #   comm
     #   ipykernel
     #   ipython
     #   ipywidgets
     #   jupyter-client
     #   jupyter-core
     #   matplotlib-inline
     #   nbclient
     #   nbformat
-typing-extensions==4.9.0
+typing-extensions==4.11.0
     # via
-    #   cloudpathlib
     #   domdf-python-tools
     #   huggingface-hub
     #   ipython
     #   lightning
     #   lightning-utilities
     #   molflux
     #   myst-nb
@@ -612,37 +581,33 @@
     #   pydata-sphinx-theme
     #   pytorch-lightning
     #   sphinx-toolbox
     #   sqlalchemy
     #   torch
 tzdata==2024.1
     # via pandas
-urllib3==1.26.18
+urllib3==2.2.1
     # via
     #   botocore
     #   requests
     #   responses
 wcwidth==0.2.13
     # via prompt-toolkit
 webencodings==0.5.1
     # via html5lib
-websocket-client==1.7.0
+websocket-client==1.8.0
     # via qlient
-werkzeug==3.0.1
-    # via tensorboard
-wheel==0.42.0
+wheel==0.43.0
     # via sphinx-togglebutton
 widgetsnbextension==4.0.10
     # via ipywidgets
 xxhash==3.4.1
     # via
     #   datasets
     #   evaluate
 yarl==1.9.4
     # via aiohttp
-zipp==3.17.0
-    # via
-    #   importlib-metadata
-    #   importlib-resources
+zipp==3.18.1
+    # via importlib-metadata
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `physicsml-0.2.3/pinned-versions/3.9/lockfile.openmm.txt` & `physicsml-0.2.4/pinned-versions/3.11/lockfile.ase.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 #
-# This file is autogenerated by pip-compile with Python 3.9
+# This file is autogenerated by pip-compile with Python 3.11
 # by the following command:
 #
-#    nox -s dependencies_pin-3.9(extra='openmm')
+#    nox -s dependencies_pin-3.11(extra='ase')
 #
-absl-py==2.1.0
-    # via tensorboard
 accessible-pygments==0.0.4
     # via pydata-sphinx-theme
-aiohttp==3.9.3
+aiohttp==3.9.5
     # via
     #   datasets
     #   fsspec
     #   torch-geometric
 aiosignal==1.3.1
     # via aiohttp
 alabaster==0.7.16
@@ -23,16 +21,14 @@
     # via apeye
 appnope==0.1.4
     # via ipykernel
 ase==3.22.1
     # via physicsml (pyproject.toml)
 asttokens==2.4.1
     # via stack-data
-async-timeout==4.0.3
-    # via aiohttp
 attrs==23.2.0
     # via
     #   aiohttp
     #   jsonschema
     #   jupyter-cache
     #   referencing
 autodocsumm==0.2.12
@@ -41,67 +37,67 @@
     # via
     #   pydata-sphinx-theme
     #   sphinx
 beautifulsoup4==4.12.3
     # via
     #   pydata-sphinx-theme
     #   sphinx-toolbox
-boto3==1.34.45
+boto3==1.34.91
     # via
     #   cloudpathlib
     #   molflux
-botocore==1.34.45
+botocore==1.34.91
     # via
     #   boto3
     #   molflux
     #   s3transfer
 cachecontrol==0.14.0
     # via sphinx-toolbox
 certifi==2024.2.2
     # via requests
 charset-normalizer==3.3.2
     # via requests
 click==8.1.7
     # via jupyter-cache
-cloudpathlib==0.17.0
+cloudpathlib==0.18.1
     # via molflux
 colorama==0.4.6
     # via molflux
-comm==0.2.1
+comm==0.2.2
     # via
     #   ipykernel
     #   ipywidgets
-contourpy==1.2.0
+contourpy==1.2.1
     # via matplotlib
-coverage==7.4.1
+coverage==7.5.0
     # via
     #   coverage-badge
     #   physicsml (pyproject.toml)
-coverage-badge==1.1.0
+coverage-badge==1.1.1
     # via physicsml (pyproject.toml)
-cssutils==2.9.0
+cssutils==2.10.2
     # via dict2css
 cycler==0.12.1
     # via matplotlib
-datasets==2.17.1
+datasets==2.19.0
     # via
     #   evaluate
     #   molflux
 debugpy==1.8.1
     # via ipykernel
 decorator==5.1.1
     # via ipython
 dict2css==0.3.0.post1
     # via sphinx-toolbox
 dill==0.3.8
     # via
     #   datasets
     #   evaluate
     #   multiprocess
-docutils==0.20.1
+docutils==0.21.2
     # via
     #   myst-parser
     #   pydata-sphinx-theme
     #   sphinx
     #   sphinx-prompt
     #   sphinx-tabs
     #   sphinx-togglebutton
@@ -112,79 +108,69 @@
     #   apeye-core
     #   dict2css
     #   sphinx-toolbox
 e3nn==0.5.1
     # via physicsml (pyproject.toml)
 evaluate==0.4.1
     # via molflux
-exceptiongroup==1.2.0
-    # via
-    #   ipython
-    #   pytest
 executing==2.0.1
     # via stack-data
 fastjsonschema==2.19.1
     # via nbformat
-filelock==3.13.1
+filelock==3.13.4
     # via
     #   cachecontrol
     #   datasets
     #   huggingface-hub
     #   sphinx-toolbox
     #   torch
-fonttools==4.49.0
+fonttools==4.51.0
     # via matplotlib
 frozenlist==1.4.1
     # via
     #   aiohttp
     #   aiosignal
-fsspec==2023.10.0
+fsspec==2024.3.1
     # via
     #   datasets
     #   evaluate
     #   huggingface-hub
     #   lightning
     #   molflux
     #   pytorch-lightning
+    #   torch
     #   torch-geometric
-grpcio==1.60.1
-    # via tensorboard
-h5py==3.10.0
+h5py==3.11.0
     # via
     #   molflux
     #   physicsml (pyproject.toml)
 html5lib==1.1
     # via sphinx-toolbox
-huggingface-hub==0.20.3
+huggingface-hub==0.22.2
     # via
     #   datasets
     #   evaluate
-idna==3.6
+idna==3.7
     # via
     #   apeye-core
     #   requests
     #   yarl
 imagesize==1.4.1
     # via sphinx
 importlib-metadata==4.13.0
     # via
     #   jupyter-cache
-    #   jupyter-client
-    #   markdown
     #   myst-nb
     #   qlient-core
-    #   sphinx
     #   torchani
-importlib-resources==6.1.1
-    # via matplotlib
 iniconfig==2.0.0
     # via pytest
-ipykernel==6.29.2
+ipykernel==6.29.4
     # via myst-nb
-ipython==8.18.1
+ipython==8.23.0
     # via
     #   ipykernel
     #   ipywidgets
     #   myst-nb
 ipywidgets==8.1.2
     # via physicsml (pyproject.toml)
 jedi==0.19.1
@@ -196,66 +182,63 @@
     #   sphinx-jinja2-compat
     #   torch
     #   torch-geometric
 jmespath==1.0.1
     # via
     #   boto3
     #   botocore
-joblib==1.3.2
+joblib==1.4.0
     # via
     #   molflux
     #   scikit-learn
 jsonschema==4.21.1
     # via nbformat
 jsonschema-specifications==2023.12.1
     # via jsonschema
 jupyter-cache==1.0.0
     # via myst-nb
-jupyter-client==8.6.0
+jupyter-client==8.6.1
     # via
     #   ipykernel
     #   nbclient
-jupyter-core==5.7.1
+jupyter-core==5.7.2
     # via
     #   ipykernel
     #   jupyter-client
     #   nbclient
     #   nbformat
 jupyterlab-widgets==3.0.10
     # via ipywidgets
 jupytext==1.16.1
     # via physicsml (pyproject.toml)
 kiwisolver==1.4.5
     # via matplotlib
 lark-parser==0.12.0
     # via torchani
-lightning==2.2.0.post0
+lightning==2.2.3
     # via physicsml (pyproject.toml)
-lightning-utilities==0.10.1
+lightning-utilities==0.11.2
     # via
     #   lightning
     #   pytorch-lightning
     #   torchmetrics
-markdown==3.5.2
-    # via tensorboard
 markdown-it-py==3.0.0
     # via
     #   jupytext
     #   mdit-py-plugins
     #   myst-parser
 markupsafe==2.1.5
     # via
     #   jinja2
     #   sphinx-jinja2-compat
-    #   werkzeug
-matplotlib==3.8.3
+matplotlib==3.8.4
     # via
     #   ase
     #   physicsml (pyproject.toml)
-matplotlib-inline==0.1.6
+matplotlib-inline==0.1.7
     # via
     #   ipykernel
     #   ipython
 mdit-py-plugins==0.4.0
     # via
     #   jupytext
     #   myst-parser
@@ -265,43 +248,43 @@
     # via molflux
 molflux==0.3.0
     # via physicsml (pyproject.toml)
 more-itertools==10.2.0
     # via molflux
 mpmath==1.3.0
     # via sympy
-msgpack==1.0.7
+msgpack==1.0.8
     # via cachecontrol
 multidict==6.0.5
     # via
     #   aiohttp
     #   yarl
 multiprocess==0.70.16
     # via
     #   datasets
     #   evaluate
-myst-nb==1.0.0
+myst-nb==1.1.0
     # via physicsml (pyproject.toml)
-myst-parser==2.0.0
+myst-parser==3.0.0
     # via myst-nb
 natsort==8.4.0
     # via domdf-python-tools
-nbclient==0.9.0
+nbclient==0.10.0
     # via
     #   jupyter-cache
     #   myst-nb
-nbformat==5.9.2
+nbformat==5.10.4
     # via
     #   jupyter-cache
     #   jupytext
     #   myst-nb
     #   nbclient
 nest-asyncio==1.6.0
     # via ipykernel
-networkx==3.2.1
+networkx==3.3
     # via torch
 numpy==1.26.4
     # via
     #   ase
     #   contourpy
     #   datasets
     #   evaluate
@@ -312,22 +295,21 @@
     #   opt-einsum
     #   pandas
     #   pyarrow
     #   pytorch-lightning
     #   rdkit
     #   scikit-learn
     #   scipy
-    #   tensorboard
     #   torch-geometric
     #   torchmetrics
 opt-einsum==3.3.0
     # via opt-einsum-fx
 opt-einsum-fx==0.1.4
     # via e3nn
-packaging==23.2
+packaging==24.0
     # via
     #   datasets
     #   evaluate
     #   huggingface-hub
     #   ipykernel
     #   jupytext
     #   lightning
@@ -335,114 +317,111 @@
     #   matplotlib
     #   opt-einsum-fx
     #   pydata-sphinx-theme
     #   pytest
     #   pytorch-lightning
     #   sphinx
     #   torchmetrics
-pandas==2.2.0
+pandas==2.2.2
     # via
     #   datasets
     #   evaluate
     #   molflux
-parso==0.8.3
+parso==0.8.4
     # via jedi
 pexpect==4.9.0
     # via ipython
-pillow==10.2.0
+pillow==10.3.0
     # via
     #   matplotlib
     #   rdkit
-platformdirs==4.2.0
+platformdirs==4.2.1
     # via
     #   apeye
     #   jupyter-core
-pluggy==1.4.0
+pluggy==1.5.0
     # via pytest
 prompt-toolkit==3.0.43
     # via ipython
-protobuf==4.25.3
-    # via tensorboard
 psutil==5.9.8
     # via
     #   ipykernel
     #   torch-geometric
 ptyprocess==0.7.0
     # via pexpect
 pure-eval==0.2.2
     # via stack-data
-pyarrow==15.0.0
+pyarrow==16.0.0
     # via
     #   datasets
     #   molflux
 pyarrow-hotfix==0.6
     # via datasets
-pydantic==1.10.14
+pydantic==1.10.15
     # via molflux
 pydata-sphinx-theme==0.15.2
     # via sphinx-book-theme
 pygments==2.17.2
     # via
     #   accessible-pygments
     #   ipython
     #   pydata-sphinx-theme
     #   sphinx
     #   sphinx-prompt
     #   sphinx-tabs
-pyparsing==3.1.1
+pyparsing==3.1.2
     # via
     #   matplotlib
     #   torch-geometric
-pytest==8.0.1
+pytest==8.1.1
     # via physicsml (pyproject.toml)
-python-dateutil==2.8.2
+python-dateutil==2.9.0.post0
     # via
     #   botocore
     #   jupyter-client
     #   matplotlib
     #   molflux
     #   pandas
-pytorch-lightning==2.2.0.post0
+pytorch-lightning==2.2.3
     # via lightning
 pytz==2024.1
     # via pandas
 pyyaml==6.0.1
     # via
     #   datasets
     #   huggingface-hub
     #   jupyter-cache
     #   jupytext
     #   lightning
     #   molflux
     #   myst-nb
     #   myst-parser
     #   pytorch-lightning
-pyzmq==25.1.2
+pyzmq==26.0.2
     # via
     #   ipykernel
     #   jupyter-client
 qlient==1.0.0
     # via molflux
 qlient-core==1.0.1
     # via qlient
-rapidfuzz==3.6.1
+rapidfuzz==3.8.1
     # via thefuzz
 rdkit==2023.9.5
     # via physicsml (pyproject.toml)
-referencing==0.33.0
+referencing==0.35.0
     # via
     #   jsonschema
     #   jsonschema-specifications
 requests==2.31.0
     # via
     #   apeye
     #   cachecontrol
     #   datasets
     #   evaluate
-    #   fsspec
     #   huggingface-hub
     #   molflux
     #   qlient
     #   responses
     #   sphinx
     #   torch-geometric
     #   torchani
@@ -452,38 +431,37 @@
     # via
     #   jsonschema
     #   referencing
 ruamel-yaml==0.18.6
     # via sphinx-toolbox
 ruamel-yaml-clib==0.2.8
     # via ruamel-yaml
-s3transfer==0.10.0
+s3transfer==0.10.1
     # via boto3
-scikit-learn==1.4.1.post1
+scikit-learn==1.4.2
     # via
     #   molflux
     #   torch-geometric
-scipy==1.12.0
+scipy==1.13.0
     # via
     #   ase
     #   e3nn
     #   molflux
     #   scikit-learn
     #   torch-geometric
 six==1.16.0
     # via
     #   asttokens
     #   html5lib
     #   python-dateutil
-    #   tensorboard
 snowballstemmer==2.2.0
     # via sphinx
 soupsieve==2.5
     # via beautifulsoup4
-sphinx==7.2.6
+sphinx==7.3.7
     # via
     #   autodocsumm
     #   myst-nb
     #   myst-parser
     #   physicsml (pyproject.toml)
     #   pydata-sphinx-theme
     #   sphinx-autodoc-typehints
@@ -491,15 +469,15 @@
     #   sphinx-design
     #   sphinx-inline-tabs
     #   sphinx-prompt
     #   sphinx-sitemap
     #   sphinx-tabs
     #   sphinx-togglebutton
     #   sphinx-toolbox
-sphinx-autodoc-typehints==2.0.0
+sphinx-autodoc-typehints==2.1.0
     # via sphinx-toolbox
 sphinx-book-theme==1.1.2
     # via physicsml (pyproject.toml)
 sphinx-design==0.5.0
     # via physicsml (pyproject.toml)
 sphinx-inline-tabs==2023.4.21
     # via physicsml (pyproject.toml)
@@ -523,56 +501,48 @@
     # via sphinx
 sphinxcontrib-jsmath==1.0.1
     # via sphinx
 sphinxcontrib-qthelp==1.0.7
     # via sphinx
 sphinxcontrib-serializinghtml==1.1.10
     # via sphinx
-sqlalchemy==2.0.27
+sqlalchemy==2.0.29
     # via jupyter-cache
 stack-data==0.6.3
     # via ipython
 sympy==1.12
     # via
     #   e3nn
     #   torch
 tabulate==0.9.0
     # via
     #   jupyter-cache
     #   sphinx-toolbox
 tenacity==8.2.3
     # via molflux
-tensorboard==2.16.2
-    # via physicsml (pyproject.toml)
-tensorboard-data-server==0.7.2
-    # via tensorboard
 thefuzz==0.22.1
     # via molflux
-threadpoolctl==3.3.0
+threadpoolctl==3.4.0
     # via scikit-learn
 toml==0.10.2
     # via jupytext
-tomli==2.0.1
-    # via
-    #   coverage
-    #   pytest
-torch==2.0.1
+torch==2.3.0
     # via
     #   e3nn
     #   lightning
     #   opt-einsum-fx
     #   physicsml (pyproject.toml)
     #   pytorch-lightning
     #   torchani
     #   torchmetrics
-torch-geometric==2.5.0
+torch-geometric==2.5.3
     # via physicsml (pyproject.toml)
 torchani==2.2.3
     # via physicsml (pyproject.toml)
-torchmetrics==1.3.1
+torchmetrics==1.3.2
     # via
     #   lightning
     #   pytorch-lightning
 tornado==6.4
     # via
     #   ipykernel
     #   jupyter-client
@@ -581,28 +551,27 @@
     #   datasets
     #   evaluate
     #   huggingface-hub
     #   lightning
     #   molflux
     #   pytorch-lightning
     #   torch-geometric
-traitlets==5.14.1
+traitlets==5.14.3
     # via
     #   comm
     #   ipykernel
     #   ipython
     #   ipywidgets
     #   jupyter-client
     #   jupyter-core
     #   matplotlib-inline
     #   nbclient
     #   nbformat
-typing-extensions==4.9.0
+typing-extensions==4.11.0
     # via
-    #   cloudpathlib
     #   domdf-python-tools
     #   huggingface-hub
     #   ipython
     #   lightning
     #   lightning-utilities
     #   molflux
     #   myst-nb
@@ -610,37 +579,33 @@
     #   pydata-sphinx-theme
     #   pytorch-lightning
     #   sphinx-toolbox
     #   sqlalchemy
     #   torch
 tzdata==2024.1
     # via pandas
-urllib3==1.26.18
+urllib3==2.2.1
     # via
     #   botocore
     #   requests
     #   responses
 wcwidth==0.2.13
     # via prompt-toolkit
 webencodings==0.5.1
     # via html5lib
-websocket-client==1.7.0
+websocket-client==1.8.0
     # via qlient
-werkzeug==3.0.1
-    # via tensorboard
-wheel==0.42.0
+wheel==0.43.0
     # via sphinx-togglebutton
 widgetsnbextension==4.0.10
     # via ipywidgets
 xxhash==3.4.1
     # via
     #   datasets
     #   evaluate
 yarl==1.9.4
     # via aiohttp
-zipp==3.17.0
-    # via
-    #   importlib-metadata
-    #   importlib-resources
+zipp==3.18.1
+    # via importlib-metadata
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `physicsml-0.2.3/pinned-versions/3.9/lockfile.rdkit.txt` & `physicsml-0.2.4/pinned-versions/3.8/lockfile.openmm.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 #
-# This file is autogenerated by pip-compile with Python 3.9
+# This file is autogenerated by pip-compile with Python 3.8
 # by the following command:
 #
-#    nox -s dependencies_pin-3.9(extra='rdkit')
+#    nox -s dependencies_pin-3.8(extra='openmm')
 #
-absl-py==2.1.0
-    # via tensorboard
 accessible-pygments==0.0.4
     # via pydata-sphinx-theme
-aiohttp==3.9.3
+aiohttp==3.9.5
     # via
     #   datasets
     #   fsspec
     #   torch-geometric
 aiosignal==1.3.1
     # via aiohttp
-alabaster==0.7.16
+alabaster==0.7.13
     # via sphinx
 apeye==1.4.1
     # via sphinx-toolbox
 apeye-core==1.1.5
     # via apeye
 appnope==0.1.4
-    # via ipykernel
+    # via
+    #   ipykernel
+    #   ipython
 ase==3.22.1
     # via physicsml (pyproject.toml)
 asttokens==2.4.1
     # via stack-data
 async-timeout==4.0.3
     # via aiohttp
 attrs==23.2.0
@@ -37,154 +37,155 @@
     #   referencing
 autodocsumm==0.2.12
     # via sphinx-toolbox
 babel==2.14.0
     # via
     #   pydata-sphinx-theme
     #   sphinx
+backcall==0.2.0
+    # via ipython
 beautifulsoup4==4.12.3
     # via
     #   pydata-sphinx-theme
     #   sphinx-toolbox
-boto3==1.34.45
+boto3==1.34.91
     # via
     #   cloudpathlib
     #   molflux
-botocore==1.34.45
+botocore==1.34.91
     # via
     #   boto3
     #   molflux
     #   s3transfer
 cachecontrol==0.14.0
     # via sphinx-toolbox
 certifi==2024.2.2
     # via requests
 charset-normalizer==3.3.2
     # via requests
 click==8.1.7
     # via jupyter-cache
-cloudpathlib==0.17.0
+cloudpathlib==0.18.1
     # via molflux
 colorama==0.4.6
     # via molflux
-comm==0.2.1
+comm==0.2.2
     # via
     #   ipykernel
     #   ipywidgets
-contourpy==1.2.0
+contourpy==1.1.1
     # via matplotlib
-coverage==7.4.1
+coverage==7.5.0
     # via
     #   coverage-badge
     #   physicsml (pyproject.toml)
-coverage-badge==1.1.0
+coverage-badge==1.1.1
     # via physicsml (pyproject.toml)
-cssutils==2.9.0
+cssutils==2.10.2
     # via dict2css
 cycler==0.12.1
     # via matplotlib
-datasets==2.17.1
+datasets==2.19.0
     # via
     #   evaluate
     #   molflux
 debugpy==1.8.1
     # via ipykernel
 decorator==5.1.1
     # via ipython
 dict2css==0.3.0.post1
     # via sphinx-toolbox
 dill==0.3.8
     # via
     #   datasets
     #   evaluate
     #   multiprocess
-docutils==0.20.1
+docutils==0.19
     # via
     #   myst-parser
     #   pydata-sphinx-theme
     #   sphinx
-    #   sphinx-prompt
     #   sphinx-tabs
     #   sphinx-togglebutton
     #   sphinx-toolbox
 domdf-python-tools==3.8.0.post2
     # via
     #   apeye
     #   apeye-core
     #   dict2css
     #   sphinx-toolbox
 e3nn==0.5.1
     # via physicsml (pyproject.toml)
 evaluate==0.4.1
     # via molflux
-exceptiongroup==1.2.0
-    # via
-    #   ipython
-    #   pytest
+exceptiongroup==1.2.1
+    # via pytest
 executing==2.0.1
     # via stack-data
 fastjsonschema==2.19.1
     # via nbformat
-filelock==3.13.1
+filelock==3.13.4
     # via
     #   cachecontrol
     #   datasets
     #   huggingface-hub
     #   sphinx-toolbox
     #   torch
-fonttools==4.49.0
+fonttools==4.51.0
     # via matplotlib
 frozenlist==1.4.1
     # via
     #   aiohttp
     #   aiosignal
-fsspec==2023.10.0
+fsspec==2024.3.1
     # via
     #   datasets
     #   evaluate
     #   huggingface-hub
     #   lightning
     #   molflux
     #   pytorch-lightning
+    #   torch
     #   torch-geometric
-grpcio==1.60.1
-    # via tensorboard
-h5py==3.10.0
+h5py==3.11.0
     # via
     #   molflux
     #   physicsml (pyproject.toml)
 html5lib==1.1
     # via sphinx-toolbox
-huggingface-hub==0.20.3
+huggingface-hub==0.22.2
     # via
     #   datasets
     #   evaluate
-idna==3.6
+idna==3.7
     # via
     #   apeye-core
     #   requests
     #   yarl
 imagesize==1.4.1
     # via sphinx
 importlib-metadata==4.13.0
     # via
+    #   domdf-python-tools
     #   jupyter-cache
     #   jupyter-client
-    #   markdown
     #   myst-nb
     #   qlient-core
     #   sphinx
     #   torchani
-importlib-resources==6.1.1
-    # via matplotlib
+importlib-resources==6.4.0
+    # via
+    #   jsonschema
+    #   jsonschema-specifications
+    #   matplotlib
 iniconfig==2.0.0
     # via pytest
-ipykernel==6.29.2
+ipykernel==6.29.4
     # via myst-nb
-ipython==8.18.1
+ipython==8.12.3
     # via
     #   ipykernel
     #   ipywidgets
     #   myst-nb
 ipywidgets==8.1.2
     # via physicsml (pyproject.toml)
 jedi==0.19.1
@@ -196,114 +197,111 @@
     #   sphinx-jinja2-compat
     #   torch
     #   torch-geometric
 jmespath==1.0.1
     # via
     #   boto3
     #   botocore
-joblib==1.3.2
+joblib==1.4.0
     # via
     #   molflux
     #   scikit-learn
 jsonschema==4.21.1
     # via nbformat
 jsonschema-specifications==2023.12.1
     # via jsonschema
-jupyter-cache==1.0.0
+jupyter-cache==0.6.1
     # via myst-nb
-jupyter-client==8.6.0
+jupyter-client==8.6.1
     # via
     #   ipykernel
     #   nbclient
-jupyter-core==5.7.1
+jupyter-core==5.7.2
     # via
     #   ipykernel
     #   jupyter-client
     #   nbclient
     #   nbformat
 jupyterlab-widgets==3.0.10
     # via ipywidgets
 jupytext==1.16.1
     # via physicsml (pyproject.toml)
 kiwisolver==1.4.5
     # via matplotlib
 lark-parser==0.12.0
     # via torchani
-lightning==2.2.0.post0
+lightning==2.2.3
     # via physicsml (pyproject.toml)
-lightning-utilities==0.10.1
+lightning-utilities==0.11.2
     # via
     #   lightning
     #   pytorch-lightning
     #   torchmetrics
-markdown==3.5.2
-    # via tensorboard
-markdown-it-py==3.0.0
+markdown-it-py==2.2.0
     # via
     #   jupytext
     #   mdit-py-plugins
     #   myst-parser
 markupsafe==2.1.5
     # via
     #   jinja2
     #   sphinx-jinja2-compat
-    #   werkzeug
-matplotlib==3.8.3
+matplotlib==3.7.5
     # via
     #   ase
     #   physicsml (pyproject.toml)
-matplotlib-inline==0.1.6
+matplotlib-inline==0.1.7
     # via
     #   ipykernel
     #   ipython
-mdit-py-plugins==0.4.0
+mdit-py-plugins==0.3.5
     # via
     #   jupytext
     #   myst-parser
 mdurl==0.1.2
     # via markdown-it-py
 mergedeep==1.3.4
     # via molflux
 molflux==0.3.0
     # via physicsml (pyproject.toml)
 more-itertools==10.2.0
     # via molflux
 mpmath==1.3.0
     # via sympy
-msgpack==1.0.7
+msgpack==1.0.8
     # via cachecontrol
 multidict==6.0.5
     # via
     #   aiohttp
     #   yarl
 multiprocess==0.70.16
     # via
     #   datasets
     #   evaluate
-myst-nb==1.0.0
+myst-nb==0.17.2
     # via physicsml (pyproject.toml)
-myst-parser==2.0.0
+myst-parser==0.18.1
     # via myst-nb
 natsort==8.4.0
     # via domdf-python-tools
-nbclient==0.9.0
+nbclient==0.7.4
     # via
     #   jupyter-cache
     #   myst-nb
-nbformat==5.9.2
+nbformat==5.10.4
     # via
     #   jupyter-cache
     #   jupytext
     #   myst-nb
     #   nbclient
 nest-asyncio==1.6.0
     # via ipykernel
-networkx==3.2.1
+networkx==3.1
     # via torch
-numpy==1.26.4
+numpy==1.24.4
     # via
     #   ase
     #   contourpy
     #   datasets
     #   evaluate
     #   h5py
     #   lightning
@@ -312,22 +310,21 @@
     #   opt-einsum
     #   pandas
     #   pyarrow
     #   pytorch-lightning
     #   rdkit
     #   scikit-learn
     #   scipy
-    #   tensorboard
     #   torch-geometric
     #   torchmetrics
 opt-einsum==3.3.0
     # via opt-einsum-fx
 opt-einsum-fx==0.1.4
     # via e3nn
-packaging==23.2
+packaging==24.0
     # via
     #   datasets
     #   evaluate
     #   huggingface-hub
     #   ipykernel
     #   jupytext
     #   lightning
@@ -335,114 +332,117 @@
     #   matplotlib
     #   opt-einsum-fx
     #   pydata-sphinx-theme
     #   pytest
     #   pytorch-lightning
     #   sphinx
     #   torchmetrics
-pandas==2.2.0
+pandas==2.0.3
     # via
     #   datasets
     #   evaluate
     #   molflux
-parso==0.8.3
+parso==0.8.4
     # via jedi
 pexpect==4.9.0
     # via ipython
-pillow==10.2.0
+pickleshare==0.7.5
+    # via ipython
+pillow==10.3.0
     # via
     #   matplotlib
     #   rdkit
-platformdirs==4.2.0
+pkgutil-resolve-name==1.3.10
+    # via jsonschema
+platformdirs==4.2.1
     # via
     #   apeye
     #   jupyter-core
-pluggy==1.4.0
+pluggy==1.5.0
     # via pytest
 prompt-toolkit==3.0.43
     # via ipython
-protobuf==4.25.3
-    # via tensorboard
 psutil==5.9.8
     # via
     #   ipykernel
     #   torch-geometric
 ptyprocess==0.7.0
     # via pexpect
 pure-eval==0.2.2
     # via stack-data
-pyarrow==15.0.0
+pyarrow==16.0.0
     # via
     #   datasets
     #   molflux
 pyarrow-hotfix==0.6
     # via datasets
-pydantic==1.10.14
+pydantic==1.10.15
     # via molflux
-pydata-sphinx-theme==0.15.2
+pydata-sphinx-theme==0.14.4
     # via sphinx-book-theme
 pygments==2.17.2
     # via
     #   accessible-pygments
     #   ipython
     #   pydata-sphinx-theme
     #   sphinx
     #   sphinx-prompt
     #   sphinx-tabs
-pyparsing==3.1.1
+pyparsing==3.1.2
     # via
     #   matplotlib
     #   torch-geometric
-pytest==8.0.1
+pytest==8.1.1
     # via physicsml (pyproject.toml)
-python-dateutil==2.8.2
+python-dateutil==2.9.0.post0
     # via
     #   botocore
     #   jupyter-client
     #   matplotlib
     #   molflux
     #   pandas
-pytorch-lightning==2.2.0.post0
+pytorch-lightning==2.2.3
     # via lightning
 pytz==2024.1
-    # via pandas
+    # via
+    #   babel
+    #   pandas
 pyyaml==6.0.1
     # via
     #   datasets
     #   huggingface-hub
     #   jupyter-cache
     #   jupytext
     #   lightning
     #   molflux
     #   myst-nb
     #   myst-parser
     #   pytorch-lightning
-pyzmq==25.1.2
+pyzmq==26.0.2
     # via
     #   ipykernel
     #   jupyter-client
 qlient==1.0.0
     # via molflux
 qlient-core==1.0.1
     # via qlient
-rapidfuzz==3.6.1
+rapidfuzz==3.8.1
     # via thefuzz
 rdkit==2023.9.5
     # via physicsml (pyproject.toml)
-referencing==0.33.0
+referencing==0.35.0
     # via
     #   jsonschema
     #   jsonschema-specifications
 requests==2.31.0
     # via
     #   apeye
     #   cachecontrol
     #   datasets
     #   evaluate
-    #   fsspec
     #   huggingface-hub
     #   molflux
     #   qlient
     #   responses
     #   sphinx
     #   torch-geometric
     #   torchani
@@ -452,38 +452,37 @@
     # via
     #   jsonschema
     #   referencing
 ruamel-yaml==0.18.6
     # via sphinx-toolbox
 ruamel-yaml-clib==0.2.8
     # via ruamel-yaml
-s3transfer==0.10.0
+s3transfer==0.10.1
     # via boto3
-scikit-learn==1.4.1.post1
+scikit-learn==1.3.2
     # via
     #   molflux
     #   torch-geometric
-scipy==1.12.0
+scipy==1.10.1
     # via
     #   ase
     #   e3nn
     #   molflux
     #   scikit-learn
     #   torch-geometric
 six==1.16.0
     # via
     #   asttokens
     #   html5lib
     #   python-dateutil
-    #   tensorboard
 snowballstemmer==2.2.0
     # via sphinx
 soupsieve==2.5
     # via beautifulsoup4
-sphinx==7.2.6
+sphinx==5.3.0
     # via
     #   autodocsumm
     #   myst-nb
     #   myst-parser
     #   physicsml (pyproject.toml)
     #   pydata-sphinx-theme
     #   sphinx-autodoc-typehints
@@ -491,88 +490,84 @@
     #   sphinx-design
     #   sphinx-inline-tabs
     #   sphinx-prompt
     #   sphinx-sitemap
     #   sphinx-tabs
     #   sphinx-togglebutton
     #   sphinx-toolbox
-sphinx-autodoc-typehints==2.0.0
+sphinx-autodoc-typehints==1.23.0
     # via sphinx-toolbox
-sphinx-book-theme==1.1.2
+sphinx-book-theme==1.0.1
     # via physicsml (pyproject.toml)
 sphinx-design==0.5.0
     # via physicsml (pyproject.toml)
 sphinx-inline-tabs==2023.4.21
     # via physicsml (pyproject.toml)
 sphinx-jinja2-compat==0.2.0.post1
     # via sphinx-toolbox
-sphinx-prompt==1.8.0
+sphinx-prompt==1.5.0
     # via sphinx-toolbox
 sphinx-sitemap==2.5.1
     # via physicsml (pyproject.toml)
 sphinx-tabs==3.4.5
     # via sphinx-toolbox
 sphinx-togglebutton==0.3.2
     # via physicsml (pyproject.toml)
 sphinx-toolbox==3.5.0
     # via physicsml (pyproject.toml)
-sphinxcontrib-applehelp==1.0.8
+sphinxcontrib-applehelp==1.0.4
     # via sphinx
-sphinxcontrib-devhelp==1.0.6
+sphinxcontrib-devhelp==1.0.2
     # via sphinx
-sphinxcontrib-htmlhelp==2.0.5
+sphinxcontrib-htmlhelp==2.0.1
     # via sphinx
 sphinxcontrib-jsmath==1.0.1
     # via sphinx
-sphinxcontrib-qthelp==1.0.7
+sphinxcontrib-qthelp==1.0.3
     # via sphinx
-sphinxcontrib-serializinghtml==1.1.10
+sphinxcontrib-serializinghtml==1.1.5
     # via sphinx
-sqlalchemy==2.0.27
+sqlalchemy==2.0.29
     # via jupyter-cache
 stack-data==0.6.3
     # via ipython
 sympy==1.12
     # via
     #   e3nn
     #   torch
 tabulate==0.9.0
     # via
     #   jupyter-cache
     #   sphinx-toolbox
 tenacity==8.2.3
     # via molflux
-tensorboard==2.16.2
-    # via physicsml (pyproject.toml)
-tensorboard-data-server==0.7.2
-    # via tensorboard
 thefuzz==0.22.1
     # via molflux
-threadpoolctl==3.3.0
+threadpoolctl==3.4.0
     # via scikit-learn
 toml==0.10.2
     # via jupytext
 tomli==2.0.1
     # via
     #   coverage
     #   pytest
-torch==2.0.1
+torch==2.3.0
     # via
     #   e3nn
     #   lightning
     #   opt-einsum-fx
     #   physicsml (pyproject.toml)
     #   pytorch-lightning
     #   torchani
     #   torchmetrics
-torch-geometric==2.5.0
+torch-geometric==2.5.3
     # via physicsml (pyproject.toml)
 torchani==2.2.3
     # via physicsml (pyproject.toml)
-torchmetrics==1.3.1
+torchmetrics==1.3.2
     # via
     #   lightning
     #   pytorch-lightning
 tornado==6.4
     # via
     #   ipykernel
     #   jupyter-client
@@ -581,66 +576,66 @@
     #   datasets
     #   evaluate
     #   huggingface-hub
     #   lightning
     #   molflux
     #   pytorch-lightning
     #   torch-geometric
-traitlets==5.14.1
+traitlets==5.14.3
     # via
     #   comm
     #   ipykernel
     #   ipython
     #   ipywidgets
     #   jupyter-client
     #   jupyter-core
     #   matplotlib-inline
     #   nbclient
     #   nbformat
-typing-extensions==4.9.0
+typing-extensions==4.11.0
     # via
     #   cloudpathlib
     #   domdf-python-tools
     #   huggingface-hub
     #   ipython
     #   lightning
     #   lightning-utilities
     #   molflux
     #   myst-nb
+    #   myst-parser
     #   pydantic
     #   pydata-sphinx-theme
     #   pytorch-lightning
     #   sphinx-toolbox
     #   sqlalchemy
     #   torch
+    #   torchmetrics
 tzdata==2024.1
     # via pandas
 urllib3==1.26.18
     # via
     #   botocore
     #   requests
     #   responses
 wcwidth==0.2.13
     # via prompt-toolkit
 webencodings==0.5.1
     # via html5lib
-websocket-client==1.7.0
+websocket-client==1.8.0
     # via qlient
-werkzeug==3.0.1
-    # via tensorboard
-wheel==0.42.0
+wheel==0.43.0
     # via sphinx-togglebutton
 widgetsnbextension==4.0.10
     # via ipywidgets
 xxhash==3.4.1
     # via
     #   datasets
     #   evaluate
 yarl==1.9.4
     # via aiohttp
-zipp==3.17.0
+zipp==3.18.1
     # via
     #   importlib-metadata
     #   importlib-resources
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `physicsml-0.2.3/pyproject.toml` & `physicsml-0.2.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -23,21 +23,19 @@
     'Typing :: Typed',
 ]
 
 dynamic = ['version']
 
 dependencies = [
     'molflux',
-    'torch>=2.0,<2.1',
+    'torch>=2.0',
     'lightning>=2.1',
     'torch-geometric>=2.5.0',
-    'torch-nl',
     'e3nn',
     'torchani!=2.2.4', # bug in torchani where it tries to import cuaev when not built
-    'tensorboard',
 ]
 
 [project.optional-dependencies]
 openeye = [
     'openeye-toolkits<2023.0.0; python_version == "3.8"',  # openeye 2023 not supported on python 3.8
     'openeye-toolkits',
 ]
```

### Comparing `physicsml-0.2.3/src/physicsml/backends/backend_selector.py` & `physicsml-0.2.4/src/physicsml/backends/backend_selector.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/src/physicsml/backends/openeye_backend.py` & `physicsml-0.2.4/src/physicsml/backends/openeye_backend.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/src/physicsml/backends/rdkit_backend.py` & `physicsml-0.2.4/src/physicsml/backends/rdkit_backend.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/src/physicsml/featurisation/physicsml_features/atom_features.py` & `physicsml-0.2.4/src/physicsml/featurisation/physicsml_features/atom_features.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/src/physicsml/featurisation/physicsml_features/bond_features.py` & `physicsml-0.2.4/src/physicsml/featurisation/physicsml_features/bond_features.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/src/physicsml/featurisation/physicsml_features/physicsml_features.py` & `physicsml-0.2.4/src/physicsml/featurisation/physicsml_features/physicsml_features.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/src/physicsml/lightning/config.py` & `physicsml-0.2.4/src/physicsml/lightning/config.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/src/physicsml/lightning/datamodule.py` & `physicsml-0.2.4/src/physicsml/lightning/datamodule.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/src/physicsml/lightning/graph_datasets/graph_dataset.py` & `physicsml-0.2.4/src/physicsml/lightning/graph_datasets/graph_dataset.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/src/physicsml/lightning/graph_datasets/neighbourhood_list_torch.py` & `physicsml-0.2.4/src/physicsml/lightning/graph_datasets/neighbourhood_list_torch.py`

 * *Files 4% similar despite different names*

```diff
@@ -59,27 +59,39 @@
     initial_edge_indices: Optional[torch.Tensor],
     initial_edge_attrs: Optional[torch.Tensor],
     pbc: Optional[Tuple[bool, bool, bool]],
     cell: Optional[torch.Tensor],
     self_interaction: bool,
 ) -> Tuple[torch.Tensor, Optional[torch.Tensor], torch.Tensor]:
     if (pbc is not None) and (cell is not None):
+        cell = cell.type(positions.dtype).to(positions.device)
+
+        # solve pos = coefs^T @ cell
+        # pos = pos - torch.floor(coefs) @ cell
+        coefs = torch.floor(torch.matmul(positions, torch.inverse(cell)))
+        wrapped_positions = positions - torch.matmul(coefs, cell)
+
         # find edge indices
         nbhd_edge_indices, _, nbhd_cell_shift_vector = compute_neighborlist(
             cutoff=cutoff,
-            pos=positions,
-            cell=cell.type(positions.dtype).to(positions.device),
+            pos=wrapped_positions,
+            cell=cell,
             pbc=torch.tensor(pbc).to(positions.device),
             batch=torch.zeros(
                 positions.shape[0],
                 dtype=torch.long,
                 device=positions.device,
             ),
             self_interaction=self_interaction,
         )
+
+        if nbhd_cell_shift_vector.numel() > 0:
+            nbhd_cell_shift_vector = nbhd_cell_shift_vector + (
+                coefs[nbhd_edge_indices[0]] - coefs[nbhd_edge_indices[1]]
+            )
     else:
         nbhd_edge_indices, nbhd_cell_shift_vector = compute_neighborlist_n2_no_cell(
             cutoff=cutoff,
             pos=positions,
             self_interaction=self_interaction,
         )
```

### Comparing `physicsml-0.2.3/src/physicsml/lightning/graph_datasets/torch_nl_vendored/geometry.py` & `physicsml-0.2.4/src/physicsml/lightning/graph_datasets/torch_nl_vendored/geometry.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/src/physicsml/lightning/graph_datasets/torch_nl_vendored/linked_cell.py` & `physicsml-0.2.4/src/physicsml/lightning/graph_datasets/torch_nl_vendored/linked_cell.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/src/physicsml/lightning/graph_datasets/torch_nl_vendored/naive_impl.py` & `physicsml-0.2.4/src/physicsml/lightning/graph_datasets/torch_nl_vendored/naive_impl.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/src/physicsml/lightning/graph_datasets/torch_nl_vendored/neighbor_list.py` & `physicsml-0.2.4/src/physicsml/lightning/graph_datasets/torch_nl_vendored/neighbor_list.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/src/physicsml/lightning/graph_datasets/torch_nl_vendored/timer.py` & `physicsml-0.2.4/src/physicsml/lightning/graph_datasets/torch_nl_vendored/timer.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/src/physicsml/lightning/graph_datasets/torch_nl_vendored/utils.py` & `physicsml-0.2.4/src/physicsml/lightning/graph_datasets/torch_nl_vendored/utils.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/src/physicsml/lightning/losses/barlow_twins_loss.py` & `physicsml-0.2.4/src/physicsml/lightning/losses/barlow_twins_loss.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/src/physicsml/lightning/losses/loss_base.py` & `physicsml-0.2.4/src/physicsml/lightning/losses/loss_base.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/src/physicsml/lightning/losses/masked_mse_loss.py` & `physicsml-0.2.4/src/physicsml/lightning/losses/masked_mse_loss.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/src/physicsml/lightning/losses/multitask_losses.py` & `physicsml-0.2.4/src/physicsml/lightning/losses/multitask_losses.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/src/physicsml/lightning/losses/serial_bce_w_logits_loss.py` & `physicsml-0.2.4/src/physicsml/lightning/losses/serial_bce_w_logits_loss.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/src/physicsml/lightning/losses/stock_losses.py` & `physicsml-0.2.4/src/physicsml/lightning/losses/stock_losses.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/src/physicsml/lightning/losses/weighted_mse_loss.py` & `physicsml-0.2.4/src/physicsml/lightning/losses/weighted_mse_loss.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/src/physicsml/lightning/model.py` & `physicsml-0.2.4/src/physicsml/lightning/model.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/src/physicsml/lightning/model_uncertainty.py` & `physicsml-0.2.4/src/physicsml/lightning/model_uncertainty.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/src/physicsml/lightning/module.py` & `physicsml-0.2.4/src/physicsml/lightning/module.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/src/physicsml/lightning/pre_batching_in_memory.py` & `physicsml-0.2.4/src/physicsml/lightning/pre_batching_in_memory.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/src/physicsml/lightning/pre_batching_on_disk.py` & `physicsml-0.2.4/src/physicsml/lightning/pre_batching_on_disk.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/src/physicsml/models/allegro/allegro_prism.py` & `physicsml-0.2.4/src/physicsml/models/allegro/allegro_prism.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/src/physicsml/models/allegro/mean_var/default_configs.py` & `physicsml-0.2.4/src/physicsml/models/allegro/mean_var/default_configs.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/src/physicsml/models/allegro/mean_var/mean_var_allegro_model.py` & `physicsml-0.2.4/src/physicsml/models/allegro/mean_var/mean_var_allegro_model.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/src/physicsml/models/allegro/mean_var/mean_var_allegro_module.py` & `physicsml-0.2.4/src/physicsml/models/allegro/mean_var/mean_var_allegro_module.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/src/physicsml/models/allegro/modules/allegro.py` & `physicsml-0.2.4/src/physicsml/models/allegro/modules/allegro.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/src/physicsml/models/allegro/modules/channels.py` & `physicsml-0.2.4/src/physicsml/models/allegro/modules/channels.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/src/physicsml/models/allegro/modules/contract.py` & `physicsml-0.2.4/src/physicsml/models/allegro/modules/contract.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/src/physicsml/models/allegro/modules/cutoffs.py` & `physicsml-0.2.4/src/physicsml/models/allegro/modules/cutoffs.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/src/physicsml/models/allegro/modules/fc.py` & `physicsml-0.2.4/src/physicsml/models/allegro/modules/fc.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/src/physicsml/models/allegro/modules/layout.py` & `physicsml-0.2.4/src/physicsml/models/allegro/modules/layout.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/src/physicsml/models/allegro/modules/linear.py` & `physicsml-0.2.4/src/physicsml/models/allegro/modules/linear.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/src/physicsml/models/allegro/modules/radial.py` & `physicsml-0.2.4/src/physicsml/models/allegro/modules/radial.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/src/physicsml/models/allegro/modules/spmm.py` & `physicsml-0.2.4/src/physicsml/models/allegro/modules/spmm.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/src/physicsml/models/allegro/supervised/allegro_model.py` & `physicsml-0.2.4/src/physicsml/models/allegro/supervised/allegro_model.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/src/physicsml/models/allegro/supervised/allegro_module.py` & `physicsml-0.2.4/src/physicsml/models/allegro/supervised/allegro_module.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/src/physicsml/models/allegro/supervised/default_configs.py` & `physicsml-0.2.4/src/physicsml/models/allegro/supervised/default_configs.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/src/physicsml/models/ani/ani_1_2_defaults.py` & `physicsml-0.2.4/src/physicsml/models/ani/ani_1_2_defaults.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/src/physicsml/models/ani/ani_datamodule.py` & `physicsml-0.2.4/src/physicsml/models/ani/ani_datamodule.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/src/physicsml/models/ani/ani_dataset.py` & `physicsml-0.2.4/src/physicsml/models/ani/ani_dataset.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/src/physicsml/models/ani/ani_prism.py` & `physicsml-0.2.4/src/physicsml/models/ani/ani_prism.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/src/physicsml/models/ani/config.py` & `physicsml-0.2.4/src/physicsml/models/ani/config.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/src/physicsml/models/ani/ensemble/default_configs.py` & `physicsml-0.2.4/src/physicsml/models/ani/ensemble/default_configs.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/src/physicsml/models/ani/ensemble/ensemble_ani_model.py` & `physicsml-0.2.4/src/physicsml/models/ani/ensemble/ensemble_ani_model.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/src/physicsml/models/ani/ensemble/ensemble_ani_module.py` & `physicsml-0.2.4/src/physicsml/models/ani/ensemble/ensemble_ani_module.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 from typing import Any, Dict, List, Optional
 
 import torch
 from molflux.modelzoo.models.lightning.module import (
     SingleBatchStepOutput,
 )
 from torchani import ANIModel
-from torchani.aev import AEVComputer
 
 from physicsml.lightning.losses.construct_loss import construct_loss
 from physicsml.lightning.module import PhysicsMLModuleBase
 from physicsml.models.ani.ani_1_2_defaults import (
     ani_1_2_aev_configs,
     ani_1_2_net_sizes_dict,
 )
 from physicsml.models.ani.ensemble.default_configs import EnsembleANIModelConfig
+from physicsml.models.ani.modules.aev import AEVComputer  # type: ignore
 
 
 def atomic_nets_to_module(net_sizes: Dict[str, Any]) -> Dict[str, torch.nn.Sequential]:
     atomic_nets = OrderedDict()
     for a in net_sizes.keys():
         layers = net_sizes[a]
         modules: List[Any] = []
```

### Comparing `physicsml-0.2.3/src/physicsml/models/ani/mean_var/default_configs.py` & `physicsml-0.2.4/src/physicsml/models/ani/mean_var/default_configs.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/src/physicsml/models/ani/mean_var/mean_var_ani_model.py` & `physicsml-0.2.4/src/physicsml/models/ani/mean_var/mean_var_ani_model.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/src/physicsml/models/ani/mean_var/mean_var_ani_module.py` & `physicsml-0.2.4/src/physicsml/models/ani/mean_var/mean_var_ani_module.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 from typing import Any, Dict, List, Optional
 
 import torch
 from molflux.modelzoo.models.lightning.module import (
     SingleBatchStepOutput,
 )
 from torchani import ANIModel
-from torchani.aev import AEVComputer
 
 from physicsml.lightning.losses.construct_loss import construct_loss
 from physicsml.lightning.module import PhysicsMLModuleBase
 from physicsml.models.ani.ani_1_2_defaults import (
     ani_1_2_aev_configs,
     ani_1_2_net_sizes_dict,
 )
 from physicsml.models.ani.mean_var.default_configs import MeanVarANIModelConfig
+from physicsml.models.ani.modules.aev import AEVComputer  # type: ignore
 
 
 def atomic_nets_to_module(net_sizes: Dict[str, Any]) -> Dict[str, torch.nn.Sequential]:
     atomic_nets = OrderedDict()
     for a in net_sizes.keys():
         layers = net_sizes[a]
         modules: List[Any] = []
```

### Comparing `physicsml-0.2.3/src/physicsml/models/ani/supervised/ani_model.py` & `physicsml-0.2.4/src/physicsml/models/ani/supervised/ani_model.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/src/physicsml/models/ani/supervised/ani_module.py` & `physicsml-0.2.4/src/physicsml/models/ani/supervised/ani_module.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 from typing import Any, Dict, List, Optional
 
 import torch
 from molflux.modelzoo.models.lightning.module import (
     SingleBatchStepOutput,
 )
 from torchani import ANIModel
-from torchani.aev import AEVComputer
 
 from physicsml.lightning.losses.construct_loss import construct_loss
 from physicsml.lightning.module import PhysicsMLModuleBase
 from physicsml.models.ani.ani_1_2_defaults import (
     ani_1_2_aev_configs,
     ani_1_2_net_sizes_dict,
 )
+from physicsml.models.ani.modules.aev import AEVComputer  # type: ignore
 from physicsml.models.ani.supervised.default_configs import ANIModelConfig
 
 
 class PooledANIModule(PhysicsMLModuleBase):
     """
     Class for pooled ani model
     """
```

### Comparing `physicsml-0.2.3/src/physicsml/models/ani/supervised/default_configs.py` & `physicsml-0.2.4/src/physicsml/models/ani/supervised/default_configs.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/src/physicsml/models/egnn/adapter/adapter_egnn_model.py` & `physicsml-0.2.4/src/physicsml/models/egnn/adapter/adapter_egnn_model.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/src/physicsml/models/egnn/adapter/adapter_egnn_module.py` & `physicsml-0.2.4/src/physicsml/models/egnn/adapter/adapter_egnn_module.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/src/physicsml/models/egnn/adapter/adapter_egnn_utils.py` & `physicsml-0.2.4/src/physicsml/models/egnn/adapter/adapter_egnn_utils.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/src/physicsml/models/egnn/adapter/default_configs.py` & `physicsml-0.2.4/src/physicsml/models/egnn/adapter/default_configs.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/src/physicsml/models/egnn/egnn_prism.py` & `physicsml-0.2.4/src/physicsml/models/egnn/egnn_prism.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/src/physicsml/models/egnn/egnn_utils.py` & `physicsml-0.2.4/src/physicsml/models/egnn/egnn_utils.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/src/physicsml/models/egnn/mean_var/default_configs.py` & `physicsml-0.2.4/src/physicsml/models/egnn/mean_var/default_configs.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/src/physicsml/models/egnn/mean_var/mean_var_egnn_model.py` & `physicsml-0.2.4/src/physicsml/models/egnn/mean_var/mean_var_egnn_model.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/src/physicsml/models/egnn/mean_var/mean_var_egnn_module.py` & `physicsml-0.2.4/src/physicsml/models/egnn/mean_var/mean_var_egnn_module.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/src/physicsml/models/egnn/ssf/default_configs.py` & `physicsml-0.2.4/src/physicsml/models/egnn/ssf/default_configs.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/src/physicsml/models/egnn/ssf/ssf_egnn_model.py` & `physicsml-0.2.4/src/physicsml/models/egnn/ssf/ssf_egnn_model.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/src/physicsml/models/egnn/ssf/ssf_egnn_module.py` & `physicsml-0.2.4/src/physicsml/models/egnn/ssf/ssf_egnn_module.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/src/physicsml/models/egnn/ssf/ssf_egnn_utils.py` & `physicsml-0.2.4/src/physicsml/models/egnn/ssf/ssf_egnn_utils.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/src/physicsml/models/egnn/supervised/default_configs.py` & `physicsml-0.2.4/src/physicsml/models/egnn/supervised/default_configs.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/src/physicsml/models/egnn/supervised/egnn_model.py` & `physicsml-0.2.4/src/physicsml/models/egnn/supervised/egnn_model.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/src/physicsml/models/egnn/supervised/egnn_module.py` & `physicsml-0.2.4/src/physicsml/models/egnn/supervised/egnn_module.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/src/physicsml/models/mace/adapter/adapter_mace_model.py` & `physicsml-0.2.4/src/physicsml/models/mace/adapter/adapter_mace_model.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/src/physicsml/models/mace/adapter/adapter_mace_module.py` & `physicsml-0.2.4/src/physicsml/models/mace/adapter/adapter_mace_module.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/src/physicsml/models/mace/adapter/adapter_mace_utils.py` & `physicsml-0.2.4/src/physicsml/models/mace/adapter/adapter_mace_utils.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/src/physicsml/models/mace/adapter/default_configs.py` & `physicsml-0.2.4/src/physicsml/models/mace/adapter/default_configs.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/src/physicsml/models/mace/mace_prism.py` & `physicsml-0.2.4/src/physicsml/models/mace/mace_prism.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/src/physicsml/models/mace/mean_var/default_configs.py` & `physicsml-0.2.4/src/physicsml/models/mace/mean_var/default_configs.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/src/physicsml/models/mace/mean_var/mean_var_mace_model.py` & `physicsml-0.2.4/src/physicsml/models/mace/mean_var/mean_var_mace_model.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/src/physicsml/models/mace/mean_var/mean_var_mace_module.py` & `physicsml-0.2.4/src/physicsml/models/mace/mean_var/mean_var_mace_module.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/src/physicsml/models/mace/modules/_activation.py` & `physicsml-0.2.4/src/physicsml/models/mace/modules/_activation.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/src/physicsml/models/mace/modules/blocks.py` & `physicsml-0.2.4/src/physicsml/models/mace/modules/blocks.py`

 * *Files 1% similar despite different names*

```diff
@@ -250,8 +250,9 @@
 
         if shift is not None:
             self.register_buffer("shift", torch.tensor(shift))
         else:
             self.register_buffer("shift", torch.tensor(0.0))
 
     def forward(self, x: torch.Tensor) -> torch.Tensor:
-        return self.scale * x + self.shift
+        scaled_shifted_x: torch.Tensor = self.scale * x + self.shift
+        return scaled_shifted_x
```

### Comparing `physicsml-0.2.3/src/physicsml/models/mace/modules/cg.py` & `physicsml-0.2.4/src/physicsml/models/mace/modules/cg.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/src/physicsml/models/mace/modules/irreps_tools.py` & `physicsml-0.2.4/src/physicsml/models/mace/modules/irreps_tools.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/src/physicsml/models/mace/modules/mace.py` & `physicsml-0.2.4/src/physicsml/models/mace/modules/mace.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/src/physicsml/models/mace/modules/radial.py` & `physicsml-0.2.4/src/physicsml/models/mace/modules/radial.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/src/physicsml/models/mace/modules/symmetric_contraction.py` & `physicsml-0.2.4/src/physicsml/models/mace/modules/symmetric_contraction.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/src/physicsml/models/mace/ssf/default_configs.py` & `physicsml-0.2.4/src/physicsml/models/mace/ssf/default_configs.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/src/physicsml/models/mace/ssf/ssf_mace_model.py` & `physicsml-0.2.4/src/physicsml/models/mace/ssf/ssf_mace_model.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/src/physicsml/models/mace/ssf/ssf_mace_module.py` & `physicsml-0.2.4/src/physicsml/models/mace/ssf/ssf_mace_module.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/src/physicsml/models/mace/ssf/ssf_mace_utils.py` & `physicsml-0.2.4/src/physicsml/models/mace/ssf/ssf_mace_utils.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/src/physicsml/models/mace/supervised/default_configs.py` & `physicsml-0.2.4/src/physicsml/models/mace/supervised/default_configs.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/src/physicsml/models/mace/supervised/mace_model.py` & `physicsml-0.2.4/src/physicsml/models/mace/supervised/mace_model.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/src/physicsml/models/mace/supervised/mace_module.py` & `physicsml-0.2.4/src/physicsml/models/mace/supervised/mace_module.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/src/physicsml/models/nequip/adapter/adapter_nequip_model.py` & `physicsml-0.2.4/src/physicsml/models/nequip/adapter/adapter_nequip_model.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/src/physicsml/models/nequip/adapter/adapter_nequip_module.py` & `physicsml-0.2.4/src/physicsml/models/nequip/adapter/adapter_nequip_module.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/src/physicsml/models/nequip/adapter/adapter_nequip_utils.py` & `physicsml-0.2.4/src/physicsml/models/nequip/adapter/adapter_nequip_utils.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/src/physicsml/models/nequip/adapter/default_configs.py` & `physicsml-0.2.4/src/physicsml/models/nequip/adapter/default_configs.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/src/physicsml/models/nequip/mean_var/default_configs.py` & `physicsml-0.2.4/src/physicsml/models/nequip/mean_var/default_configs.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/src/physicsml/models/nequip/mean_var/mean_var_nequip_model.py` & `physicsml-0.2.4/src/physicsml/models/nequip/mean_var/mean_var_nequip_model.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/src/physicsml/models/nequip/mean_var/mean_var_nequip_module.py` & `physicsml-0.2.4/src/physicsml/models/nequip/mean_var/mean_var_nequip_module.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/src/physicsml/models/nequip/modules/_activation.py` & `physicsml-0.2.4/src/physicsml/models/nequip/modules/_activation.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/src/physicsml/models/nequip/modules/_gate.py` & `physicsml-0.2.4/src/physicsml/models/nequip/modules/_gate.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/src/physicsml/models/nequip/modules/convnet_layer.py` & `physicsml-0.2.4/src/physicsml/models/nequip/modules/convnet_layer.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/src/physicsml/models/nequip/modules/interaction_block.py` & `physicsml-0.2.4/src/physicsml/models/nequip/modules/interaction_block.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/src/physicsml/models/nequip/modules/nequip.py` & `physicsml-0.2.4/src/physicsml/models/nequip/modules/nequip.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/src/physicsml/models/nequip/modules/radial.py` & `physicsml-0.2.4/src/physicsml/models/nequip/modules/radial.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/src/physicsml/models/nequip/modules/scale_shift.py` & `physicsml-0.2.4/src/physicsml/models/nequip/modules/scale_shift.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,8 +14,9 @@
 
         if shift is not None:
             self.register_buffer("shift", torch.tensor(shift))
         else:
             self.register_buffer("shift", torch.tensor(0.0))
 
     def forward(self, x: torch.Tensor) -> torch.Tensor:
-        return self.scale * x + self.shift
+        scaled_shifted_x: torch.Tensor = self.scale * x + self.shift
+        return scaled_shifted_x
```

### Comparing `physicsml-0.2.3/src/physicsml/models/nequip/nequip_prism.py` & `physicsml-0.2.4/src/physicsml/models/nequip/nequip_prism.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/src/physicsml/models/nequip/ssf/default_configs.py` & `physicsml-0.2.4/src/physicsml/models/nequip/ssf/default_configs.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/src/physicsml/models/nequip/ssf/ssf_nequip_model.py` & `physicsml-0.2.4/src/physicsml/models/nequip/ssf/ssf_nequip_model.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/src/physicsml/models/nequip/ssf/ssf_nequip_module.py` & `physicsml-0.2.4/src/physicsml/models/nequip/ssf/ssf_nequip_module.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/src/physicsml/models/nequip/ssf/ssf_nequip_utils.py` & `physicsml-0.2.4/src/physicsml/models/nequip/ssf/ssf_nequip_utils.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/src/physicsml/models/nequip/supervised/default_configs.py` & `physicsml-0.2.4/src/physicsml/models/nequip/supervised/default_configs.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/src/physicsml/models/nequip/supervised/nequip_model.py` & `physicsml-0.2.4/src/physicsml/models/nequip/supervised/nequip_model.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/src/physicsml/models/nequip/supervised/nequip_module.py` & `physicsml-0.2.4/src/physicsml/models/nequip/supervised/nequip_module.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/src/physicsml/models/prism.py` & `physicsml-0.2.4/src/physicsml/models/prism.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/src/physicsml/models/tensor_net/modules/embedding.py` & `physicsml-0.2.4/src/physicsml/models/tensor_net/modules/embedding.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,16 +23,15 @@
         mu_k = torch.linspace(float(torch.exp(-torch.tensor(cut_off))), 1.0, num_radial)
         beta_k = ((2 / num_radial) * (1 - torch.exp(-torch.tensor(cut_off)))) ** -2
 
         self.register_buffer("mu_k", mu_k.unsqueeze(0))
         self.register_buffer("beta_k", beta_k.unsqueeze(0))
 
     def forward(self, r_ji: torch.Tensor) -> torch.Tensor:
-        rbf = torch.exp(-self.beta_k * (torch.exp(-r_ji) - self.mu_k) ** 2)  # type: ignore
-
+        rbf = torch.exp(-self.beta_k * (torch.exp(-r_ji) - self.mu_k) ** 2)
         return rbf
 
 
 class MLP(torch.nn.Module):
     def __init__(
         self,
         c_in: int,
```

### Comparing `physicsml-0.2.3/src/physicsml/models/tensor_net/modules/interaction.py` & `physicsml-0.2.4/src/physicsml/models/tensor_net/modules/interaction.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/src/physicsml/models/tensor_net/modules/output.py` & `physicsml-0.2.4/src/physicsml/models/tensor_net/modules/output.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/src/physicsml/models/tensor_net/modules/utils.py` & `physicsml-0.2.4/src/physicsml/models/tensor_net/modules/utils.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/src/physicsml/models/tensor_net/supervised/default_configs.py` & `physicsml-0.2.4/src/physicsml/models/tensor_net/supervised/default_configs.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/src/physicsml/models/tensor_net/supervised/tensor_net_model.py` & `physicsml-0.2.4/src/physicsml/models/tensor_net/supervised/tensor_net_model.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/src/physicsml/models/tensor_net/supervised/tensor_net_module.py` & `physicsml-0.2.4/src/physicsml/models/tensor_net/supervised/tensor_net_module.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/src/physicsml/models/utils.py` & `physicsml-0.2.4/src/physicsml/models/utils.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/src/physicsml/plugins/ase/ase_ani.py` & `physicsml-0.2.4/src/physicsml/plugins/ase/ase_ani.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/src/physicsml/plugins/ase/ase_graph.py` & `physicsml-0.2.4/src/physicsml/plugins/ase/ase_graph.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/src/physicsml/plugins/ase/calculator.py` & `physicsml-0.2.4/src/physicsml/plugins/ase/calculator.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/src/physicsml/plugins/ase/load.py` & `physicsml-0.2.4/src/physicsml/plugins/ase/load.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/src/physicsml/plugins/openmm/load.py` & `physicsml-0.2.4/src/physicsml/plugins/openmm/load.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/src/physicsml/plugins/openmm/openmm_ani.py` & `physicsml-0.2.4/src/physicsml/plugins/openmm/openmm_ani.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/src/physicsml/plugins/openmm/openmm_base.py` & `physicsml-0.2.4/src/physicsml/plugins/openmm/openmm_base.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/src/physicsml/plugins/openmm/openmm_graph.py` & `physicsml-0.2.4/src/physicsml/plugins/openmm/openmm_graph.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/src/physicsml/plugins/openmm/physicsml_potential.py` & `physicsml-0.2.4/src/physicsml/plugins/openmm/physicsml_potential.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/src/physicsml/utils.py` & `physicsml-0.2.4/src/physicsml/utils.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/src/physicsml.egg-info/PKG-INFO` & `physicsml-0.2.4/src/physicsml.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: physicsml
-Version: 0.2.3
+Version: 0.2.4
 Summary: A package for all physics based/related models
 Author: Exscientia
 Maintainer: Exscientia
 Project-URL: documentation, https://github.com/exscientia/physicsml/issues
 Project-URL: repository, https://github.com/exscientia/physicsml.git
 Project-URL: issue-tracker, https://github.com/exscientia/physicsml/issues
 Project-URL: changelog, https://github.com/exscientia/physicsml/src/main/CHANGELOG.md
@@ -19,21 +19,19 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: molflux
-Requires-Dist: torch<2.1,>=2.0
+Requires-Dist: torch>=2.0
 Requires-Dist: lightning>=2.1
 Requires-Dist: torch-geometric>=2.5.0
-Requires-Dist: torch-nl
 Requires-Dist: e3nn
 Requires-Dist: torchani!=2.2.4
-Requires-Dist: tensorboard
 Provides-Extra: openeye
 Requires-Dist: openeye-toolkits<2023.0.0; python_version == "3.8" and extra == "openeye"
 Requires-Dist: openeye-toolkits; extra == "openeye"
 Provides-Extra: rdkit
 Requires-Dist: rdkit; extra == "rdkit"
 Provides-Extra: ase
 Requires-Dist: rdkit; extra == "ase"
```

### Comparing `physicsml-0.2.3/src/physicsml.egg-info/SOURCES.txt` & `physicsml-0.2.4/src/physicsml.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 CHANGELOG.md
 LICENSE
 README.md
 environment.yml
 init_conda_venv.sh
 init_python_venv.sh
 noxfile.py
-openmm_env.yaml
 pyproject.toml
 .github/workflows/dev-ci-actions.yaml
 .github/workflows/docs-build-deploy.yaml
 .github/workflows/latest-tests.yaml
 .github/workflows/main-ci-actions.yaml
 .github/workflows/pinned-tests.yaml
 .github/workflows/publish-package.yaml
@@ -156,14 +155,16 @@
 src/physicsml/models/ani/ensemble/default_configs.py
 src/physicsml/models/ani/ensemble/ensemble_ani_model.py
 src/physicsml/models/ani/ensemble/ensemble_ani_module.py
 src/physicsml/models/ani/mean_var/__init__.py
 src/physicsml/models/ani/mean_var/default_configs.py
 src/physicsml/models/ani/mean_var/mean_var_ani_model.py
 src/physicsml/models/ani/mean_var/mean_var_ani_module.py
+src/physicsml/models/ani/modules/__init__.py
+src/physicsml/models/ani/modules/aev.py
 src/physicsml/models/ani/supervised/__init__.py
 src/physicsml/models/ani/supervised/ani_model.py
 src/physicsml/models/ani/supervised/ani_module.py
 src/physicsml/models/ani/supervised/default_configs.py
 src/physicsml/models/egnn/__init__.py
 src/physicsml/models/egnn/egnn_prism.py
 src/physicsml/models/egnn/egnn_utils.py
```

### Comparing `physicsml-0.2.3/src/physicsml.egg-info/entry_points.txt` & `physicsml-0.2.4/src/physicsml.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/tests/ase/conftest.py` & `physicsml-0.2.4/tests/ase/conftest.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/tests/ase/test_ase_ani.py` & `physicsml-0.2.4/tests/ase/test_ase_ani.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/tests/ase/test_ase_graph.py` & `physicsml-0.2.4/tests/ase/test_ase_graph.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/tests/data/alanine-dipeptide-truncated.pdb` & `physicsml-0.2.4/tests/data/alanine-dipeptide-truncated.pdb`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/tests/data/ani1x.h5` & `physicsml-0.2.4/tests/data/ani1x.h5`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/tests/data/ani_model/featurisation_metadata.json` & `physicsml-0.2.4/tests/data/ani_model/featurisation_metadata.json`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/tests/data/ani_model/model_artefacts/module_checkpoint.ckpt` & `physicsml-0.2.4/tests/data/ani_model/model_artefacts/module_checkpoint.ckpt`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/tests/data/ani_model/model_config.json` & `physicsml-0.2.4/tests/data/ani_model/model_config.json`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/tests/data/egnn_model/featurisation_metadata.json` & `physicsml-0.2.4/tests/data/egnn_model/featurisation_metadata.json`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/tests/data/egnn_model/model_artefacts/module_checkpoint.ckpt` & `physicsml-0.2.4/tests/data/egnn_model/model_artefacts/module_checkpoint.ckpt`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/tests/data/egnn_model/model_config.json` & `physicsml-0.2.4/tests/data/egnn_model/model_config.json`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/tests/data/gdb9.csv` & `physicsml-0.2.4/tests/data/gdb9.csv`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/tests/data/gdb9.sdf` & `physicsml-0.2.4/tests/data/gdb9.sdf`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/tests/data/mace_model/featurisation_metadata.json` & `physicsml-0.2.4/tests/data/mace_model/featurisation_metadata.json`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/tests/data/mace_model/model_artefacts/module_checkpoint.ckpt` & `physicsml-0.2.4/tests/data/mace_model/model_artefacts/module_checkpoint.ckpt`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/tests/data/mace_model/model_config.json` & `physicsml-0.2.4/tests/data/mace_model/model_config.json`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/tests/data/nequip_model/featurisation_metadata.json` & `physicsml-0.2.4/tests/data/nequip_model/featurisation_metadata.json`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/tests/data/nequip_model/model_artefacts/module_checkpoint.ckpt` & `physicsml-0.2.4/tests/data/nequip_model/model_artefacts/module_checkpoint.ckpt`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/tests/data/nequip_model/model_config.json` & `physicsml-0.2.4/tests/data/nequip_model/model_config.json`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/tests/openeye/conftest.py` & `physicsml-0.2.4/tests/openeye/conftest.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/tests/openeye/core/data/test_datamodule.py` & `physicsml-0.2.4/tests/openeye/core/data/test_datamodule.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/tests/openeye/core/data/test_graph_dataset.py` & `physicsml-0.2.4/tests/openeye/core/data/test_graph_dataset.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/tests/openeye/core/featurisation/test_physicsml_featurisation.py` & `physicsml-0.2.4/tests/openeye/core/featurisation/test_physicsml_featurisation.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/tests/openeye/integration/prism/test_egnn_prism.py` & `physicsml-0.2.4/tests/openeye/integration/prism/test_egnn_prism.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/tests/openeye/integration/training/egnn/test_egnn.py` & `physicsml-0.2.4/tests/openeye/integration/training/egnn/test_egnn.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/tests/openmm/conftest.py` & `physicsml-0.2.4/tests/openmm/conftest.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/tests/openmm/test_openmm_ani.py` & `physicsml-0.2.4/tests/openmm/test_openmm_ani.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/tests/openmm/test_openmm_egnn.py` & `physicsml-0.2.4/tests/openmm/test_openmm_egnn.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/tests/openmm/test_openmm_mace.py` & `physicsml-0.2.4/tests/openmm/test_openmm_mace.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/tests/openmm/test_openmm_nequip.py` & `physicsml-0.2.4/tests/openmm/test_openmm_nequip.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/tests/openmm/test_openmm_nnp_potential.py` & `physicsml-0.2.4/tests/openmm/test_openmm_nnp_potential.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/tests/rdkit/conftest.py` & `physicsml-0.2.4/tests/rdkit/conftest.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/tests/rdkit/core/data/test_datamodule.py` & `physicsml-0.2.4/tests/rdkit/core/data/test_datamodule.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/tests/rdkit/core/data/test_graph_dataset.py` & `physicsml-0.2.4/tests/rdkit/core/data/test_graph_dataset.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/tests/rdkit/core/featurisation/test_physicsml_featurisation.py` & `physicsml-0.2.4/tests/rdkit/core/featurisation/test_physicsml_featurisation.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/tests/rdkit/integration/prism/test_allegro_prism.py` & `physicsml-0.2.4/tests/rdkit/integration/prism/test_allegro_prism.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/tests/rdkit/integration/prism/test_ani_prism.py` & `physicsml-0.2.4/tests/rdkit/integration/prism/test_ani_prism.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/tests/rdkit/integration/prism/test_egnn_prism.py` & `physicsml-0.2.4/tests/rdkit/integration/prism/test_egnn_prism.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/tests/rdkit/integration/prism/test_mace_prism.py` & `physicsml-0.2.4/tests/rdkit/integration/prism/test_mace_prism.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/tests/rdkit/integration/prism/test_nequip_prism.py` & `physicsml-0.2.4/tests/rdkit/integration/prism/test_nequip_prism.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/tests/rdkit/integration/training/allegro/test_allegro_energy_charges.py` & `physicsml-0.2.4/tests/rdkit/integration/training/allegro/test_allegro_energy_charges.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/tests/rdkit/integration/training/allegro/test_allegro_forces.py` & `physicsml-0.2.4/tests/rdkit/integration/training/allegro/test_allegro_forces.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/tests/rdkit/integration/training/allegro/test_allegro_mean_var.py` & `physicsml-0.2.4/tests/rdkit/integration/training/allegro/test_allegro_mean_var.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/tests/rdkit/integration/training/allegro/test_allergo.py` & `physicsml-0.2.4/tests/rdkit/integration/training/allegro/test_allergo.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/tests/rdkit/integration/training/ani/test_ani.py` & `physicsml-0.2.4/tests/rdkit/integration/training/ani/test_ani.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/tests/rdkit/integration/training/ani/test_ani_ensemble.py` & `physicsml-0.2.4/tests/rdkit/integration/training/ani/test_ani_ensemble.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/tests/rdkit/integration/training/ani/test_ani_forces.py` & `physicsml-0.2.4/tests/rdkit/integration/training/ani/test_ani_forces.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/tests/rdkit/integration/training/ani/test_ani_mean_var.py` & `physicsml-0.2.4/tests/rdkit/integration/training/ani/test_ani_mean_var.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/tests/rdkit/integration/training/egnn/test_adapter_egnn.py` & `physicsml-0.2.4/tests/rdkit/integration/training/egnn/test_adapter_egnn.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/tests/rdkit/integration/training/egnn/test_egnn.py` & `physicsml-0.2.4/tests/rdkit/integration/training/egnn/test_egnn.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/tests/rdkit/integration/training/egnn/test_egnn_energy_charges.py` & `physicsml-0.2.4/tests/rdkit/integration/training/egnn/test_egnn_energy_charges.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/tests/rdkit/integration/training/egnn/test_egnn_forces.py` & `physicsml-0.2.4/tests/rdkit/integration/training/egnn/test_egnn_forces.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/tests/rdkit/integration/training/egnn/test_egnn_mean_var.py` & `physicsml-0.2.4/tests/rdkit/integration/training/egnn/test_egnn_mean_var.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/tests/rdkit/integration/training/egnn/test_ssf_egnn.py` & `physicsml-0.2.4/tests/rdkit/integration/training/egnn/test_ssf_egnn.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/tests/rdkit/integration/training/mace/test_adapter_mace.py` & `physicsml-0.2.4/tests/rdkit/integration/training/mace/test_adapter_mace.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/tests/rdkit/integration/training/mace/test_mace.py` & `physicsml-0.2.4/tests/rdkit/integration/training/mace/test_mace.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/tests/rdkit/integration/training/mace/test_mace_energy_charges.py` & `physicsml-0.2.4/tests/rdkit/integration/training/mace/test_mace_energy_charges.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/tests/rdkit/integration/training/mace/test_mace_forces.py` & `physicsml-0.2.4/tests/rdkit/integration/training/mace/test_mace_forces.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/tests/rdkit/integration/training/mace/test_mace_mean_var.py` & `physicsml-0.2.4/tests/rdkit/integration/training/mace/test_mace_mean_var.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/tests/rdkit/integration/training/mace/test_ssf_mace.py` & `physicsml-0.2.4/tests/rdkit/integration/training/mace/test_ssf_mace.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/tests/rdkit/integration/training/nequip/test_adapter_nequip.py` & `physicsml-0.2.4/tests/rdkit/integration/training/nequip/test_adapter_nequip.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/tests/rdkit/integration/training/nequip/test_nequip.py` & `physicsml-0.2.4/tests/rdkit/integration/training/nequip/test_nequip.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/tests/rdkit/integration/training/nequip/test_nequip_energy_charges.py` & `physicsml-0.2.4/tests/rdkit/integration/training/nequip/test_nequip_energy_charges.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/tests/rdkit/integration/training/nequip/test_nequip_forces.py` & `physicsml-0.2.4/tests/rdkit/integration/training/nequip/test_nequip_forces.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/tests/rdkit/integration/training/nequip/test_nequip_mean_var.py` & `physicsml-0.2.4/tests/rdkit/integration/training/nequip/test_nequip_mean_var.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/tests/rdkit/integration/training/nequip/test_ssf_nequip.py` & `physicsml-0.2.4/tests/rdkit/integration/training/nequip/test_ssf_nequip.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/tests/rdkit/integration/training/tensor_net/test_tensor_net.py` & `physicsml-0.2.4/tests/rdkit/integration/training/tensor_net/test_tensor_net.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/tests/rdkit/integration/training/tensor_net/test_tensor_net_energy_charges.py` & `physicsml-0.2.4/tests/rdkit/integration/training/tensor_net/test_tensor_net_energy_charges.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.3/tests/rdkit/integration/training/tensor_net/test_tensor_net_forces.py` & `physicsml-0.2.4/tests/rdkit/integration/training/tensor_net/test_tensor_net_forces.py`

 * *Files identical despite different names*


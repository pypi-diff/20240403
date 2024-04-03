# Comparing `tmp/physicsml-0.2.0.tar.gz` & `tmp/physicsml-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "physicsml-0.2.0.tar", last modified: Thu Mar  7 14:58:49 2024, max compression
+gzip compressed data, was "physicsml-0.2.1.tar", last modified: Wed Apr  3 15:53:14 2024, max compression
```

## Comparing `physicsml-0.2.0.tar` & `physicsml-0.2.1.tar`

### file list

```diff
@@ -1,446 +1,454 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:49.683005 physicsml-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-03-07 14:58:04.000000 physicsml-0.2.0/.envrc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:49.611005 physicsml-0.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:49.623005 physicsml-0.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-03-07 14:58:04.000000 physicsml-0.2.0/.github/workflows/dev-ci-actions.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      884 2024-03-07 14:58:04.000000 physicsml-0.2.0/.github/workflows/docs-build-deploy.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-03-07 14:58:04.000000 physicsml-0.2.0/.github/workflows/latest-tests.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-03-07 14:58:04.000000 physicsml-0.2.0/.github/workflows/main-ci-actions.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-03-07 14:58:04.000000 physicsml-0.2.0/.github/workflows/pinned-tests.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-03-07 14:58:04.000000 physicsml-0.2.0/.github/workflows/publish-package.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-03-07 14:58:04.000000 physicsml-0.2.0/.github/workflows/quality-typing-checks.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-03-07 14:58:04.000000 physicsml-0.2.0/.github/workflows/release-ci-actions.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-03-07 14:58:04.000000 physicsml-0.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-03-07 14:58:04.000000 physicsml-0.2.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-03-07 14:58:04.000000 physicsml-0.2.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-03-07 14:58:04.000000 physicsml-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4650 2024-03-07 14:58:49.683005 physicsml-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-03-07 14:58:04.000000 physicsml-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:49.623005 physicsml-0.2.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-03-07 14:58:04.000000 physicsml-0.2.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-03-07 14:58:04.000000 physicsml-0.2.0/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:49.623005 physicsml-0.2.0/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:49.627005 physicsml-0.2.0/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     3348 2024-03-07 14:58:04.000000 physicsml-0.2.0/docs/source/_static/PhysicsML_Logo-01.svg
--rw-r--r--   0 runner    (1001) docker     (127)     7381 2024-03-07 14:58:04.000000 physicsml-0.2.0/docs/source/_static/PhysicsML_Logo_PhyML_logo full dark-cropped.svg
--rw-r--r--   0 runner    (1001) docker     (127)     7503 2024-03-07 14:58:04.000000 physicsml-0.2.0/docs/source/_static/PhysicsML_Logo_PhyML_logo full dark.svg
--rw-r--r--   0 runner    (1001) docker     (127)     7380 2024-03-07 14:58:04.000000 physicsml-0.2.0/docs/source/_static/PhysicsML_Logo_PhyML_logo full light-cropped.svg
--rw-r--r--   0 runner    (1001) docker     (127)     7502 2024-03-07 14:58:04.000000 physicsml-0.2.0/docs/source/_static/PhysicsML_Logo_PhyML_logo full light.svg
--rw-r--r--   0 runner    (1001) docker     (127)     7824 2024-03-07 14:58:04.000000 physicsml-0.2.0/docs/source/_static/PhysicsML_Logo_PhyML_logo text dark.svg
--rw-r--r--   0 runner    (1001) docker     (127)     7836 2024-03-07 14:58:04.000000 physicsml-0.2.0/docs/source/_static/PhysicsML_Logo_PhyML_logo text light.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-03-07 14:58:04.000000 physicsml-0.2.0/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-03-07 14:58:04.000000 physicsml-0.2.0/docs/source/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:49.615005 physicsml-0.2.0/docs/source/pages/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:49.627005 physicsml-0.2.0/docs/source/pages/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)     5631 2024-03-07 14:58:04.000000 physicsml-0.2.0/docs/source/pages/datasets/qm_datasets.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:49.627005 physicsml-0.2.0/docs/source/pages/features/
--rw-r--r--   0 runner    (1001) docker     (127)   489710 2024-03-07 14:58:04.000000 physicsml-0.2.0/docs/source/pages/features/gdb9_trunc.parquet
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-03-07 14:58:04.000000 physicsml-0.2.0/docs/source/pages/features/how_to_add_reps.md
--rw-r--r--   0 runner    (1001) docker     (127)     9303 2024-03-07 14:58:04.000000 physicsml-0.2.0/docs/source/pages/features/intro.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:49.627005 physicsml-0.2.0/docs/source/pages/models/
--rw-r--r--   0 runner    (1001) docker     (127)     4886 2024-03-07 14:58:04.000000 physicsml-0.2.0/docs/source/pages/models/allegro.md
--rw-r--r--   0 runner    (1001) docker     (127)     3349 2024-03-07 14:58:04.000000 physicsml-0.2.0/docs/source/pages/models/ani.md
--rw-r--r--   0 runner    (1001) docker     (127)    10655 2024-03-07 14:58:04.000000 physicsml-0.2.0/docs/source/pages/models/egnn.md
--rw-r--r--   0 runner    (1001) docker     (127)     6295 2024-03-07 14:58:04.000000 physicsml-0.2.0/docs/source/pages/models/how_to_add_models.md
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-03-07 14:58:04.000000 physicsml-0.2.0/docs/source/pages/models/intro.md
--rw-r--r--   0 runner    (1001) docker     (127)     8347 2024-03-07 14:58:04.000000 physicsml-0.2.0/docs/source/pages/models/mace.md
--rw-r--r--   0 runner    (1001) docker     (127)     8998 2024-03-07 14:58:04.000000 physicsml-0.2.0/docs/source/pages/models/nequip.md
--rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-03-07 14:58:04.000000 physicsml-0.2.0/docs/source/pages/models/tensor_net.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:49.627005 physicsml-0.2.0/docs/source/pages/philosophy/
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-03-07 14:58:04.000000 physicsml-0.2.0/docs/source/pages/philosophy/molflux.md
--rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-03-07 14:58:04.000000 physicsml-0.2.0/docs/source/pages/philosophy/philosophy.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:49.627005 physicsml-0.2.0/docs/source/pages/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-03-07 14:58:04.000000 physicsml-0.2.0/docs/source/pages/plugins/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     4578 2024-03-07 14:58:04.000000 physicsml-0.2.0/docs/source/pages/plugins/alanine-dipeptide-truncated.pdb
--rw-r--r--   0 runner    (1001) docker     (127)     3899 2024-03-07 14:58:04.000000 physicsml-0.2.0/docs/source/pages/plugins/ase.md
--rw-r--r--   0 runner    (1001) docker     (127)     5335 2024-03-07 14:58:04.000000 physicsml-0.2.0/docs/source/pages/plugins/openmm.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:49.631005 physicsml-0.2.0/docs/source/pages/structure/
--rw-r--r--   0 runner    (1001) docker     (127)     7237 2024-03-07 14:58:04.000000 physicsml-0.2.0/docs/source/pages/structure/lightning_layer.md
--rw-r--r--   0 runner    (1001) docker     (127)     4803 2024-03-07 14:58:04.000000 physicsml-0.2.0/docs/source/pages/structure/molflux_layer.md
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-03-07 14:58:04.000000 physicsml-0.2.0/docs/source/pages/structure/physicsml_structure.md
--rw-r--r--   0 runner    (1001) docker     (127)     6294 2024-03-07 14:58:04.000000 physicsml-0.2.0/docs/source/pages/structure/torch_layer.md
--rw-r--r--   0 runner    (1001) docker     (127)     2906 2024-03-07 14:58:04.000000 physicsml-0.2.0/docs/source/pages/structure/transfer_learning.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:49.635005 physicsml-0.2.0/docs/source/pages/tutorials/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-07 14:58:04.000000 physicsml-0.2.0/docs/source/pages/tutorials/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     7462 2024-03-07 14:58:04.000000 physicsml-0.2.0/docs/source/pages/tutorials/ani1x_energy_forces_training.md
--rw-r--r--   0 runner    (1001) docker     (127)  1610932 2024-03-07 14:58:04.000000 physicsml-0.2.0/docs/source/pages/tutorials/ani1x_truncated.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     9729 2024-03-07 14:58:04.000000 physicsml-0.2.0/docs/source/pages/tutorials/gdb9_training.md
--rw-r--r--   0 runner    (1001) docker     (127)   489710 2024-03-07 14:58:04.000000 physicsml-0.2.0/docs/source/pages/tutorials/gdb9_trunc.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     7678 2024-03-07 14:58:04.000000 physicsml-0.2.0/docs/source/pages/tutorials/gdb9_uncertainty.md
--rw-r--r--   0 runner    (1001) docker     (127)    10605 2024-03-07 14:58:04.000000 physicsml-0.2.0/docs/source/pages/tutorials/transfer_learning.md
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-03-07 14:58:04.000000 physicsml-0.2.0/environment.yml
--rwxr-xr-x   0 runner    (1001) docker     (127)     1053 2024-03-07 14:58:04.000000 physicsml-0.2.0/init_conda_venv.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      714 2024-03-07 14:58:04.000000 physicsml-0.2.0/init_python_venv.sh
--rw-r--r--   0 runner    (1001) docker     (127)    12413 2024-03-07 14:58:04.000000 physicsml-0.2.0/noxfile.py
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-03-07 14:58:04.000000 physicsml-0.2.0/openmm_env.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:49.615005 physicsml-0.2.0/pinned-versions/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:49.635005 physicsml-0.2.0/pinned-versions/3.10/
--rw-r--r--   0 runner    (1001) docker     (127)    12169 2024-03-07 14:58:04.000000 physicsml-0.2.0/pinned-versions/3.10/lockfile.ase.txt
--rw-r--r--   0 runner    (1001) docker     (127)    12168 2024-03-07 14:58:04.000000 physicsml-0.2.0/pinned-versions/3.10/lockfile.core.txt
--rw-r--r--   0 runner    (1001) docker     (127)    12237 2024-03-07 14:58:04.000000 physicsml-0.2.0/pinned-versions/3.10/lockfile.openeye.txt
--rw-r--r--   0 runner    (1001) docker     (127)    12172 2024-03-07 14:58:04.000000 physicsml-0.2.0/pinned-versions/3.10/lockfile.openmm.txt
--rw-r--r--   0 runner    (1001) docker     (127)    12171 2024-03-07 14:58:04.000000 physicsml-0.2.0/pinned-versions/3.10/lockfile.rdkit.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:49.635005 physicsml-0.2.0/pinned-versions/3.11/
--rw-r--r--   0 runner    (1001) docker     (127)    11991 2024-03-07 14:58:04.000000 physicsml-0.2.0/pinned-versions/3.11/lockfile.ase.txt
--rw-r--r--   0 runner    (1001) docker     (127)    11990 2024-03-07 14:58:04.000000 physicsml-0.2.0/pinned-versions/3.11/lockfile.core.txt
--rw-r--r--   0 runner    (1001) docker     (127)    12059 2024-03-07 14:58:04.000000 physicsml-0.2.0/pinned-versions/3.11/lockfile.openeye.txt
--rw-r--r--   0 runner    (1001) docker     (127)    11994 2024-03-07 14:58:04.000000 physicsml-0.2.0/pinned-versions/3.11/lockfile.openmm.txt
--rw-r--r--   0 runner    (1001) docker     (127)    11993 2024-03-07 14:58:04.000000 physicsml-0.2.0/pinned-versions/3.11/lockfile.rdkit.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:49.635005 physicsml-0.2.0/pinned-versions/3.8/
--rw-r--r--   0 runner    (1001) docker     (127)    13023 2024-03-07 14:58:04.000000 physicsml-0.2.0/pinned-versions/3.8/lockfile.ase.txt
--rw-r--r--   0 runner    (1001) docker     (127)    13022 2024-03-07 14:58:04.000000 physicsml-0.2.0/pinned-versions/3.8/lockfile.core.txt
--rw-r--r--   0 runner    (1001) docker     (127)    13193 2024-03-07 14:58:04.000000 physicsml-0.2.0/pinned-versions/3.8/lockfile.openeye.txt
--rw-r--r--   0 runner    (1001) docker     (127)    13026 2024-03-07 14:58:04.000000 physicsml-0.2.0/pinned-versions/3.8/lockfile.openmm.txt
--rw-r--r--   0 runner    (1001) docker     (127)    13025 2024-03-07 14:58:04.000000 physicsml-0.2.0/pinned-versions/3.8/lockfile.rdkit.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:49.635005 physicsml-0.2.0/pinned-versions/3.9/
--rw-r--r--   0 runner    (1001) docker     (127)    12324 2024-03-07 14:58:04.000000 physicsml-0.2.0/pinned-versions/3.9/lockfile.ase.txt
--rw-r--r--   0 runner    (1001) docker     (127)    12323 2024-03-07 14:58:04.000000 physicsml-0.2.0/pinned-versions/3.9/lockfile.core.txt
--rw-r--r--   0 runner    (1001) docker     (127)    12392 2024-03-07 14:58:04.000000 physicsml-0.2.0/pinned-versions/3.9/lockfile.openeye.txt
--rw-r--r--   0 runner    (1001) docker     (127)    12327 2024-03-07 14:58:04.000000 physicsml-0.2.0/pinned-versions/3.9/lockfile.openmm.txt
--rw-r--r--   0 runner    (1001) docker     (127)    12326 2024-03-07 14:58:04.000000 physicsml-0.2.0/pinned-versions/3.9/lockfile.rdkit.txt
--rw-r--r--   0 runner    (1001) docker     (127)     7393 2024-03-07 14:58:04.000000 physicsml-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-07 14:58:49.683005 physicsml-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:49.615005 physicsml-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:49.635005 physicsml-0.2.0/src/physicsml/
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:49.639005 physicsml-0.2.0/src/physicsml/backends/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2286 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/backends/backend_selector.py
--rw-r--r--   0 runner    (1001) docker     (127)     4970 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/backends/openeye_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     4927 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/backends/rdkit_backend.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:49.639005 physicsml-0.2.0/src/physicsml/featurisation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/featurisation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:49.639005 physicsml-0.2.0/src/physicsml/featurisation/physicsml_features/
--rw-r--r--   0 runner    (1001) docker     (127)     4246 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/featurisation/physicsml_features/atom_features.py
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/featurisation/physicsml_features/bond_features.py
--rw-r--r--   0 runner    (1001) docker     (127)     5600 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/featurisation/physicsml_features/physicsml_features.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:49.639005 physicsml-0.2.0/src/physicsml/lightning/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/lightning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3569 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/lightning/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5705 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/lightning/datamodule.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:49.639005 physicsml-0.2.0/src/physicsml/lightning/graph_datasets/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/lightning/graph_datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13126 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/lightning/graph_datasets/graph_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     5515 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/lightning/graph_datasets/neighbourhood_list_torch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:49.643005 physicsml-0.2.0/src/physicsml/lightning/losses/
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/lightning/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10118 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/lightning/losses/barlow_twins_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/lightning/losses/construct_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/lightning/losses/loss_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/lightning/losses/masked_mse_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/lightning/losses/multitask_losses.py
--rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/lightning/losses/serial_bce_w_logits_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)      982 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/lightning/losses/stock_losses.py
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/lightning/losses/weighted_mse_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     4642 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/lightning/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6462 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/lightning/model_uncertainty.py
--rw-r--r--   0 runner    (1001) docker     (127)     6630 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/lightning/module.py
--rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/lightning/pre_batching_in_memory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/lightning/pre_batching_on_disk.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:49.643005 physicsml-0.2.0/src/physicsml/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:49.643005 physicsml-0.2.0/src/physicsml/models/allegro/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/models/allegro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4108 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/models/allegro/allegro_prism.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:49.643005 physicsml-0.2.0/src/physicsml/models/allegro/mean_var/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/models/allegro/mean_var/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/models/allegro/mean_var/default_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/models/allegro/mean_var/mean_var_allegro_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6496 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/models/allegro/mean_var/mean_var_allegro_module.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:49.643005 physicsml-0.2.0/src/physicsml/models/allegro/modules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/models/allegro/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24182 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/models/allegro/modules/allegro.py
--rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/models/allegro/modules/channels.py
--rw-r--r--   0 runner    (1001) docker     (127)    15463 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/models/allegro/modules/contract.py
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/models/allegro/modules/cutoffs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5427 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/models/allegro/modules/fc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2759 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/models/allegro/modules/layout.py
--rw-r--r--   0 runner    (1001) docker     (127)     8447 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/models/allegro/modules/linear.py
--rw-r--r--   0 runner    (1001) docker     (127)     3696 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/models/allegro/modules/radial.py
--rw-r--r--   0 runner    (1001) docker     (127)     5406 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/models/allegro/modules/spmm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:49.647005 physicsml-0.2.0/src/physicsml/models/allegro/supervised/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/models/allegro/supervised/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/models/allegro/supervised/allegro_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5639 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/models/allegro/supervised/allegro_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/models/allegro/supervised/default_configs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:49.647005 physicsml-0.2.0/src/physicsml/models/ani/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/models/ani/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4619 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/models/ani/ani_1_2_defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     5150 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/models/ani/ani_datamodule.py
--rw-r--r--   0 runner    (1001) docker     (127)     5859 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/models/ani/ani_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2826 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/models/ani/ani_prism.py
--rw-r--r--   0 runner    (1001) docker     (127)     2688 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/models/ani/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:49.647005 physicsml-0.2.0/src/physicsml/models/ani/ensemble/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/models/ani/ensemble/default_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/models/ani/ensemble/ensemble_ani_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     9754 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/models/ani/ensemble/ensemble_ani_module.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:49.647005 physicsml-0.2.0/src/physicsml/models/ani/mean_var/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/models/ani/mean_var/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/models/ani/mean_var/default_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/models/ani/mean_var/mean_var_ani_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     8955 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/models/ani/mean_var/mean_var_ani_module.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:49.647005 physicsml-0.2.0/src/physicsml/models/ani/supervised/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/models/ani/supervised/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/models/ani/supervised/ani_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     8395 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/models/ani/supervised/ani_module.py
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/models/ani/supervised/default_configs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:49.647005 physicsml-0.2.0/src/physicsml/models/egnn/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/models/egnn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:49.647005 physicsml-0.2.0/src/physicsml/models/egnn/adapter/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/models/egnn/adapter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/models/egnn/adapter/adapter_egnn_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6317 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/models/egnn/adapter/adapter_egnn_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     6599 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/models/egnn/adapter/adapter_egnn_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/models/egnn/adapter/default_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4251 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/models/egnn/egnn_prism.py
--rw-r--r--   0 runner    (1001) docker     (127)    15452 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/models/egnn/egnn_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:49.651005 physicsml-0.2.0/src/physicsml/models/egnn/mean_var/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/models/egnn/mean_var/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/models/egnn/mean_var/default_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/models/egnn/mean_var/mean_var_egnn_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6987 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/models/egnn/mean_var/mean_var_egnn_module.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:49.651005 physicsml-0.2.0/src/physicsml/models/egnn/ssf/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/models/egnn/ssf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/models/egnn/ssf/default_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/models/egnn/ssf/ssf_egnn_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6159 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/models/egnn/ssf/ssf_egnn_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     3689 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/models/egnn/ssf/ssf_egnn_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:49.651005 physicsml-0.2.0/src/physicsml/models/egnn/supervised/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/models/egnn/supervised/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/models/egnn/supervised/default_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/models/egnn/supervised/egnn_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6308 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/models/egnn/supervised/egnn_module.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:49.651005 physicsml-0.2.0/src/physicsml/models/mace/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/models/mace/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:49.651005 physicsml-0.2.0/src/physicsml/models/mace/adapter/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/models/mace/adapter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/models/mace/adapter/adapter_mace_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     8422 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/models/mace/adapter/adapter_mace_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     8480 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/models/mace/adapter/adapter_mace_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/models/mace/adapter/default_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4194 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/models/mace/mace_prism.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:49.651005 physicsml-0.2.0/src/physicsml/models/mace/mean_var/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/models/mace/mean_var/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/models/mace/mean_var/default_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/models/mace/mean_var/mean_var_mace_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     8887 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/models/mace/mean_var/mean_var_mace_module.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:49.655005 physicsml-0.2.0/src/physicsml/models/mace/modules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/models/mace/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3773 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/models/mace/modules/_activation.py
--rw-r--r--   0 runner    (1001) docker     (127)     8197 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/models/mace/modules/blocks.py
--rw-r--r--   0 runner    (1001) docker     (127)     4377 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/models/mace/modules/cg.py
--rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/models/mace/modules/irreps_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     8507 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/models/mace/modules/mace.py
--rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/models/mace/modules/radial.py
--rw-r--r--   0 runner    (1001) docker     (127)     9635 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/models/mace/modules/symmetric_contraction.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:49.655005 physicsml-0.2.0/src/physicsml/models/mace/ssf/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/models/mace/ssf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/models/mace/ssf/default_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/models/mace/ssf/ssf_mace_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     8236 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/models/mace/ssf/ssf_mace_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     6820 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/models/mace/ssf/ssf_mace_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:49.655005 physicsml-0.2.0/src/physicsml/models/mace/supervised/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/models/mace/supervised/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/models/mace/supervised/default_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/models/mace/supervised/mace_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     8133 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/models/mace/supervised/mace_module.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:49.655005 physicsml-0.2.0/src/physicsml/models/nequip/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/models/nequip/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:49.655005 physicsml-0.2.0/src/physicsml/models/nequip/adapter/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/models/nequip/adapter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/models/nequip/adapter/adapter_nequip_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6696 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/models/nequip/adapter/adapter_nequip_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     7075 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/models/nequip/adapter/adapter_nequip_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/models/nequip/adapter/default_configs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:49.655005 physicsml-0.2.0/src/physicsml/models/nequip/mean_var/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/models/nequip/mean_var/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/models/nequip/mean_var/default_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/models/nequip/mean_var/mean_var_nequip_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     7196 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/models/nequip/mean_var/mean_var_nequip_module.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:49.659005 physicsml-0.2.0/src/physicsml/models/nequip/modules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/models/nequip/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3773 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/models/nequip/modules/_activation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5727 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/models/nequip/modules/_gate.py
--rw-r--r--   0 runner    (1001) docker     (127)     3466 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/models/nequip/modules/convnet_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3683 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/models/nequip/modules/interaction_block.py
--rw-r--r--   0 runner    (1001) docker     (127)     5968 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/models/nequip/modules/nequip.py
--rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/models/nequip/modules/radial.py
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/models/nequip/modules/scale_shift.py
--rw-r--r--   0 runner    (1001) docker     (127)     4494 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/models/nequip/nequip_prism.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:49.659005 physicsml-0.2.0/src/physicsml/models/nequip/ssf/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/models/nequip/ssf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/models/nequip/ssf/default_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/models/nequip/ssf/ssf_nequip_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6522 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/models/nequip/ssf/ssf_nequip_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     5306 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/models/nequip/ssf/ssf_nequip_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:49.659005 physicsml-0.2.0/src/physicsml/models/nequip/supervised/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/models/nequip/supervised/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/models/nequip/supervised/default_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/models/nequip/supervised/nequip_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6431 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/models/nequip/supervised/nequip_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     4990 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/models/prism.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:49.659005 physicsml-0.2.0/src/physicsml/models/tensor_net/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/models/tensor_net/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:49.659005 physicsml-0.2.0/src/physicsml/models/tensor_net/modules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/models/tensor_net/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7368 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/models/tensor_net/modules/embedding.py
--rw-r--r--   0 runner    (1001) docker     (127)     3621 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/models/tensor_net/modules/interaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/models/tensor_net/modules/output.py
--rw-r--r--   0 runner    (1001) docker     (127)     3279 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/models/tensor_net/modules/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:49.659005 physicsml-0.2.0/src/physicsml/models/tensor_net/supervised/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/models/tensor_net/supervised/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/models/tensor_net/supervised/default_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/models/tensor_net/supervised/tensor_net_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4882 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/models/tensor_net/supervised/tensor_net_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     3593 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/models/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:49.659005 physicsml-0.2.0/src/physicsml/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:49.659005 physicsml-0.2.0/src/physicsml/plugins/ase/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/plugins/ase/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/plugins/ase/ase_ani.py
--rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/plugins/ase/ase_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     3717 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/plugins/ase/calculator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/plugins/ase/load.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:49.663005 physicsml-0.2.0/src/physicsml/plugins/openmm/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/plugins/openmm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/plugins/openmm/load.py
--rw-r--r--   0 runner    (1001) docker     (127)     2630 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/plugins/openmm/openmm_ani.py
--rw-r--r--   0 runner    (1001) docker     (127)     4533 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/plugins/openmm/openmm_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6232 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/plugins/openmm/openmm_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     5370 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/plugins/openmm/physicsml_potential.py
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     3130 2024-03-07 14:58:04.000000 physicsml-0.2.0/src/physicsml/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-03-07 14:58:49.000000 physicsml-0.2.0/src/physicsml/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:49.679005 physicsml-0.2.0/src/physicsml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4650 2024-03-07 14:58:49.000000 physicsml-0.2.0/src/physicsml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15962 2024-03-07 14:58:49.000000 physicsml-0.2.0/src/physicsml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-07 14:58:49.000000 physicsml-0.2.0/src/physicsml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-03-07 14:58:49.000000 physicsml-0.2.0/src/physicsml.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-03-07 14:58:49.000000 physicsml-0.2.0/src/physicsml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-07 14:58:49.000000 physicsml-0.2.0/src/physicsml.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:49.663005 physicsml-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:04.000000 physicsml-0.2.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:49.663005 physicsml-0.2.0/tests/ase/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:04.000000 physicsml-0.2.0/tests/ase/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9983 2024-03-07 14:58:04.000000 physicsml-0.2.0/tests/ase/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-03-07 14:58:04.000000 physicsml-0.2.0/tests/ase/test_ase_ani.py
--rw-r--r--   0 runner    (1001) docker     (127)     2865 2024-03-07 14:58:04.000000 physicsml-0.2.0/tests/ase/test_ase_graph.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:49.663005 physicsml-0.2.0/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)     4578 2024-03-07 14:58:04.000000 physicsml-0.2.0/tests/data/alanine-dipeptide-truncated.pdb
--rw-r--r--   0 runner    (1001) docker     (127)   698696 2024-03-07 14:58:04.000000 physicsml-0.2.0/tests/data/ani1x.h5
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:49.663005 physicsml-0.2.0/tests/data/ani_model/
--rw-r--r--   0 runner    (1001) docker     (127)     5795 2024-03-07 14:58:04.000000 physicsml-0.2.0/tests/data/ani_model/featurisation_metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:49.663005 physicsml-0.2.0/tests/data/ani_model/model_artefacts/
--rw-r--r--   0 runner    (1001) docker     (127)  1320280 2024-03-07 14:58:04.000000 physicsml-0.2.0/tests/data/ani_model/model_artefacts/module_checkpoint.ckpt
--rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-03-07 14:58:04.000000 physicsml-0.2.0/tests/data/ani_model/model_config.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:49.667005 physicsml-0.2.0/tests/data/egnn_model/
--rw-r--r--   0 runner    (1001) docker     (127)     5795 2024-03-07 14:58:04.000000 physicsml-0.2.0/tests/data/egnn_model/featurisation_metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:49.667005 physicsml-0.2.0/tests/data/egnn_model/model_artefacts/
--rw-r--r--   0 runner    (1001) docker     (127)    52081 2024-03-07 14:58:04.000000 physicsml-0.2.0/tests/data/egnn_model/model_artefacts/module_checkpoint.ckpt
--rw-r--r--   0 runner    (1001) docker     (127)     3496 2024-03-07 14:58:04.000000 physicsml-0.2.0/tests/data/egnn_model/model_config.json
--rw-r--r--   0 runner    (1001) docker     (127)    20277 2024-03-07 14:58:04.000000 physicsml-0.2.0/tests/data/gdb9.csv
--rw-r--r--   0 runner    (1001) docker     (127)    98022 2024-03-07 14:58:04.000000 physicsml-0.2.0/tests/data/gdb9.sdf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:49.667005 physicsml-0.2.0/tests/data/mace_model/
--rw-r--r--   0 runner    (1001) docker     (127)     5795 2024-03-07 14:58:04.000000 physicsml-0.2.0/tests/data/mace_model/featurisation_metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:49.667005 physicsml-0.2.0/tests/data/mace_model/model_artefacts/
--rw-r--r--   0 runner    (1001) docker     (127)   117170 2024-03-07 14:58:04.000000 physicsml-0.2.0/tests/data/mace_model/model_artefacts/module_checkpoint.ckpt
--rw-r--r--   0 runner    (1001) docker     (127)     3433 2024-03-07 14:58:04.000000 physicsml-0.2.0/tests/data/mace_model/model_config.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:49.667005 physicsml-0.2.0/tests/data/nequip_model/
--rw-r--r--   0 runner    (1001) docker     (127)     5795 2024-03-07 14:58:04.000000 physicsml-0.2.0/tests/data/nequip_model/featurisation_metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:49.667005 physicsml-0.2.0/tests/data/nequip_model/model_artefacts/
--rw-r--r--   0 runner    (1001) docker     (127)    86167 2024-03-07 14:58:04.000000 physicsml-0.2.0/tests/data/nequip_model/model_artefacts/module_checkpoint.ckpt
--rw-r--r--   0 runner    (1001) docker     (127)     3501 2024-03-07 14:58:04.000000 physicsml-0.2.0/tests/data/nequip_model/model_config.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:49.667005 physicsml-0.2.0/tests/openeye/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:04.000000 physicsml-0.2.0/tests/openeye/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9987 2024-03-07 14:58:04.000000 physicsml-0.2.0/tests/openeye/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:49.667005 physicsml-0.2.0/tests/openeye/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:04.000000 physicsml-0.2.0/tests/openeye/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:49.667005 physicsml-0.2.0/tests/openeye/core/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:04.000000 physicsml-0.2.0/tests/openeye/core/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-03-07 14:58:04.000000 physicsml-0.2.0/tests/openeye/core/data/test_datamodule.py
--rw-r--r--   0 runner    (1001) docker     (127)     6036 2024-03-07 14:58:04.000000 physicsml-0.2.0/tests/openeye/core/data/test_graph_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:49.671005 physicsml-0.2.0/tests/openeye/core/featurisation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:04.000000 physicsml-0.2.0/tests/openeye/core/featurisation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4999 2024-03-07 14:58:04.000000 physicsml-0.2.0/tests/openeye/core/featurisation/test_physicsml_featurisation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:49.671005 physicsml-0.2.0/tests/openeye/integration/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:04.000000 physicsml-0.2.0/tests/openeye/integration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:49.671005 physicsml-0.2.0/tests/openeye/integration/prism/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:04.000000 physicsml-0.2.0/tests/openeye/integration/prism/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3258 2024-03-07 14:58:04.000000 physicsml-0.2.0/tests/openeye/integration/prism/test_egnn_prism.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:49.671005 physicsml-0.2.0/tests/openeye/integration/training/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:04.000000 physicsml-0.2.0/tests/openeye/integration/training/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:49.671005 physicsml-0.2.0/tests/openeye/integration/training/egnn/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:04.000000 physicsml-0.2.0/tests/openeye/integration/training/egnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-03-07 14:58:04.000000 physicsml-0.2.0/tests/openeye/integration/training/egnn/test_egnn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:49.671005 physicsml-0.2.0/tests/openmm/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:04.000000 physicsml-0.2.0/tests/openmm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9942 2024-03-07 14:58:04.000000 physicsml-0.2.0/tests/openmm/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    10818 2024-03-07 14:58:04.000000 physicsml-0.2.0/tests/openmm/test_openmm_ani.py
--rw-r--r--   0 runner    (1001) docker     (127)    12348 2024-03-07 14:58:04.000000 physicsml-0.2.0/tests/openmm/test_openmm_egnn.py
--rw-r--r--   0 runner    (1001) docker     (127)    12488 2024-03-07 14:58:04.000000 physicsml-0.2.0/tests/openmm/test_openmm_mace.py
--rw-r--r--   0 runner    (1001) docker     (127)    12848 2024-03-07 14:58:04.000000 physicsml-0.2.0/tests/openmm/test_openmm_nequip.py
--rw-r--r--   0 runner    (1001) docker     (127)     7101 2024-03-07 14:58:04.000000 physicsml-0.2.0/tests/openmm/test_openmm_nnp_potential.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:49.671005 physicsml-0.2.0/tests/rdkit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:04.000000 physicsml-0.2.0/tests/rdkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9982 2024-03-07 14:58:04.000000 physicsml-0.2.0/tests/rdkit/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:49.671005 physicsml-0.2.0/tests/rdkit/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:04.000000 physicsml-0.2.0/tests/rdkit/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:49.671005 physicsml-0.2.0/tests/rdkit/core/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:04.000000 physicsml-0.2.0/tests/rdkit/core/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-03-07 14:58:04.000000 physicsml-0.2.0/tests/rdkit/core/data/test_datamodule.py
--rw-r--r--   0 runner    (1001) docker     (127)     6036 2024-03-07 14:58:04.000000 physicsml-0.2.0/tests/rdkit/core/data/test_graph_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:49.671005 physicsml-0.2.0/tests/rdkit/core/featurisation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:04.000000 physicsml-0.2.0/tests/rdkit/core/featurisation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4978 2024-03-07 14:58:04.000000 physicsml-0.2.0/tests/rdkit/core/featurisation/test_physicsml_featurisation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:49.671005 physicsml-0.2.0/tests/rdkit/integration/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:04.000000 physicsml-0.2.0/tests/rdkit/integration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:49.675005 physicsml-0.2.0/tests/rdkit/integration/prism/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:04.000000 physicsml-0.2.0/tests/rdkit/integration/prism/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3573 2024-03-07 14:58:04.000000 physicsml-0.2.0/tests/rdkit/integration/prism/test_allegro_prism.py
--rw-r--r--   0 runner    (1001) docker     (127)     2966 2024-03-07 14:58:04.000000 physicsml-0.2.0/tests/rdkit/integration/prism/test_ani_prism.py
--rw-r--r--   0 runner    (1001) docker     (127)     3258 2024-03-07 14:58:04.000000 physicsml-0.2.0/tests/rdkit/integration/prism/test_egnn_prism.py
--rw-r--r--   0 runner    (1001) docker     (127)     3346 2024-03-07 14:58:04.000000 physicsml-0.2.0/tests/rdkit/integration/prism/test_mace_prism.py
--rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-03-07 14:58:04.000000 physicsml-0.2.0/tests/rdkit/integration/prism/test_nequip_prism.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:49.675005 physicsml-0.2.0/tests/rdkit/integration/training/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:04.000000 physicsml-0.2.0/tests/rdkit/integration/training/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:49.675005 physicsml-0.2.0/tests/rdkit/integration/training/allegro/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:04.000000 physicsml-0.2.0/tests/rdkit/integration/training/allegro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-03-07 14:58:04.000000 physicsml-0.2.0/tests/rdkit/integration/training/allegro/test_allegro_energy_charges.py
--rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-03-07 14:58:04.000000 physicsml-0.2.0/tests/rdkit/integration/training/allegro/test_allegro_forces.py
--rw-r--r--   0 runner    (1001) docker     (127)     3375 2024-03-07 14:58:04.000000 physicsml-0.2.0/tests/rdkit/integration/training/allegro/test_allegro_mean_var.py
--rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-03-07 14:58:04.000000 physicsml-0.2.0/tests/rdkit/integration/training/allegro/test_allergo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:49.675005 physicsml-0.2.0/tests/rdkit/integration/training/ani/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:04.000000 physicsml-0.2.0/tests/rdkit/integration/training/ani/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-03-07 14:58:04.000000 physicsml-0.2.0/tests/rdkit/integration/training/ani/test_ani.py
--rw-r--r--   0 runner    (1001) docker     (127)     2877 2024-03-07 14:58:04.000000 physicsml-0.2.0/tests/rdkit/integration/training/ani/test_ani_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-03-07 14:58:04.000000 physicsml-0.2.0/tests/rdkit/integration/training/ani/test_ani_forces.py
--rw-r--r--   0 runner    (1001) docker     (127)     2724 2024-03-07 14:58:04.000000 physicsml-0.2.0/tests/rdkit/integration/training/ani/test_ani_mean_var.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:49.675005 physicsml-0.2.0/tests/rdkit/integration/training/egnn/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:04.000000 physicsml-0.2.0/tests/rdkit/integration/training/egnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2075 2024-03-07 14:58:04.000000 physicsml-0.2.0/tests/rdkit/integration/training/egnn/test_adapter_egnn.py
--rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-03-07 14:58:04.000000 physicsml-0.2.0/tests/rdkit/integration/training/egnn/test_egnn.py
--rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-03-07 14:58:04.000000 physicsml-0.2.0/tests/rdkit/integration/training/egnn/test_egnn_energy_charges.py
--rw-r--r--   0 runner    (1001) docker     (127)     2343 2024-03-07 14:58:04.000000 physicsml-0.2.0/tests/rdkit/integration/training/egnn/test_egnn_forces.py
--rw-r--r--   0 runner    (1001) docker     (127)     3024 2024-03-07 14:58:04.000000 physicsml-0.2.0/tests/rdkit/integration/training/egnn/test_egnn_mean_var.py
--rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-03-07 14:58:04.000000 physicsml-0.2.0/tests/rdkit/integration/training/egnn/test_ssf_egnn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:49.679005 physicsml-0.2.0/tests/rdkit/integration/training/mace/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:04.000000 physicsml-0.2.0/tests/rdkit/integration/training/mace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2165 2024-03-07 14:58:04.000000 physicsml-0.2.0/tests/rdkit/integration/training/mace/test_adapter_mace.py
--rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-03-07 14:58:04.000000 physicsml-0.2.0/tests/rdkit/integration/training/mace/test_mace.py
--rw-r--r--   0 runner    (1001) docker     (127)     2985 2024-03-07 14:58:04.000000 physicsml-0.2.0/tests/rdkit/integration/training/mace/test_mace_energy_charges.py
--rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-03-07 14:58:04.000000 physicsml-0.2.0/tests/rdkit/integration/training/mace/test_mace_forces.py
--rw-r--r--   0 runner    (1001) docker     (127)     3081 2024-03-07 14:58:04.000000 physicsml-0.2.0/tests/rdkit/integration/training/mace/test_mace_mean_var.py
--rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-03-07 14:58:04.000000 physicsml-0.2.0/tests/rdkit/integration/training/mace/test_ssf_mace.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:49.679005 physicsml-0.2.0/tests/rdkit/integration/training/nequip/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:04.000000 physicsml-0.2.0/tests/rdkit/integration/training/nequip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-03-07 14:58:04.000000 physicsml-0.2.0/tests/rdkit/integration/training/nequip/test_adapter_nequip.py
--rw-r--r--   0 runner    (1001) docker     (127)     2121 2024-03-07 14:58:04.000000 physicsml-0.2.0/tests/rdkit/integration/training/nequip/test_nequip.py
--rw-r--r--   0 runner    (1001) docker     (127)     3089 2024-03-07 14:58:04.000000 physicsml-0.2.0/tests/rdkit/integration/training/nequip/test_nequip_energy_charges.py
--rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-03-07 14:58:04.000000 physicsml-0.2.0/tests/rdkit/integration/training/nequip/test_nequip_forces.py
--rw-r--r--   0 runner    (1001) docker     (127)     3248 2024-03-07 14:58:04.000000 physicsml-0.2.0/tests/rdkit/integration/training/nequip/test_nequip_mean_var.py
--rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-03-07 14:58:04.000000 physicsml-0.2.0/tests/rdkit/integration/training/nequip/test_ssf_nequip.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:49.679005 physicsml-0.2.0/tests/rdkit/integration/training/tensor_net/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 14:58:04.000000 physicsml-0.2.0/tests/rdkit/integration/training/tensor_net/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-03-07 14:58:04.000000 physicsml-0.2.0/tests/rdkit/integration/training/tensor_net/test_tensor_net.py
--rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-03-07 14:58:04.000000 physicsml-0.2.0/tests/rdkit/integration/training/tensor_net/test_tensor_net_energy_charges.py
--rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-03-07 14:58:04.000000 physicsml-0.2.0/tests/rdkit/integration/training/tensor_net/test_tensor_net_forces.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:53:14.114492 physicsml-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-04-03 15:52:59.000000 physicsml-0.2.1/.envrc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:53:14.038493 physicsml-0.2.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:53:14.050493 physicsml-0.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-03 15:52:59.000000 physicsml-0.2.1/.github/workflows/dev-ci-actions.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-03 15:52:59.000000 physicsml-0.2.1/.github/workflows/docs-build-deploy.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-04-03 15:52:59.000000 physicsml-0.2.1/.github/workflows/latest-tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-03 15:52:59.000000 physicsml-0.2.1/.github/workflows/main-ci-actions.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-04-03 15:52:59.000000 physicsml-0.2.1/.github/workflows/pinned-tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-03 15:52:59.000000 physicsml-0.2.1/.github/workflows/publish-package.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-03 15:52:59.000000 physicsml-0.2.1/.github/workflows/quality-typing-checks.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-03 15:52:59.000000 physicsml-0.2.1/.github/workflows/release-ci-actions.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-03 15:52:59.000000 physicsml-0.2.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-04-03 15:52:59.000000 physicsml-0.2.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-04-03 15:52:59.000000 physicsml-0.2.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-03 15:52:59.000000 physicsml-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4650 2024-04-03 15:53:14.110492 physicsml-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-04-03 15:52:59.000000 physicsml-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:53:14.054493 physicsml-0.2.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-03 15:52:59.000000 physicsml-0.2.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-03 15:52:59.000000 physicsml-0.2.1/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:53:14.054493 physicsml-0.2.1/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:53:14.054493 physicsml-0.2.1/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     3348 2024-04-03 15:52:59.000000 physicsml-0.2.1/docs/source/_static/PhysicsML_Logo-01.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     7381 2024-04-03 15:52:59.000000 physicsml-0.2.1/docs/source/_static/PhysicsML_Logo_PhyML_logo full dark-cropped.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     7503 2024-04-03 15:52:59.000000 physicsml-0.2.1/docs/source/_static/PhysicsML_Logo_PhyML_logo full dark.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     7380 2024-04-03 15:52:59.000000 physicsml-0.2.1/docs/source/_static/PhysicsML_Logo_PhyML_logo full light-cropped.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     7502 2024-04-03 15:52:59.000000 physicsml-0.2.1/docs/source/_static/PhysicsML_Logo_PhyML_logo full light.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     7824 2024-04-03 15:52:59.000000 physicsml-0.2.1/docs/source/_static/PhysicsML_Logo_PhyML_logo text dark.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     7836 2024-04-03 15:52:59.000000 physicsml-0.2.1/docs/source/_static/PhysicsML_Logo_PhyML_logo text light.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-04-03 15:52:59.000000 physicsml-0.2.1/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-04-03 15:52:59.000000 physicsml-0.2.1/docs/source/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:53:14.042493 physicsml-0.2.1/docs/source/pages/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:53:14.054493 physicsml-0.2.1/docs/source/pages/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)     5631 2024-04-03 15:52:59.000000 physicsml-0.2.1/docs/source/pages/datasets/qm_datasets.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:53:14.054493 physicsml-0.2.1/docs/source/pages/features/
+-rw-r--r--   0 runner    (1001) docker     (127)   489710 2024-04-03 15:52:59.000000 physicsml-0.2.1/docs/source/pages/features/gdb9_trunc.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-03 15:52:59.000000 physicsml-0.2.1/docs/source/pages/features/how_to_add_reps.md
+-rw-r--r--   0 runner    (1001) docker     (127)     9303 2024-04-03 15:52:59.000000 physicsml-0.2.1/docs/source/pages/features/intro.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:53:14.054493 physicsml-0.2.1/docs/source/pages/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     4886 2024-04-03 15:52:59.000000 physicsml-0.2.1/docs/source/pages/models/allegro.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3349 2024-04-03 15:52:59.000000 physicsml-0.2.1/docs/source/pages/models/ani.md
+-rw-r--r--   0 runner    (1001) docker     (127)    10655 2024-04-03 15:52:59.000000 physicsml-0.2.1/docs/source/pages/models/egnn.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6295 2024-04-03 15:52:59.000000 physicsml-0.2.1/docs/source/pages/models/how_to_add_models.md
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-03 15:52:59.000000 physicsml-0.2.1/docs/source/pages/models/intro.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8347 2024-04-03 15:52:59.000000 physicsml-0.2.1/docs/source/pages/models/mace.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8998 2024-04-03 15:52:59.000000 physicsml-0.2.1/docs/source/pages/models/nequip.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-04-03 15:52:59.000000 physicsml-0.2.1/docs/source/pages/models/tensor_net.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:53:14.058493 physicsml-0.2.1/docs/source/pages/philosophy/
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-03 15:52:59.000000 physicsml-0.2.1/docs/source/pages/philosophy/molflux.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-04-03 15:52:59.000000 physicsml-0.2.1/docs/source/pages/philosophy/philosophy.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:53:14.058493 physicsml-0.2.1/docs/source/pages/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-03 15:52:59.000000 physicsml-0.2.1/docs/source/pages/plugins/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     4578 2024-04-03 15:52:59.000000 physicsml-0.2.1/docs/source/pages/plugins/alanine-dipeptide-truncated.pdb
+-rw-r--r--   0 runner    (1001) docker     (127)     3899 2024-04-03 15:52:59.000000 physicsml-0.2.1/docs/source/pages/plugins/ase.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5335 2024-04-03 15:52:59.000000 physicsml-0.2.1/docs/source/pages/plugins/openmm.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:53:14.058493 physicsml-0.2.1/docs/source/pages/structure/
+-rw-r--r--   0 runner    (1001) docker     (127)     7237 2024-04-03 15:52:59.000000 physicsml-0.2.1/docs/source/pages/structure/lightning_layer.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4803 2024-04-03 15:52:59.000000 physicsml-0.2.1/docs/source/pages/structure/molflux_layer.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-03 15:52:59.000000 physicsml-0.2.1/docs/source/pages/structure/physicsml_structure.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6294 2024-04-03 15:52:59.000000 physicsml-0.2.1/docs/source/pages/structure/torch_layer.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2906 2024-04-03 15:52:59.000000 physicsml-0.2.1/docs/source/pages/structure/transfer_learning.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:53:14.062493 physicsml-0.2.1/docs/source/pages/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-03 15:52:59.000000 physicsml-0.2.1/docs/source/pages/tutorials/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     7462 2024-04-03 15:52:59.000000 physicsml-0.2.1/docs/source/pages/tutorials/ani1x_energy_forces_training.md
+-rw-r--r--   0 runner    (1001) docker     (127)  1610932 2024-04-03 15:52:59.000000 physicsml-0.2.1/docs/source/pages/tutorials/ani1x_truncated.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     9729 2024-04-03 15:52:59.000000 physicsml-0.2.1/docs/source/pages/tutorials/gdb9_training.md
+-rw-r--r--   0 runner    (1001) docker     (127)   489710 2024-04-03 15:52:59.000000 physicsml-0.2.1/docs/source/pages/tutorials/gdb9_trunc.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     7678 2024-04-03 15:52:59.000000 physicsml-0.2.1/docs/source/pages/tutorials/gdb9_uncertainty.md
+-rw-r--r--   0 runner    (1001) docker     (127)    10605 2024-04-03 15:52:59.000000 physicsml-0.2.1/docs/source/pages/tutorials/transfer_learning.md
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-03 15:52:59.000000 physicsml-0.2.1/environment.yml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1053 2024-04-03 15:52:59.000000 physicsml-0.2.1/init_conda_venv.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      714 2024-04-03 15:52:59.000000 physicsml-0.2.1/init_python_venv.sh
+-rw-r--r--   0 runner    (1001) docker     (127)    12217 2024-04-03 15:52:59.000000 physicsml-0.2.1/noxfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-03 15:52:59.000000 physicsml-0.2.1/openmm_env.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:53:14.042493 physicsml-0.2.1/pinned-versions/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:53:14.062493 physicsml-0.2.1/pinned-versions/3.10/
+-rw-r--r--   0 runner    (1001) docker     (127)    12169 2024-04-03 15:52:59.000000 physicsml-0.2.1/pinned-versions/3.10/lockfile.ase.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    12168 2024-04-03 15:52:59.000000 physicsml-0.2.1/pinned-versions/3.10/lockfile.core.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    12237 2024-04-03 15:52:59.000000 physicsml-0.2.1/pinned-versions/3.10/lockfile.openeye.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    12172 2024-04-03 15:52:59.000000 physicsml-0.2.1/pinned-versions/3.10/lockfile.openmm.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    12171 2024-04-03 15:52:59.000000 physicsml-0.2.1/pinned-versions/3.10/lockfile.rdkit.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:53:14.062493 physicsml-0.2.1/pinned-versions/3.11/
+-rw-r--r--   0 runner    (1001) docker     (127)    11991 2024-04-03 15:52:59.000000 physicsml-0.2.1/pinned-versions/3.11/lockfile.ase.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11990 2024-04-03 15:52:59.000000 physicsml-0.2.1/pinned-versions/3.11/lockfile.core.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    12059 2024-04-03 15:52:59.000000 physicsml-0.2.1/pinned-versions/3.11/lockfile.openeye.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11994 2024-04-03 15:52:59.000000 physicsml-0.2.1/pinned-versions/3.11/lockfile.openmm.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11993 2024-04-03 15:52:59.000000 physicsml-0.2.1/pinned-versions/3.11/lockfile.rdkit.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:53:14.062493 physicsml-0.2.1/pinned-versions/3.8/
+-rw-r--r--   0 runner    (1001) docker     (127)    13023 2024-04-03 15:52:59.000000 physicsml-0.2.1/pinned-versions/3.8/lockfile.ase.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    13022 2024-04-03 15:52:59.000000 physicsml-0.2.1/pinned-versions/3.8/lockfile.core.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    13193 2024-04-03 15:52:59.000000 physicsml-0.2.1/pinned-versions/3.8/lockfile.openeye.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    13026 2024-04-03 15:52:59.000000 physicsml-0.2.1/pinned-versions/3.8/lockfile.openmm.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    13025 2024-04-03 15:52:59.000000 physicsml-0.2.1/pinned-versions/3.8/lockfile.rdkit.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:53:14.066493 physicsml-0.2.1/pinned-versions/3.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    12324 2024-04-03 15:52:59.000000 physicsml-0.2.1/pinned-versions/3.9/lockfile.ase.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    12323 2024-04-03 15:52:59.000000 physicsml-0.2.1/pinned-versions/3.9/lockfile.core.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    12392 2024-04-03 15:52:59.000000 physicsml-0.2.1/pinned-versions/3.9/lockfile.openeye.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    12327 2024-04-03 15:52:59.000000 physicsml-0.2.1/pinned-versions/3.9/lockfile.openmm.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    12326 2024-04-03 15:52:59.000000 physicsml-0.2.1/pinned-versions/3.9/lockfile.rdkit.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     7505 2024-04-03 15:52:59.000000 physicsml-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 15:53:14.114492 physicsml-0.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:53:14.042493 physicsml-0.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:53:14.066493 physicsml-0.2.1/src/physicsml/
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:53:14.066493 physicsml-0.2.1/src/physicsml/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2286 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/backends/backend_selector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4970 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/backends/openeye_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4927 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/backends/rdkit_backend.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:53:14.066493 physicsml-0.2.1/src/physicsml/featurisation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/featurisation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:53:14.066493 physicsml-0.2.1/src/physicsml/featurisation/physicsml_features/
+-rw-r--r--   0 runner    (1001) docker     (127)     4246 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/featurisation/physicsml_features/atom_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/featurisation/physicsml_features/bond_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5600 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/featurisation/physicsml_features/physicsml_features.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:53:14.066493 physicsml-0.2.1/src/physicsml/lightning/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/lightning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3569 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/lightning/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5705 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/lightning/datamodule.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:53:14.070493 physicsml-0.2.1/src/physicsml/lightning/graph_datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/lightning/graph_datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13126 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/lightning/graph_datasets/graph_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5583 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/lightning/graph_datasets/neighbourhood_list_torch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:53:14.070493 physicsml-0.2.1/src/physicsml/lightning/graph_datasets/torch_nl_vendored/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/lightning/graph_datasets/torch_nl_vendored/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/lightning/graph_datasets/torch_nl_vendored/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12716 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/lightning/graph_datasets/torch_nl_vendored/linked_cell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2482 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/lightning/graph_datasets/torch_nl_vendored/naive_impl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5236 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/lightning/graph_datasets/torch_nl_vendored/neighbor_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/lightning/graph_datasets/torch_nl_vendored/timer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/lightning/graph_datasets/torch_nl_vendored/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:53:14.070493 physicsml-0.2.1/src/physicsml/lightning/losses/
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/lightning/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10118 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/lightning/losses/barlow_twins_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/lightning/losses/construct_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/lightning/losses/loss_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/lightning/losses/masked_mse_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/lightning/losses/multitask_losses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/lightning/losses/serial_bce_w_logits_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/lightning/losses/stock_losses.py
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/lightning/losses/weighted_mse_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4642 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/lightning/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6462 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/lightning/model_uncertainty.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6630 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/lightning/module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/lightning/pre_batching_in_memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/lightning/pre_batching_on_disk.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:53:14.070493 physicsml-0.2.1/src/physicsml/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:53:14.070493 physicsml-0.2.1/src/physicsml/models/allegro/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/models/allegro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4108 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/models/allegro/allegro_prism.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:53:14.074493 physicsml-0.2.1/src/physicsml/models/allegro/mean_var/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/models/allegro/mean_var/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/models/allegro/mean_var/default_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/models/allegro/mean_var/mean_var_allegro_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6496 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/models/allegro/mean_var/mean_var_allegro_module.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:53:14.074493 physicsml-0.2.1/src/physicsml/models/allegro/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/models/allegro/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24182 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/models/allegro/modules/allegro.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/models/allegro/modules/channels.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15463 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/models/allegro/modules/contract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/models/allegro/modules/cutoffs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5427 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/models/allegro/modules/fc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2759 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/models/allegro/modules/layout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8447 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/models/allegro/modules/linear.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3696 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/models/allegro/modules/radial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5406 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/models/allegro/modules/spmm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:53:14.074493 physicsml-0.2.1/src/physicsml/models/allegro/supervised/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/models/allegro/supervised/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/models/allegro/supervised/allegro_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5639 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/models/allegro/supervised/allegro_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/models/allegro/supervised/default_configs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:53:14.074493 physicsml-0.2.1/src/physicsml/models/ani/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/models/ani/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4619 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/models/ani/ani_1_2_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5150 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/models/ani/ani_datamodule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5859 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/models/ani/ani_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2826 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/models/ani/ani_prism.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2688 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/models/ani/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:53:14.074493 physicsml-0.2.1/src/physicsml/models/ani/ensemble/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/models/ani/ensemble/default_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/models/ani/ensemble/ensemble_ani_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9754 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/models/ani/ensemble/ensemble_ani_module.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:53:14.074493 physicsml-0.2.1/src/physicsml/models/ani/mean_var/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/models/ani/mean_var/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/models/ani/mean_var/default_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/models/ani/mean_var/mean_var_ani_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8955 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/models/ani/mean_var/mean_var_ani_module.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:53:14.078493 physicsml-0.2.1/src/physicsml/models/ani/supervised/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/models/ani/supervised/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/models/ani/supervised/ani_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8395 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/models/ani/supervised/ani_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/models/ani/supervised/default_configs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:53:14.078493 physicsml-0.2.1/src/physicsml/models/egnn/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/models/egnn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:53:14.078493 physicsml-0.2.1/src/physicsml/models/egnn/adapter/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/models/egnn/adapter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/models/egnn/adapter/adapter_egnn_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6317 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/models/egnn/adapter/adapter_egnn_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6599 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/models/egnn/adapter/adapter_egnn_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/models/egnn/adapter/default_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4251 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/models/egnn/egnn_prism.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15452 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/models/egnn/egnn_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:53:14.078493 physicsml-0.2.1/src/physicsml/models/egnn/mean_var/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/models/egnn/mean_var/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/models/egnn/mean_var/default_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/models/egnn/mean_var/mean_var_egnn_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6987 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/models/egnn/mean_var/mean_var_egnn_module.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:53:14.078493 physicsml-0.2.1/src/physicsml/models/egnn/ssf/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/models/egnn/ssf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/models/egnn/ssf/default_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/models/egnn/ssf/ssf_egnn_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6159 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/models/egnn/ssf/ssf_egnn_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3689 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/models/egnn/ssf/ssf_egnn_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:53:14.078493 physicsml-0.2.1/src/physicsml/models/egnn/supervised/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/models/egnn/supervised/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/models/egnn/supervised/default_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/models/egnn/supervised/egnn_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6308 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/models/egnn/supervised/egnn_module.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:53:14.082493 physicsml-0.2.1/src/physicsml/models/mace/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/models/mace/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:53:14.082493 physicsml-0.2.1/src/physicsml/models/mace/adapter/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/models/mace/adapter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/models/mace/adapter/adapter_mace_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8422 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/models/mace/adapter/adapter_mace_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8480 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/models/mace/adapter/adapter_mace_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/models/mace/adapter/default_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4194 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/models/mace/mace_prism.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:53:14.082493 physicsml-0.2.1/src/physicsml/models/mace/mean_var/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/models/mace/mean_var/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/models/mace/mean_var/default_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/models/mace/mean_var/mean_var_mace_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8887 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/models/mace/mean_var/mean_var_mace_module.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:53:14.082493 physicsml-0.2.1/src/physicsml/models/mace/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/models/mace/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3773 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/models/mace/modules/_activation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8197 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/models/mace/modules/blocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4377 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/models/mace/modules/cg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/models/mace/modules/irreps_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8507 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/models/mace/modules/mace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/models/mace/modules/radial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9635 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/models/mace/modules/symmetric_contraction.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:53:14.082493 physicsml-0.2.1/src/physicsml/models/mace/ssf/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/models/mace/ssf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/models/mace/ssf/default_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/models/mace/ssf/ssf_mace_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8236 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/models/mace/ssf/ssf_mace_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6820 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/models/mace/ssf/ssf_mace_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:53:14.086493 physicsml-0.2.1/src/physicsml/models/mace/supervised/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/models/mace/supervised/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/models/mace/supervised/default_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/models/mace/supervised/mace_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8133 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/models/mace/supervised/mace_module.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:53:14.086493 physicsml-0.2.1/src/physicsml/models/nequip/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/models/nequip/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:53:14.086493 physicsml-0.2.1/src/physicsml/models/nequip/adapter/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/models/nequip/adapter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/models/nequip/adapter/adapter_nequip_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6696 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/models/nequip/adapter/adapter_nequip_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7075 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/models/nequip/adapter/adapter_nequip_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/models/nequip/adapter/default_configs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:53:14.086493 physicsml-0.2.1/src/physicsml/models/nequip/mean_var/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/models/nequip/mean_var/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/models/nequip/mean_var/default_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/models/nequip/mean_var/mean_var_nequip_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7196 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/models/nequip/mean_var/mean_var_nequip_module.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:53:14.086493 physicsml-0.2.1/src/physicsml/models/nequip/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/models/nequip/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3773 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/models/nequip/modules/_activation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5727 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/models/nequip/modules/_gate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3466 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/models/nequip/modules/convnet_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3683 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/models/nequip/modules/interaction_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5968 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/models/nequip/modules/nequip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/models/nequip/modules/radial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/models/nequip/modules/scale_shift.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4494 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/models/nequip/nequip_prism.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:53:14.086493 physicsml-0.2.1/src/physicsml/models/nequip/ssf/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/models/nequip/ssf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/models/nequip/ssf/default_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/models/nequip/ssf/ssf_nequip_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6522 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/models/nequip/ssf/ssf_nequip_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5306 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/models/nequip/ssf/ssf_nequip_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:53:14.090493 physicsml-0.2.1/src/physicsml/models/nequip/supervised/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/models/nequip/supervised/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/models/nequip/supervised/default_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/models/nequip/supervised/nequip_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6431 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/models/nequip/supervised/nequip_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4990 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/models/prism.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:53:14.090493 physicsml-0.2.1/src/physicsml/models/tensor_net/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/models/tensor_net/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:53:14.090493 physicsml-0.2.1/src/physicsml/models/tensor_net/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/models/tensor_net/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7368 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/models/tensor_net/modules/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3621 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/models/tensor_net/modules/interaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/models/tensor_net/modules/output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3279 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/models/tensor_net/modules/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:53:14.090493 physicsml-0.2.1/src/physicsml/models/tensor_net/supervised/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/models/tensor_net/supervised/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/models/tensor_net/supervised/default_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/models/tensor_net/supervised/tensor_net_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4882 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/models/tensor_net/supervised/tensor_net_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3593 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/models/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:53:14.090493 physicsml-0.2.1/src/physicsml/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:53:14.090493 physicsml-0.2.1/src/physicsml/plugins/ase/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/plugins/ase/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/plugins/ase/ase_ani.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/plugins/ase/ase_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3717 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/plugins/ase/calculator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/plugins/ase/load.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:53:14.090493 physicsml-0.2.1/src/physicsml/plugins/openmm/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/plugins/openmm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/plugins/openmm/load.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2630 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/plugins/openmm/openmm_ani.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4533 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/plugins/openmm/openmm_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6232 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/plugins/openmm/openmm_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5370 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/plugins/openmm/physicsml_potential.py
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     3130 2024-04-03 15:52:59.000000 physicsml-0.2.1/src/physicsml/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-03 15:53:13.000000 physicsml-0.2.1/src/physicsml/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:53:14.110492 physicsml-0.2.1/src/physicsml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4650 2024-04-03 15:53:13.000000 physicsml-0.2.1/src/physicsml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    16449 2024-04-03 15:53:14.000000 physicsml-0.2.1/src/physicsml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 15:53:13.000000 physicsml-0.2.1/src/physicsml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-04-03 15:53:13.000000 physicsml-0.2.1/src/physicsml.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-03 15:53:13.000000 physicsml-0.2.1/src/physicsml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-03 15:53:13.000000 physicsml-0.2.1/src/physicsml.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:53:14.094493 physicsml-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 15:52:59.000000 physicsml-0.2.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:53:14.094493 physicsml-0.2.1/tests/ase/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 15:52:59.000000 physicsml-0.2.1/tests/ase/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9983 2024-04-03 15:52:59.000000 physicsml-0.2.1/tests/ase/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-04-03 15:52:59.000000 physicsml-0.2.1/tests/ase/test_ase_ani.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2865 2024-04-03 15:52:59.000000 physicsml-0.2.1/tests/ase/test_ase_graph.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:53:14.094493 physicsml-0.2.1/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     4578 2024-04-03 15:52:59.000000 physicsml-0.2.1/tests/data/alanine-dipeptide-truncated.pdb
+-rw-r--r--   0 runner    (1001) docker     (127)   698696 2024-04-03 15:52:59.000000 physicsml-0.2.1/tests/data/ani1x.h5
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:53:14.094493 physicsml-0.2.1/tests/data/ani_model/
+-rw-r--r--   0 runner    (1001) docker     (127)     5795 2024-04-03 15:52:59.000000 physicsml-0.2.1/tests/data/ani_model/featurisation_metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:53:14.094493 physicsml-0.2.1/tests/data/ani_model/model_artefacts/
+-rw-r--r--   0 runner    (1001) docker     (127)  1320280 2024-04-03 15:52:59.000000 physicsml-0.2.1/tests/data/ani_model/model_artefacts/module_checkpoint.ckpt
+-rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-04-03 15:52:59.000000 physicsml-0.2.1/tests/data/ani_model/model_config.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:53:14.098492 physicsml-0.2.1/tests/data/egnn_model/
+-rw-r--r--   0 runner    (1001) docker     (127)     5795 2024-04-03 15:52:59.000000 physicsml-0.2.1/tests/data/egnn_model/featurisation_metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:53:14.098492 physicsml-0.2.1/tests/data/egnn_model/model_artefacts/
+-rw-r--r--   0 runner    (1001) docker     (127)    52081 2024-04-03 15:52:59.000000 physicsml-0.2.1/tests/data/egnn_model/model_artefacts/module_checkpoint.ckpt
+-rw-r--r--   0 runner    (1001) docker     (127)     3496 2024-04-03 15:52:59.000000 physicsml-0.2.1/tests/data/egnn_model/model_config.json
+-rw-r--r--   0 runner    (1001) docker     (127)    20277 2024-04-03 15:52:59.000000 physicsml-0.2.1/tests/data/gdb9.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    98022 2024-04-03 15:52:59.000000 physicsml-0.2.1/tests/data/gdb9.sdf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:53:14.098492 physicsml-0.2.1/tests/data/mace_model/
+-rw-r--r--   0 runner    (1001) docker     (127)     5795 2024-04-03 15:52:59.000000 physicsml-0.2.1/tests/data/mace_model/featurisation_metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:53:14.098492 physicsml-0.2.1/tests/data/mace_model/model_artefacts/
+-rw-r--r--   0 runner    (1001) docker     (127)   117170 2024-04-03 15:52:59.000000 physicsml-0.2.1/tests/data/mace_model/model_artefacts/module_checkpoint.ckpt
+-rw-r--r--   0 runner    (1001) docker     (127)     3433 2024-04-03 15:52:59.000000 physicsml-0.2.1/tests/data/mace_model/model_config.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:53:14.098492 physicsml-0.2.1/tests/data/nequip_model/
+-rw-r--r--   0 runner    (1001) docker     (127)     5795 2024-04-03 15:52:59.000000 physicsml-0.2.1/tests/data/nequip_model/featurisation_metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:53:14.098492 physicsml-0.2.1/tests/data/nequip_model/model_artefacts/
+-rw-r--r--   0 runner    (1001) docker     (127)    86167 2024-04-03 15:52:59.000000 physicsml-0.2.1/tests/data/nequip_model/model_artefacts/module_checkpoint.ckpt
+-rw-r--r--   0 runner    (1001) docker     (127)     3501 2024-04-03 15:52:59.000000 physicsml-0.2.1/tests/data/nequip_model/model_config.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:53:14.098492 physicsml-0.2.1/tests/openeye/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 15:52:59.000000 physicsml-0.2.1/tests/openeye/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9987 2024-04-03 15:52:59.000000 physicsml-0.2.1/tests/openeye/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:53:14.098492 physicsml-0.2.1/tests/openeye/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 15:52:59.000000 physicsml-0.2.1/tests/openeye/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:53:14.098492 physicsml-0.2.1/tests/openeye/core/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 15:52:59.000000 physicsml-0.2.1/tests/openeye/core/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-04-03 15:52:59.000000 physicsml-0.2.1/tests/openeye/core/data/test_datamodule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6036 2024-04-03 15:52:59.000000 physicsml-0.2.1/tests/openeye/core/data/test_graph_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:53:14.098492 physicsml-0.2.1/tests/openeye/core/featurisation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 15:52:59.000000 physicsml-0.2.1/tests/openeye/core/featurisation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4999 2024-04-03 15:52:59.000000 physicsml-0.2.1/tests/openeye/core/featurisation/test_physicsml_featurisation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:53:14.098492 physicsml-0.2.1/tests/openeye/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 15:52:59.000000 physicsml-0.2.1/tests/openeye/integration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:53:14.098492 physicsml-0.2.1/tests/openeye/integration/prism/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 15:52:59.000000 physicsml-0.2.1/tests/openeye/integration/prism/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3258 2024-04-03 15:52:59.000000 physicsml-0.2.1/tests/openeye/integration/prism/test_egnn_prism.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:53:14.098492 physicsml-0.2.1/tests/openeye/integration/training/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 15:52:59.000000 physicsml-0.2.1/tests/openeye/integration/training/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:53:14.102492 physicsml-0.2.1/tests/openeye/integration/training/egnn/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 15:52:59.000000 physicsml-0.2.1/tests/openeye/integration/training/egnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-04-03 15:52:59.000000 physicsml-0.2.1/tests/openeye/integration/training/egnn/test_egnn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:53:14.102492 physicsml-0.2.1/tests/openmm/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 15:52:59.000000 physicsml-0.2.1/tests/openmm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9942 2024-04-03 15:52:59.000000 physicsml-0.2.1/tests/openmm/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10818 2024-04-03 15:52:59.000000 physicsml-0.2.1/tests/openmm/test_openmm_ani.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16225 2024-04-03 15:52:59.000000 physicsml-0.2.1/tests/openmm/test_openmm_egnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16422 2024-04-03 15:52:59.000000 physicsml-0.2.1/tests/openmm/test_openmm_mace.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16903 2024-04-03 15:52:59.000000 physicsml-0.2.1/tests/openmm/test_openmm_nequip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7399 2024-04-03 15:52:59.000000 physicsml-0.2.1/tests/openmm/test_openmm_nnp_potential.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:53:14.102492 physicsml-0.2.1/tests/rdkit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 15:52:59.000000 physicsml-0.2.1/tests/rdkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9982 2024-04-03 15:52:59.000000 physicsml-0.2.1/tests/rdkit/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:53:14.102492 physicsml-0.2.1/tests/rdkit/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 15:52:59.000000 physicsml-0.2.1/tests/rdkit/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:53:14.102492 physicsml-0.2.1/tests/rdkit/core/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 15:52:59.000000 physicsml-0.2.1/tests/rdkit/core/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-04-03 15:52:59.000000 physicsml-0.2.1/tests/rdkit/core/data/test_datamodule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6036 2024-04-03 15:52:59.000000 physicsml-0.2.1/tests/rdkit/core/data/test_graph_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:53:14.102492 physicsml-0.2.1/tests/rdkit/core/featurisation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 15:52:59.000000 physicsml-0.2.1/tests/rdkit/core/featurisation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4978 2024-04-03 15:52:59.000000 physicsml-0.2.1/tests/rdkit/core/featurisation/test_physicsml_featurisation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:53:14.102492 physicsml-0.2.1/tests/rdkit/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 15:52:59.000000 physicsml-0.2.1/tests/rdkit/integration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:53:14.102492 physicsml-0.2.1/tests/rdkit/integration/prism/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 15:52:59.000000 physicsml-0.2.1/tests/rdkit/integration/prism/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3573 2024-04-03 15:52:59.000000 physicsml-0.2.1/tests/rdkit/integration/prism/test_allegro_prism.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2966 2024-04-03 15:52:59.000000 physicsml-0.2.1/tests/rdkit/integration/prism/test_ani_prism.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3258 2024-04-03 15:52:59.000000 physicsml-0.2.1/tests/rdkit/integration/prism/test_egnn_prism.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3346 2024-04-03 15:52:59.000000 physicsml-0.2.1/tests/rdkit/integration/prism/test_mace_prism.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-04-03 15:52:59.000000 physicsml-0.2.1/tests/rdkit/integration/prism/test_nequip_prism.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:53:14.102492 physicsml-0.2.1/tests/rdkit/integration/training/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 15:52:59.000000 physicsml-0.2.1/tests/rdkit/integration/training/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:53:14.106492 physicsml-0.2.1/tests/rdkit/integration/training/allegro/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 15:52:59.000000 physicsml-0.2.1/tests/rdkit/integration/training/allegro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-04-03 15:52:59.000000 physicsml-0.2.1/tests/rdkit/integration/training/allegro/test_allegro_energy_charges.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-04-03 15:52:59.000000 physicsml-0.2.1/tests/rdkit/integration/training/allegro/test_allegro_forces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3375 2024-04-03 15:52:59.000000 physicsml-0.2.1/tests/rdkit/integration/training/allegro/test_allegro_mean_var.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-04-03 15:52:59.000000 physicsml-0.2.1/tests/rdkit/integration/training/allegro/test_allergo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:53:14.106492 physicsml-0.2.1/tests/rdkit/integration/training/ani/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 15:52:59.000000 physicsml-0.2.1/tests/rdkit/integration/training/ani/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-04-03 15:52:59.000000 physicsml-0.2.1/tests/rdkit/integration/training/ani/test_ani.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2877 2024-04-03 15:52:59.000000 physicsml-0.2.1/tests/rdkit/integration/training/ani/test_ani_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-04-03 15:52:59.000000 physicsml-0.2.1/tests/rdkit/integration/training/ani/test_ani_forces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2724 2024-04-03 15:52:59.000000 physicsml-0.2.1/tests/rdkit/integration/training/ani/test_ani_mean_var.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:53:14.106492 physicsml-0.2.1/tests/rdkit/integration/training/egnn/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 15:52:59.000000 physicsml-0.2.1/tests/rdkit/integration/training/egnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2075 2024-04-03 15:52:59.000000 physicsml-0.2.1/tests/rdkit/integration/training/egnn/test_adapter_egnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-04-03 15:52:59.000000 physicsml-0.2.1/tests/rdkit/integration/training/egnn/test_egnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-04-03 15:52:59.000000 physicsml-0.2.1/tests/rdkit/integration/training/egnn/test_egnn_energy_charges.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2343 2024-04-03 15:52:59.000000 physicsml-0.2.1/tests/rdkit/integration/training/egnn/test_egnn_forces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3024 2024-04-03 15:52:59.000000 physicsml-0.2.1/tests/rdkit/integration/training/egnn/test_egnn_mean_var.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-04-03 15:52:59.000000 physicsml-0.2.1/tests/rdkit/integration/training/egnn/test_ssf_egnn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:53:14.106492 physicsml-0.2.1/tests/rdkit/integration/training/mace/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 15:52:59.000000 physicsml-0.2.1/tests/rdkit/integration/training/mace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2165 2024-04-03 15:52:59.000000 physicsml-0.2.1/tests/rdkit/integration/training/mace/test_adapter_mace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-04-03 15:52:59.000000 physicsml-0.2.1/tests/rdkit/integration/training/mace/test_mace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2985 2024-04-03 15:52:59.000000 physicsml-0.2.1/tests/rdkit/integration/training/mace/test_mace_energy_charges.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-04-03 15:52:59.000000 physicsml-0.2.1/tests/rdkit/integration/training/mace/test_mace_forces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3081 2024-04-03 15:52:59.000000 physicsml-0.2.1/tests/rdkit/integration/training/mace/test_mace_mean_var.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-04-03 15:52:59.000000 physicsml-0.2.1/tests/rdkit/integration/training/mace/test_ssf_mace.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:53:14.110492 physicsml-0.2.1/tests/rdkit/integration/training/nequip/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 15:52:59.000000 physicsml-0.2.1/tests/rdkit/integration/training/nequip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-04-03 15:52:59.000000 physicsml-0.2.1/tests/rdkit/integration/training/nequip/test_adapter_nequip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2121 2024-04-03 15:52:59.000000 physicsml-0.2.1/tests/rdkit/integration/training/nequip/test_nequip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3089 2024-04-03 15:52:59.000000 physicsml-0.2.1/tests/rdkit/integration/training/nequip/test_nequip_energy_charges.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-04-03 15:52:59.000000 physicsml-0.2.1/tests/rdkit/integration/training/nequip/test_nequip_forces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3248 2024-04-03 15:52:59.000000 physicsml-0.2.1/tests/rdkit/integration/training/nequip/test_nequip_mean_var.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-04-03 15:52:59.000000 physicsml-0.2.1/tests/rdkit/integration/training/nequip/test_ssf_nequip.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:53:14.110492 physicsml-0.2.1/tests/rdkit/integration/training/tensor_net/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 15:52:59.000000 physicsml-0.2.1/tests/rdkit/integration/training/tensor_net/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-04-03 15:52:59.000000 physicsml-0.2.1/tests/rdkit/integration/training/tensor_net/test_tensor_net.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-04-03 15:52:59.000000 physicsml-0.2.1/tests/rdkit/integration/training/tensor_net/test_tensor_net_energy_charges.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-04-03 15:52:59.000000 physicsml-0.2.1/tests/rdkit/integration/training/tensor_net/test_tensor_net_forces.py
```

### Comparing `physicsml-0.2.0/.envrc` & `physicsml-0.2.1/.envrc`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/.github/workflows/docs-build-deploy.yaml` & `physicsml-0.2.1/.github/workflows/docs-build-deploy.yaml`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/.github/workflows/latest-tests.yaml` & `physicsml-0.2.1/.github/workflows/latest-tests.yaml`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/.github/workflows/pinned-tests.yaml` & `physicsml-0.2.1/.github/workflows/pinned-tests.yaml`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/.github/workflows/publish-package.yaml` & `physicsml-0.2.1/.github/workflows/publish-package.yaml`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/.github/workflows/quality-typing-checks.yaml` & `physicsml-0.2.1/.github/workflows/quality-typing-checks.yaml`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/.gitignore` & `physicsml-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/.pre-commit-config.yaml` & `physicsml-0.2.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/CHANGELOG.md` & `physicsml-0.2.1/CHANGELOG.md`

 * *Files 19% similar despite different names*

```diff
@@ -5,14 +5,19 @@
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/), and this project
 adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 ---------------------------------------------------------
 
 ## [Unreleased]
 
 ---------------------------------------------------------
+## [0.2.1] - 2024-04-03
+
+## Fixed
+
+* Fixed bug in neighbour list with torchscript
 
 ## [0.2.0] - 2024-03-07
 
 ## Fixed
 
 * Improved neighbour list computation (10x faster)
```

### Comparing `physicsml-0.2.0/LICENSE` & `physicsml-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/PKG-INFO` & `physicsml-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: physicsml
-Version: 0.2.0
+Version: 0.2.1
 Summary: A package for all physics based/related models
 Author: Exscientia
 Maintainer: Exscientia
 Project-URL: documentation, https://github.com/exscientia/physicsml/issues
 Project-URL: repository, https://github.com/exscientia/physicsml.git
 Project-URL: issue-tracker, https://github.com/exscientia/physicsml/issues
 Project-URL: changelog, https://github.com/exscientia/physicsml/src/main/CHANGELOG.md
```

### Comparing `physicsml-0.2.0/README.md` & `physicsml-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/docs/Makefile` & `physicsml-0.2.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/docs/make.bat` & `physicsml-0.2.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/docs/source/_static/PhysicsML_Logo-01.svg` & `physicsml-0.2.1/docs/source/_static/PhysicsML_Logo-01.svg`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/docs/source/_static/PhysicsML_Logo_PhyML_logo full dark-cropped.svg` & `physicsml-0.2.1/docs/source/_static/PhysicsML_Logo_PhyML_logo full dark-cropped.svg`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/docs/source/_static/PhysicsML_Logo_PhyML_logo full dark.svg` & `physicsml-0.2.1/docs/source/_static/PhysicsML_Logo_PhyML_logo full dark.svg`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/docs/source/_static/PhysicsML_Logo_PhyML_logo full light-cropped.svg` & `physicsml-0.2.1/docs/source/_static/PhysicsML_Logo_PhyML_logo full light-cropped.svg`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/docs/source/_static/PhysicsML_Logo_PhyML_logo full light.svg` & `physicsml-0.2.1/docs/source/_static/PhysicsML_Logo_PhyML_logo full light.svg`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/docs/source/_static/PhysicsML_Logo_PhyML_logo text dark.svg` & `physicsml-0.2.1/docs/source/_static/PhysicsML_Logo_PhyML_logo text dark.svg`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/docs/source/_static/PhysicsML_Logo_PhyML_logo text light.svg` & `physicsml-0.2.1/docs/source/_static/PhysicsML_Logo_PhyML_logo text light.svg`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/docs/source/conf.py` & `physicsml-0.2.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/docs/source/index.md` & `physicsml-0.2.1/docs/source/index.md`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/docs/source/pages/datasets/qm_datasets.md` & `physicsml-0.2.1/docs/source/pages/datasets/qm_datasets.md`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/docs/source/pages/features/gdb9_trunc.parquet` & `physicsml-0.2.1/docs/source/pages/features/gdb9_trunc.parquet`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/docs/source/pages/features/how_to_add_reps.md` & `physicsml-0.2.1/docs/source/pages/features/how_to_add_reps.md`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/docs/source/pages/features/intro.md` & `physicsml-0.2.1/docs/source/pages/features/intro.md`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/docs/source/pages/models/allegro.md` & `physicsml-0.2.1/docs/source/pages/models/allegro.md`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/docs/source/pages/models/ani.md` & `physicsml-0.2.1/docs/source/pages/models/ani.md`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/docs/source/pages/models/egnn.md` & `physicsml-0.2.1/docs/source/pages/models/egnn.md`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/docs/source/pages/models/how_to_add_models.md` & `physicsml-0.2.1/docs/source/pages/models/how_to_add_models.md`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/docs/source/pages/models/intro.md` & `physicsml-0.2.1/docs/source/pages/models/intro.md`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/docs/source/pages/models/mace.md` & `physicsml-0.2.1/docs/source/pages/models/mace.md`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/docs/source/pages/models/nequip.md` & `physicsml-0.2.1/docs/source/pages/models/nequip.md`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/docs/source/pages/models/tensor_net.md` & `physicsml-0.2.1/docs/source/pages/models/tensor_net.md`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/docs/source/pages/philosophy/molflux.md` & `physicsml-0.2.1/docs/source/pages/philosophy/molflux.md`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/docs/source/pages/philosophy/philosophy.md` & `physicsml-0.2.1/docs/source/pages/philosophy/philosophy.md`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/docs/source/pages/plugins/alanine-dipeptide-truncated.pdb` & `physicsml-0.2.1/docs/source/pages/plugins/alanine-dipeptide-truncated.pdb`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/docs/source/pages/plugins/ase.md` & `physicsml-0.2.1/docs/source/pages/plugins/ase.md`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/docs/source/pages/plugins/openmm.md` & `physicsml-0.2.1/docs/source/pages/plugins/openmm.md`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/docs/source/pages/structure/lightning_layer.md` & `physicsml-0.2.1/docs/source/pages/structure/lightning_layer.md`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/docs/source/pages/structure/molflux_layer.md` & `physicsml-0.2.1/docs/source/pages/structure/molflux_layer.md`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/docs/source/pages/structure/physicsml_structure.md` & `physicsml-0.2.1/docs/source/pages/structure/physicsml_structure.md`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/docs/source/pages/structure/torch_layer.md` & `physicsml-0.2.1/docs/source/pages/structure/torch_layer.md`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/docs/source/pages/structure/transfer_learning.md` & `physicsml-0.2.1/docs/source/pages/structure/transfer_learning.md`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/docs/source/pages/tutorials/ani1x_energy_forces_training.md` & `physicsml-0.2.1/docs/source/pages/tutorials/ani1x_energy_forces_training.md`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/docs/source/pages/tutorials/ani1x_truncated.parquet` & `physicsml-0.2.1/docs/source/pages/tutorials/ani1x_truncated.parquet`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/docs/source/pages/tutorials/gdb9_training.md` & `physicsml-0.2.1/docs/source/pages/tutorials/gdb9_training.md`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/docs/source/pages/tutorials/gdb9_trunc.parquet` & `physicsml-0.2.1/docs/source/pages/tutorials/gdb9_trunc.parquet`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/docs/source/pages/tutorials/gdb9_uncertainty.md` & `physicsml-0.2.1/docs/source/pages/tutorials/gdb9_uncertainty.md`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/docs/source/pages/tutorials/transfer_learning.md` & `physicsml-0.2.1/docs/source/pages/tutorials/transfer_learning.md`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/init_conda_venv.sh` & `physicsml-0.2.1/init_conda_venv.sh`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/init_python_venv.sh` & `physicsml-0.2.1/init_python_venv.sh`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/noxfile.py` & `physicsml-0.2.1/noxfile.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 BUILD_TOOLS = ["build"]
 COVERAGE_TOOLS = ["coverage[toml]", "coverage-badge"]
 FORMATTING_TOOLS = ["black[jupyter]~=23.0"]
 LINTING_TOOLS = ["ruff~=0.0.292"]
 LOCKFILE_TOOLS = ["pip-tools>=7.0.0"]  # default --resolver=backtracking
 
 EXTRAS = [None, "openmm", "rdkit", "ase", "openeye"]
-DONT_TEST = [None, "openmm", "openeye"]
+DONT_TEST = [None, "openeye", "openmm"]
 
 def resolve_lockfile_path(python_version: str, extra: Optional[str] = None, rootdir: str = PINNED_VERSIONS) -> pathlib.Path:
     """Resolves the expected lockfile path for a given python version and extra."""
     lockfile_name = f"lockfile.{extra or 'core'}.txt"
     return pathlib.Path(rootdir) / python_version / lockfile_name
 
 
@@ -265,19 +265,15 @@
         lockfile_path: The path to the lockfile to use for constraining the
             testing environment.
         notify: If True, coverage reporting sessions are queued up on success.
     """
 
     # Setup which files and tests to target
     # install test dependencies and extra dependencies
-    if extra == "openmm":
-        session.conda_install("openmm", "openmm-torch", "openmm-ml", "pytorch>=2.0,<2.1", channel=["conda-forge"])
-        package_extras = ",".join(["tests", extra])
-
-    elif extra is not None:
+    if extra is not None:
         package_extras = ",".join(["tests", extra])
 
     else:
         package_extras = ",".join(["tests"])
 
     # all tests requiring the extra are in their own dir and
     tests_target_dirs = [f"tests/{extra}"]
```

### Comparing `physicsml-0.2.0/pinned-versions/3.10/lockfile.ase.txt` & `physicsml-0.2.1/pinned-versions/3.10/lockfile.ase.txt`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/pinned-versions/3.10/lockfile.core.txt` & `physicsml-0.2.1/pinned-versions/3.10/lockfile.core.txt`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/pinned-versions/3.10/lockfile.openeye.txt` & `physicsml-0.2.1/pinned-versions/3.10/lockfile.openeye.txt`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/pinned-versions/3.10/lockfile.openmm.txt` & `physicsml-0.2.1/pinned-versions/3.10/lockfile.openmm.txt`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/pinned-versions/3.10/lockfile.rdkit.txt` & `physicsml-0.2.1/pinned-versions/3.10/lockfile.rdkit.txt`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/pinned-versions/3.11/lockfile.ase.txt` & `physicsml-0.2.1/pinned-versions/3.11/lockfile.ase.txt`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/pinned-versions/3.11/lockfile.core.txt` & `physicsml-0.2.1/pinned-versions/3.11/lockfile.core.txt`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/pinned-versions/3.11/lockfile.openeye.txt` & `physicsml-0.2.1/pinned-versions/3.11/lockfile.openeye.txt`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/pinned-versions/3.11/lockfile.openmm.txt` & `physicsml-0.2.1/pinned-versions/3.11/lockfile.openmm.txt`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/pinned-versions/3.11/lockfile.rdkit.txt` & `physicsml-0.2.1/pinned-versions/3.11/lockfile.rdkit.txt`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/pinned-versions/3.8/lockfile.ase.txt` & `physicsml-0.2.1/pinned-versions/3.8/lockfile.ase.txt`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/pinned-versions/3.8/lockfile.core.txt` & `physicsml-0.2.1/pinned-versions/3.8/lockfile.core.txt`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/pinned-versions/3.8/lockfile.openeye.txt` & `physicsml-0.2.1/pinned-versions/3.8/lockfile.openeye.txt`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/pinned-versions/3.8/lockfile.openmm.txt` & `physicsml-0.2.1/pinned-versions/3.8/lockfile.openmm.txt`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/pinned-versions/3.8/lockfile.rdkit.txt` & `physicsml-0.2.1/pinned-versions/3.8/lockfile.rdkit.txt`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/pinned-versions/3.9/lockfile.ase.txt` & `physicsml-0.2.1/pinned-versions/3.9/lockfile.ase.txt`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/pinned-versions/3.9/lockfile.core.txt` & `physicsml-0.2.1/pinned-versions/3.9/lockfile.core.txt`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/pinned-versions/3.9/lockfile.openeye.txt` & `physicsml-0.2.1/pinned-versions/3.9/lockfile.openeye.txt`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/pinned-versions/3.9/lockfile.openmm.txt` & `physicsml-0.2.1/pinned-versions/3.9/lockfile.openmm.txt`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/pinned-versions/3.9/lockfile.rdkit.txt` & `physicsml-0.2.1/pinned-versions/3.9/lockfile.rdkit.txt`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/pyproject.toml` & `physicsml-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -161,14 +161,18 @@
 show_error_codes = true
 
 [[tool.mypy.overrides]]
 module = "physicsml.models.allegro.modules.*"
 ignore_errors = true
 
 [[tool.mypy.overrides]]
+module = "physicsml.lightning.graph_datasets.torch_nl_vendored.*"
+ignore_errors = true
+
+[[tool.mypy.overrides]]
 check_untyped_defs = true
 disallow_untyped_defs = false
 module = 'tests.*'
 
 [[tool.mypy.overrides]]
 check_untyped_defs = true
 disallow_untyped_decorators = false
```

### Comparing `physicsml-0.2.0/src/physicsml/backends/backend_selector.py` & `physicsml-0.2.1/src/physicsml/backends/backend_selector.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/src/physicsml/backends/openeye_backend.py` & `physicsml-0.2.1/src/physicsml/backends/openeye_backend.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/src/physicsml/backends/rdkit_backend.py` & `physicsml-0.2.1/src/physicsml/backends/rdkit_backend.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/src/physicsml/featurisation/physicsml_features/atom_features.py` & `physicsml-0.2.1/src/physicsml/featurisation/physicsml_features/atom_features.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/src/physicsml/featurisation/physicsml_features/bond_features.py` & `physicsml-0.2.1/src/physicsml/featurisation/physicsml_features/bond_features.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/src/physicsml/featurisation/physicsml_features/physicsml_features.py` & `physicsml-0.2.1/src/physicsml/featurisation/physicsml_features/physicsml_features.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/src/physicsml/lightning/config.py` & `physicsml-0.2.1/src/physicsml/lightning/config.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/src/physicsml/lightning/datamodule.py` & `physicsml-0.2.1/src/physicsml/lightning/datamodule.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/src/physicsml/lightning/graph_datasets/graph_dataset.py` & `physicsml-0.2.1/src/physicsml/lightning/graph_datasets/graph_dataset.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/src/physicsml/lightning/graph_datasets/neighbourhood_list_torch.py` & `physicsml-0.2.1/src/physicsml/lightning/graph_datasets/neighbourhood_list_torch.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 from typing import Optional, Tuple
 
 import torch
 from torch_geometric.utils import (
     coalesce,
     to_undirected,
 )
-from torch_nl import compute_neighborlist
+
+from physicsml.lightning.graph_datasets.torch_nl_vendored.neighbor_list import (
+    compute_neighborlist,
+)
 
 # tracing torch geom funcs to ensure that they use the required overloading
 to_undirected_ts = torch.jit.trace(
     to_undirected,
     (
         torch.tensor([[0, 0, 1, 2], [2, 2, 1, 0]]),
         torch.tensor([[0, 1], [0, 1], [1, 2], [2, 1]]).float(),
```

### Comparing `physicsml-0.2.0/src/physicsml/lightning/losses/barlow_twins_loss.py` & `physicsml-0.2.1/src/physicsml/lightning/losses/barlow_twins_loss.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/src/physicsml/lightning/losses/loss_base.py` & `physicsml-0.2.1/src/physicsml/lightning/losses/loss_base.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/src/physicsml/lightning/losses/masked_mse_loss.py` & `physicsml-0.2.1/src/physicsml/lightning/losses/masked_mse_loss.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/src/physicsml/lightning/losses/multitask_losses.py` & `physicsml-0.2.1/src/physicsml/lightning/losses/multitask_losses.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/src/physicsml/lightning/losses/serial_bce_w_logits_loss.py` & `physicsml-0.2.1/src/physicsml/lightning/losses/serial_bce_w_logits_loss.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/src/physicsml/lightning/losses/stock_losses.py` & `physicsml-0.2.1/src/physicsml/lightning/losses/stock_losses.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/src/physicsml/lightning/losses/weighted_mse_loss.py` & `physicsml-0.2.1/src/physicsml/lightning/losses/weighted_mse_loss.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/src/physicsml/lightning/model.py` & `physicsml-0.2.1/src/physicsml/lightning/model.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/src/physicsml/lightning/model_uncertainty.py` & `physicsml-0.2.1/src/physicsml/lightning/model_uncertainty.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/src/physicsml/lightning/module.py` & `physicsml-0.2.1/src/physicsml/lightning/module.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/src/physicsml/lightning/pre_batching_in_memory.py` & `physicsml-0.2.1/src/physicsml/lightning/pre_batching_in_memory.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/src/physicsml/lightning/pre_batching_on_disk.py` & `physicsml-0.2.1/src/physicsml/lightning/pre_batching_on_disk.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/src/physicsml/models/allegro/allegro_prism.py` & `physicsml-0.2.1/src/physicsml/models/allegro/allegro_prism.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/src/physicsml/models/allegro/mean_var/default_configs.py` & `physicsml-0.2.1/src/physicsml/models/allegro/mean_var/default_configs.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/src/physicsml/models/allegro/mean_var/mean_var_allegro_model.py` & `physicsml-0.2.1/src/physicsml/models/allegro/mean_var/mean_var_allegro_model.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/src/physicsml/models/allegro/mean_var/mean_var_allegro_module.py` & `physicsml-0.2.1/src/physicsml/models/allegro/mean_var/mean_var_allegro_module.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/src/physicsml/models/allegro/modules/allegro.py` & `physicsml-0.2.1/src/physicsml/models/allegro/modules/allegro.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/src/physicsml/models/allegro/modules/channels.py` & `physicsml-0.2.1/src/physicsml/models/allegro/modules/channels.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/src/physicsml/models/allegro/modules/contract.py` & `physicsml-0.2.1/src/physicsml/models/allegro/modules/contract.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/src/physicsml/models/allegro/modules/cutoffs.py` & `physicsml-0.2.1/src/physicsml/models/allegro/modules/cutoffs.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/src/physicsml/models/allegro/modules/fc.py` & `physicsml-0.2.1/src/physicsml/models/allegro/modules/fc.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/src/physicsml/models/allegro/modules/layout.py` & `physicsml-0.2.1/src/physicsml/models/allegro/modules/layout.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/src/physicsml/models/allegro/modules/linear.py` & `physicsml-0.2.1/src/physicsml/models/allegro/modules/linear.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/src/physicsml/models/allegro/modules/radial.py` & `physicsml-0.2.1/src/physicsml/models/allegro/modules/radial.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/src/physicsml/models/allegro/modules/spmm.py` & `physicsml-0.2.1/src/physicsml/models/allegro/modules/spmm.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/src/physicsml/models/allegro/supervised/allegro_model.py` & `physicsml-0.2.1/src/physicsml/models/allegro/supervised/allegro_model.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/src/physicsml/models/allegro/supervised/allegro_module.py` & `physicsml-0.2.1/src/physicsml/models/allegro/supervised/allegro_module.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/src/physicsml/models/allegro/supervised/default_configs.py` & `physicsml-0.2.1/src/physicsml/models/allegro/supervised/default_configs.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/src/physicsml/models/ani/ani_1_2_defaults.py` & `physicsml-0.2.1/src/physicsml/models/ani/ani_1_2_defaults.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/src/physicsml/models/ani/ani_datamodule.py` & `physicsml-0.2.1/src/physicsml/models/ani/ani_datamodule.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/src/physicsml/models/ani/ani_dataset.py` & `physicsml-0.2.1/src/physicsml/models/ani/ani_dataset.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/src/physicsml/models/ani/ani_prism.py` & `physicsml-0.2.1/src/physicsml/models/ani/ani_prism.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/src/physicsml/models/ani/config.py` & `physicsml-0.2.1/src/physicsml/models/ani/config.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/src/physicsml/models/ani/ensemble/default_configs.py` & `physicsml-0.2.1/src/physicsml/models/ani/ensemble/default_configs.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/src/physicsml/models/ani/ensemble/ensemble_ani_model.py` & `physicsml-0.2.1/src/physicsml/models/ani/ensemble/ensemble_ani_model.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/src/physicsml/models/ani/ensemble/ensemble_ani_module.py` & `physicsml-0.2.1/src/physicsml/models/ani/ensemble/ensemble_ani_module.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/src/physicsml/models/ani/mean_var/default_configs.py` & `physicsml-0.2.1/src/physicsml/models/ani/mean_var/default_configs.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/src/physicsml/models/ani/mean_var/mean_var_ani_model.py` & `physicsml-0.2.1/src/physicsml/models/ani/mean_var/mean_var_ani_model.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/src/physicsml/models/ani/mean_var/mean_var_ani_module.py` & `physicsml-0.2.1/src/physicsml/models/ani/mean_var/mean_var_ani_module.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/src/physicsml/models/ani/supervised/ani_model.py` & `physicsml-0.2.1/src/physicsml/models/ani/supervised/ani_model.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/src/physicsml/models/ani/supervised/ani_module.py` & `physicsml-0.2.1/src/physicsml/models/ani/supervised/ani_module.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/src/physicsml/models/ani/supervised/default_configs.py` & `physicsml-0.2.1/src/physicsml/models/ani/supervised/default_configs.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/src/physicsml/models/egnn/adapter/adapter_egnn_model.py` & `physicsml-0.2.1/src/physicsml/models/egnn/adapter/adapter_egnn_model.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/src/physicsml/models/egnn/adapter/adapter_egnn_module.py` & `physicsml-0.2.1/src/physicsml/models/egnn/adapter/adapter_egnn_module.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/src/physicsml/models/egnn/adapter/adapter_egnn_utils.py` & `physicsml-0.2.1/src/physicsml/models/egnn/adapter/adapter_egnn_utils.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/src/physicsml/models/egnn/adapter/default_configs.py` & `physicsml-0.2.1/src/physicsml/models/egnn/adapter/default_configs.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/src/physicsml/models/egnn/egnn_prism.py` & `physicsml-0.2.1/src/physicsml/models/egnn/egnn_prism.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/src/physicsml/models/egnn/egnn_utils.py` & `physicsml-0.2.1/src/physicsml/models/egnn/egnn_utils.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/src/physicsml/models/egnn/mean_var/default_configs.py` & `physicsml-0.2.1/src/physicsml/models/egnn/mean_var/default_configs.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/src/physicsml/models/egnn/mean_var/mean_var_egnn_model.py` & `physicsml-0.2.1/src/physicsml/models/egnn/mean_var/mean_var_egnn_model.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/src/physicsml/models/egnn/mean_var/mean_var_egnn_module.py` & `physicsml-0.2.1/src/physicsml/models/egnn/mean_var/mean_var_egnn_module.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/src/physicsml/models/egnn/ssf/default_configs.py` & `physicsml-0.2.1/src/physicsml/models/egnn/ssf/default_configs.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/src/physicsml/models/egnn/ssf/ssf_egnn_model.py` & `physicsml-0.2.1/src/physicsml/models/egnn/ssf/ssf_egnn_model.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/src/physicsml/models/egnn/ssf/ssf_egnn_module.py` & `physicsml-0.2.1/src/physicsml/models/egnn/ssf/ssf_egnn_module.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/src/physicsml/models/egnn/ssf/ssf_egnn_utils.py` & `physicsml-0.2.1/src/physicsml/models/egnn/ssf/ssf_egnn_utils.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/src/physicsml/models/egnn/supervised/default_configs.py` & `physicsml-0.2.1/src/physicsml/models/egnn/supervised/default_configs.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/src/physicsml/models/egnn/supervised/egnn_model.py` & `physicsml-0.2.1/src/physicsml/models/egnn/supervised/egnn_model.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/src/physicsml/models/egnn/supervised/egnn_module.py` & `physicsml-0.2.1/src/physicsml/models/egnn/supervised/egnn_module.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/src/physicsml/models/mace/adapter/adapter_mace_model.py` & `physicsml-0.2.1/src/physicsml/models/mace/adapter/adapter_mace_model.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/src/physicsml/models/mace/adapter/adapter_mace_module.py` & `physicsml-0.2.1/src/physicsml/models/mace/adapter/adapter_mace_module.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/src/physicsml/models/mace/adapter/adapter_mace_utils.py` & `physicsml-0.2.1/src/physicsml/models/mace/adapter/adapter_mace_utils.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/src/physicsml/models/mace/adapter/default_configs.py` & `physicsml-0.2.1/src/physicsml/models/mace/adapter/default_configs.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/src/physicsml/models/mace/mace_prism.py` & `physicsml-0.2.1/src/physicsml/models/mace/mace_prism.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/src/physicsml/models/mace/mean_var/default_configs.py` & `physicsml-0.2.1/src/physicsml/models/mace/mean_var/default_configs.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/src/physicsml/models/mace/mean_var/mean_var_mace_model.py` & `physicsml-0.2.1/src/physicsml/models/mace/mean_var/mean_var_mace_model.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/src/physicsml/models/mace/mean_var/mean_var_mace_module.py` & `physicsml-0.2.1/src/physicsml/models/mace/mean_var/mean_var_mace_module.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/src/physicsml/models/mace/modules/_activation.py` & `physicsml-0.2.1/src/physicsml/models/mace/modules/_activation.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/src/physicsml/models/mace/modules/blocks.py` & `physicsml-0.2.1/src/physicsml/models/mace/modules/blocks.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/src/physicsml/models/mace/modules/cg.py` & `physicsml-0.2.1/src/physicsml/models/mace/modules/cg.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/src/physicsml/models/mace/modules/irreps_tools.py` & `physicsml-0.2.1/src/physicsml/models/mace/modules/irreps_tools.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/src/physicsml/models/mace/modules/mace.py` & `physicsml-0.2.1/src/physicsml/models/mace/modules/mace.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/src/physicsml/models/mace/modules/radial.py` & `physicsml-0.2.1/src/physicsml/models/mace/modules/radial.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/src/physicsml/models/mace/modules/symmetric_contraction.py` & `physicsml-0.2.1/src/physicsml/models/mace/modules/symmetric_contraction.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/src/physicsml/models/mace/ssf/default_configs.py` & `physicsml-0.2.1/src/physicsml/models/mace/ssf/default_configs.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/src/physicsml/models/mace/ssf/ssf_mace_model.py` & `physicsml-0.2.1/src/physicsml/models/mace/ssf/ssf_mace_model.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/src/physicsml/models/mace/ssf/ssf_mace_module.py` & `physicsml-0.2.1/src/physicsml/models/mace/ssf/ssf_mace_module.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/src/physicsml/models/mace/ssf/ssf_mace_utils.py` & `physicsml-0.2.1/src/physicsml/models/mace/ssf/ssf_mace_utils.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/src/physicsml/models/mace/supervised/default_configs.py` & `physicsml-0.2.1/src/physicsml/models/mace/supervised/default_configs.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/src/physicsml/models/mace/supervised/mace_model.py` & `physicsml-0.2.1/src/physicsml/models/mace/supervised/mace_model.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/src/physicsml/models/mace/supervised/mace_module.py` & `physicsml-0.2.1/src/physicsml/models/mace/supervised/mace_module.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/src/physicsml/models/nequip/adapter/adapter_nequip_model.py` & `physicsml-0.2.1/src/physicsml/models/nequip/adapter/adapter_nequip_model.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/src/physicsml/models/nequip/adapter/adapter_nequip_module.py` & `physicsml-0.2.1/src/physicsml/models/nequip/adapter/adapter_nequip_module.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/src/physicsml/models/nequip/adapter/adapter_nequip_utils.py` & `physicsml-0.2.1/src/physicsml/models/nequip/adapter/adapter_nequip_utils.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/src/physicsml/models/nequip/adapter/default_configs.py` & `physicsml-0.2.1/src/physicsml/models/nequip/adapter/default_configs.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/src/physicsml/models/nequip/mean_var/default_configs.py` & `physicsml-0.2.1/src/physicsml/models/nequip/mean_var/default_configs.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/src/physicsml/models/nequip/mean_var/mean_var_nequip_model.py` & `physicsml-0.2.1/src/physicsml/models/nequip/mean_var/mean_var_nequip_model.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/src/physicsml/models/nequip/mean_var/mean_var_nequip_module.py` & `physicsml-0.2.1/src/physicsml/models/nequip/mean_var/mean_var_nequip_module.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/src/physicsml/models/nequip/modules/_activation.py` & `physicsml-0.2.1/src/physicsml/models/nequip/modules/_activation.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/src/physicsml/models/nequip/modules/_gate.py` & `physicsml-0.2.1/src/physicsml/models/nequip/modules/_gate.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/src/physicsml/models/nequip/modules/convnet_layer.py` & `physicsml-0.2.1/src/physicsml/models/nequip/modules/convnet_layer.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/src/physicsml/models/nequip/modules/interaction_block.py` & `physicsml-0.2.1/src/physicsml/models/nequip/modules/interaction_block.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/src/physicsml/models/nequip/modules/nequip.py` & `physicsml-0.2.1/src/physicsml/models/nequip/modules/nequip.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/src/physicsml/models/nequip/modules/radial.py` & `physicsml-0.2.1/src/physicsml/models/nequip/modules/radial.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/src/physicsml/models/nequip/modules/scale_shift.py` & `physicsml-0.2.1/src/physicsml/models/nequip/modules/scale_shift.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/src/physicsml/models/nequip/nequip_prism.py` & `physicsml-0.2.1/src/physicsml/models/nequip/nequip_prism.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/src/physicsml/models/nequip/ssf/default_configs.py` & `physicsml-0.2.1/src/physicsml/models/nequip/ssf/default_configs.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/src/physicsml/models/nequip/ssf/ssf_nequip_model.py` & `physicsml-0.2.1/src/physicsml/models/nequip/ssf/ssf_nequip_model.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/src/physicsml/models/nequip/ssf/ssf_nequip_module.py` & `physicsml-0.2.1/src/physicsml/models/nequip/ssf/ssf_nequip_module.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/src/physicsml/models/nequip/ssf/ssf_nequip_utils.py` & `physicsml-0.2.1/src/physicsml/models/nequip/ssf/ssf_nequip_utils.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/src/physicsml/models/nequip/supervised/default_configs.py` & `physicsml-0.2.1/src/physicsml/models/nequip/supervised/default_configs.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/src/physicsml/models/nequip/supervised/nequip_model.py` & `physicsml-0.2.1/src/physicsml/models/nequip/supervised/nequip_model.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/src/physicsml/models/nequip/supervised/nequip_module.py` & `physicsml-0.2.1/src/physicsml/models/nequip/supervised/nequip_module.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/src/physicsml/models/prism.py` & `physicsml-0.2.1/src/physicsml/models/prism.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/src/physicsml/models/tensor_net/modules/embedding.py` & `physicsml-0.2.1/src/physicsml/models/tensor_net/modules/embedding.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/src/physicsml/models/tensor_net/modules/interaction.py` & `physicsml-0.2.1/src/physicsml/models/tensor_net/modules/interaction.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/src/physicsml/models/tensor_net/modules/output.py` & `physicsml-0.2.1/src/physicsml/models/tensor_net/modules/output.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/src/physicsml/models/tensor_net/modules/utils.py` & `physicsml-0.2.1/src/physicsml/models/tensor_net/modules/utils.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/src/physicsml/models/tensor_net/supervised/default_configs.py` & `physicsml-0.2.1/src/physicsml/models/tensor_net/supervised/default_configs.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/src/physicsml/models/tensor_net/supervised/tensor_net_model.py` & `physicsml-0.2.1/src/physicsml/models/tensor_net/supervised/tensor_net_model.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/src/physicsml/models/tensor_net/supervised/tensor_net_module.py` & `physicsml-0.2.1/src/physicsml/models/tensor_net/supervised/tensor_net_module.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/src/physicsml/models/utils.py` & `physicsml-0.2.1/src/physicsml/models/utils.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/src/physicsml/plugins/ase/ase_ani.py` & `physicsml-0.2.1/src/physicsml/plugins/ase/ase_ani.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/src/physicsml/plugins/ase/ase_graph.py` & `physicsml-0.2.1/src/physicsml/plugins/ase/ase_graph.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/src/physicsml/plugins/ase/calculator.py` & `physicsml-0.2.1/src/physicsml/plugins/ase/calculator.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/src/physicsml/plugins/ase/load.py` & `physicsml-0.2.1/src/physicsml/plugins/ase/load.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/src/physicsml/plugins/openmm/load.py` & `physicsml-0.2.1/src/physicsml/plugins/openmm/load.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/src/physicsml/plugins/openmm/openmm_ani.py` & `physicsml-0.2.1/src/physicsml/plugins/openmm/openmm_ani.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/src/physicsml/plugins/openmm/openmm_base.py` & `physicsml-0.2.1/src/physicsml/plugins/openmm/openmm_base.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/src/physicsml/plugins/openmm/openmm_graph.py` & `physicsml-0.2.1/src/physicsml/plugins/openmm/openmm_graph.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/src/physicsml/plugins/openmm/physicsml_potential.py` & `physicsml-0.2.1/src/physicsml/plugins/openmm/physicsml_potential.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/src/physicsml/utils.py` & `physicsml-0.2.1/src/physicsml/utils.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/src/physicsml.egg-info/PKG-INFO` & `physicsml-0.2.1/src/physicsml.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: physicsml
-Version: 0.2.0
+Version: 0.2.1
 Summary: A package for all physics based/related models
 Author: Exscientia
 Maintainer: Exscientia
 Project-URL: documentation, https://github.com/exscientia/physicsml/issues
 Project-URL: repository, https://github.com/exscientia/physicsml.git
 Project-URL: issue-tracker, https://github.com/exscientia/physicsml/issues
 Project-URL: changelog, https://github.com/exscientia/physicsml/src/main/CHANGELOG.md
```

### Comparing `physicsml-0.2.0/src/physicsml.egg-info/SOURCES.txt` & `physicsml-0.2.1/src/physicsml.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -104,14 +104,21 @@
 src/physicsml/lightning/model_uncertainty.py
 src/physicsml/lightning/module.py
 src/physicsml/lightning/pre_batching_in_memory.py
 src/physicsml/lightning/pre_batching_on_disk.py
 src/physicsml/lightning/graph_datasets/__init__.py
 src/physicsml/lightning/graph_datasets/graph_dataset.py
 src/physicsml/lightning/graph_datasets/neighbourhood_list_torch.py
+src/physicsml/lightning/graph_datasets/torch_nl_vendored/__init__.py
+src/physicsml/lightning/graph_datasets/torch_nl_vendored/geometry.py
+src/physicsml/lightning/graph_datasets/torch_nl_vendored/linked_cell.py
+src/physicsml/lightning/graph_datasets/torch_nl_vendored/naive_impl.py
+src/physicsml/lightning/graph_datasets/torch_nl_vendored/neighbor_list.py
+src/physicsml/lightning/graph_datasets/torch_nl_vendored/timer.py
+src/physicsml/lightning/graph_datasets/torch_nl_vendored/utils.py
 src/physicsml/lightning/losses/__init__.py
 src/physicsml/lightning/losses/barlow_twins_loss.py
 src/physicsml/lightning/losses/construct_loss.py
 src/physicsml/lightning/losses/loss_base.py
 src/physicsml/lightning/losses/masked_mse_loss.py
 src/physicsml/lightning/losses/multitask_losses.py
 src/physicsml/lightning/losses/serial_bce_w_logits_loss.py
```

### Comparing `physicsml-0.2.0/src/physicsml.egg-info/entry_points.txt` & `physicsml-0.2.1/src/physicsml.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/src/physicsml.egg-info/requires.txt` & `physicsml-0.2.1/src/physicsml.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/tests/ase/conftest.py` & `physicsml-0.2.1/tests/ase/conftest.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/tests/ase/test_ase_ani.py` & `physicsml-0.2.1/tests/ase/test_ase_ani.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/tests/ase/test_ase_graph.py` & `physicsml-0.2.1/tests/ase/test_ase_graph.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/tests/data/alanine-dipeptide-truncated.pdb` & `physicsml-0.2.1/tests/data/alanine-dipeptide-truncated.pdb`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/tests/data/ani1x.h5` & `physicsml-0.2.1/tests/data/ani1x.h5`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/tests/data/ani_model/featurisation_metadata.json` & `physicsml-0.2.1/tests/data/ani_model/featurisation_metadata.json`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/tests/data/ani_model/model_artefacts/module_checkpoint.ckpt` & `physicsml-0.2.1/tests/data/ani_model/model_artefacts/module_checkpoint.ckpt`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/tests/data/ani_model/model_config.json` & `physicsml-0.2.1/tests/data/ani_model/model_config.json`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/tests/data/egnn_model/featurisation_metadata.json` & `physicsml-0.2.1/tests/data/egnn_model/featurisation_metadata.json`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/tests/data/egnn_model/model_artefacts/module_checkpoint.ckpt` & `physicsml-0.2.1/tests/data/egnn_model/model_artefacts/module_checkpoint.ckpt`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/tests/data/egnn_model/model_config.json` & `physicsml-0.2.1/tests/data/egnn_model/model_config.json`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/tests/data/gdb9.csv` & `physicsml-0.2.1/tests/data/gdb9.csv`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/tests/data/gdb9.sdf` & `physicsml-0.2.1/tests/data/gdb9.sdf`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/tests/data/mace_model/featurisation_metadata.json` & `physicsml-0.2.1/tests/data/mace_model/featurisation_metadata.json`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/tests/data/mace_model/model_artefacts/module_checkpoint.ckpt` & `physicsml-0.2.1/tests/data/mace_model/model_artefacts/module_checkpoint.ckpt`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/tests/data/mace_model/model_config.json` & `physicsml-0.2.1/tests/data/mace_model/model_config.json`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/tests/data/nequip_model/featurisation_metadata.json` & `physicsml-0.2.1/tests/data/nequip_model/featurisation_metadata.json`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/tests/data/nequip_model/model_artefacts/module_checkpoint.ckpt` & `physicsml-0.2.1/tests/data/nequip_model/model_artefacts/module_checkpoint.ckpt`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/tests/data/nequip_model/model_config.json` & `physicsml-0.2.1/tests/data/nequip_model/model_config.json`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/tests/openeye/conftest.py` & `physicsml-0.2.1/tests/openeye/conftest.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/tests/openeye/core/data/test_datamodule.py` & `physicsml-0.2.1/tests/openeye/core/data/test_datamodule.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/tests/openeye/core/data/test_graph_dataset.py` & `physicsml-0.2.1/tests/openeye/core/data/test_graph_dataset.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/tests/openeye/core/featurisation/test_physicsml_featurisation.py` & `physicsml-0.2.1/tests/openeye/core/featurisation/test_physicsml_featurisation.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/tests/openeye/integration/prism/test_egnn_prism.py` & `physicsml-0.2.1/tests/openeye/integration/prism/test_egnn_prism.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/tests/openeye/integration/training/egnn/test_egnn.py` & `physicsml-0.2.1/tests/openeye/integration/training/egnn/test_egnn.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/tests/openmm/conftest.py` & `physicsml-0.2.1/tests/openmm/conftest.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/tests/openmm/test_openmm_ani.py` & `physicsml-0.2.1/tests/openmm/test_openmm_ani.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/tests/openmm/test_openmm_egnn.py` & `physicsml-0.2.1/tests/openmm/test_openmm_egnn.py`

 * *Files 14% similar despite different names*

```diff
@@ -235,14 +235,126 @@
                 torch.float64,
             ),
             torchscript_module_64(pos.double()) * 627,
             rtol=1e-7,
         )
 
 
+def test_openmm_egnn_cell(featurised_ani1x_atomic_nums):
+    dataset_feated, x_features, featurisation_metadata = featurised_ani1x_atomic_nums
+
+    # specify the model config
+    model_config = {
+        "name": "egnn_model",  # the model name
+        "config": {
+            "x_features": x_features,
+            "y_features": [
+                "wb97x_dz.energy",
+                "wb97x_dz.forces",
+            ],
+            "datamodule": {
+                "y_graph_scalars": ["wb97x_dz.energy"],
+                "y_node_vector": "wb97x_dz.forces",
+                "num_elements": 4,
+                "cut_off": 5.0,
+            },
+            "num_node_feats": 4,
+            "num_edge_feats": 0,
+            "num_layers": 4,
+            "num_layers_phi": 2,
+            "c_hidden": 12,
+            "dropout": 0.1,
+            "compute_forces": True,
+            "mlp_activation": "SiLU",
+            "y_graph_scalars_loss_config": {
+                "name": "MSELoss",
+                "weight": 1.0,
+            },
+            "y_node_vector_loss_config": {
+                "name": "MSELoss",
+                "weight": 1.0,
+            },
+        },
+    }
+
+    model = mz.load_from_dict(model_config)
+
+    with tempfile.TemporaryDirectory() as tmpdir:
+        model.train(
+            train_data=dataset_feated,
+            validation_data=dataset_feated,
+            trainer_config={
+                "accelerator": "gpu" if torch.cuda.is_available() else "cpu",
+                "max_epochs": 10,
+                "default_root_dir": tmpdir,
+                "precision": "64",
+            },
+            datamodule_config={
+                "train": {"batch_size": 4},
+                "num_workers": 0,
+            },
+        )
+
+        core.save_model(model, tmpdir, featurisation_metadata)
+
+        openmm_module = deepcopy(model).to_openmm(  # type: ignore
+            physicsml_model=model,
+            featurisation_metadata=featurisation_metadata,
+            atom_list=[6, 6, 6, 6, 6, 6, 6, 6, 6, 6, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1],
+            precision="64",
+            cell=[[32, 0, 0], [0, 32, 0], [0, 0, 32]],
+            pbc=(True, True, True),
+        )
+        torchscript_module = to_openmm_torchscript(
+            model_path=tmpdir,
+            atom_list=[6, 6, 6, 6, 6, 6, 6, 6, 6, 6, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1],
+            device="cuda" if torch.cuda.is_available() else "cpu",
+            precision="64",
+            cell=[[32, 0, 0], [0, 32, 0], [0, 0, 32]],
+            pbc=(True, True, True),
+        )
+
+    preds = model.predict(
+        dataset_feated,
+        trainer_config={"accelerator": "gpu" if torch.cuda.is_available() else "cpu"},
+    )
+
+    assert "egnn_model::wb97x_dz.energy" in preds.keys()
+    assert len(preds) == 2
+    assert len(preds["egnn_model::wb97x_dz.energy"]) == 88
+
+    pos = torch.tensor(dataset_feated[0]["physicsml_coordinates"]).double()
+    pos = pos.to("cuda" if torch.cuda.is_available() else "cpu")
+    pos.requires_grad = True
+    out = openmm_module(pos)
+    ts_out = torchscript_module(pos)
+
+    assert torch.allclose(
+        torch.tensor(preds["egnn_model::wb97x_dz.energy"][0] * 627).type(torch.float64),
+        ts_out * 627,
+        rtol=1e-7,
+    )
+    assert torch.allclose(out * 627, ts_out * 627, rtol=1e-7)
+
+    with torch.enable_grad():
+        for _ in range(10):
+            energy = torchscript_module(pos)
+            grad_outputs = [torch.ones_like(energy)]
+            torch.autograd.grad(
+                outputs=[energy],  # [n_graphs, ]
+                inputs=[pos],  # [n_nodes, 3]
+                grad_outputs=grad_outputs,
+                retain_graph=False,  # Make sure the graph is not destroyed during training
+                create_graph=False,  # Create graph for second derivative
+                allow_unused=True,
+            )[
+                0
+            ]  # [n_nodes, 3]
+
+
 def test_openmm_egnn_boxvectors(featurised_ani1x_atomic_nums):
     dataset_feated, x_features, featurisation_metadata = featurised_ani1x_atomic_nums
     # specify the model config
     model_config = {
         "name": "egnn_model",  # the model name
         "config": {
             "x_features": x_features,
```

### Comparing `physicsml-0.2.0/tests/openmm/test_openmm_mace.py` & `physicsml-0.2.1/tests/openmm/test_openmm_nequip.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,40 +4,43 @@
 import molflux.core as core
 import molflux.modelzoo as mz
 import torch
 
 from physicsml.plugins.openmm.load import to_openmm_torchscript
 
 
-def test_openmm_mace(featurised_ani1x_atomic_nums):
+def test_openmm_nequip(featurised_ani1x_atomic_nums):
     dataset_feated, x_features, featurisation_metadata = featurised_ani1x_atomic_nums
 
     # specify the model config
     model_config = {
-        "name": "mace_model",  # the model name
+        "name": "nequip_model",  # the model name
         "config": {
             "x_features": x_features,
             "y_features": [
                 "wb97x_dz.energy",
                 "wb97x_dz.forces",
             ],
             "datamodule": {
                 "y_graph_scalars": ["wb97x_dz.energy"],
                 "y_node_vector": "wb97x_dz.forces",
                 "num_elements": 4,
             },
             "num_node_feats": 4,
+            "num_layers": 2,
+            "max_ell": 2,
+            "parity": True,
+            "num_features": 4,
+            "mlp_irreps": "8x0e",
             "num_bessel": 8,
+            "bessel_basis_trainable": True,
             "num_polynomial_cutoff": 6,
-            "max_ell": 2,
-            "num_interactions": 2,
-            "hidden_irreps": "4x0e + 4x1o",
-            "mlp_irreps": "5x0e",
+            "self_connection": True,
+            "resnet": True,
             "avg_num_neighbours": 10.0,
-            "correlation": 2,
             "compute_forces": True,
             "y_graph_scalars_loss_config": {
                 "name": "MSELoss",
                 "weight": 1.0,
             },
             "y_node_vector_loss_config": {
                 "name": "MSELoss",
@@ -89,70 +92,73 @@
         )
 
     preds = model.predict(
         dataset_feated,
         trainer_config={"accelerator": "gpu" if torch.cuda.is_available() else "cpu"},
     )
 
-    assert "mace_model::wb97x_dz.energy" in preds.keys()
+    assert "nequip_model::wb97x_dz.energy" in preds.keys()
     assert len(preds) == 2
-    assert len(preds["mace_model::wb97x_dz.energy"]) == 88
+    assert len(preds["nequip_model::wb97x_dz.energy"]) == 88
 
     pos = torch.tensor(dataset_feated[0]["physicsml_coordinates"])
     out = openmm_module(pos)
     ts_out = torchscript_module(pos)
 
     assert torch.allclose(
-        torch.tensor(preds["mace_model::wb97x_dz.energy"][0] * 627),
+        torch.tensor(preds["nequip_model::wb97x_dz.energy"][0] * 627),
         ts_out * 627,
         rtol=1e-7,
     )
     assert torch.allclose(out * 627, ts_out * 627, rtol=1e-7)
 
     for _ in range(20):
         assert torch.allclose(
-            torch.tensor(preds["mace_model::wb97x_dz.energy"][0] * 627),
+            torch.tensor(preds["nequip_model::wb97x_dz.energy"][0] * 627),
             torchscript_module_32(pos.float()) * 627,
             rtol=1e-7,
         )
         assert torch.allclose(
-            torch.tensor(preds["mace_model::wb97x_dz.energy"][0] * 627).type(
+            torch.tensor(preds["nequip_model::wb97x_dz.energy"][0] * 627).type(
                 torch.float64,
             ),
             torchscript_module_64(pos.double()) * 627,
             rtol=1e-7,
         )
 
 
-def test_openmm_mace_64(featurised_ani1x_atomic_nums):
+def test_openmm_nequip_64(featurised_ani1x_atomic_nums):
     dataset_feated, x_features, featurisation_metadata = featurised_ani1x_atomic_nums
 
     # specify the model config
     model_config = {
-        "name": "mace_model",  # the model name
+        "name": "nequip_model",  # the model name
         "config": {
             "x_features": x_features,
             "y_features": [
                 "wb97x_dz.energy",
                 "wb97x_dz.forces",
             ],
             "datamodule": {
                 "y_graph_scalars": ["wb97x_dz.energy"],
                 "y_node_vector": "wb97x_dz.forces",
                 "num_elements": 4,
             },
             "num_node_feats": 4,
+            "num_layers": 2,
+            "max_ell": 2,
+            "parity": True,
+            "num_features": 4,
+            "mlp_irreps": "8x0e",
             "num_bessel": 8,
+            "bessel_basis_trainable": True,
             "num_polynomial_cutoff": 6,
-            "max_ell": 2,
-            "num_interactions": 2,
-            "hidden_irreps": "4x0e + 4x1o",
-            "mlp_irreps": "5x0e",
+            "self_connection": True,
+            "resnet": True,
             "avg_num_neighbours": 10.0,
-            "correlation": 2,
             "compute_forces": True,
             "y_graph_scalars_loss_config": {
                 "name": "MSELoss",
                 "weight": 1.0,
             },
             "y_node_vector_loss_config": {
                 "name": "MSELoss",
@@ -207,70 +213,194 @@
         )
 
     preds = model.predict(
         dataset_feated,
         trainer_config={"accelerator": "gpu" if torch.cuda.is_available() else "cpu"},
     )
 
-    assert "mace_model::wb97x_dz.energy" in preds.keys()
+    assert "nequip_model::wb97x_dz.energy" in preds.keys()
     assert len(preds) == 2
-    assert len(preds["mace_model::wb97x_dz.energy"]) == 88
+    assert len(preds["nequip_model::wb97x_dz.energy"]) == 88
 
     pos = torch.tensor(dataset_feated[0]["physicsml_coordinates"]).double()
     out = openmm_module(pos)
     ts_out = torchscript_module(pos)
 
     assert torch.allclose(
-        torch.tensor(preds["mace_model::wb97x_dz.energy"][0] * 627).type(torch.float64),
+        torch.tensor(preds["nequip_model::wb97x_dz.energy"][0] * 627).type(
+            torch.float64,
+        ),
         ts_out * 627,
         rtol=1e-7,
     )
     assert torch.allclose(out * 627, ts_out * 627, rtol=1e-7)
 
     for _ in range(20):
         assert torch.allclose(
-            torch.tensor(preds["mace_model::wb97x_dz.energy"][0] * 627),
+            torch.tensor(preds["nequip_model::wb97x_dz.energy"][0] * 627),
             torchscript_module_32(pos.float()) * 627,
             rtol=1e-7,
         )
         assert torch.allclose(
-            torch.tensor(preds["mace_model::wb97x_dz.energy"][0] * 627).type(
+            torch.tensor(preds["nequip_model::wb97x_dz.energy"][0] * 627).type(
                 torch.float64,
             ),
             torchscript_module_64(pos.double()) * 627,
             rtol=1e-7,
         )
 
 
-def test_openmm_mace_boxvectors(featurised_ani1x_atomic_nums):
+def test_openmm_nequip_cell(featurised_ani1x_atomic_nums):
     dataset_feated, x_features, featurisation_metadata = featurised_ani1x_atomic_nums
+
+    # specify the model config
     model_config = {
-        "name": "mace_model",  # the model name
+        "name": "nequip_model",  # the model name
+        "config": {
+            "x_features": x_features,
+            "y_features": [
+                "wb97x_dz.energy",
+                "wb97x_dz.forces",
+            ],
+            "datamodule": {
+                "y_graph_scalars": ["wb97x_dz.energy"],
+                "y_node_vector": "wb97x_dz.forces",
+                "num_elements": 4,
+            },
+            "num_node_feats": 4,
+            "num_layers": 2,
+            "max_ell": 2,
+            "parity": True,
+            "num_features": 4,
+            "mlp_irreps": "8x0e",
+            "num_bessel": 8,
+            "bessel_basis_trainable": True,
+            "num_polynomial_cutoff": 6,
+            "self_connection": True,
+            "resnet": True,
+            "avg_num_neighbours": 10.0,
+            "compute_forces": True,
+            "y_graph_scalars_loss_config": {
+                "name": "MSELoss",
+                "weight": 1.0,
+            },
+            "y_node_vector_loss_config": {
+                "name": "MSELoss",
+                "weight": 1.0,
+            },
+        },
+    }
+
+    model = mz.load_from_dict(model_config)
+
+    with tempfile.TemporaryDirectory() as tmpdir:
+        model.train(
+            train_data=dataset_feated,
+            validation_data=dataset_feated,
+            trainer_config={
+                "accelerator": "gpu" if torch.cuda.is_available() else "cpu",
+                "max_epochs": 10,
+                "default_root_dir": tmpdir,
+                "precision": "64",
+            },
+            datamodule_config={
+                "train": {"batch_size": 4},
+                "num_workers": 0,
+            },
+        )
+
+        core.save_model(model, tmpdir, featurisation_metadata)
+
+        openmm_module = deepcopy(model).to_openmm(  # type: ignore
+            physicsml_model=model,
+            featurisation_metadata=featurisation_metadata,
+            atom_list=[6, 6, 6, 6, 6, 6, 6, 6, 6, 6, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1],
+            precision="64",
+            cell=[[32, 0, 0], [0, 32, 0], [0, 0, 32]],
+            pbc=(True, True, True),
+        )
+        torchscript_module = to_openmm_torchscript(
+            model_path=tmpdir,
+            atom_list=[6, 6, 6, 6, 6, 6, 6, 6, 6, 6, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1],
+            device="cuda" if torch.cuda.is_available() else "cpu",
+            precision="64",
+            cell=[[32, 0, 0], [0, 32, 0], [0, 0, 32]],
+            pbc=(True, True, True),
+        )
+
+    preds = model.predict(
+        dataset_feated,
+        trainer_config={"accelerator": "gpu" if torch.cuda.is_available() else "cpu"},
+    )
+
+    assert "nequip_model::wb97x_dz.energy" in preds.keys()
+    assert len(preds) == 2
+    assert len(preds["nequip_model::wb97x_dz.energy"]) == 88
+
+    pos = torch.tensor(dataset_feated[0]["physicsml_coordinates"]).double()
+    pos = pos.to("cuda" if torch.cuda.is_available() else "cpu")
+    pos.requires_grad = True
+    out = openmm_module(pos)
+    ts_out = torchscript_module(pos)
+
+    assert torch.allclose(
+        torch.tensor(preds["nequip_model::wb97x_dz.energy"][0] * 627).type(
+            torch.float64,
+        ),
+        ts_out * 627,
+        rtol=1e-7,
+    )
+    assert torch.allclose(out * 627, ts_out * 627, rtol=1e-7)
+
+    with torch.enable_grad():
+        for _ in range(10):
+            energy = torchscript_module(pos)
+            grad_outputs = [torch.ones_like(energy)]
+            torch.autograd.grad(
+                outputs=[energy],  # [n_graphs, ]
+                inputs=[pos],  # [n_nodes, 3]
+                grad_outputs=grad_outputs,
+                retain_graph=False,  # Make sure the graph is not destroyed during training
+                create_graph=False,  # Create graph for second derivative
+                allow_unused=True,
+            )[
+                0
+            ]  # [n_nodes, 3]
+
+
+def test_openmm_nequip_boxvectors(featurised_ani1x_atomic_nums):
+    dataset_feated, x_features, featurisation_metadata = featurised_ani1x_atomic_nums
+    # specify the model config
+    model_config = {
+        "name": "nequip_model",  # the model name
         "config": {
             "x_features": x_features,
             "y_features": [
                 "wb97x_dz.energy",
                 "wb97x_dz.forces",
             ],
             "datamodule": {
                 "y_graph_scalars": ["wb97x_dz.energy"],
                 "y_node_vector": "wb97x_dz.forces",
                 "num_elements": 4,
                 "cell": [[5.0, 0.0, 0.0], [0.0, 5.0, 0.0], [0.0, 0.0, 5.0]],
                 "pbc": (True, True, True),
             },
             "num_node_feats": 4,
+            "num_layers": 2,
+            "max_ell": 2,
+            "parity": True,
+            "num_features": 4,
+            "mlp_irreps": "8x0e",
             "num_bessel": 8,
+            "bessel_basis_trainable": True,
             "num_polynomial_cutoff": 6,
-            "max_ell": 2,
-            "num_interactions": 2,
-            "hidden_irreps": "4x0e + 4x1o",
-            "mlp_irreps": "5x0e",
+            "self_connection": True,
+            "resnet": True,
             "avg_num_neighbours": 10.0,
-            "correlation": 2,
             "compute_forces": True,
             "y_graph_scalars_loss_config": {
                 "name": "MSELoss",
                 "weight": 1.0,
             },
             "y_node_vector_loss_config": {
                 "name": "MSELoss",
@@ -316,35 +446,35 @@
             precision="64",
             device="cuda" if torch.cuda.is_available() else "cpu",
         )
     preds = model.predict(
         dataset_feated,
         trainer_config={"accelerator": "gpu" if torch.cuda.is_available() else "cpu"},
     )
-    assert "mace_model::wb97x_dz.energy" in preds.keys()
+    assert "nequip_model::wb97x_dz.energy" in preds.keys()
     assert len(preds) == 2
-    assert len(preds["mace_model::wb97x_dz.energy"]) == 88
+    assert len(preds["nequip_model::wb97x_dz.energy"]) == 88
     pos = torch.tensor(dataset_feated[0]["physicsml_coordinates"])
     cell = torch.tensor(model.model_config.datamodule.cell)  # type: ignore
     out = openmm_module(pos, cell)
     ts_out = torchscript_module(pos, cell)
     assert torch.allclose(
-        torch.tensor(preds["mace_model::wb97x_dz.energy"][0] * 627),
+        torch.tensor(preds["nequip_model::wb97x_dz.energy"][0] * 627),
         ts_out * 627,
         rtol=1e-7,
     )
     assert torch.allclose(out * 627, ts_out * 627, rtol=1e-7)
     ts_out_diff_cell = torchscript_module(pos, 0.5 * cell)
     assert not torch.allclose(ts_out_diff_cell * 627, ts_out * 627, rtol=1e-7)
     for _ in range(20):
         assert torch.allclose(
-            torch.tensor(preds["mace_model::wb97x_dz.energy"][0] * 627),
+            torch.tensor(preds["nequip_model::wb97x_dz.energy"][0] * 627),
             torchscript_module_32(pos.float(), cell.float()) * 627,
             rtol=1e-7,
         )
         assert torch.allclose(
-            torch.tensor(preds["mace_model::wb97x_dz.energy"][0] * 627).type(
+            torch.tensor(preds["nequip_model::wb97x_dz.energy"][0] * 627).type(
                 torch.float64,
             ),
             torchscript_module_64(pos.double(), cell.double()) * 627,
             rtol=1e-7,
         )
```

### Comparing `physicsml-0.2.0/tests/openmm/test_openmm_nequip.py` & `physicsml-0.2.1/tests/openmm/test_openmm_mace.py`

 * *Files 25% similar despite different names*

```diff
@@ -4,43 +4,40 @@
 import molflux.core as core
 import molflux.modelzoo as mz
 import torch
 
 from physicsml.plugins.openmm.load import to_openmm_torchscript
 
 
-def test_openmm_nequip(featurised_ani1x_atomic_nums):
+def test_openmm_mace(featurised_ani1x_atomic_nums):
     dataset_feated, x_features, featurisation_metadata = featurised_ani1x_atomic_nums
 
     # specify the model config
     model_config = {
-        "name": "nequip_model",  # the model name
+        "name": "mace_model",  # the model name
         "config": {
             "x_features": x_features,
             "y_features": [
                 "wb97x_dz.energy",
                 "wb97x_dz.forces",
             ],
             "datamodule": {
                 "y_graph_scalars": ["wb97x_dz.energy"],
                 "y_node_vector": "wb97x_dz.forces",
                 "num_elements": 4,
             },
             "num_node_feats": 4,
-            "num_layers": 2,
-            "max_ell": 2,
-            "parity": True,
-            "num_features": 4,
-            "mlp_irreps": "8x0e",
             "num_bessel": 8,
-            "bessel_basis_trainable": True,
             "num_polynomial_cutoff": 6,
-            "self_connection": True,
-            "resnet": True,
+            "max_ell": 2,
+            "num_interactions": 2,
+            "hidden_irreps": "4x0e + 4x1o",
+            "mlp_irreps": "5x0e",
             "avg_num_neighbours": 10.0,
+            "correlation": 2,
             "compute_forces": True,
             "y_graph_scalars_loss_config": {
                 "name": "MSELoss",
                 "weight": 1.0,
             },
             "y_node_vector_loss_config": {
                 "name": "MSELoss",
@@ -92,73 +89,70 @@
         )
 
     preds = model.predict(
         dataset_feated,
         trainer_config={"accelerator": "gpu" if torch.cuda.is_available() else "cpu"},
     )
 
-    assert "nequip_model::wb97x_dz.energy" in preds.keys()
+    assert "mace_model::wb97x_dz.energy" in preds.keys()
     assert len(preds) == 2
-    assert len(preds["nequip_model::wb97x_dz.energy"]) == 88
+    assert len(preds["mace_model::wb97x_dz.energy"]) == 88
 
     pos = torch.tensor(dataset_feated[0]["physicsml_coordinates"])
     out = openmm_module(pos)
     ts_out = torchscript_module(pos)
 
     assert torch.allclose(
-        torch.tensor(preds["nequip_model::wb97x_dz.energy"][0] * 627),
+        torch.tensor(preds["mace_model::wb97x_dz.energy"][0] * 627),
         ts_out * 627,
         rtol=1e-7,
     )
     assert torch.allclose(out * 627, ts_out * 627, rtol=1e-7)
 
     for _ in range(20):
         assert torch.allclose(
-            torch.tensor(preds["nequip_model::wb97x_dz.energy"][0] * 627),
+            torch.tensor(preds["mace_model::wb97x_dz.energy"][0] * 627),
             torchscript_module_32(pos.float()) * 627,
             rtol=1e-7,
         )
         assert torch.allclose(
-            torch.tensor(preds["nequip_model::wb97x_dz.energy"][0] * 627).type(
+            torch.tensor(preds["mace_model::wb97x_dz.energy"][0] * 627).type(
                 torch.float64,
             ),
             torchscript_module_64(pos.double()) * 627,
             rtol=1e-7,
         )
 
 
-def test_openmm_nequip_64(featurised_ani1x_atomic_nums):
+def test_openmm_mace_64(featurised_ani1x_atomic_nums):
     dataset_feated, x_features, featurisation_metadata = featurised_ani1x_atomic_nums
 
     # specify the model config
     model_config = {
-        "name": "nequip_model",  # the model name
+        "name": "mace_model",  # the model name
         "config": {
             "x_features": x_features,
             "y_features": [
                 "wb97x_dz.energy",
                 "wb97x_dz.forces",
             ],
             "datamodule": {
                 "y_graph_scalars": ["wb97x_dz.energy"],
                 "y_node_vector": "wb97x_dz.forces",
                 "num_elements": 4,
             },
             "num_node_feats": 4,
-            "num_layers": 2,
-            "max_ell": 2,
-            "parity": True,
-            "num_features": 4,
-            "mlp_irreps": "8x0e",
             "num_bessel": 8,
-            "bessel_basis_trainable": True,
             "num_polynomial_cutoff": 6,
-            "self_connection": True,
-            "resnet": True,
+            "max_ell": 2,
+            "num_interactions": 2,
+            "hidden_irreps": "4x0e + 4x1o",
+            "mlp_irreps": "5x0e",
             "avg_num_neighbours": 10.0,
+            "correlation": 2,
             "compute_forces": True,
             "y_graph_scalars_loss_config": {
                 "name": "MSELoss",
                 "weight": 1.0,
             },
             "y_node_vector_loss_config": {
                 "name": "MSELoss",
@@ -213,76 +207,183 @@
         )
 
     preds = model.predict(
         dataset_feated,
         trainer_config={"accelerator": "gpu" if torch.cuda.is_available() else "cpu"},
     )
 
-    assert "nequip_model::wb97x_dz.energy" in preds.keys()
+    assert "mace_model::wb97x_dz.energy" in preds.keys()
     assert len(preds) == 2
-    assert len(preds["nequip_model::wb97x_dz.energy"]) == 88
+    assert len(preds["mace_model::wb97x_dz.energy"]) == 88
 
     pos = torch.tensor(dataset_feated[0]["physicsml_coordinates"]).double()
     out = openmm_module(pos)
     ts_out = torchscript_module(pos)
 
     assert torch.allclose(
-        torch.tensor(preds["nequip_model::wb97x_dz.energy"][0] * 627).type(
-            torch.float64,
-        ),
+        torch.tensor(preds["mace_model::wb97x_dz.energy"][0] * 627).type(torch.float64),
         ts_out * 627,
         rtol=1e-7,
     )
     assert torch.allclose(out * 627, ts_out * 627, rtol=1e-7)
 
     for _ in range(20):
         assert torch.allclose(
-            torch.tensor(preds["nequip_model::wb97x_dz.energy"][0] * 627),
+            torch.tensor(preds["mace_model::wb97x_dz.energy"][0] * 627),
             torchscript_module_32(pos.float()) * 627,
             rtol=1e-7,
         )
         assert torch.allclose(
-            torch.tensor(preds["nequip_model::wb97x_dz.energy"][0] * 627).type(
+            torch.tensor(preds["mace_model::wb97x_dz.energy"][0] * 627).type(
                 torch.float64,
             ),
             torchscript_module_64(pos.double()) * 627,
             rtol=1e-7,
         )
 
 
-def test_openmm_nequip_boxvectors(featurised_ani1x_atomic_nums):
+def test_openmm_mace_cell(featurised_ani1x_atomic_nums):
     dataset_feated, x_features, featurisation_metadata = featurised_ani1x_atomic_nums
+
     # specify the model config
     model_config = {
-        "name": "nequip_model",  # the model name
+        "name": "mace_model",  # the model name
+        "config": {
+            "x_features": x_features,
+            "y_features": [
+                "wb97x_dz.energy",
+                "wb97x_dz.forces",
+            ],
+            "datamodule": {
+                "y_graph_scalars": ["wb97x_dz.energy"],
+                "y_node_vector": "wb97x_dz.forces",
+                "num_elements": 4,
+            },
+            "num_node_feats": 4,
+            "num_bessel": 8,
+            "num_polynomial_cutoff": 6,
+            "max_ell": 2,
+            "num_interactions": 2,
+            "hidden_irreps": "4x0e + 4x1o",
+            "mlp_irreps": "5x0e",
+            "avg_num_neighbours": 10.0,
+            "correlation": 2,
+            "compute_forces": True,
+            "y_graph_scalars_loss_config": {
+                "name": "MSELoss",
+                "weight": 1.0,
+            },
+            "y_node_vector_loss_config": {
+                "name": "MSELoss",
+                "weight": 1.0,
+            },
+        },
+    }
+
+    model = mz.load_from_dict(model_config)
+
+    with tempfile.TemporaryDirectory() as tmpdir:
+        model.train(
+            train_data=dataset_feated,
+            validation_data=dataset_feated,
+            trainer_config={
+                "accelerator": "gpu" if torch.cuda.is_available() else "cpu",
+                "max_epochs": 10,
+                "default_root_dir": tmpdir,
+                "precision": "64",
+            },
+            datamodule_config={
+                "train": {"batch_size": 4},
+                "num_workers": 0,
+            },
+        )
+
+        core.save_model(model, tmpdir, featurisation_metadata)
+
+        openmm_module = deepcopy(model).to_openmm(  # type: ignore
+            physicsml_model=model,
+            featurisation_metadata=featurisation_metadata,
+            atom_list=[6, 6, 6, 6, 6, 6, 6, 6, 6, 6, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1],
+            precision="64",
+            cell=[[32, 0, 0], [0, 32, 0], [0, 0, 32]],
+            pbc=(True, True, True),
+        )
+        torchscript_module = to_openmm_torchscript(
+            model_path=tmpdir,
+            atom_list=[6, 6, 6, 6, 6, 6, 6, 6, 6, 6, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1],
+            device="cuda" if torch.cuda.is_available() else "cpu",
+            precision="64",
+            cell=[[32, 0, 0], [0, 32, 0], [0, 0, 32]],
+            pbc=(True, True, True),
+        )
+
+    preds = model.predict(
+        dataset_feated,
+        trainer_config={"accelerator": "gpu" if torch.cuda.is_available() else "cpu"},
+    )
+
+    assert "mace_model::wb97x_dz.energy" in preds.keys()
+    assert len(preds) == 2
+    assert len(preds["mace_model::wb97x_dz.energy"]) == 88
+
+    pos = torch.tensor(dataset_feated[0]["physicsml_coordinates"]).double()
+    pos = pos.to("cuda" if torch.cuda.is_available() else "cpu")
+    pos.requires_grad = True
+    out = openmm_module(pos)
+    ts_out = torchscript_module(pos)
+
+    assert torch.allclose(
+        torch.tensor(preds["mace_model::wb97x_dz.energy"][0] * 627).type(torch.float64),
+        ts_out * 627,
+        rtol=1e-7,
+    )
+    assert torch.allclose(out * 627, ts_out * 627, rtol=1e-7)
+
+    with torch.enable_grad():
+        for _ in range(10):
+            energy = torchscript_module(pos)
+            grad_outputs = [torch.ones_like(energy)]
+            torch.autograd.grad(
+                outputs=[energy],  # [n_graphs, ]
+                inputs=[pos],  # [n_nodes, 3]
+                grad_outputs=grad_outputs,
+                retain_graph=False,  # Make sure the graph is not destroyed during training
+                create_graph=False,  # Create graph for second derivative
+                allow_unused=True,
+            )[
+                0
+            ]  # [n_nodes, 3]
+
+
+def test_openmm_mace_boxvectors(featurised_ani1x_atomic_nums):
+    dataset_feated, x_features, featurisation_metadata = featurised_ani1x_atomic_nums
+    model_config = {
+        "name": "mace_model",  # the model name
         "config": {
             "x_features": x_features,
             "y_features": [
                 "wb97x_dz.energy",
                 "wb97x_dz.forces",
             ],
             "datamodule": {
                 "y_graph_scalars": ["wb97x_dz.energy"],
                 "y_node_vector": "wb97x_dz.forces",
                 "num_elements": 4,
                 "cell": [[5.0, 0.0, 0.0], [0.0, 5.0, 0.0], [0.0, 0.0, 5.0]],
                 "pbc": (True, True, True),
             },
             "num_node_feats": 4,
-            "num_layers": 2,
-            "max_ell": 2,
-            "parity": True,
-            "num_features": 4,
-            "mlp_irreps": "8x0e",
             "num_bessel": 8,
-            "bessel_basis_trainable": True,
             "num_polynomial_cutoff": 6,
-            "self_connection": True,
-            "resnet": True,
+            "max_ell": 2,
+            "num_interactions": 2,
+            "hidden_irreps": "4x0e + 4x1o",
+            "mlp_irreps": "5x0e",
             "avg_num_neighbours": 10.0,
+            "correlation": 2,
             "compute_forces": True,
             "y_graph_scalars_loss_config": {
                 "name": "MSELoss",
                 "weight": 1.0,
             },
             "y_node_vector_loss_config": {
                 "name": "MSELoss",
@@ -328,35 +429,35 @@
             precision="64",
             device="cuda" if torch.cuda.is_available() else "cpu",
         )
     preds = model.predict(
         dataset_feated,
         trainer_config={"accelerator": "gpu" if torch.cuda.is_available() else "cpu"},
     )
-    assert "nequip_model::wb97x_dz.energy" in preds.keys()
+    assert "mace_model::wb97x_dz.energy" in preds.keys()
     assert len(preds) == 2
-    assert len(preds["nequip_model::wb97x_dz.energy"]) == 88
+    assert len(preds["mace_model::wb97x_dz.energy"]) == 88
     pos = torch.tensor(dataset_feated[0]["physicsml_coordinates"])
     cell = torch.tensor(model.model_config.datamodule.cell)  # type: ignore
     out = openmm_module(pos, cell)
     ts_out = torchscript_module(pos, cell)
     assert torch.allclose(
-        torch.tensor(preds["nequip_model::wb97x_dz.energy"][0] * 627),
+        torch.tensor(preds["mace_model::wb97x_dz.energy"][0] * 627),
         ts_out * 627,
         rtol=1e-7,
     )
     assert torch.allclose(out * 627, ts_out * 627, rtol=1e-7)
     ts_out_diff_cell = torchscript_module(pos, 0.5 * cell)
     assert not torch.allclose(ts_out_diff_cell * 627, ts_out * 627, rtol=1e-7)
     for _ in range(20):
         assert torch.allclose(
-            torch.tensor(preds["nequip_model::wb97x_dz.energy"][0] * 627),
+            torch.tensor(preds["mace_model::wb97x_dz.energy"][0] * 627),
             torchscript_module_32(pos.float(), cell.float()) * 627,
             rtol=1e-7,
         )
         assert torch.allclose(
-            torch.tensor(preds["nequip_model::wb97x_dz.energy"][0] * 627).type(
+            torch.tensor(preds["mace_model::wb97x_dz.energy"][0] * 627).type(
                 torch.float64,
             ),
             torchscript_module_64(pos.double(), cell.double()) * 627,
             rtol=1e-7,
         )
```

### Comparing `physicsml-0.2.0/tests/openmm/test_openmm_nnp_potential.py` & `physicsml-0.2.1/tests/openmm/test_openmm_nnp_potential.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,25 @@
 # type: ignore
 from typing import Dict
 
 import pytest
 import torch
-from openmmml.mlpotential import MLPotential
 
-import openmm as mm
-import openmm.app as app
-from physicsml.plugins.openmm.physicsml_potential import (
-    PhysicsMLPotentialImplFactory,  # noqa F401
-)
+try:
+    from openmmml.mlpotential import MLPotential
+
+    import openmm as mm
+    import openmm.app as app
+    from physicsml.plugins.openmm.physicsml_potential import (
+        PhysicsMLPotentialImplFactory,  # noqa F401
+    )
+
+    OPENMM_ = True
+except:  # noqa
+    OPENMM_ = False
 
 NNP_MODELS = [
     {
         "model": "ANI",
         "model_path": "tests/data/ani_model",
         "total_value": -5265.576795347246,
         "mm_value": -159.59874317381482,
@@ -40,14 +46,15 @@
         "mm_value": -159.59874317381482,
         "mixed_value": -2176.9882577057383,
     },
 ]
 ALANINE_DIPEPTIDE_PATH = "tests/data/alanine-dipeptide-truncated.pdb"
 
 
+@pytest.mark.skipif(not OPENMM_, reason="no openmm")
 @pytest.mark.parametrize("model_properties", NNP_MODELS)
 def test_nnp_potential_system_cpu(
     model_properties: Dict,
     platform: str = "cpu",
 ) -> None:
     # fetch the .pdb file
     pdb = app.PDBFile(ALANINE_DIPEPTIDE_PATH)
@@ -77,14 +84,15 @@
 
     # get energy
     energy = mm_context.getState(getEnergy=True).getPotentialEnergy()
 
     assert energy._value == pytest.approx(model_properties["total_value"], 1e-4)
 
 
+@pytest.mark.skipif(not OPENMM_, reason="no openmm")
 @pytest.mark.skipif(not torch.cuda.is_available(), reason="no gpus")
 @pytest.mark.parametrize("model_properties", NNP_MODELS)
 def test_nnp_potential_system_gpu(
     model_properties: Dict,
     platform: str = "cuda",
 ) -> None:
     # fetch the .pdb file
@@ -115,14 +123,15 @@
 
     # get energy
     energy = mm_context.getState(getEnergy=True).getPotentialEnergy()
 
     assert energy._value == pytest.approx(model_properties["total_value"], 1e-4)
 
 
+@pytest.mark.skipif(not OPENMM_, reason="no openmm")
 @pytest.mark.parametrize("model_properties", NNP_MODELS)
 def test_nnp_mixed_potential_system_cpu(
     model_properties: str,
     platform: str = "cpu",
 ) -> None:
     pdb = app.PDBFile(ALANINE_DIPEPTIDE_PATH)
     # specify the amber force fields
@@ -171,14 +180,15 @@
     mm_energy = mm_context.getState(getEnergy=True).getPotentialEnergy()
     mixed_energy = mixed_context.getState(getEnergy=True).getPotentialEnergy()
 
     assert mm_energy._value == pytest.approx(model_properties["mm_value"], 1e-4)
     assert mixed_energy._value == pytest.approx(model_properties["mixed_value"], 1e-4)
 
 
+@pytest.mark.skipif(not OPENMM_, reason="no openmm")
 @pytest.mark.skipif(not torch.cuda.is_available(), reason="no gpus")
 @pytest.mark.parametrize("model_properties", NNP_MODELS)
 def test_nnp_mixed_potential_system_gpu(
     model_properties: str,
     platform: str = "cuda",
 ) -> None:
     pdb = app.PDBFile(ALANINE_DIPEPTIDE_PATH)
```

### Comparing `physicsml-0.2.0/tests/rdkit/conftest.py` & `physicsml-0.2.1/tests/rdkit/conftest.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/tests/rdkit/core/data/test_datamodule.py` & `physicsml-0.2.1/tests/rdkit/core/data/test_datamodule.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/tests/rdkit/core/data/test_graph_dataset.py` & `physicsml-0.2.1/tests/rdkit/core/data/test_graph_dataset.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/tests/rdkit/core/featurisation/test_physicsml_featurisation.py` & `physicsml-0.2.1/tests/rdkit/core/featurisation/test_physicsml_featurisation.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/tests/rdkit/integration/prism/test_allegro_prism.py` & `physicsml-0.2.1/tests/rdkit/integration/prism/test_allegro_prism.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/tests/rdkit/integration/prism/test_ani_prism.py` & `physicsml-0.2.1/tests/rdkit/integration/prism/test_ani_prism.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/tests/rdkit/integration/prism/test_egnn_prism.py` & `physicsml-0.2.1/tests/rdkit/integration/prism/test_egnn_prism.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/tests/rdkit/integration/prism/test_mace_prism.py` & `physicsml-0.2.1/tests/rdkit/integration/prism/test_mace_prism.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/tests/rdkit/integration/prism/test_nequip_prism.py` & `physicsml-0.2.1/tests/rdkit/integration/prism/test_nequip_prism.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/tests/rdkit/integration/training/allegro/test_allegro_energy_charges.py` & `physicsml-0.2.1/tests/rdkit/integration/training/allegro/test_allegro_energy_charges.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/tests/rdkit/integration/training/allegro/test_allegro_forces.py` & `physicsml-0.2.1/tests/rdkit/integration/training/allegro/test_allegro_forces.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/tests/rdkit/integration/training/allegro/test_allegro_mean_var.py` & `physicsml-0.2.1/tests/rdkit/integration/training/allegro/test_allegro_mean_var.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/tests/rdkit/integration/training/allegro/test_allergo.py` & `physicsml-0.2.1/tests/rdkit/integration/training/allegro/test_allergo.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/tests/rdkit/integration/training/ani/test_ani.py` & `physicsml-0.2.1/tests/rdkit/integration/training/ani/test_ani.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/tests/rdkit/integration/training/ani/test_ani_ensemble.py` & `physicsml-0.2.1/tests/rdkit/integration/training/ani/test_ani_ensemble.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/tests/rdkit/integration/training/ani/test_ani_forces.py` & `physicsml-0.2.1/tests/rdkit/integration/training/ani/test_ani_forces.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/tests/rdkit/integration/training/ani/test_ani_mean_var.py` & `physicsml-0.2.1/tests/rdkit/integration/training/ani/test_ani_mean_var.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/tests/rdkit/integration/training/egnn/test_adapter_egnn.py` & `physicsml-0.2.1/tests/rdkit/integration/training/egnn/test_adapter_egnn.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/tests/rdkit/integration/training/egnn/test_egnn.py` & `physicsml-0.2.1/tests/rdkit/integration/training/egnn/test_egnn.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/tests/rdkit/integration/training/egnn/test_egnn_energy_charges.py` & `physicsml-0.2.1/tests/rdkit/integration/training/egnn/test_egnn_energy_charges.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/tests/rdkit/integration/training/egnn/test_egnn_forces.py` & `physicsml-0.2.1/tests/rdkit/integration/training/egnn/test_egnn_forces.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/tests/rdkit/integration/training/egnn/test_egnn_mean_var.py` & `physicsml-0.2.1/tests/rdkit/integration/training/egnn/test_egnn_mean_var.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/tests/rdkit/integration/training/egnn/test_ssf_egnn.py` & `physicsml-0.2.1/tests/rdkit/integration/training/egnn/test_ssf_egnn.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/tests/rdkit/integration/training/mace/test_adapter_mace.py` & `physicsml-0.2.1/tests/rdkit/integration/training/mace/test_adapter_mace.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/tests/rdkit/integration/training/mace/test_mace.py` & `physicsml-0.2.1/tests/rdkit/integration/training/mace/test_mace.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/tests/rdkit/integration/training/mace/test_mace_energy_charges.py` & `physicsml-0.2.1/tests/rdkit/integration/training/mace/test_mace_energy_charges.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/tests/rdkit/integration/training/mace/test_mace_forces.py` & `physicsml-0.2.1/tests/rdkit/integration/training/mace/test_mace_forces.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/tests/rdkit/integration/training/mace/test_mace_mean_var.py` & `physicsml-0.2.1/tests/rdkit/integration/training/mace/test_mace_mean_var.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/tests/rdkit/integration/training/mace/test_ssf_mace.py` & `physicsml-0.2.1/tests/rdkit/integration/training/mace/test_ssf_mace.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/tests/rdkit/integration/training/nequip/test_adapter_nequip.py` & `physicsml-0.2.1/tests/rdkit/integration/training/nequip/test_adapter_nequip.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/tests/rdkit/integration/training/nequip/test_nequip.py` & `physicsml-0.2.1/tests/rdkit/integration/training/nequip/test_nequip.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/tests/rdkit/integration/training/nequip/test_nequip_energy_charges.py` & `physicsml-0.2.1/tests/rdkit/integration/training/nequip/test_nequip_energy_charges.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/tests/rdkit/integration/training/nequip/test_nequip_forces.py` & `physicsml-0.2.1/tests/rdkit/integration/training/nequip/test_nequip_forces.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/tests/rdkit/integration/training/nequip/test_nequip_mean_var.py` & `physicsml-0.2.1/tests/rdkit/integration/training/nequip/test_nequip_mean_var.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/tests/rdkit/integration/training/nequip/test_ssf_nequip.py` & `physicsml-0.2.1/tests/rdkit/integration/training/nequip/test_ssf_nequip.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/tests/rdkit/integration/training/tensor_net/test_tensor_net.py` & `physicsml-0.2.1/tests/rdkit/integration/training/tensor_net/test_tensor_net.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/tests/rdkit/integration/training/tensor_net/test_tensor_net_energy_charges.py` & `physicsml-0.2.1/tests/rdkit/integration/training/tensor_net/test_tensor_net_energy_charges.py`

 * *Files identical despite different names*

### Comparing `physicsml-0.2.0/tests/rdkit/integration/training/tensor_net/test_tensor_net_forces.py` & `physicsml-0.2.1/tests/rdkit/integration/training/tensor_net/test_tensor_net_forces.py`

 * *Files identical despite different names*


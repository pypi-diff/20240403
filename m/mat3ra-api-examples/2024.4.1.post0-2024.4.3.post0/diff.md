# Comparing `tmp/mat3ra-api-examples-2024.4.1.post0.tar.gz` & `tmp/mat3ra-api-examples-2024.4.3.post0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mat3ra-api-examples-2024.4.1.post0.tar", last modified: Mon Apr  1 22:44:12 2024, max compression
+gzip compressed data, was "mat3ra-api-examples-2024.4.3.post0.tar", last modified: Wed Apr  3 18:31:48 2024, max compression
```

## Comparing `mat3ra-api-examples-2024.4.1.post0.tar` & `mat3ra-api-examples-2024.4.3.post0.tar`

### file list

```diff
@@ -1,135 +1,138 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:44:12.146363 mat3ra-api-examples-2024.4.1.post0/
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:44:12.118363 mat3ra-api-examples-2024.4.1.post0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:44:12.122363 mat3ra-api-examples-2024.4.1.post0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/.github/workflows/check_links.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4311 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/.github/workflows/cicd.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/.github/workflows/zip_release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/.lycheeignore
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    10319 2024-04-01 22:44:12.146363 mat3ra-api-examples-2024.4.1.post0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9012 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:44:12.122363 mat3ra-api-examples-2024.4.1.post0/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:44:12.122363 mat3ra-api-examples-2024.4.1.post0/examples/assets/
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/examples/assets/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/examples/assets/Si.pz-vbc.UPF
--rw-r--r--   0 runner    (1001) docker     (127)     4003 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/examples/assets/bash_workflow_template.json
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/examples/assets/mp-978534.poscar
--rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/examples/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:44:12.126363 mat3ra-api-examples-2024.4.1.post0/examples/job/
--rw-r--r--   0 runner    (1001) docker     (127)     7697 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/examples/job/create_and_submit_job.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     4122 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/examples/job/create_and_submit_job.py
--rw-r--r--   0 runner    (1001) docker     (127)    15077 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/examples/job/get-file-from-job.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    10084 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/examples/job/get-file-from-job.py
--rw-r--r--   0 runner    (1001) docker     (127)    20232 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/examples/job/ml-train-model-predict-properties.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    11044 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/examples/job/ml-train-model-predict-properties.py
--rw-r--r--   0 runner    (1001) docker     (127)    21020 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/examples/job/run-simulations-and-extract-properties.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    12744 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/examples/job/run-simulations-and-extract-properties.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:44:12.126363 mat3ra-api-examples-2024.4.1.post0/examples/material/
--rw-r--r--   0 runner    (1001) docker     (127)     6934 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/examples/material/create_material.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     4029 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/examples/material/create_material.py
--rw-r--r--   0 runner    (1001) docker     (127)     6220 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/examples/material/get_materials_by_formula.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     3423 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/examples/material/get_materials_by_formula.py
--rw-r--r--   0 runner    (1001) docker     (127)     6044 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/examples/material/import_materials_from_materialsproject.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     3514 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/examples/material/import_materials_from_materialsproject.py
--rw-r--r--   0 runner    (1001) docker     (127)     6132 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/examples/material/upload_materials_from_file_poscar.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     3545 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/examples/material/upload_materials_from_file_poscar.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:44:12.126363 mat3ra-api-examples-2024.4.1.post0/examples/system/
--rw-r--r--   0 runner    (1001) docker     (127)     3859 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/examples/system/get_authentication_params.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/examples/system/get_authentication_params.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:44:12.130363 mat3ra-api-examples-2024.4.1.post0/examples/workflow/
--rw-r--r--   0 runner    (1001) docker     (127)     6714 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/examples/workflow/get_workflows.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     3683 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/examples/workflow/get_workflows.py
--rw-r--r--   0 runner    (1001) docker     (127)    11692 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/examples/workflow/qe_scf_calculation.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     6954 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/examples/workflow/qe_scf_calculation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:44:12.118363 mat3ra-api-examples-2024.4.1.post0/extra/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:44:12.130363 mat3ra-api-examples-2024.4.1.post0/extra/css/
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/extra/css/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:44:12.130363 mat3ra-api-examples-2024.4.1.post0/images/
--rw-r--r--   0 runner    (1001) docker     (127)   413869 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/images/reusable-kernel.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:44:12.142363 mat3ra-api-examples-2024.4.1.post0/mat3ra_api_examples.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10319 2024-04-01 22:44:12.000000 mat3ra-api-examples-2024.4.1.post0/mat3ra_api_examples.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4356 2024-04-01 22:44:12.000000 mat3ra-api-examples-2024.4.1.post0/mat3ra_api_examples.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 22:44:12.000000 mat3ra-api-examples-2024.4.1.post0/mat3ra_api_examples.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-01 22:44:12.000000 mat3ra-api-examples-2024.4.1.post0/mat3ra_api_examples.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-01 22:44:12.000000 mat3ra-api-examples-2024.4.1.post0/mat3ra_api_examples.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-01 22:44:12.000000 mat3ra-api-examples-2024.4.1.post0/mat3ra_api_examples.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/mkdocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:44:12.122363 mat3ra-api-examples-2024.4.1.post0/other/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:44:12.134363 mat3ra-api-examples-2024.4.1.post0/other/assets/
--rw-r--r--   0 runner    (1001) docker     (127)     5159 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/other/assets/README.md
--rw-r--r--   0 runner    (1001) docker     (127)   638208 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/other/assets/bitter-sweet.csv
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/other/assets/bittersweet_xgboost.pkl
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/other/assets/deepchem_smiles_vocab.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/other/assets/gamma_alumina_digne_et_al.poscar
--rwxr-xr-x   0 runner    (1001) docker     (127)    12157 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/other/assets/sci_adv_dean_data.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:44:12.134363 mat3ra-api-examples-2024.4.1.post0/other/experiments/
--rw-r--r--   0 runner    (1001) docker     (127)    25385 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/other/experiments/create_interface_with_min_energy_by_miller_indices.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    24590 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/other/experiments/create_interface_with_relaxation_alignn.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    24267 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/other/experiments/create_interface_with_relaxation_ase_emt.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    24750 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/other/experiments/create_interface_with_relaxation_matgl_m3gnet.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:44:12.134363 mat3ra-api-examples-2024.4.1.post0/other/experiments/uploads/
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/other/experiments/uploads/Gr.json
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/other/experiments/uploads/Ni.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:44:12.134363 mat3ra-api-examples-2024.4.1.post0/other/jarvis/
--rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/other/jarvis/import_material_from_jarvis_db_entry.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    15663 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/other/jarvis/run_job_using_material_from_jarvis_db.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:44:12.134363 mat3ra-api-examples-2024.4.1.post0/other/job/
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/other/job/Smiles_Generation_Markov_Chain.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    11316 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/other/job/Smiles_Generation_Markov_Chain.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:44:12.134363 mat3ra-api-examples-2024.4.1.post0/other/jupyterlite/
--rw-r--r--   0 runner    (1001) docker     (127)     7503 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/other/jupyterlite/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:44:12.134363 mat3ra-api-examples-2024.4.1.post0/other/machine_learning/
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/other/machine_learning/Classification_of_Bitterness_XGBoost.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    18602 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/other/machine_learning/Classification_of_Bitterness_XGBoost.py
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/other/machine_learning/Prediction_of_Perovskite_Unit_Cell_Volume.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    11454 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/other/machine_learning/Prediction_of_Perovskite_Unit_Cell_Volume.py
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/other/machine_learning/neural_network_train.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    19205 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/other/machine_learning/neural_network_train.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:44:12.138363 mat3ra-api-examples-2024.4.1.post0/other/materials_designer/
--rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/other/materials_designer/Introduction.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/other/materials_designer/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)    16625 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/other/materials_designer/create_interface_with_min_strain_zsl.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    29841 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/other/materials_designer/create_interface_with_relaxation_ase_emt.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     8402 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/other/materials_designer/import_material_from_jarvis_db_entry.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     8443 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/other/materials_designer/import_materials_from_files.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:44:12.138363 mat3ra-api-examples-2024.4.1.post0/other/materials_designer/src/
--rw-r--r--   0 runner    (1001) docker     (127)    11964 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/other/materials_designer/src/pymatgen_coherent_interface_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)    12408 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/other/materials_designer/src/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:44:12.138363 mat3ra-api-examples-2024.4.1.post0/other/materials_designer/uploads/
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/other/materials_designer/uploads/README
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:44:12.138363 mat3ra-api-examples-2024.4.1.post0/other/materialsproject/
--rw-r--r--   0 runner    (1001) docker     (127)     9232 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/other/materialsproject/api_interoperability_showcase.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     5708 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/other/materialsproject/api_interoperability_showcase.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:44:12.138363 mat3ra-api-examples-2024.4.1.post0/other/python_transformations/
--rw-r--r--   0 runner    (1001) docker     (127)     8929 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/other/python_transformations/1_layer_on_substrate.py
--rw-r--r--   0 runner    (1001) docker     (127)    19706 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/other/python_transformations/2_strain_matching.py
--rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/other/python_transformations/3_imports.py
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/other/python_transformations/4_custom_transformation.py
--rw-r--r--   0 runner    (1001) docker     (127)      677 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/other/python_transformations/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:44:12.142363 mat3ra-api-examples-2024.4.1.post0/other/webinar/
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/other/webinar/adsorption-study.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    10676 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/other/webinar/adsorption-study.py
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/other/webinar/generate-al2o3-slab-structures.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     8820 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/other/webinar/generate-al2o3-slab-structures.py
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/other/webinar/predict_with_machine_learning.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     5649 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/other/webinar/predict_with_machine_learning.py
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/other/webinar/wulff-construction-surface-energy-study-cu.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    15454 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/other/webinar/wulff-construction-surface-energy-study-cu.py
--rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:44:12.142363 mat3ra-api-examples-2024.4.1.post0/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1669 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/scripts/change-branch-in-urls.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/scripts/env.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)     2267 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/scripts/render-notebooks.sh
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 22:44:12.146363 mat3ra-api-examples-2024.4.1.post0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:44:12.142363 mat3ra-api-examples-2024.4.1.post0/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7875 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/utils/generic.py
--rw-r--r--   0 runner    (1001) docker     (127)     7735 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/utils/material.py
--rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/utils/notebook.py
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/utils/settings.json
--rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/utils/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:44:12.142363 mat3ra-api-examples-2024.4.1.post0/utils/web/
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/utils/web/renderjson.css
--rw-r--r--   0 runner    (1001) docker     (127)    10845 2024-04-01 22:43:37.000000 mat3ra-api-examples-2024.4.1.post0/utils/web/renderjson.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:31:48.142079 mat3ra-api-examples-2024.4.3.post0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:31:48.118079 mat3ra-api-examples-2024.4.3.post0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:31:48.126079 mat3ra-api-examples-2024.4.3.post0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/.github/workflows/check_links.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4311 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/.github/workflows/cicd.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/.github/workflows/zip_release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/.lycheeignore
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    10324 2024-04-03 18:31:48.142079 mat3ra-api-examples-2024.4.3.post0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9017 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/config.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:31:48.126079 mat3ra-api-examples-2024.4.3.post0/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:31:48.126079 mat3ra-api-examples-2024.4.3.post0/examples/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/examples/assets/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/examples/assets/Si.pz-vbc.UPF
+-rw-r--r--   0 runner    (1001) docker     (127)     4003 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/examples/assets/bash_workflow_template.json
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/examples/assets/mp-978534.poscar
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/examples/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:31:48.126079 mat3ra-api-examples-2024.4.3.post0/examples/job/
+-rw-r--r--   0 runner    (1001) docker     (127)     8581 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/examples/job/create_and_submit_job.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     4122 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/examples/job/create_and_submit_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15961 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/examples/job/get-file-from-job.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    10084 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/examples/job/get-file-from-job.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21116 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/examples/job/ml-train-model-predict-properties.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    11044 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/examples/job/ml-train-model-predict-properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21904 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/examples/job/run-simulations-and-extract-properties.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    12744 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/examples/job/run-simulations-and-extract-properties.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:31:48.130079 mat3ra-api-examples-2024.4.3.post0/examples/material/
+-rw-r--r--   0 runner    (1001) docker     (127)     7818 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/examples/material/create_material.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     4029 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/examples/material/create_material.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7104 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/examples/material/get_materials_by_formula.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     3423 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/examples/material/get_materials_by_formula.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7016 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/examples/material/upload_materials_from_file_poscar.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     3545 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/examples/material/upload_materials_from_file_poscar.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:31:48.130079 mat3ra-api-examples-2024.4.3.post0/examples/system/
+-rw-r--r--   0 runner    (1001) docker     (127)     4669 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/examples/system/get_authentication_params.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/examples/system/get_authentication_params.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:31:48.130079 mat3ra-api-examples-2024.4.3.post0/examples/workflow/
+-rw-r--r--   0 runner    (1001) docker     (127)     7598 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/examples/workflow/get_workflows.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     3683 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/examples/workflow/get_workflows.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12576 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/examples/workflow/qe_scf_calculation.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     6954 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/examples/workflow/qe_scf_calculation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:31:48.122079 mat3ra-api-examples-2024.4.3.post0/extra/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:31:48.130079 mat3ra-api-examples-2024.4.3.post0/extra/css/
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/extra/css/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:31:48.130079 mat3ra-api-examples-2024.4.3.post0/images/
+-rw-r--r--   0 runner    (1001) docker     (127)   413869 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/images/reusable-kernel.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:31:48.142079 mat3ra-api-examples-2024.4.3.post0/mat3ra_api_examples.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10324 2024-04-03 18:31:48.000000 mat3ra-api-examples-2024.4.3.post0/mat3ra_api_examples.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4404 2024-04-03 18:31:48.000000 mat3ra-api-examples-2024.4.3.post0/mat3ra_api_examples.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 18:31:48.000000 mat3ra-api-examples-2024.4.3.post0/mat3ra_api_examples.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-03 18:31:48.000000 mat3ra-api-examples-2024.4.3.post0/mat3ra_api_examples.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-03 18:31:48.000000 mat3ra-api-examples-2024.4.3.post0/mat3ra_api_examples.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-03 18:31:48.000000 mat3ra-api-examples-2024.4.3.post0/mat3ra_api_examples.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/mkdocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:31:48.130079 mat3ra-api-examples-2024.4.3.post0/other/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:31:48.134079 mat3ra-api-examples-2024.4.3.post0/other/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)     5159 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/assets/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)   638208 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/assets/bitter-sweet.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/assets/bittersweet_xgboost.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/assets/deepchem_smiles_vocab.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/assets/gamma_alumina_digne_et_al.poscar
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12157 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/assets/sci_adv_dean_data.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:31:48.134079 mat3ra-api-examples-2024.4.3.post0/other/experiments/
+-rw-r--r--   0 runner    (1001) docker     (127)    25385 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/experiments/create_interface_with_min_energy_by_miller_indices.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    24590 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/experiments/create_interface_with_relaxation_alignn.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    24267 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/experiments/create_interface_with_relaxation_ase_emt.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    24750 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/experiments/create_interface_with_relaxation_matgl_m3gnet.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:31:48.134079 mat3ra-api-examples-2024.4.3.post0/other/experiments/uploads/
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/experiments/uploads/Gr.json
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/experiments/uploads/Ni.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:31:48.134079 mat3ra-api-examples-2024.4.3.post0/other/jarvis/
+-rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/jarvis/import_material_from_jarvis_db_entry.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    15663 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/jarvis/run_job_using_material_from_jarvis_db.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:31:48.134079 mat3ra-api-examples-2024.4.3.post0/other/job/
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/job/Smiles_Generation_Markov_Chain.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    11316 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/job/Smiles_Generation_Markov_Chain.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:31:48.134079 mat3ra-api-examples-2024.4.3.post0/other/machine_learning/
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/machine_learning/Classification_of_Bitterness_XGBoost.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    18602 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/machine_learning/Classification_of_Bitterness_XGBoost.py
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/machine_learning/Prediction_of_Perovskite_Unit_Cell_Volume.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    11454 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/machine_learning/Prediction_of_Perovskite_Unit_Cell_Volume.py
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/machine_learning/neural_network_train.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    19205 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/machine_learning/neural_network_train.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:31:48.134079 mat3ra-api-examples-2024.4.3.post0/other/materials_designer/
+-rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/materials_designer/Introduction.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/materials_designer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16800 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/materials_designer/create_interface_with_min_strain_zsl.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    30016 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/materials_designer/create_interface_with_relaxation_ase_emt.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     7560 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/materials_designer/import_material_from_jarvis_db_entry.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     8618 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/materials_designer/import_materials_from_files.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:31:48.134079 mat3ra-api-examples-2024.4.3.post0/other/materials_designer/src/
+-rw-r--r--   0 runner    (1001) docker     (127)    11964 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/materials_designer/src/pymatgen_coherent_interface_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12408 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/materials_designer/src/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:31:48.134079 mat3ra-api-examples-2024.4.3.post0/other/materials_designer/uploads/
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/materials_designer/uploads/README
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:31:48.138079 mat3ra-api-examples-2024.4.3.post0/other/materialsproject/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/materialsproject/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10185 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/materialsproject/api_interoperability_showcase.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     5708 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/materialsproject/api_interoperability_showcase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6044 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/materialsproject/import_materials_from_materialsproject.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     3514 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/materialsproject/import_materials_from_materialsproject.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:31:48.138079 mat3ra-api-examples-2024.4.3.post0/other/python_transformations/
+-rw-r--r--   0 runner    (1001) docker     (127)     8929 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/python_transformations/1_layer_on_substrate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19706 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/python_transformations/2_strain_matching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/python_transformations/3_imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/python_transformations/4_custom_transformation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/python_transformations/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:31:48.138079 mat3ra-api-examples-2024.4.3.post0/other/webinar/
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/webinar/adsorption-study.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    10676 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/webinar/adsorption-study.py
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/webinar/generate-al2o3-slab-structures.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     8820 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/webinar/generate-al2o3-slab-structures.py
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/webinar/predict_with_machine_learning.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     5649 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/webinar/predict_with_machine_learning.py
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/webinar/wulff-construction-surface-energy-study-cu.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    15454 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/webinar/wulff-construction-surface-energy-study-cu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:31:48.138079 mat3ra-api-examples-2024.4.3.post0/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1669 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/scripts/change-branch-in-urls.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/scripts/env.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2267 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/scripts/render-notebooks.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 18:31:48.142079 mat3ra-api-examples-2024.4.3.post0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:31:48.138079 mat3ra-api-examples-2024.4.3.post0/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7875 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/utils/generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7880 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/utils/jupyterlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7735 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/utils/material.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/utils/notebook.py
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/utils/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/utils/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:31:48.138079 mat3ra-api-examples-2024.4.3.post0/utils/web/
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/utils/web/renderjson.css
+-rw-r--r--   0 runner    (1001) docker     (127)    10845 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/utils/web/renderjson.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/wheel_server.py
```

### Comparing `mat3ra-api-examples-2024.4.1.post0/.gitattributes` & `mat3ra-api-examples-2024.4.3.post0/.gitattributes`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.4.1.post0/.github/workflows/cicd.yml` & `mat3ra-api-examples-2024.4.3.post0/.github/workflows/cicd.yml`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.4.1.post0/.github/workflows/zip_release.yml` & `mat3ra-api-examples-2024.4.3.post0/.github/workflows/zip_release.yml`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.4.1.post0/.gitignore` & `mat3ra-api-examples-2024.4.3.post0/.gitignore`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.4.1.post0/PKG-INFO` & `mat3ra-api-examples-2024.4.3.post0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mat3ra-api-examples
-Version: 2024.4.1.post0
+Version: 2024.4.3.post0
 Summary: Mat3ra API Examples
 Project-URL: homepage, https://exabyte-io.github.io/api-examples
 Project-URL: documentation, https://exabyte-io.github.io/api-examples
 Project-URL: repository, https://github.com/Exabyte-io/api-examples
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: ase>=3.21.1
@@ -39,15 +39,15 @@
 | Folder            | Notebook                                | Description |
 | ------------------|-----------------------------------------| ----------- |
 | [Examples/System](examples/system/)     | [Get Authentication Params](examples/system/get_authentication_params.ipynb)               | Demonstrates how to programatically find your user ID and access token.
 | [Examples/Workflow](examples/workflow/) | [Get Workflows](examples/workflow/get_workflows.ipynb)                           | Walks through how to [query](https://docs.mat3ra.com/rest-api/query-structure/) the Mat3ra API to programatically search for workflows. In this example, we search for workflows that calculate the total energy of a material.
 | [Examples/Workflow](examples/workflow/) | [Quantum Espresso Workflow and Job](examples/workflow/qe_scf_calculation.ipynb)  | Create Quantum Espresso workflow starting from QE input file; create and submit job; after the job is finished, download output file, and finally perform postprocessing analysis.
 | [Examples/Material](examples/material/) | [Get Materials by Formula](examples/material/get_materials_by_formula.ipynb)                | Shows how [queries](https://docs.mat3ra.com/rest-api/query-structure/) can be made to search for materials stored on your account by their formula. In this example, we search for a system containing Si.
 | [Examples/Material](examples/material/) | [Create Material](examples/material/create_material.ipynb)                         | Gives an overview of how materials can be generated in [JSON format](https://docs.mat3ra.com/materials/data/) and uploaded to your user account. In this example, we create an FCC Si crystal and upload it.
-| [Examples/Material](examples/material/) | [Import Materials from Materials Project](examples/material/import_materials_from_materialsproject.ipynb) | Demonstrates how materials can be imported from [Materials Project](https://materialsproject.org/about), if their Materials Project ID is known. In this example, we import monoclinic and hexagonal SiGe cells.
+| [Examples/Material](examples/material/) | [Import Materials from Materials Project](other/materialsproject/import_materials_from_materialsproject.ipynb) | Demonstrates how materials can be imported from [Materials Project](https://materialsproject.org/about), if their Materials Project ID is known. In this example, we import monoclinic and hexagonal SiGe cells.
 | [Examples/Material](examples/material/) | [Import Materials from Poscar](examples/material/upload_materials_from_file_poscar.ipynb)            | Provides an example of how materials can be imported directly from Poscar files (a common chemical file format best-known [for its use in VASP](https://www.vasp.at/wiki/index.php/Input)). In this example, we import the unit cell of SiGe.
 | [Examples/Job](examples/job/)            | [Create and Submit Job](examples/job/create_and_submit_job.ipynb)                   | Shows how to use the Mat3ra API to [create jobs](https://docs.mat3ra.com/jobs/data/) and run them on our cluster. In this example, we run a DFT calculation to get the total energy of an FCC Si unit cell using Quantum Espresso.
 | [Examples/Job](examples/job/)            | [Get File from Job](examples/job/get-file-from-job.ipynb) | Uses the Mat3ra API to query for a list of files produced by a job, describes the metadata assigned to each file, and ends by demonstrating how to download any remote file generated by a job to the local disk.
 | [Examples/Job](examples/job/)            | [Run Simulations and Extract Properties](examples/job/run-simulations-and-extract-properties.ipynb)  | Demonstrates copying a [bank workflow](https://docs.mat3ra.com/workflows/bank/) to an account and using it to calculate the [properties](https://docs.mat3ra.com/properties/overview/) of multiple materials. In this example, we determine the [band gap](https://docs.mat3ra.com/properties-directory/non-scalar/band-gaps/) of Si and Ge.
 | [Examples/Job](examples/job/)            | [ML - Train Model Predict Properties](examples/job/ml-train-model-predict-properties.ipynb)     | Demonstrates the  generation of a training dataset and subsequent training of a [machine learning](https://docs.mat3ra.com/software-directory/overview/#machine-learning) model. In this example, we calculate the band gaps of Si and SiGe, and using various materials properties as descriptors, train a model to predict their band gaps. Finally, we use this trained model to predict the band gap of Ge.
```

### Comparing `mat3ra-api-examples-2024.4.1.post0/README.md` & `mat3ra-api-examples-2024.4.3.post0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 | Folder            | Notebook                                | Description |
 | ------------------|-----------------------------------------| ----------- |
 | [Examples/System](examples/system/)     | [Get Authentication Params](examples/system/get_authentication_params.ipynb)               | Demonstrates how to programatically find your user ID and access token.
 | [Examples/Workflow](examples/workflow/) | [Get Workflows](examples/workflow/get_workflows.ipynb)                           | Walks through how to [query](https://docs.mat3ra.com/rest-api/query-structure/) the Mat3ra API to programatically search for workflows. In this example, we search for workflows that calculate the total energy of a material.
 | [Examples/Workflow](examples/workflow/) | [Quantum Espresso Workflow and Job](examples/workflow/qe_scf_calculation.ipynb)  | Create Quantum Espresso workflow starting from QE input file; create and submit job; after the job is finished, download output file, and finally perform postprocessing analysis.
 | [Examples/Material](examples/material/) | [Get Materials by Formula](examples/material/get_materials_by_formula.ipynb)                | Shows how [queries](https://docs.mat3ra.com/rest-api/query-structure/) can be made to search for materials stored on your account by their formula. In this example, we search for a system containing Si.
 | [Examples/Material](examples/material/) | [Create Material](examples/material/create_material.ipynb)                         | Gives an overview of how materials can be generated in [JSON format](https://docs.mat3ra.com/materials/data/) and uploaded to your user account. In this example, we create an FCC Si crystal and upload it.
-| [Examples/Material](examples/material/) | [Import Materials from Materials Project](examples/material/import_materials_from_materialsproject.ipynb) | Demonstrates how materials can be imported from [Materials Project](https://materialsproject.org/about), if their Materials Project ID is known. In this example, we import monoclinic and hexagonal SiGe cells.
+| [Examples/Material](examples/material/) | [Import Materials from Materials Project](other/materialsproject/import_materials_from_materialsproject.ipynb) | Demonstrates how materials can be imported from [Materials Project](https://materialsproject.org/about), if their Materials Project ID is known. In this example, we import monoclinic and hexagonal SiGe cells.
 | [Examples/Material](examples/material/) | [Import Materials from Poscar](examples/material/upload_materials_from_file_poscar.ipynb)            | Provides an example of how materials can be imported directly from Poscar files (a common chemical file format best-known [for its use in VASP](https://www.vasp.at/wiki/index.php/Input)). In this example, we import the unit cell of SiGe.
 | [Examples/Job](examples/job/)            | [Create and Submit Job](examples/job/create_and_submit_job.ipynb)                   | Shows how to use the Mat3ra API to [create jobs](https://docs.mat3ra.com/jobs/data/) and run them on our cluster. In this example, we run a DFT calculation to get the total energy of an FCC Si unit cell using Quantum Espresso.
 | [Examples/Job](examples/job/)            | [Get File from Job](examples/job/get-file-from-job.ipynb) | Uses the Mat3ra API to query for a list of files produced by a job, describes the metadata assigned to each file, and ends by demonstrating how to download any remote file generated by a job to the local disk.
 | [Examples/Job](examples/job/)            | [Run Simulations and Extract Properties](examples/job/run-simulations-and-extract-properties.ipynb)  | Demonstrates copying a [bank workflow](https://docs.mat3ra.com/workflows/bank/) to an account and using it to calculate the [properties](https://docs.mat3ra.com/properties/overview/) of multiple materials. In this example, we determine the [band gap](https://docs.mat3ra.com/properties-directory/non-scalar/band-gaps/) of Si and Ge.
 | [Examples/Job](examples/job/)            | [ML - Train Model Predict Properties](examples/job/ml-train-model-predict-properties.ipynb)     | Demonstrates the  generation of a training dataset and subsequent training of a [machine learning](https://docs.mat3ra.com/software-directory/overview/#machine-learning) model. In this example, we calculate the band gaps of Si and SiGe, and using various materials properties as descriptors, train a model to predict their band gaps. Finally, we use this trained model to predict the band gap of Ge.
```

### Comparing `mat3ra-api-examples-2024.4.1.post0/examples/assets/bash_workflow_template.json` & `mat3ra-api-examples-2024.4.3.post0/examples/assets/bash_workflow_template.json`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.4.1.post0/examples/config.py` & `mat3ra-api-examples-2024.4.3.post0/examples/config.py`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.4.1.post0/examples/job/create_and_submit_job.ipynb` & `mat3ra-api-examples-2024.4.3.post0/examples/job/create_and_submit_job.ipynb`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9995875179340029%*

 * *Differences: {"'cells'": '{3: {\'source\': {insert: [(7, \'import sys\\n\'), (19, \'    !GIT_BRANCH="dev"; '*

 * *            'export GIT_BRANCH; curl -s '*

 * *            '"https://raw.githubusercontent.com/Exabyte-io/api-examples/${GIT_BRANCH}/scripts/env.sh" '*

 * *            '| bash\\n\'), (20, \'\\n\'), (21, \'if sys.platform == "emscripten":\\n\'), (22, '*

 * *            '\'    apiConfig = data_from_host.get("apiConfig")\\n\'), (23, \'    '*

 * *            'os.environ.update(data_from_host.get("environ", {}))\\n\'), (24, \'    '*

 * *      […]*

```diff
@@ -62,26 +62,47 @@
                 "# @title Authorization Form\n",
                 "ACCOUNT_ID = \"ACCOUNT_ID\"  # @param {type:\"string\"}\n",
                 "AUTH_TOKEN = \"AUTH_TOKEN\"  # @param {type:\"string\"}\n",
                 "MATERIALS_PROJECT_API_KEY = \"MATERIALS_PROJECT_API_KEY\"  # @param {type:\"string\"}\n",
                 "ORGANIZATION_ID = \"ORGANIZATION_ID\"  # @param {type:\"string\"}\n",
                 "\n",
                 "import os\n",
+                "import sys\n",
                 "\n",
                 "if \"COLAB_JUPYTER_IP\" in os.environ:\n",
                 "    os.environ.update(\n",
                 "        dict(\n",
                 "            ACCOUNT_ID=ACCOUNT_ID,\n",
                 "            AUTH_TOKEN=AUTH_TOKEN,\n",
                 "            MATERIALS_PROJECT_API_KEY=MATERIALS_PROJECT_API_KEY,\n",
                 "            ORGANIZATION_ID=ORGANIZATION_ID,\n",
                 "        )\n",
                 "    )\n",
                 "\n",
-                "    !GIT_BRANCH=\"dev\"; export GIT_BRANCH; curl -s \"https://raw.githubusercontent.com/Exabyte-io/api-examples/${GIT_BRANCH}/scripts/env.sh\" | bash"
+                "    !GIT_BRANCH=\"dev\"; export GIT_BRANCH; curl -s \"https://raw.githubusercontent.com/Exabyte-io/api-examples/${GIT_BRANCH}/scripts/env.sh\" | bash\n",
+                "\n",
+                "if sys.platform == \"emscripten\":\n",
+                "    apiConfig = data_from_host.get(\"apiConfig\")\n",
+                "    os.environ.update(data_from_host.get(\"environ\", {}))\n",
+                "    os.environ.update(\n",
+                "        dict(\n",
+                "            ACCOUNT_ID=apiConfig.get(\"accountId\"),\n",
+                "            AUTH_TOKEN=apiConfig.get(\"authToken\"),\n",
+                "            MATERIALS_PROJECT_API_KEY=MATERIALS_PROJECT_API_KEY,\n",
+                "            ORGANIZATION_ID=apiConfig.get(\"organizationId\") or \"\",\n",
+                "        )\n",
+                "    )\n",
+                "\n",
+                "    import micropip\n",
+                "\n",
+                "    await micropip.install(\"mat3ra-api-examples\", deps=False)\n",
+                "    await micropip.install(\"exabyte-api-client\")\n",
+                "    from utils.jupyterlite import install_packages\n",
+                "\n",
+                "    await install_packages(\"\", \"../../config.yml\")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "id": "QRLd1WW23sR6"
```

### Comparing `mat3ra-api-examples-2024.4.1.post0/examples/job/create_and_submit_job.py` & `mat3ra-api-examples-2024.4.3.post0/examples/job/create_and_submit_job.py`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.4.1.post0/examples/job/get-file-from-job.ipynb` & `mat3ra-api-examples-2024.4.3.post0/examples/job/get-file-from-job.ipynb`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9996309370988447%*

 * *Differences: {"'cells'": '{3: {\'source\': {insert: [(7, \'import sys\\n\'), (19, \'    !GIT_BRANCH="dev"; '*

 * *            'export GIT_BRANCH; curl -s '*

 * *            '"https://raw.githubusercontent.com/Exabyte-io/api-examples/${GIT_BRANCH}/scripts/env.sh" '*

 * *            '| bash\\n\'), (20, \'\\n\'), (21, \'if sys.platform == "emscripten":\\n\'), (22, '*

 * *            '\'    apiConfig = data_from_host.get("apiConfig")\\n\'), (23, \'    '*

 * *            'os.environ.update(data_from_host.get("environ", {}))\\n\'), (24, \'    '*

 * *      […]*

```diff
@@ -84,26 +84,47 @@
                 "# @title Authorization Form\n",
                 "ACCOUNT_ID = \"ACCOUNT_ID\"  # @param {type:\"string\"}\n",
                 "AUTH_TOKEN = \"AUTH_TOKEN\"  # @param {type:\"string\"}\n",
                 "MATERIALS_PROJECT_API_KEY = \"MATERIALS_PROJECT_API_KEY\"  # @param {type:\"string\"}\n",
                 "ORGANIZATION_ID = \"ORGANIZATION_ID\"  # @param {type:\"string\"}\n",
                 "\n",
                 "import os\n",
+                "import sys\n",
                 "\n",
                 "if \"COLAB_JUPYTER_IP\" in os.environ:\n",
                 "    os.environ.update(\n",
                 "        dict(\n",
                 "            ACCOUNT_ID=ACCOUNT_ID,\n",
                 "            AUTH_TOKEN=AUTH_TOKEN,\n",
                 "            MATERIALS_PROJECT_API_KEY=MATERIALS_PROJECT_API_KEY,\n",
                 "            ORGANIZATION_ID=ORGANIZATION_ID,\n",
                 "        )\n",
                 "    )\n",
                 "\n",
-                "    !GIT_BRANCH=\"dev\"; export GIT_BRANCH; curl -s \"https://raw.githubusercontent.com/Exabyte-io/api-examples/${GIT_BRANCH}/scripts/env.sh\" | bash"
+                "    !GIT_BRANCH=\"dev\"; export GIT_BRANCH; curl -s \"https://raw.githubusercontent.com/Exabyte-io/api-examples/${GIT_BRANCH}/scripts/env.sh\" | bash\n",
+                "\n",
+                "if sys.platform == \"emscripten\":\n",
+                "    apiConfig = data_from_host.get(\"apiConfig\")\n",
+                "    os.environ.update(data_from_host.get(\"environ\", {}))\n",
+                "    os.environ.update(\n",
+                "        dict(\n",
+                "            ACCOUNT_ID=apiConfig.get(\"accountId\"),\n",
+                "            AUTH_TOKEN=apiConfig.get(\"authToken\"),\n",
+                "            MATERIALS_PROJECT_API_KEY=MATERIALS_PROJECT_API_KEY,\n",
+                "            ORGANIZATION_ID=apiConfig.get(\"organizationId\") or \"\",\n",
+                "        )\n",
+                "    )\n",
+                "\n",
+                "    import micropip\n",
+                "\n",
+                "    await micropip.install(\"mat3ra-api-examples\", deps=False)\n",
+                "    await micropip.install(\"exabyte-api-client\")\n",
+                "    from utils.jupyterlite import install_packages\n",
+                "\n",
+                "    await install_packages(\"\", \"../../config.yml\")"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {
                 "id": "6Z9Cr0_M8GIs"
```

### Comparing `mat3ra-api-examples-2024.4.1.post0/examples/job/get-file-from-job.py` & `mat3ra-api-examples-2024.4.3.post0/examples/job/get-file-from-job.py`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.4.1.post0/examples/job/ml-train-model-predict-properties.ipynb` & `mat3ra-api-examples-2024.4.3.post0/examples/job/ml-train-model-predict-properties.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999853912601626%*

 * *Differences: {"'cells'": '{3: {\'source\': {insert: [(7, \'import sys\\n\'), (19, \'    !GIT_BRANCH="dev"; '*

 * *            'export GIT_BRANCH; curl -s '*

 * *            '"https://raw.githubusercontent.com/Exabyte-io/api-examples/${GIT_BRANCH}/scripts/env.sh" '*

 * *            '| bash\\n\'), (20, \'\\n\'), (21, \'if sys.platform == "emscripten":\\n\'), (22, '*

 * *            '\'    apiConfig = data_from_host.get("apiConfig")\\n\'), (23, \'    '*

 * *            'os.environ.update(data_from_host.get("environ", {}))\\n\'), (24, \'    '*

 * *      […]*

```diff
@@ -84,26 +84,47 @@
                 "# @title Authorization Form\n",
                 "ACCOUNT_ID = \"ACCOUNT_ID\"  # @param {type:\"string\"}\n",
                 "AUTH_TOKEN = \"AUTH_TOKEN\"  # @param {type:\"string\"}\n",
                 "MATERIALS_PROJECT_API_KEY = \"MATERIALS_PROJECT_API_KEY\"  # @param {type:\"string\"}\n",
                 "ORGANIZATION_ID = \"ORGANIZATION_ID\"  # @param {type:\"string\"}\n",
                 "\n",
                 "import os\n",
+                "import sys\n",
                 "\n",
                 "if \"COLAB_JUPYTER_IP\" in os.environ:\n",
                 "    os.environ.update(\n",
                 "        dict(\n",
                 "            ACCOUNT_ID=ACCOUNT_ID,\n",
                 "            AUTH_TOKEN=AUTH_TOKEN,\n",
                 "            MATERIALS_PROJECT_API_KEY=MATERIALS_PROJECT_API_KEY,\n",
                 "            ORGANIZATION_ID=ORGANIZATION_ID,\n",
                 "        )\n",
                 "    )\n",
                 "\n",
-                "    !GIT_BRANCH=\"dev\"; export GIT_BRANCH; curl -s \"https://raw.githubusercontent.com/Exabyte-io/api-examples/${GIT_BRANCH}/scripts/env.sh\" | bash"
+                "    !GIT_BRANCH=\"dev\"; export GIT_BRANCH; curl -s \"https://raw.githubusercontent.com/Exabyte-io/api-examples/${GIT_BRANCH}/scripts/env.sh\" | bash\n",
+                "\n",
+                "if sys.platform == \"emscripten\":\n",
+                "    apiConfig = data_from_host.get(\"apiConfig\")\n",
+                "    os.environ.update(data_from_host.get(\"environ\", {}))\n",
+                "    os.environ.update(\n",
+                "        dict(\n",
+                "            ACCOUNT_ID=apiConfig.get(\"accountId\"),\n",
+                "            AUTH_TOKEN=apiConfig.get(\"authToken\"),\n",
+                "            MATERIALS_PROJECT_API_KEY=MATERIALS_PROJECT_API_KEY,\n",
+                "            ORGANIZATION_ID=apiConfig.get(\"organizationId\") or \"\",\n",
+                "        )\n",
+                "    )\n",
+                "\n",
+                "    import micropip\n",
+                "\n",
+                "    await micropip.install(\"mat3ra-api-examples\", deps=False)\n",
+                "    await micropip.install(\"exabyte-api-client\")\n",
+                "    from utils.jupyterlite import install_packages\n",
+                "\n",
+                "    await install_packages(\"\", \"../../config.yml\")"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {
                 "id": "EMKMnghw2Qxa"
```

### Comparing `mat3ra-api-examples-2024.4.1.post0/examples/job/ml-train-model-predict-properties.py` & `mat3ra-api-examples-2024.4.3.post0/examples/job/ml-train-model-predict-properties.py`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.4.1.post0/examples/job/run-simulations-and-extract-properties.ipynb` & `mat3ra-api-examples-2024.4.3.post0/examples/job/run-simulations-and-extract-properties.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998330429732869%*

 * *Differences: {"'cells'": '{3: {\'source\': {insert: [(7, \'import sys\\n\'), (19, \'    !GIT_BRANCH="dev"; '*

 * *            'export GIT_BRANCH; curl -s '*

 * *            '"https://raw.githubusercontent.com/Exabyte-io/api-examples/${GIT_BRANCH}/scripts/env.sh" '*

 * *            '| bash\\n\'), (20, \'\\n\'), (21, \'if sys.platform == "emscripten":\\n\'), (22, '*

 * *            '\'    apiConfig = data_from_host.get("apiConfig")\\n\'), (23, \'    '*

 * *            'os.environ.update(data_from_host.get("environ", {}))\\n\'), (24, \'    '*

 * *      […]*

```diff
@@ -91,26 +91,47 @@
                 "# @title Authorization Form\n",
                 "ACCOUNT_ID = \"ACCOUNT_ID\"  # @param {type:\"string\"}\n",
                 "AUTH_TOKEN = \"AUTH_TOKEN\"  # @param {type:\"string\"}\n",
                 "MATERIALS_PROJECT_API_KEY = \"MATERIALS_PROJECT_API_KEY\"  # @param {type:\"string\"}\n",
                 "ORGANIZATION_ID = \"ORGANIZATION_ID\"  # @param {type:\"string\"}\n",
                 "\n",
                 "import os\n",
+                "import sys\n",
                 "\n",
                 "if \"COLAB_JUPYTER_IP\" in os.environ:\n",
                 "    os.environ.update(\n",
                 "        dict(\n",
                 "            ACCOUNT_ID=ACCOUNT_ID,\n",
                 "            AUTH_TOKEN=AUTH_TOKEN,\n",
                 "            MATERIALS_PROJECT_API_KEY=MATERIALS_PROJECT_API_KEY,\n",
                 "            ORGANIZATION_ID=ORGANIZATION_ID,\n",
                 "        )\n",
                 "    )\n",
                 "\n",
-                "    !GIT_BRANCH=\"dev\"; export GIT_BRANCH; curl -s \"https://raw.githubusercontent.com/Exabyte-io/api-examples/${GIT_BRANCH}/scripts/env.sh\" | bash"
+                "    !GIT_BRANCH=\"dev\"; export GIT_BRANCH; curl -s \"https://raw.githubusercontent.com/Exabyte-io/api-examples/${GIT_BRANCH}/scripts/env.sh\" | bash\n",
+                "\n",
+                "if sys.platform == \"emscripten\":\n",
+                "    apiConfig = data_from_host.get(\"apiConfig\")\n",
+                "    os.environ.update(data_from_host.get(\"environ\", {}))\n",
+                "    os.environ.update(\n",
+                "        dict(\n",
+                "            ACCOUNT_ID=apiConfig.get(\"accountId\"),\n",
+                "            AUTH_TOKEN=apiConfig.get(\"authToken\"),\n",
+                "            MATERIALS_PROJECT_API_KEY=MATERIALS_PROJECT_API_KEY,\n",
+                "            ORGANIZATION_ID=apiConfig.get(\"organizationId\") or \"\",\n",
+                "        )\n",
+                "    )\n",
+                "\n",
+                "    import micropip\n",
+                "\n",
+                "    await micropip.install(\"mat3ra-api-examples\", deps=False)\n",
+                "    await micropip.install(\"exabyte-api-client\")\n",
+                "    from utils.jupyterlite import install_packages\n",
+                "\n",
+                "    await install_packages(\"\", \"../../config.yml\")"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {
                 "id": "jS3-0-VzGuQP"
```

### Comparing `mat3ra-api-examples-2024.4.1.post0/examples/job/run-simulations-and-extract-properties.py` & `mat3ra-api-examples-2024.4.3.post0/examples/job/run-simulations-and-extract-properties.py`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.4.1.post0/examples/material/create_material.ipynb` & `mat3ra-api-examples-2024.4.3.post0/examples/material/create_material.ipynb`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999415650406504%*

 * *Differences: {"'cells'": '{3: {\'source\': {insert: [(7, \'import sys\\n\'), (19, \'    !GIT_BRANCH="dev"; '*

 * *            'export GIT_BRANCH; curl -s '*

 * *            '"https://raw.githubusercontent.com/Exabyte-io/api-examples/${GIT_BRANCH}/scripts/env.sh" '*

 * *            '| bash\\n\'), (20, \'\\n\'), (21, \'if sys.platform == "emscripten":\\n\'), (22, '*

 * *            '\'    apiConfig = data_from_host.get("apiConfig")\\n\'), (23, \'    '*

 * *            'os.environ.update(data_from_host.get("environ", {}))\\n\'), (24, \'    '*

 * *      […]*

```diff
@@ -57,26 +57,47 @@
                 "# @title Authorization Form\n",
                 "ACCOUNT_ID = \"ACCOUNT_ID\"  # @param {type:\"string\"}\n",
                 "AUTH_TOKEN = \"AUTH_TOKEN\"  # @param {type:\"string\"}\n",
                 "MATERIALS_PROJECT_API_KEY = \"MATERIALS_PROJECT_API_KEY\"  # @param {type:\"string\"}\n",
                 "ORGANIZATION_ID = \"ORGANIZATION_ID\"  # @param {type:\"string\"}\n",
                 "\n",
                 "import os\n",
+                "import sys\n",
                 "\n",
                 "if \"COLAB_JUPYTER_IP\" in os.environ:\n",
                 "    os.environ.update(\n",
                 "        dict(\n",
                 "            ACCOUNT_ID=ACCOUNT_ID,\n",
                 "            AUTH_TOKEN=AUTH_TOKEN,\n",
                 "            MATERIALS_PROJECT_API_KEY=MATERIALS_PROJECT_API_KEY,\n",
                 "            ORGANIZATION_ID=ORGANIZATION_ID,\n",
                 "        )\n",
                 "    )\n",
                 "\n",
-                "    !GIT_BRANCH=\"dev\"; export GIT_BRANCH; curl -s \"https://raw.githubusercontent.com/Exabyte-io/api-examples/${GIT_BRANCH}/scripts/env.sh\" | bash"
+                "    !GIT_BRANCH=\"dev\"; export GIT_BRANCH; curl -s \"https://raw.githubusercontent.com/Exabyte-io/api-examples/${GIT_BRANCH}/scripts/env.sh\" | bash\n",
+                "\n",
+                "if sys.platform == \"emscripten\":\n",
+                "    apiConfig = data_from_host.get(\"apiConfig\")\n",
+                "    os.environ.update(data_from_host.get(\"environ\", {}))\n",
+                "    os.environ.update(\n",
+                "        dict(\n",
+                "            ACCOUNT_ID=apiConfig.get(\"accountId\"),\n",
+                "            AUTH_TOKEN=apiConfig.get(\"authToken\"),\n",
+                "            MATERIALS_PROJECT_API_KEY=MATERIALS_PROJECT_API_KEY,\n",
+                "            ORGANIZATION_ID=apiConfig.get(\"organizationId\") or \"\",\n",
+                "        )\n",
+                "    )\n",
+                "\n",
+                "    import micropip\n",
+                "\n",
+                "    await micropip.install(\"mat3ra-api-examples\", deps=False)\n",
+                "    await micropip.install(\"exabyte-api-client\")\n",
+                "    from utils.jupyterlite import install_packages\n",
+                "\n",
+                "    await install_packages(\"\", \"../../config.yml\")"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {
                 "id": "n3qID8yysRA9"
```

### Comparing `mat3ra-api-examples-2024.4.1.post0/examples/material/create_material.py` & `mat3ra-api-examples-2024.4.3.post0/examples/material/create_material.py`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.4.1.post0/examples/material/get_materials_by_formula.ipynb` & `mat3ra-api-examples-2024.4.3.post0/other/materialsproject/import_materials_from_materialsproject.ipynb`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9650074404761905%*

 * *Differences: {"'cells'": "{0: {'metadata': {'id': 'y_SM_JBc9vrV'}, 'source': {insert: [(0, '<a "*

 * *            'href="https://colab.research.google.com/github/Exabyte-io/api-examples/blob/dev/examples/material/import_materials_from_materialsproject.ipynb" '*

 * *            'target="_parent">\\n\')], delete: [0]}}, 1: {\'metadata\': {\'id\': '*

 * *            "'amffxwKY9vrX'}, 'source': {insert: [(2, 'This example demonstrates how to import "*

 * *            'materials from the materials project database via '*

 * *            "[Material]( […]*

```diff
@@ -1,38 +1,38 @@
 {
     "cells": [
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {
-                "id": "M9pqcsQ_CzO_"
+                "id": "y_SM_JBc9vrV"
             },
             "source": [
-                "<a href=\"https://colab.research.google.com/github/Exabyte-io/api-examples/blob/dev/examples/material/get_materials_by_formula.ipynb\" target=\"_parent\">\n",
+                "<a href=\"https://colab.research.google.com/github/Exabyte-io/api-examples/blob/dev/examples/material/import_materials_from_materialsproject.ipynb\" target=\"_parent\">\n",
                 "<img alt=\"Open in Google Colab\" src=\"https://user-images.githubusercontent.com/20477508/128780728-491fea90-9b23-495f-a091-11681150db37.jpeg\" width=\"150\" border=\"0\">\n",
                 "</a>"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {
-                "id": "wK3ZoE8wCzPB"
+                "id": "amffxwKY9vrX"
             },
             "source": [
                 "# Overview\n",
                 "\n",
-                "Inside this example we contact [Material](https://docs.mat3ra.com/api/Material/get_materials) endpoint to obtain a list materials that an account has access to. We use chemical formula to filter the list."
+                "This example demonstrates how to import materials from the materials project database via [Material](https://docs.mat3ra.com/api/Material/post_materials_import) endpoint."
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {
-                "id": "eTDhujSFCzPC"
+                "id": "c-nHvPSy9vrY"
             },
             "source": [
                 "# Complete Authorization Form and Initialize Settings\n",
                 "\n",
                 "This will also determine environment and set all environment variables. We determine if we are using Jupyter Notebooks or Google Colab to run this tutorial.\n",
                 "\n",
                 "If you are running this notebook from Google Colab, Colab takes ~1 min to execute the following cell.\n",
@@ -47,15 +47,15 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "cellView": "form",
-                "id": "LbQQf3GpCzPD"
+                "id": "6KqWoLdv9vrY"
             },
             "outputs": [],
             "source": [
                 "# @title Authorization Form\n",
                 "ACCOUNT_ID = \"ACCOUNT_ID\"  # @param {type:\"string\"}\n",
                 "AUTH_TOKEN = \"AUTH_TOKEN\"  # @param {type:\"string\"}\n",
                 "MATERIALS_PROJECT_API_KEY = \"MATERIALS_PROJECT_API_KEY\"  # @param {type:\"string\"}\n",
@@ -76,131 +76,111 @@
                 "    !GIT_BRANCH=\"dev\"; export GIT_BRANCH; curl -s \"https://raw.githubusercontent.com/Exabyte-io/api-examples/${GIT_BRANCH}/scripts/env.sh\" | bash"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {
-                "id": "ClaSpX4BCzPD"
+                "id": "5wAnsWE-9vrZ"
             },
             "source": [
                 "# Imports"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
-                "id": "kMwJxlkQCzPE"
+                "id": "e9EGeIkg9vrZ"
             },
             "outputs": [],
             "source": [
-                "from utils.settings import ENDPOINT_ARGS, ACCOUNT_ID\n",
+                "from utils.settings import ENDPOINT_ARGS, MATERIALS_PROJECT_API_KEY\n",
                 "from utils.generic import display_JSON\n",
                 "\n",
                 "from exabyte_api_client.endpoints.materials import MaterialEndpoints"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {
-                "id": "mbtRgwoBCzPE"
+                "id": "C2Dxa1qZ9vra"
             },
             "source": [
                 "## Set Parameters\n",
                 "\n",
-                "- **QUERY**: A query describing the documents to find. See [Meteor collection](https://docs.meteor.com/api/collections.html#Mongo-Collection-find) for more information."
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {
-                "id": "KZWqlxVcCzPF"
-            },
-            "outputs": [],
-            "source": [
-                "QUERY = {\"formula\": \"Si\", \"owner._id\": ACCOUNT_ID}"
-            ]
-        },
-        {
-            "attachments": {},
-            "cell_type": "markdown",
-            "metadata": {
-                "id": "wtOfD1UuCzPF"
-            },
-            "source": [
-                "## Initialize the endpoint"
+                "- **MATERIALS_PROJECT_IDS**: a list of material IDs to be imported\n",
+                "\n",
+                "- **TAGS**: a list of [tags](https://docs.mat3ra.com/entities-general/data/#tags) to assign to imported materials"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
-                "id": "dolF1C6-CzPG"
+                "id": "6xpZA6M_9vra"
             },
             "outputs": [],
             "source": [
-                "endpoint = MaterialEndpoints(*ENDPOINT_ARGS)"
+                "MATERIALS_PROJECT_IDS = [\"mp-978534\", \"mp-1096549\"]\n",
+                "TAGS = [\"tag1\", \"tag2\"]"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {
-                "id": "kziWNLGnCzPG"
+                "id": "11YzfvYk9vrb"
             },
             "source": [
-                "## List materials\n",
+                "## Import materials\n",
                 "\n",
-                "Contact the endpoint to list materials according to the query above."
+                "Initialize `MaterialEndpoints` class and call `import_from_materialsproject` function to import materials."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
-                "id": "IE-K3TexCzPH"
+                "id": "Ar05ANgq9vrb"
             },
             "outputs": [],
             "source": [
-                "materials = endpoint.list(QUERY)"
+                "endpoint = MaterialEndpoints(*ENDPOINT_ARGS)\n",
+                "materials = endpoint.import_from_materialsproject(MATERIALS_PROJECT_API_KEY, MATERIALS_PROJECT_IDS, tags=TAGS)"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {
-                "id": "fP8c01zaCzPH"
+                "id": "DPMW1MDy9vrc"
             },
             "source": [
-                "## Print materials\n",
+                "## Print imported materials\n",
                 "\n",
-                "Print the list of materials saved under the corresponding variable in pretty JSON below."
+                "Print the list of imported materials in pretty JSON below."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
-                "id": "LRVpf37eCzPH",
-                "pycharm": {
-                    "name": "#%%\n"
-                }
+                "id": "n7WgbbkJ9vrc"
             },
             "outputs": [],
             "source": [
                 "display_JSON(materials)"
             ]
         }
     ],
     "metadata": {
         "colab": {
-            "name": "get_materials_by_formula.ipynb",
+            "name": "import_materials_from_materialsproject.ipynb",
             "provenance": []
         },
         "kernelspec": {
             "display_name": "Python 3",
             "language": "python",
             "name": "python3"
         },
```

### Comparing `mat3ra-api-examples-2024.4.1.post0/examples/material/get_materials_by_formula.py` & `mat3ra-api-examples-2024.4.3.post0/examples/material/get_materials_by_formula.py`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.4.1.post0/examples/material/import_materials_from_materialsproject.ipynb` & `mat3ra-api-examples-2024.4.3.post0/examples/material/get_materials_by_formula.ipynb`

 * *Files 19% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9645065693960511%*

 * *Differences: {"'cells'": "{0: {'metadata': {'id': 'M9pqcsQ_CzO_'}, 'source': {insert: [(0, '<a "*

 * *            'href="https://colab.research.google.com/github/Exabyte-io/api-examples/blob/dev/examples/material/get_materials_by_formula.ipynb" '*

 * *            'target="_parent">\\n\')], delete: [0]}}, 1: {\'metadata\': {\'id\': '*

 * *            "'wK3ZoE8wCzPB'}, 'source': {insert: [(2, 'Inside this example we contact "*

 * *            '[Material](https://docs.mat3ra.com/api/Material/get_materials) endpoint to obtain a '*

 * *            ' […]*

```diff
@@ -1,38 +1,38 @@
 {
     "cells": [
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {
-                "id": "y_SM_JBc9vrV"
+                "id": "M9pqcsQ_CzO_"
             },
             "source": [
-                "<a href=\"https://colab.research.google.com/github/Exabyte-io/api-examples/blob/dev/examples/material/import_materials_from_materialsproject.ipynb\" target=\"_parent\">\n",
+                "<a href=\"https://colab.research.google.com/github/Exabyte-io/api-examples/blob/dev/examples/material/get_materials_by_formula.ipynb\" target=\"_parent\">\n",
                 "<img alt=\"Open in Google Colab\" src=\"https://user-images.githubusercontent.com/20477508/128780728-491fea90-9b23-495f-a091-11681150db37.jpeg\" width=\"150\" border=\"0\">\n",
                 "</a>"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {
-                "id": "amffxwKY9vrX"
+                "id": "wK3ZoE8wCzPB"
             },
             "source": [
                 "# Overview\n",
                 "\n",
-                "This example demonstrates how to import materials from the materials project database via [Material](https://docs.mat3ra.com/api/Material/post_materials_import) endpoint."
+                "Inside this example we contact [Material](https://docs.mat3ra.com/api/Material/get_materials) endpoint to obtain a list materials that an account has access to. We use chemical formula to filter the list."
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {
-                "id": "c-nHvPSy9vrY"
+                "id": "eTDhujSFCzPC"
             },
             "source": [
                 "# Complete Authorization Form and Initialize Settings\n",
                 "\n",
                 "This will also determine environment and set all environment variables. We determine if we are using Jupyter Notebooks or Google Colab to run this tutorial.\n",
                 "\n",
                 "If you are running this notebook from Google Colab, Colab takes ~1 min to execute the following cell.\n",
@@ -47,140 +47,181 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "cellView": "form",
-                "id": "6KqWoLdv9vrY"
+                "id": "LbQQf3GpCzPD"
             },
             "outputs": [],
             "source": [
                 "# @title Authorization Form\n",
                 "ACCOUNT_ID = \"ACCOUNT_ID\"  # @param {type:\"string\"}\n",
                 "AUTH_TOKEN = \"AUTH_TOKEN\"  # @param {type:\"string\"}\n",
                 "MATERIALS_PROJECT_API_KEY = \"MATERIALS_PROJECT_API_KEY\"  # @param {type:\"string\"}\n",
                 "ORGANIZATION_ID = \"ORGANIZATION_ID\"  # @param {type:\"string\"}\n",
                 "\n",
                 "import os\n",
+                "import sys\n",
                 "\n",
                 "if \"COLAB_JUPYTER_IP\" in os.environ:\n",
                 "    os.environ.update(\n",
                 "        dict(\n",
                 "            ACCOUNT_ID=ACCOUNT_ID,\n",
                 "            AUTH_TOKEN=AUTH_TOKEN,\n",
                 "            MATERIALS_PROJECT_API_KEY=MATERIALS_PROJECT_API_KEY,\n",
                 "            ORGANIZATION_ID=ORGANIZATION_ID,\n",
                 "        )\n",
                 "    )\n",
                 "\n",
-                "    !GIT_BRANCH=\"dev\"; export GIT_BRANCH; curl -s \"https://raw.githubusercontent.com/Exabyte-io/api-examples/${GIT_BRANCH}/scripts/env.sh\" | bash"
+                "    !GIT_BRANCH=\"dev\"; export GIT_BRANCH; curl -s \"https://raw.githubusercontent.com/Exabyte-io/api-examples/${GIT_BRANCH}/scripts/env.sh\" | bash\n",
+                "\n",
+                "if sys.platform == \"emscripten\":\n",
+                "    apiConfig = data_from_host.get(\"apiConfig\")\n",
+                "    os.environ.update(data_from_host.get(\"environ\", {}))\n",
+                "    os.environ.update(\n",
+                "        dict(\n",
+                "            ACCOUNT_ID=apiConfig.get(\"accountId\"),\n",
+                "            AUTH_TOKEN=apiConfig.get(\"authToken\"),\n",
+                "            MATERIALS_PROJECT_API_KEY=MATERIALS_PROJECT_API_KEY,\n",
+                "            ORGANIZATION_ID=apiConfig.get(\"organizationId\") or \"\",\n",
+                "        )\n",
+                "    )\n",
+                "\n",
+                "    import micropip\n",
+                "\n",
+                "    await micropip.install(\"mat3ra-api-examples\", deps=False)\n",
+                "    await micropip.install(\"exabyte-api-client\")\n",
+                "    from utils.jupyterlite import install_packages\n",
+                "\n",
+                "    await install_packages(\"\", \"../../config.yml\")"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {
-                "id": "5wAnsWE-9vrZ"
+                "id": "ClaSpX4BCzPD"
             },
             "source": [
                 "# Imports"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
-                "id": "e9EGeIkg9vrZ"
+                "id": "kMwJxlkQCzPE"
             },
             "outputs": [],
             "source": [
-                "from utils.settings import ENDPOINT_ARGS, MATERIALS_PROJECT_API_KEY\n",
+                "from utils.settings import ENDPOINT_ARGS, ACCOUNT_ID\n",
                 "from utils.generic import display_JSON\n",
                 "\n",
                 "from exabyte_api_client.endpoints.materials import MaterialEndpoints"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {
-                "id": "C2Dxa1qZ9vra"
+                "id": "mbtRgwoBCzPE"
             },
             "source": [
                 "## Set Parameters\n",
                 "\n",
-                "- **MATERIALS_PROJECT_IDS**: a list of material IDs to be imported\n",
-                "\n",
-                "- **TAGS**: a list of [tags](https://docs.mat3ra.com/entities-general/data/#tags) to assign to imported materials"
+                "- **QUERY**: A query describing the documents to find. See [Meteor collection](https://docs.meteor.com/api/collections.html#Mongo-Collection-find) for more information."
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {
+                "id": "KZWqlxVcCzPF"
+            },
+            "outputs": [],
+            "source": [
+                "QUERY = {\"formula\": \"Si\", \"owner._id\": ACCOUNT_ID}"
+            ]
+        },
+        {
+            "attachments": {},
+            "cell_type": "markdown",
+            "metadata": {
+                "id": "wtOfD1UuCzPF"
+            },
+            "source": [
+                "## Initialize the endpoint"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
-                "id": "6xpZA6M_9vra"
+                "id": "dolF1C6-CzPG"
             },
             "outputs": [],
             "source": [
-                "MATERIALS_PROJECT_IDS = [\"mp-978534\", \"mp-1096549\"]\n",
-                "TAGS = [\"tag1\", \"tag2\"]"
+                "endpoint = MaterialEndpoints(*ENDPOINT_ARGS)"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {
-                "id": "11YzfvYk9vrb"
+                "id": "kziWNLGnCzPG"
             },
             "source": [
-                "## Import materials\n",
+                "## List materials\n",
                 "\n",
-                "Initialize `MaterialEndpoints` class and call `import_from_materialsproject` function to import materials."
+                "Contact the endpoint to list materials according to the query above."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
-                "id": "Ar05ANgq9vrb"
+                "id": "IE-K3TexCzPH"
             },
             "outputs": [],
             "source": [
-                "endpoint = MaterialEndpoints(*ENDPOINT_ARGS)\n",
-                "materials = endpoint.import_from_materialsproject(MATERIALS_PROJECT_API_KEY, MATERIALS_PROJECT_IDS, tags=TAGS)"
+                "materials = endpoint.list(QUERY)"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {
-                "id": "DPMW1MDy9vrc"
+                "id": "fP8c01zaCzPH"
             },
             "source": [
-                "## Print imported materials\n",
+                "## Print materials\n",
                 "\n",
-                "Print the list of imported materials in pretty JSON below."
+                "Print the list of materials saved under the corresponding variable in pretty JSON below."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
-                "id": "n7WgbbkJ9vrc"
+                "id": "LRVpf37eCzPH",
+                "pycharm": {
+                    "name": "#%%\n"
+                }
             },
             "outputs": [],
             "source": [
                 "display_JSON(materials)"
             ]
         }
     ],
     "metadata": {
         "colab": {
-            "name": "import_materials_from_materialsproject.ipynb",
+            "name": "get_materials_by_formula.ipynb",
             "provenance": []
         },
         "kernelspec": {
             "display_name": "Python 3",
             "language": "python",
             "name": "python3"
         },
```

### Comparing `mat3ra-api-examples-2024.4.1.post0/examples/material/import_materials_from_materialsproject.py` & `mat3ra-api-examples-2024.4.3.post0/other/materialsproject/import_materials_from_materialsproject.py`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.4.1.post0/examples/material/upload_materials_from_file_poscar.ipynb` & `mat3ra-api-examples-2024.4.3.post0/examples/material/upload_materials_from_file_poscar.ipynb`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9994554924242425%*

 * *Differences: {"'cells'": "{3: {'source': {insert: [(7, 'import sys\\n'), (22, '    "*

 * *            'os.chdir(os.path.join("api-examples", '*

 * *            'os.path.dirname(get_notebook_info()["notebook_path"])))\\n\'), (23, \'\\n\'), (24, '*

 * *            '\'if sys.platform == "emscripten":\\n\'), (25, \'    apiConfig = '*

 * *            'data_from_host.get("apiConfig")\\n\'), (26, \'    '*

 * *            'os.environ.update(data_from_host.get("environ", {}))\\n\'), (27, \'    '*

 * *            "os.environ.update(\\n'), (28, '        dict(\ […]*

```diff
@@ -58,29 +58,50 @@
                 "# @title Authorization Form\n",
                 "ACCOUNT_ID = \"ACCOUNT_ID\"  # @param {type:\"string\"}\n",
                 "AUTH_TOKEN = \"AUTH_TOKEN\"  # @param {type:\"string\"}\n",
                 "MATERIALS_PROJECT_API_KEY = \"MATERIALS_PROJECT_API_KEY\"  # @param {type:\"string\"}\n",
                 "ORGANIZATION_ID = \"ORGANIZATION_ID\"  # @param {type:\"string\"}\n",
                 "\n",
                 "import os\n",
+                "import sys\n",
                 "\n",
                 "if \"COLAB_JUPYTER_IP\" in os.environ:\n",
                 "    os.environ.update(\n",
                 "        dict(\n",
                 "            ACCOUNT_ID=ACCOUNT_ID,\n",
                 "            AUTH_TOKEN=AUTH_TOKEN,\n",
                 "            MATERIALS_PROJECT_API_KEY=MATERIALS_PROJECT_API_KEY,\n",
                 "            ORGANIZATION_ID=ORGANIZATION_ID,\n",
                 "        )\n",
                 "    )\n",
                 "\n",
                 "    !GIT_BRANCH=\"dev\"; export GIT_BRANCH; export IS_USING_GIT_LFS=true; curl -s \"https://raw.githubusercontent.com/Exabyte-io/api-examples/${GIT_BRANCH}/scripts/env.sh\" | bash\n",
                 "    from examples.utils.notebook import get_notebook_info\n",
                 "\n",
-                "    os.chdir(os.path.join(\"api-examples\", os.path.dirname(get_notebook_info()[\"notebook_path\"])))"
+                "    os.chdir(os.path.join(\"api-examples\", os.path.dirname(get_notebook_info()[\"notebook_path\"])))\n",
+                "\n",
+                "if sys.platform == \"emscripten\":\n",
+                "    apiConfig = data_from_host.get(\"apiConfig\")\n",
+                "    os.environ.update(data_from_host.get(\"environ\", {}))\n",
+                "    os.environ.update(\n",
+                "        dict(\n",
+                "            ACCOUNT_ID=apiConfig.get(\"accountId\"),\n",
+                "            AUTH_TOKEN=apiConfig.get(\"authToken\"),\n",
+                "            MATERIALS_PROJECT_API_KEY=MATERIALS_PROJECT_API_KEY,\n",
+                "            ORGANIZATION_ID=apiConfig.get(\"organizationId\") or \"\",\n",
+                "        )\n",
+                "    )\n",
+                "\n",
+                "    import micropip\n",
+                "\n",
+                "    await micropip.install(\"mat3ra-api-examples\", deps=False)\n",
+                "    await micropip.install(\"exabyte-api-client\")\n",
+                "    from utils.jupyterlite import install_packages\n",
+                "\n",
+                "    await install_packages(\"\", \"../../config.yml\")"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {
                 "id": "QuS0AUReuC-s"
```

### Comparing `mat3ra-api-examples-2024.4.1.post0/examples/material/upload_materials_from_file_poscar.py` & `mat3ra-api-examples-2024.4.3.post0/examples/material/upload_materials_from_file_poscar.py`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.4.1.post0/examples/system/get_authentication_params.ipynb` & `mat3ra-api-examples-2024.4.3.post0/examples/system/get_authentication_params.ipynb`

 * *Files 13% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9992424242424243%*

 * *Differences: {"'cells'": '{4: {\'source\': {insert: [(9, \'import sys\\n\'), (12, \'    !GIT_BRANCH="dev"; '*

 * *            'export GIT_BRANCH; curl -s '*

 * *            '"https://raw.githubusercontent.com/Exabyte-io/api-examples/${GIT_BRANCH}/scripts/env.sh" '*

 * *            '| bash\\n\'), (13, \'\\n\'), (14, \'if sys.platform == "emscripten":\\n\'), (15, '*

 * *            '\'    apiConfig = data_from_host.get("apiConfig")\\n\'), (16, \'    '*

 * *            'os.environ.update(data_from_host.get("environ", {}))\\n\'), (17, \'    '*

 * *      […]*

```diff
@@ -55,17 +55,37 @@
                 "\n",
                 "# avoid storing password in plaintext\n",
                 "from getpass import getpass\n",
                 "\n",
                 "PASSWORD = getpass(\"Please enter password: \")\n",
                 "\n",
                 "import os\n",
+                "import sys\n",
                 "\n",
                 "if \"COLAB_JUPYTER_IP\" in os.environ:\n",
-                "    !GIT_BRANCH=\"dev\"; export GIT_BRANCH; curl -s \"https://raw.githubusercontent.com/Exabyte-io/api-examples/${GIT_BRANCH}/scripts/env.sh\" | bash"
+                "    !GIT_BRANCH=\"dev\"; export GIT_BRANCH; curl -s \"https://raw.githubusercontent.com/Exabyte-io/api-examples/${GIT_BRANCH}/scripts/env.sh\" | bash\n",
+                "\n",
+                "if sys.platform == \"emscripten\":\n",
+                "    apiConfig = data_from_host.get(\"apiConfig\")\n",
+                "    os.environ.update(data_from_host.get(\"environ\", {}))\n",
+                "    os.environ.update(\n",
+                "        dict(\n",
+                "            ACCOUNT_ID=apiConfig.get(\"accountId\"),\n",
+                "            AUTH_TOKEN=apiConfig.get(\"authToken\"),\n",
+                "            ORGANIZATION_ID=apiConfig.get(\"organizationId\") or \"\",\n",
+                "        )\n",
+                "    )\n",
+                "\n",
+                "    import micropip\n",
+                "\n",
+                "    await micropip.install(\"mat3ra-api-examples\", deps=False)\n",
+                "    await micropip.install(\"exabyte-api-client\")\n",
+                "    from utils.jupyterlite import install_packages\n",
+                "\n",
+                "    await install_packages(\"\", \"../../config.yml\")"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
```

### Comparing `mat3ra-api-examples-2024.4.1.post0/examples/system/get_authentication_params.py` & `mat3ra-api-examples-2024.4.3.post0/examples/system/get_authentication_params.py`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.4.1.post0/examples/workflow/get_workflows.ipynb` & `mat3ra-api-examples-2024.4.3.post0/other/materials_designer/import_material_from_jarvis_db_entry.ipynb`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7368701182396036%*

 * *Differences: {"'cells'": "{1: {'metadata': {replace: OrderedDict()}, 'source': ['## 1. Set Parameters'], 'id': "*

 * *            "'4299768d', delete: ['attachments']}, 3: {'metadata': {replace: OrderedDict()}, "*

 * *            "'source': ['## 2. Install Packages'], 'id': '8b00ab6854f2263b', delete: "*

 * *            "['attachments']}, 5: {'metadata': {replace: OrderedDict()}, 'source': {insert: [(0, "*

 * *            "'## 3. Data Processing\\n'), (2, '### 3.1. Get data and wrap it in dataframe')], "*

 * *            "delete: [12, 10, 9, 8, […]*

```diff
@@ -1,233 +1,280 @@
 {
     "cells": [
         {
-            "attachments": {},
             "cell_type": "markdown",
-            "metadata": {
-                "id": "rqmhDMSkIQAT"
-            },
+            "id": "826fcc4c",
+            "metadata": {},
             "source": [
-                "<a href=\"https://colab.research.google.com/github/Exabyte-io/api-examples/blob/dev/examples/workflow/get_workflows.ipynb\" target=\"_parent\">\n",
-                "<img alt=\"Open in Google Colab\" src=\"https://user-images.githubusercontent.com/20477508/128780728-491fea90-9b23-495f-a091-11681150db37.jpeg\" width=\"150\" border=\"0\">\n",
-                "</a>"
+                "# Import 2D material from JARVIS database\n",
+                "\n",
+                "Import a structure from the NIST JARVIS database by its ID. Use data at <a href=\"https://figshare.com/articles/dataset/Monolayer_data_for_heterostructure/22344571\" target=\"_blank\">JARVIS-DFT</a> to find the ID of the structure you are interested in.\n",
+                "\n",
+                "<h2 style=\"color:green\">Usage</h2>\n",
+                "\n",
+                "1. Set Input Parameters (e.g. `JARVIS_ID`) below or use the default value\n",
+                "1. Click \"Run\" > \"Run All Cells\" to run all cells\n",
+                "1. Wait for the run to complete (it should take ~30 sec first time to install packages). Scroll down to view cell results.\n",
+                "\n",
+                "## Methodology\n",
+                "\n",
+                "The following happens in the script below:\n",
+                "\n",
+                "1. Install `express-py` alongside the necessary packages\n",
+                "2. Import the material from JARVIS database\n",
+                "3. Convert the material to ESSE format\n",
+                "4. Pass the material to the outside runtime"
             ]
         },
         {
-            "attachments": {},
             "cell_type": "markdown",
-            "metadata": {
-                "id": "OtfhrLhwIQAV"
-            },
+            "id": "4299768d",
+            "metadata": {},
             "source": [
-                "# Overview\n",
-                "\n",
-                "Inside this example we contact [Workflow](https://docs.mat3ra.com/api/Workflows/get_workflows) endpoint to obtain a list of workflows that an account has access to."
+                "## 1. Set Parameters"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 2,
+            "id": "9c1f4e9e",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "# Note: JVASP-670 is an entry for MoTe2 and JVASP-6838 is an entry for GaTe\n",
+                "JARVIS_IDS = [\n",
+                "    \"JVASP-670\",\n",
+                "    \"JVASP-6838\",\n",
+                "]"
             ]
         },
         {
-            "attachments": {},
             "cell_type": "markdown",
+            "id": "8b00ab6854f2263b",
+            "metadata": {},
+            "source": [
+                "## 2. Install Packages"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "ef2b38a5-de7e-419e-b605-110e9e0095f5",
             "metadata": {
-                "id": "stJCOZz0IQAW"
+                "trusted": true
             },
+            "outputs": [],
             "source": [
-                "# Complete Authorization Form and Initialize Settings\n",
-                "\n",
-                "This will also determine environment and set all environment variables. We determine if we are using Jupyter Notebooks or Google Colab to run this tutorial.\n",
-                "\n",
-                "If you are running this notebook from Google Colab, Colab takes ~1 min to execute the following cell.\n",
-                "\n",
-                "ACCOUNT_ID and AUTH_TOKEN - Authentication parameters needed for when making requests to [Mat3ra.com's API Endpoints](https://docs.mat3ra.com/rest-api/endpoints/).\n",
-                "\n",
-                "MATERIALS_PROJECT_API_KEY - Authentication parameter needed for when making requests to [Material Project's API](https://materialsproject.org/open)\n",
-                "\n",
-                "ORGANIZATION_ID - Authentication parameter needed for when working with collaborative accounts https://docs.mat3ra.com/collaboration/organizations/overview/\n",
+                "import sys\n",
+                "if sys.platform == \"emscripten\":\n",
+                "    import micropip\n",
+                "    await micropip.install('mat3ra-api-examples', deps=False)\n",
+                "from utils.jupyterlite import install_packages\n",
+                "await install_packages(\"import_material_from_jarvis_db_entry.ipynb\",\"../../config.yml\")"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "f418c51a7f794f9f",
+            "metadata": {},
+            "source": [
+                "## 3. Data Processing\n",
                 "\n",
-                "> <span style=\"color: orange\">**NOTE**</span>: If you are running this notebook from Jupyter, the variables ACCOUNT_ID, AUTH_TOKEN, MATERIALS_PROJECT_API_KEY, and ORGANIZATION_ID should be set in the file [settings.json](../../utils/settings.json) if you need to use these variables. To obtain API token parameters, please see the following link to the documentation explaining how to get them: https://docs.mat3ra.com/accounts/ui/preferences/api/"
+                "### 3.1. Get data and wrap it in dataframe"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
+            "id": "b1ee775d1476f884",
             "metadata": {
-                "cellView": "form",
-                "colab": {
-                    "base_uri": "https://localhost:8080/"
-                },
-                "id": "KenNuzjjIQAW",
-                "outputId": "1622a36b-7d5c-4798-a684-ca9f1e069ff2"
+                "collapsed": false,
+                "trusted": true
             },
             "outputs": [],
             "source": [
-                "# @title Authorization Form\n",
-                "ACCOUNT_ID = \"ACCOUNT_ID\"  # @param {type:\"string\"}\n",
-                "AUTH_TOKEN = \"AUTH_TOKEN\"  # @param {type:\"string\"}\n",
-                "MATERIALS_PROJECT_API_KEY = \"MATERIALS_PROJECT_API_KEY\"  # @param {type:\"string\"}\n",
-                "ORGANIZATION_ID = \"ORGANIZATION_ID\"  # @param {type:\"string\"}\n",
-                "\n",
-                "import os\n",
+                "import pandas as pd\n",
+                "from jarvis.db.figshare import data\n",
                 "\n",
-                "if \"COLAB_JUPYTER_IP\" in os.environ:\n",
-                "    os.environ.update(\n",
-                "        dict(\n",
-                "            ACCOUNT_ID=ACCOUNT_ID,\n",
-                "            AUTH_TOKEN=AUTH_TOKEN,\n",
-                "            MATERIALS_PROJECT_API_KEY=MATERIALS_PROJECT_API_KEY,\n",
-                "            ORGANIZATION_ID=ORGANIZATION_ID,\n",
-                "        )\n",
-                "    )\n",
-                "\n",
-                "    !GIT_BRANCH=\"dev\"; export GIT_BRANCH; curl -s \"https://raw.githubusercontent.com/Exabyte-io/api-examples/${GIT_BRANCH}/scripts/env.sh\" | bash"
+                "dft_2d = data(\"dft_2d\")\n",
+                "dft_3d = data(\"dft_3d\")\n",
+                "dataframe_2d = pd.DataFrame(dft_2d)\n",
+                "dataframe_3d = pd.DataFrame(dft_3d)\n",
+                "dataframe= pd.concat([dataframe_2d, dataframe_3d])"
             ]
         },
         {
-            "attachments": {},
             "cell_type": "markdown",
-            "metadata": {
-                "id": "t0TQd18kIQAX"
-            },
+            "id": "57b0d358",
+            "metadata": {},
             "source": [
-                "## Imports"
+                "### 3.2. Preview the dataframe"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "metadata": {
-                "id": "dX3VXdWJIQAX"
-            },
+            "id": "0e34472a",
+            "metadata": {},
             "outputs": [],
             "source": [
-                "from utils.settings import ENDPOINT_ARGS, ACCOUNT_ID\n",
-                "from utils.generic import display_JSON\n",
-                "\n",
-                "from exabyte_api_client.endpoints.workflows import WorkflowEndpoints"
+                "dataframe"
             ]
         },
         {
-            "attachments": {},
             "cell_type": "markdown",
-            "metadata": {
-                "id": "h8JubXPxIQAY"
-            },
+            "id": "15fe5f9de299c935",
+            "metadata": {},
             "source": [
-                "## Set Parameters\n",
-                "\n",
-                "- **QUERY**: A query describing the documents to find. See [Meteor collection](https://docs.meteor.com/api/collections.html#Mongo-Collection-find) for more information. \n",
-                "\n",
-                "- **limit**: Maximum number of results to return. See [Meteor collection](https://docs.meteor.com/api/collections.html#Mongo-Collection-find) for more information."
+                "### 3.3. Filter data"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "metadata": {
-                "id": "xCEktmwiIQAZ"
-            },
+            "id": "a771a36a",
+            "metadata": {},
             "outputs": [],
             "source": [
-                "QUERY = {\"name\": \"Total Energy\", \"owner._id\": ACCOUNT_ID}\n",
+                "import json\n",
+                "from express import ExPrESS\n",
                 "\n",
-                "OPTIONS = {\"limit\": 2}"
+                "dataframe_entries_for_jarvis_ids = dataframe[(dataframe[\"jid\"].isin(JARVIS_IDS))]\n",
+                "dataframe_entries_as_json = dataframe_entries_for_jarvis_ids.to_json(orient=\"records\")\n",
+                "jarvis_db_entries = json.loads(dataframe_entries_as_json)"
             ]
         },
         {
-            "attachments": {},
             "cell_type": "markdown",
-            "metadata": {
-                "id": "1fgv7cWSIQAZ"
-            },
+            "id": "ef5f9e9d",
+            "metadata": {},
             "source": [
-                "## Initialize the endpoint\n",
-                "\n",
-                "Initialize a helper class to interact with `WorkflowEndpoints`. This only has to be done once."
+                "### 3.4. Convert to ESSE format"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
+            "id": "c41fb68c6d25fe48",
             "metadata": {
-                "id": "pwEMspn7IQAa"
+                "collapsed": false,
+                "trusted": true
             },
             "outputs": [],
             "source": [
-                "endpoint = WorkflowEndpoints(*ENDPOINT_ARGS)"
+                "def convert_jarvis_entry_to_esse(jarvis_db_entry):\n",
+                "    jarvis_db_entry_json = json.dumps(jarvis_db_entry)\n",
+                "    kwargs = {\n",
+                "        \"structure_string\": jarvis_db_entry_json,\n",
+                "        \"cell_type\": \"original\",\n",
+                "        \"structure_format\": \"jarvis-db-entry\",\n",
+                "    }\n",
+                "    handler = ExPrESS(\"structure\", **kwargs)\n",
+                "    esse = handler.property(\"material\", **kwargs)\n",
+                "    poscar = handler.parser.jarvis_db_entry_json_to_poscar(jarvis_db_entry_json)\n",
+                "    return (esse, poscar)\n",
+                "\n",
+                "esse_entries = list(map(lambda e: convert_jarvis_entry_to_esse(e)[0], jarvis_db_entries))\n",
+                "poscars = list(map(lambda e: convert_jarvis_entry_to_esse(e)[1], jarvis_db_entries))"
             ]
         },
         {
-            "attachments": {},
             "cell_type": "markdown",
-            "metadata": {
-                "id": "iKpJYJYjIQAa"
-            },
+            "id": "8770ec48",
+            "metadata": {},
             "source": [
-                "## List workflows\n",
-                "\n",
-                "Contact the endpoint to list workflows according to the query above."
+                "### 3.5. Preview the data"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "metadata": {
-                "id": "wzFp8DcCIQAa"
-            },
+            "id": "860b5c1b",
+            "metadata": {},
             "outputs": [],
             "source": [
-                "workflows = endpoint.list(QUERY, OPTIONS)"
+                "from src.utils import poscar_to_ase\n",
+                "from ase.visualize import view\n",
+                "from ase.io import write\n",
+                "from ase.build import make_supercell\n",
+                "from IPython.display import Image\n",
+                "\n",
+                "# Uncomment to see the JSON\n",
+                "# print(json.dumps(data, indent=4))\n",
+                "\n",
+                "\n",
+                "materials = list(map(lambda p: poscar_to_ase(p), poscars))\n",
+                "\n",
+                "def visualize_material(material, index: int, number_of_repetitions: int = 3):\n",
+                "    \"\"\"\n",
+                "    Visualize the material using ASE's visualization tool\n",
+                "    Repeat the unit cell to make it easier to see.\n",
+                "\n",
+                "    Args:\n",
+                "        material: The material to visualize (Ase.Atoms object)\n",
+                "        index: The index of the material\n",
+                "        number_of_repetitions: The number of unit cell repetitions to visualize\n",
+                "    \"\"\"\n",
+                "    # Set the number of unit cell repetition for the structure to make it easier to see\n",
+                "    n = number_of_repetitions\n",
+                "    material_repeat = make_supercell(material, [[n,0,0],[0,n,0],[0,0,n]])\n",
+                "    filename = f\"material-{index}.png\"\n",
+                "    write(filename, material_repeat)\n",
+                "    img = Image(filename=filename)\n",
+                "    print(filename, \"-\", material.symbols)\n",
+                "    display(img)\n",
+                "\n",
+                "for idx, material in enumerate(materials):\n",
+                "    visualize_material(material, idx)"
             ]
         },
         {
-            "attachments": {},
             "cell_type": "markdown",
-            "metadata": {
-                "id": "mrZ2nEmJIQAb"
-            },
+            "id": "a4a48479c7ea090f",
+            "metadata": {},
             "source": [
-                "## Print workflows\n",
-                "\n",
-                "Print the list of workflows saved under the corresponding variable in pretty JSON below."
+                "## 4. Pass data to the outside runtime"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "metadata": {
-                "colab": {
-                    "base_uri": "https://localhost:8080/"
-                },
-                "id": "KSJgpWRzIQAb",
-                "outputId": "7ee3b7f6-208f-427e-ee32-07486078072c"
-            },
+            "id": "00b187ab",
+            "metadata": {},
             "outputs": [],
             "source": [
-                "display_JSON(workflows)"
+                "from utils.jupyterlite import set_data\n",
+                "\n",
+                "output_materials = esse_entries\n",
+                "set_data(\"materials\", output_materials)"
             ]
         }
     ],
     "metadata": {
-        "colab": {
-            "name": "get_workflows.ipynb",
-            "provenance": []
-        },
         "kernelspec": {
-            "display_name": "Python 3",
+            "display_name": ".venv",
             "language": "python",
             "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.8.6"
+            "version": "3.11.4"
+        },
+        "widgets": {
+            "application/vnd.jupyter.widget-state+json": {
+                "state": {},
+                "version_major": 2,
+                "version_minor": 0
+            }
         }
     },
     "nbformat": 4,
-    "nbformat_minor": 1
+    "nbformat_minor": 5
 }
```

### Comparing `mat3ra-api-examples-2024.4.1.post0/examples/workflow/get_workflows.py` & `mat3ra-api-examples-2024.4.3.post0/examples/workflow/get_workflows.py`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.4.1.post0/examples/workflow/qe_scf_calculation.ipynb` & `mat3ra-api-examples-2024.4.3.post0/examples/workflow/qe_scf_calculation.ipynb`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9997217382888115%*

 * *Differences: {"'cells'": '{4: {\'source\': {insert: [(7, \'import sys\\n\'), (19, \'    !GIT_BRANCH="dev"; '*

 * *            'export GIT_BRANCH; curl -s '*

 * *            '"https://raw.githubusercontent.com/Exabyte-io/api-examples/${GIT_BRANCH}/scripts/env.sh" '*

 * *            '| bash\\n\'), (20, \'\\n\'), (21, \'if sys.platform == "emscripten":\\n\'), (22, '*

 * *            '\'    apiConfig = data_from_host.get("apiConfig")\\n\'), (23, \'    '*

 * *            'os.environ.update(data_from_host.get("environ", {}))\\n\'), (24, \'    '*

 * *      […]*

```diff
@@ -57,26 +57,47 @@
                 "# @title Authorization Form\n",
                 "ACCOUNT_ID = \"ACCOUNT_ID\"  # @param {type:\"string\"}\n",
                 "AUTH_TOKEN = \"AUTH_TOKEN\"  # @param {type:\"string\"}\n",
                 "MATERIALS_PROJECT_API_KEY = \"MATERIALS_PROJECT_API_KEY\"  # @param {type:\"string\"}\n",
                 "ORGANIZATION_ID = \"ORGANIZATION_ID\"  # @param {type:\"string\"}\n",
                 "\n",
                 "import os\n",
+                "import sys\n",
                 "\n",
                 "if \"COLAB_JUPYTER_IP\" in os.environ:\n",
                 "    os.environ.update(\n",
                 "        dict(\n",
                 "            ACCOUNT_ID=ACCOUNT_ID,\n",
                 "            AUTH_TOKEN=AUTH_TOKEN,\n",
                 "            MATERIALS_PROJECT_API_KEY=MATERIALS_PROJECT_API_KEY,\n",
                 "            ORGANIZATION_ID=ORGANIZATION_ID,\n",
                 "        )\n",
                 "    )\n",
                 "\n",
-                "    !GIT_BRANCH=\"dev\"; export GIT_BRANCH; curl -s \"https://raw.githubusercontent.com/Exabyte-io/api-examples/${GIT_BRANCH}/scripts/env.sh\" | bash"
+                "    !GIT_BRANCH=\"dev\"; export GIT_BRANCH; curl -s \"https://raw.githubusercontent.com/Exabyte-io/api-examples/${GIT_BRANCH}/scripts/env.sh\" | bash\n",
+                "\n",
+                "if sys.platform == \"emscripten\":\n",
+                "    apiConfig = data_from_host.get(\"apiConfig\")\n",
+                "    os.environ.update(data_from_host.get(\"environ\", {}))\n",
+                "    os.environ.update(\n",
+                "        dict(\n",
+                "            ACCOUNT_ID=apiConfig.get(\"accountId\"),\n",
+                "            AUTH_TOKEN=apiConfig.get(\"authToken\"),\n",
+                "            MATERIALS_PROJECT_API_KEY=MATERIALS_PROJECT_API_KEY,\n",
+                "            ORGANIZATION_ID=apiConfig.get(\"organizationId\") or \"\",\n",
+                "        )\n",
+                "    )\n",
+                "\n",
+                "    import micropip\n",
+                "\n",
+                "    await micropip.install(\"mat3ra-api-examples\", deps=False)\n",
+                "    await micropip.install(\"exabyte-api-client\")\n",
+                "    from utils.jupyterlite import install_packages\n",
+                "\n",
+                "    await install_packages(\"\", \"../../config.yml\")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "504fd5dd-5411-4073-be50-62dd84baeb9b",
             "metadata": {},
```

### Comparing `mat3ra-api-examples-2024.4.1.post0/examples/workflow/qe_scf_calculation.py` & `mat3ra-api-examples-2024.4.3.post0/examples/workflow/qe_scf_calculation.py`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.4.1.post0/images/reusable-kernel.png` & `mat3ra-api-examples-2024.4.3.post0/images/reusable-kernel.png`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.4.1.post0/mat3ra_api_examples.egg-info/PKG-INFO` & `mat3ra-api-examples-2024.4.3.post0/mat3ra_api_examples.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mat3ra-api-examples
-Version: 2024.4.1.post0
+Version: 2024.4.3.post0
 Summary: Mat3ra API Examples
 Project-URL: homepage, https://exabyte-io.github.io/api-examples
 Project-URL: documentation, https://exabyte-io.github.io/api-examples
 Project-URL: repository, https://github.com/Exabyte-io/api-examples
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: ase>=3.21.1
@@ -39,15 +39,15 @@
 | Folder            | Notebook                                | Description |
 | ------------------|-----------------------------------------| ----------- |
 | [Examples/System](examples/system/)     | [Get Authentication Params](examples/system/get_authentication_params.ipynb)               | Demonstrates how to programatically find your user ID and access token.
 | [Examples/Workflow](examples/workflow/) | [Get Workflows](examples/workflow/get_workflows.ipynb)                           | Walks through how to [query](https://docs.mat3ra.com/rest-api/query-structure/) the Mat3ra API to programatically search for workflows. In this example, we search for workflows that calculate the total energy of a material.
 | [Examples/Workflow](examples/workflow/) | [Quantum Espresso Workflow and Job](examples/workflow/qe_scf_calculation.ipynb)  | Create Quantum Espresso workflow starting from QE input file; create and submit job; after the job is finished, download output file, and finally perform postprocessing analysis.
 | [Examples/Material](examples/material/) | [Get Materials by Formula](examples/material/get_materials_by_formula.ipynb)                | Shows how [queries](https://docs.mat3ra.com/rest-api/query-structure/) can be made to search for materials stored on your account by their formula. In this example, we search for a system containing Si.
 | [Examples/Material](examples/material/) | [Create Material](examples/material/create_material.ipynb)                         | Gives an overview of how materials can be generated in [JSON format](https://docs.mat3ra.com/materials/data/) and uploaded to your user account. In this example, we create an FCC Si crystal and upload it.
-| [Examples/Material](examples/material/) | [Import Materials from Materials Project](examples/material/import_materials_from_materialsproject.ipynb) | Demonstrates how materials can be imported from [Materials Project](https://materialsproject.org/about), if their Materials Project ID is known. In this example, we import monoclinic and hexagonal SiGe cells.
+| [Examples/Material](examples/material/) | [Import Materials from Materials Project](other/materialsproject/import_materials_from_materialsproject.ipynb) | Demonstrates how materials can be imported from [Materials Project](https://materialsproject.org/about), if their Materials Project ID is known. In this example, we import monoclinic and hexagonal SiGe cells.
 | [Examples/Material](examples/material/) | [Import Materials from Poscar](examples/material/upload_materials_from_file_poscar.ipynb)            | Provides an example of how materials can be imported directly from Poscar files (a common chemical file format best-known [for its use in VASP](https://www.vasp.at/wiki/index.php/Input)). In this example, we import the unit cell of SiGe.
 | [Examples/Job](examples/job/)            | [Create and Submit Job](examples/job/create_and_submit_job.ipynb)                   | Shows how to use the Mat3ra API to [create jobs](https://docs.mat3ra.com/jobs/data/) and run them on our cluster. In this example, we run a DFT calculation to get the total energy of an FCC Si unit cell using Quantum Espresso.
 | [Examples/Job](examples/job/)            | [Get File from Job](examples/job/get-file-from-job.ipynb) | Uses the Mat3ra API to query for a list of files produced by a job, describes the metadata assigned to each file, and ends by demonstrating how to download any remote file generated by a job to the local disk.
 | [Examples/Job](examples/job/)            | [Run Simulations and Extract Properties](examples/job/run-simulations-and-extract-properties.ipynb)  | Demonstrates copying a [bank workflow](https://docs.mat3ra.com/workflows/bank/) to an account and using it to calculate the [properties](https://docs.mat3ra.com/properties/overview/) of multiple materials. In this example, we determine the [band gap](https://docs.mat3ra.com/properties-directory/non-scalar/band-gaps/) of Si and Ge.
 | [Examples/Job](examples/job/)            | [ML - Train Model Predict Properties](examples/job/ml-train-model-predict-properties.ipynb)     | Demonstrates the  generation of a training dataset and subsequent training of a [machine learning](https://docs.mat3ra.com/software-directory/overview/#machine-learning) model. In this example, we calculate the band gaps of Si and SiGe, and using various materials properties as descriptors, train a model to predict their band gaps. Finally, we use this trained model to predict the band gap of Ge.
```

### Comparing `mat3ra-api-examples-2024.4.1.post0/mat3ra_api_examples.egg-info/SOURCES.txt` & `mat3ra-api-examples-2024.4.3.post0/mat3ra_api_examples.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 .gitattributes
 .gitignore
 .lycheeignore
 .pre-commit-config.yaml
 README.md
+config.yml
 mkdocs.yml
 pyproject.toml
+wheel_server.py
 .github/workflows/check_links.yml
 .github/workflows/cicd.yml
 .github/workflows/zip_release.yml
 examples/config.py
 examples/assets/README.md
 examples/assets/Si.pz-vbc.UPF
 examples/assets/bash_workflow_template.json
@@ -21,16 +23,14 @@
 examples/job/ml-train-model-predict-properties.py
 examples/job/run-simulations-and-extract-properties.ipynb
 examples/job/run-simulations-and-extract-properties.py
 examples/material/create_material.ipynb
 examples/material/create_material.py
 examples/material/get_materials_by_formula.ipynb
 examples/material/get_materials_by_formula.py
-examples/material/import_materials_from_materialsproject.ipynb
-examples/material/import_materials_from_materialsproject.py
 examples/material/upload_materials_from_file_poscar.ipynb
 examples/material/upload_materials_from_file_poscar.py
 examples/system/get_authentication_params.ipynb
 examples/system/get_authentication_params.py
 examples/workflow/get_workflows.ipynb
 examples/workflow/get_workflows.py
 examples/workflow/qe_scf_calculation.ipynb
@@ -39,14 +39,15 @@
 images/reusable-kernel.png
 mat3ra_api_examples.egg-info/PKG-INFO
 mat3ra_api_examples.egg-info/SOURCES.txt
 mat3ra_api_examples.egg-info/dependency_links.txt
 mat3ra_api_examples.egg-info/entry_points.txt
 mat3ra_api_examples.egg-info/requires.txt
 mat3ra_api_examples.egg-info/top_level.txt
+other/__init__.py
 other/assets/README.md
 other/assets/bitter-sweet.csv
 other/assets/bittersweet_xgboost.pkl
 other/assets/deepchem_smiles_vocab.txt
 other/assets/gamma_alumina_digne_et_al.poscar
 other/assets/sci_adv_dean_data.csv
 other/experiments/create_interface_with_min_energy_by_miller_indices.ipynb
@@ -56,33 +57,34 @@
 other/experiments/src
 other/experiments/uploads/Gr.json
 other/experiments/uploads/Ni.json
 other/jarvis/import_material_from_jarvis_db_entry.ipynb
 other/jarvis/run_job_using_material_from_jarvis_db.ipynb
 other/job/Smiles_Generation_Markov_Chain.ipynb
 other/job/Smiles_Generation_Markov_Chain.py
-other/jupyterlite/utils.py
 other/machine_learning/Classification_of_Bitterness_XGBoost.ipynb
 other/machine_learning/Classification_of_Bitterness_XGBoost.py
 other/machine_learning/Prediction_of_Perovskite_Unit_Cell_Volume.ipynb
 other/machine_learning/Prediction_of_Perovskite_Unit_Cell_Volume.py
 other/machine_learning/neural_network_train.ipynb
 other/machine_learning/neural_network_train.py
 other/materials_designer/Introduction.ipynb
-other/materials_designer/config.yml
+other/materials_designer/__init__.py
 other/materials_designer/create_interface_with_min_strain_zsl.ipynb
 other/materials_designer/create_interface_with_relaxation_ase_emt.ipynb
 other/materials_designer/import_material_from_jarvis_db_entry.ipynb
 other/materials_designer/import_materials_from_files.ipynb
-other/materials_designer/jupyterlite
 other/materials_designer/src/pymatgen_coherent_interface_builder.py
 other/materials_designer/src/utils.py
 other/materials_designer/uploads/README
+other/materialsproject/__init__.py
 other/materialsproject/api_interoperability_showcase.ipynb
 other/materialsproject/api_interoperability_showcase.py
+other/materialsproject/import_materials_from_materialsproject.ipynb
+other/materialsproject/import_materials_from_materialsproject.py
 other/python_transformations/1_layer_on_substrate.py
 other/python_transformations/2_strain_matching.py
 other/python_transformations/3_imports.py
 other/python_transformations/4_custom_transformation.py
 other/python_transformations/README.md
 other/webinar/adsorption-study.ipynb
 other/webinar/adsorption-study.py
@@ -93,13 +95,14 @@
 other/webinar/wulff-construction-surface-energy-study-cu.ipynb
 other/webinar/wulff-construction-surface-energy-study-cu.py
 scripts/change-branch-in-urls.sh
 scripts/env.sh
 scripts/render-notebooks.sh
 utils/__init__.py
 utils/generic.py
+utils/jupyterlite.py
 utils/material.py
 utils/notebook.py
 utils/settings.json
 utils/settings.py
 utils/web/renderjson.css
 utils/web/renderjson.js
```

### Comparing `mat3ra-api-examples-2024.4.1.post0/mkdocs.yml` & `mat3ra-api-examples-2024.4.3.post0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.4.1.post0/other/assets/README.md` & `mat3ra-api-examples-2024.4.3.post0/other/assets/README.md`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.4.1.post0/other/assets/bitter-sweet.csv` & `mat3ra-api-examples-2024.4.3.post0/other/assets/bitter-sweet.csv`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.4.1.post0/other/assets/gamma_alumina_digne_et_al.poscar` & `mat3ra-api-examples-2024.4.3.post0/other/assets/gamma_alumina_digne_et_al.poscar`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.4.1.post0/other/assets/sci_adv_dean_data.csv` & `mat3ra-api-examples-2024.4.3.post0/other/assets/sci_adv_dean_data.csv`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.4.1.post0/other/experiments/create_interface_with_min_energy_by_miller_indices.ipynb` & `mat3ra-api-examples-2024.4.3.post0/other/experiments/create_interface_with_min_energy_by_miller_indices.ipynb`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.4.1.post0/other/experiments/create_interface_with_relaxation_alignn.ipynb` & `mat3ra-api-examples-2024.4.3.post0/other/experiments/create_interface_with_relaxation_alignn.ipynb`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.4.1.post0/other/experiments/create_interface_with_relaxation_ase_emt.ipynb` & `mat3ra-api-examples-2024.4.3.post0/other/experiments/create_interface_with_relaxation_ase_emt.ipynb`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.4.1.post0/other/experiments/create_interface_with_relaxation_matgl_m3gnet.ipynb` & `mat3ra-api-examples-2024.4.3.post0/other/experiments/create_interface_with_relaxation_matgl_m3gnet.ipynb`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.4.1.post0/other/experiments/uploads/Gr.json` & `mat3ra-api-examples-2024.4.3.post0/other/experiments/uploads/Gr.json`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.4.1.post0/other/experiments/uploads/Ni.json` & `mat3ra-api-examples-2024.4.3.post0/other/experiments/uploads/Ni.json`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.4.1.post0/other/jarvis/import_material_from_jarvis_db_entry.ipynb` & `mat3ra-api-examples-2024.4.3.post0/other/jarvis/import_material_from_jarvis_db_entry.ipynb`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.4.1.post0/other/jarvis/run_job_using_material_from_jarvis_db.ipynb` & `mat3ra-api-examples-2024.4.3.post0/other/jarvis/run_job_using_material_from_jarvis_db.ipynb`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.4.1.post0/other/job/Smiles_Generation_Markov_Chain.py` & `mat3ra-api-examples-2024.4.3.post0/other/job/Smiles_Generation_Markov_Chain.py`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.4.1.post0/other/jupyterlite/utils.py` & `mat3ra-api-examples-2024.4.3.post0/utils/jupyterlite.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-from IPython.display import display, Javascript
 import json
 import os
 from enum import Enum
 
+from IPython.display import Javascript, display
+
 UPLOADS_FOLDER = "uploads"
 
 
 class EnvironmentEnum(Enum):
     PYODIDE = "pyodide"
     PYTHON = "python"
 
@@ -56,17 +57,24 @@
     Args:
         notebook_name (string): The name of the notebook for which to install packages.
         requirements_path (string): The path to the requirements file.
         verbose (bool): Whether to print the names of the installed packages and status of installation.
     """
     if ENVIRONMENT == EnvironmentEnum.PYODIDE:
         await micropip.install("pyyaml")
+        # PyYAML has to be installed before being imported in Pyodide and can't appear at the top of the file
     import yaml
 
-    with open(requirements_path, "r") as f:
+    base_path = os.getcwd()
+    if requirements_path is None:
+        requirements_file = os.path.normpath(os.path.join(base_path, "./config.yml"))
+    else:
+        requirements_file = os.path.normpath(os.path.join(base_path, requirements_path))
+
+    with open(requirements_file, "r") as f:
         requirements = yaml.safe_load(f)
 
     # Hash the requirements to avoid re-installing packages
     requirements_hash = str(hash(json.dumps(requirements)))
     if os.environ.get("requirements_hash") != requirements_hash:
         packages_default_common = requirements.get("default", {}).get("packages_common", []) or []
         packages_default_environment_specific = (
@@ -78,15 +86,16 @@
         )
         if notebook_requirements:
             packages_notebook_common = notebook_requirements.get("packages_common", []) or []
             packages_notebook_environment_specific = (
                 notebook_requirements.get(f"packages_{ENVIRONMENT.value}", []) or []
             )
         else:
-            raise ValueError(f"No packages found for notebook {notebook_name}")
+            packages_notebook_common = []
+            packages_notebook_environment_specific = []
 
         # Note: environment specific packages have to be installed first,
         # because in Pyodide common packages might depend on them
         packages = [
             *packages_default_environment_specific,
             *packages_notebook_environment_specific,
             *packages_default_common,
```

### Comparing `mat3ra-api-examples-2024.4.1.post0/other/machine_learning/Classification_of_Bitterness_XGBoost.py` & `mat3ra-api-examples-2024.4.3.post0/other/machine_learning/Classification_of_Bitterness_XGBoost.py`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.4.1.post0/other/machine_learning/Prediction_of_Perovskite_Unit_Cell_Volume.py` & `mat3ra-api-examples-2024.4.3.post0/other/machine_learning/Prediction_of_Perovskite_Unit_Cell_Volume.py`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.4.1.post0/other/machine_learning/neural_network_train.py` & `mat3ra-api-examples-2024.4.3.post0/other/machine_learning/neural_network_train.py`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.4.1.post0/other/materials_designer/Introduction.ipynb` & `mat3ra-api-examples-2024.4.3.post0/other/materials_designer/Introduction.ipynb`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.4.1.post0/other/materials_designer/config.yml` & `mat3ra-api-examples-2024.4.3.post0/config.yml`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # The following types of kernels are supported:
 # 1. python
 # 2. pyodide
 # Accordingly, the packages are installed using the kernel type, e.g., packages_pyodide.
 # The default packages are installed for all the notebooks.
 default:
   packages_common:
+    - pandas==1.5.3
     - ase==3.22.1
   packages_python:
     - pymatgen==2023.9.10
   packages_pyodide:
     - lzma
     - sqlite3
     - https://files.mat3ra.com:44318/uploads/pymatgen-2023.9.10-py3-none-any.whl
@@ -17,38 +18,36 @@
     - https://files.pythonhosted.org/packages/d9/0e/2a05efa11ea33513fbdf4a2e2576fe94fd8fa5ad226dbb9c660886390974/ruamel.yaml-0.17.32-py3-none-any.whl
     - networkx==3.2.1
     - monty==2023.11.3
     - scipy==1.11.2
     - tabulate==0.9.0
     - sympy==1.12
     - uncertainties==3.1.6
+    - jinja2
 notebooks:
   - name: create_interface_with_min_strain_zsl.ipynb
     packages_common:
-      - pandas==1.5.3
       - ipywidgets
       - plotly==5.18
       - nbformat>=4.2.0
     packages_python:
     packages_pyodide:
   - name: import_material_from_jarvis_db_entry.ipynb
     packages_common:
-      - pandas==1.5.3
       - express-py==2024.2.2.post2
       - mat3ra-esse
       - jarvis-tools
       - munch
       - setuptools
     packages_python:
     packages_pyodide:
       - https://files.mat3ra.com:44318/uploads/paginate-0.5.6-py3-none-any.whl
       - https://files.mat3ra.com:44318/uploads/watchdog-2.3.1-py3-none-any.whl
   - name: import_materials_from_files.ipynb
     packages_common:
-      - pandas==1.5.3
       - express-py==2024.2.2.post2
       - mat3ra-esse
       - munch
       - setuptools
     packages_python:
     packages_pyodide:
       - https://files.mat3ra.com:44318/uploads/paginate-0.5.6-py3-none-any.whl
```

### Comparing `mat3ra-api-examples-2024.4.1.post0/other/materials_designer/create_interface_with_min_strain_zsl.ipynb` & `mat3ra-api-examples-2024.4.3.post0/other/materials_designer/create_interface_with_min_strain_zsl.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9992904761904762%*

 * *Differences: {"'cells'": '{8: {\'source\': [\'import sys\\n\', \'if sys.platform == "emscripten":\\n\', \'    '*

 * *            'import micropip\\n\', "    await micropip.install(\'mat3ra-api-examples\', '*

 * *            'deps=False)\\n", \'from utils.jupyterlite import install_packages\\n\', \'await '*

 * *            'install_packages("create_interface_with_min_strain_zsl.ipynb","../../config.yml")\']}, '*

 * *            "10: {'source': {insert: [(0, 'from utils.jupyterlite import get_data\\n')], delete: "*

 * *            "[0]}}, 24: {'s […]*

```diff
@@ -112,17 +112,20 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "from jupyterlite.utils import install_packages\n",
-                "\n",
-                "await install_packages(\"create_interface_with_min_strain_zsl.ipynb\")"
+                "import sys\n",
+                "if sys.platform == \"emscripten\":\n",
+                "    import micropip\n",
+                "    await micropip.install('mat3ra-api-examples', deps=False)\n",
+                "from utils.jupyterlite import install_packages\n",
+                "await install_packages(\"create_interface_with_min_strain_zsl.ipynb\",\"../../config.yml\")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## 3. Load and prepare input Materials\n"
@@ -132,15 +135,15 @@
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "collapsed": false
             },
             "outputs": [],
             "source": [
-                "from jupyterlite.utils import get_data\n",
+                "from utils.jupyterlite import get_data\n",
                 "from pymatgen.analysis.structure_analyzer import SpacegroupAnalyzer\n",
                 "from src.utils import to_pymatgen\n",
                 "\n",
                 "# Get the list of input materials and load them into `materials_in` variable\n",
                 "get_data(\"materials_in\", globals())\n",
                 "\n",
                 "if \"materials_in\" in globals():\n",
@@ -427,15 +430,15 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "from src.utils import from_pymatgen\n",
-                "from jupyterlite.utils import set_data\n",
+                "from utils.jupyterlite import set_data\n",
                 "\n",
                 "materials = list(map(lambda interface_config: from_pymatgen(interface_config[\"interface\"]), selected_interfaces))\n",
                 "\n",
                 "set_data(\"materials\", materials)"
             ]
         }
     ],
```

### Comparing `mat3ra-api-examples-2024.4.1.post0/other/materials_designer/create_interface_with_relaxation_ase_emt.ipynb` & `mat3ra-api-examples-2024.4.3.post0/other/materials_designer/create_interface_with_relaxation_ase_emt.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9994661458333334%*

 * *Differences: {"'cells'": '{8: {\'source\': [\'import sys\\n\', \'if sys.platform == "emscripten":\\n\', \'    '*

 * *            'import micropip\\n\', "    await micropip.install(\'mat3ra-api-examples\', '*

 * *            'deps=False)\\n", \'from utils.jupyterlite import install_packages\\n\', \'await '*

 * *            'install_packages("create_interface_with_min_strain_zsl.ipynb","../../config.yml")\']}, '*

 * *            "10: {'source': {insert: [(0, 'from utils.jupyterlite import get_data\\n')], delete: "*

 * *            "[0]}}, 30: {'s […]*

```diff
@@ -118,17 +118,20 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "from jupyterlite.utils import install_packages\n",
-                "\n",
-                "await install_packages(\"create_interface_with_min_strain_zsl.ipynb\")"
+                "import sys\n",
+                "if sys.platform == \"emscripten\":\n",
+                "    import micropip\n",
+                "    await micropip.install('mat3ra-api-examples', deps=False)\n",
+                "from utils.jupyterlite import install_packages\n",
+                "await install_packages(\"create_interface_with_min_strain_zsl.ipynb\",\"../../config.yml\")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "collapsed": false
             },
@@ -139,15 +142,15 @@
         {
             "cell_type": "code",
             "metadata": {
                 "collapsed": false
             },
             "outputs": [],
             "source": [
-                "from jupyterlite.utils import get_data\n",
+                "from utils.jupyterlite import get_data\n",
                 "from pymatgen.analysis.structure_analyzer import SpacegroupAnalyzer\n",
                 "from src.utils import to_pymatgen\n",
                 "\n",
                 "# Get the list of input materials and load them into `materials_in` variable\n",
                 "get_data(\"materials_in\", globals())\n",
                 "\n",
                 "if \"materials_in\" in globals():\n",
@@ -685,15 +688,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "from jupyterlite.utils import set_data\n",
+                "from utils.jupyterlite import set_data\n",
                 "from src.utils import from_pymatgen\n",
                 "\n",
                 "esse_final_interface = from_pymatgen(ase_to_pymatgen(ase_final_interface))\n",
                 "esse_final_interface[\n",
                 "    'name'] = f\"{esse_final_interface['name']}, Interface, Strain: {interface_strain}, {name_relaxation_suffix}\"\n",
                 "\n",
                 "materials_out = [esse_final_interface]\n",
```

### Comparing `mat3ra-api-examples-2024.4.1.post0/other/materials_designer/import_materials_from_files.ipynb` & `mat3ra-api-examples-2024.4.3.post0/other/materials_designer/import_materials_from_files.ipynb`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9991421568627451%*

 * *Differences: {"'cells'": '{4: {\'source\': [\'import sys\\n\', \'if sys.platform == "emscripten":\\n\', \'    '*

 * *            'import micropip\\n\', "    await micropip.install(\'mat3ra-api-examples\', '*

 * *            'deps=False)\\n", \'from utils.jupyterlite import install_packages\\n\', \'await '*

 * *            'install_packages("import_materials_from_files.ipynb","../../config.yml")\']}, 16: '*

 * *            "{'source': {insert: [(0, 'from utils.jupyterlite import set_data\\n')], delete: "*

 * *            '[0]}}}'}*

```diff
@@ -66,17 +66,20 @@
             "execution_count": null,
             "id": "ef2b38a5-de7e-419e-b605-110e9e0095f5",
             "metadata": {
                 "trusted": true
             },
             "outputs": [],
             "source": [
-                "from jupyterlite.utils import install_packages\n",
-                "\n",
-                "await install_packages(\"import_materials_from_files.ipynb\")"
+                "import sys\n",
+                "if sys.platform == \"emscripten\":\n",
+                "    import micropip\n",
+                "    await micropip.install('mat3ra-api-examples', deps=False)\n",
+                "from utils.jupyterlite import install_packages\n",
+                "await install_packages(\"import_materials_from_files.ipynb\",\"../../config.yml\")"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "f418c51a7f794f9f",
             "metadata": {},
             "source": [
@@ -255,15 +258,15 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "00b187ab",
             "metadata": {},
             "outputs": [],
             "source": [
-                "from jupyterlite.utils import set_data\n",
+                "from utils.jupyterlite import set_data\n",
                 "\n",
                 "output_materials = esse_entries\n",
                 "set_data(\"materials\", output_materials)"
             ]
         }
     ],
     "metadata": {
```

### Comparing `mat3ra-api-examples-2024.4.1.post0/other/materials_designer/src/pymatgen_coherent_interface_builder.py` & `mat3ra-api-examples-2024.4.3.post0/other/materials_designer/src/pymatgen_coherent_interface_builder.py`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.4.1.post0/other/materials_designer/src/utils.py` & `mat3ra-api-examples-2024.4.3.post0/other/materials_designer/src/utils.py`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.4.1.post0/other/materialsproject/api_interoperability_showcase.ipynb` & `mat3ra-api-examples-2024.4.3.post0/other/materialsproject/api_interoperability_showcase.ipynb`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9996104336043361%*

 * *Differences: {"'cells'": '{3: {\'source\': {insert: [(7, \'import sys\\n\'), (19, \'    !GIT_BRANCH="dev"; '*

 * *            'export GIT_BRANCH; curl -s '*

 * *            '"https://raw.githubusercontent.com/Exabyte-io/api-examples/${GIT_BRANCH}/scripts/env.sh" '*

 * *            '| bash\\n\'), (20, \'\\n\'), (21, \'if sys.platform == "emscripten":\\n\'), (22, '*

 * *            '\'    apiConfig = data_from_host.get("apiConfig")\\n\'), (23, \'    ACCOUNT_ID = '*

 * *            'apiConfig.get("accountId")\\n\'), (24, \'    AUTH_TOKEN = '*

 * *      […]*

```diff
@@ -62,26 +62,47 @@
                 "# @title Authorization Form\n",
                 "ACCOUNT_ID = \"ACCOUNT_ID\"  # @param {type:\"string\"}\n",
                 "AUTH_TOKEN = \"AUTH_TOKEN\"  # @param {type:\"string\"}\n",
                 "MATERIALS_PROJECT_API_KEY = \"MATERIALS_PROJECT_API_KEY\"  # @param {type:\"string\"}\n",
                 "ORGANIZATION_ID = \"ORGANIZATION_ID\"  # @param {type:\"string\"}\n",
                 "\n",
                 "import os\n",
+                "import sys\n",
                 "\n",
                 "if \"COLAB_JUPYTER_IP\" in os.environ:\n",
                 "    os.environ.update(\n",
                 "        dict(\n",
                 "            ACCOUNT_ID=ACCOUNT_ID,\n",
                 "            AUTH_TOKEN=AUTH_TOKEN,\n",
                 "            MATERIALS_PROJECT_API_KEY=MATERIALS_PROJECT_API_KEY,\n",
                 "            ORGANIZATION_ID=ORGANIZATION_ID,\n",
                 "        )\n",
                 "    )\n",
                 "\n",
-                "    !GIT_BRANCH=\"dev\"; export GIT_BRANCH; curl -s \"https://raw.githubusercontent.com/Exabyte-io/api-examples/${GIT_BRANCH}/scripts/env.sh\" | bash"
+                "    !GIT_BRANCH=\"dev\"; export GIT_BRANCH; curl -s \"https://raw.githubusercontent.com/Exabyte-io/api-examples/${GIT_BRANCH}/scripts/env.sh\" | bash\n",
+                "\n",
+                "if sys.platform == \"emscripten\":\n",
+                "    apiConfig = data_from_host.get(\"apiConfig\")\n",
+                "    ACCOUNT_ID = apiConfig.get(\"accountId\")\n",
+                "    AUTH_TOKEN = apiConfig.get(\"authToken\")\n",
+                "    ORGANIZATION_ID = apiConfig.get(\"organizationId\") or \"\"\n",
+                "    os.environ.update(\n",
+                "        dict(\n",
+                "            ACCOUNT_ID=ACCOUNT_ID,\n",
+                "            AUTH_TOKEN=AUTH_TOKEN,\n",
+                "            MATERIALS_PROJECT_API_KEY=MATERIALS_PROJECT_API_KEY,\n",
+                "            ORGANIZATION_ID=ORGANIZATION_ID,\n",
+                "        )\n",
+                "    )\n",
+                "    \n",
+                "    import micropip\n",
+                "    await micropip.install('mat3ra-api-examples', deps=False)\n",
+                "    await micropip.install(\"exabyte-api-client\")\n",
+                "    from utils.jupyterlite import install_packages\n",
+                "    await install_packages(\"api_interoperability_showcase.ipynb\",\"../../config.yml\")"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "id": "welcome-supplement",
             "metadata": {
```

### Comparing `mat3ra-api-examples-2024.4.1.post0/other/materialsproject/api_interoperability_showcase.py` & `mat3ra-api-examples-2024.4.3.post0/other/materialsproject/api_interoperability_showcase.py`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.4.1.post0/other/python_transformations/1_layer_on_substrate.py` & `mat3ra-api-examples-2024.4.3.post0/other/python_transformations/1_layer_on_substrate.py`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.4.1.post0/other/python_transformations/2_strain_matching.py` & `mat3ra-api-examples-2024.4.3.post0/other/python_transformations/2_strain_matching.py`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.4.1.post0/other/python_transformations/3_imports.py` & `mat3ra-api-examples-2024.4.3.post0/other/python_transformations/3_imports.py`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.4.1.post0/other/python_transformations/4_custom_transformation.py` & `mat3ra-api-examples-2024.4.3.post0/other/python_transformations/4_custom_transformation.py`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.4.1.post0/other/python_transformations/README.md` & `mat3ra-api-examples-2024.4.3.post0/other/python_transformations/README.md`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.4.1.post0/other/webinar/adsorption-study.py` & `mat3ra-api-examples-2024.4.3.post0/other/webinar/adsorption-study.py`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.4.1.post0/other/webinar/generate-al2o3-slab-structures.py` & `mat3ra-api-examples-2024.4.3.post0/other/webinar/generate-al2o3-slab-structures.py`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.4.1.post0/other/webinar/predict_with_machine_learning.py` & `mat3ra-api-examples-2024.4.3.post0/other/webinar/predict_with_machine_learning.py`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.4.1.post0/other/webinar/wulff-construction-surface-energy-study-cu.py` & `mat3ra-api-examples-2024.4.3.post0/other/webinar/wulff-construction-surface-energy-study-cu.py`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.4.1.post0/pyproject.toml` & `mat3ra-api-examples-2024.4.3.post0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -79,7 +79,11 @@
 line-length = 120
 target-version = "py38"
 
 [tool.isort]
 profile = "black"
 multi_line_output = 3
 include_trailing_comma = true
+
+[[tool.mypy.overrides]]
+module = "yaml"
+ignore_missing_imports = true
```

### Comparing `mat3ra-api-examples-2024.4.1.post0/scripts/change-branch-in-urls.sh` & `mat3ra-api-examples-2024.4.3.post0/scripts/change-branch-in-urls.sh`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.4.1.post0/scripts/env.sh` & `mat3ra-api-examples-2024.4.3.post0/scripts/env.sh`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.4.1.post0/scripts/render-notebooks.sh` & `mat3ra-api-examples-2024.4.3.post0/scripts/render-notebooks.sh`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.4.1.post0/utils/generic.py` & `mat3ra-api-examples-2024.4.3.post0/utils/generic.py`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.4.1.post0/utils/material.py` & `mat3ra-api-examples-2024.4.3.post0/utils/material.py`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.4.1.post0/utils/notebook.py` & `mat3ra-api-examples-2024.4.3.post0/utils/notebook.py`

 * *Files identical despite different names*

### Comparing `mat3ra-api-examples-2024.4.1.post0/utils/settings.py` & `mat3ra-api-examples-2024.4.3.post0/utils/settings.py`

 * *Files 7% similar despite different names*

```diff
@@ -45,12 +45,12 @@
 # Advanced settings. Should not need adjustments.
 
 # HOST: Hostname of the RESTful API server. Defaults to platform.mat3ra.com.
 # PORT: The port RESTful API server is listening on. Defaults to 443.
 # VERSION: RESTFul API version. Defaults to 2018-10-01.
 # SECURE: Whether to use secure connection. Defaults to True.
 
-PORT = 443
-SECURE = True
-VERSION = "2018-10-01"
-HOST = "platform.mat3ra.com"
+PORT = os.environ.get("API_PORT", 443)
+SECURE = os.environ.get("API_SECURE") != "false"
+VERSION = os.environ.get("API_VERSION", "2018-10-01")
+HOST = os.environ.get("API_HOST", "platform.mat3ra.com")
 ENDPOINT_ARGS = [HOST, PORT, ACCOUNT_ID, AUTH_TOKEN, VERSION, SECURE]
```

### Comparing `mat3ra-api-examples-2024.4.1.post0/utils/web/renderjson.js` & `mat3ra-api-examples-2024.4.3.post0/utils/web/renderjson.js`

 * *Files identical despite different names*


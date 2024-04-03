# Comparing `tmp/easyreflectometrylib-0.0.5.tar.gz` & `tmp/easyreflectometrylib-0.0.6.tar.gz`

## Comparing `easyreflectometrylib-0.0.5.tar` & `easyreflectometrylib-0.0.6.tar`

### file list

```diff
@@ -1,134 +1,137 @@
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.5/. codecov.yml
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.5/.coveragerc
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.5/CHANGELOG.md
--rw-r--r--   0        0        0     3380 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.5/CONTRIBUTING.rst
--rw-r--r--   0        0        0     2094 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.5/Makefile
--rw-r--r--   0        0        0     2366 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.5/.github/workflows/codeql-analysis.yml
--rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.5/.github/workflows/documentation-build.yml
--rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.5/.github/workflows/ossar-analysis.yml
--rw-r--r--   0        0        0     2133 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.5/.github/workflows/python-ci.yml
--rw-r--r--   0        0        0     1179 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.5/.github/workflows/python-package.yml
--rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.5/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.5/EasyReflectometry/__init__.py
--rw-r--r--   0        0        0     2250 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.5/EasyReflectometry/data.py
--rw-r--r--   0        0        0     2532 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.5/EasyReflectometry/fitting.py
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.5/EasyReflectometry/main.py
--rw-r--r--   0        0        0     2627 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.5/EasyReflectometry/plot.py
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.5/EasyReflectometry/calculators/__init__.py
--rw-r--r--   0        0        0     5938 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.5/EasyReflectometry/calculators/calculator_base.py
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.5/EasyReflectometry/calculators/factory.py
--rw-r--r--   0        0        0     5326 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.5/EasyReflectometry/calculators/wrapper_base.py
--rw-r--r--   0        0        0     5967 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.5/EasyReflectometry/calculators/bornagain/calculator.py
--rw-r--r--   0        0        0    11345 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.5/EasyReflectometry/calculators/bornagain/wrapper.py
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.5/EasyReflectometry/calculators/refl1d/calculator.py
--rw-r--r--   0        0        0     6684 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.5/EasyReflectometry/calculators/refl1d/wrapper.py
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.5/EasyReflectometry/calculators/refnx/calculator.py
--rw-r--r--   0        0        0     5134 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.5/EasyReflectometry/calculators/refnx/wrapper.py
--rw-r--r--   0        0        0     6581 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.5/EasyReflectometry/experiment/model.py
--rw-r--r--   0        0        0     2129 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.5/EasyReflectometry/experiment/models.py
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.5/EasyReflectometry/measurement/data.py
--rw-r--r--   0        0        0      977 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.5/EasyReflectometry/sample/__init__.py
--rw-r--r--   0        0        0     2652 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.5/EasyReflectometry/sample/sample.py
--rw-r--r--   0        0        0     6316 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.5/EasyReflectometry/sample/assemblies/base_assembly.py
--rw-r--r--   0        0        0     7018 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.5/EasyReflectometry/sample/assemblies/gradient_layer.py
--rw-r--r--   0        0        0     3857 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.5/EasyReflectometry/sample/assemblies/multilayer.py
--rw-r--r--   0        0        0     3858 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.5/EasyReflectometry/sample/assemblies/repeating_multilayer.py
--rw-r--r--   0        0        0    12533 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.5/EasyReflectometry/sample/assemblies/surfactant_layer.py
--rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.5/EasyReflectometry/sample/elements/base_element.py
--rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.5/EasyReflectometry/sample/elements/base_element_collection.py
--rw-r--r--   0        0        0     1485 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.5/EasyReflectometry/sample/elements/layer_collection.py
--rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.5/EasyReflectometry/sample/elements/material_collection.py
--rw-r--r--   0        0        0     4316 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.5/EasyReflectometry/sample/elements/layers/layer.py
--rw-r--r--   0        0        0    11805 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.5/EasyReflectometry/sample/elements/layers/layer_area_per_molecule.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.5/EasyReflectometry/sample/elements/materials/material.py
--rw-r--r--   0        0        0     7243 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.5/EasyReflectometry/sample/elements/materials/material_density.py
--rw-r--r--   0        0        0     7869 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.5/EasyReflectometry/sample/elements/materials/material_mixture.py
--rw-r--r--   0        0        0     5498 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.5/EasyReflectometry/sample/elements/materials/material_solvated.py
--rw-r--r--   0        0        0     2658 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.5/EasyReflectometry/special/calculations.py
--rw-r--r--   0        0        0     2213 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.5/EasyReflectometry/special/parsing.py
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.5/docs/Makefile
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.5/docs/authors.rst
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.5/docs/calculators.rst
--rwxr-xr-x   0        0        0     5956 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.5/docs/conf.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.5/docs/contributing.rst
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.5/docs/index.rst
--rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.5/docs/installation.rst
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.5/docs/make.bat
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.5/docs/usage.rst
--rw-r--r--   0        0        0    21690 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.5/docs/_static/favicon.ico
--rw-r--r--   0        0        0   395415 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.5/docs/_static/logo.png
--rw-r--r--   0        0        0     4350 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.5/docs/_static/logo.svg
--rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.5/docs/api/api.rst
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.5/docs/api/data.rst
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.5/docs/api/model.rst
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.5/docs/api/sample.rst
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.5/docs/api/assemblies/gradient_layer.rst
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.5/docs/api/assemblies/multilayer.rst
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.5/docs/api/assemblies/repeating_multilayer.rst
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.5/docs/api/assemblies/surfactant_layer.rst
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.5/docs/api/elements/layer.rst
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.5/docs/api/elements/layer_area_per_molecule.rst
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.5/docs/api/elements/material.rst
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.5/docs/api/elements/material_density.rst
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.5/docs/api/elements/material_mixture.rst
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.5/docs/api/elements/material_solvated.rst
--rw-r--r--   0        0        0     6045 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.5/docs/sample/assemblies_library.rst
--rw-r--r--   0        0        0     2504 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.5/docs/sample/layer_library.rst
--rw-r--r--   0        0        0     3928 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.5/docs/sample/material_library.rst
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.5/docs/sample/sample.rst
--rw-r--r--   0        0        0    11193 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.5/docs/tutorials/material_solvated.ipynb
--rw-r--r--   0        0        0    16625 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.5/docs/tutorials/monolayer.ipynb
--rw-r--r--   0        0        0    15983 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.5/docs/tutorials/multi_contrast.ipynb
--rw-r--r--   0        0        0    10735 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.5/docs/tutorials/repeating.ipynb
--rw-r--r--   0        0        0    16767 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.5/docs/tutorials/simple_fitting.ipynb
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.5/docs/tutorials/tutorials.rst
--rw-r--r--   0        0        0     6072 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.5/docs/tutorials/_static/d70d2o.ort
--rw-r--r--   0        0        0     9511 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.5/docs/tutorials/_static/dspc.png
--rw-r--r--   0        0        0    28683 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.5/docs/tutorials/_static/example.ort
--rw-r--r--   0        0        0   118247 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.5/docs/tutorials/_static/monolayer.png
--rw-r--r--   0        0        0    17846 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.5/docs/tutorials/_static/monolayer.svg
--rw-r--r--   0        0        0    16065 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.5/docs/tutorials/_static/multiple.ort
--rw-r--r--   0        0        0    40781 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.5/docs/tutorials/_static/polymer_film.png
--rw-r--r--   0        0        0     7945 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.5/docs/tutorials/_static/polymer_film.svg
--rw-r--r--   0        0        0    41627 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.5/docs/tutorials/_static/repeating.png
--rw-r--r--   0        0        0    10198 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.5/docs/tutorials/_static/repeating.svg
--rw-r--r--   0        0        0    38132 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.5/docs/tutorials/_static/repeating_layers.ort
--rw-r--r--   0        0        0     5554 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.5/tests/test_data.py
--rw-r--r--   0        0        0     2060 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.5/tests/test_fitting.py
--rw-r--r--   0        0        0    29131 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.5/tests/_static/example.ort
--rw-r--r--   0        0        0     2654 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.5/tests/_static/test_example1.ort
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.5/tests/_static/test_example1.txt
--rw-r--r--   0        0        0     2928 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.5/tests/_static/test_example2.ort
--rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.5/tests/_static/test_example3.ort
--rw-r--r--   0        0        0     2802 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.5/tests/_static/test_example4.ort
--rw-r--r--   0        0        0     6068 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.5/tests/calculators/bornagain/test_bornagain_calculator.py
--rw-r--r--   0        0        0    10642 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.5/tests/calculators/bornagain/test_bornagain_wrapper.py
--rw-r--r--   0        0        0     5839 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.5/tests/calculators/refl1d/test_refl1d_calculator.py
--rw-r--r--   0        0        0    11365 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.5/tests/calculators/refl1d/test_refl1d_wrapper.py
--rw-r--r--   0        0        0     5628 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.5/tests/calculators/refnx/test_refnx_calculator.py
--rw-r--r--   0        0        0    11240 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.5/tests/calculators/refnx/test_refnx_wrapper.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.5/tests/experiment/__init__.py
--rw-r--r--   0        0        0    17764 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.5/tests/experiment/test_model.py
--rw-r--r--   0        0        0     3517 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.5/tests/sample/test_sample.py
--rw-r--r--   0        0        0     7687 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.5/tests/sample/assemblies/test_base_assembly.py
--rw-r--r--   0        0        0     7407 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.5/tests/sample/assemblies/test_gradient_layer.py
--rw-r--r--   0        0        0     7685 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.5/tests/sample/assemblies/test_multilayer.py
--rw-r--r--   0        0        0     9075 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.5/tests/sample/assemblies/test_repeating_multilayer.py
--rw-r--r--   0        0        0     8578 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.5/tests/sample/assemblies/test_surfactant_layer.py
--rw-r--r--   0        0        0     3375 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.5/tests/sample/elements/test_layer_collection.py
--rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.5/tests/sample/elements/test_material_collection.py
--rw-r--r--   0        0        0     4235 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.5/tests/sample/elements/layers/test_layer.py
--rw-r--r--   0        0        0     6828 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.5/tests/sample/elements/layers/test_layer_area_per_molecule.py
--rw-r--r--   0        0        0     2092 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.5/tests/sample/elements/materials/test_material.py
--rw-r--r--   0        0        0     2366 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.5/tests/sample/elements/materials/test_material_density.py
--rw-r--r--   0        0        0     5887 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.5/tests/sample/elements/materials/test_material_mixture.py
--rw-r--r--   0        0        0     5403 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.5/tests/sample/elements/materials/test_material_solvated.py
--rw-r--r--   0        0        0     1245 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.5/tests/special/test_calculations.py
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.5/vscode-template/README.rst
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.5/vscode-template/settings.json
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.5/.gitignore
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.5/AUTHORS.rst
--rw-r--r--   0        0        0     1538 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.5/LICENSE
--rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.5/README.rst
--rw-r--r--   0        0        0     3049 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     3203 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/. codecov.yml
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/.coveragerc
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/CHANGELOG.md
+-rw-r--r--   0        0        0     3380 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/CONTRIBUTING.rst
+-rw-r--r--   0        0        0     2094 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/Makefile
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/.github/release-drafter.yml
+-rw-r--r--   0        0        0     2366 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/.github/workflows/documentation-build.yml
+-rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/.github/workflows/ossar-analysis.yml
+-rw-r--r--   0        0        0     2133 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/.github/workflows/python-ci.yml
+-rw-r--r--   0        0        0     1179 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/.github/workflows/release-drafter-verify-pr-labels.yml
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/.github/workflows/release-drafter.yml
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/EasyReflectometry/__init__.py
+-rw-r--r--   0        0        0     2250 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/EasyReflectometry/data.py
+-rw-r--r--   0        0        0     2532 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/EasyReflectometry/fitting.py
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/EasyReflectometry/main.py
+-rw-r--r--   0        0        0     2627 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/EasyReflectometry/plot.py
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/EasyReflectometry/calculators/__init__.py
+-rw-r--r--   0        0        0     5938 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/EasyReflectometry/calculators/calculator_base.py
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/EasyReflectometry/calculators/factory.py
+-rw-r--r--   0        0        0     5326 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/EasyReflectometry/calculators/wrapper_base.py
+-rw-r--r--   0        0        0     5967 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/EasyReflectometry/calculators/bornagain/calculator.py
+-rw-r--r--   0        0        0    11345 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/EasyReflectometry/calculators/bornagain/wrapper.py
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/EasyReflectometry/calculators/refl1d/calculator.py
+-rw-r--r--   0        0        0     6684 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/EasyReflectometry/calculators/refl1d/wrapper.py
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/EasyReflectometry/calculators/refnx/calculator.py
+-rw-r--r--   0        0        0     5134 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/EasyReflectometry/calculators/refnx/wrapper.py
+-rw-r--r--   0        0        0     7240 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/EasyReflectometry/experiment/model.py
+-rw-r--r--   0        0        0     2129 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/EasyReflectometry/experiment/models.py
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/EasyReflectometry/measurement/data.py
+-rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/EasyReflectometry/sample/__init__.py
+-rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/EasyReflectometry/sample/base_core.py
+-rw-r--r--   0        0        0     3148 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/EasyReflectometry/sample/sample.py
+-rw-r--r--   0        0        0     5904 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/EasyReflectometry/sample/assemblies/base_assembly.py
+-rw-r--r--   0        0        0     7139 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/EasyReflectometry/sample/assemblies/gradient_layer.py
+-rw-r--r--   0        0        0     3864 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/EasyReflectometry/sample/assemblies/multilayer.py
+-rw-r--r--   0        0        0     3865 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/EasyReflectometry/sample/assemblies/repeating_multilayer.py
+-rw-r--r--   0        0        0    13079 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/EasyReflectometry/sample/assemblies/surfactant_layer.py
+-rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/EasyReflectometry/sample/elements/base_element_collection.py
+-rw-r--r--   0        0        0     4308 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/EasyReflectometry/sample/elements/layers/layer.py
+-rw-r--r--   0        0        0    12302 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/EasyReflectometry/sample/elements/layers/layer_area_per_molecule.py
+-rw-r--r--   0        0        0     1479 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/EasyReflectometry/sample/elements/layers/layer_collection.py
+-rw-r--r--   0        0        0     3070 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/EasyReflectometry/sample/elements/materials/material.py
+-rw-r--r--   0        0        0     1846 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/EasyReflectometry/sample/elements/materials/material_collection.py
+-rw-r--r--   0        0        0     7499 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/EasyReflectometry/sample/elements/materials/material_density.py
+-rw-r--r--   0        0        0     7781 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/EasyReflectometry/sample/elements/materials/material_mixture.py
+-rw-r--r--   0        0        0     6458 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/EasyReflectometry/sample/elements/materials/material_solvated.py
+-rw-r--r--   0        0        0     2658 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/EasyReflectometry/special/calculations.py
+-rw-r--r--   0        0        0     2213 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/EasyReflectometry/special/parsing.py
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/docs/Makefile
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/docs/authors.rst
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/docs/calculators.rst
+-rwxr-xr-x   0        0        0     5930 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/docs/conf.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/docs/contributing.rst
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/docs/index.rst
+-rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/docs/installation.rst
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/docs/make.bat
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/docs/usage.rst
+-rw-r--r--   0        0        0    21690 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/docs/_static/favicon.ico
+-rw-r--r--   0        0        0   395415 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/docs/_static/logo.png
+-rw-r--r--   0        0        0     4350 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/docs/_static/logo.svg
+-rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/docs/api/api.rst
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/docs/api/data.rst
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/docs/api/model.rst
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/docs/api/sample.rst
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/docs/api/assemblies/gradient_layer.rst
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/docs/api/assemblies/multilayer.rst
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/docs/api/assemblies/repeating_multilayer.rst
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/docs/api/assemblies/surfactant_layer.rst
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/docs/api/elements/layer.rst
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/docs/api/elements/layer_area_per_molecule.rst
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/docs/api/elements/material.rst
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/docs/api/elements/material_density.rst
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/docs/api/elements/material_mixture.rst
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/docs/api/elements/material_solvated.rst
+-rw-r--r--   0        0        0     6045 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/docs/sample/assemblies_library.rst
+-rw-r--r--   0        0        0     2504 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/docs/sample/layer_library.rst
+-rw-r--r--   0        0        0     3928 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/docs/sample/material_library.rst
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/docs/sample/sample.rst
+-rw-r--r--   0        0        0    11193 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/docs/tutorials/material_solvated.ipynb
+-rw-r--r--   0        0        0    16625 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/docs/tutorials/monolayer.ipynb
+-rw-r--r--   0        0        0    15983 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/docs/tutorials/multi_contrast.ipynb
+-rw-r--r--   0        0        0    10735 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/docs/tutorials/repeating.ipynb
+-rw-r--r--   0        0        0    16765 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/docs/tutorials/simple_fitting.ipynb
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/docs/tutorials/tutorials.rst
+-rw-r--r--   0        0        0     6072 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/docs/tutorials/_static/d70d2o.ort
+-rw-r--r--   0        0        0     9511 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/docs/tutorials/_static/dspc.png
+-rw-r--r--   0        0        0    28683 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/docs/tutorials/_static/example.ort
+-rw-r--r--   0        0        0   118247 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/docs/tutorials/_static/monolayer.png
+-rw-r--r--   0        0        0    17846 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/docs/tutorials/_static/monolayer.svg
+-rw-r--r--   0        0        0    16065 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/docs/tutorials/_static/multiple.ort
+-rw-r--r--   0        0        0    40781 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/docs/tutorials/_static/polymer_film.png
+-rw-r--r--   0        0        0     7945 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/docs/tutorials/_static/polymer_film.svg
+-rw-r--r--   0        0        0    41627 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/docs/tutorials/_static/repeating.png
+-rw-r--r--   0        0        0    10198 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/docs/tutorials/_static/repeating.svg
+-rw-r--r--   0        0        0    38132 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/docs/tutorials/_static/repeating_layers.ort
+-rw-r--r--   0        0        0     5554 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/tests/test_data.py
+-rw-r--r--   0        0        0     2060 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/tests/test_fitting.py
+-rw-r--r--   0        0        0    29131 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/tests/_static/example.ort
+-rw-r--r--   0        0        0     2654 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/tests/_static/test_example1.ort
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/tests/_static/test_example1.txt
+-rw-r--r--   0        0        0     2928 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/tests/_static/test_example2.ort
+-rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/tests/_static/test_example3.ort
+-rw-r--r--   0        0        0     2802 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/tests/_static/test_example4.ort
+-rw-r--r--   0        0        0     6068 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/tests/calculators/bornagain/test_bornagain_calculator.py
+-rw-r--r--   0        0        0    10642 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/tests/calculators/bornagain/test_bornagain_wrapper.py
+-rw-r--r--   0        0        0     5839 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/tests/calculators/refl1d/test_refl1d_calculator.py
+-rw-r--r--   0        0        0    11365 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/tests/calculators/refl1d/test_refl1d_wrapper.py
+-rw-r--r--   0        0        0     5628 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/tests/calculators/refnx/test_refnx_calculator.py
+-rw-r--r--   0        0        0    11240 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/tests/calculators/refnx/test_refnx_wrapper.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/tests/experiment/__init__.py
+-rw-r--r--   0        0        0    18616 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/tests/experiment/test_model.py
+-rw-r--r--   0        0        0     3730 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/tests/sample/test_sample.py
+-rw-r--r--   0        0        0     7687 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/tests/sample/assemblies/test_base_assembly.py
+-rw-r--r--   0        0        0     7563 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/tests/sample/assemblies/test_gradient_layer.py
+-rw-r--r--   0        0        0     7693 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/tests/sample/assemblies/test_multilayer.py
+-rw-r--r--   0        0        0     9082 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/tests/sample/assemblies/test_repeating_multilayer.py
+-rw-r--r--   0        0        0     8883 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/tests/sample/assemblies/test_surfactant_layer.py
+-rw-r--r--   0        0        0     3383 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/tests/sample/elements/test_layer_collection.py
+-rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/tests/sample/elements/test_material_collection.py
+-rw-r--r--   0        0        0     4235 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/tests/sample/elements/layers/test_layer.py
+-rw-r--r--   0        0        0     6607 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/tests/sample/elements/layers/test_layer_area_per_molecule.py
+-rw-r--r--   0        0        0     2092 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/tests/sample/elements/materials/test_material.py
+-rw-r--r--   0        0        0     2366 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/tests/sample/elements/materials/test_material_density.py
+-rw-r--r--   0        0        0     5295 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/tests/sample/elements/materials/test_material_mixture.py
+-rw-r--r--   0        0        0     5171 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/tests/sample/elements/materials/test_material_solvated.py
+-rw-r--r--   0        0        0     1245 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/tests/special/test_calculations.py
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/vscode-template/README.rst
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/vscode-template/settings.json
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/.gitignore
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/AUTHORS.rst
+-rw-r--r--   0        0        0     1538 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/LICENSE
+-rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/README.rst
+-rw-r--r--   0        0        0     3049 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     3203 2020-02-02 00:00:00.000000 easyreflectometrylib-0.0.6/PKG-INFO
```

### Comparing `easyreflectometrylib-0.0.5/CONTRIBUTING.rst` & `easyreflectometrylib-0.0.6/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `easyreflectometrylib-0.0.5/Makefile` & `easyreflectometrylib-0.0.6/Makefile`

 * *Files identical despite different names*

### Comparing `easyreflectometrylib-0.0.5/.github/workflows/codeql-analysis.yml` & `easyreflectometrylib-0.0.6/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `easyreflectometrylib-0.0.5/.github/workflows/documentation-build.yml` & `easyreflectometrylib-0.0.6/.github/workflows/documentation-build.yml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-# This pipeline
-# - builds developer documentation 
-# - pushes documentation to gh-pages branch of the same repository
+# This workflow will
+# - build developer documentation 
+# - push documentation to gh-pages branch of the same repository
 #
 # Deployment is handled by pages-build-deployment bot
 
 name: Build Documentation and Push to gh-pages Branch 
 
 # Controls when the workflow will run
 on:
@@ -22,28 +22,27 @@
   build_documentation:
     runs-on: ubuntu-latest
     steps:
     - name: Checkout
       uses: actions/checkout@master
       with:
         fetch-depth: 0 # otherwise, you will failed to push refs to dest repo
-    - name: Upgrade pip
-      run: |
-        python -m pip install --upgrade pip
     - name: Set up Python
       uses: actions/setup-python@v5
       with:
         python-version: 3.9
-    - name: Install Pandoc, EasyReflectometry and dependencies
+    - name: Install Pandoc, repo and dependencies
       run: |
         sudo apt install pandoc
         pip install . '.[docs]'
+
     - name: Build and Commit
       uses: sphinx-notes/pages@master
       with:
         install_requirements: true
-        documentation_path: docs
+        documentation_path: docs/src
     - name: Push changes
       uses: ad-m/github-push-action@master
       continue-on-error: true
       with:
-        branch: gh-pages
+        github_token: ${{ secrets.CORE_TOKEN }}
+        branch: gh-pages
```

### Comparing `easyreflectometrylib-0.0.5/.github/workflows/ossar-analysis.yml` & `easyreflectometrylib-0.0.6/.github/workflows/ossar-analysis.yml`

 * *Files identical despite different names*

### Comparing `easyreflectometrylib-0.0.5/.github/workflows/python-ci.yml` & `easyreflectometrylib-0.0.6/.github/workflows/python-ci.yml`

 * *Files identical despite different names*

### Comparing `easyreflectometrylib-0.0.5/.github/workflows/python-package.yml` & `easyreflectometrylib-0.0.6/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `easyreflectometrylib-0.0.5/.github/workflows/python-publish.yml` & `easyreflectometrylib-0.0.6/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `easyreflectometrylib-0.0.5/EasyReflectometry/data.py` & `easyreflectometrylib-0.0.6/EasyReflectometry/data.py`

 * *Files identical despite different names*

### Comparing `easyreflectometrylib-0.0.5/EasyReflectometry/fitting.py` & `easyreflectometrylib-0.0.6/EasyReflectometry/fitting.py`

 * *Files identical despite different names*

### Comparing `easyreflectometrylib-0.0.5/EasyReflectometry/plot.py` & `easyreflectometrylib-0.0.6/EasyReflectometry/plot.py`

 * *Files identical despite different names*

### Comparing `easyreflectometrylib-0.0.5/EasyReflectometry/calculators/__init__.py` & `easyreflectometrylib-0.0.6/EasyReflectometry/calculators/__init__.py`

 * *Files identical despite different names*

### Comparing `easyreflectometrylib-0.0.5/EasyReflectometry/calculators/calculator_base.py` & `easyreflectometrylib-0.0.6/EasyReflectometry/calculators/calculator_base.py`

 * *Files identical despite different names*

### Comparing `easyreflectometrylib-0.0.5/EasyReflectometry/calculators/wrapper_base.py` & `easyreflectometrylib-0.0.6/EasyReflectometry/calculators/wrapper_base.py`

 * *Files identical despite different names*

### Comparing `easyreflectometrylib-0.0.5/EasyReflectometry/calculators/bornagain/calculator.py` & `easyreflectometrylib-0.0.6/EasyReflectometry/calculators/bornagain/calculator.py`

 * *Files identical despite different names*

### Comparing `easyreflectometrylib-0.0.5/EasyReflectometry/calculators/bornagain/wrapper.py` & `easyreflectometrylib-0.0.6/EasyReflectometry/calculators/bornagain/wrapper.py`

 * *Files identical despite different names*

### Comparing `easyreflectometrylib-0.0.5/EasyReflectometry/calculators/refl1d/calculator.py` & `easyreflectometrylib-0.0.6/EasyReflectometry/calculators/refl1d/calculator.py`

 * *Files identical despite different names*

### Comparing `easyreflectometrylib-0.0.5/EasyReflectometry/calculators/refl1d/wrapper.py` & `easyreflectometrylib-0.0.6/EasyReflectometry/calculators/refl1d/wrapper.py`

 * *Files identical despite different names*

### Comparing `easyreflectometrylib-0.0.5/EasyReflectometry/calculators/refnx/calculator.py` & `easyreflectometrylib-0.0.6/EasyReflectometry/calculators/refnx/calculator.py`

 * *Files identical despite different names*

### Comparing `easyreflectometrylib-0.0.5/EasyReflectometry/calculators/refnx/wrapper.py` & `easyreflectometrylib-0.0.6/EasyReflectometry/calculators/refnx/wrapper.py`

 * *Files identical despite different names*

### Comparing `easyreflectometrylib-0.0.5/EasyReflectometry/experiment/model.py` & `easyreflectometrylib-0.0.6/EasyReflectometry/experiment/model.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,18 +5,17 @@
 from copy import deepcopy
 
 import yaml
 from easyCore import np
 from easyCore.Objects.ObjectClasses import BaseObj
 from easyCore.Objects.ObjectClasses import Parameter
 
+from EasyReflectometry.sample import BaseAssembly
 from EasyReflectometry.sample import Layer
 from EasyReflectometry.sample import LayerCollection
-from EasyReflectometry.sample import Multilayer
-from EasyReflectometry.sample import RepeatingMultilayer
 from EasyReflectometry.sample import Sample
 
 LAYER_DETAILS = {
     'scale': {
         'description': 'Scaling of the reflectomety profile',
         'url': 'https://github.com/reflectivity/edu_outreach/blob/master/refl_maths/paper.tex',
         'value': 1.0,
@@ -44,14 +43,21 @@
 
 
 class Model(BaseObj):
     """Model is the class that represents the experiment.
     It is used to store the information about the experiment and to perform the calculations.
     """
 
+    # Added in super().__init__
+    name: str
+    sample: Sample
+    scale: Parameter
+    background: Parameter
+    resolution: Parameter
+
     def __init__(
         self,
         sample: Sample,
         scale: Parameter,
         background: Parameter,
         resolution: Parameter,
         name: str = 'EasyModel',
@@ -122,24 +128,26 @@
             scale=scale,
             background=background,
             resolution=resolution,
             name=name,
             interface=interface,
         )
 
-    def add_item(self, *items: Layer | RepeatingMultilayer) -> None:
+    def add_item(self, *assemblies: list[BaseAssembly]) -> None:
         """Add a layer or item to the model sample.
 
-        :param items: Layers or items to add to model sample.
+        :param assemblies: Assemblies to add to model sample.
         """
-        for arg in items:
-            if issubclass(arg.__class__, Multilayer):
+        for arg in assemblies:
+            if issubclass(arg.__class__, BaseAssembly):
                 self.sample.append(arg)
                 if self.interface is not None:
                     self.interface().add_item_to_model(arg.uid, self.uid)
+            else:
+                raise ValueError(f'Object {arg} is not a valid type, must be a child of BaseAssembly.')
 
     def duplicate_item(self, idx: int) -> None:
         """Duplicate a given item or layer in a sample.
 
         :param idx: Index of the item or layer to duplicate
         """
         to_duplicate = self.sample[idx]
@@ -185,7 +193,19 @@
                 'sample': self.sample._dict_repr,
             }
         }
 
     def __repr__(self) -> str:
         """String representation of the layer."""
         return yaml.dump(self._dict_repr, sort_keys=False)
+
+    def as_dict(self, skip: list = None) -> dict:
+        """Produces a cleaned dict using a custom as_dict method to skip necessary things.
+        The resulting dict matches the paramters in __init__
+
+        :param skip: List of keys to skip, defaults to `None`.
+        """
+        if skip is None:
+            skip = []
+        this_dict = super().as_dict(skip=skip)
+        this_dict['sample'] = self.sample.as_dict()
+        return this_dict
```

### Comparing `easyreflectometrylib-0.0.5/EasyReflectometry/experiment/models.py` & `easyreflectometrylib-0.0.6/EasyReflectometry/experiment/models.py`

 * *Files identical despite different names*

### Comparing `easyreflectometrylib-0.0.5/EasyReflectometry/sample/__init__.py` & `easyreflectometrylib-0.0.6/EasyReflectometry/sample/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from .assemblies.base_assembly import BaseAssembly
 from .assemblies.gradient_layer import GradientLayer
 from .assemblies.multilayer import Multilayer
 from .assemblies.repeating_multilayer import RepeatingMultilayer
 from .assemblies.surfactant_layer import SurfactantLayer
-from .elements.layer_collection import LayerCollection
 from .elements.layers.layer import Layer
 from .elements.layers.layer_area_per_molecule import LayerAreaPerMolecule
-from .elements.material_collection import MaterialCollection
+from .elements.layers.layer_collection import LayerCollection
 from .elements.materials.material import Material
+from .elements.materials.material_collection import MaterialCollection
 from .elements.materials.material_mixture import MaterialMixture
 from .elements.materials.material_solvated import MaterialSolvated
 from .sample import Sample
 
 __all__ = (
     BaseAssembly,
     GradientLayer,
```

### Comparing `easyreflectometrylib-0.0.5/EasyReflectometry/sample/sample.py` & `easyreflectometrylib-0.0.6/EasyReflectometry/sample/sample.py`

 * *Files 19% similar despite different names*

```diff
@@ -72,9 +72,22 @@
     # Representation
     @property
     def _dict_repr(self) -> dict:
         """A simplified dict representation."""
         return {self.name: [i._dict_repr for i in self]}
 
     def __repr__(self) -> str:
-        """String representation of the layer."""
+        """String representation of the sample."""
         return yaml.dump(self._dict_repr, sort_keys=False)
+
+    def as_dict(self, skip: list = None) -> dict:
+        """Produces a cleaned dict using a custom as_dict method to skip necessary things.
+        The resulting dict matches the paramters in __init__
+
+        :param skip: List of keys to skip, defaults to `None`.
+        """
+        if skip is None:
+            skip = []
+        this_dict = super().as_dict(skip=skip)
+        for i, layer in enumerate(self.data):
+            this_dict['data'][i] = layer.as_dict()
+        return this_dict
```

### Comparing `easyreflectometrylib-0.0.5/EasyReflectometry/sample/assemblies/base_assembly.py` & `easyreflectometrylib-0.0.6/EasyReflectometry/sample/assemblies/base_assembly.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,18 @@
-from abc import abstractmethod
 from typing import Any
 from typing import Optional
 
-import yaml
 from easyCore.Fitting.Constraints import ObjConstraint
-from easyCore.Objects.ObjectClasses import BaseObj
 
-from ..elements.layer_collection import LayerCollection
+from ..base_core import BaseCore
 from ..elements.layers.layer import Layer
+from ..elements.layers.layer_collection import LayerCollection
 
 
-class BaseAssembly(BaseObj):
+class BaseAssembly(BaseCore):
     """Assembly of layers.
     The front layer (front_layer) is the layer the neutron beam starts in, it has an index of 0.
     The back layer (back_layer) is the final layer from which the unreflected neutron beam is transmitted,
     its index number depends on the number of finite layers in the system, but it might be accessed at index -1.
     """
 
     # Added in super().__init__
@@ -28,39 +26,27 @@
     def __init__(
         self,
         name: str,
         type: str,
         interface,
         **layers: LayerCollection,
     ):
-        super().__init__(name=name, **layers)
+        super().__init__(name=name, interface=interface, **layers)
 
-        # Updates interface using property in base object
-        self.interface = interface
         # Type is needed when fitting in EasyCore
         self._type = type
         self._roughness_constraints_setup = False
         self._thickness_constraints_setup = False
 
-    @abstractmethod
-    def default(cls, interface=None) -> Any:
-        ...
-
-    @abstractmethod
-    def _dict_repr(self) -> dict[str, str]:
-        ...
-
     @property
-    def uid(self) -> int:
-        """Get UID from the borg map"""
-        return self._borg.map.convert_id_to_key(self)
-
-    def __repr__(self) -> str:
-        """String representation of the object."""
-        return yaml.dump(self._dict_repr, sort_keys=False)
+    def type(self) -> str:
+        """Get type of the assembly.
+        Needed by the GUI.
+        """
+        return self._type
 
     @property
     def front_layer(self) -> Optional[Layer]:
         """Get the front layer in the assembly."""
         if len(self.layers) == 0:
             return None
         return self.layers[0]
@@ -73,15 +59,15 @@
         """
         if len(self.layers) == 0:
             self.layers.append(layer)
         else:
             self.layers[0] = layer
 
     @property
-    def back_layer(self) -> Optional[None]:
+    def back_layer(self) -> Optional[Layer]:
         """Get the back layer in the assembly."""
 
         if len(self.layers) < 2:
             return None
         return self.layers[-1]
 
     @back_layer.setter
```

### Comparing `easyreflectometrylib-0.0.5/EasyReflectometry/sample/assemblies/gradient_layer.py` & `easyreflectometrylib-0.0.6/EasyReflectometry/sample/assemblies/gradient_layer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 from numpy import arange
 
-from ..elements.layer_collection import LayerCollection
 from ..elements.layers.layer import Layer
+from ..elements.layers.layer_collection import LayerCollection
 from ..elements.materials.material import Material
 from .base_assembly import BaseAssembly
 
 
 class GradientLayer(BaseAssembly):
     """A set of discrete gradient layers changing from the front to the back material.
     The front layer is where the neutron beam starts in, it has an index of 0.
@@ -149,20 +149,21 @@
             'thickness': self.thickness,
             'discretisation_elements': self._discretisation_elements,
             'back_layer': self.back_layer._dict_repr,
             'front_layer': self.front_layer._dict_repr,
         }
 
     def as_dict(self, skip: list = None) -> dict:
+        """Produces a cleaned dict using a custom as_dict method to skip necessary things.
+        The resulting dict matches the paramters in __init__
+
+        :param skip: List of keys to skip, defaults to `None`.
         """
-        Cleaned dictionary. Custom as_dict method to skip generated layers.
-        """
-        if skip is None:
-            skip = []
         this_dict = super().as_dict(skip=skip)
+        # Determined in __init__
         del this_dict['layers']
         return this_dict
 
 
 def _linear_gradient(
     front_value: float,
     back_value: float,
```

### Comparing `easyreflectometrylib-0.0.5/EasyReflectometry/sample/assemblies/multilayer.py` & `easyreflectometrylib-0.0.6/EasyReflectometry/sample/assemblies/multilayer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
-from ..elements.layer_collection import LayerCollection
 from ..elements.layers.layer import Layer
+from ..elements.layers.layer_collection import LayerCollection
 from .base_assembly import BaseAssembly
 
 
 class Multilayer(BaseAssembly):
     """A multi layer is build from a single or a list of `Layer` or `LayerCollection`.
     The multi layer will arrange the layers as slabs, allowing the reflectometry to be determined from them.
     The front layer is where the neutron beam starts in, it has an index of 0.
```

### Comparing `easyreflectometrylib-0.0.5/EasyReflectometry/sample/assemblies/repeating_multilayer.py` & `easyreflectometrylib-0.0.6/EasyReflectometry/sample/assemblies/repeating_multilayer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 from copy import deepcopy
 
 from easyCore.Objects.ObjectClasses import Parameter
 
-from ..elements.layer_collection import LayerCollection
 from ..elements.layers.layer import Layer
+from ..elements.layers.layer_collection import LayerCollection
 from .multilayer import Multilayer
 
 REPEATINGMULTILAYER_DETAILS = {
     'repetitions': {
         'description': 'Number of repetitions of the given series of layers',
         'value': 1,
         'min': 1,
```

### Comparing `easyreflectometrylib-0.0.5/EasyReflectometry/sample/assemblies/surfactant_layer.py` & `easyreflectometrylib-0.0.6/EasyReflectometry/sample/assemblies/surfactant_layer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from __future__ import annotations
 
 from typing import Optional
 
 from easyCore.Fitting.Constraints import ObjConstraint
 from easyCore.Objects.ObjectClasses import Parameter
 
-from ..elements.layer_collection import LayerCollection
 from ..elements.layers.layer_area_per_molecule import LayerAreaPerMolecule
+from ..elements.layers.layer_collection import LayerCollection
 from ..elements.materials.material import Material
 from .base_assembly import BaseAssembly
 
 
 class SurfactantLayer(BaseAssembly):
     """A surfactant layer constructs a series of layers representing the
-    head and tail groups of a surfactant. 
-    This assembly allows the definition of a surfactant or lipid using the chemistry 
+    head and tail groups of a surfactant.
+    This assembly allows the definition of a surfactant or lipid using the chemistry
     of the head (head_layer) and tail (tail_layer) regions, additionally
     this approach will make the application of constraints such as conformal roughness
     or area per molecule more straight forward.
 
     More information about the usage of this assembly is available in the
     `surfactant documentation`_
 
@@ -46,22 +46,22 @@
             name=name,
             type='Surfactant Layer',
             layers=surfactant,
             interface=interface,
         )
 
         self.interface = interface
-        self.head_layer.area_per_molecule.enabled = True
+        self.head_layer._area_per_molecule.enabled = True
         area_per_molecule = ObjConstraint(
-            dependent_obj=self.head_layer.area_per_molecule,
+            dependent_obj=self.head_layer._area_per_molecule,
             operator='',
-            independent_obj=self.tail_layer.area_per_molecule,
+            independent_obj=self.tail_layer._area_per_molecule,
         )
-        self.tail_layer.area_per_molecule.user_constraints['area_per_molecule'] = area_per_molecule
-        self.tail_layer.area_per_molecule.user_constraints['area_per_molecule'].enabled = constrain_area_per_molecule
+        self.tail_layer._area_per_molecule.user_constraints['area_per_molecule'] = area_per_molecule
+        self.tail_layer._area_per_molecule.user_constraints['area_per_molecule'].enabled = constrain_area_per_molecule
 
         self._setup_roughness_constraints()
         if conformal_roughness:
             self._enable_roughness_constraints()
 
     # Class methods for instance creation
     @classmethod
@@ -87,15 +87,15 @@
             thickness=10.0,
             solvent=d2o,
             solvent_fraction=0.2,
             area_per_molecule=48.2,
             roughness=3.0,
             name='DPPC Head',
         )
-        return cls([tail, head], name='DPPC', interface=interface)
+        return cls([tail, head], interface=interface)
 
     @classmethod
     def from_pars(
         cls,
         tail_layer_molecular_formula: str,
         tail_layer_thickness: float,
         tail_layer_solvent: Material,
@@ -167,25 +167,25 @@
     def head_layer(self, layer: LayerAreaPerMolecule) -> None:
         """Set the head layer of the surfactant surface."""
         self.back_layer = layer
 
     @property
     def constrain_area_per_molecule(self) -> bool:
         """Get the area per molecule constraint status."""
-        return self.tail_layer.area_per_molecule.user_constraints['area_per_molecule'].enabled
+        return self.tail_layer._area_per_molecule.user_constraints['area_per_molecule'].enabled
 
     @constrain_area_per_molecule.setter
     def constrain_area_per_molecule(self, status: bool):
         """Set the status for the area per molecule constraint such that the head and tail layers have the
         same area per molecule.
 
         :param x: Boolean description the wanted of the constraint.
         """
-        self.tail_layer.area_per_molecule.user_constraints['area_per_molecule'].enabled = status
-        self.tail_layer.area_per_molecule.value = self.tail_layer.area_per_molecule.raw_value
+        self.tail_layer._area_per_molecule.user_constraints['area_per_molecule'].enabled = status
+        self.tail_layer._area_per_molecule.value = self.tail_layer._area_per_molecule.raw_value
 
     @property
     def conformal_roughness(self) -> bool:
         """Get the roughness constraint status."""
         return self.tail_layer.roughness.user_constraints['roughness_1'].enabled
 
     @conformal_roughness.setter
@@ -220,70 +220,82 @@
     ):
         """Constrain structural parameters between surfactant layer objects.
 
         :param another_contrast: The surfactant layer to constrain
         """
         if head_layer_thickness:
             head_layer_thickness_constraint = ObjConstraint(
-                self.head_layer.thickness, '', another_contrast.head_layer.thickness
+                dependent_obj=self.head_layer.thickness,
+                operator='',
+                independent_obj=another_contrast.head_layer.thickness,
+            )
+            another_contrast.head_layer.thickness.user_constraints[f'{another_contrast.name}'] = (
+                head_layer_thickness_constraint
             )
-            another_contrast.head_layer.thickness.user_constraints[
-                f'{another_contrast.name}'
-            ] = head_layer_thickness_constraint
         if tail_layer_thickness:
             tail_layer_thickness_constraint = ObjConstraint(
-                self.tail_layer.thickness, '', another_contrast.tail_layer.thickness
+                dependent_obj=self.tail_layer.thickness, operator='', independent_obj=another_contrast.tail_layer.thickness
+            )
+            another_contrast.tail_layer.thickness.user_constraints[f'{another_contrast.name}'] = (
+                tail_layer_thickness_constraint
             )
-            another_contrast.tail_layer.thickness.user_constraints[
-                f'{another_contrast.name}'
-            ] = tail_layer_thickness_constraint
         if head_layer_area_per_molecule:
             head_layer_area_per_molecule_constraint = ObjConstraint(
-                self.head_layer.area_per_molecule, '', another_contrast.head_layer.area_per_molecule
+                dependent_obj=self.head_layer._area_per_molecule,
+                operator='',
+                independent_obj=another_contrast.head_layer._area_per_molecule,
+            )
+            another_contrast.head_layer._area_per_molecule.user_constraints[f'{another_contrast.name}'] = (
+                head_layer_area_per_molecule_constraint
             )
-            another_contrast.head_layer.area_per_molecule.user_constraints[
-                f'{another_contrast.name}'
-            ] = head_layer_area_per_molecule_constraint
         if tail_layer_area_per_molecule:
             tail_layer_area_per_molecule_constraint = ObjConstraint(
-                self.tail_layer.area_per_molecule, '', another_contrast.tail_layer.area_per_molecule
+                dependent_obj=self.tail_layer._area_per_molecule,
+                operator='',
+                independent_obj=another_contrast.tail_layer._area_per_molecule,
+            )
+            another_contrast.tail_layer._area_per_molecule.user_constraints[f'{another_contrast.name}'] = (
+                tail_layer_area_per_molecule_constraint
             )
-            another_contrast.tail_layer.area_per_molecule.user_constraints[
-                f'{another_contrast.name}'
-            ] = tail_layer_area_per_molecule_constraint
         if head_layer_fraction:
             head_layer_fraction_constraint = ObjConstraint(
-                self.head_layer.material.fraction, '', another_contrast.head_layer.material.fraction
+                dependent_obj=self.head_layer.material._fraction,
+                operator='',
+                independent_obj=another_contrast.head_layer.material._fraction,
+            )
+            another_contrast.head_layer.material._fraction.user_constraints[f'{another_contrast.name}'] = (
+                head_layer_fraction_constraint
             )
-            another_contrast.head_layer.material.fraction.user_constraints[
-                f'{another_contrast.name}'
-            ] = head_layer_fraction_constraint
         if tail_layer_fraction:
             tail_layer_fraction_constraint = ObjConstraint(
-                self.tail_layer.material.fraction, '', another_contrast.tail_layer.material.fraction
+                dependent_obj=self.tail_layer.material._fraction,
+                operator='',
+                independent_obj=another_contrast.tail_layer.material._fraction,
+            )
+            another_contrast.tail_layer.material._fraction.user_constraints[f'{another_contrast.name}'] = (
+                tail_layer_fraction_constraint
             )
-            another_contrast.tail_layer.material.fraction.user_constraints[
-                f'{another_contrast.name}'
-            ] = tail_layer_fraction_constraint
 
     @property
     def _dict_repr(self) -> dict:
         """A simplified dict representation."""
         return {
-            'head_layer': self.head_layer._dict_repr,
-            'tail_layer': self.tail_layer._dict_repr,
-            'area per molecule constrained': self.constrain_area_per_molecule,
-            'conformal roughness': self.conformal_roughness,
+            self.name: {
+                'head_layer': self.head_layer._dict_repr,
+                'tail_layer': self.tail_layer._dict_repr,
+                'area per molecule constrained': self.constrain_area_per_molecule,
+                'conformal roughness': self.conformal_roughness,
+            }
         }
 
     def as_dict(self, skip: list = None) -> dict:
-        """Cleaned dictionary. Custom as_dict method to skip necessary things."""
-        if skip is None:
-            skip = []
+        """Produces a cleaned dict using a custom as_dict method to skip necessary things.
+        The resulting dict matches the paramters in __init__
+
+        :param skip: List of keys to skip, defaults to `None`.
+        """
         this_dict = super().as_dict(skip=skip)
-        for i in this_dict['layers']['data']:
-            del i['material']
-            del i['_scattering_length_real']
-            del i['_scattering_length_imag']
+        this_dict['layers']['data'][0] = self.tail_layer.as_dict()
+        this_dict['layers']['data'][1] = self.head_layer.as_dict()
         this_dict['constrain_area_per_molecule'] = self.constrain_area_per_molecule
         this_dict['conformal_roughness'] = self.conformal_roughness
         return this_dict
```

### Comparing `easyreflectometrylib-0.0.5/EasyReflectometry/sample/elements/base_element.py` & `easyreflectometrylib-0.0.6/EasyReflectometry/sample/elements/base_element_collection.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from abc import abstractmethod
 from typing import Any
 
 import yaml
-from easyCore.Objects.ObjectClasses import BaseObj
+from easyCore.Objects.Groups import BaseCollection
 
 
-class BaseElement(BaseObj):
+class BaseElementCollection(BaseCollection):
     def __init__(
         self,
         name: str,
         interface,
+        *args,
         **kwargs,
     ):
-        super().__init__(name=name, **kwargs)
+        super().__init__(name, *args, **kwargs)
         self.interface = interface
 
     @abstractmethod
     def default(cls, interface=None) -> Any:
         ...
 
     @abstractmethod
```

### Comparing `easyreflectometrylib-0.0.5/EasyReflectometry/sample/elements/layer_collection.py` & `easyreflectometrylib-0.0.6/EasyReflectometry/sample/elements/layers/layer_collection.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 __author__ = 'github.com/arm61'
 
-from .base_element_collection import BaseElementCollection
-from .layers.layer import Layer
+from ..base_element_collection import BaseElementCollection
+from .layer import Layer
 
 
 class LayerCollection(BaseElementCollection):
     # Added in super().__init__
     layers: list[Layer]
 
     def __init__(
```

### Comparing `easyreflectometrylib-0.0.5/EasyReflectometry/sample/elements/material_collection.py` & `easyreflectometrylib-0.0.6/EasyReflectometry/sample/elements/materials/material_collection.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 __author__ = 'github.com/arm61'
 
-from .base_element_collection import BaseElementCollection
-from .materials.material import Material
-from .materials.material_mixture import MaterialMixture
+from ..base_element_collection import BaseElementCollection
+from .material import Material
+from .material_mixture import MaterialMixture
 
 
 class MaterialCollection(BaseElementCollection):
     def __init__(
         self,
         *materials: tuple[Material | MaterialMixture],
         name: str = 'EasyMaterials',
```

### Comparing `easyreflectometrylib-0.0.5/EasyReflectometry/sample/elements/layers/layer.py` & `easyreflectometrylib-0.0.6/EasyReflectometry/sample/elements/layers/layer.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 __author__ = 'github.com/arm61'
 
 from copy import deepcopy
 
 from easyCore import np
 from easyCore.Objects.ObjectClasses import Parameter
 
-from ..base_element import BaseElement
+from ...base_core import BaseCore
 from ..materials.material import Material
 
 LAYER_DETAILS = {
     'thickness': {
         'description': 'The thickness of the layer in angstroms',
         'url': 'https://github.com/reflectivity/edu_outreach/blob/master/refl_maths/paper.tex',
         'value': 10.0,
@@ -28,15 +28,15 @@
         'min': 0.0,
         'max': np.Inf,
         'fixed': True,
     },
 }
 
 
-class Layer(BaseElement):
+class Layer(BaseCore):
     # Added in super().__init__
     #: Material that makes up the layer.
     material: Material
     #: Thickness of the layer in Angstrom.
     thickness: Parameter
     #: Roughness of the layer in Angstrom.
     roughness: Parameter
```

### Comparing `easyreflectometrylib-0.0.5/EasyReflectometry/sample/elements/layers/layer_area_per_molecule.py` & `easyreflectometrylib-0.0.6/EasyReflectometry/sample/elements/layers/layer_area_per_molecule.py`

 * *Files 6% similar despite different names*

```diff
@@ -67,15 +67,15 @@
 
     def __init__(
         self,
         molecular_formula: str,
         thickness: Parameter,
         solvent: Material,
         solvent_fraction: Parameter,
-        area_per_molecule: Parameter,
+        area_per_molecule: float,
         roughness: Parameter,
         name: str = 'EasyLayerAreaPerMolecule',
         interface=None,
     ):
         """Constructor.
 
         :param molecular_formula: Formula for the molecule in the layer.
@@ -90,68 +90,72 @@
 
         # Create the solvated molecule and corresponding constraints
         molecule = Material.from_pars(0.0, 0.0, name=molecular_formula, interface=interface)
 
         default_options = deepcopy(LAYER_AREA_PER_MOLECULE_DETAILS)
         del default_options['sl']['value']
         del default_options['isl']['value']
-        scattering_length_real = Parameter('scattering_length_real', 0.0, **default_options['sl'])
-        scattering_length_imag = Parameter('scattering_length_imag', 0.0, **default_options['isl'])
+        del default_options['area_per_molecule']['value']
+
+        # Will be added as components later in the init
+        _scattering_length_real = Parameter('scattering_length_real', 0.0, **default_options['sl'])
+        _scattering_length_imag = Parameter('scattering_length_imag', 0.0, **default_options['isl'])
+        _area_per_molecule = Parameter('area_per_molecule', area_per_molecule, **default_options['area_per_molecule'])
 
         # Constrain the real part of the sld value for the molecule
         constraint_sld_real = FunctionalConstraint(
             dependent_obj=molecule.sld,
             func=area_per_molecule_to_scattering_length_density,
-            independent_objs=[scattering_length_real, thickness, area_per_molecule],
+            independent_objs=[_scattering_length_real, thickness, _area_per_molecule],
         )
         thickness.user_constraints['area_per_molecule'] = constraint_sld_real
-        area_per_molecule.user_constraints['area_per_molecule'] = constraint_sld_real
-        scattering_length_real.user_constraints['area_per_molecule'] = constraint_sld_real
+        _area_per_molecule.user_constraints['area_per_molecule'] = constraint_sld_real
+        _scattering_length_real.user_constraints['area_per_molecule'] = constraint_sld_real
 
         # Constrain the imaginary part of the sld value for the molecule
         constraint_sld_imag = FunctionalConstraint(
             dependent_obj=molecule.isld,
             func=area_per_molecule_to_scattering_length_density,
-            independent_objs=[scattering_length_imag, thickness, area_per_molecule],
+            independent_objs=[_scattering_length_imag, thickness, _area_per_molecule],
         )
         thickness.user_constraints['iarea_per_molecule'] = constraint_sld_imag
-        area_per_molecule.user_constraints['iarea_per_molecule'] = constraint_sld_imag
-        scattering_length_imag.user_constraints['iarea_per_molecule'] = constraint_sld_imag
+        _area_per_molecule.user_constraints['iarea_per_molecule'] = constraint_sld_imag
+        _scattering_length_imag.user_constraints['iarea_per_molecule'] = constraint_sld_imag
 
         solvated_molecule = MaterialSolvated(
             material=molecule,
             solvent=solvent,
             solvent_fraction=solvent_fraction,
             interface=interface,
         )
         super().__init__(
             material=solvated_molecule,
             thickness=thickness,
             roughness=roughness,
             name=name,
             interface=interface,
         )
-        self._add_component('_scattering_length_real', scattering_length_real)
-        self._add_component('_scattering_length_imag', scattering_length_imag)
-        self._add_component('_area_per_molecule', area_per_molecule)
+        self._add_component('_scattering_length_real', _scattering_length_real)
+        self._add_component('_scattering_length_imag', _scattering_length_imag)
+        self._add_component('_area_per_molecule', _area_per_molecule)
 
         scattering_length = neutron_scattering_length(molecular_formula)
         self._scattering_length_real.value = scattering_length.real
         self._scattering_length_imag.value = scattering_length.imag
         self._molecular_formula = molecular_formula
         self.interface = interface
 
     # Class methods for instance creation
     @classmethod
     def default(cls, interface=None) -> LayerAreaPerMolecule:
         """A default instance for layer defined from molecule formula and area per molecule.
 
         :param interface: Calculator interface, defaults to `None`.
         """
-        area_per_molecule = Parameter('area_per_molecule', **LAYER_AREA_PER_MOLECULE_DETAILS['area_per_molecule'])
+        area_per_molecule = LAYER_AREA_PER_MOLECULE_DETAILS['area_per_molecule']['value']
         thickness = Parameter('thickness', **LAYER_AREA_PER_MOLECULE_DETAILS['thickness'])
         roughness = Parameter('roughness', **LAYER_AREA_PER_MOLECULE_DETAILS['roughness'])
         solvent_fraction = Parameter('solvent_fraction', **LAYER_AREA_PER_MOLECULE_DETAILS['solvent_fraction'])
         solvent = Material.from_pars(6.36, 0, 'D2O', interface=interface)
         return cls(
             molecular_formula=LAYER_AREA_PER_MOLECULE_DETAILS['molecular_formula'],
             thickness=thickness,
@@ -182,16 +186,14 @@
         :param solvent_fraction: Fraction of solvent in layer. Fx solvation or coverage.
         :param area_per_molecule: Area per molecule.
         :param roughness: Upper roughness on the layer in Angstrom.
         :param name: Identifier, defaults to 'EasyLayerAreaPerMolecule'.
         :param interface: Calculator interface, defaults to `None`.
         """
         default_options = deepcopy(LAYER_AREA_PER_MOLECULE_DETAILS)
-        del default_options['area_per_molecule']['value']
-        area_per_molecule = Parameter('area_per_molecule', area_per_molecule, **default_options['area_per_molecule'])
         del default_options['thickness']['value']
         thickness = Parameter('thickness', thickness, **default_options['thickness'])
         del default_options['roughness']['value']
         roughness = Parameter('roughness', roughness, **default_options['roughness'])
         del default_options['solvent_fraction']['value']
         solvent_fraction = Parameter('solvent_fraction', solvent_fraction, **default_options['solvent_fraction'])
 
@@ -203,17 +205,27 @@
             area_per_molecule=area_per_molecule,
             roughness=roughness,
             name=name,
             interface=interface,
         )
 
     @property
-    def area_per_molecule(self) -> Parameter:
+    def area_per_molecule(self) -> float:
         """Get the area per molecule."""
-        return self._area_per_molecule
+        return self._area_per_molecule.raw_value
+
+    @area_per_molecule.setter
+    def area_per_molecule(self, new_area_per_molecule: float) -> None:
+        """Set the area per molecule.
+
+        :param new_area_per_molecule: New area per molecule.
+        """
+        if new_area_per_molecule < 0:
+            raise ValueError('new_area_per_molecule must be greater than 0.0.')
+        self._area_per_molecule.value = new_area_per_molecule
 
     @property
     def molecule(self) -> Material:
         """Get the molecule material."""
         return self.material.material
 
     @property
@@ -226,15 +238,15 @@
         """Set the solvent material.
 
         :param new_solvent: New solvent material.
         """
         self.material.solvent = new_solvent
 
     @property
-    def solvent_fraction(self) -> Parameter:
+    def solvent_fraction(self) -> float:
         """Get the fraction of the layer occupied by the solvent.
         This could be a result of either water solvating the molecule, or incomplete surface coverage of the molecules.
         """
         return self.material.solvent_fraction
 
     @solvent_fraction.setter
     def solvent_fraction(self, solvent_fraction: float) -> None:
@@ -263,25 +275,25 @@
         self._scattering_length_imag.value = scattering_length.imag
 
         self.molecule.name = formula_string
         self.material._update_name()
 
     @property
     def _dict_repr(self) -> dict[str, str]:
-        """Dictionary representation of the :py:class:`Layerarea_per_molecule` object. Produces a simple dictionary"""
+        """Dictionary representation of the `area_per_molecule` object. Produces a simple dictionary"""
         dict_repr = super()._dict_repr
         dict_repr['molecular_formula'] = self._molecular_formula
-        dict_repr['area_per_molecule'] = f'{self.area_per_molecule.raw_value:.2f} ' f'{self.area_per_molecule.unit}'
+        dict_repr['area_per_molecule'] = f'{self.area_per_molecule:.2f} ' f'{self._area_per_molecule.unit}'
         return dict_repr
 
     def as_dict(self, skip: list = None) -> dict[str, str]:
-        """Produces a cleaned  using a austom as_dict method to skip necessary things.
+        """Produces a cleaned dict using a custom as_dict method to skip necessary things.
+        The resulting dict matches the paramters in __init__
 
-        :param skip: List of keys to skip, defaults to :py:attr:`None`.
+        :param skip: List of keys to skip, defaults to `None`.
         """
-        if skip is None:
-            skip = []
         this_dict = super().as_dict(skip=skip)
+        this_dict['solvent_fraction'] = self.material._fraction.as_dict()
         del this_dict['material']
         del this_dict['_scattering_length_real']
         del this_dict['_scattering_length_imag']
         return this_dict
```

### Comparing `easyreflectometrylib-0.0.5/EasyReflectometry/sample/elements/materials/material.py` & `easyreflectometrylib-0.0.6/EasyReflectometry/sample/elements/materials/material.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from copy import deepcopy
 from typing import ClassVar
 
 from easyCore import np
 from easyCore.Objects.ObjectClasses import Parameter
 
-from ..base_element import BaseElement
+from ...base_core import BaseCore
 
 MATERIAL_DEFAULTS = {
     'sld': {
         'description': 'The real scattering length density for a material in e-6 per squared angstrom.',
         'url': 'https://www.ncnr.nist.gov/resources/activation/',
         'value': 4.186,
         'units': '1 / angstrom ** 2',
@@ -28,15 +28,15 @@
         'min': -np.Inf,
         'max': np.Inf,
         'fixed': True,
     },
 }
 
 
-class Material(BaseElement):
+class Material(BaseCore):
     # Added in super().__init__
     sld: ClassVar[Parameter]
     isld: ClassVar[Parameter]
 
     def __init__(
         self,
         sld: Parameter,
```

### Comparing `easyreflectometrylib-0.0.5/EasyReflectometry/sample/elements/materials/material_density.py` & `easyreflectometrylib-0.0.6/EasyReflectometry/sample/elements/materials/material_density.py`

 * *Files 5% similar despite different names*

```diff
@@ -170,12 +170,21 @@
         """Dictionary representation of the instance."""
         mat_dict = super()._dict_repr
         mat_dict['chemical_structure'] = self._chemical_structure
         mat_dict['density'] = f'{self.density.raw_value:.2e} {self.density.unit}'
         return mat_dict
 
     def as_dict(self, skip: list = []) -> dict[str, str]:
-        """Custom as_dict method to skip necessary things."""
+        """Produces a cleaned dict using a custom as_dict method to skip necessary things.
+        The resulting dict matches the paramters in __init__
+
+        :param skip: List of keys to skip, defaults to `None`.
+        """
         this_dict = super().as_dict(skip=skip)
-        del this_dict['sld'], this_dict['isld'], this_dict['scattering_length_real']
-        del this_dict['scattering_length_imag'], this_dict['molecular_weight']
+        # From Material
+        del this_dict['sld']
+        del this_dict['isld']
+        # Determined in __init__
+        del this_dict['scattering_length_real']
+        del this_dict['scattering_length_imag']
+        del this_dict['molecular_weight']
         return this_dict
```

### Comparing `easyreflectometrylib-0.0.5/EasyReflectometry/sample/elements/materials/material_mixture.py` & `easyreflectometrylib-0.0.6/EasyReflectometry/sample/elements/materials/material_mixture.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from typing import Optional
 
 from easyCore.Fitting.Constraints import FunctionalConstraint
 from easyCore.Objects.ObjectClasses import Parameter
 
 from EasyReflectometry.special.calculations import weighted_average
 
-from ..base_element import BaseElement
+from ...base_core import BaseCore
 from .material import MATERIAL_DEFAULTS
 from .material import Material
 
 MATERIALMIXTURE_DEFAULTS = {
     'fraction': {
         'description': 'The fraction of material b in material a',
         'value': 0.5,
@@ -20,15 +20,15 @@
         'min': 0,
         'max': 1,
         'fixed': True,
     }
 }
 
 
-class MaterialMixture(BaseElement):
+class MaterialMixture(BaseCore):
     # Added in super().__init__
     _material_a: Material
     _material_b: Material
     _fraction: Parameter
 
     def __init__(
         self,
@@ -40,43 +40,45 @@
     ):
         """Constructor.
 
         :param material_a: The first material.
         :param material_b: The second material.
         :param fraction: The fraction of material_b in material_a.
         :param name: Name of the material, defaults to None that causes the name to be constructed.
-        :param interface: Calculator interface, defaults to :py:attr:`None`.
+        :param interface: Calculator interface, defaults to `None`.
         """
-        super().__init__(
-            name,
-            _material_a=material_a,
-            _material_b=material_b,
-            _fraction=fraction,
-            interface=interface,
-        )
-        if name is None:
-            self._update_name()
-
         sld = weighted_average(
-            a=self._material_a.sld.raw_value,
-            b=self._material_b.sld.raw_value,
-            p=self._fraction.raw_value,
+            a=material_a.sld.raw_value,
+            b=material_b.sld.raw_value,
+            p=fraction.raw_value,
         )
         isld = weighted_average(
-            a=self._material_a.isld.raw_value,
-            b=self._material_b.isld.raw_value,
-            p=self._fraction.raw_value,
+            a=material_a.isld.raw_value,
+            b=material_b.isld.raw_value,
+            p=fraction.raw_value,
         )
         default_options = deepcopy(MATERIAL_DEFAULTS)
         del default_options['sld']['value']
         del default_options['isld']['value']
 
         self._sld = Parameter('sld', sld, **default_options['sld'])
         self._isld = Parameter('isld', isld, **default_options['isld'])
 
+        # To avoid problems when setting the interface
+        # self._sld and self._isld need to be declared before calling the super constructor
+        super().__init__(
+            name,
+            _material_a=material_a,
+            _material_b=material_b,
+            _fraction=fraction,
+            interface=interface,
+        )
+        if name is None:
+            self._update_name()
+
         self._materials_constraints()
         self.interface = interface
 
     # Class constructors
     @classmethod
     def default(cls, interface=None) -> MaterialMixture:
         """Default instance for a mixture of two materials."""
@@ -101,15 +103,15 @@
     ) -> MaterialMixture:
         """Instance of mixture of two materials where the parameters are known.
 
         :param material_a: The first material.
         :param material_b: The second material.
         :param fraction: The fraction of material_b in material_a.
         :param name: Name of the material, defaults to 'EasyMaterialMixture'.
-        :param interface: Calculator interface, defaults to :py:attr:`None`.
+        :param interface: Calculator interface, defaults to `None`.
         """
         default_options = deepcopy(MATERIALMIXTURE_DEFAULTS)
         del default_options['fraction']['value']
         fraction = Parameter('fraction', fraction, **default_options['fraction'])
 
         return cls(
             material_a=material_a,
@@ -119,20 +121,20 @@
             interface=interface,
         )
 
     def _get_linkable_attributes(self):
         return [self._sld, self._isld]
 
     @property
-    def sld(self):
-        return self._sld
+    def sld(self) -> float:
+        return self._sld.raw_value
 
     @property
-    def isld(self):
-        return self._isld
+    def isld(self) -> float:
+        return self._isld.raw_value
 
     def _materials_constraints(self):
         self._sld.enabled = True
         self._isld.enabled = True
         constraint = FunctionalConstraint(
             dependent_obj=self._sld,
             func=weighted_average,
@@ -149,48 +151,27 @@
         )
         self._material_a.isld.user_constraints['isld'] = iconstraint
         self._material_b.isld.user_constraints['isld'] = iconstraint
         self._fraction.user_constraints['isld'] = iconstraint
         iconstraint()
 
     @property
-    def fraction(self) -> Parameter:
-        """
-        :return: the fraction of material a.
-        """
-        return self._fraction
+    def fraction(self) -> float:
+        """Get the fraction of material_b."""
+        return self._fraction.raw_value
 
     @fraction.setter
     def fraction(self, fraction: float) -> None:
-        """
-        Setter for fraction of material a.
-
-        :param fraction: double
-        """
-        if not isinstance(fraction, float):
-            raise ValueError('fraction must be a float')
-        self._fraction = fraction
+        """Setter for fraction of material_b.
 
-    @property
-    def fraction(self) -> Parameter:
-        """
-        :return: the fraction of material a.
-        """
-        return self._fraction
-
-    @fraction.setter
-    def fraction(self, fraction: float) -> None:
-        """
-        Setter for fraction of material a.
-
-        :param fraction: double
+        :param fraction: The fraction of material_b in material_a.
         """
         if not isinstance(fraction, float):
             raise ValueError('fraction must be a float')
-        self._fraction = fraction
+        self._fraction.raw_value = fraction
 
     @property
     def material_a(self) -> Material:
         """Getter for material_a."""
         return self._material_a
 
     @material_a.setter
@@ -227,23 +208,26 @@
 
     # Representation
     @property
     def _dict_repr(self) -> dict[str, str]:
         """A simplified dict representation."""
         return {
             self.name: {
-                'fraction': self._fraction.raw_value,
+                'fraction': f'{self._fraction.raw_value:.3f} {self._fraction.unit}',
                 'sld': f'{self._sld.raw_value:.3f}e-6 {self._sld.unit}',
                 'isld': f'{self._isld.raw_value:.3f}e-6 {self._isld.unit}',
                 'material_a': self._material_a._dict_repr,
                 'material_b': self._material_b._dict_repr,
             }
         }
 
     def as_dict(self, skip: list = None) -> dict[str, str]:
-        """Custom as_dict method to skip necessary things."""
-        if skip is None:
-            skip = []
+        """Produces a cleaned dict using a custom as_dict method to skip necessary things.
+        The resulting dict matches the paramters in __init__
+
+        :param skip: List of keys to skip, defaults to `None`.
+        """
         this_dict = super().as_dict(skip=skip)
-        this_dict['material_a'] = self._material_a
-        this_dict['material_b'] = self._material_b
+        this_dict['material_a'] = self._material_a.as_dict()
+        this_dict['material_b'] = self._material_b.as_dict()
+        this_dict['fraction'] = self._fraction.as_dict()
         return this_dict
```

### Comparing `easyreflectometrylib-0.0.5/EasyReflectometry/sample/elements/materials/material_solvated.py` & `easyreflectometrylib-0.0.6/EasyReflectometry/sample/elements/materials/material_solvated.py`

 * *Files 24% similar despite different names*

```diff
@@ -116,15 +116,15 @@
         """Set the solvent.
 
         :param new_solvent: Solvent to be used.
         """
         self.material_b = new_solvent
 
     @property
-    def solvent_fraction(self) -> Parameter:
+    def solvent_fraction(self) -> float:
         """Get the fraction of layer described by the solvent.
         This might be fraction of:
         Solvation where solvent is within the layer
         Patches of solvent in the layer where no material is present.
         """
         return self.fraction
 
@@ -149,14 +149,35 @@
 
     # Representation
     @property
     def _dict_repr(self) -> dict[str, str]:
         """A simplified dict representation."""
         return {
             self.name: {
-                'solvent_fraction': self.solvent_fraction.raw_value,
+                'solvent_fraction': f'{self._fraction.raw_value:.3f} {self._fraction.unit}',
                 'sld': f'{self._sld.raw_value:.3f}e-6 {self._sld.unit}',
                 'isld': f'{self._isld.raw_value:.3f}e-6 {self._isld.unit}',
                 'material': self.material._dict_repr,
                 'solvent': self.solvent._dict_repr,
             }
         }
+
+    def as_dict(self, skip: list = None) -> dict[str, str]:
+        """Produces a cleaned dict using a custom as_dict method to skip necessary things.
+        The resulting dict matches the paramters in __init__
+
+        :param skip: List of keys to skip, defaults to `None`.
+        """
+        this_dict = super().as_dict(skip=skip)
+        this_dict['material'] = self.material.as_dict()
+        this_dict['solvent'] = self.solvent.as_dict()
+        this_dict['solvent_fraction'] = self._fraction.as_dict()
+        # Property and protected varible from material_mixture
+        del this_dict['material_a']
+        del this_dict['_material_a']
+        # Property and protected varible from material_mixture
+        del this_dict['material_b']
+        del this_dict['_material_b']
+        # Property and protected varible from material_mixture
+        del this_dict['fraction']
+        del this_dict['_fraction']
+        return this_dict
```

### Comparing `easyreflectometrylib-0.0.5/EasyReflectometry/special/calculations.py` & `easyreflectometrylib-0.0.6/EasyReflectometry/special/calculations.py`

 * *Files identical despite different names*

### Comparing `easyreflectometrylib-0.0.5/EasyReflectometry/special/parsing.py` & `easyreflectometrylib-0.0.6/EasyReflectometry/special/parsing.py`

 * *Files identical despite different names*

### Comparing `easyreflectometrylib-0.0.5/docs/Makefile` & `easyreflectometrylib-0.0.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `easyreflectometrylib-0.0.5/docs/calculators.rst` & `easyreflectometrylib-0.0.6/docs/calculators.rst`

 * *Files identical despite different names*

### Comparing `easyreflectometrylib-0.0.5/docs/conf.py` & `easyreflectometrylib-0.0.6/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,20 +21,18 @@
 import os
 import sys
 import toml
 from pathlib import Path
 
 sys.path.insert(0, os.path.abspath('..'))
 
-main_root = Path(__file__).parents[2]
+main_root = Path(__file__).parents[1]
 sys.path.append(str(main_root))
 project_info = toml.load(os.path.join(main_root, 'pyproject.toml'))
 
-import EasyReflectometry
-
 # -- General configuration ---------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 #
 # needs_sphinx = '1.0'
 
 # Add any Sphinx extension module names here, as strings. They can be
```

### Comparing `easyreflectometrylib-0.0.5/docs/installation.rst` & `easyreflectometrylib-0.0.6/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `easyreflectometrylib-0.0.5/docs/make.bat` & `easyreflectometrylib-0.0.6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `easyreflectometrylib-0.0.5/docs/_static/favicon.ico` & `easyreflectometrylib-0.0.6/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `easyreflectometrylib-0.0.5/docs/_static/logo.png` & `easyreflectometrylib-0.0.6/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `easyreflectometrylib-0.0.5/docs/_static/logo.svg` & `easyreflectometrylib-0.0.6/docs/_static/logo.svg`

 * *Files identical despite different names*

### Comparing `easyreflectometrylib-0.0.5/docs/api/api.rst` & `easyreflectometrylib-0.0.6/docs/api/api.rst`

 * *Files identical despite different names*

### Comparing `easyreflectometrylib-0.0.5/docs/sample/assemblies_library.rst` & `easyreflectometrylib-0.0.6/docs/sample/assemblies_library.rst`

 * *Files identical despite different names*

### Comparing `easyreflectometrylib-0.0.5/docs/sample/layer_library.rst` & `easyreflectometrylib-0.0.6/docs/sample/layer_library.rst`

 * *Files identical despite different names*

### Comparing `easyreflectometrylib-0.0.5/docs/sample/material_library.rst` & `easyreflectometrylib-0.0.6/docs/sample/material_library.rst`

 * *Files identical despite different names*

### Comparing `easyreflectometrylib-0.0.5/docs/tutorials/material_solvated.ipynb` & `easyreflectometrylib-0.0.6/docs/tutorials/material_solvated.ipynb`

 * *Files identical despite different names*

### Comparing `easyreflectometrylib-0.0.5/docs/tutorials/monolayer.ipynb` & `easyreflectometrylib-0.0.6/docs/tutorials/monolayer.ipynb`

 * *Files identical despite different names*

### Comparing `easyreflectometrylib-0.0.5/docs/tutorials/multi_contrast.ipynb` & `easyreflectometrylib-0.0.6/docs/tutorials/multi_contrast.ipynb`

 * *Files identical despite different names*

### Comparing `easyreflectometrylib-0.0.5/docs/tutorials/repeating.ipynb` & `easyreflectometrylib-0.0.6/docs/tutorials/repeating.ipynb`

 * *Files identical despite different names*

### Comparing `easyreflectometrylib-0.0.5/docs/tutorials/simple_fitting.ipynb` & `easyreflectometrylib-0.0.6/docs/tutorials/simple_fitting.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999556737588653%*

 * *Differences: {"'cells'": "{30: {'source': {insert: [(6, 'subphase.roughness.bounds = (1, 15)\\n')], delete: "*

 * *            '[6]}}}'}*

```diff
@@ -337,15 +337,15 @@
             "source": [
                 "# Thicknesses\n",
                 "sio2_layer.thickness.bounds = (15, 50)\n",
                 "film_layer.thickness.bounds = (200, 300)\n",
                 "# Roughnesses\n",
                 "sio2_layer.roughness.bounds = (1, 15)\n",
                 "film_layer.roughness.bounds = (1, 15)\n",
-                "superphase.roughness.bounds = (1, 15)\n",
+                "subphase.roughness.bounds = (1, 15)\n",
                 "# Scattering length density\n",
                 "film_layer.material.sld.bounds = (0.1, 3)"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "4b909563-a780-4c35-8995-17e53d559114",
```

### Comparing `easyreflectometrylib-0.0.5/docs/tutorials/_static/d70d2o.ort` & `easyreflectometrylib-0.0.6/docs/tutorials/_static/d70d2o.ort`

 * *Files identical despite different names*

### Comparing `easyreflectometrylib-0.0.5/docs/tutorials/_static/dspc.png` & `easyreflectometrylib-0.0.6/docs/tutorials/_static/dspc.png`

 * *Files identical despite different names*

### Comparing `easyreflectometrylib-0.0.5/docs/tutorials/_static/example.ort` & `easyreflectometrylib-0.0.6/docs/tutorials/_static/example.ort`

 * *Files identical despite different names*

### Comparing `easyreflectometrylib-0.0.5/docs/tutorials/_static/monolayer.png` & `easyreflectometrylib-0.0.6/docs/tutorials/_static/monolayer.png`

 * *Files identical despite different names*

### Comparing `easyreflectometrylib-0.0.5/docs/tutorials/_static/monolayer.svg` & `easyreflectometrylib-0.0.6/docs/tutorials/_static/monolayer.svg`

 * *Files identical despite different names*

### Comparing `easyreflectometrylib-0.0.5/docs/tutorials/_static/multiple.ort` & `easyreflectometrylib-0.0.6/docs/tutorials/_static/multiple.ort`

 * *Files identical despite different names*

### Comparing `easyreflectometrylib-0.0.5/docs/tutorials/_static/polymer_film.png` & `easyreflectometrylib-0.0.6/docs/tutorials/_static/polymer_film.png`

 * *Files identical despite different names*

### Comparing `easyreflectometrylib-0.0.5/docs/tutorials/_static/polymer_film.svg` & `easyreflectometrylib-0.0.6/docs/tutorials/_static/polymer_film.svg`

 * *Files identical despite different names*

### Comparing `easyreflectometrylib-0.0.5/docs/tutorials/_static/repeating.png` & `easyreflectometrylib-0.0.6/docs/tutorials/_static/repeating.png`

 * *Files identical despite different names*

### Comparing `easyreflectometrylib-0.0.5/docs/tutorials/_static/repeating.svg` & `easyreflectometrylib-0.0.6/docs/tutorials/_static/repeating.svg`

 * *Files identical despite different names*

### Comparing `easyreflectometrylib-0.0.5/docs/tutorials/_static/repeating_layers.ort` & `easyreflectometrylib-0.0.6/docs/tutorials/_static/repeating_layers.ort`

 * *Files identical despite different names*

### Comparing `easyreflectometrylib-0.0.5/tests/test_data.py` & `easyreflectometrylib-0.0.6/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `easyreflectometrylib-0.0.5/tests/test_fitting.py` & `easyreflectometrylib-0.0.6/tests/test_fitting.py`

 * *Files identical despite different names*

### Comparing `easyreflectometrylib-0.0.5/tests/_static/example.ort` & `easyreflectometrylib-0.0.6/tests/_static/example.ort`

 * *Files identical despite different names*

### Comparing `easyreflectometrylib-0.0.5/tests/_static/test_example1.ort` & `easyreflectometrylib-0.0.6/tests/_static/test_example1.ort`

 * *Files identical despite different names*

### Comparing `easyreflectometrylib-0.0.5/tests/_static/test_example2.ort` & `easyreflectometrylib-0.0.6/tests/_static/test_example2.ort`

 * *Files identical despite different names*

### Comparing `easyreflectometrylib-0.0.5/tests/_static/test_example3.ort` & `easyreflectometrylib-0.0.6/tests/_static/test_example3.ort`

 * *Files identical despite different names*

### Comparing `easyreflectometrylib-0.0.5/tests/_static/test_example4.ort` & `easyreflectometrylib-0.0.6/tests/_static/test_example4.ort`

 * *Files identical despite different names*

### Comparing `easyreflectometrylib-0.0.5/tests/calculators/bornagain/test_bornagain_calculator.py` & `easyreflectometrylib-0.0.6/tests/calculators/bornagain/test_bornagain_calculator.py`

 * *Files identical despite different names*

### Comparing `easyreflectometrylib-0.0.5/tests/calculators/bornagain/test_bornagain_wrapper.py` & `easyreflectometrylib-0.0.6/tests/calculators/bornagain/test_bornagain_wrapper.py`

 * *Files identical despite different names*

### Comparing `easyreflectometrylib-0.0.5/tests/calculators/refl1d/test_refl1d_calculator.py` & `easyreflectometrylib-0.0.6/tests/calculators/refl1d/test_refl1d_calculator.py`

 * *Files identical despite different names*

### Comparing `easyreflectometrylib-0.0.5/tests/calculators/refl1d/test_refl1d_wrapper.py` & `easyreflectometrylib-0.0.6/tests/calculators/refl1d/test_refl1d_wrapper.py`

 * *Files identical despite different names*

### Comparing `easyreflectometrylib-0.0.5/tests/calculators/refnx/test_refnx_calculator.py` & `easyreflectometrylib-0.0.6/tests/calculators/refnx/test_refnx_calculator.py`

 * *Files identical despite different names*

### Comparing `easyreflectometrylib-0.0.5/tests/calculators/refnx/test_refnx_wrapper.py` & `easyreflectometrylib-0.0.6/tests/calculators/refnx/test_refnx_wrapper.py`

 * *Files identical despite different names*

### Comparing `easyreflectometrylib-0.0.5/tests/experiment/test_model.py` & `easyreflectometrylib-0.0.6/tests/experiment/test_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,23 +5,26 @@
 __author__ = 'github.com/arm61'
 __version__ = '0.0.1'
 
 
 import unittest
 
 import numpy as np
+import pytest
 from numpy.testing import assert_equal
 
 from EasyReflectometry.calculators import CalculatorFactory
 from EasyReflectometry.experiment.model import Model
 from EasyReflectometry.sample import Layer
 from EasyReflectometry.sample import LayerCollection
 from EasyReflectometry.sample import Material
+from EasyReflectometry.sample import Multilayer
 from EasyReflectometry.sample import RepeatingMultilayer
 from EasyReflectometry.sample import Sample
+from EasyReflectometry.sample import SurfactantLayer
 
 
 class TestModel(unittest.TestCase):
     def test_default(self):
         p = Model.default()
         assert_equal(p.name, 'EasyModel')
         assert_equal(p.interface, None)
@@ -83,21 +86,35 @@
         m2 = Material.from_pars(0.487, 0.000, 'Potassium')
         l1 = Layer.from_pars(m1, 5.0, 2.0, 'thinBoron')
         l2 = Layer.from_pars(m2, 50.0, 1.0, 'thickPotassium')
         ls1 = LayerCollection.from_pars(l1, l2, name='twoLayer1')
         ls2 = LayerCollection.from_pars(l2, l1, name='twoLayer2')
         o1 = RepeatingMultilayer.from_pars(ls1, 2.0, 'twoLayerItem1')
         o2 = RepeatingMultilayer.from_pars(ls2, 1.0, 'oneLayerItem2')
+        surfactant = SurfactantLayer.default()
+        multilayer = Multilayer.default()
         d = Sample.from_pars(o1, name='myModel')
         mod = Model.from_pars(d, 2, 1e-5, 2.0, 'newModel')
         assert_equal(len(mod.sample), 1)
         mod.add_item(o2)
         assert_equal(len(mod.sample), 2)
         assert_equal(mod.sample[1].name, 'oneLayerItem2')
         assert_equal(issubclass(mod.sample[1].__class__, RepeatingMultilayer), True)
+        mod.add_item(surfactant)
+        assert_equal(len(mod.sample), 3)
+        mod.add_item(multilayer)
+        assert_equal(len(mod.sample), 4)
+
+    def test_add_item_exception(self):
+        # When
+        mod = Model.default()
+
+        # Then Expect
+        with pytest.raises(ValueError):
+            mod.add_item('not an assembly')
 
     def test_add_item_with_interface_refnx(self):
         interface = CalculatorFactory()
         m1 = Material.from_pars(6.908, -0.278, 'Boron')
         m2 = Material.from_pars(0.487, 0.000, 'Potassium')
         l1 = Layer.from_pars(m1, 5.0, 2.0, 'thinBoron')
         l2 = Layer.from_pars(m2, 50.0, 1.0, 'thickPotassium')
@@ -316,10 +333,18 @@
         p = Model.default()
         assert (
             p.__repr__()
             == 'EasyModel:\n  scale: 1.0\n  background: 1.0e-08\n  resolution: 5.0 %\n  sample:\n    EasySample:\n    - EasyMultilayer:\n        EasyLayers:\n        - EasyLayer:\n            material:\n              EasyMaterial:\n                sld: 4.186e-6 1 / angstrom ** 2\n                isld: 0.000e-6 1 / angstrom ** 2\n            thickness: 10.000 angstrom\n            roughness: 3.300 angstrom\n        - EasyLayer:\n            material:\n              EasyMaterial:\n                sld: 4.186e-6 1 / angstrom ** 2\n                isld: 0.000e-6 1 / angstrom ** 2\n            thickness: 10.000 angstrom\n            roughness: 3.300 angstrom\n    - EasyMultilayer:\n        EasyLayers:\n        - EasyLayer:\n            material:\n              EasyMaterial:\n                sld: 4.186e-6 1 / angstrom ** 2\n                isld: 0.000e-6 1 / angstrom ** 2\n            thickness: 10.000 angstrom\n            roughness: 3.300 angstrom\n        - EasyLayer:\n            material:\n              EasyMaterial:\n                sld: 4.186e-6 1 / angstrom ** 2\n                isld: 0.000e-6 1 / angstrom ** 2\n            thickness: 10.000 angstrom\n            roughness: 3.300 angstrom\n'  # noqa: E501
         )
 
     def test_dict_round_trip(self):
-        p = Model.default()
-        q = Model.from_dict(p.as_dict())
+        interface = CalculatorFactory()
+        p = Model.default(interface)
+        surfactant = SurfactantLayer.default()
+        p.add_item(surfactant)
+        multilayer = Multilayer.default()
+        p.add_item(multilayer)
+        repeating = RepeatingMultilayer.default()
+        p.add_item(repeating)
+        src_dict = p.as_dict()
+        q = Model.from_dict(src_dict)
         assert p.as_data_dict() == q.as_data_dict()
```

### Comparing `easyreflectometrylib-0.0.5/tests/sample/test_sample.py` & `easyreflectometrylib-0.0.6/tests/sample/test_sample.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 """
 Tests for Sample class.
 """
+
 __author__ = 'github.com/arm61'
 __version__ = '0.0.1'
 
 import unittest
 
 from numpy.testing import assert_equal
 
-from EasyReflectometry.sample.assemblies.repeating_multilayer import RepeatingMultilayer
-from EasyReflectometry.sample.elements.layer_collection import LayerCollection
-from EasyReflectometry.sample.elements.layers.layer import Layer
-from EasyReflectometry.sample.elements.materials.material import Material
-from EasyReflectometry.sample.sample import Sample
+from EasyReflectometry.sample import Layer
+from EasyReflectometry.sample import LayerCollection
+from EasyReflectometry.sample import Material
+from EasyReflectometry.sample import Multilayer
+from EasyReflectometry.sample import RepeatingMultilayer
+from EasyReflectometry.sample import Sample
+from EasyReflectometry.sample import SurfactantLayer
 
 
 class TestSample(unittest.TestCase):
     def test_default(self):
         p = Sample.default()
         assert_equal(p.name, 'EasySample')
         assert_equal(p.interface, None)
@@ -59,9 +62,16 @@
         assert (
             p.__repr__()
             == 'EasySample:\n- EasyMultilayer:\n    EasyLayers:\n    - EasyLayer:\n        material:\n          EasyMaterial:\n            sld: 4.186e-6 1 / angstrom ** 2\n            isld: 0.000e-6 1 / angstrom ** 2\n        thickness: 10.000 angstrom\n        roughness: 3.300 angstrom\n    - EasyLayer:\n        material:\n          EasyMaterial:\n            sld: 4.186e-6 1 / angstrom ** 2\n            isld: 0.000e-6 1 / angstrom ** 2\n        thickness: 10.000 angstrom\n        roughness: 3.300 angstrom\n- EasyMultilayer:\n    EasyLayers:\n    - EasyLayer:\n        material:\n          EasyMaterial:\n            sld: 4.186e-6 1 / angstrom ** 2\n            isld: 0.000e-6 1 / angstrom ** 2\n        thickness: 10.000 angstrom\n        roughness: 3.300 angstrom\n    - EasyLayer:\n        material:\n          EasyMaterial:\n            sld: 4.186e-6 1 / angstrom ** 2\n            isld: 0.000e-6 1 / angstrom ** 2\n        thickness: 10.000 angstrom\n        roughness: 3.300 angstrom\n'  # noqa: E501
         )
 
     def test_dict_round_trip(self):
         p = Sample.default()
+        surfactant = SurfactantLayer.default()
+        p.append(surfactant)
+        multilayer = Multilayer.default()
+        p.append(multilayer)
+        repeating = RepeatingMultilayer.default()
+        p.append(repeating)
+
         q = Sample.from_dict(p.as_dict())
         assert p.as_data_dict() == q.as_data_dict()
```

### Comparing `easyreflectometrylib-0.0.5/tests/sample/assemblies/test_base_assembly.py` & `easyreflectometrylib-0.0.6/tests/sample/assemblies/test_base_assembly.py`

 * *Files identical despite different names*

### Comparing `easyreflectometrylib-0.0.5/tests/sample/assemblies/test_gradient_layer.py` & `easyreflectometrylib-0.0.6/tests/sample/assemblies/test_gradient_layer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Tests for GradientLayer class module
 """
+
 from unittest.mock import MagicMock
 
 import pytest
 from numpy.testing import assert_almost_equal
 
 import EasyReflectometry.sample.assemblies.gradient_layer
 from EasyReflectometry.sample.assemblies.gradient_layer import GradientLayer
@@ -174,7 +175,13 @@
     assert mock_Material.from_pars.call_args_list[1][0] == (2.0, 2.0)
     assert mock_Material.from_pars.call_args_list[2][0] == (3.0, 3.0)
     assert mock_Layer.from_pars.call_count == 3
     assert mock_Layer.from_pars.call_args_list[0][1]['material'] == 'Material_from_pars'
     assert mock_Layer.from_pars.call_args_list[0][1]['thickness'] == 0.0
     assert mock_Layer.from_pars.call_args_list[0][1]['name'] == '0'
     assert mock_Layer.from_pars.call_args_list[0][1]['interface'] is None
+
+
+def test_dict_round_trip():
+    p = GradientLayer.default()
+    q = GradientLayer.from_dict(p.as_dict())
+    assert p.as_data_dict() == q.as_data_dict()
```

### Comparing `easyreflectometrylib-0.0.5/tests/sample/assemblies/test_multilayer.py` & `easyreflectometrylib-0.0.6/tests/sample/assemblies/test_multilayer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 """
 Tests for MultiLayer class module
 """
+
 __author__ = 'github.com/arm61'
 __version__ = '0.0.1'
 
 import unittest
 
 from numpy.testing import assert_equal
 from numpy.testing import assert_raises
 
 from EasyReflectometry.calculators.factory import CalculatorFactory
 from EasyReflectometry.sample.assemblies.multilayer import Multilayer
-from EasyReflectometry.sample.elements.layer_collection import LayerCollection
 from EasyReflectometry.sample.elements.layers.layer import Layer
+from EasyReflectometry.sample.elements.layers.layer_collection import LayerCollection
 from EasyReflectometry.sample.elements.materials.material import Material
 
 
 class TestMultilayer(unittest.TestCase):
     def test_default(self):
         p = Multilayer.default()
         assert_equal(p.name, 'EasyMultilayer')
```

### Comparing `easyreflectometrylib-0.0.5/tests/sample/assemblies/test_repeating_multilayer.py` & `easyreflectometrylib-0.0.6/tests/sample/assemblies/test_repeating_multilayer.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 import unittest
 
 from numpy.testing import assert_equal
 from numpy.testing import assert_raises
 
 from EasyReflectometry.calculators import CalculatorFactory
 from EasyReflectometry.sample.assemblies.repeating_multilayer import RepeatingMultilayer
-from EasyReflectometry.sample.elements.layer_collection import LayerCollection
 from EasyReflectometry.sample.elements.layers.layer import Layer
+from EasyReflectometry.sample.elements.layers.layer_collection import LayerCollection
 from EasyReflectometry.sample.elements.materials.material import Material
 
 
 class TestRepeatingMultilayer(unittest.TestCase):
     def test_default(self):
         p = RepeatingMultilayer.default()
         assert_equal(p.name, 'EasyRepeatingMultilayer')
```

### Comparing `easyreflectometrylib-0.0.5/tests/sample/assemblies/test_surfactant_layer.py` & `easyreflectometrylib-0.0.6/tests/sample/assemblies/test_surfactant_layer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 """
 Tests for SurfactantLayer class module
 """
+
 __author__ = 'github.com/arm61'
 __version__ = '0.0.1'
 
 
 import unittest
 
 from EasyReflectometry.sample.assemblies.surfactant_layer import SurfactantLayer
 from EasyReflectometry.sample.elements.layers.layer import Layer
 from EasyReflectometry.sample.elements.materials.material import Material
 
 
 class TestSurfactantLayer(unittest.TestCase):
     def test_default(self):
         p = SurfactantLayer.default()
-        assert p.name == 'DPPC'
+        assert p.name == 'EasySurfactantLayer'
         assert p._type == 'Surfactant Layer'
 
         assert p.layers[0].name == 'DPPC Tail'
         assert p.front_layer.name == 'DPPC Tail'
         assert p.tail_layer.name == 'DPPC Tail'
         assert p.tail_layer.molecular_formula == 'C32D64'
 
@@ -33,39 +34,39 @@
         noth2o = Material.from_pars(0.561, 0, 'nH2O')
         p = SurfactantLayer.from_pars('C8O10H12P', 12, h2o, 0.5, 50, 2, 'C10H24', 10, noth2o, 0.2, 40, 3, name='A Test')
         assert p.layers[0].name == 'A Test Tail Layer'
         assert p.tail_layer.name == 'A Test Tail Layer'
         assert p.tail_layer.molecular_formula == 'C8O10H12P'
         assert p.tail_layer.thickness.raw_value == 12
         assert p.tail_layer.solvent.as_data_dict() == h2o.as_data_dict()
-        assert p.tail_layer.solvent_fraction.raw_value == 0.5
-        assert p.tail_layer.area_per_molecule.raw_value == 50
+        assert p.tail_layer.solvent_fraction == 0.5
+        assert p.tail_layer.area_per_molecule == 50
         assert p.tail_layer.roughness.raw_value == 2
         assert p.layers[1].name == 'A Test Head Layer'
         assert p.head_layer.name == 'A Test Head Layer'
         assert p.head_layer.molecular_formula == 'C10H24'
         assert p.head_layer.thickness.raw_value == 10
         assert p.head_layer.solvent.as_data_dict() == noth2o.as_data_dict()
-        assert p.head_layer.solvent_fraction.raw_value == 0.2
-        assert p.head_layer.area_per_molecule.raw_value == 40
+        assert p.head_layer.solvent_fraction == 0.2
+        assert p.head_layer.area_per_molecule == 40
         assert p.name == 'A Test'
 
     def test_constraint_area_per_molecule(self):
         p = SurfactantLayer.default()
-        p.tail_layer.area_per_molecule.value = 30
-        assert p.tail_layer.area_per_molecule.raw_value == 30.0
-        assert p.head_layer.area_per_molecule.raw_value == 48.2
+        p.tail_layer._area_per_molecule.value = 30
+        assert p.tail_layer.area_per_molecule == 30.0
+        assert p.head_layer.area_per_molecule == 48.2
         assert p.constrain_area_per_molecule is False
         p.constrain_area_per_molecule = True
-        assert p.tail_layer.area_per_molecule.raw_value == 30
-        assert p.head_layer.area_per_molecule.raw_value == 30
+        assert p.tail_layer.area_per_molecule == 30
+        assert p.head_layer.area_per_molecule == 30
         assert p.constrain_area_per_molecule is True
-        p.tail_layer.area_per_molecule.value = 40
-        assert p.tail_layer.area_per_molecule.raw_value == 40
-        assert p.head_layer.area_per_molecule.raw_value == 40
+        p.tail_layer._area_per_molecule.value = 40
+        assert p.tail_layer.area_per_molecule == 40
+        assert p.head_layer.area_per_molecule == 40
 
     def test_conformal_roughness(self):
         p = SurfactantLayer.default()
         p.tail_layer.roughness.value = 2
         assert p.tail_layer.roughness.raw_value == 2
         assert p.head_layer.roughness.raw_value == 3
         p.conformal_roughness = True
@@ -93,54 +94,60 @@
         assert p.tail_layer.roughness.raw_value == 4
         assert p.head_layer.roughness.raw_value == 4
         assert layer.roughness.raw_value == 4
 
     def test_dict_repr(self):
         p = SurfactantLayer.default()
         assert p._dict_repr == {
-            'head_layer': {
-                'DPPC Head': {
-                    'material': {
-                        'C10H18NO8P in D2O': {
-                            'solvent_fraction': 0.2,
-                            'sld': '2.269e-6 1 / angstrom ** 2',
-                            'isld': '0.000e-6 1 / angstrom ** 2',
-                            'material': {
-                                'C10H18NO8P': {'sld': '1.246e-6 1 / angstrom ** 2', 'isld': '0.000e-6 1 / angstrom ** 2'}
-                            },
-                            'solvent': {'D2O': {'sld': '6.360e-6 1 / angstrom ** 2', 'isld': '0.000e-6 1 / angstrom ** 2'}},
-                        }
+            'EasySurfactantLayer': {
+                'head_layer': {
+                    'DPPC Head': {
+                        'material': {
+                            'C10H18NO8P in D2O': {
+                                'solvent_fraction': '0.200 dimensionless',
+                                'sld': '2.269e-6 1 / angstrom ** 2',
+                                'isld': '0.000e-6 1 / angstrom ** 2',
+                                'material': {
+                                    'C10H18NO8P': {'sld': '1.246e-6 1 / angstrom ** 2', 'isld': '0.000e-6 1 / angstrom ** 2'}
+                                },
+                                'solvent': {
+                                    'D2O': {'sld': '6.360e-6 1 / angstrom ** 2', 'isld': '0.000e-6 1 / angstrom ** 2'}
+                                },
+                            }
+                        },
+                        'thickness': '10.000 angstrom',
+                        'roughness': '3.000 angstrom',
                     },
-                    'thickness': '10.000 angstrom',
-                    'roughness': '3.000 angstrom',
+                    'molecular_formula': 'C10H18NO8P',
+                    'area_per_molecule': '48.20 angstrom ** 2',
                 },
-                'molecular_formula': 'C10H18NO8P',
-                'area_per_molecule': '48.20 angstrom ** 2',
-            },
-            'tail_layer': {
-                'DPPC Tail': {
-                    'material': {
-                        'C32D64 in Air': {
-                            'solvent_fraction': 0.0,
-                            'sld': '8.297e-6 1 / angstrom ** 2',
-                            'isld': '0.000e-6 1 / angstrom ** 2',
-                            'material': {
-                                'C32D64': {'sld': '8.297e-6 1 / angstrom ** 2', 'isld': '0.000e-6 1 / angstrom ** 2'}
-                            },
-                            'solvent': {'Air': {'sld': '0.000e-6 1 / angstrom ** 2', 'isld': '0.000e-6 1 / angstrom ** 2'}},
-                        }
+                'tail_layer': {
+                    'DPPC Tail': {
+                        'material': {
+                            'C32D64 in Air': {
+                                'solvent_fraction': '0.000 dimensionless',
+                                'sld': '8.297e-6 1 / angstrom ** 2',
+                                'isld': '0.000e-6 1 / angstrom ** 2',
+                                'material': {
+                                    'C32D64': {'sld': '8.297e-6 1 / angstrom ** 2', 'isld': '0.000e-6 1 / angstrom ** 2'}
+                                },
+                                'solvent': {
+                                    'Air': {'sld': '0.000e-6 1 / angstrom ** 2', 'isld': '0.000e-6 1 / angstrom ** 2'}
+                                },
+                            }
+                        },
+                        'thickness': '16.000 angstrom',
+                        'roughness': '3.000 angstrom',
                     },
-                    'thickness': '16.000 angstrom',
-                    'roughness': '3.000 angstrom',
+                    'molecular_formula': 'C32D64',
+                    'area_per_molecule': '48.20 angstrom ** 2',
                 },
-                'molecular_formula': 'C32D64',
-                'area_per_molecule': '48.20 angstrom ** 2',
-            },
-            'area per molecule constrained': False,
-            'conformal roughness': False,
+                'area per molecule constrained': False,
+                'conformal roughness': False,
+            }
         }
 
     def test_get_head_layer(self):
         # When
         p = SurfactantLayer.default()
 
         # Then Expect
```

### Comparing `easyreflectometrylib-0.0.5/tests/sample/elements/test_layer_collection.py` & `easyreflectometrylib-0.0.6/tests/sample/elements/test_layer_collection.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 """
 Tests for LayerCollection class.
 """
+
 __author__ = 'github.com/arm61'
 __version__ = '0.0.1'
 
 import unittest
 
 from numpy.testing import assert_equal
 
 from EasyReflectometry.sample.assemblies.repeating_multilayer import RepeatingMultilayer
-from EasyReflectometry.sample.elements.layer_collection import LayerCollection
 from EasyReflectometry.sample.elements.layers.layer import Layer
+from EasyReflectometry.sample.elements.layers.layer_collection import LayerCollection
 from EasyReflectometry.sample.elements.materials.material import Material
 
 
 class TestLayerCollection(unittest.TestCase):
     def test_default(self):
         p = LayerCollection.default()
         assert_equal(p.name, 'EasyLayers')
```

### Comparing `easyreflectometrylib-0.0.5/tests/sample/elements/test_material_collection.py` & `easyreflectometrylib-0.0.6/tests/sample/elements/test_material_collection.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """
 Tests for LayerCollection class.
 """
+
 __author__ = 'github.com/arm61'
 __version__ = '0.0.1'
 
 import unittest
 
-from EasyReflectometry.sample.elements.material_collection import MaterialCollection
 from EasyReflectometry.sample.elements.materials.material import Material
+from EasyReflectometry.sample.elements.materials.material_collection import MaterialCollection
 
 
 class TestLayerCollection(unittest.TestCase):
     def test_default(self):
         p = MaterialCollection.default()
         assert p.name == 'EasyMaterials'
         assert p.interface is None
```

### Comparing `easyreflectometrylib-0.0.5/tests/sample/elements/layers/test_layer.py` & `easyreflectometrylib-0.0.6/tests/sample/elements/layers/test_layer.py`

 * *Files identical despite different names*

### Comparing `easyreflectometrylib-0.0.5/tests/sample/elements/layers/test_layer_area_per_molecule.py` & `easyreflectometrylib-0.0.6/tests/sample/elements/layers/test_layer_area_per_molecule.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,156 +1,157 @@
 """
 Tests for LayerAreaPerMolecule class.
 """
+
 import unittest
 
 from numpy.testing import assert_almost_equal
 
 from EasyReflectometry.sample.elements.layers.layer_area_per_molecule import LayerAreaPerMolecule
 from EasyReflectometry.sample.elements.materials.material import Material
 
 
 class TestLayerAreaPerMolecule(unittest.TestCase):
     def test_default(self):
         p = LayerAreaPerMolecule.default()
         assert p.molecular_formula == 'C10H18NO8P'
-        assert p.area_per_molecule.raw_value == 48.2
-        assert str(p.area_per_molecule.unit) == 'angstrom ** 2'
-        assert p.area_per_molecule.fixed is True
+        assert p.area_per_molecule == 48.2
+        assert str(p._area_per_molecule.unit) == 'angstrom ** 2'
+        assert p._area_per_molecule.fixed is True
         assert p.thickness.raw_value == 10.0
         assert str(p.thickness.unit) == 'angstrom'
         assert p.thickness.fixed is True
         assert p.roughness.raw_value == 3.3
         assert str(p.roughness.unit) == 'angstrom'
         assert p.roughness.fixed is True
-        assert_almost_equal(p.material.sld.raw_value, 2.2691419)
-        assert_almost_equal(p.material.isld.raw_value, 0)
+        assert_almost_equal(p.material.sld, 2.2691419)
+        assert_almost_equal(p.material.isld, 0)
         assert p.material.name == 'C10H18NO8P in D2O'
         assert p.solvent.sld.raw_value == 6.36
         assert p.solvent.isld.raw_value == 0
         assert p.solvent.name == 'D2O'
-        assert p.solvent_fraction.raw_value == 0.2
-        assert str(p.solvent_fraction.unit) == 'dimensionless'
-        assert p.solvent_fraction.fixed is True
+        assert p.solvent_fraction == 0.2
+        assert str(p.material._fraction.unit) == 'dimensionless'
+        assert p.material._fraction.fixed is True
 
     def test_from_pars(self):
         h2o = Material.from_pars(-0.561, 0, 'H2O')
         p = LayerAreaPerMolecule.from_pars(
             molecular_formula='C8O10H12P',
             thickness=12,
             solvent=h2o,
             solvent_fraction=0.5,
             area_per_molecule=50,
             roughness=2,
             name='PG/H2O',
         )
         assert p.molecular_formula == 'C8O10H12P'
-        assert p.area_per_molecule.raw_value == 50
+        assert p.area_per_molecule == 50
         assert p.thickness.raw_value == 12
         assert p.roughness.raw_value == 2
         assert p.solvent.sld.raw_value == -0.561
         assert p.solvent.isld.raw_value == 0
-        assert p.solvent_fraction.raw_value == 0.5
+        assert p.solvent_fraction == 0.5
 
     def test_from_pars_constraint(self):
         h2o = Material.from_pars(-0.561, 0, 'H2O')
         p = LayerAreaPerMolecule.from_pars(
             molecular_formula='C8O10H12P',
             thickness=12,
             solvent=h2o,
             solvent_fraction=0.5,
             area_per_molecule=50,
             roughness=2,
             name='PG/H2O',
         )
         assert p.molecular_formula == 'C8O10H12P'
-        assert p.area_per_molecule.raw_value == 50
-        assert_almost_equal(p.material.sld.raw_value, 0.31513666667)
+        assert p.area_per_molecule == 50
+        assert_almost_equal(p.material.sld, 0.31513666667)
         assert p.thickness.raw_value == 12
         assert p.roughness.raw_value == 2
         assert p.solvent.sld.raw_value == -0.561
         assert p.solvent.isld.raw_value == 0
-        assert p.solvent_fraction.raw_value == 0.5
-        p.area_per_molecule.value = 30
-        assert p.area_per_molecule.raw_value == 30
-        assert_almost_equal(p.material.sld.raw_value, 0.712227778)
+        assert p.solvent_fraction == 0.5
+        p.area_per_molecule = 30
+        assert p.area_per_molecule == 30
+        assert_almost_equal(p.material.sld, 0.712227778)
         p.thickness.value = 10
         assert p.thickness.raw_value == 10
-        assert_almost_equal(p.material.sld.raw_value, 0.910773333)
+        assert_almost_equal(p.material.sld, 0.910773333)
 
     def test_solvent_change(self):
         h2o = Material.from_pars(-0.561, 0, 'H2O')
         p = LayerAreaPerMolecule.from_pars(
             molecular_formula='C8O10H12P',
             thickness=12,
             solvent=h2o,
             solvent_fraction=0.5,
             area_per_molecule=50,
             roughness=2,
             name='PG/H2O',
         )
         assert p.molecular_formula == 'C8O10H12P'
-        assert p.area_per_molecule.raw_value == 50
+        assert p.area_per_molecule == 50
         print(p.material)
-        assert_almost_equal(p.material.sld.raw_value, 0.31513666667)
+        assert_almost_equal(p.material.sld, 0.31513666667)
         assert p.thickness.raw_value == 12
         assert p.roughness.raw_value == 2
         assert p.solvent.sld.raw_value == -0.561
         assert p.solvent.isld.raw_value == 0
-        assert p.solvent_fraction.raw_value == 0.5
+        assert p.solvent_fraction == 0.5
         d2o = Material.from_pars(6.335, 0, 'D2O')
         p.solvent = d2o
         assert p.molecular_formula == 'C8O10H12P'
-        assert p.area_per_molecule.raw_value == 50
-        assert_almost_equal(p.material.sld.raw_value, 3.7631366667)
+        assert p.area_per_molecule == 50
+        assert_almost_equal(p.material.sld, 3.7631366667)
         assert p.thickness.raw_value == 12
         assert p.roughness.raw_value == 2
         assert p.solvent.sld.raw_value == 6.335
         assert p.solvent.isld.raw_value == 0
-        assert p.solvent_fraction.raw_value == 0.5
+        assert p.solvent_fraction == 0.5
 
     def test_molecular_formula_change(self):
         h2o = Material.from_pars(-0.561, 0, 'H2O')
         p = LayerAreaPerMolecule.from_pars(
             molecular_formula='C8O10H12P',
             thickness=12,
             solvent=h2o,
             solvent_fraction=0.5,
             area_per_molecule=50,
             roughness=2,
             name='PG/H2O',
         )
         assert p.molecular_formula == 'C8O10H12P'
-        assert p.area_per_molecule.raw_value == 50
-        assert_almost_equal(p.material.sld.raw_value, 0.31513666667)
+        assert p.area_per_molecule == 50
+        assert_almost_equal(p.material.sld, 0.31513666667)
         assert p.thickness.raw_value == 12
         assert p.roughness.raw_value == 2
 
         assert p.solvent.sld.raw_value == -0.561
         assert p.solvent.isld.raw_value == 0
-        assert p.solvent_fraction.raw_value == 0.5
+        assert p.solvent_fraction == 0.5
         assert p.material.name == 'C8O10H12P in H2O'
         p.molecular_formula = 'C8O10D12P'
         assert p.molecular_formula == 'C8O10D12P'
-        assert p.area_per_molecule.raw_value == 50
-        assert_almost_equal(p.material.sld.raw_value, 1.3566266666666666)
+        assert p.area_per_molecule == 50
+        assert_almost_equal(p.material.sld, 1.3566266666666666)
         assert p.thickness.raw_value == 12
         assert p.roughness.raw_value == 2
         assert p.solvent.sld.raw_value == -0.561
         assert p.solvent.isld.raw_value == 0
-        assert p.solvent_fraction.raw_value == 0.5
+        assert p.solvent_fraction == 0.5
         assert p.material.name == 'C8O10D12P in H2O'
 
     def test_dict_repr(self):
         p = LayerAreaPerMolecule.default()
         assert p._dict_repr == {
             'EasyLayerAreaPerMolecule': {
                 'material': {
                     'C10H18NO8P in D2O': {
-                        'solvent_fraction': 0.2,
+                        'solvent_fraction': '0.200 dimensionless',
                         'sld': '2.269e-6 1 / angstrom ** 2',
                         'isld': '0.000e-6 1 / angstrom ** 2',
                         'material': {
                             'C10H18NO8P': {'sld': '1.246e-6 1 / angstrom ** 2', 'isld': '0.000e-6 1 / angstrom ** 2'}
                         },
                         'solvent': {'D2O': {'sld': '6.360e-6 1 / angstrom ** 2', 'isld': '0.000e-6 1 / angstrom ** 2'}},
                     }
```

### Comparing `easyreflectometrylib-0.0.5/tests/sample/elements/materials/test_material.py` & `easyreflectometrylib-0.0.6/tests/sample/elements/materials/test_material.py`

 * *Files identical despite different names*

### Comparing `easyreflectometrylib-0.0.5/tests/sample/elements/materials/test_material_density.py` & `easyreflectometrylib-0.0.6/tests/sample/elements/materials/test_material_density.py`

 * *Files identical despite different names*

### Comparing `easyreflectometrylib-0.0.5/tests/sample/elements/materials/test_material_mixture.py` & `easyreflectometrylib-0.0.6/tests/sample/elements/materials/test_material_mixture.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,134 +4,123 @@
 from numpy.testing import assert_almost_equal
 
 from EasyReflectometry.sample.elements.materials.material import Material
 from EasyReflectometry.sample.elements.materials.material_mixture import MaterialMixture
 
 
 class TestMaterialMixture(unittest.TestCase):
-
     def test_default(self):
         p = MaterialMixture.default()
-        assert p._fraction.raw_value == 0.5
+        assert p.fraction == 0.5
         assert str(p._fraction.unit) == 'dimensionless'
-        assert p.sld.raw_value == Material.default().sld.raw_value
-        assert p.isld.raw_value == Material.default().isld.raw_value
-        assert str(p.sld.unit) == '1 / angstrom ** 2'
-        assert str(p.isld.unit) == '1 / angstrom ** 2'
+        assert p.sld == Material.default().sld.raw_value
+        assert p.isld == Material.default().isld.raw_value
+        assert str(p._sld.unit) == '1 / angstrom ** 2'
+        assert str(p._isld.unit) == '1 / angstrom ** 2'
 
     def test_default_constraint(self):
         p = MaterialMixture.default()
-        assert p._fraction.raw_value == 0.5
+        assert p.fraction == 0.5
         assert str(p._fraction.unit) == 'dimensionless'
-        assert p.sld.raw_value == Material.default().sld.raw_value
-        assert p.isld.raw_value == Material.default().isld.raw_value
+        assert p.sld == Material.default().sld.raw_value
+        assert p.isld == Material.default().isld.raw_value
         p.material_a.sld.value = 0
         p.material_b.isld.value = -1
-        assert_almost_equal(p.sld.raw_value, 2.093)
-        assert_almost_equal(p.isld.raw_value, -0.5)
-        assert str(p.sld.unit) == '1 / angstrom ** 2'
-        assert str(p.isld.unit) == '1 / angstrom ** 2'
-    
+        assert_almost_equal(p.sld, 2.093)
+        assert_almost_equal(p.isld, -0.5)
+        assert str(p._sld.unit) == '1 / angstrom ** 2'
+        assert str(p._isld.unit) == '1 / angstrom ** 2'
+
     def test_fraction_constraint(self):
         p = Material.default()
         q = Material.from_pars(6.908, -0.278, 'Boron')
         r = MaterialMixture.from_pars(p, q, 0.2)
-        assert r._fraction.raw_value == 0.2
-        assert_almost_equal(r.sld.raw_value, 4.7304)
-        assert_almost_equal(r.isld.raw_value, -0.0556)
+        assert r.fraction == 0.2
+        assert_almost_equal(r.sld, 4.7304)
+        assert_almost_equal(r.isld, -0.0556)
         r._fraction.value = 0.5
-        assert r._fraction.raw_value == 0.5
-        assert_almost_equal(r.sld.raw_value, 5.54700)
-        assert_almost_equal(r.isld.raw_value, -0.1390)
+        assert r.fraction == 0.5
+        assert_almost_equal(r.sld, 5.54700)
+        assert_almost_equal(r.isld, -0.1390)
 
     def test_material_a_change(self):
         p = MaterialMixture.default()
-        assert p._fraction.raw_value == 0.5
+        assert p.fraction == 0.5
         assert str(p._fraction.unit) == 'dimensionless'
-        assert p.sld.raw_value == Material.default().sld.raw_value
-        assert p.isld.raw_value == Material.default().isld.raw_value
+        assert p.sld == Material.default().sld.raw_value
+        assert p.isld == Material.default().isld.raw_value
         q = Material.from_pars(6.908, -0.278, 'Boron')
         p.material_a = q
-        assert p._fraction.raw_value == 0.5
+        assert p.fraction == 0.5
         assert str(p._fraction.unit) == 'dimensionless'
-        assert_almost_equal(p.sld.raw_value, 5.54700)
-        assert_almost_equal(p.isld.raw_value, -0.1390)
+        assert_almost_equal(p.sld, 5.54700)
+        assert_almost_equal(p.isld, -0.1390)
 
     def test_material_b_change(self):
         p = MaterialMixture.default()
-        assert p._fraction.raw_value == 0.5
+        assert p.fraction == 0.5
         assert str(p._fraction.unit) == 'dimensionless'
-        assert p.sld.raw_value == Material.default().sld.raw_value
-        assert p.isld.raw_value == Material.default().isld.raw_value
+        assert p.sld == Material.default().sld.raw_value
+        assert p.isld == Material.default().isld.raw_value
         q = Material.from_pars(6.908, -0.278, 'Boron')
         p.material_b = q
-        assert p._fraction.raw_value == 0.5
+        assert p.fraction == 0.5
         assert str(p._fraction.unit) == 'dimensionless'
-        assert_almost_equal(p.sld.raw_value, 5.54700)
-        assert_almost_equal(p.isld.raw_value, -0.1390)
+        assert_almost_equal(p.sld, 5.54700)
+        assert_almost_equal(p.isld, -0.1390)
 
     def test_material_b_change_double(self):
         p = MaterialMixture.default()
-        assert p._fraction.raw_value == 0.5
+        assert p.fraction == 0.5
         assert str(p._fraction.unit) == 'dimensionless'
-        assert p.sld.raw_value == Material.default().sld.raw_value
-        assert p.isld.raw_value == Material.default().isld.raw_value
+        assert p.sld == Material.default().sld.raw_value
+        assert p.isld == Material.default().isld.raw_value
         q = Material.from_pars(6.908, -0.278, 'Boron')
         p.material_b = q
         assert p.name == 'EasyMaterial/Boron'
-        assert p._fraction.raw_value == 0.5
+        assert p.fraction == 0.5
         assert str(p._fraction.unit) == 'dimensionless'
-        assert_almost_equal(p.sld.raw_value, 5.54700)
-        assert_almost_equal(p.isld.raw_value, -0.1390)
+        assert_almost_equal(p.sld, 5.54700)
+        assert_almost_equal(p.isld, -0.1390)
         r = Material.from_pars(0.00, 0.00, 'ACMW')
         p.material_b = r
         assert p.name == 'EasyMaterial/ACMW'
-        assert p._fraction.raw_value == 0.5
+        assert p.fraction == 0.5
         assert str(p._fraction.unit) == 'dimensionless'
-        assert_almost_equal(p.sld.raw_value, 2.0930)
-        assert_almost_equal(p.isld.raw_value, 0.0000)
+        assert_almost_equal(p.sld, 2.0930)
+        assert_almost_equal(p.isld, 0.0000)
 
     def test_from_pars(self):
         p = Material.default()
         q = Material.from_pars(6.908, -0.278, 'Boron')
         r = MaterialMixture.from_pars(p, q, 0.2)
-        assert r._fraction.raw_value == 0.2
+        assert r.fraction == 0.2
         assert str(r._fraction.unit) == 'dimensionless'
-        assert_almost_equal(r.sld.raw_value, 4.7304)
-        assert_almost_equal(r.isld.raw_value, -0.0556)
-        assert str(r.sld.unit) == '1 / angstrom ** 2'
-        assert str(r.isld.unit) == '1 / angstrom ** 2'
+        assert_almost_equal(r.sld, 4.7304)
+        assert_almost_equal(r.isld, -0.0556)
+        assert str(r._sld.unit) == '1 / angstrom ** 2'
+        assert str(r._isld.unit) == '1 / angstrom ** 2'
 
     def test_dict_repr(self):
         p = MaterialMixture.default()
         assert p._dict_repr == {
             'EasyMaterial/EasyMaterial': {
-                'fraction': 0.5,
+                'fraction': '0.500 dimensionless',
                 'sld': '4.186e-6 1 / angstrom ** 2',
                 'isld': '0.000e-6 1 / angstrom ** 2',
-                'material_a': {
-                    'EasyMaterial': {
-                        'sld': '4.186e-6 1 / angstrom ** 2',
-                        'isld': '0.000e-6 1 / angstrom ** 2'
-                    }
-                },
-                'material_b': {
-                    'EasyMaterial': {
-                        'sld': '4.186e-6 1 / angstrom ** 2',
-                        'isld': '0.000e-6 1 / angstrom ** 2'
-                    }
-                }
+                'material_a': {'EasyMaterial': {'sld': '4.186e-6 1 / angstrom ** 2', 'isld': '0.000e-6 1 / angstrom ** 2'}},
+                'material_b': {'EasyMaterial': {'sld': '4.186e-6 1 / angstrom ** 2', 'isld': '0.000e-6 1 / angstrom ** 2'}},
             }
         }
 
     def test_dict_round_trip(self):
         p = MaterialMixture.default()
         q = MaterialMixture.from_dict(p.as_dict())
         assert p.as_data_dict() == q.as_data_dict()
-    
+
     def test_update_name(self):
         # When
         p = MaterialMixture.default()
         mock_material_a = MagicMock()
         mock_material_a.name = 'name_a'
         p._material_a = mock_material_a
         mock_material_b = MagicMock()
```

### Comparing `easyreflectometrylib-0.0.5/tests/special/test_calculations.py` & `easyreflectometrylib-0.0.6/tests/special/test_calculations.py`

 * *Files identical despite different names*

### Comparing `easyreflectometrylib-0.0.5/LICENSE` & `easyreflectometrylib-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `easyreflectometrylib-0.0.5/README.rst` & `easyreflectometrylib-0.0.6/README.rst`

 * *Files identical despite different names*

### Comparing `easyreflectometrylib-0.0.5/pyproject.toml` & `easyreflectometrylib-0.0.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling<=1.21.0"]  
 build-backend = "hatchling.build"
 
 [project]
 name = "EasyReflectometryLib"
-version = "0.0.5"
+version = "0.0.6"
 description = "A reflectometry python package built on the EasyScience framework."
 readme = "README.rst"
 authors = [
     {name = "Andrew R. McCluskey", email = "andrew.mccluskey@ess.eu"}, 
     {name = "Andrew Sazonov"}, 
     {name = "Simon Ward"},
     {name = "Andreas Pedersen", email = "andreas.pedersen@ess.eu"}
```

### Comparing `easyreflectometrylib-0.0.5/PKG-INFO` & `easyreflectometrylib-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EasyReflectometryLib
-Version: 0.0.5
+Version: 0.0.6
 Summary: A reflectometry python package built on the EasyScience framework.
 Project-URL: homepage, https://docs.easyreflectometry.org
 Project-URL: documentation, https://docs.easyreflectometry.org
 Author: Andrew Sazonov, Simon Ward
 Author-email: "Andrew R. McCluskey" <andrew.mccluskey@ess.eu>, Andreas Pedersen <andreas.pedersen@ess.eu>
 Maintainer-email: "Andrew R. McCluskey" <andrew.mccluskey@ess.eu>, Andreas Pedersen <andreas.pedersen@ess.eu>
 License-Expression: BSD-3-Clause
```


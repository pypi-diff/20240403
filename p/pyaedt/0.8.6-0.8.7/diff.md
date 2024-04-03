# Comparing `tmp/pyaedt-0.8.6.tar.gz` & `tmp/pyaedt-0.8.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyaedt-0.8.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pyaedt-0.8.7.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pyaedt-0.8.6.tar` & `pyaedt-0.8.7.tar`

### file list

```diff
@@ -1,172 +1,172 @@
--rw-r--r--   0        0        0     1111 2024-01-15 14:46:43.299586 pyaedt-0.8.6/LICENSE
--rw-r--r--   0        0        0    10530 2024-03-18 17:45:23.661309 pyaedt-0.8.6/README.md
--rw-r--r--   0        0        0     3483 2024-03-29 10:51:29.642256 pyaedt-0.8.6/pyaedt/__init__.py
--rw-r--r--   0        0        0    33008 2024-03-26 16:57:20.130563 pyaedt-0.8.6/pyaedt/aedt_logger.py
--rw-r--r--   0        0        0     6966 2024-01-15 14:46:46.784077 pyaedt-0.8.6/pyaedt/application/AEDT_File_Management.py
--rw-r--r--   0        0        0    94519 2024-03-28 13:42:32.175958 pyaedt-0.8.6/pyaedt/application/Analysis.py
--rw-r--r--   0        0        0    56666 2024-03-25 07:54:07.614787 pyaedt-0.8.6/pyaedt/application/Analysis3D.py
--rw-r--r--   0        0        0    18326 2024-03-28 21:24:14.340969 pyaedt-0.8.6/pyaedt/application/Analysis3DLayout.py
--rw-r--r--   0        0        0     3225 2024-02-29 11:54:55.496422 pyaedt-0.8.6/pyaedt/application/AnalysisMaxwellCircuit.py
--rw-r--r--   0        0        0    20926 2024-03-28 21:24:14.340969 pyaedt-0.8.6/pyaedt/application/AnalysisNexxim.py
--rw-r--r--   0        0        0     4655 2024-03-26 16:57:20.130563 pyaedt-0.8.6/pyaedt/application/AnalysisRMxprt.py
--rw-r--r--   0        0        0     4856 2024-03-19 10:22:25.002309 pyaedt-0.8.6/pyaedt/application/AnalysisTwinBuilder.py
--rw-r--r--   0        0        0   141844 2024-03-28 13:42:32.175958 pyaedt-0.8.6/pyaedt/application/Design.py
--rw-r--r--   0        0        0     6194 2024-01-15 14:46:46.784077 pyaedt-0.8.6/pyaedt/application/JobManager.py
--rw-r--r--   0        0        0    80771 2024-03-29 10:05:09.590029 pyaedt-0.8.6/pyaedt/application/Variables.py
--rw-r--r--   0        0        0        0 2024-01-15 14:46:46.784077 pyaedt-0.8.6/pyaedt/application/__init__.py
--rw-r--r--   0        0        0    13127 2024-03-26 16:57:20.146189 pyaedt-0.8.6/pyaedt/application/aedt_objects.py
--rw-r--r--   0        0        0    38436 2024-03-26 16:57:20.146189 pyaedt-0.8.6/pyaedt/application/design_solutions.py
--rw-r--r--   0        0        0    64136 2024-03-28 10:29:41.033629 pyaedt-0.8.6/pyaedt/circuit.py
--rw-r--r--   0        0        0    10629 2024-03-28 13:42:32.175958 pyaedt-0.8.6/pyaedt/common_rpc.py
--rw-r--r--   0        0        0    93288 2024-03-29 10:05:09.590029 pyaedt-0.8.6/pyaedt/desktop.py
--rw-r--r--   0        0        0    25696 2024-03-26 16:57:20.146189 pyaedt-0.8.6/pyaedt/downloads.py
--rw-r--r--   0        0        0      210 2024-02-23 11:42:00.605018 pyaedt-0.8.6/pyaedt/edb.py
--rw-r--r--   0        0        0    11572 2024-02-02 15:24:22.962207 pyaedt-0.8.6/pyaedt/emit.py
--rw-r--r--   0        0        0     6102 2024-01-31 09:29:01.341575 pyaedt-0.8.6/pyaedt/emit_core/Couplings.py
--rw-r--r--   0        0        0     3762 2024-01-15 14:46:46.846578 pyaedt-0.8.6/pyaedt/emit_core/__init__.py
--rw-r--r--   0        0        0     2664 2024-01-15 14:46:46.846578 pyaedt-0.8.6/pyaedt/emit_core/emit_constants.py
--rw-r--r--   0        0        0        2 2024-01-15 14:46:46.846578 pyaedt-0.8.6/pyaedt/emit_core/results/__init__.py
--rw-r--r--   0        0        0     7406 2024-01-15 14:46:46.846578 pyaedt-0.8.6/pyaedt/emit_core/results/results.py
--rw-r--r--   0        0        0    30545 2024-01-15 14:46:46.846578 pyaedt-0.8.6/pyaedt/emit_core/results/revision.py
--rw-r--r--   0        0        0     9836 2024-01-15 14:46:46.846578 pyaedt-0.8.6/pyaedt/generic/Ansys.png
--rw-r--r--   0        0        0      761 2024-02-02 18:09:12.170567 pyaedt-0.8.6/pyaedt/generic/AnsysTemplate.json
--rw-r--r--   0        0        0    15945 2024-03-26 16:57:20.146189 pyaedt-0.8.6/pyaedt/generic/DataHandlers.py
--rw-r--r--   0        0        0    16547 2024-03-22 09:31:18.787406 pyaedt-0.8.6/pyaedt/generic/LoadAEDTFile.py
--rw-r--r--   0        0        0        0 2024-01-15 14:46:46.862204 pyaedt-0.8.6/pyaedt/generic/__init__.py
--rw-r--r--   0        0        0     1413 2024-01-15 14:46:46.862204 pyaedt-0.8.6/pyaedt/generic/ami.json
--rw-r--r--   0        0        0     3347 2024-03-26 16:57:20.146189 pyaedt-0.8.6/pyaedt/generic/clr_module.py
--rw-r--r--   0        0        0    37660 2024-03-29 10:05:09.590029 pyaedt-0.8.6/pyaedt/generic/compliance.py
--rw-r--r--   0        0        0    90632 2024-03-29 10:05:09.590029 pyaedt-0.8.6/pyaedt/generic/configurations.py
--rw-r--r--   0        0        0    28707 2024-03-19 10:51:59.720444 pyaedt-0.8.6/pyaedt/generic/constants.py
--rw-r--r--   0        0        0    73959 2024-03-22 09:23:21.834111 pyaedt-0.8.6/pyaedt/generic/design_types.py
--rw-r--r--   0        0        0      168 2024-01-15 14:46:46.862204 pyaedt-0.8.6/pyaedt/generic/desktop_sessions.py
--rw-r--r--   0        0        0     3934 2024-03-26 16:57:20.146189 pyaedt-0.8.6/pyaedt/generic/filesystem.py
--rw-r--r--   0        0        0    66060 2024-03-28 13:42:32.191576 pyaedt-0.8.6/pyaedt/generic/general_methods.py
--rw-r--r--   0        0        0     9430 2024-03-26 16:57:20.146189 pyaedt-0.8.6/pyaedt/generic/grpc_plugin.py
--rw-r--r--   0        0        0     3473 2024-01-15 14:46:46.862204 pyaedt-0.8.6/pyaedt/generic/grpc_plugin_dll.py
--rw-r--r--   0        0        0    45059 2024-03-28 13:42:32.191576 pyaedt-0.8.6/pyaedt/generic/ibis_reader.py
--rw-r--r--   0        0        0     2776 2024-01-15 14:46:46.862204 pyaedt-0.8.6/pyaedt/generic/ibis_v7.json
--rw-r--r--   0        0        0     7029 2024-01-15 14:46:46.862204 pyaedt-0.8.6/pyaedt/generic/near_field_import.py
--rw-r--r--   0        0        0    21859 2024-03-28 13:42:32.191576 pyaedt-0.8.6/pyaedt/generic/pdf.py
--rw-r--r--   0        0        0    65225 2024-03-26 16:57:20.146189 pyaedt-0.8.6/pyaedt/generic/plot.py
--rw-r--r--   0        0        0    20256 2024-01-15 14:46:46.862204 pyaedt-0.8.6/pyaedt/generic/python_optimizers.py
--rw-r--r--   0        0        0     3536 2024-01-15 14:46:46.862204 pyaedt-0.8.6/pyaedt/generic/report_file_parser.py
--rw-r--r--   0        0        0    17381 2024-03-22 09:31:18.803030 pyaedt-0.8.6/pyaedt/generic/settings.py
--rw-r--r--   0        0        0    25174 2024-03-28 13:42:32.191576 pyaedt-0.8.6/pyaedt/generic/spisim.py
--rw-r--r--   0        0        0    20374 2024-03-29 10:05:09.590029 pyaedt-0.8.6/pyaedt/generic/touchstone_parser.py
--rw-r--r--   0        0        0   266167 2024-03-28 10:29:41.033629 pyaedt-0.8.6/pyaedt/hfss.py
--rw-r--r--   0        0        0    85858 2024-03-28 10:29:41.049261 pyaedt-0.8.6/pyaedt/hfss3dlayout.py
--rw-r--r--   0        0        0   278583 2024-03-28 10:29:41.049261 pyaedt-0.8.6/pyaedt/icepak.py
--rw-r--r--   0        0        0   127370 2024-03-28 13:42:32.191576 pyaedt-0.8.6/pyaedt/maxwell.py
--rw-r--r--   0        0        0     7953 2024-03-26 16:57:20.161819 pyaedt-0.8.6/pyaedt/maxwellcircuit.py
--rw-r--r--   0        0        0    24538 2024-03-28 10:29:41.049261 pyaedt-0.8.6/pyaedt/mechanical.py
--rw-r--r--   0        0        0     3642 2024-01-15 14:46:46.877830 pyaedt-0.8.6/pyaedt/misc/Console.py_build
--rw-r--r--   0        0        0     2230 2024-01-15 14:46:46.877830 pyaedt-0.8.6/pyaedt/misc/Job_Settings.areg
--rw-r--r--   0        0        0     3394 2024-01-15 14:46:46.877830 pyaedt-0.8.6/pyaedt/misc/Jupyter.py_build
--rw-r--r--   0        0        0     4125 2024-01-15 14:46:46.877830 pyaedt-0.8.6/pyaedt/misc/Run_PyAEDT_Script.py_build
--rw-r--r--   0        0        0     3526 2024-01-15 14:46:46.877830 pyaedt-0.8.6/pyaedt/misc/Run_PyAEDT_Toolkit_Script.py_build
--rw-r--r--   0        0        0      202 2024-01-15 14:46:46.877830 pyaedt-0.8.6/pyaedt/misc/__init__.py
--rw-r--r--   0        0        0    10796 2024-03-26 16:57:20.161819 pyaedt-0.8.6/pyaedt/misc/aedtlib_personalib_install.py
--rw-r--r--   0        0        0    19870 2024-01-15 14:46:46.877830 pyaedt-0.8.6/pyaedt/misc/amat.xml
--rw-r--r--   0        0        0     2620 2024-01-15 14:46:46.877830 pyaedt-0.8.6/pyaedt/misc/ansys_cloud.areg
--rw-r--r--   0        0        0     2013 2024-01-15 14:46:46.877830 pyaedt-0.8.6/pyaedt/misc/config.schema.json
--rw-r--r--   0        0        0     3554 2024-01-31 09:29:01.341575 pyaedt-0.8.6/pyaedt/misc/console_setup.py
--rw-r--r--   0        0        0       48 2024-01-15 14:46:46.893455 pyaedt-0.8.6/pyaedt/misc/create_remote_dir.py
--rw-r--r--   0        0        0    15250 2024-01-15 14:46:46.893455 pyaedt-0.8.6/pyaedt/misc/images/gallery/PyAEDT.png
--rw-r--r--   0        0        0      855 2024-01-15 14:46:46.893455 pyaedt-0.8.6/pyaedt/misc/images/large/pyansys.png
--rw-r--r--   0        0        0     5630 2024-03-08 09:00:54.059074 pyaedt-0.8.6/pyaedt/misc/install_extra_toolkits.py
--rw-r--r--   0        0        0     1728 2024-01-15 14:46:46.893455 pyaedt-0.8.6/pyaedt/misc/jupyter_template.ipynb
--rw-r--r--   0        0        0     2700 2024-03-26 16:57:20.161819 pyaedt-0.8.6/pyaedt/misc/misc.py
--rw-r--r--   0        0        0   771467 2024-01-15 14:46:46.893455 pyaedt-0.8.6/pyaedt/misc/ml_data_file_train_100MHz_1GHz.json
--rw-r--r--   0        0        0   502580 2024-01-15 14:46:46.893455 pyaedt-0.8.6/pyaedt/misc/ml_data_file_train_1GHz_10GHz.json
--rw-r--r--   0        0        0   162026 2024-01-15 14:46:46.909082 pyaedt-0.8.6/pyaedt/misc/patch_svr_model_100MHz_1GHz.joblib
--rw-r--r--   0        0        0   134414 2024-01-15 14:46:46.909082 pyaedt-0.8.6/pyaedt/misc/patch_svr_model_1GHz_10GHz.joblib
--rw-r--r--   0        0        0      289 2024-01-15 14:46:46.909082 pyaedt-0.8.6/pyaedt/misc/pyaedt.runtimeconfig.json
--rw-r--r--   0        0        0      960 2024-01-15 14:46:46.909082 pyaedt-0.8.6/pyaedt/misc/pyaedt_local_config.acf
--rw-r--r--   0        0        0    16550 2024-01-15 14:46:46.909082 pyaedt-0.8.6/pyaedt/misc/pyansys-logo-black-cropped.png
--rw-r--r--   0        0        0       61 2024-03-20 11:24:34.893979 pyaedt-0.8.6/pyaedt/misc/spisim_com_configuration_files/__init__.py
--rw-r--r--   0        0        0     5192 2024-03-20 11:24:34.893979 pyaedt-0.8.6/pyaedt/misc/spisim_com_configuration_files/com_120d_8.json
--rw-r--r--   0        0        0     5153 2024-03-20 11:24:34.893979 pyaedt-0.8.6/pyaedt/misc/spisim_com_configuration_files/com_93_8.json
--rw-r--r--   0        0        0     5155 2024-03-20 11:24:34.893979 pyaedt-0.8.6/pyaedt/misc/spisim_com_configuration_files/com_94_17.json
--rw-r--r--   0        0        0    12280 2024-03-21 13:54:18.817623 pyaedt-0.8.6/pyaedt/misc/spisim_com_configuration_files/com_parameters.py
--rw-r--r--   0        0        0    15308 2024-03-20 11:24:34.893979 pyaedt-0.8.6/pyaedt/misc/spisim_com_configuration_files/com_settings_mapping.py
--rw-r--r--   0        0        0      868 2024-01-15 14:46:46.909082 pyaedt-0.8.6/pyaedt/misc/template.acf
--rw-r--r--   0        0        0        0 2024-01-15 14:46:46.909082 pyaedt-0.8.6/pyaedt/modeler/__init__.py
--rw-r--r--   0        0        0        0 2024-01-15 14:46:46.909082 pyaedt-0.8.6/pyaedt/modeler/advanced_cad/__init__.py
--rw-r--r--   0        0        0    14073 2024-02-09 10:30:11.555002 pyaedt-0.8.6/pyaedt/modeler/advanced_cad/actors.py
--rw-r--r--   0        0        0    20019 2024-02-09 10:30:11.570630 pyaedt-0.8.6/pyaedt/modeler/advanced_cad/multiparts.py
--rw-r--r--   0        0        0    18513 2024-01-15 14:46:46.909082 pyaedt-0.8.6/pyaedt/modeler/advanced_cad/oms.py
--rw-r--r--   0        0        0    16809 2024-01-15 14:46:46.909082 pyaedt-0.8.6/pyaedt/modeler/advanced_cad/parts.py
--rw-r--r--   0        0        0   126188 2024-01-15 14:46:46.909082 pyaedt-0.8.6/pyaedt/modeler/advanced_cad/stackup_3d.py
--rw-r--r--   0        0        0    80015 2024-03-26 16:57:20.161819 pyaedt-0.8.6/pyaedt/modeler/cad/Modeler.py
--rw-r--r--   0        0        0   335869 2024-03-29 10:05:09.590029 pyaedt-0.8.6/pyaedt/modeler/cad/Primitives.py
--rw-r--r--   0        0        0    13476 2024-03-27 08:05:29.244957 pyaedt-0.8.6/pyaedt/modeler/cad/Primitives2D.py
--rw-r--r--   0        0        0   143005 2024-03-29 10:05:09.590029 pyaedt-0.8.6/pyaedt/modeler/cad/Primitives3D.py
--rw-r--r--   0        0        0        0 2024-01-15 14:46:46.924709 pyaedt-0.8.6/pyaedt/modeler/cad/__init__.py
--rw-r--r--   0        0        0    29696 2024-03-20 14:17:37.957610 pyaedt-0.8.6/pyaedt/modeler/cad/component_array.py
--rw-r--r--   0        0        0    40015 2024-03-26 16:57:20.177502 pyaedt-0.8.6/pyaedt/modeler/cad/components_3d.py
--rw-r--r--   0        0        0    49410 2024-03-26 16:57:20.177502 pyaedt-0.8.6/pyaedt/modeler/cad/elements3d.py
--rw-r--r--   0        0        0    59382 2024-03-29 09:46:43.596170 pyaedt-0.8.6/pyaedt/modeler/cad/object3d.py
--rw-r--r--   0        0        0    53212 2024-03-26 16:57:20.177502 pyaedt-0.8.6/pyaedt/modeler/cad/polylines.py
--rw-r--r--   0        0        0    12604 2024-01-15 14:46:46.924709 pyaedt-0.8.6/pyaedt/modeler/calculators.py
--rw-r--r--   0        0        0    44084 2024-03-29 10:05:09.605657 pyaedt-0.8.6/pyaedt/modeler/circuits/PrimitivesCircuit.py
--rw-r--r--   0        0        0    39272 2024-01-15 14:46:46.924709 pyaedt-0.8.6/pyaedt/modeler/circuits/PrimitivesEmit.py
--rw-r--r--   0        0        0     8396 2024-01-15 14:46:46.924709 pyaedt-0.8.6/pyaedt/modeler/circuits/PrimitivesMaxwellCircuit.py
--rw-r--r--   0        0        0    67681 2024-03-07 09:29:30.863283 pyaedt-0.8.6/pyaedt/modeler/circuits/PrimitivesNexxim.py
--rw-r--r--   0        0        0    15130 2024-01-15 14:46:46.924709 pyaedt-0.8.6/pyaedt/modeler/circuits/PrimitivesTwinBuilder.py
--rw-r--r--   0        0        0        0 2024-01-15 14:46:46.924709 pyaedt-0.8.6/pyaedt/modeler/circuits/__init__.py
--rw-r--r--   0        0        0    34191 2024-03-26 16:57:20.177502 pyaedt-0.8.6/pyaedt/modeler/circuits/object3dcircuit.py
--rw-r--r--   0        0        0    68182 2024-03-28 10:29:41.049261 pyaedt-0.8.6/pyaedt/modeler/geometry_operators.py
--rw-r--r--   0        0        0     6929 2024-01-15 14:46:46.924709 pyaedt-0.8.6/pyaedt/modeler/modeler2d.py
--rw-r--r--   0        0        0    66173 2024-03-28 13:42:32.191576 pyaedt-0.8.6/pyaedt/modeler/modeler3d.py
--rw-r--r--   0        0        0    33255 2024-03-26 16:57:20.177502 pyaedt-0.8.6/pyaedt/modeler/modelerpcb.py
--rw-r--r--   0        0        0    50776 2024-03-26 16:57:20.177502 pyaedt-0.8.6/pyaedt/modeler/pcb/Primitives3DLayout.py
--rw-r--r--   0        0        0        0 2024-01-15 14:46:46.940332 pyaedt-0.8.6/pyaedt/modeler/pcb/__init__.py
--rw-r--r--   0        0        0    65931 2024-03-28 10:29:41.049261 pyaedt-0.8.6/pyaedt/modeler/pcb/object3dlayout.py
--rw-r--r--   0        0        0    23852 2024-03-26 16:57:20.193074 pyaedt-0.8.6/pyaedt/modeler/schematic.py
--rw-r--r--   0        0        0    54859 2024-03-28 13:42:32.207202 pyaedt-0.8.6/pyaedt/modules/AdvancedPostProcessing.py
--rw-r--r--   0        0        0   169955 2024-03-26 16:57:20.193074 pyaedt-0.8.6/pyaedt/modules/Boundary.py
--rw-r--r--   0        0        0    71690 2024-03-28 13:42:32.207202 pyaedt-0.8.6/pyaedt/modules/CableModeling.py
--rw-r--r--   0        0        0    16319 2024-01-15 14:46:46.940332 pyaedt-0.8.6/pyaedt/modules/CircuitTemplates.py
--rw-r--r--   0        0        0    56766 2024-03-29 10:05:09.605657 pyaedt-0.8.6/pyaedt/modules/DesignXPloration.py
--rw-r--r--   0        0        0    40449 2024-03-26 16:57:20.208700 pyaedt-0.8.6/pyaedt/modules/LayerStackup.py
--rw-r--r--   0        0        0   104701 2024-03-29 10:05:09.605657 pyaedt-0.8.6/pyaedt/modules/Material.py
--rw-r--r--   0        0        0    33683 2024-03-26 16:57:20.208700 pyaedt-0.8.6/pyaedt/modules/MaterialLib.py
--rw-r--r--   0        0        0    53774 2024-03-26 16:57:20.208700 pyaedt-0.8.6/pyaedt/modules/Mesh.py
--rw-r--r--   0        0        0    12018 2024-03-26 16:57:20.208700 pyaedt-0.8.6/pyaedt/modules/Mesh3DLayout.py
--rw-r--r--   0        0        0    48847 2024-03-26 16:57:20.208700 pyaedt-0.8.6/pyaedt/modules/MeshIcepak.py
--rw-r--r--   0        0        0     4437 2024-01-15 14:46:46.940332 pyaedt-0.8.6/pyaedt/modules/OptimetricsTemplates.py
--rw-r--r--   0        0        0   206587 2024-03-28 13:42:32.207202 pyaedt-0.8.6/pyaedt/modules/PostProcessor.py
--rw-r--r--   0        0        0    72048 2024-03-08 13:11:00.118100 pyaedt-0.8.6/pyaedt/modules/SetupTemplates.py
--rw-r--r--   0        0        0   147780 2024-03-28 10:29:41.064891 pyaedt-0.8.6/pyaedt/modules/SolveSetup.py
--rw-r--r--   0        0        0    34324 2024-03-26 16:57:20.224324 pyaedt-0.8.6/pyaedt/modules/SolveSweeps.py
--rw-r--r--   0        0        0        0 2024-01-15 14:46:46.955959 pyaedt-0.8.6/pyaedt/modules/__init__.py
--rw-r--r--   0        0        0    31434 2024-03-26 16:57:20.224324 pyaedt-0.8.6/pyaedt/modules/monitor_icepak.py
--rw-r--r--   0        0        0   132190 2024-03-26 16:57:20.224324 pyaedt-0.8.6/pyaedt/modules/report_templates.py
--rw-r--r--   0        0        0   134882 2024-03-28 13:42:32.207202 pyaedt-0.8.6/pyaedt/modules/solutions.py
--rw-r--r--   0        0        0    97835 2024-03-26 16:57:20.224324 pyaedt-0.8.6/pyaedt/q3d.py
--rw-r--r--   0        0        0    10664 2024-02-02 15:24:22.977836 pyaedt-0.8.6/pyaedt/rmxprt.py
--rw-r--r--   0        0        0        0 2024-01-15 14:46:46.955959 pyaedt-0.8.6/pyaedt/rpc/__init__.py
--rw-r--r--   0        0        0      415 2024-01-15 14:46:46.955959 pyaedt-0.8.6/pyaedt/rpc/local_server.py
--rw-r--r--   0        0        0    42133 2024-03-28 13:42:32.207202 pyaedt-0.8.6/pyaedt/rpc/rpyc_services.py
--rw-r--r--   0        0        0        0 2024-01-15 14:46:46.955959 pyaedt-0.8.6/pyaedt/sbrplus/__init__.py
--rw-r--r--   0        0        0     9463 2024-01-15 14:46:46.955959 pyaedt-0.8.6/pyaedt/sbrplus/hdm_parser.py
--rw-r--r--   0        0        0     2096 2024-01-15 14:46:46.955959 pyaedt-0.8.6/pyaedt/sbrplus/hdm_utils.py
--rw-r--r--   0        0        0     2607 2024-01-15 14:46:46.955959 pyaedt-0.8.6/pyaedt/sbrplus/matlab/HdmObject.m
--rw-r--r--   0        0        0       97 2024-01-15 14:46:46.955959 pyaedt-0.8.6/pyaedt/sbrplus/matlab/README.md
--rw-r--r--   0        0        0      735 2024-01-15 14:46:46.955959 pyaedt-0.8.6/pyaedt/sbrplus/matlab/SbrBounceType.m
--rw-r--r--   0        0        0     2886 2024-01-15 14:46:46.971583 pyaedt-0.8.6/pyaedt/sbrplus/matlab/StopWatch.m
--rw-r--r--   0        0        0     1402 2024-01-15 14:46:46.971583 pyaedt-0.8.6/pyaedt/sbrplus/matlab/add_3dlight.m
--rw-r--r--   0        0        0      340 2024-01-15 14:46:46.971583 pyaedt-0.8.6/pyaedt/sbrplus/matlab/amp2db.m
--rw-r--r--   0        0        0    36837 2024-01-15 14:46:46.971583 pyaedt-0.8.6/pyaedt/sbrplus/matlab/draw_rays1.m
--rw-r--r--   0        0        0     4322 2024-01-15 14:46:46.971583 pyaedt-0.8.6/pyaedt/sbrplus/matlab/draw_wfobj.m
--rw-r--r--   0        0        0    31414 2024-01-15 14:46:46.971583 pyaedt-0.8.6/pyaedt/sbrplus/matlab/filter_rays1.m
--rw-r--r--   0        0        0     1504 2024-01-15 14:46:46.971583 pyaedt-0.8.6/pyaedt/sbrplus/matlab/filtered_tracks.m
--rw-r--r--   0        0        0    20853 2024-01-15 14:46:46.971583 pyaedt-0.8.6/pyaedt/sbrplus/matlab/ld_sbrplushdm.m
--rw-r--r--   0        0        0    14781 2024-01-15 14:46:46.971583 pyaedt-0.8.6/pyaedt/sbrplus/matlab/ld_wfobj.m
--rw-r--r--   0        0        0      318 2024-01-15 14:46:46.971583 pyaedt-0.8.6/pyaedt/sbrplus/matlab/pwr2db.m
--rw-r--r--   0        0        0     2607 2024-01-15 14:46:46.971583 pyaedt-0.8.6/pyaedt/sbrplus/matlab/validate_sfields.m
--rw-r--r--   0        0        0     7621 2024-03-26 16:57:20.224324 pyaedt-0.8.6/pyaedt/sbrplus/plot.py
--rw-r--r--   0        0        0    21628 2024-03-28 13:42:32.207202 pyaedt-0.8.6/pyaedt/twinbuilder.py
--rw-r--r--   0        0        0     6767 2024-03-29 10:51:29.642256 pyaedt-0.8.6/pyproject.toml
--rw-r--r--   0        0        0    16443 1970-01-01 00:00:00.000000 pyaedt-0.8.6/PKG-INFO
+-rw-r--r--   0        0        0     1111 2024-01-08 19:14:30.151334 pyaedt-0.8.7/LICENSE
+-rw-r--r--   0        0        0    10530 2024-03-18 17:51:52.716931 pyaedt-0.8.7/README.md
+-rw-r--r--   0        0        0     3483 2024-04-03 08:15:12.879753 pyaedt-0.8.7/pyaedt/__init__.py
+-rw-r--r--   0        0        0    33008 2024-03-26 18:55:40.973822 pyaedt-0.8.7/pyaedt/aedt_logger.py
+-rw-r--r--   0        0        0     6966 2023-11-15 14:48:55.940401 pyaedt-0.8.7/pyaedt/application/AEDT_File_Management.py
+-rw-r--r--   0        0        0    94519 2024-03-28 08:42:12.578899 pyaedt-0.8.7/pyaedt/application/Analysis.py
+-rw-r--r--   0        0        0    56666 2024-03-28 13:42:38.055724 pyaedt-0.8.7/pyaedt/application/Analysis3D.py
+-rw-r--r--   0        0        0    18347 2024-03-29 15:34:49.291988 pyaedt-0.8.7/pyaedt/application/Analysis3DLayout.py
+-rw-r--r--   0        0        0     3225 2024-02-29 13:41:13.886891 pyaedt-0.8.7/pyaedt/application/AnalysisMaxwellCircuit.py
+-rw-r--r--   0        0        0    20947 2024-03-29 15:34:49.291988 pyaedt-0.8.7/pyaedt/application/AnalysisNexxim.py
+-rw-r--r--   0        0        0     4655 2024-03-26 18:55:40.973822 pyaedt-0.8.7/pyaedt/application/AnalysisRMxprt.py
+-rw-r--r--   0        0        0     4856 2024-03-22 10:54:58.724857 pyaedt-0.8.7/pyaedt/application/AnalysisTwinBuilder.py
+-rw-r--r--   0        0        0   141844 2024-04-01 07:45:19.391915 pyaedt-0.8.7/pyaedt/application/Design.py
+-rw-r--r--   0        0        0     6194 2023-11-15 14:48:55.940401 pyaedt-0.8.7/pyaedt/application/JobManager.py
+-rw-r--r--   0        0        0    80899 2024-03-29 15:34:49.307604 pyaedt-0.8.7/pyaedt/application/Variables.py
+-rw-r--r--   0        0        0        0 2023-11-15 14:48:55.940401 pyaedt-0.8.7/pyaedt/application/__init__.py
+-rw-r--r--   0        0        0    13127 2024-03-26 18:55:40.973822 pyaedt-0.8.7/pyaedt/application/aedt_objects.py
+-rw-r--r--   0        0        0    38436 2024-03-26 18:55:40.973822 pyaedt-0.8.7/pyaedt/application/design_solutions.py
+-rw-r--r--   0        0        0    64136 2024-03-28 13:42:38.055724 pyaedt-0.8.7/pyaedt/circuit.py
+-rw-r--r--   0        0        0    10629 2024-03-28 08:42:12.594588 pyaedt-0.8.7/pyaedt/common_rpc.py
+-rw-r--r--   0        0        0    92849 2024-04-02 14:49:39.042380 pyaedt-0.8.7/pyaedt/desktop.py
+-rw-r--r--   0        0        0    25696 2024-03-26 18:55:40.989446 pyaedt-0.8.7/pyaedt/downloads.py
+-rw-r--r--   0        0        0      210 2024-02-23 10:20:46.907198 pyaedt-0.8.7/pyaedt/edb.py
+-rw-r--r--   0        0        0    11572 2024-02-02 15:15:46.553784 pyaedt-0.8.7/pyaedt/emit.py
+-rw-r--r--   0        0        0     6102 2024-01-31 08:29:55.307606 pyaedt-0.8.7/pyaedt/emit_core/Couplings.py
+-rw-r--r--   0        0        0     3762 2024-02-06 15:33:49.564252 pyaedt-0.8.7/pyaedt/emit_core/__init__.py
+-rw-r--r--   0        0        0     2664 2023-11-15 14:48:56.128198 pyaedt-0.8.7/pyaedt/emit_core/emit_constants.py
+-rw-r--r--   0        0        0        2 2023-11-15 14:48:56.128198 pyaedt-0.8.7/pyaedt/emit_core/results/__init__.py
+-rw-r--r--   0        0        0     7406 2023-11-15 14:48:56.128198 pyaedt-0.8.7/pyaedt/emit_core/results/results.py
+-rw-r--r--   0        0        0    30545 2023-12-04 07:28:21.919850 pyaedt-0.8.7/pyaedt/emit_core/results/revision.py
+-rw-r--r--   0        0        0     9836 2024-01-08 11:44:42.739939 pyaedt-0.8.7/pyaedt/generic/Ansys.png
+-rw-r--r--   0        0        0      761 2024-02-02 17:43:33.722695 pyaedt-0.8.7/pyaedt/generic/AnsysTemplate.json
+-rw-r--r--   0        0        0    15945 2024-03-26 18:55:40.989446 pyaedt-0.8.7/pyaedt/generic/DataHandlers.py
+-rw-r--r--   0        0        0    16547 2024-03-22 10:54:58.724857 pyaedt-0.8.7/pyaedt/generic/LoadAEDTFile.py
+-rw-r--r--   0        0        0        0 2023-11-15 14:48:56.128198 pyaedt-0.8.7/pyaedt/generic/__init__.py
+-rw-r--r--   0        0        0     1413 2023-11-15 14:48:56.128198 pyaedt-0.8.7/pyaedt/generic/ami.json
+-rw-r--r--   0        0        0     3347 2024-03-26 18:55:40.989446 pyaedt-0.8.7/pyaedt/generic/clr_module.py
+-rw-r--r--   0        0        0    37660 2024-03-29 09:59:34.311519 pyaedt-0.8.7/pyaedt/generic/compliance.py
+-rw-r--r--   0        0        0    90998 2024-04-02 14:49:39.042380 pyaedt-0.8.7/pyaedt/generic/configurations.py
+-rw-r--r--   0        0        0    28707 2024-03-19 11:00:02.376642 pyaedt-0.8.7/pyaedt/generic/constants.py
+-rw-r--r--   0        0        0    73959 2024-03-22 10:54:58.724857 pyaedt-0.8.7/pyaedt/generic/design_types.py
+-rw-r--r--   0        0        0      168 2023-11-15 14:48:56.143712 pyaedt-0.8.7/pyaedt/generic/desktop_sessions.py
+-rw-r--r--   0        0        0     3934 2024-03-26 18:55:40.989446 pyaedt-0.8.7/pyaedt/generic/filesystem.py
+-rw-r--r--   0        0        0    66060 2024-03-28 13:42:38.055724 pyaedt-0.8.7/pyaedt/generic/general_methods.py
+-rw-r--r--   0        0        0     9430 2024-03-26 18:55:40.989446 pyaedt-0.8.7/pyaedt/generic/grpc_plugin.py
+-rw-r--r--   0        0        0     3473 2024-02-06 15:33:49.564252 pyaedt-0.8.7/pyaedt/generic/grpc_plugin_dll.py
+-rw-r--r--   0        0        0    45059 2024-03-28 08:42:12.594588 pyaedt-0.8.7/pyaedt/generic/ibis_reader.py
+-rw-r--r--   0        0        0     2776 2024-01-02 08:48:38.514823 pyaedt-0.8.7/pyaedt/generic/ibis_v7.json
+-rw-r--r--   0        0        0     7029 2023-11-15 14:48:56.143712 pyaedt-0.8.7/pyaedt/generic/near_field_import.py
+-rw-r--r--   0        0        0    21859 2024-03-28 13:42:38.055724 pyaedt-0.8.7/pyaedt/generic/pdf.py
+-rw-r--r--   0        0        0    65225 2024-03-28 13:42:38.055724 pyaedt-0.8.7/pyaedt/generic/plot.py
+-rw-r--r--   0        0        0    20256 2023-11-15 14:48:56.143712 pyaedt-0.8.7/pyaedt/generic/python_optimizers.py
+-rw-r--r--   0        0        0     3536 2024-02-06 15:33:49.564252 pyaedt-0.8.7/pyaedt/generic/report_file_parser.py
+-rw-r--r--   0        0        0    17381 2024-03-22 10:54:58.740472 pyaedt-0.8.7/pyaedt/generic/settings.py
+-rw-r--r--   0        0        0    25174 2024-03-28 08:42:12.594588 pyaedt-0.8.7/pyaedt/generic/spisim.py
+-rw-r--r--   0        0        0    20374 2024-03-29 09:59:34.311519 pyaedt-0.8.7/pyaedt/generic/touchstone_parser.py
+-rw-r--r--   0        0        0   271206 2024-04-03 07:09:02.589712 pyaedt-0.8.7/pyaedt/hfss.py
+-rw-r--r--   0        0        0    85858 2024-03-28 13:42:38.071355 pyaedt-0.8.7/pyaedt/hfss3dlayout.py
+-rw-r--r--   0        0        0   278583 2024-03-28 13:42:38.071355 pyaedt-0.8.7/pyaedt/icepak.py
+-rw-r--r--   0        0        0   127720 2024-04-01 08:15:37.788471 pyaedt-0.8.7/pyaedt/maxwell.py
+-rw-r--r--   0        0        0     7953 2024-03-26 18:55:41.005072 pyaedt-0.8.7/pyaedt/maxwellcircuit.py
+-rw-r--r--   0        0        0    24538 2024-03-28 13:42:38.071355 pyaedt-0.8.7/pyaedt/mechanical.py
+-rw-r--r--   0        0        0     3642 2023-11-15 14:48:56.159371 pyaedt-0.8.7/pyaedt/misc/Console.py_build
+-rw-r--r--   0        0        0     2230 2023-11-15 14:48:56.159371 pyaedt-0.8.7/pyaedt/misc/Job_Settings.areg
+-rw-r--r--   0        0        0     3394 2023-11-15 14:48:56.159371 pyaedt-0.8.7/pyaedt/misc/Jupyter.py_build
+-rw-r--r--   0        0        0     4125 2023-11-15 14:48:56.159371 pyaedt-0.8.7/pyaedt/misc/Run_PyAEDT_Script.py_build
+-rw-r--r--   0        0        0     3526 2023-11-15 14:48:56.159371 pyaedt-0.8.7/pyaedt/misc/Run_PyAEDT_Toolkit_Script.py_build
+-rw-r--r--   0        0        0      202 2023-11-15 14:48:56.159371 pyaedt-0.8.7/pyaedt/misc/__init__.py
+-rw-r--r--   0        0        0    10796 2024-03-26 18:55:41.005072 pyaedt-0.8.7/pyaedt/misc/aedtlib_personalib_install.py
+-rw-r--r--   0        0        0    19870 2023-11-15 14:48:56.174972 pyaedt-0.8.7/pyaedt/misc/amat.xml
+-rw-r--r--   0        0        0     2620 2023-11-15 14:48:56.174972 pyaedt-0.8.7/pyaedt/misc/ansys_cloud.areg
+-rw-r--r--   0        0        0     2013 2024-01-03 08:09:11.617311 pyaedt-0.8.7/pyaedt/misc/config.schema.json
+-rw-r--r--   0        0        0     3554 2024-01-31 08:29:55.323250 pyaedt-0.8.7/pyaedt/misc/console_setup.py
+-rw-r--r--   0        0        0       48 2023-11-15 14:48:56.174972 pyaedt-0.8.7/pyaedt/misc/create_remote_dir.py
+-rw-r--r--   0        0        0    15250 2023-11-15 14:48:56.174972 pyaedt-0.8.7/pyaedt/misc/images/gallery/PyAEDT.png
+-rw-r--r--   0        0        0      855 2023-11-15 14:48:56.174972 pyaedt-0.8.7/pyaedt/misc/images/large/pyansys.png
+-rw-r--r--   0        0        0     5630 2024-03-08 09:52:28.386458 pyaedt-0.8.7/pyaedt/misc/install_extra_toolkits.py
+-rw-r--r--   0        0        0     1728 2023-11-15 14:48:56.174972 pyaedt-0.8.7/pyaedt/misc/jupyter_template.ipynb
+-rw-r--r--   0        0        0     2700 2024-03-26 18:55:41.005072 pyaedt-0.8.7/pyaedt/misc/misc.py
+-rw-r--r--   0        0        0   771467 2023-11-15 14:48:56.174972 pyaedt-0.8.7/pyaedt/misc/ml_data_file_train_100MHz_1GHz.json
+-rw-r--r--   0        0        0   502580 2023-11-15 14:48:56.190611 pyaedt-0.8.7/pyaedt/misc/ml_data_file_train_1GHz_10GHz.json
+-rw-r--r--   0        0        0   162026 2023-11-15 14:48:56.190611 pyaedt-0.8.7/pyaedt/misc/patch_svr_model_100MHz_1GHz.joblib
+-rw-r--r--   0        0        0   134414 2023-11-15 14:48:56.190611 pyaedt-0.8.7/pyaedt/misc/patch_svr_model_1GHz_10GHz.joblib
+-rw-r--r--   0        0        0      289 2023-11-15 14:48:56.190611 pyaedt-0.8.7/pyaedt/misc/pyaedt.runtimeconfig.json
+-rw-r--r--   0        0        0      960 2023-11-15 14:48:56.190611 pyaedt-0.8.7/pyaedt/misc/pyaedt_local_config.acf
+-rw-r--r--   0        0        0    16550 2023-11-15 14:48:56.190611 pyaedt-0.8.7/pyaedt/misc/pyansys-logo-black-cropped.png
+-rw-r--r--   0        0        0       61 2024-03-22 10:54:58.740472 pyaedt-0.8.7/pyaedt/misc/spisim_com_configuration_files/__init__.py
+-rw-r--r--   0        0        0     5192 2024-03-22 10:54:58.740472 pyaedt-0.8.7/pyaedt/misc/spisim_com_configuration_files/com_120d_8.json
+-rw-r--r--   0        0        0     5153 2024-03-22 10:54:58.740472 pyaedt-0.8.7/pyaedt/misc/spisim_com_configuration_files/com_93_8.json
+-rw-r--r--   0        0        0     5155 2024-03-22 10:54:58.740472 pyaedt-0.8.7/pyaedt/misc/spisim_com_configuration_files/com_94_17.json
+-rw-r--r--   0        0        0    12280 2024-03-22 10:54:58.740472 pyaedt-0.8.7/pyaedt/misc/spisim_com_configuration_files/com_parameters.py
+-rw-r--r--   0        0        0    15308 2024-03-22 10:54:58.740472 pyaedt-0.8.7/pyaedt/misc/spisim_com_configuration_files/com_settings_mapping.py
+-rw-r--r--   0        0        0      868 2023-11-15 14:48:56.190611 pyaedt-0.8.7/pyaedt/misc/template.acf
+-rw-r--r--   0        0        0        0 2023-11-15 14:48:56.190611 pyaedt-0.8.7/pyaedt/modeler/__init__.py
+-rw-r--r--   0        0        0        0 2023-11-15 14:48:56.190611 pyaedt-0.8.7/pyaedt/modeler/advanced_cad/__init__.py
+-rw-r--r--   0        0        0    14073 2024-02-09 10:07:59.429453 pyaedt-0.8.7/pyaedt/modeler/advanced_cad/actors.py
+-rw-r--r--   0        0        0    20019 2024-02-09 10:07:59.429453 pyaedt-0.8.7/pyaedt/modeler/advanced_cad/multiparts.py
+-rw-r--r--   0        0        0    18513 2023-11-15 14:48:56.190611 pyaedt-0.8.7/pyaedt/modeler/advanced_cad/oms.py
+-rw-r--r--   0        0        0    16809 2023-11-15 14:48:56.190611 pyaedt-0.8.7/pyaedt/modeler/advanced_cad/parts.py
+-rw-r--r--   0        0        0   126188 2024-02-06 15:33:49.579885 pyaedt-0.8.7/pyaedt/modeler/advanced_cad/stackup_3d.py
+-rw-r--r--   0        0        0    80015 2024-03-26 18:55:41.005072 pyaedt-0.8.7/pyaedt/modeler/cad/Modeler.py
+-rw-r--r--   0        0        0   335961 2024-04-01 07:45:19.391915 pyaedt-0.8.7/pyaedt/modeler/cad/Primitives.py
+-rw-r--r--   0        0        0    13476 2024-03-27 08:05:27.450020 pyaedt-0.8.7/pyaedt/modeler/cad/Primitives2D.py
+-rw-r--r--   0        0        0   143002 2024-04-01 07:45:19.407506 pyaedt-0.8.7/pyaedt/modeler/cad/Primitives3D.py
+-rw-r--r--   0        0        0        0 2023-11-15 14:48:56.206131 pyaedt-0.8.7/pyaedt/modeler/cad/__init__.py
+-rw-r--r--   0        0        0    29696 2024-03-20 14:17:36.246401 pyaedt-0.8.7/pyaedt/modeler/cad/component_array.py
+-rw-r--r--   0        0        0    40015 2024-03-26 18:55:41.020699 pyaedt-0.8.7/pyaedt/modeler/cad/components_3d.py
+-rw-r--r--   0        0        0    49410 2024-03-26 18:55:41.020699 pyaedt-0.8.7/pyaedt/modeler/cad/elements3d.py
+-rw-r--r--   0        0        0    59455 2024-04-01 12:04:06.409314 pyaedt-0.8.7/pyaedt/modeler/cad/object3d.py
+-rw-r--r--   0        0        0    53212 2024-03-26 18:55:41.020699 pyaedt-0.8.7/pyaedt/modeler/cad/polylines.py
+-rw-r--r--   0        0        0    12604 2023-11-15 14:48:56.206131 pyaedt-0.8.7/pyaedt/modeler/calculators.py
+-rw-r--r--   0        0        0    44084 2024-03-29 09:59:34.311519 pyaedt-0.8.7/pyaedt/modeler/circuits/PrimitivesCircuit.py
+-rw-r--r--   0        0        0    39272 2024-02-06 15:33:49.595515 pyaedt-0.8.7/pyaedt/modeler/circuits/PrimitivesEmit.py
+-rw-r--r--   0        0        0     8396 2023-11-15 14:48:56.221789 pyaedt-0.8.7/pyaedt/modeler/circuits/PrimitivesMaxwellCircuit.py
+-rw-r--r--   0        0        0    67681 2024-03-07 08:39:44.005598 pyaedt-0.8.7/pyaedt/modeler/circuits/PrimitivesNexxim.py
+-rw-r--r--   0        0        0    15130 2023-11-15 14:48:56.221789 pyaedt-0.8.7/pyaedt/modeler/circuits/PrimitivesTwinBuilder.py
+-rw-r--r--   0        0        0        0 2023-11-15 14:48:56.221789 pyaedt-0.8.7/pyaedt/modeler/circuits/__init__.py
+-rw-r--r--   0        0        0    34191 2024-03-26 18:55:41.020699 pyaedt-0.8.7/pyaedt/modeler/circuits/object3dcircuit.py
+-rw-r--r--   0        0        0    68182 2024-03-28 13:42:38.086947 pyaedt-0.8.7/pyaedt/modeler/geometry_operators.py
+-rw-r--r--   0        0        0     6929 2023-11-15 14:48:56.221789 pyaedt-0.8.7/pyaedt/modeler/modeler2d.py
+-rw-r--r--   0        0        0    66173 2024-03-28 13:42:38.086947 pyaedt-0.8.7/pyaedt/modeler/modeler3d.py
+-rw-r--r--   0        0        0    33255 2024-03-26 18:55:41.036345 pyaedt-0.8.7/pyaedt/modeler/modelerpcb.py
+-rw-r--r--   0        0        0    50776 2024-03-26 18:55:41.036345 pyaedt-0.8.7/pyaedt/modeler/pcb/Primitives3DLayout.py
+-rw-r--r--   0        0        0        0 2023-11-15 14:48:56.221789 pyaedt-0.8.7/pyaedt/modeler/pcb/__init__.py
+-rw-r--r--   0        0        0    65931 2024-03-28 13:42:38.086947 pyaedt-0.8.7/pyaedt/modeler/pcb/object3dlayout.py
+-rw-r--r--   0        0        0    23852 2024-03-26 18:55:41.036345 pyaedt-0.8.7/pyaedt/modeler/schematic.py
+-rw-r--r--   0        0        0    54859 2024-03-28 13:42:38.086947 pyaedt-0.8.7/pyaedt/modules/AdvancedPostProcessing.py
+-rw-r--r--   0        0        0   169955 2024-03-26 18:55:41.036345 pyaedt-0.8.7/pyaedt/modules/Boundary.py
+-rw-r--r--   0        0        0    71690 2024-03-28 08:42:12.610163 pyaedt-0.8.7/pyaedt/modules/CableModeling.py
+-rw-r--r--   0        0        0    16319 2023-11-15 14:48:56.237302 pyaedt-0.8.7/pyaedt/modules/CircuitTemplates.py
+-rw-r--r--   0        0        0    56766 2024-03-29 09:59:34.311519 pyaedt-0.8.7/pyaedt/modules/DesignXPloration.py
+-rw-r--r--   0        0        0    40449 2024-03-26 18:55:41.036345 pyaedt-0.8.7/pyaedt/modules/LayerStackup.py
+-rw-r--r--   0        0        0   104701 2024-03-29 09:59:34.311519 pyaedt-0.8.7/pyaedt/modules/Material.py
+-rw-r--r--   0        0        0    33683 2024-03-26 18:55:41.051947 pyaedt-0.8.7/pyaedt/modules/MaterialLib.py
+-rw-r--r--   0        0        0    53774 2024-03-26 18:55:41.051947 pyaedt-0.8.7/pyaedt/modules/Mesh.py
+-rw-r--r--   0        0        0    12018 2024-03-26 18:55:41.051947 pyaedt-0.8.7/pyaedt/modules/Mesh3DLayout.py
+-rw-r--r--   0        0        0    48847 2024-03-26 18:55:41.051947 pyaedt-0.8.7/pyaedt/modules/MeshIcepak.py
+-rw-r--r--   0        0        0     4437 2023-11-15 14:48:56.237302 pyaedt-0.8.7/pyaedt/modules/OptimetricsTemplates.py
+-rw-r--r--   0        0        0   206587 2024-03-28 13:42:38.086947 pyaedt-0.8.7/pyaedt/modules/PostProcessor.py
+-rw-r--r--   0        0        0    72048 2024-03-08 11:06:30.309390 pyaedt-0.8.7/pyaedt/modules/SetupTemplates.py
+-rw-r--r--   0        0        0   147780 2024-03-28 13:42:38.086947 pyaedt-0.8.7/pyaedt/modules/SolveSetup.py
+-rw-r--r--   0        0        0    34324 2024-03-26 18:55:41.051947 pyaedt-0.8.7/pyaedt/modules/SolveSweeps.py
+-rw-r--r--   0        0        0        0 2023-11-15 14:48:56.252956 pyaedt-0.8.7/pyaedt/modules/__init__.py
+-rw-r--r--   0        0        0    31434 2024-03-26 18:55:41.051947 pyaedt-0.8.7/pyaedt/modules/monitor_icepak.py
+-rw-r--r--   0        0        0   132190 2024-03-26 18:55:41.067597 pyaedt-0.8.7/pyaedt/modules/report_templates.py
+-rw-r--r--   0        0        0   134882 2024-04-02 06:26:14.161852 pyaedt-0.8.7/pyaedt/modules/solutions.py
+-rw-r--r--   0        0        0    97835 2024-03-26 18:55:41.067597 pyaedt-0.8.7/pyaedt/q3d.py
+-rw-r--r--   0        0        0    10664 2024-02-02 15:15:46.569416 pyaedt-0.8.7/pyaedt/rmxprt.py
+-rw-r--r--   0        0        0        0 2023-11-15 14:48:56.252956 pyaedt-0.8.7/pyaedt/rpc/__init__.py
+-rw-r--r--   0        0        0      415 2023-11-15 14:48:56.252956 pyaedt-0.8.7/pyaedt/rpc/local_server.py
+-rw-r--r--   0        0        0    42133 2024-03-28 08:42:12.610163 pyaedt-0.8.7/pyaedt/rpc/rpyc_services.py
+-rw-r--r--   0        0        0        0 2023-11-15 14:48:56.252956 pyaedt-0.8.7/pyaedt/sbrplus/__init__.py
+-rw-r--r--   0        0        0     9463 2023-11-15 14:48:56.252956 pyaedt-0.8.7/pyaedt/sbrplus/hdm_parser.py
+-rw-r--r--   0        0        0     2096 2023-11-15 14:48:56.252956 pyaedt-0.8.7/pyaedt/sbrplus/hdm_utils.py
+-rw-r--r--   0        0        0     2607 2023-11-15 14:48:56.252956 pyaedt-0.8.7/pyaedt/sbrplus/matlab/HdmObject.m
+-rw-r--r--   0        0        0       97 2023-11-15 14:48:56.252956 pyaedt-0.8.7/pyaedt/sbrplus/matlab/README.md
+-rw-r--r--   0        0        0      735 2023-11-15 14:48:56.252956 pyaedt-0.8.7/pyaedt/sbrplus/matlab/SbrBounceType.m
+-rw-r--r--   0        0        0     2886 2023-11-15 14:48:56.252956 pyaedt-0.8.7/pyaedt/sbrplus/matlab/StopWatch.m
+-rw-r--r--   0        0        0     1402 2023-11-15 14:48:56.252956 pyaedt-0.8.7/pyaedt/sbrplus/matlab/add_3dlight.m
+-rw-r--r--   0        0        0      340 2023-11-15 14:48:56.268468 pyaedt-0.8.7/pyaedt/sbrplus/matlab/amp2db.m
+-rw-r--r--   0        0        0    36837 2023-11-15 14:48:56.268468 pyaedt-0.8.7/pyaedt/sbrplus/matlab/draw_rays1.m
+-rw-r--r--   0        0        0     4322 2023-11-15 14:48:56.268468 pyaedt-0.8.7/pyaedt/sbrplus/matlab/draw_wfobj.m
+-rw-r--r--   0        0        0    31414 2023-11-15 14:48:56.268468 pyaedt-0.8.7/pyaedt/sbrplus/matlab/filter_rays1.m
+-rw-r--r--   0        0        0     1504 2023-11-15 14:48:56.268468 pyaedt-0.8.7/pyaedt/sbrplus/matlab/filtered_tracks.m
+-rw-r--r--   0        0        0    20853 2023-11-15 14:48:56.268468 pyaedt-0.8.7/pyaedt/sbrplus/matlab/ld_sbrplushdm.m
+-rw-r--r--   0        0        0    14781 2023-11-15 14:48:56.268468 pyaedt-0.8.7/pyaedt/sbrplus/matlab/ld_wfobj.m
+-rw-r--r--   0        0        0      318 2023-11-15 14:48:56.268468 pyaedt-0.8.7/pyaedt/sbrplus/matlab/pwr2db.m
+-rw-r--r--   0        0        0     2607 2023-11-15 14:48:56.268468 pyaedt-0.8.7/pyaedt/sbrplus/matlab/validate_sfields.m
+-rw-r--r--   0        0        0     7621 2024-03-26 18:55:41.067597 pyaedt-0.8.7/pyaedt/sbrplus/plot.py
+-rw-r--r--   0        0        0    21628 2024-03-28 08:42:12.610163 pyaedt-0.8.7/pyaedt/twinbuilder.py
+-rw-r--r--   0        0        0     6767 2024-04-02 21:38:59.514185 pyaedt-0.8.7/pyproject.toml
+-rw-r--r--   0        0        0    16443 1970-01-01 00:00:00.000000 pyaedt-0.8.7/PKG-INFO
```

### Comparing `pyaedt-0.8.6/LICENSE` & `pyaedt-0.8.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.6/README.md` & `pyaedt-0.8.7/README.md`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.6/pyaedt/__init__.py` & `pyaedt-0.8.7/pyaedt/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
 
 deprecation_warning()
 
 #
 
 pyaedt_path = os.path.dirname(__file__)
-__version__ = "0.8.6"
+__version__ = "0.8.7"
 version = __version__
 
 #
 
 import pyaedt.downloads as downloads
 from pyaedt.generic import constants
 import pyaedt.generic.DataHandlers as data_handler
```

### Comparing `pyaedt-0.8.6/pyaedt/aedt_logger.py` & `pyaedt-0.8.7/pyaedt/aedt_logger.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.6/pyaedt/application/AEDT_File_Management.py` & `pyaedt-0.8.7/pyaedt/application/AEDT_File_Management.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.6/pyaedt/application/Analysis.py` & `pyaedt-0.8.7/pyaedt/application/Analysis.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.6/pyaedt/application/Analysis3D.py` & `pyaedt-0.8.7/pyaedt/application/Analysis3D.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.6/pyaedt/application/Analysis3DLayout.py` & `pyaedt-0.8.7/pyaedt/application/Analysis3DLayout.py`

 * *Files 1% similar despite different names*

```diff
@@ -325,23 +325,23 @@
             For example, ``["S(1, 2)", "S(1, 3)", "S(2, 3)"]``.
 
         References
         ----------
 
         >>> oModule.GetAllPorts
         """
-        next = []
+        next_xtalks = []
         if not trlist:
             trlist = [i for i in self.excitations if tx_prefix in i]
         for i in trlist:
             k = trlist.index(i) + 1
             while k < len(trlist):
-                next.append("S({},{})".format(i, trlist[k]))
+                next_xtalks.append("S({},{})".format(i, trlist[k]))
                 k += 1
-        return next
+        return next_xtalks
 
     @pyaedt_function_handler()
     def get_fext_xtalk_list(self, trlist=None, reclist=None, tx_prefix="", rx_prefix="", skip_same_index_couples=True):
         """Retrieve a list of all the far end XTalks from two lists of exctitations (driver and receiver).
 
         Parameters
         ----------
```

### Comparing `pyaedt-0.8.6/pyaedt/application/AnalysisMaxwellCircuit.py` & `pyaedt-0.8.7/pyaedt/application/AnalysisMaxwellCircuit.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.6/pyaedt/application/AnalysisNexxim.py` & `pyaedt-0.8.7/pyaedt/application/AnalysisNexxim.py`

 * *Files 1% similar despite different names*

```diff
@@ -479,23 +479,23 @@
             For example, ``["S(1, 2)", "S(1, 3)", "S(2, 3)"]``.
 
         References
         ----------
 
         >>> oEditor.GetAllPorts
         """
-        next = []
+        next_xtalks = []
         if not trlist:
             trlist = [i for i in list(self.excitations.keys()) if tx_prefix in i]
         for i in trlist:
             k = trlist.index(i) + 1
             while k < len(trlist):
-                next.append("S({},{})".format(i, trlist[k]))
+                next_xtalks.append("S({},{})".format(i, trlist[k]))
                 k += 1
-        return next
+        return next_xtalks
 
     @pyaedt_function_handler()
     def get_fext_xtalk_list(self, trlist=None, reclist=None, tx_prefix="", rx_prefix="", skip_same_index_couples=True):
         """Retrieve a list of all the far end XTalks from two lists of exctitations (driver and receiver).
 
         Parameters
         ----------
```

### Comparing `pyaedt-0.8.6/pyaedt/application/AnalysisRMxprt.py` & `pyaedt-0.8.7/pyaedt/application/AnalysisRMxprt.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.6/pyaedt/application/AnalysisTwinBuilder.py` & `pyaedt-0.8.7/pyaedt/application/AnalysisTwinBuilder.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.6/pyaedt/application/Design.py` & `pyaedt-0.8.7/pyaedt/application/Design.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.6/pyaedt/application/JobManager.py` & `pyaedt-0.8.7/pyaedt/application/JobManager.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.6/pyaedt/application/Variables.py` & `pyaedt-0.8.7/pyaedt/application/Variables.py`

 * *Files 1% similar despite different names*

```diff
@@ -780,34 +780,34 @@
         self._independent_design_variables = {}
         self._independent_project_variables = {}
         self._dependent_design_variables = {}
         self._dependent_project_variables = {}
 
     @property
     def _independent_variables(self):
-        all = {}
-        all.update(self._independent_project_variables)
-        all.update(self._independent_design_variables)
-        return all
+        all_independent = {}
+        all_independent.update(self._independent_project_variables)
+        all_independent.update(self._independent_design_variables)
+        return all_independent
 
     @property
     def _dependent_variables(self):
-        all = {}
+        all_dependent = {}
         for k, v in self._dependent_project_variables.items():
-            all[k] = v
+            all_dependent[k] = v
         for k, v in self._dependent_design_variables.items():
-            all[k] = v
-        return all
+            all_dependent[k] = v
+        return all_dependent
 
     @property
     def _all_variables(self):
-        all = {}
-        all.update(self._independent_variables)
-        all.update(self._dependent_variables)
-        return all
+        all_variables = {}
+        all_variables.update(self._independent_variables)
+        all_variables.update(self._dependent_variables)
+        return all_variables
 
     @pyaedt_function_handler()
     def __delitem__(self, key):
         """Implement del with array name or index."""
         self.delete_variable(key)
 
     @pyaedt_function_handler()
```

### Comparing `pyaedt-0.8.6/pyaedt/application/aedt_objects.py` & `pyaedt-0.8.7/pyaedt/application/aedt_objects.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.6/pyaedt/application/design_solutions.py` & `pyaedt-0.8.7/pyaedt/application/design_solutions.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.6/pyaedt/circuit.py` & `pyaedt-0.8.7/pyaedt/circuit.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.6/pyaedt/common_rpc.py` & `pyaedt-0.8.7/pyaedt/common_rpc.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.6/pyaedt/desktop.py` & `pyaedt-0.8.7/pyaedt/desktop.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,16 +54,14 @@
 
 pathname = os.path.dirname(__file__)
 
 pyaedtversion = __version__
 
 modules = [tup[1] for tup in pkgutil.iter_modules()]
 
-python_grpc_wrapper = None
-
 
 @pyaedt_function_handler()
 def launch_aedt(full_path, non_graphical, port, student_version, first_run=True):
     """Launch AEDT in gRPC mode."""
 
     def launch_desktop_on_port():
         command = [full_path, "-grpcsrv", str(port)]
@@ -235,15 +233,14 @@
 
     Returns
     -------
     bool
         ``True`` when successful, ``False`` when failed.
 
     """
-    global python_grpc_wrapper
     if settings.remote_rpc_session or (settings.aedt_version >= "2022.2" and is_grpc_api and not is_ironpython):
         if close_desktop and desktop_class.parent_desktop_id:
             pyaedt_logger.error("A child desktop session is linked to this session.")
             pyaedt_logger.error("Multiple desktop sessions must be released in reverse order.")
             return False
         elif close_desktop:
             try:
@@ -269,17 +266,16 @@
                 warnings.warn("Something went wrong closing AEDT. Exception in `_main.oDesktop.QuitApplication()`.")
         elif _desktop_sessions and len(_desktop_sessions) > 1:
             pyaedt_logger.error("A child desktop session is linked to this session.")
             pyaedt_logger.error("Multiple desktop sessions must be released in reverse order.")
             return False
         else:
             try:
-                if not python_grpc_wrapper:
-                    python_grpc_wrapper = __import__("pyaedt.generic.grpc_plugin")
-                # import pyaedt.generic.grpc_plugin as StandalonePyScriptWrapper
+                import pyaedt.generic.grpc_plugin as python_grpc_wrapper
+
                 python_grpc_wrapper.AedtAPI.ReleaseAll()
                 return True
             except Exception:  # pragma: no cover
                 warnings.warn(
                     "Something went wrong releasing AEDT. Exception in `StandalonePyScriptWrapper.Release()`."
                 )
     elif not inside_desktop:
@@ -907,15 +903,14 @@
         machine="",
         port=0,
         non_graphical=False,
         new_session=False,
         version=None,
         is_grpc=True,
     ):
-        global python_grpc_wrapper
         if not is_grpc:
             from pyaedt.generic.clr_module import _clr
 
             _clr.AddReference("Ansys.Ansoft.CoreCOMScripting")
             AnsoftCOMUtil = __import__("Ansys.Ansoft.CoreCOMScripting")
             self.COMUtil = AnsoftCOMUtil.Ansoft.CoreCOMScripting.Util.COMUtil
             StandalonePyScriptWrapper = AnsoftCOMUtil.Ansoft.CoreCOMScripting.COM.StandalonePyScriptWrapper
@@ -930,18 +925,16 @@
             sys.path.insert(0, os.path.join(base_path, "PythonFiles", "DesktopPlugin"))
             if is_linux:
                 pyaedt_path = os.path.realpath(os.path.join(os.path.dirname(os.path.realpath(__file__)), ".."))
                 os.environ["PATH"] = pyaedt_path + os.pathsep + os.environ["PATH"]
             os.environ["DesktopPluginPyAEDT"] = os.path.join(settings.aedt_install_dir, "PythonFiles", "DesktopPlugin")
             launch_msg = "AEDT installation Path {}".format(base_path)
             self.logger.info(launch_msg)
-            if not python_grpc_wrapper:
-                python_grpc_wrapper = __import__("pyaedt.generic.grpc_plugin")
-                python_grpc_wrapper = python_grpc_wrapper.generic.grpc_plugin
-            # import pyaedt.generic.grpc_plugin as StandalonePyScriptWrapper
+            import pyaedt.generic.grpc_plugin as python_grpc_wrapper
+
             if _desktop_sessions:
                 last_session = list(_desktop_sessions.values())[-1]
                 all_desktop = [i for i in last_session.odesktop.GetRunningInstancesMgr().GetAllRunningInstances()]
                 for desktop in all_desktop:
                     if port and desktop.GetGrpcServerPort() == port:
                         self.isoutsideDesktop = True
                         self.odesktop = desktop
```

### Comparing `pyaedt-0.8.6/pyaedt/downloads.py` & `pyaedt-0.8.7/pyaedt/downloads.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.6/pyaedt/emit.py` & `pyaedt-0.8.7/pyaedt/emit.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.6/pyaedt/emit_core/Couplings.py` & `pyaedt-0.8.7/pyaedt/emit_core/Couplings.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.6/pyaedt/emit_core/__init__.py` & `pyaedt-0.8.7/pyaedt/emit_core/__init__.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.6/pyaedt/emit_core/emit_constants.py` & `pyaedt-0.8.7/pyaedt/emit_core/emit_constants.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.6/pyaedt/emit_core/results/results.py` & `pyaedt-0.8.7/pyaedt/emit_core/results/results.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.6/pyaedt/emit_core/results/revision.py` & `pyaedt-0.8.7/pyaedt/emit_core/results/revision.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.6/pyaedt/generic/Ansys.png` & `pyaedt-0.8.7/pyaedt/generic/Ansys.png`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.6/pyaedt/generic/AnsysTemplate.json` & `pyaedt-0.8.7/pyaedt/generic/AnsysTemplate.json`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.6/pyaedt/generic/DataHandlers.py` & `pyaedt-0.8.7/pyaedt/generic/DataHandlers.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.6/pyaedt/generic/LoadAEDTFile.py` & `pyaedt-0.8.7/pyaedt/generic/LoadAEDTFile.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.6/pyaedt/generic/ami.json` & `pyaedt-0.8.7/pyaedt/generic/ami.json`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.6/pyaedt/generic/clr_module.py` & `pyaedt-0.8.7/pyaedt/generic/clr_module.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.6/pyaedt/generic/compliance.py` & `pyaedt-0.8.7/pyaedt/generic/compliance.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.6/pyaedt/generic/configurations.py` & `pyaedt-0.8.7/pyaedt/generic/configurations.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from collections import OrderedDict
 import copy
 from datetime import datetime
 import json
 import os
-import pkgutil
 import tempfile
 
 import pyaedt
 from pyaedt import Icepak
 from pyaedt import __version__
 from pyaedt import generate_unique_folder_name
 from pyaedt import get_pyaedt_app
@@ -688,20 +687,31 @@
     """Enables export and import of a JSON configuration file that can be applied to a new or existing design."""
 
     def __init__(self, app):
         self._app = app
         self.options = ConfigurationsOptions()
         self.results = ImportResults()
 
-        # Read the default configuration schema from pyaedt
-        schema_bytes = pkgutil.get_data(
-            __name__, os.path.join(os.path.dirname(pyaedt.__file__), "misc", "config.schema.json")
-        )
-        schema_string = schema_bytes.decode("utf-8")
-        self._schema = json.loads(schema_string)
+        pyaedt_installed_path = os.path.dirname(pyaedt.__file__)
+
+        schema_bytes = None
+
+        config_schema_path = os.path.join(pyaedt_installed_path, "misc", "config.schema.json")
+
+        if os.path.exists(config_schema_path):
+            with open(config_schema_path, "rb") as schema:
+                schema_bytes = schema.read()
+
+        if schema_bytes:
+            # Read the default configuration schema from pyaedt
+            schema_string = schema_bytes.decode("utf-8")
+            self._schema = json.loads(schema_string)
+        else:  # pragma: no cover
+            self._app.logger.error("Failed to load configuration schema.")
+            self._schema = None
 
     @staticmethod
     @pyaedt_function_handler()
     def _map_dict_value(dict_out, key, value):
         dict_out["general"]["object_mapping"][str(key)] = value
 
     @pyaedt_function_handler()
```

### Comparing `pyaedt-0.8.6/pyaedt/generic/constants.py` & `pyaedt-0.8.7/pyaedt/generic/constants.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.6/pyaedt/generic/design_types.py` & `pyaedt-0.8.7/pyaedt/generic/design_types.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.6/pyaedt/generic/filesystem.py` & `pyaedt-0.8.7/pyaedt/generic/filesystem.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.6/pyaedt/generic/general_methods.py` & `pyaedt-0.8.7/pyaedt/generic/general_methods.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.6/pyaedt/generic/grpc_plugin.py` & `pyaedt-0.8.7/pyaedt/generic/grpc_plugin.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.6/pyaedt/generic/grpc_plugin_dll.py` & `pyaedt-0.8.7/pyaedt/generic/grpc_plugin_dll.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.6/pyaedt/generic/ibis_reader.py` & `pyaedt-0.8.7/pyaedt/generic/ibis_reader.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.6/pyaedt/generic/ibis_v7.json` & `pyaedt-0.8.7/pyaedt/generic/ibis_v7.json`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.6/pyaedt/generic/near_field_import.py` & `pyaedt-0.8.7/pyaedt/generic/near_field_import.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.6/pyaedt/generic/pdf.py` & `pyaedt-0.8.7/pyaedt/generic/pdf.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.6/pyaedt/generic/plot.py` & `pyaedt-0.8.7/pyaedt/generic/plot.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.6/pyaedt/generic/python_optimizers.py` & `pyaedt-0.8.7/pyaedt/generic/python_optimizers.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.6/pyaedt/generic/report_file_parser.py` & `pyaedt-0.8.7/pyaedt/generic/report_file_parser.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.6/pyaedt/generic/settings.py` & `pyaedt-0.8.7/pyaedt/generic/settings.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.6/pyaedt/generic/spisim.py` & `pyaedt-0.8.7/pyaedt/generic/spisim.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.6/pyaedt/generic/touchstone_parser.py` & `pyaedt-0.8.7/pyaedt/generic/touchstone_parser.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.6/pyaedt/hfss.py` & `pyaedt-0.8.7/pyaedt/hfss.py`

 * *Files 1% similar despite different names*

```diff
@@ -222,17 +222,26 @@
         List of str
         """
         return self.odesign.GetChildObject("Radiation").GetChildNames()
 
     class BoundaryType(object):
         """Creates and manages boundaries."""
 
-        (PerfectE, PerfectH, Aperture, Radiation, Impedance, LayeredImp, LumpedRLC, FiniteCond, Hybrid, FEBI) = range(
-            0, 10
-        )
+        (
+            PerfectE,
+            PerfectH,
+            Aperture,
+            Radiation,
+            Impedance,
+            LayeredImp,
+            LumpedRLC,
+            FiniteCond,
+            Hybrid,
+            FEBI,
+        ) = range(0, 10)
 
     @property
     def hybrid(self):
         """HFSS hybrid mode for the active solution.
 
         For instance, it must be set to ``True`` to define the solution type as 'HFSS with Hybrid and Arrays'.
 
@@ -3629,16 +3638,16 @@
 
     @pyaedt_function_handler()
     def assign_impedance_to_sheet(self, sheet_name, sourcename=None, resistance=50, reactance=0, is_infground=False):
         """Create an impedance taking one sheet.
 
         Parameters
         ----------
-        sheet_name : str
-            Name of the sheet to apply the boundary to.
+        sheet_name : str or list
+            Name of the sheet or list to apply the boundary to.
         sourcename : str, optional
             Name of the impedance. The default is ``None``.
         resistance : optional
             Resistance value in ohms. The default is ``50``. If ``None``,
             this parameter is disabled.
         reactance : optional
             Reactance value in ohms. The default is ``0``. If ``None``,
@@ -3671,26 +3680,136 @@
         """
 
         if self.solution_type in ["Modal", "Terminal", "Transient Network"]:
             if not sourcename:
                 sourcename = generate_unique_name("Imped")
             elif sourcename in self.modeler.get_boundaries_name():
                 sourcename = generate_unique_name(sourcename)
+
+            objects = self.modeler.convert_to_selections(sheet_name, True)
+
             props = OrderedDict(
                 {
-                    "Objects": [sheet_name],
-                    "Resistance": str(resistance),
-                    "Reactance": str(reactance),
-                    "InfGroundPlane": is_infground,
+                    "Faces": objects,
                 }
             )
+            if isinstance(objects[0], str):
+                props = OrderedDict(
+                    {
+                        "Objects": objects,
+                    }
+                )
+            props["Resistance"] = str(resistance)
+            props["Reactance"] = str(reactance)
+            props["InfGroundPlane"] = is_infground
+
             return self._create_boundary(sourcename, props, "Impedance")
         return False
 
     @pyaedt_function_handler()
+    def assign_impedance_to_sheet(
+        self, sheet_name, sourcename=None, resistance=50.0, reactance=0.0, is_infground=False, reference_cs="Global"
+    ):
+        """Create an impedance taking one sheet.
+
+        Parameters
+        ----------
+        sheet_name : str or list
+            Name of the sheet or list to apply the boundary to.
+        sourcename : str, optional
+            Name of the impedance. The default is ``None``.
+        resistance : float or list, optional
+            Resistance value in ohms. The default is ``50.0``.
+            If a list of four elements is passed, an anisotropic impedance is assigned with the following order,
+            [``Zxx``, ``Zxy``, ``Zyx``, ``Zyy``].
+        reactance : optional
+            Reactance value in ohms. The default is ``0.0``.
+            If a list of four elements is passed, an anisotropic impedance is assigned with the following order,
+            [``Zxx``, ``Zxy``, ``Zyx``, ``Zyy``].
+        is_infground : bool, optional
+            Whether the impedance is an infinite ground. The default is ``False``.
+        reference_cs : str, optional
+            Name of the coordinate system for the XY plane. The default is ``"Global"``.
+            This parameter is only used for anisotropic impedance assignment.
+
+        Returns
+        -------
+        :class:`pyaedt.modules.Boundary.BoundaryObject`
+            Boundary object if successful, ``False`` otherwise.
+
+        References
+        ----------
+
+        >>> oModule.AssignImpedance
+
+        Examples
+        --------
+
+        Create a sheet and use it to create an impedance.
+
+        >>> sheet = hfss.modeler.create_rectangle(hfss.PLANE.XY,
+        ...                                       [0, 0, -90], [10, 2], name="ImpedanceSheet",
+        ...                                        matname="Copper")
+        >>> impedance_to_sheet = hfss.assign_impedance_to_sheet(sheet.name, "ImpedanceFromSheet", 100, 50)
+
+        Create a sheet and use it to create an anisotropic impedance.
+
+        >>> sheet = hfss.modeler.create_rectangle(hfss.PLANE.XY,
+        ...                                       [0, 0, -90], [10, 2], name="ImpedanceSheet",
+        ...                                        matname="Copper")
+        >>> anistropic_impedance_to_sheet = hfss.assign_impedance_to_sheet(sheet.name, "ImpedanceFromSheet",
+        ...                                                                 [377, 0, 0, 377], [0, 50, 0, 0])
+
+        """
+
+        if self.solution_type in ["Modal", "Terminal", "Transient Network"]:
+            if not sourcename:
+                sourcename = generate_unique_name("Imped")
+            elif sourcename in self.modeler.get_boundaries_name():
+                sourcename = generate_unique_name(sourcename)
+
+            objects = self.modeler.convert_to_selections(sheet_name, True)
+
+            props = OrderedDict(
+                {
+                    "Faces": objects,
+                }
+            )
+            if isinstance(objects[0], str):
+                props = OrderedDict(
+                    {
+                        "Objects": objects,
+                    }
+                )
+
+            if isinstance(resistance, list) and isinstance(reactance, list):
+                if len(resistance) == 4 and len(reactance) == 4:
+                    props["UseInfiniteGroundPlane"] = is_infground
+                    props["CoordSystem"] = reference_cs
+                    props["HasExternalLink"] = False
+                    props["ZxxResistance"] = str(resistance[0])
+                    props["ZxxReactance"] = str(reactance[0])
+                    props["ZxyResistance"] = str(resistance[1])
+                    props["ZxyReactance"] = str(reactance[1])
+                    props["ZyxResistance"] = str(resistance[2])
+                    props["ZyxReactance"] = str(reactance[2])
+                    props["ZyyResistance"] = str(resistance[3])
+                    props["ZyyReactance"] = str(reactance[3])
+                else:
+                    self.logger.error("Number of elements in resistance and reactance must be four.")
+                    return False
+                return self._create_boundary(sourcename, props, "Anisotropic Impedance")
+            else:
+                props["Resistance"] = str(resistance)
+                props["Reactance"] = str(reactance)
+                props["InfGroundPlane"] = is_infground
+                return self._create_boundary(sourcename, props, "Impedance")
+        return False
+
+    @pyaedt_function_handler()
     def create_circuit_port_from_edges(
         self,
         edge_signal,
         edge_gnd,
         port_name="",
         port_impedance="50",
         renormalize=False,
```

### Comparing `pyaedt-0.8.6/pyaedt/hfss3dlayout.py` & `pyaedt-0.8.7/pyaedt/hfss3dlayout.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.6/pyaedt/icepak.py` & `pyaedt-0.8.7/pyaedt/icepak.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.6/pyaedt/maxwell.py` & `pyaedt-0.8.7/pyaedt/maxwell.py`

 * *Files 1% similar despite different names*

```diff
@@ -962,15 +962,21 @@
         if not name:
             name = generate_unique_name("Voltage")
         face_list = self.modeler.convert_to_selections(face_list, True)
 
         if self.design_type == "Maxwell 2D":
             props = OrderedDict({"Objects": face_list, "Value": amplitude})
         else:
-            props = OrderedDict({"Faces": face_list, "Voltage": amplitude})
+            if len(face_list) == 1:
+                if isinstance(face_list[0], str) and face_list[0] in self.modeler.object_names:
+                    props = OrderedDict({"Objects": face_list, "Voltage": amplitude})
+                else:
+                    props = OrderedDict({"Faces": face_list, "Value": amplitude})
+            else:
+                props = OrderedDict({"Faces": face_list, "Voltage": amplitude})
         bound = BoundaryObject(self, name, props, "Voltage")
         if bound.create():
             self._boundaries[bound.name] = bound
             return bound
         return False
 
     @pyaedt_function_handler()
```

### Comparing `pyaedt-0.8.6/pyaedt/maxwellcircuit.py` & `pyaedt-0.8.7/pyaedt/maxwellcircuit.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.6/pyaedt/mechanical.py` & `pyaedt-0.8.7/pyaedt/mechanical.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.6/pyaedt/misc/Console.py_build` & `pyaedt-0.8.7/pyaedt/misc/Console.py_build`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.6/pyaedt/misc/Job_Settings.areg` & `pyaedt-0.8.7/pyaedt/misc/Job_Settings.areg`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.6/pyaedt/misc/Jupyter.py_build` & `pyaedt-0.8.7/pyaedt/misc/Jupyter.py_build`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.6/pyaedt/misc/Run_PyAEDT_Script.py_build` & `pyaedt-0.8.7/pyaedt/misc/Run_PyAEDT_Script.py_build`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.6/pyaedt/misc/Run_PyAEDT_Toolkit_Script.py_build` & `pyaedt-0.8.7/pyaedt/misc/Run_PyAEDT_Toolkit_Script.py_build`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.6/pyaedt/misc/aedtlib_personalib_install.py` & `pyaedt-0.8.7/pyaedt/misc/aedtlib_personalib_install.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.6/pyaedt/misc/amat.xml` & `pyaedt-0.8.7/pyaedt/misc/amat.xml`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.6/pyaedt/misc/ansys_cloud.areg` & `pyaedt-0.8.7/pyaedt/misc/ansys_cloud.areg`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.6/pyaedt/misc/config.schema.json` & `pyaedt-0.8.7/pyaedt/misc/config.schema.json`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.6/pyaedt/misc/console_setup.py` & `pyaedt-0.8.7/pyaedt/misc/console_setup.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.6/pyaedt/misc/images/gallery/PyAEDT.png` & `pyaedt-0.8.7/pyaedt/misc/images/gallery/PyAEDT.png`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.6/pyaedt/misc/images/large/pyansys.png` & `pyaedt-0.8.7/pyaedt/misc/images/large/pyansys.png`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.6/pyaedt/misc/install_extra_toolkits.py` & `pyaedt-0.8.7/pyaedt/misc/install_extra_toolkits.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.6/pyaedt/misc/jupyter_template.ipynb` & `pyaedt-0.8.7/pyaedt/misc/jupyter_template.ipynb`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.6/pyaedt/misc/misc.py` & `pyaedt-0.8.7/pyaedt/misc/misc.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.6/pyaedt/misc/ml_data_file_train_100MHz_1GHz.json` & `pyaedt-0.8.7/pyaedt/misc/ml_data_file_train_100MHz_1GHz.json`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.6/pyaedt/misc/ml_data_file_train_1GHz_10GHz.json` & `pyaedt-0.8.7/pyaedt/misc/ml_data_file_train_1GHz_10GHz.json`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.6/pyaedt/misc/patch_svr_model_100MHz_1GHz.joblib` & `pyaedt-0.8.7/pyaedt/misc/patch_svr_model_100MHz_1GHz.joblib`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.6/pyaedt/misc/patch_svr_model_1GHz_10GHz.joblib` & `pyaedt-0.8.7/pyaedt/misc/patch_svr_model_1GHz_10GHz.joblib`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.6/pyaedt/misc/pyaedt_local_config.acf` & `pyaedt-0.8.7/pyaedt/misc/pyaedt_local_config.acf`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.6/pyaedt/misc/pyansys-logo-black-cropped.png` & `pyaedt-0.8.7/pyaedt/misc/pyansys-logo-black-cropped.png`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.6/pyaedt/misc/spisim_com_configuration_files/com_120d_8.json` & `pyaedt-0.8.7/pyaedt/misc/spisim_com_configuration_files/com_120d_8.json`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.6/pyaedt/misc/spisim_com_configuration_files/com_93_8.json` & `pyaedt-0.8.7/pyaedt/misc/spisim_com_configuration_files/com_93_8.json`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.6/pyaedt/misc/spisim_com_configuration_files/com_94_17.json` & `pyaedt-0.8.7/pyaedt/misc/spisim_com_configuration_files/com_94_17.json`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.6/pyaedt/misc/spisim_com_configuration_files/com_parameters.py` & `pyaedt-0.8.7/pyaedt/misc/spisim_com_configuration_files/com_parameters.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.6/pyaedt/misc/spisim_com_configuration_files/com_settings_mapping.py` & `pyaedt-0.8.7/pyaedt/misc/spisim_com_configuration_files/com_settings_mapping.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.6/pyaedt/misc/template.acf` & `pyaedt-0.8.7/pyaedt/misc/template.acf`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.6/pyaedt/modeler/advanced_cad/actors.py` & `pyaedt-0.8.7/pyaedt/modeler/advanced_cad/actors.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.6/pyaedt/modeler/advanced_cad/multiparts.py` & `pyaedt-0.8.7/pyaedt/modeler/advanced_cad/multiparts.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.6/pyaedt/modeler/advanced_cad/oms.py` & `pyaedt-0.8.7/pyaedt/modeler/advanced_cad/oms.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.6/pyaedt/modeler/advanced_cad/parts.py` & `pyaedt-0.8.7/pyaedt/modeler/advanced_cad/parts.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.6/pyaedt/modeler/advanced_cad/stackup_3d.py` & `pyaedt-0.8.7/pyaedt/modeler/advanced_cad/stackup_3d.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.6/pyaedt/modeler/cad/Modeler.py` & `pyaedt-0.8.7/pyaedt/modeler/cad/Modeler.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.6/pyaedt/modeler/cad/Primitives.py` & `pyaedt-0.8.7/pyaedt/modeler/cad/Primitives.py`

 * *Files 0% similar despite different names*

```diff
@@ -4647,24 +4647,25 @@
             ``True`` when successful, ``False`` when failed.
 
         References
         ----------
 
         >>> oEditor.CreateUserDefinedModel
         """
-        environlist = os.environ
-        latestversion = ""
-        for l in environlist:
-            if "AWP_ROOT" in l:
-                if l > latestversion:
-                    latestversion = l
-        if not latestversion:
+        env_var = os.environ
+        latest_version = ""
+        for variable in env_var:
+            if "AWP_ROOT" in variable:
+                if variable > latest_version:
+                    latest_version = variable
+                    break
+        if not latest_version:
             self.logger.error("SpaceClaim is not found.")
         else:
-            scdm_path = os.path.join(os.environ[latestversion], "scdm")
+            scdm_path = os.path.join(os.environ[latest_version], "scdm")
         self.oeditor.CreateUserDefinedModel(
             [
                 "NAME:UserDefinedModelParameters",
                 [
                     "NAME:Definition",
                     [
                         "NAME:UDMParam",
@@ -5090,38 +5091,38 @@
         aedt_bounding_box = self.get_model_bounding_box()
         directions = {}
         inputlist = self.convert_to_selections(inputlist, True)
         for el in inputlist:
             objID = self.oeditor.GetFaceIDs(el)
             faceCenter = self.oeditor.GetFaceCenter(int(objID[0]))
             directionfound = False
-            l = 10
+            thickness = 10
             while not directionfound:
                 self.oeditor.ThickenSheet(
                     ["NAME:Selections", "Selections:=", el, "NewPartsModelFlag:=", "Model"],
-                    ["NAME:SheetThickenParameters", "Thickness:=", str(l) + "mm", "BothSides:=", False],
+                    ["NAME:SheetThickenParameters", "Thickness:=", str(thickness) + "mm", "BothSides:=", False],
                 )
                 aedt_bounding_box2 = self.get_model_bounding_box()
                 self._odesign.Undo()
                 if aedt_bounding_box != aedt_bounding_box2:
                     directions[el] = "External"
                     directionfound = True
                 self.oeditor.ThickenSheet(
                     ["NAME:Selections", "Selections:=", el, "NewPartsModelFlag:=", "Model"],
-                    ["NAME:SheetThickenParameters", "Thickness:=", "-" + str(l) + "mm", "BothSides:=", False],
+                    ["NAME:SheetThickenParameters", "Thickness:=", "-" + str(thickness) + "mm", "BothSides:=", False],
                 )
                 aedt_bounding_box2 = self.get_model_bounding_box()
 
                 self._odesign.Undo()
 
                 if aedt_bounding_box != aedt_bounding_box2:
                     directions[el] = "Internal"
                     directionfound = True
                 else:
-                    l = l + 10
+                    thickness = thickness + 10
         for el in inputlist:
             objID = self.oeditor.GetFaceIDs(el)
             faceCenter = self.oeditor.GetFaceCenter(int(objID[0]))
             if directions[el] == "Internal":
                 self.oeditor.ThickenSheet(
                     ["NAME:Selections", "Selections:=", el, "NewPartsModelFlag:=", "Model"],
                     ["NAME:SheetThickenParameters", "Thickness:=", "-" + str(value) + "mm", "BothSides:=", False],
```

### Comparing `pyaedt-0.8.6/pyaedt/modeler/cad/Primitives2D.py` & `pyaedt-0.8.7/pyaedt/modeler/cad/Primitives2D.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.6/pyaedt/modeler/cad/Primitives3D.py` & `pyaedt-0.8.7/pyaedt/modeler/cad/Primitives3D.py`

 * *Files 0% similar despite different names*

```diff
@@ -548,16 +548,16 @@
         first_argument.append("WhichAxis:="), first_argument.append(axis)
         second_argument = self._default_object_attributes(name=name, matname=material_name)
         new_object_name = self.oeditor.CreateTorus(first_argument, second_argument)
         return self._create_object(new_object_name, **kwargs)
 
     # fmt: off
     @pyaedt_function_handler()
-    def create_bondwire(self,  start_position, end_position, h1=0.2, h2=0, alpha=80, beta=5, bond_type=0,
-                        diameter=0.025,  facets=6, name=None,  matname=None, cs_axis="Z", **kwargs):  # fmt: on
+    def create_bondwire(self, start_position, end_position, h1=0.2, h2=0, alpha=80, beta=5, bond_type=0,
+                        diameter=0.025, facets=6, name=None, matname=None, cs_axis="Z", **kwargs):  # fmt: on
         # type : (list, list, float|str=0.2, float|str=0, float=80, float=5, int=0, float|str=0.025, int=6, str=None,
         # str=None) -> Object3d
         """Create a bondwire.
 
         Parameters
         ----------
         start_position : list
```

### Comparing `pyaedt-0.8.6/pyaedt/modeler/cad/component_array.py` & `pyaedt-0.8.7/pyaedt/modeler/cad/component_array.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.6/pyaedt/modeler/cad/components_3d.py` & `pyaedt-0.8.7/pyaedt/modeler/cad/components_3d.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.6/pyaedt/modeler/cad/elements3d.py` & `pyaedt-0.8.7/pyaedt/modeler/cad/elements3d.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.6/pyaedt/modeler/cad/object3d.py` & `pyaedt-0.8.7/pyaedt/modeler/cad/object3d.py`

 * *Files 2% similar despite different names*

```diff
@@ -1085,15 +1085,15 @@
                 vGeo3d = ["NAME:Geometry3DAttributeTab", vPropServers, vChangedProps]
                 vOut = ["NAME:AllTabs", vGeo3d]
                 self._primitives.oeditor.ChangeProperty(vOut)
                 self._m_name = obj_name
                 self._primitives.add_new_objects()
                 self._primitives.cleanup_objects()
         else:
-            pass
+            self.logger.warning("{} is already used in current design.".format(obj_name))
 
     @property
     def valid_properties(self):
         """Valid properties.
 
         References
         ----------
```

### Comparing `pyaedt-0.8.6/pyaedt/modeler/cad/polylines.py` & `pyaedt-0.8.7/pyaedt/modeler/cad/polylines.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.6/pyaedt/modeler/calculators.py` & `pyaedt-0.8.7/pyaedt/modeler/calculators.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.6/pyaedt/modeler/circuits/PrimitivesCircuit.py` & `pyaedt-0.8.7/pyaedt/modeler/circuits/PrimitivesCircuit.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.6/pyaedt/modeler/circuits/PrimitivesEmit.py` & `pyaedt-0.8.7/pyaedt/modeler/circuits/PrimitivesEmit.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.6/pyaedt/modeler/circuits/PrimitivesMaxwellCircuit.py` & `pyaedt-0.8.7/pyaedt/modeler/circuits/PrimitivesMaxwellCircuit.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.6/pyaedt/modeler/circuits/PrimitivesNexxim.py` & `pyaedt-0.8.7/pyaedt/modeler/circuits/PrimitivesNexxim.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.6/pyaedt/modeler/circuits/PrimitivesTwinBuilder.py` & `pyaedt-0.8.7/pyaedt/modeler/circuits/PrimitivesTwinBuilder.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.6/pyaedt/modeler/circuits/object3dcircuit.py` & `pyaedt-0.8.7/pyaedt/modeler/circuits/object3dcircuit.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.6/pyaedt/modeler/geometry_operators.py` & `pyaedt-0.8.7/pyaedt/modeler/geometry_operators.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.6/pyaedt/modeler/modeler2d.py` & `pyaedt-0.8.7/pyaedt/modeler/modeler2d.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.6/pyaedt/modeler/modeler3d.py` & `pyaedt-0.8.7/pyaedt/modeler/modeler3d.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.6/pyaedt/modeler/modelerpcb.py` & `pyaedt-0.8.7/pyaedt/modeler/modelerpcb.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.6/pyaedt/modeler/pcb/Primitives3DLayout.py` & `pyaedt-0.8.7/pyaedt/modeler/pcb/Primitives3DLayout.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.6/pyaedt/modeler/pcb/object3dlayout.py` & `pyaedt-0.8.7/pyaedt/modeler/pcb/object3dlayout.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.6/pyaedt/modeler/schematic.py` & `pyaedt-0.8.7/pyaedt/modeler/schematic.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.6/pyaedt/modules/AdvancedPostProcessing.py` & `pyaedt-0.8.7/pyaedt/modules/AdvancedPostProcessing.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.6/pyaedt/modules/Boundary.py` & `pyaedt-0.8.7/pyaedt/modules/Boundary.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.6/pyaedt/modules/CableModeling.py` & `pyaedt-0.8.7/pyaedt/modules/CableModeling.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.6/pyaedt/modules/CircuitTemplates.py` & `pyaedt-0.8.7/pyaedt/modules/CircuitTemplates.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.6/pyaedt/modules/DesignXPloration.py` & `pyaedt-0.8.7/pyaedt/modules/DesignXPloration.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.6/pyaedt/modules/LayerStackup.py` & `pyaedt-0.8.7/pyaedt/modules/LayerStackup.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.6/pyaedt/modules/Material.py` & `pyaedt-0.8.7/pyaedt/modules/Material.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.6/pyaedt/modules/MaterialLib.py` & `pyaedt-0.8.7/pyaedt/modules/MaterialLib.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.6/pyaedt/modules/Mesh.py` & `pyaedt-0.8.7/pyaedt/modules/Mesh.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.6/pyaedt/modules/Mesh3DLayout.py` & `pyaedt-0.8.7/pyaedt/modules/Mesh3DLayout.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.6/pyaedt/modules/MeshIcepak.py` & `pyaedt-0.8.7/pyaedt/modules/MeshIcepak.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.6/pyaedt/modules/OptimetricsTemplates.py` & `pyaedt-0.8.7/pyaedt/modules/OptimetricsTemplates.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.6/pyaedt/modules/PostProcessor.py` & `pyaedt-0.8.7/pyaedt/modules/PostProcessor.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.6/pyaedt/modules/SetupTemplates.py` & `pyaedt-0.8.7/pyaedt/modules/SetupTemplates.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.6/pyaedt/modules/SolveSetup.py` & `pyaedt-0.8.7/pyaedt/modules/SolveSetup.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.6/pyaedt/modules/SolveSweeps.py` & `pyaedt-0.8.7/pyaedt/modules/SolveSweeps.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.6/pyaedt/modules/monitor_icepak.py` & `pyaedt-0.8.7/pyaedt/modules/monitor_icepak.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.6/pyaedt/modules/report_templates.py` & `pyaedt-0.8.7/pyaedt/modules/report_templates.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.6/pyaedt/modules/solutions.py` & `pyaedt-0.8.7/pyaedt/modules/solutions.py`

 * *Files 0% similar despite different names*

```diff
@@ -2594,15 +2594,15 @@
     @pyaedt_function_handler()
     def _update_both(self):
         """Update far field."""
         self.ff.farfield_data = self.ff.combine_farfield(phi_scan=self._phi, theta_scan=self._theta)
 
         self.ff.mesh = self.ff.get_far_field_mesh(self.farfield_quantity, self.quantity_format)
 
-        self.output.overwrite(self.ff.mesh)
+        self.output.copy_from(self.ff.mesh)
         return
 
     @pyaedt_function_handler()
     def update_phi(self, phi):
         """Update the Phi value."""
         self._phi = phi
         self._update_both()
```

### Comparing `pyaedt-0.8.6/pyaedt/q3d.py` & `pyaedt-0.8.7/pyaedt/q3d.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.6/pyaedt/rmxprt.py` & `pyaedt-0.8.7/pyaedt/rmxprt.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.6/pyaedt/rpc/rpyc_services.py` & `pyaedt-0.8.7/pyaedt/rpc/rpyc_services.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.6/pyaedt/sbrplus/hdm_parser.py` & `pyaedt-0.8.7/pyaedt/sbrplus/hdm_parser.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.6/pyaedt/sbrplus/hdm_utils.py` & `pyaedt-0.8.7/pyaedt/sbrplus/hdm_utils.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.6/pyaedt/sbrplus/matlab/HdmObject.m` & `pyaedt-0.8.7/pyaedt/sbrplus/matlab/HdmObject.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.6/pyaedt/sbrplus/matlab/SbrBounceType.m` & `pyaedt-0.8.7/pyaedt/sbrplus/matlab/SbrBounceType.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.6/pyaedt/sbrplus/matlab/StopWatch.m` & `pyaedt-0.8.7/pyaedt/sbrplus/matlab/StopWatch.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.6/pyaedt/sbrplus/matlab/add_3dlight.m` & `pyaedt-0.8.7/pyaedt/sbrplus/matlab/add_3dlight.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.6/pyaedt/sbrplus/matlab/draw_rays1.m` & `pyaedt-0.8.7/pyaedt/sbrplus/matlab/draw_rays1.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.6/pyaedt/sbrplus/matlab/draw_wfobj.m` & `pyaedt-0.8.7/pyaedt/sbrplus/matlab/draw_wfobj.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.6/pyaedt/sbrplus/matlab/filter_rays1.m` & `pyaedt-0.8.7/pyaedt/sbrplus/matlab/filter_rays1.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.6/pyaedt/sbrplus/matlab/filtered_tracks.m` & `pyaedt-0.8.7/pyaedt/sbrplus/matlab/filtered_tracks.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.6/pyaedt/sbrplus/matlab/ld_sbrplushdm.m` & `pyaedt-0.8.7/pyaedt/sbrplus/matlab/ld_sbrplushdm.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.6/pyaedt/sbrplus/matlab/ld_wfobj.m` & `pyaedt-0.8.7/pyaedt/sbrplus/matlab/ld_wfobj.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.6/pyaedt/sbrplus/matlab/validate_sfields.m` & `pyaedt-0.8.7/pyaedt/sbrplus/matlab/validate_sfields.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.6/pyaedt/sbrplus/plot.py` & `pyaedt-0.8.7/pyaedt/sbrplus/plot.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.6/pyaedt/twinbuilder.py` & `pyaedt-0.8.7/pyaedt/twinbuilder.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.6/pyproject.toml` & `pyaedt-0.8.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -33,25 +33,25 @@
     "pyedb>=0.5.0; python_version > '3.7'",
     "pytomlpp; python_version < '3.12'",
     "rpyc>=6.0.0,<6.1",
 ]
 
 [project.optional-dependencies]
 tests = [
-    "imageio>=2.30.0,<2.34",
-    "ipython>=7.30.0,<8.23",
+    "imageio>=2.30.0,<2.35",
+    "ipython>=7.30.0,<8.24",
     "joblib>=1.0.0,<1.4",
     "matplotlib>=3.5.0,<3.9",
     "mock>=5.1.0,<5.2",
     "numpy>=1.20.0,<2",
     "openpyxl>=3.1.0,<3.3",
     "osmnx>=1.1.0,<1.10",
     "pandas>=1.1.0,<2.3",
     "pytest>=7.4.0,<8.2",
-    "pytest-cov>=4.0.0,<4.2",
+    "pytest-cov>=4.0.0,<5.1",
     "pytest-xdist>=3.5.0,<3.6",
     "pyedb>=0.4.0,<0.5; python_version == '3.7'",
     "pyedb>=0.5.0,<0.8; python_version > '3.7'",
     "pyvista>=0.38.0,<0.44",
     "scikit-learn>=1.0.0,<1.5",
     "scikit-rf>=0.30.0,<0.33",
     "SRTM.py",
@@ -62,19 +62,19 @@
     "ansys-pythonnet>=3.1.0rc3",
     "cffi==1.15.1; platform_system=='Linux' and python_version == '3.7'",
     "cffi>=1.16.0,<1.17; platform_system=='Linux' and python_version > '3.7'",
     "dotnetcore2==3.1.23; platform_system=='Linux'",
     "pywin32>=303; platform_system=='Windows'",
 ]
 doc = [
-    "ansys-sphinx-theme>=0.10.0,<0.15",
+    "ansys-sphinx-theme>=0.10.0,<0.16",
     "imageio>=2.30.0,<2.35",
     #"imageio-ffmpeg>=0.4.0,<0.5",
     "ipython>=7.34.0; python_version == '3.7'",
-    "ipython>=8.13.0,<8.23; python_version > '3.7'",
+    "ipython>=8.13.0,<8.24; python_version > '3.7'",
     #"ipywidgets>=8.0.0,<8.2",
     "joblib>=1.3.0,<1.4",
     "jupyterlab>=4.0.0,<4.3",
     "matplotlib>=3.5.0,<3.9",
     "nbsphinx>=0.9.0,<0.10",
     "numpydoc>=1.5.0,<1.8",
     "openpyxl>=3.0.0,<3.2",
@@ -98,15 +98,15 @@
     "sphinx_design>=0.4.0,<0.6",
     #"sphinxcontrib-websupport",
     "SRTM.py",
     "utm",
     "vtk==9.2.6",
 ]
 doc-noexamples = [
-    "ansys-sphinx-theme>=0.10.0,<0.15",
+    "ansys-sphinx-theme>=0.10.0,<0.16",
     "imageio>=2.30.0,<2.35",
     #"imageio-ffmpeg",
     "numpydoc>=1.5.0,<1.8",
     # "recommonmark",
     "Sphinx==5.3.0; python_version == '3.7'",
     "Sphinx>=7.1.0,<7.3; python_version > '3.7'",
     "sphinx-autobuild==2021.3.14; python_version == '3.7'",
```

### Comparing `pyaedt-0.8.6/PKG-INFO` & `pyaedt-0.8.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaedt
-Version: 0.8.6
+Version: 0.8.7
 Summary: Higher-Level Pythonic Ansys Electronics Desktop Framework
 Author-email: "ANSYS, Inc." <pyansys.core@ansys.com>
 Maintainer-email: PyAEDT developers <massimo.capodiferro@ansys.com>
 Requires-Python: >=3.7,<4
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
@@ -30,18 +30,18 @@
 Requires-Dist: osmnx>=1.1.0,<1.10 ; extra == "all"
 Requires-Dist: pandas>=1.1.0,<2.3 ; extra == "all"
 Requires-Dist: pyvista>=0.38.0,<0.44 ; extra == "all"
 Requires-Dist: scikit-rf>=0.30.0,<0.33 ; extra == "all"
 Requires-Dist: SRTM.py ; extra == "all"
 Requires-Dist: utm ; extra == "all"
 Requires-Dist: vtk==9.2.6 ; extra == "all"
-Requires-Dist: ansys-sphinx-theme>=0.10.0,<0.15 ; extra == "doc"
+Requires-Dist: ansys-sphinx-theme>=0.10.0,<0.16 ; extra == "doc"
 Requires-Dist: imageio>=2.30.0,<2.35 ; extra == "doc"
 Requires-Dist: ipython>=7.34.0 ; extra == "doc" and ( python_version == '3.7')
-Requires-Dist: ipython>=8.13.0,<8.23 ; extra == "doc" and ( python_version > '3.7')
+Requires-Dist: ipython>=8.13.0,<8.24 ; extra == "doc" and ( python_version > '3.7')
 Requires-Dist: joblib>=1.3.0,<1.4 ; extra == "doc"
 Requires-Dist: jupyterlab>=4.0.0,<4.3 ; extra == "doc"
 Requires-Dist: matplotlib>=3.5.0,<3.9 ; extra == "doc"
 Requires-Dist: nbsphinx>=0.9.0,<0.10 ; extra == "doc"
 Requires-Dist: numpydoc>=1.5.0,<1.8 ; extra == "doc"
 Requires-Dist: openpyxl>=3.0.0,<3.2 ; extra == "doc"
 Requires-Dist: osmnx>=1.1.0,<1.10 ; extra == "doc"
@@ -56,15 +56,15 @@
 Requires-Dist: sphinx-copybutton>=0.5.0,<0.6 ; extra == "doc"
 Requires-Dist: sphinx-gallery>=0.14.0,<0.16 ; extra == "doc"
 Requires-Dist: sphinx-jinja>=2.0,<2.1 ; extra == "doc"
 Requires-Dist: sphinx_design>=0.4.0,<0.6 ; extra == "doc"
 Requires-Dist: SRTM.py ; extra == "doc"
 Requires-Dist: utm ; extra == "doc"
 Requires-Dist: vtk==9.2.6 ; extra == "doc"
-Requires-Dist: ansys-sphinx-theme>=0.10.0,<0.15 ; extra == "doc-noexamples"
+Requires-Dist: ansys-sphinx-theme>=0.10.0,<0.16 ; extra == "doc-noexamples"
 Requires-Dist: imageio>=2.30.0,<2.35 ; extra == "doc-noexamples"
 Requires-Dist: numpydoc>=1.5.0,<1.8 ; extra == "doc-noexamples"
 Requires-Dist: Sphinx==5.3.0 ; extra == "doc-noexamples" and ( python_version == '3.7')
 Requires-Dist: Sphinx>=7.1.0,<7.3 ; extra == "doc-noexamples" and ( python_version > '3.7')
 Requires-Dist: sphinx-autobuild==2021.3.14 ; extra == "doc-noexamples" and ( python_version == '3.7')
 Requires-Dist: sphinx-autobuild==2021.3.14 ; extra == "doc-noexamples" and ( python_version == '3.8')
 Requires-Dist: sphinx-autobuild==2024.2.4 ; extra == "doc-noexamples" and ( python_version > '3.8')
@@ -73,25 +73,25 @@
 Requires-Dist: sphinx_design>=0.4.0,<0.6 ; extra == "doc-noexamples"
 Requires-Dist: sphinx-jinja>=2.0,<2.1 ; extra == "doc-noexamples"
 Requires-Dist: ansys-pythonnet>=3.1.0rc3 ; extra == "dotnet"
 Requires-Dist: cffi==1.15.1 ; extra == "dotnet" and ( platform_system=='Linux' and python_version == '3.7')
 Requires-Dist: cffi>=1.16.0,<1.17 ; extra == "dotnet" and ( platform_system=='Linux' and python_version > '3.7')
 Requires-Dist: dotnetcore2==3.1.23 ; extra == "dotnet" and ( platform_system=='Linux')
 Requires-Dist: pywin32>=303 ; extra == "dotnet" and ( platform_system=='Windows')
-Requires-Dist: imageio>=2.30.0,<2.34 ; extra == "tests"
-Requires-Dist: ipython>=7.30.0,<8.23 ; extra == "tests"
+Requires-Dist: imageio>=2.30.0,<2.35 ; extra == "tests"
+Requires-Dist: ipython>=7.30.0,<8.24 ; extra == "tests"
 Requires-Dist: joblib>=1.0.0,<1.4 ; extra == "tests"
 Requires-Dist: matplotlib>=3.5.0,<3.9 ; extra == "tests"
 Requires-Dist: mock>=5.1.0,<5.2 ; extra == "tests"
 Requires-Dist: numpy>=1.20.0,<2 ; extra == "tests"
 Requires-Dist: openpyxl>=3.1.0,<3.3 ; extra == "tests"
 Requires-Dist: osmnx>=1.1.0,<1.10 ; extra == "tests"
 Requires-Dist: pandas>=1.1.0,<2.3 ; extra == "tests"
 Requires-Dist: pytest>=7.4.0,<8.2 ; extra == "tests"
-Requires-Dist: pytest-cov>=4.0.0,<4.2 ; extra == "tests"
+Requires-Dist: pytest-cov>=4.0.0,<5.1 ; extra == "tests"
 Requires-Dist: pytest-xdist>=3.5.0,<3.6 ; extra == "tests"
 Requires-Dist: pyedb>=0.4.0,<0.5 ; extra == "tests" and ( python_version == '3.7')
 Requires-Dist: pyedb>=0.5.0,<0.8 ; extra == "tests" and ( python_version > '3.7')
 Requires-Dist: pyvista>=0.38.0,<0.44 ; extra == "tests"
 Requires-Dist: scikit-learn>=1.0.0,<1.5 ; extra == "tests"
 Requires-Dist: scikit-rf>=0.30.0,<0.33 ; extra == "tests"
 Requires-Dist: SRTM.py ; extra == "tests"
```


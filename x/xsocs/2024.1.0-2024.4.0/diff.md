# Comparing `tmp/xsocs-2024.1.0.tar.gz` & `tmp/xsocs-2024.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xsocs-2024.1.0.tar", last modified: Fri Jan 26 13:25:53 2024, max compression
+gzip compressed data, was "xsocs-2024.4.0.tar", last modified: Wed Apr  3 14:57:06 2024, max compression
```

## Comparing `xsocs-2024.1.0.tar` & `xsocs-2024.4.0.tar`

### file list

```diff
@@ -1,192 +1,192 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-26 13:25:53.006017 xsocs-2024.1.0/
--rw-rw-rw-   0 root         (0) root         (0)     4765 2024-01-26 13:25:32.000000 xsocs-2024.1.0/CHANGELOG.rst
--rw-rw-rw-   0 root         (0) root         (0)     1101 2024-01-26 12:48:32.000000 xsocs-2024.1.0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      112 2024-01-26 12:48:32.000000 xsocs-2024.1.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2917 2024-01-26 13:25:53.006017 xsocs-2024.1.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1136 2024-01-26 12:48:32.000000 xsocs-2024.1.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-26 13:25:52.962017 xsocs-2024.1.0/doc/
--rw-rw-rw-   0 root         (0) root         (0)     7703 2024-01-26 12:48:32.000000 xsocs-2024.1.0/doc/conf.py
--rw-rw-rw-   0 root         (0) root         (0)     2979 2024-01-26 12:48:32.000000 xsocs-2024.1.0/doc/fileformat.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-26 13:25:52.962017 xsocs-2024.1.0/doc/img/
--rw-rw-rw-   0 root         (0) root         (0)    99637 2024-01-26 12:48:32.000000 xsocs-2024.1.0/doc/img/input_file.png
--rw-rw-rw-   0 root         (0) root         (0)     1032 2024-01-26 12:48:32.000000 xsocs-2024.1.0/doc/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     2399 2024-01-26 12:48:32.000000 xsocs-2024.1.0/doc/install.rst
--rw-rw-rw-   0 root         (0) root         (0)     1313 2024-01-26 12:48:32.000000 xsocs-2024.1.0/doc/modules.rst
--rw-rw-rw-   0 root         (0) root         (0)      614 2024-01-26 12:48:32.000000 xsocs-2024.1.0/doc/troubleshooting.rst
--rw-rw-rw-   0 root         (0) root         (0)     1204 2024-01-26 12:48:32.000000 xsocs-2024.1.0/doc/tutorials.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-26 13:25:52.966017 xsocs-2024.1.0/doc/usage/
--rw-rw-rw-   0 root         (0) root         (0)     2340 2024-01-26 12:48:32.000000 xsocs-2024.1.0/doc/usage/conversion.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-26 13:25:52.974017 xsocs-2024.1.0/doc/usage/img/
--rw-rw-rw-   0 root         (0) root         (0)   114617 2024-01-26 12:48:32.000000 xsocs-2024.1.0/doc/usage/img/com_results_view.png
--rw-rw-rw-   0 root         (0) root         (0)    83045 2024-01-26 12:48:32.000000 xsocs-2024.1.0/doc/usage/img/conversion_dialog.png
--rw-rw-rw-   0 root         (0) root         (0)      622 2024-01-26 12:48:32.000000 xsocs-2024.1.0/doc/usage/img/draw_roi_button.png
--rw-rw-rw-   0 root         (0) root         (0)     1403 2024-01-26 12:48:32.000000 xsocs-2024.1.0/doc/usage/img/export_fit_button.png
--rw-rw-rw-   0 root         (0) root         (0)     1113 2024-01-26 12:48:32.000000 xsocs-2024.1.0/doc/usage/img/fit_results_button.png
--rw-rw-rw-   0 root         (0) root         (0)   156322 2024-01-26 12:48:32.000000 xsocs-2024.1.0/doc/usage/img/fit_results_view.png
--rw-rw-rw-   0 root         (0) root         (0)     1113 2024-01-26 12:48:32.000000 xsocs-2024.1.0/doc/usage/img/intensity_plot_button.png
--rw-rw-rw-   0 root         (0) root         (0)   136848 2024-01-26 12:48:32.000000 xsocs-2024.1.0/doc/usage/img/intensity_view.png
--rw-rw-rw-   0 root         (0) root         (0)     7280 2024-01-26 12:48:32.000000 xsocs-2024.1.0/doc/usage/img/main_view.png
--rw-rw-rw-   0 root         (0) root         (0)    41461 2024-01-26 12:48:32.000000 xsocs-2024.1.0/doc/usage/img/merge_window.png
--rw-rw-rw-   0 root         (0) root         (0)    37829 2024-01-26 12:48:32.000000 xsocs-2024.1.0/doc/usage/img/open_dialog.png
--rw-rw-rw-   0 root         (0) root         (0)      926 2024-01-26 12:48:32.000000 xsocs-2024.1.0/doc/usage/img/open_icon.png
--rw-rw-rw-   0 root         (0) root         (0)    34780 2024-01-26 12:48:32.000000 xsocs-2024.1.0/doc/usage/img/project_tree.png
--rw-rw-rw-   0 root         (0) root         (0)    86754 2024-01-26 12:48:32.000000 xsocs-2024.1.0/doc/usage/img/qspace_stack_view.png
--rw-rw-rw-   0 root         (0) root         (0)     1053 2024-01-26 12:48:32.000000 xsocs-2024.1.0/doc/usage/img/qspace_view_button.png
--rw-rw-rw-   0 root         (0) root         (0)   110038 2024-01-26 12:48:32.000000 xsocs-2024.1.0/doc/usage/img/qspace_window.png
--rw-rw-rw-   0 root         (0) root         (0)   145447 2024-01-26 12:48:32.000000 xsocs-2024.1.0/doc/usage/img/shift_editor.png
--rw-rw-rw-   0 root         (0) root         (0)     2876 2024-01-26 12:48:32.000000 xsocs-2024.1.0/doc/usage/img/to_qspace_button.png
--rw-rw-rw-   0 root         (0) root         (0)     2898 2024-01-26 12:48:32.000000 xsocs-2024.1.0/doc/usage/intensity_view.rst
--rw-rw-rw-   0 root         (0) root         (0)     6751 2024-01-26 12:48:32.000000 xsocs-2024.1.0/doc/usage/project.rst
--rw-rw-rw-   0 root         (0) root         (0)     2535 2024-01-26 12:48:32.000000 xsocs-2024.1.0/doc/usage/project_view.rst
--rw-rw-rw-   0 root         (0) root         (0)     3053 2024-01-26 12:48:32.000000 xsocs-2024.1.0/doc/usage/qspace_view.rst
--rw-rw-rw-   0 root         (0) root         (0)     1763 2024-01-26 12:48:32.000000 xsocs-2024.1.0/doc/usage/results_view.rst
--rw-rw-rw-   0 root         (0) root         (0)      786 2024-01-26 12:48:32.000000 xsocs-2024.1.0/doc/usage/starting.rst
--rw-rw-rw-   0 root         (0) root         (0)      388 2024-01-26 12:48:32.000000 xsocs-2024.1.0/doc/using.rst
--rw-rw-rw-   0 root         (0) root         (0)      101 2024-01-26 12:48:32.000000 xsocs-2024.1.0/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1632 2024-01-26 13:25:53.010017 xsocs-2024.1.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       70 2024-01-26 12:48:32.000000 xsocs-2024.1.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-26 13:25:52.954017 xsocs-2024.1.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-26 13:25:52.974017 xsocs-2024.1.0/src/xsocs/
--rw-rw-rw-   0 root         (0) root         (0)      523 2024-01-26 12:48:32.000000 xsocs-2024.1.0/src/xsocs/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      847 2024-01-26 12:48:32.000000 xsocs-2024.1.0/src/xsocs/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-26 13:25:52.978017 xsocs-2024.1.0/src/xsocs/_app/
--rw-rw-rw-   0 root         (0) root         (0)       33 2024-01-26 12:48:32.000000 xsocs-2024.1.0/src/xsocs/_app/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2633 2024-01-26 12:48:32.000000 xsocs-2024.1.0/src/xsocs/_app/concat.py
--rw-rw-rw-   0 root         (0) root         (0)     1162 2024-01-26 12:48:32.000000 xsocs-2024.1.0/src/xsocs/_app/gui.py
--rw-rw-rw-   0 root         (0) root         (0)      714 2024-01-26 12:48:32.000000 xsocs-2024.1.0/src/xsocs/_config.py
--rw-rw-rw-   0 root         (0) root         (0)     2776 2024-01-26 13:25:32.000000 xsocs-2024.1.0/src/xsocs/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-26 13:25:52.978017 xsocs-2024.1.0/src/xsocs/examples/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-26 13:25:32.000000 xsocs-2024.1.0/src/xsocs/examples/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2600 2024-01-26 12:48:32.000000 xsocs-2024.1.0/src/xsocs/examples/id01_merge.py
--rw-rw-rw-   0 root         (0) root         (0)     1985 2024-01-26 12:48:32.000000 xsocs-2024.1.0/src/xsocs/examples/id01_peak.py
--rw-rw-rw-   0 root         (0) root         (0)     1681 2024-01-26 12:48:32.000000 xsocs-2024.1.0/src/xsocs/examples/id01_qspace.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-26 13:25:52.978017 xsocs-2024.1.0/src/xsocs/gui/
--rw-rw-rw-   0 root         (0) root         (0)      335 2024-01-26 12:48:32.000000 xsocs-2024.1.0/src/xsocs/gui/Utils.py
--rw-rw-rw-   0 root         (0) root         (0)    11955 2024-01-26 12:48:32.000000 xsocs-2024.1.0/src/xsocs/gui/XsocsGui.py
--rw-rw-rw-   0 root         (0) root         (0)      740 2024-01-26 12:48:32.000000 xsocs-2024.1.0/src/xsocs/gui/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      816 2024-01-26 12:48:32.000000 xsocs-2024.1.0/src/xsocs/gui/gui.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-26 13:25:52.982017 xsocs-2024.1.0/src/xsocs/gui/model/
--rw-rw-rw-   0 root         (0) root         (0)     5309 2024-01-26 12:48:32.000000 xsocs-2024.1.0/src/xsocs/gui/model/Model.py
--rw-rw-rw-   0 root         (0) root         (0)      360 2024-01-26 12:48:32.000000 xsocs-2024.1.0/src/xsocs/gui/model/ModelDef.py
--rw-rw-rw-   0 root         (0) root         (0)    39319 2024-01-26 12:48:32.000000 xsocs-2024.1.0/src/xsocs/gui/model/Node.py
--rw-rw-rw-   0 root         (0) root         (0)     1780 2024-01-26 12:48:32.000000 xsocs-2024.1.0/src/xsocs/gui/model/NodeEditor.py
--rw-rw-rw-   0 root         (0) root         (0)     4576 2024-01-26 12:48:32.000000 xsocs-2024.1.0/src/xsocs/gui/model/Nodes.py
--rw-rw-rw-   0 root         (0) root         (0)    13616 2024-01-26 12:48:32.000000 xsocs-2024.1.0/src/xsocs/gui/model/TreeView.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-26 13:25:32.000000 xsocs-2024.1.0/src/xsocs/gui/model/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-26 13:25:52.982017 xsocs-2024.1.0/src/xsocs/gui/process/
--rw-rw-rw-   0 root         (0) root         (0)     8467 2024-01-26 12:48:32.000000 xsocs-2024.1.0/src/xsocs/gui/process/FitWidget.py
--rw-rw-rw-   0 root         (0) root         (0)    43220 2024-01-26 12:48:32.000000 xsocs-2024.1.0/src/xsocs/gui/process/MergeWidget.py
--rw-rw-rw-   0 root         (0) root         (0)    34942 2024-01-26 12:48:32.000000 xsocs-2024.1.0/src/xsocs/gui/process/QSpaceWidget.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-26 13:25:32.000000 xsocs-2024.1.0/src/xsocs/gui/process/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-26 13:25:52.986017 xsocs-2024.1.0/src/xsocs/gui/project/
--rw-rw-rw-   0 root         (0) root         (0)      964 2024-01-26 12:48:32.000000 xsocs-2024.1.0/src/xsocs/gui/project/AcqDataGroup.py
--rw-rw-rw-   0 root         (0) root         (0)     2299 2024-01-26 12:48:32.000000 xsocs-2024.1.0/src/xsocs/gui/project/FitGroup.py
--rw-rw-rw-   0 root         (0) root         (0)     8312 2024-01-26 12:48:32.000000 xsocs-2024.1.0/src/xsocs/gui/project/Hdf5Nodes.py
--rw-rw-rw-   0 root         (0) root         (0)     7846 2024-01-26 12:48:32.000000 xsocs-2024.1.0/src/xsocs/gui/project/IntensityGroup.py
--rw-rw-rw-   0 root         (0) root         (0)      712 2024-01-26 12:48:32.000000 xsocs-2024.1.0/src/xsocs/gui/project/ProjectDef.py
--rw-rw-rw-   0 root         (0) root         (0)     9049 2024-01-26 12:48:32.000000 xsocs-2024.1.0/src/xsocs/gui/project/ProjectItem.py
--rw-rw-rw-   0 root         (0) root         (0)    22762 2024-01-26 12:48:32.000000 xsocs-2024.1.0/src/xsocs/gui/project/ProjectNodes.py
--rw-rw-rw-   0 root         (0) root         (0)     3348 2024-01-26 12:48:32.000000 xsocs-2024.1.0/src/xsocs/gui/project/QSpaceGroup.py
--rw-rw-rw-   0 root         (0) root         (0)     1984 2024-01-26 12:48:32.000000 xsocs-2024.1.0/src/xsocs/gui/project/ScanPositionsItem.py
--rw-rw-rw-   0 root         (0) root         (0)     3309 2024-01-26 12:48:32.000000 xsocs-2024.1.0/src/xsocs/gui/project/ShiftGroup.py
--rw-rw-rw-   0 root         (0) root         (0)      703 2024-01-26 12:48:32.000000 xsocs-2024.1.0/src/xsocs/gui/project/XsocsH5Factory.py
--rw-rw-rw-   0 root         (0) root         (0)     2956 2024-01-26 12:48:32.000000 xsocs-2024.1.0/src/xsocs/gui/project/XsocsProject.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-26 13:25:32.000000 xsocs-2024.1.0/src/xsocs/gui/project/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-26 13:25:52.986017 xsocs-2024.1.0/src/xsocs/gui/silx_imports/
--rw-rw-rw-   0 root         (0) root         (0)    25629 2024-01-26 12:48:32.000000 xsocs-2024.1.0/src/xsocs/gui/silx_imports/ImageRois.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-26 13:25:32.000000 xsocs-2024.1.0/src/xsocs/gui/silx_imports/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-26 13:25:52.986017 xsocs-2024.1.0/src/xsocs/gui/view/
--rw-rw-rw-   0 root         (0) root         (0)    11311 2024-01-26 12:48:32.000000 xsocs-2024.1.0/src/xsocs/gui/view/FitView.py
--rw-rw-rw-   0 root         (0) root         (0)    28432 2024-01-26 12:48:32.000000 xsocs-2024.1.0/src/xsocs/gui/view/QspaceView.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-26 13:25:32.000000 xsocs-2024.1.0/src/xsocs/gui/view/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-26 13:25:52.986017 xsocs-2024.1.0/src/xsocs/gui/view/fitview/
--rw-rw-rw-   0 root         (0) root         (0)     3085 2024-01-26 12:48:32.000000 xsocs-2024.1.0/src/xsocs/gui/view/fitview/DropPlotWidget.py
--rw-rw-rw-   0 root         (0) root         (0)     7574 2024-01-26 12:48:32.000000 xsocs-2024.1.0/src/xsocs/gui/view/fitview/FitModel.py
--rw-rw-rw-   0 root         (0) root         (0)     1949 2024-01-26 12:48:32.000000 xsocs-2024.1.0/src/xsocs/gui/view/fitview/Plotter.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-26 13:25:32.000000 xsocs-2024.1.0/src/xsocs/gui/view/fitview/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-26 13:25:52.986017 xsocs-2024.1.0/src/xsocs/gui/view/intensity/
--rw-rw-rw-   0 root         (0) root         (0)    25463 2024-01-26 12:48:32.000000 xsocs-2024.1.0/src/xsocs/gui/view/intensity/IntensityView.py
--rw-rw-rw-   0 root         (0) root         (0)     6050 2024-01-26 12:48:32.000000 xsocs-2024.1.0/src/xsocs/gui/view/intensity/RectRoiWidget.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-26 13:25:32.000000 xsocs-2024.1.0/src/xsocs/gui/view/intensity/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-26 13:25:52.990017 xsocs-2024.1.0/src/xsocs/gui/view/shift/
--rw-rw-rw-   0 root         (0) root         (0)    16556 2024-01-26 12:48:32.000000 xsocs-2024.1.0/src/xsocs/gui/view/shift/ShiftSubject.py
--rw-rw-rw-   0 root         (0) root         (0)    33144 2024-01-26 12:48:32.000000 xsocs-2024.1.0/src/xsocs/gui/view/shift/ShiftView.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-26 13:25:32.000000 xsocs-2024.1.0/src/xsocs/gui/view/shift/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-26 13:25:52.990017 xsocs-2024.1.0/src/xsocs/gui/widgets/
--rw-rw-rw-   0 root         (0) root         (0)     6723 2024-01-26 12:48:32.000000 xsocs-2024.1.0/src/xsocs/gui/widgets/AcqParamsWidget.py
--rw-rw-rw-   0 root         (0) root         (0)     1008 2024-01-26 12:48:32.000000 xsocs-2024.1.0/src/xsocs/gui/widgets/Buttons.py
--rw-rw-rw-   0 root         (0) root         (0)     1482 2024-01-26 12:48:32.000000 xsocs-2024.1.0/src/xsocs/gui/widgets/Containers.py
--rw-rw-rw-   0 root         (0) root         (0)     2485 2024-01-26 12:48:32.000000 xsocs-2024.1.0/src/xsocs/gui/widgets/FileChooser.py
--rw-rw-rw-   0 root         (0) root         (0)     3801 2024-01-26 12:48:32.000000 xsocs-2024.1.0/src/xsocs/gui/widgets/Input.py
--rw-rw-rw-   0 root         (0) root         (0)      820 2024-01-26 12:48:32.000000 xsocs-2024.1.0/src/xsocs/gui/widgets/PlotGrabber.py
--rw-rw-rw-   0 root         (0) root         (0)     1052 2024-01-26 12:48:32.000000 xsocs-2024.1.0/src/xsocs/gui/widgets/PointWidget.py
--rw-rw-rw-   0 root         (0) root         (0)     6984 2024-01-26 12:48:32.000000 xsocs-2024.1.0/src/xsocs/gui/widgets/ProjectChooser.py
--rw-rw-rw-   0 root         (0) root         (0)     3309 2024-01-26 12:48:32.000000 xsocs-2024.1.0/src/xsocs/gui/widgets/RoiAxisWidget.py
--rw-rw-rw-   0 root         (0) root         (0)     6819 2024-01-26 12:48:32.000000 xsocs-2024.1.0/src/xsocs/gui/widgets/ScatterPlot.py
--rw-rw-rw-   0 root         (0) root         (0)    10134 2024-01-26 12:48:32.000000 xsocs-2024.1.0/src/xsocs/gui/widgets/Wizard.py
--rw-rw-rw-   0 root         (0) root         (0)    38852 2024-01-26 12:48:32.000000 xsocs-2024.1.0/src/xsocs/gui/widgets/XsocsPlot2D.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-26 13:25:32.000000 xsocs-2024.1.0/src/xsocs/gui/widgets/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-26 13:25:52.994017 xsocs-2024.1.0/src/xsocs/io/
--rw-rw-rw-   0 root         (0) root         (0)    12366 2024-01-26 12:48:32.000000 xsocs-2024.1.0/src/xsocs/io/FitH5.py
--rw-rw-rw-   0 root         (0) root         (0)    19829 2024-01-26 12:48:32.000000 xsocs-2024.1.0/src/xsocs/io/QSpaceH5.py
--rw-rw-rw-   0 root         (0) root         (0)     5248 2024-01-26 12:48:32.000000 xsocs-2024.1.0/src/xsocs/io/ShiftH5.py
--rw-rw-rw-   0 root         (0) root         (0)    14238 2024-01-26 12:48:32.000000 xsocs-2024.1.0/src/xsocs/io/XsocsH5.py
--rw-rw-rw-   0 root         (0) root         (0)     8222 2024-01-26 12:48:32.000000 xsocs-2024.1.0/src/xsocs/io/XsocsH5Base.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-26 13:25:32.000000 xsocs-2024.1.0/src/xsocs/io/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      725 2024-01-26 12:48:32.000000 xsocs-2024.1.0/src/xsocs/io/_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     9893 2024-01-26 12:48:32.000000 xsocs-2024.1.0/src/xsocs/io/bliss.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-26 13:25:52.994017 xsocs-2024.1.0/src/xsocs/process/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-26 13:25:32.000000 xsocs-2024.1.0/src/xsocs/process/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-26 13:25:52.994017 xsocs-2024.1.0/src/xsocs/process/fit/
--rw-rw-rw-   0 root         (0) root         (0)      501 2024-01-26 12:48:32.000000 xsocs-2024.1.0/src/xsocs/process/fit/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    20366 2024-01-26 12:48:32.000000 xsocs-2024.1.0/src/xsocs/process/fit/peak_fit.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-26 13:25:52.994017 xsocs-2024.1.0/src/xsocs/process/merge/
--rw-rw-rw-   0 root         (0) root         (0)    26914 2024-01-26 12:48:32.000000 xsocs-2024.1.0/src/xsocs/process/merge/KmapMerger.py
--rw-rw-rw-   0 root         (0) root         (0)    10971 2024-01-26 12:48:32.000000 xsocs-2024.1.0/src/xsocs/process/merge/KmapSpecParser.py
--rw-rw-rw-   0 root         (0) root         (0)      288 2024-01-26 12:48:32.000000 xsocs-2024.1.0/src/xsocs/process/merge/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4216 2024-01-26 12:48:32.000000 xsocs-2024.1.0/src/xsocs/process/merge/helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-26 13:25:52.994017 xsocs-2024.1.0/src/xsocs/process/qspace/
--rw-rw-rw-   0 root         (0) root         (0)    58202 2024-01-26 12:48:32.000000 xsocs-2024.1.0/src/xsocs/process/qspace/QSpaceConverter.py
--rw-rw-rw-   0 root         (0) root         (0)      327 2024-01-26 12:48:32.000000 xsocs-2024.1.0/src/xsocs/process/qspace/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2559 2024-01-26 12:48:32.000000 xsocs-2024.1.0/src/xsocs/process/qspace/helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-26 13:25:52.994017 xsocs-2024.1.0/src/xsocs/process/shift/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-26 13:25:32.000000 xsocs-2024.1.0/src/xsocs/process/shift/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12922 2024-01-26 12:48:32.000000 xsocs-2024.1.0/src/xsocs/process/shift/shift.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-26 13:25:52.998017 xsocs-2024.1.0/src/xsocs/process/test/
--rw-rw-rw-   0 root         (0) root         (0)      479 2024-01-26 12:48:32.000000 xsocs-2024.1.0/src/xsocs/process/test/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5248 2024-01-26 12:48:32.000000 xsocs-2024.1.0/src/xsocs/process/test/test_fitter.py
--rw-rw-rw-   0 root         (0) root         (0)     4847 2024-01-26 12:48:32.000000 xsocs-2024.1.0/src/xsocs/process/test/test_merger.py
--rw-rw-rw-   0 root         (0) root         (0)     2309 2024-01-26 12:48:32.000000 xsocs-2024.1.0/src/xsocs/process/test/test_parser.py
--rw-rw-rw-   0 root         (0) root         (0)     5095 2024-01-26 12:48:32.000000 xsocs-2024.1.0/src/xsocs/process/test/test_qspace.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-26 13:25:52.998017 xsocs-2024.1.0/src/xsocs/resources/
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-01-26 12:48:32.000000 xsocs-2024.1.0/src/xsocs/resources/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-26 13:25:52.954017 xsocs-2024.1.0/src/xsocs/resources/gui/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-26 13:25:53.002017 xsocs-2024.1.0/src/xsocs/resources/gui/icons/
--rw-rw-rw-   0 root         (0) root         (0)     7819 2024-01-26 12:48:32.000000 xsocs-2024.1.0/src/xsocs/resources/gui/icons/bliss.png
--rw-rw-rw-   0 root         (0) root         (0)    14896 2024-01-26 12:48:32.000000 xsocs-2024.1.0/src/xsocs/resources/gui/icons/bliss.svg
--rw-rw-rw-   0 root         (0) root         (0)     1904 2024-01-26 12:48:32.000000 xsocs-2024.1.0/src/xsocs/resources/gui/icons/create_project.png
--rw-rw-rw-   0 root         (0) root         (0)     6666 2024-01-26 12:48:32.000000 xsocs-2024.1.0/src/xsocs/resources/gui/icons/create_project.svg
--rw-rw-rw-   0 root         (0) root         (0)    16556 2024-01-26 12:48:32.000000 xsocs-2024.1.0/src/xsocs/resources/gui/icons/gears.png
--rw-rw-rw-   0 root         (0) root         (0)     6931 2024-01-26 12:48:32.000000 xsocs-2024.1.0/src/xsocs/resources/gui/icons/gears.svg
--rw-rw-rw-   0 root         (0) root         (0)     4224 2024-01-26 12:48:32.000000 xsocs-2024.1.0/src/xsocs/resources/gui/icons/logo.png
--rw-rw-rw-   0 root         (0) root         (0)   182541 2024-01-26 12:48:32.000000 xsocs-2024.1.0/src/xsocs/resources/gui/icons/logo.svg
--rw-rw-rw-   0 root         (0) root         (0)     1478 2024-01-26 12:48:32.000000 xsocs-2024.1.0/src/xsocs/resources/gui/icons/save_2dscatter.png
--rw-rw-rw-   0 root         (0) root         (0)     3737 2024-01-26 12:48:32.000000 xsocs-2024.1.0/src/xsocs/resources/gui/icons/save_2dscatter.svg
--rw-rw-rw-   0 root         (0) root         (0)     1558 2024-01-26 12:48:32.000000 xsocs-2024.1.0/src/xsocs/resources/gui/icons/spec.png
--rw-rw-rw-   0 root         (0) root         (0)     2260 2024-01-26 12:48:32.000000 xsocs-2024.1.0/src/xsocs/resources/gui/icons/spec.svg
--rw-rw-rw-   0 root         (0) root         (0)     4661 2024-01-26 12:48:32.000000 xsocs-2024.1.0/src/xsocs/resources/gui/icons/xsocs.png
--rw-rw-rw-   0 root         (0) root         (0)     3252 2024-01-26 12:48:32.000000 xsocs-2024.1.0/src/xsocs/resources/gui/icons/xsocs.svg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-26 13:25:53.002017 xsocs-2024.1.0/src/xsocs/test/
--rw-rw-rw-   0 root         (0) root         (0)      684 2024-01-26 12:48:32.000000 xsocs-2024.1.0/src/xsocs/test/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      460 2024-01-26 12:48:32.000000 xsocs-2024.1.0/src/xsocs/test/test_version.py
--rw-rw-rw-   0 root         (0) root         (0)      261 2024-01-26 12:48:32.000000 xsocs-2024.1.0/src/xsocs/test/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-26 13:25:53.002017 xsocs-2024.1.0/src/xsocs/util/
--rw-rw-rw-   0 root         (0) root         (0)     2141 2024-01-26 12:48:32.000000 xsocs-2024.1.0/src/xsocs/util/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-26 13:25:53.002017 xsocs-2024.1.0/src/xsocs.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2917 2024-01-26 13:25:52.000000 xsocs-2024.1.0/src/xsocs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5085 2024-01-26 13:25:52.000000 xsocs-2024.1.0/src/xsocs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-01-26 13:25:52.000000 xsocs-2024.1.0/src/xsocs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       52 2024-01-26 13:25:52.000000 xsocs-2024.1.0/src/xsocs.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-01-26 13:25:52.000000 xsocs-2024.1.0/src/xsocs.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      193 2024-01-26 13:25:52.000000 xsocs-2024.1.0/src/xsocs.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2024-01-26 13:25:52.000000 xsocs-2024.1.0/src/xsocs.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 14:57:06.663433 xsocs-2024.4.0/
+-rw-rw-rw-   0 root         (0) root         (0)     5072 2024-04-03 14:28:08.000000 xsocs-2024.4.0/CHANGELOG.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1101 2024-04-03 13:23:19.000000 xsocs-2024.4.0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      112 2024-04-03 13:23:19.000000 xsocs-2024.4.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3606 2024-04-03 14:57:06.663433 xsocs-2024.4.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1800 2024-04-03 13:23:19.000000 xsocs-2024.4.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 14:57:06.635433 xsocs-2024.4.0/doc/
+-rw-rw-rw-   0 root         (0) root         (0)     7703 2024-04-03 13:23:19.000000 xsocs-2024.4.0/doc/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)     2979 2024-04-03 13:23:19.000000 xsocs-2024.4.0/doc/fileformat.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 14:57:06.635433 xsocs-2024.4.0/doc/img/
+-rw-rw-rw-   0 root         (0) root         (0)    99637 2024-04-03 13:23:19.000000 xsocs-2024.4.0/doc/img/input_file.png
+-rw-rw-rw-   0 root         (0) root         (0)     1032 2024-04-03 13:23:19.000000 xsocs-2024.4.0/doc/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2399 2024-04-03 13:23:19.000000 xsocs-2024.4.0/doc/install.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1313 2024-04-03 13:23:19.000000 xsocs-2024.4.0/doc/modules.rst
+-rw-rw-rw-   0 root         (0) root         (0)      614 2024-04-03 13:23:19.000000 xsocs-2024.4.0/doc/troubleshooting.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1204 2024-04-03 13:23:19.000000 xsocs-2024.4.0/doc/tutorials.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 14:57:06.639433 xsocs-2024.4.0/doc/usage/
+-rw-rw-rw-   0 root         (0) root         (0)     2340 2024-04-03 13:23:19.000000 xsocs-2024.4.0/doc/usage/conversion.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 14:57:06.647433 xsocs-2024.4.0/doc/usage/img/
+-rw-rw-rw-   0 root         (0) root         (0)   114617 2024-04-03 13:23:19.000000 xsocs-2024.4.0/doc/usage/img/com_results_view.png
+-rw-rw-rw-   0 root         (0) root         (0)    83045 2024-04-03 13:23:19.000000 xsocs-2024.4.0/doc/usage/img/conversion_dialog.png
+-rw-rw-rw-   0 root         (0) root         (0)      622 2024-04-03 13:23:19.000000 xsocs-2024.4.0/doc/usage/img/draw_roi_button.png
+-rw-rw-rw-   0 root         (0) root         (0)     1403 2024-04-03 13:23:19.000000 xsocs-2024.4.0/doc/usage/img/export_fit_button.png
+-rw-rw-rw-   0 root         (0) root         (0)     1113 2024-04-03 13:23:19.000000 xsocs-2024.4.0/doc/usage/img/fit_results_button.png
+-rw-rw-rw-   0 root         (0) root         (0)   156322 2024-04-03 13:23:19.000000 xsocs-2024.4.0/doc/usage/img/fit_results_view.png
+-rw-rw-rw-   0 root         (0) root         (0)     1113 2024-04-03 13:23:19.000000 xsocs-2024.4.0/doc/usage/img/intensity_plot_button.png
+-rw-rw-rw-   0 root         (0) root         (0)   136848 2024-04-03 13:23:19.000000 xsocs-2024.4.0/doc/usage/img/intensity_view.png
+-rw-rw-rw-   0 root         (0) root         (0)     7280 2024-04-03 13:23:19.000000 xsocs-2024.4.0/doc/usage/img/main_view.png
+-rw-rw-rw-   0 root         (0) root         (0)    41461 2024-04-03 13:23:19.000000 xsocs-2024.4.0/doc/usage/img/merge_window.png
+-rw-rw-rw-   0 root         (0) root         (0)    37829 2024-04-03 13:23:19.000000 xsocs-2024.4.0/doc/usage/img/open_dialog.png
+-rw-rw-rw-   0 root         (0) root         (0)      926 2024-04-03 13:23:19.000000 xsocs-2024.4.0/doc/usage/img/open_icon.png
+-rw-rw-rw-   0 root         (0) root         (0)    34780 2024-04-03 13:23:19.000000 xsocs-2024.4.0/doc/usage/img/project_tree.png
+-rw-rw-rw-   0 root         (0) root         (0)    86754 2024-04-03 13:23:19.000000 xsocs-2024.4.0/doc/usage/img/qspace_stack_view.png
+-rw-rw-rw-   0 root         (0) root         (0)     1053 2024-04-03 13:23:19.000000 xsocs-2024.4.0/doc/usage/img/qspace_view_button.png
+-rw-rw-rw-   0 root         (0) root         (0)   110038 2024-04-03 13:23:19.000000 xsocs-2024.4.0/doc/usage/img/qspace_window.png
+-rw-rw-rw-   0 root         (0) root         (0)   145447 2024-04-03 13:23:19.000000 xsocs-2024.4.0/doc/usage/img/shift_editor.png
+-rw-rw-rw-   0 root         (0) root         (0)     2876 2024-04-03 13:23:19.000000 xsocs-2024.4.0/doc/usage/img/to_qspace_button.png
+-rw-rw-rw-   0 root         (0) root         (0)     2898 2024-04-03 13:23:19.000000 xsocs-2024.4.0/doc/usage/intensity_view.rst
+-rw-rw-rw-   0 root         (0) root         (0)     6751 2024-04-03 13:23:19.000000 xsocs-2024.4.0/doc/usage/project.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2535 2024-04-03 13:23:19.000000 xsocs-2024.4.0/doc/usage/project_view.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3053 2024-04-03 13:23:19.000000 xsocs-2024.4.0/doc/usage/qspace_view.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1763 2024-04-03 13:23:19.000000 xsocs-2024.4.0/doc/usage/results_view.rst
+-rw-rw-rw-   0 root         (0) root         (0)      786 2024-04-03 13:23:19.000000 xsocs-2024.4.0/doc/usage/starting.rst
+-rw-rw-rw-   0 root         (0) root         (0)      977 2024-04-03 13:23:19.000000 xsocs-2024.4.0/doc/using.rst
+-rw-rw-rw-   0 root         (0) root         (0)      101 2024-04-03 13:23:19.000000 xsocs-2024.4.0/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     1643 2024-04-03 14:57:06.667434 xsocs-2024.4.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       70 2024-04-03 13:23:19.000000 xsocs-2024.4.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 14:57:06.631433 xsocs-2024.4.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 14:57:06.647433 xsocs-2024.4.0/src/xsocs/
+-rw-rw-rw-   0 root         (0) root         (0)      523 2024-04-03 13:23:19.000000 xsocs-2024.4.0/src/xsocs/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      847 2024-04-03 13:23:19.000000 xsocs-2024.4.0/src/xsocs/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 14:57:06.651433 xsocs-2024.4.0/src/xsocs/_app/
+-rw-rw-rw-   0 root         (0) root         (0)       33 2024-04-03 13:23:19.000000 xsocs-2024.4.0/src/xsocs/_app/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2633 2024-04-03 13:23:19.000000 xsocs-2024.4.0/src/xsocs/_app/concat.py
+-rw-rw-rw-   0 root         (0) root         (0)     1162 2024-04-03 13:23:19.000000 xsocs-2024.4.0/src/xsocs/_app/gui.py
+-rw-rw-rw-   0 root         (0) root         (0)      714 2024-04-03 13:23:19.000000 xsocs-2024.4.0/src/xsocs/_config.py
+-rw-rw-rw-   0 root         (0) root         (0)     2776 2024-04-03 14:28:08.000000 xsocs-2024.4.0/src/xsocs/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 14:57:06.651433 xsocs-2024.4.0/src/xsocs/examples/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-03 14:56:49.000000 xsocs-2024.4.0/src/xsocs/examples/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2600 2024-04-03 13:23:19.000000 xsocs-2024.4.0/src/xsocs/examples/id01_merge.py
+-rw-rw-rw-   0 root         (0) root         (0)     1985 2024-04-03 13:23:19.000000 xsocs-2024.4.0/src/xsocs/examples/id01_peak.py
+-rw-rw-rw-   0 root         (0) root         (0)     1681 2024-04-03 13:23:19.000000 xsocs-2024.4.0/src/xsocs/examples/id01_qspace.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 14:57:06.651433 xsocs-2024.4.0/src/xsocs/gui/
+-rw-rw-rw-   0 root         (0) root         (0)      335 2024-04-03 13:23:19.000000 xsocs-2024.4.0/src/xsocs/gui/Utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    11955 2024-04-03 13:23:19.000000 xsocs-2024.4.0/src/xsocs/gui/XsocsGui.py
+-rw-rw-rw-   0 root         (0) root         (0)      740 2024-04-03 13:23:19.000000 xsocs-2024.4.0/src/xsocs/gui/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      816 2024-04-03 13:23:19.000000 xsocs-2024.4.0/src/xsocs/gui/gui.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 14:57:06.651433 xsocs-2024.4.0/src/xsocs/gui/model/
+-rw-rw-rw-   0 root         (0) root         (0)     5309 2024-04-03 13:23:19.000000 xsocs-2024.4.0/src/xsocs/gui/model/Model.py
+-rw-rw-rw-   0 root         (0) root         (0)      360 2024-04-03 13:23:19.000000 xsocs-2024.4.0/src/xsocs/gui/model/ModelDef.py
+-rw-rw-rw-   0 root         (0) root         (0)    39319 2024-04-03 13:23:19.000000 xsocs-2024.4.0/src/xsocs/gui/model/Node.py
+-rw-rw-rw-   0 root         (0) root         (0)     1780 2024-04-03 13:23:19.000000 xsocs-2024.4.0/src/xsocs/gui/model/NodeEditor.py
+-rw-rw-rw-   0 root         (0) root         (0)     4576 2024-04-03 13:23:19.000000 xsocs-2024.4.0/src/xsocs/gui/model/Nodes.py
+-rw-rw-rw-   0 root         (0) root         (0)    13616 2024-04-03 13:23:19.000000 xsocs-2024.4.0/src/xsocs/gui/model/TreeView.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-03 14:56:49.000000 xsocs-2024.4.0/src/xsocs/gui/model/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 14:57:06.651433 xsocs-2024.4.0/src/xsocs/gui/process/
+-rw-rw-rw-   0 root         (0) root         (0)     8467 2024-04-03 13:23:19.000000 xsocs-2024.4.0/src/xsocs/gui/process/FitWidget.py
+-rw-rw-rw-   0 root         (0) root         (0)    43220 2024-04-03 13:23:19.000000 xsocs-2024.4.0/src/xsocs/gui/process/MergeWidget.py
+-rw-rw-rw-   0 root         (0) root         (0)    34942 2024-04-03 13:23:19.000000 xsocs-2024.4.0/src/xsocs/gui/process/QSpaceWidget.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-03 14:56:49.000000 xsocs-2024.4.0/src/xsocs/gui/process/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 14:57:06.651433 xsocs-2024.4.0/src/xsocs/gui/project/
+-rw-rw-rw-   0 root         (0) root         (0)      964 2024-04-03 13:23:19.000000 xsocs-2024.4.0/src/xsocs/gui/project/AcqDataGroup.py
+-rw-rw-rw-   0 root         (0) root         (0)     2299 2024-04-03 13:23:19.000000 xsocs-2024.4.0/src/xsocs/gui/project/FitGroup.py
+-rw-rw-rw-   0 root         (0) root         (0)     8312 2024-04-03 13:23:19.000000 xsocs-2024.4.0/src/xsocs/gui/project/Hdf5Nodes.py
+-rw-rw-rw-   0 root         (0) root         (0)     7846 2024-04-03 13:23:19.000000 xsocs-2024.4.0/src/xsocs/gui/project/IntensityGroup.py
+-rw-rw-rw-   0 root         (0) root         (0)      712 2024-04-03 13:23:19.000000 xsocs-2024.4.0/src/xsocs/gui/project/ProjectDef.py
+-rw-rw-rw-   0 root         (0) root         (0)     9047 2024-04-03 13:23:19.000000 xsocs-2024.4.0/src/xsocs/gui/project/ProjectItem.py
+-rw-rw-rw-   0 root         (0) root         (0)    22762 2024-04-03 13:23:19.000000 xsocs-2024.4.0/src/xsocs/gui/project/ProjectNodes.py
+-rw-rw-rw-   0 root         (0) root         (0)     3348 2024-04-03 13:23:19.000000 xsocs-2024.4.0/src/xsocs/gui/project/QSpaceGroup.py
+-rw-rw-rw-   0 root         (0) root         (0)     1984 2024-04-03 13:23:19.000000 xsocs-2024.4.0/src/xsocs/gui/project/ScanPositionsItem.py
+-rw-rw-rw-   0 root         (0) root         (0)     3309 2024-04-03 13:23:19.000000 xsocs-2024.4.0/src/xsocs/gui/project/ShiftGroup.py
+-rw-rw-rw-   0 root         (0) root         (0)      703 2024-04-03 13:23:19.000000 xsocs-2024.4.0/src/xsocs/gui/project/XsocsH5Factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     2956 2024-04-03 13:23:19.000000 xsocs-2024.4.0/src/xsocs/gui/project/XsocsProject.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-03 14:56:49.000000 xsocs-2024.4.0/src/xsocs/gui/project/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 14:57:06.655434 xsocs-2024.4.0/src/xsocs/gui/silx_imports/
+-rw-rw-rw-   0 root         (0) root         (0)    25629 2024-04-03 13:23:19.000000 xsocs-2024.4.0/src/xsocs/gui/silx_imports/ImageRois.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-03 14:56:49.000000 xsocs-2024.4.0/src/xsocs/gui/silx_imports/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 14:57:06.655434 xsocs-2024.4.0/src/xsocs/gui/view/
+-rw-rw-rw-   0 root         (0) root         (0)    11311 2024-04-03 13:23:19.000000 xsocs-2024.4.0/src/xsocs/gui/view/FitView.py
+-rw-rw-rw-   0 root         (0) root         (0)    28432 2024-04-03 13:23:19.000000 xsocs-2024.4.0/src/xsocs/gui/view/QspaceView.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-03 14:56:49.000000 xsocs-2024.4.0/src/xsocs/gui/view/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 14:57:06.655434 xsocs-2024.4.0/src/xsocs/gui/view/fitview/
+-rw-rw-rw-   0 root         (0) root         (0)     3085 2024-04-03 13:23:19.000000 xsocs-2024.4.0/src/xsocs/gui/view/fitview/DropPlotWidget.py
+-rw-rw-rw-   0 root         (0) root         (0)     7574 2024-04-03 13:23:19.000000 xsocs-2024.4.0/src/xsocs/gui/view/fitview/FitModel.py
+-rw-rw-rw-   0 root         (0) root         (0)     1949 2024-04-03 13:23:19.000000 xsocs-2024.4.0/src/xsocs/gui/view/fitview/Plotter.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-03 14:56:49.000000 xsocs-2024.4.0/src/xsocs/gui/view/fitview/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 14:57:06.655434 xsocs-2024.4.0/src/xsocs/gui/view/intensity/
+-rw-rw-rw-   0 root         (0) root         (0)    25463 2024-04-03 13:23:19.000000 xsocs-2024.4.0/src/xsocs/gui/view/intensity/IntensityView.py
+-rw-rw-rw-   0 root         (0) root         (0)     6050 2024-04-03 13:23:19.000000 xsocs-2024.4.0/src/xsocs/gui/view/intensity/RectRoiWidget.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-03 14:56:49.000000 xsocs-2024.4.0/src/xsocs/gui/view/intensity/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 14:57:06.655434 xsocs-2024.4.0/src/xsocs/gui/view/shift/
+-rw-rw-rw-   0 root         (0) root         (0)    16556 2024-04-03 13:23:19.000000 xsocs-2024.4.0/src/xsocs/gui/view/shift/ShiftSubject.py
+-rw-rw-rw-   0 root         (0) root         (0)    33144 2024-04-03 13:23:19.000000 xsocs-2024.4.0/src/xsocs/gui/view/shift/ShiftView.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-03 14:56:49.000000 xsocs-2024.4.0/src/xsocs/gui/view/shift/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 14:57:06.655434 xsocs-2024.4.0/src/xsocs/gui/widgets/
+-rw-rw-rw-   0 root         (0) root         (0)     6723 2024-04-03 13:23:19.000000 xsocs-2024.4.0/src/xsocs/gui/widgets/AcqParamsWidget.py
+-rw-rw-rw-   0 root         (0) root         (0)     1008 2024-04-03 13:23:19.000000 xsocs-2024.4.0/src/xsocs/gui/widgets/Buttons.py
+-rw-rw-rw-   0 root         (0) root         (0)     1482 2024-04-03 13:23:19.000000 xsocs-2024.4.0/src/xsocs/gui/widgets/Containers.py
+-rw-rw-rw-   0 root         (0) root         (0)     2485 2024-04-03 13:23:19.000000 xsocs-2024.4.0/src/xsocs/gui/widgets/FileChooser.py
+-rw-rw-rw-   0 root         (0) root         (0)     2394 2024-04-03 13:23:19.000000 xsocs-2024.4.0/src/xsocs/gui/widgets/Input.py
+-rw-rw-rw-   0 root         (0) root         (0)      820 2024-04-03 13:23:19.000000 xsocs-2024.4.0/src/xsocs/gui/widgets/PlotGrabber.py
+-rw-rw-rw-   0 root         (0) root         (0)     1052 2024-04-03 13:23:19.000000 xsocs-2024.4.0/src/xsocs/gui/widgets/PointWidget.py
+-rw-rw-rw-   0 root         (0) root         (0)     6984 2024-04-03 13:23:19.000000 xsocs-2024.4.0/src/xsocs/gui/widgets/ProjectChooser.py
+-rw-rw-rw-   0 root         (0) root         (0)     3309 2024-04-03 13:23:19.000000 xsocs-2024.4.0/src/xsocs/gui/widgets/RoiAxisWidget.py
+-rw-rw-rw-   0 root         (0) root         (0)     6819 2024-04-03 13:23:19.000000 xsocs-2024.4.0/src/xsocs/gui/widgets/ScatterPlot.py
+-rw-rw-rw-   0 root         (0) root         (0)    10134 2024-04-03 13:23:19.000000 xsocs-2024.4.0/src/xsocs/gui/widgets/Wizard.py
+-rw-rw-rw-   0 root         (0) root         (0)    38852 2024-04-03 13:23:19.000000 xsocs-2024.4.0/src/xsocs/gui/widgets/XsocsPlot2D.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-03 14:56:49.000000 xsocs-2024.4.0/src/xsocs/gui/widgets/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 14:57:06.659433 xsocs-2024.4.0/src/xsocs/io/
+-rw-rw-rw-   0 root         (0) root         (0)    12366 2024-04-03 13:23:19.000000 xsocs-2024.4.0/src/xsocs/io/FitH5.py
+-rw-rw-rw-   0 root         (0) root         (0)    19829 2024-04-03 13:23:19.000000 xsocs-2024.4.0/src/xsocs/io/QSpaceH5.py
+-rw-rw-rw-   0 root         (0) root         (0)     5248 2024-04-03 13:23:19.000000 xsocs-2024.4.0/src/xsocs/io/ShiftH5.py
+-rw-rw-rw-   0 root         (0) root         (0)    14238 2024-04-03 13:23:19.000000 xsocs-2024.4.0/src/xsocs/io/XsocsH5.py
+-rw-rw-rw-   0 root         (0) root         (0)     8222 2024-04-03 13:23:19.000000 xsocs-2024.4.0/src/xsocs/io/XsocsH5Base.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-03 14:56:49.000000 xsocs-2024.4.0/src/xsocs/io/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      725 2024-04-03 13:23:19.000000 xsocs-2024.4.0/src/xsocs/io/_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     9893 2024-04-03 13:23:19.000000 xsocs-2024.4.0/src/xsocs/io/bliss.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 14:57:06.659433 xsocs-2024.4.0/src/xsocs/process/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-03 14:56:49.000000 xsocs-2024.4.0/src/xsocs/process/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 14:57:06.659433 xsocs-2024.4.0/src/xsocs/process/fit/
+-rw-rw-rw-   0 root         (0) root         (0)      501 2024-04-03 13:23:19.000000 xsocs-2024.4.0/src/xsocs/process/fit/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    20612 2024-04-03 13:23:19.000000 xsocs-2024.4.0/src/xsocs/process/fit/peak_fit.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 14:57:06.659433 xsocs-2024.4.0/src/xsocs/process/merge/
+-rw-rw-rw-   0 root         (0) root         (0)    26914 2024-04-03 13:23:19.000000 xsocs-2024.4.0/src/xsocs/process/merge/KmapMerger.py
+-rw-rw-rw-   0 root         (0) root         (0)    10971 2024-04-03 13:23:19.000000 xsocs-2024.4.0/src/xsocs/process/merge/KmapSpecParser.py
+-rw-rw-rw-   0 root         (0) root         (0)      288 2024-04-03 13:23:19.000000 xsocs-2024.4.0/src/xsocs/process/merge/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4216 2024-04-03 13:23:19.000000 xsocs-2024.4.0/src/xsocs/process/merge/helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 14:57:06.659433 xsocs-2024.4.0/src/xsocs/process/qspace/
+-rw-rw-rw-   0 root         (0) root         (0)    58152 2024-04-03 13:23:19.000000 xsocs-2024.4.0/src/xsocs/process/qspace/QSpaceConverter.py
+-rw-rw-rw-   0 root         (0) root         (0)      327 2024-04-03 13:23:19.000000 xsocs-2024.4.0/src/xsocs/process/qspace/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2559 2024-04-03 13:23:19.000000 xsocs-2024.4.0/src/xsocs/process/qspace/helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 14:57:06.659433 xsocs-2024.4.0/src/xsocs/process/shift/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-03 14:56:49.000000 xsocs-2024.4.0/src/xsocs/process/shift/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12922 2024-04-03 13:23:19.000000 xsocs-2024.4.0/src/xsocs/process/shift/shift.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 14:57:06.659433 xsocs-2024.4.0/src/xsocs/process/test/
+-rw-rw-rw-   0 root         (0) root         (0)      479 2024-04-03 13:23:19.000000 xsocs-2024.4.0/src/xsocs/process/test/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5248 2024-04-03 13:23:19.000000 xsocs-2024.4.0/src/xsocs/process/test/test_fitter.py
+-rw-rw-rw-   0 root         (0) root         (0)     4847 2024-04-03 13:23:19.000000 xsocs-2024.4.0/src/xsocs/process/test/test_merger.py
+-rw-rw-rw-   0 root         (0) root         (0)     2309 2024-04-03 13:23:19.000000 xsocs-2024.4.0/src/xsocs/process/test/test_parser.py
+-rw-rw-rw-   0 root         (0) root         (0)     5095 2024-04-03 13:23:19.000000 xsocs-2024.4.0/src/xsocs/process/test/test_qspace.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 14:57:06.659433 xsocs-2024.4.0/src/xsocs/resources/
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-03 13:23:19.000000 xsocs-2024.4.0/src/xsocs/resources/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 14:57:06.635433 xsocs-2024.4.0/src/xsocs/resources/gui/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 14:57:06.663433 xsocs-2024.4.0/src/xsocs/resources/gui/icons/
+-rw-rw-rw-   0 root         (0) root         (0)     7819 2024-04-03 13:23:19.000000 xsocs-2024.4.0/src/xsocs/resources/gui/icons/bliss.png
+-rw-rw-rw-   0 root         (0) root         (0)    14896 2024-04-03 13:23:19.000000 xsocs-2024.4.0/src/xsocs/resources/gui/icons/bliss.svg
+-rw-rw-rw-   0 root         (0) root         (0)     1904 2024-04-03 13:23:19.000000 xsocs-2024.4.0/src/xsocs/resources/gui/icons/create_project.png
+-rw-rw-rw-   0 root         (0) root         (0)     6666 2024-04-03 13:23:19.000000 xsocs-2024.4.0/src/xsocs/resources/gui/icons/create_project.svg
+-rw-rw-rw-   0 root         (0) root         (0)    16556 2024-04-03 13:23:19.000000 xsocs-2024.4.0/src/xsocs/resources/gui/icons/gears.png
+-rw-rw-rw-   0 root         (0) root         (0)     6931 2024-04-03 13:23:19.000000 xsocs-2024.4.0/src/xsocs/resources/gui/icons/gears.svg
+-rw-rw-rw-   0 root         (0) root         (0)     4224 2024-04-03 13:23:19.000000 xsocs-2024.4.0/src/xsocs/resources/gui/icons/logo.png
+-rw-rw-rw-   0 root         (0) root         (0)   182541 2024-04-03 13:23:19.000000 xsocs-2024.4.0/src/xsocs/resources/gui/icons/logo.svg
+-rw-rw-rw-   0 root         (0) root         (0)     1478 2024-04-03 13:23:19.000000 xsocs-2024.4.0/src/xsocs/resources/gui/icons/save_2dscatter.png
+-rw-rw-rw-   0 root         (0) root         (0)     3737 2024-04-03 13:23:19.000000 xsocs-2024.4.0/src/xsocs/resources/gui/icons/save_2dscatter.svg
+-rw-rw-rw-   0 root         (0) root         (0)     1558 2024-04-03 13:23:19.000000 xsocs-2024.4.0/src/xsocs/resources/gui/icons/spec.png
+-rw-rw-rw-   0 root         (0) root         (0)     2260 2024-04-03 13:23:19.000000 xsocs-2024.4.0/src/xsocs/resources/gui/icons/spec.svg
+-rw-rw-rw-   0 root         (0) root         (0)     4661 2024-04-03 13:23:19.000000 xsocs-2024.4.0/src/xsocs/resources/gui/icons/xsocs.png
+-rw-rw-rw-   0 root         (0) root         (0)     3252 2024-04-03 13:23:19.000000 xsocs-2024.4.0/src/xsocs/resources/gui/icons/xsocs.svg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 14:57:06.663433 xsocs-2024.4.0/src/xsocs/test/
+-rw-rw-rw-   0 root         (0) root         (0)      684 2024-04-03 13:23:19.000000 xsocs-2024.4.0/src/xsocs/test/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      460 2024-04-03 13:23:19.000000 xsocs-2024.4.0/src/xsocs/test/test_version.py
+-rw-rw-rw-   0 root         (0) root         (0)      261 2024-04-03 13:23:19.000000 xsocs-2024.4.0/src/xsocs/test/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 14:57:06.663433 xsocs-2024.4.0/src/xsocs/util/
+-rw-rw-rw-   0 root         (0) root         (0)     2131 2024-04-03 13:23:19.000000 xsocs-2024.4.0/src/xsocs/util/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 14:57:06.663433 xsocs-2024.4.0/src/xsocs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3606 2024-04-03 14:57:06.000000 xsocs-2024.4.0/src/xsocs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5085 2024-04-03 14:57:06.000000 xsocs-2024.4.0/src/xsocs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-03 14:57:06.000000 xsocs-2024.4.0/src/xsocs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       52 2024-04-03 14:57:06.000000 xsocs-2024.4.0/src/xsocs.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-03 14:57:06.000000 xsocs-2024.4.0/src/xsocs.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      203 2024-04-03 14:57:06.000000 xsocs-2024.4.0/src/xsocs.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2024-04-03 14:57:06.000000 xsocs-2024.4.0/src/xsocs.egg-info/top_level.txt
```

### Comparing `xsocs-2024.1.0/CHANGELOG.rst` & `xsocs-2024.4.0/CHANGELOG.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,26 @@
 Change Log
 ==========
 
+v2024.4.0: 2024/04/03
+---------------------
+
+* Compatibility:
+
+  - Added support of `numpy v2` (MR: !161)
+
+* User interface:
+
+  - Updated line edit style to support dark theme (MR: !162)
+
+* Documentation:
+
+  - Added zenodo DOI and xsocs publication reference (MR: !160)
+  - Updated documentation (MR: !63)
+
 v2024.1.0: 2024/01/26
 ---------------------
 
 - Added support for SXDM command from both BLISS and SPEC-like syntax (MR: !156)
 - Fixed silx v2 support (MR: !157)
 - Fixed FitWidget display (MR: !157)
 - Fixed GUI issue with Python>=3.10 (MR: !154)
```

### Comparing `xsocs-2024.1.0/LICENSE` & `xsocs-2024.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xsocs-2024.1.0/PKG-INFO` & `xsocs-2024.4.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xsocs
-Version: 2024.1.0
+Version: 2024.4.0
 Summary: Xray Strain Orientation Calculation Software
 Home-page: https://gitlab.esrf.fr/kmap/xsocs
 Author: ESRF
 Author-email: silx@esrf.fr
 License: MIT
 Project-URL: Documentation, https://kmap.gitlab-pages.esrf.fr/xsocs/
 Classifier: Development Status :: 4 - Beta
@@ -28,14 +28,15 @@
 Requires-Dist: numpy
 Requires-Dist: h5py
 Requires-Dist: fabio
 Requires-Dist: silx>=1.0.0
 Requires-Dist: xrayutilities
 Requires-Dist: scipy
 Requires-Dist: setuptools
+Requires-Dist: packaging
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: build; extra == "dev"
 Requires-Dist: flake8; extra == "dev"
 Requires-Dist: nbsphinx; extra == "dev"
 Requires-Dist: pillow; extra == "dev"
 Requires-Dist: setuptools; extra == "dev"
@@ -84,7 +85,19 @@
 See `Using X-Socs documentation <http://kmap.gitlab-pages.esrf.fr/xsocs/using.html>`_ and
 the `video tutorials <http://kmap.gitlab-pages.esrf.fr/xsocs/tutorials.html>`_.
 
 License
 -------
 
 The source code of X-SOCS is licensed under the `MIT license <https://gitlab.esrf.fr/kmap/xsocs/blob/main/LICENSE>`_.
+
+References
+----------
+
+X-SOCS can be referred by its DOI on Zenodo: |zenodo DOI|
+
+.. |zenodo DOI| image:: https://zenodo.org/badge/DOI/10.5281/zenodo.10777448.svg
+  :target: https://doi.org/10.5281/zenodo.10777448
+
+Reference publication:
+
+Chahine, G. A., Richard, M.-I., Homs-Regojo, R. A., Tran-Caliste, T. N., Carbone, D., Jacques, V. L. R., Grifone, R., Boesecke, P., Katzer, J., Costina, I., Djazouli, H., Schroeder, T. & Schulli, T. U. *"Imaging of strain and lattice orientation by quick scanning X-ray microscopy combined with three-dimensional reciprocal space mapping."* `J. Appl. Cryst. (2014) 47, 762-769. <https://doi.org/10.1107/S1600576714004506>`_
```

### Comparing `xsocs-2024.1.0/doc/conf.py` & `xsocs-2024.4.0/doc/conf.py`

 * *Files identical despite different names*

### Comparing `xsocs-2024.1.0/doc/fileformat.rst` & `xsocs-2024.4.0/doc/fileformat.rst`

 * *Files identical despite different names*

### Comparing `xsocs-2024.1.0/doc/img/input_file.png` & `xsocs-2024.4.0/doc/img/input_file.png`

 * *Files identical despite different names*

### Comparing `xsocs-2024.1.0/doc/index.rst` & `xsocs-2024.4.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `xsocs-2024.1.0/doc/install.rst` & `xsocs-2024.4.0/doc/install.rst`

 * *Files identical despite different names*

### Comparing `xsocs-2024.1.0/doc/modules.rst` & `xsocs-2024.4.0/doc/modules.rst`

 * *Files identical despite different names*

### Comparing `xsocs-2024.1.0/doc/troubleshooting.rst` & `xsocs-2024.4.0/doc/troubleshooting.rst`

 * *Files identical despite different names*

### Comparing `xsocs-2024.1.0/doc/tutorials.rst` & `xsocs-2024.4.0/doc/tutorials.rst`

 * *Files identical despite different names*

### Comparing `xsocs-2024.1.0/doc/usage/conversion.rst` & `xsocs-2024.4.0/doc/usage/conversion.rst`

 * *Files identical despite different names*

### Comparing `xsocs-2024.1.0/doc/usage/img/com_results_view.png` & `xsocs-2024.4.0/doc/usage/img/com_results_view.png`

 * *Files identical despite different names*

### Comparing `xsocs-2024.1.0/doc/usage/img/conversion_dialog.png` & `xsocs-2024.4.0/doc/usage/img/conversion_dialog.png`

 * *Files identical despite different names*

### Comparing `xsocs-2024.1.0/doc/usage/img/draw_roi_button.png` & `xsocs-2024.4.0/doc/usage/img/draw_roi_button.png`

 * *Files identical despite different names*

### Comparing `xsocs-2024.1.0/doc/usage/img/export_fit_button.png` & `xsocs-2024.4.0/doc/usage/img/export_fit_button.png`

 * *Files identical despite different names*

### Comparing `xsocs-2024.1.0/doc/usage/img/fit_results_button.png` & `xsocs-2024.4.0/doc/usage/img/fit_results_button.png`

 * *Files identical despite different names*

### Comparing `xsocs-2024.1.0/doc/usage/img/fit_results_view.png` & `xsocs-2024.4.0/doc/usage/img/fit_results_view.png`

 * *Files identical despite different names*

### Comparing `xsocs-2024.1.0/doc/usage/img/intensity_plot_button.png` & `xsocs-2024.4.0/doc/usage/img/intensity_plot_button.png`

 * *Files identical despite different names*

### Comparing `xsocs-2024.1.0/doc/usage/img/intensity_view.png` & `xsocs-2024.4.0/doc/usage/img/intensity_view.png`

 * *Files identical despite different names*

### Comparing `xsocs-2024.1.0/doc/usage/img/main_view.png` & `xsocs-2024.4.0/doc/usage/img/main_view.png`

 * *Files identical despite different names*

### Comparing `xsocs-2024.1.0/doc/usage/img/merge_window.png` & `xsocs-2024.4.0/doc/usage/img/merge_window.png`

 * *Files identical despite different names*

### Comparing `xsocs-2024.1.0/doc/usage/img/open_dialog.png` & `xsocs-2024.4.0/doc/usage/img/open_dialog.png`

 * *Files identical despite different names*

### Comparing `xsocs-2024.1.0/doc/usage/img/open_icon.png` & `xsocs-2024.4.0/doc/usage/img/open_icon.png`

 * *Files identical despite different names*

### Comparing `xsocs-2024.1.0/doc/usage/img/project_tree.png` & `xsocs-2024.4.0/doc/usage/img/project_tree.png`

 * *Files identical despite different names*

### Comparing `xsocs-2024.1.0/doc/usage/img/qspace_stack_view.png` & `xsocs-2024.4.0/doc/usage/img/qspace_stack_view.png`

 * *Files identical despite different names*

### Comparing `xsocs-2024.1.0/doc/usage/img/qspace_view_button.png` & `xsocs-2024.4.0/doc/usage/img/qspace_view_button.png`

 * *Files identical despite different names*

### Comparing `xsocs-2024.1.0/doc/usage/img/qspace_window.png` & `xsocs-2024.4.0/doc/usage/img/qspace_window.png`

 * *Files identical despite different names*

### Comparing `xsocs-2024.1.0/doc/usage/img/shift_editor.png` & `xsocs-2024.4.0/doc/usage/img/shift_editor.png`

 * *Files identical despite different names*

### Comparing `xsocs-2024.1.0/doc/usage/img/to_qspace_button.png` & `xsocs-2024.4.0/doc/usage/img/to_qspace_button.png`

 * *Files identical despite different names*

### Comparing `xsocs-2024.1.0/doc/usage/intensity_view.rst` & `xsocs-2024.4.0/doc/usage/intensity_view.rst`

 * *Files identical despite different names*

### Comparing `xsocs-2024.1.0/doc/usage/project.rst` & `xsocs-2024.4.0/doc/usage/project.rst`

 * *Files identical despite different names*

### Comparing `xsocs-2024.1.0/doc/usage/project_view.rst` & `xsocs-2024.4.0/doc/usage/project_view.rst`

 * *Files identical despite different names*

### Comparing `xsocs-2024.1.0/doc/usage/qspace_view.rst` & `xsocs-2024.4.0/doc/usage/qspace_view.rst`

 * *Files identical despite different names*

### Comparing `xsocs-2024.1.0/doc/usage/results_view.rst` & `xsocs-2024.4.0/doc/usage/results_view.rst`

 * *Files identical despite different names*

### Comparing `xsocs-2024.1.0/doc/usage/starting.rst` & `xsocs-2024.4.0/doc/usage/starting.rst`

 * *Files identical despite different names*

### Comparing `xsocs-2024.1.0/setup.cfg` & `xsocs-2024.4.0/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 	numpy
 	h5py
 	fabio
 	silx>=1.0.0
 	xrayutilities
 	scipy
 	setuptools
+	packaging
 package_dir = 
 	=src
 packages = find:
 python_requires = >=3.7
 zip_safe = False
 
 [options.entry_points]
```

### Comparing `xsocs-2024.1.0/src/xsocs/__init__.py` & `xsocs-2024.4.0/src/xsocs/__init__.py`

 * *Files identical despite different names*

### Comparing `xsocs-2024.1.0/src/xsocs/__main__.py` & `xsocs-2024.4.0/src/xsocs/__main__.py`

 * *Files identical despite different names*

### Comparing `xsocs-2024.1.0/src/xsocs/_app/concat.py` & `xsocs-2024.4.0/src/xsocs/_app/concat.py`

 * *Files identical despite different names*

### Comparing `xsocs-2024.1.0/src/xsocs/_app/gui.py` & `xsocs-2024.4.0/src/xsocs/_app/gui.py`

 * *Files identical despite different names*

### Comparing `xsocs-2024.1.0/src/xsocs/_config.py` & `xsocs-2024.4.0/src/xsocs/_config.py`

 * *Files identical despite different names*

### Comparing `xsocs-2024.1.0/src/xsocs/_version.py` & `xsocs-2024.4.0/src/xsocs/_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 ]
 
 RELEASE_LEVEL_VALUE = {"dev": 0, "alpha": 10, "beta": 11, "candidate": 12, "final": 15}
 
 PRERELEASE_NORMALIZED_NAME = {"dev": "a", "alpha": "a", "beta": "b", "candidate": "rc"}
 
 MAJOR = 2024
-MINOR = 1
+MINOR = 4
 MICRO = 0
 RELEV = "final"  # <16
 SERIAL = 0  # <16
 
 
 _version_info = namedtuple(
     "version_info", ["major", "minor", "micro", "releaselevel", "serial"]
```

### Comparing `xsocs-2024.1.0/src/xsocs/examples/id01_merge.py` & `xsocs-2024.4.0/src/xsocs/examples/id01_merge.py`

 * *Files identical despite different names*

### Comparing `xsocs-2024.1.0/src/xsocs/examples/id01_peak.py` & `xsocs-2024.4.0/src/xsocs/examples/id01_peak.py`

 * *Files identical despite different names*

### Comparing `xsocs-2024.1.0/src/xsocs/examples/id01_qspace.py` & `xsocs-2024.4.0/src/xsocs/examples/id01_qspace.py`

 * *Files identical despite different names*

### Comparing `xsocs-2024.1.0/src/xsocs/gui/XsocsGui.py` & `xsocs-2024.4.0/src/xsocs/gui/XsocsGui.py`

 * *Files identical despite different names*

### Comparing `xsocs-2024.1.0/src/xsocs/gui/__init__.py` & `xsocs-2024.4.0/src/xsocs/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `xsocs-2024.1.0/src/xsocs/gui/gui.py` & `xsocs-2024.4.0/src/xsocs/gui/gui.py`

 * *Files identical despite different names*

### Comparing `xsocs-2024.1.0/src/xsocs/gui/model/Model.py` & `xsocs-2024.4.0/src/xsocs/gui/model/Model.py`

 * *Files identical despite different names*

### Comparing `xsocs-2024.1.0/src/xsocs/gui/model/Node.py` & `xsocs-2024.4.0/src/xsocs/gui/model/Node.py`

 * *Files identical despite different names*

### Comparing `xsocs-2024.1.0/src/xsocs/gui/model/NodeEditor.py` & `xsocs-2024.4.0/src/xsocs/gui/model/NodeEditor.py`

 * *Files identical despite different names*

### Comparing `xsocs-2024.1.0/src/xsocs/gui/model/Nodes.py` & `xsocs-2024.4.0/src/xsocs/gui/model/Nodes.py`

 * *Files identical despite different names*

### Comparing `xsocs-2024.1.0/src/xsocs/gui/model/TreeView.py` & `xsocs-2024.4.0/src/xsocs/gui/model/TreeView.py`

 * *Files identical despite different names*

### Comparing `xsocs-2024.1.0/src/xsocs/gui/process/FitWidget.py` & `xsocs-2024.4.0/src/xsocs/gui/process/FitWidget.py`

 * *Files identical despite different names*

### Comparing `xsocs-2024.1.0/src/xsocs/gui/process/MergeWidget.py` & `xsocs-2024.4.0/src/xsocs/gui/process/MergeWidget.py`

 * *Files identical despite different names*

### Comparing `xsocs-2024.1.0/src/xsocs/gui/process/QSpaceWidget.py` & `xsocs-2024.4.0/src/xsocs/gui/process/QSpaceWidget.py`

 * *Files identical despite different names*

### Comparing `xsocs-2024.1.0/src/xsocs/gui/project/AcqDataGroup.py` & `xsocs-2024.4.0/src/xsocs/gui/project/AcqDataGroup.py`

 * *Files identical despite different names*

### Comparing `xsocs-2024.1.0/src/xsocs/gui/project/FitGroup.py` & `xsocs-2024.4.0/src/xsocs/gui/project/FitGroup.py`

 * *Files identical despite different names*

### Comparing `xsocs-2024.1.0/src/xsocs/gui/project/Hdf5Nodes.py` & `xsocs-2024.4.0/src/xsocs/gui/project/Hdf5Nodes.py`

 * *Files identical despite different names*

### Comparing `xsocs-2024.1.0/src/xsocs/gui/project/IntensityGroup.py` & `xsocs-2024.4.0/src/xsocs/gui/project/IntensityGroup.py`

 * *Files identical despite different names*

### Comparing `xsocs-2024.1.0/src/xsocs/gui/project/ProjectDef.py` & `xsocs-2024.4.0/src/xsocs/gui/project/ProjectDef.py`

 * *Files identical despite different names*

### Comparing `xsocs-2024.1.0/src/xsocs/gui/project/ProjectItem.py` & `xsocs-2024.4.0/src/xsocs/gui/project/ProjectItem.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,15 +95,15 @@
     def __setXsocsAttributes(self, xsocsClass, processLevel):
         if self.mode not in ("r",):
             with self._get_file() as h5f:
                 item = h5f[self.path]
                 if self.XsocsClass is not None and "XsocsClass" not in item.attrs:
                     # for some reason there was an error when using
                     # attrs.get(), so I had to use "not in" instead
-                    item.attrs["XsocsClass"] = np.string_(xsocsClass)
+                    item.attrs["XsocsClass"] = np.bytes_(xsocsClass)
                 if processLevel is not None and item.attrs.get("XsocsLevel") is None:
                     item.attrs["XsocsLevel"] = processLevel
                 del item
 
     def parent(self, classinfo=None):
         """
         Returns this Project item's parent. Or None if this is the toplevel
@@ -222,15 +222,15 @@
 
     def setItemName(self, itemName):
         """
         Sets the item's custom name.
         :param itemName:
         :return:
         """
-        itemName = np.string_(
+        itemName = np.bytes_(
             "{{0:<{0}}}".format(ProjectItem.MaxNameLength).format(itemName)
         )
         with self._get_file():
             self._set_scalar_data(self.path + "/" + self.ItemNamePath, itemName)
 
     def getItemName(self):
         """
```

### Comparing `xsocs-2024.1.0/src/xsocs/gui/project/ProjectNodes.py` & `xsocs-2024.4.0/src/xsocs/gui/project/ProjectNodes.py`

 * *Files identical despite different names*

### Comparing `xsocs-2024.1.0/src/xsocs/gui/project/QSpaceGroup.py` & `xsocs-2024.4.0/src/xsocs/gui/project/QSpaceGroup.py`

 * *Files identical despite different names*

### Comparing `xsocs-2024.1.0/src/xsocs/gui/project/ScanPositionsItem.py` & `xsocs-2024.4.0/src/xsocs/gui/project/ScanPositionsItem.py`

 * *Files identical despite different names*

### Comparing `xsocs-2024.1.0/src/xsocs/gui/project/ShiftGroup.py` & `xsocs-2024.4.0/src/xsocs/gui/project/ShiftGroup.py`

 * *Files identical despite different names*

### Comparing `xsocs-2024.1.0/src/xsocs/gui/project/XsocsH5Factory.py` & `xsocs-2024.4.0/src/xsocs/gui/project/XsocsH5Factory.py`

 * *Files identical despite different names*

### Comparing `xsocs-2024.1.0/src/xsocs/gui/project/XsocsProject.py` & `xsocs-2024.4.0/src/xsocs/gui/project/XsocsProject.py`

 * *Files identical despite different names*

### Comparing `xsocs-2024.1.0/src/xsocs/gui/silx_imports/ImageRois.py` & `xsocs-2024.4.0/src/xsocs/gui/silx_imports/ImageRois.py`

 * *Files identical despite different names*

### Comparing `xsocs-2024.1.0/src/xsocs/gui/view/FitView.py` & `xsocs-2024.4.0/src/xsocs/gui/view/FitView.py`

 * *Files identical despite different names*

### Comparing `xsocs-2024.1.0/src/xsocs/gui/view/QspaceView.py` & `xsocs-2024.4.0/src/xsocs/gui/view/QspaceView.py`

 * *Files identical despite different names*

### Comparing `xsocs-2024.1.0/src/xsocs/gui/view/fitview/DropPlotWidget.py` & `xsocs-2024.4.0/src/xsocs/gui/view/fitview/DropPlotWidget.py`

 * *Files identical despite different names*

### Comparing `xsocs-2024.1.0/src/xsocs/gui/view/fitview/FitModel.py` & `xsocs-2024.4.0/src/xsocs/gui/view/fitview/FitModel.py`

 * *Files identical despite different names*

### Comparing `xsocs-2024.1.0/src/xsocs/gui/view/fitview/Plotter.py` & `xsocs-2024.4.0/src/xsocs/gui/view/fitview/Plotter.py`

 * *Files identical despite different names*

### Comparing `xsocs-2024.1.0/src/xsocs/gui/view/intensity/IntensityView.py` & `xsocs-2024.4.0/src/xsocs/gui/view/intensity/IntensityView.py`

 * *Files identical despite different names*

### Comparing `xsocs-2024.1.0/src/xsocs/gui/view/intensity/RectRoiWidget.py` & `xsocs-2024.4.0/src/xsocs/gui/view/intensity/RectRoiWidget.py`

 * *Files identical despite different names*

### Comparing `xsocs-2024.1.0/src/xsocs/gui/view/shift/ShiftSubject.py` & `xsocs-2024.4.0/src/xsocs/gui/view/shift/ShiftSubject.py`

 * *Files identical despite different names*

### Comparing `xsocs-2024.1.0/src/xsocs/gui/view/shift/ShiftView.py` & `xsocs-2024.4.0/src/xsocs/gui/view/shift/ShiftView.py`

 * *Files identical despite different names*

### Comparing `xsocs-2024.1.0/src/xsocs/gui/widgets/AcqParamsWidget.py` & `xsocs-2024.4.0/src/xsocs/gui/widgets/AcqParamsWidget.py`

 * *Files identical despite different names*

### Comparing `xsocs-2024.1.0/src/xsocs/gui/widgets/Buttons.py` & `xsocs-2024.4.0/src/xsocs/gui/widgets/Buttons.py`

 * *Files identical despite different names*

### Comparing `xsocs-2024.1.0/src/xsocs/gui/widgets/Containers.py` & `xsocs-2024.4.0/src/xsocs/gui/widgets/Containers.py`

 * *Files identical despite different names*

### Comparing `xsocs-2024.1.0/src/xsocs/gui/widgets/FileChooser.py` & `xsocs-2024.4.0/src/xsocs/gui/widgets/FileChooser.py`

 * *Files identical despite different names*

### Comparing `xsocs-2024.1.0/src/xsocs/gui/widgets/PlotGrabber.py` & `xsocs-2024.4.0/src/xsocs/gui/widgets/PlotGrabber.py`

 * *Files identical despite different names*

### Comparing `xsocs-2024.1.0/src/xsocs/gui/widgets/PointWidget.py` & `xsocs-2024.4.0/src/xsocs/gui/widgets/PointWidget.py`

 * *Files identical despite different names*

### Comparing `xsocs-2024.1.0/src/xsocs/gui/widgets/ProjectChooser.py` & `xsocs-2024.4.0/src/xsocs/gui/widgets/ProjectChooser.py`

 * *Files identical despite different names*

### Comparing `xsocs-2024.1.0/src/xsocs/gui/widgets/RoiAxisWidget.py` & `xsocs-2024.4.0/src/xsocs/gui/widgets/RoiAxisWidget.py`

 * *Files identical despite different names*

### Comparing `xsocs-2024.1.0/src/xsocs/gui/widgets/ScatterPlot.py` & `xsocs-2024.4.0/src/xsocs/gui/widgets/ScatterPlot.py`

 * *Files identical despite different names*

### Comparing `xsocs-2024.1.0/src/xsocs/gui/widgets/Wizard.py` & `xsocs-2024.4.0/src/xsocs/gui/widgets/Wizard.py`

 * *Files identical despite different names*

### Comparing `xsocs-2024.1.0/src/xsocs/gui/widgets/XsocsPlot2D.py` & `xsocs-2024.4.0/src/xsocs/gui/widgets/XsocsPlot2D.py`

 * *Files identical despite different names*

### Comparing `xsocs-2024.1.0/src/xsocs/io/FitH5.py` & `xsocs-2024.4.0/src/xsocs/io/FitH5.py`

 * *Files identical despite different names*

### Comparing `xsocs-2024.1.0/src/xsocs/io/QSpaceH5.py` & `xsocs-2024.4.0/src/xsocs/io/QSpaceH5.py`

 * *Files identical despite different names*

### Comparing `xsocs-2024.1.0/src/xsocs/io/ShiftH5.py` & `xsocs-2024.4.0/src/xsocs/io/ShiftH5.py`

 * *Files identical despite different names*

### Comparing `xsocs-2024.1.0/src/xsocs/io/XsocsH5.py` & `xsocs-2024.4.0/src/xsocs/io/XsocsH5.py`

 * *Files identical despite different names*

### Comparing `xsocs-2024.1.0/src/xsocs/io/XsocsH5Base.py` & `xsocs-2024.4.0/src/xsocs/io/XsocsH5Base.py`

 * *Files identical despite different names*

### Comparing `xsocs-2024.1.0/src/xsocs/io/_utils.py` & `xsocs-2024.4.0/src/xsocs/io/_utils.py`

 * *Files identical despite different names*

### Comparing `xsocs-2024.1.0/src/xsocs/io/bliss.py` & `xsocs-2024.4.0/src/xsocs/io/bliss.py`

 * *Files identical despite different names*

### Comparing `xsocs-2024.1.0/src/xsocs/process/fit/peak_fit.py` & `xsocs-2024.4.0/src/xsocs/process/fit/peak_fit.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 import logging
 import functools
 import multiprocessing
 
 import numpy
+from packaging.version import Version
 from scipy.optimize import leastsq
 
 from silx.math.fit import snip1d
 
 from ... import config
 from ...io import QSpaceH5
 from ...io.FitH5 import BackgroundTypes, FitH5, FitH5Writer
 from ...util import gaussian, project
 
 
 _logger = logging.getLogger(__name__)
 
 
+# To support np.array's copy argument behaviour change between numpy v1 and v2
+NP_OPTIONAL_COPY: bool = False if Version(numpy.version.version).major < 2 else None
+
+
 class FitTypes(object):
     """Kind of fit available"""
 
     GAUSSIAN = 0
     """1 gaussian fit"""
 
     CENTROID = 1
@@ -111,15 +116,17 @@
 
         :param int dimension: QSpace dimension from which to return result
         :param str parameter: Name of the result to return
         :param bool copy: True to return a copy, False to return internal data
         :return: A 1D array
         :rtype: numpy.ndarray
         """
-        return numpy.array(self._fit_results[dimension][parameter], copy=copy)
+        return numpy.array(
+            self._fit_results[dimension][parameter], copy=copy or NP_OPTIONAL_COPY
+        )
 
     _FIT_ENTRY_NAMES = {FitTypes.GAUSSIAN: "Gaussian", FitTypes.CENTROID: "Centroid"}
 
     _FIT_PROCESS_NAMES = {FitTypes.GAUSSIAN: "gauss_0", FitTypes.CENTROID: "centroid"}
 
     def to_fit_h5(self, fit_h5, mode="a"):
         """Write fit results to an HDF5 file
```

### Comparing `xsocs-2024.1.0/src/xsocs/process/merge/KmapMerger.py` & `xsocs-2024.4.0/src/xsocs/process/merge/KmapMerger.py`

 * *Files identical despite different names*

### Comparing `xsocs-2024.1.0/src/xsocs/process/merge/KmapSpecParser.py` & `xsocs-2024.4.0/src/xsocs/process/merge/KmapSpecParser.py`

 * *Files identical despite different names*

### Comparing `xsocs-2024.1.0/src/xsocs/process/merge/helpers.py` & `xsocs-2024.4.0/src/xsocs/process/merge/helpers.py`

 * *Files identical despite different names*

### Comparing `xsocs-2024.1.0/src/xsocs/process/qspace/QSpaceConverter.py` & `xsocs-2024.4.0/src/xsocs/process/qspace/QSpaceConverter.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,24 +56,24 @@
         Set the coordinate system of the returned array
     :return: Array Q vectors of shape:
         (nb images, image height, image width, coordinates).
         Coordinates are either (qx, qy, qz) or (pitch, roll, radial)
         depending on coordinates argument.
     :rtype: numpy.ndarray
     """
-    phi = np.array(phi, copy=False, dtype=np.float64)
-    eta = np.array(eta, copy=False, dtype=np.float64)
-    nu = np.array(nu, copy=False, dtype=np.float64)
-    delta = np.array(delta, copy=False, dtype=np.float64)
+    phi = np.asarray(phi, dtype=np.float64)
+    eta = np.asarray(eta, dtype=np.float64)
+    nu = np.asarray(nu, dtype=np.float64)
+    delta = np.asarray(delta, dtype=np.float64)
 
     n_images = len(eta)
 
     if isinstance(beam_energy, numbers.Real):  # Convert to array
         beam_energy = [beam_energy] * n_images
-    beam_energy = np.array(beam_energy, copy=False, dtype=np.float64)
+    beam_energy = np.asarray(beam_energy, dtype=np.float64)
 
     qconv = xu.experiment.QConversion(["y-", "z-"], ["z-", "y-"], [1, 0, 0])
 
     # convention for coordinate system:
     # x downstream
     # z upwards
     # y to the "outside"
```

### Comparing `xsocs-2024.1.0/src/xsocs/process/qspace/helpers.py` & `xsocs-2024.4.0/src/xsocs/process/qspace/helpers.py`

 * *Files identical despite different names*

### Comparing `xsocs-2024.1.0/src/xsocs/process/shift/shift.py` & `xsocs-2024.4.0/src/xsocs/process/shift/shift.py`

 * *Files identical despite different names*

### Comparing `xsocs-2024.1.0/src/xsocs/process/test/test_fitter.py` & `xsocs-2024.4.0/src/xsocs/process/test/test_fitter.py`

 * *Files identical despite different names*

### Comparing `xsocs-2024.1.0/src/xsocs/process/test/test_merger.py` & `xsocs-2024.4.0/src/xsocs/process/test/test_merger.py`

 * *Files identical despite different names*

### Comparing `xsocs-2024.1.0/src/xsocs/process/test/test_parser.py` & `xsocs-2024.4.0/src/xsocs/process/test/test_parser.py`

 * *Files identical despite different names*

### Comparing `xsocs-2024.1.0/src/xsocs/process/test/test_qspace.py` & `xsocs-2024.4.0/src/xsocs/process/test/test_qspace.py`

 * *Files identical despite different names*

### Comparing `xsocs-2024.1.0/src/xsocs/resources/gui/icons/bliss.png` & `xsocs-2024.4.0/src/xsocs/resources/gui/icons/bliss.png`

 * *Files identical despite different names*

### Comparing `xsocs-2024.1.0/src/xsocs/resources/gui/icons/bliss.svg` & `xsocs-2024.4.0/src/xsocs/resources/gui/icons/bliss.svg`

 * *Files identical despite different names*

### Comparing `xsocs-2024.1.0/src/xsocs/resources/gui/icons/create_project.png` & `xsocs-2024.4.0/src/xsocs/resources/gui/icons/create_project.png`

 * *Files identical despite different names*

### Comparing `xsocs-2024.1.0/src/xsocs/resources/gui/icons/create_project.svg` & `xsocs-2024.4.0/src/xsocs/resources/gui/icons/create_project.svg`

 * *Files identical despite different names*

### Comparing `xsocs-2024.1.0/src/xsocs/resources/gui/icons/gears.png` & `xsocs-2024.4.0/src/xsocs/resources/gui/icons/gears.png`

 * *Files identical despite different names*

### Comparing `xsocs-2024.1.0/src/xsocs/resources/gui/icons/gears.svg` & `xsocs-2024.4.0/src/xsocs/resources/gui/icons/gears.svg`

 * *Files identical despite different names*

### Comparing `xsocs-2024.1.0/src/xsocs/resources/gui/icons/logo.png` & `xsocs-2024.4.0/src/xsocs/resources/gui/icons/logo.png`

 * *Files identical despite different names*

### Comparing `xsocs-2024.1.0/src/xsocs/resources/gui/icons/logo.svg` & `xsocs-2024.4.0/src/xsocs/resources/gui/icons/logo.svg`

 * *Files identical despite different names*

### Comparing `xsocs-2024.1.0/src/xsocs/resources/gui/icons/save_2dscatter.png` & `xsocs-2024.4.0/src/xsocs/resources/gui/icons/save_2dscatter.png`

 * *Files identical despite different names*

### Comparing `xsocs-2024.1.0/src/xsocs/resources/gui/icons/save_2dscatter.svg` & `xsocs-2024.4.0/src/xsocs/resources/gui/icons/save_2dscatter.svg`

 * *Files identical despite different names*

### Comparing `xsocs-2024.1.0/src/xsocs/resources/gui/icons/spec.png` & `xsocs-2024.4.0/src/xsocs/resources/gui/icons/spec.png`

 * *Files identical despite different names*

### Comparing `xsocs-2024.1.0/src/xsocs/resources/gui/icons/spec.svg` & `xsocs-2024.4.0/src/xsocs/resources/gui/icons/spec.svg`

 * *Files identical despite different names*

### Comparing `xsocs-2024.1.0/src/xsocs/resources/gui/icons/xsocs.png` & `xsocs-2024.4.0/src/xsocs/resources/gui/icons/xsocs.png`

 * *Files identical despite different names*

### Comparing `xsocs-2024.1.0/src/xsocs/resources/gui/icons/xsocs.svg` & `xsocs-2024.4.0/src/xsocs/resources/gui/icons/xsocs.svg`

 * *Files identical despite different names*

### Comparing `xsocs-2024.1.0/src/xsocs/test/__init__.py` & `xsocs-2024.4.0/src/xsocs/test/__init__.py`

 * *Files identical despite different names*

### Comparing `xsocs-2024.1.0/src/xsocs/util/__init__.py` & `xsocs-2024.4.0/src/xsocs/util/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
     This assumes sorted bins of the same size.
 
     :param numpy.ndarray centers: 1D array of bin centers
     :return: Bin edges min, max, step
     :rtype: List[float]
     """
-    centers = numpy.array(centers, copy=False)
+    centers = numpy.asarray(centers)
     nbins = centers.shape[0] - 1
     min_, max_ = numpy.min(centers), numpy.max(centers)
     step = (max_ - min_) / nbins
     return min_ - step / 2.0, max_ + step / 2.0, step
 
 
 _SQRT_2_PI = numpy.sqrt(2 * numpy.pi)
```

### Comparing `xsocs-2024.1.0/src/xsocs.egg-info/PKG-INFO` & `xsocs-2024.4.0/src/xsocs.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xsocs
-Version: 2024.1.0
+Version: 2024.4.0
 Summary: Xray Strain Orientation Calculation Software
 Home-page: https://gitlab.esrf.fr/kmap/xsocs
 Author: ESRF
 Author-email: silx@esrf.fr
 License: MIT
 Project-URL: Documentation, https://kmap.gitlab-pages.esrf.fr/xsocs/
 Classifier: Development Status :: 4 - Beta
@@ -28,14 +28,15 @@
 Requires-Dist: numpy
 Requires-Dist: h5py
 Requires-Dist: fabio
 Requires-Dist: silx>=1.0.0
 Requires-Dist: xrayutilities
 Requires-Dist: scipy
 Requires-Dist: setuptools
+Requires-Dist: packaging
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: build; extra == "dev"
 Requires-Dist: flake8; extra == "dev"
 Requires-Dist: nbsphinx; extra == "dev"
 Requires-Dist: pillow; extra == "dev"
 Requires-Dist: setuptools; extra == "dev"
@@ -84,7 +85,19 @@
 See `Using X-Socs documentation <http://kmap.gitlab-pages.esrf.fr/xsocs/using.html>`_ and
 the `video tutorials <http://kmap.gitlab-pages.esrf.fr/xsocs/tutorials.html>`_.
 
 License
 -------
 
 The source code of X-SOCS is licensed under the `MIT license <https://gitlab.esrf.fr/kmap/xsocs/blob/main/LICENSE>`_.
+
+References
+----------
+
+X-SOCS can be referred by its DOI on Zenodo: |zenodo DOI|
+
+.. |zenodo DOI| image:: https://zenodo.org/badge/DOI/10.5281/zenodo.10777448.svg
+  :target: https://doi.org/10.5281/zenodo.10777448
+
+Reference publication:
+
+Chahine, G. A., Richard, M.-I., Homs-Regojo, R. A., Tran-Caliste, T. N., Carbone, D., Jacques, V. L. R., Grifone, R., Boesecke, P., Katzer, J., Costina, I., Djazouli, H., Schroeder, T. & Schulli, T. U. *"Imaging of strain and lattice orientation by quick scanning X-ray microscopy combined with three-dimensional reciprocal space mapping."* `J. Appl. Cryst. (2014) 47, 762-769. <https://doi.org/10.1107/S1600576714004506>`_
```

### Comparing `xsocs-2024.1.0/src/xsocs.egg-info/SOURCES.txt` & `xsocs-2024.4.0/src/xsocs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

